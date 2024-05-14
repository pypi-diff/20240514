# Comparing `tmp/types-hvac-2.1.0.20240329.tar.gz` & `tmp/types-hvac-2.1.0.20240514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-hvac-2.1.0.20240329.tar", last modified: Fri Mar 29 02:13:41 2024, max compression
+gzip compressed data, was "types-hvac-2.1.0.20240514.tar", last modified: Tue May 14 02:20:24 2024, max compression
```

## Comparing `types-hvac-2.1.0.20240329.tar` & `types-hvac-2.1.0.20240514.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.196651 types-hvac-2.1.0.20240329/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-29 02:13:39.000000 types-hvac-2.1.0.20240329/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-29 02:13:39.000000 types-hvac-2.1.0.20240329/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-29 02:13:41.196651 types-hvac-2.1.0.20240329/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.188651 types-hvac-2.1.0.20240329/hvac-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-29 02:13:39.000000 types-hvac-2.1.0.20240329/hvac-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/adapters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.188651 types-hvac-2.1.0.20240329/hvac-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.192651 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/approle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/aws.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/azure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/cert.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/gcp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/github.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/jwt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/ldap.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/legacy_mfa.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/oidc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/okta.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/radius.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/userpass.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.192651 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/active_directory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/aws.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/azure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/consul.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/gcp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/identity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/kv.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/kv_v1.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/kv_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/pki.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/rabbitmq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/ssh.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/transit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.196651 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/audit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/capabilities.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/health.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/init.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/key.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/leader.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/lease.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/mount.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/policies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/policy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/quota.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/raft.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/seal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/system_backend_mixin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/wrapping.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/vault_api_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/api/vault_api_category.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.196651 types-hvac-2.1.0.20240329/hvac-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/approle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/aws.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/azure.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/gcp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/identity.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/constants/transit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:39.000000 types-hvac-2.1.0.20240329/hvac-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.196651 types-hvac-2.1.0.20240329/hvac-stubs/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-03-29 02:13:28.000000 types-hvac-2.1.0.20240329/hvac-stubs/v1/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 02:13:41.196651 types-hvac-2.1.0.20240329/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-03-29 02:13:39.000000 types-hvac-2.1.0.20240329/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:13:41.196651 types-hvac-2.1.0.20240329/types_hvac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-29 02:13:41.000000 types-hvac-2.1.0.20240329/types_hvac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-29 02:13:41.000000 types-hvac-2.1.0.20240329/types_hvac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:13:41.000000 types-hvac-2.1.0.20240329/types_hvac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 02:13:41.000000 types-hvac-2.1.0.20240329/types_hvac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 02:13:41.000000 types-hvac-2.1.0.20240329/types_hvac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.112275 types-hvac-2.1.0.20240514/hvac-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/hvac-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/adapters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.112275 types-hvac-2.1.0.20240514/hvac-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.116275 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/approle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/aws.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/azure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/cert.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/gcp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/github.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/jwt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/ldap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/legacy_mfa.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/oidc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/okta.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/radius.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/userpass.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.116275 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/active_directory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/aws.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/azure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/consul.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/gcp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/identity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv_v1.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/pki.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/rabbitmq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/ssh.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/audit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/capabilities.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/health.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/init.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/key.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/leader.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/lease.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/mount.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/policies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/policy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/quota.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/raft.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/seal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/system_backend_mixin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/wrapping.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/vault_api_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/api/vault_api_category.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/hvac-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/approle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/aws.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/azure.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/gcp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/identity.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/constants/transit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:23.000000 types-hvac-2.1.0.20240514/hvac-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/hvac-stubs/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-14 02:20:13.000000 types-hvac-2.1.0.20240514/hvac-stubs/v1/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-14 02:20:22.000000 types-hvac-2.1.0.20240514/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:20:24.120276 types-hvac-2.1.0.20240514/types_hvac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 02:20:24.000000 types-hvac-2.1.0.20240514/types_hvac.egg-info/top_level.txt
```

### Comparing `types-hvac-2.1.0.20240329/PKG-INFO` & `types-hvac-2.1.0.20240514/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hvac
-Version: 2.1.0.20240329
+Version: 2.1.0.20240514
 Summary: Typing stubs for hvac
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hvac.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-hvac` aims to provide accurate annotations
 for `hvac==2.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hvac. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `cc4b1cbbb3252c4063581132c49dedc4d62480f8` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `3195f9fb1b4275144177441815e8132d4a600c83` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/adapters.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/adapters.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def close(self) -> None: ...
     def get(self, url: str, **kwargs: Any) -> _R: ...
     def post(self, url: str, **kwargs: Any) -> _R: ...
     def put(self, url: str, **kwargs: Any) -> _R: ...
     def delete(self, url: str, **kwargs: Any) -> _R: ...
     def list(self, url: str, **kwargs: Any) -> _R: ...
     def head(self, url: str, **kwargs: Any) -> _R: ...
-    def login(self, url: str, use_token: bool = True, **kwargs: Any): ...
+    def login(self, url: str, use_token: bool = True, **kwargs: Any) -> Response: ...
     @abstractmethod
     def get_login_token(self, response: _R) -> str: ...
     @abstractmethod
     def request(
         self, method, url: str, headers: Mapping[str, str] | None = None, raise_exception: bool = True, **kwargs: Any
     ) -> _R: ...
```

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/__init__.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/approle.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/approle.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/aws.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/aws.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/azure.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/azure.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/cert.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/cert.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/gcp.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/gcp.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/github.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/github.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/jwt.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/jwt.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/kubernetes.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/kubernetes.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/ldap.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/ldap.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/legacy_mfa.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/legacy_mfa.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/oidc.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/oidc.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/okta.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/okta.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/radius.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/radius.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/token.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/token.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/auth_methods/userpass.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/auth_methods/userpass.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/__init__.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/active_directory.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/active_directory.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/aws.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/aws.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/azure.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/azure.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/consul.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/consul.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/database.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/database.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/gcp.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/gcp.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/identity.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/identity.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/kv_v2.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/kv_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/pki.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/pki.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/rabbitmq.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/rabbitmq.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/ssh.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/ssh.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/transform.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transform.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/secrets_engines/transit.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/secrets_engines/transit.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/__init__.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/audit.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/audit.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/auth.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/health.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/health.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/init.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/init.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/key.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/key.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/mount.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/mount.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/policies.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/policies.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/quota.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/quota.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/system_backend/raft.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/system_backend/raft.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/api/vault_api_category.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/api/vault_api_category.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/exceptions.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/hvac-stubs/utils.pyi` & `types-hvac-2.1.0.20240514/hvac-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-hvac-2.1.0.20240329/setup.py` & `types-hvac-2.1.0.20240514/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-hvac` aims to provide accurate annotations
 for `hvac==2.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hvac. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `cc4b1cbbb3252c4063581132c49dedc4d62480f8` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `3195f9fb1b4275144177441815e8132d4a600c83` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.0.20240329",
+      version="2.1.0.20240514",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hvac.md",
```

### Comparing `types-hvac-2.1.0.20240329/types_hvac.egg-info/PKG-INFO` & `types-hvac-2.1.0.20240514/types_hvac.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-hvac
-Version: 2.1.0.20240329
+Version: 2.1.0.20240514
 Summary: Typing stubs for hvac
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/hvac.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-hvac` aims to provide accurate annotations
 for `hvac==2.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/hvac. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `cc4b1cbbb3252c4063581132c49dedc4d62480f8` and was tested
-with mypy 1.9.0, pyright 1.1.356, and
-pytype 2024.3.19.
+This package was generated from typeshed commit `3195f9fb1b4275144177441815e8132d4a600c83` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

### Comparing `types-hvac-2.1.0.20240329/types_hvac.egg-info/SOURCES.txt` & `types-hvac-2.1.0.20240514/types_hvac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

