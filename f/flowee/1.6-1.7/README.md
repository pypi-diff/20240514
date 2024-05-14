# Comparing `tmp/flowee-1.6.tar.gz` & `tmp/flowee-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowee-1.6.tar", last modified: Tue May 14 01:43:33 2024, max compression
+gzip compressed data, was "flowee-1.7.tar", last modified: Tue May 14 01:55:22 2024, max compression
```

## Comparing `flowee-1.6.tar` & `flowee-1.7.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/
--rw-r--r--   0 dario     (1000) dario     (1000)      129 2024-05-14 01:43:33.902655 flowee-1.6/PKG-INFO
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/
--rw-r--r--   0 dario     (1000) dario     (1000)       29 2024-05-03 17:58:36.000000 flowee-1.6/flowee/__init__.py
--rw-r--r--   0 dario     (1000) dario     (1000)    10278 2024-05-09 17:30:50.000000 flowee-1.6/flowee/main.py
--rw-r--r--   0 dario     (1000) dario     (1000)     2140 2024-05-14 01:37:19.000000 flowee-1.6/flowee/utils.py
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/
--rw-r--r--   0 dario     (1000) dario     (1000)        0 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/__init_.py
--rw-r--r--   0 dario     (1000) dario     (1000)      636 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/index.html
--rw-r--r--   0 dario     (1000) dario     (1000)      470 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/package.json
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/public/
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/public/assets/
--rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Bucket.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/BucketPolicy.png
--rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/CacheCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Certificate.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Cluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/ConfigurationSet.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/DBCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/DBClusterNep.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Database.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Datastore.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Detector.png
--rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Distribution.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/EventBus.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Function.png
--rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Group.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/HostedZone.png
--rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Instance.png
--rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/InstanceConnect.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Key.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Keyspace.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Method.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Protection.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Queue.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/RestApi.png
--rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Secret.png
--rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/StateMachine.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Stream.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Table.png
--rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/TopicRule.png
--rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/Trail.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/UserPool.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/VPC.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/WebACL.png
--rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/assets/preact.svg
--rw-r--r--   0 dario     (1000) dario     (1000)     1497 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/public/vite.svg
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/src/
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee/web/src/@types/
--rw-r--r--   0 dario     (1000) dario     (1000)       62 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/@types/edges.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      809 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/@types/node.ts
--rw-r--r--   0 dario     (1000) dario     (1000)     2362 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/app.tsx
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/assets/
--rw-r--r--   0 dario     (1000) dario     (1000)    18801 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/App.png
--rw-r--r--   0 dario     (1000) dario     (1000)    21168 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)     5561 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19421 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11123 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    10559 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9220 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11223 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14674 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    17740 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20193 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9425 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22687 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    18512 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20178 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11295 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png
--rw-r--r--   0 dario     (1000) dario     (1000)      947 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Bucket.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/BucketPolicy.png
--rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/CacheCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Certificate.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Cluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/ConfigurationSet.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/DBCluster.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/DBClusterNep.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Database.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Datastore.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Detector.png
--rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Distribution.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/EventBus.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Function.png
--rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Group.png
--rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/HostedZone.png
--rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Instance.png
--rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/InstanceConnect.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Key.png
--rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Keyspace.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Method.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Protection.png
--rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Queue.png
--rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png
--rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/RestApi.png
--rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Secret.png
--rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/StateMachine.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Stream.png
--rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Table.png
--rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/TopicRule.png
--rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/Trail.png
--rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/UserPool.png
--rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/VPC.png
--rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/WebACL.png
--rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/assets/preact.svg
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.882655 flowee-1.6/flowee/web/src/components/
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/components/GroupNode/
--rw-r--r--   0 dario     (1000) dario     (1000)      540 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/GroupNode/index.tsx
--rw-r--r--   0 dario     (1000) dario     (1000)      502 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/GroupNode/styles.ts
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/components/ResourceNode/
--rw-r--r--   0 dario     (1000) dario     (1000)      499 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/ResourceNode/index.tsx
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/components/SubGroupNode/
--rw-r--r--   0 dario     (1000) dario     (1000)       80 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/components/SubGroupNode/index.tsx
--rw-r--r--   0 dario     (1000) dario     (1000)       34 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/constants.ts
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/generators/
--rw-r--r--   0 dario     (1000) dario     (1000)      488 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createGroup.ts
--rw-r--r--   0 dario     (1000) dario     (1000)     2371 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createGroupNodes.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      686 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createResource.ts
--rw-r--r--   0 dario     (1000) dario     (1000)     1081 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createResourceNodes.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      773 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/generators/createSubgroup.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      303 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/index.css
--rw-r--r--   0 dario     (1000) dario     (1000)      135 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/main.tsx
--rw-r--r--   0 dario     (1000) dario     (1000)   213276 2024-05-02 23:32:35.000000 flowee-1.6/flowee/web/src/schema.json
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.902655 flowee-1.6/flowee/web/src/utils/
--rw-r--r--   0 dario     (1000) dario     (1000)     1060 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/utils/index.ts
--rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/src/vite-env.d.ts
--rw-r--r--   0 dario     (1000) dario     (1000)      763 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/tsconfig.json
--rw-r--r--   0 dario     (1000) dario     (1000)      233 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/tsconfig.node.json
--rw-r--r--   0 dario     (1000) dario     (1000)      164 2024-05-03 17:58:36.000000 flowee-1.6/flowee/web/vite.config.ts
--rw-r--r--   0 dario     (1000) dario     (1000)    51326 2024-05-09 11:16:39.000000 flowee-1.6/flowee/web/yarn.lock
-drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:43:33.892655 flowee-1.6/flowee.egg-info/
--rw-r--r--   0 dario     (1000) dario     (1000)      129 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/PKG-INFO
--rw-r--r--   0 dario     (1000) dario     (1000)     4677 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/SOURCES.txt
--rw-r--r--   0 dario     (1000) dario     (1000)        1 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/dependency_links.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       44 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/entry_points.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       17 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/requires.txt
--rw-r--r--   0 dario     (1000) dario     (1000)        7 2024-05-14 01:43:33.000000 flowee-1.6/flowee.egg-info/top_level.txt
--rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-14 01:43:33.902655 flowee-1.6/setup.cfg
--rw-r--r--   0 dario     (1000) dario     (1000)     1945 2024-05-14 01:43:26.000000 flowee-1.6/setup.py
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.915269 flowee-1.7/
+-rw-r--r--   0 dario     (1000) dario     (1000)     3044 2024-05-14 01:55:22.915269 flowee-1.7/PKG-INFO
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.895269 flowee-1.7/flowee/
+-rw-r--r--   0 dario     (1000) dario     (1000)       29 2024-05-03 17:58:36.000000 flowee-1.7/flowee/__init__.py
+-rw-r--r--   0 dario     (1000) dario     (1000)    10278 2024-05-09 17:30:50.000000 flowee-1.7/flowee/main.py
+-rw-r--r--   0 dario     (1000) dario     (1000)     2140 2024-05-14 01:37:19.000000 flowee-1.7/flowee/utils.py
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.895269 flowee-1.7/flowee/web/
+-rw-r--r--   0 dario     (1000) dario     (1000)        0 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/__init_.py
+-rw-r--r--   0 dario     (1000) dario     (1000)      636 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/index.html
+-rw-r--r--   0 dario     (1000) dario     (1000)      470 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/package.json
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.895269 flowee-1.7/flowee/web/public/
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.895269 flowee-1.7/flowee/web/public/assets/
+-rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Bucket.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/BucketPolicy.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/CacheCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Certificate.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Cluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/ConfigurationSet.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/DBCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/DBClusterNep.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Database.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Datastore.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Detector.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Distribution.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/EventBus.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Function.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Group.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/HostedZone.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Instance.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/InstanceConnect.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Key.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Keyspace.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Method.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Protection.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Queue.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/RestApi.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Secret.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/StateMachine.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Stream.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Table.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/TopicRule.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/Trail.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/UserPool.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/VPC.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/WebACL.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/assets/preact.svg
+-rw-r--r--   0 dario     (1000) dario     (1000)     1497 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/public/vite.svg
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.905269 flowee-1.7/flowee/web/src/
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.905269 flowee-1.7/flowee/web/src/@types/
+-rw-r--r--   0 dario     (1000) dario     (1000)       62 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/@types/edges.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      809 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/@types/node.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)     2362 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/app.tsx
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.905269 flowee-1.7/flowee/web/src/assets/
+-rw-r--r--   0 dario     (1000) dario     (1000)    18801 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/App.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    21168 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     5561 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19421 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11123 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    10559 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9220 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11223 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14674 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    17740 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20193 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9425 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22687 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    18512 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20178 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11295 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png
+-rw-r--r--   0 dario     (1000) dario     (1000)      947 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16959 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Bucket.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3108 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/BucketPolicy.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    12740 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/CacheCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     9127 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Certificate.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13749 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Cluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16036 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/ConfigurationSet.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2605 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/DBCluster.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19338 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/DBClusterNep.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16472 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Database.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22295 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Datastore.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20168 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Detector.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    21046 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Distribution.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19396 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/EventBus.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14573 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Function.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     6923 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Group.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    22509 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/HostedZone.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     5263 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Instance.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    18340 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/InstanceConnect.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13205 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Key.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    16343 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Keyspace.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3221 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Method.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13896 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Protection.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    19469 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Queue.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     2329 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    11575 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/RestApi.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    15864 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Secret.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     8303 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/StateMachine.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14778 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Stream.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     3455 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Table.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    17095 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/TopicRule.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    10009 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/Trail.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    14385 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/UserPool.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    13838 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/VPC.png
+-rw-r--r--   0 dario     (1000) dario     (1000)    20830 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/WebACL.png
+-rw-r--r--   0 dario     (1000) dario     (1000)     1591 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/assets/preact.svg
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.895269 flowee-1.7/flowee/web/src/components/
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.905269 flowee-1.7/flowee/web/src/components/GroupNode/
+-rw-r--r--   0 dario     (1000) dario     (1000)      540 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/components/GroupNode/index.tsx
+-rw-r--r--   0 dario     (1000) dario     (1000)      502 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/components/GroupNode/styles.ts
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.905269 flowee-1.7/flowee/web/src/components/ResourceNode/
+-rw-r--r--   0 dario     (1000) dario     (1000)      499 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/components/ResourceNode/index.tsx
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.905269 flowee-1.7/flowee/web/src/components/SubGroupNode/
+-rw-r--r--   0 dario     (1000) dario     (1000)       80 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/components/SubGroupNode/index.tsx
+-rw-r--r--   0 dario     (1000) dario     (1000)       34 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/constants.ts
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.915269 flowee-1.7/flowee/web/src/generators/
+-rw-r--r--   0 dario     (1000) dario     (1000)      488 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/generators/createGroup.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)     2371 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/generators/createGroupNodes.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      686 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/generators/createResource.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)     1081 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/generators/createResourceNodes.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      773 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/generators/createSubgroup.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      303 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/index.css
+-rw-r--r--   0 dario     (1000) dario     (1000)      135 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/main.tsx
+-rw-r--r--   0 dario     (1000) dario     (1000)   213276 2024-05-02 23:32:35.000000 flowee-1.7/flowee/web/src/schema.json
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.915269 flowee-1.7/flowee/web/src/utils/
+-rw-r--r--   0 dario     (1000) dario     (1000)     1060 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/utils/index.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/src/vite-env.d.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)      763 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/tsconfig.json
+-rw-r--r--   0 dario     (1000) dario     (1000)      233 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/tsconfig.node.json
+-rw-r--r--   0 dario     (1000) dario     (1000)      164 2024-05-03 17:58:36.000000 flowee-1.7/flowee/web/vite.config.ts
+-rw-r--r--   0 dario     (1000) dario     (1000)    51326 2024-05-09 11:16:39.000000 flowee-1.7/flowee/web/yarn.lock
+drwxr-xr-x   0 dario     (1000) dario     (1000)        0 2024-05-14 01:55:22.895269 flowee-1.7/flowee.egg-info/
+-rw-r--r--   0 dario     (1000) dario     (1000)     3044 2024-05-14 01:55:22.000000 flowee-1.7/flowee.egg-info/PKG-INFO
+-rw-r--r--   0 dario     (1000) dario     (1000)     4677 2024-05-14 01:55:22.000000 flowee-1.7/flowee.egg-info/SOURCES.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)        1 2024-05-14 01:55:22.000000 flowee-1.7/flowee.egg-info/dependency_links.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       44 2024-05-14 01:55:22.000000 flowee-1.7/flowee.egg-info/entry_points.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       17 2024-05-14 01:55:22.000000 flowee-1.7/flowee.egg-info/requires.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)        7 2024-05-14 01:55:22.000000 flowee-1.7/flowee.egg-info/top_level.txt
+-rw-r--r--   0 dario     (1000) dario     (1000)       38 2024-05-14 01:55:22.915269 flowee-1.7/setup.cfg
+-rw-r--r--   0 dario     (1000) dario     (1000)     2328 2024-05-14 01:55:17.000000 flowee-1.7/setup.py
```

### Comparing `flowee-1.6/flowee/main.py` & `flowee-1.7/flowee/main.py`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/utils.py` & `flowee-1.7/flowee/utils.py`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/index.html` & `flowee-1.7/flowee/web/index.html`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Bucket.png` & `flowee-1.7/flowee/web/public/assets/Bucket.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/BucketPolicy.png` & `flowee-1.7/flowee/web/public/assets/BucketPolicy.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/CacheCluster.png` & `flowee-1.7/flowee/web/public/assets/CacheCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Certificate.png` & `flowee-1.7/flowee/web/public/assets/Certificate.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Cluster.png` & `flowee-1.7/flowee/web/public/assets/Cluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/ConfigurationSet.png` & `flowee-1.7/flowee/web/public/assets/ConfigurationSet.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/DBCluster.png` & `flowee-1.7/flowee/web/public/assets/DBCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/DBClusterNep.png` & `flowee-1.7/flowee/web/public/assets/DBClusterNep.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Database.png` & `flowee-1.7/flowee/web/public/assets/Database.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Datastore.png` & `flowee-1.7/flowee/web/public/assets/Datastore.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Detector.png` & `flowee-1.7/flowee/web/public/assets/Detector.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Distribution.png` & `flowee-1.7/flowee/web/public/assets/Distribution.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/EventBus.png` & `flowee-1.7/flowee/web/public/assets/EventBus.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Function.png` & `flowee-1.7/flowee/web/public/assets/Function.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Group.png` & `flowee-1.7/flowee/web/public/assets/Group.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/HostedZone.png` & `flowee-1.7/flowee/web/public/assets/HostedZone.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Instance.png` & `flowee-1.7/flowee/web/public/assets/Instance.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/InstanceConnect.png` & `flowee-1.7/flowee/web/public/assets/InstanceConnect.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Key.png` & `flowee-1.7/flowee/web/public/assets/Key.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Keyspace.png` & `flowee-1.7/flowee/web/public/assets/Keyspace.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Method.png` & `flowee-1.7/flowee/web/public/assets/Method.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Protection.png` & `flowee-1.7/flowee/web/public/assets/Protection.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Queue.png` & `flowee-1.7/flowee/web/public/assets/Queue.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png` & `flowee-1.7/flowee/web/public/assets/Res_AWS-IoT_Policy_48.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/RestApi.png` & `flowee-1.7/flowee/web/public/assets/RestApi.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Secret.png` & `flowee-1.7/flowee/web/public/assets/Secret.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/StateMachine.png` & `flowee-1.7/flowee/web/public/assets/StateMachine.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Stream.png` & `flowee-1.7/flowee/web/public/assets/Stream.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Table.png` & `flowee-1.7/flowee/web/public/assets/Table.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/TopicRule.png` & `flowee-1.7/flowee/web/public/assets/TopicRule.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/Trail.png` & `flowee-1.7/flowee/web/public/assets/Trail.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/UserPool.png` & `flowee-1.7/flowee/web/public/assets/UserPool.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/VPC.png` & `flowee-1.7/flowee/web/public/assets/VPC.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/WebACL.png` & `flowee-1.7/flowee/web/public/assets/WebACL.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/assets/preact.svg` & `flowee-1.7/flowee/web/public/assets/preact.svg`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/public/vite.svg` & `flowee-1.7/flowee/web/public/vite.svg`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/@types/node.ts` & `flowee-1.7/flowee/web/src/@types/node.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/app.tsx` & `flowee-1.7/flowee/web/src/app.tsx`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/App.png` & `flowee-1.7/flowee/web/src/assets/App.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Backup_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Billing-Conductor_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Cost-Explorer_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Cost-and-Usage-Report_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Express-Workflows_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Organizations_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Private-Certificate-Authority_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_AWS-Storage-Gateway_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_Amazon-Aurora_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_Amazon-CloudWatch_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_Amazon-Elastic-Block-Store_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_Amazon-Elastic-Inference_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_Amazon-MemoryDB-for-Redis_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_Amazon-Simple-Storage-Service-Glacier_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png` & `flowee-1.7/flowee/web/src/assets/Arch_Amazon-VPC-Lattice_64@5x.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png` & `flowee-1.7/flowee/web/src/assets/Arch_Elastic-Load-Balancing_32.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Bucket.png` & `flowee-1.7/flowee/web/src/assets/Bucket.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/BucketPolicy.png` & `flowee-1.7/flowee/web/src/assets/BucketPolicy.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/CacheCluster.png` & `flowee-1.7/flowee/web/src/assets/CacheCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Certificate.png` & `flowee-1.7/flowee/web/src/assets/Certificate.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Cluster.png` & `flowee-1.7/flowee/web/src/assets/Cluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/ConfigurationSet.png` & `flowee-1.7/flowee/web/src/assets/ConfigurationSet.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/DBCluster.png` & `flowee-1.7/flowee/web/src/assets/DBCluster.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/DBClusterNep.png` & `flowee-1.7/flowee/web/src/assets/DBClusterNep.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Database.png` & `flowee-1.7/flowee/web/src/assets/Database.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Datastore.png` & `flowee-1.7/flowee/web/src/assets/Datastore.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Detector.png` & `flowee-1.7/flowee/web/src/assets/Detector.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Distribution.png` & `flowee-1.7/flowee/web/src/assets/Distribution.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/EventBus.png` & `flowee-1.7/flowee/web/src/assets/EventBus.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Function.png` & `flowee-1.7/flowee/web/src/assets/Function.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Group.png` & `flowee-1.7/flowee/web/src/assets/Group.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/HostedZone.png` & `flowee-1.7/flowee/web/src/assets/HostedZone.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Instance.png` & `flowee-1.7/flowee/web/src/assets/Instance.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/InstanceConnect.png` & `flowee-1.7/flowee/web/src/assets/InstanceConnect.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Key.png` & `flowee-1.7/flowee/web/src/assets/Key.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Keyspace.png` & `flowee-1.7/flowee/web/src/assets/Keyspace.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Method.png` & `flowee-1.7/flowee/web/src/assets/Method.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Protection.png` & `flowee-1.7/flowee/web/src/assets/Protection.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Queue.png` & `flowee-1.7/flowee/web/src/assets/Queue.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png` & `flowee-1.7/flowee/web/src/assets/Res_AWS-IoT_Policy_48.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/RestApi.png` & `flowee-1.7/flowee/web/src/assets/RestApi.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Secret.png` & `flowee-1.7/flowee/web/src/assets/Secret.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/StateMachine.png` & `flowee-1.7/flowee/web/src/assets/StateMachine.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Stream.png` & `flowee-1.7/flowee/web/src/assets/Stream.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Table.png` & `flowee-1.7/flowee/web/src/assets/Table.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/TopicRule.png` & `flowee-1.7/flowee/web/src/assets/TopicRule.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/Trail.png` & `flowee-1.7/flowee/web/src/assets/Trail.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/UserPool.png` & `flowee-1.7/flowee/web/src/assets/UserPool.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/VPC.png` & `flowee-1.7/flowee/web/src/assets/VPC.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/WebACL.png` & `flowee-1.7/flowee/web/src/assets/WebACL.png`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/assets/preact.svg` & `flowee-1.7/flowee/web/src/assets/preact.svg`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/components/GroupNode/index.tsx` & `flowee-1.7/flowee/web/src/components/GroupNode/index.tsx`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/generators/createGroupNodes.ts` & `flowee-1.7/flowee/web/src/generators/createGroupNodes.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/generators/createResource.ts` & `flowee-1.7/flowee/web/src/generators/createResource.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/generators/createResourceNodes.ts` & `flowee-1.7/flowee/web/src/generators/createResourceNodes.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/generators/createSubgroup.ts` & `flowee-1.7/flowee/web/src/generators/createSubgroup.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/schema.json` & `flowee-1.7/flowee/web/src/schema.json`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/src/utils/index.ts` & `flowee-1.7/flowee/web/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/tsconfig.json` & `flowee-1.7/flowee/web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee/web/yarn.lock` & `flowee-1.7/flowee/web/yarn.lock`

 * *Files identical despite different names*

### Comparing `flowee-1.6/flowee.egg-info/SOURCES.txt` & `flowee-1.7/flowee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flowee-1.6/setup.py` & `flowee-1.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os, time, subprocess, sys
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.MD").read_text()
+
 
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         try:
             if sys.platform.startswith('win'):
                 subprocess.call(['playwright.cmd', 'install-deps'])  # Adjust if necessary
@@ -38,24 +43,28 @@
 if os.path.exists(dist_path):
     import shutil
     shutil.rmtree(dist_path)
 
 time.sleep(3)
 setup(
     name='flowee',
-    version='1.6',
+    version='1.7',
     packages=find_packages(),
     install_requires=[
         'playwright',
         'click'
     ],
+    description='A CLI tool to create AWS diagrams from Cloudformation templates.',
     package_data={'flowee': ['web/*/**/**/*']},
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'flowee=flowee.cli:main',
         ],
     },
     cmdclass={
         'install': PostInstallCommand,
     },
+    author='Westpoint Software Solutions',
+    long_description=long_description,
+    long_description_content_type='text/markdown'
 )
```

