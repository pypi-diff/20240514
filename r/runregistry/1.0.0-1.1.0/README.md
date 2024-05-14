# Comparing `tmp/runregistry-1.0.0.tar.gz` & `tmp/runregistry-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runregistry-1.0.0.tar", last modified: Mon Aug  7 08:33:43 2023, max compression
+gzip compressed data, was "runregistry-1.1.0.tar", last modified: Tue May 14 13:01:59 2024, max compression
```

## Comparing `runregistry-1.0.0.tar` & `runregistry-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-08-07 08:33:43.886661 runregistry-1.0.0/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1071 2023-07-04 10:38:26.000000 runregistry-1.0.0/LICENSE
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    19956 2023-08-07 08:33:43.886661 runregistry-1.0.0/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    19625 2023-07-25 12:16:04.000000 runregistry-1.0.0/README.md
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-08-07 08:33:43.882660 runregistry-1.0.0/runregistry/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      174 2023-07-25 12:16:04.000000 runregistry-1.0.0/runregistry/__init__.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     5448 2023-07-04 12:05:22.000000 runregistry-1.0.0/runregistry/attributes.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    18170 2023-08-07 08:31:20.000000 runregistry-1.0.0/runregistry/runregistry.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     5556 2023-07-04 12:06:58.000000 runregistry-1.0.0/runregistry/utils.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-08-07 08:33:43.886661 runregistry-1.0.0/runregistry.egg-info/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    19956 2023-08-07 08:33:43.000000 runregistry-1.0.0/runregistry.egg-info/PKG-INFO
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      453 2023-08-07 08:33:43.000000 runregistry-1.0.0/runregistry.egg-info/SOURCES.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2023-08-07 08:33:43.000000 runregistry-1.0.0/runregistry.egg-info/dependency_links.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       36 2023-08-07 08:33:43.000000 runregistry-1.0.0/runregistry.egg-info/requires.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       18 2023-08-07 08:33:43.000000 runregistry-1.0.0/runregistry.egg-info/top_level.txt
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2023-08-07 08:33:43.890661 runregistry-1.0.0/setup.cfg
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1118 2023-07-25 12:16:04.000000 runregistry-1.0.0/setup.py
-drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-08-07 08:33:43.886661 runregistry-1.0.0/tests/
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-07-04 10:38:26.000000 runregistry-1.0.0/tests/__init__.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      895 2023-07-04 11:54:19.000000 runregistry-1.0.0/tests/advanced_rr_operations.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2054 2023-07-04 11:55:10.000000 runregistry-1.0.0/tests/sample_json_generation_from_CTPPS.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      956 2023-07-25 12:16:04.000000 runregistry-1.0.0/tests/stress_test.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    13122 2023-07-25 12:16:04.000000 runregistry-1.0.0/tests/test_client.py
--rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      966 2023-07-04 12:05:13.000000 runregistry-1.0.0/tests/test_utils.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2024-05-14 13:01:59.361204 runregistry-1.1.0/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1071 2023-08-14 14:01:57.000000 runregistry-1.1.0/LICENSE
+-rw-r--r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    19840 2024-05-14 13:01:59.361204 runregistry-1.1.0/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    19428 2024-05-14 13:01:08.000000 runregistry-1.1.0/README.md
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2024-05-14 13:01:59.361204 runregistry-1.1.0/runregistry/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      174 2024-05-14 13:01:08.000000 runregistry-1.1.0/runregistry/__init__.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     5448 2023-08-14 14:01:57.000000 runregistry-1.1.0/runregistry/attributes.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    20101 2024-05-14 13:01:08.000000 runregistry-1.1.0/runregistry/runregistry.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     5897 2024-05-14 13:01:08.000000 runregistry-1.1.0/runregistry/utils.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2024-05-14 13:01:59.361204 runregistry-1.1.0/runregistry.egg-info/
+-rw-r--r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    19840 2024-05-14 13:01:59.000000 runregistry-1.1.0/runregistry.egg-info/PKG-INFO
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      458 2024-05-14 13:01:59.000000 runregistry-1.1.0/runregistry.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        1 2024-05-14 13:01:59.000000 runregistry-1.1.0/runregistry.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       36 2024-05-14 13:01:59.000000 runregistry-1.1.0/runregistry.egg-info/requires.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       18 2024-05-14 13:01:59.000000 runregistry-1.1.0/runregistry.egg-info/top_level.txt
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)       38 2024-05-14 13:01:59.361204 runregistry-1.1.0/setup.cfg
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     1118 2023-08-14 14:01:57.000000 runregistry-1.1.0/setup.py
+drwxrwxr-x   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2024-05-14 13:01:59.361204 runregistry-1.1.0/tests/
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)        0 2023-08-14 14:01:57.000000 runregistry-1.1.0/tests/__init__.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2054 2023-08-14 14:01:57.000000 runregistry-1.1.0/tests/sample_json_generation_from_CTPPS.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      956 2023-08-14 14:01:57.000000 runregistry-1.1.0/tests/stress_test.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)     2848 2024-05-14 13:01:08.000000 runregistry-1.1.0/tests/test_advanced_rr_operations.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)    13112 2024-05-14 13:01:08.000000 runregistry-1.1.0/tests/test_client.py
+-rw-rw-r--   0 dpapagiannis  (1000) dpapagiannis  (1000)      966 2023-09-05 13:46:33.000000 runregistry-1.1.0/tests/test_utils.py
```

### Comparing `runregistry-1.0.0/LICENSE` & `runregistry-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runregistry-1.0.0/PKG-INFO` & `runregistry-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: runregistry
-Version: 1.0.0
+Version: 1.1.0
 Summary: CMS Run Registry client
 Home-page: https://github.com/cms-DQM/runregistry_api_client/
 Author: Fabio Espinosa
 Author-email: f.e@cern.ch
 Maintainer: CMS DQM team
 Maintainer-email: cms-dqm-coreTeam@cern.ch
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: cernrequests
+Requires-Dist: python-dotenv
 
 ![Build Status](https://github.com/cms-DQM/runregistry_api_client/actions/workflows/test_package.yaml/badge.svg)
 
 # Run Registry Client
 
 Python client to retrieve and query data from [CMS Run Registry](https://cmsrunregistry.web.cern.ch).
 
@@ -27,48 +30,48 @@
 
 ## Python version and Virtual env
 
 Python version>=3.6 is required for this package.
 A virtual environment is also required, if you are in lxplus you should run the following commands:
 
 ```bash
-virtualenv -p `which python3` venv
+virtualenv -p $(which python3) venv
 source venv/bin/activate
 ```
 
 ## Installation
 
 ```bash
 pip install runregistry
 ```
 
 ## Authentication Prerequisites
 
 > **Warning**
-> Grid certificates have been deprecated by CERN. As of version `1.0.0`, the `runregistry` 
-> client only works with a client ID and a secret. 
+> Grid certificates have been deprecated by CERN. As of version `1.0.0`, the `runregistry`
+> client only works with a client ID and a secret.
 
-You will need to create an SSO registration for your application which is going to be using the runregistry API client. 
+You will need to create an SSO registration for your application which is going to be using the runregistry API client.
 
 Instructions on how to do it can be found on the [`cernrequests`](https://github.com/CMSTrackerDPG/cernrequests) GitHub page.
 
-Once you have a client ID and a secret, you will need to store them in a file named `.env`. A [sample file](.env_sample) is provided so that you can edit it and rename it to `.env`. 
+Once you have a client ID and a secret, you will need to store them in a file named `.env`. A [sample file](.env_sample) is provided so that you can edit it and rename it to `.env`.
 
 Alternatively, you can run `export SSO_CLIENT_ID=...` and `export SSO_CLIENT_SECRET=...` on the same terminal that you will be running your python script in.
 
 ## Usage
 
-### Get a single run (get_run):
+### Get a single run (get_run)
 
 ```python
 import runregistry
 run = runregistry.get_run(run_number=328762)
 ```
 
-### Query several runs (get_runs):
+### Query several runs (get_runs)
 
 ```python
 import runregistry
 runs = runregistry.get_runs(filter={
    'run_number':{
       'or': [328762, 323555, 323444]
     }
@@ -404,15 +407,15 @@
     ```python
     runregistry.make_significant_runs(run=362761)
     ```
 2. Reset RR attributes and reload data from OMS:
     ```python
     runregistry.reset_RR_attributes_and_refresh_runs(run=362761)
     ```
-3. Move runs from one state to another: 
+3. Move runs from one state to another:
     ```python
     runregistry.move_runs("OPEN", "SIGNOFF", run=362761)
     ```
 
 ## Troubleshooting
 
 ### Support
@@ -424,28 +427,25 @@
 ```bash
 python3 -m pip install --upgrade pip build twine
 python3 -m build
 python3 -m twine upload --skip-existing --repository pypi dist/*
 ```
 Instructions from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
-## Testing
+## Running the tests
 
 ### Locally
 
-> **TODO**
-> Remove the qa environment after migration.
+You will be needing a file named `.env` with the following variables:
 
-You will be needing a file named `.env` with the following variables
 ```bash
 SSO_CLIENT_ID=<change>
 SSO_CLIENT_SECRET=<change>
-ENVIRONMENT=qa
+ENVIRONMENT=development
 ```
-While most of the tests work on the development deployment, some fail and need the production one. This is the reason we are setting `ENVIRONMENT=qa`.
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 pip install -r testing-requirements.txt
 pip install -e .
@@ -466,12 +466,12 @@
 
 ### Should I be using `runregistry_api_client` for getting OMS data?
 
 No*.
 
 Our recommendation is to query Run Registry only for data that RR is responsible for.
 
-<small>*It's not that you can't, it's just that this puts extra burden on the application, making it slow for everyone.</small> 
+<small>*It's not that you can't, it's just that this puts extra burden on the application, making it slow for everyone.</small>
 
 ### Is the token stored somewhere and reused?
 
-No, almost every function call gets a new token. This is not ideal, and it may be improved in the future.   
+No, almost every function call gets a new token. This is not ideal, and it may be improved in the future.
```

### Comparing `runregistry-1.0.0/README.md` & `runregistry-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,48 +15,48 @@
 
 ## Python version and Virtual env
 
 Python version>=3.6 is required for this package.
 A virtual environment is also required, if you are in lxplus you should run the following commands:
 
 ```bash
-virtualenv -p `which python3` venv
+virtualenv -p $(which python3) venv
 source venv/bin/activate
 ```
 
 ## Installation
 
 ```bash
 pip install runregistry
 ```
 
 ## Authentication Prerequisites
 
 > **Warning**
-> Grid certificates have been deprecated by CERN. As of version `1.0.0`, the `runregistry` 
-> client only works with a client ID and a secret. 
+> Grid certificates have been deprecated by CERN. As of version `1.0.0`, the `runregistry`
+> client only works with a client ID and a secret.
 
-You will need to create an SSO registration for your application which is going to be using the runregistry API client. 
+You will need to create an SSO registration for your application which is going to be using the runregistry API client.
 
 Instructions on how to do it can be found on the [`cernrequests`](https://github.com/CMSTrackerDPG/cernrequests) GitHub page.
 
-Once you have a client ID and a secret, you will need to store them in a file named `.env`. A [sample file](.env_sample) is provided so that you can edit it and rename it to `.env`. 
+Once you have a client ID and a secret, you will need to store them in a file named `.env`. A [sample file](.env_sample) is provided so that you can edit it and rename it to `.env`.
 
 Alternatively, you can run `export SSO_CLIENT_ID=...` and `export SSO_CLIENT_SECRET=...` on the same terminal that you will be running your python script in.
 
 ## Usage
 
-### Get a single run (get_run):
+### Get a single run (get_run)
 
 ```python
 import runregistry
 run = runregistry.get_run(run_number=328762)
 ```
 
-### Query several runs (get_runs):
+### Query several runs (get_runs)
 
 ```python
 import runregistry
 runs = runregistry.get_runs(filter={
    'run_number':{
       'or': [328762, 323555, 323444]
     }
@@ -392,15 +392,15 @@
     ```python
     runregistry.make_significant_runs(run=362761)
     ```
 2. Reset RR attributes and reload data from OMS:
     ```python
     runregistry.reset_RR_attributes_and_refresh_runs(run=362761)
     ```
-3. Move runs from one state to another: 
+3. Move runs from one state to another:
     ```python
     runregistry.move_runs("OPEN", "SIGNOFF", run=362761)
     ```
 
 ## Troubleshooting
 
 ### Support
@@ -412,28 +412,25 @@
 ```bash
 python3 -m pip install --upgrade pip build twine
 python3 -m build
 python3 -m twine upload --skip-existing --repository pypi dist/*
 ```
 Instructions from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
-## Testing
+## Running the tests
 
 ### Locally
 
-> **TODO**
-> Remove the qa environment after migration.
+You will be needing a file named `.env` with the following variables:
 
-You will be needing a file named `.env` with the following variables
 ```bash
 SSO_CLIENT_ID=<change>
 SSO_CLIENT_SECRET=<change>
-ENVIRONMENT=qa
+ENVIRONMENT=development
 ```
-While most of the tests work on the development deployment, some fail and need the production one. This is the reason we are setting `ENVIRONMENT=qa`.
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 pip install -r testing-requirements.txt
 pip install -e .
@@ -454,12 +451,12 @@
 
 ### Should I be using `runregistry_api_client` for getting OMS data?
 
 No*.
 
 Our recommendation is to query Run Registry only for data that RR is responsible for.
 
-<small>*It's not that you can't, it's just that this puts extra burden on the application, making it slow for everyone.</small> 
+<small>*It's not that you can't, it's just that this puts extra burden on the application, making it slow for everyone.</small>
 
 ### Is the token stored somewhere and reused?
 
-No, almost every function call gets a new token. This is not ideal, and it may be improved in the future.   
+No, almost every function call gets a new token. This is not ideal, and it may be improved in the future.
```

### Comparing `runregistry-1.0.0/runregistry/attributes.py` & `runregistry-1.1.0/runregistry/attributes.py`

 * *Files identical despite different names*

### Comparing `runregistry-1.0.0/runregistry/runregistry.py` & `runregistry-1.1.0/runregistry/runregistry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import os
+import time
 import json
 import requests
-import time
 from dotenv import load_dotenv
 from cernrequests import get_api_token, get_with_token
-from runregistry.utils import transform_to_rr_run_filter, transform_to_rr_dataset_filter
+from runregistry.utils import (
+    transform_to_rr_run_filter,
+    transform_to_rr_dataset_filter,
+    __parse_runs_arg,
+)
 
 load_dotenv()
 
+
 # Silence unverified HTTPS warning:
 # urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 PAGE_SIZE = 50
 
+# Offline table
+WAITING_DQM_GUI_CONSTANT = "waiting dqm gui"
+
 staging_cert = ""
 staging_key = ""
 api_url = ""
 use_cookies = True
 email = "api@api"
 client_id = os.environ.get("SSO_CLIENT_ID")
 client_secret = os.environ.get("SSO_CLIENT_SECRET")
@@ -356,15 +364,15 @@
 # advanced RR operations ==============================================================================
 # Online Table
 def move_runs(from_, to_, run=None, runs=[], **kwargs):
     """
     move run/runs from one state to another
     """
     if not run and not runs:
-        print("move_runs(): no 'run' and 'runs' arguments were provided, return")
+        print("move_runs(): no 'run' and 'runs' arguments were provided")
         return
 
     states = ["SIGNOFF", "OPEN", "COMPLETED"]
     if from_ not in states or to_ not in states:
         print(
             "move_runs(): get states '",
             from_,
@@ -384,87 +392,105 @@
         payload = json.dumps({"run_number": run})
         return requests.post(url, headers=headers, data=payload)
 
     answers = []
     for run_number in runs:
         payload = json.dumps({"run_number": run_number})
         answer = requests.post(url, headers=headers, data=payload).json()
-        answers += [answer]
+        answers.append(answer)
 
     return answers
 
 
 def make_significant_runs(run=None, runs=[], **kwargs):
     """
     mark run/runs significant
     """
     if not run and not runs:
-        print("move_runs(): no 'run' and 'runs' arguments were provided, return")
+        print("make_significant_runs(): no 'run' and 'runs' arguments were provided")
         return
 
     url = "%s/runs/mark_significant" % (api_url)
 
     headers = _get_headers(token=_get_token())
 
     if run:
         data = {"run_number": run}
         return requests.post(url, headers=headers, json=data)
 
     answers = []
     for run_number in runs:
         data = {"run_number": run}
         answer = requests.post(url, headers=headers, json=data)
-        answers += [answer]
+        answers.append(answer)
 
     return answers
 
 
-def reset_RR_attributes_and_refresh_runs(run=None, runs=[], **kwargs):
+def reset_RR_attributes_and_refresh_runs(runs=[], **kwargs):
     """
     reset RR attributes and refresh run/runs
     """
-    if not run and not runs:
-        print("move_runs(): no 'run' and 'runs' arguments were provided, return")
+    runs = __parse_runs_arg(runs)
+    if not runs:
+        print(
+            "reset_RR_attributes_and_refresh_runs(): no 'runs' arguments were provided"
+        )
         return
+    headers = _get_headers(token=_get_token())
+    answers = []
+    for run_number in runs:
+        url = "%s/runs/reset_and_refresh_run/%d" % (api_url, run_number)
+        answer = requests.post(url, headers=headers)
+        answers.append(answer)
 
-    url = "%s/runs/reset_and_refresh_run" % (api_url)
+    return answers
 
-    headers = _get_headers(token=_get_token())
 
-    if run:
-        url = "%s/runs/reset_and_refresh_run/%d" % (api_url, run)
-        return requests.post(url, headers=headers)
+def manually_refresh_components_statuses_for_runs(runs=[], **kwargs):
+    """
+    Refreshes all components statuses for the runs specified that have not been
+    changed by shifters.
+    """
+    runs = __parse_runs_arg(runs)
+
+    if not runs:
+        print(
+            "manually_refresh_components_statuses_for_runs(): no 'runs' arguments were provided, return"
+        )
+        return
 
+    headers = _get_headers(token=_get_token())
     answers = []
     for run_number in runs:
-        url = "%s/runs/reset_and_refresh_run/%d" % (api_url, run_number)
+        url = "%s/runs/refresh_run/%d" % (api_url, run_number)
         answer = requests.post(url, headers=headers)
-        answers += [answer]
+        answers.append(answer)
 
     return answers
 
 
 def edit_rr_lumisections(
     run,
     lumi_start,
     lumi_end,
     component,
     status,
     comment="",
     cause="",
     dataset_name="online",
-    **kwargs
+    **kwargs,
 ):
     """
     WIP edit RR lumisections attributes
     """
     states = ["GOOD", "BAD", "STANDBY", "EXCLUDED", "NONSET"]
     if status not in states:
         print(
-            "move_runs(): get status '",
+            "edit_rr_lumisections(): get status '",
             status,
             "', while allowed statuses are ",
             states,
             ", return",
         )
         return
 
@@ -481,26 +507,23 @@
                 "cause": cause,
             },
             "run_number": run,
             "dataset_name": dataset_name,
             "component": component,
         }
     )
-    return requests.post(url, headers=headers, data=payload)
-
-
-# Offline table
-WAITING_DQM_GUI_CONSTANT = "waiting dqm gui"
+    return requests.put(url, headers=headers, data=payload)
 
 
 def move_datasets(
     from_, to_, dataset_name, workspace="global", run=None, runs=[], **kwargs
 ):
     """
-    move offline dataset/datasets from one state to another
+    Move offline dataset/datasets from one state to another.
+    Requires a privileged token.
     """
     if not run and not runs:
         print("move_datasets(): no 'run' and 'runs' arguments were provided, return")
         return
 
     states = ["SIGNOFF", "OPEN", "COMPLETED", WAITING_DQM_GUI_CONSTANT]
     if from_ not in states or to_ not in states:
@@ -524,13 +547,52 @@
             {"run_number": run, "dataset_name": dataset_name, "workspace": workspace}
         )
         return requests.post(url, headers=headers, data=payload)
 
     answers = []
     for run_number in runs:
         payload = json.dumps(
-            {"run_number": run, "dataset_name": dataset_name, "workspace": workspace}
+            {
+                "run_number": run_number,
+                "dataset_name": dataset_name,
+                "workspace": workspace,
+            }
         )
         answer = requests.post(url, headers=headers, data=payload).json()
-        answers += [answer]
+        answers.append(answer)
 
     return answers
+
+
+def change_run_class(run_numbers, new_class):
+    """
+    Method for changing the class of a run (or runs),
+    e.g. from "Commissioning22" to "Cosmics22".
+    Requires a privileged token.
+    """
+    headers = _get_headers(token=_get_token())
+
+    def _execute_request_for_single_run(run_number, new_class):
+        payload = json.dumps({"class": new_class})
+        return requests.put(
+            url="%s/manual_run_edit/%s/class" % (api_url, run_number),
+            headers=headers,
+            data=payload,
+        )
+
+    if not isinstance(new_class, str):
+        raise Exception('Invalid input for "new_class"')
+    answers = []
+    if isinstance(run_numbers, list):
+        for run_number in run_numbers:
+            if not isinstance(run_number, int):
+                raise Exception(
+                    "Invalid run number value found in run_numbers. Please provide a list of numbers."
+                )
+            answers.append(_execute_request_for_single_run(run_number, new_class))
+    elif isinstance(run_numbers, int):
+        answers.append(_execute_request_for_single_run(run_numbers, new_class))
+    else:
+        raise Exception(
+            'Invalid input for "run_numbers". Please provide a list of numbers.'
+        )
+    return answers
```

### Comparing `runregistry-1.0.0/runregistry/utils.py` & `runregistry-1.1.0/runregistry/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,35 @@
-import json
-
 from runregistry.attributes import (
     run_table_attributes,
     run_triplet_attributes,
     run_rr_attributes,
     run_oms_attributes,
     dataset_table_attributes,
     dataset_attributes,
     dataset_triplet_attributes,
 )
 
 
+def __parse_runs_arg(runs):
+    """
+    Helper function to parse runs arguments.
+    Returns a list.
+    """
+    if isinstance(runs, int):
+        return [runs]
+    elif isinstance(runs, str):
+        try:
+            runs = int(runs)
+            return [runs]
+        except:
+            return []
+    elif isinstance(runs, list):
+        return runs
+
+
 def transform_to_rr_run_filter(run_filter):
     """
     Transforms a filter to a compatible filter that RR back end understands.
     :param run_filter: a filter that the user inputs into the api client
     :return: returns a filter that runregistry back end understands.
     """
     if run_filter == None:
```

### Comparing `runregistry-1.0.0/runregistry.egg-info/PKG-INFO` & `runregistry-1.1.0/runregistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: runregistry
-Version: 1.0.0
+Version: 1.1.0
 Summary: CMS Run Registry client
 Home-page: https://github.com/cms-DQM/runregistry_api_client/
 Author: Fabio Espinosa
 Author-email: f.e@cern.ch
 Maintainer: CMS DQM team
 Maintainer-email: cms-dqm-coreTeam@cern.ch
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: cernrequests
+Requires-Dist: python-dotenv
 
 ![Build Status](https://github.com/cms-DQM/runregistry_api_client/actions/workflows/test_package.yaml/badge.svg)
 
 # Run Registry Client
 
 Python client to retrieve and query data from [CMS Run Registry](https://cmsrunregistry.web.cern.ch).
 
@@ -27,48 +30,48 @@
 
 ## Python version and Virtual env
 
 Python version>=3.6 is required for this package.
 A virtual environment is also required, if you are in lxplus you should run the following commands:
 
 ```bash
-virtualenv -p `which python3` venv
+virtualenv -p $(which python3) venv
 source venv/bin/activate
 ```
 
 ## Installation
 
 ```bash
 pip install runregistry
 ```
 
 ## Authentication Prerequisites
 
 > **Warning**
-> Grid certificates have been deprecated by CERN. As of version `1.0.0`, the `runregistry` 
-> client only works with a client ID and a secret. 
+> Grid certificates have been deprecated by CERN. As of version `1.0.0`, the `runregistry`
+> client only works with a client ID and a secret.
 
-You will need to create an SSO registration for your application which is going to be using the runregistry API client. 
+You will need to create an SSO registration for your application which is going to be using the runregistry API client.
 
 Instructions on how to do it can be found on the [`cernrequests`](https://github.com/CMSTrackerDPG/cernrequests) GitHub page.
 
-Once you have a client ID and a secret, you will need to store them in a file named `.env`. A [sample file](.env_sample) is provided so that you can edit it and rename it to `.env`. 
+Once you have a client ID and a secret, you will need to store them in a file named `.env`. A [sample file](.env_sample) is provided so that you can edit it and rename it to `.env`.
 
 Alternatively, you can run `export SSO_CLIENT_ID=...` and `export SSO_CLIENT_SECRET=...` on the same terminal that you will be running your python script in.
 
 ## Usage
 
-### Get a single run (get_run):
+### Get a single run (get_run)
 
 ```python
 import runregistry
 run = runregistry.get_run(run_number=328762)
 ```
 
-### Query several runs (get_runs):
+### Query several runs (get_runs)
 
 ```python
 import runregistry
 runs = runregistry.get_runs(filter={
    'run_number':{
       'or': [328762, 323555, 323444]
     }
@@ -404,15 +407,15 @@
     ```python
     runregistry.make_significant_runs(run=362761)
     ```
 2. Reset RR attributes and reload data from OMS:
     ```python
     runregistry.reset_RR_attributes_and_refresh_runs(run=362761)
     ```
-3. Move runs from one state to another: 
+3. Move runs from one state to another:
     ```python
     runregistry.move_runs("OPEN", "SIGNOFF", run=362761)
     ```
 
 ## Troubleshooting
 
 ### Support
@@ -424,28 +427,25 @@
 ```bash
 python3 -m pip install --upgrade pip build twine
 python3 -m build
 python3 -m twine upload --skip-existing --repository pypi dist/*
 ```
 Instructions from [here](https://packaging.python.org/en/latest/tutorials/packaging-projects/).
 
-## Testing
+## Running the tests
 
 ### Locally
 
-> **TODO**
-> Remove the qa environment after migration.
+You will be needing a file named `.env` with the following variables:
 
-You will be needing a file named `.env` with the following variables
 ```bash
 SSO_CLIENT_ID=<change>
 SSO_CLIENT_SECRET=<change>
-ENVIRONMENT=qa
+ENVIRONMENT=development
 ```
-While most of the tests work on the development deployment, some fail and need the production one. This is the reason we are setting `ENVIRONMENT=qa`.
 
 ```bash
 python3 -m venv venv
 source venv/bin/activate
 pip install -r requirements.txt
 pip install -r testing-requirements.txt
 pip install -e .
@@ -466,12 +466,12 @@
 
 ### Should I be using `runregistry_api_client` for getting OMS data?
 
 No*.
 
 Our recommendation is to query Run Registry only for data that RR is responsible for.
 
-<small>*It's not that you can't, it's just that this puts extra burden on the application, making it slow for everyone.</small> 
+<small>*It's not that you can't, it's just that this puts extra burden on the application, making it slow for everyone.</small>
 
 ### Is the token stored somewhere and reused?
 
-No, almost every function call gets a new token. This is not ideal, and it may be improved in the future.   
+No, almost every function call gets a new token. This is not ideal, and it may be improved in the future.
```

### Comparing `runregistry-1.0.0/setup.py` & `runregistry-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `runregistry-1.0.0/tests/sample_json_generation_from_CTPPS.py` & `runregistry-1.1.0/tests/sample_json_generation_from_CTPPS.py`

 * *Files identical despite different names*

### Comparing `runregistry-1.0.0/tests/stress_test.py` & `runregistry-1.1.0/tests/stress_test.py`

 * *Files identical despite different names*

### Comparing `runregistry-1.0.0/tests/test_client.py` & `runregistry-1.1.0/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import pytest
 import json
 
 from runregistry.runregistry import (
     get_run,
     get_runs,
     get_dataset_names_of_run,
@@ -45,15 +43,15 @@
     # Gets runs between run number 309000 and 310000
     filter_run = {"run_number": {"and": [{">": 309000}, {"<": 310000}]}}
     runs = get_runs(filter=filter_run)
     assert len(runs) > 0
     # Gets runs that contain lumisections that classified DT as GOOD AND lumsiections that classified hcal as STANDBY
     filter_run = {
         "run_number": {"and": [{">": 309000}, {"<": 310000}]},
-        "dt-dt": "GOOD"
+        "dt-dt": "GOOD",
         # 'hcal': 'STANDBY'
     }
 
     runs = get_runs(filter=filter_run)
     assert len(runs) > 0
     runs = []
```

### Comparing `runregistry-1.0.0/tests/test_utils.py` & `runregistry-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

