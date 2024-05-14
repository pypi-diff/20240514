# Comparing `tmp/updateheaders-0.0.0.tar.gz` & `tmp/updateheaders-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "updateheaders-0.0.0.tar", last modified: Thu May  2 08:31:44 2024, max compression
+gzip compressed data, was "updateheaders-1.1.tar", last modified: Tue May 14 16:55:02 2024, max compression
```

## Comparing `updateheaders-0.0.0.tar` & `updateheaders-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-02 08:31:44.265328 updateheaders-0.0.0/
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)       80 2024-05-02 08:31:44.265328 updateheaders-0.0.0/PKG-INFO
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-02 08:31:44.265328 updateheaders-0.0.0/Updateheaders/
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      250 2024-05-02 08:29:40.000000 updateheaders-0.0.0/Updateheaders/Client.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-02 08:31:44.265328 updateheaders-0.0.0/Updateheaders.egg-info/
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)       80 2024-05-02 08:31:44.000000 updateheaders-0.0.0/Updateheaders.egg-info/PKG-INFO
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      180 2024-05-02 08:31:44.000000 updateheaders-0.0.0/Updateheaders.egg-info/SOURCES.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-02 08:31:44.000000 updateheaders-0.0.0/Updateheaders.egg-info/dependency_links.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       14 2024-05-02 08:31:44.000000 updateheaders-0.0.0/Updateheaders.egg-info/top_level.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-02 08:31:44.265328 updateheaders-0.0.0/setup.cfg
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      100 2024-05-02 08:31:11.000000 updateheaders-0.0.0/setup.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-14 16:55:02.054954 updateheaders-1.1/
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)       78 2024-05-14 16:55:02.054954 updateheaders-1.1/PKG-INFO
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-14 16:55:02.044954 updateheaders-1.1/Updateheaders/
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      250 2024-05-14 16:47:27.000000 updateheaders-1.1/Updateheaders/Client.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-14 16:55:02.054954 updateheaders-1.1/Updateheaders.egg-info/
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)       78 2024-05-14 16:55:02.000000 updateheaders-1.1/Updateheaders.egg-info/PKG-INFO
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      180 2024-05-14 16:55:02.000000 updateheaders-1.1/Updateheaders.egg-info/SOURCES.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-14 16:55:02.000000 updateheaders-1.1/Updateheaders.egg-info/dependency_links.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       14 2024-05-14 16:55:02.000000 updateheaders-1.1/Updateheaders.egg-info/top_level.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-14 16:55:02.054954 updateheaders-1.1/setup.cfg
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      117 2024-05-14 16:54:46.000000 updateheaders-1.1/setup.py
```

