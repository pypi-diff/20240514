# Comparing `tmp/cpf_and_cnpj_generator-0.0.0.1.tar.gz` & `tmp/cpf_and_cnpj_generator-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpf_and_cnpj_generator-0.0.0.1.tar", last modified: Tue May 14 08:57:03 2024, max compression
+gzip compressed data, was "cpf_and_cnpj_generator-0.0.1.tar", last modified: Tue May 14 09:10:20 2024, max compression
```

## Comparing `cpf_and_cnpj_generator-0.0.0.1.tar` & `cpf_and_cnpj_generator-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/
--rw-rw-rw-   0        0        0     1077 2024-05-14 08:31:41.000000 cpf_and_cnpj_generator-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3084 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2365 2024-05-14 08:34:47.000000 cpf_and_cnpj_generator-0.0.0.1/README.md
--rw-rw-rw-   0        0        0      804 2024-05-14 08:56:46.000000 cpf_and_cnpj_generator-0.0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.147857 cpf_and_cnpj_generator-0.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.163482 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/
--rw-rw-rw-   0        0        0       82 2024-05-14 08:43:45.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/__init__.py
--rw-rw-rw-   0        0        0     1254 2024-05-14 08:41:49.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/cnpj_generator.py
--rw-rw-rw-   0        0        0     1537 2024-05-14 08:39:49.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator/cpf_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:57:03.194733 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/
--rw-rw-rw-   0        0        0     3084 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-14 08:57:03.000000 cpf_and_cnpj_generator-0.0.0.1/src/cpf_and_cnpj_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:10:20.461606 cpf_and_cnpj_generator-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 09:10:10.000000 cpf_and_cnpj_generator-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-14 09:10:20.461606 cpf_and_cnpj_generator-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-14 09:10:10.000000 cpf_and_cnpj_generator-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 09:10:10.000000 cpf_and_cnpj_generator-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 09:10:20.461606 cpf_and_cnpj_generator-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:10:20.461606 cpf_and_cnpj_generator-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:10:20.461606 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 09:10:10.000000 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-14 09:10:10.000000 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator/cnpj_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-14 09:10:10.000000 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator/cpf_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 09:10:20.461606 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-14 09:10:20.000000 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-14 09:10:20.000000 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 09:10:20.000000 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 09:10:20.000000 cpf_and_cnpj_generator-0.0.1/src/cpf_and_cnpj_generator.egg-info/top_level.txt
```

### Comparing `cpf_and_cnpj_generator-0.0.0.1/pyproject.toml` & `cpf_and_cnpj_generator-0.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[build-system]
-requires = [
-    "setuptools>=61"
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "cpf_and_cnpj-generator"
-version = "0.0.0.1"
-authors = [
-  { name="Gabriel Logan" },
-]
-description = "This npm package provides JavaScript functions to generate valid Brazilian CPF (Cadastro de Pessoas Físicas) and CNPJ (Cadastro Nacional da Pessoa Jurídica) numbers."
-readme = "README.md"
-requires-python = ">=3.1"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://gabriel-logan.github.io/Gerador-CPF-e-CNPJ-valido/documentation"
+[build-system]
+requires = [
+    "setuptools>=61"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "cpf-and-cnpj-generator"
+version = "0.0.1"
+authors = [
+  { name="Gabriel Logan" },
+]
+description = "This pypi package provides Python functions to generate valid Brazilian CPF (Cadastro de Pessoas Físicas) and CNPJ (Cadastro Nacional da Pessoa Jurídica) numbers."
+readme = "README.md"
+requires-python = ">=3.1"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://gabriel-logan.github.io/Gerador-CPF-e-CNPJ-valido"
 "Bug Tracker" = "https://github.com/gabriel-logan/Gerador-CPF-e-CNPJ-valido/tree/main/packages/python"
```

