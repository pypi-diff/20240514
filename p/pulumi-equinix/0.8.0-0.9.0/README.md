# Comparing `tmp/pulumi_equinix-0.8.0.tar.gz` & `tmp/pulumi_equinix-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_equinix-0.8.0.tar", last modified: Tue Apr  2 22:41:07 2024, max compression
+gzip compressed data, was "pulumi_equinix-0.9.0.tar", last modified: Tue May 14 14:31:30 2024, max compression
```

## Comparing `pulumi_equinix-0.8.0.tar` & `pulumi_equinix-0.9.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.924653 pulumi_equinix-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-02 22:41:07.924653 pulumi_equinix-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.908653 pulumi_equinix-0.8.0/pulumi_equinix/
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.908653 pulumi_equinix-0.8.0/pulumi_equinix/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.912653 pulumi_equinix-0.8.0/pulumi_equinix/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)   234701 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41365 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/cloud_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    41755 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_cloud_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_routing_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_service_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_service_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25331 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/network.py
--rw-r--r--   0 runner    (1001) docker     (127)   448327 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37312 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/routing_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    49242 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/fabric/service_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.920653 pulumi_equinix-0.8.0/pulumi_equinix/metal/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    43853 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/bgp_session.py
--rw-r--r--   0 runner    (1001) docker     (127)   116162 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/device_network_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_device_bgp_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_interconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_ip_block_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_metro.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_port.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_precreated_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_spot_market_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/get_vrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    51542 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/interconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/ip_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    74121 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/port_vlan_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/project_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    48229 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    29621 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    42384 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    18162 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/metal/vrf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.924653 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    68241 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25536 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/acl_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)   104546 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    22397 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/device_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    26888 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_device_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_device_software.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_device_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    23179 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/network_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    97627 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/networkedge/ssh_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:41:07.908653 pulumi_equinix-0.8.0/pulumi_equinix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/pulumi_equinix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:41:07.924653 pulumi_equinix-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 22:41:07.000000 pulumi_equinix-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.653773 pulumi_equinix-0.9.0/pulumi_equinix/
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.653773 pulumi_equinix-0.9.0/pulumi_equinix/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.657773 pulumi_equinix-0.9.0/pulumi_equinix/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)   234801 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41117 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/cloud_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43191 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_cloud_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_routing_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_service_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_service_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25175 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)   449076 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37312 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/routing_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52222 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/service_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.661773 pulumi_equinix-0.9.0/pulumi_equinix/metal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43843 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116295 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/device_network_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device_bgp_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_ip_block_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_metro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_precreated_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51542 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/ip_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74111 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/port_vlan_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/project_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48329 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29621 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42484 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18262 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/vrf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69946 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25536 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/acl_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104546 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29791 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26748 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23179 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/network_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99377 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.653773 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/setup.py
```

### Comparing `pulumi_equinix-0.8.0/PKG-INFO` & `pulumi_equinix-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_equinix
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_equinix-0.8.0/README.md` & `pulumi_equinix-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/__init__.py` & `pulumi_equinix-0.9.0/pulumi_equinix/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/_enums.py` & `pulumi_equinix-0.9.0/pulumi_equinix/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/_utilities.py` & `pulumi_equinix-0.9.0/pulumi_equinix/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/config/vars.py` & `pulumi_equinix-0.9.0/pulumi_equinix/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/__init__.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/_enums.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/_inputs.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,15 +658,15 @@
         :param pulumi.Input['ConnectionASideAccessPointNetworkArgs'] network: network access point information
         :param pulumi.Input[Union[str, 'AccessPointPeeringType']] peering_type: Peering Type- PRIVATE,MICROSOFT,PUBLIC, MANUAL
         :param pulumi.Input['ConnectionASideAccessPointPortArgs'] port: Port access point information
         :param pulumi.Input['ConnectionASideAccessPointProfileArgs'] profile: Service Profile
         :param pulumi.Input[str] provider_connection_id: Provider assigned Connection Id
         :param pulumi.Input['ConnectionASideAccessPointRouterArgs'] router: Cloud Router access point information that replaces `gateway`
         :param pulumi.Input[str] seller_region: Access point seller region
-        :param pulumi.Input[Union[str, 'AccessPointType']] type: Interface type
+        :param pulumi.Input[Union[str, 'AccessPointType']] type: Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         :param pulumi.Input['ConnectionASideAccessPointVirtualDeviceArgs'] virtual_device: Virtual device
         """
         if account is not None:
             pulumi.set(__self__, "account", account)
         if authentication_key is not None:
             pulumi.set(__self__, "authentication_key", authentication_key)
         if gateway is not None:
@@ -858,15 +858,15 @@
     def seller_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "seller_region", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'AccessPointType']]]:
         """
-        Interface type
+        Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'AccessPointType']]]):
         pulumi.set(self, "type", value)
 
@@ -1062,15 +1062,15 @@
     def __init__(__self__, *,
                  id: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[int] id: id
         :param pulumi.Input[str] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] uuid: Equinix-assigned interface identifier
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
@@ -1099,15 +1099,15 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned interface identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -1116,15 +1116,15 @@
 class ConnectionASideAccessPointLinkProtocolArgs:
     def __init__(__self__, *,
                  type: Optional[pulumi.Input[Union[str, 'AccessPointLinkProtocolType']]] = None,
                  vlan_c_tag: Optional[pulumi.Input[int]] = None,
                  vlan_s_tag: Optional[pulumi.Input[int]] = None,
                  vlan_tag: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[Union[str, 'AccessPointLinkProtocolType']] type: Interface type
+        :param pulumi.Input[Union[str, 'AccessPointLinkProtocolType']] type: Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         :param pulumi.Input[int] vlan_c_tag: Vlan Customer Tag information, vlanCTag value specified for QINQ connections
         :param pulumi.Input[int] vlan_s_tag: Vlan Provider Tag information, vlanSTag value specified for QINQ connections
         :param pulumi.Input[int] vlan_tag: Vlan Tag information, vlanTag value specified for DOT1Q connections
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if vlan_c_tag is not None:
@@ -1134,15 +1134,15 @@
         if vlan_tag is not None:
             pulumi.set(__self__, "vlan_tag", vlan_tag)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'AccessPointLinkProtocolType']]]:
         """
-        Interface type
+        Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'AccessPointLinkProtocolType']]]):
         pulumi.set(self, "type", value)
 
@@ -1257,15 +1257,15 @@
 @pulumi.input_type
 class ConnectionASideAccessPointNetworkArgs:
     def __init__(__self__, *,
                  href: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] uuid: Equinix-assigned Network identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
@@ -1280,15 +1280,15 @@
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Network identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -1300,15 +1300,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  redundancy: Optional[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
         :param pulumi.Input[str] name: Port name
         :param pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs'] redundancy: Redundancy Information
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] uuid: Equinix-assigned Port identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if redundancy is not None:
             pulumi.set(__self__, "redundancy", redundancy)
@@ -1351,15 +1351,15 @@
     def redundancy(self, value: Optional[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']]):
         pulumi.set(self, "redundancy", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Port identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -1368,16 +1368,16 @@
 class ConnectionASideAccessPointPortRedundancyArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] enabled: Access point redundancy
-        :param pulumi.Input[str] group: Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
-        :param pulumi.Input[str] priority: Connection priority in redundancy group - PRIMARY, SECONDARY
+        :param pulumi.Input[str] group: Port redundancy group
+        :param pulumi.Input[str] priority: Priority type-Primary or Secondary
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
@@ -1394,27 +1394,27 @@
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
         """
-        Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
+        Port redundancy group
         """
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[str]]:
         """
-        Connection priority in redundancy group - PRIMARY, SECONDARY
+        Priority type-Primary or Secondary
         """
         return pulumi.get(self, "priority")
 
     @priority.setter
     def priority(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "priority", value)
 
@@ -1425,20 +1425,20 @@
                  type: pulumi.Input[Union[str, 'ProfileType']],
                  uuid: pulumi.Input[str],
                  access_point_type_configs: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionASideAccessPointProfileAccessPointTypeConfigArgs']]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  href: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Union[str, 'ProfileType']] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[Union[str, 'ProfileType']] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
+        :param pulumi.Input[str] uuid: Equinix assigned service profile identifier
         :param pulumi.Input[Sequence[pulumi.Input['ConnectionASideAccessPointProfileAccessPointTypeConfigArgs']]] access_point_type_configs: Access point config information
         :param pulumi.Input[str] description: User-provided service description
-        :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[str] name: Port name
+        :param pulumi.Input[str] href: Service Profile URI response attribute
+        :param pulumi.Input[str] name: Customer-assigned service profile name
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
         if access_point_type_configs is not None:
             pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -1447,27 +1447,27 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[Union[str, 'ProfileType']]:
         """
-        Interface type
+        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[Union[str, 'ProfileType']]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> pulumi.Input[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix assigned service profile identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: pulumi.Input[str]):
         pulumi.set(self, "uuid", value)
 
@@ -1495,66 +1495,66 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource Identifier
+        Service Profile URI response attribute
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Port name
+        Customer-assigned service profile name
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class ConnectionASideAccessPointProfileAccessPointTypeConfigArgs:
     def __init__(__self__, *,
                  type: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] type: Type of access point type config - VD, COLO
+        :param pulumi.Input[str] uuid: Equinix-assigned access point type config identifier
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Interface type
+        Type of access point type config - VD, COLO
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned access point type config identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -1603,17 +1603,17 @@
     def __init__(__self__, *,
                  href: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[str] name: Port name
-        :param pulumi.Input[str] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] name: Customer-assigned Virtual Device Name
+        :param pulumi.Input[str] type: Virtual Device type
+        :param pulumi.Input[str] uuid: Equinix-assigned Virtual Device identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if type is not None:
             pulumi.set(__self__, "type", type)
@@ -1632,39 +1632,39 @@
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Port name
+        Customer-assigned Virtual Device Name
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Interface type
+        Virtual Device type
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Virtual Device identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -1712,69 +1712,69 @@
 class ConnectionASideServiceTokenArgs:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  href: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[Union[str, 'ServiceTokenType']]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] description: User-provided service description
-        :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[Union[str, 'ServiceTokenType']] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] description: Service token description
+        :param pulumi.Input[str] href: An absolute URL that is the subject of the link's context
+        :param pulumi.Input[Union[str, 'ServiceTokenType']] type: Token type - VC_TOKEN
+        :param pulumi.Input[str] uuid: Equinix-assigned service token identifier
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if href is not None:
             pulumi.set(__self__, "href", href)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        User-provided service description
+        Service token description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource Identifier
+        An absolute URL that is the subject of the link's context
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'ServiceTokenType']]]:
         """
-        Interface type
+        Token type - VC_TOKEN
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'ServiceTokenType']]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned service token identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -2227,15 +2227,15 @@
                  additional_info: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionOperationErrorAdditionalInfoArgs']]]] = None,
                  correlation_id: Optional[pulumi.Input[str]] = None,
                  details: Optional[pulumi.Input[str]] = None,
                  error_code: Optional[pulumi.Input[str]] = None,
                  error_message: Optional[pulumi.Input[str]] = None,
                  help: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['ConnectionOperationErrorAdditionalInfoArgs']]] additional_info: Connection side additional information
+        :param pulumi.Input[Sequence[pulumi.Input['ConnectionOperationErrorAdditionalInfoArgs']]] additional_info: Pricing error additional Info
         :param pulumi.Input[str] correlation_id: CorrelationId
         :param pulumi.Input[str] details: Details
         :param pulumi.Input[str] error_code: Error  code
         :param pulumi.Input[str] error_message: Error Message
         :param pulumi.Input[str] help: Help
         """
         if additional_info is not None:
@@ -2251,15 +2251,15 @@
         if help is not None:
             pulumi.set(__self__, "help", help)
 
     @property
     @pulumi.getter(name="additionalInfo")
     def additional_info(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionOperationErrorAdditionalInfoArgs']]]]:
         """
-        Connection side additional information
+        Pricing error additional Info
         """
         return pulumi.get(self, "additional_info")
 
     @additional_info.setter
     def additional_info(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionOperationErrorAdditionalInfoArgs']]]]):
         pulumi.set(self, "additional_info", value)
 
@@ -2595,15 +2595,15 @@
         :param pulumi.Input['ConnectionZSideAccessPointNetworkArgs'] network: network access point information
         :param pulumi.Input[Union[str, 'AccessPointPeeringType']] peering_type: Peering Type- PRIVATE,MICROSOFT,PUBLIC, MANUAL
         :param pulumi.Input['ConnectionZSideAccessPointPortArgs'] port: Port access point information
         :param pulumi.Input['ConnectionZSideAccessPointProfileArgs'] profile: Service Profile
         :param pulumi.Input[str] provider_connection_id: Provider assigned Connection Id
         :param pulumi.Input['ConnectionZSideAccessPointRouterArgs'] router: Cloud Router access point information that replaces `gateway`
         :param pulumi.Input[str] seller_region: Access point seller region
-        :param pulumi.Input[Union[str, 'AccessPointType']] type: Interface type
+        :param pulumi.Input[Union[str, 'AccessPointType']] type: Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         :param pulumi.Input['ConnectionZSideAccessPointVirtualDeviceArgs'] virtual_device: Virtual device
         """
         if account is not None:
             pulumi.set(__self__, "account", account)
         if authentication_key is not None:
             pulumi.set(__self__, "authentication_key", authentication_key)
         if gateway is not None:
@@ -2795,15 +2795,15 @@
     def seller_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "seller_region", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'AccessPointType']]]:
         """
-        Interface type
+        Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'AccessPointType']]]):
         pulumi.set(self, "type", value)
 
@@ -2999,15 +2999,15 @@
     def __init__(__self__, *,
                  id: Optional[pulumi.Input[int]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[int] id: id
         :param pulumi.Input[str] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] uuid: Equinix-assigned interface identifier
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
@@ -3036,15 +3036,15 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned interface identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -3053,15 +3053,15 @@
 class ConnectionZSideAccessPointLinkProtocolArgs:
     def __init__(__self__, *,
                  type: Optional[pulumi.Input[Union[str, 'AccessPointLinkProtocolType']]] = None,
                  vlan_c_tag: Optional[pulumi.Input[int]] = None,
                  vlan_s_tag: Optional[pulumi.Input[int]] = None,
                  vlan_tag: Optional[pulumi.Input[int]] = None):
         """
-        :param pulumi.Input[Union[str, 'AccessPointLinkProtocolType']] type: Interface type
+        :param pulumi.Input[Union[str, 'AccessPointLinkProtocolType']] type: Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         :param pulumi.Input[int] vlan_c_tag: Vlan Customer Tag information, vlanCTag value specified for QINQ connections
         :param pulumi.Input[int] vlan_s_tag: Vlan Provider Tag information, vlanSTag value specified for QINQ connections
         :param pulumi.Input[int] vlan_tag: Vlan Tag information, vlanTag value specified for DOT1Q connections
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if vlan_c_tag is not None:
@@ -3071,15 +3071,15 @@
         if vlan_tag is not None:
             pulumi.set(__self__, "vlan_tag", vlan_tag)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'AccessPointLinkProtocolType']]]:
         """
-        Interface type
+        Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'AccessPointLinkProtocolType']]]):
         pulumi.set(self, "type", value)
 
@@ -3194,15 +3194,15 @@
 @pulumi.input_type
 class ConnectionZSideAccessPointNetworkArgs:
     def __init__(__self__, *,
                  href: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] uuid: Equinix-assigned Network identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
@@ -3217,15 +3217,15 @@
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Network identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -3237,15 +3237,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  redundancy: Optional[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
         :param pulumi.Input[str] name: Port name
         :param pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs'] redundancy: Redundancy Information
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] uuid: Equinix-assigned Port identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if redundancy is not None:
             pulumi.set(__self__, "redundancy", redundancy)
@@ -3288,15 +3288,15 @@
     def redundancy(self, value: Optional[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']]):
         pulumi.set(self, "redundancy", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Port identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -3305,16 +3305,16 @@
 class ConnectionZSideAccessPointPortRedundancyArgs:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  group: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] enabled: Access point redundancy
-        :param pulumi.Input[str] group: Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
-        :param pulumi.Input[str] priority: Connection priority in redundancy group - PRIMARY, SECONDARY
+        :param pulumi.Input[str] group: Port redundancy group
+        :param pulumi.Input[str] priority: Priority type-Primary or Secondary
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
@@ -3331,27 +3331,27 @@
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter
     def group(self) -> Optional[pulumi.Input[str]]:
         """
-        Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
+        Port redundancy group
         """
         return pulumi.get(self, "group")
 
     @group.setter
     def group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "group", value)
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[str]]:
         """
-        Connection priority in redundancy group - PRIMARY, SECONDARY
+        Priority type-Primary or Secondary
         """
         return pulumi.get(self, "priority")
 
     @priority.setter
     def priority(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "priority", value)
 
@@ -3362,20 +3362,20 @@
                  type: pulumi.Input[Union[str, 'ProfileType']],
                  uuid: pulumi.Input[str],
                  access_point_type_configs: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionZSideAccessPointProfileAccessPointTypeConfigArgs']]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  href: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Union[str, 'ProfileType']] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[Union[str, 'ProfileType']] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
+        :param pulumi.Input[str] uuid: Equinix assigned service profile identifier
         :param pulumi.Input[Sequence[pulumi.Input['ConnectionZSideAccessPointProfileAccessPointTypeConfigArgs']]] access_point_type_configs: Access point config information
         :param pulumi.Input[str] description: User-provided service description
-        :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[str] name: Port name
+        :param pulumi.Input[str] href: Service Profile URI response attribute
+        :param pulumi.Input[str] name: Customer-assigned service profile name
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
         if access_point_type_configs is not None:
             pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -3384,27 +3384,27 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[Union[str, 'ProfileType']]:
         """
-        Interface type
+        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[Union[str, 'ProfileType']]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> pulumi.Input[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix assigned service profile identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: pulumi.Input[str]):
         pulumi.set(self, "uuid", value)
 
@@ -3432,66 +3432,66 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource Identifier
+        Service Profile URI response attribute
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Port name
+        Customer-assigned service profile name
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class ConnectionZSideAccessPointProfileAccessPointTypeConfigArgs:
     def __init__(__self__, *,
                  type: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] type: Type of access point type config - VD, COLO
+        :param pulumi.Input[str] uuid: Equinix-assigned access point type config identifier
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Interface type
+        Type of access point type config - VD, COLO
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned access point type config identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -3540,17 +3540,17 @@
     def __init__(__self__, *,
                  href: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[str] name: Port name
-        :param pulumi.Input[str] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] name: Customer-assigned Virtual Device Name
+        :param pulumi.Input[str] type: Virtual Device type
+        :param pulumi.Input[str] uuid: Equinix-assigned Virtual Device identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if type is not None:
             pulumi.set(__self__, "type", type)
@@ -3569,39 +3569,39 @@
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Port name
+        Customer-assigned Virtual Device Name
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Interface type
+        Virtual Device type
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Virtual Device identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -3649,69 +3649,69 @@
 class ConnectionZSideServiceTokenArgs:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  href: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[Union[str, 'ServiceTokenType']]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] description: User-provided service description
-        :param pulumi.Input[str] href: Unique Resource Identifier
-        :param pulumi.Input[Union[str, 'ServiceTokenType']] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[str] description: Service token description
+        :param pulumi.Input[str] href: An absolute URL that is the subject of the link's context
+        :param pulumi.Input[Union[str, 'ServiceTokenType']] type: Token type - VC_TOKEN
+        :param pulumi.Input[str] uuid: Equinix-assigned service token identifier
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if href is not None:
             pulumi.set(__self__, "href", href)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        User-provided service description
+        Service token description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource Identifier
+        An absolute URL that is the subject of the link's context
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'ServiceTokenType']]]:
         """
-        Interface type
+        Token type - VC_TOKEN
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'ServiceTokenType']]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned service token identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -5702,30 +5702,30 @@
 @pulumi.input_type
 class ServiceProfileMarketingInfoProcessStepArgs:
     def __init__(__self__, *,
                  description: Optional[pulumi.Input[str]] = None,
                  sub_title: Optional[pulumi.Input[str]] = None,
                  title: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] description: Description of authorization key
+        :param pulumi.Input[str] description: Description
         :param pulumi.Input[str] sub_title: Sub Title
         :param pulumi.Input[str] title: Title
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if sub_title is not None:
             pulumi.set(__self__, "sub_title", sub_title)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description of authorization key
+        Description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/cloud_router.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/cloud_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,49 +15,50 @@
 
 @pulumi.input_type
 class CloudRouterArgs:
     def __init__(__self__, *,
                  account: pulumi.Input['CloudRouterAccountArgs'],
                  location: pulumi.Input['CloudRouterLocationArgs'],
                  notifications: pulumi.Input[Sequence[pulumi.Input['CloudRouterNotificationArgs']]],
-                 order: pulumi.Input['CloudRouterOrderArgs'],
                  package: pulumi.Input['CloudRouterPackageArgs'],
                  project: pulumi.Input['CloudRouterProjectArgs'],
                  type: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
                  href: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 order: Optional[pulumi.Input['CloudRouterOrderArgs']] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a CloudRouter resource.
         :param pulumi.Input['CloudRouterAccountArgs'] account: Customer account information that is associated with this Fabric Cloud Router
         :param pulumi.Input['CloudRouterLocationArgs'] location: Fabric Cloud Router location
         :param pulumi.Input[Sequence[pulumi.Input['CloudRouterNotificationArgs']]] notifications: Preferences for notifications on Fabric Cloud Router configuration or status changes
-        :param pulumi.Input['CloudRouterOrderArgs'] order: Order information related to this Fabric Cloud Router
         :param pulumi.Input['CloudRouterPackageArgs'] package: Fabric Cloud Router Package Type
-        :param pulumi.Input['CloudRouterProjectArgs'] project: Customer resource hierarchy project information.Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
-        :param pulumi.Input[str] type: Notification Type - ALL,CONNECTION*APPROVAL,SALES*REP_NOTIFICATIONS, NOTIFICATIONS
+        :param pulumi.Input['CloudRouterProjectArgs'] project: Customer resource hierarchy project information. Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
+        :param pulumi.Input[str] type: Defines the FCR type like; XF_ROUTER
         :param pulumi.Input[str] description: Customer-provided Fabric Cloud Router description
-        :param pulumi.Input[str] href: Unique Resource URL
+        :param pulumi.Input[str] href: Fabric Cloud Router URI information
         :param pulumi.Input[str] name: Fabric Cloud Router name. An alpha-numeric 24 characters string which can include only hyphens and underscores
+        :param pulumi.Input['CloudRouterOrderArgs'] order: Order information related to this Fabric Cloud Router
         :param pulumi.Input[str] uuid: Equinix-assigned Fabric Cloud Router identifier
         """
         pulumi.set(__self__, "account", account)
         pulumi.set(__self__, "location", location)
         pulumi.set(__self__, "notifications", notifications)
-        pulumi.set(__self__, "order", order)
         pulumi.set(__self__, "package", package)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "type", type)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if order is not None:
+            pulumi.set(__self__, "order", order)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def account(self) -> pulumi.Input['CloudRouterAccountArgs']:
         """
@@ -91,53 +92,41 @@
 
     @notifications.setter
     def notifications(self, value: pulumi.Input[Sequence[pulumi.Input['CloudRouterNotificationArgs']]]):
         pulumi.set(self, "notifications", value)
 
     @property
     @pulumi.getter
-    def order(self) -> pulumi.Input['CloudRouterOrderArgs']:
-        """
-        Order information related to this Fabric Cloud Router
-        """
-        return pulumi.get(self, "order")
-
-    @order.setter
-    def order(self, value: pulumi.Input['CloudRouterOrderArgs']):
-        pulumi.set(self, "order", value)
-
-    @property
-    @pulumi.getter
     def package(self) -> pulumi.Input['CloudRouterPackageArgs']:
         """
         Fabric Cloud Router Package Type
         """
         return pulumi.get(self, "package")
 
     @package.setter
     def package(self, value: pulumi.Input['CloudRouterPackageArgs']):
         pulumi.set(self, "package", value)
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Input['CloudRouterProjectArgs']:
         """
-        Customer resource hierarchy project information.Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
+        Customer resource hierarchy project information. Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input['CloudRouterProjectArgs']):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
-        Notification Type - ALL,CONNECTION*APPROVAL,SALES*REP_NOTIFICATIONS, NOTIFICATIONS
+        Defines the FCR type like; XF_ROUTER
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
@@ -153,15 +142,15 @@
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource URL
+        Fabric Cloud Router URI information
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
@@ -175,14 +164,26 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
+    def order(self) -> Optional[pulumi.Input['CloudRouterOrderArgs']]:
+        """
+        Order information related to this Fabric Cloud Router
+        """
+        return pulumi.get(self, "order")
+
+    @order.setter
+    def order(self, value: Optional[pulumi.Input['CloudRouterOrderArgs']]):
+        pulumi.set(self, "order", value)
+
+    @property
+    @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
         Equinix-assigned Fabric Cloud Router identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
@@ -219,23 +220,23 @@
         :param pulumi.Input[int] bgp_ipv6_routes_count: Number of IPv6 BGP routes in use (including non-distinct prefixes)
         :param pulumi.Input[Sequence[pulumi.Input['CloudRouterChangeLogArgs']]] change_logs: Captures Fabric Cloud Router lifecycle change information
         :param pulumi.Input[int] connections_count: Number of connections associated with this Fabric Cloud Router instance
         :param pulumi.Input[str] description: Customer-provided Fabric Cloud Router description
         :param pulumi.Input[int] distinct_ipv4_prefixes_count: Number of distinct IPv4 routes
         :param pulumi.Input[int] distinct_ipv6_prefixes_count: Number of distinct IPv6 routes
         :param pulumi.Input[int] equinix_asn: Equinix ASN
-        :param pulumi.Input[str] href: Unique Resource URL
+        :param pulumi.Input[str] href: Fabric Cloud Router URI information
         :param pulumi.Input['CloudRouterLocationArgs'] location: Fabric Cloud Router location
         :param pulumi.Input[str] name: Fabric Cloud Router name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input['CloudRouterNotificationArgs']]] notifications: Preferences for notifications on Fabric Cloud Router configuration or status changes
         :param pulumi.Input['CloudRouterOrderArgs'] order: Order information related to this Fabric Cloud Router
         :param pulumi.Input['CloudRouterPackageArgs'] package: Fabric Cloud Router Package Type
-        :param pulumi.Input['CloudRouterProjectArgs'] project: Customer resource hierarchy project information.Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
+        :param pulumi.Input['CloudRouterProjectArgs'] project: Customer resource hierarchy project information. Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
         :param pulumi.Input[str] state: Fabric Cloud Router overall state
-        :param pulumi.Input[str] type: Notification Type - ALL,CONNECTION*APPROVAL,SALES*REP_NOTIFICATIONS, NOTIFICATIONS
+        :param pulumi.Input[str] type: Defines the FCR type like; XF_ROUTER
         :param pulumi.Input[str] uuid: Equinix-assigned Fabric Cloud Router identifier
         """
         if account is not None:
             pulumi.set(__self__, "account", account)
         if bgp_ipv4_routes_count is not None:
             pulumi.set(__self__, "bgp_ipv4_routes_count", bgp_ipv4_routes_count)
         if bgp_ipv6_routes_count is not None:
@@ -381,15 +382,15 @@
     def equinix_asn(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "equinix_asn", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource URL
+        Fabric Cloud Router URI information
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
@@ -453,15 +454,15 @@
     def package(self, value: Optional[pulumi.Input['CloudRouterPackageArgs']]):
         pulumi.set(self, "package", value)
 
     @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input['CloudRouterProjectArgs']]:
         """
-        Customer resource hierarchy project information.Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
+        Customer resource hierarchy project information. Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: Optional[pulumi.Input['CloudRouterProjectArgs']]):
         pulumi.set(self, "project", value)
 
@@ -477,15 +478,15 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Notification Type - ALL,CONNECTION*APPROVAL,SALES*REP_NOTIFICATIONS, NOTIFICATIONS
+        Defines the FCR type like; XF_ROUTER
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -555,22 +556,22 @@
         pulumi.export("routerId", router.id)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['CloudRouterAccountArgs']] account: Customer account information that is associated with this Fabric Cloud Router
         :param pulumi.Input[str] description: Customer-provided Fabric Cloud Router description
-        :param pulumi.Input[str] href: Unique Resource URL
+        :param pulumi.Input[str] href: Fabric Cloud Router URI information
         :param pulumi.Input[pulumi.InputType['CloudRouterLocationArgs']] location: Fabric Cloud Router location
         :param pulumi.Input[str] name: Fabric Cloud Router name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CloudRouterNotificationArgs']]]] notifications: Preferences for notifications on Fabric Cloud Router configuration or status changes
         :param pulumi.Input[pulumi.InputType['CloudRouterOrderArgs']] order: Order information related to this Fabric Cloud Router
         :param pulumi.Input[pulumi.InputType['CloudRouterPackageArgs']] package: Fabric Cloud Router Package Type
-        :param pulumi.Input[pulumi.InputType['CloudRouterProjectArgs']] project: Customer resource hierarchy project information.Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
-        :param pulumi.Input[str] type: Notification Type - ALL,CONNECTION*APPROVAL,SALES*REP_NOTIFICATIONS, NOTIFICATIONS
+        :param pulumi.Input[pulumi.InputType['CloudRouterProjectArgs']] project: Customer resource hierarchy project information. Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
+        :param pulumi.Input[str] type: Defines the FCR type like; XF_ROUTER
         :param pulumi.Input[str] uuid: Equinix-assigned Fabric Cloud Router identifier
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: CloudRouterArgs,
@@ -654,16 +655,14 @@
             if location is None and not opts.urn:
                 raise TypeError("Missing required property 'location'")
             __props__.__dict__["location"] = location
             __props__.__dict__["name"] = name
             if notifications is None and not opts.urn:
                 raise TypeError("Missing required property 'notifications'")
             __props__.__dict__["notifications"] = notifications
-            if order is None and not opts.urn:
-                raise TypeError("Missing required property 'order'")
             __props__.__dict__["order"] = order
             if package is None and not opts.urn:
                 raise TypeError("Missing required property 'package'")
             __props__.__dict__["package"] = package
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
@@ -720,23 +719,23 @@
         :param pulumi.Input[int] bgp_ipv6_routes_count: Number of IPv6 BGP routes in use (including non-distinct prefixes)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CloudRouterChangeLogArgs']]]] change_logs: Captures Fabric Cloud Router lifecycle change information
         :param pulumi.Input[int] connections_count: Number of connections associated with this Fabric Cloud Router instance
         :param pulumi.Input[str] description: Customer-provided Fabric Cloud Router description
         :param pulumi.Input[int] distinct_ipv4_prefixes_count: Number of distinct IPv4 routes
         :param pulumi.Input[int] distinct_ipv6_prefixes_count: Number of distinct IPv6 routes
         :param pulumi.Input[int] equinix_asn: Equinix ASN
-        :param pulumi.Input[str] href: Unique Resource URL
+        :param pulumi.Input[str] href: Fabric Cloud Router URI information
         :param pulumi.Input[pulumi.InputType['CloudRouterLocationArgs']] location: Fabric Cloud Router location
         :param pulumi.Input[str] name: Fabric Cloud Router name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CloudRouterNotificationArgs']]]] notifications: Preferences for notifications on Fabric Cloud Router configuration or status changes
         :param pulumi.Input[pulumi.InputType['CloudRouterOrderArgs']] order: Order information related to this Fabric Cloud Router
         :param pulumi.Input[pulumi.InputType['CloudRouterPackageArgs']] package: Fabric Cloud Router Package Type
-        :param pulumi.Input[pulumi.InputType['CloudRouterProjectArgs']] project: Customer resource hierarchy project information.Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
+        :param pulumi.Input[pulumi.InputType['CloudRouterProjectArgs']] project: Customer resource hierarchy project information. Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
         :param pulumi.Input[str] state: Fabric Cloud Router overall state
-        :param pulumi.Input[str] type: Notification Type - ALL,CONNECTION*APPROVAL,SALES*REP_NOTIFICATIONS, NOTIFICATIONS
+        :param pulumi.Input[str] type: Defines the FCR type like; XF_ROUTER
         :param pulumi.Input[str] uuid: Equinix-assigned Fabric Cloud Router identifier
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CloudRouterState.__new__(_CloudRouterState)
 
         __props__.__dict__["account"] = account
@@ -832,15 +831,15 @@
         """
         return pulumi.get(self, "equinix_asn")
 
     @property
     @pulumi.getter
     def href(self) -> pulumi.Output[str]:
         """
-        Unique Resource URL
+        Fabric Cloud Router URI information
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def location(self) -> pulumi.Output['outputs.CloudRouterLocation']:
         """
@@ -880,15 +879,15 @@
         """
         return pulumi.get(self, "package")
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Output['outputs.CloudRouterProject']:
         """
-        Customer resource hierarchy project information.Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
+        Customer resource hierarchy project information. Applicable to customers onboarded to Equinix Identity and Access Management. For more information see Identity and Access Management: Projects
         """
         return pulumi.get(self, "project")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
@@ -896,15 +895,15 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        Notification Type - ALL,CONNECTION*APPROVAL,SALES*REP_NOTIFICATIONS, NOTIFICATIONS
+        Defines the FCR type like; XF_ROUTER
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/connection.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,48 +17,49 @@
 
 @pulumi.input_type
 class ConnectionArgs:
     def __init__(__self__, *,
                  a_side: pulumi.Input['ConnectionASideArgs'],
                  bandwidth: pulumi.Input[int],
                  notifications: pulumi.Input[Sequence[pulumi.Input['ConnectionNotificationArgs']]],
-                 order: pulumi.Input['ConnectionOrderArgs'],
                  type: pulumi.Input[Union[str, 'ConnectionType']],
                  z_side: pulumi.Input['ConnectionZSideArgs'],
                  additional_info: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 order: Optional[pulumi.Input['ConnectionOrderArgs']] = None,
                  project: Optional[pulumi.Input['ConnectionProjectArgs']] = None,
                  redundancy: Optional[pulumi.Input['ConnectionRedundancyArgs']] = None):
         """
         The set of arguments for constructing a Connection resource.
         :param pulumi.Input['ConnectionASideArgs'] a_side: Requester or Customer side connection configuration object of the multi-segment connection
         :param pulumi.Input[int] bandwidth: Connection bandwidth in Mbps
         :param pulumi.Input[Sequence[pulumi.Input['ConnectionNotificationArgs']]] notifications: Preferences for notifications on connection configuration or status changes
-        :param pulumi.Input['ConnectionOrderArgs'] order: Order details
-        :param pulumi.Input[Union[str, 'ConnectionType']] type: Interface type
+        :param pulumi.Input[Union[str, 'ConnectionType']] type: Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         :param pulumi.Input['ConnectionZSideArgs'] z_side: Destination or Provider side connection configuration object of the multi-segment connection
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection side additional information
-        :param pulumi.Input[str] description: User-provided service description
-        :param pulumi.Input[str] name: Port name
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection additional information
+        :param pulumi.Input[str] description: Customer-provided connection description
+        :param pulumi.Input[str] name: Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
+        :param pulumi.Input['ConnectionOrderArgs'] order: Order details
         :param pulumi.Input['ConnectionProjectArgs'] project: Project information
-        :param pulumi.Input['ConnectionRedundancyArgs'] redundancy: Redundancy Information
+        :param pulumi.Input['ConnectionRedundancyArgs'] redundancy: Connection Redundancy Configuration
         """
         pulumi.set(__self__, "a_side", a_side)
         pulumi.set(__self__, "bandwidth", bandwidth)
         pulumi.set(__self__, "notifications", notifications)
-        pulumi.set(__self__, "order", order)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "z_side", z_side)
         if additional_info is not None:
             pulumi.set(__self__, "additional_info", additional_info)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if order is not None:
+            pulumi.set(__self__, "order", order)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if redundancy is not None:
             pulumi.set(__self__, "redundancy", redundancy)
 
     @property
     @pulumi.getter(name="aSide")
@@ -94,29 +95,17 @@
 
     @notifications.setter
     def notifications(self, value: pulumi.Input[Sequence[pulumi.Input['ConnectionNotificationArgs']]]):
         pulumi.set(self, "notifications", value)
 
     @property
     @pulumi.getter
-    def order(self) -> pulumi.Input['ConnectionOrderArgs']:
-        """
-        Order details
-        """
-        return pulumi.get(self, "order")
-
-    @order.setter
-    def order(self, value: pulumi.Input['ConnectionOrderArgs']):
-        pulumi.set(self, "order", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> pulumi.Input[Union[str, 'ConnectionType']]:
         """
-        Interface type
+        Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[Union[str, 'ConnectionType']]):
         pulumi.set(self, "type", value)
 
@@ -132,63 +121,75 @@
     def z_side(self, value: pulumi.Input['ConnectionZSideArgs']):
         pulumi.set(self, "z_side", value)
 
     @property
     @pulumi.getter(name="additionalInfo")
     def additional_info(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]]:
         """
-        Connection side additional information
+        Connection additional information
         """
         return pulumi.get(self, "additional_info")
 
     @additional_info.setter
     def additional_info(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]]):
         pulumi.set(self, "additional_info", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        User-provided service description
+        Customer-provided connection description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Port name
+        Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
+    def order(self) -> Optional[pulumi.Input['ConnectionOrderArgs']]:
+        """
+        Order details
+        """
+        return pulumi.get(self, "order")
+
+    @order.setter
+    def order(self, value: Optional[pulumi.Input['ConnectionOrderArgs']]):
+        pulumi.set(self, "order", value)
+
+    @property
+    @pulumi.getter
     def project(self) -> Optional[pulumi.Input['ConnectionProjectArgs']]:
         """
         Project information
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: Optional[pulumi.Input['ConnectionProjectArgs']]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
     def redundancy(self) -> Optional[pulumi.Input['ConnectionRedundancyArgs']]:
         """
-        Redundancy Information
+        Connection Redundancy Configuration
         """
         return pulumi.get(self, "redundancy")
 
     @redundancy.setter
     def redundancy(self, value: Optional[pulumi.Input['ConnectionRedundancyArgs']]):
         pulumi.set(self, "redundancy", value)
 
@@ -214,31 +215,31 @@
                  state: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[Union[str, 'ConnectionType']]] = None,
                  uuid: Optional[pulumi.Input[str]] = None,
                  z_side: Optional[pulumi.Input['ConnectionZSideArgs']] = None):
         """
         Input properties used for looking up and filtering Connection resources.
         :param pulumi.Input['ConnectionASideArgs'] a_side: Requester or Customer side connection configuration object of the multi-segment connection
-        :param pulumi.Input['ConnectionAccountArgs'] account: Account
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection side additional information
+        :param pulumi.Input['ConnectionAccountArgs'] account: Customer account information that is associated with this connection
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection additional information
         :param pulumi.Input[int] bandwidth: Connection bandwidth in Mbps
         :param pulumi.Input['ConnectionChangeLogArgs'] change_log: Captures connection lifecycle change information
-        :param pulumi.Input[str] description: User-provided service description
+        :param pulumi.Input[str] description: Customer-provided connection description
         :param pulumi.Input[str] direction: Connection directionality from the requester point of view
-        :param pulumi.Input[str] href: Unique Resource Identifier
+        :param pulumi.Input[str] href: Connection URI information
         :param pulumi.Input[bool] is_remote: Connection property derived from access point locations
-        :param pulumi.Input[str] name: Port name
+        :param pulumi.Input[str] name: Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input['ConnectionNotificationArgs']]] notifications: Preferences for notifications on connection configuration or status changes
         :param pulumi.Input['ConnectionOperationArgs'] operation: Connection type-specific operational data
         :param pulumi.Input['ConnectionOrderArgs'] order: Order details
         :param pulumi.Input['ConnectionProjectArgs'] project: Project information
-        :param pulumi.Input['ConnectionRedundancyArgs'] redundancy: Redundancy Information
+        :param pulumi.Input['ConnectionRedundancyArgs'] redundancy: Connection Redundancy Configuration
         :param pulumi.Input[str] state: Connection overall state
-        :param pulumi.Input[Union[str, 'ConnectionType']] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[Union[str, 'ConnectionType']] type: Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
+        :param pulumi.Input[str] uuid: Equinix-assigned connection identifier
         :param pulumi.Input['ConnectionZSideArgs'] z_side: Destination or Provider side connection configuration object of the multi-segment connection
         """
         if a_side is not None:
             pulumi.set(__self__, "a_side", a_side)
         if account is not None:
             pulumi.set(__self__, "account", account)
         if additional_info is not None:
@@ -288,27 +289,27 @@
     def a_side(self, value: Optional[pulumi.Input['ConnectionASideArgs']]):
         pulumi.set(self, "a_side", value)
 
     @property
     @pulumi.getter
     def account(self) -> Optional[pulumi.Input['ConnectionAccountArgs']]:
         """
-        Account
+        Customer account information that is associated with this connection
         """
         return pulumi.get(self, "account")
 
     @account.setter
     def account(self, value: Optional[pulumi.Input['ConnectionAccountArgs']]):
         pulumi.set(self, "account", value)
 
     @property
     @pulumi.getter(name="additionalInfo")
     def additional_info(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]]:
         """
-        Connection side additional information
+        Connection additional information
         """
         return pulumi.get(self, "additional_info")
 
     @additional_info.setter
     def additional_info(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]]):
         pulumi.set(self, "additional_info", value)
 
@@ -336,15 +337,15 @@
     def change_log(self, value: Optional[pulumi.Input['ConnectionChangeLogArgs']]):
         pulumi.set(self, "change_log", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        User-provided service description
+        Customer-provided connection description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -360,15 +361,15 @@
     def direction(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "direction", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource Identifier
+        Connection URI information
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
@@ -384,15 +385,15 @@
     def is_remote(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_remote", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Port name
+        Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -444,15 +445,15 @@
     def project(self, value: Optional[pulumi.Input['ConnectionProjectArgs']]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
     def redundancy(self) -> Optional[pulumi.Input['ConnectionRedundancyArgs']]:
         """
-        Redundancy Information
+        Connection Redundancy Configuration
         """
         return pulumi.get(self, "redundancy")
 
     @redundancy.setter
     def redundancy(self, value: Optional[pulumi.Input['ConnectionRedundancyArgs']]):
         pulumi.set(self, "redundancy", value)
 
@@ -468,27 +469,27 @@
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'ConnectionType']]]:
         """
-        Interface type
+        Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'ConnectionType']]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned connection identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
@@ -519,16 +520,14 @@
                  order: Optional[pulumi.Input[pulumi.InputType['ConnectionOrderArgs']]] = None,
                  project: Optional[pulumi.Input[pulumi.InputType['ConnectionProjectArgs']]] = None,
                  redundancy: Optional[pulumi.Input[pulumi.InputType['ConnectionRedundancyArgs']]] = None,
                  type: Optional[pulumi.Input[Union[str, 'ConnectionType']]] = None,
                  z_side: Optional[pulumi.Input[pulumi.InputType['ConnectionZSideArgs']]] = None,
                  __props__=None):
         """
-        Fabric V4 API compatible resource allows creation and management of Equinix Fabric connection
-
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
         metro = config.get("metro")
@@ -592,34 +591,32 @@
         pulumi.export("connectionProviderStatus", colo2_aws.operation.provider_status)
         pulumi.export("awsDirectConnectId", colo2_aws.z_side.access_point.provider_connection_id)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ConnectionASideArgs']] a_side: Requester or Customer side connection configuration object of the multi-segment connection
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection side additional information
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection additional information
         :param pulumi.Input[int] bandwidth: Connection bandwidth in Mbps
-        :param pulumi.Input[str] description: User-provided service description
-        :param pulumi.Input[str] name: Port name
+        :param pulumi.Input[str] description: Customer-provided connection description
+        :param pulumi.Input[str] name: Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ConnectionNotificationArgs']]]] notifications: Preferences for notifications on connection configuration or status changes
         :param pulumi.Input[pulumi.InputType['ConnectionOrderArgs']] order: Order details
         :param pulumi.Input[pulumi.InputType['ConnectionProjectArgs']] project: Project information
-        :param pulumi.Input[pulumi.InputType['ConnectionRedundancyArgs']] redundancy: Redundancy Information
-        :param pulumi.Input[Union[str, 'ConnectionType']] type: Interface type
+        :param pulumi.Input[pulumi.InputType['ConnectionRedundancyArgs']] redundancy: Connection Redundancy Configuration
+        :param pulumi.Input[Union[str, 'ConnectionType']] type: Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         :param pulumi.Input[pulumi.InputType['ConnectionZSideArgs']] z_side: Destination or Provider side connection configuration object of the multi-segment connection
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ConnectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Fabric V4 API compatible resource allows creation and management of Equinix Fabric connection
-
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
         metro = config.get("metro")
@@ -727,16 +724,14 @@
                 raise TypeError("Missing required property 'bandwidth'")
             __props__.__dict__["bandwidth"] = bandwidth
             __props__.__dict__["description"] = description
             __props__.__dict__["name"] = name
             if notifications is None and not opts.urn:
                 raise TypeError("Missing required property 'notifications'")
             __props__.__dict__["notifications"] = notifications
-            if order is None and not opts.urn:
-                raise TypeError("Missing required property 'order'")
             __props__.__dict__["order"] = order
             __props__.__dict__["project"] = project
             __props__.__dict__["redundancy"] = redundancy
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
             if z_side is None and not opts.urn:
@@ -783,31 +778,31 @@
         Get an existing Connection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ConnectionASideArgs']] a_side: Requester or Customer side connection configuration object of the multi-segment connection
-        :param pulumi.Input[pulumi.InputType['ConnectionAccountArgs']] account: Account
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection side additional information
+        :param pulumi.Input[pulumi.InputType['ConnectionAccountArgs']] account: Customer account information that is associated with this connection
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] additional_info: Connection additional information
         :param pulumi.Input[int] bandwidth: Connection bandwidth in Mbps
         :param pulumi.Input[pulumi.InputType['ConnectionChangeLogArgs']] change_log: Captures connection lifecycle change information
-        :param pulumi.Input[str] description: User-provided service description
+        :param pulumi.Input[str] description: Customer-provided connection description
         :param pulumi.Input[str] direction: Connection directionality from the requester point of view
-        :param pulumi.Input[str] href: Unique Resource Identifier
+        :param pulumi.Input[str] href: Connection URI information
         :param pulumi.Input[bool] is_remote: Connection property derived from access point locations
-        :param pulumi.Input[str] name: Port name
+        :param pulumi.Input[str] name: Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ConnectionNotificationArgs']]]] notifications: Preferences for notifications on connection configuration or status changes
         :param pulumi.Input[pulumi.InputType['ConnectionOperationArgs']] operation: Connection type-specific operational data
         :param pulumi.Input[pulumi.InputType['ConnectionOrderArgs']] order: Order details
         :param pulumi.Input[pulumi.InputType['ConnectionProjectArgs']] project: Project information
-        :param pulumi.Input[pulumi.InputType['ConnectionRedundancyArgs']] redundancy: Redundancy Information
+        :param pulumi.Input[pulumi.InputType['ConnectionRedundancyArgs']] redundancy: Connection Redundancy Configuration
         :param pulumi.Input[str] state: Connection overall state
-        :param pulumi.Input[Union[str, 'ConnectionType']] type: Interface type
-        :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
+        :param pulumi.Input[Union[str, 'ConnectionType']] type: Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
+        :param pulumi.Input[str] uuid: Equinix-assigned connection identifier
         :param pulumi.Input[pulumi.InputType['ConnectionZSideArgs']] z_side: Destination or Provider side connection configuration object of the multi-segment connection
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ConnectionState.__new__(_ConnectionState)
 
         __props__.__dict__["a_side"] = a_side
@@ -839,23 +834,23 @@
         """
         return pulumi.get(self, "a_side")
 
     @property
     @pulumi.getter
     def account(self) -> pulumi.Output['outputs.ConnectionAccount']:
         """
-        Account
+        Customer account information that is associated with this connection
         """
         return pulumi.get(self, "account")
 
     @property
     @pulumi.getter(name="additionalInfo")
     def additional_info(self) -> pulumi.Output[Optional[Sequence[Mapping[str, Any]]]]:
         """
-        Connection side additional information
+        Connection additional information
         """
         return pulumi.get(self, "additional_info")
 
     @property
     @pulumi.getter
     def bandwidth(self) -> pulumi.Output[int]:
         """
@@ -871,15 +866,15 @@
         """
         return pulumi.get(self, "change_log")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        User-provided service description
+        Customer-provided connection description
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def direction(self) -> pulumi.Output[str]:
         """
@@ -887,15 +882,15 @@
         """
         return pulumi.get(self, "direction")
 
     @property
     @pulumi.getter
     def href(self) -> pulumi.Output[str]:
         """
-        Unique Resource Identifier
+        Connection URI information
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter(name="isRemote")
     def is_remote(self) -> pulumi.Output[bool]:
         """
@@ -903,15 +898,15 @@
         """
         return pulumi.get(self, "is_remote")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Port name
+        Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def notifications(self) -> pulumi.Output[Sequence['outputs.ConnectionNotification']]:
         """
@@ -943,15 +938,15 @@
         """
         return pulumi.get(self, "project")
 
     @property
     @pulumi.getter
     def redundancy(self) -> pulumi.Output[Optional['outputs.ConnectionRedundancy']]:
         """
-        Redundancy Information
+        Connection Redundancy Configuration
         """
         return pulumi.get(self, "redundancy")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
@@ -959,23 +954,23 @@
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        Interface type
+        Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> pulumi.Output[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned connection identifier
         """
         return pulumi.get(self, "uuid")
 
     @property
     @pulumi.getter(name="zSide")
     def z_side(self) -> pulumi.Output['outputs.ConnectionZSide']:
         """
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_cloud_router.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_cloud_router.py`

 * *Files 18% similar despite different names*

```diff
@@ -278,22 +278,30 @@
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Cloud Router for a given UUID
 
     API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#fabric-cloud-routers
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     cloud_router_data_name = equinix.fabric.get_cloud_router(uuid="<uuid_of_cloud_router>")
+    pulumi.export("id", cloud_router_data_name.id)
+    pulumi.export("name", cloud_router_data_name.name)
+    pulumi.export("accountNumber", cloud_router_data_name.accounts[0].account_number)
+    pulumi.export("equinixAsn", cloud_router_data_name.equinix_asn)
+    pulumi.export("metroCode", cloud_router_data_name.locations[0].metro_code)
+    pulumi.export("metroName", cloud_router_data_name.locations[0].metro_name)
+    pulumi.export("region", cloud_router_data_name.locations[0].region)
+    pulumi.export("packageCode", cloud_router_data_name.packages[0].code)
+    pulumi.export("projectId", cloud_router_data_name.projects[0].project_id)
+    pulumi.export("type", cloud_router_data_name.type)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned Fabric Cloud Router identifier
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -328,20 +336,28 @@
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Cloud Router for a given UUID
 
     API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#fabric-cloud-routers
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     cloud_router_data_name = equinix.fabric.get_cloud_router(uuid="<uuid_of_cloud_router>")
+    pulumi.export("id", cloud_router_data_name.id)
+    pulumi.export("name", cloud_router_data_name.name)
+    pulumi.export("accountNumber", cloud_router_data_name.accounts[0].account_number)
+    pulumi.export("equinixAsn", cloud_router_data_name.equinix_asn)
+    pulumi.export("metroCode", cloud_router_data_name.locations[0].metro_code)
+    pulumi.export("metroName", cloud_router_data_name.locations[0].metro_name)
+    pulumi.export("region", cloud_router_data_name.locations[0].region)
+    pulumi.export("packageCode", cloud_router_data_name.packages[0].code)
+    pulumi.export("projectId", cloud_router_data_name.projects[0].project_id)
+    pulumi.export("type", cloud_router_data_name.type)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned Fabric Cloud Router identifier
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_connection.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_interconnection.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,331 +7,360 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'GetConnectionResult',
-    'AwaitableGetConnectionResult',
-    'get_connection',
-    'get_connection_output',
+    'GetInterconnectionResult',
+    'AwaitableGetInterconnectionResult',
+    'get_interconnection',
+    'get_interconnection_output',
 ]
 
 @pulumi.output_type
-class GetConnectionResult:
+class GetInterconnectionResult:
     """
-    A collection of values returned by getConnection.
+    A collection of values returned by getInterconnection.
     """
-    def __init__(__self__, a_side=None, account=None, additional_info=None, bandwidth=None, change_log=None, description=None, direction=None, href=None, id=None, is_remote=None, name=None, notifications=None, operation=None, order=None, project=None, redundancy=None, state=None, type=None, uuid=None, z_side=None):
-        if a_side and not isinstance(a_side, dict):
-            raise TypeError("Expected argument 'a_side' to be a dict")
-        pulumi.set(__self__, "a_side", a_side)
-        if account and not isinstance(account, dict):
-            raise TypeError("Expected argument 'account' to be a dict")
-        pulumi.set(__self__, "account", account)
-        if additional_info and not isinstance(additional_info, list):
-            raise TypeError("Expected argument 'additional_info' to be a list")
-        pulumi.set(__self__, "additional_info", additional_info)
-        if bandwidth and not isinstance(bandwidth, int):
-            raise TypeError("Expected argument 'bandwidth' to be a int")
-        pulumi.set(__self__, "bandwidth", bandwidth)
-        if change_log and not isinstance(change_log, dict):
-            raise TypeError("Expected argument 'change_log' to be a dict")
-        pulumi.set(__self__, "change_log", change_log)
+    def __init__(__self__, authorization_code=None, connection_id=None, contact_email=None, description=None, facility=None, id=None, metro=None, mode=None, name=None, organization_id=None, ports=None, project_id=None, redundancy=None, service_token_type=None, service_tokens=None, speed=None, status=None, tags=None, token=None, type=None, vlans=None, vrfs=None):
+        if authorization_code and not isinstance(authorization_code, str):
+            raise TypeError("Expected argument 'authorization_code' to be a str")
+        pulumi.set(__self__, "authorization_code", authorization_code)
+        if connection_id and not isinstance(connection_id, str):
+            raise TypeError("Expected argument 'connection_id' to be a str")
+        pulumi.set(__self__, "connection_id", connection_id)
+        if contact_email and not isinstance(contact_email, str):
+            raise TypeError("Expected argument 'contact_email' to be a str")
+        pulumi.set(__self__, "contact_email", contact_email)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
-        if direction and not isinstance(direction, str):
-            raise TypeError("Expected argument 'direction' to be a str")
-        pulumi.set(__self__, "direction", direction)
-        if href and not isinstance(href, str):
-            raise TypeError("Expected argument 'href' to be a str")
-        pulumi.set(__self__, "href", href)
+        if facility and not isinstance(facility, str):
+            raise TypeError("Expected argument 'facility' to be a str")
+        pulumi.set(__self__, "facility", facility)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if is_remote and not isinstance(is_remote, bool):
-            raise TypeError("Expected argument 'is_remote' to be a bool")
-        pulumi.set(__self__, "is_remote", is_remote)
+        if metro and not isinstance(metro, str):
+            raise TypeError("Expected argument 'metro' to be a str")
+        pulumi.set(__self__, "metro", metro)
+        if mode and not isinstance(mode, str):
+            raise TypeError("Expected argument 'mode' to be a str")
+        pulumi.set(__self__, "mode", mode)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if notifications and not isinstance(notifications, list):
-            raise TypeError("Expected argument 'notifications' to be a list")
-        pulumi.set(__self__, "notifications", notifications)
-        if operation and not isinstance(operation, dict):
-            raise TypeError("Expected argument 'operation' to be a dict")
-        pulumi.set(__self__, "operation", operation)
-        if order and not isinstance(order, dict):
-            raise TypeError("Expected argument 'order' to be a dict")
-        pulumi.set(__self__, "order", order)
-        if project and not isinstance(project, dict):
-            raise TypeError("Expected argument 'project' to be a dict")
-        pulumi.set(__self__, "project", project)
-        if redundancy and not isinstance(redundancy, dict):
-            raise TypeError("Expected argument 'redundancy' to be a dict")
+        if organization_id and not isinstance(organization_id, str):
+            raise TypeError("Expected argument 'organization_id' to be a str")
+        pulumi.set(__self__, "organization_id", organization_id)
+        if ports and not isinstance(ports, list):
+            raise TypeError("Expected argument 'ports' to be a list")
+        pulumi.set(__self__, "ports", ports)
+        if project_id and not isinstance(project_id, str):
+            raise TypeError("Expected argument 'project_id' to be a str")
+        pulumi.set(__self__, "project_id", project_id)
+        if redundancy and not isinstance(redundancy, str):
+            raise TypeError("Expected argument 'redundancy' to be a str")
         pulumi.set(__self__, "redundancy", redundancy)
-        if state and not isinstance(state, str):
-            raise TypeError("Expected argument 'state' to be a str")
-        pulumi.set(__self__, "state", state)
+        if service_token_type and not isinstance(service_token_type, str):
+            raise TypeError("Expected argument 'service_token_type' to be a str")
+        pulumi.set(__self__, "service_token_type", service_token_type)
+        if service_tokens and not isinstance(service_tokens, list):
+            raise TypeError("Expected argument 'service_tokens' to be a list")
+        pulumi.set(__self__, "service_tokens", service_tokens)
+        if speed and not isinstance(speed, str):
+            raise TypeError("Expected argument 'speed' to be a str")
+        pulumi.set(__self__, "speed", speed)
+        if status and not isinstance(status, str):
+            raise TypeError("Expected argument 'status' to be a str")
+        pulumi.set(__self__, "status", status)
+        if tags and not isinstance(tags, list):
+            raise TypeError("Expected argument 'tags' to be a list")
+        pulumi.set(__self__, "tags", tags)
+        if token and not isinstance(token, str):
+            raise TypeError("Expected argument 'token' to be a str")
+        pulumi.set(__self__, "token", token)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
-        if uuid and not isinstance(uuid, str):
-            raise TypeError("Expected argument 'uuid' to be a str")
-        pulumi.set(__self__, "uuid", uuid)
-        if z_side and not isinstance(z_side, dict):
-            raise TypeError("Expected argument 'z_side' to be a dict")
-        pulumi.set(__self__, "z_side", z_side)
+        if vlans and not isinstance(vlans, list):
+            raise TypeError("Expected argument 'vlans' to be a list")
+        pulumi.set(__self__, "vlans", vlans)
+        if vrfs and not isinstance(vrfs, list):
+            raise TypeError("Expected argument 'vrfs' to be a list")
+        pulumi.set(__self__, "vrfs", vrfs)
 
     @property
-    @pulumi.getter(name="aSide")
-    def a_side(self) -> 'outputs.GetConnectionASideResult':
+    @pulumi.getter(name="authorizationCode")
+    def authorization_code(self) -> str:
+        return pulumi.get(self, "authorization_code")
+
+    @property
+    @pulumi.getter(name="connectionId")
+    def connection_id(self) -> str:
+        return pulumi.get(self, "connection_id")
+
+    @property
+    @pulumi.getter(name="contactEmail")
+    def contact_email(self) -> str:
         """
-        Requester or Customer side connection configuration object of the multi-segment connection
+        The preferred email used for communication and notifications about the Equinix Fabric interconnection.
         """
-        return pulumi.get(self, "a_side")
+        return pulumi.get(self, "contact_email")
 
     @property
     @pulumi.getter
-    def account(self) -> 'outputs.GetConnectionAccountResult':
+    def description(self) -> str:
         """
-        Customer account information that is associated with this connection
+        Description of the connection resource.
         """
-        return pulumi.get(self, "account")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="additionalInfo")
-    def additional_info(self) -> Sequence[Mapping[str, Any]]:
+    @pulumi.getter
+    def facility(self) -> str:
         """
-        Connection additional information
+        (**Deprecated**) Slug of a facility to which the connection belongs. Use metro instead; read the facility to metro migration guide
         """
-        return pulumi.get(self, "additional_info")
+        warnings.warn("""Use metro instead of facility. For more information, read the migration guide.""", DeprecationWarning)
+        pulumi.log.warn("""facility is deprecated: Use metro instead of facility. For more information, read the migration guide.""")
+
+        return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
-    def bandwidth(self) -> int:
+    def id(self) -> str:
         """
-        Connection bandwidth in Mbps
+        Port UUID.
         """
-        return pulumi.get(self, "bandwidth")
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="changeLog")
-    def change_log(self) -> 'outputs.GetConnectionChangeLogResult':
+    @pulumi.getter
+    def metro(self) -> str:
         """
-        Captures connection lifecycle change information
+        Slug of a metro to which the connection belongs.
         """
-        return pulumi.get(self, "change_log")
+        return pulumi.get(self, "metro")
 
     @property
     @pulumi.getter
-    def description(self) -> str:
+    def mode(self) -> str:
         """
-        Customer-provided connection description
+        Mode for connections in IBX facilities with the dedicated type - standard or tunnel.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "mode")
 
     @property
     @pulumi.getter
-    def direction(self) -> str:
+    def name(self) -> str:
         """
-        Connection directionality from the requester point of view
+        Port name.
         """
-        return pulumi.get(self, "direction")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def href(self) -> str:
+    @pulumi.getter(name="organizationId")
+    def organization_id(self) -> str:
         """
-        Connection URI information
+        ID of the organization where the connection is scoped to.
         """
-        return pulumi.get(self, "href")
+        return pulumi.get(self, "organization_id")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def ports(self) -> Sequence['outputs.GetInterconnectionPortResult']:
         """
-        The provider-assigned unique ID for this managed resource.
+        List of connection ports - primary (`ports[0]`) and secondary (`ports[1]`)
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "ports")
 
     @property
-    @pulumi.getter(name="isRemote")
-    def is_remote(self) -> bool:
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> str:
         """
-        Connection property derived from access point locations
+        ID of project to which the connection belongs.
         """
-        return pulumi.get(self, "is_remote")
+        return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def redundancy(self) -> str:
         """
-        Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
+        Connection redundancy, reduntant or primary.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "redundancy")
 
     @property
-    @pulumi.getter
-    def notifications(self) -> Sequence['outputs.GetConnectionNotificationResult']:
+    @pulumi.getter(name="serviceTokenType")
+    def service_token_type(self) -> str:
         """
-        Preferences for notifications on connection configuration or status changes
+        Type of service token, a_side or z_side. One available in shared connection.
         """
-        return pulumi.get(self, "notifications")
+        return pulumi.get(self, "service_token_type")
 
     @property
-    @pulumi.getter
-    def operation(self) -> 'outputs.GetConnectionOperationResult':
+    @pulumi.getter(name="serviceTokens")
+    def service_tokens(self) -> Sequence['outputs.GetInterconnectionServiceTokenResult']:
         """
-        Connection type-specific operational data
+        List of connection service tokens with attributes
         """
-        return pulumi.get(self, "operation")
+        return pulumi.get(self, "service_tokens")
 
     @property
     @pulumi.getter
-    def order(self) -> 'outputs.GetConnectionOrderResult':
+    def speed(self) -> str:
         """
-        Order details
+        Port speed in bits per second.
         """
-        return pulumi.get(self, "order")
+        return pulumi.get(self, "speed")
 
     @property
     @pulumi.getter
-    def project(self) -> 'outputs.GetConnectionProjectResult':
+    def status(self) -> str:
         """
-        Project information
+        Port status.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
-    def redundancy(self) -> 'outputs.GetConnectionRedundancyResult':
+    def tags(self) -> Sequence[str]:
         """
-        Connection Redundancy Configuration
+        String list of tags.
         """
-        return pulumi.get(self, "redundancy")
+        return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
-    def state(self) -> str:
+    def token(self) -> str:
         """
-        Connection overall state
+        (Deprecated) Fabric Token required to configure the connection in Equinix Fabric with the equinix_ecx_l2_connection resource or from the [Equinix Fabric Portal](https://ecxfabric.equinix.com/dashboard). If your organization already has connection service tokens enabled, use `service_tokens` instead.
         """
-        return pulumi.get(self, "state")
+        warnings.warn("""If your organization already has connection service tokens enabled, use `service_tokens` instead""", DeprecationWarning)
+        pulumi.log.warn("""token is deprecated: If your organization already has connection service tokens enabled, use `service_tokens` instead""")
+
+        return pulumi.get(self, "token")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
+        Token type, `a_side` or `z_side`.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
-    def uuid(self) -> str:
+    def vlans(self) -> Sequence[int]:
         """
-        Equinix-assigned connection identifier
+        Attached VLANs. Only available in shared connection. One vlan for Primary/Single connection and two vlans for Redundant connection.
         """
-        return pulumi.get(self, "uuid")
+        return pulumi.get(self, "vlans")
 
     @property
-    @pulumi.getter(name="zSide")
-    def z_side(self) -> 'outputs.GetConnectionZSideResult':
-        """
-        Destination or Provider side connection configuration object of the multi-segment connection
-        """
-        return pulumi.get(self, "z_side")
+    @pulumi.getter
+    def vrfs(self) -> Sequence[str]:
+        return pulumi.get(self, "vrfs")
 
 
-class AwaitableGetConnectionResult(GetConnectionResult):
+class AwaitableGetInterconnectionResult(GetInterconnectionResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetConnectionResult(
-            a_side=self.a_side,
-            account=self.account,
-            additional_info=self.additional_info,
-            bandwidth=self.bandwidth,
-            change_log=self.change_log,
+        return GetInterconnectionResult(
+            authorization_code=self.authorization_code,
+            connection_id=self.connection_id,
+            contact_email=self.contact_email,
             description=self.description,
-            direction=self.direction,
-            href=self.href,
+            facility=self.facility,
             id=self.id,
-            is_remote=self.is_remote,
+            metro=self.metro,
+            mode=self.mode,
             name=self.name,
-            notifications=self.notifications,
-            operation=self.operation,
-            order=self.order,
-            project=self.project,
+            organization_id=self.organization_id,
+            ports=self.ports,
+            project_id=self.project_id,
             redundancy=self.redundancy,
-            state=self.state,
+            service_token_type=self.service_token_type,
+            service_tokens=self.service_tokens,
+            speed=self.speed,
+            status=self.status,
+            tags=self.tags,
+            token=self.token,
             type=self.type,
-            uuid=self.uuid,
-            z_side=self.z_side)
+            vlans=self.vlans,
+            vrfs=self.vrfs)
 
 
-def get_connection(uuid: Optional[str] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetConnectionResult:
+def get_interconnection(connection_id: Optional[str] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInterconnectionResult:
     """
-    Fabric V4 API compatible data resource that allow user to fetch connection for a given UUID
+    Use this data source to retrieve a [connection resource](https://metal.equinix.com/developers/docs/networking/fabric/)
+
+    > Equinix Metal connection with with Service Token A-side / Z-side (service_token_type) is not generally available and may not be enabled yet for your organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    connection_data_name = equinix.fabric.get_connection(uuid="<uuid_of_connection>")
+    example = equinix.metal.get_interconnection(connection_id="4347e805-eb46-4699-9eb9-5c116e6a017d")
     ```
-    <!--End PulumiCodeChooser -->
+
+
+    :param str connection_id: ID of the connection resource.
     """
     __args__ = dict()
-    __args__['uuid'] = uuid
+    __args__['connectionId'] = connection_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:fabric/getConnection:getConnection', __args__, opts=opts, typ=GetConnectionResult).value
+    __ret__ = pulumi.runtime.invoke('equinix:metal/getInterconnection:getInterconnection', __args__, opts=opts, typ=GetInterconnectionResult).value
 
-    return AwaitableGetConnectionResult(
-        a_side=pulumi.get(__ret__, 'a_side'),
-        account=pulumi.get(__ret__, 'account'),
-        additional_info=pulumi.get(__ret__, 'additional_info'),
-        bandwidth=pulumi.get(__ret__, 'bandwidth'),
-        change_log=pulumi.get(__ret__, 'change_log'),
+    return AwaitableGetInterconnectionResult(
+        authorization_code=pulumi.get(__ret__, 'authorization_code'),
+        connection_id=pulumi.get(__ret__, 'connection_id'),
+        contact_email=pulumi.get(__ret__, 'contact_email'),
         description=pulumi.get(__ret__, 'description'),
-        direction=pulumi.get(__ret__, 'direction'),
-        href=pulumi.get(__ret__, 'href'),
+        facility=pulumi.get(__ret__, 'facility'),
         id=pulumi.get(__ret__, 'id'),
-        is_remote=pulumi.get(__ret__, 'is_remote'),
+        metro=pulumi.get(__ret__, 'metro'),
+        mode=pulumi.get(__ret__, 'mode'),
         name=pulumi.get(__ret__, 'name'),
-        notifications=pulumi.get(__ret__, 'notifications'),
-        operation=pulumi.get(__ret__, 'operation'),
-        order=pulumi.get(__ret__, 'order'),
-        project=pulumi.get(__ret__, 'project'),
+        organization_id=pulumi.get(__ret__, 'organization_id'),
+        ports=pulumi.get(__ret__, 'ports'),
+        project_id=pulumi.get(__ret__, 'project_id'),
         redundancy=pulumi.get(__ret__, 'redundancy'),
-        state=pulumi.get(__ret__, 'state'),
+        service_token_type=pulumi.get(__ret__, 'service_token_type'),
+        service_tokens=pulumi.get(__ret__, 'service_tokens'),
+        speed=pulumi.get(__ret__, 'speed'),
+        status=pulumi.get(__ret__, 'status'),
+        tags=pulumi.get(__ret__, 'tags'),
+        token=pulumi.get(__ret__, 'token'),
         type=pulumi.get(__ret__, 'type'),
-        uuid=pulumi.get(__ret__, 'uuid'),
-        z_side=pulumi.get(__ret__, 'z_side'))
+        vlans=pulumi.get(__ret__, 'vlans'),
+        vrfs=pulumi.get(__ret__, 'vrfs'))
 
 
-@_utilities.lift_output_func(get_connection)
-def get_connection_output(uuid: Optional[pulumi.Input[str]] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetConnectionResult]:
+@_utilities.lift_output_func(get_interconnection)
+def get_interconnection_output(connection_id: Optional[pulumi.Input[str]] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInterconnectionResult]:
     """
-    Fabric V4 API compatible data resource that allow user to fetch connection for a given UUID
+    Use this data source to retrieve a [connection resource](https://metal.equinix.com/developers/docs/networking/fabric/)
+
+    > Equinix Metal connection with with Service Token A-side / Z-side (service_token_type) is not generally available and may not be enabled yet for your organization.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    connection_data_name = equinix.fabric.get_connection(uuid="<uuid_of_connection>")
+    example = equinix.metal.get_interconnection(connection_id="4347e805-eb46-4699-9eb9-5c116e6a017d")
     ```
-    <!--End PulumiCodeChooser -->
+
+
+    :param str connection_id: ID of the connection resource.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_network.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_network.py`

 * *Files 9% similar despite different names*

```diff
@@ -204,22 +204,28 @@
 def get_network(uuid: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Network for a given UUID
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     network_data_name = equinix.fabric.get_network(uuid="<uuid_of_network>")
+    pulumi.export("id", network_data_name.id)
+    pulumi.export("name", network_data_name.name)
+    pulumi.export("scope", network_data_name.scope)
+    pulumi.export("type", network_data_name.type)
+    pulumi.export("region", network_data_name.locations[0].region)
     ```
-    <!--End PulumiCodeChooser -->
+
+
+    :param str uuid: Equinix-assigned network identifier
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('equinix:fabric/getNetwork:getNetwork', __args__, opts=opts, typ=GetNetworkResult).value
 
     return AwaitableGetNetworkResult(
@@ -243,17 +249,23 @@
 def get_network_output(uuid: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Network for a given UUID
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     network_data_name = equinix.fabric.get_network(uuid="<uuid_of_network>")
+    pulumi.export("id", network_data_name.id)
+    pulumi.export("name", network_data_name.name)
+    pulumi.export("scope", network_data_name.scope)
+    pulumi.export("type", network_data_name.type)
+    pulumi.export("region", network_data_name.locations[0].region)
     ```
-    <!--End PulumiCodeChooser -->
+
+
+    :param str uuid: Equinix-assigned network identifier
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_port.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_port.py`

 * *Files 9% similar despite different names*

```diff
@@ -264,22 +264,34 @@
 def get_port(uuid: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPortResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch port by uuid
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     port_data_name = equinix.fabric.get_port(uuid="<uuid_of_port>")
+    pulumi.export("id", port_data_name.id)
+    pulumi.export("name", port_data_name.name)
+    pulumi.export("state", port_data_name.state)
+    pulumi.export("accountName", port_data_name.account.account_name)
+    pulumi.export("type", port_data_name.type)
+    pulumi.export("bandwidth", port_data_name.bandwidth)
+    pulumi.export("usedBandwidth", port_data_name.used_bandwidth)
+    pulumi.export("encapsulationType", port_data_name.encapsulation.type)
+    pulumi.export("ibx", port_data_name.location.ibx)
+    pulumi.export("metroCode", port_data_name.location.metro_code)
+    pulumi.export("metroName", port_data_name.location.metro_name)
+    pulumi.export("region", port_data_name.location.region)
+    pulumi.export("deviceRedundancyEnabled", port_data_name.device.redundancies[0].enabled)
+    pulumi.export("deviceRedundancyPriority", port_data_name.device.redundancies[0].priority)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned port identifier
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -311,20 +323,32 @@
 def get_port_output(uuid: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPortResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch port by uuid
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     port_data_name = equinix.fabric.get_port(uuid="<uuid_of_port>")
+    pulumi.export("id", port_data_name.id)
+    pulumi.export("name", port_data_name.name)
+    pulumi.export("state", port_data_name.state)
+    pulumi.export("accountName", port_data_name.account.account_name)
+    pulumi.export("type", port_data_name.type)
+    pulumi.export("bandwidth", port_data_name.bandwidth)
+    pulumi.export("usedBandwidth", port_data_name.used_bandwidth)
+    pulumi.export("encapsulationType", port_data_name.encapsulation.type)
+    pulumi.export("ibx", port_data_name.location.ibx)
+    pulumi.export("metroCode", port_data_name.location.metro_code)
+    pulumi.export("metroName", port_data_name.location.metro_name)
+    pulumi.export("region", port_data_name.location.region)
+    pulumi.export("deviceRedundancyEnabled", port_data_name.device.redundancies[0].enabled)
+    pulumi.export("deviceRedundancyPriority", port_data_name.device.redundancies[0].priority)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned port identifier
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_routing_protocol.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_virtual_circuit.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,336 +4,316 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
 
 __all__ = [
-    'GetRoutingProtocolResult',
-    'AwaitableGetRoutingProtocolResult',
-    'get_routing_protocol',
-    'get_routing_protocol_output',
+    'GetVirtualCircuitResult',
+    'AwaitableGetVirtualCircuitResult',
+    'get_virtual_circuit',
+    'get_virtual_circuit_output',
 ]
 
 @pulumi.output_type
-class GetRoutingProtocolResult:
+class GetVirtualCircuitResult:
     """
-    A collection of values returned by getRoutingProtocol.
+    A collection of values returned by getVirtualCircuit.
     """
-    def __init__(__self__, bfd=None, bgp_auth_key=None, bgp_ipv4=None, bgp_ipv6=None, change_logs=None, changes=None, connection_uuid=None, customer_asn=None, description=None, direct_ipv4=None, direct_ipv6=None, equinix_asn=None, href=None, id=None, name=None, operations=None, state=None, type=None, uuid=None):
-        if bfd and not isinstance(bfd, dict):
-            raise TypeError("Expected argument 'bfd' to be a dict")
-        pulumi.set(__self__, "bfd", bfd)
-        if bgp_auth_key and not isinstance(bgp_auth_key, str):
-            raise TypeError("Expected argument 'bgp_auth_key' to be a str")
-        pulumi.set(__self__, "bgp_auth_key", bgp_auth_key)
-        if bgp_ipv4 and not isinstance(bgp_ipv4, dict):
-            raise TypeError("Expected argument 'bgp_ipv4' to be a dict")
-        pulumi.set(__self__, "bgp_ipv4", bgp_ipv4)
-        if bgp_ipv6 and not isinstance(bgp_ipv6, dict):
-            raise TypeError("Expected argument 'bgp_ipv6' to be a dict")
-        pulumi.set(__self__, "bgp_ipv6", bgp_ipv6)
-        if change_logs and not isinstance(change_logs, list):
-            raise TypeError("Expected argument 'change_logs' to be a list")
-        pulumi.set(__self__, "change_logs", change_logs)
-        if changes and not isinstance(changes, list):
-            raise TypeError("Expected argument 'changes' to be a list")
-        pulumi.set(__self__, "changes", changes)
-        if connection_uuid and not isinstance(connection_uuid, str):
-            raise TypeError("Expected argument 'connection_uuid' to be a str")
-        pulumi.set(__self__, "connection_uuid", connection_uuid)
-        if customer_asn and not isinstance(customer_asn, int):
-            raise TypeError("Expected argument 'customer_asn' to be a int")
-        pulumi.set(__self__, "customer_asn", customer_asn)
+    def __init__(__self__, connection_id=None, customer_ip=None, description=None, id=None, md5=None, metal_ip=None, name=None, nni_vlan=None, nni_vnid=None, peer_asn=None, port_id=None, project_id=None, speed=None, status=None, subnet=None, tags=None, virtual_circuit_id=None, vlan_id=None, vnid=None, vrf_id=None):
+        if connection_id and not isinstance(connection_id, str):
+            raise TypeError("Expected argument 'connection_id' to be a str")
+        pulumi.set(__self__, "connection_id", connection_id)
+        if customer_ip and not isinstance(customer_ip, str):
+            raise TypeError("Expected argument 'customer_ip' to be a str")
+        pulumi.set(__self__, "customer_ip", customer_ip)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
-        if direct_ipv4 and not isinstance(direct_ipv4, dict):
-            raise TypeError("Expected argument 'direct_ipv4' to be a dict")
-        pulumi.set(__self__, "direct_ipv4", direct_ipv4)
-        if direct_ipv6 and not isinstance(direct_ipv6, dict):
-            raise TypeError("Expected argument 'direct_ipv6' to be a dict")
-        pulumi.set(__self__, "direct_ipv6", direct_ipv6)
-        if equinix_asn and not isinstance(equinix_asn, int):
-            raise TypeError("Expected argument 'equinix_asn' to be a int")
-        pulumi.set(__self__, "equinix_asn", equinix_asn)
-        if href and not isinstance(href, str):
-            raise TypeError("Expected argument 'href' to be a str")
-        pulumi.set(__self__, "href", href)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if md5 and not isinstance(md5, str):
+            raise TypeError("Expected argument 'md5' to be a str")
+        pulumi.set(__self__, "md5", md5)
+        if metal_ip and not isinstance(metal_ip, str):
+            raise TypeError("Expected argument 'metal_ip' to be a str")
+        pulumi.set(__self__, "metal_ip", metal_ip)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if operations and not isinstance(operations, list):
-            raise TypeError("Expected argument 'operations' to be a list")
-        pulumi.set(__self__, "operations", operations)
-        if state and not isinstance(state, str):
-            raise TypeError("Expected argument 'state' to be a str")
-        pulumi.set(__self__, "state", state)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
-        if uuid and not isinstance(uuid, str):
-            raise TypeError("Expected argument 'uuid' to be a str")
-        pulumi.set(__self__, "uuid", uuid)
+        if nni_vlan and not isinstance(nni_vlan, int):
+            raise TypeError("Expected argument 'nni_vlan' to be a int")
+        pulumi.set(__self__, "nni_vlan", nni_vlan)
+        if nni_vnid and not isinstance(nni_vnid, int):
+            raise TypeError("Expected argument 'nni_vnid' to be a int")
+        pulumi.set(__self__, "nni_vnid", nni_vnid)
+        if peer_asn and not isinstance(peer_asn, int):
+            raise TypeError("Expected argument 'peer_asn' to be a int")
+        pulumi.set(__self__, "peer_asn", peer_asn)
+        if port_id and not isinstance(port_id, str):
+            raise TypeError("Expected argument 'port_id' to be a str")
+        pulumi.set(__self__, "port_id", port_id)
+        if project_id and not isinstance(project_id, str):
+            raise TypeError("Expected argument 'project_id' to be a str")
+        pulumi.set(__self__, "project_id", project_id)
+        if speed and not isinstance(speed, str):
+            raise TypeError("Expected argument 'speed' to be a str")
+        pulumi.set(__self__, "speed", speed)
+        if status and not isinstance(status, str):
+            raise TypeError("Expected argument 'status' to be a str")
+        pulumi.set(__self__, "status", status)
+        if subnet and not isinstance(subnet, str):
+            raise TypeError("Expected argument 'subnet' to be a str")
+        pulumi.set(__self__, "subnet", subnet)
+        if tags and not isinstance(tags, list):
+            raise TypeError("Expected argument 'tags' to be a list")
+        pulumi.set(__self__, "tags", tags)
+        if virtual_circuit_id and not isinstance(virtual_circuit_id, str):
+            raise TypeError("Expected argument 'virtual_circuit_id' to be a str")
+        pulumi.set(__self__, "virtual_circuit_id", virtual_circuit_id)
+        if vlan_id and not isinstance(vlan_id, str):
+            raise TypeError("Expected argument 'vlan_id' to be a str")
+        pulumi.set(__self__, "vlan_id", vlan_id)
+        if vnid and not isinstance(vnid, int):
+            raise TypeError("Expected argument 'vnid' to be a int")
+        pulumi.set(__self__, "vnid", vnid)
+        if vrf_id and not isinstance(vrf_id, str):
+            raise TypeError("Expected argument 'vrf_id' to be a str")
+        pulumi.set(__self__, "vrf_id", vrf_id)
+
+    @property
+    @pulumi.getter(name="connectionId")
+    def connection_id(self) -> str:
+        """
+        UUID of Connection where the VC is scoped to.
+        """
+        return pulumi.get(self, "connection_id")
 
     @property
-    @pulumi.getter
-    def bfd(self) -> 'outputs.GetRoutingProtocolBfdResult':
+    @pulumi.getter(name="customerIp")
+    def customer_ip(self) -> str:
         """
-        Bidirectional Forwarding Detection
+        The Customer IP address which the CSR switch will peer with. Will default to the other usable IP in the subnet.
         """
-        return pulumi.get(self, "bfd")
+        return pulumi.get(self, "customer_ip")
 
     @property
-    @pulumi.getter(name="bgpAuthKey")
-    def bgp_auth_key(self) -> str:
+    @pulumi.getter
+    def description(self) -> str:
         """
-        BGP authorization key
+        Description for the Virtual Circuit resource.
         """
-        return pulumi.get(self, "bgp_auth_key")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="bgpIpv4")
-    def bgp_ipv4(self) -> 'outputs.GetRoutingProtocolBgpIpv4Result':
+    @pulumi.getter
+    def id(self) -> str:
         """
-        Routing Protocol BGP IPv4
+        The provider-assigned unique ID for this managed resource.
         """
-        return pulumi.get(self, "bgp_ipv4")
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="bgpIpv6")
-    def bgp_ipv6(self) -> 'outputs.GetRoutingProtocolBgpIpv6Result':
+    @pulumi.getter
+    def md5(self) -> str:
         """
-        Routing Protocol BGP IPv6
+        The password that can be set for the VRF BGP peer
         """
-        return pulumi.get(self, "bgp_ipv6")
+        return pulumi.get(self, "md5")
 
     @property
-    @pulumi.getter(name="changeLogs")
-    def change_logs(self) -> Sequence['outputs.GetRoutingProtocolChangeLogResult']:
+    @pulumi.getter(name="metalIp")
+    def metal_ip(self) -> str:
         """
-        Captures Routing Protocol lifecycle change information
+        The Metal IP address for the SVI (Switch Virtual Interface) of the VirtualCircuit. Will default to the first usable IP in the subnet.
         """
-        return pulumi.get(self, "change_logs")
+        return pulumi.get(self, "metal_ip")
 
     @property
     @pulumi.getter
-    def changes(self) -> Sequence['outputs.GetRoutingProtocolChangeResult']:
+    def name(self) -> str:
         """
-        Routing Protocol configuration Changes
+        Name of the virtual circuit resource.
         """
-        return pulumi.get(self, "changes")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="connectionUuid")
-    def connection_uuid(self) -> str:
-        """
-        Connection URI associated with Routing Protocol
-        """
-        return pulumi.get(self, "connection_uuid")
+    @pulumi.getter(name="nniVlan")
+    def nni_vlan(self) -> int:
+        return pulumi.get(self, "nni_vlan")
 
     @property
-    @pulumi.getter(name="customerAsn")
-    def customer_asn(self) -> int:
-        """
-        Customer-provided ASN
-        """
-        return pulumi.get(self, "customer_asn")
+    @pulumi.getter(name="nniVnid")
+    def nni_vnid(self) -> int:
+        return pulumi.get(self, "nni_vnid")
 
     @property
-    @pulumi.getter
-    def description(self) -> str:
+    @pulumi.getter(name="peerAsn")
+    def peer_asn(self) -> int:
         """
-        Customer-provided Fabric Routing Protocol description
+        The BGP ASN of the peer. The same ASN may be the used across several VCs, but it cannot be the same as the local_asn of the VRF.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "peer_asn")
 
     @property
-    @pulumi.getter(name="directIpv4")
-    def direct_ipv4(self) -> 'outputs.GetRoutingProtocolDirectIpv4Result':
+    @pulumi.getter(name="portId")
+    def port_id(self) -> str:
         """
-        Routing Protocol Direct IPv4
+        UUID of the Connection Port where the VC is scoped to.
         """
-        return pulumi.get(self, "direct_ipv4")
+        return pulumi.get(self, "port_id")
 
     @property
-    @pulumi.getter(name="directIpv6")
-    def direct_ipv6(self) -> 'outputs.GetRoutingProtocolDirectIpv6Result':
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> str:
         """
-        Routing Protocol Direct IPv6
+        ID of project to which the VC belongs.
         """
-        return pulumi.get(self, "direct_ipv6")
+        return pulumi.get(self, "project_id")
 
     @property
-    @pulumi.getter(name="equinixAsn")
-    def equinix_asn(self) -> int:
+    @pulumi.getter
+    def speed(self) -> str:
         """
-        Equinix ASN
+        Speed of the Virtual Circuit resource.
         """
-        return pulumi.get(self, "equinix_asn")
+        return pulumi.get(self, "speed")
 
     @property
     @pulumi.getter
-    def href(self) -> str:
+    def status(self) -> str:
         """
-        Routing Protocol URI information
+        Status of the virtal circuit.
         """
-        return pulumi.get(self, "href")
+        return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def subnet(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        A subnet from one of the IP
+        blocks associated with the VRF that we will help create an IP reservation for. Can only be either a /30 or /31.
+        * For a /31 block, it will only have two IP addresses, which will be used for
+        the metal_ip and customer_ip.
+        * For a /30 block, it will have four IP addresses, but the first and last IP addresses are not usable. We will default to the first usable IP address for the metal_ip.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "subnet")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def tags(self) -> Sequence[str]:
         """
-        Routing Protocol name. An alpha-numeric 24 characters string which can include only hyphens and underscores
+        Tags for the Virtual Circuit resource.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "tags")
 
     @property
-    @pulumi.getter
-    def operations(self) -> Sequence['outputs.GetRoutingProtocolOperationResult']:
-        """
-        Routing Protocol type-specific operational data
-        """
-        return pulumi.get(self, "operations")
+    @pulumi.getter(name="virtualCircuitId")
+    def virtual_circuit_id(self) -> str:
+        return pulumi.get(self, "virtual_circuit_id")
 
     @property
-    @pulumi.getter
-    def state(self) -> str:
-        """
-        Routing Protocol overall state
-        """
-        return pulumi.get(self, "state")
+    @pulumi.getter(name="vlanId")
+    def vlan_id(self) -> str:
+        return pulumi.get(self, "vlan_id")
 
     @property
     @pulumi.getter
-    def type(self) -> str:
+    def vnid(self) -> int:
         """
-        Defines the routing protocol type like BGP or DIRECT
+        , `nni_vlan`, `nni_nvid` - VLAN parameters, see the
+        [documentation for Equinix Fabric](https://metal.equinix.com/developers/docs/networking/fabric/).
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "vnid")
 
     @property
-    @pulumi.getter
-    def uuid(self) -> str:
+    @pulumi.getter(name="vrfId")
+    def vrf_id(self) -> str:
         """
-        Equinix-assigned routing protocol identifier
+        UUID of the VLAN to associate.
         """
-        return pulumi.get(self, "uuid")
+        return pulumi.get(self, "vrf_id")
 
 
-class AwaitableGetRoutingProtocolResult(GetRoutingProtocolResult):
+class AwaitableGetVirtualCircuitResult(GetVirtualCircuitResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetRoutingProtocolResult(
-            bfd=self.bfd,
-            bgp_auth_key=self.bgp_auth_key,
-            bgp_ipv4=self.bgp_ipv4,
-            bgp_ipv6=self.bgp_ipv6,
-            change_logs=self.change_logs,
-            changes=self.changes,
-            connection_uuid=self.connection_uuid,
-            customer_asn=self.customer_asn,
+        return GetVirtualCircuitResult(
+            connection_id=self.connection_id,
+            customer_ip=self.customer_ip,
             description=self.description,
-            direct_ipv4=self.direct_ipv4,
-            direct_ipv6=self.direct_ipv6,
-            equinix_asn=self.equinix_asn,
-            href=self.href,
             id=self.id,
+            md5=self.md5,
+            metal_ip=self.metal_ip,
             name=self.name,
-            operations=self.operations,
-            state=self.state,
-            type=self.type,
-            uuid=self.uuid)
+            nni_vlan=self.nni_vlan,
+            nni_vnid=self.nni_vnid,
+            peer_asn=self.peer_asn,
+            port_id=self.port_id,
+            project_id=self.project_id,
+            speed=self.speed,
+            status=self.status,
+            subnet=self.subnet,
+            tags=self.tags,
+            virtual_circuit_id=self.virtual_circuit_id,
+            vlan_id=self.vlan_id,
+            vnid=self.vnid,
+            vrf_id=self.vrf_id)
 
 
-def get_routing_protocol(connection_uuid: Optional[str] = None,
-                         uuid: Optional[str] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRoutingProtocolResult:
+def get_virtual_circuit(virtual_circuit_id: Optional[str] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVirtualCircuitResult:
     """
-    Fabric V4 API compatible data resource that allow user to fetch routing protocol for a given UUID
-
-    API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#routing-protocols
-
-    ## Example Usage
+    Use this data source to retrieve a virtual circuit resource from
+    [Equinix Fabric - software-defined interconnections](https://metal.equinix.com/developers/docs/networking/fabric/)
 
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_equinix as equinix
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
-    routing_protocol_data_name = equinix.fabric.get_routing_protocol(connection_uuid="<uuid_of_connection_routing_protocol_is_applied_to>",
-        uuid="<uuid_of_routing_protocol>")
-    ```
-    <!--End PulumiCodeChooser -->
 
-
-    :param str connection_uuid: Connection URI associated with Routing Protocol
+    :param str virtual_circuit_id: ID of the virtual circuit resource
     """
     __args__ = dict()
-    __args__['connectionUuid'] = connection_uuid
-    __args__['uuid'] = uuid
+    __args__['virtualCircuitId'] = virtual_circuit_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:fabric/getRoutingProtocol:getRoutingProtocol', __args__, opts=opts, typ=GetRoutingProtocolResult).value
+    __ret__ = pulumi.runtime.invoke('equinix:metal/getVirtualCircuit:getVirtualCircuit', __args__, opts=opts, typ=GetVirtualCircuitResult).value
 
-    return AwaitableGetRoutingProtocolResult(
-        bfd=pulumi.get(__ret__, 'bfd'),
-        bgp_auth_key=pulumi.get(__ret__, 'bgp_auth_key'),
-        bgp_ipv4=pulumi.get(__ret__, 'bgp_ipv4'),
-        bgp_ipv6=pulumi.get(__ret__, 'bgp_ipv6'),
-        change_logs=pulumi.get(__ret__, 'change_logs'),
-        changes=pulumi.get(__ret__, 'changes'),
-        connection_uuid=pulumi.get(__ret__, 'connection_uuid'),
-        customer_asn=pulumi.get(__ret__, 'customer_asn'),
+    return AwaitableGetVirtualCircuitResult(
+        connection_id=pulumi.get(__ret__, 'connection_id'),
+        customer_ip=pulumi.get(__ret__, 'customer_ip'),
         description=pulumi.get(__ret__, 'description'),
-        direct_ipv4=pulumi.get(__ret__, 'direct_ipv4'),
-        direct_ipv6=pulumi.get(__ret__, 'direct_ipv6'),
-        equinix_asn=pulumi.get(__ret__, 'equinix_asn'),
-        href=pulumi.get(__ret__, 'href'),
         id=pulumi.get(__ret__, 'id'),
+        md5=pulumi.get(__ret__, 'md5'),
+        metal_ip=pulumi.get(__ret__, 'metal_ip'),
         name=pulumi.get(__ret__, 'name'),
-        operations=pulumi.get(__ret__, 'operations'),
-        state=pulumi.get(__ret__, 'state'),
-        type=pulumi.get(__ret__, 'type'),
-        uuid=pulumi.get(__ret__, 'uuid'))
-
-
-@_utilities.lift_output_func(get_routing_protocol)
-def get_routing_protocol_output(connection_uuid: Optional[pulumi.Input[str]] = None,
-                                uuid: Optional[pulumi.Input[str]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoutingProtocolResult]:
+        nni_vlan=pulumi.get(__ret__, 'nni_vlan'),
+        nni_vnid=pulumi.get(__ret__, 'nni_vnid'),
+        peer_asn=pulumi.get(__ret__, 'peer_asn'),
+        port_id=pulumi.get(__ret__, 'port_id'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        speed=pulumi.get(__ret__, 'speed'),
+        status=pulumi.get(__ret__, 'status'),
+        subnet=pulumi.get(__ret__, 'subnet'),
+        tags=pulumi.get(__ret__, 'tags'),
+        virtual_circuit_id=pulumi.get(__ret__, 'virtual_circuit_id'),
+        vlan_id=pulumi.get(__ret__, 'vlan_id'),
+        vnid=pulumi.get(__ret__, 'vnid'),
+        vrf_id=pulumi.get(__ret__, 'vrf_id'))
+
+
+@_utilities.lift_output_func(get_virtual_circuit)
+def get_virtual_circuit_output(virtual_circuit_id: Optional[pulumi.Input[str]] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualCircuitResult]:
     """
-    Fabric V4 API compatible data resource that allow user to fetch routing protocol for a given UUID
-
-    API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#routing-protocols
-
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_equinix as equinix
+    Use this data source to retrieve a virtual circuit resource from
+    [Equinix Fabric - software-defined interconnections](https://metal.equinix.com/developers/docs/networking/fabric/)
 
-    routing_protocol_data_name = equinix.fabric.get_routing_protocol(connection_uuid="<uuid_of_connection_routing_protocol_is_applied_to>",
-        uuid="<uuid_of_routing_protocol>")
-    ```
-    <!--End PulumiCodeChooser -->
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
 
-    :param str connection_uuid: Connection URI associated with Routing Protocol
+    :param str virtual_circuit_id: ID of the virtual circuit resource
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_service_profile.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_precreated_ip_block.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,347 +4,282 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
 
 __all__ = [
-    'GetServiceProfileResult',
-    'AwaitableGetServiceProfileResult',
-    'get_service_profile',
-    'get_service_profile_output',
+    'GetPrecreatedIpBlockResult',
+    'AwaitableGetPrecreatedIpBlockResult',
+    'get_precreated_ip_block',
+    'get_precreated_ip_block_output',
 ]
 
 @pulumi.output_type
-class GetServiceProfileResult:
+class GetPrecreatedIpBlockResult:
     """
-    A collection of values returned by getServiceProfile.
+    A collection of values returned by getPrecreatedIpBlock.
     """
-    def __init__(__self__, access_point_type_configs=None, account=None, allowed_emails=None, change_log=None, custom_fields=None, description=None, href=None, id=None, marketing_info=None, metros=None, name=None, notifications=None, ports=None, project=None, self_profile=None, state=None, tags=None, type=None, uuid=None, virtual_devices=None, visibility=None):
-        if access_point_type_configs and not isinstance(access_point_type_configs, list):
-            raise TypeError("Expected argument 'access_point_type_configs' to be a list")
-        pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
-        if account and not isinstance(account, dict):
-            raise TypeError("Expected argument 'account' to be a dict")
-        pulumi.set(__self__, "account", account)
-        if allowed_emails and not isinstance(allowed_emails, list):
-            raise TypeError("Expected argument 'allowed_emails' to be a list")
-        pulumi.set(__self__, "allowed_emails", allowed_emails)
-        if change_log and not isinstance(change_log, dict):
-            raise TypeError("Expected argument 'change_log' to be a dict")
-        pulumi.set(__self__, "change_log", change_log)
-        if custom_fields and not isinstance(custom_fields, list):
-            raise TypeError("Expected argument 'custom_fields' to be a list")
-        pulumi.set(__self__, "custom_fields", custom_fields)
-        if description and not isinstance(description, str):
-            raise TypeError("Expected argument 'description' to be a str")
-        pulumi.set(__self__, "description", description)
-        if href and not isinstance(href, str):
-            raise TypeError("Expected argument 'href' to be a str")
-        pulumi.set(__self__, "href", href)
+    def __init__(__self__, address=None, address_family=None, cidr=None, cidr_notation=None, facility=None, gateway=None, global_=None, id=None, manageable=None, management=None, metro=None, netmask=None, network=None, project_id=None, public=None, quantity=None, type=None, vrf_id=None):
+        if address and not isinstance(address, str):
+            raise TypeError("Expected argument 'address' to be a str")
+        pulumi.set(__self__, "address", address)
+        if address_family and not isinstance(address_family, int):
+            raise TypeError("Expected argument 'address_family' to be a int")
+        pulumi.set(__self__, "address_family", address_family)
+        if cidr and not isinstance(cidr, int):
+            raise TypeError("Expected argument 'cidr' to be a int")
+        pulumi.set(__self__, "cidr", cidr)
+        if cidr_notation and not isinstance(cidr_notation, str):
+            raise TypeError("Expected argument 'cidr_notation' to be a str")
+        pulumi.set(__self__, "cidr_notation", cidr_notation)
+        if facility and not isinstance(facility, str):
+            raise TypeError("Expected argument 'facility' to be a str")
+        pulumi.set(__self__, "facility", facility)
+        if gateway and not isinstance(gateway, str):
+            raise TypeError("Expected argument 'gateway' to be a str")
+        pulumi.set(__self__, "gateway", gateway)
+        if global_ and not isinstance(global_, bool):
+            raise TypeError("Expected argument 'global_' to be a bool")
+        pulumi.set(__self__, "global_", global_)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if marketing_info and not isinstance(marketing_info, dict):
-            raise TypeError("Expected argument 'marketing_info' to be a dict")
-        pulumi.set(__self__, "marketing_info", marketing_info)
-        if metros and not isinstance(metros, list):
-            raise TypeError("Expected argument 'metros' to be a list")
-        pulumi.set(__self__, "metros", metros)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-        if notifications and not isinstance(notifications, list):
-            raise TypeError("Expected argument 'notifications' to be a list")
-        pulumi.set(__self__, "notifications", notifications)
-        if ports and not isinstance(ports, list):
-            raise TypeError("Expected argument 'ports' to be a list")
-        pulumi.set(__self__, "ports", ports)
-        if project and not isinstance(project, dict):
-            raise TypeError("Expected argument 'project' to be a dict")
-        pulumi.set(__self__, "project", project)
-        if self_profile and not isinstance(self_profile, bool):
-            raise TypeError("Expected argument 'self_profile' to be a bool")
-        pulumi.set(__self__, "self_profile", self_profile)
-        if state and not isinstance(state, str):
-            raise TypeError("Expected argument 'state' to be a str")
-        pulumi.set(__self__, "state", state)
-        if tags and not isinstance(tags, list):
-            raise TypeError("Expected argument 'tags' to be a list")
-        pulumi.set(__self__, "tags", tags)
+        if manageable and not isinstance(manageable, bool):
+            raise TypeError("Expected argument 'manageable' to be a bool")
+        pulumi.set(__self__, "manageable", manageable)
+        if management and not isinstance(management, bool):
+            raise TypeError("Expected argument 'management' to be a bool")
+        pulumi.set(__self__, "management", management)
+        if metro and not isinstance(metro, str):
+            raise TypeError("Expected argument 'metro' to be a str")
+        pulumi.set(__self__, "metro", metro)
+        if netmask and not isinstance(netmask, str):
+            raise TypeError("Expected argument 'netmask' to be a str")
+        pulumi.set(__self__, "netmask", netmask)
+        if network and not isinstance(network, str):
+            raise TypeError("Expected argument 'network' to be a str")
+        pulumi.set(__self__, "network", network)
+        if project_id and not isinstance(project_id, str):
+            raise TypeError("Expected argument 'project_id' to be a str")
+        pulumi.set(__self__, "project_id", project_id)
+        if public and not isinstance(public, bool):
+            raise TypeError("Expected argument 'public' to be a bool")
+        pulumi.set(__self__, "public", public)
+        if quantity and not isinstance(quantity, int):
+            raise TypeError("Expected argument 'quantity' to be a int")
+        pulumi.set(__self__, "quantity", quantity)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
-        if uuid and not isinstance(uuid, str):
-            raise TypeError("Expected argument 'uuid' to be a str")
-        pulumi.set(__self__, "uuid", uuid)
-        if virtual_devices and not isinstance(virtual_devices, list):
-            raise TypeError("Expected argument 'virtual_devices' to be a list")
-        pulumi.set(__self__, "virtual_devices", virtual_devices)
-        if visibility and not isinstance(visibility, str):
-            raise TypeError("Expected argument 'visibility' to be a str")
-        pulumi.set(__self__, "visibility", visibility)
-
-    @property
-    @pulumi.getter(name="accessPointTypeConfigs")
-    def access_point_type_configs(self) -> Sequence['outputs.GetServiceProfileAccessPointTypeConfigResult']:
-        """
-        Access point config information
-        """
-        return pulumi.get(self, "access_point_type_configs")
+        if vrf_id and not isinstance(vrf_id, str):
+            raise TypeError("Expected argument 'vrf_id' to be a str")
+        pulumi.set(__self__, "vrf_id", vrf_id)
 
     @property
     @pulumi.getter
-    def account(self) -> 'outputs.GetServiceProfileAccountResult':
-        """
-        Service Profile Owner Account Information
-        """
-        return pulumi.get(self, "account")
+    def address(self) -> str:
+        return pulumi.get(self, "address")
 
     @property
-    @pulumi.getter(name="allowedEmails")
-    def allowed_emails(self) -> Sequence[str]:
-        """
-        Array of contact emails
-        """
-        return pulumi.get(self, "allowed_emails")
+    @pulumi.getter(name="addressFamily")
+    def address_family(self) -> int:
+        return pulumi.get(self, "address_family")
 
     @property
-    @pulumi.getter(name="changeLog")
-    def change_log(self) -> 'outputs.GetServiceProfileChangeLogResult':
-        """
-        Captures connection lifecycle change information
-        """
-        return pulumi.get(self, "change_log")
+    @pulumi.getter
+    def cidr(self) -> int:
+        return pulumi.get(self, "cidr")
 
     @property
-    @pulumi.getter(name="customFields")
-    def custom_fields(self) -> Sequence['outputs.GetServiceProfileCustomFieldResult']:
+    @pulumi.getter(name="cidrNotation")
+    def cidr_notation(self) -> str:
         """
-        Custom Fields
+        CIDR notation of the looked up block.
         """
-        return pulumi.get(self, "custom_fields")
+        return pulumi.get(self, "cidr_notation")
 
     @property
     @pulumi.getter
-    def description(self) -> str:
-        """
-        User-provided service description
-        """
-        return pulumi.get(self, "description")
+    def facility(self) -> Optional[str]:
+        return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
-    def href(self) -> str:
-        """
-        Service Profile URI response attribute
-        """
-        return pulumi.get(self, "href")
+    def gateway(self) -> str:
+        return pulumi.get(self, "gateway")
+
+    @property
+    @pulumi.getter(name="global")
+    def global_(self) -> Optional[bool]:
+        return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="marketingInfo")
-    def marketing_info(self) -> 'outputs.GetServiceProfileMarketingInfoResult':
-        """
-        Marketing Info
-        """
-        return pulumi.get(self, "marketing_info")
-
-    @property
     @pulumi.getter
-    def metros(self) -> Sequence['outputs.GetServiceProfileMetroResult']:
-        """
-        Access point config information
-        """
-        return pulumi.get(self, "metros")
+    def manageable(self) -> bool:
+        return pulumi.get(self, "manageable")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
-        """
-        Customer-assigned service profile name
-        """
-        return pulumi.get(self, "name")
+    def management(self) -> bool:
+        return pulumi.get(self, "management")
 
     @property
     @pulumi.getter
-    def notifications(self) -> Sequence['outputs.GetServiceProfileNotificationResult']:
-        """
-        Preferences for notifications on connection configuration or status changes
-        """
-        return pulumi.get(self, "notifications")
+    def metro(self) -> Optional[str]:
+        return pulumi.get(self, "metro")
 
     @property
     @pulumi.getter
-    def ports(self) -> Sequence['outputs.GetServiceProfilePortResult']:
-        """
-        Ports
-        """
-        return pulumi.get(self, "ports")
+    def netmask(self) -> str:
+        return pulumi.get(self, "netmask")
 
     @property
     @pulumi.getter
-    def project(self) -> 'outputs.GetServiceProfileProjectResult':
-        """
-        Project information
-        """
-        return pulumi.get(self, "project")
+    def network(self) -> str:
+        return pulumi.get(self, "network")
 
     @property
-    @pulumi.getter(name="selfProfile")
-    def self_profile(self) -> bool:
-        """
-        Self Profile indicating if the profile is created for customer's  self use
-        """
-        return pulumi.get(self, "self_profile")
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> str:
+        return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
-    def state(self) -> str:
-        """
-        Service profile state - ACTIVE, PENDING_APPROVAL, DELETED, REJECTED
-        """
-        return pulumi.get(self, "state")
+    def public(self) -> bool:
+        return pulumi.get(self, "public")
 
     @property
     @pulumi.getter
-    def tags(self) -> Sequence[str]:
-        """
-        Tags attached to the connection
-        """
-        return pulumi.get(self, "tags")
+    def quantity(self) -> int:
+        return pulumi.get(self, "quantity")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
-        """
         return pulumi.get(self, "type")
 
     @property
-    @pulumi.getter
-    def uuid(self) -> str:
-        """
-        Equinix assigned service profile identifier
-        """
-        return pulumi.get(self, "uuid")
-
-    @property
-    @pulumi.getter(name="virtualDevices")
-    def virtual_devices(self) -> Sequence['outputs.GetServiceProfileVirtualDeviceResult']:
-        """
-        Virtual Devices
-        """
-        return pulumi.get(self, "virtual_devices")
-
-    @property
-    @pulumi.getter
-    def visibility(self) -> str:
-        """
-        Service profile visibility - PUBLIC, PRIVATE
-        """
-        return pulumi.get(self, "visibility")
+    @pulumi.getter(name="vrfId")
+    def vrf_id(self) -> str:
+        return pulumi.get(self, "vrf_id")
 
 
-class AwaitableGetServiceProfileResult(GetServiceProfileResult):
+class AwaitableGetPrecreatedIpBlockResult(GetPrecreatedIpBlockResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetServiceProfileResult(
-            access_point_type_configs=self.access_point_type_configs,
-            account=self.account,
-            allowed_emails=self.allowed_emails,
-            change_log=self.change_log,
-            custom_fields=self.custom_fields,
-            description=self.description,
-            href=self.href,
+        return GetPrecreatedIpBlockResult(
+            address=self.address,
+            address_family=self.address_family,
+            cidr=self.cidr,
+            cidr_notation=self.cidr_notation,
+            facility=self.facility,
+            gateway=self.gateway,
+            global_=self.global_,
             id=self.id,
-            marketing_info=self.marketing_info,
-            metros=self.metros,
-            name=self.name,
-            notifications=self.notifications,
-            ports=self.ports,
-            project=self.project,
-            self_profile=self.self_profile,
-            state=self.state,
-            tags=self.tags,
+            manageable=self.manageable,
+            management=self.management,
+            metro=self.metro,
+            netmask=self.netmask,
+            network=self.network,
+            project_id=self.project_id,
+            public=self.public,
+            quantity=self.quantity,
             type=self.type,
-            uuid=self.uuid,
-            virtual_devices=self.virtual_devices,
-            visibility=self.visibility)
+            vrf_id=self.vrf_id)
 
 
-def get_service_profile(uuid: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceProfileResult:
+def get_precreated_ip_block(address_family: Optional[int] = None,
+                            facility: Optional[str] = None,
+                            global_: Optional[bool] = None,
+                            metro: Optional[str] = None,
+                            project_id: Optional[str] = None,
+                            public: Optional[bool] = None,
+                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrecreatedIpBlockResult:
     """
-    Fabric V4 API compatible data resource that allow user to fetch Service Profile by UUID filter criteria
+    Use this data source to get CIDR expression for precreated (management) IPv6 and IPv4 blocks in Equinix Metal.
+    You can then use the cidrsubnet TF builtin function to derive subnets.
+
+    > For backward compatibility, this data source will also return reserved (elastic) IP blocks.
+
+    > Precreated (management) IP blocks for a metro will not be available until first device is created in that metro.
+
+    > Public IPv4 blocks auto-assigned (management) to a device cannot be retrieved. If you need that information, consider using the metal.Device data source instead.
 
-    ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_equinix as equinix
-
-    service_profile_data_name = equinix.fabric.get_service_profile(uuid="<uuid_of_service_profile>")
-    ```
-    <!--End PulumiCodeChooser -->
+    :param int address_family: 4 or 6, depending on which block you are looking for.
+    :param str facility: Facility of the searched block. (for non-global blocks). Use metro instead; read the facility to metro migration guide
+    :param bool global_: Whether to look for global block. Default is false for backward compatibility.
+    :param str metro: Metro of the searched block (for non-global blocks).
+    :param str project_id: ID of the project where the searched block should be.
+    :param bool public: Whether to look for public or private block.
     """
     __args__ = dict()
-    __args__['uuid'] = uuid
+    __args__['addressFamily'] = address_family
+    __args__['facility'] = facility
+    __args__['global'] = global_
+    __args__['metro'] = metro
+    __args__['projectId'] = project_id
+    __args__['public'] = public
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:fabric/getServiceProfile:getServiceProfile', __args__, opts=opts, typ=GetServiceProfileResult).value
+    __ret__ = pulumi.runtime.invoke('equinix:metal/getPrecreatedIpBlock:getPrecreatedIpBlock', __args__, opts=opts, typ=GetPrecreatedIpBlockResult).value
 
-    return AwaitableGetServiceProfileResult(
-        access_point_type_configs=pulumi.get(__ret__, 'access_point_type_configs'),
-        account=pulumi.get(__ret__, 'account'),
-        allowed_emails=pulumi.get(__ret__, 'allowed_emails'),
-        change_log=pulumi.get(__ret__, 'change_log'),
-        custom_fields=pulumi.get(__ret__, 'custom_fields'),
-        description=pulumi.get(__ret__, 'description'),
-        href=pulumi.get(__ret__, 'href'),
+    return AwaitableGetPrecreatedIpBlockResult(
+        address=pulumi.get(__ret__, 'address'),
+        address_family=pulumi.get(__ret__, 'address_family'),
+        cidr=pulumi.get(__ret__, 'cidr'),
+        cidr_notation=pulumi.get(__ret__, 'cidr_notation'),
+        facility=pulumi.get(__ret__, 'facility'),
+        gateway=pulumi.get(__ret__, 'gateway'),
+        global_=pulumi.get(__ret__, 'global_'),
         id=pulumi.get(__ret__, 'id'),
-        marketing_info=pulumi.get(__ret__, 'marketing_info'),
-        metros=pulumi.get(__ret__, 'metros'),
-        name=pulumi.get(__ret__, 'name'),
-        notifications=pulumi.get(__ret__, 'notifications'),
-        ports=pulumi.get(__ret__, 'ports'),
-        project=pulumi.get(__ret__, 'project'),
-        self_profile=pulumi.get(__ret__, 'self_profile'),
-        state=pulumi.get(__ret__, 'state'),
-        tags=pulumi.get(__ret__, 'tags'),
+        manageable=pulumi.get(__ret__, 'manageable'),
+        management=pulumi.get(__ret__, 'management'),
+        metro=pulumi.get(__ret__, 'metro'),
+        netmask=pulumi.get(__ret__, 'netmask'),
+        network=pulumi.get(__ret__, 'network'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        public=pulumi.get(__ret__, 'public'),
+        quantity=pulumi.get(__ret__, 'quantity'),
         type=pulumi.get(__ret__, 'type'),
-        uuid=pulumi.get(__ret__, 'uuid'),
-        virtual_devices=pulumi.get(__ret__, 'virtual_devices'),
-        visibility=pulumi.get(__ret__, 'visibility'))
+        vrf_id=pulumi.get(__ret__, 'vrf_id'))
 
 
-@_utilities.lift_output_func(get_service_profile)
-def get_service_profile_output(uuid: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceProfileResult]:
+@_utilities.lift_output_func(get_precreated_ip_block)
+def get_precreated_ip_block_output(address_family: Optional[pulumi.Input[int]] = None,
+                                   facility: Optional[pulumi.Input[Optional[str]]] = None,
+                                   global_: Optional[pulumi.Input[Optional[bool]]] = None,
+                                   metro: Optional[pulumi.Input[Optional[str]]] = None,
+                                   project_id: Optional[pulumi.Input[str]] = None,
+                                   public: Optional[pulumi.Input[bool]] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrecreatedIpBlockResult]:
     """
-    Fabric V4 API compatible data resource that allow user to fetch Service Profile by UUID filter criteria
+    Use this data source to get CIDR expression for precreated (management) IPv6 and IPv4 blocks in Equinix Metal.
+    You can then use the cidrsubnet TF builtin function to derive subnets.
+
+    > For backward compatibility, this data source will also return reserved (elastic) IP blocks.
+
+    > Precreated (management) IP blocks for a metro will not be available until first device is created in that metro.
+
+    > Public IPv4 blocks auto-assigned (management) to a device cannot be retrieved. If you need that information, consider using the metal.Device data source instead.
 
-    ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_equinix as equinix
-
-    service_profile_data_name = equinix.fabric.get_service_profile(uuid="<uuid_of_service_profile>")
-    ```
-    <!--End PulumiCodeChooser -->
+    :param int address_family: 4 or 6, depending on which block you are looking for.
+    :param str facility: Facility of the searched block. (for non-global blocks). Use metro instead; read the facility to metro migration guide
+    :param bool global_: Whether to look for global block. Default is false for backward compatibility.
+    :param str metro: Metro of the searched block (for non-global blocks).
+    :param str project_id: ID of the project where the searched block should be.
+    :param bool public: Whether to look for public or private block.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/get_service_profiles.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_facility.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,160 +8,173 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._inputs import *
 
 __all__ = [
-    'GetServiceProfilesResult',
-    'AwaitableGetServiceProfilesResult',
-    'get_service_profiles',
-    'get_service_profiles_output',
+    'GetFacilityResult',
+    'AwaitableGetFacilityResult',
+    'get_facility',
+    'get_facility_output',
 ]
 
 @pulumi.output_type
-class GetServiceProfilesResult:
+class GetFacilityResult:
     """
-    A collection of values returned by getServiceProfiles.
+    A collection of values returned by getFacility.
     """
-    def __init__(__self__, data=None, filter=None, id=None, sort=None, view_point=None):
-        if data and not isinstance(data, list):
-            raise TypeError("Expected argument 'data' to be a list")
-        pulumi.set(__self__, "data", data)
-        if filter and not isinstance(filter, dict):
-            raise TypeError("Expected argument 'filter' to be a dict")
-        pulumi.set(__self__, "filter", filter)
+    def __init__(__self__, capacities=None, code=None, features=None, features_requireds=None, id=None, metro=None, name=None):
+        if capacities and not isinstance(capacities, list):
+            raise TypeError("Expected argument 'capacities' to be a list")
+        pulumi.set(__self__, "capacities", capacities)
+        if code and not isinstance(code, str):
+            raise TypeError("Expected argument 'code' to be a str")
+        pulumi.set(__self__, "code", code)
+        if features and not isinstance(features, list):
+            raise TypeError("Expected argument 'features' to be a list")
+        pulumi.set(__self__, "features", features)
+        if features_requireds and not isinstance(features_requireds, list):
+            raise TypeError("Expected argument 'features_requireds' to be a list")
+        pulumi.set(__self__, "features_requireds", features_requireds)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if sort and not isinstance(sort, list):
-            raise TypeError("Expected argument 'sort' to be a list")
-        pulumi.set(__self__, "sort", sort)
-        if view_point and not isinstance(view_point, str):
-            raise TypeError("Expected argument 'view_point' to be a str")
-        pulumi.set(__self__, "view_point", view_point)
+        if metro and not isinstance(metro, str):
+            raise TypeError("Expected argument 'metro' to be a str")
+        pulumi.set(__self__, "metro", metro)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
-    def data(self) -> Sequence['outputs.GetServiceProfilesDatumResult']:
-        """
-        List of Service Profiles
-        """
-        return pulumi.get(self, "data")
+    def capacities(self) -> Optional[Sequence['outputs.GetFacilityCapacityResult']]:
+        return pulumi.get(self, "capacities")
+
+    @property
+    @pulumi.getter
+    def code(self) -> str:
+        return pulumi.get(self, "code")
 
     @property
     @pulumi.getter
-    def filter(self) -> Optional['outputs.GetServiceProfilesFilterResult']:
+    def features(self) -> Sequence[str]:
         """
-        Service Profile Search Filter
+        The features of the facility.
         """
-        return pulumi.get(self, "filter")
+        return pulumi.get(self, "features")
+
+    @property
+    @pulumi.getter(name="featuresRequireds")
+    def features_requireds(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "features_requireds")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def sort(self) -> Optional[Sequence['outputs.GetServiceProfilesSortResult']]:
+    def metro(self) -> str:
         """
-        Service Profile Sort criteria for Search Request response payload
+        The metro code the facility is part of.
         """
-        return pulumi.get(self, "sort")
+        return pulumi.get(self, "metro")
 
     @property
-    @pulumi.getter(name="viewPoint")
-    def view_point(self) -> Optional[str]:
+    @pulumi.getter
+    def name(self) -> str:
         """
-        flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
+        The name of the facility.
         """
-        return pulumi.get(self, "view_point")
+        return pulumi.get(self, "name")
 
 
-class AwaitableGetServiceProfilesResult(GetServiceProfilesResult):
+class AwaitableGetFacilityResult(GetFacilityResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetServiceProfilesResult(
-            data=self.data,
-            filter=self.filter,
+        return GetFacilityResult(
+            capacities=self.capacities,
+            code=self.code,
+            features=self.features,
+            features_requireds=self.features_requireds,
             id=self.id,
-            sort=self.sort,
-            view_point=self.view_point)
+            metro=self.metro,
+            name=self.name)
 
 
-def get_service_profiles(filter: Optional[pulumi.InputType['GetServiceProfilesFilterArgs']] = None,
-                         sort: Optional[Sequence[pulumi.InputType['GetServiceProfilesSortArgs']]] = None,
-                         view_point: Optional[str] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceProfilesResult:
+def get_facility(capacities: Optional[Sequence[pulumi.InputType['GetFacilityCapacityArgs']]] = None,
+                 code: Optional[str] = None,
+                 features_requireds: Optional[Sequence[str]] = None,
+                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFacilityResult:
     """
-    Fabric V4 API compatible data resource that allow user to fetch Service Profile by name filter criteria
+    > **Deprecated** Use `metal_get_metro` instead.  For more information, refer to the facility to metro migration guide.
+
+    Provides an Equinix Metal facility datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    service_profiles_data_name = equinix.fabric.get_service_profiles(filter=equinix.fabric.GetServiceProfilesFilterArgs(
-        operator="=",
-        property="/name",
-        values=["<list_of_profiles_to_return>"],
-    ))
+    ny5 = equinix.metal.get_facility(code="ny5")
+    pulumi.export("id", ny5.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param pulumi.InputType['GetServiceProfilesFilterArgs'] filter: Service Profile Search Filter
-    :param Sequence[pulumi.InputType['GetServiceProfilesSortArgs']] sort: Service Profile Sort criteria for Search Request response payload
-    :param str view_point: flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
+    :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
+    :param str code: The facility code to search for facilities.
+    :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
+           possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
     """
     __args__ = dict()
-    __args__['filter'] = filter
-    __args__['sort'] = sort
-    __args__['viewPoint'] = view_point
+    __args__['capacities'] = capacities
+    __args__['code'] = code
+    __args__['featuresRequireds'] = features_requireds
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:fabric/getServiceProfiles:getServiceProfiles', __args__, opts=opts, typ=GetServiceProfilesResult).value
+    __ret__ = pulumi.runtime.invoke('equinix:metal/getFacility:getFacility', __args__, opts=opts, typ=GetFacilityResult).value
 
-    return AwaitableGetServiceProfilesResult(
-        data=pulumi.get(__ret__, 'data'),
-        filter=pulumi.get(__ret__, 'filter'),
+    return AwaitableGetFacilityResult(
+        capacities=pulumi.get(__ret__, 'capacities'),
+        code=pulumi.get(__ret__, 'code'),
+        features=pulumi.get(__ret__, 'features'),
+        features_requireds=pulumi.get(__ret__, 'features_requireds'),
         id=pulumi.get(__ret__, 'id'),
-        sort=pulumi.get(__ret__, 'sort'),
-        view_point=pulumi.get(__ret__, 'view_point'))
+        metro=pulumi.get(__ret__, 'metro'),
+        name=pulumi.get(__ret__, 'name'))
 
 
-@_utilities.lift_output_func(get_service_profiles)
-def get_service_profiles_output(filter: Optional[pulumi.Input[Optional[pulumi.InputType['GetServiceProfilesFilterArgs']]]] = None,
-                                sort: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetServiceProfilesSortArgs']]]]] = None,
-                                view_point: Optional[pulumi.Input[Optional[str]]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceProfilesResult]:
+@_utilities.lift_output_func(get_facility)
+def get_facility_output(capacities: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetFacilityCapacityArgs']]]]] = None,
+                        code: Optional[pulumi.Input[str]] = None,
+                        features_requireds: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFacilityResult]:
     """
-    Fabric V4 API compatible data resource that allow user to fetch Service Profile by name filter criteria
+    > **Deprecated** Use `metal_get_metro` instead.  For more information, refer to the facility to metro migration guide.
+
+    Provides an Equinix Metal facility datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    service_profiles_data_name = equinix.fabric.get_service_profiles(filter=equinix.fabric.GetServiceProfilesFilterArgs(
-        operator="=",
-        property="/name",
-        values=["<list_of_profiles_to_return>"],
-    ))
+    ny5 = equinix.metal.get_facility(code="ny5")
+    pulumi.export("id", ny5.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param pulumi.InputType['GetServiceProfilesFilterArgs'] filter: Service Profile Search Filter
-    :param Sequence[pulumi.InputType['GetServiceProfilesSortArgs']] sort: Service Profile Sort criteria for Search Request response payload
-    :param str view_point: flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
+    :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
+    :param str code: The facility code to search for facilities.
+    :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
+           possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/network.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,14 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Fabric V4 API compatible resource allows creation and management of Equinix Fabric Network
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         new_network = equinix.fabric.Network("newNetwork",
             notifications=[equinix.fabric.NetworkNotificationArgs(
                 emails=[
@@ -361,15 +360,14 @@
             )],
             project=equinix.fabric.NetworkProjectArgs(
                 project_id="776847000642406",
             ),
             scope="GLOBAL",
             type="EVPLAN")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['NetworkLocationArgs']] location: Fabric Network location
         :param pulumi.Input[str] name: Fabric Network name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkNotificationArgs']]]] notifications: Preferences for notifications on Fabric Network configuration or status changes
         :param pulumi.Input[pulumi.InputType['NetworkProjectArgs']] project: Fabric Network project
@@ -383,15 +381,14 @@
                  args: NetworkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Fabric V4 API compatible resource allows creation and management of Equinix Fabric Network
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         new_network = equinix.fabric.Network("newNetwork",
             notifications=[equinix.fabric.NetworkNotificationArgs(
                 emails=[
@@ -402,15 +399,14 @@
             )],
             project=equinix.fabric.NetworkProjectArgs(
                 project_id="776847000642406",
             ),
             scope="GLOBAL",
             type="EVPLAN")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param NetworkArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/outputs.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -833,15 +833,15 @@
         :param 'ConnectionASideAccessPointNetworkArgs' network: network access point information
         :param Union[str, 'AccessPointPeeringType'] peering_type: Peering Type- PRIVATE,MICROSOFT,PUBLIC, MANUAL
         :param 'ConnectionASideAccessPointPortArgs' port: Port access point information
         :param 'ConnectionASideAccessPointProfileArgs' profile: Service Profile
         :param str provider_connection_id: Provider assigned Connection Id
         :param 'ConnectionASideAccessPointRouterArgs' router: Cloud Router access point information that replaces `gateway`
         :param str seller_region: Access point seller region
-        :param Union[str, 'AccessPointType'] type: Interface type
+        :param Union[str, 'AccessPointType'] type: Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         :param 'ConnectionASideAccessPointVirtualDeviceArgs' virtual_device: Virtual device
         """
         if account is not None:
             pulumi.set(__self__, "account", account)
         if authentication_key is not None:
             pulumi.set(__self__, "authentication_key", authentication_key)
         if gateway is not None:
@@ -978,15 +978,15 @@
         """
         return pulumi.get(self, "seller_region")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="virtualDevice")
     def virtual_device(self) -> Optional['outputs.ConnectionASideAccessPointVirtualDevice']:
         """
@@ -1165,15 +1165,15 @@
     def __init__(__self__, *,
                  id: Optional[int] = None,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
         :param int id: id
         :param str type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str uuid: Equinix-assigned interface identifier
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
@@ -1194,15 +1194,15 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned interface identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionASideAccessPointLinkProtocol(dict):
     @staticmethod
@@ -1228,15 +1228,15 @@
 
     def __init__(__self__, *,
                  type: Optional[str] = None,
                  vlan_c_tag: Optional[int] = None,
                  vlan_s_tag: Optional[int] = None,
                  vlan_tag: Optional[int] = None):
         """
-        :param Union[str, 'AccessPointLinkProtocolType'] type: Interface type
+        :param Union[str, 'AccessPointLinkProtocolType'] type: Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         :param int vlan_c_tag: Vlan Customer Tag information, vlanCTag value specified for QINQ connections
         :param int vlan_s_tag: Vlan Provider Tag information, vlanSTag value specified for QINQ connections
         :param int vlan_tag: Vlan Tag information, vlanTag value specified for DOT1Q connections
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if vlan_c_tag is not None:
@@ -1246,15 +1246,15 @@
         if vlan_tag is not None:
             pulumi.set(__self__, "vlan_tag", vlan_tag)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="vlanCTag")
     def vlan_c_tag(self) -> Optional[int]:
         """
@@ -1356,15 +1356,15 @@
 @pulumi.output_type
 class ConnectionASideAccessPointNetwork(dict):
     def __init__(__self__, *,
                  href: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str uuid: Equinix-assigned Network identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
@@ -1375,15 +1375,15 @@
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Network identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionASideAccessPointPort(dict):
     def __init__(__self__, *,
@@ -1391,15 +1391,15 @@
                  name: Optional[str] = None,
                  redundancy: Optional['outputs.ConnectionASideAccessPointPortRedundancy'] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
         :param str name: Port name
         :param 'ConnectionASideAccessPointPortRedundancyArgs' redundancy: Redundancy Information
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str uuid: Equinix-assigned Port identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if redundancy is not None:
             pulumi.set(__self__, "redundancy", redundancy)
@@ -1430,29 +1430,29 @@
         """
         return pulumi.get(self, "redundancy")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Port identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionASideAccessPointPortRedundancy(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  group: Optional[str] = None,
                  priority: Optional[str] = None):
         """
         :param bool enabled: Access point redundancy
-        :param str group: Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
-        :param str priority: Connection priority in redundancy group - PRIMARY, SECONDARY
+        :param str group: Port redundancy group
+        :param str priority: Priority type-Primary or Secondary
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
@@ -1465,23 +1465,23 @@
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def group(self) -> Optional[str]:
         """
-        Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
+        Port redundancy group
         """
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[str]:
         """
-        Connection priority in redundancy group - PRIMARY, SECONDARY
+        Priority type-Primary or Secondary
         """
         return pulumi.get(self, "priority")
 
 
 @pulumi.output_type
 class ConnectionASideAccessPointProfile(dict):
     @staticmethod
@@ -1505,20 +1505,20 @@
                  type: str,
                  uuid: str,
                  access_point_type_configs: Optional[Sequence['outputs.ConnectionASideAccessPointProfileAccessPointTypeConfig']] = None,
                  description: Optional[str] = None,
                  href: Optional[str] = None,
                  name: Optional[str] = None):
         """
-        :param Union[str, 'ProfileType'] type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param Union[str, 'ProfileType'] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
+        :param str uuid: Equinix assigned service profile identifier
         :param Sequence['ConnectionASideAccessPointProfileAccessPointTypeConfigArgs'] access_point_type_configs: Access point config information
         :param str description: User-provided service description
-        :param str href: Unique Resource Identifier
-        :param str name: Port name
+        :param str href: Service Profile URI response attribute
+        :param str name: Customer-assigned service profile name
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
         if access_point_type_configs is not None:
             pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -1527,23 +1527,23 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Interface type
+        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> str:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix assigned service profile identifier
         """
         return pulumi.get(self, "uuid")
 
     @property
     @pulumi.getter(name="accessPointTypeConfigs")
     def access_point_type_configs(self) -> Optional[Sequence['outputs.ConnectionASideAccessPointProfileAccessPointTypeConfig']]:
         """
@@ -1559,54 +1559,54 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def href(self) -> Optional[str]:
         """
-        Unique Resource Identifier
+        Service Profile URI response attribute
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Port name
+        Customer-assigned service profile name
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class ConnectionASideAccessPointProfileAccessPointTypeConfig(dict):
     def __init__(__self__, *,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
-        :param str type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str type: Type of access point type config - VD, COLO
+        :param str uuid: Equinix-assigned access point type config identifier
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Type of access point type config - VD, COLO
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned access point type config identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionASideAccessPointRouter(dict):
     def __init__(__self__, *,
@@ -1643,17 +1643,17 @@
     def __init__(__self__, *,
                  href: Optional[str] = None,
                  name: Optional[str] = None,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
-        :param str name: Port name
-        :param str type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str name: Customer-assigned Virtual Device Name
+        :param str type: Virtual Device type
+        :param str uuid: Equinix-assigned Virtual Device identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if type is not None:
             pulumi.set(__self__, "type", type)
@@ -1668,31 +1668,31 @@
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Port name
+        Customer-assigned Virtual Device Name
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Virtual Device type
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Virtual Device identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionASideAdditionalInfo(dict):
     def __init__(__self__, *,
@@ -1728,57 +1728,57 @@
 class ConnectionASideServiceToken(dict):
     def __init__(__self__, *,
                  description: Optional[str] = None,
                  href: Optional[str] = None,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
-        :param str description: User-provided service description
-        :param str href: Unique Resource Identifier
-        :param Union[str, 'ServiceTokenType'] type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str description: Service token description
+        :param str href: An absolute URL that is the subject of the link's context
+        :param Union[str, 'ServiceTokenType'] type: Token type - VC_TOKEN
+        :param str uuid: Equinix-assigned service token identifier
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if href is not None:
             pulumi.set(__self__, "href", href)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         """
-        User-provided service description
+        Service token description
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def href(self) -> Optional[str]:
         """
-        Unique Resource Identifier
+        An absolute URL that is the subject of the link's context
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Token type - VC_TOKEN
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned service token identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionAccount(dict):
     @staticmethod
@@ -2252,15 +2252,15 @@
                  additional_info: Optional[Sequence['outputs.ConnectionOperationErrorAdditionalInfo']] = None,
                  correlation_id: Optional[str] = None,
                  details: Optional[str] = None,
                  error_code: Optional[str] = None,
                  error_message: Optional[str] = None,
                  help: Optional[str] = None):
         """
-        :param Sequence['ConnectionOperationErrorAdditionalInfoArgs'] additional_info: Connection side additional information
+        :param Sequence['ConnectionOperationErrorAdditionalInfoArgs'] additional_info: Pricing error additional Info
         :param str correlation_id: CorrelationId
         :param str details: Details
         :param str error_code: Error  code
         :param str error_message: Error Message
         :param str help: Help
         """
         if additional_info is not None:
@@ -2276,15 +2276,15 @@
         if help is not None:
             pulumi.set(__self__, "help", help)
 
     @property
     @pulumi.getter(name="additionalInfo")
     def additional_info(self) -> Optional[Sequence['outputs.ConnectionOperationErrorAdditionalInfo']]:
         """
-        Connection side additional information
+        Pricing error additional Info
         """
         return pulumi.get(self, "additional_info")
 
     @property
     @pulumi.getter(name="correlationId")
     def correlation_id(self) -> Optional[str]:
         """
@@ -2632,15 +2632,15 @@
         :param 'ConnectionZSideAccessPointNetworkArgs' network: network access point information
         :param Union[str, 'AccessPointPeeringType'] peering_type: Peering Type- PRIVATE,MICROSOFT,PUBLIC, MANUAL
         :param 'ConnectionZSideAccessPointPortArgs' port: Port access point information
         :param 'ConnectionZSideAccessPointProfileArgs' profile: Service Profile
         :param str provider_connection_id: Provider assigned Connection Id
         :param 'ConnectionZSideAccessPointRouterArgs' router: Cloud Router access point information that replaces `gateway`
         :param str seller_region: Access point seller region
-        :param Union[str, 'AccessPointType'] type: Interface type
+        :param Union[str, 'AccessPointType'] type: Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         :param 'ConnectionZSideAccessPointVirtualDeviceArgs' virtual_device: Virtual device
         """
         if account is not None:
             pulumi.set(__self__, "account", account)
         if authentication_key is not None:
             pulumi.set(__self__, "authentication_key", authentication_key)
         if gateway is not None:
@@ -2777,15 +2777,15 @@
         """
         return pulumi.get(self, "seller_region")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="virtualDevice")
     def virtual_device(self) -> Optional['outputs.ConnectionZSideAccessPointVirtualDevice']:
         """
@@ -2964,15 +2964,15 @@
     def __init__(__self__, *,
                  id: Optional[int] = None,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
         :param int id: id
         :param str type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str uuid: Equinix-assigned interface identifier
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
@@ -2993,15 +2993,15 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned interface identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionZSideAccessPointLinkProtocol(dict):
     @staticmethod
@@ -3027,15 +3027,15 @@
 
     def __init__(__self__, *,
                  type: Optional[str] = None,
                  vlan_c_tag: Optional[int] = None,
                  vlan_s_tag: Optional[int] = None,
                  vlan_tag: Optional[int] = None):
         """
-        :param Union[str, 'AccessPointLinkProtocolType'] type: Interface type
+        :param Union[str, 'AccessPointLinkProtocolType'] type: Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         :param int vlan_c_tag: Vlan Customer Tag information, vlanCTag value specified for QINQ connections
         :param int vlan_s_tag: Vlan Provider Tag information, vlanSTag value specified for QINQ connections
         :param int vlan_tag: Vlan Tag information, vlanTag value specified for DOT1Q connections
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if vlan_c_tag is not None:
@@ -3045,15 +3045,15 @@
         if vlan_tag is not None:
             pulumi.set(__self__, "vlan_tag", vlan_tag)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Type of the link protocol - UNTAGGED, DOT1Q, QINQ, EVPN_VXLAN
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="vlanCTag")
     def vlan_c_tag(self) -> Optional[int]:
         """
@@ -3155,15 +3155,15 @@
 @pulumi.output_type
 class ConnectionZSideAccessPointNetwork(dict):
     def __init__(__self__, *,
                  href: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str uuid: Equinix-assigned Network identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
@@ -3174,15 +3174,15 @@
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Network identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionZSideAccessPointPort(dict):
     def __init__(__self__, *,
@@ -3190,15 +3190,15 @@
                  name: Optional[str] = None,
                  redundancy: Optional['outputs.ConnectionZSideAccessPointPortRedundancy'] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
         :param str name: Port name
         :param 'ConnectionZSideAccessPointPortRedundancyArgs' redundancy: Redundancy Information
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str uuid: Equinix-assigned Port identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if redundancy is not None:
             pulumi.set(__self__, "redundancy", redundancy)
@@ -3229,29 +3229,29 @@
         """
         return pulumi.get(self, "redundancy")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Port identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionZSideAccessPointPortRedundancy(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  group: Optional[str] = None,
                  priority: Optional[str] = None):
         """
         :param bool enabled: Access point redundancy
-        :param str group: Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
-        :param str priority: Connection priority in redundancy group - PRIMARY, SECONDARY
+        :param str group: Port redundancy group
+        :param str priority: Priority type-Primary or Secondary
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if group is not None:
             pulumi.set(__self__, "group", group)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
@@ -3264,23 +3264,23 @@
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def group(self) -> Optional[str]:
         """
-        Redundancy group identifier (Use the redundancy.0.group UUID of primary connection; e.g. one(equinix*fabric*connection.primary*port*connection.redundancy).group or equinix*fabric*connection.primary*port*connection.redundancy.0.group)
+        Port redundancy group
         """
         return pulumi.get(self, "group")
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[str]:
         """
-        Connection priority in redundancy group - PRIMARY, SECONDARY
+        Priority type-Primary or Secondary
         """
         return pulumi.get(self, "priority")
 
 
 @pulumi.output_type
 class ConnectionZSideAccessPointProfile(dict):
     @staticmethod
@@ -3304,20 +3304,20 @@
                  type: str,
                  uuid: str,
                  access_point_type_configs: Optional[Sequence['outputs.ConnectionZSideAccessPointProfileAccessPointTypeConfig']] = None,
                  description: Optional[str] = None,
                  href: Optional[str] = None,
                  name: Optional[str] = None):
         """
-        :param Union[str, 'ProfileType'] type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param Union[str, 'ProfileType'] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
+        :param str uuid: Equinix assigned service profile identifier
         :param Sequence['ConnectionZSideAccessPointProfileAccessPointTypeConfigArgs'] access_point_type_configs: Access point config information
         :param str description: User-provided service description
-        :param str href: Unique Resource Identifier
-        :param str name: Port name
+        :param str href: Service Profile URI response attribute
+        :param str name: Customer-assigned service profile name
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
         if access_point_type_configs is not None:
             pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -3326,23 +3326,23 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Interface type
+        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> str:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix assigned service profile identifier
         """
         return pulumi.get(self, "uuid")
 
     @property
     @pulumi.getter(name="accessPointTypeConfigs")
     def access_point_type_configs(self) -> Optional[Sequence['outputs.ConnectionZSideAccessPointProfileAccessPointTypeConfig']]:
         """
@@ -3358,54 +3358,54 @@
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def href(self) -> Optional[str]:
         """
-        Unique Resource Identifier
+        Service Profile URI response attribute
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Port name
+        Customer-assigned service profile name
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class ConnectionZSideAccessPointProfileAccessPointTypeConfig(dict):
     def __init__(__self__, *,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
-        :param str type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str type: Type of access point type config - VD, COLO
+        :param str uuid: Equinix-assigned access point type config identifier
         """
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Type of access point type config - VD, COLO
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned access point type config identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionZSideAccessPointRouter(dict):
     def __init__(__self__, *,
@@ -3442,17 +3442,17 @@
     def __init__(__self__, *,
                  href: Optional[str] = None,
                  name: Optional[str] = None,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
-        :param str name: Port name
-        :param str type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str name: Customer-assigned Virtual Device Name
+        :param str type: Virtual Device type
+        :param str uuid: Equinix-assigned Virtual Device identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if type is not None:
             pulumi.set(__self__, "type", type)
@@ -3467,31 +3467,31 @@
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Port name
+        Customer-assigned Virtual Device Name
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Virtual Device type
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned Virtual Device identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class ConnectionZSideAdditionalInfo(dict):
     def __init__(__self__, *,
@@ -3527,57 +3527,57 @@
 class ConnectionZSideServiceToken(dict):
     def __init__(__self__, *,
                  description: Optional[str] = None,
                  href: Optional[str] = None,
                  type: Optional[str] = None,
                  uuid: Optional[str] = None):
         """
-        :param str description: User-provided service description
-        :param str href: Unique Resource Identifier
-        :param Union[str, 'ServiceTokenType'] type: Interface type
-        :param str uuid: Equinix-assigned virtual gateway identifier
+        :param str description: Service token description
+        :param str href: An absolute URL that is the subject of the link's context
+        :param Union[str, 'ServiceTokenType'] type: Token type - VC_TOKEN
+        :param str uuid: Equinix-assigned service token identifier
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if href is not None:
             pulumi.set(__self__, "href", href)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         """
-        User-provided service description
+        Service token description
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def href(self) -> Optional[str]:
         """
-        Unique Resource Identifier
+        An absolute URL that is the subject of the link's context
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        Interface type
+        Token type - VC_TOKEN
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
-        Equinix-assigned virtual gateway identifier
+        Equinix-assigned service token identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class NetworkChange(dict):
     def __init__(__self__, *,
@@ -5561,30 +5561,30 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  description: Optional[str] = None,
                  sub_title: Optional[str] = None,
                  title: Optional[str] = None):
         """
-        :param str description: Description of authorization key
+        :param str description: Description
         :param str sub_title: Sub Title
         :param str title: Title
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if sub_title is not None:
             pulumi.set(__self__, "sub_title", sub_title)
         if title is not None:
             pulumi.set(__self__, "title", title)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         """
-        Description of authorization key
+        Description
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="subTitle")
     def sub_title(self) -> Optional[str]:
         """
@@ -6514,46 +6514,47 @@
 
 
 @pulumi.output_type
 class GetConnectionASideAccessPointResult(dict):
     def __init__(__self__, *,
                  accounts: Sequence['outputs.GetConnectionASideAccessPointAccountResult'],
                  location: 'outputs.GetConnectionASideAccessPointLocationResult',
+                 provider_connection_id: str,
                  authentication_key: Optional[str] = None,
                  gateway: Optional['outputs.GetConnectionASideAccessPointGatewayResult'] = None,
                  interface: Optional['outputs.GetConnectionASideAccessPointInterfaceResult'] = None,
                  link_protocol: Optional['outputs.GetConnectionASideAccessPointLinkProtocolResult'] = None,
                  network: Optional['outputs.GetConnectionASideAccessPointNetworkResult'] = None,
                  peering_type: Optional[str] = None,
                  port: Optional['outputs.GetConnectionASideAccessPointPortResult'] = None,
                  profile: Optional['outputs.GetConnectionASideAccessPointProfileResult'] = None,
-                 provider_connection_id: Optional[str] = None,
                  router: Optional['outputs.GetConnectionASideAccessPointRouterResult'] = None,
                  seller_region: Optional[str] = None,
                  type: Optional[str] = None,
                  virtual_device: Optional['outputs.GetConnectionASideAccessPointVirtualDeviceResult'] = None):
         """
         :param Sequence['GetConnectionASideAccessPointAccountArgs'] accounts: Account
         :param 'GetConnectionASideAccessPointLocationArgs' location: Access point location
+        :param str provider_connection_id: Provider assigned Connection Id
         :param str authentication_key: Authentication key for provider based connections
         :param 'GetConnectionASideAccessPointGatewayArgs' gateway: **Deprecated** `gateway` Use `router` attribute instead
         :param 'GetConnectionASideAccessPointInterfaceArgs' interface: Virtual device interface
         :param 'GetConnectionASideAccessPointLinkProtocolArgs' link_protocol: Connection link protocol
         :param 'GetConnectionASideAccessPointNetworkArgs' network: network access point information
         :param str peering_type: Peering Type- PRIVATE,MICROSOFT,PUBLIC, MANUAL
         :param 'GetConnectionASideAccessPointPortArgs' port: Port access point information
         :param 'GetConnectionASideAccessPointProfileArgs' profile: Service Profile
-        :param str provider_connection_id: Provider assigned Connection Id
         :param 'GetConnectionASideAccessPointRouterArgs' router: Cloud Router access point information that replaces `gateway`
         :param str seller_region: Access point seller region
         :param str type: Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         :param 'GetConnectionASideAccessPointVirtualDeviceArgs' virtual_device: Virtual device
         """
         pulumi.set(__self__, "accounts", accounts)
         pulumi.set(__self__, "location", location)
+        pulumi.set(__self__, "provider_connection_id", provider_connection_id)
         if authentication_key is not None:
             pulumi.set(__self__, "authentication_key", authentication_key)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
         if interface is not None:
             pulumi.set(__self__, "interface", interface)
         if link_protocol is not None:
@@ -6562,16 +6563,14 @@
             pulumi.set(__self__, "network", network)
         if peering_type is not None:
             pulumi.set(__self__, "peering_type", peering_type)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if profile is not None:
             pulumi.set(__self__, "profile", profile)
-        if provider_connection_id is not None:
-            pulumi.set(__self__, "provider_connection_id", provider_connection_id)
         if router is not None:
             pulumi.set(__self__, "router", router)
         if seller_region is not None:
             pulumi.set(__self__, "seller_region", seller_region)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if virtual_device is not None:
@@ -6590,14 +6589,22 @@
     def location(self) -> 'outputs.GetConnectionASideAccessPointLocationResult':
         """
         Access point location
         """
         return pulumi.get(self, "location")
 
     @property
+    @pulumi.getter(name="providerConnectionId")
+    def provider_connection_id(self) -> str:
+        """
+        Provider assigned Connection Id
+        """
+        return pulumi.get(self, "provider_connection_id")
+
+    @property
     @pulumi.getter(name="authenticationKey")
     def authentication_key(self) -> Optional[str]:
         """
         Authentication key for provider based connections
         """
         return pulumi.get(self, "authentication_key")
 
@@ -6657,22 +6664,14 @@
     def profile(self) -> Optional['outputs.GetConnectionASideAccessPointProfileResult']:
         """
         Service Profile
         """
         return pulumi.get(self, "profile")
 
     @property
-    @pulumi.getter(name="providerConnectionId")
-    def provider_connection_id(self) -> Optional[str]:
-        """
-        Provider assigned Connection Id
-        """
-        return pulumi.get(self, "provider_connection_id")
-
-    @property
     @pulumi.getter
     def router(self) -> Optional['outputs.GetConnectionASideAccessPointRouterResult']:
         """
         Cloud Router access point information that replaces `gateway`
         """
         return pulumi.get(self, "router")
 
@@ -7102,15 +7101,15 @@
                  type: str,
                  uuid: str):
         """
         :param Sequence['GetConnectionASideAccessPointProfileAccessPointTypeConfigArgs'] access_point_type_configs: Access point config information
         :param str description: User-provided service description
         :param str href: Service Profile URI response attribute
         :param str name: Customer-assigned service profile name
-        :param str type: Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE
+        :param str type: Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE, IA_PROFILE
         :param str uuid: Equinix assigned service profile identifier
         """
         pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "href", href)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
@@ -7148,15 +7147,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE
+        Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE, IA_PROFILE
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> str:
         """
@@ -7167,33 +7166,33 @@
 
 @pulumi.output_type
 class GetConnectionASideAccessPointProfileAccessPointTypeConfigResult(dict):
     def __init__(__self__, *,
                  type: str,
                  uuid: str):
         """
-        :param str type: Type of access point type config - VD, COLO
-        :param str uuid: Equinix-assigned access point type config identifier
+        :param str type: Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
+        :param str uuid: Equinix-assigned connection identifier
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Type of access point type config - VD, COLO
+        Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> str:
         """
-        Equinix-assigned access point type config identifier
+        Equinix-assigned connection identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class GetConnectionASideAccessPointRouterResult(dict):
     def __init__(__self__, *,
@@ -7932,46 +7931,47 @@
 
 
 @pulumi.output_type
 class GetConnectionZSideAccessPointResult(dict):
     def __init__(__self__, *,
                  accounts: Sequence['outputs.GetConnectionZSideAccessPointAccountResult'],
                  location: 'outputs.GetConnectionZSideAccessPointLocationResult',
+                 provider_connection_id: str,
                  authentication_key: Optional[str] = None,
                  gateway: Optional['outputs.GetConnectionZSideAccessPointGatewayResult'] = None,
                  interface: Optional['outputs.GetConnectionZSideAccessPointInterfaceResult'] = None,
                  link_protocol: Optional['outputs.GetConnectionZSideAccessPointLinkProtocolResult'] = None,
                  network: Optional['outputs.GetConnectionZSideAccessPointNetworkResult'] = None,
                  peering_type: Optional[str] = None,
                  port: Optional['outputs.GetConnectionZSideAccessPointPortResult'] = None,
                  profile: Optional['outputs.GetConnectionZSideAccessPointProfileResult'] = None,
-                 provider_connection_id: Optional[str] = None,
                  router: Optional['outputs.GetConnectionZSideAccessPointRouterResult'] = None,
                  seller_region: Optional[str] = None,
                  type: Optional[str] = None,
                  virtual_device: Optional['outputs.GetConnectionZSideAccessPointVirtualDeviceResult'] = None):
         """
         :param Sequence['GetConnectionZSideAccessPointAccountArgs'] accounts: Account
         :param 'GetConnectionZSideAccessPointLocationArgs' location: Access point location
+        :param str provider_connection_id: Provider assigned Connection Id
         :param str authentication_key: Authentication key for provider based connections
         :param 'GetConnectionZSideAccessPointGatewayArgs' gateway: **Deprecated** `gateway` Use `router` attribute instead
         :param 'GetConnectionZSideAccessPointInterfaceArgs' interface: Virtual device interface
         :param 'GetConnectionZSideAccessPointLinkProtocolArgs' link_protocol: Connection link protocol
         :param 'GetConnectionZSideAccessPointNetworkArgs' network: network access point information
         :param str peering_type: Peering Type- PRIVATE,MICROSOFT,PUBLIC, MANUAL
         :param 'GetConnectionZSideAccessPointPortArgs' port: Port access point information
         :param 'GetConnectionZSideAccessPointProfileArgs' profile: Service Profile
-        :param str provider_connection_id: Provider assigned Connection Id
         :param 'GetConnectionZSideAccessPointRouterArgs' router: Cloud Router access point information that replaces `gateway`
         :param str seller_region: Access point seller region
         :param str type: Access point type - COLO, VD, VG, SP, IGW, SUBNET, CLOUD_ROUTER, NETWORK
         :param 'GetConnectionZSideAccessPointVirtualDeviceArgs' virtual_device: Virtual device
         """
         pulumi.set(__self__, "accounts", accounts)
         pulumi.set(__self__, "location", location)
+        pulumi.set(__self__, "provider_connection_id", provider_connection_id)
         if authentication_key is not None:
             pulumi.set(__self__, "authentication_key", authentication_key)
         if gateway is not None:
             pulumi.set(__self__, "gateway", gateway)
         if interface is not None:
             pulumi.set(__self__, "interface", interface)
         if link_protocol is not None:
@@ -7980,16 +7980,14 @@
             pulumi.set(__self__, "network", network)
         if peering_type is not None:
             pulumi.set(__self__, "peering_type", peering_type)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if profile is not None:
             pulumi.set(__self__, "profile", profile)
-        if provider_connection_id is not None:
-            pulumi.set(__self__, "provider_connection_id", provider_connection_id)
         if router is not None:
             pulumi.set(__self__, "router", router)
         if seller_region is not None:
             pulumi.set(__self__, "seller_region", seller_region)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if virtual_device is not None:
@@ -8008,14 +8006,22 @@
     def location(self) -> 'outputs.GetConnectionZSideAccessPointLocationResult':
         """
         Access point location
         """
         return pulumi.get(self, "location")
 
     @property
+    @pulumi.getter(name="providerConnectionId")
+    def provider_connection_id(self) -> str:
+        """
+        Provider assigned Connection Id
+        """
+        return pulumi.get(self, "provider_connection_id")
+
+    @property
     @pulumi.getter(name="authenticationKey")
     def authentication_key(self) -> Optional[str]:
         """
         Authentication key for provider based connections
         """
         return pulumi.get(self, "authentication_key")
 
@@ -8075,22 +8081,14 @@
     def profile(self) -> Optional['outputs.GetConnectionZSideAccessPointProfileResult']:
         """
         Service Profile
         """
         return pulumi.get(self, "profile")
 
     @property
-    @pulumi.getter(name="providerConnectionId")
-    def provider_connection_id(self) -> Optional[str]:
-        """
-        Provider assigned Connection Id
-        """
-        return pulumi.get(self, "provider_connection_id")
-
-    @property
     @pulumi.getter
     def router(self) -> Optional['outputs.GetConnectionZSideAccessPointRouterResult']:
         """
         Cloud Router access point information that replaces `gateway`
         """
         return pulumi.get(self, "router")
 
@@ -8520,15 +8518,15 @@
                  type: str,
                  uuid: str):
         """
         :param Sequence['GetConnectionZSideAccessPointProfileAccessPointTypeConfigArgs'] access_point_type_configs: Access point config information
         :param str description: User-provided service description
         :param str href: Service Profile URI response attribute
         :param str name: Customer-assigned service profile name
-        :param str type: Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE
+        :param str type: Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE, IA_PROFILE
         :param str uuid: Equinix assigned service profile identifier
         """
         pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "href", href)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
@@ -8566,15 +8564,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE
+        Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE, IA_PROFILE
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> str:
         """
@@ -8585,33 +8583,33 @@
 
 @pulumi.output_type
 class GetConnectionZSideAccessPointProfileAccessPointTypeConfigResult(dict):
     def __init__(__self__, *,
                  type: str,
                  uuid: str):
         """
-        :param str type: Type of access point type config - VD, COLO
-        :param str uuid: Equinix-assigned access point type config identifier
+        :param str type: Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
+        :param str uuid: Equinix-assigned connection identifier
         """
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Type of access point type config - VD, COLO
+        Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> str:
         """
-        Equinix-assigned access point type config identifier
+        Equinix-assigned connection identifier
         """
         return pulumi.get(self, "uuid")
 
 
 @pulumi.output_type
 class GetConnectionZSideAccessPointRouterResult(dict):
     def __init__(__self__, *,
@@ -11830,14 +11828,15 @@
                  ports: Sequence['outputs.GetServiceProfilesDatumPortResult'],
                  projects: Sequence['outputs.GetServiceProfilesDatumProjectResult'],
                  self_profile: bool,
                  state: str,
                  tags: Sequence[str],
                  type: str,
                  uuid: str,
+                 view_point: str,
                  virtual_devices: Sequence['outputs.GetServiceProfilesDatumVirtualDeviceResult'],
                  visibility: str):
         """
         :param Sequence['GetServiceProfilesDatumAccessPointTypeConfigArgs'] access_point_type_configs: Access point config information
         :param Sequence['GetServiceProfilesDatumAccountArgs'] accounts: Service Profile Owner Account Information
         :param Sequence[str] allowed_emails: Array of contact emails
         :param Sequence['GetServiceProfilesDatumChangeLogArgs'] change_logs: Captures connection lifecycle change information
@@ -11849,16 +11848,17 @@
         :param str name: Customer-assigned service profile name
         :param Sequence['GetServiceProfilesDatumNotificationArgs'] notifications: Preferences for notifications on connection configuration or status changes
         :param Sequence['GetServiceProfilesDatumPortArgs'] ports: Ports
         :param Sequence['GetServiceProfilesDatumProjectArgs'] projects: Project information
         :param bool self_profile: Self Profile indicating if the profile is created for customer's  self use
         :param str state: Service profile state - ACTIVE, PENDING_APPROVAL, DELETED, REJECTED
         :param Sequence[str] tags: Tags attached to the connection
-        :param str type: Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE
+        :param str type: Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE, IA_PROFILE
         :param str uuid: Equinix assigned service profile identifier
+        :param str view_point: flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
         :param Sequence['GetServiceProfilesDatumVirtualDeviceArgs'] virtual_devices: Virtual Devices
         :param str visibility: Service profile visibility - PUBLIC, PRIVATE
         """
         pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         pulumi.set(__self__, "accounts", accounts)
         pulumi.set(__self__, "allowed_emails", allowed_emails)
         pulumi.set(__self__, "change_logs", change_logs)
@@ -11872,14 +11872,15 @@
         pulumi.set(__self__, "ports", ports)
         pulumi.set(__self__, "projects", projects)
         pulumi.set(__self__, "self_profile", self_profile)
         pulumi.set(__self__, "state", state)
         pulumi.set(__self__, "tags", tags)
         pulumi.set(__self__, "type", type)
         pulumi.set(__self__, "uuid", uuid)
+        pulumi.set(__self__, "view_point", view_point)
         pulumi.set(__self__, "virtual_devices", virtual_devices)
         pulumi.set(__self__, "visibility", visibility)
 
     @property
     @pulumi.getter(name="accessPointTypeConfigs")
     def access_point_type_configs(self) -> Sequence['outputs.GetServiceProfilesDatumAccessPointTypeConfigResult']:
         """
@@ -12007,27 +12008,35 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE
+        Service profile type - L2_PROFILE, L3_PROFILE, ECIA_PROFILE, ECMC_PROFILE, IA_PROFILE
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> str:
         """
         Equinix assigned service profile identifier
         """
         return pulumi.get(self, "uuid")
 
     @property
+    @pulumi.getter(name="viewPoint")
+    def view_point(self) -> str:
+        """
+        flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
+        """
+        return pulumi.get(self, "view_point")
+
+    @property
     @pulumi.getter(name="virtualDevices")
     def virtual_devices(self) -> Sequence['outputs.GetServiceProfilesDatumVirtualDeviceResult']:
         """
         Virtual Devices
         """
         return pulumi.get(self, "virtual_devices")
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/routing_protocol.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/routing_protocol.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/fabric/service_profile.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/service_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,32 +27,34 @@
                  name: Optional[pulumi.Input[str]] = None,
                  notifications: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileNotificationArgs']]]] = None,
                  ports: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortArgs']]]] = None,
                  project: Optional[pulumi.Input['ServiceProfileProjectArgs']] = None,
                  self_profile: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[Union[str, 'ProfileState']]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 view_point: Optional[pulumi.Input[str]] = None,
                  virtual_devices: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileVirtualDeviceArgs']]]] = None,
                  visibility: Optional[pulumi.Input[Union[str, 'ProfileVisibility']]] = None):
         """
         The set of arguments for constructing a ServiceProfile resource.
-        :param pulumi.Input[str] description: Description of authorization key
-        :param pulumi.Input[Union[str, 'ProfileType']] type: Type of access point type config - VD, COLO
+        :param pulumi.Input[str] description: User-provided service description
+        :param pulumi.Input[Union[str, 'ProfileType']] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileAccessPointTypeConfigArgs']]] access_point_type_configs: Access point config information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_emails: Array of contact emails
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileCustomFieldArgs']]] custom_fields: Custom Fields
         :param pulumi.Input['ServiceProfileMarketingInfoArgs'] marketing_info: Marketing Info
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileMetroArgs']]] metros: Access point config information
-        :param pulumi.Input[str] name: Metro Name
+        :param pulumi.Input[str] name: Customer-assigned service profile name
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileNotificationArgs']]] notifications: Preferences for notifications on connection configuration or status changes
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortArgs']]] ports: Ports
         :param pulumi.Input['ServiceProfileProjectArgs'] project: Project information
         :param pulumi.Input[bool] self_profile: Self Profile indicating if the profile is created for customer's  self use
         :param pulumi.Input[Union[str, 'ProfileState']] state: Service profile state - ACTIVE, PENDING_APPROVAL, DELETED, REJECTED
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags attached to the connection
+        :param pulumi.Input[str] view_point: Flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileVirtualDeviceArgs']]] virtual_devices: Virtual Devices
         :param pulumi.Input[Union[str, 'ProfileVisibility']] visibility: Service profile visibility - PUBLIC, PRIVATE
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "type", type)
         if access_point_type_configs is not None:
             pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
@@ -74,36 +76,38 @@
             pulumi.set(__self__, "project", project)
         if self_profile is not None:
             pulumi.set(__self__, "self_profile", self_profile)
         if state is not None:
             pulumi.set(__self__, "state", state)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if view_point is not None:
+            pulumi.set(__self__, "view_point", view_point)
         if virtual_devices is not None:
             pulumi.set(__self__, "virtual_devices", virtual_devices)
         if visibility is not None:
             pulumi.set(__self__, "visibility", visibility)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Input[str]:
         """
-        Description of authorization key
+        User-provided service description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: pulumi.Input[str]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[Union[str, 'ProfileType']]:
         """
-        Type of access point type config - VD, COLO
+        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[Union[str, 'ProfileType']]):
         pulumi.set(self, "type", value)
 
@@ -167,15 +171,15 @@
     def metros(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileMetroArgs']]]]):
         pulumi.set(self, "metros", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Metro Name
+        Customer-assigned service profile name
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -248,14 +252,26 @@
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
+    @pulumi.getter(name="viewPoint")
+    def view_point(self) -> Optional[pulumi.Input[str]]:
+        """
+        Flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
+        """
+        return pulumi.get(self, "view_point")
+
+    @view_point.setter
+    def view_point(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "view_point", value)
+
+    @property
     @pulumi.getter(name="virtualDevices")
     def virtual_devices(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileVirtualDeviceArgs']]]]:
         """
         Virtual Devices
         """
         return pulumi.get(self, "virtual_devices")
 
@@ -293,36 +309,38 @@
                  ports: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortArgs']]]] = None,
                  project: Optional[pulumi.Input['ServiceProfileProjectArgs']] = None,
                  self_profile: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[Union[str, 'ProfileState']]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[Union[str, 'ProfileType']]] = None,
                  uuid: Optional[pulumi.Input[str]] = None,
+                 view_point: Optional[pulumi.Input[str]] = None,
                  virtual_devices: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileVirtualDeviceArgs']]]] = None,
                  visibility: Optional[pulumi.Input[Union[str, 'ProfileVisibility']]] = None):
         """
         Input properties used for looking up and filtering ServiceProfile resources.
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileAccessPointTypeConfigArgs']]] access_point_type_configs: Access point config information
         :param pulumi.Input['ServiceProfileAccountArgs'] account: Service Profile Owner Account Information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_emails: Array of contact emails
         :param pulumi.Input['ServiceProfileChangeLogArgs'] change_log: Captures connection lifecycle change information
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileCustomFieldArgs']]] custom_fields: Custom Fields
-        :param pulumi.Input[str] description: Description of authorization key
-        :param pulumi.Input[str] href: Unique Resource URL
+        :param pulumi.Input[str] description: User-provided service description
+        :param pulumi.Input[str] href: Service Profile URI response attribute
         :param pulumi.Input['ServiceProfileMarketingInfoArgs'] marketing_info: Marketing Info
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileMetroArgs']]] metros: Access point config information
-        :param pulumi.Input[str] name: Metro Name
+        :param pulumi.Input[str] name: Customer-assigned service profile name
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileNotificationArgs']]] notifications: Preferences for notifications on connection configuration or status changes
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfilePortArgs']]] ports: Ports
         :param pulumi.Input['ServiceProfileProjectArgs'] project: Project information
         :param pulumi.Input[bool] self_profile: Self Profile indicating if the profile is created for customer's  self use
         :param pulumi.Input[Union[str, 'ProfileState']] state: Service profile state - ACTIVE, PENDING_APPROVAL, DELETED, REJECTED
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags attached to the connection
-        :param pulumi.Input[Union[str, 'ProfileType']] type: Type of access point type config - VD, COLO
-        :param pulumi.Input[str] uuid: Colo/Port Uuid
+        :param pulumi.Input[Union[str, 'ProfileType']] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
+        :param pulumi.Input[str] uuid: Equinix assigned service profile identifier
+        :param pulumi.Input[str] view_point: Flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
         :param pulumi.Input[Sequence[pulumi.Input['ServiceProfileVirtualDeviceArgs']]] virtual_devices: Virtual Devices
         :param pulumi.Input[Union[str, 'ProfileVisibility']] visibility: Service profile visibility - PUBLIC, PRIVATE
         """
         if access_point_type_configs is not None:
             pulumi.set(__self__, "access_point_type_configs", access_point_type_configs)
         if account is not None:
             pulumi.set(__self__, "account", account)
@@ -354,14 +372,16 @@
             pulumi.set(__self__, "state", state)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
+        if view_point is not None:
+            pulumi.set(__self__, "view_point", view_point)
         if virtual_devices is not None:
             pulumi.set(__self__, "virtual_devices", virtual_devices)
         if visibility is not None:
             pulumi.set(__self__, "visibility", visibility)
 
     @property
     @pulumi.getter(name="accessPointTypeConfigs")
@@ -423,27 +443,27 @@
     def custom_fields(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileCustomFieldArgs']]]]):
         pulumi.set(self, "custom_fields", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description of authorization key
+        User-provided service description
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
-        Unique Resource URL
+        Service Profile URI response attribute
         """
         return pulumi.get(self, "href")
 
     @href.setter
     def href(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "href", value)
 
@@ -471,15 +491,15 @@
     def metros(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileMetroArgs']]]]):
         pulumi.set(self, "metros", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Metro Name
+        Customer-assigned service profile name
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -555,35 +575,47 @@
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[Union[str, 'ProfileType']]]:
         """
-        Type of access point type config - VD, COLO
+        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[Union[str, 'ProfileType']]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Colo/Port Uuid
+        Equinix assigned service profile identifier
         """
         return pulumi.get(self, "uuid")
 
     @uuid.setter
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
     @property
+    @pulumi.getter(name="viewPoint")
+    def view_point(self) -> Optional[pulumi.Input[str]]:
+        """
+        Flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
+        """
+        return pulumi.get(self, "view_point")
+
+    @view_point.setter
+    def view_point(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "view_point", value)
+
+    @property
     @pulumi.getter(name="virtualDevices")
     def virtual_devices(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServiceProfileVirtualDeviceArgs']]]]:
         """
         Virtual Devices
         """
         return pulumi.get(self, "virtual_devices")
 
@@ -619,14 +651,15 @@
                  notifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileNotificationArgs']]]]] = None,
                  ports: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfilePortArgs']]]]] = None,
                  project: Optional[pulumi.Input[pulumi.InputType['ServiceProfileProjectArgs']]] = None,
                  self_profile: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[Union[str, 'ProfileState']]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[Union[str, 'ProfileType']]] = None,
+                 view_point: Optional[pulumi.Input[str]] = None,
                  virtual_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileVirtualDeviceArgs']]]]] = None,
                  visibility: Optional[pulumi.Input[Union[str, 'ProfileVisibility']]] = None,
                  __props__=None):
         """
         Fabric V4 API compatible resource allows creation and management of Equinix Fabric Service Profile
 
         ## Example Usage
@@ -680,25 +713,26 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileAccessPointTypeConfigArgs']]]] access_point_type_configs: Access point config information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_emails: Array of contact emails
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileCustomFieldArgs']]]] custom_fields: Custom Fields
-        :param pulumi.Input[str] description: Description of authorization key
+        :param pulumi.Input[str] description: User-provided service description
         :param pulumi.Input[pulumi.InputType['ServiceProfileMarketingInfoArgs']] marketing_info: Marketing Info
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileMetroArgs']]]] metros: Access point config information
-        :param pulumi.Input[str] name: Metro Name
+        :param pulumi.Input[str] name: Customer-assigned service profile name
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileNotificationArgs']]]] notifications: Preferences for notifications on connection configuration or status changes
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfilePortArgs']]]] ports: Ports
         :param pulumi.Input[pulumi.InputType['ServiceProfileProjectArgs']] project: Project information
         :param pulumi.Input[bool] self_profile: Self Profile indicating if the profile is created for customer's  self use
         :param pulumi.Input[Union[str, 'ProfileState']] state: Service profile state - ACTIVE, PENDING_APPROVAL, DELETED, REJECTED
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags attached to the connection
-        :param pulumi.Input[Union[str, 'ProfileType']] type: Type of access point type config - VD, COLO
+        :param pulumi.Input[Union[str, 'ProfileType']] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
+        :param pulumi.Input[str] view_point: Flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileVirtualDeviceArgs']]]] virtual_devices: Virtual Devices
         :param pulumi.Input[Union[str, 'ProfileVisibility']] visibility: Service profile visibility - PUBLIC, PRIVATE
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -782,14 +816,15 @@
                  notifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileNotificationArgs']]]]] = None,
                  ports: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfilePortArgs']]]]] = None,
                  project: Optional[pulumi.Input[pulumi.InputType['ServiceProfileProjectArgs']]] = None,
                  self_profile: Optional[pulumi.Input[bool]] = None,
                  state: Optional[pulumi.Input[Union[str, 'ProfileState']]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[Union[str, 'ProfileType']]] = None,
+                 view_point: Optional[pulumi.Input[str]] = None,
                  virtual_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileVirtualDeviceArgs']]]]] = None,
                  visibility: Optional[pulumi.Input[Union[str, 'ProfileVisibility']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -811,14 +846,15 @@
             __props__.__dict__["project"] = project
             __props__.__dict__["self_profile"] = self_profile
             __props__.__dict__["state"] = state
             __props__.__dict__["tags"] = tags
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
+            __props__.__dict__["view_point"] = view_point
             __props__.__dict__["virtual_devices"] = virtual_devices
             __props__.__dict__["visibility"] = visibility
             __props__.__dict__["account"] = None
             __props__.__dict__["change_log"] = None
             __props__.__dict__["href"] = None
             __props__.__dict__["uuid"] = None
         super(ServiceProfile, __self__).__init__(
@@ -845,41 +881,43 @@
             ports: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfilePortArgs']]]]] = None,
             project: Optional[pulumi.Input[pulumi.InputType['ServiceProfileProjectArgs']]] = None,
             self_profile: Optional[pulumi.Input[bool]] = None,
             state: Optional[pulumi.Input[Union[str, 'ProfileState']]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             type: Optional[pulumi.Input[Union[str, 'ProfileType']]] = None,
             uuid: Optional[pulumi.Input[str]] = None,
+            view_point: Optional[pulumi.Input[str]] = None,
             virtual_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileVirtualDeviceArgs']]]]] = None,
             visibility: Optional[pulumi.Input[Union[str, 'ProfileVisibility']]] = None) -> 'ServiceProfile':
         """
         Get an existing ServiceProfile resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileAccessPointTypeConfigArgs']]]] access_point_type_configs: Access point config information
         :param pulumi.Input[pulumi.InputType['ServiceProfileAccountArgs']] account: Service Profile Owner Account Information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_emails: Array of contact emails
         :param pulumi.Input[pulumi.InputType['ServiceProfileChangeLogArgs']] change_log: Captures connection lifecycle change information
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileCustomFieldArgs']]]] custom_fields: Custom Fields
-        :param pulumi.Input[str] description: Description of authorization key
-        :param pulumi.Input[str] href: Unique Resource URL
+        :param pulumi.Input[str] description: User-provided service description
+        :param pulumi.Input[str] href: Service Profile URI response attribute
         :param pulumi.Input[pulumi.InputType['ServiceProfileMarketingInfoArgs']] marketing_info: Marketing Info
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileMetroArgs']]]] metros: Access point config information
-        :param pulumi.Input[str] name: Metro Name
+        :param pulumi.Input[str] name: Customer-assigned service profile name
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileNotificationArgs']]]] notifications: Preferences for notifications on connection configuration or status changes
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfilePortArgs']]]] ports: Ports
         :param pulumi.Input[pulumi.InputType['ServiceProfileProjectArgs']] project: Project information
         :param pulumi.Input[bool] self_profile: Self Profile indicating if the profile is created for customer's  self use
         :param pulumi.Input[Union[str, 'ProfileState']] state: Service profile state - ACTIVE, PENDING_APPROVAL, DELETED, REJECTED
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags attached to the connection
-        :param pulumi.Input[Union[str, 'ProfileType']] type: Type of access point type config - VD, COLO
-        :param pulumi.Input[str] uuid: Colo/Port Uuid
+        :param pulumi.Input[Union[str, 'ProfileType']] type: Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
+        :param pulumi.Input[str] uuid: Equinix assigned service profile identifier
+        :param pulumi.Input[str] view_point: Flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServiceProfileVirtualDeviceArgs']]]] virtual_devices: Virtual Devices
         :param pulumi.Input[Union[str, 'ProfileVisibility']] visibility: Service profile visibility - PUBLIC, PRIVATE
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceProfileState.__new__(_ServiceProfileState)
 
@@ -897,14 +935,15 @@
         __props__.__dict__["ports"] = ports
         __props__.__dict__["project"] = project
         __props__.__dict__["self_profile"] = self_profile
         __props__.__dict__["state"] = state
         __props__.__dict__["tags"] = tags
         __props__.__dict__["type"] = type
         __props__.__dict__["uuid"] = uuid
+        __props__.__dict__["view_point"] = view_point
         __props__.__dict__["virtual_devices"] = virtual_devices
         __props__.__dict__["visibility"] = visibility
         return ServiceProfile(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accessPointTypeConfigs")
     def access_point_type_configs(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceProfileAccessPointTypeConfig']]]:
@@ -945,23 +984,23 @@
         """
         return pulumi.get(self, "custom_fields")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[str]:
         """
-        Description of authorization key
+        User-provided service description
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def href(self) -> pulumi.Output[str]:
         """
-        Unique Resource URL
+        Service Profile URI response attribute
         """
         return pulumi.get(self, "href")
 
     @property
     @pulumi.getter(name="marketingInfo")
     def marketing_info(self) -> pulumi.Output[Optional['outputs.ServiceProfileMarketingInfo']]:
         """
@@ -977,15 +1016,15 @@
         """
         return pulumi.get(self, "metros")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Metro Name
+        Customer-assigned service profile name
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def notifications(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceProfileNotification']]]:
         """
@@ -1033,27 +1072,35 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
         """
-        Type of access point type config - VD, COLO
+        Service profile type - L2*PROFILE, L3*PROFILE, ECIA*PROFILE, ECMC*PROFILE
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def uuid(self) -> pulumi.Output[str]:
         """
-        Colo/Port Uuid
+        Equinix assigned service profile identifier
         """
         return pulumi.get(self, "uuid")
 
     @property
+    @pulumi.getter(name="viewPoint")
+    def view_point(self) -> pulumi.Output[Optional[str]]:
+        """
+        Flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
+        """
+        return pulumi.get(self, "view_point")
+
+    @property
     @pulumi.getter(name="virtualDevices")
     def virtual_devices(self) -> pulumi.Output[Optional[Sequence['outputs.ServiceProfileVirtualDevice']]]:
         """
         Virtual Devices
         """
         return pulumi.get(self, "virtual_devices")
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/__init__.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/_enums.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/_inputs.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                  address: Optional[pulumi.Input[str]] = None,
                  cidr: Optional[pulumi.Input[int]] = None,
                  family: Optional[pulumi.Input[int]] = None,
                  gateway: Optional[pulumi.Input[str]] = None,
                  public: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[str] address: IPv4 or IPv6 address string.
-        :param pulumi.Input[int] cidr: CIDR suffix for IP address block to be assigned, i.e. amount of addresses.
+        :param pulumi.Input[int] cidr: Bit length of the network mask of the address.
         :param pulumi.Input[int] family: IP version. One of `4`, `6`.
         :param pulumi.Input[str] gateway: Address of router.
         :param pulumi.Input[bool] public: Whether the address is routable from the Internet.
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if cidr is not None:
@@ -159,15 +159,15 @@
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[pulumi.Input[int]]:
         """
-        CIDR suffix for IP address block to be assigned, i.e. amount of addresses.
+        Bit length of the network mask of the address.
         """
         return pulumi.get(self, "cidr")
 
     @cidr.setter
     def cidr(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cidr", value)
 
@@ -217,15 +217,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] bonded: Whether this port is part of a bond in bonded network setup.
         :param pulumi.Input[str] id: ID of the port.
         :param pulumi.Input[str] mac: MAC address assigned to the port.
         :param pulumi.Input[str] name: Name of the port (e.g. `eth0`, or `bond0`).
-        :param pulumi.Input[str] type: One of `private_ipv4`, `public_ipv4`, `public_ipv6`.
+        :param pulumi.Input[str] type: Type of the port (e.g. `NetworkPort` or `NetworkBondPort`).
         """
         if bonded is not None:
             pulumi.set(__self__, "bonded", bonded)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if mac is not None:
             pulumi.set(__self__, "mac", mac)
@@ -282,15 +282,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
-        One of `private_ipv4`, `public_ipv4`, `public_ipv6`.
+        Type of the port (e.g. `NetworkPort` or `NetworkBondPort`).
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -1002,26 +1002,26 @@
 
 @pulumi.input_type
 class GetDevicesSortArgs:
     def __init__(__self__, *,
                  attribute: str,
                  direction: Optional[str] = None):
         """
-        :param str attribute: The attribute used to filter. Filter attributes are case-sensitive
+        :param str attribute: The attribute used to sort the results. Sort attributes are case-sensitive
         :param str direction: Sort results in ascending or descending order. Strings are sorted in alphabetical order. One of: asc, desc
         """
         pulumi.set(__self__, "attribute", attribute)
         if direction is not None:
             pulumi.set(__self__, "direction", direction)
 
     @property
     @pulumi.getter
     def attribute(self) -> str:
         """
-        The attribute used to filter. Filter attributes are case-sensitive
+        The attribute used to sort the results. Sort attributes are case-sensitive
         """
         return pulumi.get(self, "attribute")
 
     @attribute.setter
     def attribute(self, value: str):
         pulumi.set(self, "attribute", value)
 
@@ -1193,26 +1193,26 @@
 
 @pulumi.input_type
 class GetPlansSortArgs:
     def __init__(__self__, *,
                  attribute: str,
                  direction: Optional[str] = None):
         """
-        :param str attribute: The attribute used to filter. Filter attributes are case-sensitive
+        :param str attribute: The attribute used to sort the results. Sort attributes are case-sensitive
         :param str direction: Sort results in ascending or descending order. Strings are sorted in alphabetical order. One of: asc, desc
         """
         pulumi.set(__self__, "attribute", attribute)
         if direction is not None:
             pulumi.set(__self__, "direction", direction)
 
     @property
     @pulumi.getter
     def attribute(self) -> str:
         """
-        The attribute used to filter. Filter attributes are case-sensitive
+        The attribute used to sort the results. Sort attributes are case-sensitive
         """
         return pulumi.get(self, "attribute")
 
     @attribute.setter
     def attribute(self, value: str):
         pulumi.set(self, "attribute", value)
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/bgp_session.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/bgp_session.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/device.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,16 @@
                  user_ssh_key_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  wait_for_reservation_deprovision: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Device resource.
         :param pulumi.Input[Union[str, 'OperatingSystem']] operating_system: The operating system slug. To find the slug, or visit
                [Operating Systems API docs](https://metal.equinix.com/developers/api/operatingsystems), set your
                API auth token in the top of the page and see JSON from the API response.
-        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit
-               [Device plans API docs](https://metal.equinix.com/developers/api/plans), set your auth token in the
-               top of the page and see JSON from the API response.
+        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit the
+               [bare-metal server](https://deploy.equinix.com/product/bare-metal/servers/) and [plan documentation](https://deploy.equinix.com/developers/docs/metal/hardware/standard-servers/).
         :param pulumi.Input[str] project_id: The ID of the project in which to create the device
         :param pulumi.Input[bool] always_pxe: If true, a device with OS `custom_ipxe` will continue to boot via iPXE
                on reboots.
         :param pulumi.Input['DeviceBehaviorArgs'] behavior: Behavioral overrides that change how the resource handles certain attribute updates. See Behavior below for more details.
         :param pulumi.Input[Union[str, 'BillingCycle']] billing_cycle: monthly or hourly
         :param pulumi.Input[str] custom_data: A string of the desired Custom Data for the device.  By default, changing this attribute will cause the provider to destroy and recreate your device.  If `reinstall` is specified or `behavior.allow_changes` includes `"custom_data"`, the device will be updated in-place instead of recreated.
         :param pulumi.Input[str] description: The device description.
@@ -164,17 +163,16 @@
     def operating_system(self, value: pulumi.Input[Union[str, 'OperatingSystem']]):
         pulumi.set(self, "operating_system", value)
 
     @property
     @pulumi.getter
     def plan(self) -> pulumi.Input[Union[str, 'Plan']]:
         """
-        The device plan slug. To find the plan slug, visit
-        [Device plans API docs](https://metal.equinix.com/developers/api/plans), set your auth token in the
-        top of the page and see JSON from the API response.
+        The device plan slug. To find the plan slug, visit the
+        [bare-metal server](https://deploy.equinix.com/product/bare-metal/servers/) and [plan documentation](https://deploy.equinix.com/developers/docs/metal/hardware/standard-servers/).
         """
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: pulumi.Input[Union[str, 'Plan']]):
         pulumi.set(self, "plan", value)
 
@@ -566,17 +564,16 @@
                equinix_metal_port,
                metal.DeviceNetworkType resources or
                metal.Port datasource.
                See network_types guide for more info.
         :param pulumi.Input[Union[str, 'OperatingSystem']] operating_system: The operating system slug. To find the slug, or visit
                [Operating Systems API docs](https://metal.equinix.com/developers/api/operatingsystems), set your
                API auth token in the top of the page and see JSON from the API response.
-        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit
-               [Device plans API docs](https://metal.equinix.com/developers/api/plans), set your auth token in the
-               top of the page and see JSON from the API response.
+        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit the
+               [bare-metal server](https://deploy.equinix.com/product/bare-metal/servers/) and [plan documentation](https://deploy.equinix.com/developers/docs/metal/hardware/standard-servers/).
         :param pulumi.Input[Sequence[pulumi.Input['DevicePortArgs']]] ports: List of ports assigned to the device. See Ports Attribute below for
                more details.
         :param pulumi.Input[str] project_id: The ID of the project in which to create the device
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_ssh_key_ids: Array of IDs of the project SSH keys which should be added to the device. If you specify this array, only the listed project SSH keys (and any SSH keys for the users specified in user_ssh_key_ids) will be added. If no SSH keys are specified (both user_ssh_keys_ids and project_ssh_key_ids are empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included.  Project SSH keys can be created with the metal.ProjectSshKey resource.
         :param pulumi.Input['DeviceReinstallArgs'] reinstall: Whether the device should be reinstalled instead of destroyed when
                modifying user_data, custom_data, or operating system. See Reinstall below for more
                details.
@@ -988,17 +985,16 @@
     def operating_system(self, value: Optional[pulumi.Input[Union[str, 'OperatingSystem']]]):
         pulumi.set(self, "operating_system", value)
 
     @property
     @pulumi.getter
     def plan(self) -> Optional[pulumi.Input[Union[str, 'Plan']]]:
         """
-        The device plan slug. To find the plan slug, visit
-        [Device plans API docs](https://metal.equinix.com/developers/api/plans), set your auth token in the
-        top of the page and see JSON from the API response.
+        The device plan slug. To find the plan slug, visit the
+        [bare-metal server](https://deploy.equinix.com/product/bare-metal/servers/) and [plan documentation](https://deploy.equinix.com/developers/docs/metal/hardware/standard-servers/).
         """
         return pulumi.get(self, "plan")
 
     @plan.setter
     def plan(self, value: Optional[pulumi.Input[Union[str, 'Plan']]]):
         pulumi.set(self, "plan", value)
 
@@ -1290,17 +1286,16 @@
         :param pulumi.Input[str] ipxe_script_url: URL pointing to a hosted iPXE script. More information is in the
                [Custom iPXE](https://metal.equinix.com/developers/docs/servers/custom-ipxe/) doc.
         :param pulumi.Input[bool] locked: Whether the device is locked or unlocked. Locking a device prevents you from deleting or reinstalling the device or performing a firmware update on the device, and it prevents an instance with a termination time set from being reclaimed, even if the termination time was reached
         :param pulumi.Input[str] metro: Metro area for the new device. Conflicts with `facilities`.
         :param pulumi.Input[Union[str, 'OperatingSystem']] operating_system: The operating system slug. To find the slug, or visit
                [Operating Systems API docs](https://metal.equinix.com/developers/api/operatingsystems), set your
                API auth token in the top of the page and see JSON from the API response.
-        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit
-               [Device plans API docs](https://metal.equinix.com/developers/api/plans), set your auth token in the
-               top of the page and see JSON from the API response.
+        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit the
+               [bare-metal server](https://deploy.equinix.com/product/bare-metal/servers/) and [plan documentation](https://deploy.equinix.com/developers/docs/metal/hardware/standard-servers/).
         :param pulumi.Input[str] project_id: The ID of the project in which to create the device
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_ssh_key_ids: Array of IDs of the project SSH keys which should be added to the device. If you specify this array, only the listed project SSH keys (and any SSH keys for the users specified in user_ssh_key_ids) will be added. If no SSH keys are specified (both user_ssh_keys_ids and project_ssh_key_ids are empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included.  Project SSH keys can be created with the metal.ProjectSshKey resource.
         :param pulumi.Input[pulumi.InputType['DeviceReinstallArgs']] reinstall: Whether the device should be reinstalled instead of destroyed when
                modifying user_data, custom_data, or operating system. See Reinstall below for more
                details.
         :param pulumi.Input[str] storage: JSON for custom partitioning. Only usable on reserved hardware. More
                information in in the
@@ -1552,17 +1547,16 @@
                equinix_metal_port,
                metal.DeviceNetworkType resources or
                metal.Port datasource.
                See network_types guide for more info.
         :param pulumi.Input[Union[str, 'OperatingSystem']] operating_system: The operating system slug. To find the slug, or visit
                [Operating Systems API docs](https://metal.equinix.com/developers/api/operatingsystems), set your
                API auth token in the top of the page and see JSON from the API response.
-        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit
-               [Device plans API docs](https://metal.equinix.com/developers/api/plans), set your auth token in the
-               top of the page and see JSON from the API response.
+        :param pulumi.Input[Union[str, 'Plan']] plan: The device plan slug. To find the plan slug, visit the
+               [bare-metal server](https://deploy.equinix.com/product/bare-metal/servers/) and [plan documentation](https://deploy.equinix.com/developers/docs/metal/hardware/standard-servers/).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DevicePortArgs']]]] ports: List of ports assigned to the device. See Ports Attribute below for
                more details.
         :param pulumi.Input[str] project_id: The ID of the project in which to create the device
         :param pulumi.Input[Sequence[pulumi.Input[str]]] project_ssh_key_ids: Array of IDs of the project SSH keys which should be added to the device. If you specify this array, only the listed project SSH keys (and any SSH keys for the users specified in user_ssh_key_ids) will be added. If no SSH keys are specified (both user_ssh_keys_ids and project_ssh_key_ids are empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included.  Project SSH keys can be created with the metal.ProjectSshKey resource.
         :param pulumi.Input[pulumi.InputType['DeviceReinstallArgs']] reinstall: Whether the device should be reinstalled instead of destroyed when
                modifying user_data, custom_data, or operating system. See Reinstall below for more
                details.
@@ -1844,17 +1838,16 @@
         """
         return pulumi.get(self, "operating_system")
 
     @property
     @pulumi.getter
     def plan(self) -> pulumi.Output[str]:
         """
-        The device plan slug. To find the plan slug, visit
-        [Device plans API docs](https://metal.equinix.com/developers/api/plans), set your auth token in the
-        top of the page and see JSON from the API response.
+        The device plan slug. To find the plan slug, visit the
+        [bare-metal server](https://deploy.equinix.com/product/bare-metal/servers/) and [plan documentation](https://deploy.equinix.com/developers/docs/metal/hardware/standard-servers/).
         """
         return pulumi.get(self, "plan")
 
     @property
     @pulumi.getter
     def ports(self) -> pulumi.Output[Sequence['outputs.DevicePort']]:
         """
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/device_network_type.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/device_network_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/gateway.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['GatewayTimeoutsArgs']]] = None,
                  vlan_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to create Metal Gateway resources in Equinix Metal.
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
@@ -264,15 +264,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: GatewayArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to create Metal Gateway resources in Equinix Metal.
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_device.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -332,34 +332,30 @@
 
     > **Note:** All arguments including the `root_password` and `user_data` will be stored in
      the raw state as plain-text.
     Read more about sensitive data in state.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(project_id=local["project_id"],
         hostname="mydevice")
     pulumi.export("id", test.id)
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("ipv4", test.access_public_ipv4)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device ID.
            
            > **NOTE:** You should pass either `device_id`, or both `project_id` and `hostname`.
     :param str hostname: The device name.
     :param str project_id: The id of the project in which the devices exists.
@@ -411,34 +407,30 @@
 
     > **Note:** All arguments including the `root_password` and `user_data` will be stored in
      the raw state as plain-text.
     Read more about sensitive data in state.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(project_id=local["project_id"],
         hostname="mydevice")
     pulumi.export("id", test.id)
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("ipv4", test.access_public_ipv4)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device ID.
            
            > **NOTE:** You should pass either `device_id`, or both `project_id` and `hostname`.
     :param str hostname: The device name.
     :param str project_id: The id of the project in which the devices exists.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_device_bgp_neighbors.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device_bgp_neighbors.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,23 +75,21 @@
     and have a BGP session assigned.
 
     To learn more about using BGP in Equinix Metal, see the
     metal.BgpSession resource documentation.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device_bgp_neighbors(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("bgpNeighborsListing", test.bgp_neighbors)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of BGP-enabled device whose neighbors to list.
     """
     __args__ = dict()
     __args__['deviceId'] = device_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -113,21 +111,19 @@
     and have a BGP session assigned.
 
     To learn more about using BGP in Equinix Metal, see the
     metal.BgpSession resource documentation.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device_bgp_neighbors(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("bgpNeighborsListing", test.bgp_neighbors)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of BGP-enabled device whose neighbors to list.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_devices.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_devices.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     """
     The datasource can be used to find a list of devices which meet filter criteria.
 
     If you need to fetch a single device by ID or by project ID and hostname, use the metal.Device datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(project_id=local["project_id"],
         filters=[
             equinix.metal.GetDevicesFilterArgs(
@@ -133,25 +132,22 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("devices", example.devices)
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(search="database")
     pulumi.export("devices", example.devices)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## search vs filter
 
     The difference between `search` and `filter` is that `search` is an API parameter, interpreted by the Equinix Metal service. The "filter" arguments will reduce the API list (or search) results by applying client-side filtering, within this provider.
 
 
     :param Sequence[pulumi.InputType['GetDevicesFilterArgs']] filters: One or more attribute/values pairs to filter. List of atributes to filter can be found in the attribute reference of the `metal.Device` datasource.
@@ -188,15 +184,14 @@
     """
     The datasource can be used to find a list of devices which meet filter criteria.
 
     If you need to fetch a single device by ID or by project ID and hostname, use the metal.Device datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(project_id=local["project_id"],
         filters=[
             equinix.metal.GetDevicesFilterArgs(
@@ -209,25 +204,22 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("devices", example.devices)
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(search="database")
     pulumi.export("devices", example.devices)
     ```
-    <!--End PulumiCodeChooser -->
 
     ## search vs filter
 
     The difference between `search` and `filter` is that `search` is an API parameter, interpreted by the Equinix Metal service. The "filter" arguments will reduce the API list (or search) results by applying client-side filtering, within this provider.
 
 
     :param Sequence[pulumi.InputType['GetDevicesFilterArgs']] filters: One or more attribute/values pairs to filter. List of atributes to filter can be found in the attribute reference of the `metal.Device` datasource.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_facility.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,181 +4,181 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
-from ._inputs import *
 
 __all__ = [
-    'GetFacilityResult',
-    'AwaitableGetFacilityResult',
-    'get_facility',
-    'get_facility_output',
+    'GetDeviceTypeResult',
+    'AwaitableGetDeviceTypeResult',
+    'get_device_type',
+    'get_device_type_output',
 ]
 
 @pulumi.output_type
-class GetFacilityResult:
+class GetDeviceTypeResult:
     """
-    A collection of values returned by getFacility.
+    A collection of values returned by getDeviceType.
     """
-    def __init__(__self__, capacities=None, code=None, features=None, features_requireds=None, id=None, metro=None, name=None):
-        if capacities and not isinstance(capacities, list):
-            raise TypeError("Expected argument 'capacities' to be a list")
-        pulumi.set(__self__, "capacities", capacities)
+    def __init__(__self__, category=None, code=None, description=None, id=None, metro_codes=None, name=None, vendor=None):
+        if category and not isinstance(category, str):
+            raise TypeError("Expected argument 'category' to be a str")
+        pulumi.set(__self__, "category", category)
         if code and not isinstance(code, str):
             raise TypeError("Expected argument 'code' to be a str")
         pulumi.set(__self__, "code", code)
-        if features and not isinstance(features, list):
-            raise TypeError("Expected argument 'features' to be a list")
-        pulumi.set(__self__, "features", features)
-        if features_requireds and not isinstance(features_requireds, list):
-            raise TypeError("Expected argument 'features_requireds' to be a list")
-        pulumi.set(__self__, "features_requireds", features_requireds)
+        if description and not isinstance(description, str):
+            raise TypeError("Expected argument 'description' to be a str")
+        pulumi.set(__self__, "description", description)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if metro and not isinstance(metro, str):
-            raise TypeError("Expected argument 'metro' to be a str")
-        pulumi.set(__self__, "metro", metro)
+        if metro_codes and not isinstance(metro_codes, list):
+            raise TypeError("Expected argument 'metro_codes' to be a list")
+        pulumi.set(__self__, "metro_codes", metro_codes)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
+        if vendor and not isinstance(vendor, str):
+            raise TypeError("Expected argument 'vendor' to be a str")
+        pulumi.set(__self__, "vendor", vendor)
 
     @property
     @pulumi.getter
-    def capacities(self) -> Optional[Sequence['outputs.GetFacilityCapacityResult']]:
-        return pulumi.get(self, "capacities")
+    def category(self) -> str:
+        return pulumi.get(self, "category")
 
     @property
     @pulumi.getter
     def code(self) -> str:
+        """
+        Device type short code, unique identifier of a network device type
+        """
         return pulumi.get(self, "code")
 
     @property
     @pulumi.getter
-    def features(self) -> Sequence[str]:
+    def description(self) -> str:
         """
-        The features of the facility.
+        Device type textual description
         """
-        return pulumi.get(self, "features")
-
-    @property
-    @pulumi.getter(name="featuresRequireds")
-    def features_requireds(self) -> Optional[Sequence[str]]:
-        return pulumi.get(self, "features_requireds")
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter
-    def metro(self) -> str:
-        """
-        The metro code the facility is part of.
-        """
-        return pulumi.get(self, "metro")
+    @pulumi.getter(name="metroCodes")
+    def metro_codes(self) -> Sequence[str]:
+        return pulumi.get(self, "metro_codes")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        The name of the facility.
-        """
         return pulumi.get(self, "name")
 
+    @property
+    @pulumi.getter
+    def vendor(self) -> str:
+        return pulumi.get(self, "vendor")
 
-class AwaitableGetFacilityResult(GetFacilityResult):
+
+class AwaitableGetDeviceTypeResult(GetDeviceTypeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetFacilityResult(
-            capacities=self.capacities,
+        return GetDeviceTypeResult(
+            category=self.category,
             code=self.code,
-            features=self.features,
-            features_requireds=self.features_requireds,
+            description=self.description,
             id=self.id,
-            metro=self.metro,
-            name=self.name)
+            metro_codes=self.metro_codes,
+            name=self.name,
+            vendor=self.vendor)
 
 
-def get_facility(capacities: Optional[Sequence[pulumi.InputType['GetFacilityCapacityArgs']]] = None,
-                 code: Optional[str] = None,
-                 features_requireds: Optional[Sequence[str]] = None,
-                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFacilityResult:
+def get_device_type(category: Optional[str] = None,
+                    metro_codes: Optional[Sequence[str]] = None,
+                    name: Optional[str] = None,
+                    vendor: Optional[str] = None,
+                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDeviceTypeResult:
     """
-    > **Deprecated** Use `metal_get_metro` instead.  For more information, refer to the facility to metro migration guide.
-
-    Provides an Equinix Metal facility datasource.
+    Use this data source to get Equinix Network Edge device type details. For further details, check supported
+    [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    ny5 = equinix.metal.get_facility(code="ny5")
-    pulumi.export("id", ny5.id)
+    cisco_router = equinix.networkedge.get_device_type(category="Router",
+        metro_codes=[
+            "DC",
+            "SV",
+        ],
+        vendor="Cisco")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
-    :param str code: The facility code to search for facilities.
-    :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
-           possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
+    :param str category: Device type category. One of: `Router`, `Firewall`, `SDWAN`.
+    :param Sequence[str] metro_codes: List of metro codes where device type has to be available
+    :param str name: Device type name.
+    :param str vendor: Device type vendor i.e. `Cisco`, `Juniper Networks`, `VERSA Networks`.
     """
     __args__ = dict()
-    __args__['capacities'] = capacities
-    __args__['code'] = code
-    __args__['featuresRequireds'] = features_requireds
+    __args__['category'] = category
+    __args__['metroCodes'] = metro_codes
+    __args__['name'] = name
+    __args__['vendor'] = vendor
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:metal/getFacility:getFacility', __args__, opts=opts, typ=GetFacilityResult).value
+    __ret__ = pulumi.runtime.invoke('equinix:networkedge/getDeviceType:getDeviceType', __args__, opts=opts, typ=GetDeviceTypeResult).value
 
-    return AwaitableGetFacilityResult(
-        capacities=pulumi.get(__ret__, 'capacities'),
+    return AwaitableGetDeviceTypeResult(
+        category=pulumi.get(__ret__, 'category'),
         code=pulumi.get(__ret__, 'code'),
-        features=pulumi.get(__ret__, 'features'),
-        features_requireds=pulumi.get(__ret__, 'features_requireds'),
+        description=pulumi.get(__ret__, 'description'),
         id=pulumi.get(__ret__, 'id'),
-        metro=pulumi.get(__ret__, 'metro'),
-        name=pulumi.get(__ret__, 'name'))
+        metro_codes=pulumi.get(__ret__, 'metro_codes'),
+        name=pulumi.get(__ret__, 'name'),
+        vendor=pulumi.get(__ret__, 'vendor'))
 
 
-@_utilities.lift_output_func(get_facility)
-def get_facility_output(capacities: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetFacilityCapacityArgs']]]]] = None,
-                        code: Optional[pulumi.Input[str]] = None,
-                        features_requireds: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFacilityResult]:
+@_utilities.lift_output_func(get_device_type)
+def get_device_type_output(category: Optional[pulumi.Input[Optional[str]]] = None,
+                           metro_codes: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
+                           name: Optional[pulumi.Input[Optional[str]]] = None,
+                           vendor: Optional[pulumi.Input[Optional[str]]] = None,
+                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDeviceTypeResult]:
     """
-    > **Deprecated** Use `metal_get_metro` instead.  For more information, refer to the facility to metro migration guide.
-
-    Provides an Equinix Metal facility datasource.
+    Use this data source to get Equinix Network Edge device type details. For further details, check supported
+    [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    ny5 = equinix.metal.get_facility(code="ny5")
-    pulumi.export("id", ny5.id)
+    cisco_router = equinix.networkedge.get_device_type(category="Router",
+        metro_codes=[
+            "DC",
+            "SV",
+        ],
+        vendor="Cisco")
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
-    :param str code: The facility code to search for facilities.
-    :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
-           possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
+    :param str category: Device type category. One of: `Router`, `Firewall`, `SDWAN`.
+    :param Sequence[str] metro_codes: List of metro codes where device type has to be available
+    :param str name: Device type name.
+    :param str vendor: Device type vendor i.e. `Cisco`, `Juniper Networks`, `VERSA Networks`.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_gateway.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_gateway.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,31 +124,29 @@
 
 
 def get_gateway(gateway_id: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGatewayResult:
     """
     Use this datasource to retrieve Metal Gateway resources in Equinix Metal.
 
-    > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     # Create Metal Gateway for a VLAN with a private IPv4 block with 8 IP addresses
     test_vlan = equinix.metal.Vlan("testVlan",
         description="test VLAN in SV",
         metro="sv",
         project_id=local["project_id"])
     test_gateway = equinix.metal.get_gateway(gateway_id=local["gateway_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str gateway_id: UUID of the metal gateway resource to retrieve.
     """
     __args__ = dict()
     __args__['gatewayId'] = gateway_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -167,29 +165,27 @@
 
 @_utilities.lift_output_func(get_gateway)
 def get_gateway_output(gateway_id: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGatewayResult]:
     """
     Use this datasource to retrieve Metal Gateway resources in Equinix Metal.
 
-    > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     # Create Metal Gateway for a VLAN with a private IPv4 block with 8 IP addresses
     test_vlan = equinix.metal.Vlan("testVlan",
         description="test VLAN in SV",
         metro="sv",
         project_id=local["project_id"])
     test_gateway = equinix.metal.get_gateway(gateway_id=local["gateway_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str gateway_id: UUID of the metal gateway resource to retrieve.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_hardware_reservation.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_hardware_reservation.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,23 +152,21 @@
     """
     Use this data source to retrieve a [hardware reservation resource from Equinix Metal](https://metal.equinix.com/developers/docs/deploy/reserved/).
 
     You can look up hardware reservation by its ID or by ID of device which occupies it.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_hardware_reservation(id="4347e805-eb46-4699-9eb9-5c116e6a0172")
     example_by_device_id = equinix.metal.get_hardware_reservation(device_id="ff85aa58-c106-4624-8f1c-7c64554047ea")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of device occupying the reservation.
     :param str id: ID of the hardware reservation.
     """
     __args__ = dict()
     __args__['deviceId'] = device_id
@@ -195,22 +193,20 @@
     """
     Use this data source to retrieve a [hardware reservation resource from Equinix Metal](https://metal.equinix.com/developers/docs/deploy/reserved/).
 
     You can look up hardware reservation by its ID or by ID of device which occupies it.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_hardware_reservation(id="4347e805-eb46-4699-9eb9-5c116e6a0172")
     example_by_device_id = equinix.metal.get_hardware_reservation(device_id="ff85aa58-c106-4624-8f1c-7c64554047ea")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of device occupying the reservation.
     :param str id: ID of the hardware reservation.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_interconnection.py` & `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,364 +7,363 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 
 __all__ = [
-    'GetInterconnectionResult',
-    'AwaitableGetInterconnectionResult',
-    'get_interconnection',
-    'get_interconnection_output',
+    'GetConnectionResult',
+    'AwaitableGetConnectionResult',
+    'get_connection',
+    'get_connection_output',
 ]
 
 @pulumi.output_type
-class GetInterconnectionResult:
+class GetConnectionResult:
     """
-    A collection of values returned by getInterconnection.
+    A collection of values returned by getConnection.
     """
-    def __init__(__self__, authorization_code=None, connection_id=None, contact_email=None, description=None, facility=None, id=None, metro=None, mode=None, name=None, organization_id=None, ports=None, project_id=None, redundancy=None, service_token_type=None, service_tokens=None, speed=None, status=None, tags=None, token=None, type=None, vlans=None, vrfs=None):
-        if authorization_code and not isinstance(authorization_code, str):
-            raise TypeError("Expected argument 'authorization_code' to be a str")
-        pulumi.set(__self__, "authorization_code", authorization_code)
-        if connection_id and not isinstance(connection_id, str):
-            raise TypeError("Expected argument 'connection_id' to be a str")
-        pulumi.set(__self__, "connection_id", connection_id)
-        if contact_email and not isinstance(contact_email, str):
-            raise TypeError("Expected argument 'contact_email' to be a str")
-        pulumi.set(__self__, "contact_email", contact_email)
+    def __init__(__self__, a_side=None, account=None, additional_info=None, bandwidth=None, change_log=None, description=None, direction=None, href=None, id=None, is_remote=None, name=None, notifications=None, operation=None, order=None, project=None, redundancy=None, state=None, type=None, uuid=None, z_side=None):
+        if a_side and not isinstance(a_side, dict):
+            raise TypeError("Expected argument 'a_side' to be a dict")
+        pulumi.set(__self__, "a_side", a_side)
+        if account and not isinstance(account, dict):
+            raise TypeError("Expected argument 'account' to be a dict")
+        pulumi.set(__self__, "account", account)
+        if additional_info and not isinstance(additional_info, list):
+            raise TypeError("Expected argument 'additional_info' to be a list")
+        pulumi.set(__self__, "additional_info", additional_info)
+        if bandwidth and not isinstance(bandwidth, int):
+            raise TypeError("Expected argument 'bandwidth' to be a int")
+        pulumi.set(__self__, "bandwidth", bandwidth)
+        if change_log and not isinstance(change_log, dict):
+            raise TypeError("Expected argument 'change_log' to be a dict")
+        pulumi.set(__self__, "change_log", change_log)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
-        if facility and not isinstance(facility, str):
-            raise TypeError("Expected argument 'facility' to be a str")
-        pulumi.set(__self__, "facility", facility)
+        if direction and not isinstance(direction, str):
+            raise TypeError("Expected argument 'direction' to be a str")
+        pulumi.set(__self__, "direction", direction)
+        if href and not isinstance(href, str):
+            raise TypeError("Expected argument 'href' to be a str")
+        pulumi.set(__self__, "href", href)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if metro and not isinstance(metro, str):
-            raise TypeError("Expected argument 'metro' to be a str")
-        pulumi.set(__self__, "metro", metro)
-        if mode and not isinstance(mode, str):
-            raise TypeError("Expected argument 'mode' to be a str")
-        pulumi.set(__self__, "mode", mode)
+        if is_remote and not isinstance(is_remote, bool):
+            raise TypeError("Expected argument 'is_remote' to be a bool")
+        pulumi.set(__self__, "is_remote", is_remote)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
-        if organization_id and not isinstance(organization_id, str):
-            raise TypeError("Expected argument 'organization_id' to be a str")
-        pulumi.set(__self__, "organization_id", organization_id)
-        if ports and not isinstance(ports, list):
-            raise TypeError("Expected argument 'ports' to be a list")
-        pulumi.set(__self__, "ports", ports)
-        if project_id and not isinstance(project_id, str):
-            raise TypeError("Expected argument 'project_id' to be a str")
-        pulumi.set(__self__, "project_id", project_id)
-        if redundancy and not isinstance(redundancy, str):
-            raise TypeError("Expected argument 'redundancy' to be a str")
+        if notifications and not isinstance(notifications, list):
+            raise TypeError("Expected argument 'notifications' to be a list")
+        pulumi.set(__self__, "notifications", notifications)
+        if operation and not isinstance(operation, dict):
+            raise TypeError("Expected argument 'operation' to be a dict")
+        pulumi.set(__self__, "operation", operation)
+        if order and not isinstance(order, dict):
+            raise TypeError("Expected argument 'order' to be a dict")
+        pulumi.set(__self__, "order", order)
+        if project and not isinstance(project, dict):
+            raise TypeError("Expected argument 'project' to be a dict")
+        pulumi.set(__self__, "project", project)
+        if redundancy and not isinstance(redundancy, dict):
+            raise TypeError("Expected argument 'redundancy' to be a dict")
         pulumi.set(__self__, "redundancy", redundancy)
-        if service_token_type and not isinstance(service_token_type, str):
-            raise TypeError("Expected argument 'service_token_type' to be a str")
-        pulumi.set(__self__, "service_token_type", service_token_type)
-        if service_tokens and not isinstance(service_tokens, list):
-            raise TypeError("Expected argument 'service_tokens' to be a list")
-        pulumi.set(__self__, "service_tokens", service_tokens)
-        if speed and not isinstance(speed, str):
-            raise TypeError("Expected argument 'speed' to be a str")
-        pulumi.set(__self__, "speed", speed)
-        if status and not isinstance(status, str):
-            raise TypeError("Expected argument 'status' to be a str")
-        pulumi.set(__self__, "status", status)
-        if tags and not isinstance(tags, list):
-            raise TypeError("Expected argument 'tags' to be a list")
-        pulumi.set(__self__, "tags", tags)
-        if token and not isinstance(token, str):
-            raise TypeError("Expected argument 'token' to be a str")
-        pulumi.set(__self__, "token", token)
+        if state and not isinstance(state, str):
+            raise TypeError("Expected argument 'state' to be a str")
+        pulumi.set(__self__, "state", state)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
-        if vlans and not isinstance(vlans, list):
-            raise TypeError("Expected argument 'vlans' to be a list")
-        pulumi.set(__self__, "vlans", vlans)
-        if vrfs and not isinstance(vrfs, list):
-            raise TypeError("Expected argument 'vrfs' to be a list")
-        pulumi.set(__self__, "vrfs", vrfs)
+        if uuid and not isinstance(uuid, str):
+            raise TypeError("Expected argument 'uuid' to be a str")
+        pulumi.set(__self__, "uuid", uuid)
+        if z_side and not isinstance(z_side, dict):
+            raise TypeError("Expected argument 'z_side' to be a dict")
+        pulumi.set(__self__, "z_side", z_side)
 
     @property
-    @pulumi.getter(name="authorizationCode")
-    def authorization_code(self) -> str:
-        return pulumi.get(self, "authorization_code")
-
-    @property
-    @pulumi.getter(name="connectionId")
-    def connection_id(self) -> str:
-        return pulumi.get(self, "connection_id")
-
-    @property
-    @pulumi.getter(name="contactEmail")
-    def contact_email(self) -> str:
+    @pulumi.getter(name="aSide")
+    def a_side(self) -> 'outputs.GetConnectionASideResult':
         """
-        The preferred email used for communication and notifications about the Equinix Fabric interconnection.
+        Requester or Customer side connection configuration object of the multi-segment connection
         """
-        return pulumi.get(self, "contact_email")
+        return pulumi.get(self, "a_side")
 
     @property
     @pulumi.getter
-    def description(self) -> str:
+    def account(self) -> 'outputs.GetConnectionAccountResult':
         """
-        Description of the connection resource.
+        Customer account information that is associated with this connection
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "account")
 
     @property
-    @pulumi.getter
-    def facility(self) -> str:
+    @pulumi.getter(name="additionalInfo")
+    def additional_info(self) -> Sequence[Mapping[str, Any]]:
         """
-        (**Deprecated**) Slug of a facility to which the connection belongs. Use metro instead; read the facility to metro migration guide
+        Connection additional information
         """
-        warnings.warn("""Use metro instead of facility. For more information, read the migration guide.""", DeprecationWarning)
-        pulumi.log.warn("""facility is deprecated: Use metro instead of facility. For more information, read the migration guide.""")
-
-        return pulumi.get(self, "facility")
+        return pulumi.get(self, "additional_info")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def bandwidth(self) -> int:
         """
-        Port UUID.
+        Connection bandwidth in Mbps
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "bandwidth")
 
     @property
-    @pulumi.getter
-    def metro(self) -> str:
+    @pulumi.getter(name="changeLog")
+    def change_log(self) -> 'outputs.GetConnectionChangeLogResult':
         """
-        Slug of a metro to which the connection belongs.
+        Captures connection lifecycle change information
         """
-        return pulumi.get(self, "metro")
+        return pulumi.get(self, "change_log")
 
     @property
     @pulumi.getter
-    def mode(self) -> str:
+    def description(self) -> str:
         """
-        Mode for connections in IBX facilities with the dedicated type - standard or tunnel.
+        Customer-provided connection description
         """
-        return pulumi.get(self, "mode")
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def direction(self) -> str:
         """
-        Port name.
+        Connection directionality from the requester point of view
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "direction")
 
     @property
-    @pulumi.getter(name="organizationId")
-    def organization_id(self) -> str:
+    @pulumi.getter
+    def href(self) -> str:
         """
-        ID of the organization where the connection is scoped to.
+        Connection URI information
         """
-        return pulumi.get(self, "organization_id")
+        return pulumi.get(self, "href")
 
     @property
     @pulumi.getter
-    def ports(self) -> Sequence['outputs.GetInterconnectionPortResult']:
+    def id(self) -> str:
         """
-        List of connection ports - primary (`ports[0]`) and secondary (`ports[1]`)
+        The provider-assigned unique ID for this managed resource.
         """
-        return pulumi.get(self, "ports")
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> str:
+    @pulumi.getter(name="isRemote")
+    def is_remote(self) -> bool:
         """
-        ID of project to which the connection belongs.
+        Connection property derived from access point locations
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "is_remote")
 
     @property
     @pulumi.getter
-    def redundancy(self) -> str:
+    def name(self) -> str:
         """
-        Connection redundancy, reduntant or primary.
+        Connection name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         """
-        return pulumi.get(self, "redundancy")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="serviceTokenType")
-    def service_token_type(self) -> str:
+    @pulumi.getter
+    def notifications(self) -> Sequence['outputs.GetConnectionNotificationResult']:
         """
-        Type of service token, a_side or z_side. One available in shared connection.
+        Preferences for notifications on connection configuration or status changes
         """
-        return pulumi.get(self, "service_token_type")
+        return pulumi.get(self, "notifications")
 
     @property
-    @pulumi.getter(name="serviceTokens")
-    def service_tokens(self) -> Sequence['outputs.GetInterconnectionServiceTokenResult']:
+    @pulumi.getter
+    def operation(self) -> 'outputs.GetConnectionOperationResult':
         """
-        List of connection service tokens with attributes
+        Connection type-specific operational data
         """
-        return pulumi.get(self, "service_tokens")
+        return pulumi.get(self, "operation")
 
     @property
     @pulumi.getter
-    def speed(self) -> str:
+    def order(self) -> 'outputs.GetConnectionOrderResult':
         """
-        Port speed in bits per second.
+        Order details
         """
-        return pulumi.get(self, "speed")
+        return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
-    def status(self) -> str:
+    def project(self) -> 'outputs.GetConnectionProjectResult':
         """
-        Port status.
+        Project information
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "project")
 
     @property
     @pulumi.getter
-    def tags(self) -> Sequence[str]:
+    def redundancy(self) -> 'outputs.GetConnectionRedundancyResult':
         """
-        String list of tags.
+        Connection Redundancy Configuration
         """
-        return pulumi.get(self, "tags")
+        return pulumi.get(self, "redundancy")
 
     @property
     @pulumi.getter
-    def token(self) -> str:
+    def state(self) -> str:
         """
-        (Deprecated) Fabric Token required to configure the connection in Equinix Fabric with the equinix_ecx_l2_connection resource or from the [Equinix Fabric Portal](https://ecxfabric.equinix.com/dashboard). If your organization already has connection service tokens enabled, use `service_tokens` instead.
+        Connection overall state
         """
-        warnings.warn("""If your organization already has connection service tokens enabled, use `service_tokens` instead""", DeprecationWarning)
-        pulumi.log.warn("""token is deprecated: If your organization already has connection service tokens enabled, use `service_tokens` instead""")
-
-        return pulumi.get(self, "token")
+        return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        Token type, `a_side` or `z_side`.
+        Defines the connection type like EVPL*VC, EPL*VC, IPWAN*VC, IP*VC, ACCESS*EPL*VC, EVPLAN*VC, EPLAN*VC, EIA*VC, EC*VC
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
-    def vlans(self) -> Sequence[int]:
+    def uuid(self) -> str:
         """
-        Attached VLANs. Only available in shared connection. One vlan for Primary/Single connection and two vlans for Redundant connection.
+        Equinix-assigned connection identifier
         """
-        return pulumi.get(self, "vlans")
+        return pulumi.get(self, "uuid")
 
     @property
-    @pulumi.getter
-    def vrfs(self) -> Sequence[str]:
-        return pulumi.get(self, "vrfs")
+    @pulumi.getter(name="zSide")
+    def z_side(self) -> 'outputs.GetConnectionZSideResult':
+        """
+        Destination or Provider side connection configuration object of the multi-segment connection
+        """
+        return pulumi.get(self, "z_side")
 
 
-class AwaitableGetInterconnectionResult(GetInterconnectionResult):
+class AwaitableGetConnectionResult(GetConnectionResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetInterconnectionResult(
-            authorization_code=self.authorization_code,
-            connection_id=self.connection_id,
-            contact_email=self.contact_email,
+        return GetConnectionResult(
+            a_side=self.a_side,
+            account=self.account,
+            additional_info=self.additional_info,
+            bandwidth=self.bandwidth,
+            change_log=self.change_log,
             description=self.description,
-            facility=self.facility,
+            direction=self.direction,
+            href=self.href,
             id=self.id,
-            metro=self.metro,
-            mode=self.mode,
+            is_remote=self.is_remote,
             name=self.name,
-            organization_id=self.organization_id,
-            ports=self.ports,
-            project_id=self.project_id,
+            notifications=self.notifications,
+            operation=self.operation,
+            order=self.order,
+            project=self.project,
             redundancy=self.redundancy,
-            service_token_type=self.service_token_type,
-            service_tokens=self.service_tokens,
-            speed=self.speed,
-            status=self.status,
-            tags=self.tags,
-            token=self.token,
+            state=self.state,
             type=self.type,
-            vlans=self.vlans,
-            vrfs=self.vrfs)
+            uuid=self.uuid,
+            z_side=self.z_side)
 
 
-def get_interconnection(connection_id: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInterconnectionResult:
+def get_connection(uuid: Optional[str] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetConnectionResult:
     """
-    Use this data source to retrieve a [connection resource](https://metal.equinix.com/developers/docs/networking/fabric/)
-
-    > Equinix Metal connection with with Service Token A-side / Z-side (service_token_type) is not generally available and may not be enabled yet for your organization.
+    Fabric V4 API compatible data resource that allow user to fetch connection for a given UUID
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    example = equinix.metal.get_interconnection(connection_id="4347e805-eb46-4699-9eb9-5c116e6a017d")
+    connection_data_name = equinix.fabric.get_connection(uuid="<uuid_of_connection>")
+    pulumi.export("id", connection_data_name.id)
+    pulumi.export("name", connection_data_name.bandwidth)
+    pulumi.export("accountNumber", connection_data_name.account.account_number)
+    pulumi.export("bandwidth", connection_data_name.bandwidth)
+    pulumi.export("projectId", connection_data_name.project.project_id)
+    pulumi.export("redundancyGroup", connection_data_name.redundancy.group)
+    pulumi.export("redundancyPriority", connection_data_name.redundancy.priority)
+    pulumi.export("state", connection_data_name.state)
+    pulumi.export("type", connection_data_name.type)
+    pulumi.export("accessPointType", connection_data_name.a_side.access_point.type)
+    pulumi.export("accessPointLinkProtocolType", connection_data_name.a_side.access_point.link_protocol.type)
+    pulumi.export("accessPointLinkProtocolVlanTag", connection_data_name.a_side.access_point.link_protocol.vlan_tag)
+    pulumi.export("accessPointLinkProtocolVlanCTag", connection_data_name.a_side.access_point.link_protocol.vlan_c_tag)
+    pulumi.export("accessPointLinkProtocolVlanSTag", connection_data_name.a_side.access_point.link_protocol.vlan_s_tag)
+    pulumi.export("accessPointProviderConnectionId", connection_data_name.a_side.access_point.provider_connection_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str connection_id: ID of the connection resource.
+    :param str uuid: Equinix-assigned connection identifier
     """
     __args__ = dict()
-    __args__['connectionId'] = connection_id
+    __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:metal/getInterconnection:getInterconnection', __args__, opts=opts, typ=GetInterconnectionResult).value
+    __ret__ = pulumi.runtime.invoke('equinix:fabric/getConnection:getConnection', __args__, opts=opts, typ=GetConnectionResult).value
 
-    return AwaitableGetInterconnectionResult(
-        authorization_code=pulumi.get(__ret__, 'authorization_code'),
-        connection_id=pulumi.get(__ret__, 'connection_id'),
-        contact_email=pulumi.get(__ret__, 'contact_email'),
+    return AwaitableGetConnectionResult(
+        a_side=pulumi.get(__ret__, 'a_side'),
+        account=pulumi.get(__ret__, 'account'),
+        additional_info=pulumi.get(__ret__, 'additional_info'),
+        bandwidth=pulumi.get(__ret__, 'bandwidth'),
+        change_log=pulumi.get(__ret__, 'change_log'),
         description=pulumi.get(__ret__, 'description'),
-        facility=pulumi.get(__ret__, 'facility'),
+        direction=pulumi.get(__ret__, 'direction'),
+        href=pulumi.get(__ret__, 'href'),
         id=pulumi.get(__ret__, 'id'),
-        metro=pulumi.get(__ret__, 'metro'),
-        mode=pulumi.get(__ret__, 'mode'),
+        is_remote=pulumi.get(__ret__, 'is_remote'),
         name=pulumi.get(__ret__, 'name'),
-        organization_id=pulumi.get(__ret__, 'organization_id'),
-        ports=pulumi.get(__ret__, 'ports'),
-        project_id=pulumi.get(__ret__, 'project_id'),
+        notifications=pulumi.get(__ret__, 'notifications'),
+        operation=pulumi.get(__ret__, 'operation'),
+        order=pulumi.get(__ret__, 'order'),
+        project=pulumi.get(__ret__, 'project'),
         redundancy=pulumi.get(__ret__, 'redundancy'),
-        service_token_type=pulumi.get(__ret__, 'service_token_type'),
-        service_tokens=pulumi.get(__ret__, 'service_tokens'),
-        speed=pulumi.get(__ret__, 'speed'),
-        status=pulumi.get(__ret__, 'status'),
-        tags=pulumi.get(__ret__, 'tags'),
-        token=pulumi.get(__ret__, 'token'),
+        state=pulumi.get(__ret__, 'state'),
         type=pulumi.get(__ret__, 'type'),
-        vlans=pulumi.get(__ret__, 'vlans'),
-        vrfs=pulumi.get(__ret__, 'vrfs'))
+        uuid=pulumi.get(__ret__, 'uuid'),
+        z_side=pulumi.get(__ret__, 'z_side'))
 
 
-@_utilities.lift_output_func(get_interconnection)
-def get_interconnection_output(connection_id: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInterconnectionResult]:
+@_utilities.lift_output_func(get_connection)
+def get_connection_output(uuid: Optional[pulumi.Input[str]] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetConnectionResult]:
     """
-    Use this data source to retrieve a [connection resource](https://metal.equinix.com/developers/docs/networking/fabric/)
-
-    > Equinix Metal connection with with Service Token A-side / Z-side (service_token_type) is not generally available and may not be enabled yet for your organization.
+    Fabric V4 API compatible data resource that allow user to fetch connection for a given UUID
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
-    example = equinix.metal.get_interconnection(connection_id="4347e805-eb46-4699-9eb9-5c116e6a017d")
+    connection_data_name = equinix.fabric.get_connection(uuid="<uuid_of_connection>")
+    pulumi.export("id", connection_data_name.id)
+    pulumi.export("name", connection_data_name.bandwidth)
+    pulumi.export("accountNumber", connection_data_name.account.account_number)
+    pulumi.export("bandwidth", connection_data_name.bandwidth)
+    pulumi.export("projectId", connection_data_name.project.project_id)
+    pulumi.export("redundancyGroup", connection_data_name.redundancy.group)
+    pulumi.export("redundancyPriority", connection_data_name.redundancy.priority)
+    pulumi.export("state", connection_data_name.state)
+    pulumi.export("type", connection_data_name.type)
+    pulumi.export("accessPointType", connection_data_name.a_side.access_point.type)
+    pulumi.export("accessPointLinkProtocolType", connection_data_name.a_side.access_point.link_protocol.type)
+    pulumi.export("accessPointLinkProtocolVlanTag", connection_data_name.a_side.access_point.link_protocol.vlan_tag)
+    pulumi.export("accessPointLinkProtocolVlanCTag", connection_data_name.a_side.access_point.link_protocol.vlan_c_tag)
+    pulumi.export("accessPointLinkProtocolVlanSTag", connection_data_name.a_side.access_point.link_protocol.vlan_s_tag)
+    pulumi.export("accessPointProviderConnectionId", connection_data_name.a_side.access_point.provider_connection_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
-    :param str connection_id: ID of the connection resource.
+    :param str uuid: Equinix-assigned connection identifier
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_ip_block_ranges.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_ip_block_ranges.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,24 +131,22 @@
 
     There are four types of IP blocks in Equinix: equinix_metal_global IPv4, public IPv4, private IPv4 and IPv6. Both global and public IPv4 are routable from the Internet. Public IPv4 blocks are allocated in a facility or metro, and addresses from it can only be assigned to devices in that location. Addresses from Global IPv4 block can be assigned to a device in any metro.
 
     The datasource has 4 list attributes: `global_ipv4`, `public_ipv4`, `private_ipv4` and `ipv6`, each listing CIDR notation (`<network>/<mask>`) of respective blocks from the project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test = equinix.metal.get_ip_block_ranges(project_id=project_id)
     pulumi.export("out", test)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and metro, all the block from the project will be listed.   Use metro instead; read the facility to metro migration guide
     :param str metro: Metro code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and facility, all the block from the project will be listed.
     :param str project_id: ID of the project from which to list the blocks.
@@ -181,24 +179,22 @@
 
     There are four types of IP blocks in Equinix: equinix_metal_global IPv4, public IPv4, private IPv4 and IPv6. Both global and public IPv4 are routable from the Internet. Public IPv4 blocks are allocated in a facility or metro, and addresses from it can only be assigned to devices in that location. Addresses from Global IPv4 block can be assigned to a device in any metro.
 
     The datasource has 4 list attributes: `global_ipv4`, `public_ipv4`, `private_ipv4` and `ipv6`, each listing CIDR notation (`<network>/<mask>`) of respective blocks from the project.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test = equinix.metal.get_ip_block_ranges(project_id=project_id)
     pulumi.export("out", test)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and metro, all the block from the project will be listed.   Use metro instead; read the facility to metro migration guide
     :param str metro: Metro code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and facility, all the block from the project will be listed.
     :param str project_id: ID of the project from which to list the blocks.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_metro.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_metro.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,23 +92,21 @@
               code: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMetroResult:
     """
     Provides an Equinix Metal metro datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     sv = equinix.metal.get_metro(code="sv")
     pulumi.export("id", sv.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the metro must have capacity.
     :param str code: The metro code to search for.
     """
     __args__ = dict()
     __args__['capacities'] = capacities
@@ -129,22 +127,20 @@
                      code: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetroResult]:
     """
     Provides an Equinix Metal metro datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     sv = equinix.metal.get_metro(code="sv")
     pulumi.export("id", sv.id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the metro must have capacity.
     :param str code: The metro code to search for.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_operating_system.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_operating_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,14 @@
                          version: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOperatingSystemResult:
     """
     Use this data source to get Equinix Metal Operating System image.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_operating_system(distro="ubuntu",
         version="20.04",
         provisionable_on="c3.medium.x86")
@@ -114,15 +113,14 @@
         hostname="tf.ubuntu",
         plan=equinix.metal.Plan.C3_MEDIUM_X86,
         metro="ny",
         operating_system=example.id.apply(lambda x: equinix.metal.OperatingSystem(x)),
         billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=local["project_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str distro: Name of the OS distribution.
     :param str name: Name or part of the name of the distribution. Case insensitive.
     :param str provisionable_on: Plan name.
     :param str version: Version of the distribution.
     """
@@ -150,15 +148,14 @@
                                 version: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOperatingSystemResult]:
     """
     Use this data source to get Equinix Metal Operating System image.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_operating_system(distro="ubuntu",
         version="20.04",
         provisionable_on="c3.medium.x86")
@@ -166,15 +163,14 @@
         hostname="tf.ubuntu",
         plan=equinix.metal.Plan.C3_MEDIUM_X86,
         metro="ny",
         operating_system=example.id.apply(lambda x: equinix.metal.OperatingSystem(x)),
         billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=local["project_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str distro: Name of the OS distribution.
     :param str name: Name or part of the name of the distribution. Case insensitive.
     :param str provisionable_on: Plan name.
     :param str version: Version of the distribution.
     """
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_organization.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_organization.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,23 +137,21 @@
                      organization_id: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOrganizationResult:
     """
     Provides an Equinix Metal organization datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_organization(organization_id=local["org_id"])
     pulumi.export("projectsInTheOrg", test.project_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Description string.
     :param str name: The organization name.
     :param str organization_id: The UUID of the organization resource.
            
            Exactly one of `name` or `organization_id` must be given.
@@ -183,23 +181,21 @@
                             organization_id: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOrganizationResult]:
     """
     Provides an Equinix Metal organization datasource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_organization(organization_id=local["org_id"])
     pulumi.export("projectsInTheOrg", test.project_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Description string.
     :param str name: The organization name.
     :param str organization_id: The UUID of the organization resource.
            
            Exactly one of `name` or `organization_id` must be given.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_plans.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_plans.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,15 +77,14 @@
               sorts: Optional[Sequence[pulumi.InputType['GetPlansSortArgs']]] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPlansResult:
     """
     Provides an Equinix Metal plans datasource. This can be used to find plans that meet a filter criteria.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -102,17 +101,15 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("plans", example.plans)
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(filters=[
         equinix.metal.GetPlansFilterArgs(
             attribute="class",
@@ -130,23 +127,21 @@
                 "sv",
             ],
             all=True,
         ),
     ])
     pulumi.export("plans", example.plans)
     ```
-    <!--End PulumiCodeChooser -->
 
     ### Ignoring Changes to Plans/Metro
 
     Preserve deployed device plan, facility and metro when creating a new execution plan.
 
     As described in the `data-resource-behavior` feature as shown in the example below.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_plans = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -171,32 +166,29 @@
         hostname="example",
         plan=example_plans.plans[0].name.apply(lambda x: equinix.metal.Plan(x)),
         metro=example_plans.plans[0].available_in_metros[0],
         operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
         billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=var["project_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
     If your use case requires dynamic changes of a device plan or metro you can define the lifecycle with a condition.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     config = pulumi.Config()
     ignore_plans_metros_changes = config.get_bool("ignorePlansMetrosChanges")
     if ignore_plans_metros_changes is None:
         ignore_plans_metros_changes = False
     example_plans = equinix.metal.get_plans()
     # required device arguments
     example_device = equinix.metal.Device("exampleDevice")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetPlansFilterArgs']] filters: One or more attribute/values pairs to filter off of
     :param Sequence[pulumi.InputType['GetPlansSortArgs']] sorts: One or more attribute/direction pairs on which to sort results. If multiple
            sorts are provided, they will be applied in order
     """
     __args__ = dict()
@@ -217,15 +209,14 @@
                      sorts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetPlansSortArgs']]]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPlansResult]:
     """
     Provides an Equinix Metal plans datasource. This can be used to find plans that meet a filter criteria.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -242,17 +233,15 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("plans", example.plans)
     ```
-    <!--End PulumiCodeChooser -->
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(filters=[
         equinix.metal.GetPlansFilterArgs(
             attribute="class",
@@ -270,23 +259,21 @@
                 "sv",
             ],
             all=True,
         ),
     ])
     pulumi.export("plans", example.plans)
     ```
-    <!--End PulumiCodeChooser -->
 
     ### Ignoring Changes to Plans/Metro
 
     Preserve deployed device plan, facility and metro when creating a new execution plan.
 
     As described in the `data-resource-behavior` feature as shown in the example below.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_plans = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -311,32 +298,29 @@
         hostname="example",
         plan=example_plans.plans[0].name.apply(lambda x: equinix.metal.Plan(x)),
         metro=example_plans.plans[0].available_in_metros[0],
         operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
         billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=var["project_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
     If your use case requires dynamic changes of a device plan or metro you can define the lifecycle with a condition.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     config = pulumi.Config()
     ignore_plans_metros_changes = config.get_bool("ignorePlansMetrosChanges")
     if ignore_plans_metros_changes is None:
         ignore_plans_metros_changes = False
     example_plans = equinix.metal.get_plans()
     # required device arguments
     example_device = equinix.metal.Device("exampleDevice")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetPlansFilterArgs']] filters: One or more attribute/values pairs to filter off of
     :param Sequence[pulumi.InputType['GetPlansSortArgs']] sorts: One or more attribute/direction pairs on which to sort results. If multiple
            sorts are provided, they will be applied in order
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_port.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,14 @@
     Use this data source to read ports of existing devices. You can read port by either its UUID,
     or by a device UUID and port name.
 
     ## Example Usage
 
     Create a device and read it's eth0 port to the datasource.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test_device = equinix.metal.Device("testDevice",
         hostname="tfacc-test-device-port",
@@ -224,15 +223,14 @@
         metro="sv",
         operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
         billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=project_id)
     test_port = equinix.metal.get_port_output(device_id=test_device.id,
         name="eth0")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device UUID where to lookup the port.
     :param str name: Name of the port to look up, i.e. `bond0`, `eth1`.
     :param str port_id: ID of the port to read, conflicts with `device_id`.
     """
     __args__ = dict()
@@ -269,15 +267,14 @@
     Use this data source to read ports of existing devices. You can read port by either its UUID,
     or by a device UUID and port name.
 
     ## Example Usage
 
     Create a device and read it's eth0 port to the datasource.
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test_device = equinix.metal.Device("testDevice",
         hostname="tfacc-test-device-port",
@@ -285,15 +282,14 @@
         metro="sv",
         operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
         billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=project_id)
     test_port = equinix.metal.get_port_output(device_id=test_device.id,
         name="eth0")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device UUID where to lookup the port.
     :param str name: Name of the port to look up, i.e. `bond0`, `eth1`.
     :param str port_id: ID of the port to read, conflicts with `device_id`.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_precreated_ip_block.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_reserved_ip_block.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetPrecreatedIpBlockResult',
-    'AwaitableGetPrecreatedIpBlockResult',
-    'get_precreated_ip_block',
-    'get_precreated_ip_block_output',
+    'GetReservedIpBlockResult',
+    'AwaitableGetReservedIpBlockResult',
+    'get_reserved_ip_block',
+    'get_reserved_ip_block_output',
 ]
 
 @pulumi.output_type
-class GetPrecreatedIpBlockResult:
+class GetReservedIpBlockResult:
     """
-    A collection of values returned by getPrecreatedIpBlock.
+    A collection of values returned by getReservedIpBlock.
     """
-    def __init__(__self__, address=None, address_family=None, cidr=None, cidr_notation=None, facility=None, gateway=None, global_=None, id=None, manageable=None, management=None, metro=None, netmask=None, network=None, project_id=None, public=None, quantity=None, type=None, vrf_id=None):
+    def __init__(__self__, address=None, address_family=None, cidr=None, cidr_notation=None, facility=None, gateway=None, global_=None, id=None, ip_address=None, manageable=None, management=None, metro=None, netmask=None, network=None, project_id=None, public=None, quantity=None, type=None, vrf_id=None):
         if address and not isinstance(address, str):
             raise TypeError("Expected argument 'address' to be a str")
         pulumi.set(__self__, "address", address)
         if address_family and not isinstance(address_family, int):
             raise TypeError("Expected argument 'address_family' to be a int")
         pulumi.set(__self__, "address_family", address_family)
         if cidr and not isinstance(cidr, int):
@@ -42,14 +42,17 @@
         pulumi.set(__self__, "gateway", gateway)
         if global_ and not isinstance(global_, bool):
             raise TypeError("Expected argument 'global_' to be a bool")
         pulumi.set(__self__, "global_", global_)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if ip_address and not isinstance(ip_address, str):
+            raise TypeError("Expected argument 'ip_address' to be a str")
+        pulumi.set(__self__, "ip_address", ip_address)
         if manageable and not isinstance(manageable, bool):
             raise TypeError("Expected argument 'manageable' to be a bool")
         pulumi.set(__self__, "manageable", manageable)
         if management and not isinstance(management, bool):
             raise TypeError("Expected argument 'management' to be a bool")
         pulumi.set(__self__, "management", management)
         if metro and not isinstance(metro, str):
@@ -69,16 +72,16 @@
         pulumi.set(__self__, "public", public)
         if quantity and not isinstance(quantity, int):
             raise TypeError("Expected argument 'quantity' to be a int")
         pulumi.set(__self__, "quantity", quantity)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
-        if vrf_id and not isinstance(vrf_id, str):
-            raise TypeError("Expected argument 'vrf_id' to be a str")
+        if vrf_id and not isinstance(vrf_id, int):
+            raise TypeError("Expected argument 'vrf_id' to be a int")
         pulumi.set(__self__, "vrf_id", vrf_id)
 
     @property
     @pulumi.getter
     def address(self) -> str:
         return pulumi.get(self, "address")
 
@@ -91,55 +94,57 @@
     @pulumi.getter
     def cidr(self) -> int:
         return pulumi.get(self, "cidr")
 
     @property
     @pulumi.getter(name="cidrNotation")
     def cidr_notation(self) -> str:
-        """
-        CIDR notation of the looked up block.
-        """
         return pulumi.get(self, "cidr_notation")
 
     @property
     @pulumi.getter
-    def facility(self) -> Optional[str]:
+    def facility(self) -> str:
+        warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
+        pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
+
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
     def gateway(self) -> str:
         return pulumi.get(self, "gateway")
 
     @property
     @pulumi.getter(name="global")
-    def global_(self) -> Optional[bool]:
+    def global_(self) -> bool:
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="ipAddress")
+    def ip_address(self) -> Optional[str]:
+        return pulumi.get(self, "ip_address")
+
+    @property
     @pulumi.getter
     def manageable(self) -> bool:
         return pulumi.get(self, "manageable")
 
     @property
     @pulumi.getter
     def management(self) -> bool:
         return pulumi.get(self, "management")
 
     @property
     @pulumi.getter
-    def metro(self) -> Optional[str]:
+    def metro(self) -> str:
         return pulumi.get(self, "metro")
 
     @property
     @pulumi.getter
     def netmask(self) -> str:
         return pulumi.get(self, "netmask")
 
@@ -162,124 +167,114 @@
     @pulumi.getter
     def quantity(self) -> int:
         return pulumi.get(self, "quantity")
 
     @property
     @pulumi.getter
     def type(self) -> str:
+        """
+        One of `global_ipv4`, `public_ipv4`, `private_ipv4`, `public_ipv6`,or `vrf`
+        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="vrfId")
-    def vrf_id(self) -> str:
+    def vrf_id(self) -> int:
         return pulumi.get(self, "vrf_id")
 
 
-class AwaitableGetPrecreatedIpBlockResult(GetPrecreatedIpBlockResult):
+class AwaitableGetReservedIpBlockResult(GetReservedIpBlockResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPrecreatedIpBlockResult(
+        return GetReservedIpBlockResult(
             address=self.address,
             address_family=self.address_family,
             cidr=self.cidr,
             cidr_notation=self.cidr_notation,
             facility=self.facility,
             gateway=self.gateway,
             global_=self.global_,
             id=self.id,
+            ip_address=self.ip_address,
             manageable=self.manageable,
             management=self.management,
             metro=self.metro,
             netmask=self.netmask,
             network=self.network,
             project_id=self.project_id,
             public=self.public,
             quantity=self.quantity,
             type=self.type,
             vrf_id=self.vrf_id)
 
 
-def get_precreated_ip_block(address_family: Optional[int] = None,
-                            facility: Optional[str] = None,
-                            global_: Optional[bool] = None,
-                            metro: Optional[str] = None,
-                            project_id: Optional[str] = None,
-                            public: Optional[bool] = None,
-                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPrecreatedIpBlockResult:
+def get_reserved_ip_block(id: Optional[str] = None,
+                          ip_address: Optional[str] = None,
+                          project_id: Optional[str] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetReservedIpBlockResult:
     """
-    Use this data source to get CIDR expression for precreated (management) IPv6 and IPv4 blocks in Equinix Metal.
-    You can then use the cidrsubnet TF builtin function to derive subnets.
+    Use this data source to find IP address blocks in Equinix Metal. You can use IP address or a block
+    ID for lookup.
 
-    > For backward compatibility, this data source will also return reserved (elastic) IP blocks.
+    > For backward compatibility, this data source can be also used for precreated (management) IP blocks.
 
-    > Precreated (management) IP blocks for a metro will not be available until first device is created in that metro.
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
-    > Public IPv4 blocks auto-assigned (management) to a device cannot be retrieved. If you need that information, consider using the metal.Device data source instead.
 
-
-    :param int address_family: 4 or 6, depending on which block you are looking for.
-    :param str facility: Facility of the searched block. (for non-global blocks). Use metro instead; read the facility to metro migration guide
-    :param bool global_: Whether to look for global block. Default is false for backward compatibility.
-    :param str metro: Metro of the searched block (for non-global blocks).
-    :param str project_id: ID of the project where the searched block should be.
-    :param bool public: Whether to look for public or private block.
+    :param str id: UUID of the IP address block to look up.
+    :param str ip_address: Block containing this IP address will be returned.
+           
+           > **NOTE:** You should pass either `id`, or both `project_id` and `ip_address`.
+    :param str project_id: UUID of the project where the searched block should be.
     """
     __args__ = dict()
-    __args__['addressFamily'] = address_family
-    __args__['facility'] = facility
-    __args__['global'] = global_
-    __args__['metro'] = metro
+    __args__['id'] = id
+    __args__['ipAddress'] = ip_address
     __args__['projectId'] = project_id
-    __args__['public'] = public
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:metal/getPrecreatedIpBlock:getPrecreatedIpBlock', __args__, opts=opts, typ=GetPrecreatedIpBlockResult).value
+    __ret__ = pulumi.runtime.invoke('equinix:metal/getReservedIpBlock:getReservedIpBlock', __args__, opts=opts, typ=GetReservedIpBlockResult).value
 
-    return AwaitableGetPrecreatedIpBlockResult(
+    return AwaitableGetReservedIpBlockResult(
         address=pulumi.get(__ret__, 'address'),
         address_family=pulumi.get(__ret__, 'address_family'),
         cidr=pulumi.get(__ret__, 'cidr'),
         cidr_notation=pulumi.get(__ret__, 'cidr_notation'),
         facility=pulumi.get(__ret__, 'facility'),
         gateway=pulumi.get(__ret__, 'gateway'),
         global_=pulumi.get(__ret__, 'global_'),
         id=pulumi.get(__ret__, 'id'),
+        ip_address=pulumi.get(__ret__, 'ip_address'),
         manageable=pulumi.get(__ret__, 'manageable'),
         management=pulumi.get(__ret__, 'management'),
         metro=pulumi.get(__ret__, 'metro'),
         netmask=pulumi.get(__ret__, 'netmask'),
         network=pulumi.get(__ret__, 'network'),
         project_id=pulumi.get(__ret__, 'project_id'),
         public=pulumi.get(__ret__, 'public'),
         quantity=pulumi.get(__ret__, 'quantity'),
         type=pulumi.get(__ret__, 'type'),
         vrf_id=pulumi.get(__ret__, 'vrf_id'))
 
 
-@_utilities.lift_output_func(get_precreated_ip_block)
-def get_precreated_ip_block_output(address_family: Optional[pulumi.Input[int]] = None,
-                                   facility: Optional[pulumi.Input[Optional[str]]] = None,
-                                   global_: Optional[pulumi.Input[Optional[bool]]] = None,
-                                   metro: Optional[pulumi.Input[Optional[str]]] = None,
-                                   project_id: Optional[pulumi.Input[str]] = None,
-                                   public: Optional[pulumi.Input[bool]] = None,
-                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrecreatedIpBlockResult]:
+@_utilities.lift_output_func(get_reserved_ip_block)
+def get_reserved_ip_block_output(id: Optional[pulumi.Input[Optional[str]]] = None,
+                                 ip_address: Optional[pulumi.Input[Optional[str]]] = None,
+                                 project_id: Optional[pulumi.Input[Optional[str]]] = None,
+                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetReservedIpBlockResult]:
     """
-    Use this data source to get CIDR expression for precreated (management) IPv6 and IPv4 blocks in Equinix Metal.
-    You can then use the cidrsubnet TF builtin function to derive subnets.
-
-    > For backward compatibility, this data source will also return reserved (elastic) IP blocks.
+    Use this data source to find IP address blocks in Equinix Metal. You can use IP address or a block
+    ID for lookup.
 
-    > Precreated (management) IP blocks for a metro will not be available until first device is created in that metro.
+    > For backward compatibility, this data source can be also used for precreated (management) IP blocks.
 
-    > Public IPv4 blocks auto-assigned (management) to a device cannot be retrieved. If you need that information, consider using the metal.Device data source instead.
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
 
-    :param int address_family: 4 or 6, depending on which block you are looking for.
-    :param str facility: Facility of the searched block. (for non-global blocks). Use metro instead; read the facility to metro migration guide
-    :param bool global_: Whether to look for global block. Default is false for backward compatibility.
-    :param str metro: Metro of the searched block (for non-global blocks).
-    :param str project_id: ID of the project where the searched block should be.
-    :param bool public: Whether to look for public or private block.
+    :param str id: UUID of the IP address block to look up.
+    :param str ip_address: Block containing this IP address will be returned.
+           
+           > **NOTE:** You should pass either `id`, or both `project_id` and `ip_address`.
+    :param str project_id: UUID of the project where the searched block should be.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_project.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,23 +148,21 @@
                 project_id: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectResult:
     """
     Use this datasource to retrieve attributes of the Project API resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     tf_project1 = equinix.metal.get_project(name="Terraform Fun")
     pulumi.export("usersOfTerraformFun", tf_project1.user_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name which is used to look up the project.
     :param str project_id: The UUID by which to look up the project.
     """
     __args__ = dict()
     __args__['name'] = name
@@ -190,22 +188,20 @@
                        project_id: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectResult]:
     """
     Use this datasource to retrieve attributes of the Project API resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     tf_project1 = equinix.metal.get_project(name="Terraform Fun")
     pulumi.export("usersOfTerraformFun", tf_project1.user_ids)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name which is used to look up the project.
     :param str project_id: The UUID by which to look up the project.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_project_ssh_key.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project_ssh_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,23 +142,21 @@
                         search: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectSshKeyResult:
     """
     Use this datasource to retrieve attributes of a Project SSH Key API resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     my_key = equinix.metal.get_project_ssh_key(search="username@hostname",
         project_id=local["project_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the SSH Key to search for in the Equinix Metal project.
     :param str project_id: The Equinix Metal project id of the Equinix Metal SSH Key.
            
            > **NOTE:** One of either `search` or `id` must be provided along with `project_id`.
     :param str search: The name, fingerprint, or public_key of the SSH Key to search for
@@ -189,23 +187,21 @@
                                search: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectSshKeyResult]:
     """
     Use this datasource to retrieve attributes of a Project SSH Key API resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     my_key = equinix.metal.get_project_ssh_key(search="username@hostname",
         project_id=local["project_id"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the SSH Key to search for in the Equinix Metal project.
     :param str project_id: The Equinix Metal project id of the Equinix Metal SSH Key.
            
            > **NOTE:** One of either `search` or `id` must be provided along with `project_id`.
     :param str search: The name, fingerprint, or public_key of the SSH Key to search for
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_spot_market_price.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,23 +93,21 @@
     """
     Use this data source to get Equinix Metal Spot Market Price for a plan.
 
     ## Example Usage
 
     Lookup by metro:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_spot_market_price(metro="sv",
         plan="c3.small.x86")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Name of the facility. Use metro instead; read the facility to metro migration guide
     :param str metro: Name of the metro.
     :param str plan: Name of the plan.
     """
     __args__ = dict()
@@ -135,23 +133,21 @@
     """
     Use this data source to get Equinix Metal Spot Market Price for a plan.
 
     ## Example Usage
 
     Lookup by metro:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_spot_market_price(metro="sv",
         plan="c3.small.x86")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Name of the facility. Use metro instead; read the facility to metro migration guide
     :param str metro: Name of the metro.
     :param str plan: Name of the plan.
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_spot_market_request.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_virtual_circuit.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_key.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,315 +5,363 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = [
-    'GetVirtualCircuitResult',
-    'AwaitableGetVirtualCircuitResult',
-    'get_virtual_circuit',
-    'get_virtual_circuit_output',
-]
-
-@pulumi.output_type
-class GetVirtualCircuitResult:
-    """
-    A collection of values returned by getVirtualCircuit.
-    """
-    def __init__(__self__, connection_id=None, customer_ip=None, description=None, id=None, md5=None, metal_ip=None, name=None, nni_vlan=None, nni_vnid=None, peer_asn=None, port_id=None, project_id=None, speed=None, status=None, subnet=None, tags=None, virtual_circuit_id=None, vlan_id=None, vnid=None, vrf_id=None):
-        if connection_id and not isinstance(connection_id, str):
-            raise TypeError("Expected argument 'connection_id' to be a str")
-        pulumi.set(__self__, "connection_id", connection_id)
-        if customer_ip and not isinstance(customer_ip, str):
-            raise TypeError("Expected argument 'customer_ip' to be a str")
-        pulumi.set(__self__, "customer_ip", customer_ip)
-        if description and not isinstance(description, str):
-            raise TypeError("Expected argument 'description' to be a str")
-        pulumi.set(__self__, "description", description)
-        if id and not isinstance(id, str):
-            raise TypeError("Expected argument 'id' to be a str")
-        pulumi.set(__self__, "id", id)
-        if md5 and not isinstance(md5, str):
-            raise TypeError("Expected argument 'md5' to be a str")
-        pulumi.set(__self__, "md5", md5)
-        if metal_ip and not isinstance(metal_ip, str):
-            raise TypeError("Expected argument 'metal_ip' to be a str")
-        pulumi.set(__self__, "metal_ip", metal_ip)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-        if nni_vlan and not isinstance(nni_vlan, int):
-            raise TypeError("Expected argument 'nni_vlan' to be a int")
-        pulumi.set(__self__, "nni_vlan", nni_vlan)
-        if nni_vnid and not isinstance(nni_vnid, int):
-            raise TypeError("Expected argument 'nni_vnid' to be a int")
-        pulumi.set(__self__, "nni_vnid", nni_vnid)
-        if peer_asn and not isinstance(peer_asn, int):
-            raise TypeError("Expected argument 'peer_asn' to be a int")
-        pulumi.set(__self__, "peer_asn", peer_asn)
-        if port_id and not isinstance(port_id, str):
-            raise TypeError("Expected argument 'port_id' to be a str")
-        pulumi.set(__self__, "port_id", port_id)
-        if project_id and not isinstance(project_id, str):
-            raise TypeError("Expected argument 'project_id' to be a str")
-        pulumi.set(__self__, "project_id", project_id)
-        if speed and not isinstance(speed, str):
-            raise TypeError("Expected argument 'speed' to be a str")
-        pulumi.set(__self__, "speed", speed)
-        if status and not isinstance(status, str):
-            raise TypeError("Expected argument 'status' to be a str")
-        pulumi.set(__self__, "status", status)
-        if subnet and not isinstance(subnet, str):
-            raise TypeError("Expected argument 'subnet' to be a str")
-        pulumi.set(__self__, "subnet", subnet)
-        if tags and not isinstance(tags, list):
-            raise TypeError("Expected argument 'tags' to be a list")
-        pulumi.set(__self__, "tags", tags)
-        if virtual_circuit_id and not isinstance(virtual_circuit_id, str):
-            raise TypeError("Expected argument 'virtual_circuit_id' to be a str")
-        pulumi.set(__self__, "virtual_circuit_id", virtual_circuit_id)
-        if vlan_id and not isinstance(vlan_id, str):
-            raise TypeError("Expected argument 'vlan_id' to be a str")
-        pulumi.set(__self__, "vlan_id", vlan_id)
-        if vnid and not isinstance(vnid, int):
-            raise TypeError("Expected argument 'vnid' to be a int")
-        pulumi.set(__self__, "vnid", vnid)
-        if vrf_id and not isinstance(vrf_id, str):
-            raise TypeError("Expected argument 'vrf_id' to be a str")
-        pulumi.set(__self__, "vrf_id", vrf_id)
-
-    @property
-    @pulumi.getter(name="connectionId")
-    def connection_id(self) -> str:
-        """
-        UUID of Connection where the VC is scoped to.
-        """
-        return pulumi.get(self, "connection_id")
+__all__ = ['SshKeyArgs', 'SshKey']
 
-    @property
-    @pulumi.getter(name="customerIp")
-    def customer_ip(self) -> str:
-        """
-        The Customer IP address which the CSR switch will peer with. Will default to the other usable IP in the subnet.
-        """
-        return pulumi.get(self, "customer_ip")
+@pulumi.input_type
+class SshKeyArgs:
+    def __init__(__self__, *,
+                 public_key: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a SshKey resource.
+        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
+               interpolation function.
+        :param pulumi.Input[str] name: The name of SSH key used for identification.
+        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
+               leave it out, the ssh key will be created under the default project id of your organization.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
+        """
+        pulumi.set(__self__, "public_key", public_key)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> pulumi.Input[str]:
+        """
+        The SSH public key. If this is a file, it can be read using the file
+        interpolation function.
+        """
+        return pulumi.get(self, "public_key")
+
+    @public_key.setter
+    def public_key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter
-    def description(self) -> str:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Description for the Virtual Circuit resource.
+        The name of SSH key used for identification.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The provider-assigned unique ID for this managed resource.
+        Unique Identifier for the project resource where the SSH key is scoped to.If you
+        leave it out, the ssh key will be created under the default project id of your organization.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "project_id")
+
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_id", value)
 
     @property
     @pulumi.getter
-    def md5(self) -> str:
+    def type(self) -> Optional[pulumi.Input[str]]:
         """
-        The password that can be set for the VRF BGP peer
+        The type of SSH key: `RSA` (default) or `DSA`.
         """
-        return pulumi.get(self, "md5")
+        return pulumi.get(self, "type")
 
-    @property
-    @pulumi.getter(name="metalIp")
-    def metal_ip(self) -> str:
-        """
-        The Metal IP address for the SVI (Switch Virtual Interface) of the VirtualCircuit. Will default to the first usable IP in the subnet.
-        """
-        return pulumi.get(self, "metal_ip")
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
+
+
+@pulumi.input_type
+class _SshKeyState:
+    def __init__(__self__, *,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 public_key: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 uuid: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering SshKey resources.
+        :param pulumi.Input[str] name: The name of SSH key used for identification.
+        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
+               leave it out, the ssh key will be created under the default project id of your organization.
+        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
+               interpolation function.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
+        :param pulumi.Input[str] uuid: The unique identifier of the key
+        """
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if project_id is not None:
+            pulumi.set(__self__, "project_id", project_id)
+        if public_key is not None:
+            pulumi.set(__self__, "public_key", public_key)
+        if type is not None:
+            pulumi.set(__self__, "type", type)
+        if uuid is not None:
+            pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the virtual circuit resource.
+        The name of SSH key used for identification.
         """
         return pulumi.get(self, "name")
 
-    @property
-    @pulumi.getter(name="nniVlan")
-    def nni_vlan(self) -> int:
-        return pulumi.get(self, "nni_vlan")
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="nniVnid")
-    def nni_vnid(self) -> int:
-        return pulumi.get(self, "nni_vnid")
-
-    @property
-    @pulumi.getter(name="peerAsn")
-    def peer_asn(self) -> int:
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The BGP ASN of the peer. The same ASN may be the used across several VCs, but it cannot be the same as the local_asn of the VRF.
+        Unique Identifier for the project resource where the SSH key is scoped to.If you
+        leave it out, the ssh key will be created under the default project id of your organization.
         """
-        return pulumi.get(self, "peer_asn")
+        return pulumi.get(self, "project_id")
 
-    @property
-    @pulumi.getter(name="portId")
-    def port_id(self) -> str:
-        """
-        UUID of the Connection Port where the VC is scoped to.
-        """
-        return pulumi.get(self, "port_id")
+    @project_id.setter
+    def project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project_id", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> str:
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> Optional[pulumi.Input[str]]:
         """
-        ID of project to which the VC belongs.
+        The SSH public key. If this is a file, it can be read using the file
+        interpolation function.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "public_key")
+
+    @public_key.setter
+    def public_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "public_key", value)
 
     @property
     @pulumi.getter
-    def speed(self) -> str:
+    def type(self) -> Optional[pulumi.Input[str]]:
         """
-        Speed of the Virtual Circuit resource.
+        The type of SSH key: `RSA` (default) or `DSA`.
         """
-        return pulumi.get(self, "speed")
+        return pulumi.get(self, "type")
+
+    @type.setter
+    def type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
-    def status(self) -> str:
+    def uuid(self) -> Optional[pulumi.Input[str]]:
         """
-        Status of the virtal circuit.
+        The unique identifier of the key
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "uuid")
+
+    @uuid.setter
+    def uuid(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "uuid", value)
+
+
+class SshKey(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 public_key: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        Resource `networkedge.SshKey` allows creation and management of Equinix Network Edge SSH keys.
+
+        ## Example Usage
+        ```python
+        import pulumi
+        import pulumi_equinix as equinix
+
+        ssh_key = equinix.networkedge.SshKey("sshKey",
+            name="johnKent",
+            public_key=(lambda path: open(path).read())("/Users/John/.ssh/ne_rsa.pub"))
+        pulumi.export("sshKeyId", ssh_key.id)
+        ```
+
+        ## Import
+
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id}
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] name: The name of SSH key used for identification.
+        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
+               leave it out, the ssh key will be created under the default project id of your organization.
+        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
+               interpolation function.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: SshKeyArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        Resource `networkedge.SshKey` allows creation and management of Equinix Network Edge SSH keys.
+
+        ## Example Usage
+        ```python
+        import pulumi
+        import pulumi_equinix as equinix
+
+        ssh_key = equinix.networkedge.SshKey("sshKey",
+            name="johnKent",
+            public_key=(lambda path: open(path).read())("/Users/John/.ssh/ne_rsa.pub"))
+        pulumi.export("sshKeyId", ssh_key.id)
+        ```
+
+        ## Import
+
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id}
+        ```
+
+        :param str resource_name: The name of the resource.
+        :param SshKeyArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(SshKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 project_id: Optional[pulumi.Input[str]] = None,
+                 public_key: Optional[pulumi.Input[str]] = None,
+                 type: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = SshKeyArgs.__new__(SshKeyArgs)
+
+            __props__.__dict__["name"] = name
+            __props__.__dict__["project_id"] = project_id
+            if public_key is None and not opts.urn:
+                raise TypeError("Missing required property 'public_key'")
+            __props__.__dict__["public_key"] = public_key
+            __props__.__dict__["type"] = type
+            __props__.__dict__["uuid"] = None
+        super(SshKey, __self__).__init__(
+            'equinix:networkedge/sshKey:SshKey',
+            resource_name,
+            __props__,
+            opts)
+
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            project_id: Optional[pulumi.Input[str]] = None,
+            public_key: Optional[pulumi.Input[str]] = None,
+            type: Optional[pulumi.Input[str]] = None,
+            uuid: Optional[pulumi.Input[str]] = None) -> 'SshKey':
+        """
+        Get an existing SshKey resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] name: The name of SSH key used for identification.
+        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
+               leave it out, the ssh key will be created under the default project id of your organization.
+        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
+               interpolation function.
+        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
+        :param pulumi.Input[str] uuid: The unique identifier of the key
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _SshKeyState.__new__(_SshKeyState)
+
+        __props__.__dict__["name"] = name
+        __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["public_key"] = public_key
+        __props__.__dict__["type"] = type
+        __props__.__dict__["uuid"] = uuid
+        return SshKey(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def subnet(self) -> str:
+    def name(self) -> pulumi.Output[str]:
         """
-        A subnet from one of the IP
-        blocks associated with the VRF that we will help create an IP reservation for. Can only be either a /30 or /31.
-        * For a /31 block, it will only have two IP addresses, which will be used for
-        the metal_ip and customer_ip.
-        * For a /30 block, it will have four IP addresses, but the first and last IP addresses are not usable. We will default to the first usable IP address for the metal_ip.
+        The name of SSH key used for identification.
         """
-        return pulumi.get(self, "subnet")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def tags(self) -> Sequence[str]:
+    @pulumi.getter(name="projectId")
+    def project_id(self) -> pulumi.Output[str]:
         """
-        Tags for the Virtual Circuit resource.
+        Unique Identifier for the project resource where the SSH key is scoped to.If you
+        leave it out, the ssh key will be created under the default project id of your organization.
         """
-        return pulumi.get(self, "tags")
+        return pulumi.get(self, "project_id")
 
     @property
-    @pulumi.getter(name="virtualCircuitId")
-    def virtual_circuit_id(self) -> str:
-        return pulumi.get(self, "virtual_circuit_id")
+    @pulumi.getter(name="publicKey")
+    def public_key(self) -> pulumi.Output[str]:
+        """
+        The SSH public key. If this is a file, it can be read using the file
+        interpolation function.
+        """
+        return pulumi.get(self, "public_key")
 
     @property
-    @pulumi.getter(name="vlanId")
-    def vlan_id(self) -> str:
-        return pulumi.get(self, "vlan_id")
+    @pulumi.getter
+    def type(self) -> pulumi.Output[Optional[str]]:
+        """
+        The type of SSH key: `RSA` (default) or `DSA`.
+        """
+        return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
-    def vnid(self) -> int:
+    def uuid(self) -> pulumi.Output[str]:
         """
-        , `nni_vlan`, `nni_nvid` - VLAN parameters, see the
-        [documentation for Equinix Fabric](https://metal.equinix.com/developers/docs/networking/fabric/).
+        The unique identifier of the key
         """
-        return pulumi.get(self, "vnid")
+        return pulumi.get(self, "uuid")
 
-    @property
-    @pulumi.getter(name="vrfId")
-    def vrf_id(self) -> str:
-        """
-        UUID of the VLAN to associate.
-        """
-        return pulumi.get(self, "vrf_id")
-
-
-class AwaitableGetVirtualCircuitResult(GetVirtualCircuitResult):
-    # pylint: disable=using-constant-test
-    def __await__(self):
-        if False:
-            yield self
-        return GetVirtualCircuitResult(
-            connection_id=self.connection_id,
-            customer_ip=self.customer_ip,
-            description=self.description,
-            id=self.id,
-            md5=self.md5,
-            metal_ip=self.metal_ip,
-            name=self.name,
-            nni_vlan=self.nni_vlan,
-            nni_vnid=self.nni_vnid,
-            peer_asn=self.peer_asn,
-            port_id=self.port_id,
-            project_id=self.project_id,
-            speed=self.speed,
-            status=self.status,
-            subnet=self.subnet,
-            tags=self.tags,
-            virtual_circuit_id=self.virtual_circuit_id,
-            vlan_id=self.vlan_id,
-            vnid=self.vnid,
-            vrf_id=self.vrf_id)
-
-
-def get_virtual_circuit(virtual_circuit_id: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVirtualCircuitResult:
-    """
-    Use this data source to retrieve a virtual circuit resource from
-    [Equinix Fabric - software-defined interconnections](https://metal.equinix.com/developers/docs/networking/fabric/)
-
-    > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
-
-
-    :param str virtual_circuit_id: ID of the virtual circuit resource
-    """
-    __args__ = dict()
-    __args__['virtualCircuitId'] = virtual_circuit_id
-    opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('equinix:metal/getVirtualCircuit:getVirtualCircuit', __args__, opts=opts, typ=GetVirtualCircuitResult).value
-
-    return AwaitableGetVirtualCircuitResult(
-        connection_id=pulumi.get(__ret__, 'connection_id'),
-        customer_ip=pulumi.get(__ret__, 'customer_ip'),
-        description=pulumi.get(__ret__, 'description'),
-        id=pulumi.get(__ret__, 'id'),
-        md5=pulumi.get(__ret__, 'md5'),
-        metal_ip=pulumi.get(__ret__, 'metal_ip'),
-        name=pulumi.get(__ret__, 'name'),
-        nni_vlan=pulumi.get(__ret__, 'nni_vlan'),
-        nni_vnid=pulumi.get(__ret__, 'nni_vnid'),
-        peer_asn=pulumi.get(__ret__, 'peer_asn'),
-        port_id=pulumi.get(__ret__, 'port_id'),
-        project_id=pulumi.get(__ret__, 'project_id'),
-        speed=pulumi.get(__ret__, 'speed'),
-        status=pulumi.get(__ret__, 'status'),
-        subnet=pulumi.get(__ret__, 'subnet'),
-        tags=pulumi.get(__ret__, 'tags'),
-        virtual_circuit_id=pulumi.get(__ret__, 'virtual_circuit_id'),
-        vlan_id=pulumi.get(__ret__, 'vlan_id'),
-        vnid=pulumi.get(__ret__, 'vnid'),
-        vrf_id=pulumi.get(__ret__, 'vrf_id'))
-
-
-@_utilities.lift_output_func(get_virtual_circuit)
-def get_virtual_circuit_output(virtual_circuit_id: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVirtualCircuitResult]:
-    """
-    Use this data source to retrieve a virtual circuit resource from
-    [Equinix Fabric - software-defined interconnections](https://metal.equinix.com/developers/docs/networking/fabric/)
-
-    > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
-
-
-    :param str virtual_circuit_id: ID of the virtual circuit resource
-    """
-    ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_vlan.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vlan.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,39 +123,35 @@
     Provides an Equinix Metal Virtual Network datasource. VLANs data sources can be
     searched by VLAN UUID, or project UUID and vxlan number.
 
     ## Example Usage
 
     Fetch a vlan by ID:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     foovlan = equinix.metal.Vlan("foovlan",
         project_id=local["project_id"],
         metro="sv",
         vxlan=5)
     dsvlan = equinix.metal.get_vlan_output(vlan_id=foovlan.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Fetch a vlan by project ID, vxlan and metro
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dsvlan = equinix.metal.get_vlan(project_id=local["project_id"],
         vxlan=5,
         metro="sv")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility where the VLAN is deployed. Deprecated, see https://feedback.equinixmetal.com/changelog/bye-facilities-hello-again-metros
     :param str metro: Metro where the VLAN is deployed.
            
            > **NOTE:** You must set either `vlan_id` or a combination of `vxlan`, `project_id`, and, `metro` or `facility`.
     :param str project_id: UUID of parent project of the VLAN. Use together with the vxlan number and metro or facility.
@@ -193,39 +189,35 @@
     Provides an Equinix Metal Virtual Network datasource. VLANs data sources can be
     searched by VLAN UUID, or project UUID and vxlan number.
 
     ## Example Usage
 
     Fetch a vlan by ID:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     foovlan = equinix.metal.Vlan("foovlan",
         project_id=local["project_id"],
         metro="sv",
         vxlan=5)
     dsvlan = equinix.metal.get_vlan_output(vlan_id=foovlan.id)
     ```
-    <!--End PulumiCodeChooser -->
 
     Fetch a vlan by project ID, vxlan and metro
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dsvlan = equinix.metal.get_vlan(project_id=local["project_id"],
         vxlan=5,
         metro="sv")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility where the VLAN is deployed. Deprecated, see https://feedback.equinixmetal.com/changelog/bye-facilities-hello-again-metros
     :param str metro: Metro where the VLAN is deployed.
            
            > **NOTE:** You must set either `vlan_id` or a combination of `vxlan`, `project_id`, and, `metro` or `facility`.
     :param str project_id: UUID of parent project of the VLAN. Use together with the vxlan number and metro or facility.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/get_vrf.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vrf.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,26 +126,24 @@
 
 
 def get_vrf(vrf_id: Optional[str] = None,
             opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetVrfResult:
     """
     Use this data source to retrieve a VRF resource.
 
-    > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_vrf = equinix.metal.get_vrf(vrf_id="48630899-9ff2-4ce6-a93f-50ff4ebcdf6e")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str vrf_id: ID of the VRF resource
     """
     __args__ = dict()
     __args__['vrfId'] = vrf_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -164,24 +162,22 @@
 
 @_utilities.lift_output_func(get_vrf)
 def get_vrf_output(vrf_id: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVrfResult]:
     """
     Use this data source to retrieve a VRF resource.
 
-    > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+    See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_vrf = equinix.metal.get_vrf(vrf_id="48630899-9ff2-4ce6-a93f-50ff4ebcdf6e")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str vrf_id: ID of the VRF resource
     """
     ...
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/interconnection.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/interconnection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/ip_attachment.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/ip_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/organization.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/organization_member.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/organization_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/outputs.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                  address: Optional[str] = None,
                  cidr: Optional[int] = None,
                  family: Optional[int] = None,
                  gateway: Optional[str] = None,
                  public: Optional[bool] = None):
         """
         :param str address: IPv4 or IPv6 address string.
-        :param int cidr: CIDR suffix for IP address block to be assigned, i.e. amount of addresses.
+        :param int cidr: Bit length of the network mask of the address.
         :param int family: IP version. One of `4`, `6`.
         :param str gateway: Address of router.
         :param bool public: Whether the address is routable from the Internet.
         """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if cidr is not None:
@@ -187,15 +187,15 @@
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def cidr(self) -> Optional[int]:
         """
-        CIDR suffix for IP address block to be assigned, i.e. amount of addresses.
+        Bit length of the network mask of the address.
         """
         return pulumi.get(self, "cidr")
 
     @property
     @pulumi.getter
     def family(self) -> Optional[int]:
         """
@@ -229,15 +229,15 @@
                  name: Optional[str] = None,
                  type: Optional[str] = None):
         """
         :param bool bonded: Whether this port is part of a bond in bonded network setup.
         :param str id: ID of the port.
         :param str mac: MAC address assigned to the port.
         :param str name: Name of the port (e.g. `eth0`, or `bond0`).
-        :param str type: One of `private_ipv4`, `public_ipv4`, `public_ipv6`.
+        :param str type: Type of the port (e.g. `NetworkPort` or `NetworkBondPort`).
         """
         if bonded is not None:
             pulumi.set(__self__, "bonded", bonded)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if mac is not None:
             pulumi.set(__self__, "mac", mac)
@@ -278,15 +278,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        One of `private_ipv4`, `public_ipv4`, `public_ipv6`.
+        Type of the port (e.g. `NetworkPort` or `NetworkBondPort`).
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class DeviceReinstall(dict):
     @staticmethod
@@ -1613,26 +1613,26 @@
 
 @pulumi.output_type
 class GetDevicesSortResult(dict):
     def __init__(__self__, *,
                  attribute: str,
                  direction: Optional[str] = None):
         """
-        :param str attribute: The attribute used to filter. Filter attributes are case-sensitive
+        :param str attribute: The attribute used to sort the results. Sort attributes are case-sensitive
         :param str direction: Sort results in ascending or descending order. Strings are sorted in alphabetical order. One of: asc, desc
         """
         pulumi.set(__self__, "attribute", attribute)
         if direction is not None:
             pulumi.set(__self__, "direction", direction)
 
     @property
     @pulumi.getter
     def attribute(self) -> str:
         """
-        The attribute used to filter. Filter attributes are case-sensitive
+        The attribute used to sort the results. Sort attributes are case-sensitive
         """
         return pulumi.get(self, "attribute")
 
     @property
     @pulumi.getter
     def direction(self) -> Optional[str]:
         """
@@ -2121,26 +2121,26 @@
 
 @pulumi.output_type
 class GetPlansSortResult(dict):
     def __init__(__self__, *,
                  attribute: str,
                  direction: Optional[str] = None):
         """
-        :param str attribute: The attribute used to filter. Filter attributes are case-sensitive
+        :param str attribute: The attribute used to sort the results. Sort attributes are case-sensitive
         :param str direction: Sort results in ascending or descending order. Strings are sorted in alphabetical order. One of: asc, desc
         """
         pulumi.set(__self__, "attribute", attribute)
         if direction is not None:
             pulumi.set(__self__, "direction", direction)
 
     @property
     @pulumi.getter
     def attribute(self) -> str:
         """
-        The attribute used to filter. Filter attributes are case-sensitive
+        The attribute used to sort the results. Sort attributes are case-sensitive
         """
         return pulumi.get(self, "attribute")
 
     @property
     @pulumi.getter
     def direction(self) -> Optional[str]:
         """
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/port.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/port_vlan_attachment.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/port_vlan_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/project.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/project_api_key.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/project_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/project_ssh_key.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/reserved_ip_block.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/reserved_ip_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -585,15 +585,15 @@
 
         Public blocks are allocated in a metro. Addresses from public blocks can only be assigned to devices in the metro. Public blocks can have mask from /24 (256 addresses) to /32 (1 address). If you create public block with this resource, you must fill the metro argument.
 
         Addresses from global blocks can be assigned in any metro. Global blocks can have mask from /30 (4 addresses), to /32 (1 address). If you create global block with this resource, you must specify type = "global_ipv4" and you must omit the metro argument.
 
         Once IP block is allocated or imported, an address from it can be assigned to device with the `metal.IpAttachment` resource.
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
@@ -659,15 +659,15 @@
 
         Public blocks are allocated in a metro. Addresses from public blocks can only be assigned to devices in the metro. Public blocks can have mask from /24 (256 addresses) to /32 (1 address). If you create public block with this resource, you must fill the metro argument.
 
         Addresses from global blocks can be assigned in any metro. Global blocks can have mask from /30 (4 addresses), to /32 (1 address). If you create global block with this resource, you must specify type = "global_ipv4" and you must omit the metro argument.
 
         Once IP block is allocated or imported, an address from it can be assigned to device with the `metal.IpAttachment` resource.
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/spot_market_request.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/ssh_key.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/user_api_key.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/user_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/virtual_circuit.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/virtual_circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -589,15 +589,15 @@
                  vlan_id: Optional[pulumi.Input[str]] = None,
                  vrf_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to associate VLAN with a Dedicated Port from
         [Equinix Fabric - software-defined interconnections](https://metal.equinix.com/developers/docs/networking/fabric/#associating-a-vlan-with-a-dedicated-port).
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
@@ -651,15 +651,15 @@
                  resource_name: str,
                  args: VirtualCircuitArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to associate VLAN with a Dedicated Port from
         [Equinix Fabric - software-defined interconnections](https://metal.equinix.com/developers/docs/networking/fabric/#associating-a-vlan-with-a-dedicated-port).
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/vlan.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/metal/vrf.py` & `pulumi_equinix-0.9.0/pulumi_equinix/metal/vrf.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,15 +228,15 @@
                  metro: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Use this resource to manage a VRF.
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
@@ -279,15 +279,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: VrfArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Use this resource to manage a VRF.
 
-        > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
+        See the [Virtual Routing and Forwarding documentation](https://deploy.equinix.com/developers/docs/metal/layer2-networking/vrf/) for product details and API reference material.
 
         ## Example Usage
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         config = pulumi.Config()
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/__init__.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/_enums.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/_inputs.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'DeviceClusterDetailsNode0Args',
     'DeviceClusterDetailsNode0VendorConfigurationArgs',
     'DeviceClusterDetailsNode1Args',
     'DeviceClusterDetailsNode1VendorConfigurationArgs',
     'DeviceInterfaceArgs',
     'DeviceLinkDeviceArgs',
     'DeviceLinkLinkArgs',
+    'DeviceLinkMetroLinkArgs',
     'DeviceSecondaryDeviceArgs',
     'DeviceSecondaryDeviceInterfaceArgs',
     'DeviceSecondaryDeviceSshKeyArgs',
     'DeviceSshKeyArgs',
 ]
 
 @pulumi.input_type
@@ -325,23 +326,21 @@
     def __init__(__self__, *,
                  license_file_id: Optional[pulumi.Input[str]] = None,
                  license_token: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None,
                  vendor_configuration: Optional[pulumi.Input['DeviceClusterDetailsNode0VendorConfigurationArgs']] = None):
         """
-        :param pulumi.Input[str] license_file_id: Identifier of a license file that will be applied on the device.
-        :param pulumi.Input[str] license_token: License Token applicable for some device types in BYOL licensing
-               mode.
+        :param pulumi.Input[str] license_file_id: License file id. This is necessary for Fortinet and Juniper clusters.
+        :param pulumi.Input[str] license_token: License token. This is necessary for Palo Alto clusters.
         :param pulumi.Input[str] name: Device name.
         :param pulumi.Input[str] uuid: Device unique identifier.
-        :param pulumi.Input['DeviceClusterDetailsNode0VendorConfigurationArgs'] vendor_configuration: Map of vendor specific configuration parameters for a device
-               (controller1, activationKey, managementType, siteId, systemIpAddress)
-               * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-               on a device (max one key).  See SSH Key below for more details.
+        :param pulumi.Input['DeviceClusterDetailsNode0VendorConfigurationArgs'] vendor_configuration: An object that has fields relevant to the vendor of the
+               cluster device. See Cluster Details - Nodes - Vendor Configuration
+               below for more details.
         """
         if license_file_id is not None:
             pulumi.set(__self__, "license_file_id", license_file_id)
         if license_token is not None:
             pulumi.set(__self__, "license_token", license_token)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -350,28 +349,27 @@
         if vendor_configuration is not None:
             pulumi.set(__self__, "vendor_configuration", vendor_configuration)
 
     @property
     @pulumi.getter(name="licenseFileId")
     def license_file_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Identifier of a license file that will be applied on the device.
+        License file id. This is necessary for Fortinet and Juniper clusters.
         """
         return pulumi.get(self, "license_file_id")
 
     @license_file_id.setter
     def license_file_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "license_file_id", value)
 
     @property
     @pulumi.getter(name="licenseToken")
     def license_token(self) -> Optional[pulumi.Input[str]]:
         """
-        License Token applicable for some device types in BYOL licensing
-        mode.
+        License token. This is necessary for Palo Alto clusters.
         """
         return pulumi.get(self, "license_token")
 
     @license_token.setter
     def license_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "license_token", value)
 
@@ -399,18 +397,17 @@
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
     @property
     @pulumi.getter(name="vendorConfiguration")
     def vendor_configuration(self) -> Optional[pulumi.Input['DeviceClusterDetailsNode0VendorConfigurationArgs']]:
         """
-        Map of vendor specific configuration parameters for a device
-        (controller1, activationKey, managementType, siteId, systemIpAddress)
-        * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-        on a device (max one key).  See SSH Key below for more details.
+        An object that has fields relevant to the vendor of the
+        cluster device. See Cluster Details - Nodes - Vendor Configuration
+        below for more details.
         """
         return pulumi.get(self, "vendor_configuration")
 
     @vendor_configuration.setter
     def vendor_configuration(self, value: Optional[pulumi.Input['DeviceClusterDetailsNode0VendorConfigurationArgs']]):
         pulumi.set(self, "vendor_configuration", value)
 
@@ -527,23 +524,21 @@
     def __init__(__self__, *,
                  license_file_id: Optional[pulumi.Input[str]] = None,
                  license_token: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None,
                  vendor_configuration: Optional[pulumi.Input['DeviceClusterDetailsNode1VendorConfigurationArgs']] = None):
         """
-        :param pulumi.Input[str] license_file_id: Identifier of a license file that will be applied on the device.
-        :param pulumi.Input[str] license_token: License Token applicable for some device types in BYOL licensing
-               mode.
+        :param pulumi.Input[str] license_file_id: License file id. This is necessary for Fortinet and Juniper clusters.
+        :param pulumi.Input[str] license_token: License token. This is necessary for Palo Alto clusters.
         :param pulumi.Input[str] name: Device name.
         :param pulumi.Input[str] uuid: Device unique identifier.
-        :param pulumi.Input['DeviceClusterDetailsNode1VendorConfigurationArgs'] vendor_configuration: Map of vendor specific configuration parameters for a device
-               (controller1, activationKey, managementType, siteId, systemIpAddress)
-               * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-               on a device (max one key).  See SSH Key below for more details.
+        :param pulumi.Input['DeviceClusterDetailsNode1VendorConfigurationArgs'] vendor_configuration: An object that has fields relevant to the vendor of the
+               cluster device. See Cluster Details - Nodes - Vendor Configuration
+               below for more details.
         """
         if license_file_id is not None:
             pulumi.set(__self__, "license_file_id", license_file_id)
         if license_token is not None:
             pulumi.set(__self__, "license_token", license_token)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -552,28 +547,27 @@
         if vendor_configuration is not None:
             pulumi.set(__self__, "vendor_configuration", vendor_configuration)
 
     @property
     @pulumi.getter(name="licenseFileId")
     def license_file_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Identifier of a license file that will be applied on the device.
+        License file id. This is necessary for Fortinet and Juniper clusters.
         """
         return pulumi.get(self, "license_file_id")
 
     @license_file_id.setter
     def license_file_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "license_file_id", value)
 
     @property
     @pulumi.getter(name="licenseToken")
     def license_token(self) -> Optional[pulumi.Input[str]]:
         """
-        License Token applicable for some device types in BYOL licensing
-        mode.
+        License token. This is necessary for Palo Alto clusters.
         """
         return pulumi.get(self, "license_token")
 
     @license_token.setter
     def license_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "license_token", value)
 
@@ -601,18 +595,17 @@
     def uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uuid", value)
 
     @property
     @pulumi.getter(name="vendorConfiguration")
     def vendor_configuration(self) -> Optional[pulumi.Input['DeviceClusterDetailsNode1VendorConfigurationArgs']]:
         """
-        Map of vendor specific configuration parameters for a device
-        (controller1, activationKey, managementType, siteId, systemIpAddress)
-        * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-        on a device (max one key).  See SSH Key below for more details.
+        An object that has fields relevant to the vendor of the
+        cluster device. See Cluster Details - Nodes - Vendor Configuration
+        below for more details.
         """
         return pulumi.get(self, "vendor_configuration")
 
     @vendor_configuration.setter
     def vendor_configuration(self, value: Optional[pulumi.Input['DeviceClusterDetailsNode1VendorConfigurationArgs']]):
         pulumi.set(self, "vendor_configuration", value)
 
@@ -1074,14 +1067,83 @@
 
     @src_zone_code.setter
     def src_zone_code(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "src_zone_code", value)
 
 
 @pulumi.input_type
+class DeviceLinkMetroLinkArgs:
+    def __init__(__self__, *,
+                 account_number: pulumi.Input[str],
+                 metro_code: pulumi.Input[str],
+                 throughput: pulumi.Input[str],
+                 throughput_unit: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] account_number: billing account number to be used for
+               connection charges
+        :param pulumi.Input[str] metro_code: connection metro code.
+        :param pulumi.Input[str] throughput: connection throughput.
+        :param pulumi.Input[str] throughput_unit: connection throughput unit (Mbps or Gbps).
+        """
+        pulumi.set(__self__, "account_number", account_number)
+        pulumi.set(__self__, "metro_code", metro_code)
+        pulumi.set(__self__, "throughput", throughput)
+        pulumi.set(__self__, "throughput_unit", throughput_unit)
+
+    @property
+    @pulumi.getter(name="accountNumber")
+    def account_number(self) -> pulumi.Input[str]:
+        """
+        billing account number to be used for
+        connection charges
+        """
+        return pulumi.get(self, "account_number")
+
+    @account_number.setter
+    def account_number(self, value: pulumi.Input[str]):
+        pulumi.set(self, "account_number", value)
+
+    @property
+    @pulumi.getter(name="metroCode")
+    def metro_code(self) -> pulumi.Input[str]:
+        """
+        connection metro code.
+        """
+        return pulumi.get(self, "metro_code")
+
+    @metro_code.setter
+    def metro_code(self, value: pulumi.Input[str]):
+        pulumi.set(self, "metro_code", value)
+
+    @property
+    @pulumi.getter
+    def throughput(self) -> pulumi.Input[str]:
+        """
+        connection throughput.
+        """
+        return pulumi.get(self, "throughput")
+
+    @throughput.setter
+    def throughput(self, value: pulumi.Input[str]):
+        pulumi.set(self, "throughput", value)
+
+    @property
+    @pulumi.getter(name="throughputUnit")
+    def throughput_unit(self) -> pulumi.Input[str]:
+        """
+        connection throughput unit (Mbps or Gbps).
+        """
+        return pulumi.get(self, "throughput_unit")
+
+    @throughput_unit.setter
+    def throughput_unit(self, value: pulumi.Input[str]):
+        pulumi.set(self, "throughput_unit", value)
+
+
+@pulumi.input_type
 class DeviceSecondaryDeviceArgs:
     def __init__(__self__, *,
                  account_number: pulumi.Input[str],
                  metro_code: pulumi.Input[str],
                  name: pulumi.Input[str],
                  notifications: pulumi.Input[Sequence[pulumi.Input[str]]],
                  acl_template_id: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/acl_template.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/acl_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/bgp.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/bgp.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/device.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/device_link.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device_link.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,36 +14,49 @@
 __all__ = ['DeviceLinkArgs', 'DeviceLink']
 
 @pulumi.input_type
 class DeviceLinkArgs:
     def __init__(__self__, *,
                  devices: pulumi.Input[Sequence[pulumi.Input['DeviceLinkDeviceArgs']]],
                  links: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]]] = None,
+                 metro_links: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
+                 redundancy_type: Optional[pulumi.Input[str]] = None,
                  subnet: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a DeviceLink resource.
         :param pulumi.Input[Sequence[pulumi.Input['DeviceLinkDeviceArgs']]] devices: definition of one or more devices belonging to the
                device link. See Device section below for more details.
         :param pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]] links: definition of one or more, inter metro, connections belonging
                to the device link. See Link section below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]] metro_links: definition of one or more, inter metro, connections belonging
+               to the device link. See Metro Link section below for more details.
         :param pulumi.Input[str] name: device link name.
         :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the device link is scoped to.If you
                leave it out, the device link will be created under the default project id of your organization.
+        :param pulumi.Input[str] redundancy_type: Whether the connection should be created through 
+               Fabric's primary or secondary port. Supported values: `PRIMARY` (Default), `SECONDARY`, `HYBRID`
         :param pulumi.Input[str] subnet: device link subnet in CIDR format. Not required for link
                between self configured devices.
         """
         pulumi.set(__self__, "devices", devices)
         if links is not None:
+            warnings.warn("""Links is deprecated. Please use metro links instead.""", DeprecationWarning)
+            pulumi.log.warn("""links is deprecated: Links is deprecated. Please use metro links instead.""")
+        if links is not None:
             pulumi.set(__self__, "links", links)
+        if metro_links is not None:
+            pulumi.set(__self__, "metro_links", metro_links)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
+        if redundancy_type is not None:
+            pulumi.set(__self__, "redundancy_type", redundancy_type)
         if subnet is not None:
             pulumi.set(__self__, "subnet", subnet)
 
     @property
     @pulumi.getter
     def devices(self) -> pulumi.Input[Sequence[pulumi.Input['DeviceLinkDeviceArgs']]]:
         """
@@ -59,21 +72,37 @@
     @property
     @pulumi.getter
     def links(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]]]:
         """
         definition of one or more, inter metro, connections belonging
         to the device link. See Link section below for more details.
         """
+        warnings.warn("""Links is deprecated. Please use metro links instead.""", DeprecationWarning)
+        pulumi.log.warn("""links is deprecated: Links is deprecated. Please use metro links instead.""")
+
         return pulumi.get(self, "links")
 
     @links.setter
     def links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]]]):
         pulumi.set(self, "links", value)
 
     @property
+    @pulumi.getter(name="metroLinks")
+    def metro_links(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]]]:
+        """
+        definition of one or more, inter metro, connections belonging
+        to the device link. See Metro Link section below for more details.
+        """
+        return pulumi.get(self, "metro_links")
+
+    @metro_links.setter
+    def metro_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]]]):
+        pulumi.set(self, "metro_links", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         device link name.
         """
         return pulumi.get(self, "name")
 
@@ -91,14 +120,27 @@
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_id", value)
 
     @property
+    @pulumi.getter(name="redundancyType")
+    def redundancy_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Whether the connection should be created through 
+        Fabric's primary or secondary port. Supported values: `PRIMARY` (Default), `SECONDARY`, `HYBRID`
+        """
+        return pulumi.get(self, "redundancy_type")
+
+    @redundancy_type.setter
+    def redundancy_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redundancy_type", value)
+
+    @property
     @pulumi.getter
     def subnet(self) -> Optional[pulumi.Input[str]]:
         """
         device link subnet in CIDR format. Not required for link
         between self configured devices.
         """
         return pulumi.get(self, "subnet")
@@ -109,42 +151,55 @@
 
 
 @pulumi.input_type
 class _DeviceLinkState:
     def __init__(__self__, *,
                  devices: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkDeviceArgs']]]] = None,
                  links: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]]] = None,
+                 metro_links: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
+                 redundancy_type: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  subnet: Optional[pulumi.Input[str]] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering DeviceLink resources.
         :param pulumi.Input[Sequence[pulumi.Input['DeviceLinkDeviceArgs']]] devices: definition of one or more devices belonging to the
                device link. See Device section below for more details.
         :param pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]] links: definition of one or more, inter metro, connections belonging
                to the device link. See Link section below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]] metro_links: definition of one or more, inter metro, connections belonging
+               to the device link. See Metro Link section below for more details.
         :param pulumi.Input[str] name: device link name.
         :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the device link is scoped to.If you
                leave it out, the device link will be created under the default project id of your organization.
+        :param pulumi.Input[str] redundancy_type: Whether the connection should be created through 
+               Fabric's primary or secondary port. Supported values: `PRIMARY` (Default), `SECONDARY`, `HYBRID`
         :param pulumi.Input[str] status: device link provisioning status on a given device. One of `PROVISIONING`,
                `PROVISIONED`, `DEPROVISIONING`, `DEPROVISIONED`, `FAILED`.
         :param pulumi.Input[str] subnet: device link subnet in CIDR format. Not required for link
                between self configured devices.
         :param pulumi.Input[str] uuid: Device link unique identifier.
         """
         if devices is not None:
             pulumi.set(__self__, "devices", devices)
         if links is not None:
+            warnings.warn("""Links is deprecated. Please use metro links instead.""", DeprecationWarning)
+            pulumi.log.warn("""links is deprecated: Links is deprecated. Please use metro links instead.""")
+        if links is not None:
             pulumi.set(__self__, "links", links)
+        if metro_links is not None:
+            pulumi.set(__self__, "metro_links", metro_links)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
+        if redundancy_type is not None:
+            pulumi.set(__self__, "redundancy_type", redundancy_type)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if subnet is not None:
             pulumi.set(__self__, "subnet", subnet)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
@@ -164,21 +219,37 @@
     @property
     @pulumi.getter
     def links(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]]]:
         """
         definition of one or more, inter metro, connections belonging
         to the device link. See Link section below for more details.
         """
+        warnings.warn("""Links is deprecated. Please use metro links instead.""", DeprecationWarning)
+        pulumi.log.warn("""links is deprecated: Links is deprecated. Please use metro links instead.""")
+
         return pulumi.get(self, "links")
 
     @links.setter
     def links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkLinkArgs']]]]):
         pulumi.set(self, "links", value)
 
     @property
+    @pulumi.getter(name="metroLinks")
+    def metro_links(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]]]:
+        """
+        definition of one or more, inter metro, connections belonging
+        to the device link. See Metro Link section below for more details.
+        """
+        return pulumi.get(self, "metro_links")
+
+    @metro_links.setter
+    def metro_links(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DeviceLinkMetroLinkArgs']]]]):
+        pulumi.set(self, "metro_links", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         device link name.
         """
         return pulumi.get(self, "name")
 
@@ -196,14 +267,27 @@
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_id", value)
 
     @property
+    @pulumi.getter(name="redundancyType")
+    def redundancy_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Whether the connection should be created through 
+        Fabric's primary or secondary port. Supported values: `PRIMARY` (Default), `SECONDARY`, `HYBRID`
+        """
+        return pulumi.get(self, "redundancy_type")
+
+    @redundancy_type.setter
+    def redundancy_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redundancy_type", value)
+
+    @property
     @pulumi.getter
     def status(self) -> Optional[pulumi.Input[str]]:
         """
         device link provisioning status on a given device. One of `PROVISIONING`,
         `PROVISIONED`, `DEPROVISIONING`, `DEPROVISIONED`, `FAILED`.
         """
         return pulumi.get(self, "status")
@@ -241,16 +325,18 @@
 class DeviceLink(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkDeviceArgs']]]]] = None,
                  links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkLinkArgs']]]]] = None,
+                 metro_links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkMetroLinkArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
+                 redundancy_type: Optional[pulumi.Input[str]] = None,
                  subnet: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Resource `networkedge.DeviceLink` allows creation and management of Equinix
         Network Edge virtual network device links.
 
         ## Example Usage
@@ -303,17 +389,21 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkDeviceArgs']]]] devices: definition of one or more devices belonging to the
                device link. See Device section below for more details.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkLinkArgs']]]] links: definition of one or more, inter metro, connections belonging
                to the device link. See Link section below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkMetroLinkArgs']]]] metro_links: definition of one or more, inter metro, connections belonging
+               to the device link. See Metro Link section below for more details.
         :param pulumi.Input[str] name: device link name.
         :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the device link is scoped to.If you
                leave it out, the device link will be created under the default project id of your organization.
+        :param pulumi.Input[str] redundancy_type: Whether the connection should be created through 
+               Fabric's primary or secondary port. Supported values: `PRIMARY` (Default), `SECONDARY`, `HYBRID`
         :param pulumi.Input[str] subnet: device link subnet in CIDR format. Not required for link
                between self configured devices.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -384,32 +474,36 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkDeviceArgs']]]]] = None,
                  links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkLinkArgs']]]]] = None,
+                 metro_links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkMetroLinkArgs']]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
+                 redundancy_type: Optional[pulumi.Input[str]] = None,
                  subnet: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = DeviceLinkArgs.__new__(DeviceLinkArgs)
 
             if devices is None and not opts.urn:
                 raise TypeError("Missing required property 'devices'")
             __props__.__dict__["devices"] = devices
             __props__.__dict__["links"] = links
+            __props__.__dict__["metro_links"] = metro_links
             __props__.__dict__["name"] = name
             __props__.__dict__["project_id"] = project_id
+            __props__.__dict__["redundancy_type"] = redundancy_type
             __props__.__dict__["subnet"] = subnet
             __props__.__dict__["status"] = None
             __props__.__dict__["uuid"] = None
         super(DeviceLink, __self__).__init__(
             'equinix:networkedge/deviceLink:DeviceLink',
             resource_name,
             __props__,
@@ -417,47 +511,55 @@
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkDeviceArgs']]]]] = None,
             links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkLinkArgs']]]]] = None,
+            metro_links: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkMetroLinkArgs']]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             project_id: Optional[pulumi.Input[str]] = None,
+            redundancy_type: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
             subnet: Optional[pulumi.Input[str]] = None,
             uuid: Optional[pulumi.Input[str]] = None) -> 'DeviceLink':
         """
         Get an existing DeviceLink resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkDeviceArgs']]]] devices: definition of one or more devices belonging to the
                device link. See Device section below for more details.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkLinkArgs']]]] links: definition of one or more, inter metro, connections belonging
                to the device link. See Link section below for more details.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkMetroLinkArgs']]]] metro_links: definition of one or more, inter metro, connections belonging
+               to the device link. See Metro Link section below for more details.
         :param pulumi.Input[str] name: device link name.
         :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the device link is scoped to.If you
                leave it out, the device link will be created under the default project id of your organization.
+        :param pulumi.Input[str] redundancy_type: Whether the connection should be created through 
+               Fabric's primary or secondary port. Supported values: `PRIMARY` (Default), `SECONDARY`, `HYBRID`
         :param pulumi.Input[str] status: device link provisioning status on a given device. One of `PROVISIONING`,
                `PROVISIONED`, `DEPROVISIONING`, `DEPROVISIONED`, `FAILED`.
         :param pulumi.Input[str] subnet: device link subnet in CIDR format. Not required for link
                between self configured devices.
         :param pulumi.Input[str] uuid: Device link unique identifier.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _DeviceLinkState.__new__(_DeviceLinkState)
 
         __props__.__dict__["devices"] = devices
         __props__.__dict__["links"] = links
+        __props__.__dict__["metro_links"] = metro_links
         __props__.__dict__["name"] = name
         __props__.__dict__["project_id"] = project_id
+        __props__.__dict__["redundancy_type"] = redundancy_type
         __props__.__dict__["status"] = status
         __props__.__dict__["subnet"] = subnet
         __props__.__dict__["uuid"] = uuid
         return DeviceLink(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
@@ -471,17 +573,29 @@
     @property
     @pulumi.getter
     def links(self) -> pulumi.Output[Optional[Sequence['outputs.DeviceLinkLink']]]:
         """
         definition of one or more, inter metro, connections belonging
         to the device link. See Link section below for more details.
         """
+        warnings.warn("""Links is deprecated. Please use metro links instead.""", DeprecationWarning)
+        pulumi.log.warn("""links is deprecated: Links is deprecated. Please use metro links instead.""")
+
         return pulumi.get(self, "links")
 
     @property
+    @pulumi.getter(name="metroLinks")
+    def metro_links(self) -> pulumi.Output[Optional[Sequence['outputs.DeviceLinkMetroLink']]]:
+        """
+        definition of one or more, inter metro, connections belonging
+        to the device link. See Metro Link section below for more details.
+        """
+        return pulumi.get(self, "metro_links")
+
+    @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         device link name.
         """
         return pulumi.get(self, "name")
 
@@ -491,14 +605,23 @@
         """
         Unique Identifier for the project resource where the device link is scoped to.If you
         leave it out, the device link will be created under the default project id of your organization.
         """
         return pulumi.get(self, "project_id")
 
     @property
+    @pulumi.getter(name="redundancyType")
+    def redundancy_type(self) -> pulumi.Output[Optional[str]]:
+        """
+        Whether the connection should be created through 
+        Fabric's primary or secondary port. Supported values: `PRIMARY` (Default), `SECONDARY`, `HYBRID`
+        """
+        return pulumi.get(self, "redundancy_type")
+
+    @property
     @pulumi.getter
     def status(self) -> pulumi.Output[str]:
         """
         device link provisioning status on a given device. One of `PROVISIONING`,
         `PROVISIONED`, `DEPROVISIONING`, `DEPROVISIONED`, `FAILED`.
         """
         return pulumi.get(self, "status")
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_account.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,25 +114,23 @@
     billing account in a given metro location.
 
     Billing account reference is required to create Network Edge virtual device
     in corresponding metro location.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dc = equinix.networkedge.get_account(metro_code="DC",
         status="Active",
         project_id="a86d7112-d740-4758-9c9c-31e66373746b")
     pulumi.export("number", dc.number)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str metro_code: Account location metro code.
     :param str name: Account name for filtering.
     :param str project_id: Unique Identifier for the project resource where the account is scoped to.If you
            leave it out, all the billing accounts under all projects in your organization will be returned and it may return more than one account.
     :param str status: Account status for filtering. Possible values are: `Active`, `Processing`,
@@ -167,25 +165,23 @@
     billing account in a given metro location.
 
     Billing account reference is required to create Network Edge virtual device
     in corresponding metro location.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dc = equinix.networkedge.get_account(metro_code="DC",
         status="Active",
         project_id="a86d7112-d740-4758-9c9c-31e66373746b")
     pulumi.export("number", dc.number)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str metro_code: Account location metro code.
     :param str name: Account name for filtering.
     :param str project_id: Unique Identifier for the project resource where the account is scoped to.If you
            leave it out, all the billing accounts under all projects in your organization will be returned and it may return more than one account.
     :param str status: Account status for filtering. Possible values are: `Active`, `Processing`,
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_device.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -536,23 +536,21 @@
                valid_status_list: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDeviceResult:
     """
     Use this data source to get Equinix Network Edge device details.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     by_uuid = equinix.networkedge.get_device(uuid="f0b5c553-cdeb-4bc3-95b8-23db9ccfd5ee")
     by_name = equinix.networkedge.get_device(name="Arcus-Gateway-A1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of an existing Equinix Network Edge device
     :param str uuid: UUID of an existing Equinix Network Edge device
     :param str valid_status_list: Device states to be considered valid when searching for a device by name
            
            NOTE: Exactly one of either `uuid` or `name` must be specified.
@@ -619,23 +617,21 @@
                       valid_status_list: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDeviceResult]:
     """
     Use this data source to get Equinix Network Edge device details.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     by_uuid = equinix.networkedge.get_device(uuid="f0b5c553-cdeb-4bc3-95b8-23db9ccfd5ee")
     by_name = equinix.networkedge.get_device(name="Arcus-Gateway-A1")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of an existing Equinix Network Edge device
     :param str uuid: UUID of an existing Equinix Network Edge device
     :param str valid_status_list: Device states to be considered valid when searching for a device by name
            
            NOTE: Exactly one of either `uuid` or `name` must be specified.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_device_platform.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,24 +132,22 @@
     """
     Use this data source to get Equinix Network Edge device platform configuration details
     for a given device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_large = equinix.networkedge.get_device_platform(device_type="CSR1000V",
         flavor="large",
         packages=["IPBASE"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int core_count: Number of CPU cores used to limit platform search results.
     :param str device_type: Device type code
     :param str flavor: Device platform flavor that determines number of CPU cores and memory.
            Supported values are: `small`, `medium`, `large`, `xlarge`.
     :param Sequence[str] license_options: List of device licensing options to limit platform search result.
@@ -191,24 +189,22 @@
     """
     Use this data source to get Equinix Network Edge device platform configuration details
     for a given device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_large = equinix.networkedge.get_device_platform(device_type="CSR1000V",
         flavor="large",
         packages=["IPBASE"])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param int core_count: Number of CPU cores used to limit platform search results.
     :param str device_type: Device type code
     :param str flavor: Device platform flavor that determines number of CPU cores and memory.
            Supported values are: `small`, `medium`, `large`, `xlarge`.
     :param Sequence[str] license_options: List of device licensing options to limit platform search result.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/get_device_software.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_software.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,25 +158,23 @@
     """
     Use this data source to get Equinix Network Edge device software details for a given
     device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_latest1609 = equinix.networkedge.get_device_software(device_type="CSR1000V",
         most_recent=True,
         packages=["IPBASE"],
         version_regex="^16.09.+")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_type: Code of a device type.
     :param bool most_recent: Boolean value to indicate that most recent version should be used *(in
            case when more than one result is returned)*.
     :param Sequence[str] packages: Limits returned versions to those that are supported by given software
            package codes.
@@ -217,25 +215,23 @@
     """
     Use this data source to get Equinix Network Edge device software details for a given
     device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_latest1609 = equinix.networkedge.get_device_software(device_type="CSR1000V",
         most_recent=True,
         packages=["IPBASE"],
         version_regex="^16.09.+")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str device_type: Code of a device type.
     :param bool most_recent: Boolean value to indicate that most recent version should be used *(in
            case when more than one result is returned)*.
     :param Sequence[str] packages: Limits returned versions to those that are supported by given software
            package codes.
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/network_file.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/network_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/outputs.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     'DeviceClusterDetailsNode0',
     'DeviceClusterDetailsNode0VendorConfiguration',
     'DeviceClusterDetailsNode1',
     'DeviceClusterDetailsNode1VendorConfiguration',
     'DeviceInterface',
     'DeviceLinkDevice',
     'DeviceLinkLink',
+    'DeviceLinkMetroLink',
     'DeviceSecondaryDevice',
     'DeviceSecondaryDeviceInterface',
     'DeviceSecondaryDeviceSshKey',
     'DeviceSshKey',
     'GetDeviceClusterDetailResult',
     'GetDeviceClusterDetailNode0Result',
     'GetDeviceClusterDetailNode0VendorConfigurationResult',
@@ -348,23 +349,21 @@
     def __init__(__self__, *,
                  license_file_id: Optional[str] = None,
                  license_token: Optional[str] = None,
                  name: Optional[str] = None,
                  uuid: Optional[str] = None,
                  vendor_configuration: Optional['outputs.DeviceClusterDetailsNode0VendorConfiguration'] = None):
         """
-        :param str license_file_id: Identifier of a license file that will be applied on the device.
-        :param str license_token: License Token applicable for some device types in BYOL licensing
-               mode.
+        :param str license_file_id: License file id. This is necessary for Fortinet and Juniper clusters.
+        :param str license_token: License token. This is necessary for Palo Alto clusters.
         :param str name: Device name.
         :param str uuid: Device unique identifier.
-        :param 'DeviceClusterDetailsNode0VendorConfigurationArgs' vendor_configuration: Map of vendor specific configuration parameters for a device
-               (controller1, activationKey, managementType, siteId, systemIpAddress)
-               * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-               on a device (max one key).  See SSH Key below for more details.
+        :param 'DeviceClusterDetailsNode0VendorConfigurationArgs' vendor_configuration: An object that has fields relevant to the vendor of the
+               cluster device. See Cluster Details - Nodes - Vendor Configuration
+               below for more details.
         """
         if license_file_id is not None:
             pulumi.set(__self__, "license_file_id", license_file_id)
         if license_token is not None:
             pulumi.set(__self__, "license_token", license_token)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -373,24 +372,23 @@
         if vendor_configuration is not None:
             pulumi.set(__self__, "vendor_configuration", vendor_configuration)
 
     @property
     @pulumi.getter(name="licenseFileId")
     def license_file_id(self) -> Optional[str]:
         """
-        Identifier of a license file that will be applied on the device.
+        License file id. This is necessary for Fortinet and Juniper clusters.
         """
         return pulumi.get(self, "license_file_id")
 
     @property
     @pulumi.getter(name="licenseToken")
     def license_token(self) -> Optional[str]:
         """
-        License Token applicable for some device types in BYOL licensing
-        mode.
+        License token. This is necessary for Palo Alto clusters.
         """
         return pulumi.get(self, "license_token")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -406,18 +404,17 @@
         """
         return pulumi.get(self, "uuid")
 
     @property
     @pulumi.getter(name="vendorConfiguration")
     def vendor_configuration(self) -> Optional['outputs.DeviceClusterDetailsNode0VendorConfiguration']:
         """
-        Map of vendor specific configuration parameters for a device
-        (controller1, activationKey, managementType, siteId, systemIpAddress)
-        * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-        on a device (max one key).  See SSH Key below for more details.
+        An object that has fields relevant to the vendor of the
+        cluster device. See Cluster Details - Nodes - Vendor Configuration
+        below for more details.
         """
         return pulumi.get(self, "vendor_configuration")
 
 
 @pulumi.output_type
 class DeviceClusterDetailsNode0VendorConfiguration(dict):
     @staticmethod
@@ -550,23 +547,21 @@
     def __init__(__self__, *,
                  license_file_id: Optional[str] = None,
                  license_token: Optional[str] = None,
                  name: Optional[str] = None,
                  uuid: Optional[str] = None,
                  vendor_configuration: Optional['outputs.DeviceClusterDetailsNode1VendorConfiguration'] = None):
         """
-        :param str license_file_id: Identifier of a license file that will be applied on the device.
-        :param str license_token: License Token applicable for some device types in BYOL licensing
-               mode.
+        :param str license_file_id: License file id. This is necessary for Fortinet and Juniper clusters.
+        :param str license_token: License token. This is necessary for Palo Alto clusters.
         :param str name: Device name.
         :param str uuid: Device unique identifier.
-        :param 'DeviceClusterDetailsNode1VendorConfigurationArgs' vendor_configuration: Map of vendor specific configuration parameters for a device
-               (controller1, activationKey, managementType, siteId, systemIpAddress)
-               * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-               on a device (max one key).  See SSH Key below for more details.
+        :param 'DeviceClusterDetailsNode1VendorConfigurationArgs' vendor_configuration: An object that has fields relevant to the vendor of the
+               cluster device. See Cluster Details - Nodes - Vendor Configuration
+               below for more details.
         """
         if license_file_id is not None:
             pulumi.set(__self__, "license_file_id", license_file_id)
         if license_token is not None:
             pulumi.set(__self__, "license_token", license_token)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -575,24 +570,23 @@
         if vendor_configuration is not None:
             pulumi.set(__self__, "vendor_configuration", vendor_configuration)
 
     @property
     @pulumi.getter(name="licenseFileId")
     def license_file_id(self) -> Optional[str]:
         """
-        Identifier of a license file that will be applied on the device.
+        License file id. This is necessary for Fortinet and Juniper clusters.
         """
         return pulumi.get(self, "license_file_id")
 
     @property
     @pulumi.getter(name="licenseToken")
     def license_token(self) -> Optional[str]:
         """
-        License Token applicable for some device types in BYOL licensing
-        mode.
+        License token. This is necessary for Palo Alto clusters.
         """
         return pulumi.get(self, "license_token")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
@@ -608,18 +602,17 @@
         """
         return pulumi.get(self, "uuid")
 
     @property
     @pulumi.getter(name="vendorConfiguration")
     def vendor_configuration(self) -> Optional['outputs.DeviceClusterDetailsNode1VendorConfiguration']:
         """
-        Map of vendor specific configuration parameters for a device
-        (controller1, activationKey, managementType, siteId, systemIpAddress)
-        * `ssh-key` - (Optional) Definition of SSH key that will be provisioned
-        on a device (max one key).  See SSH Key below for more details.
+        An object that has fields relevant to the vendor of the
+        cluster device. See Cluster Details - Nodes - Vendor Configuration
+        below for more details.
         """
         return pulumi.get(self, "vendor_configuration")
 
 
 @pulumi.output_type
 class DeviceClusterDetailsNode1VendorConfiguration(dict):
     @staticmethod
@@ -1059,14 +1052,88 @@
         warnings.warn("""SourceZoneCode is not required""", DeprecationWarning)
         pulumi.log.warn("""src_zone_code is deprecated: SourceZoneCode is not required""")
 
         return pulumi.get(self, "src_zone_code")
 
 
 @pulumi.output_type
+class DeviceLinkMetroLink(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "accountNumber":
+            suggest = "account_number"
+        elif key == "metroCode":
+            suggest = "metro_code"
+        elif key == "throughputUnit":
+            suggest = "throughput_unit"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DeviceLinkMetroLink. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DeviceLinkMetroLink.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DeviceLinkMetroLink.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 account_number: str,
+                 metro_code: str,
+                 throughput: str,
+                 throughput_unit: str):
+        """
+        :param str account_number: billing account number to be used for
+               connection charges
+        :param str metro_code: connection metro code.
+        :param str throughput: connection throughput.
+        :param str throughput_unit: connection throughput unit (Mbps or Gbps).
+        """
+        pulumi.set(__self__, "account_number", account_number)
+        pulumi.set(__self__, "metro_code", metro_code)
+        pulumi.set(__self__, "throughput", throughput)
+        pulumi.set(__self__, "throughput_unit", throughput_unit)
+
+    @property
+    @pulumi.getter(name="accountNumber")
+    def account_number(self) -> str:
+        """
+        billing account number to be used for
+        connection charges
+        """
+        return pulumi.get(self, "account_number")
+
+    @property
+    @pulumi.getter(name="metroCode")
+    def metro_code(self) -> str:
+        """
+        connection metro code.
+        """
+        return pulumi.get(self, "metro_code")
+
+    @property
+    @pulumi.getter
+    def throughput(self) -> str:
+        """
+        connection throughput.
+        """
+        return pulumi.get(self, "throughput")
+
+    @property
+    @pulumi.getter(name="throughputUnit")
+    def throughput_unit(self) -> str:
+        """
+        connection throughput unit (Mbps or Gbps).
+        """
+        return pulumi.get(self, "throughput_unit")
+
+
+@pulumi.output_type
 class DeviceSecondaryDevice(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "accountNumber":
             suggest = "account_number"
         elif key == "metroCode":
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/ssh_key.py` & `pulumi_equinix-0.9.0/pulumi_equinix/provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,365 +3,299 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 
-__all__ = ['SshKeyArgs', 'SshKey']
+__all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
-class SshKeyArgs:
+class ProviderArgs:
     def __init__(__self__, *,
-                 public_key: pulumi.Input[str],
-                 name: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a SshKey resource.
-        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
-               interpolation function.
-        :param pulumi.Input[str] name: The name of SSH key used for identification.
-        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
-               leave it out, the ssh key will be created under the default project id of your organization.
-        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
-        """
-        pulumi.set(__self__, "public_key", public_key)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter(name="publicKey")
-    def public_key(self) -> pulumi.Input[str]:
-        """
-        The SSH public key. If this is a file, it can be read using the file
-        interpolation function.
-        """
-        return pulumi.get(self, "public_key")
-
-    @public_key.setter
-    def public_key(self, value: pulumi.Input[str]):
-        pulumi.set(self, "public_key", value)
+                 auth_token: Optional[pulumi.Input[str]] = None,
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 client_secret: Optional[pulumi.Input[str]] = None,
+                 endpoint: Optional[pulumi.Input[str]] = None,
+                 max_retries: Optional[pulumi.Input[int]] = None,
+                 max_retry_wait_seconds: Optional[pulumi.Input[int]] = None,
+                 request_timeout: Optional[pulumi.Input[int]] = None,
+                 response_max_page_size: Optional[pulumi.Input[int]] = None,
+                 token: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] auth_token: The Equinix Metal API auth key for API operations
+        :param pulumi.Input[str] client_id: API Consumer Key available under My Apps section in developer portal
+        :param pulumi.Input[str] client_secret: API Consumer secret available under My Apps section in developer portal
+        :param pulumi.Input[str] endpoint: The Equinix API base URL to point out desired environment. Defaults to https://api.equinix.com
+        :param pulumi.Input[int] max_retries: Maximum number of retries.
+        :param pulumi.Input[int] max_retry_wait_seconds: Maximum number of seconds to wait before retrying a request.
+        :param pulumi.Input[int] request_timeout: The duration of time, in seconds, that the Equinix Platform API Client should wait before canceling an API request.
+               Defaults to 30
+        :param pulumi.Input[int] response_max_page_size: The maximum number of records in a single response for REST queries that produce paginated responses
+        :param pulumi.Input[str] token: API token from the developer sandbox
+        """
+        if auth_token is not None:
+            pulumi.set(__self__, "auth_token", auth_token)
+        if client_id is not None:
+            pulumi.set(__self__, "client_id", client_id)
+        if client_secret is not None:
+            pulumi.set(__self__, "client_secret", client_secret)
+        if endpoint is not None:
+            pulumi.set(__self__, "endpoint", endpoint)
+        if max_retries is not None:
+            pulumi.set(__self__, "max_retries", max_retries)
+        if max_retry_wait_seconds is not None:
+            pulumi.set(__self__, "max_retry_wait_seconds", max_retry_wait_seconds)
+        if request_timeout is not None:
+            pulumi.set(__self__, "request_timeout", request_timeout)
+        if response_max_page_size is not None:
+            pulumi.set(__self__, "response_max_page_size", response_max_page_size)
+        if token is not None:
+            pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter(name="authToken")
+    def auth_token(self) -> Optional[pulumi.Input[str]]:
+        """
+        The Equinix Metal API auth key for API operations
+        """
+        return pulumi.get(self, "auth_token")
+
+    @auth_token.setter
+    def auth_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "auth_token", value)
+
+    @property
+    @pulumi.getter(name="clientId")
+    def client_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        API Consumer Key available under My Apps section in developer portal
+        """
+        return pulumi.get(self, "client_id")
+
+    @client_id.setter
+    def client_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "client_id", value)
+
+    @property
+    @pulumi.getter(name="clientSecret")
+    def client_secret(self) -> Optional[pulumi.Input[str]]:
+        """
+        API Consumer secret available under My Apps section in developer portal
+        """
+        return pulumi.get(self, "client_secret")
+
+    @client_secret.setter
+    def client_secret(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "client_secret", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def endpoint(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of SSH key used for identification.
+        The Equinix API base URL to point out desired environment. Defaults to https://api.equinix.com
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "endpoint")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @endpoint.setter
+    def endpoint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "endpoint", value)
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="maxRetries")
+    def max_retries(self) -> Optional[pulumi.Input[int]]:
         """
-        Unique Identifier for the project resource where the SSH key is scoped to.If you
-        leave it out, the ssh key will be created under the default project id of your organization.
+        Maximum number of retries.
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "max_retries")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_id", value)
+    @max_retries.setter
+    def max_retries(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "max_retries", value)
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The type of SSH key: `RSA` (default) or `DSA`.
-        """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
-
-
-@pulumi.input_type
-class _SshKeyState:
-    def __init__(__self__, *,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 public_key: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
-                 uuid: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering SshKey resources.
-        :param pulumi.Input[str] name: The name of SSH key used for identification.
-        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
-               leave it out, the ssh key will be created under the default project id of your organization.
-        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
-               interpolation function.
-        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
-        :param pulumi.Input[str] uuid: The unique identifier of the key
-        """
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if project_id is not None:
-            pulumi.set(__self__, "project_id", project_id)
-        if public_key is not None:
-            pulumi.set(__self__, "public_key", public_key)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-        if uuid is not None:
-            pulumi.set(__self__, "uuid", uuid)
-
-    @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of SSH key used for identification.
+    @pulumi.getter(name="maxRetryWaitSeconds")
+    def max_retry_wait_seconds(self) -> Optional[pulumi.Input[int]]:
         """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> Optional[pulumi.Input[str]]:
+        Maximum number of seconds to wait before retrying a request.
         """
-        Unique Identifier for the project resource where the SSH key is scoped to.If you
-        leave it out, the ssh key will be created under the default project id of your organization.
-        """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "max_retry_wait_seconds")
 
-    @project_id.setter
-    def project_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_id", value)
+    @max_retry_wait_seconds.setter
+    def max_retry_wait_seconds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "max_retry_wait_seconds", value)
 
     @property
-    @pulumi.getter(name="publicKey")
-    def public_key(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="requestTimeout")
+    def request_timeout(self) -> Optional[pulumi.Input[int]]:
         """
-        The SSH public key. If this is a file, it can be read using the file
-        interpolation function.
+        The duration of time, in seconds, that the Equinix Platform API Client should wait before canceling an API request.
+        Defaults to 30
         """
-        return pulumi.get(self, "public_key")
+        return pulumi.get(self, "request_timeout")
 
-    @public_key.setter
-    def public_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "public_key", value)
+    @request_timeout.setter
+    def request_timeout(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "request_timeout", value)
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="responseMaxPageSize")
+    def response_max_page_size(self) -> Optional[pulumi.Input[int]]:
         """
-        The type of SSH key: `RSA` (default) or `DSA`.
+        The maximum number of records in a single response for REST queries that produce paginated responses
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "response_max_page_size")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @response_max_page_size.setter
+    def response_max_page_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "response_max_page_size", value)
 
     @property
     @pulumi.getter
-    def uuid(self) -> Optional[pulumi.Input[str]]:
+    def token(self) -> Optional[pulumi.Input[str]]:
         """
-        The unique identifier of the key
+        API token from the developer sandbox
         """
-        return pulumi.get(self, "uuid")
+        return pulumi.get(self, "token")
 
-    @uuid.setter
-    def uuid(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "uuid", value)
+    @token.setter
+    def token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token", value)
 
 
-class SshKey(pulumi.CustomResource):
+class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 public_key: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 auth_token: Optional[pulumi.Input[str]] = None,
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 client_secret: Optional[pulumi.Input[str]] = None,
+                 endpoint: Optional[pulumi.Input[str]] = None,
+                 max_retries: Optional[pulumi.Input[int]] = None,
+                 max_retry_wait_seconds: Optional[pulumi.Input[int]] = None,
+                 request_timeout: Optional[pulumi.Input[int]] = None,
+                 response_max_page_size: Optional[pulumi.Input[int]] = None,
+                 token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Resource `networkedge.SshKey` allows creation and management of Equinix Network Edge SSH keys.
-
-        ## Example Usage
-        ```python
-        import pulumi
-        import pulumi_equinix as equinix
-
-        ssh_key = equinix.networkedge.SshKey("sshKey",
-            name="johnKent",
-            public_key=(lambda path: open(path).read())("/Users/John/.ssh/ne_rsa.pub"))
-        pulumi.export("sshKeyId", ssh_key.id)
-        ```
-
-        ## Import
-
-        This resource can be imported using an existing ID:
-
-        ```sh
-        $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id}
-        ```
+        The provider type for the equinix package. By default, resources use package-wide configuration
+        settings, however an explicit `Provider` instance may be created and passed during resource
+        construction to achieve fine-grained programmatic control over provider settings. See the
+        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The name of SSH key used for identification.
-        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
-               leave it out, the ssh key will be created under the default project id of your organization.
-        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
-               interpolation function.
-        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
+        :param pulumi.Input[str] auth_token: The Equinix Metal API auth key for API operations
+        :param pulumi.Input[str] client_id: API Consumer Key available under My Apps section in developer portal
+        :param pulumi.Input[str] client_secret: API Consumer secret available under My Apps section in developer portal
+        :param pulumi.Input[str] endpoint: The Equinix API base URL to point out desired environment. Defaults to https://api.equinix.com
+        :param pulumi.Input[int] max_retries: Maximum number of retries.
+        :param pulumi.Input[int] max_retry_wait_seconds: Maximum number of seconds to wait before retrying a request.
+        :param pulumi.Input[int] request_timeout: The duration of time, in seconds, that the Equinix Platform API Client should wait before canceling an API request.
+               Defaults to 30
+        :param pulumi.Input[int] response_max_page_size: The maximum number of records in a single response for REST queries that produce paginated responses
+        :param pulumi.Input[str] token: API token from the developer sandbox
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: SshKeyArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Resource `networkedge.SshKey` allows creation and management of Equinix Network Edge SSH keys.
-
-        ## Example Usage
-        ```python
-        import pulumi
-        import pulumi_equinix as equinix
-
-        ssh_key = equinix.networkedge.SshKey("sshKey",
-            name="johnKent",
-            public_key=(lambda path: open(path).read())("/Users/John/.ssh/ne_rsa.pub"))
-        pulumi.export("sshKeyId", ssh_key.id)
-        ```
-
-        ## Import
-
-        This resource can be imported using an existing ID:
-
-        ```sh
-        $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id}
-        ```
+        The provider type for the equinix package. By default, resources use package-wide configuration
+        settings, however an explicit `Provider` instance may be created and passed during resource
+        construction to achieve fine-grained programmatic control over provider settings. See the
+        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
-        :param SshKeyArgs args: The arguments to use to populate this resource's properties.
+        :param ProviderArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SshKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProviderArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 project_id: Optional[pulumi.Input[str]] = None,
-                 public_key: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 auth_token: Optional[pulumi.Input[str]] = None,
+                 client_id: Optional[pulumi.Input[str]] = None,
+                 client_secret: Optional[pulumi.Input[str]] = None,
+                 endpoint: Optional[pulumi.Input[str]] = None,
+                 max_retries: Optional[pulumi.Input[int]] = None,
+                 max_retry_wait_seconds: Optional[pulumi.Input[int]] = None,
+                 request_timeout: Optional[pulumi.Input[int]] = None,
+                 response_max_page_size: Optional[pulumi.Input[int]] = None,
+                 token: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SshKeyArgs.__new__(SshKeyArgs)
+            __props__ = ProviderArgs.__new__(ProviderArgs)
 
-            __props__.__dict__["name"] = name
-            __props__.__dict__["project_id"] = project_id
-            if public_key is None and not opts.urn:
-                raise TypeError("Missing required property 'public_key'")
-            __props__.__dict__["public_key"] = public_key
-            __props__.__dict__["type"] = type
-            __props__.__dict__["uuid"] = None
-        super(SshKey, __self__).__init__(
-            'equinix:networkedge/sshKey:SshKey',
+            __props__.__dict__["auth_token"] = auth_token
+            __props__.__dict__["client_id"] = client_id
+            __props__.__dict__["client_secret"] = client_secret
+            __props__.__dict__["endpoint"] = endpoint
+            __props__.__dict__["max_retries"] = pulumi.Output.from_input(max_retries).apply(pulumi.runtime.to_json) if max_retries is not None else None
+            __props__.__dict__["max_retry_wait_seconds"] = pulumi.Output.from_input(max_retry_wait_seconds).apply(pulumi.runtime.to_json) if max_retry_wait_seconds is not None else None
+            __props__.__dict__["request_timeout"] = pulumi.Output.from_input(request_timeout).apply(pulumi.runtime.to_json) if request_timeout is not None else None
+            __props__.__dict__["response_max_page_size"] = pulumi.Output.from_input(response_max_page_size).apply(pulumi.runtime.to_json) if response_max_page_size is not None else None
+            __props__.__dict__["token"] = token
+        super(Provider, __self__).__init__(
+            'equinix',
             resource_name,
             __props__,
             opts)
 
-    @staticmethod
-    def get(resource_name: str,
-            id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            project_id: Optional[pulumi.Input[str]] = None,
-            public_key: Optional[pulumi.Input[str]] = None,
-            type: Optional[pulumi.Input[str]] = None,
-            uuid: Optional[pulumi.Input[str]] = None) -> 'SshKey':
-        """
-        Get an existing SshKey resource's state with the given name, id, and optional extra
-        properties used to qualify the lookup.
-
-        :param str resource_name: The unique name of the resulting resource.
-        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] name: The name of SSH key used for identification.
-        :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
-               leave it out, the ssh key will be created under the default project id of your organization.
-        :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
-               interpolation function.
-        :param pulumi.Input[str] type: The type of SSH key: `RSA` (default) or `DSA`.
-        :param pulumi.Input[str] uuid: The unique identifier of the key
-        """
-        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
-
-        __props__ = _SshKeyState.__new__(_SshKeyState)
-
-        __props__.__dict__["name"] = name
-        __props__.__dict__["project_id"] = project_id
-        __props__.__dict__["public_key"] = public_key
-        __props__.__dict__["type"] = type
-        __props__.__dict__["uuid"] = uuid
-        return SshKey(resource_name, opts=opts, __props__=__props__)
-
     @property
-    @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="authToken")
+    def auth_token(self) -> pulumi.Output[Optional[str]]:
         """
-        The name of SSH key used for identification.
+        The Equinix Metal API auth key for API operations
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "auth_token")
 
     @property
-    @pulumi.getter(name="projectId")
-    def project_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="clientId")
+    def client_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Unique Identifier for the project resource where the SSH key is scoped to.If you
-        leave it out, the ssh key will be created under the default project id of your organization.
+        API Consumer Key available under My Apps section in developer portal
         """
-        return pulumi.get(self, "project_id")
+        return pulumi.get(self, "client_id")
 
     @property
-    @pulumi.getter(name="publicKey")
-    def public_key(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="clientSecret")
+    def client_secret(self) -> pulumi.Output[Optional[str]]:
         """
-        The SSH public key. If this is a file, it can be read using the file
-        interpolation function.
+        API Consumer secret available under My Apps section in developer portal
         """
-        return pulumi.get(self, "public_key")
+        return pulumi.get(self, "client_secret")
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Output[Optional[str]]:
+    def endpoint(self) -> pulumi.Output[Optional[str]]:
         """
-        The type of SSH key: `RSA` (default) or `DSA`.
+        The Equinix API base URL to point out desired environment. Defaults to https://api.equinix.com
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
-    def uuid(self) -> pulumi.Output[str]:
+    def token(self) -> pulumi.Output[Optional[str]]:
         """
-        The unique identifier of the key
+        API token from the developer sandbox
         """
-        return pulumi.get(self, "uuid")
+        return pulumi.get(self, "token")
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix/networkedge/ssh_user.py` & `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix.egg-info/PKG-INFO` & `pulumi_equinix-0.9.0/pulumi_equinix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-equinix
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_equinix-0.8.0/pulumi_equinix.egg-info/SOURCES.txt` & `pulumi_equinix-0.9.0/pulumi_equinix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.8.0/setup.py` & `pulumi_equinix-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.8.0"
+VERSION = "0.9.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "equinix Pulumi Package - Development Version"
```

