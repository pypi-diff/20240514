# Comparing `tmp/scanoss-1.8.0.tar.gz` & `tmp/scanoss-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanoss-1.8.0.tar", last modified: Tue Nov 14 11:19:21 2023, max compression
+gzip compressed data, was "scanoss-1.9.0.tar", last modified: Tue Jan  2 22:17:12 2024, max compression
```

## Comparing `scanoss-1.8.0.tar` & `scanoss-1.9.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.740121 scanoss-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-14 11:18:53.000000 scanoss-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2023-11-14 11:18:53.000000 scanoss-1.8.0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2023-11-14 11:19:21.740121 scanoss-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2023-11-14 11:18:53.000000 scanoss-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-14 11:18:53.000000 scanoss-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-11-14 11:19:21.740121 scanoss-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.728120 scanoss-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.728120 scanoss-1.8.0/src/protoc_gen_swagger/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/protoc_gen_swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.732120 scanoss-1.8.0/src/protoc_gen_swagger/options/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/protoc_gen_swagger/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/protoc_gen_swagger/options/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/protoc_gen_swagger/options/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/protoc_gen_swagger/options/openapiv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/protoc_gen_swagger/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.732120 scanoss-1.8.0/src/scanoss/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/common/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/common/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/common/v2/scanoss_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/components/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/components/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/components/v2/scanoss_components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.728120 scanoss-1.8.0/src/scanoss/api/cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/cryptography/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/dependencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/dependencies/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/dependencies/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/scanning/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/scanning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/scanning/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/scanning/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/semgrep/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/semgrep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/semgrep/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/semgrep/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.736121 scanoss-1.8.0/src/scanoss/api/vulnerabilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/vulnerabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.740121 scanoss-1.8.0/src/scanoss/api/vulnerabilities/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/vulnerabilities/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    41016 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/csvoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/cyclonedx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.740121 scanoss-1.8.0/src/scanoss/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-14 11:19:07.000000 scanoss-1.8.0/src/scanoss/data/build_date.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/data/spdx-exceptions.json
--rw-r--r--   0 runner    (1001) docker     (127)   228794 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/data/spdx-licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/filecount.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/scancodedeps.py
--rw-r--r--   0 runner    (1001) docker     (127)    42141 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/scanossapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/scanossbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    20426 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/scanossgrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/scantype.py
--rw-r--r--   0 runner    (1001) docker     (127)    15441 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/spdxlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/threadeddependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/threadedscanning.py
--rw-r--r--   0 runner    (1001) docker     (127)    15222 2023-11-14 11:18:53.000000 scanoss-1.8.0/src/scanoss/winnowing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 11:19:21.732120 scanoss-1.8.0/src/scanoss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2023-11-14 11:19:21.000000 scanoss-1.8.0/src/scanoss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2023-11-14 11:19:21.000000 scanoss-1.8.0/src/scanoss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 11:19:21.000000 scanoss-1.8.0/src/scanoss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-14 11:19:21.000000 scanoss-1.8.0/src/scanoss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-11-14 11:19:21.000000 scanoss-1.8.0/src/scanoss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-14 11:19:21.000000 scanoss-1.8.0/src/scanoss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-02 22:16:53.000000 scanoss-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-01-02 22:16:53.000000 scanoss-1.9.0/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-01-02 22:17:12.965267 scanoss-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-01-02 22:16:53.000000 scanoss-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-02 22:16:53.000000 scanoss-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-01-02 22:17:12.969267 scanoss-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.953267 scanoss-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.957267 scanoss-1.9.0/src/protoc_gen_swagger/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/protoc_gen_swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.957267 scanoss-1.9.0/src/protoc_gen_swagger/options/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/protoc_gen_swagger/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/protoc_gen_swagger/options/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/protoc_gen_swagger/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/api/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/api/common/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/common/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/common/v2/scanoss_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/api/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/api/components/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/components/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/components/v2/scanoss_components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.953267 scanoss-1.9.0/src/scanoss/api/cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/api/cryptography/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.961267 scanoss-1.9.0/src/scanoss/api/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/dependencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/api/dependencies/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/dependencies/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/api/scanning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/scanning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/api/scanning/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/scanning/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/api/semgrep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/semgrep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/api/semgrep/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/semgrep/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/api/vulnerabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/vulnerabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/api/vulnerabilities/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/vulnerabilities/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41523 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/csvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/cyclonedx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-02 22:17:03.000000 scanoss-1.9.0/src/scanoss/data/build_date.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/data/spdx-exceptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)   228794 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/data/spdx-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/filecount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/scancodedeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43763 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/scanossapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/scanossbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20426 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/scanossgrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15441 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/spdxlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/threadeddependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/threadedscanning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-01-02 22:16:53.000000 scanoss-1.9.0/src/scanoss/winnowing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 22:17:12.965267 scanoss-1.9.0/src/scanoss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-01-02 22:17:12.000000 scanoss-1.9.0/src/scanoss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-01-02 22:17:12.000000 scanoss-1.9.0/src/scanoss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 22:17:12.000000 scanoss-1.9.0/src/scanoss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-02 22:17:12.000000 scanoss-1.9.0/src/scanoss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-02 22:17:12.000000 scanoss-1.9.0/src/scanoss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-02 22:17:12.000000 scanoss-1.9.0/src/scanoss.egg-info/top_level.txt
```

### Comparing `scanoss-1.8.0/LICENSE` & `scanoss-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/PACKAGE.md` & `scanoss-1.9.0/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/PKG-INFO` & `scanoss-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.8.0
+Version: 1.9.0
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.8.0/README.md` & `scanoss-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/setup.cfg` & `scanoss-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/protoc_gen_swagger/__init__.py` & `scanoss-1.9.0/src/protoc_gen_swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/protoc_gen_swagger/options/__init__.py` & `scanoss-1.9.0/src/protoc_gen_swagger/options/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/protoc_gen_swagger/options/annotations_pb2.py` & `scanoss-1.9.0/src/protoc_gen_swagger/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/protoc_gen_swagger/options/openapiv2_pb2.py` & `scanoss-1.9.0/src/protoc_gen_swagger/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/__init__.py` & `scanoss-1.9.0/src/scanoss/api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,9 +17,7 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
-
-__version__ = '1.8.0'
```

### Comparing `scanoss-1.8.0/src/scanoss/api/__init__.py` & `scanoss-1.9.0/src/scanoss/api/common/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/common/__init__.py` & `scanoss-1.9.0/src/scanoss/api/common/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/common/v2/__init__.py` & `scanoss-1.9.0/src/scanoss/api/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/common/v2/scanoss_common_pb2.py` & `scanoss-1.9.0/src/scanoss/api/common/v2/scanoss_common_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/components/__init__.py` & `scanoss-1.9.0/src/scanoss/api/components/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/components/v2/__init__.py` & `scanoss-1.9.0/src/scanoss/api/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/components/v2/scanoss_components_pb2.py` & `scanoss-1.9.0/src/scanoss/api/components/v2/scanoss_components_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py` & `scanoss-1.9.0/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py` & `scanoss-1.9.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py` & `scanoss-1.9.0/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/dependencies/__init__.py` & `scanoss-1.9.0/src/scanoss/api/dependencies/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/dependencies/v2/__init__.py` & `scanoss-1.9.0/src/scanoss/api/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py` & `scanoss-1.9.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py` & `scanoss-1.9.0/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/scanning/__init__.py` & `scanoss-1.9.0/src/scanoss/api/scanning/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/scanning/v2/__init__.py` & `scanoss-1.9.0/src/scanoss/api/semgrep/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2021, SCANOSS
+   Copyright (c) 2023, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
```

### Comparing `scanoss-1.8.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py` & `scanoss-1.9.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py` & `scanoss-1.9.0/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/semgrep/__init__.py` & `scanoss-1.9.0/src/scanoss/api/semgrep/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/semgrep/v2/__init__.py` & `scanoss-1.9.0/src/scanoss/api/vulnerabilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2023, SCANOSS
+   Copyright (c) 2022, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
```

### Comparing `scanoss-1.8.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2.py` & `scanoss-1.9.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2_grpc.py` & `scanoss-1.9.0/src/scanoss/api/semgrep/v2/scanoss_semgrep_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/vulnerabilities/__init__.py` & `scanoss-1.9.0/src/scanoss/api/vulnerabilities/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/vulnerabilities/v2/__init__.py` & `scanoss-1.9.0/src/scanoss/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2022, SCANOSS
+   Copyright (c) 2021, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
@@ -17,7 +17,9 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
+
+__version__ = '1.9.0'
```

### Comparing `scanoss-1.8.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py` & `scanoss-1.9.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py` & `scanoss-1.9.0/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/cli.py` & `scanoss-1.9.0/src/scanoss/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,15 +402,15 @@
     :return: Octal code for encoded scanning options
     """
     scan_files = ScanType.SCAN_FILES.value
     scan_snippets = ScanType.SCAN_SNIPPETS.value
     scan_dependencies = 0
     if args.skip_snippets:
         scan_snippets = 0
-    if args.dependencies:
+    if args.dependencies or args.dep:
         scan_dependencies = ScanType.SCAN_DEPENDENCIES.value
     if args.dependencies_only:
         scan_files = scan_snippets = 0
         scan_dependencies = ScanType.SCAN_DEPENDENCIES.value
 
     scan_options = scan_files + scan_snippets + scan_dependencies
 
@@ -433,16 +433,16 @@
     Parameters
     ----------
         parser: ArgumentParser
             command line parser object
         args: Namespace
             Parsed arguments
     """
-    if not args.scan_dir and not args.wfp and not args.stdin:
-        print_stderr('Please specify a file/folder, fingerprint (--wfp) or STDIN (--stdin)')
+    if not args.scan_dir and not args.wfp and not args.stdin and not args.dep:
+        print_stderr('Please specify a file/folder, fingerprint (--wfp), dependency (--dep), or STDIN (--stdin)')
         parser.parse_args([args.subparser, '-h'])
         exit(1)
     if args.pac and args.proxy:
         print_stderr('Please specify one of --proxy or --pac, not both')
         parser.parse_args([args.subparser, '-h'])
         exit(1)
     scan_type: str = None
@@ -532,35 +532,41 @@
                       ignore_cert_errors=args.ignore_cert_errors, proxy=args.proxy, grpc_proxy=args.grpc_proxy,
                       pac=pac_file, ca_cert=args.ca_cert, retry=args.retry, hpsm=args.hpsm
                       )
     if args.wfp:
         if not scanner.is_file_or_snippet_scan():
             print_stderr(f'Error: Cannot specify WFP scanning if file/snippet options are disabled ({scan_options})')
             exit(1)
-        if args.threads > 1:
-            scanner.scan_wfp_file_threaded(args.wfp)
-        else:
-            scanner.scan_wfp_file(args.wfp)
+        if scanner.is_dependency_scan() and not args.dep:
+            print_stderr(f'Error: Cannot specify WFP & Dependency scanning without a dependency file ({--dep})')
+            exit(1)
+        scanner.scan_wfp_with_options(args.wfp, args.dep)
     elif args.stdin:
         contents = sys.stdin.buffer.read()
         if not scanner.scan_contents(args.stdin, contents):
             exit(1)
     elif args.scan_dir:
         if not os.path.exists(args.scan_dir):
             print_stderr(f'Error: File or folder specified does not exist: {args.scan_dir}.')
             exit(1)
         if os.path.isdir(args.scan_dir):
-            if not scanner.scan_folder_with_options(args.scan_dir, scanner.winnowing.file_map):
+            if not scanner.scan_folder_with_options(args.scan_dir, args.dep, scanner.winnowing.file_map):
                 exit(1)
         elif os.path.isfile(args.scan_dir):
-            if not scanner.scan_file_with_options(args.scan_dir, scanner.winnowing.file_map):
+            if not scanner.scan_file_with_options(args.scan_dir, args.dep, scanner.winnowing.file_map):
                 exit(1)
         else:
             print_stderr(f'Error: Path specified is neither a file or a folder: {args.scan_dir}.')
             exit(1)
+    elif args.dep:
+        if not args.dependencies_only:
+            print_stderr(f'Error: No file or folder specified to scan. Please add --dependencies-only to decorate dependency file only.')
+            exit(1)
+        if not scanner.scan_folder_with_options(".", args.dep, scanner.winnowing.file_map):
+            exit(1)
     else:
         print_stderr('No action found to process')
         exit(1)
 
 
 def dependency(parser, args):
     """
```

### Comparing `scanoss-1.8.0/src/scanoss/components.py` & `scanoss-1.9.0/src/scanoss/components.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/csvoutput.py` & `scanoss-1.9.0/src/scanoss/csvoutput.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/cyclonedx.py` & `scanoss-1.9.0/src/scanoss/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/data/spdx-exceptions.json` & `scanoss-1.9.0/src/scanoss/data/spdx-exceptions.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/data/spdx-licenses.json` & `scanoss-1.9.0/src/scanoss/data/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/filecount.py` & `scanoss-1.9.0/src/scanoss/filecount.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/scancodedeps.py` & `scanoss-1.9.0/src/scanoss/scancodedeps.py`

 * *Files 8% similar despite different names*

```diff
@@ -211,10 +211,30 @@
         except subprocess.TimeoutExpired as e:
             self.print_stderr(f'ERROR: Timed out attempting to run scancode dependency scan on {what_to_scan}: {e}')
             return False
         except Exception as e:
             self.print_stderr(f'ERROR: Issue running scancode dependency scan on {what_to_scan}: {e}')
             return False
         return True
+
+    def load_from_file(self, json_file: str = None) -> json:
+        """
+        Load the parsed JSON dependencies file and return the json object
+        :param json_file: dependency json file
+        :return: SCANOSS dependency JSON
+        """
+        if not json_file:
+            self.print_stderr('ERROR: No parsed JSON file provided to load.')
+            return None
+        if not os.path.isfile(json_file):
+            self.print_stderr(f'ERROR: parsed JSON file does not exist or is not a file: {json_file}')
+            return None
+        with open(json_file, 'r') as f:
+            try:
+                return json.loads(f.read())
+            except Exception as e:
+                self.print_stderr(f'ERROR: Problem loading input JSON: {e}')
+        return None
+
 #
 # End of ScancodeDeps Class
 #
```

### Comparing `scanoss-1.8.0/src/scanoss/scanner.py` & `scanoss-1.9.0/src/scanoss/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,33 +309,34 @@
         Check if dependency scanning is enabled
         :return: True if enabled, False otherwise
         """
         if self.scan_options & ScanType.SCAN_DEPENDENCIES.value:
             return True
         return False
 
-    def scan_folder_with_options(self, scan_dir: str, file_map: dict = None) -> bool:
+    def scan_folder_with_options(self, scan_dir: str, deps_file: str = None, file_map: dict = None) -> bool:
         """
         Scan the given folder for whatever scaning options that have been configured
         :param scan_dir: directory to scan
+        :param deps_file: pre-parsed dependency file to decorate
         :param file_map: mapping of obfuscated files back into originals
         :return: True if successful, False otherwise
         """
         success = True
         if not scan_dir:
             raise Exception(f"ERROR: Please specify a folder to scan")
         if not os.path.exists(scan_dir) or not os.path.isdir(scan_dir):
             raise Exception(f"ERROR: Specified folder does not exist or is not a folder: {scan_dir}")
         if not self.is_file_or_snippet_scan() and not self.is_dependency_scan():
             raise Exception(f"ERROR: No scan options defined to scan folder: {scan_dir}")
 
         if self.scan_output:
             self.print_msg(f'Writing results to {self.scan_output}...')
         if self.is_dependency_scan():
-            if not self.threaded_deps.run(what_to_scan=scan_dir, wait=False):  # Kick off a background dependency scan
+            if not self.threaded_deps.run(what_to_scan=scan_dir, deps_file=deps_file, wait=False):  # Kick off a background dependency scan
                 success = False
         if self.is_file_or_snippet_scan():
             if not self.scan_folder(scan_dir):
                 success = False
         if self.threaded_scan:
             if not self.__finish_scan_threaded(file_map):
                 success = False
@@ -538,33 +539,34 @@
             else:
                 success = csvo.produce_from_str(raw_output)
         else:
             self.print_stderr(f'ERROR: Unknown output format: {self.output_format}')
             success = False
         return success
 
-    def scan_file_with_options(self, file: str, file_map: dict = None) -> bool:
+    def scan_file_with_options(self, file: str, deps_file: str = None, file_map: dict = None) -> bool:
         """
         Scan the given file for whatever scaning options that have been configured
         :param file: file to scan
+        :param deps_file: pre-parsed dependency file to decorate
         :param file_map: mapping of obfuscated files back into originals
         :return: True if successful, False otherwise
         """
         success = True
         if not file:
             raise Exception(f"ERROR: Please specify a file to scan")
         if not os.path.exists(file) or not os.path.isfile(file):
             raise Exception(f"ERROR: Specified file does not exist or is not a file: {file}")
         if not self.is_file_or_snippet_scan() and not self.is_dependency_scan():
             raise Exception(f"ERROR: No scan options defined to scan file: {file}")
 
         if self.scan_output:
             self.print_msg(f'Writing results to {self.scan_output}...')
         if self.is_dependency_scan():
-            if not self.threaded_deps.run(what_to_scan=file, wait=False):  # Kick off a background dependency scan
+            if not self.threaded_deps.run(what_to_scan=file, deps_file=deps_file, wait=False):  # Kick off a background dependency scan
                 success = False
         if self.is_file_or_snippet_scan():
             if not self.scan_file(file):
                 success = False
         if self.threaded_scan:
             if not self.__finish_scan_threaded(file_map):
                 success = False
@@ -721,14 +723,43 @@
             csvo.produce_from_str(raw_output)
         else:
             self.print_stderr(f'ERROR: Unknown output format: {self.output_format}')
             success = False
 
         return success
 
+    def scan_wfp_with_options(self, wfp: str, deps_file: str, file_map: dict = None) -> bool:
+        """
+        Scan the given WFP file for whatever scaning options that have been configured
+        :param wfp: WFP file to scan
+        :param deps_file: pre-parsed dependency file to decorate
+        :param file_map: mapping of obfuscated files back into originals
+        :return: True if successful, False otherwise
+        """
+        success = True
+        wfp_file = wfp if wfp else self.wfp  # If a WFP file is specified, use it, otherwise us the default
+        if not os.path.exists(wfp_file) or not os.path.isfile(wfp_file):
+            raise Exception(f"ERROR: Specified WFP file does not exist or is not a file: {wfp_file}")
+
+        if not self.is_file_or_snippet_scan() and not self.is_dependency_scan():
+            raise Exception(f"ERROR: No scan options defined to scan folder: {scan_dir}")
+
+        if self.scan_output:
+            self.print_msg(f'Writing results to {self.scan_output}...')
+        if self.is_dependency_scan():
+            if not self.threaded_deps.run(deps_file=deps_file, wait=False):  # Kick off a background dependency scan
+                success = False
+        if self.is_file_or_snippet_scan():
+            if not self.scan_wfp_file_threaded(wfp_file, file_map):
+                success = False
+        if self.threaded_scan:
+            if not self.__finish_scan_threaded(file_map):
+                success = False
+        return success
+
     def scan_wfp_file_threaded(self, file: str = None, file_map: dict = None) -> bool:
         """
         Scan the contents of the specified WFP file (threaded)
         :param file: WFP file to scan (optional)
         :param file_map: mapping of obfuscated files back into originals (optional)
         return: True if successful, False otherwise
         """
@@ -774,16 +805,14 @@
             wfp += scan_block  # Store the WFP for the current file
         if wfp:
             self.threaded_scan.queue_add(wfp)
             queue_size += 1
 
         if not self.__run_scan_threaded(scan_started, file_count):
             success = False
-        elif not self.__finish_scan_threaded(file_map):
-            success = False
         return success
 
     def scan_wfp(self, wfp: str) -> bool:
         """
         Send the specified (single) WFP to ScanOSS for identification
         Parameters
         ----------
```

### Comparing `scanoss-1.8.0/src/scanoss/scanossapi.py` & `scanoss-1.9.0/src/scanoss/scanossapi.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/scanossbase.py` & `scanoss-1.9.0/src/scanoss/scanossbase.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/scanossgrpc.py` & `scanoss-1.9.0/src/scanoss/scanossgrpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/scantype.py` & `scanoss-1.9.0/src/scanoss/scantype.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/spdxlite.py` & `scanoss-1.9.0/src/scanoss/spdxlite.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/threadeddependencies.py` & `scanoss-1.9.0/src/scanoss/threadeddependencies.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from typing import Dict
 from dataclasses import dataclass
 
 from .scancodedeps import ScancodeDeps
 from .scanossbase import ScanossBase
 from .scanossgrpc import ScanossGrpc
 
+DEP_FILE_PREFIX = "file="  # Default prefix to signify an existing parsed dependency file
+
 
 @dataclass
 class ThreadedDependencies(ScanossBase):
     """
 
     """
     inputs: queue.Queue = queue.Queue()
@@ -60,53 +62,63 @@
         """
         responses = list(self.output.queue)
         if responses:
             for resp in responses:
                 return resp
         return None
 
-    def run(self, what_to_scan: str = None, wait: bool = True) -> bool:
+    def run(self, what_to_scan: str = None, deps_file: str = None, wait: bool = True) -> bool:
         """
         Initiate a background scan for the specified file/dir
         :param what_to_scan: file/folder to scan
+        :param deps_file: file to decorate instead of scan (overrides what_to_scan option)
         :param wait: wait for completion
         :return: True if successful, False if error encountered
         """
         what_to_scan = what_to_scan if what_to_scan else self.what_to_scan
         self._errors = False
         try:
-            self.print_msg(f'Searching {what_to_scan} for dependencies...')
-            self.inputs.put(what_to_scan)   # Set up an input queue to enable the parent to wait for completion
+            if deps_file:                                                  # Decorate the given dependencies file
+                self.print_msg(f'Decorating {deps_file} dependencies...')
+                self.inputs.put(f'{DEP_FILE_PREFIX}{deps_file}')           # Add to queue and have parent wait on it
+            else:                                                          # Search for dependencies to decorate
+                self.print_msg(f'Searching {what_to_scan} for dependencies...')
+                self.inputs.put(what_to_scan)                              # Add to queue and have parent wait on it
             self._thread = threading.Thread(target=self.scan_dependencies, daemon=True)
             self._thread.start()
         except Exception as e:
             self.print_stderr(f'ERROR: Problem running threaded dependencies: {e}')
             self._errors = True
         if wait and not self._errors:               # Wait for all inputs to complete
             self.complete()
         return False if self._errors else True
 
     def scan_dependencies(self) -> None:
         """
-        Scan for dependencies from the given file/dir (from the input queue)
+        Scan for dependencies from the given file/dir or from an input file (from the input queue).
         """
         current_thread = threading.get_ident()
         self.print_trace(f'Starting dependency worker {current_thread}...')
         try:
-            what_to_scan = self.inputs.get(timeout=5)                # Begin processing the dependency request
-            if not self.sc_deps.run_scan(what_to_scan=what_to_scan):
-                self._errors = True
-            else:
-                deps = self.sc_deps.produce_from_file()
+            what_to_scan = self.inputs.get(timeout=5)            # Begin processing the dependency request
+            deps = None
+            if what_to_scan.startswith(DEP_FILE_PREFIX):         # We have a pre-parsed dependency file, load it
+                deps = self.sc_deps.load_from_file(what_to_scan.strip(DEP_FILE_PREFIX))
+            else:                                                # Search the file/folder for dependency files to parse
+                if not self.sc_deps.run_scan(what_to_scan=what_to_scan):
+                    self._errors = True
+                else:
+                    deps = self.sc_deps.produce_from_file()
+            if not self._errors:
                 if deps is None:
                     self.print_stderr(f'Problem searching for dependencies for: {what_to_scan}')
                     self._errors = True
                 elif not deps:
                     self.print_trace(f'No dependencies found to decorate for: {what_to_scan}')
-                else:                         # TODO add API call to get dep data
+                else:
                     decorated_deps = self.grpc_api.get_dependencies(deps)
                     if decorated_deps:
                         self.output.put(decorated_deps)
                     else:
                         self._errors = True
         except Exception as e:
             self.print_stderr(f'ERROR: Problem encountered running dependency scan: {e}')
```

### Comparing `scanoss-1.8.0/src/scanoss/threadedscanning.py` & `scanoss-1.9.0/src/scanoss/threadedscanning.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss/winnowing.py` & `scanoss-1.9.0/src/scanoss/winnowing.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.8.0/src/scanoss.egg-info/PKG-INFO` & `scanoss-1.9.0/src/scanoss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.8.0
+Version: 1.9.0
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.8.0/src/scanoss.egg-info/SOURCES.txt` & `scanoss-1.9.0/src/scanoss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

