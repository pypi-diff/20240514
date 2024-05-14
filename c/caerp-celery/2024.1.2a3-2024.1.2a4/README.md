# Comparing `tmp/caerp_celery-2024.1.2a3.tar.gz` & `tmp/caerp_celery-2024.1.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caerp_celery-2024.1.2a3.tar", last modified: Thu May  2 15:11:22 2024, max compression
+gzip compressed data, was "caerp_celery-2024.1.2a4.tar", last modified: Tue May 14 15:09:16 2024, max compression
```

## Comparing `caerp_celery-2024.1.2a3.tar` & `caerp_celery-2024.1.2a4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.434054 caerp_celery-2024.1.2a3/
--rw-r--r--   0 gas       (1000) gas       (1000)      334 2024-03-06 11:08:10.000000 caerp_celery-2024.1.2a3/CHANGELOG
--rw-r--r--   0 gas       (1000) gas       (1000)       11 2024-05-02 15:09:51.000000 caerp_celery-2024.1.2a3/CURRENT_VERSION
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 caerp_celery-2024.1.2a3/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      210 2024-03-06 10:24:06.000000 caerp_celery-2024.1.2a3/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-05-02 15:11:22.433054 caerp_celery-2024.1.2a3/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     2627 2024-03-05 16:04:43.000000 caerp_celery-2024.1.2a3/README.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       46 2024-03-08 17:12:36.000000 caerp_celery-2024.1.2a3/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       38 2024-05-02 15:11:22.434054 caerp_celery-2024.1.2a3/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1372 2024-03-06 11:04:59.000000 caerp_celery-2024.1.2a3/setup.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.418054 caerp_celery-2024.1.2a3/src/
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.423054 caerp_celery-2024.1.2a3/src/caerp_celery/
--rw-r--r--   0 gas       (1000) gas       (1000)     4579 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1789 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)      585 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/exception.py
--rw-r--r--   0 gas       (1000) gas       (1000)      576 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/hacks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      753 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/interfaces.py
--rw-r--r--   0 gas       (1000) gas       (1000)      885 2024-05-02 14:38:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5747 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7465 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/models.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.427054 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/
--rw-r--r--   0 gas       (1000) gas       (1000)     2163 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3533 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/cegid.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3133 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/ebp.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3376 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/isacompta.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3264 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/quadra.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3391 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage.py
--rw-r--r--   0 gas       (1000) gas       (1000)     5798 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage_generation_expert.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.428054 caerp_celery-2024.1.2a3/src/caerp_celery/schedulers/
--rw-r--r--   0 gas       (1000) gas       (1000)       29 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/schedulers/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)      428 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/schedulers/tasks.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.433054 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/
--rw-r--r--   0 gas       (1000) gas       (1000)    10899 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/__init__.py
--rw-r--r--   0 gas       (1000) gas       (1000)    39090 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_measure_compute.py
--rw-r--r--   0 gas       (1000) gas       (1000)    14135 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_parser.py
--rw-r--r--   0 gas       (1000) gas       (1000)    29193 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/csv_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)    21494 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2015 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/json_import.py
--rw-r--r--   0 gas       (1000) gas       (1000)      392 2024-04-25 07:56:31.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/locks.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4428 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/mail.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1423 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/notification.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3397 2024-03-15 11:24:28.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/tasks.py
--rw-r--r--   0 gas       (1000) gas       (1000)      509 2024-03-15 11:23:43.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/user_connections.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6912 2024-04-25 09:04:32.000000 caerp_celery-2024.1.2a3/src/caerp_celery/tasks/utils.py
--rw-r--r--   0 gas       (1000) gas       (1000)     2765 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a3/src/caerp_celery/transactional_task.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-02 15:11:22.425054 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     1411 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       84 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/entry_points.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-06 10:23:24.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/not-zip-safe
--rw-r--r--   0 gas       (1000) gas       (1000)       45 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       13 2024-05-02 15:11:22.000000 caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/top_level.txt
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-14 15:09:16.664518 caerp_celery-2024.1.2a4/
+-rw-r--r--   0 gas       (1000) gas       (1000)      334 2024-03-06 11:08:10.000000 caerp_celery-2024.1.2a4/CHANGELOG
+-rw-r--r--   0 gas       (1000) gas       (1000)       11 2024-05-14 15:08:41.000000 caerp_celery-2024.1.2a4/CURRENT_VERSION
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-06-24 14:37:06.000000 caerp_celery-2024.1.2a4/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      210 2024-03-06 10:24:06.000000 caerp_celery-2024.1.2a4/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-05-14 15:09:16.663519 caerp_celery-2024.1.2a4/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     2627 2024-03-05 16:04:43.000000 caerp_celery-2024.1.2a4/README.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       46 2024-03-08 17:12:36.000000 caerp_celery-2024.1.2a4/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       38 2024-05-14 15:09:16.664518 caerp_celery-2024.1.2a4/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1372 2024-03-06 11:04:59.000000 caerp_celery-2024.1.2a4/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-14 15:09:16.657518 caerp_celery-2024.1.2a4/src/
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-14 15:09:16.660519 caerp_celery-2024.1.2a4/src/caerp_celery/
+-rw-r--r--   0 gas       (1000) gas       (1000)     4579 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1789 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      585 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/exception.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      576 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/hacks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      753 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/interfaces.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      885 2024-05-02 14:38:26.000000 caerp_celery-2024.1.2a4/src/caerp_celery/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5747 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7465 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/models.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-14 15:09:16.661518 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/
+-rw-r--r--   0 gas       (1000) gas       (1000)     2163 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3533 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/cegid.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3133 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/ebp.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3376 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/isacompta.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3264 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/quadra.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3391 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/sage.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     5798 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/parsers/sage_generation_expert.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-14 15:09:16.662518 caerp_celery-2024.1.2a4/src/caerp_celery/schedulers/
+-rw-r--r--   0 gas       (1000) gas       (1000)       29 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/schedulers/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      428 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/schedulers/tasks.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-14 15:09:16.663519 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/
+-rw-r--r--   0 gas       (1000) gas       (1000)    13615 2024-05-14 15:08:34.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/__init__.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    39090 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/accounting_measure_compute.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    14135 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/accounting_parser.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    29193 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/csv_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    25097 2024-05-14 15:08:34.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2015 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/json_import.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      392 2024-04-25 07:56:31.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/locks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4428 2024-03-05 16:01:26.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/mail.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1423 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/notification.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3397 2024-03-15 11:24:28.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/tasks.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      509 2024-03-15 11:23:43.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/user_connections.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6912 2024-04-25 09:04:32.000000 caerp_celery-2024.1.2a4/src/caerp_celery/tasks/utils.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     2765 2024-03-05 10:21:09.000000 caerp_celery-2024.1.2a4/src/caerp_celery/transactional_task.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2024-05-14 15:09:16.661518 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)     3213 2024-05-14 15:09:16.000000 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     1411 2024-05-14 15:09:16.000000 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-05-14 15:09:16.000000 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       84 2024-05-14 15:09:16.000000 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/entry_points.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2024-03-06 10:23:24.000000 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/not-zip-safe
+-rw-r--r--   0 gas       (1000) gas       (1000)       45 2024-05-14 15:09:16.000000 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       13 2024-05-14 15:09:16.000000 caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/top_level.txt
```

### Comparing `caerp_celery-2024.1.2a3/LICENSE.txt` & `caerp_celery-2024.1.2a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/PKG-INFO` & `caerp_celery-2024.1.2a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp_celery
-Version: 2024.1.2a3
+Version: 2024.1.2a4
 Summary: caerp_celery
 Home-page: https://framagit.org/caerp/caerp_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `caerp_celery-2024.1.2a3/README.rst` & `caerp_celery-2024.1.2a4/README.rst`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/setup.py` & `caerp_celery-2024.1.2a4/setup.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/__init__.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/conf.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/conf.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/exception.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/exception.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/hacks.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/hacks.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/interfaces.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/interfaces.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/locks.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/locks.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/mail.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/mail.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/models.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/models.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/__init__.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/cegid.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/parsers/cegid.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/ebp.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/parsers/ebp.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/isacompta.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/parsers/isacompta.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/quadra.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/parsers/quadra.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/parsers/sage.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/parsers/sage_generation_expert.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/parsers/sage_generation_expert.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/__init__.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,28 +55,48 @@
         datas = []
         for company in user_account.companies:
             datas.append(company.code_compta)
         writer.add_extra_datas(datas)
     return writer
 
 
-def _add_invoice_custom_headers(writer, invoices):
+def _add_invoice_custom_headers(writer, query):
     """
     Invoice export headers
 
     * Entreprise ;
     • Client ;
     • Date ;
     • Numéro de factures ;
     • Objet ;
     • Lieu des travaux ;
     • HT (par taux de tva) ;
     • TVA (par taux de tva) ;
     • TTC.
     """
+    return _add_task_custom_headers(writer, query, topay=True)
+
+
+def _add_estimation_custom_headers(writer, query):
+    """
+    Estimation export headers
+
+    * Entreprise ;
+    • Client ;
+    • Date ;
+    • Objet ;
+    • Lieu des travaux ;
+    • HT (par taux de tva) ;
+    • TVA (par taux de tva) ;
+    • TTC.
+    """
+    return _add_task_custom_headers(writer, query, topay=False)
+
+
+def _add_task_custom_headers(writer, query, topay):
     for tva in Tva.query():
         writer.add_extra_header(
             {
                 "label": "HT {tva.name}".format(tva=tva),
                 "name": "HT {tva.value}".format(tva=tva),
             }
         )
@@ -84,15 +104,16 @@
 
     writer.add_extra_header({"label": "Assurance", "name": "insurance_label"})
     writer.add_extra_header({"label": "Taux d'assurance", "name": "insurance_rate"})
     writer.add_extra_header(
         {"label": "Montant de l'assurance", "name": "insurance_amount"}
     )
     writer.add_extra_header({"label": "Montant TTC", "name": "ttc"})
-    writer.add_extra_header({"label": "Montant restant dû", "name": "topay"})
+    if topay:
+        writer.add_extra_header({"label": "Montant restant dû", "name": "topay"})
     return writer
 
 
 def _add_invoice_datas(writer, invoice):
     _has_insurance_module = False
     if CustomInvoiceBookEntryModule.get_by_name("insurance", invoice.prefix):
         _has_insurance_module = True
@@ -144,14 +165,66 @@
         datas.append(integer_to_amount(invoice.topay(), precision=5))
     else:
         datas.append(0)
     writer.add_extra_datas(datas)
     return writer
 
 
+def _add_estimation_datas(writer, invoice):
+    _has_insurance_module = False
+    if CustomInvoiceBookEntryModule.get_by_name("insurance", invoice.prefix):
+        _has_insurance_module = True
+
+    ht_values = invoice.tva_ht_parts()
+    tva_values = invoice.get_tvas()
+    datas = []
+    for tva in Tva.query():
+        datas.append(integer_to_amount(ht_values.get(tva.value, 0), precision=5))
+        datas.append(integer_to_amount(tva_values.get(tva.value, 0), precision=5))
+
+    if invoice.insurance:
+        datas.append(invoice.insurance.label)
+    else:
+        if not _has_insurance_module:
+            datas.append("")
+        else:
+            level = invoice.get_rate_level("insurance")
+            if level == "cae":
+                datas.append("Taux de la CAE (module assurance)")
+            elif level == "company":
+                datas.append("Taux d'assurance de l'enseigne")
+            else:
+                datas.append("")
+
+    if _has_insurance_module:
+        rate = invoice.get_rate("insurance")
+        if not rate:
+            rate = 0
+    else:
+        if invoice.insurance:
+            rate = invoice.insurance.rate
+        else:
+            rate = 0
+    datas.append("{} %".format(rate))
+
+    if _has_insurance_module:
+        insurance = invoice.total_insurance(invoice.ht)
+        rounded = translate_integer_precision(insurance)
+    else:
+        if invoice.insurance:
+            insurance = invoice.total_insurance(invoice.ht)
+            rounded = translate_integer_precision(insurance)
+        else:
+            rounded = 0
+    datas.append(integer_to_amount(rounded, precision=2))
+    datas.append(integer_to_amount(invoice.ttc, precision=5))
+    writer.add_extra_datas(datas)
+    return writer
+
+
 def _add_supplier_invoice_custom_headers(writer, supplier_invoices):
     writer.add_extra_header({"label": "Montant HT", "name": "ht"})
     writer.add_extra_header({"label": "Montant TVA", "name": "tva"})
     writer.add_extra_header({"label": "Montant TTC", "name": "ttc"})
     writer.add_extra_header({"label": "Type", "name": "typ"})
     writer.add_extra_header({"label": "Statut", "name": "status"})
     return writer
@@ -344,7 +417,24 @@
                 "credit",
                 "balance",
                 "analytical_account",
                 "company",
             ),
         },
     )
+    config.register_export_model(
+        key="estimations",
+        model=Task,
+        options={
+            "hook_init": _add_estimation_custom_headers,
+            "hook_add_row": _add_estimation_datas,
+            "foreign_key_name": "task_id",
+            "excludes": ("name", "created_at", "updated_at", "type_"),
+            "order": (
+                "company",
+                "customer",
+                "date",
+                "description",
+                "workplace",
+            ),
+        },
+    )
```

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_measure_compute.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/accounting_measure_compute.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/accounting_parser.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/accounting_parser.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/csv_import.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/csv_import.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/export.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -349,14 +349,87 @@
     result_filename = os.path.basename(filepath)
 
     logger.debug(f" -> The file {result_filename} been written")
     return result_filename
 
 
 @celery_app.task(bind=True)
+@cache_region("default_term", "estimations_details")
+def export_estimations_details_to_file(self, job_id, task_ids, format="csv"):
+    """
+    Exporting details (each lines) of given estimations
+
+    :param int job_id: The id of the job object
+    :param list task_ids: List of estimations ids to query
+    :param str format: The format in which we want to export
+    """
+
+    logger.debug(
+        f" + Exporting details for the following estimations's ids : {task_ids}"
+    )
+
+    # Mark job started
+    utils.start_job(self.request, FileGenerationJob, job_id)
+
+    headers = (
+        {"label": "Enseigne", "name": "company"},
+        {"label": "N°Devis", "name": "estimation_number"},
+        {"label": "Date", "name": "estimation_date"},
+        {"label": "Client", "name": "customer"},
+        {"label": "Description", "name": "description"},
+        {"label": "Prix Unit. HT", "name": "unit_ht"},
+        {"label": "Prix Unit. TTC", "name": "unit_ttc"},
+        {"label": "Quantité", "name": "quantity"},
+        {"label": "Unité", "name": "unity"},
+        {"label": "TVA", "name": "tva"},
+        {"label": "Total HT", "name": "total_ht"},
+        {"label": "Total TVA", "name": "tva_amount"},
+        {"label": "Total TTC", "name": "total_ttc"},
+        {"label": "Compte produit", "name": "product"},
+    )
+
+    try:
+        data = []
+        query = Task.query().filter(Task.id.in_(task_ids))
+        for estimation in query:
+            logger.debug(f" + Collecting data for estimation {estimation.id}")
+            for line in estimation.all_lines:
+                logger.debug(f"    > Computing data for line {line.id}")
+                row_data = {
+                    "company": estimation.company.name,
+                    "estimation_number": estimation.internal_number,
+                    "estimation_date": format_date(estimation.date),
+                    "customer": estimation.customer.label,
+                    "description": strip_html_tags(line.description),
+                    "unit_ht": integer_to_amount(line.unit_ht(), 5),
+                    "unit_ttc": integer_to_amount(line.unit_ttc(), 5),
+                    "quantity": line.quantity,
+                    "unity": line.unity,
+                    "tva": integer_to_amount(max(line.get_tva(), 0), 4),
+                    "total_ht": integer_to_amount(line.total_ht(), 5),
+                    "tva_amount": integer_to_amount(line.tva_amount(), 5),
+                    "total_ttc": integer_to_amount(line.total(), 5),
+                    "product": line.product.name if line.product else "",
+                }
+                data.append(row_data)
+        logger.info(" + All estimations's details data where collected !")
+
+        result_filename = _export_data_to_tabular_file(
+            headers, data, filename="detail_devis_", file_format=format
+        )
+    except Exception:
+        logger.exception("Error while generating export file")
+        errors = [GENERATION_ERROR_MESSAGE % job_id]
+        utils.record_failure(FileGenerationJob, job_id, errors)
+    else:
+        utils.record_completed(FileGenerationJob, job_id, filename=result_filename)
+    return ""
+
+
+@celery_app.task(bind=True)
 @cache_region("default_term", "invoices_details")
 def export_invoices_details_to_file(self, job_id, task_ids, format="csv"):
     """
     Exporting details (each lines) of given invoices
 
     :param int job_id: The id of the job object
     :param list task_ids: List of invoices ids to query
@@ -452,14 +525,15 @@
         {"label": "Mois", "name": "month"},
         {"label": "HT", "name": "ht"},
         {"label": "TVA", "name": "tva"},
         {"label": "TTC", "name": "ttc"},
         {"label": "Km", "name": "km"},
         {"label": "Justificatifs reçus et acceptés", "name": "justified"},
         {"label": "Paiements", "name": "paid"},
+        {"label": "Montant restant dû", "name": "topay"},
     )
 
     expense_justified_status = {
         0: "non",
         1: "oui",
     }
     expense_paid_status = {
@@ -468,14 +542,19 @@
         "waiting": "en attente",
     }
 
     try:
         data = []
         query = ExpenseSheet.query().filter(ExpenseSheet.id.in_(expense_ids))
         for expense in query:
+            # compute topay column
+            topay = 0
+            if hasattr(expense, "topay") and not expense.paid_status == "resulted":
+                topay = integer_to_amount(expense.topay())
+
             row_data = {
                 "official_number": expense.official_number,
                 "title": expense.title,
                 "user_name": expense.user.label,
                 "company_name": expense.company.name,
                 "year": expense.year,
                 "month": expense.month,
@@ -485,14 +564,15 @@
                 "km": integer_to_amount(expense.total_km),
                 "justified": expense_justified_status.get(
                     expense.justified, expense.justified
                 ),
                 "paid": expense_paid_status.get(
                     expense.paid_status, expense.paid_status
                 ),
+                "topay": topay,
             }
             data.append(row_data)
         result_filename = _export_data_to_tabular_file(
             headers, data, filename=filename, file_format=format
         )
     except Exception:
         logger.exception("Error while generating export file")
@@ -537,18 +617,18 @@
     headers = _transform_list_header_in_export_header(dataquery_object.headers())
     data = _transform_list_data_in_export_data(dataquery_object.data())
     logger.info(" + Query data collected !")
 
     # Exporting dataquery result in a file
     try:
         datequery_filename = f"{dataquery_object.name}_"
-        if start:
-            datequery_filename += f"{start[:10]}_"
-        if end:
-            datequery_filename += f"{end[:10]}_"
+        if dataquery_object.start_date:
+            datequery_filename += f"{dataquery_object.start_date.strftime('%Y-%m-%d')}_"
+        if dataquery_object.end_date:
+            datequery_filename += f"{dataquery_object.end_date.strftime('%Y-%m-%d')}_"
         result_filename = _export_data_to_tabular_file(
             headers, data, filename=datequery_filename, file_format=format
         )
     except Exception:
         logger.exception("Error while generating dataquery export file")
         errors = [GENERATION_ERROR_MESSAGE % job_id]
         utils.record_failure(FileGenerationJob, job_id, errors)
```

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/json_import.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/json_import.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/mail.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/mail.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/notification.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/tasks.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/tasks/utils.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery/transactional_task.py` & `caerp_celery-2024.1.2a4/src/caerp_celery/transactional_task.py`

 * *Files identical despite different names*

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/PKG-INFO` & `caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caerp-celery
-Version: 2024.1.2a3
+Version: 2024.1.2a4
 Summary: caerp_celery
 Home-page: https://framagit.org/caerp/caerp_celery
 Author: Coopérer Pour Entreprendre
 Author-email: contact@endi.coop
 License: GPLv3
 Keywords: web wsgi bfg pylons pyramid celery
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `caerp_celery-2024.1.2a3/src/caerp_celery.egg-info/SOURCES.txt` & `caerp_celery-2024.1.2a4/src/caerp_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

