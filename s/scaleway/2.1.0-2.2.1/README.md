# Comparing `tmp/scaleway-2.1.0.tar.gz` & `tmp/scaleway-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway-2.1.0.tar", max compression
+gzip compressed data, was "scaleway-2.2.1.tar", max compression
```

## Comparing `scaleway-2.1.0.tar` & `scaleway-2.2.1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rw-r--r--   0        0        0       76 2024-04-22 08:29:48.764789 scaleway-2.1.0/README.md
--rw-r--r--   0        0        0     1112 2024-04-22 08:30:12.112698 scaleway-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      905 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/__init__.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/__init__.py
--rw-r--r--   0        0        0      714 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v2/__init__.py
--rw-r--r--   0        0        0     8456 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v2/api.py
--rw-r--r--   0        0        0     2850 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v2/marshalling.py
--rw-r--r--   0        0        0     2638 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v2/types.py
--rw-r--r--   0        0        0      828 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v3/__init__.py
--rw-r--r--   0        0        0     8180 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v3/api.py
--rw-r--r--   0        0        0     2910 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v3/marshalling.py
--rw-r--r--   0        0        0     2678 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/account/v3/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/applesilicon/__init__.py
--rw-r--r--   0        0        0     1674 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/applesilicon/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18185 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/applesilicon/v1alpha1/api.py
--rw-r--r--   0        0        0      496 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/applesilicon/v1alpha1/content.py
--rw-r--r--   0        0        0     7838 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/applesilicon/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     7171 2024-04-22 08:29:48.764789 scaleway-2.1.0/scaleway/applesilicon/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/baremetal/__init__.py
--rw-r--r--   0        0        0     5338 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/baremetal/v1/__init__.py
--rw-r--r--   0        0        0    52768 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/baremetal/v1/api.py
--rw-r--r--   0        0        0     1063 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/baremetal/v1/content.py
--rw-r--r--   0        0        0    31593 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/baremetal/v1/marshalling.py
--rw-r--r--   0        0        0    27983 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/baremetal/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/__init__.py
--rw-r--r--   0        0        0     1414 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2alpha1/__init__.py
--rw-r--r--   0        0        0     9098 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2alpha1/api.py
--rw-r--r--   0        0        0     7732 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2alpha1/marshalling.py
--rw-r--r--   0        0        0     7103 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2alpha1/types.py
--rw-r--r--   0        0        0     2078 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2beta1/__init__.py
--rw-r--r--   0        0        0    18927 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2beta1/api.py
--rw-r--r--   0        0        0    11343 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2beta1/marshalling.py
--rw-r--r--   0        0        0    12804 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/billing/v2beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/block/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/block/v1alpha1/__init__.py
--rw-r--r--   0        0        0    25022 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/block/v1alpha1/api.py
--rw-r--r--   0        0        0      922 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/block/v1alpha1/content.py
--rw-r--r--   0        0        0    12380 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/block/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    12472 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/block/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/__init__.py
--rw-r--r--   0        0        0     4656 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1/__init__.py
--rw-r--r--   0        0        0    46974 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1/api.py
--rw-r--r--   0        0        0    20821 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1/marshalling.py
--rw-r--r--   0        0        0    20051 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1/types.py
--rw-r--r--   0        0        0     3758 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1beta1/__init__.py
--rw-r--r--   0        0        0    33332 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1beta1/api.py
--rw-r--r--   0        0        0      418 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1beta1/content.py
--rw-r--r--   0        0        0    21780 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1beta1/marshalling.py
--rw-r--r--   0        0        0    15330 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/cockpit/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/container/__init__.py
--rw-r--r--   0        0        0     5100 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/container/v1beta1/__init__.py
--rw-r--r--   0        0        0    63615 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/container/v1beta1/api.py
--rw-r--r--   0        0        0     1581 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/container/v1beta1/content.py
--rw-r--r--   0        0        0    27167 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/container/v1beta1/marshalling.py
--rw-r--r--   0        0        0    27207 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/container/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/dedibox/__init__.py
--rw-r--r--   0        0        0    19280 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/dedibox/v1/__init__.py
--rw-r--r--   0        0        0   138198 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/dedibox/v1/api.py
--rw-r--r--   0        0        0     2688 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/dedibox/v1/content.py
--rw-r--r--   0        0        0    99051 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/dedibox/v1/marshalling.py
--rw-r--r--   0        0        0    74459 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/dedibox/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/document_db/__init__.py
--rw-r--r--   0        0        0     9342 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/document_db/v1beta1/__init__.py
--rw-r--r--   0        0        0   103285 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/document_db/v1beta1/api.py
--rw-r--r--   0        0        0     1614 2024-04-22 08:29:48.768789 scaleway-2.1.0/scaleway/document_db/v1beta1/content.py
--rw-r--r--   0        0        0    52232 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/document_db/v1beta1/marshalling.py
--rw-r--r--   0        0        0    42675 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/document_db/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/domain/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/domain/v2beta1/__init__.py
--rw-r--r--   0        0        0    91007 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/domain/v2beta1/api.py
--rw-r--r--   0        0        0     1948 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/domain/v2beta1/content.py
--rw-r--r--   0        0        0    90187 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/domain/v2beta1/marshalling.py
--rw-r--r--   0        0        0    36143 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/domain/v2beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/flexibleip/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/flexibleip/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20507 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/flexibleip/v1alpha1/api.py
--rw-r--r--   0        0        0      649 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/flexibleip/v1alpha1/content.py
--rw-r--r--   0        0        0     8075 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/flexibleip/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8804 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/flexibleip/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/function/__init__.py
--rw-r--r--   0        0        0     5594 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/function/v1beta1/__init__.py
--rw-r--r--   0        0        0    65530 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/function/v1beta1/api.py
--rw-r--r--   0        0        0     1573 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/function/v1beta1/content.py
--rw-r--r--   0        0        0    29502 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/function/v1beta1/marshalling.py
--rw-r--r--   0        0        0    28712 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/function/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iam/__init__.py
--rw-r--r--   0        0        0     5586 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iam/v1alpha1/__init__.py
--rw-r--r--   0        0        0    84589 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iam/v1alpha1/api.py
--rw-r--r--   0        0        0    33530 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iam/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    30388 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iam/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/instance/__init__.py
--rw-r--r--   0        0        0    13930 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/instance/v1/__init__.py
--rw-r--r--   0        0        0   151562 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/instance/v1/api.py
--rw-r--r--   0        0        0     2388 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/instance/v1/content.py
--rw-r--r--   0        0        0   116264 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/instance/v1/marshalling.py
--rw-r--r--   0        0        0    65118 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/instance/v1/types.py
--rw-r--r--   0        0        0     6858 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/instance/v1/types_private.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iot/__init__.py
--rw-r--r--   0        0        0     5818 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iot/v1/__init__.py
--rw-r--r--   0        0        0    61877 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iot/v1/api.py
--rw-r--r--   0        0        0      363 2024-04-22 08:29:48.772789 scaleway-2.1.0/scaleway/iot/v1/content.py
--rw-r--r--   0        0        0    33954 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/iot/v1/marshalling.py
--rw-r--r--   0        0        0    29997 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/iot/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipam/__init__.py
--rw-r--r--   0        0        0      804 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipam/v1/__init__.py
--rw-r--r--   0        0        0    13582 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipam/v1/api.py
--rw-r--r--   0        0        0     6042 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipam/v1/marshalling.py
--rw-r--r--   0        0        0     6482 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipam/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipfs/__init__.py
--rw-r--r--   0        0        0     2572 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipfs/v1alpha1/__init__.py
--rw-r--r--   0        0        0    33644 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipfs/v1alpha1/api.py
--rw-r--r--   0        0        0      552 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipfs/v1alpha1/content.py
--rw-r--r--   0        0        0    12468 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipfs/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    11507 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/ipfs/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/jobs/__init__.py
--rw-r--r--   0        0        0     1760 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/jobs/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18492 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/jobs/v1alpha1/api.py
--rw-r--r--   0        0        0      402 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/jobs/v1alpha1/content.py
--rw-r--r--   0        0        0    11385 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/jobs/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     7454 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/jobs/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/k8s/__init__.py
--rw-r--r--   0        0        0     5344 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/k8s/v1/__init__.py
--rw-r--r--   0        0        0    58403 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/k8s/v1/api.py
--rw-r--r--   0        0        0      934 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/k8s/v1/content.py
--rw-r--r--   0        0        0    40250 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/k8s/v1/marshalling.py
--rw-r--r--   0        0        0    44725 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/k8s/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/lb/__init__.py
--rw-r--r--   0        0        0    13124 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/lb/v1/__init__.py
--rw-r--r--   0        0        0   227386 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/lb/v1/api.py
--rw-r--r--   0        0        0     1107 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/lb/v1/content.py
--rw-r--r--   0        0        0    82547 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/lb/v1/marshalling.py
--rw-r--r--   0        0        0    90467 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/lb/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/llm_inference/__init__.py
--rw-r--r--   0        0        0     3026 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/llm_inference/v1beta1/__init__.py
--rw-r--r--   0        0        0    31541 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/llm_inference/v1beta1/api.py
--rw-r--r--   0        0        0      443 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/llm_inference/v1beta1/content.py
--rw-r--r--   0        0        0    17690 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/llm_inference/v1beta1/marshalling.py
--rw-r--r--   0        0        0    14475 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/llm_inference/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/marketplace/__init__.py
--rw-r--r--   0        0        0     1470 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/marketplace/v2/__init__.py
--rw-r--r--   0        0        0    14905 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/marketplace/v2/api.py
--rw-r--r--   0        0        0     6721 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/marketplace/v2/marshalling.py
--rw-r--r--   0        0        0     5135 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/marketplace/v2/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/mnq/__init__.py
--rw-r--r--   0        0        0     3766 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/mnq/v1beta1/__init__.py
--rw-r--r--   0        0        0    42072 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/mnq/v1beta1/api.py
--rw-r--r--   0        0        0    18048 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/mnq/v1beta1/marshalling.py
--rw-r--r--   0        0        0    16867 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/mnq/v1beta1/types.py
--rw-r--r--   0        0        0        0 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/py.typed
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/qaas/__init__.py
--rw-r--r--   0        0        0     4200 2024-04-22 08:29:48.776789 scaleway-2.1.0/scaleway/qaas/v1alpha1/__init__.py
--rw-r--r--   0        0        0    42961 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/qaas/v1alpha1/api.py
--rw-r--r--   0        0        0      843 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/qaas/v1alpha1/content.py
--rw-r--r--   0        0        0    18882 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/qaas/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    19382 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/qaas/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/rdb/__init__.py
--rw-r--r--   0        0        0    10564 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/rdb/v1/__init__.py
--rw-r--r--   0        0        0   119808 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/rdb/v1/api.py
--rw-r--r--   0        0        0     1950 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/rdb/v1/content.py
--rw-r--r--   0        0        0    57727 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/rdb/v1/marshalling.py
--rw-r--r--   0        0        0    48945 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/rdb/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/redis/__init__.py
--rw-r--r--   0        0        0     3760 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/redis/v1/__init__.py
--rw-r--r--   0        0        0    44423 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/redis/v1/api.py
--rw-r--r--   0        0        0      488 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/redis/v1/content.py
--rw-r--r--   0        0        0    21935 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/redis/v1/marshalling.py
--rw-r--r--   0        0        0    17769 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/redis/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/registry/__init__.py
--rw-r--r--   0        0        0     1962 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/registry/v1/__init__.py
--rw-r--r--   0        0        0    29203 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/registry/v1/api.py
--rw-r--r--   0        0        0      710 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/registry/v1/content.py
--rw-r--r--   0        0        0     8195 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/registry/v1/marshalling.py
--rw-r--r--   0        0        0    11276 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/registry/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/__init__.py
--rw-r--r--   0        0        0     3160 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1alpha1/__init__.py
--rw-r--r--   0        0        0    51007 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1alpha1/api.py
--rw-r--r--   0        0        0    15827 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    21526 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1alpha1/types.py
--rw-r--r--   0        0        0     3050 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1beta1/__init__.py
--rw-r--r--   0        0        0    36548 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1beta1/api.py
--rw-r--r--   0        0        0    15392 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1beta1/marshalling.py
--rw-r--r--   0        0        0    18709 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/secret/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/serverless_sqldb/__init__.py
--rw-r--r--   0        0        0     1528 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/__init__.py
--rw-r--r--   0        0        0    19895 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/api.py
--rw-r--r--   0        0        0      427 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/content.py
--rw-r--r--   0        0        0     6440 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8013 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/types.py
--rw-r--r--   0        0        0      194 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/std/__init__.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/std/api.py
--rw-r--r--   0        0        0      129 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/std/marshalling.py
--rw-r--r--   0        0        0      469 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/std/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/tem/__init__.py
--rw-r--r--   0        0        0     2646 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/tem/v1alpha1/__init__.py
--rw-r--r--   0        0        0    26023 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/tem/v1alpha1/api.py
--rw-r--r--   0        0        0      549 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/tem/v1alpha1/content.py
--rw-r--r--   0        0        0    18144 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/tem/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    16470 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/tem/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/test/__init__.py
--rw-r--r--   0        0        0     1088 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/test/v1/__init__.py
--rw-r--r--   0        0        0    11588 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/test/v1/api.py
--rw-r--r--   0        0        0      349 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/test/v1/content.py
--rw-r--r--   0        0        0     6231 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/test/v1/marshalling.py
--rw-r--r--   0        0        0     3231 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/test/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/vpc/__init__.py
--rw-r--r--   0        0        0      818 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/vpc/v1/__init__.py
--rw-r--r--   0        0        0    11732 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/vpc/v1/api.py
--rw-r--r--   0        0        0     3338 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/vpc/v1/marshalling.py
--rw-r--r--   0        0        0     4368 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/vpc/v1/types.py
--rw-r--r--   0        0        0     1932 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/vpc/v2/__init__.py
--rw-r--r--   0        0        0    31050 2024-04-22 08:29:48.780789 scaleway-2.1.0/scaleway/vpc/v2/api.py
--rw-r--r--   0        0        0    10469 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpc/v2/marshalling.py
--rw-r--r--   0        0        0    10678 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpc/v2/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpcgw/__init__.py
--rw-r--r--   0        0        0     4846 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpcgw/v1/__init__.py
--rw-r--r--   0        0        0    81299 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpcgw/v1/api.py
--rw-r--r--   0        0        0      755 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpcgw/v1/content.py
--rw-r--r--   0        0        0    30617 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpcgw/v1/marshalling.py
--rw-r--r--   0        0        0    35539 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/vpcgw/v1/types.py
--rw-r--r--   0        0        0      127 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/webhosting/__init__.py
--rw-r--r--   0        0        0     2234 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/webhosting/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20950 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/webhosting/v1alpha1/api.py
--rw-r--r--   0        0        0      421 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/webhosting/v1alpha1/content.py
--rw-r--r--   0        0        0    14155 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/webhosting/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    13805 2024-04-22 08:29:48.784789 scaleway-2.1.0/scaleway/webhosting/v1alpha1/types.py
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 scaleway-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       76 2024-05-14 12:14:18.420369 scaleway-2.2.1/README.md
+-rw-r--r--   0        0        0     1112 2024-05-14 12:14:34.792216 scaleway-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      905 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/__init__.py
+-rw-r--r--   0        0        0     8456 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/api.py
+-rw-r--r--   0        0        0     2850 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/marshalling.py
+-rw-r--r--   0        0        0     2638 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/types.py
+-rw-r--r--   0        0        0      828 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/__init__.py
+-rw-r--r--   0        0        0     8180 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/api.py
+-rw-r--r--   0        0        0     2910 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/marshalling.py
+-rw-r--r--   0        0        0     2678 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/__init__.py
+-rw-r--r--   0        0        0     1674 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18924 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/api.py
+-rw-r--r--   0        0        0      496 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/content.py
+-rw-r--r--   0        0        0     8890 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8104 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/__init__.py
+-rw-r--r--   0        0        0     5338 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/__init__.py
+-rw-r--r--   0        0        0    52768 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/api.py
+-rw-r--r--   0        0        0     1063 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/content.py
+-rw-r--r--   0        0        0    31590 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/marshalling.py
+-rw-r--r--   0        0        0    27983 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/__init__.py
+-rw-r--r--   0        0        0     1414 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/__init__.py
+-rw-r--r--   0        0        0     9098 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/api.py
+-rw-r--r--   0        0        0     7732 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/marshalling.py
+-rw-r--r--   0        0        0     7103 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/types.py
+-rw-r--r--   0        0        0     2078 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/__init__.py
+-rw-r--r--   0        0        0    18927 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/api.py
+-rw-r--r--   0        0        0    11343 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    12804 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/__init__.py
+-rw-r--r--   0        0        0     2398 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    27041 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/api.py
+-rw-r--r--   0        0        0      922 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/content.py
+-rw-r--r--   0        0        0    13085 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    13168 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/__init__.py
+-rw-r--r--   0        0        0    46974 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/api.py
+-rw-r--r--   0        0        0    20821 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/marshalling.py
+-rw-r--r--   0        0        0    20051 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/types.py
+-rw-r--r--   0        0        0     3758 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/__init__.py
+-rw-r--r--   0        0        0    33332 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/api.py
+-rw-r--r--   0        0        0      418 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/content.py
+-rw-r--r--   0        0        0    21727 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    15330 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/container/__init__.py
+-rw-r--r--   0        0        0     5100 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/__init__.py
+-rw-r--r--   0        0        0    63615 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/api.py
+-rw-r--r--   0        0        0     1581 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/content.py
+-rw-r--r--   0        0        0    27167 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    27207 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/__init__.py
+-rw-r--r--   0        0        0    19280 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/__init__.py
+-rw-r--r--   0        0        0   138198 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/api.py
+-rw-r--r--   0        0        0     2688 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/content.py
+-rw-r--r--   0        0        0    99051 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/marshalling.py
+-rw-r--r--   0        0        0    74459 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/__init__.py
+-rw-r--r--   0        0        0     9342 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/__init__.py
+-rw-r--r--   0        0        0   103285 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/api.py
+-rw-r--r--   0        0        0     1614 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/content.py
+-rw-r--r--   0        0        0    52204 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    42675 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/__init__.py
+-rw-r--r--   0        0        0    13096 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/__init__.py
+-rw-r--r--   0        0        0    91007 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/api.py
+-rw-r--r--   0        0        0     1948 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/content.py
+-rw-r--r--   0        0        0    90138 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    36143 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    20507 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/api.py
+-rw-r--r--   0        0        0      649 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/content.py
+-rw-r--r--   0        0        0     8075 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8804 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/__init__.py
+-rw-r--r--   0        0        0     5594 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/__init__.py
+-rw-r--r--   0        0        0    65530 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/api.py
+-rw-r--r--   0        0        0     1573 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/content.py
+-rw-r--r--   0        0        0    29502 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    28712 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/__init__.py
+-rw-r--r--   0        0        0     5586 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    84589 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/api.py
+-rw-r--r--   0        0        0    33530 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    30388 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/instance/__init__.py
+-rw-r--r--   0        0        0    13930 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/__init__.py
+-rw-r--r--   0        0        0   151681 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/api.py
+-rw-r--r--   0        0        0     2388 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/content.py
+-rw-r--r--   0        0        0   116222 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/marshalling.py
+-rw-r--r--   0        0        0    65154 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/types.py
+-rw-r--r--   0        0        0     6858 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/types_private.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/__init__.py
+-rw-r--r--   0        0        0     5818 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/__init__.py
+-rw-r--r--   0        0        0    61877 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/api.py
+-rw-r--r--   0        0        0      363 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/content.py
+-rw-r--r--   0        0        0    33920 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/marshalling.py
+-rw-r--r--   0        0        0    29997 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/__init__.py
+-rw-r--r--   0        0        0    13650 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/api.py
+-rw-r--r--   0        0        0     6467 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/marshalling.py
+-rw-r--r--   0        0        0     6550 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/__init__.py
+-rw-r--r--   0        0        0     2572 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    33644 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/api.py
+-rw-r--r--   0        0        0      552 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/content.py
+-rw-r--r--   0        0        0    12468 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    11507 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/__init__.py
+-rw-r--r--   0        0        0     1760 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18492 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/api.py
+-rw-r--r--   0        0        0      402 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/content.py
+-rw-r--r--   0        0        0    11319 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     7454 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/__init__.py
+-rw-r--r--   0        0        0     5436 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/__init__.py
+-rw-r--r--   0        0        0    59478 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/api.py
+-rw-r--r--   0        0        0      934 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/content.py
+-rw-r--r--   0        0        0    40014 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/marshalling.py
+-rw-r--r--   0        0        0    44925 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/__init__.py
+-rw-r--r--   0        0        0    13124 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/__init__.py
+-rw-r--r--   0        0        0   228542 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/api.py
+-rw-r--r--   0        0        0     1107 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/content.py
+-rw-r--r--   0        0        0    82875 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/marshalling.py
+-rw-r--r--   0        0        0    91077 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/__init__.py
+-rw-r--r--   0        0        0     3026 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/__init__.py
+-rw-r--r--   0        0        0    31541 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/api.py
+-rw-r--r--   0        0        0      443 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/content.py
+-rw-r--r--   0        0        0    17687 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    14475 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/__init__.py
+-rw-r--r--   0        0        0     1470 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/__init__.py
+-rw-r--r--   0        0        0    14905 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/api.py
+-rw-r--r--   0        0        0     6721 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/marshalling.py
+-rw-r--r--   0        0        0     5135 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/__init__.py
+-rw-r--r--   0        0        0     3766 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/__init__.py
+-rw-r--r--   0        0        0    42072 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/api.py
+-rw-r--r--   0        0        0    18036 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    16867 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/py.typed
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    42961 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/api.py
+-rw-r--r--   0        0        0      843 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/content.py
+-rw-r--r--   0        0        0    18882 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    19382 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/__init__.py
+-rw-r--r--   0        0        0    10564 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/__init__.py
+-rw-r--r--   0        0        0   119808 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/api.py
+-rw-r--r--   0        0        0     1950 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/content.py
+-rw-r--r--   0        0        0    57699 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/marshalling.py
+-rw-r--r--   0        0        0    48945 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/__init__.py
+-rw-r--r--   0        0        0    44423 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/api.py
+-rw-r--r--   0        0        0      488 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/content.py
+-rw-r--r--   0        0        0    21902 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/marshalling.py
+-rw-r--r--   0        0        0    17769 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/__init__.py
+-rw-r--r--   0        0        0     1962 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/__init__.py
+-rw-r--r--   0        0        0    29203 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/api.py
+-rw-r--r--   0        0        0      710 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/content.py
+-rw-r--r--   0        0        0     8195 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/marshalling.py
+-rw-r--r--   0        0        0    11276 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/__init__.py
+-rw-r--r--   0        0        0     3160 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    51007 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/api.py
+-rw-r--r--   0        0        0    15815 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    21526 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/types.py
+-rw-r--r--   0        0        0     3050 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/__init__.py
+-rw-r--r--   0        0        0    36548 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/api.py
+-rw-r--r--   0        0        0    15383 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    18709 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/__init__.py
+-rw-r--r--   0        0        0     1528 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    19895 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/api.py
+-rw-r--r--   0        0        0      427 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/content.py
+-rw-r--r--   0        0        0     6440 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8013 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/types.py
+-rw-r--r--   0        0        0      194 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/api.py
+-rw-r--r--   0        0        0      129 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/marshalling.py
+-rw-r--r--   0        0        0      469 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/__init__.py
+-rw-r--r--   0        0        0     2646 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    26537 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/api.py
+-rw-r--r--   0        0        0      549 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/content.py
+-rw-r--r--   0        0        0    18141 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    16807 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/__init__.py
+-rw-r--r--   0        0        0     1088 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/__init__.py
+-rw-r--r--   0        0        0    11588 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/api.py
+-rw-r--r--   0        0        0      349 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/content.py
+-rw-r--r--   0        0        0     6231 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/marshalling.py
+-rw-r--r--   0        0        0     3231 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/__init__.py
+-rw-r--r--   0        0        0      818 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/__init__.py
+-rw-r--r--   0        0        0    11732 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/api.py
+-rw-r--r--   0        0        0     3338 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/marshalling.py
+-rw-r--r--   0        0        0     4368 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/types.py
+-rw-r--r--   0        0        0     1932 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/__init__.py
+-rw-r--r--   0        0        0    31050 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/api.py
+-rw-r--r--   0        0        0    10469 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/marshalling.py
+-rw-r--r--   0        0        0    10678 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/__init__.py
+-rw-r--r--   0        0        0     4846 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/__init__.py
+-rw-r--r--   0        0        0    81299 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/api.py
+-rw-r--r--   0        0        0      755 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/content.py
+-rw-r--r--   0        0        0    30617 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/marshalling.py
+-rw-r--r--   0        0        0    35539 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/__init__.py
+-rw-r--r--   0        0        0     2510 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    22954 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/api.py
+-rw-r--r--   0        0        0      421 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/content.py
+-rw-r--r--   0        0        0    14989 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    14450 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/types.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 scaleway-2.2.1/PKG-INFO
```

### Comparing `scaleway-2.1.0/pyproject.toml` & `scaleway-2.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway"
-version = "2.1.0"
+version = "2.2.1"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -20,19 +20,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-scaleway-core = "2.1.0"
+scaleway-core = "2.2.1"
 
 [tool.poetry.group.dev.dependencies]
 scaleway-core = { path = "../scaleway-core", develop = true }
-ruff = ">=0.0.286,<0.3.6"
+ruff = ">=0.0.286,<0.4.3"
 mypy = "^1.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `scaleway-2.1.0/scaleway/__init__.py` & `scaleway-2.2.1/scaleway/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v2/__init__.py` & `scaleway-2.2.1/scaleway/account/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v2/api.py` & `scaleway-2.2.1/scaleway/account/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v2/marshalling.py` & `scaleway-2.2.1/scaleway/account/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v2/types.py` & `scaleway-2.2.1/scaleway/account/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v3/__init__.py` & `scaleway-2.2.1/scaleway/account/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v3/api.py` & `scaleway-2.2.1/scaleway/account/v3/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v3/marshalling.py` & `scaleway-2.2.1/scaleway/account/v3/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/account/v3/types.py` & `scaleway-2.2.1/scaleway/account/v3/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/applesilicon/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 from .types import ListServersRequestOrderBy
 from .types import ServerStatus
 from .content import SERVER_TRANSIENT_STATUSES
 from .types import ServerTypeStock
+from .types import OS
 from .types import ServerTypeCPU
 from .types import ServerTypeDisk
 from .types import ServerTypeMemory
-from .types import OS
 from .types import ServerType
 from .types import Server
 from .types import CreateServerRequest
 from .types import DeleteServerRequest
 from .types import GetOSRequest
 from .types import GetServerRequest
 from .types import GetServerTypeRequest
@@ -27,18 +27,18 @@
 from .api import ApplesiliconV1Alpha1API
 
 __all__ = [
     "ListServersRequestOrderBy",
     "ServerStatus",
     "SERVER_TRANSIENT_STATUSES",
     "ServerTypeStock",
+    "OS",
     "ServerTypeCPU",
     "ServerTypeDisk",
     "ServerTypeMemory",
-    "OS",
     "ServerType",
     "Server",
     "CreateServerRequest",
     "DeleteServerRequest",
     "GetOSRequest",
     "GetServerRequest",
     "GetServerTypeRequest",
```

### Comparing `scaleway-2.1.0/scaleway/applesilicon/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .types import (
     ListServersRequestOrderBy,
     CreateServerRequest,
     ListOSResponse,
     ListServerTypesResponse,
     ListServersResponse,
     OS,
+    ReinstallServerRequest,
     Server,
     ServerType,
     UpdateServerRequest,
 )
 from .content import (
     SERVER_TRANSIENT_STATUSES,
 )
@@ -32,14 +33,15 @@
     unmarshal_OS,
     unmarshal_ServerType,
     unmarshal_Server,
     unmarshal_ListOSResponse,
     unmarshal_ListServerTypesResponse,
     unmarshal_ListServersResponse,
     marshal_CreateServerRequest,
+    marshal_ReinstallServerRequest,
     marshal_UpdateServerRequest,
 )
 
 
 class ApplesiliconV1Alpha1API(API):
     """ """
 
@@ -105,22 +107,24 @@
     def create_server(
         self,
         *,
         type_: str,
         zone: Optional[Zone] = None,
         name: Optional[str] = None,
         project_id: Optional[str] = None,
+        os_id: Optional[str] = None,
     ) -> Server:
         """
         Create a server.
         Create a new server in the targeted zone, specifying its configuration including name and type.
         :param type_: Create a server of the given type.
         :param zone: Zone to target. If none is passed will use default zone from the config.
         :param name: Create a server with this given name.
         :param project_id: Create a server in the given project ID.
+        :param os_id: Create a server & install the given os_id, when no os_id provided the default OS for this server type is chosen. Requesting a non-default OS will induce an extended delivery time.
         :return: :class:`Server <Server>`
 
         Usage:
         ::
 
             result = api.create_server(
                 type="example",
@@ -134,14 +138,15 @@
             f"/apple-silicon/v1alpha1/zones/{param_zone}/servers",
             body=marshal_CreateServerRequest(
                 CreateServerRequest(
                     type_=type_,
                     zone=zone,
                     name=name or random_name(prefix="as"),
                     project_id=project_id,
+                    os_id=os_id,
                 ),
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
         return unmarshal_Server(res.json())
@@ -518,20 +523,22 @@
         return unmarshal_Server(res.json())
 
     def reinstall_server(
         self,
         *,
         server_id: str,
         zone: Optional[Zone] = None,
+        os_id: Optional[str] = None,
     ) -> Server:
         """
         Reinstall a server.
         Reinstall an existing Apple silicon server (specified by its server ID) from a new image (OS). All the data on the disk is deleted and all configuration is reset to the defailt configuration values of the image (OS).
         :param server_id: UUID of the server you want to reinstall.
         :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param os_id: Reinstall the server with the target OS, when no os_id provided the default OS for the server type is used.
         :return: :class:`Server <Server>`
 
         Usage:
         ::
 
             result = api.reinstall_server(
                 server_id="example",
@@ -540,12 +547,19 @@
 
         param_zone = validate_path_param("zone", zone or self.client.default_zone)
         param_server_id = validate_path_param("server_id", server_id)
 
         res = self._request(
             "POST",
             f"/apple-silicon/v1alpha1/zones/{param_zone}/servers/{param_server_id}/reinstall",
-            body={},
+            body=marshal_ReinstallServerRequest(
+                ReinstallServerRequest(
+                    server_id=server_id,
+                    zone=zone,
+                    os_id=os_id,
+                ),
+                self.client,
+            ),
         )
 
         self._throw_on_error(res)
         return unmarshal_Server(res.json())
```

### Comparing `scaleway-2.1.0/scaleway/applesilicon/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/marshalling.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     ServerTypeMemory,
     ServerType,
     Server,
     ListOSResponse,
     ListServerTypesResponse,
     ListServersResponse,
     CreateServerRequest,
+    ReinstallServerRequest,
     UpdateServerRequest,
 )
 
 
 def unmarshal_OS(data: Any) -> OS:
     if not isinstance(data, dict):
         raise TypeError(
@@ -40,14 +41,30 @@
     if field is not None:
         args["label"] = field
 
     field = data.get("image_url", None)
     if field is not None:
         args["image_url"] = field
 
+    field = data.get("family", None)
+    if field is not None:
+        args["family"] = field
+
+    field = data.get("is_beta", None)
+    if field is not None:
+        args["is_beta"] = field
+
+    field = data.get("version", None)
+    if field is not None:
+        args["version"] = field
+
+    field = data.get("xcode_version", None)
+    if field is not None:
+        args["xcode_version"] = field
+
     field = data.get("compatible_server_types", None)
     if field is not None:
         args["compatible_server_types"] = field
 
     return OS(**args)
 
 
@@ -144,14 +161,20 @@
 
     field = data.get("minimum_lease_duration", None)
     if field is not None:
         args["minimum_lease_duration"] = field
     else:
         args["minimum_lease_duration"] = None
 
+    field = data.get("default_os", None)
+    if field is not None:
+        args["default_os"] = unmarshal_OS(field)
+    else:
+        args["default_os"] = None
+
     return ServerType(**args)
 
 
 def unmarshal_Server(data: Any) -> Server:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Server' failed as data isn't a dictionary."
@@ -191,14 +214,20 @@
     if field is not None:
         args["status"] = field
 
     field = data.get("zone", None)
     if field is not None:
         args["zone"] = field
 
+    field = data.get("os", None)
+    if field is not None:
+        args["os"] = unmarshal_OS(field)
+    else:
+        args["os"] = None
+
     field = data.get("created_at", None)
     if field is not None:
         args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
     else:
         args["created_at"] = None
 
     field = data.get("updated_at", None)
@@ -286,14 +315,29 @@
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.project_id is not None:
         output["project_id"] = request.project_id or defaults.default_project_id
 
+    if request.os_id is not None:
+        output["os_id"] = request.os_id
+
+    return output
+
+
+def marshal_ReinstallServerRequest(
+    request: ReinstallServerRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
+
+    if request.os_id is not None:
+        output["os_id"] = request.os_id
+
     return output
 
 
 def marshal_UpdateServerRequest(
     request: UpdateServerRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
```

### Comparing `scaleway-2.1.0/scaleway/applesilicon/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,35 +46,14 @@
     HIGH_STOCK = "high_stock"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 @dataclass
-class ServerTypeCPU:
-    name: str
-
-    core_count: int
-
-
-@dataclass
-class ServerTypeDisk:
-    capacity: int
-
-    type_: str
-
-
-@dataclass
-class ServerTypeMemory:
-    capacity: int
-
-    type_: str
-
-
-@dataclass
 class OS:
     id: str
     """
     Unique ID of the OS.
     """
 
     name: str
@@ -88,21 +67,62 @@
     """
 
     image_url: str
     """
     URL of the image.
     """
 
+    family: str
+    """
+    The OS family to which this OS belongs, eg. 13 or 14.
+    """
+
+    is_beta: bool
+    """
+    Describes if the OS is in beta.
+    """
+
+    version: str
+    """
+    The OS version number, eg. Sonoma has version number 14.3.
+    """
+
+    xcode_version: str
+    """
+    The current xcode version for this OS.
+    """
+
     compatible_server_types: List[str]
     """
     List of compatible server types.
     """
 
 
 @dataclass
+class ServerTypeCPU:
+    name: str
+
+    core_count: int
+
+
+@dataclass
+class ServerTypeDisk:
+    capacity: int
+
+    type_: str
+
+
+@dataclass
+class ServerTypeMemory:
+    capacity: int
+
+    type_: str
+
+
+@dataclass
 class ServerType:
     name: str
     """
     Name of the type.
     """
 
     stock: ServerTypeStock
@@ -126,14 +146,19 @@
     """
 
     minimum_lease_duration: Optional[str]
     """
     Minimum duration of the lease in seconds (example. 3.4s).
     """
 
+    default_os: Optional[OS]
+    """
+    The default OS for this server type.
+    """
+
 
 @dataclass
 class Server:
     id: str
     """
     UUID of the server.
     """
@@ -174,14 +199,19 @@
     """
 
     zone: Zone
     """
     Zone of the server.
     """
 
+    os: Optional[OS]
+    """
+    Initially installed OS, this does not necessarily reflect the current OS version.
+    """
+
     created_at: Optional[datetime]
     """
     Date on which the server was created.
     """
 
     updated_at: Optional[datetime]
     """
@@ -212,14 +242,19 @@
     """
 
     project_id: Optional[str]
     """
     Create a server in the given project ID.
     """
 
+    os_id: Optional[str]
+    """
+    Create a server & install the given os_id, when no os_id provided the default OS for this server type is chosen. Requesting a non-default OS will induce an extended delivery time.
+    """
+
 
 @dataclass
 class DeleteServerRequest:
     server_id: str
     """
     UUID of the server you want to delete.
     """
@@ -393,14 +428,19 @@
     """
 
     zone: Optional[Zone]
     """
     Zone to target. If none is passed will use default zone from the config.
     """
 
+    os_id: Optional[str]
+    """
+    Reinstall the server with the target OS, when no os_id provided the default OS for the server type is used.
+    """
+
 
 @dataclass
 class UpdateServerRequest:
     server_id: str
     """
     UUID of the server you want to update.
     """
```

### Comparing `scaleway-2.1.0/scaleway/baremetal/v1/__init__.py` & `scaleway-2.2.1/scaleway/baremetal/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/baremetal/v1/api.py` & `scaleway-2.2.1/scaleway/baremetal/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/baremetal/v1/content.py` & `scaleway-2.2.1/scaleway/baremetal/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/baremetal/v1/marshalling.py` & `scaleway-2.2.1/scaleway/baremetal/v1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1072,16 +1072,16 @@
     if request.description is not None:
         output["description"] = request.description
 
     if request.tags is not None:
         output["tags"] = request.tags
 
     if request.install is not None:
-        output["install"] = (
-            marshal_CreateServerRequestInstall(request.install, defaults),
+        output["install"] = marshal_CreateServerRequestInstall(
+            request.install, defaults
         )
 
     if request.option_ids is not None:
         output["option_ids"] = request.option_ids
 
     return output
```

### Comparing `scaleway-2.1.0/scaleway/baremetal/v1/types.py` & `scaleway-2.2.1/scaleway/baremetal/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2alpha1/__init__.py` & `scaleway-2.2.1/scaleway/billing/v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2alpha1/api.py` & `scaleway-2.2.1/scaleway/billing/v2alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/billing/v2alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2alpha1/types.py` & `scaleway-2.2.1/scaleway/billing/v2alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2beta1/__init__.py` & `scaleway-2.2.1/scaleway/billing/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2beta1/api.py` & `scaleway-2.2.1/scaleway/billing/v2beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2beta1/marshalling.py` & `scaleway-2.2.1/scaleway/billing/v2beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/billing/v2beta1/types.py` & `scaleway-2.2.1/scaleway/billing/v2beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/block/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/block/v1alpha1/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .types import Volume
 from .types import CreateSnapshotRequest
 from .types import CreateVolumeRequest
 from .types import DeleteSnapshotRequest
 from .types import DeleteVolumeRequest
 from .types import GetSnapshotRequest
 from .types import GetVolumeRequest
+from .types import ImportSnapshotFromS3Request
 from .types import ListSnapshotsRequest
 from .types import ListSnapshotsResponse
 from .types import ListVolumeTypesRequest
 from .types import ListVolumeTypesResponse
 from .types import ListVolumesRequest
 from .types import ListVolumesResponse
 from .types import UpdateSnapshotRequest
@@ -55,14 +56,15 @@
     "Volume",
     "CreateSnapshotRequest",
     "CreateVolumeRequest",
     "DeleteSnapshotRequest",
     "DeleteVolumeRequest",
     "GetSnapshotRequest",
     "GetVolumeRequest",
+    "ImportSnapshotFromS3Request",
     "ListSnapshotsRequest",
     "ListSnapshotsResponse",
     "ListVolumeTypesRequest",
     "ListVolumeTypesResponse",
     "ListVolumesRequest",
     "ListVolumesResponse",
     "UpdateSnapshotRequest",
```

### Comparing `scaleway-2.1.0/scaleway/block/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/block/v1alpha1/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .types import (
     ListSnapshotsRequestOrderBy,
     ListVolumesRequestOrderBy,
     CreateSnapshotRequest,
     CreateVolumeRequest,
     CreateVolumeRequestFromEmpty,
     CreateVolumeRequestFromSnapshot,
+    ImportSnapshotFromS3Request,
     ListSnapshotsResponse,
     ListVolumeTypesResponse,
     ListVolumesResponse,
     Snapshot,
     UpdateSnapshotRequest,
     UpdateVolumeRequest,
     Volume,
@@ -37,14 +38,15 @@
     unmarshal_Snapshot,
     unmarshal_Volume,
     unmarshal_ListSnapshotsResponse,
     unmarshal_ListVolumeTypesResponse,
     unmarshal_ListVolumesResponse,
     marshal_CreateSnapshotRequest,
     marshal_CreateVolumeRequest,
+    marshal_ImportSnapshotFromS3Request,
     marshal_UpdateSnapshotRequest,
     marshal_UpdateVolumeRequest,
 )
 
 
 class BlockV1Alpha1API(API):
     """
@@ -636,14 +638,70 @@
                 ),
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
         return unmarshal_Snapshot(res.json())
+
+    def import_snapshot_from_s3(
+        self,
+        *,
+        bucket: str,
+        key: str,
+        name: str,
+        zone: Optional[Zone] = None,
+        project_id: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        size: Optional[int] = None,
+    ) -> Snapshot:
+        """
+        Import a snapshot from a Scaleway Object Storage bucket.
+        The bucket must contain a QCOW2 image.
+        The bucket can be imported into any Availability Zone as long as it is in the same region as the bucket.
+        :param bucket: Scaleway Object Storage bucket where the object is stored.
+        :param key: The object key inside the given bucket.
+        :param name: Name of the snapshot.
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :param project_id: UUID of the Project to which the volume and the snapshot belong.
+        :param tags: List of tags assigned to the snapshot.
+        :param size: Size of the snapshot.
+        :return: :class:`Snapshot <Snapshot>`
+
+        Usage:
+        ::
+
+            result = api.import_snapshot_from_s3(
+                bucket="example",
+                key="example",
+                name="example",
+            )
+        """
+
+        param_zone = validate_path_param("zone", zone or self.client.default_zone)
+
+        res = self._request(
+            "POST",
+            f"/block/v1alpha1/zones/{param_zone}/snapshots/import-from-s3",
+            body=marshal_ImportSnapshotFromS3Request(
+                ImportSnapshotFromS3Request(
+                    bucket=bucket,
+                    key=key,
+                    name=name,
+                    zone=zone,
+                    project_id=project_id,
+                    tags=tags,
+                    size=size,
+                ),
+                self.client,
+            ),
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_Snapshot(res.json())
 
     def delete_snapshot(
         self,
         *,
         snapshot_id: str,
         zone: Optional[Zone] = None,
     ) -> None:
```

### Comparing `scaleway-2.1.0/scaleway/block/v1alpha1/content.py` & `scaleway-2.2.1/scaleway/block/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/block/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/block/v1alpha1/marshalling.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     VolumeType,
     ListVolumeTypesResponse,
     ListVolumesResponse,
     CreateSnapshotRequest,
     CreateVolumeRequestFromEmpty,
     CreateVolumeRequestFromSnapshot,
     CreateVolumeRequest,
+    ImportSnapshotFromS3Request,
     UpdateSnapshotRequest,
     UpdateVolumeRequest,
 )
 
 
 def unmarshal_Reference(data: Any) -> Reference:
     if not isinstance(data, dict):
@@ -437,14 +438,41 @@
 
     if request.tags is not None:
         output["tags"] = request.tags
 
     return output
 
 
+def marshal_ImportSnapshotFromS3Request(
+    request: ImportSnapshotFromS3Request,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
+
+    if request.bucket is not None:
+        output["bucket"] = request.bucket
+
+    if request.key is not None:
+        output["key"] = request.key
+
+    if request.name is not None:
+        output["name"] = request.name
+
+    if request.project_id is not None:
+        output["project_id"] = request.project_id or defaults.default_project_id
+
+    if request.tags is not None:
+        output["tags"] = request.tags
+
+    if request.size is not None:
+        output["size"] = request.size
+
+    return output
+
+
 def marshal_UpdateSnapshotRequest(
     request: UpdateSnapshotRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
```

### Comparing `scaleway-2.1.0/scaleway/block/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/block/v1alpha1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     type_: ReferenceType
     """
     Type of reference (link, exclusive, read_only).
     """
 
     status: ReferenceStatus
     """
-    Status of reference (attaching, attached, detaching).
+    Status of the reference. Statuses include `attaching`, `attached`, and `detaching`.
     """
 
     created_at: Optional[datetime]
     """
     Creation date of the reference.
     """
 
@@ -455,14 +455,52 @@
     zone: Optional[Zone]
     """
     Zone to target. If none is passed will use default zone from the config.
     """
 
 
 @dataclass
+class ImportSnapshotFromS3Request:
+    bucket: str
+    """
+    Scaleway Object Storage bucket where the object is stored.
+    """
+
+    key: str
+    """
+    The object key inside the given bucket.
+    """
+
+    name: str
+    """
+    Name of the snapshot.
+    """
+
+    zone: Optional[Zone]
+    """
+    Zone to target. If none is passed will use default zone from the config.
+    """
+
+    project_id: Optional[str]
+    """
+    UUID of the Project to which the volume and the snapshot belong.
+    """
+
+    tags: Optional[List[str]]
+    """
+    List of tags assigned to the snapshot.
+    """
+
+    size: Optional[int]
+    """
+    Size of the snapshot.
+    """
+
+
+@dataclass
 class ListSnapshotsRequest:
     zone: Optional[Zone]
     """
     Zone to target. If none is passed will use default zone from the config.
     """
 
     order_by: Optional[ListSnapshotsRequestOrderBy]
```

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1/__init__.py` & `scaleway-2.2.1/scaleway/cockpit/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1/api.py` & `scaleway-2.2.1/scaleway/cockpit/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1/marshalling.py` & `scaleway-2.2.1/scaleway/cockpit/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1/types.py` & `scaleway-2.2.1/scaleway/cockpit/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1beta1/__init__.py` & `scaleway-2.2.1/scaleway/cockpit/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1beta1/api.py` & `scaleway-2.2.1/scaleway/cockpit/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1beta1/marshalling.py` & `scaleway-2.2.1/scaleway/cockpit/v1beta1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,17 +611,15 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.project_id is not None:
         output["project_id"] = request.project_id or defaults.default_project_id
 
     if request.contact_point is not None:
-        output["contact_point"] = (
-            marshal_ContactPoint(request.contact_point, defaults),
-        )
+        output["contact_point"] = marshal_ContactPoint(request.contact_point, defaults)
 
     return output
 
 
 def marshal_CreateDatasourceRequest(
     request: CreateDatasourceRequest,
     defaults: ProfileDefaults,
@@ -706,15 +704,15 @@
     if request.project_id is not None:
         output["project_id"] = request.project_id or defaults.default_project_id
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.scopes is not None:
-        output["scopes"] = (marshal_TokenScopes(request.scopes, defaults),)
+        output["scopes"] = marshal_TokenScopes(request.scopes, defaults)
 
     return output
 
 
 def marshal_DeactivateCockpitRequest(
     request: DeactivateCockpitRequest,
     defaults: ProfileDefaults,
@@ -733,17 +731,15 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.project_id is not None:
         output["project_id"] = request.project_id or defaults.default_project_id
 
     if request.contact_point is not None:
-        output["contact_point"] = (
-            marshal_ContactPoint(request.contact_point, defaults),
-        )
+        output["contact_point"] = marshal_ContactPoint(request.contact_point, defaults)
 
     return output
 
 
 def marshal_DeleteGrafanaUserRequest(
     request: DeleteGrafanaUserRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.1.0/scaleway/cockpit/v1beta1/types.py` & `scaleway-2.2.1/scaleway/cockpit/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/container/v1beta1/__init__.py` & `scaleway-2.2.1/scaleway/container/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/container/v1beta1/api.py` & `scaleway-2.2.1/scaleway/container/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/container/v1beta1/content.py` & `scaleway-2.2.1/scaleway/container/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/container/v1beta1/marshalling.py` & `scaleway-2.2.1/scaleway/container/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/container/v1beta1/types.py` & `scaleway-2.2.1/scaleway/container/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/dedibox/v1/__init__.py` & `scaleway-2.2.1/scaleway/dedibox/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/dedibox/v1/api.py` & `scaleway-2.2.1/scaleway/dedibox/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/dedibox/v1/content.py` & `scaleway-2.2.1/scaleway/dedibox/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/dedibox/v1/marshalling.py` & `scaleway-2.2.1/scaleway/dedibox/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/dedibox/v1/types.py` & `scaleway-2.2.1/scaleway/dedibox/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/document_db/v1beta1/__init__.py` & `scaleway-2.2.1/scaleway/document_db/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/document_db/v1beta1/api.py` & `scaleway-2.2.1/scaleway/document_db/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/document_db/v1beta1/content.py` & `scaleway-2.2.1/scaleway/document_db/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/document_db/v1beta1/marshalling.py` & `scaleway-2.2.1/scaleway/document_db/v1beta1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1520,17 +1520,15 @@
 def marshal_CreateEndpointRequest(
     request: CreateEndpointRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.endpoint_spec is not None:
-        output["endpoint_spec"] = (
-            marshal_EndpointSpec(request.endpoint_spec, defaults),
-        )
+        output["endpoint_spec"] = marshal_EndpointSpec(request.endpoint_spec, defaults)
 
     return output
 
 
 def marshal_CreateInstanceFromSnapshotRequest(
     request: CreateInstanceFromSnapshotRequest,
     defaults: ProfileDefaults,
@@ -1866,15 +1864,15 @@
     if request.name is not None:
         output["name"] = request.name
 
     if request.tags is not None:
         output["tags"] = request.tags
 
     if request.logs_policy is not None:
-        output["logs_policy"] = (marshal_LogsPolicy(request.logs_policy, defaults),)
+        output["logs_policy"] = marshal_LogsPolicy(request.logs_policy, defaults)
 
     if request.backup_same_region is not None:
         output["backup_same_region"] = request.backup_same_region
 
     if request.backup_schedule_start_hour is not None:
         output["backup_schedule_start_hour"] = request.backup_schedule_start_hour
```

### Comparing `scaleway-2.1.0/scaleway/document_db/v1beta1/types.py` & `scaleway-2.2.1/scaleway/document_db/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/domain/v2beta1/__init__.py` & `scaleway-2.2.1/scaleway/domain/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/domain/v2beta1/api.py` & `scaleway-2.2.1/scaleway/domain/v2beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/domain/v2beta1/content.py` & `scaleway-2.2.1/scaleway/domain/v2beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/domain/v2beta1/marshalling.py` & `scaleway-2.2.1/scaleway/domain/v2beta1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -2283,16 +2283,16 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name_server is not None:
         output["name_server"] = request.name_server
 
     if request.tsig_key is not None:
-        output["tsig_key"] = (
-            marshal_ImportRawDNSZoneRequestTsigKey(request.tsig_key, defaults),
+        output["tsig_key"] = marshal_ImportRawDNSZoneRequestTsigKey(
+            request.tsig_key, defaults
         )
 
     return output
 
 
 def marshal_ImportRawDNSZoneRequestBindSource(
     request: ImportRawDNSZoneRequestBindSource,
@@ -2542,29 +2542,29 @@
 
     if request.questions is not None:
         output["questions"] = [
             marshal_ContactQuestion(item, defaults) for item in request.questions
         ]
 
     if request.extension_fr is not None:
-        output["extension_fr"] = (
-            marshal_ContactExtensionFR(request.extension_fr, defaults),
+        output["extension_fr"] = marshal_ContactExtensionFR(
+            request.extension_fr, defaults
         )
 
     if request.extension_eu is not None:
-        output["extension_eu"] = (
-            marshal_ContactExtensionEU(request.extension_eu, defaults),
+        output["extension_eu"] = marshal_ContactExtensionEU(
+            request.extension_eu, defaults
         )
 
     if request.state is not None:
         output["state"] = request.state
 
     if request.extension_nl is not None:
-        output["extension_nl"] = (
-            marshal_ContactExtensionNL(request.extension_nl, defaults),
+        output["extension_nl"] = marshal_ContactExtensionNL(
+            request.extension_nl, defaults
         )
 
     return output
 
 
 def marshal_RegistrarApiBuyDomainsRequest(
     request: RegistrarApiBuyDomainsRequest,
@@ -2691,17 +2691,15 @@
     if request.type_ is not None:
         output["type"] = str(request.type_)
 
     if request.digest is not None:
         output["digest"] = request.digest
 
     if request.public_key is not None:
-        output["public_key"] = (
-            marshal_DSRecordPublicKey(request.public_key, defaults),
-        )
+        output["public_key"] = marshal_DSRecordPublicKey(request.public_key, defaults)
 
     return output
 
 
 def marshal_DSRecord(
     request: DSRecord,
     defaults: ProfileDefaults,
@@ -2728,15 +2726,15 @@
 def marshal_RegistrarApiEnableDomainDNSSECRequest(
     request: RegistrarApiEnableDomainDNSSECRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.ds_record is not None:
-        output["ds_record"] = (marshal_DSRecord(request.ds_record, defaults),)
+        output["ds_record"] = marshal_DSRecord(request.ds_record, defaults)
 
     return output
 
 
 def marshal_RegistrarApiRegisterExternalDomainRequest(
     request: RegistrarApiRegisterExternalDomainRequest,
     defaults: ProfileDefaults,
@@ -2914,32 +2912,32 @@
     if request.questions is not None:
         output["questions"] = [
             marshal_UpdateContactRequestQuestion(item, defaults)
             for item in request.questions
         ]
 
     if request.extension_fr is not None:
-        output["extension_fr"] = (
-            marshal_ContactExtensionFR(request.extension_fr, defaults),
+        output["extension_fr"] = marshal_ContactExtensionFR(
+            request.extension_fr, defaults
         )
 
     if request.extension_eu is not None:
-        output["extension_eu"] = (
-            marshal_ContactExtensionEU(request.extension_eu, defaults),
+        output["extension_eu"] = marshal_ContactExtensionEU(
+            request.extension_eu, defaults
         )
 
     if request.whois_opt_in is not None:
         output["whois_opt_in"] = request.whois_opt_in
 
     if request.state is not None:
         output["state"] = request.state
 
     if request.extension_nl is not None:
-        output["extension_nl"] = (
-            marshal_ContactExtensionNL(request.extension_nl, defaults),
+        output["extension_nl"] = marshal_ContactExtensionNL(
+            request.extension_nl, defaults
         )
 
     return output
 
 
 def marshal_RegistrarApiUpdateDomainHostRequest(
     request: RegistrarApiUpdateDomainHostRequest,
```

### Comparing `scaleway-2.1.0/scaleway/domain/v2beta1/types.py` & `scaleway-2.2.1/scaleway/domain/v2beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/flexibleip/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/flexibleip/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/flexibleip/v1alpha1/content.py` & `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/flexibleip/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/flexibleip/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/function/v1beta1/__init__.py` & `scaleway-2.2.1/scaleway/function/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/function/v1beta1/api.py` & `scaleway-2.2.1/scaleway/function/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/function/v1beta1/content.py` & `scaleway-2.2.1/scaleway/function/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/function/v1beta1/marshalling.py` & `scaleway-2.2.1/scaleway/function/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/function/v1beta1/types.py` & `scaleway-2.2.1/scaleway/function/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/iam/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/iam/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/iam/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/iam/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/iam/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/iam/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/iam/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/iam/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/instance/v1/__init__.py` & `scaleway-2.2.1/scaleway/instance/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/instance/v1/api.py` & `scaleway-2.2.1/scaleway/instance/v1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4090,15 +4090,15 @@
         *,
         zone: Optional[Zone] = None,
         volume_id: Optional[str] = None,
         snapshot_id: Optional[str] = None,
     ) -> MigrationPlan:
         """
         Get a volume or snapshot's migration plan.
-        Given a volume or snapshot, returns the migration plan for a call to the RPC ApplyBlockMigration. This plan will include zero or one volume, and zero or more snapshots, which will need to be migrated together. This RPC does not perform the actual migration itself, ApplyBlockMigration must be used. The validation_key value returned by this call must be provided to the ApplyBlockMigration call to confirm that all resources listed in the plan should be migrated.
+        Given a volume or snapshot, returns the migration plan for a call to the "Apply a migration plan" endpoint. This plan will include zero or one volume, and zero or more snapshots, which will need to be migrated together. This endpoint does not perform the actual migration itself, the "Apply a migration plan" endpoint must be used. The validation_key value returned by this endpoint must be provided to the call to the "Apply a migration plan" endpoint to confirm that all resources listed in the plan should be migrated.
         :param zone: Zone to target. If none is passed will use default zone from the config.
         :param volume_id: The volume for which the migration plan will be generated.
         One-Of ('resource'): at most one of 'volume_id', 'snapshot_id' could be set.
         :param snapshot_id: The snapshot for which the migration plan will be generated.
         One-Of ('resource'): at most one of 'volume_id', 'snapshot_id' could be set.
         :return: :class:`MigrationPlan <MigrationPlan>`
 
@@ -4132,20 +4132,20 @@
         validation_key: str,
         zone: Optional[Zone] = None,
         volume_id: Optional[str] = None,
         snapshot_id: Optional[str] = None,
     ) -> None:
         """
         Migrate a volume and/or snapshots to SBS (Scaleway Block Storage).
-        To be used, this RPC must be preceded by a call to PlanBlockMigration. To migrate all resources mentioned in the MigrationPlan, the validation_key returned in the MigrationPlan must be provided.
-        :param validation_key: A value to be retrieved from a call to PlanBlockMigration, to confirm that the volume and/or snapshots specified in said plan should be migrated.
+        To be used, the call to this endpoint must be preceded by a call to the "Plan a migration" endpoint. To migrate all resources mentioned in the migration plan, the validation_key returned in the plan must be provided.
+        :param validation_key: A value to be retrieved from a call to the "Plan a migration" endpoint, to confirm that the volume and/or snapshots specified in said plan should be migrated.
         :param zone: Zone to target. If none is passed will use default zone from the config.
-        :param volume_id: The volume to migrate, along with potentially other resources, according to the migration plan generated with a call to PlanBlockMigration.
+        :param volume_id: The volume to migrate, along with potentially other resources, according to the migration plan generated with a call to the "Plan a migration" endpoint.
         One-Of ('resource'): at most one of 'volume_id', 'snapshot_id' could be set.
-        :param snapshot_id: The snapshot to migrate, along with potentially other resources, according to the migration plan generated with a call to PlanBlockMigration.
+        :param snapshot_id: The snapshot to migrate, along with potentially other resources, according to the migration plan generated with a call to the "Plan a migration" endpoint.
         One-Of ('resource'): at most one of 'volume_id', 'snapshot_id' could be set.
 
         Usage:
         ::
 
             result = api.apply_block_migration(
                 validation_key="example",
```

### Comparing `scaleway-2.1.0/scaleway/instance/v1/content.py` & `scaleway-2.2.1/scaleway/instance/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/instance/v1/marshalling.py` & `scaleway-2.2.1/scaleway/instance/v1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -3356,15 +3356,15 @@
     if request.state is not None:
         output["state"] = str(request.state)
 
     if request.zone is not None:
         output["zone"] = request.zone or defaults.default_zone
 
     if request.server is not None:
-        output["server"] = (marshal_ServerSummary(request.server, defaults),)
+        output["server"] = marshal_ServerSummary(request.server, defaults)
 
     return output
 
 
 def marshal_VolumeSummary(
     request: VolumeSummary,
     defaults: ProfileDefaults,
@@ -3407,31 +3407,31 @@
     if request.from_server is not None:
         output["from_server"] = request.from_server
 
     if request.public is not None:
         output["public"] = request.public
 
     if request.default_bootscript is not None:
-        output["default_bootscript"] = (
-            marshal_Bootscript(request.default_bootscript, defaults),
+        output["default_bootscript"] = marshal_Bootscript(
+            request.default_bootscript, defaults
         )
 
     if request.extra_volumes is not None:
         output["extra_volumes"] = {
             key: marshal_Volume(value, defaults)
             for key, value in request.extra_volumes.items()
         }
 
     if request.organization is not None:
         output["organization"] = (
             request.organization or defaults.default_organization_id
         )
 
     if request.root_volume is not None:
-        output["root_volume"] = (marshal_VolumeSummary(request.root_volume, defaults),)
+        output["root_volume"] = marshal_VolumeSummary(request.root_volume, defaults)
 
     if request.state is not None:
         output["state"] = str(request.state)
 
     if request.project is not None:
         output["project"] = request.project or defaults.default_project_id
 
@@ -3758,16 +3758,16 @@
     if request.enable_ipv6 is not None:
         output["enable_ipv6"] = request.enable_ipv6
 
     if request.protected is not None:
         output["protected"] = request.protected
 
     if request.security_group is not None:
-        output["security_group"] = (
-            marshal_SecurityGroupTemplate(request.security_group, defaults),
+        output["security_group"] = marshal_SecurityGroupTemplate(
+            request.security_group, defaults
         )
 
     if request.placement_group is not None:
         output["placement_group"] = request.placement_group
 
     if request.private_nics is not None:
         output["private_nics"] = request.private_nics
@@ -3934,16 +3934,16 @@
     if request.creation_date is not None:
         output["creation_date"] = request.creation_date
 
     if request.modification_date is not None:
         output["modification_date"] = request.modification_date
 
     if request.default_bootscript is not None:
-        output["default_bootscript"] = (
-            marshal_Bootscript(request.default_bootscript, defaults),
+        output["default_bootscript"] = marshal_Bootscript(
+            request.default_bootscript, defaults
         )
 
     if request.public is not None:
         output["public"] = request.public
 
     if request.state is not None:
         output["state"] = str(request.state)
@@ -3954,15 +3954,15 @@
     if request.tags is not None:
         output["tags"] = request.tags
 
     if request.zone is not None:
         output["zone"] = request.zone or defaults.default_zone
 
     if request.root_volume is not None:
-        output["root_volume"] = (marshal_VolumeSummary(request.root_volume, defaults),)
+        output["root_volume"] = marshal_VolumeSummary(request.root_volume, defaults)
 
     return output
 
 
 def marshal_PlacementGroup(
     request: PlacementGroup,
     defaults: ProfileDefaults,
@@ -4177,24 +4177,24 @@
     if request.routed_ip_enabled is not None:
         output["routed_ip_enabled"] = request.routed_ip_enabled
 
     if request.enable_ipv6 is not None:
         output["enable_ipv6"] = request.enable_ipv6
 
     if request.image is not None:
-        output["image"] = (marshal_Image(request.image, defaults),)
+        output["image"] = marshal_Image(request.image, defaults)
 
     if request.protected is not None:
         output["protected"] = request.protected
 
     if request.private_ip is not None:
         output["private_ip"] = request.private_ip
 
     if request.public_ip is not None:
-        output["public_ip"] = (marshal_ServerIp(request.public_ip, defaults),)
+        output["public_ip"] = marshal_ServerIp(request.public_ip, defaults)
 
     if request.public_ips is not None:
         output["public_ips"] = [
             marshal_ServerIp(item, defaults) for item in request.public_ips
         ]
 
     if request.modification_date is not None:
@@ -4203,47 +4203,47 @@
     if request.state_detail is not None:
         output["state_detail"] = request.state_detail
 
     if request.state is not None:
         output["state"] = str(request.state)
 
     if request.location is not None:
-        output["location"] = (marshal_ServerLocation(request.location, defaults),)
+        output["location"] = marshal_ServerLocation(request.location, defaults)
 
     if request.ipv6 is not None:
-        output["ipv6"] = (marshal_ServerIpv6(request.ipv6, defaults),)
+        output["ipv6"] = marshal_ServerIpv6(request.ipv6, defaults)
 
     if request.bootscript is not None:
-        output["bootscript"] = (marshal_Bootscript(request.bootscript, defaults),)
+        output["bootscript"] = marshal_Bootscript(request.bootscript, defaults)
 
     if request.boot_type is not None:
         output["boot_type"] = str(request.boot_type)
 
     if request.volumes is not None:
         output["volumes"] = {
             key: marshal_Volume(value, defaults)
             for key, value in request.volumes.items()
         }
 
     if request.security_group is not None:
-        output["security_group"] = (
-            marshal_SecurityGroupSummary(request.security_group, defaults),
+        output["security_group"] = marshal_SecurityGroupSummary(
+            request.security_group, defaults
         )
 
     if request.maintenances is not None:
         output["maintenances"] = [
             marshal_ServerMaintenance(item, defaults) for item in request.maintenances
         ]
 
     if request.arch is not None:
         output["arch"] = str(request.arch)
 
     if request.placement_group is not None:
-        output["placement_group"] = (
-            marshal_PlacementGroup(request.placement_group, defaults),
+        output["placement_group"] = marshal_PlacementGroup(
+            request.placement_group, defaults
         )
 
     if request.private_nics is not None:
         output["private_nics"] = [
             marshal_PrivateNIC(item, defaults) for item in request.private_nics
         ]
 
@@ -4288,16 +4288,16 @@
     if request.size is not None:
         output["size"] = request.size
 
     if request.state is not None:
         output["state"] = str(request.state)
 
     if request.base_volume is not None:
-        output["base_volume"] = (
-            marshal_SnapshotBaseVolume(request.base_volume, defaults),
+        output["base_volume"] = marshal_SnapshotBaseVolume(
+            request.base_volume, defaults
         )
 
     if request.creation_date is not None:
         output["creation_date"] = request.creation_date
 
     if request.modification_date is not None:
         output["modification_date"] = request.modification_date
```

### Comparing `scaleway-2.1.0/scaleway/instance/v1/types.py` & `scaleway-2.2.1/scaleway/instance/v1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1487,15 +1487,15 @@
     name: str
 
 
 @dataclass
 class ApplyBlockMigrationRequest:
     validation_key: str
     """
-    A value to be retrieved from a call to PlanBlockMigration, to confirm that the volume and/or snapshots specified in said plan should be migrated.
+    A value to be retrieved from a call to the "Plan a migration" endpoint, to confirm that the volume and/or snapshots specified in said plan should be migrated.
     """
 
     zone: Optional[Zone]
     """
     Zone to target. If none is passed will use default zone from the config.
     """
 
@@ -3000,15 +3000,15 @@
     snapshots: List[Snapshot]
     """
     A list of snapshots which will be migrated to SBS together and with the volume, if present.
     """
 
     validation_key: str
     """
-    A value to be passed to ApplyBlockMigrationRequest, to confirm that the execution of the plan is being requested.
+    A value to be passed to the call to the "Apply a migration plan" endpoint, to confirm that the execution of the plan is being requested.
     """
 
     volume: Optional[Volume]
     """
     A volume which will be migrated to SBS together with the snapshots, if present.
     """
```

### Comparing `scaleway-2.1.0/scaleway/instance/v1/types_private.py` & `scaleway-2.2.1/scaleway/instance/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/iot/v1/__init__.py` & `scaleway-2.2.1/scaleway/iot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/iot/v1/api.py` & `scaleway-2.2.1/scaleway/iot/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/iot/v1/marshalling.py` & `scaleway-2.2.1/scaleway/iot/v1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,21 +859,19 @@
 def marshal_DeviceMessageFilters(
     request: DeviceMessageFilters,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.publish is not None:
-        output["publish"] = (
-            marshal_DeviceMessageFiltersRule(request.publish, defaults),
-        )
+        output["publish"] = marshal_DeviceMessageFiltersRule(request.publish, defaults)
 
     if request.subscribe is not None:
-        output["subscribe"] = (
-            marshal_DeviceMessageFiltersRule(request.subscribe, defaults),
+        output["subscribe"] = marshal_DeviceMessageFiltersRule(
+            request.subscribe, defaults
         )
 
     return output
 
 
 def marshal_CreateDeviceRequest(
     request: CreateDeviceRequest,
@@ -890,16 +888,16 @@
     if request.allow_multiple_connections is not None:
         output["allow_multiple_connections"] = request.allow_multiple_connections
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.message_filters is not None:
-        output["message_filters"] = (
-            marshal_DeviceMessageFilters(request.message_filters, defaults),
+        output["message_filters"] = marshal_DeviceMessageFilters(
+            request.message_filters, defaults
         )
 
     if request.description is not None:
         output["description"] = request.description
 
     return output
 
@@ -1135,16 +1133,16 @@
     if request.allow_insecure is not None:
         output["allow_insecure"] = request.allow_insecure
 
     if request.allow_multiple_connections is not None:
         output["allow_multiple_connections"] = request.allow_multiple_connections
 
     if request.message_filters is not None:
-        output["message_filters"] = (
-            marshal_DeviceMessageFilters(request.message_filters, defaults),
+        output["message_filters"] = marshal_DeviceMessageFilters(
+            request.message_filters, defaults
         )
 
     if request.hub_id is not None:
         output["hub_id"] = request.hub_id
 
     return output
```

### Comparing `scaleway-2.1.0/scaleway/iot/v1/types.py` & `scaleway-2.2.1/scaleway/iot/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/ipam/v1/__init__.py` & `scaleway-2.2.1/scaleway/ipam/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/ipam/v1/api.py` & `scaleway-2.2.1/scaleway/ipam/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         """
         Book a new IP.
         Book a new IP from the specified source. Currently IPs can only be booked from a Private Network.
         :param source: Source in which to book the IP. Not all sources are available for booking.
         :param is_ipv6: Request an IPv6 instead of an IPv4.
         :param region: Region to target. If none is passed will use default region from the config.
         :param project_id: When creating an IP in a Private Network, the Project must match the Private Network's Project.
-        :param address: Note that only the Private Network source allows you to pick a specific IP. If the requested IP is already booked, then the call will fail.
+        :param address: The requested address should not include the subnet mask (/suffix). Note that only the Private Network source allows you to pick a specific IP. If the requested IP is already booked, then the call will fail.
         :param tags: Tags for the IP.
         :return: :class:`IP <IP>`
 
         Usage:
         ::
 
             result = api.book_ip(
```

### Comparing `scaleway-2.1.0/scaleway/ipam/v1/marshalling.py` & `scaleway-2.2.1/scaleway/ipam/v1/marshalling.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,29 +24,33 @@
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Resource' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
 
-    field = data.get("type_", None)
+    field = data.get("type", None)
     if field is not None:
         args["type_"] = field
 
     field = data.get("id", None)
     if field is not None:
         args["id"] = field
 
     field = data.get("mac_address", None)
     if field is not None:
         args["mac_address"] = field
+    else:
+        args["mac_address"] = None
 
     field = data.get("name", None)
     if field is not None:
         args["name"] = field
+    else:
+        args["name"] = None
 
     return Resource(**args)
 
 
 def unmarshal_Reverse(data: Any) -> Reverse:
     if not isinstance(data, dict):
         raise TypeError(
@@ -58,14 +62,16 @@
     field = data.get("hostname", None)
     if field is not None:
         args["hostname"] = field
 
     field = data.get("address", None)
     if field is not None:
         args["address"] = field
+    else:
+        args["address"] = None
 
     return Reverse(**args)
 
 
 def unmarshal_Source(data: Any) -> Source:
     if not isinstance(data, dict):
         raise TypeError(
@@ -73,22 +79,28 @@
         )
 
     args: Dict[str, Any] = {}
 
     field = data.get("zonal", None)
     if field is not None:
         args["zonal"] = field
+    else:
+        args["zonal"] = None
 
     field = data.get("private_network_id", None)
     if field is not None:
         args["private_network_id"] = field
+    else:
+        args["private_network_id"] = None
 
     field = data.get("subnet_id", None)
     if field is not None:
         args["subnet_id"] = field
+    else:
+        args["subnet_id"] = None
 
     return Source(**args)
 
 
 def unmarshal_IP(data: Any) -> IP:
     if not isinstance(data, dict):
         raise TypeError(
@@ -130,26 +142,34 @@
     field = data.get("region", None)
     if field is not None:
         args["region"] = field
 
     field = data.get("created_at", None)
     if field is not None:
         args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    else:
+        args["created_at"] = None
 
     field = data.get("updated_at", None)
     if field is not None:
         args["updated_at"] = parser.isoparse(field) if isinstance(field, str) else field
+    else:
+        args["updated_at"] = None
 
     field = data.get("resource", None)
     if field is not None:
         args["resource"] = unmarshal_Resource(field)
+    else:
+        args["resource"] = None
 
     field = data.get("zone", None)
     if field is not None:
         args["zone"] = field
+    else:
+        args["zone"] = None
 
     return IP(**args)
 
 
 def unmarshal_ListIPsResponse(data: Any) -> ListIPsResponse:
     if not isinstance(data, dict):
         raise TypeError(
```

### Comparing `scaleway-2.1.0/scaleway/ipam/v1/types.py` & `scaleway-2.2.1/scaleway/ipam/v1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     project_id: Optional[str]
     """
     When creating an IP in a Private Network, the Project must match the Private Network's Project.
     """
 
     address: Optional[str]
     """
-    Note that only the Private Network source allows you to pick a specific IP. If the requested IP is already booked, then the call will fail.
+    The requested address should not include the subnet mask (/suffix). Note that only the Private Network source allows you to pick a specific IP. If the requested IP is already booked, then the call will fail.
     """
 
     tags: Optional[List[str]]
     """
     Tags for the IP.
     """
```

### Comparing `scaleway-2.1.0/scaleway/ipfs/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/ipfs/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/ipfs/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/ipfs/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/ipfs/v1alpha1/content.py` & `scaleway-2.2.1/scaleway/ipfs/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/ipfs/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/ipfs/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/ipfs/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/ipfs/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/jobs/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/jobs/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/jobs/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/jobs/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/jobs/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/jobs/v1alpha1/marshalling.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,18 +316,16 @@
             key: value for key, value in request.environment_variables.items()
         }
 
     if request.job_timeout is not None:
         output["job_timeout"] = request.job_timeout
 
     if request.cron_schedule is not None:
-        output["cron_schedule"] = (
-            marshal_CreateJobDefinitionRequestCronScheduleConfig(
-                request.cron_schedule, defaults
-            ),
+        output["cron_schedule"] = marshal_CreateJobDefinitionRequestCronScheduleConfig(
+            request.cron_schedule, defaults
         )
 
     return output
 
 
 def marshal_StartJobDefinitionRequest(
     request: StartJobDefinitionRequest,
@@ -392,14 +390,12 @@
     if request.description is not None:
         output["description"] = request.description
 
     if request.job_timeout is not None:
         output["job_timeout"] = request.job_timeout
 
     if request.cron_schedule is not None:
-        output["cron_schedule"] = (
-            marshal_UpdateJobDefinitionRequestCronScheduleConfig(
-                request.cron_schedule, defaults
-            ),
+        output["cron_schedule"] = marshal_UpdateJobDefinitionRequestCronScheduleConfig(
+            request.cron_schedule, defaults
         )
 
     return output
```

### Comparing `scaleway-2.1.0/scaleway/jobs/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/jobs/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/k8s/v1/__init__.py` & `scaleway-2.2.1/scaleway/k8s/v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 from .types import ListClustersResponse
 from .types import ListNodesRequest
 from .types import ListNodesResponse
 from .types import ListPoolsRequest
 from .types import ListPoolsResponse
 from .types import ListVersionsRequest
 from .types import ListVersionsResponse
+from .types import MigrateClusterToRoutedIPsRequest
 from .types import MigrateToPrivateNetworkClusterRequest
 from .types import RebootNodeRequest
 from .types import ReplaceNodeRequest
 from .types import ResetClusterAdminTokenRequest
 from .types import SetClusterTypeRequest
 from .types import UpdateClusterRequest
 from .types import UpdatePoolRequest
@@ -136,14 +137,15 @@
     "ListClustersResponse",
     "ListNodesRequest",
     "ListNodesResponse",
     "ListPoolsRequest",
     "ListPoolsResponse",
     "ListVersionsRequest",
     "ListVersionsResponse",
+    "MigrateClusterToRoutedIPsRequest",
     "MigrateToPrivateNetworkClusterRequest",
     "RebootNodeRequest",
     "ReplaceNodeRequest",
     "ResetClusterAdminTokenRequest",
     "SetClusterTypeRequest",
     "UpdateClusterRequest",
     "UpdatePoolRequest",
```

### Comparing `scaleway-2.1.0/scaleway/k8s/v1/api.py` & `scaleway-2.2.1/scaleway/k8s/v1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -753,14 +753,49 @@
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
         return unmarshal_Cluster(res.json())
 
+    def migrate_cluster_to_routed_i_ps(
+        self,
+        *,
+        cluster_id: str,
+        region: Optional[Region] = None,
+    ) -> Cluster:
+        """
+        Migrate a cluster to Routed IPs.
+        Migrate the nodes of an existing cluster to Routed IPs and enable Routed IPs for all future nodes.
+        :param cluster_id:
+        :param region: Region to target. If none is passed will use default region from the config.
+        :return: :class:`Cluster <Cluster>`
+
+        Usage:
+        ::
+
+            result = api.migrate_cluster_to_routed_i_ps(
+                cluster_id="example",
+            )
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_cluster_id = validate_path_param("cluster_id", cluster_id)
+
+        res = self._request(
+            "POST",
+            f"/k8s/v1/regions/{param_region}/clusters/{param_cluster_id}/migrate-to-routed-ips",
+            body={},
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_Cluster(res.json())
+
     def list_pools(
         self,
         *,
         cluster_id: str,
         region: Optional[Region] = None,
         order_by: Optional[ListPoolsRequestOrderBy] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.1.0/scaleway/k8s/v1/content.py` & `scaleway-2.2.1/scaleway/k8s/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/k8s/v1/marshalling.py` & `scaleway-2.2.1/scaleway/k8s/v1/marshalling.py`

 * *Files 3% similar despite different names*

```diff
@@ -481,18 +481,14 @@
 
     field = data.get("routed_ip_enabled", None)
     if field is not None:
         args["routed_ip_enabled"] = field
     else:
         args["routed_ip_enabled"] = None
 
-    field = data.get("routed_ip_enabled", None)
-    if field is not None:
-        args["routed_ip_enabled"] = field
-
     return Cluster(**args)
 
 
 def unmarshal_Node(data: Any) -> Node:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Node' failed as data isn't a dictionary."
@@ -885,16 +881,16 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.enable is not None:
         output["enable"] = request.enable
 
     if request.maintenance_window is not None:
-        output["maintenance_window"] = (
-            marshal_MaintenanceWindow(request.maintenance_window, defaults),
+        output["maintenance_window"] = marshal_MaintenanceWindow(
+            request.maintenance_window, defaults
         )
 
     return output
 
 
 def marshal_CreateClusterRequestAutoscalerConfig(
     request: CreateClusterRequestAutoscalerConfig,
@@ -1016,18 +1012,16 @@
     if request.root_volume_type is not None:
         output["root_volume_type"] = str(request.root_volume_type)
 
     if request.public_ip_disabled is not None:
         output["public_ip_disabled"] = request.public_ip_disabled
 
     if request.upgrade_policy is not None:
-        output["upgrade_policy"] = (
-            marshal_CreateClusterRequestPoolConfigUpgradePolicy(
-                request.upgrade_policy, defaults
-            ),
+        output["upgrade_policy"] = marshal_CreateClusterRequestPoolConfigUpgradePolicy(
+            request.upgrade_policy, defaults
         )
 
     if request.root_volume_size is not None:
         output["root_volume_size"] = request.root_volume_size
 
     return output
 
@@ -1073,36 +1067,34 @@
     if request.pools is not None:
         output["pools"] = [
             marshal_CreateClusterRequestPoolConfig(item, defaults)
             for item in request.pools
         ]
 
     if request.autoscaler_config is not None:
-        output["autoscaler_config"] = (
-            marshal_CreateClusterRequestAutoscalerConfig(
-                request.autoscaler_config, defaults
-            ),
+        output["autoscaler_config"] = marshal_CreateClusterRequestAutoscalerConfig(
+            request.autoscaler_config, defaults
         )
 
     if request.auto_upgrade is not None:
-        output["auto_upgrade"] = (
-            marshal_CreateClusterRequestAutoUpgrade(request.auto_upgrade, defaults),
+        output["auto_upgrade"] = marshal_CreateClusterRequestAutoUpgrade(
+            request.auto_upgrade, defaults
         )
 
     if request.feature_gates is not None:
         output["feature_gates"] = request.feature_gates
 
     if request.admission_plugins is not None:
         output["admission_plugins"] = request.admission_plugins
 
     if request.open_id_connect_config is not None:
         output["open_id_connect_config"] = (
             marshal_CreateClusterRequestOpenIDConnectConfig(
                 request.open_id_connect_config, defaults
-            ),
+            )
         )
 
     if request.apiserver_cert_sans is not None:
         output["apiserver_cert_sans"] = request.apiserver_cert_sans
 
     if request.private_network_id is not None:
         output["private_network_id"] = request.private_network_id
@@ -1166,16 +1158,16 @@
 
     if request.kubelet_args is not None:
         output["kubelet_args"] = {
             key: value for key, value in request.kubelet_args.items()
         }
 
     if request.upgrade_policy is not None:
-        output["upgrade_policy"] = (
-            marshal_CreatePoolRequestUpgradePolicy(request.upgrade_policy, defaults),
+        output["upgrade_policy"] = marshal_CreatePoolRequestUpgradePolicy(
+            request.upgrade_policy, defaults
         )
 
     if request.zone is not None:
         output["zone"] = request.zone or defaults.default_zone
 
     if request.root_volume_type is not None:
         output["root_volume_type"] = str(request.root_volume_type)
@@ -1216,16 +1208,16 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.enable is not None:
         output["enable"] = request.enable
 
     if request.maintenance_window is not None:
-        output["maintenance_window"] = (
-            marshal_MaintenanceWindow(request.maintenance_window, defaults),
+        output["maintenance_window"] = marshal_MaintenanceWindow(
+            request.maintenance_window, defaults
         )
 
     return output
 
 
 def marshal_UpdateClusterRequestAutoscalerConfig(
     request: UpdateClusterRequestAutoscalerConfig,
@@ -1312,36 +1304,34 @@
     if request.description is not None:
         output["description"] = request.description
 
     if request.tags is not None:
         output["tags"] = request.tags
 
     if request.autoscaler_config is not None:
-        output["autoscaler_config"] = (
-            marshal_UpdateClusterRequestAutoscalerConfig(
-                request.autoscaler_config, defaults
-            ),
+        output["autoscaler_config"] = marshal_UpdateClusterRequestAutoscalerConfig(
+            request.autoscaler_config, defaults
         )
 
     if request.auto_upgrade is not None:
-        output["auto_upgrade"] = (
-            marshal_UpdateClusterRequestAutoUpgrade(request.auto_upgrade, defaults),
+        output["auto_upgrade"] = marshal_UpdateClusterRequestAutoUpgrade(
+            request.auto_upgrade, defaults
         )
 
     if request.feature_gates is not None:
         output["feature_gates"] = request.feature_gates
 
     if request.admission_plugins is not None:
         output["admission_plugins"] = request.admission_plugins
 
     if request.open_id_connect_config is not None:
         output["open_id_connect_config"] = (
             marshal_UpdateClusterRequestOpenIDConnectConfig(
                 request.open_id_connect_config, defaults
-            ),
+            )
         )
 
     if request.apiserver_cert_sans is not None:
         output["apiserver_cert_sans"] = request.apiserver_cert_sans
 
     return output
 
@@ -1385,16 +1375,16 @@
     if request.tags is not None:
         output["tags"] = request.tags
 
     if request.kubelet_args is not None:
         output["kubelet_args"] = request.kubelet_args
 
     if request.upgrade_policy is not None:
-        output["upgrade_policy"] = (
-            marshal_UpdatePoolRequestUpgradePolicy(request.upgrade_policy, defaults),
+        output["upgrade_policy"] = marshal_UpdatePoolRequestUpgradePolicy(
+            request.upgrade_policy, defaults
         )
 
     return output
 
 
 def marshal_UpgradeClusterRequest(
     request: UpgradeClusterRequest,
```

### Comparing `scaleway-2.1.0/scaleway/k8s/v1/types.py` & `scaleway-2.2.1/scaleway/k8s/v1/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1644,14 +1644,24 @@
     versions: List[Version]
     """
     Available Kubernetes versions.
     """
 
 
 @dataclass
+class MigrateClusterToRoutedIPsRequest:
+    cluster_id: str
+
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+
+@dataclass
 class MigrateToPrivateNetworkClusterRequest:
     cluster_id: str
     """
     ID of the cluster to migrate.
     """
 
     private_network_id: str
```

### Comparing `scaleway-2.1.0/scaleway/lb/v1/__init__.py` & `scaleway-2.2.1/scaleway/lb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/lb/v1/api.py` & `scaleway-2.2.1/scaleway/lb/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,25 +581,27 @@
         zone: Optional[Zone] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         ip_address: Optional[str] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         ip_type: Optional[ListIpsRequestIpType] = None,
+        tags: Optional[List[str]] = None,
     ) -> ListIpsResponse:
         """
         List IP addresses.
         List the Load Balancer flexible IP addresses held in the account (filtered by Organization ID or Project ID). It is also possible to search for a specific IP address.
         :param zone: Zone to target. If none is passed will use default zone from the config.
         :param page: The page number to return, from the paginated results.
         :param page_size: Number of IP addresses to return.
         :param ip_address: IP address to filter for.
         :param organization_id: Organization ID to filter for, only Load Balancer IP addresses from this Organization will be returned.
         :param project_id: Project ID to filter for, only Load Balancer IP addresses from this Project will be returned.
         :param ip_type: IP type to filter for.
+        :param tags: Tag to filter for, only IPs with one or more matching tags will be returned.
         :return: :class:`ListIpsResponse <ListIpsResponse>`
 
         Usage:
         ::
 
             result = api.list_i_ps()
         """
@@ -613,14 +615,15 @@
                 "ip_address": ip_address,
                 "ip_type": ip_type,
                 "organization_id": organization_id
                 or self.client.default_organization_id,
                 "page": page,
                 "page_size": page_size or self.client.default_page_size,
                 "project_id": project_id or self.client.default_project_id,
+                "tags": tags,
             },
         )
 
         self._throw_on_error(res)
         return unmarshal_ListIpsResponse(res.json())
 
     def list_i_ps_all(
@@ -629,25 +632,27 @@
         zone: Optional[Zone] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         ip_address: Optional[str] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         ip_type: Optional[ListIpsRequestIpType] = None,
+        tags: Optional[List[str]] = None,
     ) -> List[Ip]:
         """
         List IP addresses.
         List the Load Balancer flexible IP addresses held in the account (filtered by Organization ID or Project ID). It is also possible to search for a specific IP address.
         :param zone: Zone to target. If none is passed will use default zone from the config.
         :param page: The page number to return, from the paginated results.
         :param page_size: Number of IP addresses to return.
         :param ip_address: IP address to filter for.
         :param organization_id: Organization ID to filter for, only Load Balancer IP addresses from this Organization will be returned.
         :param project_id: Project ID to filter for, only Load Balancer IP addresses from this Project will be returned.
         :param ip_type: IP type to filter for.
+        :param tags: Tag to filter for, only IPs with one or more matching tags will be returned.
         :return: :class:`List[Ip] <List[Ip]>`
 
         Usage:
         ::
 
             result = api.list_i_ps_all()
         """
@@ -660,36 +665,39 @@
                 "zone": zone,
                 "page": page,
                 "page_size": page_size,
                 "ip_address": ip_address,
                 "organization_id": organization_id,
                 "project_id": project_id,
                 "ip_type": ip_type,
+                "tags": tags,
             },
         )
 
     def create_ip(
         self,
         *,
         is_ipv6: bool,
         zone: Optional[Zone] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         reverse: Optional[str] = None,
+        tags: Optional[List[str]] = None,
     ) -> Ip:
         """
         Create an IP address.
         Create a new Load Balancer flexible IP address, in the specified Scaleway Project. This can be attached to new Load Balancers created in the future.
         :param is_ipv6: If true, creates a Flexible IP with an ipv6 address.
         :param zone: Zone to target. If none is passed will use default zone from the config.
         :param organization_id: Organization ID of the Organization where the IP address should be created.
         One-Of ('project_identifier'): at most one of 'project_id', 'organization_id' could be set.
         :param project_id: Project ID of the Project where the IP address should be created.
         One-Of ('project_identifier'): at most one of 'project_id', 'organization_id' could be set.
         :param reverse: Reverse DNS (domain name) for the IP address.
+        :param tags: List of tags for the IP.
         :return: :class:`Ip <Ip>`
 
         Usage:
         ::
 
             result = api.create_ip(
                 is_ipv6=False,
@@ -702,14 +710,15 @@
             "POST",
             f"/lb/v1/zones/{param_zone}/ips",
             body=marshal_ZonedApiCreateIpRequest(
                 ZonedApiCreateIpRequest(
                     is_ipv6=is_ipv6,
                     zone=zone,
                     reverse=reverse,
+                    tags=tags,
                     project_id=project_id,
                     organization_id=organization_id,
                 ),
                 self.client,
             ),
         )
 
@@ -781,22 +790,24 @@
     def update_ip(
         self,
         *,
         ip_id: str,
         zone: Optional[Zone] = None,
         reverse: Optional[str] = None,
         lb_id: Optional[str] = None,
+        tags: Optional[List[str]] = None,
     ) -> Ip:
         """
         Update an IP address.
         Update the reverse DNS of a Load Balancer flexible IP address.
         :param ip_id: IP address ID.
         :param zone: Zone to target. If none is passed will use default zone from the config.
         :param reverse: Reverse DNS (domain name) for the IP address.
         :param lb_id: ID of the server on which to attach the flexible IP.
+        :param tags: List of tags for the IP.
         :return: :class:`Ip <Ip>`
 
         Usage:
         ::
 
             result = api.update_ip(
                 ip_id="example",
@@ -811,14 +822,15 @@
             f"/lb/v1/zones/{param_zone}/ips/{param_ip_id}",
             body=marshal_ZonedApiUpdateIpRequest(
                 ZonedApiUpdateIpRequest(
                     ip_id=ip_id,
                     zone=zone,
                     reverse=reverse,
                     lb_id=lb_id,
+                    tags=tags,
                 ),
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
         return unmarshal_Ip(res.json())
@@ -3586,24 +3598,26 @@
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         ip_address: Optional[str] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         ip_type: Optional[ListIpsRequestIpType] = None,
+        tags: Optional[List[str]] = None,
     ) -> ListIpsResponse:
         """
         List IPs.
         :param region: Region to target. If none is passed will use default region from the config.
         :param page: The page number to return, from the paginated results.
         :param page_size: Number of IP addresses to return.
         :param ip_address: IP address to filter for.
         :param organization_id: Organization ID to filter for, only Load Balancer IP addresses from this Organization will be returned.
         :param project_id: Project ID to filter for, only Load Balancer IP addresses from this Project will be returned.
         :param ip_type: IP type to filter for.
+        :param tags: Tag to filter for, only IPs with one or more matching tags will be returned.
         :return: :class:`ListIpsResponse <ListIpsResponse>`
 
         Usage:
         ::
 
             result = api.list_i_ps()
         """
@@ -3619,14 +3633,15 @@
                 "ip_address": ip_address,
                 "ip_type": ip_type,
                 "organization_id": organization_id
                 or self.client.default_organization_id,
                 "page": page,
                 "page_size": page_size or self.client.default_page_size,
                 "project_id": project_id or self.client.default_project_id,
+                "tags": tags,
             },
         )
 
         self._throw_on_error(res)
         return unmarshal_ListIpsResponse(res.json())
 
     def list_i_ps_all(
@@ -3635,24 +3650,26 @@
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         ip_address: Optional[str] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         ip_type: Optional[ListIpsRequestIpType] = None,
+        tags: Optional[List[str]] = None,
     ) -> List[Ip]:
         """
         List IPs.
         :param region: Region to target. If none is passed will use default region from the config.
         :param page: The page number to return, from the paginated results.
         :param page_size: Number of IP addresses to return.
         :param ip_address: IP address to filter for.
         :param organization_id: Organization ID to filter for, only Load Balancer IP addresses from this Organization will be returned.
         :param project_id: Project ID to filter for, only Load Balancer IP addresses from this Project will be returned.
         :param ip_type: IP type to filter for.
+        :param tags: Tag to filter for, only IPs with one or more matching tags will be returned.
         :return: :class:`List[Ip] <List[Ip]>`
 
         Usage:
         ::
 
             result = api.list_i_ps_all()
         """
@@ -3665,35 +3682,38 @@
                 "region": region,
                 "page": page,
                 "page_size": page_size,
                 "ip_address": ip_address,
                 "organization_id": organization_id,
                 "project_id": project_id,
                 "ip_type": ip_type,
+                "tags": tags,
             },
         )
 
     def create_ip(
         self,
         *,
         is_ipv6: bool,
         region: Optional[Region] = None,
         organization_id: Optional[str] = None,
         project_id: Optional[str] = None,
         reverse: Optional[str] = None,
+        tags: Optional[List[str]] = None,
     ) -> Ip:
         """
         Create an IP.
         :param is_ipv6: If true, creates a Flexible IP with an ipv6 address.
         :param region: Region to target. If none is passed will use default region from the config.
         :param organization_id: Organization ID of the Organization where the IP address should be created.
         One-Of ('project_identifier'): at most one of 'project_id', 'organization_id' could be set.
         :param project_id: Project ID of the Project where the IP address should be created.
         One-Of ('project_identifier'): at most one of 'project_id', 'organization_id' could be set.
         :param reverse: Reverse DNS (domain name) for the IP address.
+        :param tags: List of tags for the IP.
         :return: :class:`Ip <Ip>`
 
         Usage:
         ::
 
             result = api.create_ip(
                 is_ipv6=False,
@@ -3708,14 +3728,15 @@
             "POST",
             f"/lb/v1/regions/{param_region}/ips",
             body=marshal_CreateIpRequest(
                 CreateIpRequest(
                     is_ipv6=is_ipv6,
                     region=region,
                     reverse=reverse,
+                    tags=tags,
                     project_id=project_id,
                     organization_id=organization_id,
                 ),
                 self.client,
             ),
         )
 
@@ -3789,21 +3810,23 @@
     def update_ip(
         self,
         *,
         ip_id: str,
         region: Optional[Region] = None,
         reverse: Optional[str] = None,
         lb_id: Optional[str] = None,
+        tags: Optional[List[str]] = None,
     ) -> Ip:
         """
         Update an IP.
         :param ip_id: IP address ID.
         :param region: Region to target. If none is passed will use default region from the config.
         :param reverse: Reverse DNS (domain name) for the IP address.
         :param lb_id: ID of the server on which to attach the flexible IP.
+        :param tags: List of tags for the IP.
         :return: :class:`Ip <Ip>`
 
         Usage:
         ::
 
             result = api.update_ip(
                 ip_id="example",
@@ -3820,14 +3843,15 @@
             f"/lb/v1/regions/{param_region}/ips/{param_ip_id}",
             body=marshal_UpdateIpRequest(
                 UpdateIpRequest(
                     ip_id=ip_id,
                     region=region,
                     reverse=reverse,
                     lb_id=lb_id,
+                    tags=tags,
                 ),
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
         return unmarshal_Ip(res.json())
```

### Comparing `scaleway-2.1.0/scaleway/lb/v1/content.py` & `scaleway-2.2.1/scaleway/lb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/lb/v1/marshalling.py` & `scaleway-2.2.1/scaleway/lb/v1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,18 @@
     if field is not None:
         args["project_id"] = field
 
     field = data.get("reverse", None)
     if field is not None:
         args["reverse"] = field
 
+    field = data.get("tags", None)
+    if field is not None:
+        args["tags"] = field
+
     field = data.get("zone", None)
     if field is not None:
         args["zone"] = field
 
     field = data.get("lb_id", None)
     if field is not None:
         args["lb_id"] = field
@@ -1582,15 +1586,15 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.type_ is not None:
         output["type"] = str(request.type_)
 
     if request.redirect is not None:
-        output["redirect"] = (marshal_AclActionRedirect(request.redirect, defaults),)
+        output["redirect"] = marshal_AclActionRedirect(request.redirect, defaults)
 
     return output
 
 
 def marshal_AclMatch(
     request: AclMatch,
     defaults: ProfileDefaults,
@@ -1618,27 +1622,27 @@
 def marshal_CreateAclRequest(
     request: CreateAclRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.action is not None:
-        output["action"] = (marshal_AclAction(request.action, defaults),)
+        output["action"] = marshal_AclAction(request.action, defaults)
 
     if request.index is not None:
         output["index"] = request.index
 
     if request.description is not None:
         output["description"] = request.description
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.match is not None:
-        output["match"] = (marshal_AclMatch(request.match, defaults),)
+        output["match"] = marshal_AclMatch(request.match, defaults)
 
     return output
 
 
 def marshal_HealthCheckHttpConfig(
     request: HealthCheckHttpConfig,
     defaults: ProfileDefaults,
@@ -1793,15 +1797,15 @@
     if request.sticky_sessions is not None:
         output["sticky_sessions"] = str(request.sticky_sessions)
 
     if request.sticky_sessions_cookie_name is not None:
         output["sticky_sessions_cookie_name"] = request.sticky_sessions_cookie_name
 
     if request.health_check is not None:
-        output["health_check"] = (marshal_HealthCheck(request.health_check, defaults),)
+        output["health_check"] = marshal_HealthCheck(request.health_check, defaults)
 
     if request.server_ip is not None:
         output["server_ip"] = request.server_ip
 
     if request.name is not None:
         output["name"] = request.name
 
@@ -1946,14 +1950,17 @@
 
     if request.is_ipv6 is not None:
         output["is_ipv6"] = request.is_ipv6
 
     if request.reverse is not None:
         output["reverse"] = request.reverse
 
+    if request.tags is not None:
+        output["tags"] = request.tags
+
     return output
 
 
 def marshal_CreateLbRequest(
     request: CreateLbRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
@@ -2029,15 +2036,15 @@
     if request.frontend_id is not None:
         output["frontend_id"] = request.frontend_id
 
     if request.backend_id is not None:
         output["backend_id"] = request.backend_id
 
     if request.match is not None:
-        output["match"] = (marshal_RouteMatch(request.match, defaults),)
+        output["match"] = marshal_RouteMatch(request.match, defaults)
 
     return output
 
 
 def marshal_SubscriberEmailConfig(
     request: SubscriberEmailConfig,
     defaults: ProfileDefaults,
@@ -2150,21 +2157,21 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.action is not None:
-        output["action"] = (marshal_AclAction(request.action, defaults),)
+        output["action"] = marshal_AclAction(request.action, defaults)
 
     if request.index is not None:
         output["index"] = request.index
 
     if request.match is not None:
-        output["match"] = (marshal_AclMatch(request.match, defaults),)
+        output["match"] = marshal_AclMatch(request.match, defaults)
 
     if request.description is not None:
         output["description"] = request.description
 
     return output
 
 
@@ -2324,14 +2331,17 @@
 
     if request.reverse is not None:
         output["reverse"] = request.reverse
 
     if request.lb_id is not None:
         output["lb_id"] = request.lb_id
 
+    if request.tags is not None:
+        output["tags"] = request.tags
+
     return output
 
 
 def marshal_UpdateLbRequest(
     request: UpdateLbRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
@@ -2358,15 +2368,15 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.backend_id is not None:
         output["backend_id"] = request.backend_id
 
     if request.match is not None:
-        output["match"] = (marshal_RouteMatch(request.match, defaults),)
+        output["match"] = marshal_RouteMatch(request.match, defaults)
 
     return output
 
 
 def marshal_UpdateSubscriberRequest(
     request: UpdateSubscriberRequest,
     defaults: ProfileDefaults,
@@ -2420,27 +2430,27 @@
 def marshal_ZonedApiCreateAclRequest(
     request: ZonedApiCreateAclRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.action is not None:
-        output["action"] = (marshal_AclAction(request.action, defaults),)
+        output["action"] = marshal_AclAction(request.action, defaults)
 
     if request.index is not None:
         output["index"] = request.index
 
     if request.description is not None:
         output["description"] = request.description
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.match is not None:
-        output["match"] = (marshal_AclMatch(request.match, defaults),)
+        output["match"] = marshal_AclMatch(request.match, defaults)
 
     return output
 
 
 def marshal_ZonedApiCreateBackendRequest(
     request: ZonedApiCreateBackendRequest,
     defaults: ProfileDefaults,
@@ -2459,15 +2469,15 @@
     if request.sticky_sessions is not None:
         output["sticky_sessions"] = str(request.sticky_sessions)
 
     if request.sticky_sessions_cookie_name is not None:
         output["sticky_sessions_cookie_name"] = request.sticky_sessions_cookie_name
 
     if request.health_check is not None:
-        output["health_check"] = (marshal_HealthCheck(request.health_check, defaults),)
+        output["health_check"] = marshal_HealthCheck(request.health_check, defaults)
 
     if request.server_ip is not None:
         output["server_ip"] = request.server_ip
 
     if request.name is not None:
         output["name"] = request.name
 
@@ -2585,14 +2595,17 @@
 
     if request.is_ipv6 is not None:
         output["is_ipv6"] = request.is_ipv6
 
     if request.reverse is not None:
         output["reverse"] = request.reverse
 
+    if request.tags is not None:
+        output["tags"] = request.tags
+
     return output
 
 
 def marshal_ZonedApiCreateLbRequest(
     request: ZonedApiCreateLbRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
@@ -2651,15 +2664,15 @@
     if request.frontend_id is not None:
         output["frontend_id"] = request.frontend_id
 
     if request.backend_id is not None:
         output["backend_id"] = request.backend_id
 
     if request.match is not None:
-        output["match"] = (marshal_RouteMatch(request.match, defaults),)
+        output["match"] = marshal_RouteMatch(request.match, defaults)
 
     return output
 
 
 def marshal_ZonedApiCreateSubscriberRequest(
     request: ZonedApiCreateSubscriberRequest,
     defaults: ProfileDefaults,
@@ -2724,24 +2737,24 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.action is not None:
-        output["action"] = (marshal_AclAction(request.action, defaults),)
+        output["action"] = marshal_AclAction(request.action, defaults)
 
     if request.index is not None:
         output["index"] = request.index
 
     if request.description is not None:
         output["description"] = request.description
 
     if request.match is not None:
-        output["match"] = (marshal_AclMatch(request.match, defaults),)
+        output["match"] = marshal_AclMatch(request.match, defaults)
 
     return output
 
 
 def marshal_ZonedApiSetAclsRequest(
     request: ZonedApiSetAclsRequest,
     defaults: ProfileDefaults,
@@ -2784,21 +2797,21 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.action is not None:
-        output["action"] = (marshal_AclAction(request.action, defaults),)
+        output["action"] = marshal_AclAction(request.action, defaults)
 
     if request.index is not None:
         output["index"] = request.index
 
     if request.match is not None:
-        output["match"] = (marshal_AclMatch(request.match, defaults),)
+        output["match"] = marshal_AclMatch(request.match, defaults)
 
     if request.description is not None:
         output["description"] = request.description
 
     return output
 
 
@@ -2958,14 +2971,17 @@
 
     if request.reverse is not None:
         output["reverse"] = request.reverse
 
     if request.lb_id is not None:
         output["lb_id"] = request.lb_id
 
+    if request.tags is not None:
+        output["tags"] = request.tags
+
     return output
 
 
 def marshal_ZonedApiUpdateLbRequest(
     request: ZonedApiUpdateLbRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
@@ -2992,15 +3008,15 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.backend_id is not None:
         output["backend_id"] = request.backend_id
 
     if request.match is not None:
-        output["match"] = (marshal_RouteMatch(request.match, defaults),)
+        output["match"] = marshal_RouteMatch(request.match, defaults)
 
     return output
 
 
 def marshal_ZonedApiUpdateSubscriberRequest(
     request: ZonedApiUpdateSubscriberRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.1.0/scaleway/lb/v1/types.py` & `scaleway-2.2.1/scaleway/lb/v1/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,14 +436,19 @@
     """
 
     reverse: str
     """
     Reverse DNS (domain name) of the IP address.
     """
 
+    tags: List[str]
+    """
+    IP tags.
+    """
+
     zone: Zone
     """
     The zone the IP address is in.
     """
 
     lb_id: Optional[str]
     """
@@ -1480,14 +1485,19 @@
     """
 
     reverse: Optional[str]
     """
     Reverse DNS (domain name) for the IP address.
     """
 
+    tags: Optional[List[str]]
+    """
+    List of tags for the IP.
+    """
+
     project_id: Optional[str]
 
     organization_id: Optional[str]
 
 
 @dataclass
 class CreateLbRequest:
@@ -2100,14 +2110,19 @@
     """
 
     ip_type: Optional[ListIpsRequestIpType]
     """
     IP type to filter for.
     """
 
+    tags: Optional[List[str]]
+    """
+    Tag to filter for, only IPs with one or more matching tags will be returned.
+    """
+
 
 @dataclass
 class ListIpsResponse:
     ips: List[Ip]
     """
     List of IP address objects.
     """
@@ -2736,14 +2751,19 @@
     """
 
     lb_id: Optional[str]
     """
     ID of the server on which to attach the flexible IP.
     """
 
+    tags: Optional[List[str]]
+    """
+    List of tags for the IP.
+    """
+
 
 @dataclass
 class UpdateLbRequest:
     lb_id: str
     """
     Load Balancer ID.
     """
@@ -3104,14 +3124,19 @@
     """
 
     reverse: Optional[str]
     """
     Reverse DNS (domain name) for the IP address.
     """
 
+    tags: Optional[List[str]]
+    """
+    List of tags for the IP.
+    """
+
     project_id: Optional[str]
 
     organization_id: Optional[str]
 
 
 @dataclass
 class ZonedApiCreateLbRequest:
@@ -3651,14 +3676,19 @@
     """
 
     ip_type: Optional[ListIpsRequestIpType]
     """
     IP type to filter for.
     """
 
+    tags: Optional[List[str]]
+    """
+    Tag to filter for, only IPs with one or more matching tags will be returned.
+    """
+
 
 @dataclass
 class ZonedApiListLbPrivateNetworksRequest:
     lb_id: str
     """
     Load Balancer ID.
     """
@@ -4214,14 +4244,19 @@
     """
 
     lb_id: Optional[str]
     """
     ID of the server on which to attach the flexible IP.
     """
 
+    tags: Optional[List[str]]
+    """
+    List of tags for the IP.
+    """
+
 
 @dataclass
 class ZonedApiUpdateLbRequest:
     lb_id: str
     """
     Load Balancer ID.
     """
```

### Comparing `scaleway-2.1.0/scaleway/llm_inference/v1beta1/__init__.py` & `scaleway-2.2.1/scaleway/llm_inference/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/llm_inference/v1beta1/api.py` & `scaleway-2.2.1/scaleway/llm_inference/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/llm_inference/v1beta1/marshalling.py` & `scaleway-2.2.1/scaleway/llm_inference/v1beta1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -617,15 +617,15 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.deployment_id is not None:
         output["deployment_id"] = request.deployment_id
 
     if request.endpoint is not None:
-        output["endpoint"] = (marshal_EndpointSpec(request.endpoint, defaults),)
+        output["endpoint"] = marshal_EndpointSpec(request.endpoint, defaults)
 
     return output
 
 
 def marshal_SetDeploymentACLRulesRequest(
     request: SetDeploymentACLRulesRequest,
     defaults: ProfileDefaults,
```

### Comparing `scaleway-2.1.0/scaleway/llm_inference/v1beta1/types.py` & `scaleway-2.2.1/scaleway/llm_inference/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/marketplace/v2/__init__.py` & `scaleway-2.2.1/scaleway/marketplace/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/marketplace/v2/api.py` & `scaleway-2.2.1/scaleway/marketplace/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/marketplace/v2/marshalling.py` & `scaleway-2.2.1/scaleway/marketplace/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/marketplace/v2/types.py` & `scaleway-2.2.1/scaleway/marketplace/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/mnq/v1beta1/__init__.py` & `scaleway-2.2.1/scaleway/mnq/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/mnq/v1beta1/api.py` & `scaleway-2.2.1/scaleway/mnq/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/mnq/v1beta1/marshalling.py` & `scaleway-2.2.1/scaleway/mnq/v1beta1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,15 +555,15 @@
     if request.project_id is not None:
         output["project_id"] = request.project_id or defaults.default_project_id
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.permissions is not None:
-        output["permissions"] = (marshal_SnsPermissions(request.permissions, defaults),)
+        output["permissions"] = marshal_SnsPermissions(request.permissions, defaults)
 
     return output
 
 
 def marshal_SnsApiDeactivateSnsRequest(
     request: SnsApiDeactivateSnsRequest,
     defaults: ProfileDefaults,
@@ -582,15 +582,15 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.permissions is not None:
-        output["permissions"] = (marshal_SnsPermissions(request.permissions, defaults),)
+        output["permissions"] = marshal_SnsPermissions(request.permissions, defaults)
 
     return output
 
 
 def marshal_SqsApiActivateSqsRequest(
     request: SqsApiActivateSqsRequest,
     defaults: ProfileDefaults,
@@ -630,15 +630,15 @@
     if request.project_id is not None:
         output["project_id"] = request.project_id or defaults.default_project_id
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.permissions is not None:
-        output["permissions"] = (marshal_SqsPermissions(request.permissions, defaults),)
+        output["permissions"] = marshal_SqsPermissions(request.permissions, defaults)
 
     return output
 
 
 def marshal_SqsApiDeactivateSqsRequest(
     request: SqsApiDeactivateSqsRequest,
     defaults: ProfileDefaults,
@@ -657,10 +657,10 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.name is not None:
         output["name"] = request.name
 
     if request.permissions is not None:
-        output["permissions"] = (marshal_SqsPermissions(request.permissions, defaults),)
+        output["permissions"] = marshal_SqsPermissions(request.permissions, defaults)
 
     return output
```

### Comparing `scaleway-2.1.0/scaleway/mnq/v1beta1/types.py` & `scaleway-2.2.1/scaleway/mnq/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/qaas/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/qaas/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/qaas/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/qaas/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/qaas/v1alpha1/content.py` & `scaleway-2.2.1/scaleway/qaas/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/qaas/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/qaas/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/qaas/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/qaas/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/rdb/v1/__init__.py` & `scaleway-2.2.1/scaleway/rdb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/rdb/v1/api.py` & `scaleway-2.2.1/scaleway/rdb/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/rdb/v1/content.py` & `scaleway-2.2.1/scaleway/rdb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/rdb/v1/marshalling.py` & `scaleway-2.2.1/scaleway/rdb/v1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1675,17 +1675,15 @@
 def marshal_CreateEndpointRequest(
     request: CreateEndpointRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.endpoint_spec is not None:
-        output["endpoint_spec"] = (
-            marshal_EndpointSpec(request.endpoint_spec, defaults),
-        )
+        output["endpoint_spec"] = marshal_EndpointSpec(request.endpoint_spec, defaults)
 
     return output
 
 
 def marshal_CreateInstanceFromSnapshotRequest(
     request: CreateInstanceFromSnapshotRequest,
     defaults: ProfileDefaults,
@@ -2066,15 +2064,15 @@
     if request.name is not None:
         output["name"] = request.name
 
     if request.tags is not None:
         output["tags"] = request.tags
 
     if request.logs_policy is not None:
-        output["logs_policy"] = (marshal_LogsPolicy(request.logs_policy, defaults),)
+        output["logs_policy"] = marshal_LogsPolicy(request.logs_policy, defaults)
 
     if request.backup_same_region is not None:
         output["backup_same_region"] = request.backup_same_region
 
     if request.backup_schedule_start_hour is not None:
         output["backup_schedule_start_hour"] = request.backup_schedule_start_hour
```

### Comparing `scaleway-2.1.0/scaleway/rdb/v1/types.py` & `scaleway-2.2.1/scaleway/rdb/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/redis/v1/__init__.py` & `scaleway-2.2.1/scaleway/redis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/redis/v1/api.py` & `scaleway-2.2.1/scaleway/redis/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/redis/v1/marshalling.py` & `scaleway-2.2.1/scaleway/redis/v1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,18 +639,16 @@
     if request.id is not None:
         output["id"] = request.id
 
     if request.service_ips is not None:
         output["service_ips"] = request.service_ips
 
     if request.ipam_config is not None:
-        output["ipam_config"] = (
-            marshal_EndpointSpecPrivateNetworkSpecIpamConfig(
-                request.ipam_config, defaults
-            ),
+        output["ipam_config"] = marshal_EndpointSpecPrivateNetworkSpecIpamConfig(
+            request.ipam_config, defaults
         )
 
     return output
 
 
 def marshal_EndpointSpecPublicNetworkSpec(
     request: EndpointSpecPublicNetworkSpec,
```

### Comparing `scaleway-2.1.0/scaleway/redis/v1/types.py` & `scaleway-2.2.1/scaleway/redis/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/registry/v1/__init__.py` & `scaleway-2.2.1/scaleway/registry/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/registry/v1/api.py` & `scaleway-2.2.1/scaleway/registry/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/registry/v1/content.py` & `scaleway-2.2.1/scaleway/registry/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/registry/v1/marshalling.py` & `scaleway-2.2.1/scaleway/registry/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/registry/v1/types.py` & `scaleway-2.2.1/scaleway/registry/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/secret/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/secret/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/secret/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/secret/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/secret/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/secret/v1alpha1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,16 +434,16 @@
     if request.type_ is not None:
         output["type"] = str(request.type_)
 
     if request.path is not None:
         output["path"] = request.path
 
     if request.ephemeral_policy is not None:
-        output["ephemeral_policy"] = (
-            marshal_EphemeralPolicy(request.ephemeral_policy, defaults),
+        output["ephemeral_policy"] = marshal_EphemeralPolicy(
+            request.ephemeral_policy, defaults
         )
 
     return output
 
 
 def marshal_PasswordGenerationParams(
     request: PasswordGenerationParams,
@@ -481,16 +481,16 @@
     if request.description is not None:
         output["description"] = request.description
 
     if request.disable_previous is not None:
         output["disable_previous"] = request.disable_previous
 
     if request.password_generation is not None:
-        output["password_generation"] = (
-            marshal_PasswordGenerationParams(request.password_generation, defaults),
+        output["password_generation"] = marshal_PasswordGenerationParams(
+            request.password_generation, defaults
         )
 
     if request.data_crc32 is not None:
         output["data_crc32"] = request.data_crc32
 
     return output
 
@@ -540,16 +540,16 @@
     if request.description is not None:
         output["description"] = request.description
 
     if request.path is not None:
         output["path"] = request.path
 
     if request.ephemeral_policy is not None:
-        output["ephemeral_policy"] = (
-            marshal_EphemeralPolicy(request.ephemeral_policy, defaults),
+        output["ephemeral_policy"] = marshal_EphemeralPolicy(
+            request.ephemeral_policy, defaults
         )
 
     return output
 
 
 def marshal_EphemeralProperties(
     request: EphemeralProperties,
@@ -575,12 +575,12 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.description is not None:
         output["description"] = request.description
 
     if request.ephemeral_properties is not None:
-        output["ephemeral_properties"] = (
-            marshal_EphemeralProperties(request.ephemeral_properties, defaults),
+        output["ephemeral_properties"] = marshal_EphemeralProperties(
+            request.ephemeral_properties, defaults
         )
 
     return output
```

### Comparing `scaleway-2.1.0/scaleway/secret/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/secret/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/secret/v1beta1/__init__.py` & `scaleway-2.2.1/scaleway/secret/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/secret/v1beta1/api.py` & `scaleway-2.2.1/scaleway/secret/v1beta1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/secret/v1beta1/marshalling.py` & `scaleway-2.2.1/scaleway/secret/v1beta1/marshalling.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,16 +472,16 @@
     if request.type_ is not None:
         output["type"] = str(request.type_)
 
     if request.path is not None:
         output["path"] = request.path
 
     if request.ephemeral_policy is not None:
-        output["ephemeral_policy"] = (
-            marshal_EphemeralPolicy(request.ephemeral_policy, defaults),
+        output["ephemeral_policy"] = marshal_EphemeralPolicy(
+            request.ephemeral_policy, defaults
         )
 
     return output
 
 
 def marshal_CreateSecretVersionRequest(
     request: CreateSecretVersionRequest,
@@ -519,16 +519,16 @@
     if request.description is not None:
         output["description"] = request.description
 
     if request.path is not None:
         output["path"] = request.path
 
     if request.ephemeral_policy is not None:
-        output["ephemeral_policy"] = (
-            marshal_EphemeralPolicy(request.ephemeral_policy, defaults),
+        output["ephemeral_policy"] = marshal_EphemeralPolicy(
+            request.ephemeral_policy, defaults
         )
 
     return output
 
 
 def marshal_EphemeralProperties(
     request: EphemeralProperties,
@@ -554,12 +554,12 @@
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.description is not None:
         output["description"] = request.description
 
     if request.ephemeral_properties is not None:
-        output["ephemeral_properties"] = (
-            marshal_EphemeralProperties(request.ephemeral_properties, defaults),
+        output["ephemeral_properties"] = marshal_EphemeralProperties(
+            request.ephemeral_properties, defaults
         )
 
     return output
```

### Comparing `scaleway-2.1.0/scaleway/secret/v1beta1/types.py` & `scaleway-2.2.1/scaleway/secret/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/serverless_sqldb/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/tem/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/tem/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/tem/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/tem/v1alpha1/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,19 +553,19 @@
         name: Optional[str] = None,
     ) -> ListDomainsResponse:
         """
         List domains.
         Retrieve domains in a specific Project or in a specific Organization using the `region` parameter.
         :param region: Region to target. If none is passed will use default region from the config.
         :param page: Requested page number. Value must be greater or equal to 1.
-        :param page_size: Page size.
-        :param project_id:
-        :param status:
-        :param organization_id:
-        :param name:
+        :param page_size: Requested page size. Value must be between 1 and 1000.
+        :param project_id: (Optional) ID of the Project in which to list the domains.
+        :param status: (Optional) List domains under specific statuses.
+        :param organization_id: (Optional) ID of the Organization in which to list the domains.
+        :param name: (Optional) Names of the domains to list.
         :return: :class:`ListDomainsResponse <ListDomainsResponse>`
 
         Usage:
         ::
 
             result = api.list_domains()
         """
@@ -603,19 +603,19 @@
         name: Optional[str] = None,
     ) -> List[Domain]:
         """
         List domains.
         Retrieve domains in a specific Project or in a specific Organization using the `region` parameter.
         :param region: Region to target. If none is passed will use default region from the config.
         :param page: Requested page number. Value must be greater or equal to 1.
-        :param page_size: Page size.
-        :param project_id:
-        :param status:
-        :param organization_id:
-        :param name:
+        :param page_size: Requested page size. Value must be between 1 and 1000.
+        :param project_id: (Optional) ID of the Project in which to list the domains.
+        :param status: (Optional) List domains under specific statuses.
+        :param organization_id: (Optional) ID of the Organization in which to list the domains.
+        :param name: (Optional) Names of the domains to list.
         :return: :class:`List[Domain] <List[Domain]>`
 
         Usage:
         ::
 
             result = api.list_domains_all()
         """
```

### Comparing `scaleway-2.1.0/scaleway/tem/v1alpha1/content.py` & `scaleway-2.2.1/scaleway/tem/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/tem/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/tem/v1alpha1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -633,15 +633,15 @@
     if request.text is not None:
         output["text"] = request.text
 
     if request.html is not None:
         output["html"] = request.html
 
     if request.from_ is not None:
-        output["from"] = (marshal_CreateEmailRequestAddress(request.from_, defaults),)
+        output["from"] = marshal_CreateEmailRequestAddress(request.from_, defaults)
 
     if request.to is not None:
         output["to"] = [
             marshal_CreateEmailRequestAddress(item, defaults) for item in request.to
         ]
 
     if request.cc is not None:
```

### Comparing `scaleway-2.1.0/scaleway/tem/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/tem/v1alpha1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,24 +675,36 @@
     page: Optional[int]
     """
     Requested page number. Value must be greater or equal to 1.
     """
 
     page_size: Optional[int]
     """
-    Page size.
+    Requested page size. Value must be between 1 and 1000.
     """
 
     project_id: Optional[str]
+    """
+    (Optional) ID of the Project in which to list the domains.
+    """
 
     status: Optional[List[DomainStatus]]
+    """
+    (Optional) List domains under specific statuses.
+    """
 
     organization_id: Optional[str]
+    """
+    (Optional) ID of the Organization in which to list the domains.
+    """
 
     name: Optional[str]
+    """
+    (Optional) Names of the domains to list.
+    """
 
 
 @dataclass
 class ListDomainsResponse:
     total_count: int
     """
     Number of domains that match the request (without pagination).
```

### Comparing `scaleway-2.1.0/scaleway/test/v1/__init__.py` & `scaleway-2.2.1/scaleway/test/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/test/v1/api.py` & `scaleway-2.2.1/scaleway/test/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/test/v1/marshalling.py` & `scaleway-2.2.1/scaleway/test/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/test/v1/types.py` & `scaleway-2.2.1/scaleway/test/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v1/__init__.py` & `scaleway-2.2.1/scaleway/vpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v1/api.py` & `scaleway-2.2.1/scaleway/vpc/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v1/marshalling.py` & `scaleway-2.2.1/scaleway/vpc/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v1/types.py` & `scaleway-2.2.1/scaleway/vpc/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v2/__init__.py` & `scaleway-2.2.1/scaleway/vpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v2/api.py` & `scaleway-2.2.1/scaleway/vpc/v2/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v2/marshalling.py` & `scaleway-2.2.1/scaleway/vpc/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpc/v2/types.py` & `scaleway-2.2.1/scaleway/vpc/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpcgw/v1/__init__.py` & `scaleway-2.2.1/scaleway/vpcgw/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpcgw/v1/api.py` & `scaleway-2.2.1/scaleway/vpcgw/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpcgw/v1/content.py` & `scaleway-2.2.1/scaleway/vpcgw/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpcgw/v1/marshalling.py` & `scaleway-2.2.1/scaleway/vpcgw/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/vpcgw/v1/types.py` & `scaleway-2.2.1/scaleway/vpcgw/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.1.0/scaleway/webhosting/v1alpha1/__init__.py` & `scaleway-2.2.1/scaleway/webhosting/v1alpha1/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,25 +16,29 @@
 from .types import CreateHostingRequestDomainConfiguration
 from .types import DnsRecord
 from .types import Nameserver
 from .types import ControlPanel
 from .types import Hosting
 from .types import Offer
 from .types import CreateHostingRequest
+from .types import CreateSessionRequest
 from .types import DeleteHostingRequest
 from .types import DnsRecords
 from .types import GetDomainDnsRecordsRequest
 from .types import GetHostingRequest
 from .types import ListControlPanelsRequest
 from .types import ListControlPanelsResponse
 from .types import ListHostingsRequest
 from .types import ListHostingsResponse
 from .types import ListOffersRequest
 from .types import ListOffersResponse
+from .types import ResetHostingPasswordRequest
+from .types import ResetHostingPasswordResponse
 from .types import RestoreHostingRequest
+from .types import Session
 from .types import UpdateHostingRequest
 from .api import WebhostingV1Alpha1API
 
 __all__ = [
     "DnsRecordStatus",
     "DnsRecordType",
     "DnsRecordsStatus",
@@ -51,21 +55,25 @@
     "CreateHostingRequestDomainConfiguration",
     "DnsRecord",
     "Nameserver",
     "ControlPanel",
     "Hosting",
     "Offer",
     "CreateHostingRequest",
+    "CreateSessionRequest",
     "DeleteHostingRequest",
     "DnsRecords",
     "GetDomainDnsRecordsRequest",
     "GetHostingRequest",
     "ListControlPanelsRequest",
     "ListControlPanelsResponse",
     "ListHostingsRequest",
     "ListHostingsResponse",
     "ListOffersRequest",
     "ListOffersResponse",
+    "ResetHostingPasswordRequest",
+    "ResetHostingPasswordResponse",
     "RestoreHostingRequest",
+    "Session",
     "UpdateHostingRequest",
     "WebhostingV1Alpha1API",
 ]
```

### Comparing `scaleway-2.1.0/scaleway/webhosting/v1alpha1/api.py` & `scaleway-2.2.1/scaleway/webhosting/v1alpha1/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,25 +21,29 @@
     CreateHostingRequest,
     CreateHostingRequestDomainConfiguration,
     DnsRecords,
     Hosting,
     ListControlPanelsResponse,
     ListHostingsResponse,
     ListOffersResponse,
+    ResetHostingPasswordResponse,
+    Session,
     UpdateHostingRequest,
 )
 from .content import (
     HOSTING_TRANSIENT_STATUSES,
 )
 from .marshalling import (
     unmarshal_Hosting,
     unmarshal_DnsRecords,
     unmarshal_ListControlPanelsResponse,
     unmarshal_ListHostingsResponse,
     unmarshal_ListOffersResponse,
+    unmarshal_ResetHostingPasswordResponse,
+    unmarshal_Session,
     marshal_CreateHostingRequest,
     marshal_UpdateHostingRequest,
 )
 from ...std.types import (
     LanguageCode as StdLanguageCode,
 )
 
@@ -506,16 +510,15 @@
         self,
         *,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> ListControlPanelsResponse:
         """
-        List all control panels type.
-        List the control panels type: cpanel or plesk.
+        "List the control panels type: cpanel or plesk.".
         :param region: Region to target. If none is passed will use default region from the config.
         :param page: Page number to return, from the paginated results (must be a positive integer).
         :param page_size: Number of control panels to return (must be a positive integer lower or equal to 100).
         :return: :class:`ListControlPanelsResponse <ListControlPanelsResponse>`
 
         Usage:
         ::
@@ -543,16 +546,15 @@
         self,
         *,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[ControlPanel]:
         """
-        List all control panels type.
-        List the control panels type: cpanel or plesk.
+        "List the control panels type: cpanel or plesk.".
         :param region: Region to target. If none is passed will use default region from the config.
         :param page: Page number to return, from the paginated results (must be a positive integer).
         :param page_size: Number of control panels to return (must be a positive integer lower or equal to 100).
         :return: :class:`List[ControlPanel] <List[ControlPanel]>`
 
         Usage:
         ::
@@ -566,7 +568,74 @@
             fetcher=self.list_control_panels,
             args={
                 "region": region,
                 "page": page,
                 "page_size": page_size,
             },
         )
+
+    def create_session(
+        self,
+        *,
+        hosting_id: str,
+        region: Optional[Region] = None,
+    ) -> Session:
+        """
+        Create a user session.
+        :param hosting_id: Hosting ID.
+        :param region: Region to target. If none is passed will use default region from the config.
+        :return: :class:`Session <Session>`
+
+        Usage:
+        ::
+
+            result = api.create_session(
+                hosting_id="example",
+            )
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_hosting_id = validate_path_param("hosting_id", hosting_id)
+
+        res = self._request(
+            "POST",
+            f"/webhosting/v1alpha1/regions/{param_region}/hostings/{param_hosting_id}/sessions",
+            body={},
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_Session(res.json())
+
+    def reset_hosting_password(
+        self,
+        *,
+        hosting_id: str,
+        region: Optional[Region] = None,
+    ) -> ResetHostingPasswordResponse:
+        """
+        :param hosting_id: UUID of the hosting.
+        :param region: Region to target. If none is passed will use default region from the config.
+        :return: :class:`ResetHostingPasswordResponse <ResetHostingPasswordResponse>`
+
+        Usage:
+        ::
+
+            result = api.reset_hosting_password(
+                hosting_id="example",
+            )
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+        param_hosting_id = validate_path_param("hosting_id", hosting_id)
+
+        res = self._request(
+            "POST",
+            f"/webhosting/v1alpha1/regions/{param_region}/hostings/{param_hosting_id}/reset-password",
+            body={},
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_ResetHostingPasswordResponse(res.json())
```

### Comparing `scaleway-2.1.0/scaleway/webhosting/v1alpha1/marshalling.py` & `scaleway-2.2.1/scaleway/webhosting/v1alpha1/marshalling.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     DnsRecords,
     ControlPanel,
     ListControlPanelsResponse,
     ListHostingsResponse,
     OfferProduct,
     Offer,
     ListOffersResponse,
+    ResetHostingPasswordResponse,
+    Session,
     CreateHostingRequestDomainConfiguration,
     CreateHostingRequest,
     UpdateHostingRequest,
 )
 
 
 def unmarshal_HostingCpanelUrls(data: Any) -> HostingCpanelUrls:
@@ -448,14 +450,44 @@
         args["offers"] = (
             [unmarshal_Offer(v) for v in field] if field is not None else None
         )
 
     return ListOffersResponse(**args)
 
 
+def unmarshal_ResetHostingPasswordResponse(data: Any) -> ResetHostingPasswordResponse:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'ResetHostingPasswordResponse' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("password", None)
+    if field is not None:
+        args["password"] = field
+
+    return ResetHostingPasswordResponse(**args)
+
+
+def unmarshal_Session(data: Any) -> Session:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'Session' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("url", None)
+    if field is not None:
+        args["url"] = field
+
+    return Session(**args)
+
+
 def marshal_CreateHostingRequestDomainConfiguration(
     request: CreateHostingRequestDomainConfiguration,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.update_nameservers is not None:
@@ -500,15 +532,15 @@
     if request.language is not None:
         output["language"] = str(request.language)
 
     if request.domain_configuration is not None:
         output["domain_configuration"] = (
             marshal_CreateHostingRequestDomainConfiguration(
                 request.domain_configuration, defaults
-            ),
+            )
         )
 
     return output
 
 
 def marshal_UpdateHostingRequest(
     request: UpdateHostingRequest,
```

### Comparing `scaleway-2.1.0/scaleway/webhosting/v1alpha1/types.py` & `scaleway-2.2.1/scaleway/webhosting/v1alpha1/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -471,14 +471,27 @@
     domain_configuration: Optional[CreateHostingRequestDomainConfiguration]
     """
     Indicates whether to update hosting domain name servers and DNS records for domains managed by Scaleway Elements.
     """
 
 
 @dataclass
+class CreateSessionRequest:
+    hosting_id: str
+    """
+    Hosting ID.
+    """
+
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+
+@dataclass
 class DeleteHostingRequest:
     hosting_id: str
     """
     Hosting ID.
     """
 
     region: Optional[Region]
@@ -666,27 +679,56 @@
     offers: List[Offer]
     """
     List of offers.
     """
 
 
 @dataclass
+class ResetHostingPasswordRequest:
+    hosting_id: str
+    """
+    UUID of the hosting.
+    """
+
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+
+@dataclass
+class ResetHostingPasswordResponse:
+    password: str
+    """
+    New password.
+    """
+
+
+@dataclass
 class RestoreHostingRequest:
     hosting_id: str
     """
     Hosting ID.
     """
 
     region: Optional[Region]
     """
     Region to target. If none is passed will use default region from the config.
     """
 
 
 @dataclass
+class Session:
+    url: str
+    """
+    Logged user's session URL.
+    """
+
+
+@dataclass
 class UpdateHostingRequest:
     hosting_id: str
     """
     Hosting ID.
     """
 
     region: Optional[Region]
```

### Comparing `scaleway-2.1.0/PKG-INFO` & `scaleway-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway
-Version: 2.1.0
+Version: 2.2.1
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -19,14 +19,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
-Requires-Dist: scaleway-core (==2.1.0)
+Requires-Dist: scaleway-core (==2.2.1)
 Description-Content-Type: text/markdown
 
 # Scaleway Python SDK
 
 This SDK enables you to interact with Scaleway APIs.
```

