# Comparing `tmp/medspacy_quickumls-3.1a0.tar.gz` & `tmp/medspacy_quickumls-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspacy_quickumls-3.1a0.tar", last modified: Fri Mar 29 17:09:08 2024, max compression
+gzip compressed data, was "medspacy_quickumls-3.2.tar", last modified: Tue May 14 15:17:26 2024, max compression
```

## Comparing `medspacy_quickumls-3.1a0.tar` & `medspacy_quickumls-3.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.674127 medspacy_quickumls-3.1a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-03-29 17:09:08.674127 medspacy_quickumls-3.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.674127 medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-03-29 17:09:08.000000 medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-03-29 17:09:08.000000 medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 17:09:08.000000 medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-29 17:09:08.000000 medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 17:09:08.000000 medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.650128 medspacy_quickumls-3.1a0/quickumls/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/about.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18178 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10915 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/spacy_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/quickumls/umls_match.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.642127 medspacy_quickumls-3.1a0/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.646127 medspacy_quickumls-3.1a0/resources/quickumls/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.662127 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.662127 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.670127 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.670127 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.670127 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.674127 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-29 17:09:08.678128 medspacy_quickumls-3.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:08.662127 medspacy_quickumls-3.1a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/init_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/skiptest_spangroup1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/skiptest_spangroup2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/test_quickumls_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/test_quickumls_component2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-29 17:09:04.000000 medspacy_quickumls-3.1a0/tests/test_quickumls_spangroup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.376306 medspacy_quickumls-3.2/
+-rw-rw-rw-   0        0        0     1124 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       43 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9835 2024-05-14 15:17:26.376306 medspacy_quickumls-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8972 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.314758 medspacy_quickumls-3.2/medspacy_quickumls.egg-info/
+-rw-rw-rw-   0        0        0     9835 2024-05-14 15:17:26.000000 medspacy_quickumls-3.2/medspacy_quickumls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    15228 2024-05-14 15:17:26.000000 medspacy_quickumls-3.2/medspacy_quickumls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:17:26.000000 medspacy_quickumls-3.2/medspacy_quickumls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-05-14 15:17:26.000000 medspacy_quickumls-3.2/medspacy_quickumls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 15:17:26.000000 medspacy_quickumls-3.2/medspacy_quickumls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.321764 medspacy_quickumls-3.2/quickumls/
+-rw-rw-rw-   0        0        0       93 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/quickumls/__init__.py
+-rw-rw-rw-   0        0        0      657 2024-05-14 15:09:21.000000 medspacy_quickumls-3.2/quickumls/about.py
+-rw-rw-rw-   0        0        0      296 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/quickumls/client.py
+-rw-rw-rw-   0        0        0    13835 2024-05-14 15:08:27.000000 medspacy_quickumls-3.2/quickumls/constants.py
+-rw-rw-rw-   0        0        0    18659 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/quickumls/core.py
+-rw-rw-rw-   0        0        0     7342 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/quickumls/install.py
+-rw-rw-rw-   0        0        0     7558 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/quickumls/network.py
+-rw-rw-rw-   0        0        0     2731 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/quickumls/server.py
+-rw-rw-rw-   0        0        0    11134 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/quickumls/spacy_component.py
+-rw-rw-rw-   0        0        0     8565 2023-05-05 16:48:11.000000 medspacy_quickumls-3.2/quickumls/toolbox.py
+-rw-rw-rw-   0        0        0     1185 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/quickumls/umls_match.py
+-rw-rw-rw-   0        0        0      110 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.291935 medspacy_quickumls-3.2/resources/
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.293114 medspacy_quickumls-3.2/resources/quickumls/
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.324764 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.325764 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    12288 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.342567 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     6116 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6892 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2788 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2664 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2744 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     3016 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2904 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     3140 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3228 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3460 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     3148 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     7344 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3224 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4984 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     5152 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     5024 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3384 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3824 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3544 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     4064 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3624 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     5160 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3788 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     5368 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2384 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.345561 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.346699 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    20480 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.362710 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     2912 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6162 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2540 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2574 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2642 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     2884 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2778 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     2990 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3066 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3262 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     2984 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     5574 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3050 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4526 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     3546 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     4616 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3186 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3576 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3322 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     3780 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3390 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     4696 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3528 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     4828 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2336 2022-12-22 17:44:22.000000 medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+-rw-rw-rw-   0        0        0       85 2024-05-14 15:17:26.381313 medspacy_quickumls-3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2395 2023-05-05 16:17:09.000000 medspacy_quickumls-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:17:26.367782 medspacy_quickumls-3.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     1400 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/tests/init_db.py
+-rw-rw-rw-   0        0        0     1512 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/tests/skiptest_spangroup1.py
+-rw-rw-rw-   0        0        0     1364 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/tests/skiptest_spangroup2.py
+-rw-rw-rw-   0        0        0     1149 2023-05-05 16:48:11.000000 medspacy_quickumls-3.2/tests/test_basic.py
+-rw-rw-rw-   0        0        0     2274 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/tests/test_quickumls_component.py
+-rw-rw-rw-   0        0        0     1364 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/tests/test_quickumls_component2.py
+-rw-rw-rw-   0        0        0     1734 2024-05-10 21:30:30.000000 medspacy_quickumls-3.2/tests/test_quickumls_spangroup.py
```

### Comparing `medspacy_quickumls-3.1a0/PKG-INFO` & `medspacy_quickumls-3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,145 +1,140 @@
-Metadata-Version: 2.1
-Name: medspacy_quickumls
-Version: 3.1a0
-Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
-Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
-Author: Luca Soldaini, modified by Kelly Peterson and Jianlin Shi
-Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy>=1.8.2
-Requires-Dist: spacy>=3.1.3
-Requires-Dist: unidecode>=0.4.19
-Requires-Dist: nltk>=3.3
-Requires-Dist: pysimstring
-Requires-Dist: medspacy_unqlite>=0.8.1
-Requires-Dist: pytest>=6
-Requires-Dist: six
-
-[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
-
-[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
-
-# QuickUMLS
-
-QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
-It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
-For more details on how QuickUMLS works, we remand to our paper.
-
-This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
-
-## Installation
-
-1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
-2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
-3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
-    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
-    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
-    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
-    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
-
-
-## APIs
-
-A QuickUMLS object can be instantiated as follows:
-
-```python
-from quickumls import QuickUMLS
-
-matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
-                    similarity_name, window, accepted_semtypes)
-```
-
-Where:
-
-- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
-- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
-- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
-- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
-- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
-- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
-
-To use the matcher, simply call
-
-```python
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
-
-If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
-
-## spaCy pipeline component
-
-QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
-
-Adding QuickUMLS as a component in a pipeline can be done as follows:
-
-```python
-from quickumls.spacy_component import SpacyQuickUMLS
-
-# common English pipeline
-nlp = spacy.load('en_core_web_sm')
-
-quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
-nlp.add_pipe(quickumls_component)
-
-doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
-
-for ent in doc.ents:
-    print('Entity text : {}'.format(ent.text))
-    print('Label (UMLS CUI) : {}'.format(ent.label_))
-    print('Similarity : {}'.format(ent._.similarity))
-    print('Semtypes : {}'.format(ent._.semtypes))
-```
-
-## Server / Client Support
-
-Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
-
-To start the server, run `python -m quickumls.server`:
-
-```bash
-python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
-```
-
-Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
-
-To load the client, import `get_quickumls_client` from `quickumls`:
-
-```bash
-from quickumls import get_quickumls_client
-matcher = get_quickumls_client()
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-The API of the client is the same of a QuickUMLS object.
-
-
-In case you wish to run the server in the background, you can do so as follows:
-
-```bash
-nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
-
-```
-
-When you are done, don't forget to stop the server by running.
-```bash
-kill -9 `cat nohup.pid`
-rm nohup.pid
-```
-
-## References
-
-- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
-- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
+Metadata-Version: 2.1
+Name: medspacy_quickumls
+Version: 3.2
+Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
+Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
+Author: Luca Soldaini, modified by Kelly Peterson and Jianlin Shi
+Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
+
+## Release Note
+From version 3.1, we start to isolate the unqlite dependency with our pre-compiled version medspacy-unqlite, because compiling from source code can be troublesome in certain environments especially on Government Furnished Equipments. Also, multiple spaCy versions are included in the continuous integration tests. 
+
+[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
+
+# QuickUMLS
+
+QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
+It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
+For more details on how QuickUMLS works, we remand to our paper.
+
+This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
+
+## Installation
+
+1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
+2. **Install QuickUMLS**: You can do so by either running `pip install medspacy-quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>â€ </sup>.
+3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
+    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
+    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
+    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
+    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
+
+
+## APIs
+
+A QuickUMLS object can be instantiated as follows:
+
+```python
+from quickumls import QuickUMLS
+
+matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
+                    similarity_name, window, accepted_semtypes)
+```
+
+Where:
+
+- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
+- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
+- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
+- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
+- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
+- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
+
+To use the matcher, simply call
+
+```python
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
+
+If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
+
+## spaCy pipeline component
+
+QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
+
+Adding QuickUMLS as a component in a pipeline can be done as follows:
+
+```python
+from quickumls.spacy_component import SpacyQuickUMLS
+
+# common English pipeline
+nlp = spacy.load('en_core_web_sm')
+
+quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
+nlp.add_pipe(quickumls_component)
+
+doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
+
+for ent in doc.ents:
+    print('Entity text : {}'.format(ent.text))
+    print('Label (UMLS CUI) : {}'.format(ent.label_))
+    print('Similarity : {}'.format(ent._.similarity))
+    print('Semtypes : {}'.format(ent._.semtypes))
+```
+
+## Server / Client Support
+
+Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
+
+To start the server, run `python -m quickumls.server`:
+
+```bash
+python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
+```
+
+Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
+
+To load the client, import `get_quickumls_client` from `quickumls`:
+
+```bash
+from quickumls import get_quickumls_client
+matcher = get_quickumls_client()
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+The API of the client is the same of a QuickUMLS object.
+
+
+In case you wish to run the server in the background, you can do so as follows:
+
+```bash
+nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
+
+```
+
+When you are done, don't forget to stop the server by running.
+```bash
+kill -9 `cat nohup.pid`
+rm nohup.pid
+```
+
+## References
+
+- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
+- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
```

### Comparing `medspacy_quickumls-3.1a0/README.md` & `medspacy_quickumls-3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,119 +1,122 @@
-[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
-
-[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
-
-# QuickUMLS
-
-QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
-It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
-For more details on how QuickUMLS works, we remand to our paper.
-
-This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
-
-## Installation
-
-1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
-2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
-3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
-    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
-    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
-    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
-    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
-
-
-## APIs
-
-A QuickUMLS object can be instantiated as follows:
-
-```python
-from quickumls import QuickUMLS
-
-matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
-                    similarity_name, window, accepted_semtypes)
-```
-
-Where:
-
-- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
-- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
-- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
-- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
-- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
-- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
-
-To use the matcher, simply call
-
-```python
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
-
-If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
-
-## spaCy pipeline component
-
-QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
-
-Adding QuickUMLS as a component in a pipeline can be done as follows:
-
-```python
-from quickumls.spacy_component import SpacyQuickUMLS
-
-# common English pipeline
-nlp = spacy.load('en_core_web_sm')
-
-quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
-nlp.add_pipe(quickumls_component)
-
-doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
-
-for ent in doc.ents:
-    print('Entity text : {}'.format(ent.text))
-    print('Label (UMLS CUI) : {}'.format(ent.label_))
-    print('Similarity : {}'.format(ent._.similarity))
-    print('Semtypes : {}'.format(ent._.semtypes))
-```
-
-## Server / Client Support
-
-Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
-
-To start the server, run `python -m quickumls.server`:
-
-```bash
-python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
-```
-
-Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
-
-To load the client, import `get_quickumls_client` from `quickumls`:
-
-```bash
-from quickumls import get_quickumls_client
-matcher = get_quickumls_client()
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-The API of the client is the same of a QuickUMLS object.
-
-
-In case you wish to run the server in the background, you can do so as follows:
-
-```bash
-nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
-
-```
-
-When you are done, don't forget to stop the server by running.
-```bash
-kill -9 `cat nohup.pid`
-rm nohup.pid
-```
-
-## References
-
-- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
-- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
+[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
+
+## Release Note
+From version 3.1, we start to isolate the unqlite dependency with our pre-compiled version medspacy-unqlite, because compiling from source code can be troublesome in certain environments especially on Government Furnished Equipments. Also, multiple spaCy versions are included in the continuous integration tests. 
+
+[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
+
+# QuickUMLS
+
+QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
+It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
+For more details on how QuickUMLS works, we remand to our paper.
+
+This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
+
+## Installation
+
+1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
+2. **Install QuickUMLS**: You can do so by either running `pip install medspacy-quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
+3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
+    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
+    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
+    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
+    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
+
+
+## APIs
+
+A QuickUMLS object can be instantiated as follows:
+
+```python
+from quickumls import QuickUMLS
+
+matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
+                    similarity_name, window, accepted_semtypes)
+```
+
+Where:
+
+- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
+- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
+- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
+- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
+- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
+- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
+
+To use the matcher, simply call
+
+```python
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
+
+If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
+
+## spaCy pipeline component
+
+QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
+
+Adding QuickUMLS as a component in a pipeline can be done as follows:
+
+```python
+from quickumls.spacy_component import SpacyQuickUMLS
+
+# common English pipeline
+nlp = spacy.load('en_core_web_sm')
+
+quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
+nlp.add_pipe(quickumls_component)
+
+doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
+
+for ent in doc.ents:
+    print('Entity text : {}'.format(ent.text))
+    print('Label (UMLS CUI) : {}'.format(ent.label_))
+    print('Similarity : {}'.format(ent._.similarity))
+    print('Semtypes : {}'.format(ent._.semtypes))
+```
+
+## Server / Client Support
+
+Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
+
+To start the server, run `python -m quickumls.server`:
+
+```bash
+python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
+```
+
+Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
+
+To load the client, import `get_quickumls_client` from `quickumls`:
+
+```bash
+from quickumls import get_quickumls_client
+matcher = get_quickumls_client()
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+The API of the client is the same of a QuickUMLS object.
+
+
+In case you wish to run the server in the background, you can do so as follows:
+
+```bash
+nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
+
+```
+
+When you are done, don't forget to stop the server by running.
+```bash
+kill -9 `cat nohup.pid`
+rm nohup.pid
+```
+
+## References
+
+- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
+- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
```

### Comparing `medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/PKG-INFO` & `medspacy_quickumls-3.2/medspacy_quickumls.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,145 +1,140 @@
-Metadata-Version: 2.1
-Name: medspacy_quickumls
-Version: 3.1a0
-Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
-Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
-Author: Luca Soldaini, modified by Kelly Peterson and Jianlin Shi
-Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy>=1.8.2
-Requires-Dist: spacy>=3.1.3
-Requires-Dist: unidecode>=0.4.19
-Requires-Dist: nltk>=3.3
-Requires-Dist: pysimstring
-Requires-Dist: medspacy_unqlite>=0.8.1
-Requires-Dist: pytest>=6
-Requires-Dist: six
-
-[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
-
-[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
-
-# QuickUMLS
-
-QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
-It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
-For more details on how QuickUMLS works, we remand to our paper.
-
-This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
-
-## Installation
-
-1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
-2. **Install QuickUMLS**: You can do so by either running `pip install quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>†</sup>.
-3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
-    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
-    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
-    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
-    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
-
-
-## APIs
-
-A QuickUMLS object can be instantiated as follows:
-
-```python
-from quickumls import QuickUMLS
-
-matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
-                    similarity_name, window, accepted_semtypes)
-```
-
-Where:
-
-- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
-- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
-- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
-- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
-- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
-- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
-
-To use the matcher, simply call
-
-```python
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
-
-If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
-
-## spaCy pipeline component
-
-QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
-
-Adding QuickUMLS as a component in a pipeline can be done as follows:
-
-```python
-from quickumls.spacy_component import SpacyQuickUMLS
-
-# common English pipeline
-nlp = spacy.load('en_core_web_sm')
-
-quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
-nlp.add_pipe(quickumls_component)
-
-doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
-
-for ent in doc.ents:
-    print('Entity text : {}'.format(ent.text))
-    print('Label (UMLS CUI) : {}'.format(ent.label_))
-    print('Similarity : {}'.format(ent._.similarity))
-    print('Semtypes : {}'.format(ent._.semtypes))
-```
-
-## Server / Client Support
-
-Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
-
-To start the server, run `python -m quickumls.server`:
-
-```bash
-python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
-```
-
-Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
-
-To load the client, import `get_quickumls_client` from `quickumls`:
-
-```bash
-from quickumls import get_quickumls_client
-matcher = get_quickumls_client()
-text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
-matcher.match(text, best_match=True, ignore_syntax=False)
-```
-
-The API of the client is the same of a QuickUMLS object.
-
-
-In case you wish to run the server in the background, you can do so as follows:
-
-```bash
-nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
-
-```
-
-When you are done, don't forget to stop the server by running.
-```bash
-kill -9 `cat nohup.pid`
-rm nohup.pid
-```
-
-## References
-
-- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
-- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
+Metadata-Version: 2.1
+Name: medspacy-quickumls
+Version: 3.2
+Summary: QuickUMLS is a tool for fast, unsupervised biomedical concept extraction from medical text
+Home-page: https://github.com/Georgetown-IR-Lab/QuickUMLS
+Author: Luca Soldaini, modified by Kelly Peterson and Jianlin Shi
+Author-email: luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[NOTE: This is an updated fork of QuickUMLS for usage in medspacy to accelerate recent developments from the medspacy team to incorporate QuickUMLS into spacy pipelines.]
+
+## Release Note
+From version 3.1, we start to isolate the unqlite dependency with our pre-compiled version medspacy-unqlite, because compiling from source code can be troublesome in certain environments especially on Government Furnished Equipments. Also, multiple spaCy versions are included in the continuous integration tests. 
+
+[**NEW: v.1.4 supports starting multiple QuickUMLS matchers concurrently!**](https://giphy.com/embed/BlVnrxJgTGsUw) I've finally added support for [unqlite](https://github.com/coleifer/unqlite-python) as an alternative database for storage of CUIs and Semantic Types (see [here](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) for more details). unqlite-backed QuickUMLS installation support multiple matchers running at the same time. Other than better multi-processing support, unqlite should have better support for unicode.
+
+# QuickUMLS
+
+QuickUMLS (Soldaini and Goharian, 2016) is a tool for fast, unsupervised  biomedical concept extraction from medical text.
+It takes advantage of [Simstring](http://www.chokkan.org/software/simstring/) (Okazaki and Tsujii, 2010) for approximate string matching.
+For more details on how QuickUMLS works, we remand to our paper.
+
+This project should be compatible with Python 3 (Python 2 is [no longer supported](https://pythonclock.org/)) and run on any UNIX system (support for Windows is experimental, please report bugs!). **If you find any bugs, please file an issue on GitHub or email the author at luca@ir.cs.georgetown.edu**.
+
+## Installation
+
+1. **Obtain a UMLS installation** This tool requires you to have a valid UMLS installation on disk. To install UMLS, you must first obtain a [license](https://uts.nlm.nih.gov/license.html) from the National Library of Medicine; then you should download all UMLS files from [this page](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html); finally, you can install UMLS using the [MetamorphoSys](https://www.nlm.nih.gov/pubs/factsheets/umlsmetamorph.html) tool as [explained in this guide](https://www.nlm.nih.gov/research/umls/implementation_resources/metamorphosys/help.html).  The installation can be removed once the system has been initialized.
+2. **Install QuickUMLS**: You can do so by either running `pip install medspacy-quickumls` or `python setup.py install`. On macOS, using anaconda is **strongly recommended**<sup>â€ </sup>.
+3. **Create a QuickUMLS installation** Initialize the system by running `python -m quickumls.install <umls_installation_path> <destination_path>`, where `<umls_installation_path>` is where the installation files are (in particular, we need `MRCONSO.RRF` and `MRSTY.RRF`) and `<destination_path>` is the directory where the QuickUmls data files should be installed. This process will take between 5 and 30 minutes depending how fast the CPU and the drive where UMLS and QuickUMLS files are stored are (on a system with a Intel i7 6700K CPU and a 7200 RPM hard drive, initialization takes 8.5 minutes). `python -m quickumls.install` supports the following optional arguments:
+    - `-L` / `--lowercase`: if used, all concept terms are folded to lowercase before being processed. This option typically increases recall, but it might reduce precision;
+    - `-U` / `--normalize-unicode`: if used, expressions with non-ASCII characters are converted to the closest combination of ASCII characters.
+    - `-E` / `--language`: Specify the language to consider for UMLS concepts; by default, English is used. For a complete list of languages, please see [this table provided by NLM](https://www.nlm.nih.gov/research/umls/knowledge_sources/metathesaurus/release/abbreviations.html#LAT).
+    - `-d` / `--database-backend`: Specify which database backend to use for QuickUMLS. The current option is `unqlite`, but it may be expanded in the future. This backend supports multi-process reading and has better unicode compatibility, and it used as default.
+
+
+## APIs
+
+A QuickUMLS object can be instantiated as follows:
+
+```python
+from quickumls import QuickUMLS
+
+matcher = QuickUMLS(quickumls_fp, overlapping_criteria, threshold,
+                    similarity_name, window, accepted_semtypes)
+```
+
+Where:
+
+- `quickumls_fp` is the directory where the QuickUMLS data files are installed.
+- `overlapping_criteria` (optional, default: "score") is the criteria used to deal with overlapping concepts; choose "score" if the matching score of the concepts should be consider first, "length" if the longest should be considered first instead.
+- `threshold` (optional, default: 0.7) is the minimum similarity value between strings.
+- `similarity_name` (optional, default: "jaccard") is the name of similarity to use. Choose between "dice", "jaccard", "cosine", or "overlap".
+- `window` (optional, default: 5) is the maximum number of tokens to consider for matching.
+- `accepted_semtypes` (optional, default: see `constants.py`) is the set of UMLS semantic types concepts should belong to. Semantic types are identified by the letter "T" followed by three numbers (e.g., "T131", which identifies the type *"Hazardous or Poisonous Substance"*). See [here](https://metamap.nlm.nih.gov/Docs/SemanticTypes_2013AA.txt) for the full list.
+
+To use the matcher, simply call
+
+```python
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+Set `best_match` to `False` if you want to return overlapping candidates, `ignore_syntax` to `True` to disable all heuristics introduced in (Soldaini and Goharian, 2016).
+
+If the matcher throws a warning during initialization, read [this page](https://github.com/Georgetown-IR-Lab/QuickUMLS/wiki/Migration-QuickUMLS-1.3-to-1.4) to learn why and how to stop it from doing so.
+
+## spaCy pipeline component
+
+QuickUMLS can be used for standalone processing but it can also be use as a component in a modular spaCy pipeline.  This follows traditional spaCy handling of concepts to be entity objects added to the Document object.  These entity objects contain the CUI, similarity score and Semantic Types in the spacy "underscore" object.  Note that this implementation follows a [known spacy convention](https://github.com/explosion/spaCy/issues/3608) that entity Spans cannot overlap on a single token. To prevent token overlap, matches are ranked according to the `overlapping_criteria` supplied so that overlap of any tokens will be prioritized by this order.
+
+Adding QuickUMLS as a component in a pipeline can be done as follows:
+
+```python
+from quickumls.spacy_component import SpacyQuickUMLS
+
+# common English pipeline
+nlp = spacy.load('en_core_web_sm')
+
+quickumls_component = SpacyQuickUMLS(nlp, 'PATH_TO_QUICKUMLS_DATA')
+nlp.add_pipe(quickumls_component)
+
+doc = nlp('Pt c/o shortness of breath, chest pain, nausea, vomiting, diarrrhea')
+
+for ent in doc.ents:
+    print('Entity text : {}'.format(ent.text))
+    print('Label (UMLS CUI) : {}'.format(ent.label_))
+    print('Similarity : {}'.format(ent._.similarity))
+    print('Semtypes : {}'.format(ent._.semtypes))
+```
+
+## Server / Client Support
+
+Starting with v.1.2, QuickUMLS includes a support for being used in a client-server configuration. That is, you can start one QuickUMLS server, and query it from multiple scripts using a client.
+
+To start the server, run `python -m quickumls.server`:
+
+```bash
+python -m quickumls.server /path/to/quickumls/files {-P QuickUMLS port} {-H QuickUMLS host} {QuickUMLS options}
+```
+
+Host and port are optional; by default, QuickUMLS runs on `localhost:4645`. You can also pass any QuickUMLS option mentioned above to the server. To obtain a list of options for the server, run `python -m quickumls.server -h`.
+
+To load the client, import `get_quickumls_client` from `quickumls`:
+
+```bash
+from quickumls import get_quickumls_client
+matcher = get_quickumls_client()
+text = "The ulna has dislocated posteriorly from the trochlea of the humerus."
+matcher.match(text, best_match=True, ignore_syntax=False)
+```
+
+The API of the client is the same of a QuickUMLS object.
+
+
+In case you wish to run the server in the background, you can do so as follows:
+
+```bash
+nohup python -m quickumls.server /path/to/QuickUMLS {server options} > /dev/null 2>&1 & echo $! > nohup.pid
+
+```
+
+When you are done, don't forget to stop the server by running.
+```bash
+kill -9 `cat nohup.pid`
+rm nohup.pid
+```
+
+## References
+
+- Okazaki, Naoaki, and Jun'ichi Tsujii. "*Simple and efficient algorithm for approximate dictionary matching.*" COLING 2010.
+- Luca Soldaini and Nazli Goharian. "*QuickUMLS: a fast, unsupervised approach for medical concept extraction.*" MedIR Workshop, SIGIR 2016.
```

### Comparing `medspacy_quickumls-3.1a0/medspacy_quickumls.egg-info/SOURCES.txt` & `medspacy_quickumls-3.2/medspacy_quickumls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/quickumls/about.py` & `medspacy_quickumls-3.2/quickumls/about.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# inspired from:
-# https://python-packaging-user-guide.readthedocs.org/en/latest/single_source_version/
-# https://github.com/pypa/warehouse/blob/master/warehouse/__about__.py
-# https://github.com/explosion/spaCy/blob/master/spacy/about.py
-
-__title__ = 'medspacy_quickumls'
-__version__ = '3.1a0'
-__author__ = 'Luca Soldaini, modified by Kelly Peterson and Jianlin Shi'
-__email__ = 'luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu'
-__license__ = 'MIT'
-__uri__ = "https://github.com/medspacy/quickumls"
-__copyright__ = '2014-2020, Georgetown University Information Retrieval Lab, updated 2020-2023, University of Utah'
+# inspired from:
+# https://python-packaging-user-guide.readthedocs.org/en/latest/single_source_version/
+# https://github.com/pypa/warehouse/blob/master/warehouse/__about__.py
+# https://github.com/explosion/spaCy/blob/master/spacy/about.py
+
+__title__ = 'medspacy_quickumls'
+__version__ = '3.2'
+__author__ = 'Luca Soldaini, modified by Kelly Peterson and Jianlin Shi'
+__email__ = 'luca@ir.cs.georgetown.edu,kelly.peterson@hsc.utah.edu,jianlin.shi@hsc.utah.edu'
+__license__ = 'MIT'
+__uri__ = "https://github.com/medspacy/quickumls"
+__copyright__ = '2014-2020, Georgetown University Information Retrieval Lab, updated 2020-2023, University of Utah'
```

### Comparing `medspacy_quickumls-3.1a0/quickumls/constants.py` & `medspacy_quickumls-3.2/quickumls/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,198 +1,199 @@
-MEDSPACY_DEFAULT_SPAN_GROUP_NAME = "medspacy_spans"
-
-HEADERS_MRCONSO = [
-    'cui', 'lat', 'ts', 'lui', 'stt', 'sui', 'ispref', 'aui', 'saui',
-    'scui', 'sdui', 'sab', 'tty', 'code', 'str', 'srl', 'suppress', 'cvf'
-]
-HEADERS_MRSTY = [
-    'cui', 'sty', 'hier' 'desc', 'sid', 'num'
-]
-
-NEGATIONS = {'none', 'non', 'neither', 'nor', 'no', 'not'}
-
-# The following is a list of all existing semtypes along with their name and some examples. 
-# You can easily select the ones you need by commenting out the lines that are not relevant for your application.
-
-ACCEPTED_SEMTYPES = {
-    # 'T020', # Acquired Abnormality, ex.: Hemorrhoids; Hernia, Femoral; Cauliflower ear
-    # 'T052', # Activity, ex.: Expeditions; Information Distribution; Social Planning
-    # 'T100', # Age Group, ex.: Adult; Infant, Premature; Adolescent (age group)
-    # 'T087', # Amino Acid Sequence, ex.: Signal Peptides; Homologous Sequences, Amino Acid; Abnormal amino acid
-    # 'T116', # Amino Acid, Peptide, or Protein, ex.: Amino Acids, Cyclic; Glycopeptides; Keratin
-    # 'T011', # Amphibian, ex.: Salamandra; Urodela; Brazilian horned frog
-    # 'T190', # Anatomical Abnormality, ex.: Bronchial Fistula; Foot Deformities; Hyperostosis of skull
-    # 'T017', # Anatomical Structure, ex.: Cadaver; Pharyngostome; Anatomic structures
-    # 'T008', # Animal, ex.: Animals; Animals, Laboratory; Carnivore
-    'T195', # Antibiotic, ex.: Antibiotics; bactericide; Thienamycins
-    # 'T194', # Archaeon, ex.: Thermoproteales; Haloferax volcanii; Methanospirillum
-    # 'T007', # Bacterium, ex.: Acetobacter; Bacillus cereus; Cytophaga
-    # 'T053', # Behavior, ex.: Homing Behavior; Sexuality; Habitat Selection
-    # 'T038', # Biologic Function, ex.: Antibody Formation; Drug resistance; Homeostasis
-    # 'T123', # Biologically Active Substance, ex.: Cytokinins; Pheromone
-    # 'T091', # Biomedical Occupation or Discipline, ex.: Adolescent Medicine; Cellular Neurobiology; Dentistry
-    # 'T122', # Biomedical or Dental Material, ex.: Acrylic Resins; Bone Cements; Dentifrices
-    # 'T012', # Bird, ex.: Serinus; Ducks; Quail
-    'T029', # Body Location or Region, ex.: Forehead; Sublingual Region; Base of skull structure
-    'T023', # Body Part, Organ, or Organ Component, ex.: Aorta; Brain Stem; Structure of neck of femur
-    # 'T030', # Body Space or Junction, ex.: Knee joint; Greater sac of peritoneum; Synapses
-    'T031', # Body Substance, ex.: Amniotic Fluid; saliva; Smegma
-    # 'T022', # Body System, ex.: Endocrine system; Renin-angiotensin system; Reticuloendothelial System
-    # 'T088', # Carbohydrate Sequence, ex.: Carbohydrate Sequence; Abnormal carbohydrate sequence
-    # 'T025', # Cell, ex.: B-Lymphocytes; Dendritic Cells; Fibroblasts
-    # 'T026', # Cell Component, ex.: Axon; Golgi Apparatus; Organelles
-    # 'T043', # Cell Function, ex.: Cell Cycle; Cell division; Phagocytosis
-    # 'T049', # Cell or Molecular Dysfunction, ex.: DNA Damage; Wallerian Degeneration; Atypical squamous metaplasia
-    # 'T103', # Chemical, ex.: Acids; Chemicals; Ionic Liquids
-    # 'T120', # Chemical Viewed Functionally, ex.: Aerosol Propellants; Detergents; Stabilizing Agents
-    # 'T104', # Chemical Viewed Structurally, ex.: Ammonium Compounds; Cations; Sulfur Compounds
-    # 'T185', # Classification, ex.: Anatomy (MeSH Category); Tumor Stage Classification; axis i
-    'T201', # Clinical Attribute, ex.: Bone Density; heart rate; Range of Motion, Articular
-    'T200', # Clinical Drug, ex.: Ranitidine 300 MG Oral Tablet [Zantac]; Aspirin 300 MG Delayed Release Oral
-    # 'T077', # Conceptual Entity, ex.: Geographic Factors; Fractals; Secularism
-    # 'T019', # Congenital Abnormality, ex.: Albinism; Cleft palate with cleft lip; Polydactyly of toes
-    # 'T056', # Daily or Recreational Activity, ex.: Badminton; Dancing; Swimming
-    'T060', # Diagnostic Procedure, ex.: Biopsy; Heart Auscultation; Magnetic Resonance Imaging
-    'T047', # Disease or Syndrome, ex.: Diabetes Mellitus; Drug Allergy; Malabsorption Syndrome
-    'T203', # Drug Delivery Device, ex.: Nordette 21 Day Pack; {7 (Terazosin 1 MG Oral Tablet) / 7 (Terazosin 2 MG
-    # 'T065', # Educational Activity, ex.: Academic Training; Family Planning Training; Preceptorship
-    # 'T196', # Element, Ion, or Isotope, ex.: Carbon; Chromium Isotopes; Radioisotopes
-    # 'T018', # Embryonic Structure, ex.: Blastoderm; Fetus; Neural Crest
-    # 'T071', # Entity, ex.: Gifts, Financial; Image; Product Part
-    # 'T069', # Environmental Effect of Humans, ex.: Air Pollution; Desertification; Bioremediation
-    # 'T126', # Enzyme, ex.: GTP Cyclohydrolase II; enzyme substrate complex; arginine amidase
-    # 'T204', # Eukaryote, ex.: Order Acarina; Bees; Plasmodium malariae
-    # 'T051', # Event, ex.: Anniversaries; Exposure to Mumps virus (event); Device Unattended
-    # 'T050', # Experimental Model of Disease, ex.: Alloxan Diabetes; Liver Cirrhosis, Experimental; Transient Gene Knock-Out
-    # 'T099', # Family Group, ex.: Daughter; Is an only child; Unmarried Fathers
-    'T033', # Finding, ex.: Birth History; Downward displacement of diaphragm; Decreased glucose level
-    # 'T013', # Fish, ex.: Bass; Salmonidae; Whitefish
-    # 'T168', # Food, ex.: Beverages; Egg Yolk (Dietary); Ice Cream
-    # 'T021', # Fully Formed Anatomical Structure, ex.: Entire body as a whole; Female human body; Set of parts of human body
-    # 'T169', # Functional Concept, ex.: Interviewer Effect; Problem Formulation; Endogenous
-    # 'T004', # Fungus, ex.: Aspergillus clavatus; Blastomyces; Neurospora
-    # 'T028', # Gene or Genome, ex.: Alleles; Genome, Human; rRNA Operon
-    # 'T045', # Genetic Function, ex.: Early Gene Transcription; Gene Amplification; RNA Splicing
-    # 'T083', # Geographic Area, ex.: Baltimore; Canada; Far East
-    # 'T064', # Governmental or Regulatory Activity, ex.: Certification; Credentialing; Public Policy
-    # 'T096', # Group, ex.: Focus Groups; jury; teams
-    # 'T102', # Group Attribute, ex.: Family Size; Group Structure; Life Expectancy
-    # 'T131', # Hazardous or Poisonous Substance, ex.: Carcinogens; Fumigant; Mutagens
-    'T058', # Health Care Activity, ex.: ambulatory care services; Clinic Activities; Preventive Health Services
-    # 'T093', # Health Care Related Organization, ex.: Centers for Disease Control and Prevention (U.S.); Halfway Houses;
-    # 'T125', # Hormone, ex.: Enteric Hormones; thymic humoral factor; Prohormone
-    # 'T016', # Human, ex.: Homo sapiens; jean piaget; Member of public
-    # 'T068', # Human-caused Phenomenon or Process, ex.: Baby Boom; Cultural Evolution; Mass Media
-    # 'T078', # Idea or Concept, ex.: Capitalism; Civil Rights; Ethics
-    # 'T129', # Immunologic Factor, ex.: Antigens; Immunologic Factors; Blood group antigen P
-    'T130', # Indicator, Reagent, or Diagnostic Aid, ex.: Fluorescent Dyes; Indicators and Reagents; India ink stain
-    # 'T055', # Individual Behavior, ex.: Assertiveness; Grooming; Risk-Taking
-    'T037', # Injury or Poisoning, ex.: Accidental Falls; Carbon Monoxide Poisoning; Snake Bites
-    # 'T197', # Inorganic Chemical, ex.: Carbonic Acid; aluminum nitride; ferric citrate
-    'T170', # Intellectual Product, ex.: Decision Support Techniques; Information Systems; Literature
-    'T034', # Laboratory or Test Result, ex.: Blood Flow Velocity; Serum Calcium Level; Spinal Fluid Pressure
-    'T059', # Laboratory Procedure, ex.: Blood Protein Electrophoresis; Crystallography; Radioimmunoassay
-    # 'T171', # Language, ex.: Armenian language; braille; Bilingualism
-    # 'T066', # Machine Activity, ex.: Computer Simulation; Equipment Failure; Natural Language Processing
-    # 'T015', # Mammal, ex.: Ursidae Family; Hamsters; Macaca
-    # 'T073', # Manufactured Object, ex.: car seat; Cooking and Eating Utensils; Goggles
-    'T074', # Medical Device, ex.: Bone Screws; Headgear, Orthodontic; Compression Stockings
-    'T048', # Mental or Behavioral Dysfunction, ex.: Agoraphobia; Cyclothymic Disorder; Frigidity
-    'T041', # Mental Process, ex.: Anger; Auditory Fatigue; Avoidance Learning
-    # 'T063', # Molecular Biology Research Technique, ex.: Northern Blotting; Genetic Engineering; In Situ Hybridization
-    # 'T044', # Molecular Function, ex.: Binding, Competitive; Electron Transport; Glycolysis
-    # 'T085', # Molecular Sequence, ex.: Genetic Code; Homologous Sequences; Molecular Sequence
-    # 'T070', # Natural Phenomenon or Process, ex.: Air Movements; Corrosion; Lightning (phenomenon)
-    'T191', # Neoplastic Process, ex.: Abdominal Neoplasms; Bowen's Disease; Polyp in nasopharynx
-    # 'T114', # Nucleic Acid, Nucleoside, or Nucleotide, ex.: Cytosine Nucleotides; Guanine; Oligonucleotides
-    # 'T086', # Nucleotide Sequence, ex.: Base Sequence; Direct Repeat; RNA Sequence
-    # 'T090', # Occupation or Discipline, ex.: Aviation; Craniology; Ecology
-    # 'T057', # Occupational Activity, ex.: Collective Bargaining; Commerce; Containment of Biohazards
-    # 'T042', # Organ or Tissue Function, ex.: Osteogenesis; Renal Circulation; Tooth Calcification
-    # 'T109', # Organic Chemical, ex.: Benzene Derivatives
-    # 'T001', # Organism, ex.: Organism; Infectious agent; Heterotroph
-    # 'T032', # Organism Attribute, ex.: Age; Birth Weight; Eye Color
-    'T040', # Organism Function, ex.: Breeding; Hibernation; Motor Skills
-    # 'T092', # Organization, ex.: Labor Unions; United Nations; Boarding school
-    'T046', # Pathologic Function, ex.: Inflammation; Shock; Thrombosis
-    # 'T101', # Patient or Disabled Group, ex.: Amputees; Institutionalized Child; Mentally Ill Persons
-    'T121', # Pharmacologic Substance, ex.: Antiemetics; Cardiovascular Agents; Alka-Seltzer
-    'T067', # Phenomenon or Process, ex.: Disasters; Motor Traffic Accidents; Depolymerization
-    # 'T072', # Physical Object, ex.: Printed Media; Meteors; Physical object
-    'T039', # Physiologic Function, ex.: Biorhythms; Hearing; Vasodilation
-    # 'T002', # Plant, ex.: Aloe; Pollen; Helianthus species
-    # 'T098', # Population Group, ex.: Asian Americans; Ethnic group; Adult Offenders
-    # 'T097', # Professional or Occupational Group, ex.: Clergy; Demographers; Hospital Volunteers
-    # 'T094', # Professional Society, ex.: American Medical Association; International Council of Nurses; Library
-    # 'T080', # Qualitative Concept, ex.: Clinical Competence; Consumer Satisfaction; Health Status
-    # 'T081', # Quantitative Concept, ex.: Age Distribution; Metric System; Selection Bias
-    # 'T192', # Receptor, ex.: Binding Sites; Lymphocyte antigen CD4 receptor; integrin alpha11beta1
-    # 'T089', # Regulation or Law, ex.: Building Codes; Criminal Law; Health Planning Guidelines
-    # 'T014', # Reptile, ex.: Alligators; Water Mocassin; Genus Python (organism)
-    # 'T062', # Research Activity, ex.: Animal Experimentation; Biomedical Research; Experimental Replication
-    # 'T075', # Research Device, ex.: Electrodes, Enzyme; DNA Microarray Chip; Particle Count and Size Analyzer
-    # 'T095', # Self-help or Relief Organization, ex.: Alcoholics Anonymous; Charities - organization; Red Cross
-    'T184', # Sign or Symptom, ex.: Dyspnea; Nausea; Pain
-    # 'T054', # Social Behavior, ex.: Acculturation; Communication; Interpersonal Relations
-    # 'T082', # Spatial Concept, ex.: Mandibular Rest Position; Lateral; Extrinsic
-    # 'T167', # Substance, ex.: Air (substance); Fossils; Plastics
-    # 'T079', # Temporal Concept, ex.: Birth Intervals; Half-Life; Postoperative Period
-    'T061', # Therapeutic or Preventive Procedure, ex.: Cesarean section; Dermabrasion; Family psychotherapy
-    # 'T024', # Tissue, ex.: Cartilage; Endothelium; Epidermis
-    # 'T010', # Vertebrate, ex.: Vertebrates; Gnathostomata vertebrate; Craniata <chordata>
-    # 'T005', # Virus, ex.: Coliphages; Echovirus; Parvoviridae
-    # 'T127'  # Vitamin, ex.: 5,25-Dihydroxy cholecalciferol; alpha-tocopheryl oxalate; Vitamin A [EPC]
-}
-
-UNICODE_DASHES = {
-    u'\u002d', u'\u007e', u'\u00ad', u'\u058a', u'\u05be', u'\u1400',
-    u'\u1806', u'\u2010', u'\u2011', u'\u2010', u'\u2012', u'\u2013',
-    u'\u2014', u'\u2015', u'\u2053', u'\u207b', u'\u2212', u'\u208b',
-    u'\u2212', u'\u2212', u'\u2e17', u'\u2e3a', u'\u2e3b', u'\u301c',
-    u'\u3030', u'\u30a0', u'\ufe31', u'\ufe32', u'\ufe58', u'\ufe63',
-    u'\uff0d'
-}
-
-# language with missing value
-# will not have support for tokenization
-LANGUAGES = {
-    'BAQ': None,           # Basque
-    'CHI': None,           # Chinese
-    'CZE': None,           # Czech
-    'DAN': 'danish',       # Danish
-    'DUT': 'dutch',        # Dutch
-    'ENG': 'english',      # English
-    'EST': None,           # Estonian
-    'FIN': 'finnish',      # Finnish
-    'FRE': 'french',       # French
-    'GER': 'german',       # German
-    'GRE': 'greek',        # Greek
-    'HEB': None,           # Hebrew
-    'HUN': 'hungarian',    # Hungarian
-    'ITA': 'italian',      # Italian
-    'JPN': None,           # Japanese
-    'KOR': None,           # Korean
-    'LAV': None,           # Latvian
-    'NOR': 'norwegian',    # Norwegian
-    'POL': 'polish',       # Polish
-    'POR': 'portoguese',   # Portuguese
-    'RUS': 'russian',      # Russian
-    'SCR': None,           # Croatian
-    'SPA': 'spanish',      # Spanish
-    'SWE': 'swedish',      # Swedish
-    'TUR': 'turkish',      # Turkish
-}
-
-DOMAIN_SPECIFIC_STOPWORDS = {
-    'time'
-}
-
-SPACY_LANGUAGE_MAP = {
-    'ENG': 'en_core_web_sm',
-    'GER': 'de_core_news_sm',
-    'SPA': 'es_core_news_sm',
-    'POR': 'pt_core_news_sm',
-    'FRE': 'fr_core_news_sm',
-    'ITA': 'it_core_news_sm',
-    'DUT': 'nl_core_news_sm',
-    'XXX': 'xx'
-}
+MEDSPACY_DEFAULT_SPAN_GROUP_NAME = "medspacy_spans"
+
+HEADERS_MRCONSO = [
+    'cui', 'lat', 'ts', 'lui', 'stt', 'sui', 'ispref', 'aui', 'saui',
+    'scui', 'sdui', 'sab', 'tty', 'code', 'str', 'srl', 'suppress', 'cvf'
+]
+HEADERS_MRSTY = [
+    'cui', 'sty', 'hier' 'desc', 'sid', 'num'
+]
+
+NEGATIONS = {'none', 'non', 'neither', 'nor', 'no', 'not'}
+
+# The following is a list of all existing semtypes along with their name and some examples. 
+# You can easily select the ones you need by commenting out the lines that are not relevant for your application.
+
+ACCEPTED_SEMTYPES = {
+    # 'T020', # Acquired Abnormality, ex.: Hemorrhoids; Hernia, Femoral; Cauliflower ear
+    # 'T052', # Activity, ex.: Expeditions; Information Distribution; Social Planning
+    # 'T100', # Age Group, ex.: Adult; Infant, Premature; Adolescent (age group)
+    # 'T087', # Amino Acid Sequence, ex.: Signal Peptides; Homologous Sequences, Amino Acid; Abnormal amino acid
+    # 'T116', # Amino Acid, Peptide, or Protein, ex.: Amino Acids, Cyclic; Glycopeptides; Keratin
+    # 'T011', # Amphibian, ex.: Salamandra; Urodela; Brazilian horned frog
+    # 'T190', # Anatomical Abnormality, ex.: Bronchial Fistula; Foot Deformities; Hyperostosis of skull
+    # 'T017', # Anatomical Structure, ex.: Cadaver; Pharyngostome; Anatomic structures
+    # 'T008', # Animal, ex.: Animals; Animals, Laboratory; Carnivore
+    'T195', # Antibiotic, ex.: Antibiotics; bactericide; Thienamycins
+    # 'T194', # Archaeon, ex.: Thermoproteales; Haloferax volcanii; Methanospirillum
+    # 'T007', # Bacterium, ex.: Acetobacter; Bacillus cereus; Cytophaga
+    # 'T053', # Behavior, ex.: Homing Behavior; Sexuality; Habitat Selection
+    # 'T038', # Biologic Function, ex.: Antibody Formation; Drug resistance; Homeostasis
+    # 'T123', # Biologically Active Substance, ex.: Cytokinins; Pheromone
+    # 'T091', # Biomedical Occupation or Discipline, ex.: Adolescent Medicine; Cellular Neurobiology; Dentistry
+    # 'T122', # Biomedical or Dental Material, ex.: Acrylic Resins; Bone Cements; Dentifrices
+    # 'T012', # Bird, ex.: Serinus; Ducks; Quail
+    'T029', # Body Location or Region, ex.: Forehead; Sublingual Region; Base of skull structure
+    'T023', # Body Part, Organ, or Organ Component, ex.: Aorta; Brain Stem; Structure of neck of femur
+    # 'T030', # Body Space or Junction, ex.: Knee joint; Greater sac of peritoneum; Synapses
+    'T031', # Body Substance, ex.: Amniotic Fluid; saliva; Smegma
+    # 'T022', # Body System, ex.: Endocrine system; Renin-angiotensin system; Reticuloendothelial System
+    # 'T088', # Carbohydrate Sequence, ex.: Carbohydrate Sequence; Abnormal carbohydrate sequence
+    # 'T025', # Cell, ex.: B-Lymphocytes; Dendritic Cells; Fibroblasts
+    # 'T026', # Cell Component, ex.: Axon; Golgi Apparatus; Organelles
+    # 'T043', # Cell Function, ex.: Cell Cycle; Cell division; Phagocytosis
+    # 'T049', # Cell or Molecular Dysfunction, ex.: DNA Damage; Wallerian Degeneration; Atypical squamous metaplasia
+    # 'T103', # Chemical, ex.: Acids; Chemicals; Ionic Liquids
+    # 'T120', # Chemical Viewed Functionally, ex.: Aerosol Propellants; Detergents; Stabilizing Agents
+    # 'T104', # Chemical Viewed Structurally, ex.: Ammonium Compounds; Cations; Sulfur Compounds
+    # 'T185', # Classification, ex.: Anatomy (MeSH Category); Tumor Stage Classification; axis i
+    'T201', # Clinical Attribute, ex.: Bone Density; heart rate; Range of Motion, Articular
+    'T200', # Clinical Drug, ex.: Ranitidine 300 MG Oral Tablet [Zantac]; Aspirin 300 MG Delayed Release Oral
+    # 'T077', # Conceptual Entity, ex.: Geographic Factors; Fractals; Secularism
+    # 'T019', # Congenital Abnormality, ex.: Albinism; Cleft palate with cleft lip; Polydactyly of toes
+    # 'T056', # Daily or Recreational Activity, ex.: Badminton; Dancing; Swimming
+    'T060', # Diagnostic Procedure, ex.: Biopsy; Heart Auscultation; Magnetic Resonance Imaging
+    'T047', # Disease or Syndrome, ex.: Diabetes Mellitus; Drug Allergy; Malabsorption Syndrome
+    'T203', # Drug Delivery Device, ex.: Nordette 21 Day Pack; {7 (Terazosin 1 MG Oral Tablet) / 7 (Terazosin 2 MG
+    # 'T065', # Educational Activity, ex.: Academic Training; Family Planning Training; Preceptorship
+    # 'T196', # Element, Ion, or Isotope, ex.: Carbon; Chromium Isotopes; Radioisotopes
+    # 'T018', # Embryonic Structure, ex.: Blastoderm; Fetus; Neural Crest
+    # 'T071', # Entity, ex.: Gifts, Financial; Image; Product Part
+    # 'T069', # Environmental Effect of Humans, ex.: Air Pollution; Desertification; Bioremediation
+    # 'T126', # Enzyme, ex.: GTP Cyclohydrolase II; enzyme substrate complex; arginine amidase
+    # 'T204', # Eukaryote, ex.: Order Acarina; Bees; Plasmodium malariae
+    # 'T051', # Event, ex.: Anniversaries; Exposure to Mumps virus (event); Device Unattended
+    # 'T050', # Experimental Model of Disease, ex.: Alloxan Diabetes; Liver Cirrhosis, Experimental; Transient Gene Knock-Out
+    # 'T099', # Family Group, ex.: Daughter; Is an only child; Unmarried Fathers
+    'T033', # Finding, ex.: Birth History; Downward displacement of diaphragm; Decreased glucose level
+    # 'T013', # Fish, ex.: Bass; Salmonidae; Whitefish
+    # 'T168', # Food, ex.: Beverages; Egg Yolk (Dietary); Ice Cream
+    # 'T021', # Fully Formed Anatomical Structure, ex.: Entire body as a whole; Female human body; Set of parts of human body
+    # 'T169', # Functional Concept, ex.: Interviewer Effect; Problem Formulation; Endogenous
+    # 'T004', # Fungus, ex.: Aspergillus clavatus; Blastomyces; Neurospora
+    # 'T028', # Gene or Genome, ex.: Alleles; Genome, Human; rRNA Operon
+    # 'T045', # Genetic Function, ex.: Early Gene Transcription; Gene Amplification; RNA Splicing
+    # 'T083', # Geographic Area, ex.: Baltimore; Canada; Far East
+    # 'T064', # Governmental or Regulatory Activity, ex.: Certification; Credentialing; Public Policy
+    # 'T096', # Group, ex.: Focus Groups; jury; teams
+    # 'T102', # Group Attribute, ex.: Family Size; Group Structure; Life Expectancy
+    # 'T131', # Hazardous or Poisonous Substance, ex.: Carcinogens; Fumigant; Mutagens
+    'T058', # Health Care Activity, ex.: ambulatory care services; Clinic Activities; Preventive Health Services
+    # 'T093', # Health Care Related Organization, ex.: Centers for Disease Control and Prevention (U.S.); Halfway Houses;
+    # 'T125', # Hormone, ex.: Enteric Hormones; thymic humoral factor; Prohormone
+    # 'T016', # Human, ex.: Homo sapiens; jean piaget; Member of public
+    # 'T068', # Human-caused Phenomenon or Process, ex.: Baby Boom; Cultural Evolution; Mass Media
+    # 'T078', # Idea or Concept, ex.: Capitalism; Civil Rights; Ethics
+    # 'T129', # Immunologic Factor, ex.: Antigens; Immunologic Factors; Blood group antigen P
+    'T130', # Indicator, Reagent, or Diagnostic Aid, ex.: Fluorescent Dyes; Indicators and Reagents; India ink stain
+    # 'T055', # Individual Behavior, ex.: Assertiveness; Grooming; Risk-Taking
+    'T037', # Injury or Poisoning, ex.: Accidental Falls; Carbon Monoxide Poisoning; Snake Bites
+    # 'T197', # Inorganic Chemical, ex.: Carbonic Acid; aluminum nitride; ferric citrate
+    'T170', # Intellectual Product, ex.: Decision Support Techniques; Information Systems; Literature
+    'T034', # Laboratory or Test Result, ex.: Blood Flow Velocity; Serum Calcium Level; Spinal Fluid Pressure
+    'T059', # Laboratory Procedure, ex.: Blood Protein Electrophoresis; Crystallography; Radioimmunoassay
+    # 'T171', # Language, ex.: Armenian language; braille; Bilingualism
+    # 'T066', # Machine Activity, ex.: Computer Simulation; Equipment Failure; Natural Language Processing
+    # 'T015', # Mammal, ex.: Ursidae Family; Hamsters; Macaca
+    # 'T073', # Manufactured Object, ex.: car seat; Cooking and Eating Utensils; Goggles
+    'T074', # Medical Device, ex.: Bone Screws; Headgear, Orthodontic; Compression Stockings
+    'T048', # Mental or Behavioral Dysfunction, ex.: Agoraphobia; Cyclothymic Disorder; Frigidity
+    'T041', # Mental Process, ex.: Anger; Auditory Fatigue; Avoidance Learning
+    # 'T063', # Molecular Biology Research Technique, ex.: Northern Blotting; Genetic Engineering; In Situ Hybridization
+    # 'T044', # Molecular Function, ex.: Binding, Competitive; Electron Transport; Glycolysis
+    # 'T085', # Molecular Sequence, ex.: Genetic Code; Homologous Sequences; Molecular Sequence
+    # 'T070', # Natural Phenomenon or Process, ex.: Air Movements; Corrosion; Lightning (phenomenon)
+    'T191', # Neoplastic Process, ex.: Abdominal Neoplasms; Bowen's Disease; Polyp in nasopharynx
+    # 'T114', # Nucleic Acid, Nucleoside, or Nucleotide, ex.: Cytosine Nucleotides; Guanine; Oligonucleotides
+    # 'T086', # Nucleotide Sequence, ex.: Base Sequence; Direct Repeat; RNA Sequence
+    # 'T090', # Occupation or Discipline, ex.: Aviation; Craniology; Ecology
+    # 'T057', # Occupational Activity, ex.: Collective Bargaining; Commerce; Containment of Biohazards
+    # 'T042', # Organ or Tissue Function, ex.: Osteogenesis; Renal Circulation; Tooth Calcification
+    # 'T109', # Organic Chemical, ex.: Benzene Derivatives
+    # 'T001', # Organism, ex.: Organism; Infectious agent; Heterotroph
+    # 'T032', # Organism Attribute, ex.: Age; Birth Weight; Eye Color
+    'T040', # Organism Function, ex.: Breeding; Hibernation; Motor Skills
+    # 'T092', # Organization, ex.: Labor Unions; United Nations; Boarding school
+    'T046', # Pathologic Function, ex.: Inflammation; Shock; Thrombosis
+    # 'T101', # Patient or Disabled Group, ex.: Amputees; Institutionalized Child; Mentally Ill Persons
+    'T121', # Pharmacologic Substance, ex.: Antiemetics; Cardiovascular Agents; Alka-Seltzer
+    'T067', # Phenomenon or Process, ex.: Disasters; Motor Traffic Accidents; Depolymerization
+    # 'T072', # Physical Object, ex.: Printed Media; Meteors; Physical object
+    'T039', # Physiologic Function, ex.: Biorhythms; Hearing; Vasodilation
+    # 'T002', # Plant, ex.: Aloe; Pollen; Helianthus species
+    # 'T098', # Population Group, ex.: Asian Americans; Ethnic group; Adult Offenders
+    # 'T097', # Professional or Occupational Group, ex.: Clergy; Demographers; Hospital Volunteers
+    # 'T094', # Professional Society, ex.: American Medical Association; International Council of Nurses; Library
+    # 'T080', # Qualitative Concept, ex.: Clinical Competence; Consumer Satisfaction; Health Status
+    # 'T081', # Quantitative Concept, ex.: Age Distribution; Metric System; Selection Bias
+    # 'T192', # Receptor, ex.: Binding Sites; Lymphocyte antigen CD4 receptor; integrin alpha11beta1
+    # 'T089', # Regulation or Law, ex.: Building Codes; Criminal Law; Health Planning Guidelines
+    # 'T014', # Reptile, ex.: Alligators; Water Mocassin; Genus Python (organism)
+    # 'T062', # Research Activity, ex.: Animal Experimentation; Biomedical Research; Experimental Replication
+    # 'T075', # Research Device, ex.: Electrodes, Enzyme; DNA Microarray Chip; Particle Count and Size Analyzer
+    # 'T095', # Self-help or Relief Organization, ex.: Alcoholics Anonymous; Charities - organization; Red Cross
+    'T184', # Sign or Symptom, ex.: Dyspnea; Nausea; Pain
+    # 'T054', # Social Behavior, ex.: Acculturation; Communication; Interpersonal Relations
+    # 'T082', # Spatial Concept, ex.: Mandibular Rest Position; Lateral; Extrinsic
+    # 'T167', # Substance, ex.: Air (substance); Fossils; Plastics
+    # 'T079', # Temporal Concept, ex.: Birth Intervals; Half-Life; Postoperative Period
+    'T061', # Therapeutic or Preventive Procedure, ex.: Cesarean section; Dermabrasion; Family psychotherapy
+    # 'T024', # Tissue, ex.: Cartilage; Endothelium; Epidermis
+    # 'T010', # Vertebrate, ex.: Vertebrates; Gnathostomata vertebrate; Craniata <chordata>
+    # 'T005', # Virus, ex.: Coliphages; Echovirus; Parvoviridae
+    # 'T127'  # Vitamin, ex.: 5,25-Dihydroxy cholecalciferol; alpha-tocopheryl oxalate; Vitamin A [EPC]
+}
+
+UNICODE_DASHES = {
+    u'\u002d', u'\u007e', u'\u00ad', u'\u058a', u'\u05be', u'\u1400',
+    u'\u1806', u'\u2010', u'\u2011', u'\u2010', u'\u2012', u'\u2013',
+    u'\u2014', u'\u2015', u'\u2053', u'\u207b', u'\u2212', u'\u208b',
+    u'\u2212', u'\u2212', u'\u2e17', u'\u2e3a', u'\u2e3b', u'\u301c',
+    u'\u3030', u'\u30a0', u'\ufe31', u'\ufe32', u'\ufe58', u'\ufe63',
+    u'\uff0d'
+}
+
+# language with missing value
+# will not have support for tokenization
+LANGUAGES = {
+    'BAQ': None,           # Basque
+    'CHI': None,           # Chinese
+    'CZE': None,           # Czech
+    'DAN': 'danish',       # Danish
+    'DUT': 'dutch',        # Dutch
+    'ENG': 'english',      # English
+    'EST': None,           # Estonian
+    'FIN': 'finnish',      # Finnish
+    'FRE': 'french',       # French
+    'GER': 'german',       # German
+    'GRE': 'greek',        # Greek
+    'HEB': None,           # Hebrew
+    'HUN': 'hungarian',    # Hungarian
+    'ITA': 'italian',      # Italian
+    'JPN': None,           # Japanese
+    'KOR': None,           # Korean
+    'LAV': None,           # Latvian
+    'NOR': 'norwegian',    # Norwegian
+    'POL': 'polish',       # Polish
+    'POR': 'portuguese',   # Portuguese
+    'RUS': 'russian',      # Russian
+    'SCR': None,           # Croatian
+    'SPA': 'spanish',      # Spanish
+    'SWE': 'swedish',      # Swedish
+    'TUR': 'turkish',      # Turkish
+}
+
+DOMAIN_SPECIFIC_STOPWORDS = {
+    'time'
+}
+
+SPACY_LANGUAGE_MAP = {
+    'ENG': 'en_core_web_sm',
+    'GER': 'de_core_news_sm',
+    'SPA': 'es_core_news_sm',
+    'POR': 'pt_core_news_sm',
+    'FRE': 'fr_core_news_sm',
+    'ITA': 'it_core_news_sm',
+    'DUT': 'nl_core_news_sm',
+    'POL': 'pl_core_news_sm',
+    'XXX': 'xx'
+}
```

### Comparing `medspacy_quickumls-3.1a0/quickumls/core.py` & `medspacy_quickumls-3.2/quickumls/core.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,481 +1,481 @@
-# future statements for Python 2 compatibility
-from __future__ import (
-    unicode_literals, division, print_function, absolute_import)
-
-# built in modules
-import os
-import sys
-import datetime
-from six.moves import xrange
-
-# installed modules
-import spacy
-import nltk
-from unidecode import unidecode
-
-# project modules
-from . import toolbox
-from . import constants
-
-
-class QuickUMLS(object):
-    """The main class to interact with the matcher.
-    """
-    def __init__(
-            self, quickumls_fp,
-            overlapping_criteria='score', threshold=0.7, window=5,
-            similarity_name='jaccard', min_match_length=3,
-            accepted_semtypes=constants.ACCEPTED_SEMTYPES,
-            verbose=False, keep_uppercase=False,
-            spacy_component = False):
-        """Instantiate QuickUMLS object
-
-            This is the main interface through which text can be processed.
-
-        Args:
-            quickumls_fp (str): Path to which QuickUMLS was installed
-            overlapping_criteria (str, optional):
-                    One of "score" or "length". Choose how results are ranked.
-                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
-            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
-            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
-            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
-                    Similarity measure to be used. Defaults to 'jaccard'.
-            min_match_length (int, optional): TODO: ??. Defaults to 3.
-            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
-                Semantic types are identified by the letter "T" followed by three numbers
-                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
-                Defaults to constants.ACCEPTED_SEMTYPES.
-            verbose (bool, optional): TODO:??. Defaults to False.
-            keep_uppercase (bool, optional): By default QuickUMLS converts all
-                    uppercase strings to lowercase. This option disables that
-                    functionality, which makes QuickUMLS useful for
-                    distinguishing acronyms from normal words. For this the
-                    database should be installed without the -L option.
-                    Defaults to False.
-
-        Raises:
-            ValueError: Raises a ValueError if QuickUMLS was installed for a language that is not currently supported TODO: verify this?
-            OSError: Raises an OSError if the required Spacy model was not installed.
-        """
-
-        self.verbose = verbose
-
-        valid_criteria = {'length', 'score'}
-        err_msg = (
-            '"{}" is not a valid overlapping_criteria. Choose '
-            'between {}'.format(
-                overlapping_criteria, ', '.join(valid_criteria)
-            )
-        )
-        assert overlapping_criteria in valid_criteria, err_msg
-        self.overlapping_criteria = overlapping_criteria
-
-        valid_similarities = {'dice', 'jaccard', 'cosine', 'overlap'}
-        err_msg = ('"{}" is not a valid similarity name. Choose between '
-                   '{}'.format(similarity_name, ', '.join(valid_similarities)))
-        assert not(valid_similarities in valid_similarities), err_msg
-        self.similarity_name = similarity_name
-
-        simstring_fp = os.path.join(quickumls_fp, 'umls-simstring.db')
-        cuisem_fp = os.path.join(quickumls_fp, 'cui-semtypes.db')
-
-        self.valid_punct = constants.UNICODE_DASHES
-        self.negations = constants.NEGATIONS
-
-        self.window = window
-        self.ngram_length = 3
-        self.threshold = threshold
-        self.min_match_length = min_match_length
-        self.to_lowercase_flag = os.path.exists(
-            os.path.join(quickumls_fp, 'lowercase.flag')
-        )
-        self.normalize_unicode_flag = os.path.exists(
-            os.path.join(quickumls_fp, 'normalize-unicode.flag')
-        )
-        self.keep_uppercase = keep_uppercase
-
-        # Check whether data is installed with lowercase flag and QuickUMLS initiated with keeping uppercase words
-        if self.to_lowercase_flag and self.keep_uppercase:
-            raise ValueError('Database is installed with lowercase flag and QuickUMLS is initiated with '
-                             'keep_uppercase flag. This would prevent identifying concepts that contain all uppercase'
-                             'characters. Please reinstall data without --lowercase or run QuickUMLS without'
-                             '--keep_uppercase.')
-
-        language_fp = os.path.join(quickumls_fp, 'language.flag')
-
-        # download stopwords if necessary
-        try:
-            nltk.corpus.stopwords.words()
-        except LookupError:
-            nltk.download('stopwords')
-
-        if os.path.exists(language_fp):
-            with open(language_fp) as f:
-                self.language_flag = f.read().strip()
-        else:
-            self.language_flag = 'ENG'
-
-        if self.language_flag not in constants.LANGUAGES:
-            raise ValueError('Language "{}" not supported'.format(self.language_flag))
-        elif constants.LANGUAGES[self.language_flag] is None:
-            self._stopwords = set()
-            spacy_lang = 'XXX'
-        else:
-            self._stopwords = set(
-                nltk.corpus.stopwords.words(constants.LANGUAGES[self.language_flag])
-            )
-            spacy_lang = constants.SPACY_LANGUAGE_MAP[self.language_flag]
-
-        database_backend_fp = os.path.join(quickumls_fp, 'database_backend.flag')
-        if os.path.exists(database_backend_fp):
-            with open(database_backend_fp) as f:
-                self._database_backend = f.read().strip()
-        else:
-            raise ValueError("""File database_backend.flag was not found at this location: {}.  This path may have been created with leveldb
-                             or an earlier version of QuickUMLS, but leveldb is not supported by this package version
-                             """.format(quickumls_fp))
-
-        # domain specific stopwords
-        self._stopwords = self._stopwords.union(constants.DOMAIN_SPECIFIC_STOPWORDS)
-
-        self._info = None
-
-        self.accepted_semtypes = accepted_semtypes
-
-        # if this is not being executed as as spacy component, then it must be standalone
-        if spacy_component:
-            # In this case, the pipeline is external to this current class
-            self.nlp = None
-        else:
-            try:
-                self.nlp = spacy.load(spacy_lang)
-            except OSError:
-                msg = (
-                    'Model for language "{}" is not downloaded. Please '
-                    'run "python -m spacy download {}" before launching '
-                    'QuickUMLS'
-                ).format(
-                    self.language_flag,
-                    constants.SPACY_LANGUAGE_MAP.get(self.language_flag, 'xx')
-                )
-                raise OSError(msg)
-
-        self.ss_db = toolbox.SimstringDBReader(
-            simstring_fp, similarity_name, threshold
-        )
-        self.cuisem_db = toolbox.CuiSemTypesDB(
-            cuisem_fp, database_backend=self._database_backend
-        )
-
-    def get_info(self):
-        """Computes a summary of the matcher options.
-
-        Returns:
-            Dict: Dictionary containing information on the QuicUMLS instance.
-        """
-        return self.info
-
-    def get_accepted_semtypes(self):
-        return self.accepted_semtypes
-
-    @property
-    def info(self):
-        """Computes a summary of the matcher options.
-
-        Returns:
-            Dict: Dictionary containing information on the QuicUMLS instance.
-        """
-        # useful for caching of respnses
-
-        if self._info is None:
-            self._info = {
-                'threshold': self.threshold,
-                'similarity_name': self.similarity_name,
-                'window': self.window,
-                'ngram_length': self.ngram_length,
-                'min_match_length': self.min_match_length,
-                'accepted_semtypes': sorted(self.accepted_semtypes),
-                'negations': sorted(self.negations),
-                'valid_punct': sorted(self.valid_punct)
-            }
-        return self._info
-
-    def _is_valid_token(self, tok):
-        return not(
-            tok.is_punct or tok.is_space or
-            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
-        )
-
-    def _is_valid_start_token(self, tok):
-        return not(
-            tok.like_num or
-            (self._is_stop_term(tok) and tok.lemma_ not in self.negations) or
-            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
-        )
-
-    def _is_stop_term(self, tok):
-        return tok.text in self._stopwords
-
-    def _is_valid_end_token(self, tok):
-        return not(
-            tok.is_punct or tok.is_space or self._is_stop_term(tok) or
-            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
-        )
-
-    def _is_valid_middle_token(self, tok):
-        return (
-            not(tok.is_punct or tok.is_space) or
-            tok.is_bracket or
-            tok.text in self.valid_punct
-        )
-
-    def _is_ok_semtype(self, target_semtypes):
-        if self.accepted_semtypes is None:
-            ok = True
-        else:
-            ok = any(sem in self.accepted_semtypes for sem in target_semtypes)
-        return ok
-
-    def _is_longer_than_min(self, span):
-        return (span.end_char - span.start_char) >= self.min_match_length
-
-    def _make_ngrams(self, sent):
-        sent_length = len(sent)
-
-        # do not include determiners inside a span
-        skip_in_span = {token.i for token in sent if token.pos_ == 'DET'}
-
-        # invalidate a span if it includes any on these symbols
-        invalid_mid_tokens = {
-            token.i for token in sent if not self._is_valid_middle_token(token)
-        }
-
-        for i in xrange(sent_length):
-            tok = sent[i]
-
-            if not self._is_valid_token(tok):
-                continue
-
-            # do not consider this token by itself if it is
-            # a number or a stopword.
-            if self._is_valid_start_token(tok):
-                compensate = False
-            else:
-                compensate = True
-
-            span_end = min(sent_length, i + self.window) + 1
-
-            # we take a shortcut if the token is the last one
-            # in the sentence
-            if (
-                i + 1 == sent_length and            # it's the last token
-                self._is_valid_end_token(tok) and   # it's a valid end token
-                len(tok) >= self.min_match_length   # it's of miminum length
-            ):
-                yield(tok.idx, tok.idx + len(tok), tok.text)
-
-            for j in xrange(i + 1, span_end):
-                if compensate:
-                    compensate = False
-                    continue
-
-                if sent[j - 1] in invalid_mid_tokens:
-                    break
-
-                if not self._is_valid_end_token(sent[j - 1]):
-                    continue
-
-                span = sent[i:j]
-
-                if not self._is_longer_than_min(span):
-                    continue
-
-                yield (
-                    span.start_char, span.end_char,
-                    ''.join(token.text_with_ws for token in span
-                            if token.i not in skip_in_span).strip()
-                )
-
-    def _get_all_matches(self, ngrams):
-        matches = []
-        for start, end, ngram in ngrams:
-            ngram_normalized = ngram
-
-            if self.normalize_unicode_flag:
-                ngram_normalized = unidecode(ngram_normalized)
-
-            # make it lowercase
-            if self.to_lowercase_flag:
-                ngram_normalized = ngram_normalized.lower()
-
-            # If the term is all uppercase, it might be the case that
-            # no match is found; so we convert to lowercase;
-            # however, this is never needed if the string is lowercased
-            # in the step above
-            if not self.to_lowercase_flag and ngram_normalized.isupper() and not self.keep_uppercase:
-                ngram_normalized = ngram_normalized.lower()
-
-            prev_cui = None
-            ngram_cands = list(self.ss_db.get(ngram_normalized))
-
-            ngram_dict = {}
-            for match in ngram_cands:
-                cuisem_match = sorted(self.cuisem_db.get(match))
-
-                match_similarity = toolbox.get_similarity(
-                    x=ngram_normalized,
-                    y=match,
-                    n=self.ngram_length,
-                    similarity_name=self.similarity_name
-                )
-
-                if match_similarity == 0:
-                        continue
-
-                for cui, semtypes, preferred in cuisem_match:
-
-                    if not self._is_ok_semtype(semtypes):
-                        continue
-
-                    # if cui is already in the dictionary, replace only if the new score is higher
-                    if cui in ngram_dict.keys():
-                        if match_similarity > ngram_dict[cui]['similarity']:
-                            ngram_dict[cui] = {
-                                'start': start,
-                                'end': end,
-                                'ngram': ngram,
-                                'term': toolbox.safe_unicode(match),
-                                'cui': cui,
-                                'similarity': match_similarity,
-                                'semtypes': semtypes,
-                                'preferred': preferred
-                            }
-                    else: # otherwise just add it if it is not part of the dictionary
-                        ngram_dict[cui] = {
-                            'start': start,
-                            'end': end,
-                            'ngram': ngram,
-                            'term': toolbox.safe_unicode(match),
-                            'cui': cui,
-                            'similarity': match_similarity,
-                            'semtypes': semtypes,
-                            'preferred': preferred
-                        }
-
-            ngram_matches = ngram_dict.values()
-            if len(ngram_matches) > 0:
-                matches.append(
-                    sorted(
-                        ngram_matches,
-                        key=lambda m: m['similarity'] + m['preferred'],
-                        reverse=True
-                    )
-                )
-        return matches
-
-    @staticmethod
-    def _select_score(match):
-        return (match[0]['similarity'], (match[0]['end'] - match[0]['start']))
-
-    @staticmethod
-    def _select_longest(match):
-        return ((match[0]['end'] - match[0]['start']), match[0]['similarity'])
-
-    def _select_terms(self, matches):
-        sort_func = (
-            self._select_longest if self.overlapping_criteria == 'length'
-            else self._select_score
-        )
-
-        matches = sorted(matches, key=sort_func, reverse=True)
-
-        intervals = toolbox.Intervals()
-        final_matches_subset = []
-
-        for match in matches:
-            match_interval = (match[0]['start'], match[0]['end'])
-            if match_interval not in intervals:
-                final_matches_subset.append(match)
-                intervals.append(match_interval)
-
-        return final_matches_subset
-
-    def _make_token_sequences(self, parsed):
-        for i in range(len(parsed)):
-            for j in xrange(
-                    i + 1, min(i + self.window, len(parsed)) + 1):
-                span = parsed[i:j]
-
-                if not self._is_longer_than_min(span):
-                    continue
-
-                yield (span.start_char, span.end_char, span.text)
-
-    def _print_verbose_status(self, parsed, matches):
-        if not self.verbose:
-            return False
-
-        print(
-            '[{}] {:,} extracted from {:,} tokens'.format(
-                datetime.datetime.now().isoformat(),
-                sum(len(match_group) for match_group in matches),
-                len(parsed)
-            ),
-            file=sys.stderr
-        )
-        return True
-
-    def match(self, text, best_match=True, ignore_syntax=False):
-        """Perform UMLS concept resolution for the given string.
-
-        [extended_summary]
-
-        Args:
-            text (str): Text on which to run the algorithm
-
-            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
-            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False.
-
-        Returns:
-            List: List of all matches in the text
-            TODO: Describe format
-        """
-
-        parsed = self.nlp(u'{}'.format(text))
-        
-        # pass in parsed spacy doc to get concept matches
-        matches = self._match(parsed)
-
-        return matches
-        
-    def _match(self, doc, best_match=True, ignore_syntax=False):
-        """Gathers ngram matches given a spaCy document object.
-
-        [extended_summary]
-
-        Args:
-            text (Document): spaCy Document object to be used for extracting ngrams
-
-            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
-            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
-
-        Returns:
-            List: List of all matches in the text
-            TODO: Describe format
-        """
-        
-        ngrams = None
-        if ignore_syntax:
-            ngrams = self._make_token_sequences(doc)
-        else:
-            ngrams = self._make_ngrams(doc)
-
-        matches = self._get_all_matches(ngrams)
-
-        if best_match:
-            matches = self._select_terms(matches)
-
-        self._print_verbose_status(doc, matches)
-        
-        return matches
+# future statements for Python 2 compatibility
+from __future__ import (
+    unicode_literals, division, print_function, absolute_import)
+
+# built in modules
+import os
+import sys
+import datetime
+from six.moves import xrange
+
+# installed modules
+import spacy
+import nltk
+from unidecode import unidecode
+
+# project modules
+from . import toolbox
+from . import constants
+
+
+class QuickUMLS(object):
+    """The main class to interact with the matcher.
+    """
+    def __init__(
+            self, quickumls_fp,
+            overlapping_criteria='score', threshold=0.7, window=5,
+            similarity_name='jaccard', min_match_length=3,
+            accepted_semtypes=constants.ACCEPTED_SEMTYPES,
+            verbose=False, keep_uppercase=False,
+            spacy_component = False):
+        """Instantiate QuickUMLS object
+
+            This is the main interface through which text can be processed.
+
+        Args:
+            quickumls_fp (str): Path to which QuickUMLS was installed
+            overlapping_criteria (str, optional):
+                    One of "score" or "length". Choose how results are ranked.
+                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
+            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
+            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
+            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
+                    Similarity measure to be used. Defaults to 'jaccard'.
+            min_match_length (int, optional): TODO: ??. Defaults to 3.
+            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
+                Semantic types are identified by the letter "T" followed by three numbers
+                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
+                Defaults to constants.ACCEPTED_SEMTYPES.
+            verbose (bool, optional): TODO:??. Defaults to False.
+            keep_uppercase (bool, optional): By default QuickUMLS converts all
+                    uppercase strings to lowercase. This option disables that
+                    functionality, which makes QuickUMLS useful for
+                    distinguishing acronyms from normal words. For this the
+                    database should be installed without the -L option.
+                    Defaults to False.
+
+        Raises:
+            ValueError: Raises a ValueError if QuickUMLS was installed for a language that is not currently supported TODO: verify this?
+            OSError: Raises an OSError if the required Spacy model was not installed.
+        """
+
+        self.verbose = verbose
+
+        valid_criteria = {'length', 'score'}
+        err_msg = (
+            '"{}" is not a valid overlapping_criteria. Choose '
+            'between {}'.format(
+                overlapping_criteria, ', '.join(valid_criteria)
+            )
+        )
+        assert overlapping_criteria in valid_criteria, err_msg
+        self.overlapping_criteria = overlapping_criteria
+
+        valid_similarities = {'dice', 'jaccard', 'cosine', 'overlap'}
+        err_msg = ('"{}" is not a valid similarity name. Choose between '
+                   '{}'.format(similarity_name, ', '.join(valid_similarities)))
+        assert not(valid_similarities in valid_similarities), err_msg
+        self.similarity_name = similarity_name
+
+        simstring_fp = os.path.join(quickumls_fp, 'umls-simstring.db')
+        cuisem_fp = os.path.join(quickumls_fp, 'cui-semtypes.db')
+
+        self.valid_punct = constants.UNICODE_DASHES
+        self.negations = constants.NEGATIONS
+
+        self.window = window
+        self.ngram_length = 3
+        self.threshold = threshold
+        self.min_match_length = min_match_length
+        self.to_lowercase_flag = os.path.exists(
+            os.path.join(quickumls_fp, 'lowercase.flag')
+        )
+        self.normalize_unicode_flag = os.path.exists(
+            os.path.join(quickumls_fp, 'normalize-unicode.flag')
+        )
+        self.keep_uppercase = keep_uppercase
+
+        # Check whether data is installed with lowercase flag and QuickUMLS initiated with keeping uppercase words
+        if self.to_lowercase_flag and self.keep_uppercase:
+            raise ValueError('Database is installed with lowercase flag and QuickUMLS is initiated with '
+                             'keep_uppercase flag. This would prevent identifying concepts that contain all uppercase'
+                             'characters. Please reinstall data without --lowercase or run QuickUMLS without'
+                             '--keep_uppercase.')
+
+        language_fp = os.path.join(quickumls_fp, 'language.flag')
+
+        # download stopwords if necessary
+        try:
+            nltk.corpus.stopwords.words()
+        except LookupError:
+            nltk.download('stopwords')
+
+        if os.path.exists(language_fp):
+            with open(language_fp) as f:
+                self.language_flag = f.read().strip()
+        else:
+            self.language_flag = 'ENG'
+
+        if self.language_flag not in constants.LANGUAGES:
+            raise ValueError('Language "{}" not supported'.format(self.language_flag))
+        elif constants.LANGUAGES[self.language_flag] is None:
+            self._stopwords = set()
+            spacy_lang = 'XXX'
+        else:
+            self._stopwords = set(
+                nltk.corpus.stopwords.words(constants.LANGUAGES[self.language_flag])
+            )
+            spacy_lang = constants.SPACY_LANGUAGE_MAP[self.language_flag]
+
+        database_backend_fp = os.path.join(quickumls_fp, 'database_backend.flag')
+        if os.path.exists(database_backend_fp):
+            with open(database_backend_fp) as f:
+                self._database_backend = f.read().strip()
+        else:
+            raise ValueError("""File database_backend.flag was not found at this location: {}.  This path may have been created with leveldb
+                             or an earlier version of QuickUMLS, but leveldb is not supported by this package version
+                             """.format(quickumls_fp))
+
+        # domain specific stopwords
+        self._stopwords = self._stopwords.union(constants.DOMAIN_SPECIFIC_STOPWORDS)
+
+        self._info = None
+
+        self.accepted_semtypes = accepted_semtypes
+
+        # if this is not being executed as as spacy component, then it must be standalone
+        if spacy_component:
+            # In this case, the pipeline is external to this current class
+            self.nlp = None
+        else:
+            try:
+                self.nlp = spacy.load(spacy_lang)
+            except OSError:
+                msg = (
+                    'Model for language "{}" is not downloaded. Please '
+                    'run "python -m spacy download {}" before launching '
+                    'QuickUMLS'
+                ).format(
+                    self.language_flag,
+                    constants.SPACY_LANGUAGE_MAP.get(self.language_flag, 'xx')
+                )
+                raise OSError(msg)
+
+        self.ss_db = toolbox.SimstringDBReader(
+            simstring_fp, similarity_name, threshold
+        )
+        self.cuisem_db = toolbox.CuiSemTypesDB(
+            cuisem_fp, database_backend=self._database_backend
+        )
+
+    def get_info(self):
+        """Computes a summary of the matcher options.
+
+        Returns:
+            Dict: Dictionary containing information on the QuicUMLS instance.
+        """
+        return self.info
+
+    def get_accepted_semtypes(self):
+        return self.accepted_semtypes
+
+    @property
+    def info(self):
+        """Computes a summary of the matcher options.
+
+        Returns:
+            Dict: Dictionary containing information on the QuicUMLS instance.
+        """
+        # useful for caching of respnses
+
+        if self._info is None:
+            self._info = {
+                'threshold': self.threshold,
+                'similarity_name': self.similarity_name,
+                'window': self.window,
+                'ngram_length': self.ngram_length,
+                'min_match_length': self.min_match_length,
+                'accepted_semtypes': sorted(self.accepted_semtypes),
+                'negations': sorted(self.negations),
+                'valid_punct': sorted(self.valid_punct)
+            }
+        return self._info
+
+    def _is_valid_token(self, tok):
+        return not(
+            tok.is_punct or tok.is_space or
+            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
+        )
+
+    def _is_valid_start_token(self, tok):
+        return not(
+            tok.like_num or
+            (self._is_stop_term(tok) and tok.lemma_ not in self.negations) or
+            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
+        )
+
+    def _is_stop_term(self, tok):
+        return tok.text in self._stopwords
+
+    def _is_valid_end_token(self, tok):
+        return not(
+            tok.is_punct or tok.is_space or self._is_stop_term(tok) or
+            tok.pos_ == 'ADP' or tok.pos_ == 'DET' or tok.pos_ == 'CONJ'
+        )
+
+    def _is_valid_middle_token(self, tok):
+        return (
+            not(tok.is_punct or tok.is_space) or
+            tok.is_bracket or
+            tok.text in self.valid_punct
+        )
+
+    def _is_ok_semtype(self, target_semtypes):
+        if self.accepted_semtypes is None:
+            ok = True
+        else:
+            ok = any(sem in self.accepted_semtypes for sem in target_semtypes)
+        return ok
+
+    def _is_longer_than_min(self, span):
+        return (span.end_char - span.start_char) >= self.min_match_length
+
+    def _make_ngrams(self, sent):
+        sent_length = len(sent)
+
+        # do not include determiners inside a span
+        skip_in_span = {token.i for token in sent if token.pos_ == 'DET'}
+
+        # invalidate a span if it includes any on these symbols
+        invalid_mid_tokens = {
+            token.i for token in sent if not self._is_valid_middle_token(token)
+        }
+
+        for i in xrange(sent_length):
+            tok = sent[i]
+
+            if not self._is_valid_token(tok):
+                continue
+
+            # do not consider this token by itself if it is
+            # a number or a stopword.
+            if self._is_valid_start_token(tok):
+                compensate = False
+            else:
+                compensate = True
+
+            span_end = min(sent_length, i + self.window) + 1
+
+            # we take a shortcut if the token is the last one
+            # in the sentence
+            if (
+                i + 1 == sent_length and            # it's the last token
+                self._is_valid_end_token(tok) and   # it's a valid end token
+                len(tok) >= self.min_match_length   # it's of miminum length
+            ):
+                yield(tok.idx, tok.idx + len(tok), tok.text)
+
+            for j in xrange(i + 1, span_end):
+                if compensate:
+                    compensate = False
+                    continue
+
+                if sent[j - 1] in invalid_mid_tokens:
+                    break
+
+                if not self._is_valid_end_token(sent[j - 1]):
+                    continue
+
+                span = sent[i:j]
+
+                if not self._is_longer_than_min(span):
+                    continue
+
+                yield (
+                    span.start_char, span.end_char,
+                    ''.join(token.text_with_ws for token in span
+                            if token.i not in skip_in_span).strip()
+                )
+
+    def _get_all_matches(self, ngrams):
+        matches = []
+        for start, end, ngram in ngrams:
+            ngram_normalized = ngram
+
+            if self.normalize_unicode_flag:
+                ngram_normalized = unidecode(ngram_normalized)
+
+            # make it lowercase
+            if self.to_lowercase_flag:
+                ngram_normalized = ngram_normalized.lower()
+
+            # If the term is all uppercase, it might be the case that
+            # no match is found; so we convert to lowercase;
+            # however, this is never needed if the string is lowercased
+            # in the step above
+            if not self.to_lowercase_flag and ngram_normalized.isupper() and not self.keep_uppercase:
+                ngram_normalized = ngram_normalized.lower()
+
+            prev_cui = None
+            ngram_cands = list(self.ss_db.get(ngram_normalized))
+
+            ngram_dict = {}
+            for match in ngram_cands:
+                cuisem_match = sorted(self.cuisem_db.get(match))
+
+                match_similarity = toolbox.get_similarity(
+                    x=ngram_normalized,
+                    y=match,
+                    n=self.ngram_length,
+                    similarity_name=self.similarity_name
+                )
+
+                if match_similarity == 0:
+                        continue
+
+                for cui, semtypes, preferred in cuisem_match:
+
+                    if not self._is_ok_semtype(semtypes):
+                        continue
+
+                    # if cui is already in the dictionary, replace only if the new score is higher
+                    if cui in ngram_dict.keys():
+                        if match_similarity > ngram_dict[cui]['similarity']:
+                            ngram_dict[cui] = {
+                                'start': start,
+                                'end': end,
+                                'ngram': ngram,
+                                'term': toolbox.safe_unicode(match),
+                                'cui': cui,
+                                'similarity': match_similarity,
+                                'semtypes': semtypes,
+                                'preferred': preferred
+                            }
+                    else: # otherwise just add it if it is not part of the dictionary
+                        ngram_dict[cui] = {
+                            'start': start,
+                            'end': end,
+                            'ngram': ngram,
+                            'term': toolbox.safe_unicode(match),
+                            'cui': cui,
+                            'similarity': match_similarity,
+                            'semtypes': semtypes,
+                            'preferred': preferred
+                        }
+
+            ngram_matches = ngram_dict.values()
+            if len(ngram_matches) > 0:
+                matches.append(
+                    sorted(
+                        ngram_matches,
+                        key=lambda m: m['similarity'] + m['preferred'],
+                        reverse=True
+                    )
+                )
+        return matches
+
+    @staticmethod
+    def _select_score(match):
+        return (match[0]['similarity'], (match[0]['end'] - match[0]['start']))
+
+    @staticmethod
+    def _select_longest(match):
+        return ((match[0]['end'] - match[0]['start']), match[0]['similarity'])
+
+    def _select_terms(self, matches):
+        sort_func = (
+            self._select_longest if self.overlapping_criteria == 'length'
+            else self._select_score
+        )
+
+        matches = sorted(matches, key=sort_func, reverse=True)
+
+        intervals = toolbox.Intervals()
+        final_matches_subset = []
+
+        for match in matches:
+            match_interval = (match[0]['start'], match[0]['end'])
+            if match_interval not in intervals:
+                final_matches_subset.append(match)
+                intervals.append(match_interval)
+
+        return final_matches_subset
+
+    def _make_token_sequences(self, parsed):
+        for i in range(len(parsed)):
+            for j in xrange(
+                    i + 1, min(i + self.window, len(parsed)) + 1):
+                span = parsed[i:j]
+
+                if not self._is_longer_than_min(span):
+                    continue
+
+                yield (span.start_char, span.end_char, span.text)
+
+    def _print_verbose_status(self, parsed, matches):
+        if not self.verbose:
+            return False
+
+        print(
+            '[{}] {:,} extracted from {:,} tokens'.format(
+                datetime.datetime.now().isoformat(),
+                sum(len(match_group) for match_group in matches),
+                len(parsed)
+            ),
+            file=sys.stderr
+        )
+        return True
+
+    def match(self, text, best_match=True, ignore_syntax=False):
+        """Perform UMLS concept resolution for the given string.
+
+        [extended_summary]
+
+        Args:
+            text (str): Text on which to run the algorithm
+
+            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
+            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False.
+
+        Returns:
+            List: List of all matches in the text
+            TODO: Describe format
+        """
+
+        parsed = self.nlp(u'{}'.format(text))
+        
+        # pass in parsed spacy doc to get concept matches
+        matches = self._match(parsed)
+
+        return matches
+        
+    def _match(self, doc, best_match=True, ignore_syntax=False):
+        """Gathers ngram matches given a spaCy document object.
+
+        [extended_summary]
+
+        Args:
+            text (Document): spaCy Document object to be used for extracting ngrams
+
+            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
+            ignore_syntax (bool, optional): Wether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
+
+        Returns:
+            List: List of all matches in the text
+            TODO: Describe format
+        """
+        
+        ngrams = None
+        if ignore_syntax:
+            ngrams = self._make_token_sequences(doc)
+        else:
+            ngrams = self._make_ngrams(doc)
+
+        matches = self._get_all_matches(ngrams)
+
+        if best_match:
+            matches = self._select_terms(matches)
+
+        self._print_verbose_status(doc, matches)
+        
+        return matches
```

### Comparing `medspacy_quickumls-3.1a0/quickumls/install.py` & `medspacy_quickumls-3.2/quickumls/install.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-from __future__ import unicode_literals, division, print_function
-
-# built in modules
-import argparse
-import codecs
-import os
-from six.moves import input
-import shutil
-import sys
-import time
-try:
-    from unidecode import unidecode
-except ImportError:
-    pass
-
-
-# third party-dependencies
-import spacy
-
-
-# project modules
-from .toolbox import countlines, CuiSemTypesDB, SimstringDBWriter, mkdir
-from .constants import HEADERS_MRCONSO, HEADERS_MRSTY, LANGUAGES, SPACY_LANGUAGE_MAP
-
-
-def get_semantic_types(path, headers):
-    sem_types = {}
-    with codecs.open(path, encoding='utf-8') as f:
-        for i, ln in enumerate(f):
-            content = dict(zip(headers, ln.strip().split('|')))
-
-            sem_types.setdefault(content['cui'], []).append(content['sty'])
-
-    return sem_types
-
-
-def get_mrconso_iterator(path, headers, lang='ENG'):
-    with codecs.open(path, encoding='utf-8') as f:
-        for i, ln in enumerate(f):
-            content = dict(zip(headers, ln.strip().split('|')))
-
-            if content['lat'] != lang:
-                continue
-
-            yield content
-
-
-def extract_from_mrconso(
-        mrconso_path, mrsty_path, opts,
-        mrconso_header=HEADERS_MRCONSO, mrsty_header=HEADERS_MRSTY):
-
-    start = time.time()
-    print('loading semantic types...', end=' ')
-    sys.stdout.flush()
-    sem_types = get_semantic_types(mrsty_path, mrsty_header)
-    print('done in {:.2f} s'.format(time.time() - start))
-
-    start = time.time()
-
-    mrconso_iterator = get_mrconso_iterator(
-        mrconso_path, mrconso_header, opts.language
-    )
-
-    total = countlines(mrconso_path)
-
-    processed = set()
-    i = 0
-
-    for content in mrconso_iterator:
-        i += 1
-
-        if i % 100000 == 0:
-            delta = time.time() - start
-            status = (
-                '{:,} in {:.2f} s ({:.2%}, {:.1e} s / term)'
-                ''.format(i, delta, i / total, delta / i if i > 0 else 0)
-            )
-            print(status)
-
-        concept_text = content['str'].strip()
-        cui = content['cui']
-        preferred = 1 if content['ispref'] == 'Y' else 0
-
-        if opts.lowercase:
-            concept_text = concept_text.lower()
-
-        if opts.normalize_unicode:
-            concept_text = unidecode(concept_text)
-
-        if (cui, concept_text) in processed:
-            continue
-        else:
-            processed.add((cui, concept_text))
-
-        yield (concept_text, cui, sem_types[cui], preferred)
-
-    delta = time.time() - start
-    status = (
-        '\nCOMPLETED: {:,} in {:.2f} s ({:.1e} s / term)'
-        ''.format(i, delta, i / total, delta / i if i > 0 else 0)
-    )
-    print(status)
-
-
-def parse_and_encode_ngrams(extracted_it, simstring_dir, cuisty_dir, database_backend):
-    # Create destination directories for the two databases
-    mkdir(simstring_dir)
-    mkdir(cuisty_dir)
-
-    ss_db = SimstringDBWriter(simstring_dir)
-    cuisty_db = CuiSemTypesDB(cuisty_dir, database_backend=database_backend)
-
-    simstring_terms = set()
-
-    for i, (term, cui, stys, preferred) in enumerate(extracted_it, start=1):
-        if term not in simstring_terms:
-            ss_db.insert(term)
-            simstring_terms.add(term)
-
-        cuisty_db.insert(term, cui, stys, preferred)
-
-
-def install_spacy(lang):
-    """Tries to create a spacy object; if it fails, downloads the dataset"""
-
-    print(f'Determining if SpaCy for language "{lang}" is installed...')
-
-    if lang in SPACY_LANGUAGE_MAP:
-        try:
-            spacy.load(SPACY_LANGUAGE_MAP[lang])
-            print(f'SpaCy is installed and avaliable for {lang}!')
-        except OSError:
-            print(f'SpaCy is not available! Attempting to download and install...')
-            spacy.cli.download(SPACY_LANGUAGE_MAP[lang])
-    else:
-        print(f"{lang} seems not a valid model name for this spaCy version {spacy.__version__}.")
-
-
-def parse_args():
-    ap = argparse.ArgumentParser()
-    ap.add_argument(
-        'umls_installation_path',
-        help=('Location of UMLS installation files (`MRCONSO.RRF` and '
-              '`MRSTY.RRF` files)')
-    )
-    ap.add_argument(
-        'destination_path',
-        help='Location where the necessary QuickUMLS files are installed'
-    )
-    ap.add_argument(
-        '-L', '--lowercase', action='store_true',
-        help='Consider only lowercase version of tokens'
-    )
-    ap.add_argument(
-        '-U', '--normalize-unicode', action='store_true',
-        help='Normalize unicode strings to their closest ASCII representation'
-    )
-    ap.add_argument(
-        '-d', '--database-backend', choices=('unqlite',), default='unqlite',
-        help='KV database to use to store CUIs and semantic types'
-    )
-    ap.add_argument(
-        '-E', '--language', default='ENG', choices=LANGUAGES,
-        help='Extract concepts of the specified language'
-    )
-    opts = ap.parse_args()
-    return opts
-
-
-def main():
-    opts = parse_args()
-
-    install_spacy(opts.language)
-
-    if not os.path.exists(opts.destination_path):
-        msg = ('Directory "{}" does not exists; should I create it? [y/N] '
-               ''.format(opts.destination_path))
-        create = input(msg).lower().strip() == 'y'
-
-        if create:
-            os.makedirs(opts.destination_path)
-        else:
-            print('Aborting.')
-            exit(1)
-
-    if len(os.listdir(opts.destination_path)) > 0:
-        msg = ('Directory "{}" is not empty; should I empty it? [y/N] '
-               ''.format(opts.destination_path))
-        empty = input(msg).lower().strip() == 'y'
-        if empty:
-            shutil.rmtree(opts.destination_path)
-            os.mkdir(opts.destination_path)
-        else:
-            print('Aborting.')
-            exit(1)
-
-    if opts.normalize_unicode:
-        try:
-            unidecode
-        except NameError:
-            err = ('`unidecode` is needed for unicode normalization'
-                   'please install it via the `[sudo] pip install '
-                   'unidecode` command.')
-            print(err, file=sys.stderr)
-            exit(1)
-
-        flag_fp = os.path.join(opts.destination_path, 'normalize-unicode.flag')
-        open(flag_fp, 'w').close()
-
-    if opts.lowercase:
-        flag_fp = os.path.join(opts.destination_path, 'lowercase.flag')
-        open(flag_fp, 'w').close()
-
-    flag_fp = os.path.join(opts.destination_path, 'language.flag')
-    with open(flag_fp, 'w') as f:
-        f.write(opts.language)
-
-    flag_fp = os.path.join(opts.destination_path, 'database_backend.flag')
-    with open(flag_fp, 'w') as f:
-        f.write(opts.database_backend)
-
-    mrconso_path = os.path.join(opts.umls_installation_path, 'MRCONSO.RRF')
-    mrsty_path = os.path.join(opts.umls_installation_path, 'MRSTY.RRF')
-
-    mrconso_iterator = extract_from_mrconso(mrconso_path, mrsty_path, opts)
-
-    simstring_dir = os.path.join(opts.destination_path, 'umls-simstring.db')
-    cuisty_dir = os.path.join(opts.destination_path, 'cui-semtypes.db')
-
-    parse_and_encode_ngrams(mrconso_iterator, simstring_dir, cuisty_dir,
-                            database_backend=opts.database_backend)
-
-
-if __name__ == '__main__':
-    main()
+from __future__ import unicode_literals, division, print_function
+
+# built in modules
+import argparse
+import codecs
+import os
+from six.moves import input
+import shutil
+import sys
+import time
+try:
+    from unidecode import unidecode
+except ImportError:
+    pass
+
+
+# third party-dependencies
+import spacy
+
+
+# project modules
+from .toolbox import countlines, CuiSemTypesDB, SimstringDBWriter, mkdir
+from .constants import HEADERS_MRCONSO, HEADERS_MRSTY, LANGUAGES, SPACY_LANGUAGE_MAP
+
+
+def get_semantic_types(path, headers):
+    sem_types = {}
+    with codecs.open(path, encoding='utf-8') as f:
+        for i, ln in enumerate(f):
+            content = dict(zip(headers, ln.strip().split('|')))
+
+            sem_types.setdefault(content['cui'], []).append(content['sty'])
+
+    return sem_types
+
+
+def get_mrconso_iterator(path, headers, lang='ENG'):
+    with codecs.open(path, encoding='utf-8') as f:
+        for i, ln in enumerate(f):
+            content = dict(zip(headers, ln.strip().split('|')))
+
+            if content['lat'] != lang:
+                continue
+
+            yield content
+
+
+def extract_from_mrconso(
+        mrconso_path, mrsty_path, opts,
+        mrconso_header=HEADERS_MRCONSO, mrsty_header=HEADERS_MRSTY):
+
+    start = time.time()
+    print('loading semantic types...', end=' ')
+    sys.stdout.flush()
+    sem_types = get_semantic_types(mrsty_path, mrsty_header)
+    print('done in {:.2f} s'.format(time.time() - start))
+
+    start = time.time()
+
+    mrconso_iterator = get_mrconso_iterator(
+        mrconso_path, mrconso_header, opts.language
+    )
+
+    total = countlines(mrconso_path)
+
+    processed = set()
+    i = 0
+
+    for content in mrconso_iterator:
+        i += 1
+
+        if i % 100000 == 0:
+            delta = time.time() - start
+            status = (
+                '{:,} in {:.2f} s ({:.2%}, {:.1e} s / term)'
+                ''.format(i, delta, i / total, delta / i if i > 0 else 0)
+            )
+            print(status)
+
+        concept_text = content['str'].strip()
+        cui = content['cui']
+        preferred = 1 if content['ispref'] == 'Y' else 0
+
+        if opts.lowercase:
+            concept_text = concept_text.lower()
+
+        if opts.normalize_unicode:
+            concept_text = unidecode(concept_text)
+
+        if (cui, concept_text) in processed:
+            continue
+        else:
+            processed.add((cui, concept_text))
+
+        yield (concept_text, cui, sem_types[cui], preferred)
+
+    delta = time.time() - start
+    status = (
+        '\nCOMPLETED: {:,} in {:.2f} s ({:.1e} s / term)'
+        ''.format(i, delta, i / total, delta / i if i > 0 else 0)
+    )
+    print(status)
+
+
+def parse_and_encode_ngrams(extracted_it, simstring_dir, cuisty_dir, database_backend):
+    # Create destination directories for the two databases
+    mkdir(simstring_dir)
+    mkdir(cuisty_dir)
+
+    ss_db = SimstringDBWriter(simstring_dir)
+    cuisty_db = CuiSemTypesDB(cuisty_dir, database_backend=database_backend)
+
+    simstring_terms = set()
+
+    for i, (term, cui, stys, preferred) in enumerate(extracted_it, start=1):
+        if term not in simstring_terms:
+            ss_db.insert(term)
+            simstring_terms.add(term)
+
+        cuisty_db.insert(term, cui, stys, preferred)
+
+
+def install_spacy(lang):
+    """Tries to create a spacy object; if it fails, downloads the dataset"""
+
+    print(f'Determining if SpaCy for language "{lang}" is installed...')
+
+    if lang in SPACY_LANGUAGE_MAP:
+        try:
+            spacy.load(SPACY_LANGUAGE_MAP[lang])
+            print(f'SpaCy is installed and avaliable for {lang}!')
+        except OSError:
+            print(f'SpaCy is not available! Attempting to download and install...')
+            spacy.cli.download(SPACY_LANGUAGE_MAP[lang])
+    else:
+        print(f"{lang} seems not a valid model name for this spaCy version {spacy.__version__}.")
+
+
+def parse_args():
+    ap = argparse.ArgumentParser()
+    ap.add_argument(
+        'umls_installation_path',
+        help=('Location of UMLS installation files (`MRCONSO.RRF` and '
+              '`MRSTY.RRF` files)')
+    )
+    ap.add_argument(
+        'destination_path',
+        help='Location where the necessary QuickUMLS files are installed'
+    )
+    ap.add_argument(
+        '-L', '--lowercase', action='store_true',
+        help='Consider only lowercase version of tokens'
+    )
+    ap.add_argument(
+        '-U', '--normalize-unicode', action='store_true',
+        help='Normalize unicode strings to their closest ASCII representation'
+    )
+    ap.add_argument(
+        '-d', '--database-backend', choices=('unqlite',), default='unqlite',
+        help='KV database to use to store CUIs and semantic types'
+    )
+    ap.add_argument(
+        '-E', '--language', default='ENG', choices=LANGUAGES,
+        help='Extract concepts of the specified language'
+    )
+    opts = ap.parse_args()
+    return opts
+
+
+def main():
+    opts = parse_args()
+
+    install_spacy(opts.language)
+
+    if not os.path.exists(opts.destination_path):
+        msg = ('Directory "{}" does not exists; should I create it? [y/N] '
+               ''.format(opts.destination_path))
+        create = input(msg).lower().strip() == 'y'
+
+        if create:
+            os.makedirs(opts.destination_path)
+        else:
+            print('Aborting.')
+            exit(1)
+
+    if len(os.listdir(opts.destination_path)) > 0:
+        msg = ('Directory "{}" is not empty; should I empty it? [y/N] '
+               ''.format(opts.destination_path))
+        empty = input(msg).lower().strip() == 'y'
+        if empty:
+            shutil.rmtree(opts.destination_path)
+            os.mkdir(opts.destination_path)
+        else:
+            print('Aborting.')
+            exit(1)
+
+    if opts.normalize_unicode:
+        try:
+            unidecode
+        except NameError:
+            err = ('`unidecode` is needed for unicode normalization'
+                   'please install it via the `[sudo] pip install '
+                   'unidecode` command.')
+            print(err, file=sys.stderr)
+            exit(1)
+
+        flag_fp = os.path.join(opts.destination_path, 'normalize-unicode.flag')
+        open(flag_fp, 'w').close()
+
+    if opts.lowercase:
+        flag_fp = os.path.join(opts.destination_path, 'lowercase.flag')
+        open(flag_fp, 'w').close()
+
+    flag_fp = os.path.join(opts.destination_path, 'language.flag')
+    with open(flag_fp, 'w') as f:
+        f.write(opts.language)
+
+    flag_fp = os.path.join(opts.destination_path, 'database_backend.flag')
+    with open(flag_fp, 'w') as f:
+        f.write(opts.database_backend)
+
+    mrconso_path = os.path.join(opts.umls_installation_path, 'MRCONSO.RRF')
+    mrsty_path = os.path.join(opts.umls_installation_path, 'MRSTY.RRF')
+
+    mrconso_iterator = extract_from_mrconso(mrconso_path, mrsty_path, opts)
+
+    simstring_dir = os.path.join(opts.destination_path, 'umls-simstring.db')
+    cuisty_dir = os.path.join(opts.destination_path, 'cui-semtypes.db')
+
+    parse_and_encode_ngrams(mrconso_iterator, simstring_dir, cuisty_dir,
+                            database_backend=opts.database_backend)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `medspacy_quickumls-3.1a0/quickumls/server.py` & `medspacy_quickumls-3.2/quickumls/server.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from argparse import ArgumentParser
-
-from .core import QuickUMLS
-from .network import run_server
-
-
-def run_quickumls_server(opts):
-    matcher = QuickUMLS(
-        quickumls_fp=opts.quickumls_fp,
-        threshold=opts.threshold,
-        overlapping_criteria=opts.overlapping_criteria,
-        similarity_name=opts.similarity_name,
-        window=opts.window,
-        min_match_length=opts.min_match_length,
-        verbose=opts.verbose,
-        keep_uppercase=opts.keep_uppercase
-    )
-
-    run_server(matcher, host=opts.host, port=opts.port, buffersize=4096)
-
-
-def parse_args():
-    ap = ArgumentParser(
-        prog='QuickUMLS server',
-        description=(
-            'For more detailed instructions, visit '
-            'github.com/Georgetown-IR-Lab/QuickUMLS'
-        )
-    )
-
-    # required arguments
-    ap.add_argument(
-        'quickumls_fp',
-        help='directory where the QuickUMLS data files are installed.'
-    )
-
-    # server configuration
-    ap.add_argument(
-        '-H', '--host', default='localhost',
-        help='host of the server'
-    )
-    ap.add_argument(
-        '-P', '--port', default=4645, type=int,
-        help='port on which the script responds'
-    )
-
-    # QuickUMLS options
-    ap.add_argument(
-        '-t', '--threshold', default=0.7, type=float,
-        help='minimum similarity value between strings'
-    )
-    ap.add_argument(
-        '-o', '--overlapping_criteria', default='score',
-        choices=['score', 'length'],
-        help='criteria used to deal with overlapping concepts'
-    )
-
-    ap.add_argument(
-        '-s', '--similarity_name', default='jaccard',
-        choices=['dice', 'jaccard', 'cosine', 'overlap'],
-        help='name of similarity to use'
-    )
-    ap.add_argument(
-        '-w', '--window', default=5, type=int,
-        help='maximum number of tokens to consider for matching'
-    )
-    ap.add_argument(
-        '-l', '--min-match-length', default=3, type=int,
-        help='minimum length of a match'
-    )
-    ap.add_argument(
-        '-v', '--verbose', action='store_true',
-        help='return verbose information while running'
-    )
-    ap.add_argument(
-        '-u', '--keep_uppercase', action='store_true',
-        help='By default QuickUMLS converts all uppercase strings to lowercase'
-             '. This option disables that functionality, which makes QuickUMLS '
-             'useful for distinguishing acronyms from normal words. For this '
-             'the database should be installed without the -L option.'
-    )
-    return ap.parse_args()
-
-
-def main():
-    opts = parse_args()
-    run_quickumls_server(opts)
-
-
-if __name__ == '__main__':
-    main()
+from argparse import ArgumentParser
+
+from .core import QuickUMLS
+from .network import run_server
+
+
+def run_quickumls_server(opts):
+    matcher = QuickUMLS(
+        quickumls_fp=opts.quickumls_fp,
+        threshold=opts.threshold,
+        overlapping_criteria=opts.overlapping_criteria,
+        similarity_name=opts.similarity_name,
+        window=opts.window,
+        min_match_length=opts.min_match_length,
+        verbose=opts.verbose,
+        keep_uppercase=opts.keep_uppercase
+    )
+
+    run_server(matcher, host=opts.host, port=opts.port, buffersize=4096)
+
+
+def parse_args():
+    ap = ArgumentParser(
+        prog='QuickUMLS server',
+        description=(
+            'For more detailed instructions, visit '
+            'github.com/Georgetown-IR-Lab/QuickUMLS'
+        )
+    )
+
+    # required arguments
+    ap.add_argument(
+        'quickumls_fp',
+        help='directory where the QuickUMLS data files are installed.'
+    )
+
+    # server configuration
+    ap.add_argument(
+        '-H', '--host', default='localhost',
+        help='host of the server'
+    )
+    ap.add_argument(
+        '-P', '--port', default=4645, type=int,
+        help='port on which the script responds'
+    )
+
+    # QuickUMLS options
+    ap.add_argument(
+        '-t', '--threshold', default=0.7, type=float,
+        help='minimum similarity value between strings'
+    )
+    ap.add_argument(
+        '-o', '--overlapping_criteria', default='score',
+        choices=['score', 'length'],
+        help='criteria used to deal with overlapping concepts'
+    )
+
+    ap.add_argument(
+        '-s', '--similarity_name', default='jaccard',
+        choices=['dice', 'jaccard', 'cosine', 'overlap'],
+        help='name of similarity to use'
+    )
+    ap.add_argument(
+        '-w', '--window', default=5, type=int,
+        help='maximum number of tokens to consider for matching'
+    )
+    ap.add_argument(
+        '-l', '--min-match-length', default=3, type=int,
+        help='minimum length of a match'
+    )
+    ap.add_argument(
+        '-v', '--verbose', action='store_true',
+        help='return verbose information while running'
+    )
+    ap.add_argument(
+        '-u', '--keep_uppercase', action='store_true',
+        help='By default QuickUMLS converts all uppercase strings to lowercase'
+             '. This option disables that functionality, which makes QuickUMLS '
+             'useful for distinguishing acronyms from normal words. For this '
+             'the database should be installed without the -L option.'
+    )
+    return ap.parse_args()
+
+
+def main():
+    opts = parse_args()
+    run_quickumls_server(opts)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `medspacy_quickumls-3.1a0/quickumls/spacy_component.py` & `medspacy_quickumls-3.2/quickumls/spacy_component.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-from sys import platform
-from os import path
-from pathlib import Path
-from typing import Literal
-
-import spacy
-from spacy.tokens import Span
-from spacy.strings import StringStore
-from spacy.language import Language
-
-from .core import QuickUMLS
-from . import constants
-from .umls_match import UmlsMatch
-from .constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
-
-@Language.factory("medspacy_quickumls")
-class SpacyQuickUMLS(object):
-
-    def __init__(self, nlp, name = "medspacy_quickumls", quickumls_fp=None,
-                 overlapping_criteria='score',
-                 threshold=0.7,
-                 window=5,
-                 similarity_name='jaccard',
-                 min_match_length=3,
-                 accepted_semtypes=constants.ACCEPTED_SEMTYPES,
-                 verbose=False,
-                 keep_uppercase=False,
-                 best_match=True,
-                 ignore_syntax=False,
-                 result_type: Literal["ents", "group"] = "ents",
-                 span_group_name: str = MEDSPACY_DEFAULT_SPAN_GROUP_NAME,
-                 ):
-        """Instantiate SpacyQuickUMLS object
-
-            This creates a QuickUMLS spaCy component which can be used in modular pipelines.  
-            This module adds either entity Spans (default) or Span Groups to the document where the  label is the UMLS CUI and the Span's
-                "underscore" object is extended to contain additional information about matched concepts.
-            Note that this implementation follows and enforces a known spacy convention on entities
-                that entity Spans cannot overlap on a single token.  If SpanGroups are selected instead, they may overlap
-
-        Args:
-            nlp: Existing spaCy pipeline.  This is needed to update the vocabulary with UMLS CUI values
-            quickumls_fp (str): Path to QuickUMLS data
-            overlapping_criteria (str, optional):
-                    One of "score" or "length". Choose how results are ranked.
-                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
-            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
-            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
-            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
-                    Similarity measure to be used. Defaults to 'jaccard'.
-            min_match_length (int, optional): TODO: ??. Defaults to 3.
-            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
-                Semantic types are identified by the letter "T" followed by three numbers
-                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
-                Defaults to constants.ACCEPTED_SEMTYPES.
-            verbose (bool, optional): TODO:??. Defaults to False.
-            keep_uppercase (bool, optional): By default QuickUMLS converts all
-                    uppercase strings to lowercase. This option disables that
-                    functionality, which makes QuickUMLS useful for
-                    distinguishing acronyms from normal words. For this the
-                    database should be installed without the -L option.
-                    Defaults to False.
-            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
-            ignore_syntax (bool, optional): Whether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
-            result_type: "ents" (default), or "group". Determines where component will put the matched spans.
-                "ents" will add spans to doc.ents and add to any existing entities, but does not allow overlapping.
-                "group" will add spans to doc.spans under the specified group name.
-            span_group_name: The name of the span group used to store results when result_type is "group". Default is
-                "medspacy_spans".
-        """
-
-        if quickumls_fp is None:
-            # let's use a default sample that we provide in medspacy
-            # NOTE: Currently QuickUMLS uses an older fork of simstring where databases
-            # cannot be shared between Windows and POSIX systems so we distribute the sample for both:
-
-            quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_POSIX_unqlite"
-            if platform.startswith("win"):
-                quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_Windows_unqlite"
-
-            quickumls_fp = path.join(
-                Path(__file__).resolve().parents[1], "resources", "quickumls/{0}".format(quickumls_platform_dir)
-            )
-            print("Loading QuickUMLS resources from a default SAMPLE of UMLS data from here: {}".format(quickumls_fp))
-        
-        self.quickumls = QuickUMLS(quickumls_fp, 
-            # By default, the QuickUMLS objects creates its own internal spacy pipeline but this is not needed
-            # when we're using it as a component in a pipeline
-            spacy_component = True,
-            overlapping_criteria=overlapping_criteria,
-            threshold=threshold,
-            window=window,
-            similarity_name=similarity_name,
-            min_match_length=min_match_length,
-            accepted_semtypes=accepted_semtypes,
-            verbose=verbose,
-            keep_uppercase=keep_uppercase
-            )
-        
-        # save this off so that we can get vocab values of labels later
-        self.nlp = nlp
-        self.name = name
-        
-        # keep these for matching
-        self.best_match = best_match
-        self.ignore_syntax = ignore_syntax
-        self.verbose = verbose
-
-        self._result_type = result_type
-        self._span_group_name = span_group_name
-
-        # let's extend this with some proprties that we want
-        # NOTE: These two might be deprecated at some point since we now have
-        # umls_matches below which contains more information and enables overlapping
-        if not Span.has_extension("similarity"):
-            Span.set_extension('similarity', default = -1.0)
-        if not Span.has_extension("semtypes"): 
-            Span.set_extension('semtypes', default = -1.0)
-
-        # match objects are a set, since span objects with the same start/end keys
-        # would have the same values for custom attributes in spacy
-        if not Span.has_extension("umls_matches"):
-            Span.set_extension('umls_matches', default=set())
-
-    @property
-    def result_type(self) -> str:
-        """
-        The result type of the component. "ents" indicates that calling TargetMatcher will store the results in
-        doc.ents, "group" indicates that the results will be stored in the span group indicated by `span_group_name`,
-
-        Returns:
-            The result type string.
-        """
-        return self._result_type
-
-    @result_type.setter
-    def result_type(self, result_type: Literal["ents", "group"]):
-        if not (result_type == "group" or result_type == "ents"):
-            raise ValueError('result_type must be "ents", or "group".')
-        self._result_type = result_type
-
-    @property
-    def span_group_name(self) -> str:
-        """
-        The name of the span group used by this component. If `result_type` is "group", calling this component will
-        place results in the span group with this name.
-
-        Returns:
-            The span group name.
-        """
-        return self._span_group_name
-
-    @span_group_name.setter
-    def span_group_name(self, name: str):
-        if not name or not isinstance(name, str):
-            raise ValueError("Span group name must be a string.")
-        self._span_group_name = name
-        
-    def __call__(self, doc):
-        # pass in the document which has been parsed to this point in the pipeline for ngrams and matches
-        matches = self.quickumls._match(doc, best_match=self.best_match, ignore_syntax=self.ignore_syntax)
-        
-        # NOTE: Spacy spans do not allow overlapping tokens, so we prevent the overlap here
-        # For more information, see: https://github.com/explosion/spaCy/issues/3608
-        tokens_in_ents_set = set()
-
-        if self.result_type.lower() == "group":
-            # set up an empty list if there are no spans yet
-            doc.spans.setdefault(self.span_group_name, [])
-        
-        # let's track any other entities which may have been attached via upstream components
-        for ent in doc.ents:
-            for token_index in range(ent.start, ent.end):
-                tokens_in_ents_set.add(token_index)
-        
-        # Convert QuickUMLS match objects into Spans
-        for match in matches:
-            # each match may match multiple ngrams
-            for ngram_match_dict in match:
-                start_char_idx = int(ngram_match_dict['start'])
-                end_char_idx = int(ngram_match_dict['end'])
-                
-                cui = ngram_match_dict['cui']
-                # add the string to the spacy vocab
-                self.nlp.vocab.strings.add(cui)
-                # pull out the value
-                cui_label_value = self.nlp.vocab.strings[cui]
-                
-                # char_span() creates a Span from these character indices
-                # UMLS CUI should work well as the label here
-                span = doc.char_span(start_char_idx, end_char_idx, label = cui_label_value)
-                
-                # before we add this, let's make sure that this entity does not overlap any tokens added thus far
-                candidate_token_indexes = set(range(span.start, span.end))
-                
-                # check the intersection and skip this if there is any overlap
-                if self.result_type.lower() == "ents" and len(tokens_in_ents_set.intersection(candidate_token_indexes)) > 0:
-                    continue
-                    
-                # track this to make sure we do not introduce overlap later
-                tokens_in_ents_set.update(candidate_token_indexes)
-                
-                # add some custom metadata to the spans
-                span._.similarity = ngram_match_dict['similarity']
-                span._.semtypes = ngram_match_dict['semtypes']
-
-                # let's create this more fully featured match object
-                umls_match = UmlsMatch(cui,
-                                       ngram_match_dict['semtypes'],
-                                       ngram_match_dict['similarity'])
-
-                span._.umls_matches.add(umls_match)
-
-                if self.result_type.lower() == "ents":
-                    doc.ents = list(doc.ents) + [span]
-                elif self.result_type.lower() == "group":
-                    doc.spans[self.span_group_name].append(span)
-                
-        return doc
+from sys import platform
+from os import path
+from pathlib import Path
+from typing import Literal
+
+import spacy
+from spacy.tokens import Span
+from spacy.strings import StringStore
+from spacy.language import Language
+
+from .core import QuickUMLS
+from . import constants
+from .umls_match import UmlsMatch
+from .constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
+
+@Language.factory("medspacy_quickumls")
+class SpacyQuickUMLS(object):
+
+    def __init__(self, nlp, name = "medspacy_quickumls", quickumls_fp=None,
+                 overlapping_criteria='score',
+                 threshold=0.7,
+                 window=5,
+                 similarity_name='jaccard',
+                 min_match_length=3,
+                 accepted_semtypes=constants.ACCEPTED_SEMTYPES,
+                 verbose=False,
+                 keep_uppercase=False,
+                 best_match=True,
+                 ignore_syntax=False,
+                 result_type: Literal["ents", "group"] = "ents",
+                 span_group_name: str = MEDSPACY_DEFAULT_SPAN_GROUP_NAME,
+                 ):
+        """Instantiate SpacyQuickUMLS object
+
+            This creates a QuickUMLS spaCy component which can be used in modular pipelines.  
+            This module adds either entity Spans (default) or Span Groups to the document where the  label is the UMLS CUI and the Span's
+                "underscore" object is extended to contain additional information about matched concepts.
+            Note that this implementation follows and enforces a known spacy convention on entities
+                that entity Spans cannot overlap on a single token.  If SpanGroups are selected instead, they may overlap
+
+        Args:
+            nlp: Existing spaCy pipeline.  This is needed to update the vocabulary with UMLS CUI values
+            quickumls_fp (str): Path to QuickUMLS data
+            overlapping_criteria (str, optional):
+                    One of "score" or "length". Choose how results are ranked.
+                    Choose "score" for best matching score first or "length" for longest match first.. Defaults to 'score'.
+            threshold (float, optional): Minimum similarity between strings. Defaults to 0.7.
+            window (int, optional): Maximum amount of tokens to consider for matching. Defaults to 5.
+            similarity_name (str, optional): One of "dice", "jaccard", "cosine", or "overlap".
+                    Similarity measure to be used. Defaults to 'jaccard'.
+            min_match_length (int, optional): TODO: ??. Defaults to 3.
+            accepted_semtypes (List[str], optional): Set of UMLS semantic types concepts should belong to.
+                Semantic types are identified by the letter "T" followed by three numbers
+                (e.g., "T131", which identifies the type "Hazardous or Poisonous Substance").
+                Defaults to constants.ACCEPTED_SEMTYPES.
+            verbose (bool, optional): TODO:??. Defaults to False.
+            keep_uppercase (bool, optional): By default QuickUMLS converts all
+                    uppercase strings to lowercase. This option disables that
+                    functionality, which makes QuickUMLS useful for
+                    distinguishing acronyms from normal words. For this the
+                    database should be installed without the -L option.
+                    Defaults to False.
+            best_match (bool, optional): Whether to return only the top match or all overlapping candidates. Defaults to True.
+            ignore_syntax (bool, optional): Whether to use the heuristcs introduced in the paper (Soldaini and Goharian, 2016). TODO: clarify,. Defaults to False
+            result_type: "ents" (default), or "group". Determines where component will put the matched spans.
+                "ents" will add spans to doc.ents and add to any existing entities, but does not allow overlapping.
+                "group" will add spans to doc.spans under the specified group name.
+            span_group_name: The name of the span group used to store results when result_type is "group". Default is
+                "medspacy_spans".
+        """
+
+        if quickumls_fp is None:
+            # let's use a default sample that we provide in medspacy
+            # NOTE: Currently QuickUMLS uses an older fork of simstring where databases
+            # cannot be shared between Windows and POSIX systems so we distribute the sample for both:
+
+            quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_POSIX_unqlite"
+            if platform.startswith("win"):
+                quickumls_platform_dir = "QuickUMLS_SAMPLE_lowercase_Windows_unqlite"
+
+            quickumls_fp = path.join(
+                Path(__file__).resolve().parents[1], "resources", "quickumls/{0}".format(quickumls_platform_dir)
+            )
+            print("Loading QuickUMLS resources from a default SAMPLE of UMLS data from here: {}".format(quickumls_fp))
+        
+        self.quickumls = QuickUMLS(quickumls_fp, 
+            # By default, the QuickUMLS objects creates its own internal spacy pipeline but this is not needed
+            # when we're using it as a component in a pipeline
+            spacy_component = True,
+            overlapping_criteria=overlapping_criteria,
+            threshold=threshold,
+            window=window,
+            similarity_name=similarity_name,
+            min_match_length=min_match_length,
+            accepted_semtypes=accepted_semtypes,
+            verbose=verbose,
+            keep_uppercase=keep_uppercase
+            )
+        
+        # save this off so that we can get vocab values of labels later
+        self.nlp = nlp
+        self.name = name
+        
+        # keep these for matching
+        self.best_match = best_match
+        self.ignore_syntax = ignore_syntax
+        self.verbose = verbose
+
+        self._result_type = result_type
+        self._span_group_name = span_group_name
+
+        # let's extend this with some proprties that we want
+        # NOTE: These two might be deprecated at some point since we now have
+        # umls_matches below which contains more information and enables overlapping
+        if not Span.has_extension("similarity"):
+            Span.set_extension('similarity', default = -1.0)
+        if not Span.has_extension("semtypes"): 
+            Span.set_extension('semtypes', default = -1.0)
+
+        # match objects are a set, since span objects with the same start/end keys
+        # would have the same values for custom attributes in spacy
+        if not Span.has_extension("umls_matches"):
+            Span.set_extension('umls_matches', default=set())
+
+    @property
+    def result_type(self) -> str:
+        """
+        The result type of the component. "ents" indicates that calling TargetMatcher will store the results in
+        doc.ents, "group" indicates that the results will be stored in the span group indicated by `span_group_name`,
+
+        Returns:
+            The result type string.
+        """
+        return self._result_type
+
+    @result_type.setter
+    def result_type(self, result_type: Literal["ents", "group"]):
+        if not (result_type == "group" or result_type == "ents"):
+            raise ValueError('result_type must be "ents", or "group".')
+        self._result_type = result_type
+
+    @property
+    def span_group_name(self) -> str:
+        """
+        The name of the span group used by this component. If `result_type` is "group", calling this component will
+        place results in the span group with this name.
+
+        Returns:
+            The span group name.
+        """
+        return self._span_group_name
+
+    @span_group_name.setter
+    def span_group_name(self, name: str):
+        if not name or not isinstance(name, str):
+            raise ValueError("Span group name must be a string.")
+        self._span_group_name = name
+        
+    def __call__(self, doc):
+        # pass in the document which has been parsed to this point in the pipeline for ngrams and matches
+        matches = self.quickumls._match(doc, best_match=self.best_match, ignore_syntax=self.ignore_syntax)
+        
+        # NOTE: Spacy spans do not allow overlapping tokens, so we prevent the overlap here
+        # For more information, see: https://github.com/explosion/spaCy/issues/3608
+        tokens_in_ents_set = set()
+
+        if self.result_type.lower() == "group":
+            # set up an empty list if there are no spans yet
+            doc.spans.setdefault(self.span_group_name, [])
+        
+        # let's track any other entities which may have been attached via upstream components
+        for ent in doc.ents:
+            for token_index in range(ent.start, ent.end):
+                tokens_in_ents_set.add(token_index)
+        
+        # Convert QuickUMLS match objects into Spans
+        for match in matches:
+            # each match may match multiple ngrams
+            for ngram_match_dict in match:
+                start_char_idx = int(ngram_match_dict['start'])
+                end_char_idx = int(ngram_match_dict['end'])
+                
+                cui = ngram_match_dict['cui']
+                # add the string to the spacy vocab
+                self.nlp.vocab.strings.add(cui)
+                # pull out the value
+                cui_label_value = self.nlp.vocab.strings[cui]
+                
+                # char_span() creates a Span from these character indices
+                # UMLS CUI should work well as the label here
+                span = doc.char_span(start_char_idx, end_char_idx, label = cui_label_value)
+                
+                # before we add this, let's make sure that this entity does not overlap any tokens added thus far
+                candidate_token_indexes = set(range(span.start, span.end))
+                
+                # check the intersection and skip this if there is any overlap
+                if self.result_type.lower() == "ents" and len(tokens_in_ents_set.intersection(candidate_token_indexes)) > 0:
+                    continue
+                    
+                # track this to make sure we do not introduce overlap later
+                tokens_in_ents_set.update(candidate_token_indexes)
+                
+                # add some custom metadata to the spans
+                span._.similarity = ngram_match_dict['similarity']
+                span._.semtypes = ngram_match_dict['semtypes']
+
+                # let's create this more fully featured match object
+                umls_match = UmlsMatch(cui,
+                                       ngram_match_dict['semtypes'],
+                                       ngram_match_dict['similarity'])
+
+                span._.umls_matches.add(umls_match)
+
+                if self.result_type.lower() == "ents":
+                    doc.ents = list(doc.ents) + [span]
+                elif self.result_type.lower() == "group":
+                    doc.spans[self.span_group_name].append(span)
+                
+        return doc
```

### Comparing `medspacy_quickumls-3.1a0/quickumls/toolbox.py` & `medspacy_quickumls-3.2/quickumls/toolbox.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-from __future__ import unicode_literals, division, print_function
-
-# build-in modules
-import re
-import os
-from functools import wraps
-import six
-import unicodedata
-from string import punctuation
-from itertools import takewhile, repeat
-from six.moves import xrange
-
-# installed modules
-import numpy
-
-try:
-    import unqlite
-    UNQLITE_AVAILABLE = True
-except ImportError:
-    UNQLITE_AVAILABLE = False
-
-# project imports
-from pysimstring import simstring
-
-
-# Python version specific imports
-if six.PY2:
-    import cPickle as pickle
-else:
-    import pickle
-
-
-def pickle_loading(data):
-    pass
-
-
-def pickle_dumping(data):
-    pass
-
-
-def mkdir(path):
-    try:
-        os.makedirs(path)
-        return True
-    except OSError:
-        return False
-
-
-def count_ngrams(s, n):
-    return len(s) + n - 1
-
-
-def safe_unicode(s):
-    if six.PY2:
-        # in python 3, there no ambiguity on whether
-        # a string is encoded in bytes format or not
-        try:
-            s = u'%s' % s
-        except UnicodeDecodeError:
-            s = u'%s' % s.decode('utf-8')
-
-    return u'{}'.format(unicodedata.normalize('NFKD', s))
-
-
-def prepare_string_for_db_input(s):
-    if six.PY2:
-        return s.encode('utf-8')
-    else:
-        return s
-
-
-def make_ngrams(s, n):
-    # s = u'{t}{s}{t}'.format(s=safe_unicode(s), t=('$' * (n - 1)))
-    n = len(s) if len(s) < n else n
-    return (s[i:i + n] for i in xrange(len(s) - n + 1))
-
-
-def get_similarity(x, y, n, similarity_name):
-    if len(x) == 0 or len(y) == 0:
-        # we define similarity between two strings
-        # to be 0 if any of the two is empty.
-        return 0.
-
-    X, Y = set(make_ngrams(x, n)), set(make_ngrams(y, n))
-    intersec = len(X.intersection(Y))
-
-    if similarity_name == 'dice':
-        return 2 * intersec / (len(X) + len(Y))
-    elif similarity_name == 'jaccard':
-        return intersec / (len(X) + len(Y) - intersec)
-    elif similarity_name == 'cosine':
-        return intersec / numpy.sqrt(len(X) * len(Y))
-    elif similarity_name == 'overlap':
-        return intersec
-    else:
-        msg = 'Similarity {} not recognized'.format(similarity_name)
-        raise TypeError(msg)
-
-
-class SimpleTokenizer(object):
-    def __init__(self, stopwords=None, min_length=1, split_sym=None):
-        if stopwords == 'default':
-            stopwords = [
-                'a', 'an', 'and', 'are', 'as', 'at', 'be', 'by', 'for',
-                'from', 'has', 'he', 'in', 'is', 'its', 'of', 'on', 'or',
-                'that', 'the', 'to', 'was ', 'were', 'will', 'with'
-            ]
-        elif stopwords is None:
-            stopwords = []
-
-        self.stopwords = set(stopwords)
-
-        if split_sym is None:
-            split_sym = []
-
-        split_sym = punctuation + ''.join(split_sym)
-
-        self.min_length = min_length
-        self.re_tokenize = re.compile(r'&\w+;|\W+|_')
-
-    def tokenize(self, text, lower=True):
-        """Tokenize text"""
-        if lower:
-            text = text.lower()
-        for tok in self.re_tokenize.split(text):
-            if len(tok) >= self.min_length and tok not in self.stopwords:
-                yield tok
-
-    def tokenize_list(self, text, lower=True):
-        if lower:
-            text = text.lower()
-        return [
-            tok for tok in self.re_tokenize.split(text)
-            if len(tok) >= self.min_length and tok not in self.stopwords
-        ]
-
-
-def db_key_encode(term):
-    if six.PY2:
-        return term
-    else:
-        return term.encode('utf-8')
-
-
-def countlines(fn):
-    """Count lines in fn. Slightly modified version of
-    http://stackoverflow.com/a/27518377"""
-    with open(fn, 'rb') as f:
-        bufgen = takewhile(
-            lambda x: x, (f.read(1024 * 1024) for _ in repeat(None)))
-        ln = sum(buf.count(b'\n') for buf in bufgen)
-    return ln
-
-
-class SimstringDBWriter(object):
-    def __init__(self, path):
-
-        if not(os.path.exists(path)) or not(os.path.isdir(path)):
-            err_msg = (
-                '"{}" does not exists or it is not a directory.'
-            ).format(path)
-            raise IOError(err_msg)
-        else:
-            try:
-                os.makedirs(path)
-            except OSError:
-                pass
-
-        self.db = simstring.writer(
-            prepare_string_for_db_input(
-                os.path.join(path, 'umls-terms.simstring')
-            ),
-            3, False, True
-        )
-
-    def insert(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        self.db.insert(term)
-
-
-class SimstringDBReader(object):
-    def __init__(self, path, similarity_name, threshold):
-        if not(os.path.exists(path)) or not(os.path.isdir(path)):
-            err_msg = (
-                '"{}" does not exists or it is not a directory.'
-            ).format(path)
-            raise IOError(err_msg)
-
-        self.db = simstring.reader(
-            prepare_string_for_db_input(
-                os.path.join(path, 'umls-terms.simstring')
-            )
-        )
-        self.db.measure = getattr(simstring, similarity_name)
-        self.db.threshold = threshold
-
-    def get(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        return self.db.retrieve(term)
-
-
-class Intervals(object):
-    def __init__(self):
-        self.intervals = []
-
-    def _is_overlapping_intervals(self, a, b):
-        if b[0] < a[1] and b[1] > a[0]:
-            return True
-        elif a[0] < b[1] and a[1] > b[0]:
-            return True
-        else:
-            return False
-
-    def __contains__(self, interval):
-        return any(
-            self._is_overlapping_intervals(interval, other)
-            for other in self.intervals
-        )
-
-    def append(self, interval):
-        self.intervals.append(interval)
-
-
-class CuiSemTypesDB(object):
-    def __init__(self, path, database_backend='unqlite'):
-        if not (os.path.exists(path) or os.path.isdir(path)):
-            err_msg = (
-                '"{}" is not a valid directory').format(path)
-            raise IOError(err_msg)
-
-        if database_backend == 'unqlite':
-            assert UNQLITE_AVAILABLE, (
-                'You selected unqlite as database backend, but it is not '
-                'installed. Please install it via `pip install unqlite`'
-            )
-            self.cui_db = unqlite.UnQLite(os.path.join(path, 'cui.unqlite'))
-            self.cui_db_put = self.cui_db.store
-            self.cui_db_get = self.cui_db.fetch
-            self.semtypes_db = unqlite.UnQLite(os.path.join(path, 'semtypes.unqlite'))
-            self.semtypes_db_put = self.semtypes_db.store
-            self.semtypes_db_get = self.semtypes_db.fetch
-        elif database_backend == 'leveldb':
-            raise ValueError(f'database_backend {database_backend} is no longer supported')
-        else:
-            raise ValueError(f'database_backend {database_backend} not recognized')
-
-    def has_term(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        try:
-            self.cui_db_get(db_key_encode(term))
-            return True
-        except KeyError:
-            return
-
-    def insert(self, term, cui, semtypes, is_preferred):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        cui = prepare_string_for_db_input(safe_unicode(cui))
-
-        # some terms have multiple cuis associated with them,
-        # so we store them all
-        try:
-            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
-        except KeyError:
-            cuis = set()
-
-        cuis.add((cui, is_preferred))
-        self.cui_db_put(db_key_encode(term), pickle.dumps(cuis))
-
-        try:
-            self.semtypes_db_get(db_key_encode(cui))
-        except KeyError:
-            self.semtypes_db_put(
-                db_key_encode(cui), pickle.dumps(set(semtypes))
-            )
-
-    def get(self, term):
-        term = prepare_string_for_db_input(safe_unicode(term))
-        try:
-            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
-        except KeyError:
-            cuis = set()
-
-        matches = (
-            (
-                cui,
-                pickle.loads(self.semtypes_db_get(db_key_encode(cui))),
-                is_preferred
-            )
-            for cui, is_preferred in cuis
-        )
-        return matches
+from __future__ import unicode_literals, division, print_function
+
+# build-in modules
+import re
+import os
+from functools import wraps
+import six
+import unicodedata
+from string import punctuation
+from itertools import takewhile, repeat
+from six.moves import xrange
+
+# installed modules
+import numpy
+
+try:
+    import unqlite
+    UNQLITE_AVAILABLE = True
+except ImportError:
+    UNQLITE_AVAILABLE = False
+
+# project imports
+from pysimstring import simstring
+
+
+# Python version specific imports
+if six.PY2:
+    import cPickle as pickle
+else:
+    import pickle
+
+
+def pickle_loading(data):
+    pass
+
+
+def pickle_dumping(data):
+    pass
+
+
+def mkdir(path):
+    try:
+        os.makedirs(path)
+        return True
+    except OSError:
+        return False
+
+
+def count_ngrams(s, n):
+    return len(s) + n - 1
+
+
+def safe_unicode(s):
+    if six.PY2:
+        # in python 3, there no ambiguity on whether
+        # a string is encoded in bytes format or not
+        try:
+            s = u'%s' % s
+        except UnicodeDecodeError:
+            s = u'%s' % s.decode('utf-8')
+
+    return u'{}'.format(unicodedata.normalize('NFKD', s))
+
+
+def prepare_string_for_db_input(s):
+    if six.PY2:
+        return s.encode('utf-8')
+    else:
+        return s
+
+
+def make_ngrams(s, n):
+    # s = u'{t}{s}{t}'.format(s=safe_unicode(s), t=('$' * (n - 1)))
+    n = len(s) if len(s) < n else n
+    return (s[i:i + n] for i in xrange(len(s) - n + 1))
+
+
+def get_similarity(x, y, n, similarity_name):
+    if len(x) == 0 or len(y) == 0:
+        # we define similarity between two strings
+        # to be 0 if any of the two is empty.
+        return 0.
+
+    X, Y = set(make_ngrams(x, n)), set(make_ngrams(y, n))
+    intersec = len(X.intersection(Y))
+
+    if similarity_name == 'dice':
+        return 2 * intersec / (len(X) + len(Y))
+    elif similarity_name == 'jaccard':
+        return intersec / (len(X) + len(Y) - intersec)
+    elif similarity_name == 'cosine':
+        return intersec / numpy.sqrt(len(X) * len(Y))
+    elif similarity_name == 'overlap':
+        return intersec
+    else:
+        msg = 'Similarity {} not recognized'.format(similarity_name)
+        raise TypeError(msg)
+
+
+class SimpleTokenizer(object):
+    def __init__(self, stopwords=None, min_length=1, split_sym=None):
+        if stopwords == 'default':
+            stopwords = [
+                'a', 'an', 'and', 'are', 'as', 'at', 'be', 'by', 'for',
+                'from', 'has', 'he', 'in', 'is', 'its', 'of', 'on', 'or',
+                'that', 'the', 'to', 'was ', 'were', 'will', 'with'
+            ]
+        elif stopwords is None:
+            stopwords = []
+
+        self.stopwords = set(stopwords)
+
+        if split_sym is None:
+            split_sym = []
+
+        split_sym = punctuation + ''.join(split_sym)
+
+        self.min_length = min_length
+        self.re_tokenize = re.compile(r'&\w+;|\W+|_')
+
+    def tokenize(self, text, lower=True):
+        """Tokenize text"""
+        if lower:
+            text = text.lower()
+        for tok in self.re_tokenize.split(text):
+            if len(tok) >= self.min_length and tok not in self.stopwords:
+                yield tok
+
+    def tokenize_list(self, text, lower=True):
+        if lower:
+            text = text.lower()
+        return [
+            tok for tok in self.re_tokenize.split(text)
+            if len(tok) >= self.min_length and tok not in self.stopwords
+        ]
+
+
+def db_key_encode(term):
+    if six.PY2:
+        return term
+    else:
+        return term.encode('utf-8')
+
+
+def countlines(fn):
+    """Count lines in fn. Slightly modified version of
+    http://stackoverflow.com/a/27518377"""
+    with open(fn, 'rb') as f:
+        bufgen = takewhile(
+            lambda x: x, (f.read(1024 * 1024) for _ in repeat(None)))
+        ln = sum(buf.count(b'\n') for buf in bufgen)
+    return ln
+
+
+class SimstringDBWriter(object):
+    def __init__(self, path):
+
+        if not(os.path.exists(path)) or not(os.path.isdir(path)):
+            err_msg = (
+                '"{}" does not exists or it is not a directory.'
+            ).format(path)
+            raise IOError(err_msg)
+        else:
+            try:
+                os.makedirs(path)
+            except OSError:
+                pass
+
+        self.db = simstring.writer(
+            prepare_string_for_db_input(
+                os.path.join(path, 'umls-terms.simstring')
+            ),
+            3, False, True
+        )
+
+    def insert(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        self.db.insert(term)
+
+
+class SimstringDBReader(object):
+    def __init__(self, path, similarity_name, threshold):
+        if not(os.path.exists(path)) or not(os.path.isdir(path)):
+            err_msg = (
+                '"{}" does not exists or it is not a directory.'
+            ).format(path)
+            raise IOError(err_msg)
+
+        self.db = simstring.reader(
+            prepare_string_for_db_input(
+                os.path.join(path, 'umls-terms.simstring')
+            )
+        )
+        self.db.measure = getattr(simstring, similarity_name)
+        self.db.threshold = threshold
+
+    def get(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        return self.db.retrieve(term)
+
+
+class Intervals(object):
+    def __init__(self):
+        self.intervals = []
+
+    def _is_overlapping_intervals(self, a, b):
+        if b[0] < a[1] and b[1] > a[0]:
+            return True
+        elif a[0] < b[1] and a[1] > b[0]:
+            return True
+        else:
+            return False
+
+    def __contains__(self, interval):
+        return any(
+            self._is_overlapping_intervals(interval, other)
+            for other in self.intervals
+        )
+
+    def append(self, interval):
+        self.intervals.append(interval)
+
+
+class CuiSemTypesDB(object):
+    def __init__(self, path, database_backend='unqlite'):
+        if not (os.path.exists(path) or os.path.isdir(path)):
+            err_msg = (
+                '"{}" is not a valid directory').format(path)
+            raise IOError(err_msg)
+
+        if database_backend == 'unqlite':
+            assert UNQLITE_AVAILABLE, (
+                'You selected unqlite as database backend, but it is not '
+                'installed. Please install it via `pip install unqlite`'
+            )
+            self.cui_db = unqlite.UnQLite(os.path.join(path, 'cui.unqlite'))
+            self.cui_db_put = self.cui_db.store
+            self.cui_db_get = self.cui_db.fetch
+            self.semtypes_db = unqlite.UnQLite(os.path.join(path, 'semtypes.unqlite'))
+            self.semtypes_db_put = self.semtypes_db.store
+            self.semtypes_db_get = self.semtypes_db.fetch
+        elif database_backend == 'leveldb':
+            raise ValueError(f'database_backend {database_backend} is no longer supported')
+        else:
+            raise ValueError(f'database_backend {database_backend} not recognized')
+
+    def has_term(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        try:
+            self.cui_db_get(db_key_encode(term))
+            return True
+        except KeyError:
+            return
+
+    def insert(self, term, cui, semtypes, is_preferred):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        cui = prepare_string_for_db_input(safe_unicode(cui))
+
+        # some terms have multiple cuis associated with them,
+        # so we store them all
+        try:
+            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
+        except KeyError:
+            cuis = set()
+
+        cuis.add((cui, is_preferred))
+        self.cui_db_put(db_key_encode(term), pickle.dumps(cuis))
+
+        try:
+            self.semtypes_db_get(db_key_encode(cui))
+        except KeyError:
+            self.semtypes_db_put(
+                db_key_encode(cui), pickle.dumps(set(semtypes))
+            )
+
+    def get(self, term):
+        term = prepare_string_for_db_input(safe_unicode(term))
+        try:
+            cuis = pickle.loads(self.cui_db_get(db_key_encode(term)))
+        except KeyError:
+            cuis = set()
+
+        matches = (
+            (
+                cui,
+                pickle.loads(self.semtypes_db_get(db_key_encode(cui))),
+                is_preferred
+            )
+            for cui, is_preferred in cuis
+        )
+        return matches
```

### Comparing `medspacy_quickumls-3.1a0/quickumls/umls_match.py` & `medspacy_quickumls-3.2/quickumls/umls_match.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Set
-
-
-class UmlsMatch:
-
-    def __init__(self,
-                 cui: str,
-                 semtypes: Set[str],
-                 similarity: float):
-        """Instantiate UmlsMatch object
-
-                    This creates a QuickUMLS spaCy component which can be used in modular pipelines.
-                    This module adds entity Spans to the document where the entity label is the UMLS CUI and the Span's "underscore" object is extended to contains "similarity" and "semtypes" for matched concepts.
-                    Note that this implementation follows and enforces a known spacy convention that entity Spans cannot overlap on a single token.
-
-                Args:
-                    cui: UMLS controlled unique identifier (CUI) value (e.g., "C0243095")
-                    semtypes (Set[str]): List of UMLS semantic types as Type Unique Identifier values (TUI)
-                            for this matched concept (e.g., "T203")
-                    similarity (float): Similarity score between match and UMLS concept
-                """
-        self.cui = cui
-        self.semtypes = semtypes
-        self.similarity = similarity
+from typing import Set
+
+
+class UmlsMatch:
+
+    def __init__(self,
+                 cui: str,
+                 semtypes: Set[str],
+                 similarity: float):
+        """Instantiate UmlsMatch object
+
+                    This creates a QuickUMLS spaCy component which can be used in modular pipelines.
+                    This module adds entity Spans to the document where the entity label is the UMLS CUI and the Span's "underscore" object is extended to contains "similarity" and "semtypes" for matched concepts.
+                    Note that this implementation follows and enforces a known spacy convention that entity Spans cannot overlap on a single token.
+
+                Args:
+                    cui: UMLS controlled unique identifier (CUI) value (e.g., "C0243095")
+                    semtypes (Set[str]): List of UMLS semantic types as Type Unique Identifier values (TUI)
+                            for this matched concept (e.g., "T203")
+                    similarity (float): Similarity score between match and UMLS concept
+                """
+        self.cui = cui
+        self.semtypes = semtypes
+        self.similarity = similarity
```

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy_quickumls-3.2/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/setup.py` & `medspacy_quickumls-3.2/setup.py`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/tests/init_db.py` & `medspacy_quickumls-3.2/tests/init_db.py`

 * *Files identical despite different names*

### Comparing `medspacy_quickumls-3.1a0/tests/skiptest_spangroup1.py` & `medspacy_quickumls-3.2/tests/test_quickumls_component.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,78 @@
-import unittest
-from quickumls import spacy_component
-import spacy
-from quickumls.constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
-from pathlib import Path
-"""
-This test won't pass when tested with others in pytest tests. Skip it for now.
-"""
-class TestSpanGoup1(unittest.TestCase):
-    
-    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
-    @classmethod
-    def setUpClass(cls):
-        """Create sample db on the fly, to avoid os dependent path issue.
-        """
-        from .init_db import init
-        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)        
-
-
-    def test_span_groups(self):
-        """
-        Test that span groups can bs used as a result type (as opposed to entities)
-        """
-
-        # let's make sure that this pipe has been initialized
-        # At least for MacOS and Linux which are currently supported...
-
-        # allow default QuickUMLS (very small sample data) to be loaded
-        nlp = spacy.blank("en")
-
-        nlp.add_pipe("medspacy_quickumls", config={"threshold": 1.0, "result_type": "group","quickumls_fp":self.quickumls_fp})
-
-        concept_term = "dipalmitoyllecithin"
-
-        text = "Decreased {} content found in lung specimens".format(concept_term)
-
-        doc = nlp(text)
-
-        assert len(doc.ents) == 0
-
-        assert len(doc.spans[MEDSPACY_DEFAULT_SPAN_GROUP_NAME]) == 1
-
-        span = doc.spans[MEDSPACY_DEFAULT_SPAN_GROUP_NAME][0]
-
-        assert len(span._.umls_matches) > 0
+import unittest
+
+import spacy
+import warnings
+from sys import platform
+import pytest
+from pathlib import Path
+from quickumls import spacy_component
+
+class TestQuickUMLSSpangroup(unittest.TestCase):
+
+    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
+    @classmethod
+    def setUpClass(cls):
+        """Create sample db on the fly, to avoid os dependent path issue.
+        """
+        from .init_db import init
+        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)  
+
+    def test_simple_pipeline(self):
+        # let's make sure that this pipe has been initialized
+        # At least for MacOS and Linux which are currently supported...
+
+        # allow default QuickUMLS (very small sample data) to be loaded
+        nlp = spacy.blank("en")
+
+        nlp.add_pipe("medspacy_quickumls",config={"quickumls_fp":self.quickumls_fp})
+
+        assert nlp
+
+        quickumls = nlp.get_pipe("medspacy_quickumls")
+
+        print(quickumls.quickumls.info)
+
+        assert quickumls
+        # this is a member of the QuickUMLS algorithm inside the component
+        assert quickumls.quickumls
+        # Check that the simstring database exists
+        assert quickumls.quickumls.ss_db
+
+
+
+
+
+    def test_ensure_match_objects(self):
+        """
+        Test that an extraction has UmlsMatch objects for it
+        """
+
+        # let's make sure that this pipe has been initialized
+        # At least for MacOS and Linux which are currently supported...
+
+
+        # allow default QuickUMLS (very small sample data) to be loaded
+        nlp = spacy.blank("en")
+
+        nlp.add_pipe("medspacy_quickumls", config={"threshold": 1.0, "quickumls_fp":self.quickumls_fp})
+
+        pathexist=Path(self.quickumls_fp).exists()
+        print(self.quickumls_fp, pathexist)
+
+        concept_term = "dipalmitoyllecithin"
+
+        text = "Decreased {} content found in lung specimens".format(concept_term)
+
+        doc = nlp(text)
+        assert len(doc.ents) == 1
+
+        ent = doc.ents[0]
+
+        assert len(ent._.umls_matches) > 0
+
+        # make sure that we have a reasonable looking CUI
+        match_object = list(ent._.umls_matches)[0]
+
+        assert match_object.cui.startswith("C")
+
+
```

### Comparing `medspacy_quickumls-3.1a0/tests/skiptest_spangroup2.py` & `medspacy_quickumls-3.2/tests/skiptest_spangroup2.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import unittest
-from quickumls import spacy_component
-import spacy
-from quickumls.constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
-from pathlib import Path
-"""
-This test won't pass when tested with others in pytest tests. Skip it for now.
-"""
-class TestSpanGoup2(unittest.TestCase):
-
-    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
-    @classmethod
-    def setUpClass(cls):
-        """Create sample db on the fly, to avoid os dependent path issue.
-        """
-        from .init_db import init
-        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)      
-
-    def test_multiword_entity(self):
-        """
-        Test that an extraction can be made on a concept with multiple words
-        """
-
-        # let's make sure that this pipe has been initialized
-        # At least for MacOS and Linux which are currently supported...
-        # allow default QuickUMLS (very small sample data) to be loaded
-        nlp = spacy.blank("en")
-
-        nlp.add_pipe("medspacy_quickumls", config={"threshold": 0.7, "result_type": "group","quickumls_fp":self.quickumls_fp})
-
-        # the demo data contains this concept:
-        # dipalmitoyl phosphatidylcholine
-        text = """dipalmitoyl phosphatidylcholine"""
-
-        doc = nlp(text)
-
+import unittest
+from quickumls import spacy_component
+import spacy
+from quickumls.constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
+from pathlib import Path
+"""
+This test won't pass when tested with others in pytest tests. Skip it for now.
+"""
+class TestSpanGoup2(unittest.TestCase):
+
+    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
+    @classmethod
+    def setUpClass(cls):
+        """Create sample db on the fly, to avoid os dependent path issue.
+        """
+        from .init_db import init
+        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)      
+
+    def test_multiword_entity(self):
+        """
+        Test that an extraction can be made on a concept with multiple words
+        """
+
+        # let's make sure that this pipe has been initialized
+        # At least for MacOS and Linux which are currently supported...
+        # allow default QuickUMLS (very small sample data) to be loaded
+        nlp = spacy.blank("en")
+
+        nlp.add_pipe("medspacy_quickumls", config={"threshold": 0.7, "result_type": "group","quickumls_fp":self.quickumls_fp})
+
+        # the demo data contains this concept:
+        # dipalmitoyl phosphatidylcholine
+        text = """dipalmitoyl phosphatidylcholine"""
+
+        doc = nlp(text)
+
         assert len(doc.spans[MEDSPACY_DEFAULT_SPAN_GROUP_NAME]) == 1
```

### Comparing `medspacy_quickumls-3.1a0/tests/test_quickumls_component2.py` & `medspacy_quickumls-3.2/tests/test_quickumls_component2.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import unittest
-from quickumls import spacy_component
-import spacy
-from quickumls.constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
-from pathlib import Path
-"""
-This test won't pass when tested with others in pytest tests. Skip it for now.
-"""
-class TestSpanGoup2(unittest.TestCase):
-
-    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
-    @classmethod
-    def setUpClass(cls):
-        """Create sample db on the fly, to avoid os dependent path issue.
-        """
-        from .init_db import init
-        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)      
-
-    def test_multiword_entity(self):
-        """
-        Test that an extraction can be made on a concept with multiple words
-        """
-
-        # let's make sure that this pipe has been initialized
-        # At least for MacOS and Linux which are currently supported...
-        # allow default QuickUMLS (very small sample data) to be loaded
-        nlp = spacy.blank("en")
-
-        nlp.add_pipe("medspacy_quickumls", config={"threshold": 0.7, "result_type": "group","quickumls_fp":self.quickumls_fp})
-
-        # the demo data contains this concept:
-        # dipalmitoyl phosphatidylcholine
-        text = """dipalmitoyl phosphatidylcholine"""
-
-        doc = nlp(text)
-
+import unittest
+from quickumls import spacy_component
+import spacy
+from quickumls.constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
+from pathlib import Path
+"""
+This test won't pass when tested with others in pytest tests. Skip it for now.
+"""
+class TestSpanGoup2(unittest.TestCase):
+
+    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
+    @classmethod
+    def setUpClass(cls):
+        """Create sample db on the fly, to avoid os dependent path issue.
+        """
+        from .init_db import init
+        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)      
+
+    def test_multiword_entity(self):
+        """
+        Test that an extraction can be made on a concept with multiple words
+        """
+
+        # let's make sure that this pipe has been initialized
+        # At least for MacOS and Linux which are currently supported...
+        # allow default QuickUMLS (very small sample data) to be loaded
+        nlp = spacy.blank("en")
+
+        nlp.add_pipe("medspacy_quickumls", config={"threshold": 0.7, "result_type": "group","quickumls_fp":self.quickumls_fp})
+
+        # the demo data contains this concept:
+        # dipalmitoyl phosphatidylcholine
+        text = """dipalmitoyl phosphatidylcholine"""
+
+        doc = nlp(text)
+
         assert len(doc.spans[MEDSPACY_DEFAULT_SPAN_GROUP_NAME]) == 1
```

### Comparing `medspacy_quickumls-3.1a0/tests/test_quickumls_spangroup.py` & `medspacy_quickumls-3.2/tests/test_quickumls_spangroup.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import unittest
-
-import spacy
-import warnings
-from sys import platform
-import pytest
-
-from quickumls import spacy_component
-from quickumls.constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
-from pathlib import Path
-class TestQuickUMLSSpangroup(unittest.TestCase):
-
-
-    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
-    @classmethod
-    def setUpClass(cls):
-        """Create sample db on the fly, to avoid os dependent path issue.
-        """
-        from .init_db import init
-        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)  
-
-
-
-    def test_custom_span_group_name(self):
-        """
-        Test that extractions can be made for custom span group names
-        """
-
-        # let's make sure that this pipe has been initialized
-        # At least for MacOS and Linux which are currently supported...
-
-
-        # allow default QuickUMLS (very small sample data) to be loaded
-        nlp = spacy.blank("en")
-
-        custom_span_group_name = "my_own_span_group"
-
-        nlp.add_pipe("medspacy_quickumls", config={"threshold": 0.7,
-                                                   "result_type": "group",
-                                                   "span_group_name": custom_span_group_name,
-                                                   "quickumls_fp":self.quickumls_fp})
-
-        text = "Decreased dipalmitoyllecithin also branching glycosyltransferase and dipalmitoyl phosphatidylcholine"
-
-        doc = nlp(text)
-
-        assert len(doc.ents) == 0
-
-        assert MEDSPACY_DEFAULT_SPAN_GROUP_NAME not in doc.spans or len(doc.spans[MEDSPACY_DEFAULT_SPAN_GROUP_NAME]) == 0
-
-        assert len(doc.spans[custom_span_group_name]) >= 1
+import unittest
+
+import spacy
+import warnings
+from sys import platform
+import pytest
+
+from quickumls import spacy_component
+from quickumls.constants import MEDSPACY_DEFAULT_SPAN_GROUP_NAME
+from pathlib import Path
+class TestQuickUMLSSpangroup(unittest.TestCase):
+
+
+    quickumls_fp=str(Path('output', 'QuickUMLS_SAMPLE_lowercase_UNQLITE'))
+    @classmethod
+    def setUpClass(cls):
+        """Create sample db on the fly, to avoid os dependent path issue.
+        """
+        from .init_db import init
+        quickumls_fp=init(quickumls_fp=cls.quickumls_fp)  
+
+
+
+    def test_custom_span_group_name(self):
+        """
+        Test that extractions can be made for custom span group names
+        """
+
+        # let's make sure that this pipe has been initialized
+        # At least for MacOS and Linux which are currently supported...
+
+
+        # allow default QuickUMLS (very small sample data) to be loaded
+        nlp = spacy.blank("en")
+
+        custom_span_group_name = "my_own_span_group"
+
+        nlp.add_pipe("medspacy_quickumls", config={"threshold": 0.7,
+                                                   "result_type": "group",
+                                                   "span_group_name": custom_span_group_name,
+                                                   "quickumls_fp":self.quickumls_fp})
+
+        text = "Decreased dipalmitoyllecithin also branching glycosyltransferase and dipalmitoyl phosphatidylcholine"
+
+        doc = nlp(text)
+
+        assert len(doc.ents) == 0
+
+        assert MEDSPACY_DEFAULT_SPAN_GROUP_NAME not in doc.spans or len(doc.spans[MEDSPACY_DEFAULT_SPAN_GROUP_NAME]) == 0
+
+        assert len(doc.spans[custom_span_group_name]) >= 1
```

