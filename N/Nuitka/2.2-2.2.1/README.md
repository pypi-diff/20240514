# Comparing `tmp/Nuitka-2.2.tar.gz` & `tmp/Nuitka-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-2.2.tar", last modified: Tue Apr 30 08:28:45 2024, max compression, from Unix
+gzip compressed data, was "Nuitka-2.2.1.tar", last modified: Sun May  5 17:47:43 2024, max compression, from Unix
```

## Comparing `Nuitka-2.2.tar` & `Nuitka-2.2.1.tar`

### file list

```diff
@@ -1,1840 +1,1840 @@
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      235 2024-04-30 08:27:49.000000 Nuitka-2.2/Changelog.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)   152288 2024-04-30 08:27:49.000000 Nuitka-2.2/Developer_Manual.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11348 2021-04-22 06:31:42.000000 Nuitka-2.2/LICENSE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1707 2024-01-26 12:30:51.000000 Nuitka-2.2/MANIFEST.in
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.130337 Nuitka-2.2/Nuitka.egg-info/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    82954 2024-04-30 08:28:44.000000 Nuitka-2.2/Nuitka.egg-info/PKG-INFO
--rw-r--r--   0 hayen     (1000) hayen     (2000)    78171 2024-04-30 08:28:44.000000 Nuitka-2.2/Nuitka.egg-info/SOURCES.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-04-30 08:28:44.000000 Nuitka-2.2/Nuitka.egg-info/dependency_links.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)      393 2024-04-30 08:28:44.000000 Nuitka-2.2/Nuitka.egg-info/entry_points.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-02-02 15:24:24.000000 Nuitka-2.2/Nuitka.egg-info/not-zip-safe
--rw-r--r--   0 hayen     (1000) hayen     (2000)        7 2024-04-30 08:28:44.000000 Nuitka-2.2/Nuitka.egg-info/top_level.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)    82954 2024-04-30 08:28:44.290337 Nuitka-2.2/PKG-INFO
--rw-r--r--   0 hayen     (1000) hayen     (2000)    80812 2024-03-04 14:35:43.000000 Nuitka-2.2/README.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.130337 Nuitka-2.2/bin/
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1166 2024-03-04 14:35:43.000000 Nuitka-2.2/bin/autoformat-nuitka-source
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1165 2024-03-04 14:35:43.000000 Nuitka-2.2/bin/check-nuitka-with-pylint
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1181 2024-03-04 14:35:43.000000 Nuitka-2.2/bin/compare_with_cpython
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3105 2024-03-04 14:35:43.000000 Nuitka-2.2/bin/compare_with_xml
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1194 2024-03-04 14:35:43.000000 Nuitka-2.2/bin/measure-construct-performance
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.2/bin/nuitka
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.2/bin/nuitka-run
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.130337 Nuitka-2.2/doc/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.140337 Nuitka-2.2/doc/Logo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1797 2024-03-04 14:35:43.000000 Nuitka-2.2/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1553 2024-03-04 14:35:43.000000 Nuitka-2.2/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1793 2024-03-04 14:35:43.000000 Nuitka-2.2/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.140337 Nuitka-2.2/doc/images/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7585 2021-04-22 06:31:42.000000 Nuitka-2.2/doc/images/Nuitka-Logo-Horizontal.png
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4452 2021-04-22 06:31:42.000000 Nuitka-2.2/doc/images/Nuitka-Logo-Symbol.png
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9828 2022-01-09 15:54:20.000000 Nuitka-2.2/doc/images/Nuitka-Logo-Vertical.png
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33696 2024-04-30 08:27:49.000000 Nuitka-2.2/doc/nuitka-run.1
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33720 2024-04-30 08:27:49.000000 Nuitka-2.2/doc/nuitka.1
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.140337 Nuitka-2.2/lib/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4640 2024-03-04 14:35:43.000000 Nuitka-2.2/lib/hints.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.140337 Nuitka-2.2/misc/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      924 2024-03-04 14:35:43.000000 Nuitka-2.2/misc/nuitka-run.bat
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1061 2024-03-04 14:35:43.000000 Nuitka-2.2/misc/nuitka.bat
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.140337 Nuitka-2.2/nuitka/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7560 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/Builtins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5787 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/BytecodeCaching.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3800 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/Bytecodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1855 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/CacheCleanup.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11181 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/Constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2479 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11098 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/HardImportRegistry.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    38106 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/MainControl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8616 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/ModuleRegistry.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    62366 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/OptionParsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    75259 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/Options.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5432 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/OutputDirectories.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15000 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/PostProcessing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6805 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/Progress.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9654 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/PythonFlavors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4093 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/PythonOperators.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14564 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/PythonVersions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8989 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/Serialization.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4703 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/SourceCodeReferences.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13335 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/Tracing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3512 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/TreeXML.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15470 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/Variables.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2464 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/Version.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6373 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/__main__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5604 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/__past__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.140337 Nuitka-2.2/nuitka/build/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36409 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/Backend.scons
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8583 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/CCompilerVersion.scons
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3486 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/DataComposerInterface.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17749 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/Onefile.scons
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15361 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/SconsCaching.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35806 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/SconsCompilerSettings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5591 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/SconsHacks.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17868 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/SconsInterface.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2703 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/SconsProgress.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13210 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/SconsSpawn.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27035 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/SconsUtils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/include/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.150337 Nuitka-2.2/nuitka/build/include/nuitka/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8216 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/allocator.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3499 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/builtins.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5196 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/calling.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/checkers.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/checksum_tools.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9333 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2460 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/compiled_cell.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9233 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17661 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/compiled_frame.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7267 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/compiled_function.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9189 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/compiled_generator.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1866 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/compiled_method.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7688 2024-04-19 13:34:22.000000 Nuitka-2.2/nuitka/build/include/nuitka/constants.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1345 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/constants_blob.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1187 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/environment_variables.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1872 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/environment_variables_system.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5302 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/exception_groups.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50867 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/exceptions.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3792 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/filesystem_paths.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6474 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/freelists.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    86326 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/include/nuitka/hedley.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/include/nuitka/helper/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3698 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/attributes.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2692 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/boolean.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1233 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1164 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/bytes.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11894 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10644 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13168 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1834 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/complex.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13606 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1235 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/floats.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4401 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/import_hard.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1827 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/indexes.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3625 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/ints.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9599 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/iterators.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3678 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/lists.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1386 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/mappings.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4671 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12714 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5451 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5489 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2828 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15807 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13239 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5820 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4743 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5853 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5467 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20173 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8699 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3782 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4875 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2756 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10655 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9230 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5176 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4378 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5004 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4855 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4072 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/raising.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2367 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1175 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1141 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/sequences.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1054 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/sets.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8750 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/slices.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1363 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/strings.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17975 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/subscripts.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5926 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/helper/tuples.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16773 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/helpers.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6050 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/importing.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12979 2022-10-08 15:33:22.000000 Nuitka-2.2/nuitka/build/include/nuitka/incbin.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1086 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/jit_sources.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16556 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/prelude.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3237 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/printing.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1811 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/python_pgo.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2343 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/safe_string_ops.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3729 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/threading.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3447 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/tracing.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1145 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/include/nuitka/type_aliases.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3135 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/include/nuitka/unfreezing.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/appdirs/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1097 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24824 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/atomicwrites/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1069 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/bin/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1695 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/bin/scons.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/clcache/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/clcache/clcache/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-r--r--   0 hayen     (1000) hayen     (2000)       93 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    65424 2023-03-17 17:23:10.000000 Nuitka-2.2/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/colorama/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1491 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      243 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2522 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10517 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1915 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5404 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6438 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/glob2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1359 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/glob2/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)       82 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6859 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4463 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8304 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/jinja2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)       85 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/README.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2423 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17473 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1466 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-r--r--   0 hayen     (1000) hayen     (2000)       84 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17474 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/lib/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    47844 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33996 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8083 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27693 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6938 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17622 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    96183 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7358 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21540 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16000 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9589 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4197 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   121420 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4164 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    49503 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1965 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2736 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2614 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8467 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9314 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3131 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1989 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2483 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1718 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1605 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2170 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4179 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1882 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15042 2024-01-26 12:30:51.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39700 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12950 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4810 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3751 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3233 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2011 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14663 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.170337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14029 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    52665 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    40719 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24133 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14053 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2305 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34903 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    40510 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2166 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2859 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18084 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2078 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2004 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9248 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2784 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14869 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19499 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20832 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5149 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2290 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2657 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31283 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2379 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2267 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2720 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2796 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2147 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2936 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2935 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3785 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2777 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1711 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      142 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    29618 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3428 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1844 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4782 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2025 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2256 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2460 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2639 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1810 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2333 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2140 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1902 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2077 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2043 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18600 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25816 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3328 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8394 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2309 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2945 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6919 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4381 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4658 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4224 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13881 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1804 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11380 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    72761 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6841 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3579 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4375 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2827 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2513 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1991 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1819 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2502 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4695 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1927 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2473 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5992 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1831 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3730 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13016 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3415 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    48938 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3007 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3784 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4380 2024-01-26 12:30:51.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3557 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5612 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11034 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6824 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8120 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3596 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1818 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1742 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2465 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19253 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    44500 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19664 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7509 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53545 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34985 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13596 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28403 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7533 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20988 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    96818 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7752 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22350 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16068 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9565 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5239 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   135413 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5758 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    63474 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8354 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11500 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3180 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2227 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2739 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1767 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1654 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1460 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2219 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4476 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4003 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17055 2024-01-26 12:30:51.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41186 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13880 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4853 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3812 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15053 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.180338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13779 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53260 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39394 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26467 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14489 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35863 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42204 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2211 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18207 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2152 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2057 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10674 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2855 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15165 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    33537 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21762 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4464 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50660 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1667 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2316 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2840 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8618 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2226 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2978 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2977 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1653 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3827 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3389 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      313 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3631 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3444 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8494 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1753 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    29765 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1630 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1977 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3686 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2580 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2655 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1645 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2765 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2189 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1944 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2085 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15791 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26195 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13924 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4041 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2351 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2987 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7808 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4956 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5235 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4808 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14751 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1847 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12588 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    82939 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6883 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3663 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2660 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4904 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2877 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2567 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1652 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1868 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2088 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2176 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2366 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1658 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1976 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5335 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2583 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2515 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6756 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3773 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13982 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3201 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53803 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3064 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3818 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4435 2024-01-26 12:30:51.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5579 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11655 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6504 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1647 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6869 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1784 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19816 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9002 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2149 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    56578 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35213 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11061 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    27408 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21423 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    97269 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3979 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7515 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21937 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16583 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9430 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5126 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   136271 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6167 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    63768 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8183 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12836 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3087 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2630 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1674 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1311 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2076 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4356 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1805 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3860 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14831 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41983 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14673 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7394 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4357 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3546 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1972 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15577 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13597 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53509 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42760 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26676 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14272 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36753 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41191 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2122 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15570 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2014 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1943 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13182 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2734 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15027 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    38783 2023-03-17 17:23:10.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22570 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4368 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32724 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1578 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2228 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7993 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2141 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2893 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2889 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1567 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3742 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3296 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      343 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3534 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3259 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7461 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1663 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3379 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1891 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3616 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2377 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2437 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2526 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1557 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1772 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2677 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2206 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2096 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1851 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1954 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1995 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19180 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25826 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2588 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4649 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7652 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6064 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3931 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2266 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2900 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8622 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4577 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4517 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4113 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2387 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14473 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1752 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12902 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    84784 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6788 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3576 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4817 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2788 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2479 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1780 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1999 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2271 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1888 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4879 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2419 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2429 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6412 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1786 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12548 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4076 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    71693 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6632 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15278 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3134 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3896 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4648 2024-01-26 12:30:51.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3536 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5588 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12708 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6785 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      353 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4307 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1644 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3395 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21614 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9295 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2032 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/markupsafe/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10126 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      558 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4690 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/pkg_resources/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.190338 Nuitka-2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-r--r--   0 hayen     (1000) hayen     (2000)   107335 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      538 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/nuitka/build/inline_copy/tqdm/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1595 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      307 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      888 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      596 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1106 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      857 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1376 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10790 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    57572 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6948 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9726 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)       99 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13170 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4883 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28639 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3851 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2837 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    43006 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2061 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14184 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8999 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51277 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9776 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4921 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25145 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3290 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2719 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    43298 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2559 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1132 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25542 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6746 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17711 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9122 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    52446 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4171 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9607 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4881 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25554 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3294 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2723 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42954 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1138 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6854 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14097 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8970 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51695 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/zlib/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/zlib/LICENSE
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31605 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/zlib/crc32.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   591749 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/zlib/crc32.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16682 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/zlib/zconf.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    96778 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/zlib/zlib.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7247 2023-11-22 13:25:43.000000 Nuitka-2.2/nuitka/build/inline_copy/zlib/zutil.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.200338 Nuitka-2.2/nuitka/build/inline_copy/zstd/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1530 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.210337 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18198 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10157 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4455 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/debug.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13662 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3009 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2441 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34422 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/fse.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14748 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20216 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/huf.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13930 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/mem.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26976 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11706 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2728 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2497 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3828 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15880 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.210337 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    54982 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9164 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1321 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)    80283 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    66784 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2253 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7906 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-r--r--   0 hayen     (1000) hayen     (2000)   138334 2021-04-22 06:31:42.000000 Nuitka-2.2/nuitka/build/inline_copy/zstd/zstd.h
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.240337 Nuitka-2.2/nuitka/build/static_src/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    83526 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9142 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/CompiledCellType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    58843 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    72002 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledCoroutineType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    40762 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledFrameType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   110213 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledFunctionType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    67496 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledGeneratorType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    56411 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22466 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/CompiledMethodType.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19054 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersAllocator.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    37583 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersAttributes.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23690 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersBuiltin.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   114017 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3062 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersBytes.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13376 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersCalling.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   481627 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2065 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersChecksumTools.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3051 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersClasses.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   318889 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersComparisonEq.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4762 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   314072 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersComparisonGe.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   313483 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersComparisonGt.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   317286 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersComparisonLe.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   316697 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersComparisonLt.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   315637 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersComparisonNe.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36776 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20243 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersDeepcopy.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39785 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersDictionaries.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26620 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2066 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersDumpBacktraces.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2194 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersEnvironmentVariables.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2979 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7924 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersExceptions.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8349 2024-04-19 13:34:22.000000 Nuitka-2.2/nuitka/build/static_src/HelpersFiles.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28776 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2455 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersFloats.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1803 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersHeapStorage.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16080 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersImport.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16843 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersImportHard.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1815 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersJitSources.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21107 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersLists.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13944 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersListsGenerated.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1669 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersMappings.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3587 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersMatching.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   182227 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19904 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77811 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    68218 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1265 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    69479 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6300 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    83954 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13805 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   183867 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   188543 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3593 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    67184 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    79484 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1052 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77854 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    70851 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    68736 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   151107 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4242 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53151 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    77119 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    47857 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17771 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   136385 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)   142240 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    74749 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    83262 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    45341 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    83275 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    76950 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3294 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersProfiling.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersPythonPgo.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18257 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersRaising.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3868 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersSafeStrings.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3759 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersSequences.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1975 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersSlices.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32297 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersStrings.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4181 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/HelpersTuples.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6786 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/HelpersTypes.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12136 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/InspectPatcher.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    54011 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/MainProgram.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    63771 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4827 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6651 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21896 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31904 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/build/static_src/OnefileBootstrap.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8050 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/code_generation/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6491 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/AsyncgenCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10821 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/AttributeCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21926 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2371 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/BranchCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17006 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/BuiltinCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36111 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/CallCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4958 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/ClassCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    53293 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/CodeGeneration.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2408 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/CodeHelperSelection.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14320 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/CodeHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5147 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/CodeObjectCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17957 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/ComparisonCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4479 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7368 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/ConditionalCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6901 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/ConstantCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34299 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/Contexts.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8589 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/CoroutineCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1607 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/CtypesCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28934 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/DictCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2159 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/Emission.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9289 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/ErrorCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12983 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/EvalCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9011 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/ExceptionCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7384 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2126 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/ExpressionCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17852 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/FrameCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28336 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/FunctionCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7836 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/GeneratorCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6363 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/GlobalConstants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6985 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1870 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/IdCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14727 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/ImportCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1429 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/Indentation.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1574 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/IndexCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1066 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/InjectCCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3567 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/IntegerCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12211 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/IteratorCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1620 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/JitCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2055 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/LabelCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2645 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/LineNumberCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15849 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/ListCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6658 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/LoaderCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10016 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/LocalsDictCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3174 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/LoopCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1637 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/MatchCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6525 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/ModuleCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8224 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/Namify.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1860 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/NetworkxCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12733 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/OperationCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30198 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/PackageResourceCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3054 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/PrintCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/PythonAPICodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13251 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/RaisingCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3476 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/Reports.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5267 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/ReturnCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6591 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/SetCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14005 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/SliceCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10087 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/StringCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8302 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/SubscriptCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1939 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/TensorflowCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11208 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/TryCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/TupleCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2362 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/TypeAliasCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14811 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/VariableCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9155 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/VariableDeclarations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8129 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/YieldCodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/code_generation/c_types/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6102 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeBases.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1837 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1410 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3642 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5161 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5243 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3988 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19696 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2886 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/c_types/CTypeVoids.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/c_types/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/code_generation/templates/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9455 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2439 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6483 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3460 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3390 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2408 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4534 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22993 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6840 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2507 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/code_generation/templates_c/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11318 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5829 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23986 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5438 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1755 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1693 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2706 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13624 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1894 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1394 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7047 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12700 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1968 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4081 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7257 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4142 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3710 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4447 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11758 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19167 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2693 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3485 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11336 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15540 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2829 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10395 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2407 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2870 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2834 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3128 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/containers/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/containers/Namedtuples.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6553 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/containers/OrderedDicts.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      554 2022-10-08 09:07:15.000000 Nuitka-2.2/nuitka/containers/OrderedSets.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4430 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/containers/OrderedSetsFallback.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/containers/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/distutils/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2308 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/distutils/Build.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15025 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/distutils/DistutilCommands.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/distutils/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/finalizations/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1258 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/finalizations/Finalization.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6058 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/finalizations/FinalizeMarkups.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/finalizations/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/freezer/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7778 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/freezer/DependsExe.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/freezer/DllDependenciesCommon.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12816 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/freezer/DllDependenciesMacOS.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7468 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/freezer/DllDependenciesPosix.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6633 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/freezer/DllDependenciesWin32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11979 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/freezer/ImportDetection.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19236 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/freezer/IncludedDataFiles.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11455 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/freezer/IncludedEntryPoints.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9551 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/freezer/Onefile.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12245 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/freezer/Standalone.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/freezer/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.250337 Nuitka-2.2/nuitka/importing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11040 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/importing/IgnoreListing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2956 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/importing/ImportCache.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7784 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/importing/ImportResolving.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32895 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/importing/Importing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4869 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/importing/PreloadedPackages.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18804 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/importing/Recursion.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12787 2024-04-06 13:33:42.000000 Nuitka-2.2/nuitka/importing/StandardLibrary.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/importing/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/nodes/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3670 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/AsyncgenNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4115 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/AttributeLookupNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13255 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/AttributeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   379568 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/AttributeNodesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinAllNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4131 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinAnyNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2530 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/BuiltinComplexNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1731 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinDecodingNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2760 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4727 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinDictNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4982 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/BuiltinFormatNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2275 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinHashNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1457 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinInputNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5367 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinIntegerNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12812 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/BuiltinIteratorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2029 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinLenNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3639 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinNextNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3787 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinOpenNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   246360 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18648 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinRangeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9099 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/BuiltinRefNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3353 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinSumNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13576 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BuiltinTypeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1605 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/BuiltinVarsNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26146 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/BytesNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6511 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/CallNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1583 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/Checkers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   647748 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/ChildrenHavingMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8480 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ClassNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6622 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/CodeObjectSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21716 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ComparisonNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30300 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ConditionalNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    47737 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/ConstantRefNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12246 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ContainerMakingNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2867 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ContainerOperationNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4614 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/CoroutineNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1746 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/CtypesNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51053 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/DictionaryNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7889 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ExceptionNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7408 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ExecEvalNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    45046 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/ExpressionBases.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    55956 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/ExpressionBasesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ExpressionShapeMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12024 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/FrameNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3577 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/FunctionAttributeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    41167 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/FunctionNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5409 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/FutureSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6288 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/GeneratorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6961 2024-04-06 13:33:42.000000 Nuitka-2.2/nuitka/nodes/GlobalsLocalsNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    98222 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/HardImportNodesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5631 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/ImportHardNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    47892 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/ImportNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2766 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/IndicatorMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1533 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/InjectCNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11519 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/IterationHandles.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11035 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/KeyValuePairNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16821 2024-03-11 17:07:05.000000 Nuitka-2.2/nuitka/nodes/ListOperationNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23177 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/LocalsDictNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15007 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/LocalsScopes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15995 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/LoopNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1745 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/MatchNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6567 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ModuleAttributeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32830 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/ModuleNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1759 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/NetworkxNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24461 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/NodeBases.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15147 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/NodeMakingHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5580 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/NodeMetaClasses.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31948 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/OperatorNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8976 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/OperatorNodesUnary.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5228 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/OsSysNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12468 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/OutlineNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    34735 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/PackageMetadataNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12289 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/PackageResourceNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3440 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/PrintNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6805 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/ReturnNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4748 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/SideEffectNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12547 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/SliceNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    98808 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/StatementBasesGenerated.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9336 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/StatementNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28691 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/StrNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3538 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/StringConcatenationNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8329 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/SubscriptNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1411 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/TensorflowNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17886 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/TryNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2438 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/TypeMatchNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11717 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/TypeNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42396 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/VariableAssignNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10779 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/VariableDelNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4607 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/VariableNameNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    31274 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/VariableRefNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4781 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/VariableReleaseNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3937 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/YieldNodes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/nodes/shapes/
--rw-r--r--   0 hayen     (1000) hayen     (2000)   157357 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4420 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5076 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/shapes/ShapeMixins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42509 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/shapes/StandardShapes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/nodes/shapes/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/optimizations/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3358 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/optimizations/BytecodeDemotion.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/optimizations/FunctionInlining.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2177 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/optimizations/Graphs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10917 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/optimizations/Optimization.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    52575 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2287 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/optimizations/Tags.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42800 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/optimizations/TraceCollections.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    25799 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/optimizations/ValueTraces.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/optimizations/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/pgo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4932 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/pgo/PGO.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/pgo/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/plugins/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    57735 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/PluginBase.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    60566 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/plugins/standard/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30813 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3509 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10627 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/DataFilesPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5080 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/DelvewheelPlugin.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/plugins/standard/DillPlugin/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1646 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/DillPlugin/DillPlugin.c
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9826 2024-03-22 08:13:25.000000 Nuitka-2.2/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2679 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/DillPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16319 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/DllFilesPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2095 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/EnumPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/EventletPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1913 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/GeventPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4018 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/GiPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4854 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/GlfwPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    32325 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/ImplicitImports.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5024 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/KivyPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8824 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7080 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1220 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/NumpyPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7299 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1940 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/PbrPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4874 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7216 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/PmwPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51908 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3020 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/PywebViewPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1194 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/TensorflowPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13878 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/TkinterPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1174 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/TorchPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12838 2024-04-06 13:33:42.000000 Nuitka-2.2/nuitka/plugins/standard/TransformersPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1107 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/TrioPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5668 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/UpxPlugin.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/plugins/standard/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)   235710 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-01-26 12:30:51.000000 Nuitka-2.2/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12392 2024-01-26 12:30:51.000000 Nuitka-2.2/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/reports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2286 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/reports/CompilationReportReader.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2089 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/reports/LicenseReport.rst.j2
--rw-r--r--   0 hayen     (1000) hayen     (2000)    28892 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/reports/Reports.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/reports/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/specs/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5943 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2818 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/specs/BuiltinListOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    26799 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/specs/BuiltinParameterSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6098 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1190 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4834 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7112 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/specs/HardImportSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    18811 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/specs/ParameterSpecs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/specs/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.260337 Nuitka-2.2/nuitka/tools/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1631 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/Basics.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/commercial/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      847 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/commercial/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/data_composer/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15004 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/data_composer/DataComposer.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/data_composer/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1338 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/data_composer/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/environments/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2481 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/environments/CreateEnvironment.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4198 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/environments/Virtualenv.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/environments/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/general/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/general/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/general/dll_report/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/general/dll_report/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/general/dll_report/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/general/find_module/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/general/find_module/FindModuleCode.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/general/find_module/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/onefile_compressor/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12545 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/onefile_compressor/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1343 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/onefile_compressor/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/podman/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1905 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/podman/Podman.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/podman/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11623 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/podman/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/profiler/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/profiler/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2561 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/profiler/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/scanning/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3590 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2314 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/scanning/DisplayPackageData.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/scanning/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/specialize/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    51703 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/specialize/CTypeDescriptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7717 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/specialize/Common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    39747 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/specialize/SpecializeC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    36683 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/specialize/SpecializePython.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/specialize/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/testing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    56174 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/testing/Common.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1516 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/Constructs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10129 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/testing/OutputComparison.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1310 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/testing/Pythons.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8061 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/RuntimeTracing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5413 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/SearchModes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3408 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/Valgrind.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/testing/check_reference_counts/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3095 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/testing/compare_with_cpython/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    29697 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/testing/find_sxs_modules/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1980 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/testing/measure_construct_performance/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     8758 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/testing/run_nuitka_tests/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    35342 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tools/watch/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3543 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/watch/GitHub.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tools/watch/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21532 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tools/watch/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/tree/
--rw-r--r--   0 hayen     (1000) hayen     (2000)    50436 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/Building.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    75150 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ComplexCallHelperFunctions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1733 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/Extractions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2603 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/InternalModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/Operations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2841 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/ReformulationAssertStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    43887 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/ReformulationAssignmentStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2981 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationBooleanExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11746 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationCallExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15446 2024-03-14 10:27:18.000000 Nuitka-2.2/nuitka/tree/ReformulationClasses.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    38202 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/ReformulationClasses3.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6523 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationComparisonExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22207 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/ReformulationContractionExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    11266 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/ReformulationDictionaryCreation.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14805 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/ReformulationExecStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7858 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationForLoopStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    30885 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/ReformulationFunctionStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14095 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationImportStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6630 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationLambdaExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationMatchStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2442 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationMultidist.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7608 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationNamespacePackages.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4711 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationPrintStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    15606 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationSequenceCreation.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4857 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14948 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationTryExceptStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5707 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14439 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationWithStatements.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3852 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/ReformulationYieldExpressions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13488 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/SourceHandling.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3790 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/SyntaxErrors.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23153 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/tree/TreeHelpers.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    20465 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/VariableClosure.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/tree/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/nuitka/utils/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3140 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/AppDirs.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4128 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/CStrings.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6394 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/CommandLineOptions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14983 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/Distributions.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6477 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/Download.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    13368 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/Execution.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    42054 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/FileOperations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3753 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Hashing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2395 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Images.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10334 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/Importing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/InstalledPythons.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2258 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/InstanceCounters.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4586 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Jinja2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1271 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Json.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4478 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/MacOSApp.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5092 2024-03-22 08:13:25.000000 Nuitka-2.2/nuitka/utils/MemoryUsage.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     9951 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/ModuleNames.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4588 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/ReExecute.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1889 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Rest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    23857 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/SharedLibraries.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3698 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/Shebang.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Signing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2084 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/SlotMetaClasses.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6603 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/StaticLibraries.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2634 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/ThreadedExecutor.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2798 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Timing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12655 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/Utils.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    10642 2024-04-30 08:27:49.000000 Nuitka-2.2/nuitka/utils/WindowsFileUsage.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    19837 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/WindowsResources.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/Yaml.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/nuitka/utils/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2/pyproject.toml
--rw-r--r--   0 hayen     (1000) hayen     (2000)       38 2024-04-30 08:28:44.290337 Nuitka-2.2/setup.cfg
--rw-r--r--   0 hayen     (1000) hayen     (2000)    16678 2024-04-30 08:27:49.000000 Nuitka-2.2/setup.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/tests/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/tests/basics/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1798 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/AssertsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5966 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/AssignmentsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5910 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/AssignmentsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4086 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/BranchingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1136 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/BuiltinOverload.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3781 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/BuiltinSuperTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    17112 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/BuiltinsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      898 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ClassMinimalTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4796 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ClassesTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3446 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ClassesTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1438 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ClassesTest34.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4729 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ComparisonChainsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4672 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ConstantsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ConstantsTest27.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/DecoratorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/DefaultParametersTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1159 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/DoubleDeletionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      838 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/EmptyModuleTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14418 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ExceptionRaisingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      993 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ExceptionRaisingTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1490 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ExceptionRaisingTest33.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     6779 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ExecEvalTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1450 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/basics/ExtremeClosureTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1689 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/basics/FunctionObjectsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    12367 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/FunctionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3635 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/FunctionsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2658 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/basics/FunctionsTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      922 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/FutureTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/GeneratorExpressionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/GeneratorExpressionsTest_37.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/GlobalStatementTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1318 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/HelloWorldTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2501 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ImportingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/InplaceOperationsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4259 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/InspectionTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/InspectionTest_35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1650 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/InspectionTest_36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1703 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/LambdasTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2763 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/LateClosureAssignmentTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2955 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ListContractionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3361 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/LoopingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1568 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/MainProgramsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1957 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ModuleAttributesTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2008 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/OperatorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    14935 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/OrderChecksTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/OrderChecksTest27.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1484 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/OverflowFunctionsTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5885 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ParameterErrorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ParameterErrorsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      895 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/PrintFutureTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1444 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/PrintingTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      910 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/RecursionTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    24798 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/basics/ReferencingTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2109 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ReferencingTest27.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     7869 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/basics/ReferencingTest33.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5060 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/basics/ReferencingTest35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     5497 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/basics/ReferencingTest36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2932 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ReferencingTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/SlotsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1191 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/ThreadedGeneratorsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)    22998 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TrickAssignmentsTest32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1573 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TrickAssignmentsTest35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1820 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TrickAssignmentsTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2118 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TryContinueFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2244 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TryExceptContinueTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2307 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TryExceptFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2336 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TryExceptFramesTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2874 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TryReturnFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2360 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/TryYieldFinallyTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1125 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/UnicodeTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1909 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/UnpackingTest35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2143 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/VarargsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     4913 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/WithStatementsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3103 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/YieldFromTest33.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3851 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/run_all.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2302 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/basics/run_xml.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.270337 Nuitka-2.2/tests/onefile/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1341 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/onefile/HelloWorldTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1339 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/onefile/KeyboardInterruptTest.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     5846 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/onefile/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/optimizations/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      991 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/optimizations/ArgumentTypes.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1087 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/AttributesTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1053 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/CallsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      953 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/ConditionsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/DecodingOperationsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1246 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/FormatStringsTest36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1183 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/HardImportsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1007 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/HardImportsTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      950 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/optimizations/Iterations.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1292 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/LenTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1133 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/MatchingTest310.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2295 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/OperationsTest.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1365 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/optimizations/SubscriptsTest.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     8827 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/optimizations/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/packages/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/packages/package_data_files_embedding/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1576 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/package_data_files_embedding/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/packages/package_import_success_after_failure/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2414 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/packages/package_import_success_after_failure/variable_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      975 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/tests/packages/sub_package/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/packages/sub_package/kitty/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1262 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/sub_package/kitty/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      940 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/sub_package/kitty/bigkitty.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      942 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/sub_package/kitty/smallkitty.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/packages/sub_package/kitty/speak/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      961 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/sub_package/kitty/speak/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1085 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/sub_package/kitty/speak/hello.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      999 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/sub_package/kitty/speak/miau.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1001 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/sub_package/kitty/speak/purr.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.110337 Nuitka-2.2/tests/packages/top_level_attributes_3/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/packages/top_level_attributes_3/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2368 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/plugins/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/plugins/code_signing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1202 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/plugins/code_signing/CodeSigningMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/plugins/data_files/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1474 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/plugins/data_files/DataFilesMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/plugins/data_files/data_files_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/plugins/data_files/data_files_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.2/tests/plugins/data_files/data_files_package/lala.txt
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/plugins/data_files/data_files_package/sub_dir/
--rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.2/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)      309 2024-01-26 12:30:51.000000 Nuitka-2.2/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/plugins/parameters/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1162 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/plugins/parameters/ParametersMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2218 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/plugins/parameters/parameter-using-plugin.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3778 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/plugins/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/absolute_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/absolute_import/foobar/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      828 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/absolute_import/foobar/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1076 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/absolute_import/foobar/foobar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/absolute_import/foobar/local.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      893 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/absolute_import/foobar/util.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports1/CasedImportingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports1/path1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports1/path1/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports1/path1/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports1/path2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports1/path2/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports1/path2/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports2/CasedImportingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports2/path1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports2/path1/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports2/path1/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports2/path2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports2/path2/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports2/path2/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports3/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1107 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports3/CasedImportingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports3/path1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports3/path1/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports3/path1/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports3/path2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports3/path2/Some_Module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/case_imports3/path2/Some_Package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/cyclic_imports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/dash_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/dash_import/DashImportMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/dash_import/dash-module.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/dash_import/plus+module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/dash_main/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/dash_main/Dash-Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/deep/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/deep/DeepProgramMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/deep/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1012 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/deep/some_package/DeepBrother.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/deep/some_package/DeepChild.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/deep/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/deep/some_package/deep_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      984 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/deep/some_package/deep_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/dunderinit_imports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      826 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/dunderinit_imports/package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      829 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/dunderinit_imports/package/SubModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      889 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/dunderinit_imports/package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/import_variants/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1037 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/import_variants/ImportVariationsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/import_variants/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      978 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/import_variants/some_package/Child1.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1130 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/import_variants/some_package/Child2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      854 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/import_variants/some_package/Child3.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1026 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/import_variants/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/main_raises/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/main_raises/ErrorMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/main_raises/ErrorRaising.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/main_raises2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1112 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/main_raises2/ErrorRaising.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/module_attributes/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1561 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/module_attributes/package_level1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1800 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_attributes/package_level1/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1800 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1800 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/module_exits/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_exits/ErrorExitingModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_exits/Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/module_object_replacing/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1110 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1391 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/multiprocessing_using/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/multiprocessing_using/foo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/multiprocessing_using/foo/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      868 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/multiprocessing_using/foo/__main__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1791 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/multiprocessing_using/foo/entry.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/named_imports/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/named_imports/NamedImportsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/named_imports/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/named_imports/some_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      856 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/named_imports/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/named_imports/some_package/sub_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_code/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_code/PackageInitCodeMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_code/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_code/some_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_code/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_contains_main/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_contains_main/PackageContainsMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_contains_main/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_contains_main/local.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_init_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      855 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_init_import/PackageInitImportMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_init_import/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1064 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1225 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/package_init_import/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_init_issue/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_init_issue/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_init_issue/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_init_issue/some_package/child_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_missing_init/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      958 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_missing_init/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      997 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_missing_init/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_missing_init/some_package/sub_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1009 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_module_collision/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      933 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_module_collision/Something/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_module_collision/Something/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_module_collision/something.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_overload/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      884 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_overload/Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_overload/foo/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_overload/foo/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_overload/foo/bar.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_overload/foo/bar2.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_prevents_submodule/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3079 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_prevents_submodule/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.120337 Nuitka-2.2/tests/programs/package_program/
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/package_program/PackageAsMain/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/package_program/PackageAsMain/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/package_program/PackageAsMain/__main__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/pkgutil_itermodules/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1760 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/pkgutil_usage/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/pkgutil_usage/package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2021-04-22 06:31:42.000000 Nuitka-2.2/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.2/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.2/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/pkgutil_usage/package/__init__.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/plugin_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      891 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/plugin_import/PluginImportMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/plugin_import/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      803 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/plugin_import/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/plugin_import/some_package/some_module.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/reimport_main_dynamic/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/reimport_main_static/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/relative_import/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/relative_import/RelativeImportMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/relative_import/dircache.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/resource_reader37/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1202 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/resource_reader37/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2022-10-08 09:07:15.000000 Nuitka-2.2/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/resource_reader37/some_package/__init__.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     6614 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/programs/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/stdlib_overload/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/stdlib_overload/pyexpat.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.280337 Nuitka-2.2/tests/programs/stdlib_overload/some_package/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/stdlib_overload/some_package/__init__.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1268 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/tests/programs/syntax_errors/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      822 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/syntax_errors/IndentationErroring.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/syntax_errors/SyntaxErroring.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/tests/programs/unicode_bom/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      995 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/unicode_bom/unicode_bom.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/tests/programs/with space/
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/programs/with space/Space Main.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/tests/reflected/
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)    14254 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/reflected/compile_itself.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1274 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/run-tests
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/tests/standalone/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1090 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/BrotliUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2586 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/CtypesUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/DateutilsUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1168 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/FlaskUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1307 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/standalone/GiUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/GlfwUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1216 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/GtkUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1057 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/HexEncodingTest_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1118 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/IdnaUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1215 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/LxmlUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1598 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/MatplotlibUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2570 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/MetadataPackagesUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1759 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/NumpyUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      979 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/OpenGLUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1479 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PandasUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1098 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PasslibUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1248 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PendulumUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2106 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PkgResourcesRequiresUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1099 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PmwUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1369 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PyQt5Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1253 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PyQt5SSLSupport.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2198 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PyQt5Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PyQt6Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PyQt6Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PySide2Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PySide6Plugins.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/PySide6Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1371 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/RsaUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1227 2024-04-30 08:27:49.000000 Nuitka-2.2/tests/standalone/SetuptoolsUsing_311.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1005 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/ShlibUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/SocketUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1973 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/TkInterUsing.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     3260 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/Urllib3Using.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1232 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/Win32ComUsing.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     9912 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/run_all.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/tests/standalone/zip_importer/
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1296 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/standalone/zip_importer/ZipImporterMain.py
-drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-04-30 08:28:44.290337 Nuitka-2.2/tests/syntax/
--rw-r--r--   0 hayen     (1000) hayen     (2000)      844 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/AsyncgenReturn36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      818 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/AwaitInModule36.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/BreakWithoutLoop.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/ClassReturn.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/ClosureDel_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      882 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/ContinueWithoutLoop.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/DuplicateArgument.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1142 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/ExecWithNesting_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/FutureBraces.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/FutureUnknown.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/GeneratorExpressions38.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/GeneratorReturn_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/GlobalForParameter.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/Importing32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/IndentationError.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      947 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/LateFutureImport.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/MisplacedFutureImport.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/ModuleReturn.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      915 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/NonlocalForParameter32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/NonlocalNotFound32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/StarImportExtra.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/SyntaxError.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/TryExceptAllNotLast.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/TryFinallyContinue_37.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      808 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/UnpackNoTuple.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/UnpackTwoStars32.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/YieldFromInModule.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/YieldInAsync35.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/YieldInGenexp38.py
--rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/YieldInModule.py
--rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2234 2024-03-04 14:35:43.000000 Nuitka-2.2/tests/syntax/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.573850 Nuitka-2.2.1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      235 2024-04-30 08:27:49.000000 Nuitka-2.2.1/Changelog.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   152288 2024-04-30 08:27:49.000000 Nuitka-2.2.1/Developer_Manual.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11348 2021-04-22 06:31:42.000000 Nuitka-2.2.1/LICENSE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1707 2024-01-26 12:30:51.000000 Nuitka-2.2.1/MANIFEST.in
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/Nuitka.egg-info/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    82956 2024-05-05 17:47:41.000000 Nuitka-2.2.1/Nuitka.egg-info/PKG-INFO
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    78171 2024-05-05 17:47:41.000000 Nuitka-2.2.1/Nuitka.egg-info/SOURCES.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-05-05 17:47:41.000000 Nuitka-2.2.1/Nuitka.egg-info/dependency_links.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      393 2024-05-05 17:47:41.000000 Nuitka-2.2.1/Nuitka.egg-info/entry_points.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        1 2024-02-02 15:24:24.000000 Nuitka-2.2.1/Nuitka.egg-info/not-zip-safe
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        7 2024-05-05 17:47:41.000000 Nuitka-2.2.1/Nuitka.egg-info/top_level.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    82956 2024-05-05 17:47:41.573850 Nuitka-2.2.1/PKG-INFO
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    80812 2024-03-04 14:35:43.000000 Nuitka-2.2.1/README.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/bin/
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1166 2024-03-04 14:35:43.000000 Nuitka-2.2.1/bin/autoformat-nuitka-source
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1165 2024-03-04 14:35:43.000000 Nuitka-2.2.1/bin/check-nuitka-with-pylint
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1181 2024-03-04 14:35:43.000000 Nuitka-2.2.1/bin/compare_with_cpython
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3105 2024-03-04 14:35:43.000000 Nuitka-2.2.1/bin/compare_with_xml
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1194 2024-03-04 14:35:43.000000 Nuitka-2.2.1/bin/measure-construct-performance
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.2.1/bin/nuitka
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1716 2024-03-04 14:35:43.000000 Nuitka-2.2.1/bin/nuitka-run
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/doc/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/doc/Logo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1797 2024-03-04 14:35:43.000000 Nuitka-2.2.1/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1553 2024-03-04 14:35:43.000000 Nuitka-2.2.1/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1793 2024-03-04 14:35:43.000000 Nuitka-2.2.1/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/doc/images/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7585 2021-04-22 06:31:42.000000 Nuitka-2.2.1/doc/images/Nuitka-Logo-Horizontal.png
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4452 2021-04-22 06:31:42.000000 Nuitka-2.2.1/doc/images/Nuitka-Logo-Symbol.png
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9828 2022-01-09 15:54:20.000000 Nuitka-2.2.1/doc/images/Nuitka-Logo-Vertical.png
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33696 2024-04-30 08:27:49.000000 Nuitka-2.2.1/doc/nuitka-run.1
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33720 2024-04-30 08:27:49.000000 Nuitka-2.2.1/doc/nuitka.1
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/lib/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4640 2024-03-04 14:35:43.000000 Nuitka-2.2.1/lib/hints.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/misc/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      924 2024-03-04 14:35:43.000000 Nuitka-2.2.1/misc/nuitka-run.bat
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1061 2024-03-04 14:35:43.000000 Nuitka-2.2.1/misc/nuitka.bat
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/nuitka/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7560 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/Builtins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5787 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/BytecodeCaching.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3800 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/Bytecodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1855 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/CacheCleanup.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11181 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/Constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2570 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11098 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/HardImportRegistry.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    38106 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/MainControl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8616 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/ModuleRegistry.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    62366 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/OptionParsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    75259 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/Options.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5432 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/OutputDirectories.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15000 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/PostProcessing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6805 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/Progress.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9654 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/PythonFlavors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4093 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/PythonOperators.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14564 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/PythonVersions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8989 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/Serialization.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4703 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/SourceCodeReferences.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13335 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/Tracing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3512 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/TreeXML.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15470 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/Variables.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2466 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/Version.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6373 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/__main__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5604 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/__past__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/nuitka/build/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36409 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/Backend.scons
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8583 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/CCompilerVersion.scons
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3486 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/DataComposerInterface.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17749 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/Onefile.scons
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15361 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/SconsCaching.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35806 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/SconsCompilerSettings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5591 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/SconsHacks.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17868 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/SconsInterface.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2703 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/SconsProgress.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13210 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/SconsSpawn.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27035 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/SconsUtils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.463850 Nuitka-2.2.1/nuitka/build/include/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/nuitka/build/include/nuitka/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8216 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/allocator.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3499 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/builtins.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5196 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/calling.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/checkers.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/checksum_tools.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9333 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2460 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_cell.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9233 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17661 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_frame.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7267 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_function.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9189 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_generator.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1866 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_method.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7688 2024-04-19 13:34:22.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/constants.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1345 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/constants_blob.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1187 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/environment_variables.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1872 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/environment_variables_system.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5302 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/exception_groups.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50867 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/exceptions.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3792 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6474 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/freelists.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    86326 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/hedley.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3698 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/attributes.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2692 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/boolean.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1233 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1164 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/bytes.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11894 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10644 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13169 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13168 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10645 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1834 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/complex.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13606 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1235 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/floats.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4401 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1827 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/indexes.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3625 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/ints.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9599 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/iterators.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3678 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/lists.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1386 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/mappings.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4671 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12714 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5692 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5451 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5489 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2828 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15807 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13239 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5820 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4743 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5144 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5853 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5467 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20173 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8699 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3782 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3796 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4875 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2756 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10655 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9230 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5176 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4378 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5004 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4855 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4072 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/raising.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2367 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1175 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1141 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/sequences.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1054 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/sets.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8750 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/slices.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1363 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/strings.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17975 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5926 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helper/tuples.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16773 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/helpers.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6050 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/importing.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12979 2022-10-08 15:33:22.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/incbin.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1086 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/jit_sources.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16556 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/prelude.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3237 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/printing.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1811 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/python_pgo.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2343 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3729 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/threading.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3447 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/tracing.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1145 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/type_aliases.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3135 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/include/nuitka/unfreezing.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/appdirs/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1097 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24824 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/atomicwrites/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1069 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/bin/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1695 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/bin/scons.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/clcache/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/clcache/clcache/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       93 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    65424 2023-03-17 17:23:10.000000 Nuitka-2.2.1/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1491 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      243 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2522 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10517 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1915 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5404 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6438 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/glob2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1359 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/glob2/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       82 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6859 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4463 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8304 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       85 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/README.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2423 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17473 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1466 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       84 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2685 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1726 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12719 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    65386 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1626 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12281 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1400 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50849 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4428 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24500 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36528 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9197 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28559 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17474 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4340 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7308 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30853 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1722 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35875 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27644 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17080 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4214 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20501 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3316 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    47844 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33996 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8083 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27693 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6938 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17622 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    96183 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7358 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21540 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16000 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9589 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4197 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   121420 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4164 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    49503 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1965 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2736 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2614 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8467 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9314 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3131 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1989 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2483 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1718 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1605 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2170 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4179 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1882 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15042 2024-01-26 12:30:51.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39700 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12950 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4810 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3751 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3233 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2011 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14663 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.493850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14029 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    52665 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    40719 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24133 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14053 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2305 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34903 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    40510 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2166 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2859 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18084 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2078 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2004 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9248 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2784 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14869 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19499 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20832 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5149 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2290 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2657 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31283 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2379 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2267 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2720 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2796 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2147 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2936 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2935 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3785 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2777 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1711 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      142 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    29618 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3428 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2681 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2433 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1844 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4782 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2025 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2256 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2460 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2639 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1810 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2333 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2140 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1902 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2077 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2043 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18600 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25816 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3328 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8394 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2309 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2945 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6919 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4381 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4658 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4224 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13881 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1804 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11380 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    72761 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6841 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3579 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4375 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2827 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2513 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1991 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1819 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2502 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4695 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1927 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2473 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5992 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1831 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3730 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13016 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3415 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    48938 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3007 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3784 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4380 2024-01-26 12:30:51.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3557 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5612 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11034 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6824 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8120 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3596 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1818 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1742 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2465 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1776 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19253 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    44500 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19664 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7509 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53545 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34985 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13596 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28403 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7533 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20988 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    96818 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7752 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22350 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16068 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9565 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5239 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   135413 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5758 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    63474 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8354 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11500 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3180 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2227 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2739 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1767 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1654 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1460 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2219 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4476 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4003 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17055 2024-01-26 12:30:51.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41186 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13880 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4853 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3812 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2328 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15053 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13779 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53260 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39394 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26467 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14489 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35863 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42204 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2211 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18207 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2152 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2057 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10674 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2855 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15165 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    33537 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21762 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4464 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50660 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1667 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2316 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2840 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8618 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2226 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2978 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2977 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1653 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3827 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3389 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      313 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3631 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3444 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8494 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1753 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.503850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    29765 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3472 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1630 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1977 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3686 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2580 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2655 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1645 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2765 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2189 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1944 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2123 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2085 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15791 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26195 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13924 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4041 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2351 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2987 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7808 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4956 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5235 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4808 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2475 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14751 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1847 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12588 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    82939 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6883 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3663 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2660 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4904 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2877 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2567 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1652 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1868 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2088 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2176 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2366 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1658 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1976 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5335 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2583 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2515 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6756 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3773 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13982 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3201 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53803 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3064 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3818 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4435 2024-01-26 12:30:51.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3643 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5579 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11655 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6504 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1647 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6869 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1784 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19816 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9002 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2149 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    56578 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35213 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11061 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27408 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21423 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    97269 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3979 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7515 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21937 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16583 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9430 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5126 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   136271 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6167 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    63768 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8183 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12836 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3087 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2107 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2630 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1674 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1311 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2076 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4356 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1805 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3860 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14831 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41983 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14673 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7394 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4357 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3546 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1972 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15577 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13597 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53509 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42760 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26676 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14272 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36753 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41191 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2122 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15570 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2014 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1943 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13182 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2734 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15027 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    38783 2023-03-17 17:23:10.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22570 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4368 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32724 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1578 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2228 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2386 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7993 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2141 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2893 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2889 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1567 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3742 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3296 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      343 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3534 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3259 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7461 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1663 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3379 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1891 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3616 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2377 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2437 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2526 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1557 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1772 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2677 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2206 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2096 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1851 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1954 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1995 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19180 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25826 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2588 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4649 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7652 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6064 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3931 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2266 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2900 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8622 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4577 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4517 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4113 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2387 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14473 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1752 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12902 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    84784 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6788 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3576 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4817 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2788 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2479 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1563 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1780 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1999 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2006 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2271 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1888 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4879 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2419 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2429 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6412 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1786 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12548 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4076 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    71693 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6632 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15278 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3134 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3896 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4648 2024-01-26 12:30:51.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3536 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5588 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12708 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6785 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      353 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4307 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1644 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3395 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21614 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9295 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2032 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10126 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      558 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4690 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1873 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/pkg_resources/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   107335 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      538 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1595 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      283 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      307 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      888 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      596 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1106 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      857 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1376 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10790 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    57572 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6948 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9726 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       99 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13170 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4883 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28639 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3851 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2837 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    43006 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2061 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6794 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14184 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8999 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51277 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.513850 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.523851 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9776 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4921 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25145 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3290 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2719 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    43298 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2559 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1132 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25542 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6746 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17711 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9122 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    52446 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4171 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.523851 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1101 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.523851 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9607 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4881 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25554 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3294 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2723 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42954 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2533 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2445 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1138 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1440 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25495 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6854 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14097 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8970 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51695 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4165 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2022-01-09 15:54:20.000000 Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.523851 Nuitka-2.2.1/nuitka/build/inline_copy/zlib/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zlib/LICENSE
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31605 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zlib/crc32.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   591749 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zlib/crc32.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16682 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zlib/zconf.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    96778 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zlib/zlib.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7247 2023-11-22 13:25:43.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zlib/zutil.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.523851 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1530 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.523851 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18198 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10157 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4455 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3763 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13662 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3009 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2441 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34422 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14748 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20216 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13930 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26976 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11706 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2728 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2497 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3828 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15880 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.523851 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    54982 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9164 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1321 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    80283 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    66784 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2253 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7906 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   138334 2021-04-22 06:31:42.000000 Nuitka-2.2.1/nuitka/build/inline_copy/zstd/zstd.h
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/build/static_src/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    83526 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9142 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledCellType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    58843 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    72002 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    40762 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledFrameType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   110213 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledFunctionType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    67496 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    56411 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22466 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/CompiledMethodType.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19054 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersAllocator.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    37583 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersAttributes.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23690 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersBuiltin.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   114017 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3062 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersBytes.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13376 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersCalling.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   481627 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2065 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3051 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersClasses.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   318889 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4762 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   314072 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   313483 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   317286 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   316697 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   315637 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36776 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20243 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39785 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersDictionaries.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26620 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2066 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersDumpBacktraces.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2194 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersEnvironmentVariables.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2979 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7924 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersExceptions.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8349 2024-04-19 13:34:22.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersFiles.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28776 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2455 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersFloats.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1803 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16080 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersImport.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16843 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersImportHard.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1815 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersJitSources.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21107 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersLists.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13944 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1669 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersMappings.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3587 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersMatching.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   182227 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19904 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77811 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77972 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    68218 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1265 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    69479 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6300 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    83954 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13805 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   183867 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   188543 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3593 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    67184 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    79484 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1052 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77854 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    70851 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    68736 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   151107 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4242 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53151 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53253 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    77119 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    47857 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17771 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   136385 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   142240 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    74749 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    83262 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    45341 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    83275 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    76950 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3294 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersProfiling.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18257 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersRaising.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3868 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3759 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersSequences.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1975 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersSlices.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32297 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersStrings.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4181 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersTuples.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6786 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/HelpersTypes.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12136 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/InspectPatcher.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    54011 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/MainProgram.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    63771 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4827 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6651 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21896 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31904 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/build/static_src/OnefileBootstrap.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8050 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/code_generation/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6491 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/AsyncgenCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10821 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/AttributeCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21926 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2371 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/BranchCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17006 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/BuiltinCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36111 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/CallCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4958 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/ClassCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    53395 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/code_generation/CodeGeneration.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2408 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/CodeHelperSelection.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14320 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/CodeHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5147 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/CodeObjectCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17957 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/ComparisonCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4479 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7368 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/ConditionalCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6901 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/ConstantCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34299 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/Contexts.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8589 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/CoroutineCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1607 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/CtypesCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28934 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/DictCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2159 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/Emission.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9289 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/ErrorCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12983 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/EvalCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9243 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/code_generation/ExceptionCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7384 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2126 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/ExpressionCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17852 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/FrameCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28336 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/FunctionCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7836 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/GeneratorCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6363 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/GlobalConstants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6985 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1870 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/IdCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14727 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/ImportCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1429 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/Indentation.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1574 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/IndexCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1066 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/InjectCCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3567 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/IntegerCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12211 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/IteratorCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1620 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/JitCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2055 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/LabelCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2645 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/LineNumberCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15849 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/ListCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6658 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/LoaderCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10016 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/LocalsDictCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3174 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/LoopCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1637 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/MatchCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6525 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/ModuleCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8224 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/Namify.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1860 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/NetworkxCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12733 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/OperationCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30198 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/PackageResourceCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3054 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/PrintCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5670 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/PythonAPICodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13251 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/RaisingCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3476 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/Reports.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5267 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/ReturnCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6591 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/SetCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14005 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/SliceCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10087 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/StringCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8302 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/SubscriptCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1939 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/TensorflowCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11208 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/TryCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3840 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/TupleCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2362 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/TypeAliasCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14811 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/VariableCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9155 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/VariableDeclarations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8129 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/YieldCodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/code_generation/c_types/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6102 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeBases.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3432 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1837 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1410 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3642 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5161 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5243 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3988 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19696 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2886 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/c_types/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/code_generation/templates/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2948 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9455 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3040 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2439 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6483 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3460 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3390 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2408 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4534 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22993 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6840 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2507 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/code_generation/templates_c/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11318 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5829 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23986 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5438 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1755 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1693 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2706 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13624 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1894 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2618 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1394 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7047 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12700 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1968 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4081 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7257 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4142 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3710 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4447 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11758 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19167 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2693 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3485 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11336 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15540 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2829 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10395 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2407 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2870 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2834 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3128 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/containers/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1467 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/containers/Namedtuples.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6553 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/containers/OrderedDicts.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      554 2022-10-08 09:07:15.000000 Nuitka-2.2.1/nuitka/containers/OrderedSets.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4430 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/containers/OrderedSetsFallback.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/containers/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/distutils/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2308 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/distutils/Build.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15025 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/distutils/DistutilCommands.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/distutils/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/finalizations/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1258 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/finalizations/Finalization.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6058 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/finalizations/FinalizeMarkups.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/finalizations/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/freezer/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7778 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/freezer/DependsExe.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2616 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/freezer/DllDependenciesCommon.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14396 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/freezer/DllDependenciesMacOS.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7468 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/freezer/DllDependenciesPosix.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6633 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/freezer/DllDependenciesWin32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11979 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/freezer/ImportDetection.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19236 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/freezer/IncludedDataFiles.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11455 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/freezer/IncludedEntryPoints.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9551 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/freezer/Onefile.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12245 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/freezer/Standalone.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/freezer/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.533851 Nuitka-2.2.1/nuitka/importing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11040 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/importing/IgnoreListing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2956 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/importing/ImportCache.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7784 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/importing/ImportResolving.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32895 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/importing/Importing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4869 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/importing/PreloadedPackages.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18804 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/importing/Recursion.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12787 2024-04-06 13:33:42.000000 Nuitka-2.2.1/nuitka/importing/StandardLibrary.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/importing/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/nodes/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3670 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/AsyncgenNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4115 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/AttributeLookupNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13255 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/AttributeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   379568 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/AttributeNodesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinAllNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4131 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinAnyNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2530 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinComplexNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1731 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2760 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4727 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinDictNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4982 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinFormatNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2275 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinHashNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1457 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinInputNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5367 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12812 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2029 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinLenNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3639 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinNextNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3787 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinOpenNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   246360 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18648 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinRangeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9468 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinRefNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3353 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinSumNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13576 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinTypeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1605 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/BuiltinVarsNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    26146 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/BytesNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6511 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/CallNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1583 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/Checkers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   647748 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/ChildrenHavingMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8480 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ClassNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6622 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/CodeObjectSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21716 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ComparisonNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30300 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ConditionalNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    47737 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/ConstantRefNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12246 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ContainerMakingNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2867 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ContainerOperationNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4614 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/CoroutineNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1746 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/CtypesNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51053 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/DictionaryNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8151 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/nodes/ExceptionNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7408 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ExecEvalNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    45046 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/ExpressionBases.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    55956 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ExpressionShapeMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12024 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/FrameNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3577 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/FunctionAttributeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    41167 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/FunctionNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5409 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/FutureSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6288 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/GeneratorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6961 2024-04-06 13:33:42.000000 Nuitka-2.2.1/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    98222 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/HardImportNodesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5631 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/ImportHardNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    48216 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/nodes/ImportNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2766 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/IndicatorMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1533 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/InjectCNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11519 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/IterationHandles.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11035 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/KeyValuePairNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16821 2024-03-11 17:07:05.000000 Nuitka-2.2.1/nuitka/nodes/ListOperationNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23177 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/LocalsDictNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15007 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/LocalsScopes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15995 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/LoopNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1745 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/MatchNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6567 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ModuleAttributeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32830 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/ModuleNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1759 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/NetworkxNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24461 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/NodeBases.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15147 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/NodeMakingHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5580 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/NodeMetaClasses.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31948 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/OperatorNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8976 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/OperatorNodesUnary.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5228 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/OsSysNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12468 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/OutlineNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    34735 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/PackageMetadataNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12289 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/PackageResourceNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3440 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/PrintNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6805 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/ReturnNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4748 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/SideEffectNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12547 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/SliceNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    98808 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/StatementBasesGenerated.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9336 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/StatementNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28691 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/StrNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3538 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/StringConcatenationNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8329 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/SubscriptNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1411 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/TensorflowNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17886 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/TryNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2438 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/TypeMatchNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11717 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/TypeNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42396 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/VariableAssignNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10779 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/VariableDelNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4607 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/VariableNameNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    31274 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/VariableRefNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4781 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/VariableReleaseNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3937 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/YieldNodes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/nodes/shapes/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   157357 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4420 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5076 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/shapes/ShapeMixins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42509 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/shapes/StandardShapes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/nodes/shapes/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/optimizations/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3358 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/optimizations/BytecodeDemotion.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/optimizations/FunctionInlining.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2177 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/optimizations/Graphs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10917 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/optimizations/Optimization.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    52575 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2287 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/optimizations/Tags.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42800 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/optimizations/TraceCollections.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    25799 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/optimizations/ValueTraces.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/optimizations/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/pgo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4932 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/pgo/PGO.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/pgo/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/plugins/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    57735 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/PluginBase.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    60905 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/plugins/Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/plugins/standard/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30813 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3509 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10627 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5080 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/DelvewheelPlugin.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/plugins/standard/DillPlugin/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1646 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/DillPlugin/DillPlugin.c
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9826 2024-03-22 08:13:25.000000 Nuitka-2.2.1/nuitka/plugins/standard/DillPlugin/dill-postLoad.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2679 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/DillPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16496 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2095 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/EnumPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1938 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/EventletPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1913 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/GeventPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4018 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/GiPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4854 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/GlfwPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    32325 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/ImplicitImports.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5024 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/KivyPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8824 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7080 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1220 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/NumpyPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7299 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1940 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/PbrPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4874 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7216 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/PmwPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51908 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3020 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1194 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13878 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/TkinterPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1174 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/TorchPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12838 2024-04-06 13:33:42.000000 Nuitka-2.2.1/nuitka/plugins/standard/TransformersPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1107 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/plugins/standard/TrioPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5668 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/UpxPlugin.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/plugins/standard/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)   236254 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-01-26 12:30:51.000000 Nuitka-2.2.1/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12392 2024-01-26 12:30:51.000000 Nuitka-2.2.1/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/reports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2286 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/reports/CompilationReportReader.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2089 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/reports/LicenseReport.rst.j2
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    28897 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/reports/Reports.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/reports/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/specs/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5943 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2818 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2573 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    27022 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/specs/BuiltinParameterSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6098 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1190 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4834 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7112 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/specs/HardImportSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    18811 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/specs/ParameterSpecs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/specs/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/tools/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1631 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/Basics.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/tools/commercial/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      847 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/commercial/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.543851 Nuitka-2.2.1/nuitka/tools/data_composer/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15004 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/data_composer/DataComposer.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/data_composer/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1338 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/data_composer/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/environments/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2481 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/environments/CreateEnvironment.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4198 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/environments/Virtualenv.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/environments/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/general/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/general/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/general/dll_report/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/general/dll_report/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2352 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/general/dll_report/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/general/find_module/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3953 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/general/find_module/FindModuleCode.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/general/find_module/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/onefile_compressor/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12545 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/onefile_compressor/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1343 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/onefile_compressor/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/podman/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1905 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/podman/Podman.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/podman/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11623 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/podman/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/profiler/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/profiler/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2561 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/profiler/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/scanning/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3590 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2314 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/scanning/DisplayPackageData.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/scanning/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/specialize/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    51703 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7717 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/specialize/Common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    39747 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/specialize/SpecializeC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    36683 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/specialize/SpecializePython.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/specialize/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/testing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    56174 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/testing/Common.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1516 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/Constructs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10129 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/testing/OutputComparison.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1310 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/testing/Pythons.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8061 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/RuntimeTracing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5413 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/SearchModes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3408 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/Valgrind.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/testing/check_reference_counts/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3095 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/testing/compare_with_cpython/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    29697 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/testing/find_sxs_modules/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1980 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/testing/measure_construct_performance/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     8758 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/testing/run_nuitka_tests/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    35342 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tools/watch/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3543 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/watch/GitHub.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tools/watch/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21532 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tools/watch/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/tree/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    50436 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/Building.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    75150 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1733 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/Extractions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2603 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/InternalModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1544 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/Operations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2841 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/ReformulationAssertStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    43887 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2981 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11746 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationCallExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15446 2024-03-14 10:27:18.000000 Nuitka-2.2.1/nuitka/tree/ReformulationClasses.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    38202 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/ReformulationClasses3.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6523 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22207 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/ReformulationContractionExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    11266 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14805 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/ReformulationExecStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7858 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationForLoopStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    30885 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/ReformulationFunctionStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14095 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationImportStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6630 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    21311 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationMatchStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2442 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationMultidist.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7608 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationNamespacePackages.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4711 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationPrintStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    15606 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationSequenceCreation.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4857 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14948 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5707 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14439 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationWithStatements.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3852 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/ReformulationYieldExpressions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13488 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/SourceHandling.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3790 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/SyntaxErrors.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23153 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/tree/TreeHelpers.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    20465 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/VariableClosure.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/tree/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/nuitka/utils/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3140 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/AppDirs.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4128 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/CStrings.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6394 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/CommandLineOptions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14983 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/Distributions.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6477 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/Download.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    13368 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/Execution.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    42167 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/utils/FileOperations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3753 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Hashing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2395 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Images.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10334 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/Importing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7884 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/InstalledPythons.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2258 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/InstanceCounters.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4586 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Jinja2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1271 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Json.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4478 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/MacOSApp.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5092 2024-03-22 08:13:25.000000 Nuitka-2.2.1/nuitka/utils/MemoryUsage.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     9951 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/ModuleNames.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4588 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/ReExecute.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1889 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Rest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    23857 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/SharedLibraries.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3698 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/Shebang.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3687 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Signing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2084 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/SlotMetaClasses.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6603 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/StaticLibraries.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2634 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/ThreadedExecutor.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2798 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Timing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12705 2024-05-05 17:47:38.000000 Nuitka-2.2.1/nuitka/utils/Utils.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    10642 2024-04-30 08:27:49.000000 Nuitka-2.2.1/nuitka/utils/WindowsFileUsage.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    19837 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/WindowsResources.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7014 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/Yaml.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/nuitka/utils/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      865 2024-03-04 14:35:43.000000 Nuitka-2.2.1/pyproject.toml
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       38 2024-05-05 17:47:41.573850 Nuitka-2.2.1/setup.cfg
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    16678 2024-04-30 08:27:49.000000 Nuitka-2.2.1/setup.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.553851 Nuitka-2.2.1/tests/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/basics/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1798 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/AssertsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5966 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/AssignmentsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5910 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/AssignmentsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4086 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/BranchingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1136 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/BuiltinOverload.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3781 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/BuiltinSuperTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    17112 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/BuiltinsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      898 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ClassMinimalTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4796 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ClassesTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3446 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ClassesTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1438 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ClassesTest34.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4729 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ComparisonChainsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4672 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ConstantsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ConstantsTest27.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/DecoratorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2349 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/DefaultParametersTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1159 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/DoubleDeletionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      838 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/EmptyModuleTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14418 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ExceptionRaisingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      993 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ExceptionRaisingTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1490 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ExceptionRaisingTest33.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     6779 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ExecEvalTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1450 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/basics/ExtremeClosureTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1689 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/basics/FunctionObjectsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    12367 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/FunctionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3635 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/FunctionsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2658 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/basics/FunctionsTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      922 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/FutureTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/GeneratorExpressionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/GeneratorExpressionsTest_37.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3856 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/GlobalStatementTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1318 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/HelloWorldTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2501 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ImportingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/InplaceOperationsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4259 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/InspectionTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1536 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/InspectionTest_35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1650 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/InspectionTest_36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1703 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/LambdasTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2763 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/LateClosureAssignmentTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2955 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ListContractionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3361 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/LoopingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1568 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/MainProgramsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1957 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ModuleAttributesTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2008 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/OperatorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    14935 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/OrderChecksTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1859 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/OrderChecksTest27.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1484 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/OverflowFunctionsTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5885 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ParameterErrorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1931 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ParameterErrorsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      895 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/PrintFutureTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1444 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/PrintingTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      910 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/RecursionTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    24798 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/basics/ReferencingTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2109 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ReferencingTest27.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     7869 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/basics/ReferencingTest33.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5060 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/basics/ReferencingTest35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     5497 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/basics/ReferencingTest36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2932 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ReferencingTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1662 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/SlotsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1191 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/ThreadedGeneratorsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)    22998 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TrickAssignmentsTest32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1573 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TrickAssignmentsTest35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1820 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TrickAssignmentsTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2118 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TryContinueFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2244 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TryExceptContinueTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2307 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TryExceptFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2336 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TryExceptFramesTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2874 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TryReturnFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2360 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/TryYieldFinallyTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1125 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/UnicodeTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1909 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/UnpackingTest35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2143 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/VarargsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     4913 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/WithStatementsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3103 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/YieldFromTest33.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3851 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/run_all.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2302 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/basics/run_xml.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/onefile/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1341 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/onefile/HelloWorldTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1339 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/onefile/KeyboardInterruptTest.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     5846 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/onefile/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/optimizations/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      991 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/optimizations/ArgumentTypes.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1087 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/AttributesTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1053 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/CallsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      953 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/ConditionsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/DecodingOperationsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1246 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/FormatStringsTest36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1183 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/HardImportsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1007 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/HardImportsTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      950 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/optimizations/Iterations.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1292 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/LenTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1133 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/MatchingTest310.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2295 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/OperationsTest.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1365 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/optimizations/SubscriptsTest.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     8827 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/optimizations/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/packages/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/packages/package_data_files_embedding/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1576 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/package_data_files_embedding/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/packages/package_import_success_after_failure/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2414 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/packages/package_import_success_after_failure/variable_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      975 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1201 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     4138 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/tests/packages/sub_package/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/packages/sub_package/kitty/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1262 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/sub_package/kitty/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      940 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/sub_package/kitty/bigkitty.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      942 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/sub_package/kitty/smallkitty.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      961 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1085 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/hello.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      999 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/miau.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1001 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/purr.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.473850 Nuitka-2.2.1/tests/packages/top_level_attributes_3/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/packages/top_level_attributes_3/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2368 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/plugins/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/plugins/code_signing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1202 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/plugins/code_signing/CodeSigningMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/plugins/data_files/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1474 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/plugins/data_files/DataFilesMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/plugins/data_files/data_files_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/plugins/data_files/data_files_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.2.1/tests/plugins/data_files/data_files_package/lala.txt
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)        0 2022-10-08 09:07:15.000000 Nuitka-2.2.1/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      309 2024-01-26 12:30:51.000000 Nuitka-2.2.1/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/plugins/parameters/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1162 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/plugins/parameters/ParametersMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2218 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/plugins/parameters/parameter-using-plugin.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     3778 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/plugins/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/absolute_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/absolute_import/foobar/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      828 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/absolute_import/foobar/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1076 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/absolute_import/foobar/foobar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/absolute_import/foobar/local.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      893 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/absolute_import/foobar/util.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports1/CasedImportingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports1/path1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports1/path1/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports1/path1/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports1/path2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports1/path2/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports1/path2/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      840 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports2/CasedImportingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports2/path1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports2/path1/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports2/path1/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports2/path2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports2/path2/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports2/path2/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports3/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1107 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports3/CasedImportingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports3/path1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports3/path1/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports3/path1/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports3/path2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports3/path2/Some_Module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/case_imports3/path2/Some_Package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/cyclic_imports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/dash_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/dash_import/DashImportMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/dash_import/dash-module.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      849 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/dash_import/plus+module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/dash_main/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/dash_main/Dash-Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/deep/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/deep/DeepProgramMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/deep/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1012 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/deep/some_package/DeepBrother.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/deep/some_package/DeepChild.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/deep/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/deep/some_package/deep_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      984 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/deep/some_package/deep_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/dunderinit_imports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      826 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/dunderinit_imports/package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      829 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      889 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/dunderinit_imports/package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/import_variants/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1037 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/import_variants/ImportVariationsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/import_variants/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      978 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/import_variants/some_package/Child1.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1130 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/import_variants/some_package/Child2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      854 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/import_variants/some_package/Child3.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1026 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/import_variants/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/main_raises/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/main_raises/ErrorMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/main_raises/ErrorRaising.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/main_raises2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1112 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/main_raises2/ErrorRaising.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/module_attributes/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1561 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1800 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1800 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1800 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1643 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/module_exits/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_exits/ErrorExitingModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      899 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_exits/Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/module_object_replacing/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1110 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1391 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/multiprocessing_using/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/multiprocessing_using/foo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      868 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1791 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/multiprocessing_using/foo/entry.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/named_imports/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/named_imports/NamedImportsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/named_imports/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/named_imports/some_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      856 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/named_imports/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/named_imports/some_package/sub_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_code/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_code/PackageInitCodeMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_code/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_code/some_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_code/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_contains_main/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_contains_main/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_contains_main/local.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_init_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      855 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_init_import/PackageInitImportMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_init_import/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1064 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1225 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/package_init_import/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_init_issue/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      821 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_init_issue/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_init_issue/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_init_issue/some_package/child_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_missing_init/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      958 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_missing_init/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      997 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_missing_init/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_missing_init/some_package/sub_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1009 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_module_collision/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      933 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_module_collision/Something/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_module_collision/Something/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_module_collision/something.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_overload/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      884 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_overload/Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_overload/foo/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_overload/foo/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_overload/foo/bar.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_overload/foo/bar2.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_prevents_submodule/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3079 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_prevents_submodule/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.483850 Nuitka-2.2.1/tests/programs/package_program/
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/package_program/PackageAsMain/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      920 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1661 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/package_program/PackageAsMain/__main__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1760 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/pkgutil_usage/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1328 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/pkgutil_usage/package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2021-04-22 06:31:42.000000 Nuitka-2.2.1/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.2.1/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       14 2022-10-08 09:07:15.000000 Nuitka-2.2.1/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1585 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/pkgutil_usage/package/__init__.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/plugin_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      891 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/plugin_import/PluginImportMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/plugin_import/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      803 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/plugin_import/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/plugin_import/some_package/some_module.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/reimport_main_dynamic/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      943 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/reimport_main_static/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      930 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/relative_import/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/relative_import/RelativeImportMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/relative_import/dircache.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/resource_reader37/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1202 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/resource_reader37/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)       13 2022-10-08 09:07:15.000000 Nuitka-2.2.1/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/resource_reader37/some_package/__init__.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     6614 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/programs/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/stdlib_overload/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      831 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/stdlib_overload/pyexpat.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      767 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      941 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      842 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1268 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/syntax_errors/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      822 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/syntax_errors/IndentationErroring.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      833 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1111 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/unicode_bom/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      995 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      878 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/unicode_bom/unicode_bom.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/programs/with space/
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/programs/with space/Space Main.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/reflected/
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)    14254 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/reflected/compile_itself.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     1274 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/run-tests
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/standalone/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1090 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/BrotliUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2586 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/CtypesUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1950 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/DateutilsUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1168 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/FlaskUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1307 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/standalone/GiUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1022 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/GlfwUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1216 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/GtkUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1057 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/HexEncodingTest_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1118 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/IdnaUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1215 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/LxmlUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1598 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/MatplotlibUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2570 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/MetadataPackagesUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1759 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/NumpyUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      979 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/OpenGLUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1479 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PandasUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1098 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PasslibUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1248 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PendulumUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2106 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1099 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PmwUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1369 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PyQt5Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1253 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PyQt5SSLSupport.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2198 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PyQt5Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1203 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PyQt6Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     2168 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PyQt6Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PySide2Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1123 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PySide6Plugins.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1789 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/PySide6Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1371 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/RsaUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1227 2024-04-30 08:27:49.000000 Nuitka-2.2.1/tests/standalone/SetuptoolsUsing_311.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1005 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/ShlibUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1569 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/SocketUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1973 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/TkInterUsing.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     3260 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/Urllib3Using.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1232 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/Win32ComUsing.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     9912 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/run_all.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.563850 Nuitka-2.2.1/tests/standalone/zip_importer/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1296 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/standalone/zip_importer/ZipImporterMain.py
+drwxr-xr-x   0 hayen     (1000) hayen     (2000)        0 2024-05-05 17:47:41.573850 Nuitka-2.2.1/tests/syntax/
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      844 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/AsyncgenReturn36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      818 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/AwaitInModule36.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      901 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/BreakWithoutLoop.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/ClassReturn.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1002 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/ClosureDel_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      882 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/ContinueWithoutLoop.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      824 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/DuplicateArgument.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1142 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/ExecWithNesting_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      858 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/FutureBraces.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/FutureUnknown.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1073 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/GeneratorExpressions38.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      911 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/GeneratorReturn_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/GlobalForParameter.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)     1027 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/Importing32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      830 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/IndentationError.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      947 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/LateFutureImport.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      874 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/MisplacedFutureImport.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      832 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/ModuleReturn.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      915 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      827 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/NonlocalForParameter32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/NonlocalNotFound32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      939 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/StarImportExtra.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      900 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/SyntaxError.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      907 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/TryExceptAllNotLast.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      908 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/TryFinallyContinue_37.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      808 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/UnpackNoTuple.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      841 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/UnpackTwoStars32.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      825 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/YieldFromInModule.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      837 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/YieldInAsync35.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      956 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/YieldInGenexp38.py
+-rw-r--r--   0 hayen     (1000) hayen     (2000)      813 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/YieldInModule.py
+-rwxr-xr-x   0 hayen     (1000) hayen     (2000)     2234 2024-03-04 14:35:43.000000 Nuitka-2.2.1/tests/syntax/run_all.py
```

### Comparing `Nuitka-2.2/Developer_Manual.rst` & `Nuitka-2.2.1/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/LICENSE.txt` & `Nuitka-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/MANIFEST.in` & `Nuitka-2.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/Nuitka.egg-info/PKG-INFO` & `Nuitka-2.2.1/Nuitka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 2.2
+Version: 2.2.1
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Commercial, https://nuitka.net/doc/commercial.html
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-2.2/Nuitka.egg-info/SOURCES.txt` & `Nuitka-2.2.1/Nuitka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/PKG-INFO` & `Nuitka-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka
-Version: 2.2
+Version: 2.2.1
 Summary: Python compiler with full language support and CPython compatibility
 Home-page: https://nuitka.net
 Author: Kay Hayen
 Author-email: Kay.Hayen@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Commercial, https://nuitka.net/doc/commercial.html
 Project-URL: Support, https://nuitka.net/pages/support.html
```

### Comparing `Nuitka-2.2/README.rst` & `Nuitka-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/bin/autoformat-nuitka-source` & `Nuitka-2.2.1/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/bin/check-nuitka-with-pylint` & `Nuitka-2.2.1/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/bin/compare_with_cpython` & `Nuitka-2.2.1/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/bin/compare_with_xml` & `Nuitka-2.2.1/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/bin/measure-construct-performance` & `Nuitka-2.2.1/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/bin/nuitka` & `Nuitka-2.2.1/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/bin/nuitka-run` & `Nuitka-2.2.1/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-2.2.1/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-2.2.1/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-2.2.1/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-2.2.1/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-2.2.1/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-2.2.1/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/nuitka-run.1` & `Nuitka-2.2.1/doc/nuitka-run.1`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/doc/nuitka.1` & `Nuitka-2.2.1/doc/nuitka.1`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/lib/hints.py` & `Nuitka-2.2.1/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/misc/nuitka-run.bat` & `Nuitka-2.2.1/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/misc/nuitka.bat` & `Nuitka-2.2.1/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Builtins.py` & `Nuitka-2.2.1/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/BytecodeCaching.py` & `Nuitka-2.2.1/nuitka/BytecodeCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Bytecodes.py` & `Nuitka-2.2.1/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/CacheCleanup.py` & `Nuitka-2.2.1/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Constants.py` & `Nuitka-2.2.1/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Errors.py` & `Nuitka-2.2.1/nuitka/Errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,18 @@
     """
 
 
 class NuitkaForbiddenDLLEncounter(Exception):
     """This DLL is not allowed to be included."""
 
 
+class NuitkaSyntaxError(Exception):
+    """The code cannot be read due to SyntaxError"""
+
+
 #     Part of "Nuitka", an optimizing Python compiler that is compatible and
 #     integrates with CPython, but also works on its own.
 #
 #     Licensed under the Apache License, Version 2.0 (the "License");
 #     you may not use this file except in compliance with the License.
 #     You may obtain a copy of the License at
 #
```

### Comparing `Nuitka-2.2/nuitka/HardImportRegistry.py` & `Nuitka-2.2.1/nuitka/HardImportRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/MainControl.py` & `Nuitka-2.2.1/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/ModuleRegistry.py` & `Nuitka-2.2.1/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/OptionParsing.py` & `Nuitka-2.2.1/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Options.py` & `Nuitka-2.2.1/nuitka/Options.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/OutputDirectories.py` & `Nuitka-2.2.1/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/PostProcessing.py` & `Nuitka-2.2.1/nuitka/PostProcessing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Progress.py` & `Nuitka-2.2.1/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/PythonFlavors.py` & `Nuitka-2.2.1/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/PythonOperators.py` & `Nuitka-2.2.1/nuitka/PythonOperators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/PythonVersions.py` & `Nuitka-2.2.1/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Serialization.py` & `Nuitka-2.2.1/nuitka/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/SourceCodeReferences.py` & `Nuitka-2.2.1/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Tracing.py` & `Nuitka-2.2.1/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/TreeXML.py` & `Nuitka-2.2.1/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Variables.py` & `Nuitka-2.2.1/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/Version.py` & `Nuitka-2.2.1/nuitka/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V2.2
+Nuitka V2.2.1
 Copyright (C) 2024 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-2.2/nuitka/__init__.py` & `Nuitka-2.2.1/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/__main__.py` & `Nuitka-2.2.1/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/__past__.py` & `Nuitka-2.2.1/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/Backend.scons` & `Nuitka-2.2.1/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/CCompilerVersion.scons` & `Nuitka-2.2.1/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/DataComposerInterface.py` & `Nuitka-2.2.1/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/Onefile.scons` & `Nuitka-2.2.1/nuitka/build/Onefile.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/SconsCaching.py` & `Nuitka-2.2.1/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/SconsCompilerSettings.py` & `Nuitka-2.2.1/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/SconsHacks.py` & `Nuitka-2.2.1/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/SconsInterface.py` & `Nuitka-2.2.1/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/SconsProgress.py` & `Nuitka-2.2.1/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/SconsSpawn.py` & `Nuitka-2.2.1/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/SconsUtils.py` & `Nuitka-2.2.1/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/__init__.py` & `Nuitka-2.2.1/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/allocator.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/builtins.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/calling.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/checkers.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/constants.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/environment_variables.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/environment_variables.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/environment_variables_system.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/environment_variables_system.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/exception_groups.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/exception_groups.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/freelists.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/hedley.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/helpers.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/importing.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/incbin.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/jit_sources.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/jit_sources.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/prelude.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/printing.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/threading.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/tracing.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/type_aliases.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/type_aliases.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-2.2.1/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-2.2.1/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-2.2.1/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-2.2.1/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-2.2.1/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-2.2.1/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-2.2.1/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zlib/LICENSE` & `Nuitka-2.2.1/nuitka/build/inline_copy/zlib/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zlib/crc32.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zlib/crc32.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zlib/zconf.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zlib/zlib.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zlib/zutil.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-2.2.1/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-2.2.1/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersDumpBacktraces.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersDumpBacktraces.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersEnvironmentVariables.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersEnvironmentVariables.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersEnvironmentVariablesSystem.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersImport.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersJitSources.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersJitSources.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersLists.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-2.2.1/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-2.2.1/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/MainProgram.c` & `Nuitka-2.2.1/nuitka/build/static_src/MainProgram.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-2.2.1/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-2.2.1/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-2.2.1/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/AttributeCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-2.2.1/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/BranchCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/CallCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ClassCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/CodeGeneration.py` & `Nuitka-2.2.1/nuitka/code_generation/CodeGeneration.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,14 +666,15 @@
         "EXPRESSION_BUILTIN_RANGE2": generateBuiltinRange2Code,
         "EXPRESSION_BUILTIN_RANGE3": generateBuiltinRange3Code,
         "EXPRESSION_BUILTIN_XRANGE1": generateBuiltinXrange1Code,
         "EXPRESSION_BUILTIN_XRANGE2": generateBuiltinXrange2Code,
         "EXPRESSION_BUILTIN_XRANGE3": generateBuiltinXrange3Code,
         "EXPRESSION_BUILTIN_MAKE_EXCEPTION": generateBuiltinMakeExceptionCode,
         "EXPRESSION_BUILTIN_MAKE_EXCEPTION_IMPORT_ERROR": generateBuiltinMakeExceptionCode,
+        "EXPRESSION_BUILTIN_MAKE_EXCEPTION_MODULE_NOT_FOUND_ERROR": generateBuiltinMakeExceptionCode,
         "EXPRESSION_BUILTIN_REF": generateBuiltinRefCode,
         "EXPRESSION_BUILTIN_WITH_CONTEXT_REF": generateBuiltinRefCode,
         "EXPRESSION_BUILTIN_EXCEPTION_REF": generateExceptionRefCode,
         "EXPRESSION_BUILTIN_ANONYMOUS_REF": generateBuiltinAnonymousRefCode,
         "EXPRESSION_CAUGHT_EXCEPTION_TYPE_REF": generateExceptionCaughtTypeCode,
         "EXPRESSION_CAUGHT_EXCEPTION_VALUE_REF": generateExceptionCaughtValueCode,
         "EXPRESSION_CAUGHT_EXCEPTION_TRACEBACK_REF": generateExceptionCaughtTracebackCode,
```

### Comparing `Nuitka-2.2/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-2.2.1/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/CodeHelpers.py` & `Nuitka-2.2.1/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-2.2.1/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ConstantCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/Contexts.py` & `Nuitka-2.2.1/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/CtypesCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/DictCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/Emission.py` & `Nuitka-2.2.1/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ErrorCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/EvalCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ExceptionCodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,22 @@
                 to_name=value_name,
                 called_name=getExceptionIdentifier(exception_type),
                 expression=expression,
                 emit=emit,
                 context=context,
             )
 
-        if expression.getExceptionName() == "ImportError" and python_version >= 0x300:
+        if exception_type == "ImportError" and python_version >= 0x300:
+            is_new_import_error = True
+        elif exception_type == "ModuleNotFoundError" and python_version >= 0x360:
+            is_new_import_error = True
+        else:
+            is_new_import_error = False
+
+        if is_new_import_error:
             from .PythonAPICodes import getReferenceExportCode
 
             import_error_name_expression = expression.subnode_name
 
             if import_error_name_expression is not None:
                 exception_importerror_name = context.allocateTempName(
                     "make_exception_importerror_name"
```

### Comparing `Nuitka-2.2/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-2.2.1/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/FrameCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/FunctionCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/GlobalConstants.py` & `Nuitka-2.2.1/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/IdCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ImportCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/Indentation.py` & `Nuitka-2.2.1/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/IndexCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/InjectCCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/IntegerCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/IteratorCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/JitCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/JitCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/LabelCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ListCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/LoaderCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/LoopCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/MatchCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ModuleCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/Namify.py` & `Nuitka-2.2.1/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/NetworkxCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/NetworkxCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/OperationCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/PrintCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-2.2.1/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/RaisingCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/Reports.py` & `Nuitka-2.2.1/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/ReturnCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/SetCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/SliceCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/StringCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/TensorflowCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/TensorflowCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/TryCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/TupleCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/TypeAliasCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/TypeAliasCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/VariableCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-2.2.1/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/YieldCodes.py` & `Nuitka-2.2.1/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/__init__.py` & `Nuitka-2.2.1/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/c_types/__init__.py` & `Nuitka-2.2.1/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates/__init__.py` & `Nuitka-2.2.1/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-2.2.1/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/containers/Namedtuples.py` & `Nuitka-2.2.1/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/containers/OrderedDicts.py` & `Nuitka-2.2.1/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/containers/OrderedSets.py` & `Nuitka-2.2.1/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-2.2.1/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/containers/__init__.py` & `Nuitka-2.2.1/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/distutils/Build.py` & `Nuitka-2.2.1/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/distutils/DistutilCommands.py` & `Nuitka-2.2.1/nuitka/distutils/DistutilCommands.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/distutils/__init__.py` & `Nuitka-2.2.1/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/finalizations/Finalization.py` & `Nuitka-2.2.1/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-2.2.1/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/finalizations/__init__.py` & `Nuitka-2.2.1/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/DependsExe.py` & `Nuitka-2.2.1/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-2.2.1/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-2.2.1/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from nuitka.utils.Importing import getSharedLibrarySuffixes
 from nuitka.utils.Json import loadJsonFromFilename
 from nuitka.utils.SharedLibraries import (
     callInstallNameTool,
     getOtoolDependencyOutput,
     getOtoolListing,
 )
+from nuitka.utils.Utils import getArchitecture
 
 from .DllDependenciesCommon import getLdLibraryPath
 
 # Detected Python rpath is cached.
 _detected_python_rpaths = None
 
 
@@ -129,14 +130,32 @@
             filename=filename,
         ):
             paths.add(filename)
 
     return paths
 
 
+def _getNonVersionedDllFilenames(filename):
+    yield filename
+
+    if getArchitecture() == "arm64" and filename.endswith(".dylib"):
+        yield filename[:-6] + "_arm64.dylib"
+
+    match = re.match(r"^(.*?)(\.\d+)+\.dylib$", filename)
+
+    if match:
+        yield match.group(1) + ".dylib"
+
+        # TODO: The versioned filename, might do the same, and so could the
+        # "x86_64" specific DLL be a thing too, but we should have actual
+        # examples to be sure they are covered with tests.
+        if getArchitecture() == "arm64":
+            yield match.group(1) + "_arm64.dylib"
+
+
 def _resolveBinaryPathDLLsMacOS(
     original_dir, binary_filename, paths, package_specific_dirs, package_name
 ):
     # Quite a few variations to consider
     # pylint: disable=too-many-branches,too-many-locals,too-many-statements
 
     had_self = False
@@ -191,30 +210,41 @@
 
             if parts[0] == package_name.asString():
                 resolved_path = os.path.join(
                     os.path.dirname(resolved_path), ".".join(parts[1:])
                 )
 
         # Some extension modules seem to reference themselves by a different
-        # extension module name, so use that if it exists.
-        if not os.path.exists(resolved_path) and python_version >= 0x300:
+        # extension module name, so use that if it exists, and some versioned
+        # DLL dependencies do not matter.
+        if python_version >= 0x300:
             so_suffixes = getSharedLibrarySuffixes()[:-1]
 
             specific_suffix = so_suffixes[0]
             abi_suffix = so_suffixes[1]
 
-            if resolved_path.endswith(specific_suffix):
-                candidate = resolved_path[: -len(specific_suffix)] + abi_suffix
-            elif resolved_path.endswith(abi_suffix):
-                candidate = resolved_path[: -len(specific_suffix)] + abi_suffix
-            else:
-                candidate = None
+            for resolved_path_candidate in _getNonVersionedDllFilenames(resolved_path):
+                if os.path.exists(resolved_path_candidate):
+                    resolved_path = resolved_path_candidate
+                    break
+
+                if resolved_path_candidate.endswith(specific_suffix):
+                    candidate = (
+                        resolved_path_candidate[: -len(specific_suffix)] + abi_suffix
+                    )
+                elif resolved_path_candidate.endswith(abi_suffix):
+                    candidate = (
+                        resolved_path_candidate[: -len(specific_suffix)] + abi_suffix
+                    )
+                else:
+                    candidate = None
 
-            if candidate is not None and os.path.exists(candidate):
-                resolved_path = candidate
+                if candidate is not None and os.path.exists(candidate):
+                    resolved_path = candidate
+                    break
 
         # Sometimes self-dependencies are on a numbered version, but deployed is
         # one version without it. The macOS just ignores that, and so we do.
         if not os.path.exists(resolved_path):
             if os.path.basename(resolved_path) == os.path.basename(binary_filename):
                 resolved_path = binary_filename
             else:
@@ -246,14 +276,25 @@
 
             # TODO: Missing DLLs that are accepted, are not really forbidden, we
             # should instead acknowledge them as missing, and treat that properly
             # in using code.
             if acceptable is True:
                 raise NuitkaForbiddenDLLEncounter(binary_filename, plugin_name)
 
+            # We check both the user and the used DLL if they are listed. This
+            # might be a form of bug hiding, that the later is not sufficient,
+            # that we should address later.
+            acceptable, plugin_name = Plugins.isAcceptableMissingDLL(
+                package_name=package_name,
+                filename=resolved_path,
+            )
+
+            if acceptable is True:
+                raise NuitkaForbiddenDLLEncounter(binary_filename, plugin_name)
+
             if not path.startswith(("@", "/")):
                 continue
 
             inclusion_logger.sysexit(
                 "Error, failed to find path %s (resolved DLL to %s) for %s from '%s', please report the bug."
                 % (path, resolved_path, binary_filename, package_name)
             )
```

### Comparing `Nuitka-2.2/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-2.2.1/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-2.2.1/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/ImportDetection.py` & `Nuitka-2.2.1/nuitka/freezer/ImportDetection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-2.2.1/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-2.2.1/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/Onefile.py` & `Nuitka-2.2.1/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/Standalone.py` & `Nuitka-2.2.1/nuitka/freezer/Standalone.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/freezer/__init__.py` & `Nuitka-2.2.1/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/IgnoreListing.py` & `Nuitka-2.2.1/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/ImportCache.py` & `Nuitka-2.2.1/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/ImportResolving.py` & `Nuitka-2.2.1/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/Importing.py` & `Nuitka-2.2.1/nuitka/importing/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/PreloadedPackages.py` & `Nuitka-2.2.1/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/Recursion.py` & `Nuitka-2.2.1/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/StandardLibrary.py` & `Nuitka-2.2.1/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/importing/__init__.py` & `Nuitka-2.2.1/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-2.2.1/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-2.2.1/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/AttributeNodes.py` & `Nuitka-2.2.1/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-2.2.1/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinInputNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinInputNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinRefNodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from nuitka.PythonVersions import python_version
 from nuitka.specs import BuiltinParameterSpecs
 
 from .ConstantRefNodes import makeConstantRefNode
 from .ExceptionNodes import (
     ExpressionBuiltinMakeException,
     ExpressionBuiltinMakeExceptionImportError,
+    ExpressionBuiltinMakeExceptionModuleNotFoundError,
 )
 from .ExpressionBases import CompileTimeConstantExpressionBase
 from .shapes.BuiltinTypeShapes import tshape_exception_class
 
 
 class ExpressionBuiltinRefBase(CompileTimeConstantExpressionBase):
     # Base classes can be abstract, pylint: disable=abstract-method
@@ -230,14 +231,21 @@
             if exception_name == "ImportError" and python_version >= 0x300:
                 return ExpressionBuiltinMakeExceptionImportError(
                     args=args,
                     name=name,
                     path=path,
                     source_ref=source_ref,
                 )
+            elif exception_name == "ModuleNotFoundError" and python_version >= 0x360:
+                return ExpressionBuiltinMakeExceptionModuleNotFoundError(
+                    args=args,
+                    name=name,
+                    path=path,
+                    source_ref=source_ref,
+                )
             else:
                 # We expect to only get the star arguments for these.
                 assert name is None
                 assert path is None
 
                 return ExpressionBuiltinMakeException(
                     exception_name=exception_name, args=args, source_ref=source_ref
```

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/BytesNodes.py` & `Nuitka-2.2.1/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/CallNodes.py` & `Nuitka-2.2.1/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/Checkers.py` & `Nuitka-2.2.1/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-2.2.1/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ClassNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-2.2.1/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ComparisonNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ConditionalNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/CoroutineNodes.py` & `Nuitka-2.2.1/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/CtypesNodes.py` & `Nuitka-2.2.1/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/DictionaryNodes.py` & `Nuitka-2.2.1/nuitka/nodes/DictionaryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ExceptionNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ExceptionNodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,24 @@
         return False
 
     @staticmethod
     def mayRaiseExceptionOperation():
         return False
 
 
+class ExpressionBuiltinMakeExceptionModuleNotFoundError(
+    ExpressionBuiltinMakeExceptionImportError
+):
+    kind = "EXPRESSION_BUILTIN_MAKE_EXCEPTION_MODULE_NOT_FOUND_ERROR"
+
+    @staticmethod
+    def getExceptionName():
+        return "ModuleNotFoundError"
+
+
 class ExpressionCaughtMixin(ExpressionNoSideEffectsMixin):
     """Common things for all caught exception references."""
 
     __slots__ = ()
 
     def finalize(self):
         del self.parent
```

### Comparing `Nuitka-2.2/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ExpressionBases.py` & `Nuitka-2.2.1/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-2.2.1/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-2.2.1/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/FrameNodes.py` & `Nuitka-2.2.1/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-2.2.1/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/FunctionNodes.py` & `Nuitka-2.2.1/nuitka/nodes/FunctionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/FutureSpecs.py` & `Nuitka-2.2.1/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/GeneratorNodes.py` & `Nuitka-2.2.1/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-2.2.1/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-2.2.1/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ImportHardNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ImportNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ImportNodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from nuitka.importing.StandardLibrary import isStandardLibraryPath
 from nuitka.Options import (
     isExperimental,
     isStandaloneMode,
     shallMakeModule,
     shallWarnUnusualCode,
 )
+from nuitka.plugins.Plugins import Plugins
 from nuitka.PythonVersions import python_version
 from nuitka.specs.BuiltinParameterSpecs import (
     BuiltinParameterSpec,
     extractBuiltinArgs,
 )
 from nuitka.Tracing import unusual_logger
 from nuitka.utils.ModuleNames import ModuleName
@@ -921,14 +922,22 @@
         module_name = ModuleName(module_name)
         module_name_found, module_filename, module_kind, self.finding = locateModule(
             module_name=ModuleName(module_name),
             parent_package=parent_package,
             level=level_value,
         )
 
+        # Allow for the import look ahead, to change what modules are
+        # considered hard imports.
+        Plugins.onModuleUsageLookAhead(
+            module_name=module_name_found,
+            module_filename=module_filename,
+            module_kind=module_kind,
+        )
+
         self.used_modules = makeParentModuleUsagesAttempts(
             makeModuleUsageAttempt(
                 module_name=module_name_found,
                 filename=module_filename,
                 module_kind=module_kind,
                 finding=self.finding,
                 level=level_value,
```

### Comparing `Nuitka-2.2/nuitka/nodes/IndicatorMixins.py` & `Nuitka-2.2.1/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/InjectCNodes.py` & `Nuitka-2.2.1/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/IterationHandles.py` & `Nuitka-2.2.1/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-2.2.1/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ListOperationNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-2.2.1/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/LocalsScopes.py` & `Nuitka-2.2.1/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/LoopNodes.py` & `Nuitka-2.2.1/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/MatchNodes.py` & `Nuitka-2.2.1/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ModuleNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ModuleNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/NetworkxNodes.py` & `Nuitka-2.2.1/nuitka/nodes/NetworkxNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/NodeBases.py` & `Nuitka-2.2.1/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-2.2.1/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-2.2.1/nuitka/nodes/NodeMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/OperatorNodes.py` & `Nuitka-2.2.1/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-2.2.1/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/OsSysNodes.py` & `Nuitka-2.2.1/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/OutlineNodes.py` & `Nuitka-2.2.1/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-2.2.1/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-2.2.1/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/PrintNodes.py` & `Nuitka-2.2.1/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/ReturnNodes.py` & `Nuitka-2.2.1/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/SideEffectNodes.py` & `Nuitka-2.2.1/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/SliceNodes.py` & `Nuitka-2.2.1/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-2.2.1/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/StatementNodes.py` & `Nuitka-2.2.1/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/StrNodes.py` & `Nuitka-2.2.1/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-2.2.1/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/SubscriptNodes.py` & `Nuitka-2.2.1/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/TensorflowNodes.py` & `Nuitka-2.2.1/nuitka/nodes/TensorflowNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/TryNodes.py` & `Nuitka-2.2.1/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-2.2.1/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/TypeNodes.py` & `Nuitka-2.2.1/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-2.2.1/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/VariableDelNodes.py` & `Nuitka-2.2.1/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/VariableNameNodes.py` & `Nuitka-2.2.1/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/VariableRefNodes.py` & `Nuitka-2.2.1/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-2.2.1/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/YieldNodes.py` & `Nuitka-2.2.1/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/__init__.py` & `Nuitka-2.2.1/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-2.2.1/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-2.2.1/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-2.2.1/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-2.2.1/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/nodes/shapes/__init__.py` & `Nuitka-2.2.1/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-2.2.1/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/FunctionInlining.py` & `Nuitka-2.2.1/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/Graphs.py` & `Nuitka-2.2.1/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/Optimization.py` & `Nuitka-2.2.1/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-2.2.1/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/Tags.py` & `Nuitka-2.2.1/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/TraceCollections.py` & `Nuitka-2.2.1/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/ValueTraces.py` & `Nuitka-2.2.1/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/optimizations/__init__.py` & `Nuitka-2.2.1/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/pgo/PGO.py` & `Nuitka-2.2.1/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/pgo/__init__.py` & `Nuitka-2.2.1/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/PluginBase.py` & `Nuitka-2.2.1/nuitka/plugins/PluginBase.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/Plugins.py` & `Nuitka-2.2.1/nuitka/plugins/Plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from optparse import OptionConflictError, OptionGroup
 
 from nuitka import Options, OutputDirectories
 from nuitka.__past__ import basestring, iter_modules
 from nuitka.build.DataComposerInterface import deriveModuleConstantsBlobName
 from nuitka.containers.OrderedDicts import OrderedDict
 from nuitka.containers.OrderedSets import OrderedSet
+from nuitka.Errors import NuitkaSyntaxError
 from nuitka.freezer.IncludedDataFiles import IncludedDataFile
 from nuitka.freezer.IncludedEntryPoints import IncludedEntryPoint
 from nuitka.ModuleRegistry import addUsedModule
 from nuitka.PythonVersions import python_version
 from nuitka.Tracing import plugins_logger, printLine
 from nuitka.utils.FileOperations import (
     getDllBasename,
@@ -1053,25 +1054,34 @@
                 source_filename = os.path.join(module_filename, "__init__.py")
             else:
                 source_filename = module_filename
 
             if not os.path.isfile(source_filename):
                 return None
 
-            return readSourceCodeFromFilename(
-                module_name=module_name, source_filename=source_filename, pre_load=True
-            )
+            try:
+                return readSourceCodeFromFilename(
+                    module_name=module_name,
+                    source_filename=source_filename,
+                    pre_load=True,
+                )
+            except SyntaxError as e:
+                # Look ahead just not possible.
+                raise NuitkaSyntaxError(e)
 
-        for plugin in getActivePlugins():
-            plugin.onModuleUsageLookAhead(
-                module_name=module_name,
-                module_filename=module_filename,
-                module_kind=module_kind,
-                get_module_source=getModuleSourceCode,
-            )
+        try:
+            for plugin in getActivePlugins():
+                plugin.onModuleUsageLookAhead(
+                    module_name=module_name,
+                    module_filename=module_filename,
+                    module_kind=module_kind,
+                    get_module_source=getModuleSourceCode,
+                )
+        except NuitkaSyntaxError:
+            pass
 
     @staticmethod
     def onModuleRecursion(
         module_name, module_filename, module_kind, using_module_name, source_ref, reason
     ):
         for plugin in getActivePlugins():
             plugin.onModuleRecursion(
@@ -1424,15 +1434,15 @@
     @classmethod
     def isAcceptableMissingDLL(cls, package_name, filename):
         dll_basename = getDllBasename(os.path.basename(filename))
 
         # Not a DLL filename, then it cannot be true, but it's kind of strange
         # to get asked.
         if dll_basename is None:
-            return False
+            return None, None
 
         result = None
         plugin_name = None
 
         for plugin in getActivePlugins():
             value = plugin.isAcceptableMissingDLL(
                 package_name=package_name, dll_basename=dll_basename
```

### Comparing `Nuitka-2.2/nuitka/plugins/__init__.py` & `Nuitka-2.2.1/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/DillPlugin/DillPlugin.c` & `Nuitka-2.2.1/nuitka/plugins/standard/DillPlugin/DillPlugin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/DillPlugin/dill-postLoad.py` & `Nuitka-2.2.1/nuitka/plugins/standard/DillPlugin/dill-postLoad.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,20 @@
                     # consider those as well, spell-checker: ignore dylibs
                     dylib_directory = os.path.join(package_directory, ".dylibs")
 
                     if os.path.isdir(package_directory):
                         yield dylib_directory
 
     def isAcceptableMissingDLL(self, package_name, dll_basename):
+        if package_name is None:
+            return None
+
+        # Config is to be attached to top level package.
+        package_name = package_name.getTopLevelPackageName()
+
         for entry in self.config.get(package_name, section="import-hacks"):
             if self.evaluateCondition(
                 full_name=package_name, condition=entry.get("when", "True")
             ):
                 result = self._isAcceptableMissingDLL(
                     config=entry, dll_basename=dll_basename
                 )
```

### Comparing `Nuitka-2.2/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-2.2.1/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/TransformersPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/TransformersPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-2.2.1/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/__init__.py` & `Nuitka-2.2.1/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-2.2.1/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1890,14 +1890,20 @@
       - '*.txt'
 
 - module-name: 'lark' # checksum: ab5b4914
   data-files:
     dirs:
       - 'grammars'
 
+- module-name: 'librosa' # checksum: 20378624
+  anti-bloat:
+    - description: 'allow numba inside of librosa, too dependent to remove'
+      bloat-mode-overrides:
+        'numba': 'allow'
+
 - module-name: 'librosa.core.intervals' # checksum: fc442d1
   data-files:
     patterns:
       - 'intervals.msgpack'
 
 - module-name: 'libusb_package' # checksum: 5cbb45ba
   dlls:
@@ -1995,14 +2001,27 @@
         - '.etree'
 
 - module-name: 'lxml.objectify' # checksum: c4e92339
   implicit-imports:
     - depends:
         - 'lxml.etree'
 
+- module-name: 'magic' # checksum: 803cd877
+  data-files:
+    dirs:
+      - 'libmagic'
+    patterns:
+      - 'magic.mgc'
+
+  dlls:
+    - from_filenames:
+        relative_path: 'libmagic'
+        prefixes:
+          - 'libmagic'
+
 - module-name: 'markdown' # checksum: 827a8bc8
   implicit-imports:
     - depends:
         - 'markdown.extensions.*'
 
 - module-name: 'matplotlib' # checksum: 977975bb
   anti-bloat:
@@ -2294,15 +2313,15 @@
       when: 'not use_pytest'
 
 - module-name: 'nose.core' # checksum: 8247f58b
   data-files:
     patterns:
       - 'usage.txt'
 
-- module-name: 'numba' # checksum: a42885e3
+- module-name: 'numba' # checksum: 9bea0dec
   parameters:
     - 'name': 'disable-jit'
       'values': 'value in ("yes", "no")'
   anti-bloat:
     - description: 'remove numba testing reference'
       change_function:
         'test': 'un-callable'
@@ -2314,18 +2333,17 @@
       - description: "Numba JIT is disabled by default in standalone mode, make a choice explicit with '--module-parameter=numba-disable-jit=yes|no'"
         support_info: 'parameter'
         when: 'standalone and get_parameter("disable-jit", None) is None'
   import-hacks:
     - force-environment-variables:
         'NUMBA_DISABLE_JIT': '1'
       when: 'get_parameter("disable-jit", "yes" if standalone else "no") == "yes"'
-    - find-dlls-near-module:
-        # Finding libomp from there
-        - 'skimage'
-      when: 'macos'
+    # This is for "numba.np.ufunc.omppool".
+    - acceptable-missing-dlls:
+        - 'libomp'
 
 - module-name: 'numba.core.caching' # checksum: dce4aaa0
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         'from IPython.paths import get_ipython_cache_dir': 'raise ImportError'
         'from IPython.utils.path import get_ipython_cache_dir': 'raise ImportError'
@@ -6390,14 +6408,21 @@
     setup_code: 'import toga.platform'
     declarations:
       'toga_backend_module_name': 'toga.platform.get_platform_factory().__name__'
   anti-bloat:
     - change_function:
         'get_platform_factory': "'importlib.import_module(%r)' % get_variable('toga_backend_module_name')"
 
+- module-name: 'toga_cocoa' # checksum: 34886ad0
+  data-files:
+    dirs:
+      - 'resources'
+    include-metadata:
+      - 'toga-cocoa'
+
 - module-name: 'toga_gtk' # checksum: 1577803b
   data-files:
     dirs:
       - 'resources'
     include-metadata:
       - 'toga-gtk'
```

### Comparing `Nuitka-2.2/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-2.2.1/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-2.2.1/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/reports/CompilationReportReader.py` & `Nuitka-2.2.1/nuitka/reports/CompilationReportReader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-2.2.1/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/reports/Reports.py` & `Nuitka-2.2.1/nuitka/reports/Reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
     python_flavor = getPythonFlavorName()
     python_version = python_version_full_str
     os_name = getOS()
     arch_name = getArchitecture()
 
     if isWin32OrPosixWindows():
-        os_release = getWindowsRelease()
+        os_release = str(getWindowsRelease())
     elif isLinux():
         os_release = "-".join(x for x in getLinuxDistribution() if x)
     elif isMacOS():
         os_release = getMacOSRelease()
     else:
         os_release = "unknown"
```

### Comparing `Nuitka-2.2/nuitka/reports/__init__.py` & `Nuitka-2.2.1/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-2.2.1/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-2.2.1/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-2.2.1/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-2.2.1/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,21 @@
     Args:
         exception_name - (str) name of the built-in exception
 
     Returns:
         ParameterSpec that can be used to evaluate calls of these exceptions.
     """
     if exception_name == "ImportError" and python_version >= 0x300:
+        is_new_import_error = True
+    elif exception_name == "ModuleNotFoundError" and python_version >= 0x360:
+        is_new_import_error = True
+    else:
+        is_new_import_error = False
+
+    if is_new_import_error:
         # This is currently the only known built-in exception that does it, but let's
         # be general, as surely that list is going to expand only.
 
         return BuiltinParameterSpecExceptionsKwOnly(
             exception_name=exception_name, kw_only_args=("name", "path")
         )
     else:
```

### Comparing `Nuitka-2.2/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-2.2.1/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-2.2.1/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-2.2.1/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/HardImportSpecs.py` & `Nuitka-2.2.1/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/ParameterSpecs.py` & `Nuitka-2.2.1/nuitka/specs/ParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/specs/__init__.py` & `Nuitka-2.2.1/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/Basics.py` & `Nuitka-2.2.1/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/__init__.py` & `Nuitka-2.2.1/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/commercial/__init__.py` & `Nuitka-2.2.1/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-2.2.1/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/data_composer/__init__.py` & `Nuitka-2.2.1/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/data_composer/__main__.py` & `Nuitka-2.2.1/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-2.2.1/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/environments/Virtualenv.py` & `Nuitka-2.2.1/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/environments/__init__.py` & `Nuitka-2.2.1/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/general/__init__.py` & `Nuitka-2.2.1/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-2.2.1/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-2.2.1/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/general/find_module/FindModuleCode.py` & `Nuitka-2.2.1/nuitka/tools/general/find_module/FindModuleCode.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/general/find_module/__init__.py` & `Nuitka-2.2.1/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-2.2.1/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-2.2.1/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-2.2.1/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/podman/Podman.py` & `Nuitka-2.2.1/nuitka/tools/podman/Podman.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/podman/__init__.py` & `Nuitka-2.2.1/nuitka/tools/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/podman/__main__.py` & `Nuitka-2.2.1/nuitka/tools/podman/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/profiler/__init__.py` & `Nuitka-2.2.1/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/profiler/__main__.py` & `Nuitka-2.2.1/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-2.2.1/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-2.2.1/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/scanning/__init__.py` & `Nuitka-2.2.1/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-2.2.1/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/specialize/Common.py` & `Nuitka-2.2.1/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-2.2.1/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-2.2.1/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/specialize/__init__.py` & `Nuitka-2.2.1/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/Common.py` & `Nuitka-2.2.1/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/Constructs.py` & `Nuitka-2.2.1/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/OutputComparison.py` & `Nuitka-2.2.1/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/Pythons.py` & `Nuitka-2.2.1/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-2.2.1/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/SearchModes.py` & `Nuitka-2.2.1/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/Valgrind.py` & `Nuitka-2.2.1/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/__init__.py` & `Nuitka-2.2.1/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-2.2.1/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-2.2.1/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-2.2.1/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-2.2.1/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-2.2.1/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-2.2.1/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-2.2.1/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-2.2.1/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-2.2.1/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-2.2.1/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/watch/GitHub.py` & `Nuitka-2.2.1/nuitka/tools/watch/GitHub.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/watch/__init__.py` & `Nuitka-2.2.1/nuitka/tools/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tools/watch/__main__.py` & `Nuitka-2.2.1/nuitka/tools/watch/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/Building.py` & `Nuitka-2.2.1/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-2.2.1/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/Extractions.py` & `Nuitka-2.2.1/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/InternalModule.py` & `Nuitka-2.2.1/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/Operations.py` & `Nuitka-2.2.1/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationClasses.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationClasses3.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationMultidist.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-2.2.1/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/SourceHandling.py` & `Nuitka-2.2.1/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/SyntaxErrors.py` & `Nuitka-2.2.1/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/TreeHelpers.py` & `Nuitka-2.2.1/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/VariableClosure.py` & `Nuitka-2.2.1/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/tree/__init__.py` & `Nuitka-2.2.1/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/AppDirs.py` & `Nuitka-2.2.1/nuitka/utils/AppDirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/CStrings.py` & `Nuitka-2.2.1/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/CommandLineOptions.py` & `Nuitka-2.2.1/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Distributions.py` & `Nuitka-2.2.1/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Download.py` & `Nuitka-2.2.1/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Execution.py` & `Nuitka-2.2.1/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/FileOperations.py` & `Nuitka-2.2.1/nuitka/utils/FileOperations.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,19 @@
         This also is thread safe on Windows, i.e. no race is
         possible.
 
     """
 
     with withFileLock("creating directory %s" % path):
         if not os.path.isdir(path):
-            os.makedirs(path)
+            try:
+                os.makedirs(path)
+            except OSError:
+                if not os.path.exists(path):
+                    raise
 
 
 def makeContainingPath(filename):
     target_dir = os.path.dirname(filename)
 
     if not os.path.isdir(target_dir):
         makePath(target_dir)
@@ -487,17 +491,17 @@
 def getDllBasename(path):
     compare_path = os.path.normcase(path)
 
     for suffix in (".dll", ".so", ".dylib"):
         if compare_path.endswith(suffix):
             return path[: -len(suffix)]
 
-    # Linux us not case sensitive, but lets still do it properly,
-    # sometimes, it is done on non-Linux too. So we split on the
-    # normcase, but only to find out what is going on there.
+    # Linux is not case sensitive, but lets still do it properly, sometimes, it
+    # is done macOS too. So we split on the normcase, but only to find out what
+    # is going on there.
     if ".so." in compare_path:
         return path[: len(compare_path.split(".so.")[0])]
 
     return None
 
 
 def listDllFilesFromDirectory(path, prefix=None, suffixes=None):
```

### Comparing `Nuitka-2.2/nuitka/utils/Hashing.py` & `Nuitka-2.2.1/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Images.py` & `Nuitka-2.2.1/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Importing.py` & `Nuitka-2.2.1/nuitka/utils/Importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/InstalledPythons.py` & `Nuitka-2.2.1/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/InstanceCounters.py` & `Nuitka-2.2.1/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Jinja2.py` & `Nuitka-2.2.1/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Json.py` & `Nuitka-2.2.1/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/MacOSApp.py` & `Nuitka-2.2.1/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/MemoryUsage.py` & `Nuitka-2.2.1/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/ModuleNames.py` & `Nuitka-2.2.1/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/ReExecute.py` & `Nuitka-2.2.1/nuitka/utils/ReExecute.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Rest.py` & `Nuitka-2.2.1/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/SharedLibraries.py` & `Nuitka-2.2.1/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Shebang.py` & `Nuitka-2.2.1/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Signing.py` & `Nuitka-2.2.1/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/SlotMetaClasses.py` & `Nuitka-2.2.1/nuitka/utils/SlotMetaClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/StaticLibraries.py` & `Nuitka-2.2.1/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/ThreadedExecutor.py` & `Nuitka-2.2.1/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Timing.py` & `Nuitka-2.2.1/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Utils.py` & `Nuitka-2.2.1/nuitka/utils/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,33 +124,35 @@
     return _linux_distribution_info
 
 
 def getWindowsRelease():
     if not isWin32OrPosixWindows():
         return None
 
-    import ctypes
-
-    class OS_VERSION_INFO_EX(ctypes.Structure):
+    class OsVersionInfoEx(ctypes.Structure):
         _fields_ = [
             ("dwOSVersionInfoSize", ctypes.c_ulong),
             ("dwMajorVersion", ctypes.c_ulong),
             ("dwMinorVersion", ctypes.c_ulong),
             ("dwBuildNumber", ctypes.c_ulong),
             ("dwPlatformId", ctypes.c_ulong),
             ("szCSDVersion", ctypes.c_wchar * 128),
             ("wServicePackMajor", ctypes.c_ushort),
             ("wServicePackMinor", ctypes.c_ushort),
             ("wSuiteMask", ctypes.c_ushort),
             ("wProductType", ctypes.c_byte),
             ("wReserved", ctypes.c_byte),
         ]
 
-    os_version_value = OS_VERSION_INFO_EX()
-    os_version_value.dwOSVersionInfoSize = ctypes.sizeof(os_version_value)
+        def __init__(self):
+            self.dwOSVersionInfoSize = ctypes.sizeof(  # pylint: disable=invalid-name
+                self
+            )
+
+    os_version_value = OsVersionInfoEx()
 
     result = ctypes.windll.ntdll.RtlGetVersion(ctypes.byref(os_version_value))
     if result != 0:
         raiseWindowsError("Failed to get OS version")
 
     version = os_version_value.dwMajorVersion
```

### Comparing `Nuitka-2.2/nuitka/utils/WindowsFileUsage.py` & `Nuitka-2.2.1/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/WindowsResources.py` & `Nuitka-2.2.1/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/Yaml.py` & `Nuitka-2.2.1/nuitka/utils/Yaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/nuitka/utils/__init__.py` & `Nuitka-2.2.1/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/pyproject.toml` & `Nuitka-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/setup.py` & `Nuitka-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/AssertsTest.py` & `Nuitka-2.2.1/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/AssignmentsTest.py` & `Nuitka-2.2.1/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/AssignmentsTest32.py` & `Nuitka-2.2.1/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/BranchingTest.py` & `Nuitka-2.2.1/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/BuiltinOverload.py` & `Nuitka-2.2.1/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/BuiltinSuperTest.py` & `Nuitka-2.2.1/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/BuiltinsTest.py` & `Nuitka-2.2.1/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ClassMinimalTest.py` & `Nuitka-2.2.1/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ClassesTest.py` & `Nuitka-2.2.1/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ClassesTest32.py` & `Nuitka-2.2.1/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ClassesTest34.py` & `Nuitka-2.2.1/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ComparisonChainsTest.py` & `Nuitka-2.2.1/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ConstantsTest.py` & `Nuitka-2.2.1/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ConstantsTest27.py` & `Nuitka-2.2.1/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/DecoratorsTest.py` & `Nuitka-2.2.1/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/DefaultParametersTest.py` & `Nuitka-2.2.1/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/DoubleDeletionsTest.py` & `Nuitka-2.2.1/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/EmptyModuleTest.py` & `Nuitka-2.2.1/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ExceptionRaisingTest.py` & `Nuitka-2.2.1/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-2.2.1/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-2.2.1/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ExecEvalTest.py` & `Nuitka-2.2.1/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ExtremeClosureTest.py` & `Nuitka-2.2.1/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/FunctionObjectsTest.py` & `Nuitka-2.2.1/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/FunctionsTest.py` & `Nuitka-2.2.1/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/FunctionsTest32.py` & `Nuitka-2.2.1/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/FunctionsTest_2.py` & `Nuitka-2.2.1/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/FutureTest32.py` & `Nuitka-2.2.1/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-2.2.1/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-2.2.1/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/GlobalStatementTest.py` & `Nuitka-2.2.1/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/HelloWorldTest_2.py` & `Nuitka-2.2.1/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ImportingTest.py` & `Nuitka-2.2.1/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/InplaceOperationsTest.py` & `Nuitka-2.2.1/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/InspectionTest.py` & `Nuitka-2.2.1/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/InspectionTest_35.py` & `Nuitka-2.2.1/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/InspectionTest_36.py` & `Nuitka-2.2.1/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/LambdasTest.py` & `Nuitka-2.2.1/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-2.2.1/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ListContractionsTest.py` & `Nuitka-2.2.1/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/LoopingTest.py` & `Nuitka-2.2.1/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/MainProgramsTest.py` & `Nuitka-2.2.1/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ModuleAttributesTest.py` & `Nuitka-2.2.1/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/OperatorsTest.py` & `Nuitka-2.2.1/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/OrderChecksTest.py` & `Nuitka-2.2.1/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/OrderChecksTest27.py` & `Nuitka-2.2.1/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-2.2.1/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ParameterErrorsTest.py` & `Nuitka-2.2.1/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ParameterErrorsTest32.py` & `Nuitka-2.2.1/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/PrintFutureTest.py` & `Nuitka-2.2.1/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/PrintingTest_2.py` & `Nuitka-2.2.1/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/RecursionTest.py` & `Nuitka-2.2.1/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ReferencingTest.py` & `Nuitka-2.2.1/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ReferencingTest27.py` & `Nuitka-2.2.1/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ReferencingTest33.py` & `Nuitka-2.2.1/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ReferencingTest35.py` & `Nuitka-2.2.1/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ReferencingTest36.py` & `Nuitka-2.2.1/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ReferencingTest_2.py` & `Nuitka-2.2.1/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/SlotsTest.py` & `Nuitka-2.2.1/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-2.2.1/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-2.2.1/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-2.2.1/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-2.2.1/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TryContinueFinallyTest.py` & `Nuitka-2.2.1/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TryExceptContinueTest.py` & `Nuitka-2.2.1/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TryExceptFinallyTest.py` & `Nuitka-2.2.1/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TryExceptFramesTest.py` & `Nuitka-2.2.1/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TryReturnFinallyTest.py` & `Nuitka-2.2.1/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/TryYieldFinallyTest.py` & `Nuitka-2.2.1/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/UnicodeTest.py` & `Nuitka-2.2.1/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/UnpackingTest35.py` & `Nuitka-2.2.1/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/VarargsTest.py` & `Nuitka-2.2.1/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/WithStatementsTest.py` & `Nuitka-2.2.1/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/YieldFromTest33.py` & `Nuitka-2.2.1/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/run_all.py` & `Nuitka-2.2.1/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/basics/run_xml.py` & `Nuitka-2.2.1/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/onefile/HelloWorldTest.py` & `Nuitka-2.2.1/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-2.2.1/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/onefile/run_all.py` & `Nuitka-2.2.1/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/ArgumentTypes.py` & `Nuitka-2.2.1/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/AttributesTest.py` & `Nuitka-2.2.1/tests/optimizations/AttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/CallsTest.py` & `Nuitka-2.2.1/tests/optimizations/CallsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/ConditionsTest.py` & `Nuitka-2.2.1/tests/optimizations/ConditionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/DecodingOperationsTest.py` & `Nuitka-2.2.1/tests/optimizations/DecodingOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/FormatStringsTest36.py` & `Nuitka-2.2.1/tests/optimizations/FormatStringsTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/HardImportsTest.py` & `Nuitka-2.2.1/tests/optimizations/HardImportsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/HardImportsTest_2.py` & `Nuitka-2.2.1/tests/optimizations/HardImportsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/Iterations.py` & `Nuitka-2.2.1/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/LenTest.py` & `Nuitka-2.2.1/tests/optimizations/LenTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/MatchingTest310.py` & `Nuitka-2.2.1/tests/optimizations/MatchingTest310.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/OperationsTest.py` & `Nuitka-2.2.1/tests/optimizations/OperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/SubscriptsTest.py` & `Nuitka-2.2.1/tests/optimizations/SubscriptsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/optimizations/run_all.py` & `Nuitka-2.2.1/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py` & `Nuitka-2.2.1/tests/packages/package_data_files_embedding/PackageDataFilesEmbedding.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/package_data_files_embedding/__init__.py` & `Nuitka-2.2.1/tests/packages/package_data_files_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-2.2.1/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-2.2.1/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-2.2.1/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/run_all.py` & `Nuitka-2.2.1/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-2.2.1/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-2.2.1/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-2.2.1/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-2.2.1/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-2.2.1/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-2.2.1/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/plugins/code_signing/CodeSigningMain.py` & `Nuitka-2.2.1/tests/plugins/code_signing/CodeSigningMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-2.2.1/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-2.2.1/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/plugins/parameters/ParametersMain.py` & `Nuitka-2.2.1/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-2.2.1/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/plugins/run_all.py` & `Nuitka-2.2.1/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-2.2.1/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-2.2.1/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-2.2.1/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/absolute_import/foobar/local.py` & `Nuitka-2.2.1/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/absolute_import/foobar/util.py` & `Nuitka-2.2.1/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-2.2.1/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-2.2.1/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-2.2.1/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-2.2.1/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-2.2.1/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-2.2.1/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-2.2.1/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-2.2.1/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-2.2.1/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-2.2.1/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-2.2.1/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-2.2.1/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-2.2.1/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-2.2.1/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-2.2.1/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-2.2.1/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-2.2.1/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/dash_import/DashImportMain.py` & `Nuitka-2.2.1/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/dash_import/dash-module.py` & `Nuitka-2.2.1/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/dash_import/plus+module.py` & `Nuitka-2.2.1/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/dash_main/Dash-Main.py` & `Nuitka-2.2.1/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/deep/DeepProgramMain.py` & `Nuitka-2.2.1/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-2.2.1/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-2.2.1/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/deep/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-2.2.1/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-2.2.1/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-2.2.1/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-2.2.1/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-2.2.1/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-2.2.1/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-2.2.1/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-2.2.1/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-2.2.1/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/main_raises/ErrorMain.py` & `Nuitka-2.2.1/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-2.2.1/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-2.2.1/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-2.2.1/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-2.2.1/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-2.2.1/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-2.2.1/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-2.2.1/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-2.2.1/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_exits/Main.py` & `Nuitka-2.2.1/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-2.2.1/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-2.2.1/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-2.2.1/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-2.2.1/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-2.2.1/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-2.2.1/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-2.2.1/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-2.2.1/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-2.2.1/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-2.2.1/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-2.2.1/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_code/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-2.2.1/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_contains_main/__init__.py` & `Nuitka-2.2.1/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_contains_main/local.py` & `Nuitka-2.2.1/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-2.2.1/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-2.2.1/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-2.2.1/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-2.2.1/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-2.2.1/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-2.2.1/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-2.2.1/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-2.2.1/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-2.2.1/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-2.2.1/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_module_collision/something.py` & `Nuitka-2.2.1/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_overload/Main.py` & `Nuitka-2.2.1/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_overload/foo/__init__.py` & `Nuitka-2.2.1/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_overload/foo/bar.py` & `Nuitka-2.2.1/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_overload/foo/bar2.py` & `Nuitka-2.2.1/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-2.2.1/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-2.2.1/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-2.2.1/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-2.2.1/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-2.2.1/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-2.2.1/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-2.2.1/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-2.2.1/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-2.2.1/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-2.2.1/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-2.2.1/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-2.2.1/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/relative_import/dircache.py` & `Nuitka-2.2.1/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-2.2.1/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/run_all.py` & `Nuitka-2.2.1/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-2.2.1/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-2.2.1/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-2.2.1/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-2.2.1/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-2.2.1/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-2.2.1/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-2.2.1/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-2.2.1/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/programs/with space/Space Main.py` & `Nuitka-2.2.1/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/reflected/compile_itself.py` & `Nuitka-2.2.1/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/run-tests` & `Nuitka-2.2.1/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/BrotliUsing.py` & `Nuitka-2.2.1/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/CtypesUsing.py` & `Nuitka-2.2.1/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/DateutilsUsing.py` & `Nuitka-2.2.1/tests/standalone/DateutilsUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/FlaskUsing.py` & `Nuitka-2.2.1/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/GiUsing.py` & `Nuitka-2.2.1/tests/standalone/GiUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/GlfwUsing.py` & `Nuitka-2.2.1/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/GtkUsing.py` & `Nuitka-2.2.1/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/HexEncodingTest_2.py` & `Nuitka-2.2.1/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/IdnaUsing.py` & `Nuitka-2.2.1/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/LxmlUsing.py` & `Nuitka-2.2.1/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/MatplotlibUsing.py` & `Nuitka-2.2.1/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-2.2.1/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/NumpyUsing.py` & `Nuitka-2.2.1/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/OpenGLUsing.py` & `Nuitka-2.2.1/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PandasUsing.py` & `Nuitka-2.2.1/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PasslibUsing.py` & `Nuitka-2.2.1/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PendulumUsing.py` & `Nuitka-2.2.1/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-2.2.1/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PmwUsing.py` & `Nuitka-2.2.1/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PyQt5Plugins.py` & `Nuitka-2.2.1/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-2.2.1/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PyQt5Using.py` & `Nuitka-2.2.1/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PyQt6Plugins.py` & `Nuitka-2.2.1/tests/standalone/PyQt6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PyQt6Using.py` & `Nuitka-2.2.1/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PySide2Using.py` & `Nuitka-2.2.1/tests/standalone/PySide2Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PySide6Plugins.py` & `Nuitka-2.2.1/tests/standalone/PySide6Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/PySide6Using.py` & `Nuitka-2.2.1/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/RsaUsing.py` & `Nuitka-2.2.1/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/SetuptoolsUsing_311.py` & `Nuitka-2.2.1/tests/standalone/SetuptoolsUsing_311.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/ShlibUsing.py` & `Nuitka-2.2.1/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/SocketUsing.py` & `Nuitka-2.2.1/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/TkInterUsing.py` & `Nuitka-2.2.1/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/Urllib3Using.py` & `Nuitka-2.2.1/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/Win32ComUsing.py` & `Nuitka-2.2.1/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/run_all.py` & `Nuitka-2.2.1/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-2.2.1/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/AsyncgenReturn36.py` & `Nuitka-2.2.1/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/AwaitInModule36.py` & `Nuitka-2.2.1/tests/syntax/AwaitInModule36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/BreakWithoutLoop.py` & `Nuitka-2.2.1/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/ClassReturn.py` & `Nuitka-2.2.1/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/ClosureDel_2.py` & `Nuitka-2.2.1/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-2.2.1/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/DuplicateArgument.py` & `Nuitka-2.2.1/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/ExecWithNesting_2.py` & `Nuitka-2.2.1/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/FutureBraces.py` & `Nuitka-2.2.1/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/FutureUnknown.py` & `Nuitka-2.2.1/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/GeneratorExpressions38.py` & `Nuitka-2.2.1/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/GeneratorReturn_2.py` & `Nuitka-2.2.1/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/GlobalForParameter.py` & `Nuitka-2.2.1/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/Importing32.py` & `Nuitka-2.2.1/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/IndentationError.py` & `Nuitka-2.2.1/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/LateFutureImport.py` & `Nuitka-2.2.1/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/MisplacedFutureImport.py` & `Nuitka-2.2.1/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/ModuleReturn.py` & `Nuitka-2.2.1/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-2.2.1/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/NonlocalForParameter32.py` & `Nuitka-2.2.1/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/NonlocalNotFound32.py` & `Nuitka-2.2.1/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/StarImportExtra.py` & `Nuitka-2.2.1/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/SyntaxError.py` & `Nuitka-2.2.1/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-2.2.1/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-2.2.1/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/UnpackNoTuple.py` & `Nuitka-2.2.1/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/UnpackTwoStars32.py` & `Nuitka-2.2.1/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/YieldFromInModule.py` & `Nuitka-2.2.1/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/YieldInAsync35.py` & `Nuitka-2.2.1/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/YieldInGenexp38.py` & `Nuitka-2.2.1/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/YieldInModule.py` & `Nuitka-2.2.1/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-2.2/tests/syntax/run_all.py` & `Nuitka-2.2.1/tests/syntax/run_all.py`

 * *Files identical despite different names*

