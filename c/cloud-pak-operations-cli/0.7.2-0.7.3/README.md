# Comparing `tmp/cloud_pak_operations_cli-0.7.2.tar.gz` & `tmp/cloud_pak_operations_cli-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_pak_operations_cli-0.7.2.tar", last modified: Mon Apr 29 08:16:33 2024, max compression
+gzip compressed data, was "cloud_pak_operations_cli-0.7.3.tar", last modified: Tue May 14 15:22:03 2024, max compression
```

## Comparing `cloud_pak_operations_cli-0.7.2.tar` & `cloud_pak_operations_cli-0.7.3.tar`

### file list

```diff
@@ -1,205 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 08:16:33.000000 cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/download_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/get-shell-completion-script-location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.953149 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/set_config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/store_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/adm/update_dev.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/current.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/get_cluster_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/ls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/delete_terminated_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/reset_current_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_kubernetes_nfs_subdir_external_provisioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_openshift_data_foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/use.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/logout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.957149 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/regenerate_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/binaries_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    17370 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/cluster_credentials_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/config/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/cpo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.945149 cloud_pak_operations_cli-0.7.2/cpo/deps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/deploy_odf_playbook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.961149 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/abstract_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/openshift_playbook_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/playbook_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/click/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/cpd_service_spec_param_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/lazy_loading_multi_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/package_directory_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.965149 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/terraform_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/cluster_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/ingress_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/jmespath.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.969149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/token_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/user_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/global_pull_secret_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/oc.py
--rw-r--r--   0 runner    (1001) docker     (127)    46436 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_api_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.973149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/architecture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/auths_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/catalog_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource_event_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/get_pod_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/kind_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/object_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/operator_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/click.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/package_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.977149 cloud_pak_operations_cli-0.7.2/cpo/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/scripts/get_current_cluster_alias.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/cpo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/http_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/importlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/cpo/utils/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 08:16:19.000000 cloud_pak_operations_cli-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:16:33.981149 cloud_pak_operations_cli-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.881625 cloud_pak_operations_cli-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-14 15:22:03.881625 cloud_pak_operations_cli-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.881625 cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-14 15:22:03.000000 cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-14 15:22:03.000000 cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:22:03.000000 cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 15:22:03.000000 cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 15:22:03.000000 cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 15:22:03.000000 cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.857625 cloud_pak_operations_cli-0.7.3/cpo/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.857625 cloud_pak_operations_cli-0.7.3/cpo/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.857625 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/download_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/get-shell-completion-script-location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.861625 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/set_config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/store_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/adm/update_dev.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.861625 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/get_cluster_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/ls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.861625 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/operator/install_node_feature_discovery_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/operator/install_nvidia_gpu_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.861625 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pods/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pods/delete_terminated_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.861625 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/reset_current_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.861625 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/storage/install_kubernetes_nfs_subdir_external_provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/storage/install_openshift_data_foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/use.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/regenerate_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/config/binaries_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17370 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/config/cluster_credentials_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/config/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/cpo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.853625 cloud_pak_operations_cli-0.7.3/cpo/deps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/deps/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/deps/autocomplete/cpo-autocomplete-bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/deps/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/deps/playbooks/deploy_odf_playbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/deps/playbooks/install_node_feature_discovery_operator_playbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/deps/playbooks/install_nvidia_gpu_operator_playbook.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.865625 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.869625 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/abstract_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/wait_for_custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/openshift_playbook_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/playbook_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.869625 cloud_pak_operations_cli-0.7.3/cpo/lib/click/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/click/cpd_service_spec_param_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/click/lazy_loading_multi_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/click/package_directory_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.869625 cloud_pak_operations_cli-0.7.3/cpo/lib/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/cluster/cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.869625 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/dependency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/dependency_manager_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.869625 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.869625 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/terraform_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/ibm_internal_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibm_internal_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/data/cluster_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/data/ingress_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/ibm_cloud_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/jmespath.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/cluster/generic_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/cluster/generic_cluster_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/cluster_based_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/token_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/user_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.873625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/data/global_pull_secret_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.877625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/nfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/nfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/oc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46436 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_api_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.877625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/openshift_installation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.877625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/types/architecture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.877625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/auths_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/catalog_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/custom_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/custom_resource_event_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/get_pod_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/kind_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/object_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/operator_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/role_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.877625 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/utils/click.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.881625 cloud_pak_operations_cli-0.7.3/cpo/lib/plugin_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/plugin_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/plugin_manager/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/lib/plugin_manager/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.881625 cloud_pak_operations_cli-0.7.3/cpo/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/scripts/get_current_cluster_alias.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:22:03.881625 cloud_pak_operations_cli-0.7.3/cpo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/cpo/utils/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 15:21:59.000000 cloud_pak_operations_cli-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:22:03.881625 cloud_pak_operations_cli-0.7.3/setup.cfg
```

### Comparing `cloud_pak_operations_cli-0.7.2/LICENSE` & `cloud_pak_operations_cli-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/PKG-INFO` & `cloud_pak_operations_cli-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.7.2
+Version: 0.7.3
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.2 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.3 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `cloud_pak_operations_cli-0.7.2/README.md` & `cloud_pak_operations_cli-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/PKG-INFO` & `cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-pak-operations-cli
-Version: 0.7.2
+Version: 0.7.3
 Summary: IBM Cloud Pak Operations CLI
 Author-email: IBM Corporation <db2datagate@ibm.com>
 Project-URL: repository, https://github.com/IBM/cloud-pak-operations-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.2 Summary:
+Metadata-Version: 2.1 Name: cloud-pak-operations-cli Version: 0.7.3 Summary:
 IBM Cloud Pak Operations CLI Author-email: IBM Corporation
 ibm.com> Project-URL: repository, https://github.com/IBM/cloud-pak-operations-
 cli Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `cloud_pak_operations_cli-0.7.2/cloud_pak_operations_cli.egg-info/SOURCES.txt` & `cloud_pak_operations_cli-0.7.3/cloud_pak_operations_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 cpo/commands/cluster/edit.py
 cpo/commands/cluster/get_cluster_access_token.py
 cpo/commands/cluster/login.py
 cpo/commands/cluster/ls.py
 cpo/commands/cluster/reset_current_cluster.py
 cpo/commands/cluster/rm.py
 cpo/commands/cluster/use.py
+cpo/commands/cluster/operator/__init__.py
+cpo/commands/cluster/operator/install_node_feature_discovery_operator.py
+cpo/commands/cluster/operator/install_nvidia_gpu_operator.py
 cpo/commands/cluster/pods/__init__.py
 cpo/commands/cluster/pods/delete_terminated_pods.py
 cpo/commands/cluster/pull_secret/__init__.py
 cpo/commands/cluster/pull_secret/ls.py
 cpo/commands/cluster/pull_secret/rm.py
 cpo/commands/cluster/pull_secret/set.py
 cpo/commands/cluster/storage/__init__.py
@@ -55,14 +58,16 @@
 cpo/config/binaries_manager.py
 cpo/config/cluster_credentials_manager.py
 cpo/config/configuration_manager.py
 cpo/deps/autocomplete/cpo-autocomplete-bash.sh
 cpo/deps/autocomplete/cpo-autocomplete-zsh.sh
 cpo/deps/playbooks/delete_terminated_pods_playbook.yaml
 cpo/deps/playbooks/deploy_odf_playbook.yaml
+cpo/deps/playbooks/install_node_feature_discovery_operator_playbook.yaml
+cpo/deps/playbooks/install_nvidia_gpu_operator_playbook.yaml
 cpo/lib/__init__.py
 cpo/lib/jmespath.py
 cpo/lib/ansible/__init__.py
 cpo/lib/ansible/openshift_playbook_runner.py
 cpo/lib/ansible/playbook_runner.py
 cpo/lib/ansible/modules/__init__.py
 cpo/lib/ansible/modules/abstract_module.py
```

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/download_dependencies.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/download_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/get-shell-completion-script-location.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/get-shell-completion-script-location.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/install.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/install.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/ls.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/ls.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/ibm_internal_plugin/upgrade_plugins.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/set_config_option.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/set_config_option.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/store_credentials.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/store_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/adm/update_dev.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/adm/update_dev.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/add.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/add.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/current.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/current.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/edit.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/edit.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/get_cluster_access_token.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/get_cluster_access_token.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/login.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/ls.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pods/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pods/delete_terminated_pods.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pods/delete_terminated_pods.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/ls.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/ls.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/rm.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/rm.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/pull_secret/set.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/pull_secret/set.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/reset_current_cluster.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/reset_current_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/rm.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_kubernetes_nfs_subdir_external_provisioner.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/storage/install_kubernetes_nfs_subdir_external_provisioner.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/storage/install_openshift_data_foundation.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/storage/install_openshift_data_foundation.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/cluster/use.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/cluster/use.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/login.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/login.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/logout.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/logout.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/add.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/add.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/login.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/login.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/ls.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/rm.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/rm.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/oc/cluster/status.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/oc/cluster/status.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/commands/ibmcloud/regenerate_api_key.py` & `cloud_pak_operations_cli-0.7.3/cpo/commands/ibmcloud/regenerate_api_key.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/config/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/config/binaries_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/config/binaries_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/config/cluster_credentials_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/config/cluster_credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/config/configuration_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/config/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/cpo.py` & `cloud_pak_operations_cli-0.7.3/cpo/cpo.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-bash.sh` & `cloud_pak_operations_cli-0.7.3/cpo/deps/autocomplete/cpo-autocomplete-bash.sh`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh` & `cloud_pak_operations_cli-0.7.3/cpo/deps/autocomplete/cpo-autocomplete-zsh.sh`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml` & `cloud_pak_operations_cli-0.7.3/cpo/deps/playbooks/delete_terminated_pods_playbook.yaml`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/deps/playbooks/deploy_odf_playbook.yaml` & `cloud_pak_operations_cli-0.7.3/cpo/deps/playbooks/deploy_odf_playbook.yaml`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/abstract_module.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/abstract_module.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/custom_resource_event_result.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/custom_resource_event_result.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/wait_for_custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/wait_for_custom_resource_definitions.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/modules/wait_for_namespaced_custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/openshift_playbook_runner.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/openshift_playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ansible/playbook_runner.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ansible/playbook_runner.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/click/cpd_service_spec_param_type.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/click/cpd_service_spec_param_type.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/click/lazy_loading_multi_command.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/click/lazy_loading_multi_command.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/click/package_directory_details.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/click/package_directory_details.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/click/utils.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/click/utils.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/cluster/cluster_factory.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/cluster/cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/dependency_manager_binary_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,8 +94,16 @@
 
         Returns
         -------
         pathlib.Path
             path of the binary associated with the dependency
         """
 
-        return configuration_manager.get_bin_directory_path() / f"{self.get_binary_name()}-{version}"
+        binary_path = configuration_manager.get_bin_directory_path()
+
+        if self.is_located_in_subdirectory():
+            binary_path /= f"{self.get_dependency_alias()}-{version}"
+            binary_path /= self.get_binary_name()
+        else:
+            binary_path /= f"{self.get_binary_name()}-{version}"
+
+        return binary_path
```

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/dependency_manager_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/dependency_manager_plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -127,14 +127,27 @@
         DependencyVersion
             latest version of the dependency available at the official download
             location
         """
 
         pass
 
+    def is_located_in_subdirectory(self) -> bool:
+        """Returns whether the plug-in is located in a subdirectory
+
+        The name of the subdirectory must equal the alias of the dependency.
+
+        Returns
+        -------
+        bool
+            True, if the plug-in is located in a subdirectory
+        """
+
+        return False
+
     @abstractmethod
     def is_operating_system_supported(self, operating_system: OperatingSystem) -> bool:
         pass
 
     def _get_latest_dependency_version_on_github(self, owner: str, repo: str) -> DependencyVersion | None:
         """Returns the latest version of the dependency on GitHub
 
@@ -192,10 +205,10 @@
         response = requests.get(f"https://api.github.com/repos/{owner}/{repo}/releases")
         response.raise_for_status()
 
         response_json = json.loads(response.content)
         result: DependencyVersion | None = None
 
         if len(response_json) != 0:
-            result = AbstractDependencyManagerPlugIn.parse_as_semantic_version(response_json[0]["name"])
+            result = AbstractDependencyManagerPlugIn.parse_as_semantic_version(response_json[0]["tag_name"])
 
         return result
```

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/ibm_cloud_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/ibm_cloud_pak_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/ibm_cloud_terraform_provider_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/openshift_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/openshift_install_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/openshift/openshift_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/dependency_manager/plugins/terraform_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/dependency_manager/plugins/terraform_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibm_internal_plugin/ibm_internal_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/cluster_status.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/data/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/data/ingress_status.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/data/ingress_status.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/ibm_cloud_api_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/ibm_cloud_api_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/ls.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/ls.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/roks_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/ibmcloud/oc/cluster/roks_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/jmespath.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/jmespath.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/__init__.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/cluster/generic_cluster.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/cluster/generic_cluster_factory.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/cluster/generic_cluster_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/cluster_based_user_credentials.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/cluster_based_user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/credentials.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/token_credentials.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/token_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/credentials/user_credentials.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/credentials/user_credentials.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/data/global_pull_secret_data.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/data/global_pull_secret_data.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/nfs/nfs_subdir_external_provisioner.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/oc.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/oc.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_api_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_api_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/openshift_installation_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/openshift_installation_manager_plugin.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/openshift_install/types/architecture.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/openshift_install/types/architecture.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/auths_dict.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/auths_dict.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/catalog_source.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/catalog_source.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/credentials.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/credentials.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/custom_resource.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/custom_resource_event_result.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/custom_resource_event_result.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/get_pod_entry.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/get_pod_entry.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/kind_metadata.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/kind_metadata.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/object_meta.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/object_meta.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/operator_group.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/operator_group.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/role.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_binding.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/role_binding.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/role_rule.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/role_rule.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/service_account.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/service_account.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/types/subscription.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/types/subscription.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/openshift/utils/click.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/openshift/utils/click.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/package_data.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/plugin_manager/package_data.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/lib/plugin_manager/plugin_manager.py` & `cloud_pak_operations_cli-0.7.3/cpo/lib/plugin_manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/scripts/get_current_cluster_alias.py` & `cloud_pak_operations_cli-0.7.3/cpo/scripts/get_current_cluster_alias.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/compression.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/compression.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/debugger.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/download.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/error.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/error.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/file.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/file.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/http_method.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/http_method.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/importlib.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/importlib.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/logging.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/network.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/network.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/operating_system.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/operating_system.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/process.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/process.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/ssh.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/cpo/utils/wait.py` & `cloud_pak_operations_cli-0.7.3/cpo/utils/wait.py`

 * *Files identical despite different names*

### Comparing `cloud_pak_operations_cli-0.7.2/pyproject.toml` & `cloud_pak_operations_cli-0.7.3/pyproject.toml`

 * *Files identical despite different names*

