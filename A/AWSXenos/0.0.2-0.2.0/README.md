# Comparing `tmp/AWSXenos-0.0.2.tar.gz` & `tmp/awsxenos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AWSXenos-0.0.2.tar", last modified: Tue Oct 12 20:00:51 2021, max compression
+gzip compressed data, was "awsxenos-0.2.0.tar", last modified: Tue May 14 08:13:53 2024, max compression
```

## Comparing `AWSXenos-0.0.2.tar` & `awsxenos-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 20:00:51.536660 AWSXenos-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 20:00:51.532660 AWSXenos-0.0.2/AWSXenos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3384 2021-10-12 20:00:51.000000 AWSXenos-0.0.2/AWSXenos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-10-12 20:00:51.000000 AWSXenos-0.0.2/AWSXenos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-12 20:00:51.000000 AWSXenos-0.0.2/AWSXenos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-10-12 20:00:51.000000 AWSXenos-0.0.2/AWSXenos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-10-12 20:00:51.000000 AWSXenos-0.0.2/AWSXenos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-10-12 20:00:51.000000 AWSXenos-0.0.2/AWSXenos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3384 2021-10-12 20:00:51.536660 AWSXenos-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2825 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 20:00:51.536660 AWSXenos-0.0.2/awsxenos/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/awsxenos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24983 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/awsxenos/accounts.json
--rw-r--r--   0 runner    (1001) docker     (121)      548 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/awsxenos/finding.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/awsxenos/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/awsxenos/report.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14388 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/awsxenos/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/awsxenos/template.html
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-12 20:00:51.536660 AWSXenos-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 20:00:51.536660 AWSXenos-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9013 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     2367 2021-10-12 20:00:41.000000 AWSXenos-0.0.2/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:53.584090 awsxenos-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:53.584090 awsxenos-0.2.0/AWSXenos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-14 08:13:53.000000 awsxenos-0.2.0/AWSXenos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 08:13:53.000000 awsxenos-0.2.0/AWSXenos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:13:53.000000 awsxenos-0.2.0/AWSXenos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 08:13:53.000000 awsxenos-0.2.0/AWSXenos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 08:13:53.000000 awsxenos-0.2.0/AWSXenos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 08:13:53.000000 awsxenos-0.2.0/AWSXenos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 08:13:47.000000 awsxenos-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 08:13:47.000000 awsxenos-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-14 08:13:53.584090 awsxenos-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-14 08:13:47.000000 awsxenos-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:53.580090 awsxenos-0.2.0/awsxenos/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92879 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/accounts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5574 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:53.584090 awsxenos-0.2.0/awsxenos/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/efs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/eventbridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/kms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/services/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-14 08:13:47.000000 awsxenos-0.2.0/awsxenos/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 08:13:47.000000 awsxenos-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:13:53.584090 awsxenos-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-14 08:13:47.000000 awsxenos-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:53.584090 awsxenos-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:13:47.000000 awsxenos-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-14 08:13:47.000000 awsxenos-0.2.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-14 08:13:47.000000 awsxenos-0.2.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-14 08:13:47.000000 awsxenos-0.2.0/tests/test_scan.py
```

### Comparing `AWSXenos-0.0.2/LICENSE` & `awsxenos-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AWSXenos-0.0.2/awsxenos/report.py` & `awsxenos-0.2.0/awsxenos/report.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,65 @@
-from collections import defaultdict
-from typing import List, Dict, DefaultDict
 import json
+from collections import defaultdict
+from typing import DefaultDict, Dict, List
 
 from jinja2 import Environment, FileSystemLoader  # type: ignore
 from policyuniverse.arn import ARN  # type: ignore
 
-from awsxenos.finding import AccountType, Finding
 from awsxenos import package_path
 
+from awsxenos.finding import Findings, Resources
+
 
 class Report:
-    def __init__(self, findings: DefaultDict[str, AccountType], account_info: DefaultDict[str, Dict]) -> None:
+    def __init__(self, findings: Findings, account_info: Resources) -> None:
         self.summary = self._summarise(findings, account_info)
 
-    def _summarise(
-        self, findings: DefaultDict[str, AccountType], account_info: DefaultDict[str, Dict]
-    ) -> DefaultDict[str, List]:
+    def _summarise(self, findings: Findings, account_info: Resources) -> DefaultDict[str, List]:
         summary = defaultdict(list)
-        for resource, accounttype in findings.items():
-            # Refactor
-            # for account_type, principal in finding
-            if accounttype.known_accounts:
-                for finding in accounttype.known_accounts:
+
+        for resource, account_type in findings.items():
+            if account_type.known_accounts:
+                for finding in account_type.known_accounts:
                     role_arn = ARN(finding.principal)
                     summary["known_accounts"].append(
                         {
                             "ARN": resource,
-                            "principal": accounttype.known_accounts,
+                            "principal": account_type.known_accounts,
                             "external_info": account_info[role_arn.account_number],
                             "external_id": finding.external_id,
                         }
                     )
-            if accounttype.org_accounts:
-                for finding in accounttype.org_accounts:
+            if account_type.org_accounts:
+                for finding in account_type.org_accounts:
                     role_arn = ARN(finding.principal)
                     summary["org_accounts"].append(
                         {
                             "ARN": resource,
-                            "principal": accounttype.org_accounts,
+                            "principal": account_type.org_accounts,
                             "external_info": account_info[role_arn.account_number],
                         }
                     )
-            if accounttype.aws_services:
-                for finding in accounttype.aws_services:
+            if account_type.aws_services:
+                for finding in account_type.aws_services:
                     role_arn = ARN(finding.principal)
                     summary["aws_services"].append(
                         {
                             "ARN": resource,
-                            "principal": accounttype.aws_services,
+                            "principal": account_type.aws_services,
                             "external_info": account_info[role_arn.tech],
                         }
                     )
-            if accounttype.unknown_accounts:
-                for finding in accounttype.unknown_accounts:
+            if account_type.unknown_accounts:
+                for finding in account_type.unknown_accounts:
                     role_arn = ARN(finding.principal)
                     summary["unknown_accounts"].append(
                         {
                             "ARN": resource,
-                            "principal": accounttype.unknown_accounts,
+                            "principal": account_type.unknown_accounts,
                             "external_info": account_info[role_arn.account_number],
                             "external_id": finding.external_id,
                         }
                     )
         return summary
 
     def JSON_report(self) -> str:
```

### Comparing `AWSXenos-0.0.2/awsxenos/template.html` & `awsxenos-0.2.0/awsxenos/template.html`

 * *Files identical despite different names*

### Comparing `AWSXenos-0.0.2/setup.py` & `awsxenos-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 setup(
     name="AWSXenos",
-    version="0.0.2",
-    author="CostasK",
+    version="0.2.0",
+    author="Costas Kourmpoglou",
     author_email="costas.kourmpoglou@airwalkconsulting.com",
     license="MIT",
-    description="Scan and classify cross-account roles in your AWS Account",
+    description="Scan and classify cross-account roles and resources in your AWS Account",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AirWalk-Digital/AWSXenos",
     py_modules=["awsxenos"],
     packages=find_packages(),
     install_requires=[requirements],
-    python_requires=">=3.7",
-    package_data={"": ["accounts.json", "template.html"]},
+    python_requires=">=3.8",
+    package_data={"": ["config.yaml", "accounts.json", "template.html"]},
     classifiers=[
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points="""
         [console_scripts]
         awsxenos=awsxenos.scan:cli
     """,
```

### Comparing `AWSXenos-0.0.2/tests/fixtures.py` & `awsxenos-0.2.0/tests/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 from collections import defaultdict
 import datetime
-
+from awsxenos.finding import Accounts, Findings, Finding
 
 class Fixtures:
     @staticmethod
+    def mock_findings():
+        findings = Findings()
+        findings["arn:aws:iam::000000000000:role/somerole"].known_accounts.append(Finding("arn:aws:iam::999999999991:role/known",False))
+        findings["arn:aws:iam::000000000001:role/somerole"].unknown_accounts.append(Finding("arn:aws:iam::999999999992:role/unknown",False))
+        findings["arn:aws:iam::000000000002:role/somerole"].org_accounts.append(Finding("arn:aws:iam::999999999993:role/org",False))
+        findings["arn:aws:iam::000000000000:role/service-role/somerole"].aws_services.append(Finding("logging.s3.amazonaws.com",False))
+        return findings
+        
+    @staticmethod
     def mock_get_roles():
         roles = defaultdict(str)
         boto_list_roles = {
             "Roles": [
                 {
                     "Path": "/service-role/",
                     "RoleName": "AccessAnalyzerMonitor",
```

