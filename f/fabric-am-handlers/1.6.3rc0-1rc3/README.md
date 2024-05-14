# Comparing `tmp/fabric-am-handlers-1.6.3rc0.tar.gz` & `tmp/fabric-am-handlers-1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-am-handlers-1.6.3rc0.tar", last modified: Sat Feb 24 02:49:40 2024, max compression
+gzip compressed data, was "fabric-am-handlers-1rc3.tar", last modified: Thu Jul 22 21:44:39 2021, max compression
```

## Comparing `fabric-am-handlers-1.6.3rc0.tar` & `fabric-am-handlers-1rc3.tar`

### file list

```diff
@@ -1,92 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-07-19 17:49:30.462408 fabric-am-handlers-1.6.3rc0/.gitignore
--rw-r--r--   0        0        0     1071 2023-07-19 17:49:30.462542 fabric-am-handlers-1.6.3rc0/LICENSE
--rw-r--r--   0        0        0     6499 2023-07-19 17:49:30.462700 fabric-am-handlers-1.6.3rc0/README.md
--rw-r--r--   0        0        0       25 2024-02-24 02:49:27.445090 fabric-am-handlers-1.6.3rc0/fabric_am/__init__.py
--rw-r--r--   0        0        0     1512 2024-02-09 16:28:38.767953 fabric-am-handlers-1.6.3rc0/fabric_am/config/al2s_handler_config.yml
--rw-r--r--   0        0        0     1655 2023-07-19 17:49:30.463200 fabric-am-handlers-1.6.3rc0/fabric_am/config/net_handler_config.yml
--rw-r--r--   0        0        0     3173 2024-02-23 23:37:14.762422 fabric-am-handlers-1.6.3rc0/fabric_am/config/vm_handler_config.yml
--rw-r--r--   0        0        0     1448 2023-07-19 17:49:30.463601 fabric-am-handlers-1.6.3rc0/fabric_am/config/vnic_net_handler_config.yml
--rw-r--r--   0        0        0        0 2023-07-19 17:49:30.463694 fabric-am-handlers-1.6.3rc0/fabric_am/handlers/__init__.py
--rw-r--r--   0        0        0    24760 2024-02-19 14:46:08.055282 fabric-am-handlers-1.6.3rc0/fabric_am/handlers/al2s_handler.py
--rw-r--r--   0        0        0    50395 2024-02-13 21:53:38.313415 fabric-am-handlers-1.6.3rc0/fabric_am/handlers/net_handler.py
--rw-r--r--   0        0        0    21027 2023-07-19 17:49:30.464223 fabric-am-handlers-1.6.3rc0/fabric_am/handlers/oess_handler.py
--rw-r--r--   0        0        0    83291 2024-02-24 02:29:02.067271 fabric-am-handlers-1.6.3rc0/fabric_am/handlers/vm_handler.py
--rw-r--r--   0        0        0    13280 2023-07-19 17:49:30.464863 fabric-am-handlers-1.6.3rc0/fabric_am/handlers/vnic_net_handler.py
--rw-r--r--   0        0        0     9114 2023-07-19 17:49:30.465047 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/README.md
--rw-r--r--   0        0        0      289 2024-02-09 16:28:38.774711 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/al2s.yml
--rw-r--r--   0        0        0      754 2024-02-09 16:28:38.775839 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/fpga_provisioning.yml
--rwxr-xr-x   0        0        0      173 2023-07-19 17:49:30.465397 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/head_get_worker_node_for_vm.yml
--rw-r--r--   0        0        0     1293 2023-07-19 17:49:30.465520 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/head_port_provisioning.yml
--rw-r--r--   0        0        0      137 2023-07-19 17:49:30.465619 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/head_vm_post_boot_config.yml
--rw-r--r--   0        0        0     1289 2023-07-19 17:49:30.465735 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/head_vm_provisioning.yml
--rw-r--r--   0        0        0     1297 2023-07-19 17:49:30.465853 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/head_volume_provisioning.yml
--rw-r--r--   0        0        0     1168 2024-02-09 16:28:38.776131 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/inventory_template
--rw-r--r--   0        0        0      162 2024-02-23 22:06:51.941797 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/multi_function_pci_devices.yml
--rw-r--r--   0        0        0     2655 2023-07-19 17:49:30.466159 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/netam_nso_data.yml
--rw-r--r--   0        0        0      139 2023-07-19 17:49:30.466280 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/nmcli_config_nw_interface.yml
--rw-r--r--   0        0        0      108 2023-07-19 17:49:30.466417 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/nvme_cleanup.yml
--rw-r--r--   0        0        0     3631 2023-08-21 14:52:04.073676 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/fpga_provisioning/tasks/main.yml
--rwxr-xr-x   0        0        0      678 2023-07-19 17:49:30.466975 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/head_get_worker_node_for_vm/tasks/main.yml
--rw-r--r--   0        0        0     3063 2023-07-19 17:49:30.467287 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/head_port_provisioning/tasks/main.yml
--rw-r--r--   0        0        0     1925 2023-07-19 17:49:30.467701 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/head_vm_post_boot_config/tasks/main.yml
--rw-r--r--   0        0        0     3545 2023-07-19 17:49:30.468046 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/head_vm_provisioning/tasks/main.yml
--rw-r--r--   0        0        0     2614 2023-07-19 17:49:30.468292 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/head_volume_provisioning/tasks/main.yml
--rw-r--r--   0        0        0     4371 2024-02-24 02:30:14.815773 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/multi_function_pci_devices/tasks/main.yml
--rw-r--r--   0        0        0     4320 2023-07-19 17:49:30.468672 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/nmcli_config_nw_interface/tasks/main.yml
--rw-r--r--   0        0        0      505 2023-07-19 17:49:30.469103 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/nvme_cleanup/tasks/main.yml
--rw-r--r--   0        0        0      484 2023-07-19 17:49:30.469479 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/defaults/secret.yml
--rw-r--r--   0        0        0     1789 2023-07-19 17:49:30.469790 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/tasks/account-info.yml
--rw-r--r--   0        0        0     2310 2023-07-19 17:49:30.470045 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/tasks/create-circuit.yml
--rw-r--r--   0        0        0     2297 2023-07-19 17:49:30.470250 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/tasks/create-vrt.yml
--rw-r--r--   0        0        0     2333 2023-07-19 17:49:30.470380 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/tasks/delete-circuit.yml
--rw-r--r--   0        0        0     2233 2023-07-19 17:49:30.470505 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/tasks/delete-vrt.yml
--rw-r--r--   0        0        0     1734 2023-07-19 17:49:30.470608 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/tasks/main.yml
--rw-r--r--   0        0        0      701 2023-07-19 17:49:30.470781 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/oess_provisioning/vars/main.yml
--rw-r--r--   0        0        0     1629 2024-02-09 16:28:38.776860 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/ssh_keys_config/tasks/main.yml
--rw-r--r--   0        0        0     1703 2023-07-19 17:49:30.471222 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/storage_config/tasks/main.yml
--rw-r--r--   0        0        0     3337 2024-02-09 16:28:38.777908 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/check-l3connection.yml
--rw-r--r--   0        0        0     2831 2024-02-09 16:28:38.778642 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/check-space.yml
--rw-r--r--   0        0        0     2725 2024-02-09 16:28:38.779171 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/create-l3connection.yml
--rw-r--r--   0        0        0     2127 2024-02-09 16:28:38.779406 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/create-router.yml
--rw-r--r--   0        0        0     2205 2024-02-09 16:28:38.779580 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/create-space.yml
--rw-r--r--   0        0        0     1700 2024-02-09 16:28:38.780084 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/create-spaces.yml
--rw-r--r--   0        0        0     2397 2024-02-09 16:28:38.780265 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/create-token.yml
--rw-r--r--   0        0        0     1672 2024-02-09 16:28:38.780393 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/delete-l3connection.yml
--rw-r--r--   0        0        0     2432 2024-02-09 16:28:38.780686 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/delete-router.yml
--rw-r--r--   0        0        0     2796 2024-02-09 16:28:38.780928 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/delete-space.yml
--rw-r--r--   0        0        0     1498 2024-02-09 16:28:38.782309 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/delete-spaces.yml
--rw-r--r--   0        0        0     1619 2024-02-09 16:28:38.782601 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/list-cloudconnects.yml
--rw-r--r--   0        0        0     1617 2024-02-09 16:28:38.782723 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/list-myinterfaces.yml
--rw-r--r--   0        0        0     1592 2024-02-09 16:28:38.782881 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/list-spaces.yml
--rw-r--r--   0        0        0     1632 2024-02-09 16:28:38.783038 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/main.yml
--rw-r--r--   0        0        0     1980 2024-02-09 16:28:38.783404 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/search-interface.yml
--rw-r--r--   0        0        0     2108 2024-02-09 16:28:38.784098 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/tasks/search-space.yml
--rw-r--r--   0        0        0     1725 2024-02-09 16:28:38.784407 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/virtualnetworks_provisioning/vars/main.yml
--rw-r--r--   0        0        0     3204 2024-02-19 14:46:08.057857 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/worker_libvirt_operations/tasks/main.yml
--rwxr-xr-x   0        0        0     1222 2023-07-19 17:49:30.471956 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/worker_pci_provisioning/tasks/main.yml
--rw-r--r--   0        0        0      203 2023-07-19 17:49:30.472202 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/worker_pci_provisioning/templates/device.j2
--rw-r--r--   0        0        0      237 2023-07-19 17:49:30.472315 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/roles/worker_pci_provisioning/templates/device_with_mac.j2
--rw-r--r--   0        0        0      139 2024-02-09 16:28:38.786260 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/ssh_keys_config.yml
--rw-r--r--   0        0        0     1280 2023-07-19 17:49:30.472437 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/storage_config.yml
--rwxr-xr-x   0        0        0      155 2023-07-19 17:49:30.472538 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/worker_libvirt_operations.yml
--rwxr-xr-x   0        0        0      131 2023-07-19 17:49:30.472662 fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/worker_pci_provisioning.yml
--rw-r--r--   0        0        0        0 2023-07-19 17:49:30.472774 fabric-am-handlers-1.6.3rc0/fabric_am/test/__init__.py
--rw-r--r--   0        0        0     1590 2023-07-19 17:49:30.472919 fabric-am-handlers-1.6.3rc0/fabric_am/test/config/vm_handler_config.yml
--rw-r--r--   0        0        0     1289 2023-07-19 17:49:30.473072 fabric-am-handlers-1.6.3rc0/fabric_am/test/playbooks/head_vm_provisioning.yml
--rw-r--r--   0        0        0      416 2023-07-19 17:49:30.474460 fabric-am-handlers-1.6.3rc0/fabric_am/test/playbooks/inventory
--rw-r--r--   0        0        0      139 2023-07-19 17:49:30.474615 fabric-am-handlers-1.6.3rc0/fabric_am/test/playbooks/nmcli_config_nw_interface.yml
--rw-r--r--   0        0        0     1763 2023-07-19 17:49:30.475201 fabric-am-handlers-1.6.3rc0/fabric_am/test/playbooks/roles/head_vm_provisioning/tasks/main.yml
--rw-r--r--   0        0        0     3505 2023-07-19 17:49:30.475424 fabric-am-handlers-1.6.3rc0/fabric_am/test/playbooks/roles/nmcli_config_nw_interface/tasks/main.yml
--rw-r--r--   0        0        0      233 2023-07-19 17:49:30.475618 fabric-am-handlers-1.6.3rc0/fabric_am/test/playbooks/roles/worker_pci_provisioning/tasks/main.yml
--rw-r--r--   0        0        0     1302 2023-07-19 17:49:30.475792 fabric-am-handlers-1.6.3rc0/fabric_am/test/playbooks/worker_pci_provisioning.yml
--rw-r--r--   0        0        0    25111 2024-02-09 16:28:38.786619 fabric-am-handlers-1.6.3rc0/fabric_am/test/test_al2s_handler.py
--rw-r--r--   0        0        0    56127 2023-07-19 17:49:30.476034 fabric-am-handlers-1.6.3rc0/fabric_am/test/test_network_handler.py
--rw-r--r--   0        0        0    10926 2023-07-19 17:49:30.476822 fabric-am-handlers-1.6.3rc0/fabric_am/test/test_vm_handler.py
--rw-r--r--   0        0        0        0 2023-07-19 17:49:30.476983 fabric-am-handlers-1.6.3rc0/fabric_am/util/__init__.py
--rw-r--r--   0        0        0     4274 2024-02-23 22:18:34.673204 fabric-am-handlers-1.6.3rc0/fabric_am/util/am_constants.py
--rw-r--r--   0        0        0    10403 2023-07-19 17:49:30.477298 fabric-am-handlers-1.6.3rc0/fabric_am/util/ansible_helper.py
--rw-r--r--   0        0        0    10509 2023-07-19 17:49:30.477443 fabric-am-handlers-1.6.3rc0/fabric_am/util/utils.py
--rw-r--r--   0        0        0   184473 2023-07-19 17:49:30.478854 fabric-am-handlers-1.6.3rc0/images/handlers.png
--rw-r--r--   0        0        0      860 2024-02-24 02:49:36.576882 fabric-am-handlers-1.6.3rc0/pyproject.toml
--rw-r--r--   0        0        0     9988 2023-07-19 17:49:30.479316 fabric-am-handlers-1.6.3rc0/test_playbooks.py
--rw-r--r--   0        0        0     7199 1970-01-01 00:00:00.000000 fabric-am-handlers-1.6.3rc0/PKG-INFO
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.200279 fabric-am-handlers-1rc3/
+-rw-r--r--   0 komalthareja   (502) staff       (20)     1071 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/LICENSE
+-rw-r--r--   0 komalthareja   (502) staff       (20)      109 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/MANIFEST.in
+-rw-r--r--   0 komalthareja   (502) staff       (20)     7772 2021-07-22 21:44:39.199534 fabric-am-handlers-1rc3/PKG-INFO
+-rw-r--r--   0 komalthareja   (502) staff       (20)     6687 2021-07-21 17:21:56.000000 fabric-am-handlers-1rc3/README.md
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.176865 fabric-am-handlers-1rc3/fabric_am/
+-rw-r--r--   0 komalthareja   (502) staff       (20)       22 2021-07-22 21:43:21.000000 fabric-am-handlers-1rc3/fabric_am/__init__.py
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.178377 fabric-am-handlers-1rc3/fabric_am/config/
+-rw-r--r--   0 komalthareja   (502) staff       (20)     1353 2021-07-22 17:38:58.000000 fabric-am-handlers-1rc3/fabric_am/config/net_handler_config.yml
+-rw-r--r--   0 komalthareja   (502) staff       (20)     1510 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/config/vm_handler_config.yml
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.181670 fabric-am-handlers-1rc3/fabric_am/handlers/
+-rw-r--r--   0 komalthareja   (502) staff       (20)        0 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/handlers/__init__.py
+-rw-r--r--   0 komalthareja   (502) staff       (20)    19975 2021-07-22 17:43:25.000000 fabric-am-handlers-1rc3/fabric_am/handlers/net_handler.py
+-rw-r--r--   0 komalthareja   (502) staff       (20)    24969 2021-07-22 17:43:25.000000 fabric-am-handlers-1rc3/fabric_am/handlers/vm_handler.py
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.187864 fabric-am-handlers-1rc3/fabric_am/playbooks/
+-rw-r--r--   0 komalthareja   (502) staff       (20)     4500 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/playbooks/README.md
+-rwxr-xr-x   0 komalthareja   (502) staff       (20)      173 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/playbooks/head_get_worker_node_for_vm.yml
+-rw-r--r--   0 komalthareja   (502) staff       (20)     1289 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/playbooks/head_vm_provisioning.yml
+-rw-r--r--   0 komalthareja   (502) staff       (20)      921 2021-07-22 17:38:58.000000 fabric-am-handlers-1rc3/fabric_am/playbooks/inventory
+-rw-r--r--   0 komalthareja   (502) staff       (20)     1295 2021-07-22 17:38:58.000000 fabric-am-handlers-1rc3/fabric_am/playbooks/netam_nso_data.yml
+-rwxr-xr-x   0 komalthareja   (502) staff       (20)      131 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/playbooks/worker_pci_provisioning.yml
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.190518 fabric-am-handlers-1rc3/fabric_am/test/
+-rw-r--r--   0 komalthareja   (502) staff       (20)        0 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/test/__init__.py
+-rw-r--r--   0 komalthareja   (502) staff       (20)    21250 2021-07-22 17:43:25.000000 fabric-am-handlers-1rc3/fabric_am/test/test_network_handler.py
+-rw-r--r--   0 komalthareja   (502) staff       (20)    11179 2021-07-22 17:43:25.000000 fabric-am-handlers-1rc3/fabric_am/test/test_vm_handler.py
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.193343 fabric-am-handlers-1rc3/fabric_am/util/
+-rw-r--r--   0 komalthareja   (502) staff       (20)        0 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/util/__init__.py
+-rw-r--r--   0 komalthareja   (502) staff       (20)     2591 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/fabric_am/util/am_constants.py
+-rw-r--r--   0 komalthareja   (502) staff       (20)     8782 2021-07-19 13:50:44.000000 fabric-am-handlers-1rc3/fabric_am/util/ansible_helper.py
+drwxr-xr-x   0 komalthareja   (502) staff       (20)        0 2021-07-22 21:44:39.198168 fabric-am-handlers-1rc3/fabric_am_handlers.egg-info/
+-rw-r--r--   0 komalthareja   (502) staff       (20)     7772 2021-07-22 21:44:38.000000 fabric-am-handlers-1rc3/fabric_am_handlers.egg-info/PKG-INFO
+-rw-r--r--   0 komalthareja   (502) staff       (20)      881 2021-07-22 21:44:38.000000 fabric-am-handlers-1rc3/fabric_am_handlers.egg-info/SOURCES.txt
+-rw-r--r--   0 komalthareja   (502) staff       (20)        1 2021-07-22 21:44:38.000000 fabric-am-handlers-1rc3/fabric_am_handlers.egg-info/dependency_links.txt
+-rw-r--r--   0 komalthareja   (502) staff       (20)       76 2021-07-22 21:44:38.000000 fabric-am-handlers-1rc3/fabric_am_handlers.egg-info/requires.txt
+-rw-r--r--   0 komalthareja   (502) staff       (20)       10 2021-07-22 21:44:38.000000 fabric-am-handlers-1rc3/fabric_am_handlers.egg-info/top_level.txt
+-rw-r--r--   0 komalthareja   (502) staff       (20)       38 2021-07-22 21:44:39.200771 fabric-am-handlers-1rc3/setup.cfg
+-rw-r--r--   0 komalthareja   (502) staff       (20)     1177 2021-07-19 13:48:29.000000 fabric-am-handlers-1rc3/setup.py
```

### Comparing `fabric-am-handlers-1.6.3rc0/LICENSE` & `fabric-am-handlers-1rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-am-handlers-1.6.3rc0/README.md` & `fabric-am-handlers-1rc3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Requirements Status](https://requires.io/github/fabric-testbed/AMHandlers/requirements.svg?branch=main)](https://requires.io/github/fabric-testbed/AMHandlers/requirements/?branch=main)
+
 [![PyPI](https://img.shields.io/pypi/v/fabric-am-handlers?style=plastic)](https://pypi.org/project/fabric-am-handlers/)
 
 # AMHandlers
 ## Aggregate Manager
 An aggregate manager controls access to the substrate components. It controls some set of infrastructure resources in a particular site consisting of a set of servers, storage units, network elements or other components under common ownership and control. AMs inform brokers about available resources by passing to the resource advertisement information models. AMs may be associated with more than one broker and the partitioning of resources between brokers is the decision left to the AM. Oversubscription is possible, depending on the deployment needs.
 FABRIC enables a substrate provider to outsource resource arbitration and calendar scheduling to a broker. By delegating resources to the broker, the AM consents to the broker’s policies, and agrees to try to honor reservations issued by the broker if the user has authorization on the AM. 
 
@@ -56,8 +58,8 @@
 ```
 
 #### What is VEPA?
 In the standard mode the software upgrade to the `VEB` in the hypervisor simply forces each VM frame out to the external switch regardless of destination. This causes no change for destination MAC addresses external to the host, but for destinations within the host (another VM in the same VLAN) it forces that traffic to the upstream switch which forwards it back instead of handling it internally, called a hairpin turn.) It's this hairpin turn that causes the requirement for the upstream switch to have updated firmware, typical STP behavior prevents a switch from forwarding a frame back down the port it was received on. The firmware update allows the negotiation between the physical host and the upstream switch of a VEPA port which then allows this hairpin turn.
 
 VEPA simply forces VM traffic to be handled by an external switch. This allows each VM frame flow to be monitored managed and secured with all of the tools available to the physical switch. This does not provide any type of individual tunnel for the VM, or a configurable switchport but does allow for things like flow statistic gathering, ACL enforcement, etc. Basically we're just pushing the MAC forwarding decision to the physical switch and allowing that switch to perform whatever functions it has available on each transaction. The drawback here is that we are now performing one ingress and egress for each frame that was previously handled internally. This means that there are bandwidth and latency considerations to be made. Functions like Single Root I/O Virtualization (SR/IOV) and Direct Path I/O can alleviate some of the latency issues when implementing this. Like any technology there are typically trade offs that must be weighed. In this case the added control and functionality should outweigh the bandwidth and latency additions.
 
-More details about `VEPA` can be found [here](https://www.ieee802.org/1/files/public/docs2009/new-hudson-vepa_seminar-20090514d.pdf)
+More details about `VEPA` can be found [here](https://www.ieee802.org/1/files/public/docs2009/new-hudson-vepa_seminar-20090514d.pdf)
```

### Comparing `fabric-am-handlers-1.6.3rc0/fabric_am/config/al2s_handler_config.yml` & `fabric-am-handlers-1rc3/fabric_am/config/net_handler_config.yml`

 * *Files 15% similar despite different names*

```diff
@@ -17,21 +17,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
-# Author: Liang Zhang (lzhang9@es.net)
-#
-# NOTE: Set the python executable in your enviroment to {ansible_python_interpreter} 
-#
-ansible:
-  ansible_python_interpreter: /Users/lzhang9/opt/anaconda3/envs/fim-utils/bin/python
+# Author: Xi Yang (xiyang@es.net)
 playbooks:
   location: ../playbooks
   inventory_location: ../playbooks/inventory
-  hostname_suffix:
-  L2PTP: al2s.yml
-  L2Cloud: al2s.yml
-  L3VPN: al2s.yml
-  L3Cloud: al2s.yml
+  hostname_suffix: .fabric-testbed.net
+  L2Bridge: netam_nso_data.yml
+  L2PTP: netam_nso_data.yml
+  L2STS: netam_nso_data.yml
```

### Comparing `fabric-am-handlers-1.6.3rc0/fabric_am/config/vnic_net_handler_config.yml` & `fabric-am-handlers-1rc3/fabric_am/playbooks/head_vm_provisioning.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+---
 # MIT License
 #
 # Copyright (c) 2020 FABRIC Testbed
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -18,16 +19,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-ansible:
-  ansible_python_interpreter: /usr/bin/python3.6
-runtime:
-  network_name_prefix: dataplane
-playbooks:
-  location: /etc/fabric/actor/playbooks
-  inventory_location: /etc/fabric/actor/playbooks/inventory
-  admin_ssh_key: /root/.ssh/id_rsa_nova
-  L2Bridge: head_port_provisioning.yml
+# file: head_vm_provisioning.yml
+
+- hosts:
+    - fabric_head
+
+  gather_facts: no
+
+  vars:
+
+  roles:
+    - head_vm_provisioning
```

### Comparing `fabric-am-handlers-1.6.3rc0/fabric_am/handlers/al2s_handler.py` & `fabric-am-handlers-1rc3/fabric_am/handlers/net_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # MIT License
 #
-# Copyright (c) 2022 FABRIC Testbed
+# Copyright (c) 2020 FABRIC Testbed
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -28,207 +28,129 @@
 import traceback
 from typing import Tuple
 
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.plugins.handlers.config_token import ConfigToken
 from fabric_cf.actor.handlers.handler_base import HandlerBase
 from fim.slivers.capacities_labels import Labels, Capacities
-from fim.slivers.network_service import NetworkServiceSliver, MirrorDirection, NSLayer
+from fim.slivers.network_service import NetworkServiceSliver
 
 from fabric_am.util.am_constants import AmConstants
 from fabric_am.util.ansible_helper import AnsibleHelper
 
 
-class Entity():
-    """This is the base class for the virutal network classes. It provides json serialization methods."""
-
-    @classmethod
-    def from_json(cls, data):
-        jsonObj = json.loads(data)
-        return cls(**jsonObj)
-
-    def to_json(self):
-        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=2)
-
-class L3Connection(Entity):
-    def __init__(
-            self,
-            virtualRouterId: str = None,
-            interfaceId: str = None,
-            remoteName: str = None,
-            notes: str = None,
-            displayPosition: int = 1,
-            encapsulationType: str = None,
-            vlanOuterId: int = 0,
-            vlanInnerId: int = 0,
-            ipv6PrefixLength: int = 0,
-            localIPv6: str = None,
-            remoteIPv6: str = None,
-            ipv4PrefixLength: int = 0,
-            localIPv4: str = None,
-            remoteIPv4: str = None,
-            remoteASN: int = 0,
-            authnType: str = None,
-            authnConfig: dict = None,
-            mtu: int = 9001,
-            bfdEnable: bool = True,
-            gtsmEnable: bool = True,
-            cloudConnectionType: str = None,
-            cloudConnectionConfig: dict = None,
-            maxBandwidth: int = 0,
-            authoringState: str = None
-            ):
-        self.virtualRouterId = virtualRouterId
-        self.interfaceId = interfaceId
-        self.remoteName = remoteName
-        self.notes = notes
-        self.displayPosition = displayPosition
-        self.encapsulationType = encapsulationType
-        self.vlanOuterId = vlanOuterId
-        self.vlanInnerId = vlanInnerId
-        self.ipv6PrefixLength = ipv6PrefixLength
-        self.localIPv6 = localIPv6
-        self.remoteIPv6 = remoteIPv6
-        self.ipv4PrefixLength = ipv4PrefixLength
-        self.localIPv4 = localIPv4
-        self.remoteIPv4 = remoteIPv4
-        self.remoteASN = remoteASN
-        self.authnType = authnType
-        self.authnConfig = authnConfig
-        self.mtu = mtu
-        self.bfdEnable = bfdEnable
-        self.gtsmEnable = gtsmEnable
-        self.cloudConnectionType = cloudConnectionType
-        self.cloudConnectionConfig = cloudConnectionConfig
-        self.maxBandwidth = maxBandwidth
-        self.authoringState = authoringState
-    
-class Al2sHandlerException(Exception):
+class NetHandlerException(Exception):
     """
-    AL2S Handler Exception
+    VM Handler Exception
     """
     pass
 
 
-class Al2sHandler(HandlerBase):
+class NetHandler(HandlerBase):
     """
-    AL2S Handler
+    Network Handler
     """
-
-    def get_ansible_python_interpreter(self) -> str:
-        return self.get_config()[AmConstants.ANSIBLE_SECTION][
-            AmConstants.ANSIBLE_PYTHON_INTERPRETER]
-
     def create(self, unit: ConfigToken) -> Tuple[dict, ConfigToken]:
         """
         Create a Network Service
         :param unit: unit representing an NSO Network Service
         :return: tuple of result status and the unit
         """
         result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_CREATE,
                   Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
                   Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
         sliver = None
-        unit_id = None
-        service_type = None
-        service_data = None
+
         try:
-            # self.get_logger().info(f"Create invoked for unit: {unit}")
+            self.get_logger().info(f"Create invoked for unit: {unit}")
             sliver = unit.get_sliver()
             unit_id = str(unit.get_reservation_id())
             if sliver is None:
-                raise Al2sHandlerException(f"Unit # {unit} has no assigned slivers")
+                raise NetHandlerException(f"Unit # {unit} has no assigned slivers")
 
             unit_properties = unit.get_properties()  # use: TBD
 
             resource_type = str(sliver.get_type())
 
             playbook_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_LOCATION]
             inventory_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_INVENTORY]
 
             playbook = self.get_config()[AmConstants.PLAYBOOK_SECTION][resource_type]
             if playbook is None or inventory_path is None or playbook_path is None:
-                raise Al2sHandlerException(f"Missing config parameters playbook: {playbook} "
+                raise NetHandlerException(f"Missing config parameters playbook: {playbook} "
                                           f"playbook_path: {playbook_path} inventory_path: {inventory_path}")
             playbook_path_full = f"{playbook_path}/{playbook}"
 
             if sliver.get_labels() is None or sliver.get_labels().local_name is None:
                 # truncate service_name length to no greater than 53 (36+1+16)
                 sliver_name = sliver.get_name()[:16] if len(sliver.get_name()) > 16 else sliver.get_name()
                 service_name = f'{sliver_name}-{unit_id}'
             else:
                 service_name = sliver.get_labels().local_name
             service_type = resource_type.lower()
-            if service_type == 'l2ptp':
+            if service_type == 'l2bridge':
+                service_data = self.__l2bridge_create_data(sliver, service_name)
+            elif service_type == 'l2ptp':
                 service_data = self.__l2ptp_create_data(sliver, service_name)
-            elif service_type == 'l3vpn':
-                service_data = self.__l3vpn_create_data(sliver, service_name)
+            elif service_type == 'l2sts':
+                service_data = self.__l2sts_create_data(sliver, service_name)
             else:
-                raise Al2sHandlerException(f'unrecognized network service type "{service_type}"')
-
-            extra_vars = service_data
+                raise NetHandlerException(f'unrecognized network service type "{service_type}"')
+            data = {
+                "tailf-ncs:services": {
+                    f'{service_type}:{service_type}': [service_data]
+                }
+            }
+            extra_vars = {
+                "service_name": service_name,
+                "service_type": service_type,
+                "service_action": "create",
+                "data": data
+            }
             print(json.dumps(extra_vars))
-            
-            ansible_helper = AnsibleHelper(inventory_path=inventory_path, logger=self.get_logger(),
-                                           ansible_python_interpreter=self.get_ansible_python_interpreter())
+            ansible_helper = AnsibleHelper(inventory_path=inventory_path, logger=self.get_logger())
             ansible_helper.set_extra_vars(extra_vars=extra_vars)
             self.get_logger().debug(f"Executing playbook {playbook_path_full} to create Network Service")
             ansible_helper.run_playbook(playbook_path=playbook_path_full)
             ansible_callback = ansible_helper.get_result_callback()
             unreachable = ansible_callback.get_json_result_unreachable()
             if unreachable:
-                raise Al2sHandlerException(f'network service {service_name} was not committed due to connection error')
+                raise NetHandlerException(f'network service {service_name} was not committed due to connection error')
             failed = ansible_callback.get_json_result_failed()
             if failed:
                 ansible_callback.dump_all_failed(logger=self.get_logger())
-                raise Al2sHandlerException(f'network service {service_name} was not committed due to config error')
+                raise NetHandlerException(f'network service {service_name} was not committed due to config error')
             ok = ansible_callback.get_json_result_ok()
             if ok:
                 if not ok['changed']:
                     self.get_logger().info(f'network service {service_name} was committed ok but without change')
 
         except Exception as e:
             # Delete VM in case of failure
             if sliver is not None and unit_id is not None:
-                try:
-                    self.__cleanup(sliver=sliver, raise_exception=True, unit_id=unit_id)
-                except Exception as ex:
-                    self.get_logger().error(ex)
-                finally:
-                    self.get_logger().info(f"Tried to delete VM duo to failure")
-
-            ifs = []
-            if service_type is not None and service_data is not None:
-                if service_type == 'l2ptp':
-                    ifs = [arg['interfaceId'] for arg in service_data['opargs'] if 'interfaceId' in arg]
-                elif service_type == 'l3vpn':
-                    ifs = [arg['interfaceId'] for arg in service_data['opargs'] if 'interfaceId' in arg]
-                else:
-                    ifs = []
-            ext_e = Exception(e, ifs)
-
+                self.__cleanup(sliver=sliver, unit_id=unit_id)
             result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_CREATE,
                       Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_EXCEPTION,
                       Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0,
-                      Constants.PROPERTY_EXCEPTION_MESSAGE: ext_e}
+                      Constants.PROPERTY_EXCEPTION_MESSAGE: e}
             self.get_logger().error(e)
             self.get_logger().error(traceback.format_exc())
         finally:
             self.get_logger().info(f"Create completed")
         return result, unit
 
     def delete(self, unit: ConfigToken) -> Tuple[dict, ConfigToken]:
         result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_DELETE,
                   Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
                   Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
         try:
             self.get_logger().info(f"Delete invoked for unit: {unit}")
             sliver = unit.get_sliver()
             if sliver is None:
-                raise Al2sHandlerException(f"Unit # {unit} has no assigned slivers")
+                raise NetHandlerException(f"Unit # {unit} has no assigned slivers")
 
             unit_id = str(unit.get_reservation_id())
             self.__cleanup(sliver=sliver, raise_exception=True, unit_id=unit_id)
         except Exception as e:
             result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_DELETE,
                       Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_EXCEPTION,
                       Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0,
@@ -236,298 +158,242 @@
             self.get_logger().error(e)
             self.get_logger().error(traceback.format_exc())
         finally:
             self.get_logger().info(f"Delete completed")
         return result, unit
 
     def modify(self, unit: ConfigToken) -> Tuple[dict, ConfigToken]:
-        result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_MODIFY,
-                  Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
-                  Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
-        
-        # Nothing to do at this time
-        return result, unit
+        raise NetHandlerException(f"NetworkServiceSliver modify action is not supported yet...")
 
     def __cleanup(self, *, sliver: NetworkServiceSliver, unit_id: str, raise_exception: bool = False):
         if sliver.get_labels() is None or sliver.get_labels().local_name is None:
             # truncate service_name length to no greater than 53 (36+1+16)
             sliver_name = sliver.get_name()[:16] if len(sliver.get_name()) > 16 else sliver.get_name()
             service_name = f'{sliver_name}-{unit_id}'
         else:
             service_name = sliver.get_labels().local_name
         resource_type = str(sliver.get_type())
         service_type = resource_type.lower()
-        if service_type == 'l2ptp':
-            service_data = self.__l2ptp_delete_data(sliver, service_name)
-        elif service_type == 'l3vpn':
-            service_data = self.__l3vpn_delete_data(sliver, service_name)
-        elif service_type == 'l2cloud':
-            service_data = self.__l2cloud_delete_data(sliver, service_name)
-        elif service_type == 'l3cloud':
-            service_data = self.__l3cloud_delete_data(sliver, service_name)
-            
-        extra_vars = service_data
-        
+        data = {
+            "tailf-ncs:services": {
+                f'{service_type}:{service_type}': [{
+                    "name": f'{service_name}',
+                    "__state": "absent"
+                }]
+            }
+        }
+        extra_vars = {
+            "service_name": service_name,
+            "service_type": service_type,
+            "service_action": "delete",
+            "data": data
+        }
         try:
             playbook_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_LOCATION]
             inventory_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_INVENTORY]
             playbook = self.get_config()[AmConstants.PLAYBOOK_SECTION][resource_type]
             if playbook is None or inventory_path is None or playbook_path is None:
-                raise Al2sHandlerException(f"Missing config parameters playbook: {playbook} "
+                raise NetHandlerException(f"Missing config parameters playbook: {playbook} "
                                           f"playbook_path: {playbook_path} inventory_path: {inventory_path}")
             playbook_path_full = f"{playbook_path}/{playbook}"
-            ansible_helper = AnsibleHelper(inventory_path=inventory_path, logger=self.get_logger(),
-                                           ansible_python_interpreter=self.get_ansible_python_interpreter())
+            ansible_helper = AnsibleHelper(inventory_path=inventory_path, logger=self.get_logger())
             ansible_helper.set_extra_vars(extra_vars=extra_vars)
             self.get_logger().debug(f"Executing playbook {playbook_path_full} to delete Network Service")
             ansible_helper.run_playbook(playbook_path=playbook_path_full)
             ansible_callback = ansible_helper.get_result_callback()
             unreachable = ansible_callback.get_json_result_unreachable()
             if unreachable:
-                raise Al2sHandlerException(f'network service {service_name} was not cleaned up due to connection error')
+                raise NetHandlerException(f'network service {service_name} was not cleaned up due to connection error')
             failed = ansible_callback.get_json_result_failed()
             if failed:
                 ansible_callback.dump_all_failed(logger=self.get_logger())
-                raise Al2sHandlerException(f'network service {service_name} was not cleaned up due to config error')
+                raise NetHandlerException(f'network service {service_name} was not cleaned up due to config error')
             ok = ansible_callback.get_json_result_ok()
             if ok:
                 if not ok['changed']:
                     self.get_logger().info(f'network service {service_name} was cleaned up ok but without change')
 
         except Exception as e:
-            self.get_logger().error(f"Exception occurred in cleanup {unit_id} error: {e}")
+            self.get_logger().error(f"Exception occurred in cleanup {e}")
             self.get_logger().error(traceback.format_exc())
             if raise_exception:
                 raise e
 
-    def __l2ptp_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        if len(sliver.interface_info.interfaces) != 2:
-            raise Al2sHandlerException(
-                f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
+    def __l2bridge_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
+        device_name = None
+        interfaces = []
+        data = {"name": service_name, "interface": interfaces}
         for interface_name in sliver.interface_info.interfaces:
-            endpoint = {}
             interface_sliver = sliver.interface_info.interfaces[interface_name]
             labs: Labels = interface_sliver.get_labels()
             caps: Capacities = interface_sliver.get_capacities()
             if labs.device_name is None:
-                raise Al2sHandlerException(f'l2ptp - interface "{interface_name}" has no "device_name" label')
-            endpoint['node'] = labs.device_name
+                raise NetHandlerException(f'l2bridge - interface "{interface_name}" has no "device_name" label')
+            if device_name is None:
+                device_name = labs.device_name
+                data['device'] = device_name
+            elif device_name != labs.device_name:
+                raise NetHandlerException(
+                    f'l2bridge - has two different device_name "{device_name}" and "{labs.device_name}"')
+            interface = {}
             if labs.local_name is None:
-                raise Al2sHandlerException(f'l2ptp - interface "{interface_name}" has no "local_name" label')
-            if caps is not None and caps.bw is not None:
-                endpoint['bandwidth'] = caps.bw * 1000
-            endpoint['interface'] = labs.local_name
-            endpoint['tag'] = labs.vlan
-            if labs.account_id != None:
-                endpoint['cloud_account_id'] = labs.account_id
-            endpoint_list.append(endpoint)
-
-        data = {"description": service_name, 
-                "op": "create",
-                "level": "L2",
-                "l2_endpoints": endpoint_list}
-        
+                raise NetHandlerException(f'l2bridge - interface "{interface_name}" has no "local_name" label')
+            interface_type_id = re.findall(r'(\w+)(\d.+)', labs.local_name)
+            if not interface_type_id or len(interface_type_id[0]) != 2:
+                raise NetHandlerException(f'l2bridge - interface "{interface_name}" has malformed "local_name" label')
+            interface['type'] = interface_type_id[0][0]
+            interface['id'] = interface_type_id[0][1]
+            if labs.vlan is None:
+                interface['outervlan'] = 0
+            else:
+                interface['outervlan'] = labs.vlan
+            if int(interface['outervlan']) > 0 and labs.inner_vlan is not None:
+                interface['innervlan'] = labs.inner_vlan
+            if caps is not None and caps.bw is not None and caps.bw != 0:
+                interface['bandwidth'] = caps.bw # default unit = gbps
+                if caps.burst_size is not None and caps.burst_size != 0:
+                    interface['burst-size'] = caps.burst_size # default unit = mbytes
+            interfaces.append(interface)
+        if not interfaces:
+            raise NetHandlerException(f'l2bridge - none valid interface is defined in sliver')
         return data
 
-    def __l2ptp_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
+    def __l2ptp_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
+        stp_list = []
         if len(sliver.interface_info.interfaces) != 2:
-            raise Al2sHandlerException(
+            raise NetHandlerException(
                 f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
 
-        data = {"op": "delete",
-                "level": "L2",
-                "description": service_name}
-        
-        return data
-
-    def __l3vpn_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        
-        l3Connections = []
-        
-        for i, interface_name in enumerate(sliver.interface_info.interfaces, start = 1):
-            connection = L3Connection(
-                displayPosition = i,
-                encapsulationType = "DOT1Q",
-                authnType = "MD5",
-                authoringState = "LIVE")
-            
-            interface_sliver = sliver.interface_info.interfaces[interface_name]
-            labs: Labels = interface_sliver.get_labels()
-            peerlabs: Labels = interface_sliver.get_peer_labels()
-            caps: Capacities = interface_sliver.get_capacities()
-            
-            if labs.device_name is None:
-                raise Al2sHandlerException(f'l3vpn - interface "{interface_name}" has no "device_name" label')
-            if labs.local_name is None:
-                raise Al2sHandlerException(f'l3vpn - interface "{interface_name}" has no "local_name" label')
-            
-            if caps is not None and caps.bw is not None:
-                connection.maxBandwidth = caps.bw      # specified in Mbps
-                
-            # connection.device = labs.device_name
-            # connection.interface = labs.local_name
-            connection.interfaceId = labs.device_name + ":" + labs.local_name
-            # connection.interfaceId = "5079eacf-3de6-42ba-a342-832ad8117e6f"
-            
-            connection.remoteName = peerlabs.local_name
-            connection.vlanOuterId = str(labs.vlan)
-            connection.mtu = caps.mtu
-            
-            connection.ipv4PrefixLength = int(labs.ipv4_subnet.split('/')[-1])
-            connection.localIPv4 = labs.ipv4_subnet.split('/')[0]
-            connection.remoteIPv4 = peerlabs.ipv4_subnet.split('/')[0]
-            
-            connection.remoteASN = peerlabs.asn
-            
-            connection.authnConfig = {"md5": peerlabs.bgp_key}
-            
-            if peerlabs.account_id:
-                if peerlabs.local_name == 'AWS':
-                    connection.cloudConnectionType = 'AWS'
-                    connection.cloudConnectionConfig = {"ownerAccountId":peerlabs.account_id}
-                elif peerlabs.local_name == 'Google Cloud Platform':
-                    connection.cloudConnectionType = 'GCP'
-                    connection.cloudConnectionConfig = {"pairingKey":peerlabs.account_id}
-                else:
-                    raise Exception(f"Unimplemented cloud connect: {peerlabs.local_name}")
-            else:
-                connection.cloudConnectionType = 'NONCLOUD'
-                connection.cloudConnectionConfig = {}
-                
-            
-            # connection.entity = str(sliver.get_name())
-            
-            l3Connections.append(vars(connection))
-        
-        data = {"name": service_name,
-                "description": service_name,
-                "op": "create",
-                "level": "L3",
-                "opargs": l3Connections}
-        
-        return data
-
-    def __l3vpn_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise Al2sHandlerException(
-                # f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        data = {"op": "delete",
-                "level": "L3",
-                "name": service_name}
-        
-        return data
-
-    def __l2cloud_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise Al2sHandlerException(
-        #         f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
         for interface_name in sliver.interface_info.interfaces:
-            endpoint = {}
+            stp = {}
             interface_sliver = sliver.interface_info.interfaces[interface_name]
             labs: Labels = interface_sliver.get_labels()
             caps: Capacities = interface_sliver.get_capacities()
             if labs.device_name is None:
-                raise Al2sHandlerException(f'l2ptp - interface "{interface_name}" has no "device_name" label')
-            endpoint['node'] = labs.device_name
+                raise NetHandlerException(f'l2ptp - interface "{interface_name}" has no "device_name" label')
+            stp['device'] = labs.device_name
+            interface = {}
             if labs.local_name is None:
-                raise Al2sHandlerException(f'l2ptp - interface "{interface_name}" has no "local_name" label')
-            if caps is not None and caps.bw is not None:
-                endpoint['bandwidth'] = caps.bw
-            endpoint['interface'] = labs.local_name
-            endpoint['tag'] = labs.vlan
-            endpoint['cloud_account_id'] = labs.account_id
-            endpoint_list.append(endpoint)
-
-        data = {"description": service_name, 
-                "op": "create",
-                "level": "L2",
-                "l2_endpoints": endpoint_list}
-        
-        return data
-
-    def __l2cloud_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise Al2sHandlerException(
-        #         f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        data = {"op": "delete",
-                "level": "L2",
-                "description": service_name}
-        
+                raise NetHandlerException(f'l2ptp - interface "{interface_name}" has no "local_name" label')
+            interface_type_id = re.findall(r'(\w+)(\d.+)', labs.local_name)
+            if not interface_type_id or len(interface_type_id[0]) != 2:
+                raise NetHandlerException(f'l2ptp - interface "{interface_name}" has malformed "local_name" label')
+            interface['type'] = interface_type_id[0][0]
+            interface['id'] = interface_type_id[0][1]
+            if labs.vlan is None or labs.vlan == 0:
+                raise NetHandlerException(f'l2ptp - interface "{interface_name}" must be tagged (with vlan label in 1..4095)')
+            interface['outervlan'] = labs.vlan
+            if labs.inner_vlan is not None:
+                interface['innervlan'] = labs.inner_vlan
+
+            if caps is not None and caps.bw is not None and caps.bw != 0:
+                interface['bandwidth'] = caps.bw
+                if caps.burst_size is not None and caps.burst_size != 0:
+                    interface['burst-size'] = caps.burst_size
+            stp['interface'] = interface
+            stp_list.append(stp)
+
+        if stp_list[0]['device'] == stp_list[1]['device']:
+            raise NetHandlerException(
+                f'l2ptp - has two interfaces on the same device "{stp_list[0]["device"]}" (required to be different)')
+
+        data = {"name": service_name, "stp-a": stp_list[0], "stp-z": stp_list[1]}
+
+        if sliver.ero is not None and len(sliver.ero.get()) == 2:
+            ero_a2z = []
+            type, path = sliver.ero.get()
+            index = 1
+            for hop in path.get()[0]:
+                # TODO: validate hop is ipv4 using regex
+                ero_a2z.append({'index': str(index), 'address': hop})
+                index += 1
+            hop_a2z = {"hop": ero_a2z}
+            data['ero-a2z'] = hop_a2z
+
+            ero_z2a = []
+            index = 1
+            for hop in path.get()[1]:
+                # TODO: validate hop is ipv4 using regex
+                ero_z2a.append({'index': str(index), 'address': hop})
+                index += 1
+            hop_z2a = {"hop": ero_z2a}
+            data['ero-z2a'] = hop_z2a
+        else:
+            self.get_logger().info(f"l2ptp - created without ERO")
         return data
 
-    def __l3cloud_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        local_asn = ''
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise Al2sHandlerException(
-                # f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
+    def __l2sts_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
+        site_a = {}
+        site_z = {}
+        if len(sliver.interface_info.interfaces) < 2:
+            raise NetHandlerException(
+                f'l2sts - sliver requires at least 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
 
         for interface_name in sliver.interface_info.interfaces:
-            endpoint = {}
+            interfaces = {}
             interface_sliver = sliver.interface_info.interfaces[interface_name]
             labs: Labels = interface_sliver.get_labels()
             caps: Capacities = interface_sliver.get_capacities()
             if labs.device_name is None:
-                raise Al2sHandlerException(f'l3cloud - interface "{interface_name}" has no "device_name" label')
-            endpoint['node'] = labs.device_name
+                raise NetHandlerException(f'l2sts - interface "{interface_name}" has no "device_name" label')
+            interface = {}
             if labs.local_name is None:
-                raise Al2sHandlerException(f'l3cloud - interface "{interface_name}" has no "local_name" label')
-            if local_asn and  local_asn != labs.asn:
-                self.get_logger().error(f"local asn is inconsistant in __l3cloud_create_data")
-                raise Al2sHandlerException(f'l3cloud - interface "{interface_name}" has inconsistant local_asn')
-            elif not local_asn:
-                local_asn = labs.asn
-
-            if caps is not None and caps.bw is not None:
-                endpoint['bandwidth'] = caps.bw
-            endpoint['interface'] = labs.local_name
-            endpoint['tag'] = labs.vlan
-            if caps is not None and caps.jumbo is not None:
-                endpoint['jumbo'] = caps.jumbo
-            endpoint['cloud_account_id'] = labs.account_id
-            endpoint['peers'] = {}
-            if interface_name in sliver.get_peer_labels():
-                endpoint['peers']  =  [sliver.get_peer_labels()[interface_name]]
+                raise NetHandlerException(f'l2sts - interface "{interface_name}" has no "local_name" label')
+            interface_type_id = re.findall(r'(\w+)(\d.+)', labs.local_name)
+            if not interface_type_id or len(interface_type_id[0]) != 2:
+                raise NetHandlerException(f'l2sts - interface "{interface_name}" has malformed "local_name" label')
+            interface['type'] = interface_type_id[0][0]
+            interface['id'] = interface_type_id[0][1]
+            if labs.vlan is None:
+                interface['outervlan'] = 0
             else:
-                self.get_logger().error(f"Peers not found in __l3cloud_create_data")
-                raise Al2sHandlerException(f'l3cloud - interface "{interface_name}" has no peers')
-                    
-            endpoint_list.append(endpoint)
-
-        data = {"name": service_name,
-                "description": service_name,
-                "op": "create",
-                "level": "L3",
-                "asn": local_asn,
-                "l3_endpoints": endpoint_list}
-        
-        return data
+                interface['outervlan'] = labs.vlan
+            if int(interface['outervlan']) > 0 and labs.inner_vlan is not None:
+                interface['innervlan'] = labs.inner_vlan
+
+            if caps is not None and caps.bw is not None and caps.bw != 0:
+                interface['bandwidth'] = caps.bw
+                if caps.burst_size is not None and caps.burst_size != 0:
+                    interface['burst-size'] = caps.burst_size
+
+            if not site_a:
+                site_a['device'] = labs.device_name
+                site_a['interface'] = [interface]
+            elif site_a['device'] == labs.device_name:
+                site_a['interface'].append(interface)
+            elif not site_z:
+                site_z['device'] = labs.device_name
+                site_z['interface'] = [interface]
+            elif site_z['device'] == labs.device_name:
+                site_z['interface'].append(interface)
+            else:
+                raise NetHandlerException(
+                    f'l2sts - more than 2 sites are present in the list of interfaces (requires exactly 2)')
 
-    def __l3cloud_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise Al2sHandlerException(
-                # f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        data = {"op": "delete",
-                "level": "L3",
-                "name": service_name}
-        
+        if not site_a or not site_z:
+            raise NetHandlerException(
+                f'l2sts - fewer than 2 sites are present in the list of interfaces (requires exactly 2)')
+
+        data = {"name": service_name, "site-a": site_a, "site-z": site_z}
+
+        if sliver.ero is not None and len(sliver.ero.get()) == 2:
+            ero_a2z = []
+            type, path = sliver.ero.get()
+            index = 1
+            for hop in path.get()[0]:
+                # TODO: validate hop is ipv4 using regex
+                ero_a2z.append({'index': str(index), 'address': hop})
+                index += 1
+            hop_a2z = {"hop": ero_a2z}
+            data['ero-a2z'] = hop_a2z
+
+            ero_z2a = []
+            index = 1
+            for hop in path.get()[1]:
+                # TODO: validate hop is ipv4 using regex
+                ero_z2a.append({'index': str(index), 'address': hop})
+                index += 1
+            hop_z2a = {"hop": ero_z2a}
+            data['ero-z2a'] = hop_z2a
+        else:
+            self.get_logger().info(f"l2ptp - created without ERO")
         return data
-    
-    def clean_restart(self):
-        pass
-
-    def poa(self, unit: ConfigToken, data: dict) -> Tuple[dict, ConfigToken]:
-        """
-        Not implemented
-        """
-        pass
```

### Comparing `fabric-am-handlers-1.6.3rc0/fabric_am/handlers/oess_handler.py` & `fabric-am-handlers-1rc3/fabric_am/test/test_network_handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # MIT License
 #
-# Copyright (c) 2022 FABRIC Testbed
+# Copyright (c) 2020 FABRIC Testbed
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,414 +18,478 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
-# Author: 
-import json
-import re
-import traceback
-from typing import Tuple
+# Author: Ilya Baldin (ibaldin@renci.org), Xi Yang (xiwang@es.net), Komal Thareja (kthare10@renci.org)
+import unittest
+import time
+import uuid
 
 from fabric_cf.actor.core.common.constants import Constants
-from fabric_cf.actor.core.plugins.handlers.config_token import ConfigToken
-from fabric_cf.actor.handlers.handler_base import HandlerBase
-from fim.slivers.capacities_labels import Labels, Capacities
-from fim.slivers.network_service import NetworkServiceSliver, MirrorDirection, NSLayer
+from fabric_cf.actor.core.core.unit import Unit
+from fabric_cf.actor.core.util.id import ID
+from fim.slivers.attached_components import ComponentSliver, ComponentType, AttachedComponentsInfo
+from fim.slivers.capacities_labels import Capacities, Labels, CapacityHints
+from fim.slivers.instance_catalog import InstanceCatalog
+from fim.slivers.network_service import NetworkServiceSliver, ServiceType, NSLayer
+from fim.slivers.interface_info import InterfaceSliver, InterfaceType, InterfaceInfo
+from fim.slivers.path_info import Path, PathInfo, ERO
 
+# FIXME: @xiyang
+from fabric_am.handlers.net_handler import NetHandler
 from fabric_am.util.am_constants import AmConstants
-from fabric_am.util.ansible_helper import AnsibleHelper
-    
-class OessHandlerException(Exception):
-    """
-    OESS Handler Exception
-    """
-    pass
-
-
-class OessHandler(HandlerBase):
-    """
-    OESS Handler
-    """
-
-    def get_ansible_python_interpreter(self) -> str:
-        return self.get_config()[AmConstants.ANSIBLE_SECTION][
-            AmConstants.ANSIBLE_PYTHON_INTERPRETER]
-
-    def create(self, unit: ConfigToken) -> Tuple[dict, ConfigToken]:
-        """
-        Create a Network Service
-        :param unit: unit representing an NSO Network Service
-        :return: tuple of result status and the unit
-        """
-        result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_CREATE,
-                  Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
-                  Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
-        sliver = None
-        unit_id = None
-        try:
-            # self.get_logger().info(f"Create invoked for unit: {unit}")
-            sliver = unit.get_sliver()
-            unit_id = str(unit.get_reservation_id())
-            if sliver is None:
-                raise OessHandlerException(f"Unit # {unit} has no assigned slivers")
-
-            unit_properties = unit.get_properties()  # use: TBD
-
-            resource_type = str(sliver.get_type())
-
-            playbook_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_LOCATION]
-            inventory_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_INVENTORY]
-
-            playbook = self.get_config()[AmConstants.PLAYBOOK_SECTION][resource_type]
-            if playbook is None or inventory_path is None or playbook_path is None:
-                raise OessHandlerException(f"Missing config parameters playbook: {playbook} "
-                                          f"playbook_path: {playbook_path} inventory_path: {inventory_path}")
-            playbook_path_full = f"{playbook_path}/{playbook}"
-
-            if sliver.get_labels() is None or sliver.get_labels().local_name is None:
-                # truncate service_name length to no greater than 53 (36+1+16)
-                sliver_name = sliver.get_name()[:16] if len(sliver.get_name()) > 16 else sliver.get_name()
-                service_name = f'{sliver_name}-{unit_id}'
-            else:
-                service_name = sliver.get_labels().local_name
-            service_type = resource_type.lower()
-            if service_type == 'l2ptp':
-                service_data = self.__l2ptp_create_data(sliver, service_name)
-            elif service_type == 'l3vpn':
-                service_data = self.__l3vpn_create_data(sliver, service_name)
-            else:
-                raise OessHandlerException(f'unrecognized network service type "{service_type}"')
-
-            extra_vars = service_data
-            print(json.dumps(extra_vars))
-            
-            ansible_helper = AnsibleHelper(inventory_path=inventory_path, logger=self.get_logger(),
-                                           ansible_python_interpreter=self.get_ansible_python_interpreter())
-            ansible_helper.set_extra_vars(extra_vars=extra_vars)
-            self.get_logger().debug(f"Executing playbook {playbook_path_full} to create Network Service")
-            ansible_helper.run_playbook(playbook_path=playbook_path_full)
-            ansible_callback = ansible_helper.get_result_callback()
-            unreachable = ansible_callback.get_json_result_unreachable()
-            if unreachable:
-                raise OessHandlerException(f'network service {service_name} was not committed due to connection error')
-            failed = ansible_callback.get_json_result_failed()
-            if failed:
-                ansible_callback.dump_all_failed(logger=self.get_logger())
-                raise OessHandlerException(f'network service {service_name} was not committed due to config error')
-            ok = ansible_callback.get_json_result_ok()
-            if ok:
-                if not ok['changed']:
-                    self.get_logger().info(f'network service {service_name} was committed ok but without change')
-
-        except Exception as e:
-            # Delete VM in case of failure
-            if sliver is not None and unit_id is not None:
-                self.__cleanup(sliver=sliver, unit_id=unit_id)
-            
-            if service_type == 'l2ptp':
-                eps = [(ep['node'], ep['interface']) for ep in service_data['l2_endpoints']]
-            elif service_type == 'l3vpn':
-                eps = [(ep['node'], ep['interface']) for ep in service_data['l3_endpoints']]
-            ext_e = Exception(e, eps)
-                                
-            result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_CREATE,
-                      Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_EXCEPTION,
-                      Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0,
-                      Constants.PROPERTY_EXCEPTION_MESSAGE: ext_e}
-            self.get_logger().error(e)
-            self.get_logger().error(traceback.format_exc())
-        finally:
-            self.get_logger().info(f"Create completed")
-        return result, unit
-
-    def delete(self, unit: ConfigToken) -> Tuple[dict, ConfigToken]:
-        result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_DELETE,
-                  Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
-                  Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
-        try:
-            self.get_logger().info(f"Delete invoked for unit: {unit}")
-            sliver = unit.get_sliver()
-            if sliver is None:
-                raise OessHandlerException(f"Unit # {unit} has no assigned slivers")
-
-            unit_id = str(unit.get_reservation_id())
-            self.__cleanup(sliver=sliver, raise_exception=True, unit_id=unit_id)
-        except Exception as e:
-            result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_DELETE,
-                      Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_EXCEPTION,
-                      Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0,
-                      Constants.PROPERTY_EXCEPTION_MESSAGE: e}
-            self.get_logger().error(e)
-            self.get_logger().error(traceback.format_exc())
-        finally:
-            self.get_logger().info(f"Delete completed")
-        return result, unit
-
-    def modify(self, unit: ConfigToken) -> Tuple[dict, ConfigToken]:
-        raise OessHandlerException(f"OessNetworkServiceSliver modify action is not supported yet...")
-
-    def __cleanup(self, *, sliver: NetworkServiceSliver, unit_id: str, raise_exception: bool = False):
-        if sliver.get_labels() is None or sliver.get_labels().local_name is None:
-            # truncate service_name length to no greater than 53 (36+1+16)
-            sliver_name = sliver.get_name()[:16] if len(sliver.get_name()) > 16 else sliver.get_name()
-            service_name = f'{sliver_name}-{unit_id}'
-        else:
-            service_name = sliver.get_labels().local_name
-        resource_type = str(sliver.get_type())
-        service_type = resource_type.lower()
-        if service_type == 'l2ptp':
-            service_data = self.__l2ptp_delete_data(sliver, service_name)
-        elif service_type == 'l3vpn':
-            service_data = self.__l3vpn_delete_data(sliver, service_name)
-        elif service_type == 'l2cloud':
-            service_data = self.__l2cloud_delete_data(sliver, service_name)
-        elif service_type == 'l3cloud':
-            service_data = self.__l3cloud_delete_data(sliver, service_name)
-            
-        extra_vars = service_data
-        
-        try:
-            playbook_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_LOCATION]
-            inventory_path = self.get_config()[AmConstants.PLAYBOOK_SECTION][AmConstants.PB_INVENTORY]
-            playbook = self.get_config()[AmConstants.PLAYBOOK_SECTION][resource_type]
-            if playbook is None or inventory_path is None or playbook_path is None:
-                raise OessHandlerException(f"Missing config parameters playbook: {playbook} "
-                                          f"playbook_path: {playbook_path} inventory_path: {inventory_path}")
-            playbook_path_full = f"{playbook_path}/{playbook}"
-            ansible_helper = AnsibleHelper(inventory_path=inventory_path, logger=self.get_logger(),
-                                           ansible_python_interpreter=self.get_ansible_python_interpreter())
-            ansible_helper.set_extra_vars(extra_vars=extra_vars)
-            self.get_logger().debug(f"Executing playbook {playbook_path_full} to delete Network Service")
-            ansible_helper.run_playbook(playbook_path=playbook_path_full)
-            ansible_callback = ansible_helper.get_result_callback()
-            unreachable = ansible_callback.get_json_result_unreachable()
-            if unreachable:
-                raise OessHandlerException(f'network service {service_name} was not cleaned up due to connection error')
-            failed = ansible_callback.get_json_result_failed()
-            if failed:
-                ansible_callback.dump_all_failed(logger=self.get_logger())
-                raise OessHandlerException(f'network service {service_name} was not cleaned up due to config error')
-            ok = ansible_callback.get_json_result_ok()
-            if ok:
-                if not ok['changed']:
-                    self.get_logger().info(f'network service {service_name} was cleaned up ok but without change')
-
-        except Exception as e:
-            self.get_logger().error(f"Exception occurred in cleanup {unit_id} error: {e}")
-            self.get_logger().error(traceback.format_exc())
-            if raise_exception:
-                raise e
-
-    def __l2ptp_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        if len(sliver.interface_info.interfaces) != 2:
-            raise OessHandlerException(
-                f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        for interface_name in sliver.interface_info.interfaces:
-            endpoint = {}
-            interface_sliver = sliver.interface_info.interfaces[interface_name]
-            labs: Labels = interface_sliver.get_labels()
-            caps: Capacities = interface_sliver.get_capacities()
-            if labs.device_name is None:
-                raise OessHandlerException(f'l2ptp - interface "{interface_name}" has no "device_name" label')
-            endpoint['node'] = labs.device_name
-            if labs.local_name is None:
-                raise OessHandlerException(f'l2ptp - interface "{interface_name}" has no "local_name" label')
-            if caps is not None and caps.bw is not None:
-                endpoint['bandwidth'] = caps.bw * 1000
-            endpoint['interface'] = labs.local_name
-            endpoint['tag'] = labs.vlan
-            if labs.account_id != None:
-                endpoint['cloud_account_id'] = labs.account_id
-            endpoint_list.append(endpoint)
-
-        data = {"description": service_name, 
-                "op": "create",
-                "level": "L2",
-                "l2_endpoints": endpoint_list}
-        
-        return data
-
-    def __l2ptp_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        if len(sliver.interface_info.interfaces) != 2:
-            raise OessHandlerException(
-                f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        data = {"op": "delete",
-                "level": "L2",
-                "description": service_name}
-        
-        return data
-
-    def __l3vpn_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise OessHandlerException(
-                # f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-        
-        local_asn = sliver.get_labels().asn
-        for interface_name in sliver.interface_info.interfaces:
-            endpoint = {}
-            interface_sliver = sliver.interface_info.interfaces[interface_name]
-            labs: Labels = interface_sliver.get_labels()
-            peerlabs: Labels = interface_sliver.get_peer_labels()
-            caps: Capacities = interface_sliver.get_capacities()
-            if labs.device_name is None:
-                raise OessHandlerException(f'l3vpn - interface "{interface_name}" has no "device_name" label')
-            endpoint['node'] = labs.device_name
-            if labs.local_name is None:
-                raise OessHandlerException(f'l3vpn - interface "{interface_name}" has no "local_name" label')
-            if caps is not None and caps.bw is not None:
-                endpoint['bandwidth'] = caps.bw * 1000      # specified in Mbps
-            endpoint['interface'] = labs.local_name
-            endpoint['tag'] = str(labs.vlan)
-            endpoint['jumbo'] = 1 if caps is not None and caps.mtu is not None and caps.mtu > 9000 else 0
-            endpoint['cloud_account_id'] = peerlabs.account_id
-            endpoint['entity'] = str(sliver.get_name())
-             
-            peering = {}
-            peering['bfd'] = 0
-            peering['ip_version'] = 'ipv4'
-            peering['peer_ip'] = peerlabs.ipv4_subnet
-            peering['peer_asn'] = peerlabs.asn
-            peering['local_ip'] = labs.ipv4_subnet
-            peering['md5_key'] = peerlabs.bgp_key
-            endpoint['peers']  =  [peering]
-                      
-            endpoint_list.append(endpoint)
-
-        data = {"name": service_name,
-                "description": service_name,
-                "op": "create",
-                "level": "L3",
-                "asn": local_asn,
-                "l3_endpoints": endpoint_list}
-        
-        return data
-
-    def __l3vpn_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise OessHandlerException(
-                # f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        data = {"op": "delete",
-                "level": "L3",
-                "name": service_name}
-        
-        return data
-
-    def __l2cloud_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise OessHandlerException(
-        #         f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        for interface_name in sliver.interface_info.interfaces:
-            endpoint = {}
-            interface_sliver = sliver.interface_info.interfaces[interface_name]
-            labs: Labels = interface_sliver.get_labels()
-            caps: Capacities = interface_sliver.get_capacities()
-            if labs.device_name is None:
-                raise OessHandlerException(f'l2ptp - interface "{interface_name}" has no "device_name" label')
-            endpoint['node'] = labs.device_name
-            if labs.local_name is None:
-                raise OessHandlerException(f'l2ptp - interface "{interface_name}" has no "local_name" label')
-            if caps is not None and caps.bw is not None:
-                endpoint['bandwidth'] = caps.bw
-            endpoint['interface'] = labs.local_name
-            endpoint['tag'] = labs.vlan
-            endpoint['cloud_account_id'] = labs.account_id
-            endpoint_list.append(endpoint)
-
-        data = {"description": service_name, 
-                "op": "create",
-                "level": "L2",
-                "l2_endpoints": endpoint_list}
-        
-        return data
-
-    def __l2cloud_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise OessHandlerException(
-        #         f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        data = {"op": "delete",
-                "level": "L2",
-                "description": service_name}
-        
-        return data
-
-    def __l3cloud_create_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        local_asn = ''
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise OessHandlerException(
-                # f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        for interface_name in sliver.interface_info.interfaces:
-            endpoint = {}
-            interface_sliver = sliver.interface_info.interfaces[interface_name]
-            labs: Labels = interface_sliver.get_labels()
-            caps: Capacities = interface_sliver.get_capacities()
-            if labs.device_name is None:
-                raise OessHandlerException(f'l3cloud - interface "{interface_name}" has no "device_name" label')
-            endpoint['node'] = labs.device_name
-            if labs.local_name is None:
-                raise OessHandlerException(f'l3cloud - interface "{interface_name}" has no "local_name" label')
-            if local_asn and  local_asn != labs.asn:
-                self.get_logger().error(f"local asn is inconsistant in __l3cloud_create_data")
-                raise OessHandlerException(f'l3cloud - interface "{interface_name}" has inconsistant local_asn')
-            elif not local_asn:
-                local_asn = labs.asn
-
-            if caps is not None and caps.bw is not None:
-                endpoint['bandwidth'] = caps.bw
-            endpoint['interface'] = labs.local_name
-            endpoint['tag'] = labs.vlan
-            if caps is not None and caps.jumbo is not None:
-                endpoint['jumbo'] = caps.jumbo
-            endpoint['cloud_account_id'] = labs.account_id
-            endpoint['peers'] = {}
-            if interface_name in sliver.get_peer_labels():
-                endpoint['peers']  =  [sliver.get_peer_labels()[interface_name]]
-            else:
-                self.get_logger().error(f"Peers not found in __l3cloud_create_data")
-                raise OessHandlerException(f'l3cloud - interface "{interface_name}" has no peers')
-                    
-            endpoint_list.append(endpoint)
-
-        data = {"name": service_name,
-                "description": service_name,
-                "op": "create",
-                "level": "L3",
-                "asn": local_asn,
-                "l3_endpoints": endpoint_list}
-        
-        return data
-
-    def __l3cloud_delete_data(self, sliver: NetworkServiceSliver, service_name: str) -> dict:
-        endpoint_list = []
-        # if len(sliver.interface_info.interfaces) != 2:
-        #     raise OessHandlerException(
-                # f'l2ptp - sliver requires 2 interfaces but was given {len(sliver.interface_info.interfaces)}')
-
-        data = {"op": "delete",
-                "level": "L3",
-                "name": service_name}
-        
-        return data
-    
-    def clean_restart(self):
-        pass
-
-    def poa(self, unit: ConfigToken, data: dict) -> Tuple[dict, ConfigToken]:
-        """
-        Not implemented
-        """
-        pass
+
+
+class TestNetHandler(unittest.TestCase):
+    log_config = {"log-directory": ".", "log-file": "net_handler.log", "log-level": "DEBUG", "log-retain": 5,
+                  "log-size": 5000000, "logger": __name__}
+
+    def setUp(self) -> None:
+        self.unit = Unit(rid=ID(uid="rid-1"))
+
+    def test_L2Bridge(self):
+        # create a NetworkService sliver for L2Bridge
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: '../config/net_handler_config.yml'}
+
+        handler = NetHandler(log_config=self.log_config, properties=prop)
+        #
+        # create a network sliver for L2Bridge and its interfaces
+        #
+        sliver = NetworkServiceSliver()
+        # service name (set by user) - only guaranteed unique within a slice
+        sliver.set_name('L2BridgeServiceTest')
+        # if service name global uniqueness is a requirement use Labels.local_name for that (optional)
+        # e.g. concatenate name + res id (or another unique id)
+        # sliver.set_labels(Labels().set_fields(local_name='test-l2bridge-shortname'))
+        # per @xiyang he uses unit id for service name so this is not needed.
+        sliver.set_type(ServiceType.L2Bridge)
+        sliver.set_layer(NSLayer.L2)
+
+        # Interface properties
+        #
+        # The service definitions make a distinction between interface which requires
+        # type = parse(InterfaceSliver.Labels.local_name)
+        # id = parse(InterfaceSliver.Labels.local_name)
+        # outervlan = InterfaceSliver.Labels.vlan
+        # innervlan = InterfaceSliver.Labels.inner_vlan
+        # bw = InterfaceSliver.Capacities.bw (0 - best-effort)
+        # burst size = InterfaceSliver.Capacities.burst_size
+        #
+        # and STP which in addition also requires NSO device name.
+        # In deep network sliver NSO Device name goes on *each* interface, then handler.create can parse
+        # out the interfaces and figure out which STP each interface goes with based on that.
+        # NSO device name = InterfaceSliver.Labels.device_name
+        #
+        # The properties of InterfaceSlivers noted above must be copied by Orchestrator from various places
+        # a) the switch TrunkPort port the ASM ServicePort maps to in CBM
+        # b) the Shared or Dedicated ASM port on the card the ServicePort peers with in ASM
+        # c) the Shared or Dedicated CBM port the peer ASM port maps to
+        # Below for each property comments indicate where they come from by a, b, c
+
+        # Orchestrator determines peer ports in ASM (between ServicePort and corresponding Shared/Dedicated card port)
+        # and sets nodemaps to point from ASM ServicePort to corresponding CBM TrunkPort
+        # as well as between Shared/Dedicated ASM port on the NIC and the corresponding CBM Shared/Dedicated port
+
+        #
+        # create a small number of Interface slivers, set their properties and link to service
+        #
+        isl1 = InterfaceSliver()
+        # the name is set by FIM as '-' concatenation of service name
+        isl1.set_name('Interface1')
+        # this will be a ServicePort in the network service sliver. It is created by FIM automatically when
+        # the user adds a NetworkService to the ASM. The name is set by the FIM as '-' concatenation of service
+        # name and peer interface sliver name.
+        isl1.set_type(InterfaceType.ServicePort)
+
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+        # inner_vlan - not used for now - user would fill it in directly on the sliver Labels -
+        # need to discuss.
+        # sl1labs.set_fields(inner_vlan='3')
+
+        # vlan - source: (c)
+        sliver_labels.set_fields(vlan='100')
+
+        # local_name source: (a)
+        sliver_labels.set_fields(local_name='HundredGigE0/0/0/17')
+
+        # NSO device name source: (a) - need to find the owner switch of the network service in CBM
+        # and take its .name or labels.local_name
+        sliver_labels.set_fields(device_name='uky-data-sw')
+
+        # capacities (bw in Gbps, burst size is in Mbytes) source: (b)
+        sliver_capacities.set_fields(bw=1)
+
+        # assign labels and capacities
+        isl1.set_labels(sliver_labels)
+        isl1.set_capacities(sliver_capacities)
+
+        #
+        # Second interface (comments for field info origin omitted below)
+        #
+        isl2 = InterfaceSliver()
+        isl2.set_name('Interface2')
+        isl2.set_type(InterfaceType.ServicePort)
+
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+
+        # sliver_labels.set_fields(vlan='102')
+        sliver_labels.set_fields(local_name='TwentyFiveGigE0/0/0/23/1')
+        sliver_labels.set_fields(device_name='uky-data-sw')
+
+        sliver_capacities.set_fields(bw=1)
+
+        isl2.set_labels(sliver_labels)
+        isl2.set_capacities(sliver_capacities)
+
+        # create interface info object, add populated interfaces to it
+        ifi = InterfaceInfo()
+        ifi.add_interface(isl1)
+        ifi.add_interface(isl2)
+
+        # add interface info object to sliver. All of this happens automagically normally
+        sliver.interface_info = ifi
+        # set a fake unit reservation
+        uid = uuid.uuid3(uuid.NAMESPACE_DNS, 'test_L2Bridge')
+        self.unit = Unit(rid=ID(uid=str(uid)))
+        self.unit.set_sliver(sliver=sliver)
+
+        #
+        # create a service (create needs to parse out sliver information
+        # into exact parameters the service ansible script needs)
+        #
+        r, updated_unit = handler.create(unit=self.unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+
+        time.sleep(30)
+
+        #
+        # delete - need to make sure the updated unit has the right info to delete the service
+        #
+        r, updated_unit = handler.delete(updated_unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+
+    def test_L2Bridge_Hairpin(self):
+        # create a NetworkService sliver for L2Bridge
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: '../config/net_handler_config.yml'}
+
+        handler = NetHandler(log_config=self.log_config, properties=prop)
+        #
+        # create a network sliver for L2Bridge and its interfaces
+        #
+        sliver = NetworkServiceSliver()
+        # service name (set by user) - only guaranteed unique within a slice
+        sliver.set_name('L2-UKY-Hairpin')
+        # if service name global uniqueness is a requirement use Labels.local_name for that (optional)
+        # e.g. concatenate name + res id (or another unique id)
+        # sliver.set_labels(Labels().set_fields(local_name='test-l2bridge-shortname'))
+        # per @xiyang he uses unit id for service name so this is not needed.
+        sliver.set_type(ServiceType.L2Bridge)
+        sliver.set_layer(NSLayer.L2)
+
+        # Interface properties
+        #
+        # The service definitions make a distinction between interface which requires
+        # type = parse(InterfaceSliver.Labels.local_name)
+        # id = parse(InterfaceSliver.Labels.local_name)
+        # outervlan = InterfaceSliver.Labels.vlan
+        # innervlan = InterfaceSliver.Labels.inner_vlan
+        # bw = InterfaceSliver.Capacities.bw (0 - best-effort)
+        # burst size = InterfaceSliver.Capacities.burst_size
+        #
+        # and STP which in addition also requires NSO device name.
+        # In deep network sliver NSO Device name goes on *each* interface, then handler.create can parse
+        # out the interfaces and figure out which STP each interface goes with based on that.
+        # NSO device name = InterfaceSliver.Labels.device_name
+        #
+        # The properties of InterfaceSlivers noted above must be copied by Orchestrator from various places
+        # a) the switch TrunkPort port the ASM ServicePort maps to in CBM
+        # b) the Shared or Dedicated ASM port on the card the ServicePort peers with in ASM
+        # c) the Shared or Dedicated CBM port the peer ASM port maps to
+        # Below for each property comments indicate where they come from by a, b, c
+
+        # Orchestrator determines peer ports in ASM (between ServicePort and corresponding Shared/Dedicated card port)
+        # and sets nodemaps to point from ASM ServicePort to corresponding CBM TrunkPort
+        # as well as between Shared/Dedicated ASM port on the NIC and the corresponding CBM Shared/Dedicated port
+
+        #
+        # create a small number of Interface slivers, set their properties and link to service
+        #
+        isl1 = InterfaceSliver()
+        # the name is set by FIM as '-' concatenation of service name
+        isl1.set_name('Interface1')
+        # this will be a ServicePort in the network service sliver. It is created by FIM automatically when
+        # the user adds a NetworkService to the ASM. The name is set by the FIM as '-' concatenation of service
+        # name and peer interface sliver name.
+        isl1.set_type(InterfaceType.ServicePort)
+
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+        # inner_vlan - not used for now - user would fill it in directly on the sliver Labels -
+        # need to discuss.
+        # sl1labs.set_fields(inner_vlan='3')
+
+        # vlan - source: (c)
+        sliver_labels.set_fields(vlan='101')
+
+        # local_name source: (a)
+        sliver_labels.set_fields(local_name='HundredGigE0/0/0/5')
+
+        # NSO device name source: (a) - need to find the owner switch of the network service in CBM
+        # and take its .name or labels.local_name
+        sliver_labels.set_fields(device_name='uky-data-sw')
+
+        # capacities (bw in Gbps, burst size is in Mbytes) source: (b)
+        sliver_capacities.set_fields(bw=1)
+
+        # assign labels and capacities
+        isl1.set_labels(sliver_labels)
+        isl1.set_capacities(sliver_capacities)
+
+        #
+        # Second interface (comments for field info origin omitted below)
+        #
+        isl2 = InterfaceSliver()
+        isl2.set_name('Interface2')
+        isl2.set_type(InterfaceType.ServicePort)
+
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+
+        sliver_labels.set_fields(vlan='102')
+        sliver_labels.set_fields(inner_vlan='200')
+        sliver_labels.set_fields(local_name='HundredGigE0/0/0/5')
+        sliver_labels.set_fields(device_name='uky-data-sw')
+
+        sliver_capacities.set_fields(bw=1)
+
+        isl2.set_labels(sliver_labels)
+        isl2.set_capacities(sliver_capacities)
+
+        # create interface info object, add populated interfaces to it
+        ifi = InterfaceInfo()
+        ifi.add_interface(isl1)
+        ifi.add_interface(isl2)
+
+        # add interface info object to sliver. All of this happens automagically normally
+        sliver.interface_info = ifi
+        # set a fake unit reservation
+        uid = uuid.uuid3(uuid.NAMESPACE_DNS, 'test_L2Bridge')
+        self.unit = Unit(rid=ID(uid=str(uid)))
+        self.unit.set_sliver(sliver=sliver)
+
+        #
+        # create a service (create needs to parse out sliver information
+        # into exact parameters the service ansible script needs)
+        #
+        r, updated_unit = handler.create(unit=self.unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+
+        time.sleep(30)
+
+        #
+        # delete - need to make sure the updated unit has the right info to delete the service
+        #
+        r, updated_unit = handler.delete(updated_unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+
+
+    def test_L2PTP(self):
+        # create a NetworkService sliver for L2PTP
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: '../config/net_handler_config.yml'}
+
+        handler = NetHandler(log_config=self.log_config, properties=prop)
+
+        #
+        # create a network sliver for L2Bridge and its interfaces
+        #
+        sliver = NetworkServiceSliver()
+        # service name - can we use the sliver name - only guaranteed unique in the slice
+        sliver.set_name('L2PTPServiceTest')
+        sliver.set_type(ServiceType.L2PTP)
+        sliver.set_layer(NSLayer.L2)
+
+        # ERO
+        # first declare a path. Each path is a list of somethings. a2z and z2a maintained separately within Path
+        ero_path = Path()
+
+        ero_path.set_symmetric(["10.1.1.1", "10.1.1.2"])
+        # default is loose ERO, set strict=True if want otherwise
+        ero = ERO(strict=False)
+        ero.set(ero_path)
+        sliver.set_ero(ero)
+
+        #
+        # STP_A interface
+        #
+        stp_a = InterfaceSliver()
+        stp_a.set_name('Interface1')
+        stp_a.set_type(InterfaceType.ServicePort)
+
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+
+        sliver_labels.set_fields(vlan='235')
+        sliver_labels.set_fields(local_name='HundredGigE0/0/0/17')
+        sliver_labels.set_fields(device_name='renc-data-sw')
+
+        sliver_capacities.set_fields(bw=1000)
+
+        stp_a.set_labels(sliver_labels)
+        stp_a.set_capacities(sliver_capacities)
+
+        #
+        # STP_Z interface
+        #
+        stp_z = InterfaceSliver()
+        stp_z.set_name('Interface2')
+        stp_z.set_type(InterfaceType.ServicePort)
+
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+
+        sliver_labels.set_fields(vlan='235')
+        sliver_labels.set_fields(local_name='HundredGigE0/0/0/13')
+        sliver_labels.set_fields(device_name='uky-data-sw')
+
+        sliver_capacities.set_fields(bw=1000)
+
+        stp_z.set_labels(sliver_labels)
+        stp_z.set_capacities(sliver_capacities)
+
+        # create interface info object, add interfaces to it
+        ifi = InterfaceInfo()
+        ifi.add_interface(stp_a)
+        ifi.add_interface(stp_z)
+
+        # All of this happens automagically in FIM
+        sliver.interface_info = ifi
+        uid = uuid.uuid3(uuid.NAMESPACE_DNS, 'test_L2PTP')
+        self.unit = Unit(rid=ID(uid=str(uid)))
+        self.unit.set_sliver(sliver=sliver)
+
+        #
+        # create a service
+        #
+        r, updated_unit = handler.create(unit=self.unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+
+        time.sleep(30)
+
+        #
+        # delete - need to make sure the updated unit has the right info to delete the service
+        #
+        r, updated_unit = handler.delete(updated_unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+
+    def test_L2STS(self):
+        # create a NetworkService sliver for L2STS
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: '../config/net_handler_config.yml'}
+
+        handler = NetHandler(log_config=self.log_config, properties=prop)
+
+        #
+        # create a network sliver for L2Bridge and its interfaces
+        #
+        sliver = NetworkServiceSliver()
+        # service name - can we use the sliver name - only guaranteed unique in the slice
+        sliver.set_name('L2STSServiceTest')
+        sliver.set_type(ServiceType.L2STS)
+        sliver.set_layer(NSLayer.L2)
+
+        # ERO
+        # first declare a path. Each path is a list of somethings. a2z and z2a maintained separately within Path
+        ero_path = Path()
+
+        ero_path.set_symmetric(["10.1.1.1", "10.1.1.2"])
+        # default is loose ERO, set strict=True if want otherwise
+        ero = ERO(strict=False)
+        ero.set(ero_path)
+        sliver.set_ero(ero)
+
+        #
+        # site A interfaces
+        #
+        stp_a1 = InterfaceSliver()
+        stp_a1.set_name('Interface_A1')
+        stp_a1.set_type(InterfaceType.ServicePort)
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+        # untagged w/o vlan label set
+        sliver_labels.set_fields(local_name='TwentyFiveGigE0/0/0/23/1')
+        sliver_labels.set_fields(device_name='lbnl-data-sw')
+        sliver_capacities.set_fields(bw=2000)
+        stp_a1.set_labels(sliver_labels)
+        stp_a1.set_capacities(sliver_capacities)
+
+        #
+        # site Z interfaces
+        #
+        stp_z1 = InterfaceSliver()
+        stp_z1.set_name('Interface_Z1')
+        stp_z1.set_type(InterfaceType.ServicePort)
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+        sliver_labels.set_fields(vlan='235')
+        sliver_labels.set_fields(local_name='HundredGigE0/0/0/13')
+        sliver_labels.set_fields(device_name='uky-data-sw')
+        sliver_capacities.set_fields(bw=1000)
+        stp_z1.set_labels(sliver_labels)
+        stp_z1.set_capacities(sliver_capacities)
+
+        stp_z2 = InterfaceSliver()
+        stp_z2.set_name('Interface_Z2')
+        stp_z2.set_type(InterfaceType.ServicePort)
+        sliver_labels = Labels()
+        sliver_capacities = Capacities()
+        # untagged w/o vlan label set
+        sliver_labels.set_fields(local_name='TwentyFiveGigE0/0/0/23/2')
+        sliver_labels.set_fields(device_name='uky-data-sw')
+        sliver_capacities.set_fields(bw=1000)
+        stp_z2.set_labels(sliver_labels)
+        stp_z2.set_capacities(sliver_capacities)
+
+        # create interface info object, add interfaces to it
+        ifi = InterfaceInfo()
+        ifi.add_interface(stp_a1)
+        ifi.add_interface(stp_z1)
+        ifi.add_interface(stp_z2)
+
+        # All of this happens automagically in FIM
+        sliver.interface_info = ifi
+        uid = uuid.uuid3(uuid.NAMESPACE_DNS, 'test_L2STS')
+        self.unit = Unit(rid=ID(uid=str(uid)))
+        self.unit.set_sliver(sliver=sliver)
+
+        #
+        # create a service
+        #
+        r, updated_unit = handler.create(unit=self.unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+
+        time.sleep(30)
+
+        #
+        # delete - need to make sure the updated unit has the right info to delete the service
+        #
+        r, updated_unit = handler.delete(updated_unit)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
```

### Comparing `fabric-am-handlers-1.6.3rc0/fabric_am/playbooks/head_vm_provisioning.yml` & `fabric-am-handlers-1rc3/fabric_am/config/vm_handler_config.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
----
 # MIT License
 #
 # Copyright (c) 2020 FABRIC Testbed
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -19,18 +18,17 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-# file: head_vm_provisioning.yml
-
-- hosts:
-    - fabric_head
-
-  gather_facts: no
-
-  vars:
-
-  roles:
-    - head_vm_provisioning
+playbooks:
+  location: fabric_am/playbooks
+  inventory_location: fabric_am/playbooks/inventory
+  hostname_suffix: .fabric-testbed.net
+  VM: head_vm_provisioning.yml
+  GPU: worker_pci_provisioning.yml
+  SmartNIC: worker_pci_provisioning.yml
+  SharedNIC: worker_pci_provisioning.yml
+  FPGA: worker_pci_provisioning.yml
+  NVME: worker_pci_provisioning.yml
```

### Comparing `fabric-am-handlers-1.6.3rc0/fabric_am/test/test_vm_handler.py` & `fabric-am-handlers-1rc3/fabric_am/test/test_vm_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,53 +19,41 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-import logging
 import unittest
 
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.core.unit import Unit
 from fabric_cf.actor.core.util.id import ID
 from fim.slivers.attached_components import ComponentSliver, ComponentType, AttachedComponentsInfo
 from fim.slivers.capacities_labels import Capacities, Labels, CapacityHints
 from fim.slivers.instance_catalog import InstanceCatalog
-from fim.slivers.interface_info import InterfaceInfo, InterfaceSliver
 from fim.slivers.network_node import NodeSliver, NodeType
-from fim.slivers.network_service import NetworkServiceInfo, NetworkServiceSliver
-from fim.user.network_service import NetworkService
 
 from fabric_am.handlers.vm_handler import VMHandler
 from fabric_am.util.am_constants import AmConstants
 
 
 class TestVmHandler(unittest.TestCase):
-    logger = logging.getLogger(__name__)
-    log_format = \
-        '%(asctime)s - %(name)s - {%(filename)s:%(lineno)d} - [%(threadName)s] - %(levelname)s - %(message)s'
-    logging.basicConfig(handlers=[logging.StreamHandler()], format=log_format, force=True)
-
-    prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
-    handler = VMHandler(logger=logger, properties=prop)
-    handler.test_mode = True
-
+    log_config = {"log-directory": ".", "log-file": "handler.log", "log-level": "DEBUG", "log-retain": 5,
+                  "log-size": 5000000, "logger": __name__}
 
     @staticmethod
     def create_unit(include_pci: bool = True, include_image: bool = True, include_name: bool = True,
-                    include_instance_name: bool = False, include_ns: bool = False) -> Unit:
+                    include_instance_name: bool = False) -> Unit:
         """
         Create a unit
         :param include_pci:
         :param include_image:
         :param include_name:
         :param include_instance_name:
-        :param include_ns:
         :return:
         """
         u = Unit(rid=ID(uid="rid-1"))
         sliver = NodeSliver()
         cap = Capacities()
         cap.set_fields(core=4, ram=64, disk=500)
         catalog = InstanceCatalog()
@@ -81,111 +69,86 @@
 
         if include_image:
             sliver.set_properties(image_type='qcow2', image_ref='default_centos_8')
 
         if include_pci:
             component = ComponentSliver()
             labels = Labels()
-            labels.set_fields(bdf=["0000:41:00.0", "0000:41:00.1"])
+            labels.set_fields(bdf="0000:81:00.0")
             component.set_properties(type=ComponentType.SmartNIC, model='ConnectX-6', name='nic1',
                                      label_allocations=labels)
             sliver.attached_components_info = AttachedComponentsInfo()
             sliver.attached_components_info.add_device(device_info=component)
 
         if include_instance_name:
             sliver.label_allocations.set_fields(instance="instance-001")
 
-        if include_ns:
-            sliver.network_service_info = NetworkServiceInfo()
-            ns = NetworkServiceSliver()
-            ns.interface_info = InterfaceInfo()
-            ifs1 = InterfaceSliver()
-            c = Capacities()
-            c.bw = 100
-            c.unit = 1
-            l1 = Labels()
-            l1.ipv4 = '192.168.11.3'
-            l1.vlan = '200'
-            l1.local_name = 'p1'
-            la_1 = Labels()
-            la_1.mac = '0C:42:A1:EA:C7:51'
-            la_1.vlan = '200'
-            ifs1.capacities = c
-            ifs1.labels = l1
-            ifs1.label_allocations = la_1
-
-
-            ifs2 = InterfaceSliver()
-            ifs2.capacities = c
-            l2 = Labels()
-            l2.ipv4 = '192.168.11.2'
-            l2.local_name = 'p2'
-            la_2 = Labels()
-            la_2.mac = '0C:42:A1:EA:C7:52'
-
-            ifs2.labels = l2
-            ifs2.label_allocations = la_1
-
-            ns.interface_info.interfaces = {'ifs1': ifs1, 'ifs2': ifs2}
-            sliver.network_service_info.network_services = {'ns1': ns}
-
         u.set_sliver(sliver=sliver)
         return u
 
     def test_create_vm_success(self):
         """
         Test successful creation of VM with PCI devices
         :return:
         """
         u = self.create_unit()
 
-        r, u = self.handler.create(unit=u)
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.create(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
         self.assertIsNotNone(u.sliver.label_allocations.instance)
         self.assertIsNotNone(u.sliver.management_ip)
 
     def test_create_vm_success_no_pci(self):
         """
         Test successful creation of VM without PCI devices
         :return:
         """
         u = self.create_unit(include_pci=False)
 
-        r, u = self.handler.create(unit=u)
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.create(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
         self.assertIsNotNone(u.sliver.label_allocations.instance)
         self.assertIsNotNone(u.sliver.management_ip)
 
     def test_create_vm_fail_no_image(self):
         """
         Test failure to create VM when no image is specified
         :return:
         """
         u = self.create_unit(include_image=False)
 
-        r, u = self.handler.create(unit=u)
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.create(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_EXCEPTION)
         self.assertIsNone(u.sliver.label_allocations.instance)
         self.assertIsNone(u.sliver.management_ip)
 
     def test_create_vm_fail_no_config(self):
         """
         Test failure to create VM when no handler config is specified
         :return:
         """
         u = self.create_unit()
 
         prop = {}
-        handler = VMHandler(logger=self.logger, properties=prop)
+        handler = VMHandler(log_config=self.log_config, properties=prop)
 
         r, u = handler.create(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_EXCEPTION)
         self.assertIsNone(u.sliver.label_allocations.instance)
         self.assertIsNone(u.sliver.management_ip)
@@ -193,72 +156,105 @@
     def test_delete_vm_success(self):
         """
         Test successful deletion of a VM
         :return:
         """
         u = self.create_unit(include_instance_name=True, include_name=True)
 
-        r, u = self.handler.delete(unit=u)
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.delete(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
 
     def test_delete_vm_success_no_pci(self):
         """
         Test successful deletion of a VM without PCI devices
         :return:
         """
         u = self.create_unit(include_pci=False)
 
-        r, u = self.handler.delete(unit=u)
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.delete(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
 
     def test_delete_vm_fail_no_config(self):
         """
         Test failure to delete VM when no handler config is specified
         :return:
         """
         u = self.create_unit()
 
         prop = {}
-        handler = VMHandler(logger=self.logger, properties=prop)
+        handler = VMHandler(log_config=self.log_config, properties=prop)
 
         r, u = handler.delete(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_EXCEPTION)
 
     def test_delete_vm_fail_no_vm_name(self):
         """
         Test failure to delete VM when no VM Name is specified
         :return:
         """
         u = self.create_unit(include_name=False)
 
-        r, u = self.handler.delete(unit=u)
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.delete(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_DELETE)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_EXCEPTION)
 
-    def test_modify_vm_success(self):
+    def test_modify_fail_no_instance_name(self):
         """
-        Test successfully modify VM
+        Test failure to modify VM when no instance name is specified
         :return:
         """
-        u = self.create_unit(include_instance_name=True)
+        u = self.create_unit()
+
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
 
-        r, u = self.handler.modify(unit=u)
+        r, u = handler.modify(unit=u)
         self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_MODIFY)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
-        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_EXCEPTION)
 
-    def test_create_vm_with_nic_config(self):
-        u = self.create_unit(include_ns=True)
+    def test_modify_vm_fail_no_config(self):
+        """
+        Test failure to modify VM when no handler config is specified
+        :return:
+        """
+        u = self.create_unit()
 
-        r, u = self.handler.create(unit=u)
-        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_CREATE)
+        prop = {}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.modify(unit=u)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_MODIFY)
+        self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_EXCEPTION)
+        self.assertIsNotNone(r[Constants.PROPERTY_EXCEPTION_MESSAGE])
+
+    def test_modify_vm_success(self):
+        """
+        Test successfully modify VM
+        :return:
+        """
+        u = self.create_unit(include_instance_name=True)
+
+        prop = {AmConstants.CONFIG_PROPERTIES_FILE: 'config/vm_handler_config.yml'}
+        handler = VMHandler(log_config=self.log_config, properties=prop)
+
+        r, u = handler.modify(unit=u)
+        self.assertEqual(r[Constants.PROPERTY_TARGET_NAME], Constants.TARGET_MODIFY)
         self.assertEqual(r[Constants.PROPERTY_ACTION_SEQUENCE_NUMBER], 0)
         self.assertEqual(r[Constants.PROPERTY_TARGET_RESULT_CODE], Constants.RESULT_CODE_OK)
-        self.assertIsNotNone(u.sliver.label_allocations.instance)
-        self.assertIsNotNone(u.sliver.management_ip)
```

### Comparing `fabric-am-handlers-1.6.3rc0/fabric_am/util/ansible_helper.py` & `fabric-am-handlers-1rc3/fabric_am/util/ansible_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 # Create a callback plugin so we can capture the output
 import os
 import traceback
-from typing import Tuple, List
+from typing import Tuple
 
 from ansible import context
 from ansible.executor.playbook_executor import PlaybookExecutor
 from ansible.inventory.manager import InventoryManager
 from ansible.module_utils.common.collections import ImmutableDict
 from ansible.parsing.dataloader import DataLoader
 from ansible.plugins.callback import CallbackBase
@@ -125,17 +125,15 @@
     def is_failed_or_unreachable(self) -> Tuple[bool, str]:
         status = False
         msg = None
         if len(self.host_failed) > 0 or len(self.host_unreachable) > 0:
             status = True
             result = self.get_json_result_failed()
             if result is not None:
-                msg = result.get('json')
-                if msg is None:
-                    msg = result.get('msg', None)
+                msg = result.get('msg', None)
             else:
                 result = self.get_json_result_unreachable()
                 if result is not None:
                     msg = result.get('msg', None)
 
         return status, msg
 
@@ -154,71 +152,49 @@
         self.dump_all(host_result_map=self.host_unreachable, logger=logger)
 
 
 class AnsibleHelper:
     """
     Helper class to invoke the Ansible Playbook
     """
-    def __init__(self, inventory_path: str, logger, sources: str = None, ansible_python_interpreter: str = None):
+    def __init__(self, inventory_path: str, logger):
         self.results_callback = ResultsCollectorJSONCallback()
         self.loader = DataLoader()
-        if sources is None:
-            self.inventory = InventoryManager(loader=self.loader, sources=[inventory_path])
-        else:
-            self.inventory = InventoryManager(loader=self.loader, sources=sources)
+        self.inventory = InventoryManager(loader=self.loader, sources=[inventory_path])
         self.variable_manager = VariableManager(loader=self.loader, inventory=self.inventory)
         self.logger = logger
-        self.ansible_python_interpreter = ansible_python_interpreter
 
     def add_vars(self, host: str, var_name: str, value: str):
         """
         Set environment variables needed by the playbook
         @param host host
         @param var_name variable name
         @param value value
         """
         self.variable_manager.set_host_variable(host=host, varname=var_name, value=value)
 
-    def run_playbook(self, playbook_path: str, private_key_file: str = None, user: str = None):
+    def run_playbook(self, playbook_path: str):
         """
         Run a playbook
         @param playbook_path path for the playbook
-        @param private_key_file SSH private key file
-        @param user Username
         @raises Exception in case of failure
         """
         if not os.path.exists(playbook_path):
             raise PlaybookException("Playbook not found")
 
-        if user is not None:
-            context.CLIARGS = ImmutableDict(connection='smart', tags={}, listtags=False, listtasks=False,
-                                            listhosts=False,
-                                            syntax=False,
-                                            module_path=None, forks=100, private_key_file=private_key_file,
-                                            ssh_common_args=None, ssh_extra_args='-o StrictHostKeyChecking=no',
-                                            sftp_extra_args=None, timeout = 60,
-                                            scp_extra_args=None, become=False,
-                                            become_method='sudo', become_user='root', verbosity=True, check=False,
-                                            start_at_task=None, user=user)
-        else:
-            context.CLIARGS = ImmutableDict(connection='smart', tags={}, listtags=False, listtasks=False,
-                                            listhosts=False,
-                                            syntax=False,
-                                            module_path=None, forks=100, private_key_file=private_key_file,
-                                            ssh_common_args=None, ssh_extra_args='-o StrictHostKeyChecking=no',
-                                            sftp_extra_args=None, timeout = 60,
-                                            scp_extra_args=None, become=False,
-                                            become_method='sudo', become_user='root', verbosity=True, check=False,
-                                            start_at_task=None)
-
+        context.CLIARGS = ImmutableDict(connection='smart', tags={}, listtags=False, listtasks=False, listhosts=False,
+                                        syntax=False,
+                                        module_path=None, forks=100, private_key_file=None,
+                                        ssh_common_args=None, ssh_extra_args='-o StrictHostKeyChecking=no',
+                                        sftp_extra_args=None,
+                                        scp_extra_args=None, become=False,
+                                        become_method='sudo', become_user='root', verbosity=True, check=False,
+                                        start_at_task=None)
         passwords = {}
 
-        if self.ansible_python_interpreter is not None and self.ansible_python_interpreter != '':
-            self.variable_manager._extra_vars['ansible_python_interpreter'] = self.ansible_python_interpreter
-
         pbex = PlaybookExecutor(playbooks=[playbook_path], inventory=self.inventory,
                                 variable_manager=self.variable_manager,
                                 loader=self.loader, passwords=passwords)
 
         pbex._tqm._stdout_callback = self.results_callback
         try:
             results = pbex.run()
```

### Comparing `fabric-am-handlers-1.6.3rc0/PKG-INFO` & `fabric-am-handlers-1rc3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 Metadata-Version: 2.1
 Name: fabric-am-handlers
-Version: 1.6.3rc0
+Version: 1rc3
 Summary: Fabric Aggregate Manager Handlers
+Home-page: https://github.com/fabric-testbed/AMHandlers
+Author: Komal Thareja, Mauricio Tavares
+Author-email: kthare10@renci.org, mtavares@renci.org
+License: UNKNOWN
+Description: [![Requirements Status](https://requires.io/github/fabric-testbed/AMHandlers/requirements.svg?branch=main)](https://requires.io/github/fabric-testbed/AMHandlers/requirements/?branch=main)
+        
+        [![PyPI](https://img.shields.io/pypi/v/fabric-am-handlers?style=plastic)](https://pypi.org/project/fabric-am-handlers/)
+        
+        # AMHandlers
+        ## Aggregate Manager
+        An aggregate manager controls access to the substrate components. It controls some set of infrastructure resources in a particular site consisting of a set of servers, storage units, network elements or other components under common ownership and control. AMs inform brokers about available resources by passing to the resource advertisement information models. AMs may be associated with more than one broker and the partitioning of resources between brokers is the decision left to the AM. Oversubscription is possible, depending on the deployment needs.
+        FABRIC enables a substrate provider to outsource resource arbitration and calendar scheduling to a broker. By delegating resources to the broker, the AM consents to the broker’s policies, and agrees to try to honor reservations issued by the broker if the user has authorization on the AM. 
+        
+        Besides, common code each AM type has resource-specific modules that determine its resource allocation behavior (Resource Management Policy) and the specific actions it takes to provision a sliver (Resource Handler). Both plugins are invoked by AM common core code based on the resource type or type of request being considered. 
+        
+        ## Handlers
+        The AM up calls a handler interface to setup and teardown each sliver. Resource handlers perform any substrate-specific configuration actions needed to implement slivers. The handler interface includes a probe method to poll the current status of a sliver, and modify to adjust attributes of a sliver. 
+        
+        Handlers are registered and selected by resource type. Each handler invocation executes in an independent thread, so handlers may block for slow configuration actions. Handlers are invoked through a class called HandlerProcessor, which can invoke an interpreter for a handler scripting language. The handlers will be written in the Python scripting language. 
+        
+        Each handler implements 3 basic operation types for a resource:
+        - Create - provision a resource
+          - Example - create a VM or a bare-metal node, or a network connection
+        - Delete - un-provision a resource
+          - Undo the create above
+        - Modify - modify the state of a resource
+          - Modify a property of the VM, or a network connection (e.g. change bandwidth)
+          
+        Each operation can have subcommands and parameters that determine the details of the actions taken, some of which are discussed below. These parameters help ‘stitch’ multiple slivers together. A canonical example is the passing of network information from the handler provisioning the network to the handler provisioning a compute node so that the compute node ends up with correct network configuration (e.g. attached to a correct VLAN). Specific parameters for operations are a matter of convention between the resource management policy and the plugin. 
+        
+        Handlers receive the parameters as part of the provisioning workflow (sequence of redeem operations) executed by the Orchestrator on the AMs. They can also pass information back to the Orchestrator about reserved resources as part of the standard exchange of messages between AM and Orchestrator during the provisioning.
+        
+        ## Playbooks
+        Handlers use Ansible Playbooks for provisioning.  
+        
+        ## Interface and design
+        ![Class Diagram](./images/handlers.png)
+        
+        ## Configuration
+        AM Handlers require following configuration to be setup:
+        - [Inventory](./fabric_am/playbooks/inventory) information for the headnode 
+        - Handler config file (VM Handler example depicted below)
+        ### VM Handler Config File
+        VM Handler config file can be found `fabric_am/config/vm_handler_config.yml`. 
+        It describes the Playbook location and names for specific operations. 
+        ```
+        playbooks:
+          location: /etc/fabric/actor/playbooks
+          inventory_location: /etc/fabric/actor/playbooks/inventory
+          VM: head_vm_provisioning.yml
+          GPU: worker_pci_provisioning.yml
+          SmartNIC: worker_pci_provisioning.yml
+          SharedNIC: worker_pci_provisioning.yml
+          FPGA: worker_pci_provisioning.yml
+          NVME: worker_pci_provisioning.yml
+        ```
+        
+        ### PCI Devices support
+        PCI devices are passed to the VMs using PCI pass through. FABRIC also support `SRIOV` functions which are also passed on to the VMs using PCI pass through. In order to handle the hairpin connections on `SRIOV`, `VEPA` mode is enabled on the underlying bridge for the dedicated card used to host the virtual functions.
+        ```
+        [kissel@uky-w1 ~]$ sudo bridge link set dev ens6f1 hwmode vepa
+        ```
+        
+        #### What is VEPA?
+        In the standard mode the software upgrade to the `VEB` in the hypervisor simply forces each VM frame out to the external switch regardless of destination. This causes no change for destination MAC addresses external to the host, but for destinations within the host (another VM in the same VLAN) it forces that traffic to the upstream switch which forwards it back instead of handling it internally, called a hairpin turn.) It's this hairpin turn that causes the requirement for the upstream switch to have updated firmware, typical STP behavior prevents a switch from forwarding a frame back down the port it was received on. The firmware update allows the negotiation between the physical host and the upstream switch of a VEPA port which then allows this hairpin turn.
+        
+        VEPA simply forces VM traffic to be handled by an external switch. This allows each VM frame flow to be monitored managed and secured with all of the tools available to the physical switch. This does not provide any type of individual tunnel for the VM, or a configurable switchport but does allow for things like flow statistic gathering, ACL enforcement, etc. Basically we're just pushing the MAC forwarding decision to the physical switch and allowing that switch to perform whatever functions it has available on each transaction. The drawback here is that we are now performing one ingress and egress for each frame that was previously handled internally. This means that there are bandwidth and latency considerations to be made. Functions like Single Root I/O Virtualization (SR/IOV) and Direct Path I/O can alleviate some of the latency issues when implementing this. Like any technology there are typically trade offs that must be weighed. In this case the added control and functionality should outweigh the bandwidth and latency additions.
+        
+        More details about `VEPA` can be found [here](https://www.ieee802.org/1/files/public/docs2009/new-hudson-vepa_seminar-20090514d.pdf)
 Keywords: Fabric Control Framework,Aggregate Manager Handlers
-Author-email: Komal Thareja <kthare10@renci.org>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: ansible==7.5.0
-Requires-Dist: paramiko
-Requires-Dist: fabric-cf==1.6.2rc0
-Requires-Dist: pytest ; extra == "test"
-Project-URL: Home, https://fabric-testbed.net/
-Project-URL: Sources, https://github.com/fabric-testbed/ControlFramework
-Provides-Extra: test
-
-[![PyPI](https://img.shields.io/pypi/v/fabric-am-handlers?style=plastic)](https://pypi.org/project/fabric-am-handlers/)
-
-# AMHandlers
-## Aggregate Manager
-An aggregate manager controls access to the substrate components. It controls some set of infrastructure resources in a particular site consisting of a set of servers, storage units, network elements or other components under common ownership and control. AMs inform brokers about available resources by passing to the resource advertisement information models. AMs may be associated with more than one broker and the partitioning of resources between brokers is the decision left to the AM. Oversubscription is possible, depending on the deployment needs.
-FABRIC enables a substrate provider to outsource resource arbitration and calendar scheduling to a broker. By delegating resources to the broker, the AM consents to the broker’s policies, and agrees to try to honor reservations issued by the broker if the user has authorization on the AM. 
-
-Besides, common code each AM type has resource-specific modules that determine its resource allocation behavior (Resource Management Policy) and the specific actions it takes to provision a sliver (Resource Handler). Both plugins are invoked by AM common core code based on the resource type or type of request being considered. 
-
-## Handlers
-The AM up calls a handler interface to setup and teardown each sliver. Resource handlers perform any substrate-specific configuration actions needed to implement slivers. The handler interface includes a probe method to poll the current status of a sliver, and modify to adjust attributes of a sliver. 
-
-Handlers are registered and selected by resource type. Each handler invocation executes in an independent thread, so handlers may block for slow configuration actions. Handlers are invoked through a class called HandlerProcessor, which can invoke an interpreter for a handler scripting language. The handlers will be written in the Python scripting language. 
-
-Each handler implements 3 basic operation types for a resource:
-- Create - provision a resource
-  - Example - create a VM or a bare-metal node, or a network connection
-- Delete - un-provision a resource
-  - Undo the create above
-- Modify - modify the state of a resource
-  - Modify a property of the VM, or a network connection (e.g. change bandwidth)
-  
-Each operation can have subcommands and parameters that determine the details of the actions taken, some of which are discussed below. These parameters help ‘stitch’ multiple slivers together. A canonical example is the passing of network information from the handler provisioning the network to the handler provisioning a compute node so that the compute node ends up with correct network configuration (e.g. attached to a correct VLAN). Specific parameters for operations are a matter of convention between the resource management policy and the plugin. 
-
-Handlers receive the parameters as part of the provisioning workflow (sequence of redeem operations) executed by the Orchestrator on the AMs. They can also pass information back to the Orchestrator about reserved resources as part of the standard exchange of messages between AM and Orchestrator during the provisioning.
-
-## Playbooks
-Handlers use Ansible Playbooks for provisioning.  
-
-## Interface and design
-![Class Diagram](./images/handlers.png)
-
-## Configuration
-AM Handlers require following configuration to be setup:
-- [Inventory](./fabric_am/playbooks/inventory) information for the headnode 
-- Handler config file (VM Handler example depicted below)
-### VM Handler Config File
-VM Handler config file can be found `fabric_am/config/vm_handler_config.yml`. 
-It describes the Playbook location and names for specific operations. 
-```
-playbooks:
-  location: /etc/fabric/actor/playbooks
-  inventory_location: /etc/fabric/actor/playbooks/inventory
-  VM: head_vm_provisioning.yml
-  GPU: worker_pci_provisioning.yml
-  SmartNIC: worker_pci_provisioning.yml
-  SharedNIC: worker_pci_provisioning.yml
-  FPGA: worker_pci_provisioning.yml
-  NVME: worker_pci_provisioning.yml
-```
-
-### PCI Devices support
-PCI devices are passed to the VMs using PCI pass through. FABRIC also support `SRIOV` functions which are also passed on to the VMs using PCI pass through. In order to handle the hairpin connections on `SRIOV`, `VEPA` mode is enabled on the underlying bridge for the dedicated card used to host the virtual functions.
-```
-[kissel@uky-w1 ~]$ sudo bridge link set dev ens6f1 hwmode vepa
-```
-
-#### What is VEPA?
-In the standard mode the software upgrade to the `VEB` in the hypervisor simply forces each VM frame out to the external switch regardless of destination. This causes no change for destination MAC addresses external to the host, but for destinations within the host (another VM in the same VLAN) it forces that traffic to the upstream switch which forwards it back instead of handling it internally, called a hairpin turn.) It's this hairpin turn that causes the requirement for the upstream switch to have updated firmware, typical STP behavior prevents a switch from forwarding a frame back down the port it was received on. The firmware update allows the negotiation between the physical host and the upstream switch of a VEPA port which then allows this hairpin turn.
-
-VEPA simply forces VM traffic to be handled by an external switch. This allows each VM frame flow to be monitored managed and secured with all of the tools available to the physical switch. This does not provide any type of individual tunnel for the VM, or a configurable switchport but does allow for things like flow statistic gathering, ACL enforcement, etc. Basically we're just pushing the MAC forwarding decision to the physical switch and allowing that switch to perform whatever functions it has available on each transaction. The drawback here is that we are now performing one ingress and egress for each frame that was previously handled internally. This means that there are bandwidth and latency considerations to be made. Functions like Single Root I/O Virtualization (SR/IOV) and Direct Path I/O can alleviate some of the latency issues when implementing this. Like any technology there are typically trade offs that must be weighed. In this case the added control and functionality should outweigh the bandwidth and latency additions.
-
-More details about `VEPA` can be found [here](https://www.ieee802.org/1/files/public/docs2009/new-hudson-vepa_seminar-20090514d.pdf)
-
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
```

