# Comparing `tmp/validate_pyproject_schema_store-2024.4.8.tar.gz` & `tmp/validate_pyproject_schema_store-2024.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr  8 09:14:50 2024, max compression
+gzip compressed data, last modified: Mon May 13 23:51:26 2024, max compression
```

## Comparing `validate_pyproject_schema_store-2024.4.8.tar` & `validate_pyproject_schema_store-2024.5.13.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     2272 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      305 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0     2412 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1007 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/workflows/bump.yml
--rw-r--r--   0        0        0      843 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1193 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0      188 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/py.typed
--rw-r--r--   0        0        0     1373 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/schema.py
--rw-r--r--   0        0        0     6871 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/black.schema.json
--rw-r--r--   0        0        0    20516 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
--rw-r--r--   0        0        0    27093 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/hatch.schema.json
--rw-r--r--   0        0        0    44330 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/mypy.schema.json
--rw-r--r--   0        0        0    25354 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pdm.schema.json
--rw-r--r--   0        0        0    20021 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/poetry.schema.json
--rw-r--r--   0        0        0    63177 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pyright.schema.json
--rw-r--r--   0        0        0   125702 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/ruff.schema.json
--rw-r--r--   0        0        0    18672 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
--rw-r--r--   0        0        0    13647 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/setuptools.schema.json
--rw-r--r--   0        0        0      643 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/tool.json
--rw-r--r--   0        0        0      890 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/tests/test_package.py
--rw-r--r--   0        0        0      425 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/tests/test_validate_pyproject.py
--rw-r--r--   0        0        0     2422 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/tools/sync.py
--rw-r--r--   0        0        0     2218 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/.gitignore
--rw-r--r--   0        0        0    11358 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/LICENSE
--rw-r--r--   0        0        0     2081 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/README.md
--rw-r--r--   0        0        0     5445 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/pyproject.toml
--rw-r--r--   0        0        0     4100 2024-04-08 09:14:50.000000 validate_pyproject_schema_store-2024.4.8/PKG-INFO
+-rw-r--r--   0        0        0     2273 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      305 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0     2412 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/release.yml
+-rw-r--r--   0        0        0      668 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1093 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/workflows/bump.yml
+-rw-r--r--   0        0        0      843 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      885 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      188 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/py.typed
+-rw-r--r--   0        0        0     1373 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/schema.py
+-rw-r--r--   0        0        0     6871 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/black.schema.json
+-rw-r--r--   0        0        0    20516 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json
+-rw-r--r--   0        0        0    27093 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/hatch.schema.json
+-rw-r--r--   0        0        0    44330 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/mypy.schema.json
+-rw-r--r--   0        0        0    25354 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pdm.schema.json
+-rw-r--r--   0        0        0    20027 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/poetry.schema.json
+-rw-r--r--   0        0        0    70996 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pyright.schema.json
+-rw-r--r--   0        0        0   128445 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/ruff.schema.json
+-rw-r--r--   0        0        0    20535 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0    13647 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/setuptools.schema.json
+-rw-r--r--   0        0        0      691 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/tool.json
+-rw-r--r--   0        0        0    24630 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/uv.schema.json
+-rw-r--r--   0        0        0      890 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/tests/test_package.py
+-rw-r--r--   0        0        0      850 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/tests/test_validate_pyproject.py
+-rwxr-xr-x   0        0        0     2467 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/tools/sync.py
+-rw-r--r--   0        0        0     2218 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/.gitignore
+-rw-r--r--   0        0        0    11358 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/LICENSE
+-rw-r--r--   0        0        0     2080 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/README.md
+-rw-r--r--   0        0        0     4986 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/pyproject.toml
+-rw-r--r--   0        0        0     4156 2024-05-13 23:51:26.000000 validate_pyproject_schema_store-2024.5.13/PKG-INFO
```

### Comparing `validate_pyproject_schema_store-2024.4.8/.pre-commit-config.yaml` & `validate_pyproject_schema_store-2024.5.13/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==24.*]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
@@ -30,22 +30,22 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: '^src/validate_pyproject_schema_store/resources/.*\.json'
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.5"
+    rev: "v0.4.4"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.9.0"
+    rev: "v1.10.0"
     hooks:
       - id: mypy
         files: src|tests|tools
         args: []
         additional_dependencies:
           - pytest
           - importlib_resources
@@ -69,17 +69,17 @@
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.16
+    rev: v0.17
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.1
+    rev: 0.28.3
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
```

### Comparing `validate_pyproject_schema_store-2024.4.8/.github/CONTRIBUTING.md` & `validate_pyproject_schema_store-2024.5.13/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/.github/matchers/pylint.json` & `validate_pyproject_schema_store-2024.5.13/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/.github/workflows/cd.yml` & `validate_pyproject_schema_store-2024.5.13/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/.github/workflows/ci.yml` & `validate_pyproject_schema_store-2024.5.13/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -17,39 +17,30 @@
 jobs:
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.12"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
-        include:
-          - python-version: pypy-3.10
-            runs-on: ubuntu-latest
-
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - uses: actions/setup-python@v5
         with:
-          python-version: ${{ matrix.python-version }}
-          allow-prereleases: true
+          python-version: |
+            3.8
+            3.9
+            3.10
+            3.11
+            3.12
 
       - name: Setup uv
         uses: yezz123/setup-uv@v4
-        with:
-          uv-venv: ".venv"
-
-      - name: Install package
-        run: uv pip install -e .[test]
 
+      - name: Install Hatch
+        run: uv pip install --system "hatch>=1.10"
       - name: Test package
-        run: >-
-          python -m pytest -ra --cov --cov-report=xml --cov-report=term
-          --durations=20
-
-      - name: Upload coverage report
-        uses: codecov/codecov-action@v4.2.0
+        run: hatch test -ca
```

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/schema.py` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/schema.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/black.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/black.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/cibuildwheel.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/hatch.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/hatch.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/mypy.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/mypy.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pdm.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pdm.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/poetry.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/poetry.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999749599359%*

 * *Differences: {"'definitions'": "{'poetry-git-dependency': {'properties': {'git': {'anyOf': {1: {'pattern': "*

 * *                  "'^([A-Za-z0-9\\\\-]+@|https://|http://)[A-Za-z][A-Za-z0-9+.-]*(:|/)[A-Za-z0-9\\\\-\\\\.]+/[A-Za-z0-9\\\\-_\\\\.]+\\\\.git$'}}}}}}"}*

```diff
@@ -189,15 +189,15 @@
                 },
                 "git": {
                     "anyOf": [
                         {
                             "format": "uri"
                         },
                         {
-                            "pattern": "^([A-Za-z0-9\\-]+@|https://|http://)[A-Za-z][A-Za-z0-9+.-]*(:|/)[A-Za-z0-9\\-]+/[A-Za-z0-9\\-_]+\\.git$"
+                            "pattern": "^([A-Za-z0-9\\-]+@|https://|http://)[A-Za-z][A-Za-z0-9+.-]*(:|/)[A-Za-z0-9\\-\\.]+/[A-Za-z0-9\\-_\\.]+\\.git$"
                         }
                     ],
                     "description": "The url of the git repository.",
                     "type": "string"
                 },
                 "markers": {
                     "description": "The PEP 508 compliant environment markers for which the dependency should be installed.",
```

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/pyright.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/pyright.schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9168222949557181%*

 * *Differences: {"'$comment'": '"This file was originally copied from Pyright\'s repository, which is licensed '*

 * *               'under MIT, on 2024-01-17. The markdownDescription fields are for VSCode and '*

 * *               'x-intellij-html-description ones are for PyCharm."',*

 * * "'properties'": "{'disableBytesTypePromotions': {'markdownDescription': 'Disables legacy behavior "*

 * *                 'where `bytearray` and `memoryview` are considered subtypes of bytes. [PEP '*

 * *                 '688](https://peps.python.org/pep-0688/) […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "$comment": "This file was originallycopied from Pyright's repository, which is licensed under MIT, on 2024-01-17. The markdownDescription fields are for VSCode and x-intellij-html-description ones are for PyCharm.",
+    "$comment": "This file was originally copied from Pyright's repository, which is licensed under MIT, on 2024-01-17. The markdownDescription fields are for VSCode and x-intellij-html-description ones are for PyCharm.",
     "$id": "https://json.schemastore.org/partial-pyright.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "definitions": {
         "diagnostic": {
             "anyOf": [
                 {
                     "type": "boolean"
@@ -44,22 +44,24 @@
             "type": "object",
             "x-intellij-html-description": "Set of identifiers that should be assumed to contain a constant value wherever used within this program. For example, <code>{ &quot;DEBUG&quot;: true }</code> indicates that pyright should assume that the identifier <code>DEBUG</code> will always be equal to <code>True</code>. If this identifier is used within a conditional expression (such as <code>if not DEBUG:</code>) pyright will use the indicated value to determine whether the guarded block is reachable or not. Member expressions that reference one of these constants (e.g. <code>my_module.DEBUG</code>) are also supported."
         },
         "deprecateTypingAliases": {
             "$id": "#/properties/deprecateTypingAliases",
             "default": false,
             "description": "PEP 585 indicates that aliases to types in standard collections that were introduced solely to support generics are deprecated as of Python 3.9. This switch controls whether these are treated as deprecated. This applies only when `pythonVersion` is 3.9 or newer. The default value for this setting is `false` but may be switched to `true` in the future.",
+            "markdownDescription": "[PEP 585](https://peps.python.org/pep-0585/) indicates that aliases to types in standard collections that were introduced solely to support generics are deprecated as of Python 3.9. This switch controls whether these are treated as deprecated. This applies only when `pythonVersion` is 3.9 or newer. The default value for this setting is `false` but may be switched to `true` in the future.",
             "title": "Treat typing-specific aliases to standard types as deprecated",
             "type": "boolean",
             "x-intellij-html-description": "<a href=\"https://peps.python.org/pep-0585/\">PEP 585</a> indicates that aliases to types in standard collections that were introduced solely to support generics are deprecated as of Python 3.9. This switch controls whether these are treated as deprecated. This applies only when <code>pythonVersion</code> is 3.9 or newer. The default value for this setting is <code>false</code> but may be switched to <code>true</code> in the future."
         },
         "disableBytesTypePromotions": {
             "$id": "#/properties/disableBytesTypePromotions",
             "default": false,
             "description": "Disables legacy behavior where `bytearray` and `memoryview` are considered subtypes of bytes. PEP 688 deprecates this behavior, but this switch is provided to restore the older behavior.",
+            "markdownDescription": "Disables legacy behavior where `bytearray` and `memoryview` are considered subtypes of bytes. [PEP 688](https://peps.python.org/pep-0688/) deprecates this behavior, but this switch is provided to restore the older behavior.",
             "title": "Do not treat `bytearray` and `memoryview` as implicit subtypes of `bytes`",
             "type": "boolean",
             "x-intellij-html-description": "Disables legacy behavior where <code>bytearray</code> and <code>memoryview</code> are considered subtypes of bytes. <a href=\"https://peps.python.org/pep-0688/\">PEP 688</a> deprecates this behavior, but this switch is provided to restore the older behavior."
         },
         "enableExperimentalFeatures": {
             "$id": "#/properties/enableExperimentalFeatures",
             "default": false,
@@ -67,14 +69,15 @@
             "title": "Enable the use of experimental features that are not part of the Python typing spec",
             "type": "boolean"
         },
         "enableTypeIgnoreComments": {
             "$id": "#/properties/enableTypeIgnoreComments",
             "default": true,
             "description": "PEP 484 defines support for `# type: ignore` comments. This switch enables or disables support for these comments. This does not affect `# pyright: ignore` comments.",
+            "markdownDescription": "[PEP 484](https://peps.python.org/pep-0484/) defines support for `# type: ignore` comments. This switch enables or disables support for these comments. This does not affect `# pyright: ignore` comments.",
             "title": "Allow `# type: ignore` comments",
             "type": "boolean",
             "x-intellij-html-description": "<a href=\"https://peps.python.org/pep-0484/\">PEP 484</a> defines support for <code># type: ignore</code> comments. This switch enables or disables support for these comments. This does not affect <code># pyright: ignore</code> comments."
         },
         "exclude": {
             "$id": "#/properties/exclude",
             "description": "Paths of directories or files that should not be included. These override the includes directories, allowing specific subdirectories to be ignored. Note that files in the exclude paths may still be included in the analysis if they are referenced (imported) by source files that are not excluded. Paths may contain wildcard characters: `**` (a directory or multiple levels of directories), `*` (a sequence of zero or more characters), or `?` (a single character). If no exclude paths are specified, Pyright automatically excludes the following: `**/node_modules`, `**/__pycache__`, `**/.*` and any virtual environment directories.",
@@ -209,29 +212,72 @@
                 "3.7"
             ],
             "pattern": "^3\\.[0-9]+$",
             "title": "Python version to assume during type analysis",
             "type": "string",
             "x-intellij-html-description": "Specifies the version of Python that will be used to execute the source code. The version should be specified as a string in the format <code>M.m</code> where <code>M</code> is the major version and <code>m</code> is the minor (e.g. <code>3.0</code> or <code>3.6</code>). If a version is provided, pyright will generate errors if the source code makes use of language features that are not supported in that version. It will also tailor its use of type stub files, which conditionalizes type definitions based on the version. If no version is specified, pyright will use the version of the current python interpreter, if one is present."
         },
+        "reportAbstractUsage": {
+            "$id": "#/properties/reportAbstractUsage",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for the attempted instantiate an abstract or protocol class or use of an abstract method.",
+            "title": "Controls reporting of attempted instantiation of abstract class"
+        },
+        "reportArgumentType": {
+            "$id": "#/properties/reportArgumentType",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for argument type incompatibilities when evaluating a call expression.",
+            "title": "Controls reporting of incompatible argument type"
+        },
         "reportAssertAlwaysTrue": {
             "$id": "#/properties/reportAssertAlwaysTrue",
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
             "description": "Generate or suppress diagnostics for `assert` statement that will provably always assert. This can be indicative of a programming error.",
             "title": "Controls reporting `assert` expressions that will always evaluate to `True`",
             "x-intellij-html-description": "Generate or suppress diagnostics for <code>assert</code> statement that will provably always assert. This can be indicative of a programming error."
         },
+        "reportAssertTypeFailure": {
+            "$id": "#/properties/reportAssertTypeFailure",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for a type mismatch detected by the `typing.assert_type` call.",
+            "title": "Controls reporting of type mismatch detected by `typing.assert_type` call",
+            "x-intellij-html-description": "Generate or suppress diagnostics for a type mismatch detected by the <code>typing.assert_type</code> call."
+        },
+        "reportAssignmentType": {
+            "$id": "#/properties/reportAssignmentType",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for assignment type incompatibility.",
+            "title": "Controls reporting of type incompatibilities for assignments"
+        },
+        "reportAttributeAccessIssue": {
+            "$id": "#/properties/reportAttributeAccessIssue",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics related to attribute accesses.",
+            "title": "Controls reporting of issues related to attribute accesses"
+        },
         "reportCallInDefaultInitializer": {
             "$id": "#/properties/reportCallInDefaultInitializer",
             "$ref": "#/definitions/diagnostic",
             "default": "none",
             "description": "Generate or suppress diagnostics for function calls, list expressions, set expressions, or dictionary expressions within a default value initialization expression. Such calls can mask expensive operations that are performed at module initialization time.",
             "title": "Controls reporting usage of function calls within a default value initializer expression"
         },
+        "reportCallIssue": {
+            "$id": "#/properties/reportCallIssue",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics related to call expressions and arguments passed to a call target.",
+            "title": "Controls reporting of issues related to call expressions and arguments"
+        },
         "reportConstantRedefinition": {
             "$id": "#/properties/reportConstantRedefinition",
             "$ref": "#/definitions/diagnostic",
             "default": "none",
             "description": "Generate or suppress diagnostics for attempts to redefine variables whose names are all-caps with underscores and numerals.",
             "title": "Controls reporting of attempts to redefine variables that are in all-caps"
         },
@@ -270,15 +316,15 @@
             "description": "Generate or suppress diagnostics for overridden methods in a class that are missing an explicit `@override` decorator.",
             "title": "Controls reporting overridden methods that are missing an `@override` decorator",
             "x-intellij-html-description": "Generate or suppress diagnostics for overridden methods in a class that are missing an explicit <code>@override</code> decorator."
         },
         "reportImplicitStringConcatenation": {
             "$id": "#/properties/reportImplicitStringConcatenation",
             "$ref": "#/definitions/diagnostic",
-            "default": "warning",
+            "default": "none",
             "description": "Generate or suppress diagnostics for two or more string literals that follow each other, indicating an implicit concatenation. This is considered a bad practice and often masks bugs such as missing commas.",
             "title": "Controls reporting usage of implicit concatenation of string literals"
         },
         "reportImportCycles": {
             "$id": "#/properties/reportImportCycles",
             "$ref": "#/definitions/diagnostic",
             "default": "none",
@@ -311,28 +357,56 @@
             "$id": "#/properties/reportInconsistentConstructor",
             "$ref": "#/definitions/diagnostic",
             "default": "none",
             "description": "Generate or suppress diagnostics when an `__init__` method signature is inconsistent with a `__new__` signature.",
             "title": "Controls reporting of `__init__` and `__new__` methods whose signatures are inconsistent",
             "x-intellij-html-description": "Generate or suppress diagnostics when an <code>__init__</code> method signature is inconsistent with a <code>__new__</code> signature."
         },
+        "reportInconsistentOverload": {
+            "$id": "#/properties/reportInconsistentOverload",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for an overloaded function that has overload signatures that are inconsistent with each other or with the implementation.",
+            "title": "Controls reporting of inconsistencies between function overload signatures"
+        },
+        "reportIndexIssue": {
+            "$id": "#/properties/reportIndexIssue",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics related to index operations and expressions.",
+            "title": "Controls reporting of issues related to index operations and expressions"
+        },
         "reportInvalidStringEscapeSequence": {
             "$id": "#/properties/reportInvalidStringEscapeSequence",
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
             "description": "Generate or suppress diagnostics for invalid escape sequences used within string literals. The Python specification indicates that such sequences will generate a syntax error in future versions.",
             "title": "Controls reporting of invalid escape sequences used within string literals"
         },
         "reportInvalidStubStatement": {
             "$id": "#/properties/reportInvalidStubStatement",
             "$ref": "#/definitions/diagnostic",
             "default": "none",
             "description": "Generate or suppress diagnostics for statements that are syntactically correct but have no purpose within a type stub file.",
             "title": "Controls reporting of type stub statements that do not conform to PEP 484"
         },
+        "reportInvalidTypeArguments": {
+            "$id": "#/properties/reportInvalidTypeArguments",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for invalid type argument usage.",
+            "title": "Controls reporting of invalid type argument usage"
+        },
+        "reportInvalidTypeForm": {
+            "$id": "#/properties/reportInvalidTypeForm",
+            "$ref": "#/definitions/diagnostic",
+            "default": "warning",
+            "description": "Generate or suppress diagnostics for type annotations that use invalid type expression forms or are semantically invalid.",
+            "title": "Controls reporting of type expressions that use an invalid form"
+        },
         "reportInvalidTypeVarUse": {
             "$id": "#/properties/reportInvalidTypeVarUse",
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
             "description": "Generate or suppress diagnostics when a `TypeVar` is used inappropriately (e.g. if a `TypeVar` appears only once) within a generic function signature.",
             "title": "Controls reporting improper use of type variables within function signatures",
             "x-intellij-html-description": "Generate or suppress diagnostics when a <code>TypeVar</code> is used inappropriately (e.g. if a <code>TypeVar</code> appears only once) within a generic function signature."
@@ -385,14 +459,29 @@
         "reportMissingTypeStubs": {
             "$id": "#/properties/reportMissingTypeStubs",
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
             "description": "Generate or suppress diagnostics for imports that have no corresponding type stub file (either a typeshed file or a custom type stub). The type checker requires type stubs to do its best job at analysis.",
             "title": "Controls reporting of imports that cannot be resolved to type stub files"
         },
+        "reportNoOverloadImplementation": {
+            "$id": "#/properties/reportNoOverloadImplementation",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for an overloaded function or method if the implementation is not provided.",
+            "title": "Controls reporting of an overloaded function or method with a missing implementation"
+        },
+        "reportOperatorIssue": {
+            "$id": "#/properties/reportOperatorIssue",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics related to the use of unary or binary operators (like `*` or `not`).",
+            "title": "Controls reporting of diagnostics related to unary and binary operators",
+            "x-intellij-html-description": "Generate or suppress diagnostics related to the use of unary or binary operators (like <code>*</code> or <code>not</code>)."
+        },
         "reportOptionalCall": {
             "$id": "#/properties/reportOptionalCall",
             "$ref": "#/definitions/diagnostic",
             "default": "error",
             "description": "Generate or suppress diagnostics for an attempt to call a variable with an `Optional` type.",
             "title": "Controls reporting of attempts to call a variable with `Optional` type",
             "x-intellij-html-description": "Generate or suppress diagnostics for an attempt to call a variable with an <code>Optional</code> type."
@@ -440,14 +529,21 @@
         "reportOverlappingOverload": {
             "$id": "#/properties/reportOverlappingOverload",
             "$ref": "#/definitions/diagnostic",
             "default": "error",
             "description": "Generate or suppress diagnostics for function overloads that overlap in signature and obscure each other or have incompatible return types.",
             "title": "Controls reporting of function overloads that overlap in signature and obscure each other or do not agree on return type"
         },
+        "reportPossiblyUnboundVariable": {
+            "$id": "#/properties/reportPossiblyUnboundVariable",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for variables that are possibly unbound on some code paths.",
+            "title": "Controls reporting of attempts to use variable that is possibly unbound on some code paths"
+        },
         "reportPrivateImportUsage": {
             "$id": "#/properties/reportPrivateImportUsage",
             "$ref": "#/definitions/diagnostic",
             "default": "error",
             "description": "Generate or suppress diagnostics for use of a symbol from a `py.typed` module that is not meant to be exported from that module.",
             "title": "Controls reporting of improper usage of symbol imported from a `py.typed` module that is not re-exported from that module",
             "x-intellij-html-description": "Generate or suppress diagnostics for use of a symbol from a <code>py.typed</code> module that is not meant to be exported from that module."
@@ -463,14 +559,28 @@
         "reportPropertyTypeMismatch": {
             "$id": "#/properties/reportPropertyTypeMismatch",
             "$ref": "#/definitions/diagnostic",
             "default": "none",
             "description": "Generate or suppress diagnostics for properties where the type of the value passed to the setter is not assignable to the value returned by the getter. Such mismatches violate the intended use of properties, which are meant to act like variables.",
             "title": "Controls reporting of property getter/setter type mismatches"
         },
+        "reportRedeclaration": {
+            "$id": "#/properties/reportRedeclaration",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for a symbol that has more than one type declaration.",
+            "title": "Controls reporting of attempts to declare the type of a symbol multiple times"
+        },
+        "reportReturnType": {
+            "$id": "#/properties/reportReturnType",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics related to function return type compatibility.",
+            "title": "Controls reporting of function return type incompatibility"
+        },
         "reportSelfClsParameterName": {
             "$id": "#/properties/reportSelfClsParameterName",
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
             "description": "Generate or suppress diagnostics for a missing or misnamed `self` parameter in instance methods and `cls` parameter in class methods. Instance methods in metaclasses (classes that derive from `type`) are allowed to use `cls` for instance methods.",
             "title": "Controls reporting missing or misnamed `self` parameters",
             "x-intellij-html-description": "Generate or suppress diagnostics for a missing or misnamed <code>self</code> parameter in instance methods and <code>cls</code> parameter in class methods. Instance methods in metaclasses (classes that derive from <code>type</code>) are allowed to use <code>cls</code> for instance methods."
@@ -497,24 +607,31 @@
             "title": "Controls reporting of attempts to access a non-required key in a `TypedDict` without a check for its presence",
             "x-intellij-html-description": "Generate or suppress diagnostics for an attempt to access a non-required field within a <code>TypedDict</code> without first checking whether it is present."
         },
         "reportUnboundVariable": {
             "$id": "#/properties/reportUnboundVariable",
             "$ref": "#/definitions/diagnostic",
             "default": "error",
-            "description": "Generate or suppress diagnostics for unbound and possibly unbound variables.",
-            "title": "Controls reporting of attempts to use an unbound or possibly unbound variable"
+            "description": "Generate or suppress diagnostics for unbound variables.",
+            "title": "Controls reporting of attempts to use an unbound variable"
         },
         "reportUndefinedVariable": {
             "$id": "#/properties/reportUndefinedVariable",
             "$ref": "#/definitions/diagnostic",
             "default": "error",
             "description": "Generate or suppress diagnostics for undefined variables.",
             "title": "Controls reporting of attempts to use an undefined variable"
         },
+        "reportUnhashable": {
+            "$id": "#/properties/reportUnhashable",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for the use of an unhashable object in a container that requires hashability.",
+            "title": "Controls reporting of unhashable object in container that requires hashability"
+        },
         "reportUninitializedInstanceVariable": {
             "$id": "#/properties/reportUninitializedInstanceVariable",
             "$ref": "#/definitions/diagnostic",
             "default": "none",
             "description": "Generate or suppress diagnostics for instance variables within a class that are not initialized or declared within the class body or the `__init__` method.",
             "title": "Controls reporting of instance variables that are not initialized in the constructor",
             "x-intellij-html-description": "Generate or suppress diagnostics for instance variables within a class that are not initialized or declared within the class body or the <code>__init__</code> method."
@@ -650,14 +767,22 @@
             "$id": "#/properties/reportUnusedCoroutine",
             "$ref": "#/definitions/diagnostic",
             "default": "error",
             "description": "Generate or suppress diagnostics for call statements whose return value is not used in any way and is a `Coroutine`. This identifies a common error where an `await` keyword is mistakenly omitted.",
             "title": "Controls reporting of call expressions that returns `Coroutine` whose results are not consumed",
             "x-intellij-html-description": "Generate or suppress diagnostics for call statements whose return value is not used in any way and is a <code>Coroutine</code>. This identifies a common error where an <code>await</code> keyword is mistakenly omitted."
         },
+        "reportUnusedExcept": {
+            "$id": "#/properties/reportUnusedExcept",
+            "$ref": "#/definitions/diagnostic",
+            "default": "error",
+            "description": "Generate or suppress diagnostics for an `except` clause that will never be reached.",
+            "title": "Controls reporting of unreachable except clauses",
+            "x-intellij-html-description": "Generate or suppress diagnostics for an <code>except</code> clause that will never be reached."
+        },
         "reportUnusedExpression": {
             "$id": "#/properties/reportUnusedExpression",
             "$ref": "#/definitions/diagnostic",
             "default": "warning",
             "description": "Generate or suppress diagnostics for simple expressions whose results are not used in any way.",
             "title": "Controls reporting of simple expressions whose value is not used in any way"
         },
@@ -718,14 +843,15 @@
             "type": "boolean",
             "x-intellij-html-description": "When inferring the type of a list, use strict type assumptions. For example, the expression <code>[1, &#39;a&#39;, 3.4]</code> could be inferred to be of type <code>list[Any]</code> or <code>list[int | str | float]</code>. If this setting is <code>true</code>, it will use the latter (stricter) type."
         },
         "strictParameterNoneValue": {
             "$id": "#/properties/strictParameterNoneValue",
             "default": true,
             "description": "PEP 484 indicates that when a function parameter is assigned a default value of `None`, its type should implicitly be `Optional` even if the explicit type is not. When enabled, this rule requires that parameter type annotations use `Optional` explicitly in this case.",
+            "markdownDescription": "[PEP 484](https://peps.python.org/pep-0484/) indicates that when a function parameter is assigned a default value of `None`, its type should implicitly be `Optional` even if the explicit type is not. When enabled, this rule requires that parameter type annotations use `Optional` explicitly in this case.",
             "title": "Allow implicit Optional when default parameter value is None",
             "type": "boolean",
             "x-intellij-html-description": "<a href=\"https://peps.python.org/pep-0484/\">PEP 484</a> indicates that when a function parameter is assigned a default value of <code>None</code>, its type should implicitly be <code>Optional</code> even if the explicit type is not. When enabled, this rule requires that parameter type annotations use <code>Optional</code> explicitly in this case."
         },
         "strictSetInference": {
             "$id": "#/properties/strictSetInference",
             "default": false,
```

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/ruff.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/ruff.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963602140324771%*

 * *Differences: {"'definitions'": "{'Flake8CopyrightOptions': {'properties': {'author': {'type': {insert: [(1, "*

 * *                  "'null')], delete: [0]}}, 'notice-rgx': {'type': {insert: [(1, 'null')], delete: "*

 * *                  "[0]}, 'description': 'The regular expression used to match the copyright "*

 * *                  'notice, compiled with the [`regex`](https://docs.rs/regex/latest/regex/) crate. '*

 * *                  'Defaults to '*

 * *                  '`(?i)Copyright\\\\s+((?:\\\\(C\\\\)|©)\\\\s+)?\\\\d{4}((-|,\\\\s)\\ […]*

```diff
@@ -151,14 +151,30 @@
                         "array",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
+        "Flake8BooleanTrapOptions": {
+            "additionalProperties": false,
+            "properties": {
+                "extend-allowed-calls": {
+                    "description": "Additional callable functions with which to allow boolean traps.\n\nExpects to receive a list of fully-qualified names (e.g., `pydantic.Field`, rather than `Field`).",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": [
+                        "array",
+                        "null"
+                    ]
+                }
+            },
+            "type": "object"
+        },
         "Flake8BugbearOptions": {
             "additionalProperties": false,
             "properties": {
                 "extend-immutable-calls": {
                     "description": "Additional callable functions to consider \"immutable\" when evaluating, e.g., the `function-call-in-default-argument` rule (`B008`) or `function-call-in-dataclass-defaults` rule (`RUF009`).\n\nExpects to receive a list of fully-qualified names (e.g., `fastapi.Query`, rather than `Query`).",
                     "items": {
                         "type": "string"
@@ -202,44 +218,44 @@
         },
         "Flake8CopyrightOptions": {
             "additionalProperties": false,
             "properties": {
                 "author": {
                     "description": "Author to enforce within the copyright notice. If provided, the author must be present immediately following the copyright notice.",
                     "type": [
-                        "null",
-                        "string"
+                        "string",
+                        "null"
                     ]
                 },
                 "min-file-size": {
                     "description": "A minimum file size (in bytes) required for a copyright notice to be enforced. By default, all files are validated.",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "notice-rgx": {
-                    "description": "The regular expression used to match the copyright notice, compiled with the [`regex`](https://docs.rs/regex/latest/regex/) crate. Defaults to `(?i)Copyright\\s+((?:\\(C\\)|\u00a9)\\s+)?\\d{4}((-|,\\s)\\d{4})*`, which matches the following: - `Copyright 2023` - `Copyright (C) 2023` - `Copyright 2021-2023` - `Copyright (C) 2021-2023` - `Copyright (C) 2021, 2023`",
+                    "description": "The regular expression used to match the copyright notice, compiled with the [`regex`](https://docs.rs/regex/latest/regex/) crate. Defaults to `(?i)Copyright\\s+((?:\\(C\\)|\u00a9)\\s+)?\\d{4}((-|,\\s)\\d{4})*`, which matches the following:\n\n- `Copyright 2023` - `Copyright (C) 2023` - `Copyright 2021-2023` - `Copyright (C) 2021-2023` - `Copyright (C) 2021, 2023`",
                     "type": [
-                        "null",
-                        "string"
+                        "string",
+                        "null"
                     ]
                 }
             },
             "type": "object"
         },
         "Flake8ErrMsgOptions": {
             "additionalProperties": false,
             "properties": {
                 "max-string-length": {
                     "description": "Maximum string length for string literals in exception messages.",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
@@ -286,28 +302,28 @@
         "Flake8ImportConventionsOptions": {
             "additionalProperties": false,
             "properties": {
                 "aliases": {
                     "additionalProperties": {
                         "type": "string"
                     },
-                    "description": "The conventional aliases for imports. These aliases can be extended by the `extend_aliases` option.",
+                    "description": "The conventional aliases for imports. These aliases can be extended by the `extend-aliases` option.",
                     "type": [
-                        "null",
-                        "object"
+                        "object",
+                        "null"
                     ]
                 },
                 "banned-aliases": {
                     "additionalProperties": {
                         "$ref": "#/definitions/BannedAliases"
                     },
                     "description": "A mapping from module to its banned import aliases.",
                     "type": [
-                        "null",
-                        "object"
+                        "object",
+                        "null"
                     ]
                 },
                 "banned-from": {
                     "description": "A list of modules that should not be imported from using the `from ... import ...` syntax.\n\nFor example, given `banned-from = [\"pandas\"]`, `from pandas import DataFrame` would be disallowed, while `import pandas` would be allowed.",
                     "items": {
                         "type": "string"
                     },
@@ -319,16 +335,16 @@
                 },
                 "extend-aliases": {
                     "additionalProperties": {
                         "type": "string"
                     },
                     "description": "A mapping from module to conventional import alias. These aliases will be added to the `aliases` mapping.",
                     "type": [
-                        "null",
-                        "object"
+                        "object",
+                        "null"
                     ]
                 }
             },
             "type": "object"
         },
         "Flake8PytestStyleOptions": {
             "additionalProperties": false,
@@ -491,16 +507,16 @@
                 },
                 "banned-api": {
                     "additionalProperties": {
                         "$ref": "#/definitions/ApiBan"
                     },
                     "description": "Specific modules or module members that may not be imported or accessed. Note that this rule is only meant to flag accidental uses, and can be circumvented via `eval` or `importlib`.",
                     "type": [
-                        "null",
-                        "object"
+                        "object",
+                        "null"
                     ]
                 },
                 "banned-module-level-imports": {
                     "description": "List of specific modules that may not be imported at module level, and should instead be imported lazily (e.g., within a function definition, or an `if TYPE_CHECKING:` block, or some other nested context).",
                     "items": {
                         "type": "string"
                     },
@@ -641,15 +657,15 @@
                         {
                             "$ref": "#/definitions/QuoteStyle"
                         },
                         {
                             "type": "null"
                         }
                     ],
-                    "description": "Configures the preferred quote character for strings. The recommended options are * `double` (default): Use double quotes `\"` * `single`: Use single quotes `'`\n\nIn compliance with [PEP 8](https://peps.python.org/pep-0008/) and [PEP 257](https://peps.python.org/pep-0257/), Ruff prefers double quotes for triple quoted strings and docstrings even when using `quote-style = \"single\"`.\n\nRuff deviates from using the configured quotes if doing so prevents the need for escaping quote characters inside the string:\n\n```python a = \"a string without any quotes\" b = \"It's monday morning\" ```\n\nRuff will change the quotes of the string assigned to `a` to single quotes when using `quote-style = \"single\"`. However, ruff uses double quotes for he string assigned to `b` because using single quotes would require escaping the `'`, which leads to the less readable code: `'It\\'s monday morning'`.\n\nIn addition, Ruff supports the quote style `preserve` for projects that already use a mixture of single and double quotes and can't migrate to the `double` or `single` style. The quote style `preserve` leaves the quotes of all strings unchanged."
+                    "description": "Configures the preferred quote character for strings. The recommended options are\n\n* `double` (default): Use double quotes `\"` * `single`: Use single quotes `'`\n\nIn compliance with [PEP 8](https://peps.python.org/pep-0008/) and [PEP 257](https://peps.python.org/pep-0257/), Ruff prefers double quotes for triple quoted strings and docstrings even when using `quote-style = \"single\"`.\n\nRuff deviates from using the configured quotes if doing so prevents the need for escaping quote characters inside the string:\n\n```python a = \"a string without any quotes\" b = \"It's monday morning\" ```\n\nRuff will change the quotes of the string assigned to `a` to single quotes when using `quote-style = \"single\"`. However, ruff uses double quotes for he string assigned to `b` because using single quotes would require escaping the `'`, which leads to the less readable code: `'It\\'s monday morning'`.\n\nIn addition, Ruff supports the quote style `preserve` for projects that already use a mixture of single and double quotes and can't migrate to the `double` or `single` style. The quote style `preserve` leaves the quotes of all strings unchanged."
                 },
                 "skip-magic-trailing-comma": {
                     "description": "Ruff uses existing trailing commas as an indication that short lines should be left separate. If this option is set to `true`, the magic trailing comma is ignored.\n\nFor example, Ruff leaves the arguments separate even though collapsing the arguments to a single line doesn't exceed the line length if `skip-magic-trailing-comma = false`:\n\n```python # The arguments remain on separate lines because of the trailing comma after `b` def test( a, b, ): pass ```\n\nSetting `skip-magic-trailing-comma = true` changes the formatting to:\n\n```python # The arguments remain on separate lines because of the trailing comma after `b` def test(a, b): pass ```",
                     "type": [
                         "boolean",
                         "null"
                     ]
@@ -665,19 +681,19 @@
                 {
                     "type": "string"
                 }
             ]
         },
         "ImportType": {
             "enum": [
-                "first-party",
                 "future",
-                "local-folder",
                 "standard-library",
-                "third-party"
+                "third-party",
+                "first-party",
+                "local-folder"
             ],
             "type": "string"
         },
         "IndentStyle": {
             "oneOf": [
                 {
                     "description": "Use tabs to indent code.",
@@ -694,15 +710,15 @@
                     "type": "string"
                 }
             ]
         },
         "IndentWidth": {
             "description": "The size of a tab.",
             "format": "uint8",
-            "minimum": 1,
+            "minimum": 1.0,
             "type": "integer"
         },
         "IsortOptions": {
             "additionalProperties": false,
             "properties": {
                 "case-sensitive": {
                     "description": "Sort imports taking into account case sensitivity.",
@@ -865,15 +881,15 @@
                         "integer",
                         "null"
                     ]
                 },
                 "lines-between-types": {
                     "description": "The number of lines to place between \"direct\" and `import from` imports.\n\nWhen using the formatter, only the values `0` and `1` are compatible because it preserves up to one empty line after imports in nested blocks.",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "no-lines-before": {
                     "description": "A list of sections that should _not_ be delineated from the previous section via empty lines.",
@@ -933,18 +949,18 @@
                 "sections": {
                     "additionalProperties": {
                         "items": {
                             "type": "string"
                         },
                         "type": "array"
                     },
-                    "description": "A list of mappings from section names to modules. By default custom sections are output last, but this can be overridden with `section-order`.",
+                    "description": "A list of mappings from section names to modules.\n\nBy default, imports are categorized according to their type (e.g., `future`, `third-party`, and so on). This setting allows you to group modules into custom sections, to augment or override the built-in sections.\n\nFor example, to group all testing utilities, you could create a `testing` section: ```toml testing = [\"pytest\", \"hypothesis\"] ```\n\nThe values in the list are treated as glob patterns. For example, to match all packages in the LangChain ecosystem (`langchain-core`, `langchain-openai`, etc.): ```toml langchain = [\"langchain-*\"] ```\n\nCustom sections should typically be inserted into the `section-order` list to ensure that they're displayed as a standalone group and in the intended order, as in: ```toml section-order = [ \"future\", \"standard-library\", \"third-party\", \"first-party\", \"local-folder\", \"testing\" ] ```\n\nIf a custom section is omitted from `section-order`, imports in that section will be assigned to the `default-section` (which defaults to `third-party`).",
                     "type": [
-                        "null",
-                        "object"
+                        "object",
+                        "null"
                     ]
                 },
                 "single-line-exclusions": {
                     "description": "One or more modules to exclude from the single line rule.",
                     "items": {
                         "type": "string"
                     },
@@ -1004,22 +1020,22 @@
                     "type": "string"
                 }
             ]
         },
         "LineLength": {
             "description": "The length of a line of text that is considered too long.\n\nThe allowed range of values is 1..=320",
             "format": "uint16",
-            "maximum": 320,
-            "minimum": 1,
+            "maximum": 320.0,
+            "minimum": 1.0,
             "type": "integer"
         },
         "LineWidth": {
             "description": "The maximum visual width to which the formatter should try to limit a line.",
             "format": "uint16",
-            "minimum": 1,
+            "minimum": 1.0,
             "type": "integer"
         },
         "LintOptions": {
             "additionalProperties": false,
             "description": "Configures how ruff checks your code.\n\nOptions specified in the `lint` section take precedence over the deprecated top-level settings.",
             "properties": {
                 "allowed-confusables": {
@@ -1033,16 +1049,16 @@
                         "array",
                         "null"
                     ]
                 },
                 "dummy-variable-rgx": {
                     "description": "A regular expression used to identify \"dummy\" variables, or those which should be ignored when enforcing (e.g.) unused-variable rules. The default expression matches `_`, `__`, and `_var`, but not `_var_`.",
                     "type": [
-                        "null",
-                        "string"
+                        "string",
+                        "null"
                     ]
                 },
                 "exclude": {
                     "description": "A list of file patterns to exclude from linting in addition to the files excluded globally (see [`exclude`](#exclude), and [`extend-exclude`](#extend-exclude)).\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).",
                     "items": {
                         "type": "string"
                     },
@@ -1084,16 +1100,16 @@
                         "items": {
                             "$ref": "#/definitions/RuleSelector"
                         },
                         "type": "array"
                     },
                     "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, in addition to any rules excluded by `per-file-ignores`.",
                     "type": [
-                        "null",
-                        "object"
+                        "object",
+                        "null"
                     ]
                 },
                 "extend-safe-fixes": {
                     "description": "A list of rule codes or prefixes for which unsafe fixes should be considered safe.",
                     "items": {
                         "$ref": "#/definitions/RuleSelector"
                     },
@@ -1171,14 +1187,25 @@
                         },
                         {
                             "type": "null"
                         }
                     ],
                     "description": "Options for the `flake8-bandit` plugin."
                 },
+                "flake8-boolean-trap": {
+                    "anyOf": [
+                        {
+                            "$ref": "#/definitions/Flake8BooleanTrapOptions"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "description": "Options for the `flake8-boolean-trap` plugin."
+                },
                 "flake8-bugbear": {
                     "anyOf": [
                         {
                             "$ref": "#/definitions/Flake8BugbearOptions"
                         },
                         {
                             "type": "null"
@@ -1392,18 +1419,18 @@
                 "per-file-ignores": {
                     "additionalProperties": {
                         "items": {
                             "$ref": "#/definitions/RuleSelector"
                         },
                         "type": "array"
                     },
-                    "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files.",
+                    "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files. An initial '!' negates the file pattern.",
                     "type": [
-                        "null",
-                        "object"
+                        "object",
+                        "null"
                     ]
                 },
                 "preview": {
                     "description": "Whether to enable preview mode. When preview mode is enabled, Ruff will use unstable rules and fixes.",
                     "type": [
                         "boolean",
                         "null"
@@ -1509,42 +1536,42 @@
         },
         "McCabeOptions": {
             "additionalProperties": false,
             "properties": {
                 "max-complexity": {
                     "description": "The maximum McCabe complexity to allow before triggering `C901` errors.",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
         "ParametrizeNameType": {
             "enum": [
                 "csv",
-                "list",
-                "tuple"
+                "tuple",
+                "list"
             ],
             "type": "string"
         },
         "ParametrizeValuesRowType": {
             "enum": [
-                "list",
-                "tuple"
+                "tuple",
+                "list"
             ],
             "type": "string"
         },
         "ParametrizeValuesType": {
             "enum": [
-                "list",
-                "tuple"
+                "tuple",
+                "list"
             ],
             "type": "string"
         },
         "Pep8NamingOptions": {
             "additionalProperties": false,
             "properties": {
                 "classmethod-decorators": {
@@ -1714,103 +1741,103 @@
                         "array",
                         "null"
                     ]
                 },
                 "max-args": {
                     "description": "Maximum number of arguments allowed for a function or method definition (see: `PLR0913`).",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-bool-expr": {
                     "description": "Maximum number of Boolean expressions allowed within a single `if` statement (see: `PLR0916`).",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-branches": {
                     "description": "Maximum number of branches allowed for a function or method body (see: `PLR0912`).",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-locals": {
                     "description": "Maximum number of local variables allowed for a function or method body (see: `PLR0914`).",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-nested-blocks": {
                     "description": "Maximum number of nested blocks allowed within a function or method body (see: `PLR1702`).",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-positional-args": {
                     "description": "Maximum number of positional arguments allowed for a function or method definition (see: `PLR0917`).\n\nIf not specified, defaults to the value of `max-args`.",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-public-methods": {
                     "description": "Maximum number of public methods allowed for a class (see: `PLR0904`).",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-returns": {
                     "description": "Maximum number of return statements allowed for a function or method body (see `PLR0911`)",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 },
                 "max-statements": {
                     "description": "Maximum number of statements allowed for a function or method body (see: `PLR0915`).",
                     "format": "uint",
-                    "minimum": 0,
+                    "minimum": 0.0,
                     "type": [
                         "integer",
                         "null"
                     ]
                 }
             },
             "type": "object"
         },
         "PythonVersion": {
             "enum": [
-                "py310",
-                "py311",
-                "py312",
                 "py37",
                 "py38",
-                "py39"
+                "py39",
+                "py310",
+                "py311",
+                "py312"
             ],
             "type": "string"
         },
         "Quote": {
             "oneOf": [
                 {
                     "description": "Use double quotes.",
@@ -1826,17 +1853,17 @@
                     ],
                     "type": "string"
                 }
             ]
         },
         "QuoteStyle": {
             "enum": [
+                "single",
                 "double",
-                "preserve",
-                "single"
+                "preserve"
             ],
             "type": "string"
         },
         "RelativeImportsOrder": {
             "oneOf": [
                 {
                     "description": "Place \"closer\" imports (fewer `.` characters, most local) before \"further\" imports (more `.` characters, least local).",
@@ -1944,14 +1971,15 @@
                 "B033",
                 "B034",
                 "B035",
                 "B9",
                 "B90",
                 "B904",
                 "B905",
+                "B909",
                 "BLE",
                 "BLE0",
                 "BLE00",
                 "BLE001",
                 "C",
                 "C4",
                 "C40",
@@ -2258,43 +2286,52 @@
                 "FLY0",
                 "FLY00",
                 "FLY002",
                 "FURB",
                 "FURB1",
                 "FURB10",
                 "FURB101",
+                "FURB103",
                 "FURB105",
                 "FURB11",
+                "FURB110",
                 "FURB113",
+                "FURB116",
                 "FURB118",
                 "FURB12",
                 "FURB129",
                 "FURB13",
                 "FURB131",
                 "FURB132",
                 "FURB136",
                 "FURB14",
                 "FURB140",
+                "FURB142",
                 "FURB145",
                 "FURB148",
                 "FURB15",
                 "FURB152",
+                "FURB157",
                 "FURB16",
                 "FURB161",
                 "FURB163",
+                "FURB164",
+                "FURB166",
                 "FURB167",
                 "FURB168",
                 "FURB169",
                 "FURB17",
                 "FURB171",
                 "FURB177",
                 "FURB18",
                 "FURB180",
                 "FURB181",
                 "FURB187",
+                "FURB19",
+                "FURB192",
                 "G",
                 "G0",
                 "G00",
                 "G001",
                 "G002",
                 "G003",
                 "G004",
@@ -2477,16 +2514,20 @@
                 "PLE023",
                 "PLE0237",
                 "PLE024",
                 "PLE0241",
                 "PLE03",
                 "PLE030",
                 "PLE0302",
+                "PLE0303",
                 "PLE0304",
+                "PLE0305",
                 "PLE0307",
+                "PLE0308",
+                "PLE0309",
                 "PLE06",
                 "PLE060",
                 "PLE0604",
                 "PLE0605",
                 "PLE064",
                 "PLE0643",
                 "PLE07",
@@ -2525,14 +2566,18 @@
                 "PLE2502",
                 "PLE251",
                 "PLE2510",
                 "PLE2512",
                 "PLE2513",
                 "PLE2514",
                 "PLE2515",
+                "PLE4",
+                "PLE47",
+                "PLE470",
+                "PLE4703",
                 "PLR",
                 "PLR0",
                 "PLR01",
                 "PLR012",
                 "PLR0124",
                 "PLR013",
                 "PLR0133",
@@ -2563,59 +2608,67 @@
                 "PLR1704",
                 "PLR171",
                 "PLR1711",
                 "PLR1714",
                 "PLR172",
                 "PLR1722",
                 "PLR173",
+                "PLR1730",
                 "PLR1733",
                 "PLR1736",
                 "PLR2",
                 "PLR20",
                 "PLR200",
                 "PLR2004",
                 "PLR204",
                 "PLR2044",
                 "PLR5",
                 "PLR55",
                 "PLR550",
                 "PLR5501",
                 "PLR6",
+                "PLR61",
+                "PLR610",
+                "PLR6104",
                 "PLR62",
                 "PLR620",
                 "PLR6201",
                 "PLR63",
                 "PLR630",
                 "PLR6301",
                 "PLW",
                 "PLW0",
                 "PLW01",
                 "PLW010",
                 "PLW0108",
-                "PLW011",
-                "PLW0117",
                 "PLW012",
                 "PLW0120",
                 "PLW0127",
                 "PLW0128",
                 "PLW0129",
                 "PLW013",
                 "PLW0131",
                 "PLW0133",
+                "PLW017",
+                "PLW0177",
                 "PLW02",
+                "PLW021",
+                "PLW0211",
                 "PLW024",
                 "PLW0245",
                 "PLW04",
                 "PLW040",
                 "PLW0406",
                 "PLW06",
                 "PLW060",
                 "PLW0602",
                 "PLW0603",
                 "PLW0604",
+                "PLW064",
+                "PLW0642",
                 "PLW07",
                 "PLW071",
                 "PLW0711",
                 "PLW1",
                 "PLW15",
                 "PLW150",
                 "PLW1501",
@@ -2764,14 +2817,17 @@
                 "PYI051",
                 "PYI052",
                 "PYI053",
                 "PYI054",
                 "PYI055",
                 "PYI056",
                 "PYI058",
+                "PYI059",
+                "PYI06",
+                "PYI062",
                 "Q",
                 "Q0",
                 "Q00",
                 "Q000",
                 "Q001",
                 "Q002",
                 "Q003",
@@ -2817,17 +2873,19 @@
                 "RUF022",
                 "RUF023",
                 "RUF024",
                 "RUF025",
                 "RUF026",
                 "RUF027",
                 "RUF028",
+                "RUF029",
                 "RUF1",
                 "RUF10",
                 "RUF100",
+                "RUF101",
                 "RUF2",
                 "RUF20",
                 "RUF200",
                 "S",
                 "S1",
                 "S10",
                 "S101",
@@ -3074,14 +3132,15 @@
                 "UP036",
                 "UP037",
                 "UP038",
                 "UP039",
                 "UP04",
                 "UP040",
                 "UP041",
+                "UP042",
                 "W",
                 "W1",
                 "W19",
                 "W191",
                 "W2",
                 "W29",
                 "W291",
@@ -3114,26 +3173,26 @@
                 "YTT302",
                 "YTT303"
             ],
             "type": "string"
         },
         "SerializationFormat": {
             "enum": [
-                "azure",
+                "text",
                 "concise",
                 "full",
-                "github",
-                "gitlab",
-                "grouped",
                 "json",
                 "json-lines",
                 "junit",
+                "grouped",
+                "github",
+                "gitlab",
                 "pylint",
-                "sarif",
-                "text"
+                "azure",
+                "sarif"
             ],
             "type": "string"
         },
         "Strictness": {
             "oneOf": [
                 {
                     "description": "Ban imports that extend into the parent module or beyond.",
@@ -3175,24 +3234,24 @@
                 "array",
                 "null"
             ]
         },
         "cache-dir": {
             "description": "A path to the cache directory.\n\nBy default, Ruff stores cache results in a `.ruff_cache` directory in the current project root.\n\nHowever, Ruff will also respect the `RUFF_CACHE_DIR` environment variable, which takes precedence over that default.\n\nThis setting will override even the `RUFF_CACHE_DIR` environment variable, if set.",
             "type": [
-                "null",
-                "string"
+                "string",
+                "null"
             ]
         },
         "dummy-variable-rgx": {
             "deprecated": true,
             "description": "A regular expression used to identify \"dummy\" variables, or those which should be ignored when enforcing (e.g.) unused-variable rules. The default expression matches `_`, `__`, and `_var`, but not `_var_`.",
             "type": [
-                "null",
-                "string"
+                "string",
+                "null"
             ]
         },
         "exclude": {
             "description": "A list of file patterns to exclude from formatting and linting.\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).\n\nNote that you'll typically want to use [`extend-exclude`](#extend-exclude) to modify the excluded paths.",
             "items": {
                 "type": "string"
             },
@@ -3208,16 +3267,16 @@
                 "boolean",
                 "null"
             ]
         },
         "extend": {
             "description": "A path to a local `pyproject.toml` file to merge into this configuration. User home directory and environment variables will be expanded.\n\nTo resolve the current `pyproject.toml` file, Ruff will first resolve this base configuration file, then merge in any properties defined in the current configuration file.",
             "type": [
-                "null",
-                "string"
+                "string",
+                "null"
             ]
         },
         "extend-exclude": {
             "description": "A list of file patterns to omit from formatting and linting, in addition to those specified by `exclude`.\n\nExclusions are based on globs, and can be either:\n\n- Single-path patterns, like `.mypy_cache` (to exclude any directory named `.mypy_cache` in the tree), `foo.py` (to exclude any file named `foo.py`), or `foo_*.py` (to exclude any file matching `foo_*.py` ). - Relative patterns, like `directory/foo.py` (to exclude that specific file) or `directory/*.py` (to exclude any Python files in `directory`). Note that these paths are relative to the project root (e.g., the directory containing your `pyproject.toml`).\n\nFor more information on the glob syntax, refer to the [`globset` documentation](https://docs.rs/globset/latest/globset/#syntax).",
             "items": {
                 "type": "string"
             },
@@ -3264,16 +3323,16 @@
                     "$ref": "#/definitions/RuleSelector"
                 },
                 "type": "array"
             },
             "deprecated": true,
             "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, in addition to any rules excluded by `per-file-ignores`.",
             "type": [
-                "null",
-                "object"
+                "object",
+                "null"
             ]
         },
         "extend-safe-fixes": {
             "deprecated": true,
             "description": "A list of rule codes or prefixes for which unsafe fixes should be considered safe.",
             "items": {
                 "$ref": "#/definitions/RuleSelector"
@@ -3372,14 +3431,26 @@
                 {
                     "type": "null"
                 }
             ],
             "deprecated": true,
             "description": "Options for the `flake8-bandit` plugin."
         },
+        "flake8-boolean-trap": {
+            "anyOf": [
+                {
+                    "$ref": "#/definitions/Flake8BooleanTrapOptions"
+                },
+                {
+                    "type": "null"
+                }
+            ],
+            "deprecated": true,
+            "description": "Options for the `flake8-boolean-trap` plugin."
+        },
         "flake8-bugbear": {
             "anyOf": [
                 {
                     "$ref": "#/definitions/Flake8BugbearOptions"
                 },
                 {
                     "type": "null"
@@ -3655,15 +3726,15 @@
                     "type": "null"
                 }
             ],
             "deprecated": true,
             "description": "Options for the `mccabe` plugin."
         },
         "namespace-packages": {
-            "description": "Mark the specified directories as namespace packages. For the purpose of module resolution, Ruff will treat those directories as if they contained an `__init__.py` file.",
+            "description": "Mark the specified directories as namespace packages. For the purpose of module resolution, Ruff will treat those directories and all their subdirectories as if they contained an `__init__.py` file.",
             "items": {
                 "type": "string"
             },
             "type": [
                 "array",
                 "null"
             ]
@@ -3695,18 +3766,18 @@
             "additionalProperties": {
                 "items": {
                     "$ref": "#/definitions/RuleSelector"
                 },
                 "type": "array"
             },
             "deprecated": true,
-            "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files.",
+            "description": "A list of mappings from file pattern to rule codes or prefixes to exclude, when considering any matching files. An initial '!' negates the file pattern.",
             "type": [
-                "null",
-                "object"
+                "object",
+                "null"
             ]
         },
         "preview": {
             "description": "Whether to enable preview mode. When preview mode is enabled, Ruff will use unstable rules, fixes, and formatting.",
             "type": [
                 "boolean",
                 "null"
```

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/scikit-build.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/scikit-build.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761732987948265%*

 * *Differences: {"'$defs'": "{'inherit': OrderedDict([('enum', ['none', 'append', 'prepend']), ('default', "*

 * *            "'none')])}",*

 * * "'properties'": "{'ninja': {'properties': {'make-fallback': {'description': 'If Ninja is not "*

 * *                 'present on the system or is older than required, it will be downloaded via PyPI '*

 * *                 "if this is false.'}}}, 'wheel': {'properties': {'exclude': {'description': 'A "*

 * *                 'set of patterns to exclude from the wheel. This is additive to the SDist exclude  […]*

```diff
@@ -49,14 +49,22 @@
                 "state": {
                     "description": "The state of the build, one of `sdist`, `wheel`, `editable`, `metadata_wheel`, and `metadata_editable`. Takes a regex.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
+        "inherit": {
+            "default": "none",
+            "enum": [
+                "none",
+                "append",
+                "prepend"
+            ]
+        },
         "metadata": {
             "properties": {
                 "provider": {
                     "type": "string"
                 },
                 "provider-path": {
                     "type": "string"
@@ -360,15 +368,15 @@
             "type": "string"
         },
         "ninja": {
             "additionalProperties": false,
             "properties": {
                 "make-fallback": {
                     "default": true,
-                    "description": "If CMake is not present on the system or is older required, it will be downloaded via PyPI if possible. An empty string will disable this check.",
+                    "description": "If Ninja is not present on the system or is older than required, it will be downloaded via PyPI if this is false.",
                     "type": "boolean"
                 },
                 "minimum-version": {
                     "deprecated": true,
                     "description": "DEPRECATED in 0.8; use version instead.",
                     "type": "string"
                 },
@@ -419,14 +427,71 @@
                                 "required": [
                                     "any"
                                 ],
                                 "type": "object"
                             }
                         ]
                     },
+                    "inherit": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "cmake": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "args": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "define": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "targets": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "install": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "components": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "sdist": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "exclude": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "include": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            },
+                            "wheel": {
+                                "additionalProperties": false,
+                                "properties": {
+                                    "exclude": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "license-files": {
+                                        "$ref": "#/$defs/inherit"
+                                    },
+                                    "packages": {
+                                        "$ref": "#/$defs/inherit"
+                                    }
+                                },
+                                "type": "object"
+                            }
+                        },
+                        "type": "object"
+                    },
                     "install": {
                         "$ref": "#/properties/install"
                     },
                     "logging": {
                         "$ref": "#/properties/logging"
                     },
                     "metadata": {
@@ -500,15 +565,15 @@
                 },
                 "cmake": {
                     "default": true,
                     "description": "If set to True (the default), CMake will be run before building the wheel.",
                     "type": "boolean"
                 },
                 "exclude": {
-                    "description": "A set of patterns to exclude from the wheel. This is additive to the SDist exclude patterns. This applies to the source files, not the final paths. Editable installs may not respect this exclusion.",
+                    "description": "A set of patterns to exclude from the wheel. This is additive to the SDist exclude patterns. This applies to the final paths in the wheel, and can exclude files from CMake output as well.  Editable installs may not respect this exclusion.",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "expand-macos-universal-tags": {
                     "default": false,
```

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/setuptools.schema.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/setuptools.schema.json`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/src/validate_pyproject_schema_store/resources/tool.json` & `validate_pyproject_schema_store-2024.5.13/src/validate_pyproject_schema_store/resources/tool.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {"'uv'": "'https://json.schemastore.org/uv.json'"}*

```diff
@@ -4,9 +4,10 @@
     "hatch": "https://json.schemastore.org/hatch.json",
     "mypy": "https://json.schemastore.org/partial-mypy.json",
     "pdm": "https://json.schemastore.org/partial-pdm.json",
     "poetry": "https://json.schemastore.org/partial-poetry.json",
     "pyright": "https://json.schemastore.org/partial-pyright.json",
     "ruff": "https://json.schemastore.org/ruff.json",
     "scikit-build": "https://json.schemastore.org/partial-scikit-build.json",
-    "setuptools": "https://json.schemastore.org/partial-setuptools.json"
+    "setuptools": "https://json.schemastore.org/partial-setuptools.json",
+    "uv": "https://json.schemastore.org/uv.json"
 }
```

### Comparing `validate_pyproject_schema_store-2024.4.8/tests/test_package.py` & `validate_pyproject_schema_store-2024.5.13/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/tools/sync.py` & `validate_pyproject_schema_store-2024.5.13/tools/sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# /// pyproject
-# run.dependencies = [ "aiohttp", "tomlkit" ]
+#!/usr/bin/env python3
+# /// script
+# requires-python = ">=3.11"
+# dependencies = [ "aiohttp", "tomlkit" ]
 # ///
 
 
 from __future__ import annotations
 
 import asyncio
 import datetime
```

### Comparing `validate_pyproject_schema_store-2024.4.8/.gitignore` & `validate_pyproject_schema_store-2024.5.13/.gitignore`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/LICENSE` & `validate_pyproject_schema_store-2024.5.13/LICENSE`

 * *Files identical despite different names*

### Comparing `validate_pyproject_schema_store-2024.4.8/README.md` & `validate_pyproject_schema_store-2024.5.13/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,19 +51,18 @@
 ```
 
 This also has the benefit that the version will be pinned and updated by
 pre-commit automatically.
 
 ## Developing
 
-This project uses `hatch`. You can run the sync script on Python 3.11+ by
-running:
+This project uses `hatch>=1.10`. You can run the sync script by running:
 
 ```bash
-hatch run sync
+hatch run tools/sync.py
 ```
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/henryiii/validate-pyproject-schema-store/workflows/CI/badge.svg
 [actions-link]:             https://github.com/henryiii/validate-pyproject-schema-store/actions
 [pypi-link]:                https://pypi.org/project/validate-pyproject-schema-store/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/validate-pyproject-schema-store
```

### Comparing `validate_pyproject_schema_store-2024.4.8/pyproject.toml` & `validate_pyproject_schema_store-2024.5.13/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "validate-pyproject-schema-store"
-version = "2024.04.08"
+version = "2024.05.13"
 authors = [
   { name = "Henry Schreiner", email = "henryfs@princeton.edu" },
 ]
 description = "A plugin set for validate-pyproject and schema-store."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -33,27 +33,28 @@
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
   "pytest-cov >=3",
   "validate-pyproject>=0.16",
+  "tomli; python_version<'3.11'",
 ]
 docs = [
   "sphinx>=7.0",
   "myst_parser>=0.13",
   "sphinx_copybutton",
   "sphinx_autodoc_typehints",
   "furo>=2023.08.17",
 ]
 validate-pyproject = [
-  "validate-pyproject>=0.16",
+  "validate-pyproject",
 ]
 all = [
-  "validate-pyproject[all]>=0.16",
+  "validate-pyproject[all]",
 ]
 
 [project.urls]
 Homepage = "https://github.com/henryiii/validate-pyproject-schema-store"
 "Bug Tracker" = "https://github.com/henryiii/validate-pyproject-schema-store/issues"
 Discussions = "https://github.com/henryiii/validate-pyproject-schema-store/discussions"
 Changelog = "https://github.com/henryiii/validate-pyproject-schema-store/releases"
@@ -64,40 +65,32 @@
 mypy = "validate_pyproject_schema_store.schema:get_schema"
 ruff = "validate_pyproject_schema_store.schema:get_schema"
 hatch = "validate_pyproject_schema_store.schema:get_schema"
 scikit-build = "validate_pyproject_schema_store.schema:get_schema"
 poetry = "validate_pyproject_schema_store.schema:get_schema"
 pdm = "validate_pyproject_schema_store.schema:get_schema"
 pyright = "validate_pyproject_schema_store.schema:get_schema"
+uv = "validate_pyproject_schema_store.schema:get_schema"
 
 [project.entry-points."pipx.run"]
 validate-pyproject-schema-store = "validate_pyproject.cli:main"
 
 [tool.hatch.envs.default]
-path = ".venv"
+installer = "uv"
+
+[tool.hatch.envs.hatch-test]
 features = ["test"]
-dependencies = ["aiohttp", "tomlkit"]
-scripts.test = "pytest {args}"
-scripts.sync = "python tools/sync.py {args}"
-
-[tool.hatch.envs.docs]
-features = ["docs"]
-dependencies = ["sphinx-autobuild"]
-scripts.linkcheck = "sphinx-build -b linkcheck docs docs/_build/linkcheck {args}"
-scripts.build = "sphinx-build --keep-going -n -T -b=html docs docs/_build/html {args}"
-scripts.serve = "sphinx-autobuild -n -T -b=html docs docs/_build/html {args}"
-scripts.build-api-docs = "sphinx-apidoc -o docs/api/ --module-first --no-toc --force src/validate_pyproject_schema_store {args}"
 
 [tool.hatch.envs.lint]
-requirements = ["pre-commit"]
+dependencies = ["pre-commit"]
 skip-install = true
 scripts.lint = "pre-commit run --all-files --show-diff-on-failures {args}"
 
 [tool.hatch.envs.pylint]
-requirements = ["pylint"]
+dependencies = ["pylint"]
 scripts.lint = "pylint validate_pyproject_schema_store {args}"
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
```

### Comparing `validate_pyproject_schema_store-2024.4.8/PKG-INFO` & `validate_pyproject_schema_store-2024.5.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: validate-pyproject-schema-store
-Version: 2024.4.8
+Version: 2024.5.13
 Summary: A plugin set for validate-pyproject and schema-store.
 Project-URL: Homepage, https://github.com/henryiii/validate-pyproject-schema-store
 Project-URL: Bug Tracker, https://github.com/henryiii/validate-pyproject-schema-store/issues
 Project-URL: Discussions, https://github.com/henryiii/validate-pyproject-schema-store/discussions
 Project-URL: Changelog, https://github.com/henryiii/validate-pyproject-schema-store/releases
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
@@ -21,27 +21,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources; python_version < '3.9'
 Provides-Extra: all
-Requires-Dist: validate-pyproject[all]>=0.16; extra == 'all'
+Requires-Dist: validate-pyproject[all]; extra == 'all'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
+Requires-Dist: tomli; (python_version < '3.11') and extra == 'test'
 Requires-Dist: validate-pyproject>=0.16; extra == 'test'
 Provides-Extra: validate-pyproject
-Requires-Dist: validate-pyproject>=0.16; extra == 'validate-pyproject'
+Requires-Dist: validate-pyproject; extra == 'validate-pyproject'
 Description-Content-Type: text/markdown
 
 # validate-pyproject-schema-store
 
 [![Actions Status][actions-badge]][actions-link]
 
 [![PyPI version][pypi-version]][pypi-link]
@@ -93,19 +94,18 @@
 ```
 
 This also has the benefit that the version will be pinned and updated by
 pre-commit automatically.
 
 ## Developing
 
-This project uses `hatch`. You can run the sync script on Python 3.11+ by
-running:
+This project uses `hatch>=1.10`. You can run the sync script by running:
 
 ```bash
-hatch run sync
+hatch run tools/sync.py
 ```
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/henryiii/validate-pyproject-schema-store/workflows/CI/badge.svg
 [actions-link]:             https://github.com/henryiii/validate-pyproject-schema-store/actions
 [pypi-link]:                https://pypi.org/project/validate-pyproject-schema-store/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/validate-pyproject-schema-store
```

