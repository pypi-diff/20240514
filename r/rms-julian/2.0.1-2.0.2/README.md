# Comparing `tmp/rms-julian-2.0.1.tar.gz` & `tmp/rms_julian-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-julian-2.0.1.tar", last modified: Wed Jan 24 23:34:48 2024, max compression
+gzip compressed data, was "rms_julian-2.0.2.tar", last modified: Tue May 14 19:21:01 2024, max compression
```

## Comparing `rms-julian-2.0.1.tar` & `rms_julian-2.0.2.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.889913 rms-julian-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:29:34.000000 rms-julian-2.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-24 23:29:34.000000 rms-julian-2.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.877913 rms-julian-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.881913 rms-julian-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:29:34.000000 rms-julian-2.0.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:29:34.000000 rms-julian-2.0.1/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-01-24 23:29:34.000000 rms-julian-2.0.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:29:34.000000 rms-julian-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:29:34.000000 rms-julian-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-01-24 23:34:48.889913 rms-julian-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-01-24 23:29:34.000000 rms-julian-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.881913 rms-julian-2.0.1/documents/
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-01-24 23:29:34.000000 rms-julian-2.0.1/documents/ISO 8601-1988 Date-Time Representations.html
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-24 23:29:34.000000 rms-julian-2.0.1/documents/TAI-UTC_tab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-01-24 23:29:34.000000 rms-julian-2.0.1/documents/datapoly.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.885913 rms-julian-2.0.1/julian/
--rw-r--r--   0 runner    (1001) docker     (127)    28162 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/DEPRECATED.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/_TIMEZONES.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24193 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/_deltat.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:34:48.000000 rms-julian-2.0.1/julian/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.885913 rms-julian-2.0.1/julian/assets/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5255 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/assets/naif0012.tls
--rw-r--r--   0 runner    (1001) docker     (127)    14610 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/date_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/date_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/datetime_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/datetime_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    25198 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/iso_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22756 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/leap_seconds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/mjd_jd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/mjd_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/time_of_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/time_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/time_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-01-24 23:29:34.000000 rms-julian-2.0.1/julian/utc_tai_tdb_tt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-24 23:29:34.000000 rms-julian-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-24 23:29:34.000000 rms-julian-2.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.889913 rms-julian-2.0.1/rms_julian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-01-24 23:34:48.000000 rms-julian-2.0.1/rms_julian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-01-24 23:34:48.000000 rms-julian-2.0.1/rms_julian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:34:48.000000 rms-julian-2.0.1/rms_julian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-24 23:34:48.000000 rms-julian-2.0.1/rms_julian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-24 23:34:48.000000 rms-julian-2.0.1/rms_julian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-24 23:34:48.889913 rms-julian-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.885913 rms-julian-2.0.1/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)   313729 2024-01-24 23:29:34.000000 rms-julian-2.0.1/test_files/cpck15Dec2017.tpc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:34:48.889913 rms-julian-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_date_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    40744 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_date_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    20359 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_datetime_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_datetime_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    27270 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_deltat.py
--rw-r--r--   0 runner    (1001) docker     (127)    38576 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    28726 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_iso_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_leap_seconds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_mjd_jd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_mjd_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_time_of_day.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_time_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    41984 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_time_pyparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    21339 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_utc_tai_tdb_tt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34696 2024-01-24 23:29:34.000000 rms-julian-2.0.1/tests/test_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.507832 rms_julian-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:15:52.000000 rms_julian-2.0.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 19:15:52.000000 rms_julian-2.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.495832 rms_julian-2.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.499832 rms_julian-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:15:52.000000 rms_julian-2.0.2/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:15:52.000000 rms_julian-2.0.2/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-14 19:15:52.000000 rms_julian-2.0.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:15:52.000000 rms_julian-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:15:52.000000 rms_julian-2.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-05-14 19:15:52.000000 rms_julian-2.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:15:52.000000 rms_julian-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-14 19:21:01.507832 rms_julian-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-14 19:15:52.000000 rms_julian-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.499832 rms_julian-2.0.2/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-14 19:15:52.000000 rms_julian-2.0.2/documents/ISO 8601-1988 Date-Time Representations.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-14 19:15:52.000000 rms_julian-2.0.2/documents/TAI-UTC_tab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-14 19:15:52.000000 rms_julian-2.0.2/documents/datapoly.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.503832 rms_julian-2.0.2/julian/
+-rw-r--r--   0 runner    (1001) docker     (127)    28162 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/DEPRECATED.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/_TIMEZONES.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24193 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/_deltat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:21:01.000000 rms_julian-2.0.2/julian/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.503832 rms_julian-2.0.2/julian/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5255 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/assets/naif0012.tls
+-rw-r--r--   0 runner    (1001) docker     (127)    14610 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/date_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18975 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/date_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/datetime_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/datetime_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25198 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/iso_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22756 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/leap_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/mjd_jd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/mjd_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/time_of_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/time_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/time_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-05-14 19:15:52.000000 rms_julian-2.0.2/julian/utc_tai_tdb_tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-14 19:15:52.000000 rms_julian-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 19:15:52.000000 rms_julian-2.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.507832 rms_julian-2.0.2/rms_julian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-14 19:21:01.000000 rms_julian-2.0.2/rms_julian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-14 19:21:01.000000 rms_julian-2.0.2/rms_julian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:21:01.000000 rms_julian-2.0.2/rms_julian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 19:21:01.000000 rms_julian-2.0.2/rms_julian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 19:21:01.000000 rms_julian-2.0.2/rms_julian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 19:21:01.507832 rms_julian-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.503832 rms_julian-2.0.2/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   313729 2024-05-14 19:15:52.000000 rms_julian-2.0.2/test_files/cpck15Dec2017.tpc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:21:01.507832 rms_julian-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18913 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_date_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40744 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_date_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20359 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_datetime_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_datetime_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27270 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_deltat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38576 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28726 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_iso_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_leap_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_mjd_jd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_mjd_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_time_of_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_time_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41984 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_time_pyparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21339 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_utc_tai_tdb_tt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34696 2024-05-14 19:15:52.000000 rms_julian-2.0.2/tests/test_v1.py
```

### Comparing `rms-julian-2.0.1/.github/workflows/publish_to_pypi.yml` & `rms_julian-2.0.2/.github/workflows/publish_to_pypi.yml`

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

### Comparing `rms-julian-2.0.1/.github/workflows/publish_to_test_pypi.yml` & `rms_julian-2.0.2/.github/workflows/publish_to_test_pypi.yml`

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

### Comparing `rms-julian-2.0.1/.github/workflows/run-tests.yml` & `rms_julian-2.0.2/.github/workflows/run-tests.yml`

 * *Files 11% similar despite different names*

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
@@ -22,26 +22,29 @@
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
-        env:
-          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
+          token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-julian-2.0.1/.gitignore` & `rms_julian-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/LICENSE` & `rms_julian-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/PKG-INFO` & `rms_julian-2.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,29 @@
-Metadata-Version: 2.1
-Name: rms-julian
-Version: 2.0.1
-Summary: Routines for converting to and from Julian dates
-Maintainer-email: "Robert S. French" <rfrench@seti.org>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/SETI/rms-julian
-Project-URL: Repository, https://github.com/SETI/rms-julian
-Project-URL: Source, https://github.com/SETI/rms-julian
-Project-URL: Issues, https://github.com/SETI/rms-julian/issues
-Keywords: julian
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pyparsing
-Requires-Dist: rms-textkernel
-
-| PyPI Release | Test Status | Code Coverage |
-| ------------ | ----------- | ------------- |
-| [![PyPI version](https://badge.fury.io/py/rms-julian.svg)](https://badge.fury.io/py/rms-julian) | [![Build status](https://img.shields.io/github/actions/workflow/status/SETI/rms-julian/run-tests.yml?branch=main)](https://github.com/SETI/rms-julian/actions) | [![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-julian/main?logo=codecov)](https://codecov.io/gh/SETI/rms-julian) |
+[![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-julian)](https://github.com/SETI/rms-julian/releases)
+[![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-julian)](https://github.com/SETI/rms-julian/releases)
+[![Test Status](https://img.shields.io/github/actions/workflow/status/SETI/rms-julian/run-tests.yml?branch=main)](https://github.com/SETI/rms-julian/actions)
+[![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-julian/main?logo=codecov)](https://codecov.io/gh/SETI/rms-julian)
+<br />
+[![PyPI - Version](https://img.shields.io/pypi/v/rms-julian)](https://pypi.org/project/rms-julian)
+[![PyPI - Format](https://img.shields.io/pypi/format/rms-julian)](https://pypi.org/project/rms-julian)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/rms-julian)](https://pypi.org/project/rms-julian)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rms-julian)](https://pypi.org/project/rms-julian)
+<br />
+[![GitHub commits since latest release](https://img.shields.io/github/commits-since/SETI/rms-julian/latest)](https://github.com/SETI/rms-julian/commits/main/)
+[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/SETI/rms-julian)](https://github.com/SETI/rms-julian/commits/main/)
+[![GitHub last commit](https://img.shields.io/github/last-commit/SETI/rms-julian)](https://github.com/SETI/rms-julian/commits/main/)
+<br />
+[![Number of GitHub open issues](https://img.shields.io/github/issues-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/issues)
+[![Number of GitHub closed issues](https://img.shields.io/github/issues-closed-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/issues)
+[![Number of GitHub open pull requests](https://img.shields.io/github/issues-pr-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/pulls)
+[![Number of GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/pulls)
+<br />
+![GitHub License](https://img.shields.io/github/license/SETI/rms-julian)
+[![Number of GitHub stars](https://img.shields.io/github/stars/SETI/rms-julian)](https://github.com/SETI/rms-julian/stargazers)
+![GitHub forks](https://img.shields.io/github/forks/SETI/rms-julian)
 
 # rms-julian
 
 Supported versions: Python >= 3.7
 
 # PDS Ring-Moon Systems Node, SETI Institute
 # Julian Library, version 2.0
```

### Comparing `rms-julian-2.0.1/README.md` & `rms_julian-2.0.2/julian/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-| PyPI Release | Test Status | Code Coverage |
-| ------------ | ----------- | ------------- |
-| [![PyPI version](https://badge.fury.io/py/rms-julian.svg)](https://badge.fury.io/py/rms-julian) | [![Build status](https://img.shields.io/github/actions/workflow/status/SETI/rms-julian/run-tests.yml?branch=main)](https://github.com/SETI/rms-julian/actions) | [![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-julian/main?logo=codecov)](https://codecov.io/gh/SETI/rms-julian) |
-
-# rms-julian
-
-Supported versions: Python >= 3.7
-
-# PDS Ring-Moon Systems Node, SETI Institute
-# Julian Library, version 2.0
+##########################################################################################
+# julian/__init__.py
+##########################################################################################
+"""PDS Ring-Moon Systems Node, SETI Institute
+Julian Library, version 2.0
 
 This is a large set of routines for handing date and time conversions. Compared to other
 date/time libraries in Python, including CSPYCE, it has these features:
 
 - It handles the time systems Coordinated Universal Time (UTC), International Atomic Time
   (TAI), Barycentric Dynamical Time (TDB), and Terrestrial Time (TT, previously called
   Terrestrial Dynamical Time or TDT), properly accounting for leap seconds.
@@ -25,194 +20,170 @@
 
 - It provides options for how to interpret times before 1972, when the current version of
   the UTC time system was first implemented. Since 1972, leap seconds have been used to
   keep TAI in sync with UTC, ensuring that the UTC time never differs from UT1, the time
   system defined by the Earth's rotation, by more than ~ 1 second. Between 1958 and 1972,
   the UTC second was redefined as a "rubber second", which would stretch or shrink as
   necessary to ensure that every mean solar day contained exactly 86,400 UT seconds; see
-  [https://hpiers.obspm.fr/eop-pc/index.php?index=TAI-UTC_tab](https://hpiers.obspm.fr/eop-pc/index.php?index=TAI-UTC_tab).
-
+        https://hpiers.obspm.fr/eop-pc/index.php?index=TAI-UTC_tab
   Before 1958, we use UT1 in place of UTC, employing a model for the long-term variations
   in Earth's rotation as documented for the "Five Millennium Canon of Solar Eclipses:
   -1999 to +3000; see
-  [https://eclipse.gsfc.nasa.gov/SEpubs/5MCSE.html](https://eclipse.gsfc.nasa.gov/SEpubs/5MCSE.html).
-
+        https://eclipse.gsfc.nasa.gov/SEpubs/5MCSE.html
   The numerical details are here:
-  [https://eclipse.gsfc.nasa.gov/SEcat5/deltatpoly.html](https://eclipse.gsfc.nasa.gov/SEcat5/deltatpoly.html).
-
+        https://eclipse.gsfc.nasa.gov/SEcat5/deltatpoly.html
   This model can also be applied to future dates.
 
 - It supports both the modern (Gregorian) calendar and the older Julian calendar. The
   transition date can be defined by the user, or else the Julian calendar can be
   suppressed entirely.
 
 - A general parser is able to interpret almost arbitrary date-time strings correctly. This
   parser can also be used to "scrape" occurrences of dates and times from arbitrary text.
 
 
-### CALENDAR OPERATIONS
+CALENDAR OPERATIONS
 
 Every date is represented by an integer "day" value, where day = 0 on January 1, 2000.
 Various functions are provided to convert between day values and year, month, day, or day
 of year:
-
-        day_from_ymd()
-        day_from_yd()
-        ymd_from_day()
-        yd_from_day()
+    day_from_ymd(), day_from_yd(), ymd_from_day(), yd_from_day().
 
 Years prior to 1 CE are specified using the "astronomical year", which includes a year
 zero. As a result, 1 BCE is specified as year 0, 2 BCE as year -1, 4713 BCE as year -4712,
 etc. Note that there is some historical uncertainty about which years were recognized as
 leap years in Rome between the adoption of the Julian calendar in 46 BCE and about 8 CE.
 For simplicity, we follow the convention that the Julian calendar extended backward
 indefinitely, so all all years divisible by four, including 4 CE, 0 (1 BCE), -4 (5 BCE),
 -8 (9 BCE), etc., were leap years.
 
 Months are referred to by integers 1-12, 1 for January and 12 for December.
 
 Day numbers within months are 1-31; day numbers within years are 1-366.
 
 Functions are provided to determine the number of days in a specified month or year:
+    days_in_year(), days_in_ym().
 
-        days_in_year()
-        days_in_ym()
-
-Use the function `set_gregorian_start()` to specify the (Gregorian) year, month, and day for
+Use the function set_gregorian_start() to specify the (Gregorian) year, month, and day for
 the transition from the earlier Julian calendar to the modern Gregorian calendar. The
 default start date of the Gregorian calendar is October 15, 1582, when this calendar was
 first adopted in much of Europe. However, the user is free to modify this date; for
 example, Britain adopted the Gregorian calendar on September 14, 1752.
 
 Note that most calendar functions support an input parameter "proleptic", taking a value
-of `True` or `False`. If True, all calendar dates are proleptic (extrapolated backward
+of True or False. If True, all calendar dates are proleptic (extrapolated backward
 assuming the modern calendar), regardless of which calendar was in effect at the time.
 
 
-### TIME SYSTEMS
+TIME SYSTEMS
 
 All times are represented by numbers representing seconds past a specified epoch on
 January 1, 2000. Internally, TAI times serve as the intermediary between the different
 time systems (TAI, UTC, TDB, and TT). Conversions are straightforward, using:
-
-        tai_from_utc()
-        utc_from_tai()
-        tai_from_tdb()
-        tdb_from_tai()
-        tai_from_tt()
-        tt_from_tai()
-
-Alternatively, the more general function `time_from_time()` lets you specify the initial and
+    tai_from_utc(), utc_from_tai(), tai_from_tdb(), tdb_from_tai(), tai_from_tt(),
+    tt_from_tai().
+Alternatively, the more general function time_from_time() lets you specify the initial and
 final time systems of the conversion.
 
 You can also specify a time using an integer day plus the number of elapsed seconds on
 that day, and then convert between these values and any time system:
-
-        day_sec_from_utc()
-        day_sec_from_tai()
-        tai_from_day()
-        tai_from_day_sec()
-        utc_from_day()
-        utc_from_day_sec()
-
-Alternatively, the more general functions `day_sec_from_time()` and `time_from_day_sec()`
+    day_sec_from_utc(), day_sec_from_tai(), tai_from_day(), tai_from_day_sec(),
+    utc_from_day(), utc_from_day_sec().
+Alternatively, the more general functions day_sec_from_time() and time_from_day_sec()
 let you specify the initial and final time systems.
 
 
-### JULIAN DATES
+JULIAN DATES
 
 Similarly, Julian dates and Modified Julian Dates can be converted to times using any time
 system:
-
-        jd_from_time()
-        time_from_jd()
-        mjd_from_time()
-        time_from_mjd()
-        jd_from_day_sec()
-        day_sec_from_jd()
-        mjd_from_day_sec()
-        day_sec_from_mjd()
+    jd_from_time(), time_from_jd(), mjd_from_time(), time_from_mjd(),
+    jd_from_day_sec(), day_sec_from_jd(), mjd_from_day_sec(), day_sec_from_mjd().
 
 You can also convert directly between integer MJD and integer day numbers using:
-
-        mjd_from_day()
-        day_from_mjd()
+    mjd_from_day(), day_from_mjd().
 
 
-### LEAP SECOND HANDLING
+LEAP SECOND HANDLING
 
 In 1972, the UTC time system began using leap seconds to keep TAI times in sync with mean
 solar time to a precision of ~ 1 second. We provide several methods to allow the user to
 keep the leap second list up to date.
 
-If the environment variable `SPICE_LSK_FILEPATH` is defined, then this SPICE leapseconds
+If the environment variable SPICE_LSK_FILEPATH is defined, then this SPICE leapseconds
 kernel is read at startup. Otherwise, leap seconds through 2020 are always included, as
-defined in SPICE kernel file "`naif0012.tls`". You can also call the function `load_lsk()`
+defined in SPICE kernel file naif0012.tls. You can also call the function load_lsk()
 directly.
 
-Alternatively, use `insert_leap_second()` to augment the list with additional leap seconds
+Alternatively, use insert_leap_second() to augment the list with additional leap seconds
 (positive or negative).
 
-Use `seconds_on_day()` to determine the length in seconds of a given day; use
-`leapsecs_on_day()` or `leapsecs_from_ymd()` to determine the cumulative number of leap
+Use seconds_on_day() to determine the length in seconds of a given day; use
+leapsecs_on_day() or leapsecs_from_ymd() to determine the cumulative number of leap
 seconds on a given date.
 
-Use `set_ut_model()` to define how to handle times before 1972 and into the future, outside
+Use set_ut_model() to define how to handle times before 1972 and into the future, outside
 the duration of the current UTC leap second system.
 
 
-### FORMATTING
+FORMATTING
 
 Several functions are provided to express dates or times as formatted character strings:
-
-        format_day()
-        format_day_sec()
-        format_sec()
-        format_tai()
-        iso_from_tai()
-
+    format_day(), format_day_sec(), format_sec(), format_tai(), iso_from_tai().
 Most variations of the ISO 8601:1988 format are supported.
 
 Note that these functions can produce strings, bytestrings, or arbitrary arrays thereof.
 The functions operate on the entire array all at once, and can therefore be much faster
 than making individual calls over and over. For example, note that one could provide a
 NumPy memmap as input to these functions and it would write content directly into a large
 ASCII table, avoiding any conversion to/from Unicode.
 
 
-### PARSING
+PARSING
 
 We provide functions for the very fast parsing of identically-formatted strings or
 bytestrings that represent dates, times or both:
-
-        day_from_iso()
-        day_sec_from_iso()
-        sec_from_iso()
-        tai_from_iso()
-        tdb_from_iso()
-        time_from_iso()
-
+    day_from_iso(), day_sec_from_iso(), sec_from_iso(), tai_from_iso(), tdb_from_iso(),
+    time_from_iso().
 These functions recognize most variations of the ISO 8601:1988 format, and are ideal for
 interpreting date and time columns from large ASCII tables.
 
 More general parsers are provided for interpreting individual dates and times in almost
 arbitrary formats:
-
-        day_from_string()
-        day_sec_from_string()
-        sec_from_string()
-
+    day_from_string(), day_sec_from_string(), sec_from_string().
 These same parsers can also be invoked to "scrape" dates and times from almost arbitrary
 text:
-
-        days_in_strings()
-        day_sec_in_strings()
-        secs_in_strings()
-
+    days_in_strings(), day_sec_in_strings(), secs_in_strings().
 Time zones are recognized, including most standard abbreviations.
 
 For users familiar with the pyparsing module, we provide functions that generate parsers
 for a wide variety of special requirements. See:
+    date_pyparser(), datetime_pyparser(), mjd_pyparser(), time_pyparser().
+"""
+
+from julian.calendar          import *
+from julian.date_parsers      import *
+from julian.datetime_parsers  import *
+from julian.formatters        import *
+from julian.formatters        import *
+from julian.iso_parsers       import *
+from julian.leap_seconds      import *
+from julian.mjd_jd            import *
+from julian.time_of_day       import *
+from julian.time_parsers      import *
+from julian.utc_tai_tdb_tt    import *
+
+from julian.date_pyparser     import date_pyparser
+from julian.datetime_pyparser import datetime_pyparser
+from julian.mjd_pyparser      import mjd_pyparser
+from julian.time_pyparser     import time_pyparser
+
+from julian.DEPRECATED        import *
+from julian._warnings         import *
+from julian._exceptions       import *
+
+try:
+    from ._version import __version__
+except ImportError as err:
+    __version__ = 'Version unspecified'
 
-        date_pyparser()
-        datetime_pyparser()
-        time_pyparser()
+##########################################################################################
```

### Comparing `rms-julian-2.0.1/documents/ISO 8601-1988 Date-Time Representations.html` & `rms_julian-2.0.2/documents/ISO 8601-1988 Date-Time Representations.html`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/documents/TAI-UTC_tab.txt` & `rms_julian-2.0.2/documents/TAI-UTC_tab.txt`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/documents/datapoly.html` & `rms_julian-2.0.2/documents/datapoly.html`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/DEPRECATED.py` & `rms_julian-2.0.2/julian/DEPRECATED.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/_TIMEZONES.py` & `rms_julian-2.0.2/julian/_TIMEZONES.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/_deltat.py` & `rms_julian-2.0.2/julian/_deltat.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/_exceptions.py` & `rms_julian-2.0.2/julian/_exceptions.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/_utils.py` & `rms_julian-2.0.2/julian/_utils.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/_warnings.py` & `rms_julian-2.0.2/julian/_warnings.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/assets/naif0012.tls` & `rms_julian-2.0.2/julian/assets/naif0012.tls`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/calendar.py` & `rms_julian-2.0.2/julian/calendar.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/date_parsers.py` & `rms_julian-2.0.2/julian/date_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/date_pyparser.py` & `rms_julian-2.0.2/julian/date_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/datetime_parsers.py` & `rms_julian-2.0.2/julian/datetime_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/datetime_pyparser.py` & `rms_julian-2.0.2/julian/datetime_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/formatters.py` & `rms_julian-2.0.2/julian/formatters.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/iso_parsers.py` & `rms_julian-2.0.2/julian/iso_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/leap_seconds.py` & `rms_julian-2.0.2/julian/leap_seconds.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/mjd_jd.py` & `rms_julian-2.0.2/julian/mjd_jd.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/mjd_pyparser.py` & `rms_julian-2.0.2/julian/mjd_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/time_of_day.py` & `rms_julian-2.0.2/julian/time_of_day.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/time_parsers.py` & `rms_julian-2.0.2/julian/time_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/time_pyparser.py` & `rms_julian-2.0.2/julian/time_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/julian/utc_tai_tdb_tt.py` & `rms_julian-2.0.2/julian/utc_tai_tdb_tt.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/pyproject.toml` & `rms_julian-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/rms_julian.egg-info/PKG-INFO` & `rms_julian-2.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-julian
-Version: 2.0.1
+Version: 2.0.2
 Summary: Routines for converting to and from Julian dates
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-julian
 Project-URL: Repository, https://github.com/SETI/rms-julian
 Project-URL: Source, https://github.com/SETI/rms-julian
 Project-URL: Issues, https://github.com/SETI/rms-julian/issues
@@ -27,17 +27,36 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pyparsing
 Requires-Dist: rms-textkernel
 
-| PyPI Release | Test Status | Code Coverage |
-| ------------ | ----------- | ------------- |
-| [![PyPI version](https://badge.fury.io/py/rms-julian.svg)](https://badge.fury.io/py/rms-julian) | [![Build status](https://img.shields.io/github/actions/workflow/status/SETI/rms-julian/run-tests.yml?branch=main)](https://github.com/SETI/rms-julian/actions) | [![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-julian/main?logo=codecov)](https://codecov.io/gh/SETI/rms-julian) |
+[![GitHub release; latest by date](https://img.shields.io/github/v/release/SETI/rms-julian)](https://github.com/SETI/rms-julian/releases)
+[![GitHub Release Date](https://img.shields.io/github/release-date/SETI/rms-julian)](https://github.com/SETI/rms-julian/releases)
+[![Test Status](https://img.shields.io/github/actions/workflow/status/SETI/rms-julian/run-tests.yml?branch=main)](https://github.com/SETI/rms-julian/actions)
+[![Code coverage](https://img.shields.io/codecov/c/github/SETI/rms-julian/main?logo=codecov)](https://codecov.io/gh/SETI/rms-julian)
+<br />
+[![PyPI - Version](https://img.shields.io/pypi/v/rms-julian)](https://pypi.org/project/rms-julian)
+[![PyPI - Format](https://img.shields.io/pypi/format/rms-julian)](https://pypi.org/project/rms-julian)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/rms-julian)](https://pypi.org/project/rms-julian)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rms-julian)](https://pypi.org/project/rms-julian)
+<br />
+[![GitHub commits since latest release](https://img.shields.io/github/commits-since/SETI/rms-julian/latest)](https://github.com/SETI/rms-julian/commits/main/)
+[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/SETI/rms-julian)](https://github.com/SETI/rms-julian/commits/main/)
+[![GitHub last commit](https://img.shields.io/github/last-commit/SETI/rms-julian)](https://github.com/SETI/rms-julian/commits/main/)
+<br />
+[![Number of GitHub open issues](https://img.shields.io/github/issues-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/issues)
+[![Number of GitHub closed issues](https://img.shields.io/github/issues-closed-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/issues)
+[![Number of GitHub open pull requests](https://img.shields.io/github/issues-pr-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/pulls)
+[![Number of GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed-raw/SETI/rms-julian)](https://github.com/SETI/rms-julian/pulls)
+<br />
+![GitHub License](https://img.shields.io/github/license/SETI/rms-julian)
+[![Number of GitHub stars](https://img.shields.io/github/stars/SETI/rms-julian)](https://github.com/SETI/rms-julian/stargazers)
+![GitHub forks](https://img.shields.io/github/forks/SETI/rms-julian)
 
 # rms-julian
 
 Supported versions: Python >= 3.7
 
 # PDS Ring-Moon Systems Node, SETI Institute
 # Julian Library, version 2.0
```

### Comparing `rms-julian-2.0.1/rms_julian.egg-info/SOURCES.txt` & `rms_julian-2.0.2/rms_julian.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

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

### Comparing `rms-julian-2.0.1/test_files/cpck15Dec2017.tpc` & `rms_julian-2.0.2/test_files/cpck15Dec2017.tpc`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/__init__.py` & `rms_julian-2.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_calendar.py` & `rms_julian-2.0.2/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_date_parsers.py` & `rms_julian-2.0.2/tests/test_date_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_date_pyparser.py` & `rms_julian-2.0.2/tests/test_date_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_datetime_parsers.py` & `rms_julian-2.0.2/tests/test_datetime_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_datetime_pyparser.py` & `rms_julian-2.0.2/tests/test_datetime_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_deltat.py` & `rms_julian-2.0.2/tests/test_deltat.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_formatters.py` & `rms_julian-2.0.2/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_iso_parsers.py` & `rms_julian-2.0.2/tests/test_iso_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_leap_seconds.py` & `rms_julian-2.0.2/tests/test_leap_seconds.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_mjd_jd.py` & `rms_julian-2.0.2/tests/test_mjd_jd.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_mjd_pyparser.py` & `rms_julian-2.0.2/tests/test_mjd_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_time_of_day.py` & `rms_julian-2.0.2/tests/test_time_of_day.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_time_parsers.py` & `rms_julian-2.0.2/tests/test_time_parsers.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_time_pyparser.py` & `rms_julian-2.0.2/tests/test_time_pyparser.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_utc_tai_tdb_tt.py` & `rms_julian-2.0.2/tests/test_utc_tai_tdb_tt.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_utils.py` & `rms_julian-2.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rms-julian-2.0.1/tests/test_v1.py` & `rms_julian-2.0.2/tests/test_v1.py`

 * *Files identical despite different names*

