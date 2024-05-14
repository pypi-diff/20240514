# Comparing `tmp/anomalo-0.22.0.tar.gz` & `tmp/anomalo-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalo-0.22.0.tar", max compression
+gzip compressed data, was "dist/anomalo-0.9.1.tar", last modified: Wed Sep  7 16:54:04 2022, max compression
```

## Comparing `anomalo-0.22.0.tar` & `anomalo-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11344 2024-01-09 12:01:14.275198 anomalo-0.22.0/LICENSE
--rw-r--r--   0        0        0      104 2024-01-09 12:01:14.275198 anomalo-0.22.0/README.public.md
--rw-r--r--   0        0        0      172 2024-01-24 15:59:11.740188 anomalo-0.22.0/anomalo/__init__.py
--rw-r--r--   0        0        0       35 2024-01-09 12:01:14.275198 anomalo-0.22.0/anomalo/__main__.py
--rw-r--r--   0        0        0       23 2024-05-14 15:35:52.814859 anomalo-0.22.0/anomalo/__version__.py
--rwxr-xr-x   0        0        0      266 2024-01-24 15:59:11.740188 anomalo-0.22.0/anomalo/anomalo.py
--rw-r--r--   0        0        0        0 2024-01-09 12:01:14.275198 anomalo-0.22.0/anomalo/cli/__init__.py
--rw-r--r--   0        0        0     1537 2024-01-09 12:01:14.279198 anomalo-0.22.0/anomalo/cli/cli.py
--rw-r--r--   0        0        0        0 2024-01-09 12:01:14.279198 anomalo-0.22.0/anomalo/cli/save_load/__init__.py
--rw-r--r--   0        0        0     6105 2024-01-24 15:59:11.740188 anomalo-0.22.0/anomalo/cli/save_load/commands.py
--rw-r--r--   0        0        0     8322 2024-05-03 15:36:10.783731 anomalo-0.22.0/anomalo/cli/save_load/models.py
--rw-r--r--   0        0        0        0 2024-01-09 12:01:14.279198 anomalo-0.22.0/anomalo/cli/state/__init__.py
--rw-r--r--   0        0        0     6585 2024-05-03 15:36:10.783731 anomalo-0.22.0/anomalo/cli/state/api.py
--rw-r--r--   0        0        0     1343 2024-01-09 12:01:14.279198 anomalo-0.22.0/anomalo/cli/state/errors.py
--rw-r--r--   0        0        0     1438 2024-03-28 00:24:21.290171 anomalo-0.22.0/anomalo/cli/state/file.py
--rw-r--r--   0        0        0     4751 2024-03-28 00:24:21.290171 anomalo-0.22.0/anomalo/cli/state/machine.py
--rw-r--r--   0        0        0     3822 2024-03-28 00:24:21.290171 anomalo-0.22.0/anomalo/cli/state/models.py
--rw-r--r--   0        0        0    21864 2024-05-03 15:36:10.787731 anomalo-0.22.0/anomalo/client.py
--rw-r--r--   0        0        0     3726 2024-03-28 00:24:21.290171 anomalo-0.22.0/anomalo/encoder.py
--rw-r--r--   0        0        0     2005 2024-03-13 21:20:30.080917 anomalo-0.22.0/anomalo/result.py
--rw-r--r--   0        0        0      917 2024-05-14 15:35:52.814859 anomalo-0.22.0/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 anomalo-0.22.0/PKG-INFO
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/
+-rw-r--r--   0 johnjoo    (501) staff       (20)       33 2022-09-06 04:48:18.000000 anomalo-0.9.1/.gitignore
+-rw-r--r--   0 johnjoo    (501) staff       (20)    11344 2022-09-06 04:48:18.000000 anomalo-0.9.1/LICENSE.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)      308 2022-09-07 16:54:04.000000 anomalo-0.9.1/PKG-INFO
+-rw-r--r--   0 johnjoo    (501) staff       (20)      211 2022-09-06 04:48:18.000000 anomalo-0.9.1/README.txt
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo/
+-rw-r--r--   0 johnjoo    (501) staff       (20)       57 2022-09-06 04:48:18.000000 anomalo-0.9.1/anomalo/__init__.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)       22 2022-09-07 16:54:02.000000 anomalo-0.9.1/anomalo/_version.py
+-rwxr-xr-x   0 johnjoo    (501) staff       (20)     7444 2022-09-06 04:48:18.000000 anomalo-0.9.1/anomalo/anomalo.py
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/
+-rw-r--r--   0 johnjoo    (501) staff       (20)      308 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/PKG-INFO
+-rw-r--r--   0 johnjoo    (501) staff       (20)      348 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)        1 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       41 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/entry_points.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       14 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/requires.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)        8 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/top_level.txt
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/examples/
+-rw-r--r--   0 johnjoo    (501) staff       (20)     3701 2022-09-06 04:48:18.000000 anomalo-0.9.1/examples/bulk_rerun.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)     1284 2022-09-06 04:48:18.000000 anomalo-0.9.1/examples/sample.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)       29 2022-08-01 21:30:00.000000 anomalo-0.9.1/requirements.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       38 2022-09-07 16:54:04.000000 anomalo-0.9.1/setup.cfg
+-rw-r--r--   0 johnjoo    (501) staff       (20)      899 2022-09-07 16:46:35.000000 anomalo-0.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `anomalo-0.22.0/LICENSE` & `anomalo-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

