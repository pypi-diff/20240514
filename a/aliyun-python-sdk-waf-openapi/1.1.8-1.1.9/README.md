# Comparing `tmp/aliyun-python-sdk-waf-openapi-1.1.8.tar.gz` & `tmp/aliyun-python-sdk-waf-openapi-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-waf-openapi-1.1.8.tar", last modified: Tue Jan 18 09:07:56 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-waf-openapi-1.1.9.tar", last modified: Tue Aug 22 06:19:32 2023, max compression
```

## Comparing `aliyun-python-sdk-waf-openapi-1.1.8.tar` & `aliyun-python-sdk-waf-openapi-1.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/
--rw-r--r--   0 root         (0) root         (0)      575 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1577 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1577 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2870 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2522 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/
--rw-r--r--   0 root         (0) root         (0)     1885 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateByCertificateIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2259 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     5877 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateProtectionModuleRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1640 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DeleteDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1698 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DeleteInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2028 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DeleteProtectionModuleRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2085 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeCertMatchStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeCertificatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1917 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainAdvanceConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2725 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainBasicConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2711 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1708 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainNamesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRuleGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1710 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1718 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceSpecInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2536 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeLogServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2106 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleCodeConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2782 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1873 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1722 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeWafSourceIpSegmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainIpv6StatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     5656 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1839 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyLogRetrievalStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyLogServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2022 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2376 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2074 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2038 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleCacheStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2414 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/MoveResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2458 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/SetDomainRuleGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2492 2022-01-18 09:07:56.000000 aliyun-python-sdk-waf-openapi-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      543 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateByCertificateIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6691 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateProtectionModuleRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DeleteDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DeleteInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DeleteProtectionModuleRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeCertMatchStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeCertificatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainAdvanceConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainBasicConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainNamesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRuleGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceSpecInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeLogServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleCodeConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeWafSourceIpSegmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainIpv6StatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyLogRetrievalStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyLogServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleCacheStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/MoveResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/SetDomainRuleGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-08-22 06:19:32.000000 aliyun-python-sdk-waf-openapi-1.1.9/setup.py
```

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/LICENSE` & `aliyun-python-sdk-waf-openapi-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/PKG-INFO` & `aliyun-python-sdk-waf-openapi-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-waf-openapi
-Version: 1.1.8
+Version: 1.1.9
 Summary: The waf-openapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-waf-openapi
```

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/README.rst` & `aliyun-python-sdk-waf-openapi-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/PKG-INFO` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-waf-openapi
-Version: 1.1.8
+Version: 1.1.9
 Summary: The waf-openapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-waf-openapi
```

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyun_python_sdk_waf_openapi.egg-info/SOURCES.txt` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyun_python_sdk_waf_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/endpoint.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateByCertificateIdRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateByCertificateIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateDomainRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateDomainRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_IpFollowStatus(self): # Integer
 		return self.get_query_params().get('IpFollowStatus')
 
 	def set_IpFollowStatus(self, IpFollowStatus):  # Integer
 		self.add_query_param('IpFollowStatus', IpFollowStatus)
+	def get_Keepalive(self): # Boolean
+		return self.get_query_params().get('Keepalive')
+
+	def set_Keepalive(self, Keepalive):  # Boolean
+		self.add_query_param('Keepalive', Keepalive)
 	def get_SniHost(self): # String
 		return self.get_query_params().get('SniHost')
 
 	def set_SniHost(self, SniHost):  # String
 		self.add_query_param('SniHost', SniHost)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
@@ -57,89 +62,104 @@
 	def set_Http2Port(self, Http2Port):  # String
 		self.add_query_param('Http2Port', Http2Port)
 	def get_WriteTime(self): # Integer
 		return self.get_query_params().get('WriteTime')
 
 	def set_WriteTime(self, WriteTime):  # Integer
 		self.add_query_param('WriteTime', WriteTime)
-	def get_SniStatus(self): # Integer
-		return self.get_query_params().get('SniStatus')
-
-	def set_SniStatus(self, SniStatus):  # Integer
-		self.add_query_param('SniStatus', SniStatus)
 	def get_AccessHeaderMode(self): # Integer
 		return self.get_query_params().get('AccessHeaderMode')
 
 	def set_AccessHeaderMode(self, AccessHeaderMode):  # Integer
 		self.add_query_param('AccessHeaderMode', AccessHeaderMode)
-	def get_AccessType(self): # String
-		return self.get_query_params().get('AccessType')
-
-	def set_AccessType(self, AccessType):  # String
-		self.add_query_param('AccessType', AccessType)
-	def get_LogHeaders(self): # String
-		return self.get_query_params().get('LogHeaders')
-
-	def set_LogHeaders(self, LogHeaders):  # String
-		self.add_query_param('LogHeaders', LogHeaders)
 	def get_AccessHeaders(self): # String
 		return self.get_query_params().get('AccessHeaders')
 
 	def set_AccessHeaders(self, AccessHeaders):  # String
 		self.add_query_param('AccessHeaders', AccessHeaders)
-	def get_ConnectionTime(self): # Integer
-		return self.get_query_params().get('ConnectionTime')
+	def get_KeepaliveTimeout(self): # Integer
+		return self.get_query_params().get('KeepaliveTimeout')
 
-	def set_ConnectionTime(self, ConnectionTime):  # Integer
-		self.add_query_param('ConnectionTime', ConnectionTime)
+	def set_KeepaliveTimeout(self, KeepaliveTimeout):  # Integer
+		self.add_query_param('KeepaliveTimeout', KeepaliveTimeout)
 	def get_ClusterType(self): # Integer
 		return self.get_query_params().get('ClusterType')
 
 	def set_ClusterType(self, ClusterType):  # Integer
 		self.add_query_param('ClusterType', ClusterType)
-	def get_CloudNativeInstances(self): # String
-		return self.get_query_params().get('CloudNativeInstances')
-
-	def set_CloudNativeInstances(self, CloudNativeInstances):  # String
-		self.add_query_param('CloudNativeInstances', CloudNativeInstances)
 	def get_HttpsRedirect(self): # Integer
 		return self.get_query_params().get('HttpsRedirect')
 
 	def set_HttpsRedirect(self, HttpsRedirect):  # Integer
 		self.add_query_param('HttpsRedirect', HttpsRedirect)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
-	def get_SourceIps(self): # String
-		return self.get_query_params().get('SourceIps')
-
-	def set_SourceIps(self, SourceIps):  # String
-		self.add_query_param('SourceIps', SourceIps)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
-	def get_IsAccessProduct(self): # Integer
-		return self.get_query_params().get('IsAccessProduct')
-
-	def set_IsAccessProduct(self, IsAccessProduct):  # Integer
-		self.add_query_param('IsAccessProduct', IsAccessProduct)
 	def get_ReadTime(self): # Integer
 		return self.get_query_params().get('ReadTime')
 
 	def set_ReadTime(self, ReadTime):  # Integer
 		self.add_query_param('ReadTime', ReadTime)
 	def get_HttpsPort(self): # String
 		return self.get_query_params().get('HttpsPort')
 
 	def set_HttpsPort(self, HttpsPort):  # String
 		self.add_query_param('HttpsPort', HttpsPort)
+	def get_SniStatus(self): # Integer
+		return self.get_query_params().get('SniStatus')
+
+	def set_SniStatus(self, SniStatus):  # Integer
+		self.add_query_param('SniStatus', SniStatus)
+	def get_Retry(self): # Boolean
+		return self.get_query_params().get('Retry')
+
+	def set_Retry(self, Retry):  # Boolean
+		self.add_query_param('Retry', Retry)
+	def get_KeepaliveRequests(self): # Integer
+		return self.get_query_params().get('KeepaliveRequests')
+
+	def set_KeepaliveRequests(self, KeepaliveRequests):  # Integer
+		self.add_query_param('KeepaliveRequests', KeepaliveRequests)
+	def get_AccessType(self): # String
+		return self.get_query_params().get('AccessType')
+
+	def set_AccessType(self, AccessType):  # String
+		self.add_query_param('AccessType', AccessType)
+	def get_LogHeaders(self): # String
+		return self.get_query_params().get('LogHeaders')
+
+	def set_LogHeaders(self, LogHeaders):  # String
+		self.add_query_param('LogHeaders', LogHeaders)
+	def get_ConnectionTime(self): # Integer
+		return self.get_query_params().get('ConnectionTime')
+
+	def set_ConnectionTime(self, ConnectionTime):  # Integer
+		self.add_query_param('ConnectionTime', ConnectionTime)
+	def get_CloudNativeInstances(self): # String
+		return self.get_query_params().get('CloudNativeInstances')
+
+	def set_CloudNativeInstances(self, CloudNativeInstances):  # String
+		self.add_query_param('CloudNativeInstances', CloudNativeInstances)
+	def get_SourceIps(self): # String
+		return self.get_query_params().get('SourceIps')
+
+	def set_SourceIps(self, SourceIps):  # String
+		self.add_query_param('SourceIps', SourceIps)
+	def get_IsAccessProduct(self): # Integer
+		return self.get_query_params().get('IsAccessProduct')
+
+	def set_IsAccessProduct(self, IsAccessProduct):  # Integer
+		self.add_query_param('IsAccessProduct', IsAccessProduct)
 	def get_LoadBalancing(self): # Integer
 		return self.get_query_params().get('LoadBalancing')
 
 	def set_LoadBalancing(self, LoadBalancing):  # Integer
 		self.add_query_param('LoadBalancing', LoadBalancing)
 	def get_HttpToUserIp(self): # Integer
 		return self.get_query_params().get('HttpToUserIp')
```

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/CreateProtectionModuleRuleRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/CreateProtectionModuleRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DeleteDomainRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DeleteDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DeleteInstanceRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DeleteInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DeleteProtectionModuleRuleRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DeleteProtectionModuleRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeCertMatchStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeCertMatchStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeCertificatesRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeCertificatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainAdvanceConfigsRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainAdvanceConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainBasicConfigsRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainBasicConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainListRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainNamesRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainNamesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRuleGroupRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeDomainRuleGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceInfoRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceSpecInfoRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeInstanceSpecInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeLogServiceStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeLogServiceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleCodeConfigRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleCodeConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleRulesRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeProtectionModuleStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/DescribeWafSourceIpSegmentRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/DescribeWafSourceIpSegmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainIpv6StatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainIpv6StatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyDomainRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_IpFollowStatus(self): # Integer
 		return self.get_query_params().get('IpFollowStatus')
 
 	def set_IpFollowStatus(self, IpFollowStatus):  # Integer
 		self.add_query_param('IpFollowStatus', IpFollowStatus)
+	def get_Keepalive(self): # Boolean
+		return self.get_query_params().get('Keepalive')
+
+	def set_Keepalive(self, Keepalive):  # Boolean
+		self.add_query_param('Keepalive', Keepalive)
 	def get_SniHost(self): # String
 		return self.get_query_params().get('SniHost')
 
 	def set_SniHost(self, SniHost):  # String
 		self.add_query_param('SniHost', SniHost)
 	def get_HttpPort(self): # String
 		return self.get_query_params().get('HttpPort')
@@ -52,89 +57,104 @@
 	def set_Http2Port(self, Http2Port):  # String
 		self.add_query_param('Http2Port', Http2Port)
 	def get_WriteTime(self): # Integer
 		return self.get_query_params().get('WriteTime')
 
 	def set_WriteTime(self, WriteTime):  # Integer
 		self.add_query_param('WriteTime', WriteTime)
-	def get_SniStatus(self): # Integer
-		return self.get_query_params().get('SniStatus')
-
-	def set_SniStatus(self, SniStatus):  # Integer
-		self.add_query_param('SniStatus', SniStatus)
 	def get_AccessHeaderMode(self): # Integer
 		return self.get_query_params().get('AccessHeaderMode')
 
 	def set_AccessHeaderMode(self, AccessHeaderMode):  # Integer
 		self.add_query_param('AccessHeaderMode', AccessHeaderMode)
-	def get_AccessType(self): # String
-		return self.get_query_params().get('AccessType')
-
-	def set_AccessType(self, AccessType):  # String
-		self.add_query_param('AccessType', AccessType)
-	def get_LogHeaders(self): # String
-		return self.get_query_params().get('LogHeaders')
-
-	def set_LogHeaders(self, LogHeaders):  # String
-		self.add_query_param('LogHeaders', LogHeaders)
 	def get_AccessHeaders(self): # String
 		return self.get_query_params().get('AccessHeaders')
 
 	def set_AccessHeaders(self, AccessHeaders):  # String
 		self.add_query_param('AccessHeaders', AccessHeaders)
-	def get_ConnectionTime(self): # Integer
-		return self.get_query_params().get('ConnectionTime')
+	def get_KeepaliveTimeout(self): # Integer
+		return self.get_query_params().get('KeepaliveTimeout')
 
-	def set_ConnectionTime(self, ConnectionTime):  # Integer
-		self.add_query_param('ConnectionTime', ConnectionTime)
+	def set_KeepaliveTimeout(self, KeepaliveTimeout):  # Integer
+		self.add_query_param('KeepaliveTimeout', KeepaliveTimeout)
 	def get_ClusterType(self): # Integer
 		return self.get_query_params().get('ClusterType')
 
 	def set_ClusterType(self, ClusterType):  # Integer
 		self.add_query_param('ClusterType', ClusterType)
-	def get_CloudNativeInstances(self): # String
-		return self.get_query_params().get('CloudNativeInstances')
-
-	def set_CloudNativeInstances(self, CloudNativeInstances):  # String
-		self.add_query_param('CloudNativeInstances', CloudNativeInstances)
 	def get_HttpsRedirect(self): # Integer
 		return self.get_query_params().get('HttpsRedirect')
 
 	def set_HttpsRedirect(self, HttpsRedirect):  # Integer
 		self.add_query_param('HttpsRedirect', HttpsRedirect)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
-	def get_SourceIps(self): # String
-		return self.get_query_params().get('SourceIps')
-
-	def set_SourceIps(self, SourceIps):  # String
-		self.add_query_param('SourceIps', SourceIps)
 	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self, Domain):  # String
 		self.add_query_param('Domain', Domain)
-	def get_IsAccessProduct(self): # Integer
-		return self.get_query_params().get('IsAccessProduct')
-
-	def set_IsAccessProduct(self, IsAccessProduct):  # Integer
-		self.add_query_param('IsAccessProduct', IsAccessProduct)
 	def get_ReadTime(self): # Integer
 		return self.get_query_params().get('ReadTime')
 
 	def set_ReadTime(self, ReadTime):  # Integer
 		self.add_query_param('ReadTime', ReadTime)
 	def get_HttpsPort(self): # String
 		return self.get_query_params().get('HttpsPort')
 
 	def set_HttpsPort(self, HttpsPort):  # String
 		self.add_query_param('HttpsPort', HttpsPort)
+	def get_SniStatus(self): # Integer
+		return self.get_query_params().get('SniStatus')
+
+	def set_SniStatus(self, SniStatus):  # Integer
+		self.add_query_param('SniStatus', SniStatus)
+	def get_Retry(self): # Boolean
+		return self.get_query_params().get('Retry')
+
+	def set_Retry(self, Retry):  # Boolean
+		self.add_query_param('Retry', Retry)
+	def get_KeepaliveRequests(self): # Integer
+		return self.get_query_params().get('KeepaliveRequests')
+
+	def set_KeepaliveRequests(self, KeepaliveRequests):  # Integer
+		self.add_query_param('KeepaliveRequests', KeepaliveRequests)
+	def get_AccessType(self): # String
+		return self.get_query_params().get('AccessType')
+
+	def set_AccessType(self, AccessType):  # String
+		self.add_query_param('AccessType', AccessType)
+	def get_LogHeaders(self): # String
+		return self.get_query_params().get('LogHeaders')
+
+	def set_LogHeaders(self, LogHeaders):  # String
+		self.add_query_param('LogHeaders', LogHeaders)
+	def get_ConnectionTime(self): # Integer
+		return self.get_query_params().get('ConnectionTime')
+
+	def set_ConnectionTime(self, ConnectionTime):  # Integer
+		self.add_query_param('ConnectionTime', ConnectionTime)
+	def get_CloudNativeInstances(self): # String
+		return self.get_query_params().get('CloudNativeInstances')
+
+	def set_CloudNativeInstances(self, CloudNativeInstances):  # String
+		self.add_query_param('CloudNativeInstances', CloudNativeInstances)
+	def get_SourceIps(self): # String
+		return self.get_query_params().get('SourceIps')
+
+	def set_SourceIps(self, SourceIps):  # String
+		self.add_query_param('SourceIps', SourceIps)
+	def get_IsAccessProduct(self): # Integer
+		return self.get_query_params().get('IsAccessProduct')
+
+	def set_IsAccessProduct(self, IsAccessProduct):  # Integer
+		self.add_query_param('IsAccessProduct', IsAccessProduct)
 	def get_LoadBalancing(self): # Integer
 		return self.get_query_params().get('LoadBalancing')
 
 	def set_LoadBalancing(self, LoadBalancing):  # Integer
 		self.add_query_param('LoadBalancing', LoadBalancing)
 	def get_HttpToUserIp(self): # Integer
 		return self.get_query_params().get('HttpToUserIp')
```

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyLogRetrievalStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyLogRetrievalStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyLogServiceStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyLogServiceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleModeRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleRuleRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionModuleStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleCacheStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleCacheStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleStatusRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/ModifyProtectionRuleStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/MoveResourceGroupRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/MoveResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/aliyunsdkwaf_openapi/request/v20190910/SetDomainRuleGroupRequest.py` & `aliyun-python-sdk-waf-openapi-1.1.9/aliyunsdkwaf_openapi/request/v20190910/SetDomainRuleGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-waf-openapi-1.1.8/setup.py` & `aliyun-python-sdk-waf-openapi-1.1.9/setup.py`

 * *Files identical despite different names*

