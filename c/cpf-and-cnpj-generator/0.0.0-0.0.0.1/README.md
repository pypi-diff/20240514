# Comparing `tmp/cpf_and_cnpj_generator-0.0.0.tar.gz` & `tmp/cpf_and_cnpj_generator-0.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpf_and_cnpj_generator-0.0.0.tar", last modified: Tue May 14 08:46:41 2024, max compression
+gzip compressed data, was "cpf_and_cnpj_generator-0.0.0.1.tar", last modified: Tue May 14 08:57:03 2024, max compression
```

## Comparing `cpf_and_cnpj_generator-0.0.0.tar` & `cpf_and_cnpj_generator-0.0.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:46:41.431585 cpf_and_cnpj_generator-0.0.0/
--rw-rw-rw-   0        0        0     1077 2024-05-14 08:31:41.000000 cpf_and_cnpj_generator-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     3082 2024-05-14 08:46:41.427988 cpf_and_cnpj_generator-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2365 2024-05-14 08:34:47.000000 cpf_and_cnpj_generator-0.0.0/README.md
--rw-rw-rw-   0        0        0      802 2024-05-14 08:45:43.000000 cpf_and_cnpj_generator-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 08:46:41.431585 cpf_and_cnpj_generator-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 08:46:41.403371 cpf_and_cnpj_generator-0.0.0/src/
--rw-rw-rw-   0        0        0       82 2024-05-14 08:43:45.000000 cpf_and_cnpj_generator-0.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     1254 2024-05-14 08:41:49.000000 cpf_and_cnpj_generator-0.0.0/src/cnpj_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:46:41.425988 cpf_and_cnpj_generator-0.0.0/src/cpf_and_cnpj_generator.egg-info/
--rw-rw-rw-   0        0        0     3082 2024-05-14 08:46:41.000000 cpf_and_cnpj_generator-0.0.0/src/cpf_and_cnpj_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-05-14 08:46:41.000000 cpf_and_cnpj_generator-0.0.0/src/cpf_and_cnpj_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:46:41.000000 cpf_and_cnpj_generator-0.0.0/src/cpf_and_cnpj_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-14 08:46:41.000000 cpf_and_cnpj_generator-0.0.0/src/cpf_and_cnpj_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1537 2024-05-14 08:39:49.000000 cpf_and_cnpj_generator-0.0.0/src/cpf_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/
+-rw-rw-rw-   0        0        0     1077 2024-05-14 08:31:41.000000 cpf_and_cnpj_generator-0.0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3084 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2365 2024-05-14 08:34:47.000000 cpf_and_cnpj_generator-0.0.0.1/README.md
+-rw-rw-rw-   0        0        0      804 2024-05-14 08:56:46.000000 cpf_and_cnpj_generator-0.0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.147857 cpf_and_cnpj_generator-0.0.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.163482 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/
+-rw-rw-rw-   0        0        0       82 2024-05-14 08:43:45.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/__init__.py
+-rw-rw-rw-   0        0        0     1254 2024-05-14 08:41:49.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/cnpj_generator.py
+-rw-rw-rw-   0        0        0     1537 2024-05-14 08:39:49.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/cpf_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/
+-rw-rw-rw-   0        0        0     3084 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/top_level.txt
```

### Comparing `cpf_and_cnpj_generator-0.0.0/LICENSE` & `cpf_and_cnpj_generator-0.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpf_and_cnpj_generator-0.0.0/PKG-INFO` & `cpf_and_cnpj_generator-0.0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpf_and_cnpj-generator
-Version: 0.0.0
+Version: 0.0.0.1
 Summary: This npm package provides JavaScript functions to generate valid Brazilian CPF (Cadastro de Pessoas Físicas) and CNPJ (Cadastro Nacional da Pessoa Jurídica) numbers.
 Author: Gabriel Logan
 Project-URL: Homepage, https://gabriel-logan.github.io/Gerador-CPF-e-CNPJ-valido/documentation
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/Gerador-CPF-e-CNPJ-valido/tree/main/packages/python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: cpf_and_cnpj-generator Version: 0.0.0 Summary: This
-npm package provides JavaScript functions to generate valid Brazilian CPF
+Metadata-Version: 2.1 Name: cpf_and_cnpj-generator Version: 0.0.0.1 Summary:
+This npm package provides JavaScript functions to generate valid Brazilian CPF
 (Cadastro de Pessoas FÃ­sicas) and CNPJ (Cadastro Nacional da Pessoa JurÃ­dica)
 numbers. Author: Gabriel Logan Project-URL: Homepage, https://gabriel-
 logan.github.io/Gerador-CPF-e-CNPJ-valido/documentation Project-URL: Bug
 Tracker, https://github.com/gabriel-logan/Gerador-CPF-e-CNPJ-valido/tree/main/
 packages/python Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.1 Description-Content-Type: text/markdown
```

### Comparing `cpf_and_cnpj_generator-0.0.0/README.md` & `cpf_and_cnpj_generator-0.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cpf_and_cnpj_generator-0.0.0/pyproject.toml` & `cpf_and_cnpj_generator-0.0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpf_and_cnpj-generator"
-version = "0.0.0"
+version = "0.0.0.1"
 authors = [
   { name="Gabriel Logan" },
 ]
 description = "This npm package provides JavaScript functions to generate valid Brazilian CPF (Cadastro de Pessoas Físicas) and CNPJ (Cadastro Nacional da Pessoa Jurídica) numbers."
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
```

### Comparing `cpf_and_cnpj_generator-0.0.0/src/cnpj_generator.py` & `cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/cnpj_generator.py`

 * *Files identical despite different names*

### Comparing `cpf_and_cnpj_generator-0.0.0/src/cpf_and_cnpj_generator.egg-info/PKG-INFO` & `cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpf_and_cnpj-generator
-Version: 0.0.0
+Version: 0.0.0.1
 Summary: This npm package provides JavaScript functions to generate valid Brazilian CPF (Cadastro de Pessoas Físicas) and CNPJ (Cadastro Nacional da Pessoa Jurídica) numbers.
 Author: Gabriel Logan
 Project-URL: Homepage, https://gabriel-logan.github.io/Gerador-CPF-e-CNPJ-valido/documentation
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/Gerador-CPF-e-CNPJ-valido/tree/main/packages/python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: cpf_and_cnpj-generator Version: 0.0.0 Summary: This
-npm package provides JavaScript functions to generate valid Brazilian CPF
+Metadata-Version: 2.1 Name: cpf_and_cnpj-generator Version: 0.0.0.1 Summary:
+This npm package provides JavaScript functions to generate valid Brazilian CPF
 (Cadastro de Pessoas FÃ­sicas) and CNPJ (Cadastro Nacional da Pessoa JurÃ­dica)
 numbers. Author: Gabriel Logan Project-URL: Homepage, https://gabriel-
 logan.github.io/Gerador-CPF-e-CNPJ-valido/documentation Project-URL: Bug
 Tracker, https://github.com/gabriel-logan/Gerador-CPF-e-CNPJ-valido/tree/main/
 packages/python Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.1 Description-Content-Type: text/markdown
```

### Comparing `cpf_and_cnpj_generator-0.0.0/src/cpf_generator.py` & `cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/cpf_generator.py`

 * *Files identical despite different names*

