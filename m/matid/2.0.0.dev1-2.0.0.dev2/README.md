# Comparing `tmp/matid-2.0.0.dev1.tar.gz` & `tmp/matid-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matid-2.0.0.dev1.tar", last modified: Tue Jan 16 17:51:54 2024, max compression
+gzip compressed data, was "matid-2.0.0.dev2.tar", last modified: Wed Jan 17 08:52:55 2024, max compression
```

## Comparing `matid-2.0.0.dev1.tar` & `matid-2.0.0.dev2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.796791 matid-2.0.0.dev1/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11343 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/LICENSE
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       67 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/MANIFEST.in
--rw-r--r--   0 lauri     (1000) lauri     (1000)    16692 2024-01-16 17:51:54.796791 matid-2.0.0.dev1/PKG-INFO
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2486 2024-01-15 08:19:34.000000 matid-2.0.0.dev1/README.md
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.788791 matid-2.0.0.dev1/matid/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      206 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/__init__.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.788791 matid-2.0.0.dev1/matid/classification/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      106 2024-01-15 08:19:34.000000 matid-2.0.0.dev1/matid/classification/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2298 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/classification/classifications.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15443 2024-01-16 10:48:40.000000 matid-2.0.0.dev1/matid/classification/classifier.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.788791 matid-2.0.0.dev1/matid/clustering/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       82 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/clustering/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3498 2024-01-15 08:19:34.000000 matid-2.0.0.dev1/matid/clustering/cluster.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13673 2024-01-16 17:25:40.000000 matid-2.0.0.dev1/matid/clustering/sbc.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.788791 matid-2.0.0.dev1/matid/core/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       53 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/core/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      591 2023-12-05 14:26:09.000000 matid-2.0.0.dev1/matid/core/distances.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4824 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/core/lattice.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22707 2024-01-15 11:02:15.000000 matid-2.0.0.dev1/matid/core/linkedunits.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    69417 2024-01-16 10:48:40.000000 matid-2.0.0.dev1/matid/core/periodicfinder.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4263 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/core/system.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.792791 matid-2.0.0.dev1/matid/data/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        0 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/data/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      367 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/data/alphabet_data.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1064 2024-01-16 10:48:40.000000 matid-2.0.0.dev1/matid/data/constants.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6897 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/data/element_data.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)  2178977 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/data/symmetry_data.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.792791 matid-2.0.0.dev1/matid/ext/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10579 2024-01-16 10:48:40.000000 matid-2.0.0.dev1/matid/ext/celllist.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2525 2024-01-16 10:48:40.000000 matid-2.0.0.dev1/matid/ext/ext.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8874 2024-01-16 17:24:05.000000 matid-2.0.0.dev1/matid/ext/geometry.cpp
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.792791 matid-2.0.0.dev1/matid/geometry/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/geometry/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    56847 2024-01-16 14:03:56.000000 matid-2.0.0.dev1/matid/geometry/geometry.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.792791 matid-2.0.0.dev1/matid/symmetry/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      110 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/symmetry/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    56455 2024-01-16 10:48:40.000000 matid-2.0.0.dev1/matid/symmetry/symmetryanalyzer.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3257 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/symmetry/wyckoffset.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.792791 matid-2.0.0.dev1/matid/utils/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        0 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/utils/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      367 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/exceptions.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      412 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/matid/utils/segfault_protect.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1456 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/surfacegenerator.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.792791 matid-2.0.0.dev1/matid/utils/symmetry_info_generation/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2679 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/symmetry_info_generation/generate_symmetry_info.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2462 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_continuous_translations.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1070 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_conventional_transform_info.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6607 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_normalizers.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2431 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_space_group_info.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12675 2024-01-12 12:30:51.000000 matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_wyckoff_sets.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-16 17:51:54.792791 matid-2.0.0.dev1/matid.egg-info/
--rw-r--r--   0 lauri     (1000) lauri     (1000)    16692 2024-01-16 17:51:54.000000 matid-2.0.0.dev1/matid.egg-info/PKG-INFO
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1406 2024-01-16 17:51:54.000000 matid-2.0.0.dev1/matid.egg-info/SOURCES.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2024-01-16 17:51:54.000000 matid-2.0.0.dev1/matid.egg-info/dependency_links.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      102 2024-01-16 17:51:54.000000 matid-2.0.0.dev1/matid.egg-info/requires.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        6 2024-01-16 17:51:54.000000 matid-2.0.0.dev1/matid.egg-info/top_level.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1327 2024-01-16 17:25:51.000000 matid-2.0.0.dev1/pyproject.toml
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        2 2023-07-19 17:38:58.000000 matid-2.0.0.dev1/requirements.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2024-01-16 17:51:54.796791 matid-2.0.0.dev1/setup.cfg
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1987 2024-01-15 08:19:42.000000 matid-2.0.0.dev1/setup.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.698625 matid-2.0.0.dev2/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11343 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/LICENSE
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       67 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/MANIFEST.in
+-rw-r--r--   0 lauri     (1000) lauri     (1000)    16692 2024-01-17 08:52:55.698625 matid-2.0.0.dev2/PKG-INFO
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2486 2024-01-16 18:46:11.000000 matid-2.0.0.dev2/README.md
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.682625 matid-2.0.0.dev2/matid/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      206 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.686625 matid-2.0.0.dev2/matid/classification/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      106 2024-01-16 18:46:11.000000 matid-2.0.0.dev2/matid/classification/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2298 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/classification/classifications.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15443 2024-01-16 10:48:40.000000 matid-2.0.0.dev2/matid/classification/classifier.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.686625 matid-2.0.0.dev2/matid/clustering/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       82 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/clustering/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3498 2024-01-16 18:46:11.000000 matid-2.0.0.dev2/matid/clustering/cluster.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13673 2024-01-17 07:19:22.000000 matid-2.0.0.dev2/matid/clustering/sbc.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.686625 matid-2.0.0.dev2/matid/core/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       53 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/core/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      591 2023-12-05 14:26:09.000000 matid-2.0.0.dev2/matid/core/distances.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4824 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/core/lattice.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22707 2024-01-15 11:02:15.000000 matid-2.0.0.dev2/matid/core/linkedunits.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    69233 2024-01-17 08:13:19.000000 matid-2.0.0.dev2/matid/core/periodicfinder.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4263 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/core/system.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.686625 matid-2.0.0.dev2/matid/data/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        0 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/data/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      367 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/data/alphabet_data.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1064 2024-01-16 10:48:40.000000 matid-2.0.0.dev2/matid/data/constants.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6897 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/data/element_data.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)  2178977 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/data/symmetry_data.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.694625 matid-2.0.0.dev2/matid/ext/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10579 2024-01-16 10:48:40.000000 matid-2.0.0.dev2/matid/ext/celllist.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2525 2024-01-16 10:48:40.000000 matid-2.0.0.dev2/matid/ext/ext.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8874 2024-01-16 17:24:05.000000 matid-2.0.0.dev2/matid/ext/geometry.cpp
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.694625 matid-2.0.0.dev2/matid/geometry/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/geometry/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    56847 2024-01-17 06:25:22.000000 matid-2.0.0.dev2/matid/geometry/geometry.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.694625 matid-2.0.0.dev2/matid/symmetry/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      110 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/symmetry/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    56455 2024-01-16 10:48:40.000000 matid-2.0.0.dev2/matid/symmetry/symmetryanalyzer.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3257 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/symmetry/wyckoffset.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.694625 matid-2.0.0.dev2/matid/utils/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        0 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/utils/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      367 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/exceptions.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      412 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/matid/utils/segfault_protect.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1456 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/surfacegenerator.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.698625 matid-2.0.0.dev2/matid/utils/symmetry_info_generation/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2679 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/symmetry_info_generation/generate_symmetry_info.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2462 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_continuous_translations.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1070 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_conventional_transform_info.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6607 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_normalizers.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2431 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_space_group_info.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12675 2024-01-12 12:30:51.000000 matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_wyckoff_sets.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2024-01-17 08:52:55.698625 matid-2.0.0.dev2/matid.egg-info/
+-rw-r--r--   0 lauri     (1000) lauri     (1000)    16692 2024-01-17 08:52:55.000000 matid-2.0.0.dev2/matid.egg-info/PKG-INFO
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1406 2024-01-17 08:52:55.000000 matid-2.0.0.dev2/matid.egg-info/SOURCES.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2024-01-17 08:52:55.000000 matid-2.0.0.dev2/matid.egg-info/dependency_links.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      102 2024-01-17 08:52:55.000000 matid-2.0.0.dev2/matid.egg-info/requires.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        6 2024-01-17 08:52:55.000000 matid-2.0.0.dev2/matid.egg-info/top_level.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1327 2024-01-17 08:17:08.000000 matid-2.0.0.dev2/pyproject.toml
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        2 2023-07-19 17:38:58.000000 matid-2.0.0.dev2/requirements.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2024-01-17 08:52:55.698625 matid-2.0.0.dev2/setup.cfg
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1987 2024-01-15 08:19:42.000000 matid-2.0.0.dev2/setup.py
```

### Comparing `matid-2.0.0.dev1/LICENSE` & `matid-2.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/PKG-INFO` & `matid-2.0.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matid
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: MatID is a Python package for identifying and analyzing atomistic systems based on their structure.
 Author: Lauri Himanen
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `matid-2.0.0.dev1/README.md` & `matid-2.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/classification/classifications.py` & `matid-2.0.0.dev2/matid/classification/classifications.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/classification/classifier.py` & `matid-2.0.0.dev2/matid/classification/classifier.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/clustering/cluster.py` & `matid-2.0.0.dev2/matid/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/clustering/sbc.py` & `matid-2.0.0.dev2/matid/clustering/sbc.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/core/distances.py` & `matid-2.0.0.dev2/matid/core/distances.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/core/lattice.py` & `matid-2.0.0.dev2/matid/core/lattice.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/core/linkedunits.py` & `matid-2.0.0.dev2/matid/core/linkedunits.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/core/periodicfinder.py` & `matid-2.0.0.dev2/matid/core/periodicfinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,22 @@
         overlap_threshold,
         pos_tol,
     ):
         """Used to find the best candidate for a unit cell basis that could
         generate a periodic region in the structure.
 
         Args:
+            system(ase.Atoms):
+            seed_index(int):
+            possible_spans(np.ndarray):
+            neighbour_mask(np.ndarray):
+            neighbour_factors(np.ndarray):
+            bond_threshold(float):
+            overlap_threshold(float):
+            pos_tol(float):
 
         Returns:
             ase.Atoms: A system representing the best cell that was found
             np.ndarray: Position of the seed atom in the cell
         """
         positions = system.get_positions()
         numbers = system.get_atomic_numbers()
@@ -284,17 +292,17 @@
                         ].append((i_sub, tuple(dest_factor)))
 
             metric[i_span] = n_metric
             adjacency_lists.append(i_adj_list)
             adjacency_lists_add.append(i_adj_list_add)
             adjacency_lists_sub.append(i_adj_list_sub)
 
-        # Get the spans that come from the original cell basis if they are
-        # smaller than the maximum cell size.
-        periodic_spans = system.get_cell()
+        # The lattice vectors are added as possible spans if they are set as
+        # periodic and they are shorter than the maximum cell size
+        periodic_spans = system.get_cell()[system.get_pbc()]
         periodic_span_lengths = np.linalg.norm(periodic_spans, axis=1)
         periodic_filter = periodic_span_lengths <= self.max_cell_size
         n_periodic_spans = periodic_filter.sum()
         if n_periodic_spans != 0:
             for i_per_span, per_span in enumerate(periodic_spans):
                 if periodic_filter[i_per_span]:
                     # Add the basis to the spans and add a full metric score
@@ -365,17 +373,15 @@
             best_adjacency_lists_add.append(i_adjacency_list_add)
             best_adjacency_lists_sub.append(i_adjacency_list_sub)
 
         # Get graphs for each atom in the prototype cell
         seed_nodes, seed_group_index, group_data_pbc = self._find_graphs(
             seed_index,
             numbers,
-            dim,
             best_adjacency_lists,
-            neighbour_nodes,
             neighbour_indices,
             neighbour_factors,
         )
 
         # If the seed atom is not in a valid graph, no region could be found.
         if seed_group_index is None:
             return None, None, None
@@ -521,17 +527,15 @@
 
         return proto_cell, offset, n_spans
 
     def _find_graphs(
         self,
         seed_index,
         numbers,
-        dim,
         best_adjacency_lists,
-        neighbour_nodes,
         neighbour_indices,
         neighbour_factors,
     ):
         """
         Creates graphs for each atom that is contained in the prototype cell.
         These graphs represent the connectivity of the atom to other atom in the
         neighbourhood using the best basis spans.
@@ -1271,15 +1275,14 @@
         for number in atomic_number_set:
             number_indices = np.where(atomic_numbers == number)[0]
             number_to_index_map[number] = number_indices
             number_to_pos_map[number] = positions[number_indices]
 
         searched_cell_indices = set()
         used_indices = set()
-        used_seed_indices = set()
         searched_vacancy_positions = []
         queue = deque()
         collection = LinkedUnitCollection(
             system,
             unit_cell,
             is_2d,
             self.dist_matrix_radii_mic,
@@ -1290,29 +1293,25 @@
         )
         multipliers = self._get_multipliers(periodic_indices)
 
         # Start off the queue
         self._find_region_rec(
             system,
             collection,
-            number_to_index_map,
-            number_to_pos_map,
             seed_index,
             seed_pos,
             seed_number,
             unit_cell,
             seed_position,
             searched_cell_indices,
             (0, 0, 0),
             used_indices,
             searched_vacancy_positions,
-            periodic_indices,
             queue,
             multipliers,
-            used_seed_indices,
         )
 
         # Keep searching while new cells are found
         finished = False
         while not finished:
             try:
                 (
@@ -1323,29 +1322,25 @@
                 ) = queue.popleft()
             except IndexError:
                 finished = True
             else:
                 self._find_region_rec(
                     system,
                     collection,
-                    number_to_index_map,
-                    number_to_pos_map,
                     queue_seed_index,
                     queue_seed_pos,
                     seed_number,
                     queue_cell,
                     seed_position,
                     searched_cell_indices,
                     queue_index,
                     used_indices,
                     searched_vacancy_positions,
-                    periodic_indices,
                     queue,
                     multipliers,
-                    used_seed_indices,
                 )
 
         return collection
 
     def _get_multipliers(self, periodic_indices):
         """Used to calculate the multipliers that are used to multiply the cell
         basis vectors to find new unit cells.
@@ -1359,29 +1354,25 @@
 
         return multipliers
 
     def _find_region_rec(
         self,
         system,
         collection,
-        number_to_index_map,
-        number_to_pos_map,
         seed_index,
         seed_pos,
         seed_atomic_number,
         unit_cell,
         seed_offset,
         searched_cell_indices,
         cell_index,
         used_indices,
         searched_vacancy_positions,
-        periodic_indices,
         queue,
         multipliers,
-        used_seed_indices,
     ):
         """
         Args:
             system(ASE.Atoms): The original system from which the periodic
                 region is searched.
             collection(LinkedUnitCollection): Container for LinkedUnits that
                 belong to a found region.
```

### Comparing `matid-2.0.0.dev1/matid/core/system.py` & `matid-2.0.0.dev2/matid/core/system.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/data/constants.py` & `matid-2.0.0.dev2/matid/data/constants.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/data/element_data.py` & `matid-2.0.0.dev2/matid/data/element_data.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/data/symmetry_data.py` & `matid-2.0.0.dev2/matid/data/symmetry_data.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/ext/celllist.cpp` & `matid-2.0.0.dev2/matid/ext/celllist.cpp`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/ext/ext.cpp` & `matid-2.0.0.dev2/matid/ext/ext.cpp`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/ext/geometry.cpp` & `matid-2.0.0.dev2/matid/ext/geometry.cpp`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/geometry/geometry.py` & `matid-2.0.0.dev2/matid/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/symmetry/symmetryanalyzer.py` & `matid-2.0.0.dev2/matid/symmetry/symmetryanalyzer.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/symmetry/wyckoffset.py` & `matid-2.0.0.dev2/matid/symmetry/wyckoffset.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/utils/surfacegenerator.py` & `matid-2.0.0.dev2/matid/utils/surfacegenerator.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/utils/symmetry_info_generation/generate_symmetry_info.py` & `matid-2.0.0.dev2/matid/utils/symmetry_info_generation/generate_symmetry_info.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_continuous_translations.py` & `matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_continuous_translations.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_conventional_transform_info.py` & `matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_conventional_transform_info.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_normalizers.py` & `matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_normalizers.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_space_group_info.py` & `matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_space_group_info.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid/utils/symmetry_info_generation/query_wyckoff_sets.py` & `matid-2.0.0.dev2/matid/utils/symmetry_info_generation/query_wyckoff_sets.py`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/matid.egg-info/PKG-INFO` & `matid-2.0.0.dev2/matid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matid
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: MatID is a Python package for identifying and analyzing atomistic systems based on their structure.
 Author: Lauri Himanen
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `matid-2.0.0.dev1/matid.egg-info/SOURCES.txt` & `matid-2.0.0.dev2/matid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matid-2.0.0.dev1/pyproject.toml` & `matid-2.0.0.dev2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "pybind11~=2.11.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'matid'
-version = '2.0.0.dev1'
+version = '2.0.0.dev2'
 description = 'MatID is a Python package for identifying and analyzing atomistic systems based on their structure.'
 readme = "README.md"
 authors = [{ name = "Lauri Himanen" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
```

### Comparing `matid-2.0.0.dev1/setup.py` & `matid-2.0.0.dev2/setup.py`

 * *Files identical despite different names*

