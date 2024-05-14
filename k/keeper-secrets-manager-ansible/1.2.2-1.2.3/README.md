# Comparing `tmp/keeper-secrets-manager-ansible-1.2.2.tar.gz` & `tmp/keeper_secrets_manager_ansible-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-ansible-1.2.2.tar", last modified: Thu Feb 15 00:18:24 2024, max compression
+gzip compressed data, was "keeper_secrets_manager_ansible-1.2.3.tar", last modified: Tue May 14 19:28:33 2024, max compression
```

## Comparing `keeper-secrets-manager-ansible-1.2.2.tar` & `keeper_secrets_manager_ansible-1.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:18:24.753508 keeper-secrets-manager-ansible-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-02-15 00:18:24.753508 keeper-secrets-manager-ansible-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:18:24.749508 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/
--rw-r--r--   0 runner    (1001) docker     (127)    33185 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:18:24.749508 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:18:24.753508 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cache_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:18:24.753508 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/callback_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/callback_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/callback_plugins/keeper_redact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:18:24.753508 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/lookup_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/lookup_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/lookup_plugins/keeper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:18:24.753508 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-02-15 00:18:24.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-15 00:18:24.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 00:18:24.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-15 00:18:24.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 00:18:24.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-15 00:18:24.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-15 00:18:24.000000 keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 00:18:24.753508 keeper-secrets-manager-ansible-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-02-15 00:17:44.000000 keeper-secrets-manager-ansible-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:28:33.094883 keeper_secrets_manager_ansible-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-14 19:28:33.094883 keeper_secrets_manager_ansible-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:28:33.090883 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/
+-rw-r--r--   0 runner    (1001) docker     (127)    33185 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:28:33.090883 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:28:33.094883 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cache_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:28:33.094883 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/callback_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/callback_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/callback_plugins/keeper_redact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:28:33.094883 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/lookup_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/lookup_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/lookup_plugins/keeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:28:33.094883 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-14 19:28:33.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-14 19:28:33.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:28:33.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 19:28:33.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:28:33.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 19:28:33.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 19:28:33.000000 keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:28:33.094883 keeper_secrets_manager_ansible-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-14 19:27:56.000000 keeper_secrets_manager_ansible-1.2.3/setup.py
```

### Comparing `keeper-secrets-manager-ansible-1.2.2/PKG-INFO` & `keeper_secrets_manager_ansible-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-ansible
-Version: 1.2.2
+Version: 1.2.3
 Summary: Keeper Secrets Manager plugins for Ansible.
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: ops@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://app.gitbook.com/@keeper-security/s/secrets-manager/secrets-manager/integrations/ansible-plugin
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: keeper-secrets-manager-core>=16.6.2
+Requires-Dist: keeper-secrets-manager-core>=16.6.4
 Requires-Dist: keeper-secrets-manager-helper
 Requires-Dist: importlib_metadata
 Requires-Dist: ansible
 
 # Keeper Secrets Manager Ansible
 
 This module contains plugins that allow your Ansible automations to use Keeper Secrets Manager. 
@@ -49,33 +49,36 @@
 * `keeper_info` - Display information about plugin, record and field types.
 * `keeper_remove` - Remove secrets from the Keeper Vault.
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/integrations/ansible-plugin
 
 # Changes
 
+## 1.2.3
+* Updated pinned KSM SDK version to 16.6.4.
+
 ## 1.2.2
-* Add action `keeper_get_record` to return record as a dictionary.
+* Added action `keeper_get_record` to return record as a dictionary.
 * Clean up comments.
-* Update pinned KSM SDK version to 16.6.3.
+* Updated pinned KSM SDK version to 16.6.3.
 
 ## 1.2.1
-* Add action `keeper_remove` to remove secrets from the Keeper Vault
-* Update pinned KSM SDK version to 16.6.2.
+* Added action `keeper_remove` to remove secrets from the Keeper Vault
+* Updated pinned KSM SDK version to 16.6.2.
 
 ## 1.2.0
 
 * Added action `keeper_cache_records` to cache Keeper Vault records to reduce API calls.
 * Added ability to get records by title for some actions.
 * Added `array_index` and `value_key` to access individual values in complex values. Alternative to `notation`.
-* Update pinned KSM SDK version.
+* Updated pinned KSM SDK version.
 
 ## 1.1.5
 
-* Update pinned KSM SDK version. The KSM SDK has been updated to use OpenSSL 3.0.7 which resolves CVE-2022-3602, CVE-2022-3786.
+* Updated pinned KSM SDK version. The KSM SDK has been updated to use OpenSSL 3.0.7 which resolves CVE-2022-3602, CVE-2022-3786.
 
 ## 1.1.4
 
 * Move check for custom record type in `keeper_create` plugin.
 * Keeper Secret Manager SDK version pinned to 16.3.5 or greater. Allows extra field parameters
 that come from Keeper Commander.
```

### Comparing `keeper-secrets-manager-ansible-1.2.2/README.md` & `keeper_secrets_manager_ansible-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,33 +15,36 @@
 * `keeper_info` - Display information about plugin, record and field types.
 * `keeper_remove` - Remove secrets from the Keeper Vault.
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/integrations/ansible-plugin
 
 # Changes
 
+## 1.2.3
+* Updated pinned KSM SDK version to 16.6.4.
+
 ## 1.2.2
-* Add action `keeper_get_record` to return record as a dictionary.
+* Added action `keeper_get_record` to return record as a dictionary.
 * Clean up comments.
-* Update pinned KSM SDK version to 16.6.3.
+* Updated pinned KSM SDK version to 16.6.3.
 
 ## 1.2.1
-* Add action `keeper_remove` to remove secrets from the Keeper Vault
-* Update pinned KSM SDK version to 16.6.2.
+* Added action `keeper_remove` to remove secrets from the Keeper Vault
+* Updated pinned KSM SDK version to 16.6.2.
 
 ## 1.2.0
 
 * Added action `keeper_cache_records` to cache Keeper Vault records to reduce API calls.
 * Added ability to get records by title for some actions.
 * Added `array_index` and `value_key` to access individual values in complex values. Alternative to `notation`.
-* Update pinned KSM SDK version.
+* Updated pinned KSM SDK version.
 
 ## 1.1.5
 
-* Update pinned KSM SDK version. The KSM SDK has been updated to use OpenSSL 3.0.7 which resolves CVE-2022-3602, CVE-2022-3786.
+* Updated pinned KSM SDK version. The KSM SDK has been updated to use OpenSSL 3.0.7 which resolves CVE-2022-3602, CVE-2022-3786.
 
 ## 1.1.4
 
 * Move check for custom record type in `keeper_create` plugin.
 * Keeper Secret Manager SDK version pinned to 16.3.5 or greater. Allows extra field parameters
 that come from Keeper Commander.
```

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/__init__.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/__init__.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/__main__.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/__main__.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cache_records.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cache_records.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cleanup.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_cleanup.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_copy.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_copy.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_create.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_create.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get_record.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_get_record.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_info.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_info.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_init.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_init.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_password.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_password.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_remove.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_remove.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_set.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/action_plugins/keeper_set.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/callback_plugins/keeper_redact.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/callback_plugins/keeper_redact.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible/plugins/lookup_plugins/keeper.py` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible/plugins/lookup_plugins/keeper.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/PKG-INFO` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-ansible
-Version: 1.2.2
+Version: 1.2.3
 Summary: Keeper Secrets Manager plugins for Ansible.
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: ops@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://app.gitbook.com/@keeper-security/s/secrets-manager/secrets-manager/integrations/ansible-plugin
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: keeper-secrets-manager-core>=16.6.2
+Requires-Dist: keeper-secrets-manager-core>=16.6.4
 Requires-Dist: keeper-secrets-manager-helper
 Requires-Dist: importlib_metadata
 Requires-Dist: ansible
 
 # Keeper Secrets Manager Ansible
 
 This module contains plugins that allow your Ansible automations to use Keeper Secrets Manager. 
@@ -49,33 +49,36 @@
 * `keeper_info` - Display information about plugin, record and field types.
 * `keeper_remove` - Remove secrets from the Keeper Vault.
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/integrations/ansible-plugin
 
 # Changes
 
+## 1.2.3
+* Updated pinned KSM SDK version to 16.6.4.
+
 ## 1.2.2
-* Add action `keeper_get_record` to return record as a dictionary.
+* Added action `keeper_get_record` to return record as a dictionary.
 * Clean up comments.
-* Update pinned KSM SDK version to 16.6.3.
+* Updated pinned KSM SDK version to 16.6.3.
 
 ## 1.2.1
-* Add action `keeper_remove` to remove secrets from the Keeper Vault
-* Update pinned KSM SDK version to 16.6.2.
+* Added action `keeper_remove` to remove secrets from the Keeper Vault
+* Updated pinned KSM SDK version to 16.6.2.
 
 ## 1.2.0
 
 * Added action `keeper_cache_records` to cache Keeper Vault records to reduce API calls.
 * Added ability to get records by title for some actions.
 * Added `array_index` and `value_key` to access individual values in complex values. Alternative to `notation`.
-* Update pinned KSM SDK version.
+* Updated pinned KSM SDK version.
 
 ## 1.1.5
 
-* Update pinned KSM SDK version. The KSM SDK has been updated to use OpenSSL 3.0.7 which resolves CVE-2022-3602, CVE-2022-3786.
+* Updated pinned KSM SDK version. The KSM SDK has been updated to use OpenSSL 3.0.7 which resolves CVE-2022-3602, CVE-2022-3786.
 
 ## 1.1.4
 
 * Move check for custom record type in `keeper_create` plugin.
 * Keeper Secret Manager SDK version pinned to 16.3.5 or greater. Allows extra field parameters
 that come from Keeper Commander.
```

### Comparing `keeper-secrets-manager-ansible-1.2.2/keeper_secrets_manager_ansible.egg-info/SOURCES.txt` & `keeper_secrets_manager_ansible-1.2.3/keeper_secrets_manager_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-ansible-1.2.2/setup.py` & `keeper_secrets_manager_ansible-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 os.chdir(here)
 
 # Get the long description from the README.md file
 with open(os.path.join(here, 'README.md'), "r", encoding='utf-8') as fp:
     long_description = fp.read()
 
 install_requires = [
-    'keeper-secrets-manager-core>=16.6.2',
+    'keeper-secrets-manager-core>=16.6.4',
     'keeper-secrets-manager-helper',
     'importlib_metadata',
     'ansible'
 ]
 
 setup(
     name="keeper-secrets-manager-ansible",
-    version='1.2.2',
+    version='1.2.3',
     description="Keeper Secrets Manager plugins for Ansible.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="ops@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

