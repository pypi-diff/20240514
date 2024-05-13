# Comparing `tmp/brdocs-validation-0.3.0.tar.gz` & `tmp/brdocs_validation-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brdocs-validation-0.3.0.tar", last modified: Tue Feb 27 17:15:31 2024, max compression
+gzip compressed data, was "brdocs_validation-0.4.0.tar", last modified: Mon May 13 23:22:41 2024, max compression
```

## Comparing `brdocs-validation-0.3.0.tar` & `brdocs_validation-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 17:15:31.902156 brdocs-validation-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-02-27 17:15:31.902156 brdocs-validation-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 17:15:31.898157 brdocs-validation-0.3.0/br_docs/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 17:15:31.898157 brdocs-validation-0.3.0/br_docs/validators/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/cnh.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/cnpj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/cns.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/cpf.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/nis.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/renavam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/te.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 17:15:31.898157 brdocs-validation-0.3.0/br_docs/validators/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/br_docs/validators/types/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 17:15:31.902156 brdocs-validation-0.3.0/brdocs_validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-02-27 17:15:31.000000 brdocs-validation-0.3.0/brdocs_validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-27 17:15:31.000000 brdocs-validation-0.3.0/brdocs_validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 17:15:31.000000 brdocs-validation-0.3.0/brdocs_validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-27 17:15:31.000000 brdocs-validation-0.3.0/brdocs_validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-27 17:15:31.000000 brdocs-validation-0.3.0/brdocs_validation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 17:15:31.902156 brdocs-validation-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 17:15:31.902156 brdocs-validation-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/tests/test_brdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/tests/test_check_two_digits.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-27 17:15:23.000000 brdocs-validation-0.3.0/tests/test_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:41.141820 brdocs_validation-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-13 23:22:41.141820 brdocs_validation-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:41.133820 brdocs_validation-0.4.0/br_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:41.137820 brdocs_validation-0.4.0/br_docs/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/cnh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/cnpj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/cns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/cpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/nis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/renavam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/sei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/te.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:41.137820 brdocs_validation-0.4.0/br_docs/validators/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/br_docs/validators/types/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:41.137820 brdocs_validation-0.4.0/brdocs_validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-13 23:22:41.000000 brdocs_validation-0.4.0/brdocs_validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-13 23:22:41.000000 brdocs_validation-0.4.0/brdocs_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 23:22:41.000000 brdocs_validation-0.4.0/brdocs_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 23:22:41.000000 brdocs_validation-0.4.0/brdocs_validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 23:22:41.000000 brdocs_validation-0.4.0/brdocs_validation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 23:22:41.141820 brdocs_validation-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:22:41.137820 brdocs_validation-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/tests/test_brdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/tests/test_check_two_digits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-13 23:22:36.000000 brdocs_validation-0.4.0/tests/test_format.py
```

### Comparing `brdocs-validation-0.3.0/LICENSE.txt` & `brdocs_validation-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/PKG-INFO` & `brdocs_validation-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brdocs-validation
-Version: 0.3.0
+Version: 0.4.0
 Summary: Validate brazilian documents using Type Hints in classes inheriting Pydantic's (V2) BaseModel
 Author-email: Vinícius Aguiar <vaguiararqdevsoftware@proton.me>
 Maintainer-email: Vinícius Aguiar <vaguiararqdevsoftware@proton.me>
 Project-URL: Repository, https://github.com/vinicius-oa/BRdocs-validation
 Keywords: pydantic-v2,cpf-validador,cnpj-validador,validador-pispasep,validador-titulo-eleitor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -50,24 +50,27 @@
 |        CPF        |                                           |   *123.456.789-01* OR _Without special chars_   |                      |
 |        CNH        |                                           |                  Only numbers                   |     Length: _11_     |
 | NIS/PIS/PASEP/NIT | Use _**NIS**_ type for _PIS, PASEP, NIT_  |       *123.45678.90-1* OR _Only numbers_        |                      |
 |        CNS        |         Cartão Nacional de Saúde          |                  Only numbers                   |                      |
 |      RENAVAM      |                                           |                  Only numbers                   | Length: _9, 10 & 11_ | 
 |        TE         |             Título de eleitor             |                  Only numbers                   |                      |
 |       CERT        | Certidão de casamento, nascimento e óbito |                  Only numbers                   |                      | 
+|        SEI        |         Número do Processo SEI            | 12345-67890123/4567-89 OR without special chars |                      |
+
 ## Usage 
 
 ```python
-from br_docs import CNPJ, CPF, CNH, NIS, CNS, RENAVAM, TE, CERT
+from br_docs import CNPJ, CPF, CNH, NIS, CNS, RENAVAM, TE, CERT, SEI
 from pydantic import BaseModel
 
 
 class User(BaseModel):
     cpf: CPF
     cnpj: CNPJ
     cnh: CNH
     nis: NIS
     cns: CNS
     renavam: RENAVAM
     te: TE
     cert: CERT
+    sei: SEI
 ```
```

### Comparing `brdocs-validation-0.3.0/README.md` & `brdocs_validation-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 |        CPF        |                                           |   *123.456.789-01* OR _Without special chars_   |                      |
 |        CNH        |                                           |                  Only numbers                   |     Length: _11_     |
 | NIS/PIS/PASEP/NIT | Use _**NIS**_ type for _PIS, PASEP, NIT_  |       *123.45678.90-1* OR _Only numbers_        |                      |
 |        CNS        |         Cartão Nacional de Saúde          |                  Only numbers                   |                      |
 |      RENAVAM      |                                           |                  Only numbers                   | Length: _9, 10 & 11_ | 
 |        TE         |             Título de eleitor             |                  Only numbers                   |                      |
 |       CERT        | Certidão de casamento, nascimento e óbito |                  Only numbers                   |                      | 
+|        SEI        |         Número do Processo SEI            | 12345-67890123/4567-89 OR without special chars |                      |
+
 ## Usage 
 
 ```python
-from br_docs import CNPJ, CPF, CNH, NIS, CNS, RENAVAM, TE, CERT
+from br_docs import CNPJ, CPF, CNH, NIS, CNS, RENAVAM, TE, CERT, SEI
 from pydantic import BaseModel
 
 
 class User(BaseModel):
     cpf: CPF
     cnpj: CNPJ
     cnh: CNH
     nis: NIS
     cns: CNS
     renavam: RENAVAM
     te: TE
     cert: CERT
-```
+    sei: SEI
+```
```

### Comparing `brdocs-validation-0.3.0/br_docs/__init__.py` & `brdocs_validation-0.4.0/br_docs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 from br_docs.validators.cnh import CNHv
 from br_docs.validators.cnpj import CNPJv
 from br_docs.validators.cns import CNSv
 from br_docs.validators.cpf import CPFv
 from br_docs.validators.nis import NISv
 from br_docs.validators.renavam import RENAVAMv
 from br_docs.validators.te import TEv
+from br_docs.validators.sei import SEIv
 
 
 CPF = Annotated[str, AfterValidator(CPFv())]
 CNPJ = Annotated[str, AfterValidator(CNPJv())]
 CNH = Annotated[str, AfterValidator(CNHv())]
 NIS = Annotated[str, AfterValidator(NISv())]
 CNS = Annotated[str, AfterValidator(CNSv())]
 RENAVAM = Annotated[str, AfterValidator(RENAVAMv())]
 TE = Annotated[str, AfterValidator(TEv())]
 CERT = Annotated[str, AfterValidator(CERTv())]
+SEI = Annotated[str, AfterValidator(SEIv())]
```

### Comparing `brdocs-validation-0.3.0/br_docs/validators/__init__.py` & `brdocs_validation-0.4.0/br_docs/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/cert.py` & `brdocs_validation-0.4.0/br_docs/validators/cert.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/cnh.py` & `brdocs_validation-0.4.0/br_docs/validators/cnh.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/cnpj.py` & `brdocs_validation-0.4.0/br_docs/validators/cnpj.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/cns.py` & `brdocs_validation-0.4.0/br_docs/validators/cns.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/cpf.py` & `brdocs_validation-0.4.0/br_docs/validators/cpf.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/nis.py` & `brdocs_validation-0.4.0/br_docs/validators/nis.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/renavam.py` & `brdocs_validation-0.4.0/br_docs/validators/renavam.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/br_docs/validators/te.py` & `brdocs_validation-0.4.0/br_docs/validators/te.py`

 * *Files identical despite different names*

### Comparing `brdocs-validation-0.3.0/brdocs_validation.egg-info/PKG-INFO` & `brdocs_validation-0.4.0/brdocs_validation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brdocs-validation
-Version: 0.3.0
+Version: 0.4.0
 Summary: Validate brazilian documents using Type Hints in classes inheriting Pydantic's (V2) BaseModel
 Author-email: Vinícius Aguiar <vaguiararqdevsoftware@proton.me>
 Maintainer-email: Vinícius Aguiar <vaguiararqdevsoftware@proton.me>
 Project-URL: Repository, https://github.com/vinicius-oa/BRdocs-validation
 Keywords: pydantic-v2,cpf-validador,cnpj-validador,validador-pispasep,validador-titulo-eleitor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -50,24 +50,27 @@
 |        CPF        |                                           |   *123.456.789-01* OR _Without special chars_   |                      |
 |        CNH        |                                           |                  Only numbers                   |     Length: _11_     |
 | NIS/PIS/PASEP/NIT | Use _**NIS**_ type for _PIS, PASEP, NIT_  |       *123.45678.90-1* OR _Only numbers_        |                      |
 |        CNS        |         Cartão Nacional de Saúde          |                  Only numbers                   |                      |
 |      RENAVAM      |                                           |                  Only numbers                   | Length: _9, 10 & 11_ | 
 |        TE         |             Título de eleitor             |                  Only numbers                   |                      |
 |       CERT        | Certidão de casamento, nascimento e óbito |                  Only numbers                   |                      | 
+|        SEI        |         Número do Processo SEI            | 12345-67890123/4567-89 OR without special chars |                      |
+
 ## Usage 
 
 ```python
-from br_docs import CNPJ, CPF, CNH, NIS, CNS, RENAVAM, TE, CERT
+from br_docs import CNPJ, CPF, CNH, NIS, CNS, RENAVAM, TE, CERT, SEI
 from pydantic import BaseModel
 
 
 class User(BaseModel):
     cpf: CPF
     cnpj: CNPJ
     cnh: CNH
     nis: NIS
     cns: CNS
     renavam: RENAVAM
     te: TE
     cert: CERT
+    sei: SEI
 ```
```

### Comparing `brdocs-validation-0.3.0/brdocs_validation.egg-info/SOURCES.txt` & `brdocs_validation-0.4.0/brdocs_validation.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 br_docs/validators/cert.py
 br_docs/validators/cnh.py
 br_docs/validators/cnpj.py
 br_docs/validators/cns.py
 br_docs/validators/cpf.py
 br_docs/validators/nis.py
 br_docs/validators/renavam.py
+br_docs/validators/sei.py
 br_docs/validators/te.py
 br_docs/validators/types/__init__.py
 br_docs/validators/types/format.py
 brdocs_validation.egg-info/PKG-INFO
 brdocs_validation.egg-info/SOURCES.txt
 brdocs_validation.egg-info/dependency_links.txt
 brdocs_validation.egg-info/requires.txt
```

### Comparing `brdocs-validation-0.3.0/pyproject.toml` & `brdocs_validation-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel >= 0.41"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brdocs-validation"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
   "pydantic>=2.0"
 ]
 requires-python = ">= 3.10"
 authors = [
   {name = "Vinícius Aguiar", email = "vaguiararqdevsoftware@proton.me"},
 ]
@@ -64,8 +64,8 @@
     pytest {posargs:tests} --basetemp="{env_tmp_dir}"
 
 [gh]
 python =
     3.12 = py312-pydantic{20,21,22,23,24,25,26}
     3.11 = py311-pydantic{20,21,22,23,24,25,26}
     3.10 = py310-pydantic{20,21,22,23,24,25,26}
-"""
+"""
```

### Comparing `brdocs-validation-0.3.0/tests/test_brdocs.py` & `brdocs_validation-0.4.0/tests/test_brdocs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from contextlib import contextmanager
 
+import pytest
 from pydantic import create_model
 from pydantic_core import ValidationError
 
-from br_docs import CNH, CPF, CNPJ, NIS, CNS, RENAVAM, TE, CERT
+from br_docs import CNH, CPF, CNPJ, NIS, CNS, RENAVAM, TE, CERT, SEI
 
 
 @contextmanager
 def validate(model_name: str, values, value_type):
     try:
         for value in values:
             try:
                 m = create_model(model_name, param=(value_type, ...))
                 m(param=value)
             except ValidationError as exc:
-                assert False, f"{exc}: {value}"
+                raise exc
         yield
     finally:
         pass
 
 
 def test_cnh(cnh_list):
     with validate(model_name='TestCNH', values=cnh_list, value_type=CNH):
@@ -54,7 +55,22 @@
     with validate(model_name='TestTE', values=te_list, value_type=TE):
         pass
 
 
 def test_cert(cert_list):
     with validate(model_name='TestCERT', values=cert_list, value_type=CERT):
         pass
+
+
+def test_valid_sei(valid_sei_list):
+    with validate(model_name='TestSEI', values=valid_sei_list, value_type=SEI):
+        pass
+
+
+def test_invalid_sei(invalid_sei_list):
+    with pytest.raises(ValidationError):
+        with validate(
+            model_name='TestSEI',
+            values=invalid_sei_list,
+            value_type=SEI,
+        ):
+            pass
```

