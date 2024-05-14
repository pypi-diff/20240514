# Comparing `tmp/openai_priority_loadbalancer-0.0.5.tar.gz` & `tmp/openai_priority_loadbalancer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-0.0.5.tar", last modified: Tue May 14 04:07:36 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-0.0.6.tar", last modified: Tue May 14 18:57:29 2024, max compression
```

## Comparing `openai_priority_loadbalancer-0.0.5.tar` & `openai_priority_loadbalancer-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 04:07:36.743723 openai_priority_loadbalancer-0.0.5/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    11502 2024-05-14 04:06:03.000000 openai_priority_loadbalancer-0.0.5/PACKAGE_README.md
--rw-rw-rw-   0        0        0    12302 2024-05-14 04:07:36.740720 openai_priority_loadbalancer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    12280 2024-05-14 03:01:51.000000 openai_priority_loadbalancer-0.0.5/README.md
--rw-rw-rw-   0        0        0      670 2024-05-14 04:07:23.000000 openai_priority_loadbalancer-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 04:07:36.745095 openai_priority_loadbalancer-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 04:07:36.639913 openai_priority_loadbalancer-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 04:07:36.675841 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       44 2024-05-14 04:07:11.000000 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0    10300 2024-05-13 20:56:00.000000 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-14 04:07:36.737350 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    12302 2024-05-14 04:07:36.000000 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2024-05-14 04:07:36.000000 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 04:07:36.000000 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-14 04:07:36.000000 openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.233017 openai_priority_loadbalancer-0.0.6/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    11693 2024-05-14 18:56:49.000000 openai_priority_loadbalancer-0.0.6/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    12528 2024-05-14 18:57:29.228920 openai_priority_loadbalancer-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12513 2024-05-14 04:17:29.000000 openai_priority_loadbalancer-0.0.6/README.md
+-rw-rw-rw-   0        0        0      711 2024-05-14 18:57:02.000000 openai_priority_loadbalancer-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:57:29.233813 openai_priority_loadbalancer-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.064963 openai_priority_loadbalancer-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.130833 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       44 2024-05-14 04:07:11.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    10367 2024-05-14 18:54:50.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:57:29.217677 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    12528 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-14 18:57:29.000000 openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-0.0.5/LICENSE` & `openai_priority_loadbalancer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-0.0.5/PACKAGE_README.md` & `openai_priority_loadbalancer-0.0.6/PACKAGE_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OpenAI Load Balancer
+# OpenAI Priority Load Balancer
 
 Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
 
 - Distribution of requests over multiple consumption instances to mitigate throttling.
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
 - Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
 
@@ -80,14 +80,18 @@
     )
     ```
 
 ### Using the Load Balancer
 
 As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
 
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
 ## Distribution of Requests
 
 ### Across Different Priorities
 
 Requests are made to the highest priority backend that is available. For example:
 
 - Priority 1, when available, will always supersede priority 2.
```

### Comparing `openai_priority_loadbalancer-0.0.5/PKG-INFO` & `openai_priority_loadbalancer-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openai>=1.17.0
 
-# OpenAI Load Balancer
+# OpenAI Priority Load Balancer
 
 Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
 
 - Distribution of requests over multiple consumption instances to mitigate throttling.
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
 - Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
 
@@ -94,14 +95,18 @@
     )
     ```
 
 ### Using the Load Balancer
 
 As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
 
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
 ## Distribution of Requests
 
 ### Across Different Priorities
 
 Requests are made to the highest priority backend that is available. For example:
 
 - Priority 1, when available, will always supersede priority 2.
```

### Comparing `openai_priority_loadbalancer-0.0.5/README.md` & `openai_priority_loadbalancer-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,180 +1,184 @@
-# Python OpenAI Load Balancer
-
-Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
-
-- Distribution of requests over multiple consumption instances to mitigate throttling.
-- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
-- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
-
-While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
-
-And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
-
-Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
-
-## Disclaimer
-
-**This is a pseudo load-balancer.**
-
-When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
-immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
-
-Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
-
-## Attribution
-
-This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
-
-## Prerequisites
-
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
-It's also good to have some knowledge of authentication and identities.
-
-## Authentication
-
-Locally, you can log into Azure via the CLI and the steps below and use the `AzureDefaultCredential` (what I use in my example). When deploying this application in Azure, it's recommended to use a managed identity for authentication. It's best to avoid using the Azure OpenAI instances' keys as that could a) accidentally leave credentials in your source code, and b) the keys are different for each instance, which would probably require expanding upon the `Backends` class. Best to just avoid keys.
-
-## Single Requestor Model
-
-I started with a single-requestor model to experiment with the algorithm to select backends. This model is not typically used, as most workloads run multiple Python workers in parallel. Nevertheless, I left the files in the repo with the `single-requestor` suffix.
-
-## Getting Started
-
-### Cloning the repo & Preparing the python environment
-
-1. Clone the repo.
-1. Open the cloned repo folder in VS Code.
-1. Open a terminal session in VS Code.
-1. Run [setup-python.ps1](./setup-python.ps1) to prepare the python environment.
-
-### Configuration
-
-For the load-balanced approach, please use the same model across all instances.
-
-1. Open [aoai.py](./aoai.py).
-1. Replace `<your-aoai-model>` with the name of your Azure OpenAI model.
-1. Replace `<your-aoai-instance>` with the primary/single Azure OpenAI instance.
-1. Replace `<your-aoai-instance-1>`, `<your-aoai-instance-2>`, `<your-aoai-instance-3>` with all the Azure OpenAI instances you want to load-balance across. Delete entries you don't need. See [Load Balancer Configuration](#load-balancer-configuration) for details.
-1. Replace the value for variable `num_of_requests` with the number of requests you wish to execute.
-
-### Credentials
-
-Locally, your `AzureDefaultCredential` is used. Each Azure OpenAI instance must be configured with the `Cognitive Services OpenAI` User role for your Azure credential (the identity you use after logging in). This ensures that you can use your credential across all Azure OpenAI instances.
-
-When running in Azure, it's advised to use managed identities.
-
-1. Log in with `az login`.
-
-## Execution
-
-1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
-1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-![Parallel Execution](./assets/parallel-execution.png)
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
-
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
-
-## Load Balancer Configuration
-
-At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
-
-I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
-The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
-While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
-
-### One Backend
-
-This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Two Backends with Same Priority
-
-Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Same Priority
-
-Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Two Different Priorities
-
-The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
-]
-```
-
-### Three Backends with Three Different Priorities
-
-An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
-]
-```
+# Python OpenAI Load Balancer
+
+TL;DR! How do I [start](#getting-started)?
+
+---
+
+Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
+
+- Distribution of requests over multiple consumption instances to mitigate throttling.
+- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
+- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
+
+While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
+
+And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
+
+Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
+
+## Disclaimer
+
+**This is a pseudo load-balancer.**
+
+When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
+immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
+
+Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
+
+## Attribution
+
+This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
+
+## Prerequisites
+
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
+It's also good to have some knowledge of authentication and identities.
+
+## Authentication
+
+Locally, you can log into Azure via the CLI and the steps below and use the `AzureDefaultCredential` (what I use in my example). When deploying this application in Azure, it's recommended to use a managed identity for authentication. It's best to avoid using the Azure OpenAI instances' keys as that could a) accidentally leave credentials in your source code, and b) the keys are different for each instance, which would probably require expanding upon the `Backends` class. Best to just avoid keys.
+
+## Single Requestor Model
+
+I started with a single-requestor model to experiment with the algorithm to select backends. This model is not typically used, as most workloads run multiple Python workers in parallel. Nevertheless, I left the files in the repo with the `single-requestor` suffix.
+
+## Getting Started
+
+### Cloning the repo & Preparing the python environment
+
+1. Clone the repo.
+1. Open the cloned repo folder in VS Code.
+1. Open a terminal session in VS Code.
+1. Run [setup-python.ps1](./setup-python.ps1) to prepare the python environment.
+
+### Configuration
+
+For the load-balanced approach, please use the same model across all instances.
+
+1. Open [aoai.py](./aoai.py).
+1. Replace `<your-aoai-model>` with the name of your Azure OpenAI model.
+1. Replace `<your-aoai-instance>` with the primary/single Azure OpenAI instance.
+1. Replace `<your-aoai-instance-1>`, `<your-aoai-instance-2>`, `<your-aoai-instance-3>` with all the Azure OpenAI instances you want to load-balance across. Delete entries you don't need. See [Load Balancer Configuration](#load-balancer-configuration) for details.
+1. Replace the value for variable `num_of_requests` with the number of requests you wish to execute.
+
+### Credentials
+
+Locally, your `AzureDefaultCredential` is used. Each Azure OpenAI instance must be configured with the `Cognitive Services OpenAI` User role for your Azure credential (the identity you use after logging in). This ensures that you can use your credential across all Azure OpenAI instances.
+
+When running in Azure, it's advised to use managed identities.
+
+1. Log in with `az login`.
+
+## Execution
+
+1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
+1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+![Parallel Execution](./assets/parallel-execution.png)
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
+
+## Load Balancer Configuration
+
+At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+
+I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
+The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
+While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
+
+### One Backend
+
+This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Two Backends with Same Priority
+
+Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Same Priority
+
+Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Two Different Priorities
+
+The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
+]
+```
+
+### Three Backends with Three Different Priorities
+
+An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
+]
+```
```

### Comparing `openai_priority_loadbalancer-0.0.5/pyproject.toml` & `openai_priority_loadbalancer-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "openai_priority_loadbalancer"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Simon Kurtz", email="simonkurtz@gmail.com" },
 ]
 description = "A multi-backend, prioritization load balancer for OpenAI"
 readme = "PACKAGE_README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "openai>=1.17.0",
+]
 [project.urls]
 Homepage = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer"
 Issues = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues"
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py` & `openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime, MINYEAR, MAXYEAR, timedelta, timezone
 from dateutil.tz import tzutc
 from httpx import Client, Response, BaseTransport, AsyncBaseTransport, AsyncClient
 from typing import List
+import logging
 import random
 import traceback
 
 class Backend:
     # Constructor
     def __init__(self, host: str, priority: int):
         self.host = host
@@ -19,24 +20,25 @@
 class BaseLoadBalancer():
     # Constructor
     def __init__(self, transport, backends: List[Backend]):
         self._transport = transport
         self.backends = backends
         self._backend_index = -1
         self._remaining_backends = 1
+        self._log = logging.getLogger("openai-priority-loadbalancer")     # https://www.loggly.com/ultimate-guide/python-logging-basics/
 
     # "Protected" Methods
     def _check_throttling(self):
         min_datetime = datetime(MINYEAR, 1, 1, tzinfo = tzutc())
 
         for backend in self.backends:
             if backend.is_throttling and datetime.now(tzutc()) >= backend.retry_after:
                 backend.is_throttling = False
                 backend.retry_after = min_datetime
-                print(f"{datetime.now()}:   Backend {backend.host} is no longer throttling.")
+                self._log.info(f"Backend {backend.host} is no longer throttling.")
 
     def _get_backend_index(self):
         # This is the main logic to pick the backend to be used
         selected_priority = float('inf')
         available_backends = []
 
         for i in range(len(self.backends)):
@@ -78,21 +80,21 @@
 
         for backend in self.backends:
             if backend.is_throttling and backend.retry_after < soonest_retry_after:
                 soonest_retry_after = backend.retry_after
                 soonest_backend = backend.host
 
         delay = int((soonest_retry_after - datetime.now(timezone.utc)).total_seconds()) + 1     # Add a 1 second buffer to ensure we don't retry too early
-        print(f"{datetime.now()}:   Soonest Retry After: {soonest_backend} - {str(delay)} second(s)")
+        self._log.info(f"Soonest Retry After: {soonest_backend} - {str(delay)} second(s)")
         return delay
 
     def _return_429(self):
-        print(f"{datetime.now()}:   No backend available!")
+        self._log.warning("No backend available!")
         retry_after = str(self._get_soonest_retry_after())
-        print(f"{datetime.now()}:   Returning HTTP 429 with Retry-After header value of {retry_after} second(s).")
+        self._log.info(f"Returning HTTP 429 with Retry-After header value of {retry_after} second(s).")
         return Response(429, content = '', headers={'Retry-After': retry_after})
 
 class AsyncLoadBalancer(BaseLoadBalancer):
     # Constructor
     def __init__(self, backends: List[Backend]):
         super().__init__(AsyncClient(), backends)
 
@@ -114,44 +116,45 @@
             request.headers = request.headers.copy()    # Create a mutable copy of the headers
             request.headers['host'] = self.backends[backend_index].host
 
             # Send the request to the backend
             try:
                 response = await self._transport.send(request)
             except Exception as e:
-                traceback.print_exc()
+                self._log.error(traceback.print_exc())
 
             if response is not None and (response.status_code == 429 or response.status_code >= 500):
                 # If the server is throttling or there's a server error, retry with a different server
-                print(f"{datetime.now()}:   Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+                self._log.info(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+
                 retry_after = int(response.headers.get('Retry-After', '-1'))
 
                 if retry_after == -1:
                     retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
 
                 if retry_after == -1:
                     retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
 
-                print(f"{datetime.now()}:   Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
+                self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
 
                 backend = self.backends[backend_index]
                 backend.is_throttling = True
                 backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
                 self._get_remaining_backends()
                 continue
 
             elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
                 # Successful requests
-                print(f"{datetime.now()}:   Request sent to server: {request.url}, Status code: {response.status_code}")
+                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
                 self.backends[backend_index].successful_call_count += 1
                 break
 
             else:
                 # Would likely be a 4xx error other than 429
-                print(f"{datetime.now()}:   Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
                 break
 
         if self._remaining_backends == 0:
             return self._return_429()
 
         return response
 
@@ -179,43 +182,44 @@
             headers['host'] = self.backends[backend_index].host
             request.headers = headers           # Assign the modified headers back to request.headers
 
             # Send the request to the backend
             try:
                 response = self._transport.send(request)
             except Exception as e:
-                traceback.print_exc()
+                self._log.error(traceback.print_exc())
 
             if response is not None and (response.status_code == 429 or response.status_code >= 500):
                 # If the server is throttling or there's a server error, retry with a different server
-                print(f"{datetime.now()}:   Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+                self._log.warning(f"Request sent to server: {request.url}, Status Code: {response.status_code} - FAIL")
+
                 retry_after = int(response.headers.get('Retry-After', '-1'))
 
                 if retry_after == -1:
                     retry_after = int(response.headers.get('x-ratelimit-reset-requests', '-1'))
 
                 if retry_after == -1:
                     retry_after = int(response.headers.get('x-ratelimit-reset-requests', '10'))
 
-                print(f"{datetime.now()}:   Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
+                self._log.info(f"Backend {self.backends[backend_index].host} is throttling. Retry after {retry_after} second(s).")
 
                 backend = self.backends[backend_index]
                 backend.is_throttling = True
                 backend.retry_after = datetime.now(tzutc()) + timedelta(seconds = retry_after)
                 self._get_remaining_backends()
                 continue
 
             elif response is not None and (response.status_code >= 200 and response.status_code <= 399):
                 # Successful requests
-                print(f"{datetime.now()}:   Request sent to server: {request.url}, Status code: {response.status_code}")
+                self._log.info(f"Request sent to server: {request.url}, Status code: {response.status_code}")
                 self.backends[backend_index].successful_call_count += 1
                 break
 
             else:
                 # Would likely be a 4xx error other than 429
-                print(f"{datetime.now()}:   Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
+                self._log.warning(f"Request sent to server: {request.url}, Status code: {response.status_code} - FAIL")
                 break
 
         if self._remaining_backends == 0:
             return self._return_429()
 
         return response
```

### Comparing `openai_priority_loadbalancer-0.0.5/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-0.0.6/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openai>=1.17.0
 
-# OpenAI Load Balancer
+# OpenAI Priority Load Balancer
 
 Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
 
 - Distribution of requests over multiple consumption instances to mitigate throttling.
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
 - Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
 
@@ -94,14 +95,18 @@
     )
     ```
 
 ### Using the Load Balancer
 
 As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
 
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
 ## Distribution of Requests
 
 ### Across Different Priorities
 
 Requests are made to the highest priority backend that is available. For example:
 
 - Priority 1, when available, will always supersede priority 2.
```

