# Comparing `tmp/anyhedge-2.1.0.tar.gz` & `tmp/anyhedge-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyhedge-2.1.0.tar", last modified: Tue May 14 19:46:46 2024, max compression
+gzip compressed data, was "anyhedge-2.1.1.tar", last modified: Tue May 14 19:51:40 2024, max compression
```

## Comparing `anyhedge-2.1.0.tar` & `anyhedge-2.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:46:46.677355 anyhedge-2.1.0/
--rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-2.1.0/LICENSE
--rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-14 19:46:46.677355 anyhedge-2.1.0/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-2.1.0/README.md
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:46:46.677355 anyhedge-2.1.0/anyhedge/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-2.1.0/anyhedge/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2426 2024-04-10 20:22:29.000000 anyhedge-2.1.0/anyhedge/bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    53693 2024-05-08 09:27:33.000000 anyhedge-2.1.0/anyhedge/contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2194 2024-05-08 03:09:46.000000 anyhedge-2.1.0/anyhedge/contract_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2024-05-08 03:40:10.000000 anyhedge-2.1.0/anyhedge/fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-2.1.0/anyhedge/javascript.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    13977 2024-05-14 19:41:31.000000 anyhedge-2.1.0/anyhedge/oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      303 2024-05-08 03:40:10.000000 anyhedge-2.1.0/anyhedge/role.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:46:46.677355 anyhedge-2.1.0/anyhedge/tests/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-2.1.0/anyhedge/tests/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-2.1.0/anyhedge/tests/test_bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    47505 2024-05-08 09:31:54.000000 anyhedge-2.1.0/anyhedge/tests/test_contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      498 2024-05-08 03:42:46.000000 anyhedge-2.1.0/anyhedge/tests/test_contract_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2024-05-08 03:40:10.000000 anyhedge-2.1.0/anyhedge/tests/test_fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-2.1.0/anyhedge/tests/test_oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-2.1.0/anyhedge/validators.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:46:46.677355 anyhedge-2.1.0/anyhedge.egg-info/
--rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-14 19:46:46.000000 anyhedge-2.1.0/anyhedge.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)      587 2024-05-14 19:46:46.000000 anyhedge-2.1.0/anyhedge.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        1 2024-05-14 19:46:46.000000 anyhedge-2.1.0/anyhedge.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)       57 2024-05-14 19:46:46.000000 anyhedge-2.1.0/anyhedge.egg-info/requires.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        9 2024-05-14 19:46:46.000000 anyhedge-2.1.0/anyhedge.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)      798 2024-05-14 19:46:27.000000 anyhedge-2.1.0/pyproject.toml
--rw-rw-r--   0 alien     (1000) alien     (1000)       38 2024-05-14 19:46:46.677355 anyhedge-2.1.0/setup.cfg
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:51:40.954349 anyhedge-2.1.1/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-2.1.1/LICENSE
+-rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-14 19:51:40.954349 anyhedge-2.1.1/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-2.1.1/README.md
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:51:40.954349 anyhedge-2.1.1/anyhedge/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-2.1.1/anyhedge/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2426 2024-04-10 20:22:29.000000 anyhedge-2.1.1/anyhedge/bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    53693 2024-05-08 09:27:33.000000 anyhedge-2.1.1/anyhedge/contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2194 2024-05-08 03:09:46.000000 anyhedge-2.1.1/anyhedge/contract_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2024-05-08 03:40:10.000000 anyhedge-2.1.1/anyhedge/fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-2.1.1/anyhedge/javascript.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    13976 2024-05-14 19:50:32.000000 anyhedge-2.1.1/anyhedge/oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      303 2024-05-08 03:40:10.000000 anyhedge-2.1.1/anyhedge/role.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:51:40.954349 anyhedge-2.1.1/anyhedge/tests/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-2.1.1/anyhedge/tests/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-2.1.1/anyhedge/tests/test_bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    47505 2024-05-08 09:31:54.000000 anyhedge-2.1.1/anyhedge/tests/test_contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      498 2024-05-08 03:42:46.000000 anyhedge-2.1.1/anyhedge/tests/test_contract_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2024-05-08 03:40:10.000000 anyhedge-2.1.1/anyhedge/tests/test_fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-2.1.1/anyhedge/tests/test_oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-2.1.1/anyhedge/validators.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 19:51:40.954349 anyhedge-2.1.1/anyhedge.egg-info/
+-rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-14 19:51:40.000000 anyhedge-2.1.1/anyhedge.egg-info/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)      587 2024-05-14 19:51:40.000000 anyhedge-2.1.1/anyhedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        1 2024-05-14 19:51:40.000000 anyhedge-2.1.1/anyhedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)       57 2024-05-14 19:51:40.000000 anyhedge-2.1.1/anyhedge.egg-info/requires.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        9 2024-05-14 19:51:40.000000 anyhedge-2.1.1/anyhedge.egg-info/top_level.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)      798 2024-05-14 19:51:00.000000 anyhedge-2.1.1/pyproject.toml
+-rw-rw-r--   0 alien     (1000) alien     (1000)       38 2024-05-14 19:51:40.954349 anyhedge-2.1.1/setup.cfg
```

### Comparing `anyhedge-2.1.0/LICENSE` & `anyhedge-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/PKG-INFO` & `anyhedge-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 2.1.0
+Version: 2.1.1
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-2.1.0/README.md` & `anyhedge-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/bch_primitives.py` & `anyhedge-2.1.1/anyhedge/bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/contract.py` & `anyhedge-2.1.1/anyhedge/contract.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/contract_primitives.py` & `anyhedge-2.1.1/anyhedge/contract_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/fee.py` & `anyhedge-2.1.1/anyhedge/fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/oracle.py` & `anyhedge-2.1.1/anyhedge/oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 class EthEM5(OracleUnit):
     name_of_oracleUnits = 'ETH(e-5)'
     name_of_standardUnits = 'ETH'
     oracleUnits_per_standardUnit = 100000
     public_key = PublicKey('038ab22e37cf020f6bbef40111ddc51083a936f0821de56ac01f799cf15b87904d')
 
 
-class EuroEM5(OracleUnit):
+class EurEM2(OracleUnit):
     name_of_oracleUnits = 'EUR(e-2)'
     name_of_standardUnits = 'EUR'
     oracleUnits_per_standardUnit = 100
     public_key = PublicKey('02bb9b3324df889a66a57bc890b3452b84a2a74ba753f8842b06bba03e0fa0dfc5')
 
 
 class InrEM0(OracleUnit):
```

### Comparing `anyhedge-2.1.0/anyhedge/tests/test_bch_primitives.py` & `anyhedge-2.1.1/anyhedge/tests/test_bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/tests/test_contract.py` & `anyhedge-2.1.1/anyhedge/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/tests/test_fee.py` & `anyhedge-2.1.1/anyhedge/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge/tests/test_oracle.py` & `anyhedge-2.1.1/anyhedge/tests/test_oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/anyhedge.egg-info/PKG-INFO` & `anyhedge-2.1.1/anyhedge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 2.1.0
+Version: 2.1.1
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-2.1.0/anyhedge.egg-info/SOURCES.txt` & `anyhedge-2.1.1/anyhedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.0/pyproject.toml` & `anyhedge-2.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'anyhedge'
-version = '2.1.0'
+version = '2.1.1'
 authors = [
   { name='emergent_reasons', email='emergent_reasons@gmail.com' },
 ]
 license = { file = "LICENSE" }
 description = 'Basic components of AnyHedge contracts'
 readme = 'README.md'
 requires-python = '>=3.10'
```

