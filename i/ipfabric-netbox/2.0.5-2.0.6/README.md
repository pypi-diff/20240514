# Comparing `tmp/ipfabric_netbox-2.0.5.tar.gz` & `tmp/ipfabric_netbox-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_netbox-2.0.5.tar", last modified: Tue Apr 30 11:01:56 2024, max compression
+gzip compressed data, was "ipfabric_netbox-2.0.6.tar", last modified: Tue May 14 16:19:48 2024, max compression
```

## Comparing `ipfabric_netbox-2.0.5.tar` & `ipfabric_netbox-2.0.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/
--rw-r--r--   0 root         (0) root         (0)       46 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1750 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1141 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.544570 ipfabric_netbox-2.0.5/ipfabric_netbox/
--rw-r--r--   0 root         (0) root         (0)     1251 2024-04-30 11:01:34.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.548570 ipfabric_netbox-2.0.5/ipfabric_netbox/api/
--rw-r--r--   0 root         (0) root         (0)      101 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2684 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/api/nested_serializers.py
--rw-r--r--   0 root         (0) root         (0)     4307 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/api/serializers.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/api/urls.py
--rw-r--r--   0 root         (0) root         (0)     4429 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/api/views.py
--rw-r--r--   0 root         (0) root         (0)     4848 2024-04-23 10:08:08.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/choices.py
--rw-r--r--   0 root         (0) root         (0)     3877 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/filtersets.py
--rw-r--r--   0 root         (0) root         (0)    43154 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/forms.py
--rw-r--r--   0 root         (0) root         (0)     2395 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/jobs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.548570 ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/
--rw-r--r--   0 root         (0) root         (0)    13813 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      431 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/0002_ipfabricsnapshot_status.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/0004_ipfabricsync_auto_merge.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29506 2024-04-30 11:01:34.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/models.py
--rw-r--r--   0 root         (0) root         (0)     1907 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/navigation.py
--rw-r--r--   0 root         (0) root         (0)     3357 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/signals.py
--rw-r--r--   0 root         (0) root         (0)     6630 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/tables.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-03-08 10:45:55.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/template_content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.544570 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.552570 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.556570 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/
--rw-r--r--   0 root         (0) root         (0)     3229 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html
--rw-r--r--   0 root         (0) root         (0)      569 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html
--rw-r--r--   0 root         (0) root         (0)      295 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/logs_pending.html
--rw-r--r--   0 root         (0) root         (0)      710 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html
--rw-r--r--   0 root         (0) root         (0)     2674 2024-03-18 10:24:22.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html
--rw-r--r--   0 root         (0) root         (0)     2136 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html
--rw-r--r--   0 root         (0) root         (0)     2885 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html
--rw-r--r--   0 root         (0) root         (0)      717 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html
--rw-r--r--   0 root         (0) root         (0)      517 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html
--rw-r--r--   0 root         (0) root         (0)      521 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html
--rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html
--rw-r--r--   0 root         (0) root         (0)     6444 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html
--rw-r--r--   0 root         (0) root         (0)     3482 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html
--rw-r--r--   0 root         (0) root         (0)     3859 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html
--rw-r--r--   0 root         (0) root         (0)     3881 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html
--rw-r--r--   0 root         (0) root         (0)     1100 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_list.html
--rw-r--r--   0 root         (0) root         (0)     2562 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/
--rw-r--r--   0 root         (0) root         (0)      368 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_all.html
--rw-r--r--   0 root         (0) root         (0)      590 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html
--rw-r--r--   0 root         (0) root         (0)       81 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_status.html
--rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html
--rw-r--r--   0 root         (0) root         (0)      167 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/sync_last_branch.html
--rw-r--r--   0 root         (0) root         (0)     5606 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.544570 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.544570 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/static/ipfabric_netbox/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/static/ipfabric_netbox/css/
--rw-r--r--   0 root         (0) root         (0)      118 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/templates/static/ipfabric_netbox/css/rack.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/ipfabric_netbox/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45898 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     4430 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20299 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/ipfutils.py
--rw-r--r--   0 root         (0) root         (0)     3221 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/logging.py
--rw-r--r--   0 root         (0) root         (0)     3119 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/nbutils.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/transform_map.py
--rw-r--r--   0 root         (0) root         (0)    28517 2024-03-18 10:24:22.000000 ipfabric_netbox-2.0.5/ipfabric_netbox/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1750 2024-04-30 11:01:56.000000 ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2942 2024-04-30 11:01:56.000000 ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 11:01:56.000000 ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 17:00:30.000000 ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-30 11:01:56.000000 ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-30 11:01:56.000000 ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 11:01:56.560570 ipfabric_netbox-2.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-30 11:01:34.000000 ipfabric_netbox-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/
+-rw-r--r--   0 root         (0) root         (0)       46 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/
+-rw-r--r--   0 root         (0) root         (0)     1251 2024-05-14 16:18:34.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.390452 ipfabric_netbox-2.0.6/ipfabric_netbox/api/
+-rw-r--r--   0 root         (0) root         (0)      101 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/nested_serializers.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/serializers.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4429 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/api/views.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2024-04-23 10:08:08.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/choices.py
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/filtersets.py
+-rw-r--r--   0 root         (0) root         (0)    43154 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/forms.py
+-rw-r--r--   0 root         (0) root         (0)     2395 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/jobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.390452 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/
+-rw-r--r--   0 root         (0) root         (0)    13813 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      431 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0002_ipfabricsnapshot_status.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0004_ipfabricsync_auto_merge.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29506 2024-05-14 16:17:46.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/models.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/navigation.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/signals.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/tables.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-03-08 10:45:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/template_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.390452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html
+-rw-r--r--   0 root         (0) root         (0)      569 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html
+-rw-r--r--   0 root         (0) root         (0)      295 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/logs_pending.html
+-rw-r--r--   0 root         (0) root         (0)      710 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html
+-rw-r--r--   0 root         (0) root         (0)     2674 2024-03-18 10:24:22.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html
+-rw-r--r--   0 root         (0) root         (0)     2136 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html
+-rw-r--r--   0 root         (0) root         (0)      717 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html
+-rw-r--r--   0 root         (0) root         (0)      517 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html
+-rw-r--r--   0 root         (0) root         (0)      521 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html
+-rw-r--r--   0 root         (0) root         (0)     6444 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html
+-rw-r--r--   0 root         (0) root         (0)     3859 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html
+-rw-r--r--   0 root         (0) root         (0)     3881 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html
+-rw-r--r--   0 root         (0) root         (0)      459 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_list.html
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/
+-rw-r--r--   0 root         (0) root         (0)      368 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_all.html
+-rw-r--r--   0 root         (0) root         (0)      590 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html
+-rw-r--r--   0 root         (0) root         (0)       81 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_status.html
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html
+-rw-r--r--   0 root         (0) root         (0)      167 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/sync_last_branch.html
+-rw-r--r--   0 root         (0) root         (0)     5606 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.386452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/ipfabric_netbox/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/ipfabric_netbox/css/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-03-11 10:17:28.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/templates/static/ipfabric_netbox/css/rack.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45898 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     4430 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20439 2024-05-14 16:18:34.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/ipfutils.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/logging.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-04-30 10:44:55.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/nbutils.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-02-20 16:51:44.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/transform_map.py
+-rw-r--r--   0 root         (0) root         (0)    28517 2024-03-18 10:24:22.000000 ipfabric_netbox-2.0.6/ipfabric_netbox/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2942 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 17:00:30.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-14 16:19:48.000000 ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 16:19:48.394452 ipfabric_netbox-2.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      961 2024-05-14 16:18:34.000000 ipfabric_netbox-2.0.6/setup.py
```

### Comparing `ipfabric_netbox-2.0.5/PKG-INFO` & `ipfabric_netbox-2.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric_netbox
-Version: 2.0.5
+Version: 2.0.6
 Summary: NetBox plugin to sync IP Fabric data into NetBox
 Home-page: https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Project-URL: Bug Tracker, https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfabric_netbox-2.0.5/README.md` & `ipfabric_netbox-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/__init__.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxIPFabricConfig(PluginConfig):
     name = "ipfabric_netbox"
     verbose_name = "NetBox IP Fabric SoT Plugin"
     description = "Sync IP Fabric into NetBox"
-    version = "2.0.5"
+    version = "2.0.6"
     base_url = "ipfabric"
 
     def ready(self):
         super().ready()
         try:
             from ipfabric_netbox.signals import ipfabric_netbox_init
```

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/api/nested_serializers.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/api/serializers.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/api/serializers.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/api/urls.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/api/urls.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/api/views.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/api/views.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/choices.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/choices.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/filtersets.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/filtersets.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/forms.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/forms.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/jobs.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/0001_initial.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/migrations/0003_ipfabricsource_type_and_more.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/models.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/models.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/navigation.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/navigation.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/signals.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/signals.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/tables.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/tables.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/diff.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/json.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/merge_form.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_button.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/site_topology_modal.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/snapshotdata.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/sync_delete.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_field_map.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/inc/transform_map_relationship_map.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabric_table.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricbranch.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsnapshot.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsource.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabricsync.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/ipfabrictransformmap_restore.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/branch_progress.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/partials/job_logs.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html` & `ipfabric_netbox-2.0.6/ipfabric_netbox/templates/ipfabric_netbox/sync_list.html`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/tests/test_models.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/urls.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/urls.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/ipfutils.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/ipfutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dcim.models import Device
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.shortcuts import get_object_or_404
 from django.utils.text import slugify
 from django_tables2 import Column
 from ipfabric import IPFClient
+from importlib import metadata
 from jinja2.sandbox import SandboxedEnvironment
 from netbox.config import get_config
 from netutils.utils import jinja2_convenience_function
 
 from ..choices import IPFabricSourceTypeChoices
 from .nbutils import device_serial_max_length
 from .nbutils import order_devices
@@ -51,14 +52,15 @@
     def __init__(self, parameters=None, transform_map=None) -> None:
         if parameters:
             self.ipf = IPFClient(**parameters, unloaded=True)
         else:
             self.ipf = IPFClient(
                 **settings.PLUGINS_CONFIG["ipfabric_netbox"], unloaded=True
             )
+        self.ipf._client.headers['user-agent'] += f'; ipfabric-netbox/{metadata.version("ipfabric-netbox")}'
         self.transform_map = transform_map
 
     def get_snapshots(self) -> dict:
         formatted_snapshots = {}
         if self.ipf:
             for snapshot_ref, snapshot in self.ipf.snapshots.items():
                 if snapshot.status != "done" and snapshot.finish_status != "done":
```

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/logging.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/nbutils.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/nbutils.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/utilities/transform_map.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/utilities/transform_map.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox/views.py` & `ipfabric_netbox-2.0.6/ipfabric_netbox/views.py`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/PKG-INFO` & `ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric_netbox
-Version: 2.0.5
+Version: 2.0.6
 Summary: NetBox plugin to sync IP Fabric data into NetBox
 Home-page: https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Project-URL: Bug Tracker, https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ipfabric_netbox-2.0.5/ipfabric_netbox.egg-info/SOURCES.txt` & `ipfabric_netbox-2.0.6/ipfabric_netbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipfabric_netbox-2.0.5/setup.py` & `ipfabric_netbox-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ipfabric_netbox",
-    version="2.0.5",
+    version="2.0.6",
     author="Solution Architecture",
     author_email="solution.architecture@ipfabric.io",
     description="NetBox plugin to sync IP Fabric data into NetBox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["ipfabric>=6.6.4", "netutils"],
     url="https://gitlab.com/ip-fabric/integrations/ipfabric-netbox-sync",
```

