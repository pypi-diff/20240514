# Comparing `tmp/bsv-sdk-0.1.1.tar.gz` & `tmp/bsv_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsv-sdk-0.1.1.tar", last modified: Tue Apr  9 02:36:55 2024, max compression
+gzip compressed data, was "bsv_sdk-0.2.0.tar", last modified: Tue May 14 01:54:42 2024, max compression
```

## Comparing `bsv-sdk-0.1.1.tar` & `bsv_sdk-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,55 @@
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-04-09 02:36:55.492012 bsv-sdk-0.1.1/
--rw-r--r--   0 aaron67    (501) staff       (20)     2241 2024-04-09 02:10:19.000000 bsv-sdk-0.1.1/LICENSE.txt
--rw-r--r--   0 aaron67    (501) staff       (20)     3254 2024-04-09 02:36:55.491958 bsv-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 aaron67    (501) staff       (20)     2498 2024-04-09 01:30:45.000000 bsv-sdk-0.1.1/README.md
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-04-09 02:36:55.490959 bsv-sdk-0.1.1/bsv/
--rw-r--r--   0 aaron67    (501) staff       (20)       52 2024-04-09 02:36:51.000000 bsv-sdk-0.1.1/bsv/__init__.py
--rw-r--r--   0 aaron67    (501) staff       (20)       44 2024-04-09 01:46:44.000000 bsv-sdk-0.1.1/bsv/hello.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-04-09 02:36:55.491793 bsv-sdk-0.1.1/bsv_sdk.egg-info/
--rw-r--r--   0 aaron67    (501) staff       (20)     3254 2024-04-09 02:36:55.000000 bsv-sdk-0.1.1/bsv_sdk.egg-info/PKG-INFO
--rw-r--r--   0 aaron67    (501) staff       (20)      258 2024-04-09 02:36:55.000000 bsv-sdk-0.1.1/bsv_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 aaron67    (501) staff       (20)        1 2024-04-09 02:36:55.000000 bsv-sdk-0.1.1/bsv_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 aaron67    (501) staff       (20)       18 2024-04-09 02:36:55.000000 bsv-sdk-0.1.1/bsv_sdk.egg-info/requires.txt
--rw-r--r--   0 aaron67    (501) staff       (20)        4 2024-04-09 02:36:55.000000 bsv-sdk-0.1.1/bsv_sdk.egg-info/top_level.txt
--rw-r--r--   0 aaron67    (501) staff       (20)      104 2024-04-09 02:08:18.000000 bsv-sdk-0.1.1/pyproject.toml
--rw-r--r--   0 aaron67    (501) staff       (20)      775 2024-04-09 02:36:55.492205 bsv-sdk-0.1.1/setup.cfg
--rw-r--r--   0 aaron67    (501) staff       (20)      315 2024-04-09 02:36:15.000000 bsv-sdk-0.1.1/setup.py
-drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-04-09 02:36:55.491642 bsv-sdk-0.1.1/tests/
--rw-r--r--   0 aaron67    (501) staff       (20)       98 2024-04-09 02:36:15.000000 bsv-sdk-0.1.1/tests/test_hello.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.955035 bsv_sdk-0.2.0/
+-rw-r--r--   0 aaron67    (501) staff       (20)     2241 2024-04-09 02:51:01.000000 bsv_sdk-0.2.0/LICENSE.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)     3960 2024-05-14 01:54:42.954983 bsv_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 aaron67    (501) staff       (20)     3209 2024-05-14 01:01:38.000000 bsv_sdk-0.2.0/README.md
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.947356 bsv_sdk-0.2.0/bsv/
+-rw-r--r--   0 aaron67    (501) staff       (20)      214 2024-05-14 01:54:28.000000 bsv_sdk-0.2.0/bsv/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      934 2024-05-04 20:20:27.000000 bsv_sdk-0.2.0/bsv/aes_cbc.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1549 2024-04-26 06:30:33.000000 bsv_sdk-0.2.0/bsv/base58.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     6737 2024-05-14 01:45:21.000000 bsv_sdk-0.2.0/bsv/constants.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2531 2024-04-26 06:26:14.000000 bsv_sdk-0.2.0/bsv/curve.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2952 2024-05-04 20:35:20.000000 bsv_sdk-0.2.0/bsv/encrypted_message.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      613 2024-04-26 03:54:23.000000 bsv_sdk-0.2.0/bsv/hash.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.948354 bsv_sdk-0.2.0/bsv/hd/
+-rw-r--r--   0 aaron67    (501) staff       (20)      266 2024-04-26 13:00:04.000000 bsv_sdk-0.2.0/bsv/hd/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     7070 2024-05-14 01:51:49.000000 bsv_sdk-0.2.0/bsv/hd/bip32.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     4015 2024-04-26 13:00:04.000000 bsv_sdk-0.2.0/bsv/hd/bip39.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1926 2024-05-14 01:46:25.000000 bsv_sdk-0.2.0/bsv/hd/bip44.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.948860 bsv_sdk-0.2.0/bsv/hd/wordlist/
+-rw-r--r--   0 aaron67    (501) staff       (20)     8192 2024-04-26 13:00:04.000000 bsv_sdk-0.2.0/bsv/hd/wordlist/chinese_simplified.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)    15164 2024-04-26 13:00:04.000000 bsv_sdk-0.2.0/bsv/hd/wordlist/english.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)    14429 2024-05-14 01:25:19.000000 bsv_sdk-0.2.0/bsv/keys.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.949725 bsv_sdk-0.2.0/bsv/script/
+-rw-r--r--   0 aaron67    (501) staff       (20)      102 2024-05-13 22:42:57.000000 bsv_sdk-0.2.0/bsv/script/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1277 2024-05-14 01:06:05.000000 bsv_sdk-0.2.0/bsv/script/script.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     7292 2024-05-14 01:39:01.000000 bsv_sdk-0.2.0/bsv/script/type.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.950812 bsv_sdk-0.2.0/bsv/service/
+-rw-r--r--   0 aaron67    (501) staff       (20)      116 2024-05-13 22:43:03.000000 bsv_sdk-0.2.0/bsv/service/__init__.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2027 2024-05-14 01:21:58.000000 bsv_sdk-0.2.0/bsv/service/provider.py
+-rw-r--r--   0 aaron67    (501) staff       (20)      780 2024-05-14 01:17:28.000000 bsv_sdk-0.2.0/bsv/service/service.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2089 2024-05-14 01:23:13.000000 bsv_sdk-0.2.0/bsv/service/whatsonchain.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    18606 2024-05-14 01:32:19.000000 bsv_sdk-0.2.0/bsv/transaction.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2614 2024-05-14 01:28:37.000000 bsv_sdk-0.2.0/bsv/unspent.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     9336 2024-05-14 01:32:09.000000 bsv_sdk-0.2.0/bsv/utils.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     7088 2024-05-14 01:18:09.000000 bsv_sdk-0.2.0/bsv/wallet.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.954728 bsv_sdk-0.2.0/bsv_sdk.egg-info/
+-rw-r--r--   0 aaron67    (501) staff       (20)     3960 2024-05-14 01:54:42.000000 bsv_sdk-0.2.0/bsv_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 aaron67    (501) staff       (20)      929 2024-05-14 01:54:42.000000 bsv_sdk-0.2.0/bsv_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)        1 2024-05-14 01:54:42.000000 bsv_sdk-0.2.0/bsv_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)       33 2024-05-14 01:54:42.000000 bsv_sdk-0.2.0/bsv_sdk.egg-info/requires.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)        4 2024-05-14 01:54:42.000000 bsv_sdk-0.2.0/bsv_sdk.egg-info/top_level.txt
+-rw-r--r--   0 aaron67    (501) staff       (20)      104 2024-04-09 02:51:01.000000 bsv_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0 aaron67    (501) staff       (20)      834 2024-05-14 01:54:42.955295 bsv_sdk-0.2.0/setup.cfg
+-rw-r--r--   0 aaron67    (501) staff       (20)      315 2024-04-09 02:51:01.000000 bsv_sdk-0.2.0/setup.py
+drwxr-xr-x   0 aaron67    (501) staff       (20)        0 2024-05-14 01:54:42.954474 bsv_sdk-0.2.0/tests/
+-rw-r--r--   0 aaron67    (501) staff       (20)     1435 2024-05-04 20:31:16.000000 bsv_sdk-0.2.0/tests/test_aes_cbc.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1163 2024-04-26 06:30:47.000000 bsv_sdk-0.2.0/tests/test_base58.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     2501 2024-04-26 06:28:18.000000 bsv_sdk-0.2.0/tests/test_curve.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1017 2024-05-04 20:37:31.000000 bsv_sdk-0.2.0/tests/test_encrypted_message.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1144 2024-04-26 03:54:23.000000 bsv_sdk-0.2.0/tests/test_hash.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    10031 2024-05-14 01:48:14.000000 bsv_sdk-0.2.0/tests/test_hd.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    11530 2024-05-13 21:41:30.000000 bsv_sdk-0.2.0/tests/test_keys.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     3505 2024-05-13 21:03:02.000000 bsv_sdk-0.2.0/tests/test_scripts.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    10974 2024-05-14 01:16:28.000000 bsv_sdk-0.2.0/tests/test_transaction.py
+-rw-r--r--   0 aaron67    (501) staff       (20)    10774 2024-05-13 20:11:43.000000 bsv_sdk-0.2.0/tests/test_utils.py
+-rw-r--r--   0 aaron67    (501) staff       (20)     1441 2024-05-14 00:30:15.000000 bsv_sdk-0.2.0/tests/test_wallet.py
```

### Comparing `bsv-sdk-0.1.1/LICENSE.txt` & `bsv_sdk-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bsv-sdk-0.1.1/PKG-INFO` & `bsv_sdk-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,92 @@
 Metadata-Version: 2.1
 Name: bsv-sdk
-Version: 0.1.1
+Version: 0.2.0
 Summary: BSV BLOCKCHAIN | Software Development Kit for Python
 Home-page: https://github.com/bitcoin-sv/py-sdk
 Author: Aaron
 Author-email: aaron@scrypt.io
 Project-URL: Bug Tracker, https://github.com/bitcoin-sv/py-sdk/issues
 Keywords: bsv
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: typing-extensions
-
-# BSV TEMPLATE
-
-BSV BLOCKCHAIN | Template repository for open-source projects
-
-Update this README with information about the project.
+Requires-Dist: pycryptodomex
+Requires-Dist: coincurve
+Requires-Dist: requests
+
+# BSV SDK
+
+[![build](https://github.com/bitcoin-sv/py-sdk/actions/workflows/build.yml/badge.svg)](https://github.com/bitcoin-sv/py-sdk/actions/workflows/build.yml)
+[![PyPI version](https://img.shields.io/pypi/v/bsv-sdk)](https://pypi.org/project/bsv-sdk)
+[![Python versions](https://img.shields.io/pypi/pyversions/bsv-sdk)](https://pypi.org/project/bsv-sdk)
+
+Welcome to the BSV Blockchain Libraries Project, the comprehensive Python SDK designed to provide an updated and unified layer for
+developing scalable applications on the BSV Blockchain. This SDK addresses the limitations of previous tools by offering a fresh,
+peer-to-peer approach, adhering to SPV, and ensuring privacy and scalability.
 
 ## Table of Contents
 
 1. [Objective](#objective)
 2. [Getting Started](#getting-started)
 3. [Features & Deliverables](#features--deliverables)
 4. [Documentation](#documentation)
 5. [Contribution Guidelines](#contribution-guidelines)
 6. [Support & Contacts](#support--contacts)
 
 ## Objective
 
-Toe objective of this project is to make it easier to create new open-source projects within Bitcoin SV.
+The BSV Blockchain Libraries Project aims to structure and maintain a middleware layer of the BSV Blockchain technology stack. By
+facilitating the development and maintenance of core libraries, it serves as an essential toolkit for developers looking to build on the BSV
+Blockchain.
 
 ## Getting Started
 
-### Fork the repo
-
-To create a project from this template:
+### Installation
 
 ```bash
-git clone https://github.com/bitcoin-sv/template
+pip install bsv-sdk
 ```
 
 ### Basic Usage
 
-
-```typescript
-// TODO: Code Example Will Go Here
+```python
+# TODO: Code Example Will Go Here
 ```
 
 For a more detailed tutorial and advanced examples, check our [Documentation](#documentation).
 
 ## Features & Deliverables
 
 - **Main Project Feature**: Description of the feature
 
 - **Main Project Feature 2**: Description of the feature
 
 - **Secondary Project Feature**: Description of the feature
 
 ## Documentation
 
-Provide detailed information and links to the various places the project is documented, including concepts, getting started guides, tutorials, and API specifications.
+Provide detailed information and links to the various places the project is documented, including concepts, getting started guides,
+tutorials, and API specifications.
 
 ## Contribution Guidelines
 
-We're always looking for contributors to help us improve the project. Whether it's bug reports, feature requests, or pull requests - all contributions are welcome.
+We're always looking for contributors to help us improve the project. Whether it's bug reports, feature requests, or pull requests - all
+contributions are welcome.
 
 1. **Fork & Clone**: Fork this repository and clone it to your local machine.
-2. **Set Up**: Run `npm install` to install all dependencies.
+2. **Set Up**: Run `pip install -r requirements.txt` to install all dependencies.
 3. **Make Changes**: Create a new branch and make your changes.
-4. **Test**: Ensure all tests pass by running `npm test`.
+4. **Test**: Ensure all tests pass by running `pytest --cov=bsv --cov-report=html`.
 5. **Commit**: Commit your changes and push to your fork.
 6. **Pull Request**: Open a pull request from your fork to this repository.
 
 For more details, check the [contribution guidelines](./CONTRIBUTING.md).
 
 For information on past releases, check out the [changelog](./CHANGELOG.md). For future plans, check the [roadmap](./ROADMAP.md)!
```

### Comparing `bsv-sdk-0.1.1/README.md` & `bsv_sdk-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,70 @@
-# BSV TEMPLATE
+# BSV SDK
 
-BSV BLOCKCHAIN | Template repository for open-source projects
-
-Update this README with information about the project.
+[![build](https://github.com/bitcoin-sv/py-sdk/actions/workflows/build.yml/badge.svg)](https://github.com/bitcoin-sv/py-sdk/actions/workflows/build.yml)
+[![PyPI version](https://img.shields.io/pypi/v/bsv-sdk)](https://pypi.org/project/bsv-sdk)
+[![Python versions](https://img.shields.io/pypi/pyversions/bsv-sdk)](https://pypi.org/project/bsv-sdk)
+
+Welcome to the BSV Blockchain Libraries Project, the comprehensive Python SDK designed to provide an updated and unified layer for
+developing scalable applications on the BSV Blockchain. This SDK addresses the limitations of previous tools by offering a fresh,
+peer-to-peer approach, adhering to SPV, and ensuring privacy and scalability.
 
 ## Table of Contents
 
 1. [Objective](#objective)
 2. [Getting Started](#getting-started)
 3. [Features & Deliverables](#features--deliverables)
 4. [Documentation](#documentation)
 5. [Contribution Guidelines](#contribution-guidelines)
 6. [Support & Contacts](#support--contacts)
 
 ## Objective
 
-Toe objective of this project is to make it easier to create new open-source projects within Bitcoin SV.
+The BSV Blockchain Libraries Project aims to structure and maintain a middleware layer of the BSV Blockchain technology stack. By
+facilitating the development and maintenance of core libraries, it serves as an essential toolkit for developers looking to build on the BSV
+Blockchain.
 
 ## Getting Started
 
-### Fork the repo
-
-To create a project from this template:
+### Installation
 
 ```bash
-git clone https://github.com/bitcoin-sv/template
+pip install bsv-sdk
 ```
 
 ### Basic Usage
 
-
-```typescript
-// TODO: Code Example Will Go Here
+```python
+# TODO: Code Example Will Go Here
 ```
 
 For a more detailed tutorial and advanced examples, check our [Documentation](#documentation).
 
 ## Features & Deliverables
 
 - **Main Project Feature**: Description of the feature
 
 - **Main Project Feature 2**: Description of the feature
 
 - **Secondary Project Feature**: Description of the feature
 
 ## Documentation
 
-Provide detailed information and links to the various places the project is documented, including concepts, getting started guides, tutorials, and API specifications.
+Provide detailed information and links to the various places the project is documented, including concepts, getting started guides,
+tutorials, and API specifications.
 
 ## Contribution Guidelines
 
-We're always looking for contributors to help us improve the project. Whether it's bug reports, feature requests, or pull requests - all contributions are welcome.
+We're always looking for contributors to help us improve the project. Whether it's bug reports, feature requests, or pull requests - all
+contributions are welcome.
 
 1. **Fork & Clone**: Fork this repository and clone it to your local machine.
-2. **Set Up**: Run `npm install` to install all dependencies.
+2. **Set Up**: Run `pip install -r requirements.txt` to install all dependencies.
 3. **Make Changes**: Create a new branch and make your changes.
-4. **Test**: Ensure all tests pass by running `npm test`.
+4. **Test**: Ensure all tests pass by running `pytest --cov=bsv --cov-report=html`.
 5. **Commit**: Commit your changes and push to your fork.
 6. **Pull Request**: Open a pull request from your fork to this repository.
 
 For more details, check the [contribution guidelines](./CONTRIBUTING.md).
 
 For information on past releases, check out the [changelog](./CHANGELOG.md). For future plans, check the [roadmap](./ROADMAP.md)!
```

### Comparing `bsv-sdk-0.1.1/bsv_sdk.egg-info/PKG-INFO` & `bsv_sdk-0.2.0/bsv_sdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,92 @@
 Metadata-Version: 2.1
 Name: bsv-sdk
-Version: 0.1.1
+Version: 0.2.0
 Summary: BSV BLOCKCHAIN | Software Development Kit for Python
 Home-page: https://github.com/bitcoin-sv/py-sdk
 Author: Aaron
 Author-email: aaron@scrypt.io
 Project-URL: Bug Tracker, https://github.com/bitcoin-sv/py-sdk/issues
 Keywords: bsv
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: typing-extensions
-
-# BSV TEMPLATE
-
-BSV BLOCKCHAIN | Template repository for open-source projects
-
-Update this README with information about the project.
+Requires-Dist: pycryptodomex
+Requires-Dist: coincurve
+Requires-Dist: requests
+
+# BSV SDK
+
+[![build](https://github.com/bitcoin-sv/py-sdk/actions/workflows/build.yml/badge.svg)](https://github.com/bitcoin-sv/py-sdk/actions/workflows/build.yml)
+[![PyPI version](https://img.shields.io/pypi/v/bsv-sdk)](https://pypi.org/project/bsv-sdk)
+[![Python versions](https://img.shields.io/pypi/pyversions/bsv-sdk)](https://pypi.org/project/bsv-sdk)
+
+Welcome to the BSV Blockchain Libraries Project, the comprehensive Python SDK designed to provide an updated and unified layer for
+developing scalable applications on the BSV Blockchain. This SDK addresses the limitations of previous tools by offering a fresh,
+peer-to-peer approach, adhering to SPV, and ensuring privacy and scalability.
 
 ## Table of Contents
 
 1. [Objective](#objective)
 2. [Getting Started](#getting-started)
 3. [Features & Deliverables](#features--deliverables)
 4. [Documentation](#documentation)
 5. [Contribution Guidelines](#contribution-guidelines)
 6. [Support & Contacts](#support--contacts)
 
 ## Objective
 
-Toe objective of this project is to make it easier to create new open-source projects within Bitcoin SV.
+The BSV Blockchain Libraries Project aims to structure and maintain a middleware layer of the BSV Blockchain technology stack. By
+facilitating the development and maintenance of core libraries, it serves as an essential toolkit for developers looking to build on the BSV
+Blockchain.
 
 ## Getting Started
 
-### Fork the repo
-
-To create a project from this template:
+### Installation
 
 ```bash
-git clone https://github.com/bitcoin-sv/template
+pip install bsv-sdk
 ```
 
 ### Basic Usage
 
-
-```typescript
-// TODO: Code Example Will Go Here
+```python
+# TODO: Code Example Will Go Here
 ```
 
 For a more detailed tutorial and advanced examples, check our [Documentation](#documentation).
 
 ## Features & Deliverables
 
 - **Main Project Feature**: Description of the feature
 
 - **Main Project Feature 2**: Description of the feature
 
 - **Secondary Project Feature**: Description of the feature
 
 ## Documentation
 
-Provide detailed information and links to the various places the project is documented, including concepts, getting started guides, tutorials, and API specifications.
+Provide detailed information and links to the various places the project is documented, including concepts, getting started guides,
+tutorials, and API specifications.
 
 ## Contribution Guidelines
 
-We're always looking for contributors to help us improve the project. Whether it's bug reports, feature requests, or pull requests - all contributions are welcome.
+We're always looking for contributors to help us improve the project. Whether it's bug reports, feature requests, or pull requests - all
+contributions are welcome.
 
 1. **Fork & Clone**: Fork this repository and clone it to your local machine.
-2. **Set Up**: Run `npm install` to install all dependencies.
+2. **Set Up**: Run `pip install -r requirements.txt` to install all dependencies.
 3. **Make Changes**: Create a new branch and make your changes.
-4. **Test**: Ensure all tests pass by running `npm test`.
+4. **Test**: Ensure all tests pass by running `pytest --cov=bsv --cov-report=html`.
 5. **Commit**: Commit your changes and push to your fork.
 6. **Pull Request**: Open a pull request from your fork to this repository.
 
 For more details, check the [contribution guidelines](./CONTRIBUTING.md).
 
 For information on past releases, check out the [changelog](./CHANGELOG.md). For future plans, check the [roadmap](./ROADMAP.md)!
```

### Comparing `bsv-sdk-0.1.1/setup.cfg` & `bsv_sdk-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bitcoin-sv/py-sdk
 project_urls = 
 	Bug Tracker = https://github.com/bitcoin-sv/py-sdk/issues
 classifiers = 
 	Intended Audience :: Developers
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Operating System :: OS Independent
 keywords = 
 	bsv
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.9
+include_package_data = True
 install_requires = 
-	typing-extensions
+	pycryptodomex
+	coincurve
+	requests
 tests_require = 
 	pytest
+	ecdsa
+
+[options.package_data]
+* = hd/wordlist/*.txt
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

