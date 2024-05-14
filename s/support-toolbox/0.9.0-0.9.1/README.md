# Comparing `tmp/support-toolbox-0.9.0.tar.gz` & `tmp/support-toolbox-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "support-toolbox-0.9.0.tar", last modified: Wed May  8 14:50:45 2024, max compression
+gzip compressed data, was "support-toolbox-0.9.1.tar", last modified: Tue May 14 02:45:18 2024, max compression
```

## Comparing `support-toolbox-0.9.0.tar` & `support-toolbox-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.425810 support-toolbox-0.9.0/support_toolbox/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4294 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/entitlements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/org.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2206 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/site.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/api/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox/app_handler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/app.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/app_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/auto_updater.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/app_handler/token_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/clear_user_layer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/delete_users.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_browse_card.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_ctk_service_account.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_integrations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18802 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/deploy_pi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/onboard_ctk_orgs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2158 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/revert_soft_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/update_saml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1969 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/api_url.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/csv_to_iris.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6168 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/resource_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-05-08 14:50:36.000000 support-toolbox-0.9.0/support_toolbox/utils/saml_parser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 14:50:45.433811 support-toolbox-0.9.0/support_toolbox.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-08 14:50:45.000000 support-toolbox-0.9.0/support_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2495 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-14 02:45:18.462542 support-toolbox-0.9.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.450542 support-toolbox-0.9.1/support_toolbox/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4294 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/entitlements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2549 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/org.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1338 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3675 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2206 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/site.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/api/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox/app_handler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/app.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/app_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/auto_updater.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/app_handler/token_manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3845 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/clear_user_layer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4590 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/delete_users.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2208 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_browse_card.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1355 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_ctk_service_account.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5379 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_integrations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18802 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/deploy_pi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      294 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/onboard_ctk_orgs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2158 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/revert_soft_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/update_saml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1969 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/api_url.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/csv_to_iris.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6258 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/resource_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2024-05-14 02:45:11.000000 support-toolbox-0.9.1/support_toolbox/utils/saml_parser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-14 02:45:18.458542 support-toolbox-0.9.1/support_toolbox.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-14 02:45:18.000000 support-toolbox-0.9.1/support_toolbox.egg-info/top_level.txt
```

### Comparing `support-toolbox-0.9.0/PKG-INFO` & `support-toolbox-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: support-toolbox
-Version: 0.9.0
+Version: 0.9.1
 Summary: A suite of CLI tools for the data.world support team
 Home-page: https://github.com/datadotworld/support-toolbox/tree/main
 Author: Jack Compton
 Author-email: jack.compton@data.world
 Requires-Dist: certifi==2023.7.22
 Requires-Dist: charset-normalizer==3.2.0
 Requires-Dist: defusedxml==0.7.1
```

### Comparing `support-toolbox-0.9.0/README.md` & `support-toolbox-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/setup.py` & `support-toolbox-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/dataset.py` & `support-toolbox-0.9.1/support_toolbox/api/dataset.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/entitlements.py` & `support-toolbox-0.9.1/support_toolbox/api/entitlements.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/file.py` & `support-toolbox-0.9.1/support_toolbox/api/file.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/org.py` & `support-toolbox-0.9.1/support_toolbox/api/org.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/project.py` & `support-toolbox-0.9.1/support_toolbox/api/project.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/service_account.py` & `support-toolbox-0.9.1/support_toolbox/api/service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/site.py` & `support-toolbox-0.9.1/support_toolbox/api/site.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/api/user.py` & `support-toolbox-0.9.1/support_toolbox/api/user.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/app_handler/app.py` & `support-toolbox-0.9.1/support_toolbox/app_handler/app.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/app_handler/auto_updater.py` & `support-toolbox-0.9.1/support_toolbox/app_handler/auto_updater.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/app_handler/token_manager.py` & `support-toolbox-0.9.1/support_toolbox/app_handler/token_manager.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/clear_user_layer.py` & `support-toolbox-0.9.1/support_toolbox/clear_user_layer.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/delete_users.py` & `support-toolbox-0.9.1/support_toolbox/delete_users.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/deploy_browse_card.py` & `support-toolbox-0.9.1/support_toolbox/deploy_browse_card.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/deploy_ctk_service_account.py` & `support-toolbox-0.9.1/support_toolbox/deploy_ctk_service_account.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/deploy_integrations.py` & `support-toolbox-0.9.1/support_toolbox/deploy_integrations.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/deploy_pi.py` & `support-toolbox-0.9.1/support_toolbox/deploy_pi.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/onboard_ctk_orgs.py` & `support-toolbox-0.9.1/support_toolbox/onboard_ctk_orgs.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/revert_soft_delete.py` & `support-toolbox-0.9.1/support_toolbox/revert_soft_delete.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/update_saml.py` & `support-toolbox-0.9.1/support_toolbox/update_saml.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/utils/api_url.py` & `support-toolbox-0.9.1/support_toolbox/utils/api_url.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/utils/metrics.py` & `support-toolbox-0.9.1/support_toolbox/utils/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     # Optional override of standard naming convention (rare but has happened before)
     standard_org_choice = input("Use the standard Data Catalog Team org (y/n): ")
     if standard_org_choice.lower() == 'n':
         org_id = input("Enter the org id: ")
         org_display_name = input("Enter the org display name: ")
 
     print(f"Onboarding {org_id}...")
-    onboard_org(api_url, admin_token, org_id, org_display_name)
+    onboard_org(api_url, admin_token, org_id, org_display_name, avatar_url="https://media.data.world/Gdb7BAcmT2Oac1801FK7_data%20catalog%20team.png.jpg")
 
     print(f"Authorizing datadotworldsupport access to {org_id}...")
     authorize_access_to_org(api_url, admin_token, org_id, party='group:datadotworldsupport/members')
 
     if existing_customer:
         # Create the baseplatformdata dataset and subsequent four datasets that makeup baseplatformdata - this is default an "All Time" metrics deployment for Existing Customers
         for dataset in BASEPLATFORM_DATASETS:
```

### Comparing `support-toolbox-0.9.0/support_toolbox/utils/resource_type.py` & `support-toolbox-0.9.1/support_toolbox/utils/resource_type.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox/utils/saml_parser.py` & `support-toolbox-0.9.1/support_toolbox/utils/saml_parser.py`

 * *Files identical despite different names*

### Comparing `support-toolbox-0.9.0/support_toolbox.egg-info/PKG-INFO` & `support-toolbox-0.9.1/support_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: support-toolbox
-Version: 0.9.0
+Version: 0.9.1
 Summary: A suite of CLI tools for the data.world support team
 Home-page: https://github.com/datadotworld/support-toolbox/tree/main
 Author: Jack Compton
 Author-email: jack.compton@data.world
 Requires-Dist: certifi==2023.7.22
 Requires-Dist: charset-normalizer==3.2.0
 Requires-Dist: defusedxml==0.7.1
```

### Comparing `support-toolbox-0.9.0/support_toolbox.egg-info/SOURCES.txt` & `support-toolbox-0.9.1/support_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

