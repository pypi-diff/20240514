# Comparing `tmp/real-estate-realtor.com-imp-local-0.0.5.tar.gz` & `tmp/real_estate_realtor_com_imp_local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real-estate-realtor.com-imp-local-0.0.5.tar", last modified: Wed Aug 16 07:33:10 2023, max compression
+gzip compressed data, was "real_estate_realtor_com_imp_local-0.0.6.tar", last modified: Tue May 14 17:43:21 2024, max compression
```

## Comparing `real-estate-realtor.com-imp-local-0.0.5.tar` & `real_estate_realtor_com_imp_local-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 07:33:10.600906 real-estate-realtor.com-imp-local-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-16 07:33:10.600906 real-estate-realtor.com-imp-local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-16 07:32:58.000000 real-estate-realtor.com-imp-local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 07:33:10.600906 real-estate-realtor.com-imp-local-0.0.5/real_estate_realtor.com_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-16 07:33:10.000000 real-estate-realtor.com-imp-local-0.0.5/real_estate_realtor.com_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-16 07:33:10.000000 real-estate-realtor.com-imp-local-0.0.5/real_estate_realtor.com_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-16 07:33:10.000000 real-estate-realtor.com-imp-local-0.0.5/real_estate_realtor.com_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-16 07:33:10.000000 real-estate-realtor.com-imp-local-0.0.5/real_estate_realtor.com_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-16 07:33:10.600906 real-estate-realtor.com-imp-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-16 07:32:58.000000 real-estate-realtor.com-imp-local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:21.233923 real_estate_realtor_com_imp_local-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-14 17:43:21.233923 real_estate_realtor_com_imp_local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 17:42:40.000000 real_estate_realtor_com_imp_local-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 17:42:40.000000 real_estate_realtor_com_imp_local-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:21.233923 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:21.233923 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:42:40.000000 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14241 2024-05-14 17:42:40.000000 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local/src/realtor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:21.233923 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-14 17:43:21.000000 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 17:43:21.000000 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:43:21.000000 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 17:43:21.000000 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 17:43:21.000000 real_estate_realtor_com_imp_local-0.0.6/real_estate_realtor_com_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:43:21.233923 real_estate_realtor_com_imp_local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-14 17:42:40.000000 real_estate_realtor_com_imp_local-0.0.6/setup.py
```

