# Comparing `tmp/flowee-1.5.tar.gz` & `tmp/flowee-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowee-1.5.tar", last modified: Tue May 14 00:42:58 2024, max compression
+gzip compressed data, was "flowee-1.6.tar", last modified: Tue May 14 01:43:33 2024, max compression
```

## Comparing `flowee-1.5.tar` & `flowee-1.6.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/
--rw-r--r--   0 dario     (1000) dario     (1000)      129 2024-05-14 00:42:58.921293 flowee-1.5/PKG-INFO
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.911294 flowee-1.5/flowee/
--rw-r--r--   0 dario     (1000) dario     (1000)       29 2024-05-03 17:58:36.000000 flowee-1.5/flowee/__init__.py
--rw-r--r--   0 dario     (1000) dario     (1000)    10278 2024-05-09 17:30:50.000000 flowee-1.5/flowee/main.py
--rw-r--r--   0 dario     (1000) dario     (1000)     2163 2024-05-14 00:42:42.000000 flowee-1.5/flowee/utils.py
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.911294 flowee-1.5/flowee/web/
--rw-r--r--   0 dario     (1000) dario     (1000)        0 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/__init_.py
--rw-r--r--   0 dario     (1000) dario     (1000)      636 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/index.html
--rw-r--r--   0 dario     (1000) dario     (1000)      470 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/package.json
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.911294 flowee-1.5/flowee/web/public/
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/public/assets/
--rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Bucket.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/BucketPolicy.png
--rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/CacheCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Certificate.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Cluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/ConfigurationSet.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/DBCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/DBClusterNep.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Database.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Datastore.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Detector.png
--rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Distribution.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/EventBus.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Function.png
--rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Group.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/HostedZone.png
--rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Instance.png
--rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/InstanceConnect.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Key.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Keyspace.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Method.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Protection.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Queue.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/RestApi.png
--rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Secret.png
--rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/StateMachine.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Stream.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Table.png
--rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/TopicRule.png
--rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/Trail.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/UserPool.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/VPC.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/WebACL.png
--rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/assets/preact.svg
--rw-r--r--   0 dario     (1000) dario     (1000)     1497 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/public/vite.svg
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/@types/
--rw-r--r--   0 dario     (1000) dario     (1000)       62 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/@types/edges.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      809 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/@types/node.ts
--rw-r--r--   0 dario     (1000) dario     (1000)     2362 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/app.tsx
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/assets/
--rw-r--r--   0 dario     (1000) dario     (1000)    18801 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/App.png
--rw-r--r--   0 dario     (1000) dario     (1000)    21168 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)     5561 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19421 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11123 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    10559 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9220 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11223 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14674 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    17740 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20193 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9425 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22687 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    18512 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20178 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11295 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)      947 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Bucket.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/BucketPolicy.png
--rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/CacheCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Certificate.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Cluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/ConfigurationSet.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/DBCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/DBClusterNep.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Database.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Datastore.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Detector.png
--rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Distribution.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/EventBus.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Function.png
--rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Group.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/HostedZone.png
--rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Instance.png
--rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/InstanceConnect.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Key.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Keyspace.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Method.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Protection.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Queue.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/RestApi.png
--rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Secret.png
--rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/StateMachine.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Stream.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Table.png
--rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/TopicRule.png
--rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/Trail.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/UserPool.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/VPC.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/WebACL.png
--rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/assets/preact.svg
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.911294 flowee-1.5/flowee/web/src/components/
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/components/GroupNode/
--rw-r--r--   0 dario     (1000) dario     (1000)      540 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/components/GroupNode/index.tsx
--rw-r--r--   0 dario     (1000) dario     (1000)      502 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/components/GroupNode/styles.ts
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/components/ResourceNode/
--rw-r--r--   0 dario     (1000) dario     (1000)      499 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/components/ResourceNode/index.tsx
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/components/SubGroupNode/
--rw-r--r--   0 dario     (1000) dario     (1000)       80 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/components/SubGroupNode/index.tsx
--rw-r--r--   0 dario     (1000) dario     (1000)       34 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/constants.ts
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/generators/
--rw-r--r--   0 dario     (1000) dario     (1000)      488 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/generators/createGroup.ts
--rw-r--r--   0 dario     (1000) dario     (1000)     2371 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/generators/createGroupNodes.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      686 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/generators/createResource.ts
--rw-r--r--   0 dario     (1000) dario     (1000)     1081 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/generators/createResourceNodes.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      773 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/generators/createSubgroup.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      303 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/index.css
--rw-r--r--   0 dario     (1000) dario     (1000)      135 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/main.tsx
--rw-r--r--   0 dario     (1000) dario     (1000)   213276 2024-05-02 23:32:35.000000 flowee-1.5/flowee/web/src/schema.json
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.921293 flowee-1.5/flowee/web/src/utils/
--rw-r--r--   0 dario     (1000) dario     (1000)     1060 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/utils/index.ts
--rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/src/vite-env.d.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      763 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/tsconfig.json
--rw-r--r--   0 dario     (1000) dario     (1000)      233 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/tsconfig.node.json
--rw-r--r--   0 dario     (1000) dario     (1000)      164 2024-05-03 17:58:36.000000 flowee-1.5/flowee/web/vite.config.ts
--rw-r--r--   0 dario     (1000) dario     (1000)    51326 2024-05-09 11:16:39.000000 flowee-1.5/flowee/web/yarn.lock
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 00:42:58.911294 flowee-1.5/flowee.egg-info/
--rw-r--r--   0 dario     (1000) dario     (1000)      129 2024-05-14 00:42:58.000000 flowee-1.5/flowee.egg-info/PKG-INFO
--rw-r--r--   0 dario     (1000) dario     (1000)     4677 2024-05-14 00:42:58.000000 flowee-1.5/flowee.egg-info/SOURCES.txt
--rw-r--r--   0 dario     (1000) dario     (1000)        1 2024-05-14 00:42:58.000000 flowee-1.5/flowee.egg-info/dependency_links.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       44 2024-05-14 00:42:58.000000 flowee-1.5/flowee.egg-info/entry_points.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       17 2024-05-14 00:42:58.000000 flowee-1.5/flowee.egg-info/requires.txt
--rw-r--r--   0 dario     (1000) dario     (1000)        7 2024-05-14 00:42:58.000000 flowee-1.5/flowee.egg-info/top_level.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-14 00:42:58.921293 flowee-1.5/setup.cfg
--rw-r--r--   0 dario     (1000) dario     (1000)     1945 2024-05-14 00:42:49.000000 flowee-1.5/setup.py
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/
+-rw-r--r--   0 dario     (1000) dario     (1000)      129 2024-05-14 01:43:33.902655 flowee-1.6/PKG-INFO
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/
+-rw-r--r--   0 dario     (1000) dario     (1000)       29 2024-05-03 17:58:36.000000 flowee-1.6/flowee/__init__.py
+-rw-r--r--   0 dario     (1000) dario     (1000)    10278 2024-05-09 17:30:50.000000 flowee-1.6/flowee/main.py
+-rw-r--r--   0 dario     (1000) dario     (1000)     2140 2024-05-14 01:37:19.000000 flowee-1.6/flowee/utils.py
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/
+-rw-r--r--   0 dario     (1000) dario     (1000)        0 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/__init_.py
+-rw-r--r--   0 dario     (1000) dario     (1000)      636 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/index.html
+-rw-r--r--   0 dario     (1000) dario     (1000)      470 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/package.json
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/public/
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/public/assets/
+-rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Bucket.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/BucketPolicy.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/CacheCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Certificate.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Cluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/ConfigurationSet.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/DBCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/DBClusterNep.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Database.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Datastore.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Detector.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Distribution.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/EventBus.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Function.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Group.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/HostedZone.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Instance.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/InstanceConnect.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Key.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Keyspace.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Method.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Protection.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Queue.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/RestApi.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Secret.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/StateMachine.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Stream.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Table.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/TopicRule.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Trail.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/UserPool.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/VPC.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/WebACL.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/preact.svg
+-rw-r--r--   0 dario     (1000) dario     (1000)     1497 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/vite.svg
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/src/
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/src/@types/
+-rw-r--r--   0 dario     (1000) dario     (1000)       62 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/@types/edges.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      809 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/@types/node.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)     2362 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/app.tsx
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/assets/
+-rw-r--r--   0 dario     (1000) dario     (1000)    18801 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/App.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    21168 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     5561 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19421 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11123 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    10559 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9220 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11223 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14674 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    17740 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20193 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9425 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22687 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    18512 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20178 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11295 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)      947 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Bucket.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/BucketPolicy.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/CacheCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Certificate.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Cluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/ConfigurationSet.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/DBCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/DBClusterNep.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Database.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Datastore.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Detector.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Distribution.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/EventBus.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Function.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Group.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/HostedZone.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Instance.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/InstanceConnect.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Key.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Keyspace.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Method.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Protection.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Queue.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/RestApi.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Secret.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/StateMachine.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Stream.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Table.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/TopicRule.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Trail.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/UserPool.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/VPC.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/WebACL.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/preact.svg
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.882655 flowee-1.6/flowee/web/src/components/
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/components/GroupNode/
+-rw-r--r--   0 dario     (1000) dario     (1000)      540 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/GroupNode/index.tsx
+-rw-r--r--   0 dario     (1000) dario     (1000)      502 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/GroupNode/styles.ts
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/components/ResourceNode/
+-rw-r--r--   0 dario     (1000) dario     (1000)      499 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/ResourceNode/index.tsx
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/components/SubGroupNode/
+-rw-r--r--   0 dario     (1000) dario     (1000)       80 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/SubGroupNode/index.tsx
+-rw-r--r--   0 dario     (1000) dario     (1000)       34 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/constants.ts
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/generators/
+-rw-r--r--   0 dario     (1000) dario     (1000)      488 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createGroup.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)     2371 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createGroupNodes.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      686 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createResource.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)     1081 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createResourceNodes.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      773 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createSubgroup.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      303 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/index.css
+-rw-r--r--   0 dario     (1000) dario     (1000)      135 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/main.tsx
+-rw-r--r--   0 dario     (1000) dario     (1000)   213276 2024-05-02 23:32:35.000000 flowee-1.6/flowee/web/src/schema.json
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/utils/
+-rw-r--r--   0 dario     (1000) dario     (1000)     1060 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/utils/index.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/vite-env.d.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      763 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/tsconfig.json
+-rw-r--r--   0 dario     (1000) dario     (1000)      233 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/tsconfig.node.json
+-rw-r--r--   0 dario     (1000) dario     (1000)      164 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/vite.config.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)    51326 2024-05-09 11:16:39.000000 flowee-1.6/flowee/web/yarn.lock
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee.egg-info/
+-rw-r--r--   0 dario     (1000) dario     (1000)      129 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/PKG-INFO
+-rw-r--r--   0 dario     (1000) dario     (1000)     4677 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/SOURCES.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)        1 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/dependency_links.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       44 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/entry_points.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       17 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/requires.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)        7 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/top_level.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-14 01:43:33.902655 flowee-1.6/setup.cfg
+-rw-r--r--   0 dario     (1000) dario     (1000)     1945 2024-05-14 01:43:26.000000 flowee-1.6/setup.py
```

### Comparing `flowee-1.5/flowee/main.py` & `flowee-1.6/flowee/main.py`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/utils.py` & `flowee-1.6/flowee/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from playwright.sync_api import sync_playwright
 import subprocess
 import os
 import pkg_resources
+import sys
 
 def get_package_installation_path(package_name):
     # Get information about the installed package
     try:
         package = pkg_resources.get_distribution(package_name)
         return package.location
     except pkg_resources.DistributionNotFound:
@@ -33,32 +34,29 @@
         screenshot_path = f"{path}/{name}.png"
         page.screenshot(path=screenshot_path)
 
         browser.close()
         print(f"Screenshot saved at: {screenshot_path}")
 
 def run_react_app(path, name):
-
+    is_shell = sys.platform.startswith('win')
     # Start the React server in the background
-    install = subprocess.run(['npm', 'install'], cwd=web_folder_path, shell=True)
-    build = subprocess.run([ 'npm','run',  'build' ], cwd=web_folder_path, shell=True)
+    install = subprocess.run(['npm', 'install'], cwd=web_folder_path, shell=is_shell)
+    build = subprocess.run([ 'npm','run',  'build' ], cwd=web_folder_path, shell=is_shell)
     print('Opening server ...')
 
     python3_command = ['python3', '-m', 'http.server', '--directory', 'dist']
     python_command = ['python', '-m', 'http.server', '--directory', 'dist']
-    choosed_python = None
 
     try:
         # Try running the command with Python 3
-        startserver = subprocess.Popen(python3_command, cwd=web_folder_path, shell=True)
-        choosed_python = 'python3'
+        startserver = subprocess.Popen(python3_command, cwd=web_folder_path, shell=is_shell)
     except FileNotFoundError:
         # If Python 3 is not found, fall back to Python
-        startserver = subprocess.Popen(python_command, cwd=web_folder_path, shell=True)
-        choosed_python = 'python'
+        startserver = subprocess.Popen(python_command, cwd=web_folder_path, shell=is_shell)
    
     print('Opening browser ...')
     take_screenshot(path, name)
 
     print('Closing server ...')
     startserver.terminate()
```

### Comparing `flowee-1.5/flowee/web/index.html` & `flowee-1.6/flowee/web/index.html`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Bucket.png` & `flowee-1.6/flowee/web/public/assets/Bucket.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/BucketPolicy.png` & `flowee-1.6/flowee/web/public/assets/BucketPolicy.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/CacheCluster.png` & `flowee-1.6/flowee/web/public/assets/CacheCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Certificate.png` & `flowee-1.6/flowee/web/public/assets/Certificate.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Cluster.png` & `flowee-1.6/flowee/web/public/assets/Cluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/ConfigurationSet.png` & `flowee-1.6/flowee/web/public/assets/ConfigurationSet.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/DBCluster.png` & `flowee-1.6/flowee/web/public/assets/DBCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/DBClusterNep.png` & `flowee-1.6/flowee/web/public/assets/DBClusterNep.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Database.png` & `flowee-1.6/flowee/web/public/assets/Database.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Datastore.png` & `flowee-1.6/flowee/web/public/assets/Datastore.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Detector.png` & `flowee-1.6/flowee/web/public/assets/Detector.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Distribution.png` & `flowee-1.6/flowee/web/public/assets/Distribution.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/EventBus.png` & `flowee-1.6/flowee/web/public/assets/EventBus.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Function.png` & `flowee-1.6/flowee/web/public/assets/Function.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Group.png` & `flowee-1.6/flowee/web/public/assets/Group.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/HostedZone.png` & `flowee-1.6/flowee/web/public/assets/HostedZone.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Instance.png` & `flowee-1.6/flowee/web/public/assets/Instance.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/InstanceConnect.png` & `flowee-1.6/flowee/web/public/assets/InstanceConnect.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Key.png` & `flowee-1.6/flowee/web/public/assets/Key.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Keyspace.png` & `flowee-1.6/flowee/web/public/assets/Keyspace.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Method.png` & `flowee-1.6/flowee/web/public/assets/Method.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Protection.png` & `flowee-1.6/flowee/web/public/assets/Protection.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Queue.png` & `flowee-1.6/flowee/web/public/assets/Queue.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png` & `flowee-1.6/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/RestApi.png` & `flowee-1.6/flowee/web/public/assets/RestApi.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Secret.png` & `flowee-1.6/flowee/web/public/assets/Secret.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/StateMachine.png` & `flowee-1.6/flowee/web/public/assets/StateMachine.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Stream.png` & `flowee-1.6/flowee/web/public/assets/Stream.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Table.png` & `flowee-1.6/flowee/web/public/assets/Table.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/TopicRule.png` & `flowee-1.6/flowee/web/public/assets/TopicRule.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/Trail.png` & `flowee-1.6/flowee/web/public/assets/Trail.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/UserPool.png` & `flowee-1.6/flowee/web/public/assets/UserPool.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/VPC.png` & `flowee-1.6/flowee/web/public/assets/VPC.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/WebACL.png` & `flowee-1.6/flowee/web/public/assets/WebACL.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/assets/preact.svg` & `flowee-1.6/flowee/web/public/assets/preact.svg`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/public/vite.svg` & `flowee-1.6/flowee/web/public/vite.svg`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/@types/node.ts` & `flowee-1.6/flowee/web/src/@types/node.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/app.tsx` & `flowee-1.6/flowee/web/src/app.tsx`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/App.png` & `flowee-1.6/flowee/web/src/assets/App.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png` & `flowee-1.6/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png` & `flowee-1.6/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Bucket.png` & `flowee-1.6/flowee/web/src/assets/Bucket.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/BucketPolicy.png` & `flowee-1.6/flowee/web/src/assets/BucketPolicy.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/CacheCluster.png` & `flowee-1.6/flowee/web/src/assets/CacheCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Certificate.png` & `flowee-1.6/flowee/web/src/assets/Certificate.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Cluster.png` & `flowee-1.6/flowee/web/src/assets/Cluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/ConfigurationSet.png` & `flowee-1.6/flowee/web/src/assets/ConfigurationSet.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/DBCluster.png` & `flowee-1.6/flowee/web/src/assets/DBCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/DBClusterNep.png` & `flowee-1.6/flowee/web/src/assets/DBClusterNep.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Database.png` & `flowee-1.6/flowee/web/src/assets/Database.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Datastore.png` & `flowee-1.6/flowee/web/src/assets/Datastore.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Detector.png` & `flowee-1.6/flowee/web/src/assets/Detector.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Distribution.png` & `flowee-1.6/flowee/web/src/assets/Distribution.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/EventBus.png` & `flowee-1.6/flowee/web/src/assets/EventBus.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Function.png` & `flowee-1.6/flowee/web/src/assets/Function.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Group.png` & `flowee-1.6/flowee/web/src/assets/Group.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/HostedZone.png` & `flowee-1.6/flowee/web/src/assets/HostedZone.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Instance.png` & `flowee-1.6/flowee/web/src/assets/Instance.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/InstanceConnect.png` & `flowee-1.6/flowee/web/src/assets/InstanceConnect.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Key.png` & `flowee-1.6/flowee/web/src/assets/Key.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Keyspace.png` & `flowee-1.6/flowee/web/src/assets/Keyspace.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Method.png` & `flowee-1.6/flowee/web/src/assets/Method.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Protection.png` & `flowee-1.6/flowee/web/src/assets/Protection.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Queue.png` & `flowee-1.6/flowee/web/src/assets/Queue.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png` & `flowee-1.6/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/RestApi.png` & `flowee-1.6/flowee/web/src/assets/RestApi.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Secret.png` & `flowee-1.6/flowee/web/src/assets/Secret.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/StateMachine.png` & `flowee-1.6/flowee/web/src/assets/StateMachine.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Stream.png` & `flowee-1.6/flowee/web/src/assets/Stream.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Table.png` & `flowee-1.6/flowee/web/src/assets/Table.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/TopicRule.png` & `flowee-1.6/flowee/web/src/assets/TopicRule.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/Trail.png` & `flowee-1.6/flowee/web/src/assets/Trail.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/UserPool.png` & `flowee-1.6/flowee/web/src/assets/UserPool.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/VPC.png` & `flowee-1.6/flowee/web/src/assets/VPC.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/WebACL.png` & `flowee-1.6/flowee/web/src/assets/WebACL.png`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/assets/preact.svg` & `flowee-1.6/flowee/web/src/assets/preact.svg`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/components/GroupNode/index.tsx` & `flowee-1.6/flowee/web/src/components/GroupNode/index.tsx`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/generators/createGroupNodes.ts` & `flowee-1.6/flowee/web/src/generators/createGroupNodes.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/generators/createResource.ts` & `flowee-1.6/flowee/web/src/generators/createResource.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/generators/createResourceNodes.ts` & `flowee-1.6/flowee/web/src/generators/createResourceNodes.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/generators/createSubgroup.ts` & `flowee-1.6/flowee/web/src/generators/createSubgroup.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/schema.json` & `flowee-1.6/flowee/web/src/schema.json`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/src/utils/index.ts` & `flowee-1.6/flowee/web/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/tsconfig.json` & `flowee-1.6/flowee/web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee/web/yarn.lock` & `flowee-1.6/flowee/web/yarn.lock`

 * *Files identical despite different names*

### Comparing `flowee-1.5/flowee.egg-info/SOURCES.txt` & `flowee-1.6/flowee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowee-1.5/setup.py` & `flowee-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 if os.path.exists(dist_path):
     import shutil
     shutil.rmtree(dist_path)
 
 time.sleep(3)
 setup(
     name='flowee',
-    version='1.5',
+    version='1.6',
     packages=find_packages(),
     install_requires=[
         'playwright',
         'click'
     ],
     package_data={'flowee': ['web/*/**/**/*']},
     include_package_data=True,
```

