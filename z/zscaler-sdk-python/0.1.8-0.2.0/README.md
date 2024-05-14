# Comparing `tmp/zscaler_sdk_python-0.1.8.tar.gz` & `tmp/zscaler_sdk_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_sdk_python-0.1.8.tar", max compression
+gzip compressed data, was "zscaler_sdk_python-0.2.0.tar", max compression
```

## Comparing `zscaler_sdk_python-0.1.8.tar` & `zscaler_sdk_python-0.2.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1113 2024-05-09 20:16:57.159292 zscaler_sdk_python-0.1.8/LICENSE.md
--rw-r--r--   0        0        0    15746 2024-05-09 20:16:57.159292 zscaler_sdk_python-0.1.8/README.md
--rw-r--r--   0        0        0     2292 2024-05-09 20:17:49.675310 zscaler_sdk_python-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1277 2024-05-09 20:17:49.679310 zscaler_sdk_python-0.1.8/zscaler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/__init__.py
--rw-r--r--   0        0        0     3195 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/cache.py
--rw-r--r--   0        0        0     1479 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/no_op_cache.py
--rw-r--r--   0        0        0     4967 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/cache/zscaler_cache.py
--rw-r--r--   0        0        0      738 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/constants.py
--rw-r--r--   0        0        0        0 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/__init__.py
--rw-r--r--   0        0        0      172 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/error.py
--rw-r--r--   0        0        0      638 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/http_error.py
--rw-r--r--   0        0        0      628 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/errors/zscaler_api_error.py
--rw-r--r--   0        0        0       63 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/exceptions/__init__.py
--rw-r--r--   0        0        0     2025 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/exceptions/exceptions.py
--rw-r--r--   0        0        0     2099 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/logger.py
--rw-r--r--   0        0        0        0 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/ratelimiter/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0        0        0      639 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/user_agent.py
--rw-r--r--   0        0        0    19073 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/utils.py
--rw-r--r--   0        0        0    21568 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/__init__.py
--rw-r--r--   0        0        0     1534 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/activate.py
--rw-r--r--   0        0        0    14194 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0        0        0     2372 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/apptotal.py
--rw-r--r--   0        0        0     2992 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/audit_logs.py
--rw-r--r--   0        0        0     3140 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/authentication_settings.py
--rw-r--r--   0        0        0     2754 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/client.py
--rw-r--r--   0        0        0    18513 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/cloud_apps.py
--rw-r--r--   0        0        0     2872 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/device_management.py
--rw-r--r--   0        0        0    27473 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/dlp.py
--rw-r--r--   0        0        0      794 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/errors.py
--rw-r--r--   0        0        0    39908 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/firewall.py
--rw-r--r--   0        0        0    11686 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/forwarding_control.py
--rw-r--r--   0        0        0     2909 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/isolation_profile.py
--rw-r--r--   0        0        0     5835 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/labels.py
--rw-r--r--   0        0        0    30762 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/locations.py
--rw-r--r--   0        0        0     6724 2024-05-09 20:16:57.179292 zscaler_sdk_python-0.1.8/zscaler/zia/sandbox.py
--rw-r--r--   0        0        0     6792 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/security.py
--rw-r--r--   0        0        0     5298 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/ssl_inspection.py
--rw-r--r--   0        0        0    30729 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/traffic.py
--rw-r--r--   0        0        0    14484 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/url_categories.py
--rw-r--r--   0        0        0    14319 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/url_filtering.py
--rw-r--r--   0        0        0    13735 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/users.py
--rw-r--r--   0        0        0    12376 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/web_dlp.py
--rw-r--r--   0        0        0     1897 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/workload_groups.py
--rw-r--r--   0        0        0     6842 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zia/zpa_gateway.py
--rw-r--r--   0        0        0     2709 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/README.md
--rw-r--r--   0        0        0    24470 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/__init__.py
--rw-r--r--   0        0        0    13187 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments.py
--rw-r--r--   0        0        0    12445 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0        0        0    12019 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0        0        0     7942 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/certificates.py
--rw-r--r--   0        0        0     3844 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/client.py
--rw-r--r--   0        0        0     2667 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0        0        0    20849 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/connectors.py
--rw-r--r--   0        0        0     6189 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/emergency_access.py
--rw-r--r--   0        0        0      844 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/errors.py
--rw-r--r--   0        0        0     2764 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/idp.py
--rw-r--r--   0        0        0    34309 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/inspection.py
--rw-r--r--   0        0        0     3176 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/isolation_profile.py
--rw-r--r--   0        0        0    21697 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/lss.py
--rw-r--r--   0        0        0     2734 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/machine_groups.py
--rw-r--r--   0        0        0    31713 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/policies.py
--rw-r--r--   0        0        0     4317 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/posture_profiles.py
--rw-r--r--   0        0        0    31880 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0        0        0     9887 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/provisioning.py
--rw-r--r--   0        0        0     3632 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/saml_attributes.py
--rw-r--r--   0        0        0     4172 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/scim_attributes.py
--rw-r--r--   0        0        0     5041 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/scim_groups.py
--rw-r--r--   0        0        0     6103 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/segment_groups.py
--rw-r--r--   0        0        0     7776 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/server_groups.py
--rw-r--r--   0        0        0     6477 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/servers.py
--rw-r--r--   0        0        0    15428 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/service_edges.py
--rw-r--r--   0        0        0     4377 2024-05-09 20:16:57.183292 zscaler_sdk_python-0.1.8/zscaler/zpa/trusted_networks.py
--rw-r--r--   0        0        0    17518 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1113 2024-05-14 20:28:06.217430 zscaler_sdk_python-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0    15746 2024-05-14 20:28:06.217430 zscaler_sdk_python-0.2.0/README.md
+-rw-r--r--   0        0        0     2314 2024-05-14 20:28:50.857702 zscaler_sdk_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1277 2024-05-14 20:28:50.861702 zscaler_sdk_python-0.2.0/zscaler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/__init__.py
+-rw-r--r--   0        0        0     3195 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/cache.py
+-rw-r--r--   0        0        0     1479 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/no_op_cache.py
+-rw-r--r--   0        0        0     4967 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0        0        0      738 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/constants.py
+-rw-r--r--   0        0        0        0 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/error.py
+-rw-r--r--   0        0        0      638 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/http_error.py
+-rw-r--r--   0        0        0      628 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/zscaler_api_error.py
+-rw-r--r--   0        0        0       63 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/exceptions/__init__.py
+-rw-r--r--   0        0        0     2025 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/logger.py
+-rw-r--r--   0        0        0        0 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0        0        0      639 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/user_agent.py
+-rw-r--r--   0        0        0    19073 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/utils.py
+-rw-r--r--   0        0        0    21568 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/__init__.py
+-rw-r--r--   0        0        0     1534 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/activate.py
+-rw-r--r--   0        0        0    14194 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0        0        0     2372 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/apptotal.py
+-rw-r--r--   0        0        0     2992 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/audit_logs.py
+-rw-r--r--   0        0        0     3140 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/authentication_settings.py
+-rw-r--r--   0        0        0     2754 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/client.py
+-rw-r--r--   0        0        0    18513 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/cloud_apps.py
+-rw-r--r--   0        0        0     2872 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/device_management.py
+-rw-r--r--   0        0        0    27473 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/dlp.py
+-rw-r--r--   0        0        0      794 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/errors.py
+-rw-r--r--   0        0        0    39908 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/firewall.py
+-rw-r--r--   0        0        0    11686 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/forwarding_control.py
+-rw-r--r--   0        0        0     2909 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/isolation_profile.py
+-rw-r--r--   0        0        0     5835 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/labels.py
+-rw-r--r--   0        0        0    30762 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/locations.py
+-rw-r--r--   0        0        0     6724 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/sandbox.py
+-rw-r--r--   0        0        0     6792 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/security.py
+-rw-r--r--   0        0        0     5298 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0        0        0    30729 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/traffic.py
+-rw-r--r--   0        0        0    14484 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/url_categories.py
+-rw-r--r--   0        0        0    14319 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/url_filtering.py
+-rw-r--r--   0        0        0    13735 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/users.py
+-rw-r--r--   0        0        0    12376 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/web_dlp.py
+-rw-r--r--   0        0        0     1897 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/workload_groups.py
+-rw-r--r--   0        0        0     6842 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/zpa_gateway.py
+-rw-r--r--   0        0        0     2709 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/README.md
+-rw-r--r--   0        0        0    24498 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/__init__.py
+-rw-r--r--   0        0        0    13187 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments.py
+-rw-r--r--   0        0        0    12445 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0        0        0    12019 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0        0        0     8054 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/certificates.py
+-rw-r--r--   0        0        0     3844 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/client.py
+-rw-r--r--   0        0        0     2667 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0        0        0    20849 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/connectors.py
+-rw-r--r--   0        0        0     6189 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/emergency_access.py
+-rw-r--r--   0        0        0      844 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/errors.py
+-rw-r--r--   0        0        0     2764 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/idp.py
+-rw-r--r--   0        0        0    33962 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/inspection.py
+-rw-r--r--   0        0        0    27713 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/isolation.py
+-rw-r--r--   0        0        0    21546 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/lss.py
+-rw-r--r--   0        0        0     2734 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/machine_groups.py
+-rw-r--r--   0        0        0    31713 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/policies.py
+-rw-r--r--   0        0        0     5640 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0        0        0    31880 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0        0        0     9887 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/provisioning.py
+-rw-r--r--   0        0        0     3632 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0        0        0     4172 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0        0        0     3691 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/scim_groups.py
+-rw-r--r--   0        0        0     6103 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/segment_groups.py
+-rw-r--r--   0        0        0     7775 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/server_groups.py
+-rw-r--r--   0        0        0     6477 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/servers.py
+-rw-r--r--   0        0        0    15428 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/service_edges.py
+-rw-r--r--   0        0        0     3684 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/trusted_networks.py
+-rw-r--r--   0        0        0    17559 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.2.0/PKG-INFO
```

### Comparing `zscaler_sdk_python-0.1.8/LICENSE.md` & `zscaler_sdk_python-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/README.md` & `zscaler_sdk_python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/pyproject.toml` & `zscaler_sdk_python-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zscaler-sdk-python"
-version = "0.1.8"
+version = "0.2.0"
 description = "Official Python SDK for the Zscaler Products (Beta)"
 authors = ["Zscaler, Inc. <devrel@zscaler.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zscaler/zscaler-sdk-python"
 repository = "https://github.com/zscaler/zscaler-sdk-python"
 documentation = "https://zscaler-sdk-python.readthedocs.io"
@@ -46,14 +46,15 @@
 yarl = "*"
 pycryptodomex = "*"
 aenum = "*"
 pydash = "*"
 flake8 = "*"
 pytz = "*"
 black = "^24.4.1"
+cryptography = "^3.4"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-mock = "*"
 pytest-recording = "*"
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/__init__.py` & `zscaler_sdk_python-0.2.0/zscaler/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.8"
+__version__ = "0.2.0"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/cache/cache.py` & `zscaler_sdk_python-0.2.0/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/cache/no_op_cache.py` & `zscaler_sdk_python-0.2.0/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/cache/zscaler_cache.py` & `zscaler_sdk_python-0.2.0/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/constants.py` & `zscaler_sdk_python-0.2.0/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/errors/http_error.py` & `zscaler_sdk_python-0.2.0/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/errors/zscaler_api_error.py` & `zscaler_sdk_python-0.2.0/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/exceptions/exceptions.py` & `zscaler_sdk_python-0.2.0/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/logger.py` & `zscaler_sdk_python-0.2.0/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/ratelimiter/ratelimiter.py` & `zscaler_sdk_python-0.2.0/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/user_agent.py` & `zscaler_sdk_python-0.2.0/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/utils.py` & `zscaler_sdk_python-0.2.0/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/__init__.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/activate.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/admin_and_role_management.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/apptotal.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/audit_logs.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/authentication_settings.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/client.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/cloud_apps.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/device_management.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/dlp.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/errors.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/firewall.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/forwarding_control.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/isolation_profile.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/labels.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/locations.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/sandbox.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/security.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/ssl_inspection.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/traffic.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/url_categories.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/url_filtering.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/users.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/web_dlp.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/workload_groups.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zia/zpa_gateway.py` & `zscaler_sdk_python-0.2.0/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/README.md` & `zscaler_sdk_python-0.2.0/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/__init__.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from zscaler.zpa.certificates import CertificatesAPI
 from zscaler.zpa.client import ZPAClient
 from zscaler.zpa.cloud_connector_groups import CloudConnectorGroupsAPI
 from zscaler.zpa.connectors import AppConnectorControllerAPI
 from zscaler.zpa.emergency_access import EmergencyAccessAPI
 from zscaler.zpa.idp import IDPControllerAPI
 from zscaler.zpa.inspection import InspectionControllerAPI
-from zscaler.zpa.isolation_profile import IsolationProfileAPI
+from zscaler.zpa.isolation import IsolationAPI
 from zscaler.zpa.lss import LSSConfigControllerAPI
 from zscaler.zpa.machine_groups import MachineGroupsAPI
 from zscaler.zpa.policies import PolicySetsAPI
 from zscaler.zpa.posture_profiles import PostureProfilesAPI
 from zscaler.zpa.privileged_remote_access import PrivilegedRemoteAccessAPI
 from zscaler.zpa.provisioning import ProvisioningKeyAPI
 from zscaler.zpa.saml_attributes import SAMLAttributesAPI
@@ -183,14 +183,16 @@
             api = self.url
         elif api_version == "v2":
             api = self.v2_url
         elif api_version == "v2_lss":
             api = self.v2_lss_url
         elif api_version == "userconfig_v1":
             api = self.user_config_url
+        elif api_version == "cbiconfig_v1":
+            api = self.cbi_url
 
         url = f"{api}/{path.lstrip('/')}"
         start_time = time.time()
         # Update headers to include the user agent
         headers_with_user_agent = self.headers.copy()
         headers_with_user_agent["User-Agent"] = self.user_agent
         # Generate a unique UUID for this request
@@ -452,15 +454,15 @@
                 if not nextPage or (max_pages is not None and page >= max_pages):
                     break
 
                 page = nextPage if page is None else page + 1
                 params["page"] = page
 
         finally:
-            time.sleep(1)  # Ensure a delay between requests regardless of outcome
+            time.sleep(2)  # Ensure a delay between requests regardless of outcome
 
         if not ret_data:
             error_msg = ERROR_MESSAGES["EMPTY_RESULTS"]
             logger.warn(error_msg)
             return BoxList([]), error_msg
 
         return BoxList(ret_data), None
@@ -494,20 +496,20 @@
         """
         The interface object for the :ref:`ZPA Browser Access Certificates interface <zpa-certificates>`.
 
         """
         return CertificatesAPI(self)
 
     @property
-    def isolation_profile(self):
+    def isolation(self):
         """
-        The interface object for the :ref:`ZPA Isolation Profiles <zpa-isolation_profile>`.
+        The interface object for the :ref:`ZPA Isolation <zpa-isolation>`.
 
         """
-        return IsolationProfileAPI(self)
+        return IsolationAPI(self)
 
     @property
     def cloud_connector_groups(self):
         """
         The interface object for the :ref:`ZPA Cloud Connector Groups interface <zpa-cloud_connector_groups>`.
 
         """
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_inspection.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/app_segments_pra.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/certificates.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/certificates.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,17 @@
             :obj:`Box`:
                 The Browser Access certificate resource record.
 
         Examples:
             >>> ba_certificate = zpa.certificates.get_certificate('99999')
 
         """
-        return self.rest.get(f"certificate/{certificate_id}")
+        response = self.rest.delete("/certificate/%s" % (certificate_id))
+        return response.status_code
+        # return self.rest.get(f"certificate/{certificate_id}")
 
     def get_enrolment(self, certificate_id: str) -> Box:
         """
         Returns information on the specified enrollment certificate.
 
         Args:
             certificate_id (str): The unique id of the enrollment certificate.
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/client.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/cloud_connector_groups.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/connectors.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/emergency_access.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/errors.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/idp.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/inspection.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/inspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,84 +41,44 @@
                     "lhs": condition["lhs"],
                     "op": condition["op"],
                     "rhs": condition["rhs"],
                 }
             )
         return rule_set
 
-    def add_custom_control(
-        self,
-        name: str,
-        default_action: str,
-        severity: str,
-        type: str,
-        rules: list,
-        **kwargs,
-    ) -> Box:
+    def list_profiles(self, **kwargs) -> BoxList:
         """
-        Adds a new ZPA Inspection Custom Control.
+        Returns the list of ZPA Inspection Profiles.
 
         Args:
-            name (str): The name of the custom control.
-            default_action (str): The default action to take for matches against this custom control.
-            severity (str): The severity for events that match this custom control.
-            type (str): The type of HTTP message this control matches.
-            rules (list): A list of Inspection Control rule objects.
-            **kwargs: Optional keyword args.
+            **kwargs:
+                Optional keyword args.
 
         Keyword Args:
-            description (str): Additional information about the custom control.
-            paranoia_level (int): The paranoia level for the custom control.
+            **pagesize (int):
+                Specifies the page size. The default size is 20 and the maximum size is 500.
+            **search (str, optional):
+                The search string used to match against features and fields.
 
         Returns:
-            :obj:`Box`: The newly created custom Inspection Control resource record.
-
-        """
-
-        payload = {
-            "name": name,
-            "defaultAction": default_action,
-            "severity": severity,
-            "rules": [],
-            "type": type,
-        }
-
-        # Handle default_action_value
-        if "default_action_value" in kwargs:
-            payload["defaultActionValue"] = kwargs["default_action_value"]
-
-        # Use the _create_rule method to restructure the Inspection Control rule and add to the payload.
-        for rule in rules:
-            payload["rules"].append(self._create_rule(rule))
+            :obj:`BoxList`: The list of ZPA Inspection Profile resource records.
 
-        # Add optional parameters to payload
-        for key, value in kwargs.items():
-            if key == "paranoia_level":
-                payload["paranoiaLevel"] = int(value)
-            elif key == "description":
-                payload["description"] = value
-            # Add other optional parameters if necessary
+        Examples:
+            Iterate over all ZPA Inspection Profiles and print them:
 
-            # Convert snake to camelcase
-            payload = convert_keys(payload)
+            .. code-block:: python
 
-        response = self.rest.post("inspectionControls/custom", json=payload)
-        if isinstance(response, Response):
-            # this is only true when the creation failed (status code is not 2xx)
-            status_code = response.status_code
-            # Handle error response
-            raise Exception(f"API call failed with status {status_code}: {response.json()}")
-        return response
+                for profile in zpa.inspection.list_profiles():
+                    print(profile)
 
-        # response = self.rest.post("/inspectionControls/custom", json=payload)
-        # if isinstance(response, Response):
-        #     status_code = response.status_code
-        #     if status_code > 299:
-        #         return None
-        # return self.get_custom_control(response.get("id"))
+        """
+        list, _ = self.rest.get_paginated_data(
+            path="/inspectionProfile",
+        )
+        return list
 
     def add_profile(self, name: str, paranoia_level: int, predef_controls_version: str, **kwargs):
         """
         Adds a ZPA Inspection Profile.
 
         Args:
             name (str):
@@ -229,41 +189,115 @@
         if isinstance(response, Response):
             # this is only true when the creation failed (status code is not 2xx)
             status_code = response.status_code
             # Handle error response
             raise Exception(f"API call failed with status {status_code}: {response.json()}")
         return response
 
-        # response = self.rest.post("/inspectionProfile", json=payload)
-        # if isinstance(response, Response):
-        #     status_code = response.status_code
-        #     if status_code > 299:
-        #         return None
-        # return self.get_profile(response.get("id"))
-
-    def delete_custom_control(self, control_id: str) -> int:
+    def update_profile(self, profile_id: str, **kwargs):
         """
-        Deletes the specified custom ZPA Inspection Control.
+        Updates the specified ZPA Inspection Profile.
 
         Args:
-            control_id (str):
-                The unique id for the custom control that will be deleted.
+            profile_id (str):
+                The unique id for the ZPA Inspection Profile that will be updated.
+            predef_controls_version (str):
+                The predefined controls version for the ZPA Inspection Profile. Defaults to `OWASP_CRS/3.3.0`.
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            **custom_controls (list):
+                A tuple list of custom controls to be added to the Inspection profile.
+
+                Custom control tuples must follow the convention below:
+
+                ``(control_id, action)``
+
+                e.g.
+
+                .. code-block:: python
+
+                    custom_controls = [(99999, "BLOCK"), (88888, "PASS")]
+            **description (str):
+                Additional information about the Inspection Profile.
+            **name (str):
+                The name of the Inspection Profile.
+            **paranoia_level (int):
+                The paranoia level for the Inspection Profile.
+            **predef_controls (list):
+                A tuple list of predefined controls to be added to the Inspection profile.
+
+                Predefined control tuples must follow the convention below:
+
+                ``(control_id, action)``
+
+                e.g.
+
+                .. code-block:: python
+
+                    predef_controls = [(77777, "BLOCK"), (66666, "PASS")]
+            **predef_controls_version (str):
+                The version of the predefined controls that will be added.
 
         Returns:
-            :obj:`int`: The status code for the operation.
+            :obj:`Box`: The updated ZPA Inspection Profile resource record.
 
         Examples:
-            Delete a custom ZPA Inspection Control with an id of `99999`.
+            Update the name and description of a ZPA Inspection Profile with the id 99999:
 
             .. code-block:: python
 
-                zpa.inspection.delete_custom_control("99999")
+                print(
+                    zpa.inspection.update_profile(
+                        "99999",
+                        name="inspect_common_predef_controls",
+                        description="Inspects common controls from the Predefined set.",
+                    )
+                )
+
+            Add a custom control to the ZPA Inspection Profile with the id 88888:
+
+            .. code-block:: python
+
+                print(
+                    zpa.inspection.update_profile(
+                        "88888",
+                        custom_controls=[("2", "BLOCK")],
+                    )
+                )
 
         """
-        return self.rest.delete(f"inspectionControls/custom/{control_id}").status_code
+        # Set payload to value of existing record
+        payload = self.get_profile(profile_id)
+        payload["predefinedControlsVersion"] = kwargs.get("predef_controls_version", "OWASP_CRS/3.3.0")
+
+        # Extend existing list of default predefined controls if the user supplies more
+        if kwargs.get("predef_controls"):
+            controls = kwargs.pop("predef_controls")
+            for control in controls:
+                payload["predefined_controls"] = [{"id": control[0], "action": control[1]} for control in controls]
+
+        # Add custom controls if provided
+        if kwargs.get("custom_controls"):
+            controls = kwargs.pop("custom_controls")
+            payload["custom_controls"] = [{"id": control[0], "action": control[1]} for control in controls]
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            payload[key] = value
+
+        # Convert from snake case to camel case
+        payload = convert_keys(payload)
+
+        resp = self.rest.put(f"inspectionProfile/{profile_id}", json=payload).status_code
+
+        # Return the object if it was updated successfully
+        if not isinstance(resp, Response):
+            return self.get_profile(profile_id)
 
     def delete_profile(self, profile_id: str):
         """
         Deletes the specified Inspection Profile.
 
         Args:
             profile_id (str):
@@ -278,40 +312,14 @@
             .. code-block:: python
 
                 zpa.inspection.delete_profile("999999")
 
         """
         return self.rest.delete(f"inspectionProfile/{profile_id}").status_code
 
-    def get_custom_control(self, control_id: str) -> Box:
-        """
-        Returns the specified custom ZPA Inspection Control.
-
-        Args:
-            control_id (str):
-                The unique id of the custom ZPA Inspection Control to be returned.
-
-        Returns:
-            :obj:`Box`: The custom ZPA Inspection Control resource record.
-
-        Examples:
-            Print the Custom Inspection Control with an id of `99999`:
-
-            .. code-block:: python
-
-                print(zpa.inspection.get_custom_control("99999"))
-
-        """
-        response = self.rest.get("/inspectionControls/custom/%s" % (control_id))
-        if isinstance(response, Response):
-            status_code = response.status_code
-            if status_code != 200:
-                return None
-        return response
-
     def get_predef_control(self, control_id: str):
         """
         Returns the specified predefined ZPA Inspection Control.
 
         Args:
             control_id (str):
                 The unique id of the predefined ZPA Inspection Control to be returned.
@@ -356,121 +364,289 @@
         response = self.rest.get("/inspectionProfile/%s" % (profile_id))
         if isinstance(response, Response):
             status_code = response.status_code
             if status_code != 200:
                 return None
         return response
 
-    def list_control_action_types(self) -> Box:
+    def list_custom_controls(self, **kwargs) -> BoxList:
         """
-        Returns a list of ZPA Inspection Control Action Types.
+        Returns a list of all custom ZPA Inspection Controls.
+
+        Args:
+            **kwargs: Optional keyword arguments.
+
+        Keyword Args:
+            **search (str):
+                The string used to search for a custom control by features and fields.
+            **sortdir (str):
+                Specifies the sorting order for the search results.
+
+                Accepted values are:
+
+                - ``ASC`` - ascending order
+                - ``DESC`` - descending order
 
         Returns:
-            :obj:`BoxList`: A list containing the ZPA Inspection Control Action Types.
+            :obj:`BoxList`: A list containing all custom ZPA Inspection Controls.
 
         Examples:
-            Iterate over the ZPA Inspection Control Action Types and print each one:
+            Print a list of all custom ZPA Inspection Controls:
 
             .. code-block:: python
 
-                for action_type in zpa.inspection.list_control_action_types():
-                    print(action_type)
+                for control in zpa.inspection.list_custom_controls():
+                    print(control)
 
         """
-        return self.rest.get("inspectionControls/actionTypes")
+        list, _ = self.rest.get_paginated_data(
+            path="/inspectionControls/custom",
+        )
+        return list
 
-    def list_control_severity_types(self) -> BoxList:
+    def get_custom_control(self, control_id: str) -> Box:
         """
-        Returns a list of Inspection Control Severity Types.
+        Returns the specified custom ZPA Inspection Control.
+
+        Args:
+            control_id (str):
+                The unique id of the custom ZPA Inspection Control to be returned.
 
         Returns:
-            :obj:`BoxList`: A list containing all valid Inspection Control Severity Types.
+            :obj:`Box`: The custom ZPA Inspection Control resource record.
 
         Examples:
-            Print all Inspection Control Severity Types
+            Print the Custom Inspection Control with an id of `99999`:
 
             .. code-block:: python
 
-                for severity in zpa.inspection.list_control_severity_types():
-                    print(severity)
+                print(zpa.inspection.get_custom_control("99999"))
 
         """
-        return self.rest.get("inspectionControls/severityTypes")
+        response = self.rest.get("/inspectionControls/custom/%s" % (control_id))
+        if isinstance(response, Response):
+            status_code = response.status_code
+            if status_code != 200:
+                return None
+        return response
 
-    def list_control_types(self) -> BoxList:
+    def add_custom_control(
+        self,
+        name: str,
+        default_action: str,
+        severity: str,
+        type: str,
+        rules: list,
+        **kwargs,
+    ) -> Box:
         """
-        Returns a list of ZPA Inspection Control Types.
+        Adds a new ZPA Inspection Custom Control.
+
+        Args:
+            name (str): The name of the custom control.
+            default_action (str): The default action to take for matches against this custom control.
+            severity (str): The severity for events that match this custom control.
+            type (str): The type of HTTP message this control matches.
+            rules (list): A list of Inspection Control rule objects.
+            **kwargs: Optional keyword args.
+
+        Keyword Args:
+            description (str): Additional information about the custom control.
+            paranoia_level (int): The paranoia level for the custom control.
 
         Returns:
-            :obj:`BoxList`: A list containing ZPA Inspection Control Types.
+            :obj:`Box`: The newly created custom Inspection Control resource record.
 
         Examples:
-            Print all ZPA Inspection Control Types:
+            Create a new custom Inspection Control with the minimum required parameters
 
             .. code-block:: python
 
-                for control_type in zpa.inspection.list_control_types():
-                    print(control_type)
-
+                print(
+                    zpa.inspection.add_custom_control(
+                        "test8",
+                        severity="INFO",
+                        description="test descr",
+                        paranoia_level="3",
+                        type="REQUEST",
+                        default_action="BLOCK",
+                        rules=[
+                            {
+                                "names": ["test"],
+                                "type": "REQUEST_HEADERS",
+                                "conditions": [("SIZE", "GE", "10"), ("VALUE", "CONTAINS", "test")],
+                            }
+                        ],
+                    )
+                )
         """
-        return self.rest.get("inspectionControls/controlTypes")
 
-    def list_custom_control_types(self) -> BoxList:
+        payload = {
+            "name": name,
+            "defaultAction": default_action,
+            "severity": severity,
+            "rules": [],
+            "type": type,
+        }
+
+        # Handle default_action_value
+        if "default_action_value" in kwargs:
+            payload["defaultActionValue"] = kwargs["default_action_value"]
+
+        # Use the _create_rule method to restructure the Inspection Control rule and add to the payload.
+        for rule in rules:
+            payload["rules"].append(self._create_rule(rule))
+
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            if key == "paranoia_level":
+                payload["paranoiaLevel"] = int(value)
+            elif key == "description":
+                payload["description"] = value
+            # Add other optional parameters if necessary
+
+            # Convert snake to camelcase
+            payload = convert_keys(payload)
+
+        response = self.rest.post("inspectionControls/custom", json=payload)
+        if isinstance(response, Response):
+            # this is only true when the creation failed (status code is not 2xx)
+            status_code = response.status_code
+            # Handle error response
+            raise Exception(f"API call failed with status {status_code}: {response.json()}")
+        return response
+
+    def update_custom_control(self, control_id: str, **kwargs) -> Box:
         """
-        Returns a list of custom ZPA Inspection Control Types.
+        Updates the specified custom ZPA Inspection Control.
+
+        Args:
+            control_id (str):
+                The unique id for the custom control that will be updated.
+            **kwargs:
+                Optional keyword args.
+
+        Keyword Args:
+            **description (str):
+                Additional information about the custom control.
+            **default_action (str):
+                The default action to take for matches against this custom control. Valid options are:
+
+                - ``PASS``
+                - ``BLOCK``
+                - ``REDIRECT``
+            **name (str):
+                The name of the custom control.
+            **paranoia_level (int):
+                The paranoia level for the custom control.
+            **rules (list):
+                A list of Inspection Control rule objects, with each object using the format::
+
+                    {
+                        "names": ["name1", "name2"],
+                        "type": "rule_type",
+                        "conditions": [
+                            ("LHS", "OP", "RHS"),
+                            ("LHS", "OP", "RHS"),
+                        ],
+                    }
+            **severity (str):
+                The severity for events that match this custom control. Valid options are:
+
+                - ``CRITICAL``
+                - ``ERROR``
+                - ``WARNING``
+                - ``INFO``
+            **type (str):
+                The type of HTTP message this control matches. Valid options are:
+
+                - ``REQUEST``
+                - ``RESPONSE``
 
         Returns:
-            :obj:`BoxList`: A list containing custom ZPA Inspection Control Types.
+            :obj:`Box`: The updated custom ZPA Inspection Control resource record.
 
         Examples:
-
-            Print all custom ZPA Inspection Control Types
+            Update the description of a custom ZPA Inspection Control with an id of 99999:
 
             .. code-block:: python
 
-                for control_type in zpa.inspection.list_custom_control_types():
-                    print(control_type)
+                print(
+                    zpa.inspection.update_custom_control(
+                        "99999",
+                        description="Updated description",
+                    )
+                )
 
-        """
-        return self.rest.get("https://config.private.zscaler.com/mgmtconfig/v1/admin/inspectionControls/customControlTypes")
+            Update the rules of a custom ZPA Inspection Control with an id of 88888:
 
-    def list_custom_controls(self, **kwargs) -> BoxList:
+            .. code-block:: python
+
+                print(
+                    zpa.inspection.update_custom_control(
+                        "88888",
+                        rules=[
+                            {
+                                "names": ["xforwardedfor_ge_20"],
+                                "type": "REQUEST_HEADERS",
+                                "conditions": [
+                                    ("SIZE", "GE", "20"),
+                                    ("VALUE", "CONTAINS", "X-Forwarded-For"),
+                                ],
+                            }
+                        ],
+                    )
+                )
         """
-        Returns a list of all custom ZPA Inspection Controls.
+        # Set payload to value of existing record and recursively convert nested dict keys from snake_case
+        # to camelCase.
+        payload = convert_keys(self.get_custom_control(control_id))
 
-        Args:
-            **kwargs: Optional keyword arguments.
+        # If the user provides rules for an update, clear the current rules then use the create_rule method to
+        # restructure the Inspection Control rule and add to the payload.
+        if kwargs.get("rules"):
+            payload["rules"] = []
+            for rule in kwargs.pop("rules"):
+                payload["rules"].append(self._create_rule(rule))
 
-        Keyword Args:
-            **search (str):
-                The string used to search for a custom control by features and fields.
-            **sortdir (str):
-                Specifies the sorting order for the search results.
+        # Add optional parameters to payload
+        for key, value in kwargs.items():
+            payload_key = snake_to_camel(key)
+            payload[payload_key] = value
 
-                Accepted values are:
+            # Special handling for default_action_value
+            if key == "default_action_value":
+                payload["defaultActionValue"] = value
 
-                - ``ASC`` - ascending order
-                - ``DESC`` - descending order
+        resp = self.rest.put(f"inspectionControls/custom/{control_id}", json=payload).status_code
+
+        # Return the object if it was updated successfully
+        if not isinstance(resp, Response):
+            return self.get_custom_control(control_id)
+
+    def delete_custom_control(self, control_id: str) -> int:
+        """
+        Deletes the specified custom ZPA Inspection Control.
+
+        Args:
+            control_id (str):
+                The unique id for the custom control that will be deleted.
 
         Returns:
-            :obj:`BoxList`: A list containing all custom ZPA Inspection Controls.
+            :obj:`int`: The status code for the operation.
 
         Examples:
-            Print a list of all custom ZPA Inspection Controls:
+            Delete a custom ZPA Inspection Control with an id of `99999`.
 
             .. code-block:: python
 
-                for control in zpa.inspection.list_custom_controls():
-                    print(control)
+                zpa.inspection.delete_custom_control("99999")
 
         """
-        list, _ = self.rest.get_paginated_data(
-            path="/inspectionControls/custom",
-        )
-        return list
+        return self.rest.delete(f"inspectionControls/custom/{control_id}").status_code
 
     def list_custom_http_methods(self) -> BoxList:
         """
         Returns a list of custom ZPA Inspection Control HTTP Methods.
 
         Returns:
             :obj:`BoxList`: A list containing custom ZPA Inspection Control HTTP Methods.
@@ -618,45 +794,14 @@
         for control_group in all_control_groups:
             if control_group["control_group"] == group_name:
                 return control_group
 
         # If we reach here, the control group was not found
         raise ValueError(f"No predefined control group named '{group_name}' found")
 
-    def list_profiles(self, **kwargs) -> BoxList:
-        """
-        Returns the list of ZPA Inspection Profiles.
-
-        Args:
-            **kwargs:
-                Optional keyword args.
-
-        Keyword Args:
-            **pagesize (int):
-                Specifies the page size. The default size is 20 and the maximum size is 500.
-            **search (str, optional):
-                The search string used to match against features and fields.
-
-        Returns:
-            :obj:`BoxList`: The list of ZPA Inspection Profile resource records.
-
-        Examples:
-            Iterate over all ZPA Inspection Profiles and print them:
-
-            .. code-block:: python
-
-                for profile in zpa.inspection.list_profiles():
-                    print(profile)
-
-        """
-        list, _ = self.rest.get_paginated_data(
-            path="/inspectionProfile",
-        )
-        return list
-
     def profile_control_attach(self, profile_id: str, action: str, **kwargs) -> Box:
         """
         Attaches or detaches all predefined ZPA Inspection Controls to a ZPA Inspection Profile.
 
         Args:
             profile_id (str):
                 The unique id for the ZPA Inspection Profile that will be modified.
@@ -715,254 +860,95 @@
             return self.get_profile(profile_id) if resp.status_code == 204 else resp.status_code
         elif action == "detach":
             resp = self.rest.put(f"inspectionProfile/{profile_id}/deAssociateAllPredefinedControls")
             return self.get_profile(profile_id) if resp.status_code == 204 else resp.status_code
         else:
             raise ValueError("Unknown action provided. Valid actions are 'attach' or 'detach'.")
 
-    def update_custom_control(self, control_id: str, **kwargs) -> Box:
+    def update_profile_and_controls(self, profile_id: str, inspection_profile: dict, **kwargs):
         """
-        Updates the specified custom ZPA Inspection Control.
-
-        Args:
-            control_id (str):
-                The unique id for the custom control that will be updated.
-            **kwargs:
-                Optional keyword args.
-
-        Keyword Args:
-            **description (str):
-                Additional information about the custom control.
-            **default_action (str):
-                The default action to take for matches against this custom control. Valid options are:
-
-                - ``PASS``
-                - ``BLOCK``
-                - ``REDIRECT``
-            **name (str):
-                The name of the custom control.
-            **paranoia_level (int):
-                The paranoia level for the custom control.
-            **rules (list):
-                A list of Inspection Control rule objects, with each object using the format::
-
-                    {
-                        "names": ["name1", "name2"],
-                        "type": "rule_type",
-                        "conditions": [
-                            ("LHS", "OP", "RHS"),
-                            ("LHS", "OP", "RHS"),
-                        ],
-                    }
-            **severity (str):
-                The severity for events that match this custom control. Valid options are:
-
-                - ``CRITICAL``
-                - ``ERROR``
-                - ``WARNING``
-                - ``INFO``
-            **type (str):
-                The type of HTTP message this control matches. Valid options are:
-
-                - ``REQUEST``
-                - ``RESPONSE``
-
-        Returns:
-            :obj:`Box`: The updated custom ZPA Inspection Control resource record.
-
-        Examples:
-            Update the description of a custom ZPA Inspection Control with an id of 99999:
-
-            .. code-block:: python
-
-                print(
-                    zpa.inspection.update_custom_control(
-                        "99999",
-                        description="Updated description",
-                    )
-                )
-
-            Update the rules of a custom ZPA Inspection Control with an id of 88888:
+        Updates the inspection profile and controls for the specified ID.
 
-            .. code-block:: python
+        Note:
+            This method has not been fully implemented and will not be maintained. There seems to be functionality
+            duplication with the default Inspection Profile update API call. `**kwargs` has been provided as a parameter
+            for you to be able to add any additional args that Zscaler may add.
 
-                print(
-                    zpa.inspection.update_custom_control(
-                        "88888",
-                        rules=[
-                            {
-                                "names": ["xforwardedfor_ge_20"],
-                                "type": "REQUEST_HEADERS",
-                                "conditions": [
-                                    ("SIZE", "GE", "20"),
-                                    ("VALUE", "CONTAINS", "X-Forwarded-For"),
-                                ],
-                            }
-                        ],
-                    )
-                )
+            If you feel that this is in error and that this functionality should be correctly implemented by zscaler-sdk-python
+            `raise an issue <https://github.com/zscaler/zscaler-sdk-python/issues>` in the zscaler-sdk-python Github repo
 
+        Args:
+            profile_id (str):
+                The unique id of the inspection profile.
+            inspection_profile (dict):
+                The new inspection profile object.
+            **kwargs:
+                Additional keyword args.
 
         """
 
-        # Set payload to value of existing record and recursively convert nested dict keys from snake_case
-        # to camelCase.
-        payload = convert_keys(self.get_custom_control(control_id))
-
-        # If the user provides rules for an update, clear the current rules then use the create_rule method to
-        # restructure the Inspection Control rule and add to the payload.
-        if kwargs.get("rules"):
-            payload["rules"] = []
-            for rule in kwargs.pop("rules"):
-                payload["rules"].append(self._create_rule(rule))
-
-        # Add optional parameters to payload
-        for key, value in kwargs.items():
-            payload_key = snake_to_camel(key)
-            payload[payload_key] = value
+        payload = {
+            "inspection_profile_id": profile_id,
+            "inspection_profile": inspection_profile,
+        }
 
-            # Special handling for default_action_value
-            if key == "default_action_value":
-                payload["defaultActionValue"] = value
+        payload = convert_keys(payload)
 
-        resp = self.rest.put(f"inspectionControls/custom/{control_id}", json=payload).status_code
+        resp = self.rest.put("inspectionProfile/{profile_id}/patch", json=payload).status_code
 
         # Return the object if it was updated successfully
         if not isinstance(resp, Response):
-            return self.get_custom_control(control_id)
+            return self.get_profile(profile_id)
 
-    def update_profile(self, profile_id: str, **kwargs):
+    def list_control_action_types(self) -> Box:
         """
-        Updates the specified ZPA Inspection Profile.
-
-        Args:
-            profile_id (str):
-                The unique id for the ZPA Inspection Profile that will be updated.
-            predef_controls_version (str):
-                The predefined controls version for the ZPA Inspection Profile. Defaults to `OWASP_CRS/3.3.0`.
-            **kwargs:
-                Optional keyword args.
-
-        Keyword Args:
-            **custom_controls (list):
-                A tuple list of custom controls to be added to the Inspection profile.
-
-                Custom control tuples must follow the convention below:
-
-                ``(control_id, action)``
-
-                e.g.
-
-                .. code-block:: python
-
-                    custom_controls = [(99999, "BLOCK"), (88888, "PASS")]
-            **description (str):
-                Additional information about the Inspection Profile.
-            **name (str):
-                The name of the Inspection Profile.
-            **paranoia_level (int):
-                The paranoia level for the Inspection Profile.
-            **predef_controls (list):
-                A tuple list of predefined controls to be added to the Inspection profile.
-
-                Predefined control tuples must follow the convention below:
-
-                ``(control_id, action)``
-
-                e.g.
-
-                .. code-block:: python
-
-                    predef_controls = [(77777, "BLOCK"), (66666, "PASS")]
-            **predef_controls_version (str):
-                The version of the predefined controls that will be added.
+        Returns a list of ZPA Inspection Control Action Types.
 
         Returns:
-            :obj:`Box`: The updated ZPA Inspection Profile resource record.
+            :obj:`BoxList`: A list containing the ZPA Inspection Control Action Types.
 
         Examples:
-            Update the name and description of a ZPA Inspection Profile with the id 99999:
-
-            .. code-block:: python
-
-                print(
-                    zpa.inspection.update_profile(
-                        "99999",
-                        name="inspect_common_predef_controls",
-                        description="Inspects common controls from the Predefined set.",
-                    )
-                )
-
-            Add a custom control to the ZPA Inspection Profile with the id 88888:
+            Iterate over the ZPA Inspection Control Action Types and print each one:
 
             .. code-block:: python
 
-                print(
-                    zpa.inspection.update_profile(
-                        "88888",
-                        custom_controls=[("2", "BLOCK")],
-                    )
-                )
+                for action_type in zpa.inspection.list_control_action_types():
+                    print(action_type)
 
         """
-        # Set payload to value of existing record
-        payload = self.get_profile(profile_id)
-        payload["predefinedControlsVersion"] = kwargs.get("predef_controls_version", "OWASP_CRS/3.3.0")
-
-        # Extend existing list of default predefined controls if the user supplies more
-        if kwargs.get("predef_controls"):
-            controls = kwargs.pop("predef_controls")
-            for control in controls:
-                payload["predefined_controls"] = [{"id": control[0], "action": control[1]} for control in controls]
+        return self.rest.get("inspectionControls/actionTypes")
 
-        # Add custom controls if provided
-        if kwargs.get("custom_controls"):
-            controls = kwargs.pop("custom_controls")
-            payload["custom_controls"] = [{"id": control[0], "action": control[1]} for control in controls]
+    def list_control_severity_types(self) -> BoxList:
+        """
+        Returns a list of Inspection Control Severity Types.
 
-        # Add optional parameters to payload
-        for key, value in kwargs.items():
-            payload[key] = value
+        Returns:
+            :obj:`BoxList`: A list containing all valid Inspection Control Severity Types.
 
-        # Convert from snake case to camel case
-        payload = convert_keys(payload)
+        Examples:
+            Print all Inspection Control Severity Types
 
-        resp = self.rest.put(f"inspectionProfile/{profile_id}", json=payload).status_code
+            .. code-block:: python
 
-        # Return the object if it was updated successfully
-        if not isinstance(resp, Response):
-            return self.get_profile(profile_id)
+                for severity in zpa.inspection.list_control_severity_types():
+                    print(severity)
 
-    def update_profile_and_controls(self, profile_id: str, inspection_profile: dict, **kwargs):
         """
-        Updates the inspection profile and controls for the specified ID.
-
-        Note:
-            This method has not been fully implemented and will not be maintained. There seems to be functionality
-            duplication with the default Inspection Profile update API call. `**kwargs` has been provided as a parameter
-            for you to be able to add any additional args that Zscaler may add.
-
-            If you feel that this is in error and that this functionality should be correctly implemented by zscaler-sdk-python
-            `raise an issue <https://github.com/zscaler/zscaler-sdk-python/issues>` in the zscaler-sdk-python Github repo
-
-        Args:
-            profile_id (str):
-                The unique id of the inspection profile.
-            inspection_profile (dict):
-                The new inspection profile object.
-            **kwargs:
-                Additional keyword args.
+        return self.rest.get("inspectionControls/severityTypes")
 
+    def list_control_types(self) -> BoxList:
         """
+        Returns a list of ZPA Inspection Control Types.
 
-        payload = {
-            "inspection_profile_id": profile_id,
-            "inspection_profile": inspection_profile,
-        }
+        Returns:
+            :obj:`BoxList`: A list containing ZPA Inspection Control Types.
 
-        payload = convert_keys(payload)
+        Examples:
+            Print all ZPA Inspection Control Types:
 
-        resp = self.rest.put("inspectionProfile/{profile_id}/patch", json=payload).status_code
+            .. code-block:: python
 
-        # Return the object if it was updated successfully
-        if not isinstance(resp, Response):
-            return self.get_profile(profile_id)
+                for control_type in zpa.inspection.list_control_types():
+                    print(control_type)
+
+        """
+        return self.rest.get("inspectionControls/controlTypes")
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/lss.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/lss.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,28 +44,28 @@
         """
         Creates a dict template for feeding conditions into the ZPA Policies API when adding or updating a policy.
 
         Args:
             conditions (list): List of condition tuples.
 
         Returns:
-            :obj:`dict`: Dictionary containing the LSS Log Receiver Policy conditions template.
+            :obj:`list`: List containing the LSS Log Receiver Policy conditions template.
 
         """
 
         template = []
 
         for condition in conditions:
-            # Template for SAML Policy Rule objects
-            if isinstance(condition, tuple) and len(condition) == 2 and condition[0] == "saml":
-                operand = {"operands": [{"objectType": "SAML", "entryValues": []}]}
-                for item in condition[1]:
+            # Template for SAML, SCIM, and SCIM_GROUP Policy Rule objects
+            if condition[0] in ["saml", "scim", "scim_group"]:
+                operand = {"operands": [{"objectType": condition[0].upper(), "entryValues": []}]}
+                for entry in condition[1]:
                     entry_values = {
-                        "lhs": item[0],
-                        "rhs": item[1],
+                        "lhs": entry[0],
+                        "rhs": entry[1],
                     }
                     operand["operands"][0]["entryValues"].append(entry_values)
             # Template for client_type Policy Rule objects
             elif condition[0] == "client_type":
                 operand = {
                     "operands": [
                         {
@@ -145,37 +145,32 @@
 
             >>> for lss_config in zpa.lss.list_configs():
             ...    print(config)
         """
         list, _ = self.rest.get_paginated_data(path="/lssConfig", **kwargs, api_version="v2")
         return list
 
-    def get_config(self, lss_id: str) -> Box:
+    def get_config(self, lss_config_id: str) -> Box:
         """
         Returns information on the specified LSS Receiver config.
 
         Args:
-            lss_id (str):
+            lss_config_id (str):
                 The unique identifier for the LSS Receiver config.
 
         Returns:
-            :obj:`Box`: The resource record for the LSS Receiver config.
+            :obj:`Box`: The resource record for the LSS Receiver config in a Box object for easy attribute access.
 
         Examples:
             Print information on the specified LSS Receiver config.
 
             >>> print(zpa.lss.get_config('99999'))
-
         """
-        response = self.rest.send("GET", "/lssConfig/%s" % (lss_id), api_version="v2")
-        if isinstance(response, Response):
-            status_code = response.status_code
-            if status_code != 200:
-                return None
-        return response
+        # Perform the GET request
+        return self.rest.get(f"lssConfig/{lss_config_id}", api_version="v2")
 
     def get_log_formats(self, log_type=None) -> Box:
         """
         Returns all available pre-configured LSS Log Formats or a specific log format if specified.
 
         LSS Log Formats are provided as either CSV, JSON, or TSV. The values can be used when
         creating or updating LSS Log Receiver configs.
@@ -204,18 +199,15 @@
                 # Return all formats
                 return Box(formats)
         else:
             response.raise_for_status()
 
     def get_status_codes(self, log_type: str = "all") -> Box:
         """
-        Returns a list of LSS Session Status Codes.
-
-        The LSS Session Status codes are used to filter the messages received by LSS. LSS Session Status Codes can be
-        used when adding or updating the filters for an LSS Log Receiver.
+        Returns a list of LSS Session Status Codes filtered by log type.
 
         Args:
             log_type (str):
                 Filter the LSS Session Status Codes by Log Type, accepted values are:
 
                 - ``all``
                 - ``app_connector_status``
@@ -236,35 +228,31 @@
 
             Print LSS Session Status Codes for `User Activity` log types.
 
             >>> for item in zpa.lss.get_status_codes(log_type="user_activity"):
             ...    print(item)
 
         """
-        path = "/statusCodes"
-        if log_type != "all":
-            if log_type in [
-                "user_activity",
-                "user_status",
-                "private_svc_edge_status",
-                "app_connector_status",
-            ]:
-                path = f"{path}/{self.source_log_map[log_type]}"
-            else:
-                raise ValueError("Incorrect log_type provided.")
-
-        full_url = f"{self.v2_admin_url}{path}"
+        full_url = f"{self.v2_admin_url}/statusCodes"
         response = requests.get(full_url, headers=self.rest.headers)
+        response.raise_for_status()
+        all_status_codes = response.json()
 
-        if response.status_code == 200:
-            # Assuming that the response is a JSON object that needs to be converted to a Box
-            response_data = Box(response.json())
-            return response_data if log_type == "all" else response_data[log_type]
+        if log_type == "all":
+            return Box(all_status_codes)
         else:
-            response.raise_for_status()
+            filtered_status_codes = {}
+            log_type_key = self.source_log_map.get(log_type)
+            if log_type_key:
+                for code, details in all_status_codes.items():
+                    if log_type_key in details.get("log_types", []):
+                        filtered_status_codes[code] = details
+                return Box(filtered_status_codes)
+            else:
+                raise ValueError("Incorrect log_type provided.")
 
     def add_lss_config(
         self,
         lss_host: str,
         lss_port: str,
         name: str,
         source_log_type: str,
@@ -481,15 +469,15 @@
             Update an LSS Log Receiver config to change from user activity to user status.
 
             Note that the ``policy_rules`` will need to be modified to be compatible with the chosen
             ``source_log_type``.
 
             .. code-block:: python
 
-                zpa.lss.update_config(
+                zpa.lss.update_lss_config(
                     name="user_status_to_siem",
                     policy_rules=[
                         ("idp", ["idp_id"]),
                         ("client_type", ["machine_tunnel"]),
                         ("saml", [("attribute_id", "11111")]),
                     ],
                     source_log_type="user_status")
@@ -514,41 +502,43 @@
                 payload["config"]["filter"] = kwargs.pop(k)
 
         # Convert tuple list to dict and add to payload
         if kwargs.get("policy_rules"):
             if keys_exists(payload, "policyRuleResource", "name"):
                 policy_name = payload["policyRuleResource"]["name"]
             else:
-                policy_name = "SIEM_POLICY"
+                policy_name = "placeholder"
             payload["policyRuleResource"] = {
                 "conditions": self._create_policy(kwargs.pop("policy_rules")),
                 "name": kwargs.pop("policy_name", policy_name),
             }
 
         # Add additional provided parameters to payload
         for key, value in kwargs.items():
             payload[snake_to_camel(key)] = value
 
-        resp = self.rest.put(f"/lssConfig/{lss_config_id}", api_version="v2", json=payload).status_code
-
-        # Return the object if it was updated successfully
-        if not isinstance(resp, Response):
+        # Send the update request to the API
+        resp = self.rest.put(f"/lssConfig/{lss_config_id}", api_version="v2", json=payload)
+        if resp.status_code == 204:
+            # Fetch and return the updated configuration as no content is returned with a 204 response
             return self.get_config(lss_config_id)
+        else:
+            raise Exception("Failed to update LSS Config, status code: {}".format(resp.status_code))
 
-    def delete_lss_config(self, lss_id: str) -> int:
+    def delete_lss_config(self, lss_config_id: str) -> int:
         """
         Delete the specified LSS Receiver Config.
 
         Args:
-            lss_id (str): The unique identifier for the LSS Receiver Config to be deleted.
+            lss_config_id (str): The unique identifier for the LSS Receiver Config to be deleted.
 
         Returns:
             :obj:`int`:
                 The response code for the operation.
 
         Examples:
             Delete an LSS Receiver config.
 
-            >>> zpa.lss.delete_config('99999')
+            >>> zpa.lss.delete_lss_config('99999')
 
         """
-        return self.rest.delete(f"/lssConfig/{lss_id}", api_version="v2").status_code
+        return self.rest.delete(f"/lssConfig/{lss_config_id}", api_version="v2").status_code
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/machine_groups.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/policies.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/policies.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/posture_profiles.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/posture_profiles.py`

 * *Files 19% similar despite different names*

```diff
@@ -48,14 +48,33 @@
             >>> for posture_profile in zpa.posture_profiles.list_profiles():
             ...    pprint(posture_profile)
         """
         list, _ = self.rest.get_paginated_data(path="/posture", **kwargs, api_version="v2")
         return list
 
     def get_profile_by_name(self, name):
+        """
+        Searches for and returns a posture profile based on its name.
+
+        This method performs a case-sensitive search through all posture profiles,
+        returning the first profile that matches the specified name exactly.
+
+        Args:
+            name (str): The name of the posture profile to search for.
+
+        Returns:
+            Box: The posture profile that matches the given name, or None if no match is found.
+
+        Examples:
+            >>> profile = zpa.posture_profiles.get_profile_by_name("Example Profile Name")
+            >>> if profile:
+            ...     print("Profile ID:", profile.id)
+            ... else:
+            ...     print("Profile not found.")
+        """
         profiles = self.list_profiles()
         for profile in profiles:
             if profile.get("name") == name:
                 return profile
         return None
 
     def get_profile(self, profile_id: str) -> Box:
@@ -80,22 +99,34 @@
                 return None
         return response
 
     def get_udid_by_profile_name(self, search_name: str, **kwargs) -> str:
         """
         Searches for a posture profile by name and returns its posture_udid.
 
+        This function searches through all configured posture profiles, comparing the
+        provided search_name against each profile's name, both exactly and with any cloud suffix removed.
+        It returns the 'posture_udid' of the first matching profile found.
+
         Args:
             search_name (str): The name of the posture profile to search for.
 
         Keyword Args:
-            **kwargs: Additional keyword arguments to pass to the list_profiles method.
+            **kwargs: Additional keyword arguments to pass to the list_profiles method, such as
+                    'max_items', 'max_pages', 'pagesize', and 'search'.
 
         Returns:
             str: The posture_udid of the found posture profile, or None if not found.
+
+        Examples:
+            >>> udid = zpa.posture_profiles.get_udid_by_profile_name("Example Profile")
+            >>> if udid:
+            ...     print(f"Found Profile UDID: {udid}")
+            ... else:
+            ...     print("Profile not found.")
         """
         profiles = self.list_profiles(**kwargs)
         for profile in profiles:
             clean_profile_name = remove_cloud_suffix(profile.get("name"))
             if clean_profile_name == search_name or profile.get("name") == search_name:
                 return profile.get("posture_udid")
         return None
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/privileged_remote_access.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/privileged_remote_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/provisioning.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/saml_attributes.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/scim_attributes.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/scim_groups.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/scim_groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 
 from box import Box, BoxList
-
+import time
 from zscaler.zpa.client import ZPAClient
 
 
 class SCIMGroupsAPI:
     def __init__(self, client: ZPAClient):
         self.rest = client
 
@@ -90,44 +90,7 @@
 
         Examples:
             >>> pprint(zpa.scim_groups.get_group('99999'))
 
         """
         response = self.rest.get(f"/scimgroup/{group_id}", **kwargs, api_version="userconfig_v1")
         return response
-
-    def search_group(self, idp_id: str, group_name: str, **kwargs) -> dict:
-        """
-        Searches and returns the SCIM group with the specified name for the given IdP.
-        """
-        page_size = kwargs.get("pagesize", 500)  # Adjust the page size as needed
-
-        # Calculate the total pages using a synchronous call
-        total_pages = 1
-        page_number = 1
-
-        # Loop over each page to search for the group
-        while True:
-            page = self._get_page(idp_id, page_number, group_name, page_size)
-            total_pages = int(page.get("total_pages", "0"))
-            for group in page.get("list", []):
-                if group.get("name") == group_name:
-                    return group  # Return the found group immediately
-            if page_number >= total_pages:
-                break
-            page_number = page_number + 1
-        return None  # Return None if the group wasn't found
-
-    def _get_page(self, idp_id, page_number, search, page_size):
-        params = {
-            "page": page_number,
-            "search": search,
-            "pagesize": page_size,
-            "sortBy": "name",
-            "sortOrder": "DSC",
-        }
-        page = self.rest.get(
-            path=f"/scimgroup/idpId/{idp_id}",
-            params=params,
-            api_version="userconfig_v1",
-        )
-        return page
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/segment_groups.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/server_groups.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/server_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
         Returns:
             :obj:`Box`: The resource record for the server group.
 
         Examples:
             >>> pprint(zpa.server_groups.get_group('99999'))
 
         """
-
         return self.rest.get(f"serverGroup/{group_id}")
 
     def get_server_group_by_name(self, name):
         groups = self.list_groups()
         for group in groups:
             if group.get("name") == name:
                 return group
```

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/servers.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/zscaler/zpa/service_edges.py` & `zscaler_sdk_python-0.2.0/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.1.8/PKG-INFO` & `zscaler_sdk_python-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.1.8
+Version: 0.2.0
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://github.com/zscaler/zscaler-sdk-python
 License: MIT
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Requires-Python: >=3.8,<4.0
@@ -22,14 +22,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Requires-Dist: aenum ; extra == "dev"
 Requires-Dist: arrow
 Requires-Dist: black (>=24.4.1,<25.0.0) ; extra == "dev"
 Requires-Dist: certifi
 Requires-Dist: charset-normalizer
+Requires-Dist: cryptography (>=3.4,<4.0)
 Requires-Dist: flake8
 Requires-Dist: flatdict
 Requires-Dist: idna
 Requires-Dist: pycryptodomex
 Requires-Dist: pydash ; extra == "dev"
 Requires-Dist: python-box (>=7.1.1,<8.0.0)
 Requires-Dist: python-dateutil
```

