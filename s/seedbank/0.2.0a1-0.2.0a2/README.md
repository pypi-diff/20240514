# Comparing `tmp/seedbank-0.2.0a1.tar.gz` & `tmp/seedbank-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedbank-0.2.0a1.tar", last modified: Tue Dec 19 14:59:33 2023, max compression
+gzip compressed data, was "seedbank-0.2.0a2.tar", last modified: Tue May 14 15:14:58 2024, max compression
```

## Comparing `seedbank-0.2.0a1.tar` & `seedbank-0.2.0a2.tar`

### file list

```diff
@@ -1,56 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.906472 seedbank-0.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.894472 seedbank-0.2.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.894472 seedbank-0.2.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.github/workflows/check-sources.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.894472 seedbank-0.2.0a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2023-12-19 14:59:33.906472 seedbank-0.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.898472 seedbank-0.2.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.898472 seedbank-0.2.0a1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      658 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/docs/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/docs/patterns.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.898472 seedbank-0.2.0a1/seedbank/
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/cupy.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/numba.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/seedbank/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.902472 seedbank-0.2.0a1/seedbank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2023-12-19 14:59:33.000000 seedbank-0.2.0a1/seedbank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-12-19 14:59:33.000000 seedbank-0.2.0a1/seedbank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 14:59:33.000000 seedbank-0.2.0a1/seedbank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-12-19 14:59:33.000000 seedbank-0.2.0a1/seedbank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-19 14:59:33.000000 seedbank-0.2.0a1/seedbank.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 14:59:33.906472 seedbank-0.2.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 14:59:33.902472 seedbank-0.2.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/init_seed.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/init_seed.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/init_seed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_cupy_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_derive.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_init_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_process_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-19 14:59:21.000000 seedbank-0.2.0a1/tests/test_randomstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.630687 seedbank-0.2.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-14 15:14:58.630687 seedbank-0.2.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.622687 seedbank-0.2.0a2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.622687 seedbank-0.2.0a2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/docs/patterns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.622687 seedbank-0.2.0a2/seedbank/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/seedbank/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.626687 seedbank-0.2.0a2/seedbank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 15:14:58.000000 seedbank-0.2.0a2/seedbank.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:14:58.630687 seedbank-0.2.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:14:58.626687 seedbank-0.2.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/init_seed.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/init_seed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/init_seed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_cupy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_derive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_init_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_process_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-14 15:14:50.000000 seedbank-0.2.0a2/tests/test_randomstate.py
```

### Comparing `seedbank-0.2.0a1/.gitignore` & `seedbank-0.2.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/LICENSE.md` & `seedbank-0.2.0a2/LICENSE.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Copyright (c) 2021–2023 Boise State University
-Copyright (c) 2023 Michael Ekstrand
+Copyright (c) 2023-2024 Drexel University and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `seedbank-0.2.0a1/PKG-INFO` & `seedbank-0.2.0a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: seedbank
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Common infrastructure for seeding random number generators.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2021–2023 Boise State University
-        Copyright (c) 2023 Michael Ekstrand
+        Copyright (c) 2023-2024 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -36,26 +36,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.17
 Requires-Dist: typing-extensions~=4.8
 Provides-Extra: dev
 Requires-Dist: setuptools>=64; extra == "dev"
 Requires-Dist: setuptools_scm>=8; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: build==1.*; extra == "dev"
+Requires-Dist: ruff>=0.2; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
-Requires-Dist: copier; extra == "dev"
+Requires-Dist: copier==9.*; extra == "dev"
+Requires-Dist: unbeheader~=1.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pyproject2conda; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-cov>=2.12; extra == "test"
+Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: pyyaml; extra == "test"
 Requires-Dist: toml; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx>=4.2; extra == "doc"
 Requires-Dist: sphinxext-opengraph>=0.5; extra == "doc"
 Requires-Dist: furo; extra == "doc"
 Provides-Extra: numba
```

### Comparing `seedbank-0.2.0a1/README.md` & `seedbank-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/docs/_templates/footer.html` & `seedbank-0.2.0a2/docs/_templates/footer.html`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/docs/api.rst` & `seedbank-0.2.0a2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/docs/conf.py` & `seedbank-0.2.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/docs/extending.rst` & `seedbank-0.2.0a2/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/docs/index.rst` & `seedbank-0.2.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/docs/patterns.rst` & `seedbank-0.2.0a2/docs/patterns.rst`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/pyproject.toml` & `seedbank-0.2.0a2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,30 +25,31 @@
   "typing-extensions ~= 4.8",
 ]
 
 [project.optional-dependencies]
 dev = [
   "setuptools>=64",
   "setuptools_scm>=8",
-  "build",
-  "twine",
-  "ruff",
+  "wheel",
+  "build ==1.*",       # p2c: -s python-build==1
+  "ruff >= 0.2",
   "pyright",
-  "copier",
+  "copier ==9.*",
+  "unbeheader ~= 1.3", # p2c: -p
   "ipython",
-  "pyproject2conda",
+  "pyproject2conda ",
   "sphinx-autobuild",
 ]
 test = [
   "pytest >= 7",
   "pytest-doctestplus",
-  "pytest-cov",
+  "pytest-cov >=2.12",
+  "coverage >=5",
   "pyyaml",
   "toml",
-  # "hypothesis",
 ]
 doc = [
   "sphinx >=4.2",
   "sphinxext-opengraph >= 0.5",
   "furo",
 ]
 numba = ["numba"]
@@ -58,36 +59,39 @@
 tf = ["tensorflow >=2,<3"]
 
 [project.urls]
 Homepage = "https://seedbank.lenksit.org"
 GitHub = "https://github.com/lenskit/seedbank"
 
 # configure build tools
-[tool.setuptools]
-packages = ["seedbank"]
+[tool.setuptools.packages.find]
+include = ["seedbank*"]
 
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 
 # settings for generating conda environments for dev & CI, when needed
 [tool.pyproject2conda]
 channels = ["conda-forge"]
+deps = ["just"]
 
 [tool.ruff]
 line-length = 100
 target-version = "py310"
-select = ["E", "F", "I"]
 exclude = [
   ".git",
   "__pycache__",
   "docs/conf.py",
   "build",
   "dist",
 ]
 
+[tool.ruff.lint]
+select = ["E", "F", "I"]
+
 [tool.ruff.lint.isort]
 section-order = [
   "future",
   "standard-library",
   "third-party",
   "testing",
   "first-party",
```

### Comparing `seedbank-0.2.0a1/seedbank/__init__.py` & `seedbank-0.2.0a2/seedbank/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Common infrastructure for initializing random number generators.
 """
+
 # pyright: reportUnknownVariableType=false
 from __future__ import annotations
 
 import logging
 from importlib import import_module
 from importlib.metadata import PackageNotFoundError, version
 from types import ModuleType
@@ -28,14 +29,15 @@
     "make_seed",
     "initialize",
     "init_file",
     "derive_seed",
     "numpy_rng",
     "numpy_random_state",
     "cupy_rng",
+    "SeedLike",
 ]
 
 # This list contains the modules that initialize seeds.
 SEED_INITIALIZERS: list[str | ModuleType] = [
     "seedbank.stdlib",
     "seedbank.numpy",
     "seedbank.numba",
```

### Comparing `seedbank-0.2.0a1/seedbank/_config.py` & `seedbank-0.2.0a2/seedbank/_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Configuration file parsing support.
 """
+
 from __future__ import annotations
 
 import logging
 from os import PathLike
 from pathlib import Path
 from typing import Any
```

### Comparing `seedbank-0.2.0a1/seedbank/_keys.py` & `seedbank-0.2.0a2/seedbank/_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,19 @@
 
 Entropy: TypeAlias = int | Sequence[int] | npt.NDArray[np.uint32]
 RNGKey: TypeAlias = int | np.integer[Any] | npt.NDArray[Any] | bytes | memoryview | str
 SeedLike: TypeAlias = np.random.SeedSequence | RNGKey
 
 
 @overload
-def make_key(data: RNGKey, single: Literal[True]) -> int:
-    ...
+def make_key(data: RNGKey, single: Literal[True]) -> int: ...
 
 
 @overload
-def make_key(data: RNGKey, single: bool = False) -> Entropy:
-    ...
+def make_key(data: RNGKey, single: bool = False) -> Entropy: ...
 
 
 def make_key(data: RNGKey, single: bool = False) -> Entropy:
     """
     Get a key, usable as entropy in a seed sequence, from a piece of data.
 
     Args:
```

### Comparing `seedbank-0.2.0a1/seedbank/_state.py` & `seedbank-0.2.0a2/seedbank/_state.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/seedbank/cupy.py` & `seedbank-0.2.0a2/seedbank/cupy.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/seedbank/numba.py` & `seedbank-0.2.0a2/seedbank/numba.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/seedbank/numpy.py` & `seedbank-0.2.0a2/seedbank/numpy.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/seedbank/tensorflow.py` & `seedbank-0.2.0a2/seedbank/tensorflow.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/seedbank.egg-info/PKG-INFO` & `seedbank-0.2.0a2/seedbank.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: seedbank
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Common infrastructure for seeding random number generators.
 Author-email: Michael Ekstrand <mdekstrand@drexel.edu>
 License: Copyright (c) 2021–2023 Boise State University
-        Copyright (c) 2023 Michael Ekstrand
+        Copyright (c) 2023-2024 Drexel University and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -36,26 +36,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.17
 Requires-Dist: typing-extensions~=4.8
 Provides-Extra: dev
 Requires-Dist: setuptools>=64; extra == "dev"
 Requires-Dist: setuptools_scm>=8; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: build==1.*; extra == "dev"
+Requires-Dist: ruff>=0.2; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
-Requires-Dist: copier; extra == "dev"
+Requires-Dist: copier==9.*; extra == "dev"
+Requires-Dist: unbeheader~=1.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pyproject2conda; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == "test"
 Requires-Dist: pytest-doctestplus; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-cov>=2.12; extra == "test"
+Requires-Dist: coverage>=5; extra == "test"
 Requires-Dist: pyyaml; extra == "test"
 Requires-Dist: toml; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx>=4.2; extra == "doc"
 Requires-Dist: sphinxext-opengraph>=0.5; extra == "doc"
 Requires-Dist: furo; extra == "doc"
 Provides-Extra: numba
```

### Comparing `seedbank-0.2.0a1/seedbank.egg-info/SOURCES.txt` & `seedbank-0.2.0a2/seedbank.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-.copier-answers.yml
 .editorconfig
 .gitattributes
 .gitignore
-.readthedocs.yml
 LICENSE.md
+MANIFEST.in
 README.md
+justfile
 pyproject.toml
-.github/workflows/check-sources.yml
-.github/workflows/test.yml
-.vscode/settings.json
 docs/api.rst
 docs/conf.py
 docs/extending.rst
 docs/index.rst
 docs/patterns.rst
 docs/_templates/base.html
 docs/_templates/footer.html
```

### Comparing `seedbank-0.2.0a1/tests/test_cupy_generator.py` & `seedbank-0.2.0a2/tests/test_cupy_generator.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/tests/test_derive.py` & `seedbank-0.2.0a2/tests/test_derive.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/tests/test_generator.py` & `seedbank-0.2.0a2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/tests/test_init.py` & `seedbank-0.2.0a2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/tests/test_init_file.py` & `seedbank-0.2.0a2/tests/test_init_file.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/tests/test_process_seed.py` & `seedbank-0.2.0a2/tests/test_process_seed.py`

 * *Files identical despite different names*

### Comparing `seedbank-0.2.0a1/tests/test_randomstate.py` & `seedbank-0.2.0a2/tests/test_randomstate.py`

 * *Files identical despite different names*

