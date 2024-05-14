# Comparing `tmp/rcsb_db-1.720.tar.gz` & `tmp/rcsb_db-1.721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb_db-1.720.tar", last modified: Thu May  9 16:07:58 2024, max compression
+gzip compressed data, was "rcsb_db-1.721.tar", last modified: Tue May 14 12:25:56 2024, max compression
```

## Comparing `rcsb_db-1.720.tar` & `rcsb_db-1.721.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.036324 rcsb_db-1.720/
--rw-r--r--   0 vsts      (1001) docker     (127)    30733 2024-05-09 15:44:54.000000 rcsb_db-1.720/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-09 15:44:54.000000 rcsb_db-1.720/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-05-09 15:44:54.000000 rcsb_db-1.720/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    25557 2024-05-09 16:07:58.036324 rcsb_db-1.720/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    24011 2024-05-09 15:44:54.000000 rcsb_db-1.720/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.020324 rcsb_db-1.720/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.020324 rcsb_db-1.720/rcsb/db/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.024324 rcsb_db-1.720/rcsb/db/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cli/ETLExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cli/RepoHoldingsEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13632 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cli/RepoLoadExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cli/RepoScanExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cli/SchemaUpdateExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8990 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cli/SequenceClustersEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.024324 rcsb_db-1.720/rcsb/db/cockroach/
--rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cockroach/CockroachDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cockroach/CockroachDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cockroach/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/cockroach/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.024324 rcsb_db-1.720/rcsb/db/crate/
--rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/crate/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/crate/CrateDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/crate/CrateDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/crate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.028324 rcsb_db-1.720/rcsb/db/define/
--rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/define/ContentDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/define/DataTypeApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15542 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/define/DataTypeApplicationInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/define/DataTypeInstanceInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/define/SchemaDefAccess.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/define/SchemaDefBuild.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/define/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.028324 rcsb_db-1.720/rcsb/db/helpers/
--rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/helpers/ContentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/helpers/DocumentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/helpers/r.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.028324 rcsb_db-1.720/rcsb/db/mongo/
--rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mongo/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mongo/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15187 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mongo/DocumentLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mongo/MongoDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    60653 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mongo/PdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mongo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.032324 rcsb_db-1.720/rcsb/db/mysql/
--rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mysql/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mysql/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mysql/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mysql/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mysql/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19191 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mysql/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/mysql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.032324 rcsb_db-1.720/rcsb/db/processors/
--rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/ClusterDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/DataExchangeStatus.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/DataTransformFactory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/RepoHoldingsDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/SchemaDefDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/SchemaDefReShape.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/processors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.032324 rcsb_db-1.720/rcsb/db/sql/
--rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/sql/QueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/sql/SqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:54.000000 rcsb_db-1.720/rcsb/db/sql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.036324 rcsb_db-1.720/rcsb/db/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/CaseNormalizedDict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/ProvenanceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/SchemaProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/TextUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/makePathList.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/utils/unescape.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.036324 rcsb_db-1.720/rcsb/db/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)    22212 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/wf/RepoLoadWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 15:44:55.000000 rcsb_db-1.720/rcsb/db/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:07:58.036324 rcsb_db-1.720/rcsb.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    25557 2024-05-09 16:07:57.000000 rcsb_db-1.720/rcsb.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-05-09 16:07:57.000000 rcsb_db-1.720/rcsb.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 16:07:57.000000 rcsb_db-1.720/rcsb.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-05-09 16:07:57.000000 rcsb_db-1.720/rcsb.db.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 15:49:33.000000 rcsb_db-1.720/rcsb.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      437 2024-05-09 16:07:57.000000 rcsb_db-1.720/rcsb.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-09 16:07:57.000000 rcsb_db-1.720/rcsb.db.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-05-09 15:44:55.000000 rcsb_db-1.720/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-09 16:07:58.036324 rcsb_db-1.720/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-05-09 15:44:55.000000 rcsb_db-1.720/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.597037 rcsb_db-1.721/
+-rw-r--r--   0 vsts      (1001) docker     (127)    30774 2024-05-14 12:08:56.000000 rcsb_db-1.721/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-14 12:08:56.000000 rcsb_db-1.721/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-05-14 12:08:56.000000 rcsb_db-1.721/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    25559 2024-05-14 12:25:56.597037 rcsb_db-1.721/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    24011 2024-05-14 12:08:56.000000 rcsb_db-1.721/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.589037 rcsb_db-1.721/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.589037 rcsb_db-1.721/rcsb/db/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.589037 rcsb_db-1.721/rcsb/db/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9528 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cli/ETLExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cli/RepoHoldingsEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13632 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cli/RepoLoadExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10064 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cli/RepoScanExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cli/SchemaUpdateExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8990 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cli/SequenceClustersEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.589037 rcsb_db-1.721/rcsb/db/cockroach/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9848 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cockroach/CockroachDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9605 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cockroach/CockroachDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5467 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cockroach/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/cockroach/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.589037 rcsb_db-1.721/rcsb/db/crate/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5142 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/crate/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7987 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/crate/CrateDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9990 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/crate/CrateDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/crate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.593037 rcsb_db-1.721/rcsb/db/define/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33223 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/define/ContentDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4169 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/define/DataTypeApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15542 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/define/DataTypeApplicationInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4188 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/define/DataTypeInstanceInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34868 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/define/SchemaDefAccess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61072 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/define/SchemaDefBuild.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/define/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.593037 rcsb_db-1.721/rcsb/db/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16974 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/helpers/ContentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35901 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/helpers/DocumentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/helpers/r.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.593037 rcsb_db-1.721/rcsb/db/mongo/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5655 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mongo/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4938 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mongo/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15187 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mongo/DocumentLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23696 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mongo/MongoDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    60653 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mongo/PdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mongo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.593037 rcsb_db-1.721/rcsb/db/mysql/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2832 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mysql/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4258 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mysql/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18626 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mysql/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mysql/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5169 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mysql/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19191 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mysql/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/mysql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.593037 rcsb_db-1.721/rcsb/db/processors/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7467 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/ClusterDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5081 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/DataExchangeStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19485 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/DataTransformFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31322 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/RepoHoldingsDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40786 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/SchemaDefDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26654 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/SchemaDefReShape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/processors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.593037 rcsb_db-1.721/rcsb/db/sql/
+-rw-r--r--   0 vsts      (1001) docker     (127)    23627 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/sql/QueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    40731 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/sql/SqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:56.000000 rcsb_db-1.721/rcsb/db/sql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.597037 rcsb_db-1.721/rcsb/db/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/CaseNormalizedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12446 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3683 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/ProvenanceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22110 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/SchemaProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/TextUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2172 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/makePathList.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1055 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/utils/unescape.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.597037 rcsb_db-1.721/rcsb/db/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)    22212 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/wf/RepoLoadWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-14 12:08:57.000000 rcsb_db-1.721/rcsb/db/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 12:25:56.597037 rcsb_db-1.721/rcsb.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    25559 2024-05-14 12:25:56.000000 rcsb_db-1.721/rcsb.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2298 2024-05-14 12:25:56.000000 rcsb_db-1.721/rcsb.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 12:25:56.000000 rcsb_db-1.721/rcsb.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      209 2024-05-14 12:25:56.000000 rcsb_db-1.721/rcsb.db.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 12:12:43.000000 rcsb_db-1.721/rcsb.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      439 2024-05-14 12:25:56.000000 rcsb_db-1.721/rcsb.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-14 12:25:56.000000 rcsb_db-1.721/rcsb.db.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-05-14 12:08:57.000000 rcsb_db-1.721/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-14 12:25:56.597037 rcsb_db-1.721/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2876 2024-05-14 12:08:57.000000 rcsb_db-1.721/setup.py
```

### Comparing `rcsb_db-1.720/HISTORY.txt` & `rcsb_db-1.721/HISTORY.txt`

 * *Files 0% similar despite different names*

```diff
@@ -352,7 +352,8 @@
  15-Dec-2023  V1.715 Revert setting for mergeValidationReports
  19-Mar-2024  V1.716 Add quality check to PdbxLoader to ensure validation report data are loaded along with the primary data;
                      Begin updating PdbxLoader and RepoLoadEx to support weekly update workflow CLI requirements
  03-Apr-2024  V1.717 Add int_list cifType to DataTypeApplicationInfo
  09-Apr-2024  V1.718 Update RepoLoadExec CLI and RepoLoadWorkflow to support CLI usage from weekly-update workflow
   6-May-2024  V1.719 Updates to CLI utilities
   9-May-2024  V1.720 Adjust provider type exclusion input to accept a list of types; update setuptools config
+ 13-May-2024  V1.721 Update requirements
```

### Comparing `rcsb_db-1.720/LICENSE` & `rcsb_db-1.721/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/PKG-INFO` & `rcsb_db-1.721/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.720
+Version: 1.721
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,23 +21,23 @@
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: jsonschema>=2.6.0
 Requires-Dist: jsondiff>=1.2.0
 Requires-Dist: strict-rfc3339
 Requires-Dist: mysqlclient>=1.3.12
 Requires-Dist: pymongo==3.12.0
-Requires-Dist: mmcif>=0.75
-Requires-Dist: rcsb.utils.config>=0.36
-Requires-Dist: rcsb.utils.io>=1.31
-Requires-Dist: rcsb.utils.multiproc>=0.18
-Requires-Dist: rcsb.utils.chemref>=0.79
+Requires-Dist: mmcif>=0.88.0
+Requires-Dist: rcsb.utils.config>=0.40
+Requires-Dist: rcsb.utils.io>=1.46
+Requires-Dist: rcsb.utils.multiproc>=0.19
+Requires-Dist: rcsb.utils.chemref>=0.91
 Requires-Dist: scandir; python_version < "3.0"
 Requires-Dist: configparser; python_version < "3.0"
-Requires-Dist: rcsb.utils.dictionary>=1.23
-Requires-Dist: rcsb.utils.repository>=0.28
+Requires-Dist: rcsb.utils.dictionary>=1.24
+Requires-Dist: rcsb.utils.repository>=0.43
 Requires-Dist: SQLAlchemy==1.4.46; sys_platform == "linux"
 Requires-Dist: crate
 Requires-Dist: psycopg2-binary
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
```

### Comparing `rcsb_db-1.720/README.md` & `rcsb_db-1.721/README.md`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cli/ETLExec.py` & `rcsb_db-1.721/rcsb/db/cli/ETLExec.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cli/RepoHoldingsEtlWorker.py` & `rcsb_db-1.721/rcsb/db/cli/RepoHoldingsEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cli/RepoLoadExec.py` & `rcsb_db-1.721/rcsb/db/cli/RepoLoadExec.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cli/RepoScanExec.py` & `rcsb_db-1.721/rcsb/db/cli/RepoScanExec.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cli/SchemaUpdateExec.py` & `rcsb_db-1.721/rcsb/db/cli/SchemaUpdateExec.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cli/SequenceClustersEtlWorker.py` & `rcsb_db-1.721/rcsb/db/cli/SequenceClustersEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cockroach/CockroachDbLoader.py` & `rcsb_db-1.721/rcsb/db/cockroach/CockroachDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cockroach/CockroachDbUtil.py` & `rcsb_db-1.721/rcsb/db/cockroach/CockroachDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/cockroach/Connection.py` & `rcsb_db-1.721/rcsb/db/cockroach/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/crate/Connection.py` & `rcsb_db-1.721/rcsb/db/crate/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/crate/CrateDbLoader.py` & `rcsb_db-1.721/rcsb/db/crate/CrateDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/crate/CrateDbUtil.py` & `rcsb_db-1.721/rcsb/db/crate/CrateDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/define/ContentDefinition.py` & `rcsb_db-1.721/rcsb/db/define/ContentDefinition.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/define/DataTypeApiProvider.py` & `rcsb_db-1.721/rcsb/db/define/DataTypeApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/define/DataTypeApplicationInfo.py` & `rcsb_db-1.721/rcsb/db/define/DataTypeApplicationInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/define/DataTypeInstanceInfo.py` & `rcsb_db-1.721/rcsb/db/define/DataTypeInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/define/SchemaDefAccess.py` & `rcsb_db-1.721/rcsb/db/define/SchemaDefAccess.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/define/SchemaDefBuild.py` & `rcsb_db-1.721/rcsb/db/define/SchemaDefBuild.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/helpers/ContentDefinitionHelper.py` & `rcsb_db-1.721/rcsb/db/helpers/ContentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/helpers/DocumentDefinitionHelper.py` & `rcsb_db-1.721/rcsb/db/helpers/DocumentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/helpers/r.py` & `rcsb_db-1.721/rcsb/db/helpers/r.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mongo/Connection.py` & `rcsb_db-1.721/rcsb/db/mongo/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mongo/ConnectionBase.py` & `rcsb_db-1.721/rcsb/db/mongo/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mongo/DocumentLoader.py` & `rcsb_db-1.721/rcsb/db/mongo/DocumentLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mongo/MongoDbUtil.py` & `rcsb_db-1.721/rcsb/db/mongo/MongoDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mongo/PdbxLoader.py` & `rcsb_db-1.721/rcsb/db/mongo/PdbxLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mysql/Connection.py` & `rcsb_db-1.721/rcsb/db/mysql/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mysql/ConnectionBase.py` & `rcsb_db-1.721/rcsb/db/mysql/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mysql/MyDbAdapter.py` & `rcsb_db-1.721/rcsb/db/mysql/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mysql/MyDbUtil.py` & `rcsb_db-1.721/rcsb/db/mysql/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mysql/MysqlSchemaImporter.py` & `rcsb_db-1.721/rcsb/db/mysql/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/mysql/SchemaDefLoader.py` & `rcsb_db-1.721/rcsb/db/mysql/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/processors/ClusterDataPrep.py` & `rcsb_db-1.721/rcsb/db/processors/ClusterDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/processors/DataExchangeStatus.py` & `rcsb_db-1.721/rcsb/db/processors/DataExchangeStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/processors/DataTransformFactory.py` & `rcsb_db-1.721/rcsb/db/processors/DataTransformFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/processors/RepoHoldingsDataPrep.py` & `rcsb_db-1.721/rcsb/db/processors/RepoHoldingsDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py` & `rcsb_db-1.721/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/processors/SchemaDefDataPrep.py` & `rcsb_db-1.721/rcsb/db/processors/SchemaDefDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/processors/SchemaDefReShape.py` & `rcsb_db-1.721/rcsb/db/processors/SchemaDefReShape.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/sql/QueryDirectives.py` & `rcsb_db-1.721/rcsb/db/sql/QueryDirectives.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/sql/SqlGen.py` & `rcsb_db-1.721/rcsb/db/sql/SqlGen.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/CaseNormalizedDict.py` & `rcsb_db-1.721/rcsb/db/utils/CaseNormalizedDict.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/PdbxSchemaMapReader.py` & `rcsb_db-1.721/rcsb/db/utils/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/ProvenanceProvider.py` & `rcsb_db-1.721/rcsb/db/utils/ProvenanceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/SchemaProvider.py` & `rcsb_db-1.721/rcsb/db/utils/SchemaProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/TextUtil.py` & `rcsb_db-1.721/rcsb/db/utils/TextUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/TimeUtil.py` & `rcsb_db-1.721/rcsb/db/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/makePathList.py` & `rcsb_db-1.721/rcsb/db/utils/makePathList.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/utils/unescape.py` & `rcsb_db-1.721/rcsb/db/utils/unescape.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb/db/wf/RepoLoadWorkflow.py` & `rcsb_db-1.721/rcsb/db/wf/RepoLoadWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/rcsb.db.egg-info/PKG-INFO` & `rcsb_db-1.721/rcsb.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.720
+Version: 1.721
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -21,23 +21,23 @@
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: jsonschema>=2.6.0
 Requires-Dist: jsondiff>=1.2.0
 Requires-Dist: strict-rfc3339
 Requires-Dist: mysqlclient>=1.3.12
 Requires-Dist: pymongo==3.12.0
-Requires-Dist: mmcif>=0.75
-Requires-Dist: rcsb.utils.config>=0.36
-Requires-Dist: rcsb.utils.io>=1.31
-Requires-Dist: rcsb.utils.multiproc>=0.18
-Requires-Dist: rcsb.utils.chemref>=0.79
+Requires-Dist: mmcif>=0.88.0
+Requires-Dist: rcsb.utils.config>=0.40
+Requires-Dist: rcsb.utils.io>=1.46
+Requires-Dist: rcsb.utils.multiproc>=0.19
+Requires-Dist: rcsb.utils.chemref>=0.91
 Requires-Dist: scandir; python_version < "3.0"
 Requires-Dist: configparser; python_version < "3.0"
-Requires-Dist: rcsb.utils.dictionary>=1.23
-Requires-Dist: rcsb.utils.repository>=0.28
+Requires-Dist: rcsb.utils.dictionary>=1.24
+Requires-Dist: rcsb.utils.repository>=0.43
 Requires-Dist: SQLAlchemy==1.4.46; sys_platform == "linux"
 Requires-Dist: crate
 Requires-Dist: psycopg2-binary
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
```

### Comparing `rcsb_db-1.720/rcsb.db.egg-info/SOURCES.txt` & `rcsb_db-1.721/rcsb.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb_db-1.720/requirements.txt` & `rcsb_db-1.721/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 pytz
 jsonschema >= 2.6.0
 jsondiff >= 1.2.0
 strict-rfc3339
 mysqlclient >= 1.3.12
 pymongo==3.12.0
 # pymongo >= 3.7.0  # need to fix this later
-mmcif >= 0.75
-rcsb.utils.config >= 0.36
-rcsb.utils.io >= 1.31
-rcsb.utils.multiproc >= 0.18
-rcsb.utils.chemref >= 0.79
+mmcif >= 0.88.0
+rcsb.utils.config >= 0.40
+rcsb.utils.io >= 1.46
+rcsb.utils.multiproc >= 0.19
+rcsb.utils.chemref >= 0.91
 scandir; python_version < "3.0"
 configparser; python_version < "3.0"
-rcsb.utils.dictionary >= 1.23
-rcsb.utils.repository >= 0.28
+rcsb.utils.dictionary >= 1.24
+rcsb.utils.repository >= 0.43
 #
 SQLAlchemy == 1.4.46; sys_platform == 'linux'
 # For crate and cockroach -
 crate
 psycopg2-binary
```

### Comparing `rcsb_db-1.720/setup.py` & `rcsb_db-1.721/setup.py`

 * *Files identical despite different names*

