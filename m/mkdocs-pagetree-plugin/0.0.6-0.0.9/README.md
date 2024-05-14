# Comparing `tmp/mkdocs-pagetree-plugin-0.0.6.tar.gz` & `tmp/mkdocs-pagetree-plugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-pagetree-plugin-0.0.6.tar", last modified: Sun Nov 26 20:32:37 2023, max compression
+gzip compressed data, was "mkdocs-pagetree-plugin-0.0.9.tar", last modified: Wed Dec 13 18:50:26 2023, max compression
```

## Comparing `mkdocs-pagetree-plugin-0.0.6.tar` & `mkdocs-pagetree-plugin-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.941363 mkdocs-pagetree-plugin-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.937363 mkdocs-pagetree-plugin-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.937363 mkdocs-pagetree-plugin-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2023-11-26 20:32:37.941363 mkdocs-pagetree-plugin-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.937363 mkdocs-pagetree-plugin-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.937363 mkdocs-pagetree-plugin-0.0.6/docs/section_1/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/docs/section_1/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/docs/section_1/subpage_1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.937363 mkdocs-pagetree-plugin-0.0.6/docs/section_1/subsection_1/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/docs/section_1/subsection_1/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.937363 mkdocs-pagetree-plugin-0.0.6/docs/section_2/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/docs/section_2/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/docs/section_2/pagetree.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/docs/toplevelpage.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.937363 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.941363 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/js/mkdocs_pagetree_plugin.js
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.941363 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/templates/nav_item.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/templates/nav_sub.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/templates/pagetree.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:32:37.941363 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2023-11-26 20:32:37.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-11-26 20:32:37.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 20:32:37.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-26 20:32:37.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-26 20:32:37.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-26 20:32:37.000000 mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-11-26 20:32:23.000000 mkdocs-pagetree-plugin-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 20:32:37.941363 mkdocs-pagetree-plugin-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.555400 mkdocs-pagetree-plugin-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.547400 mkdocs-pagetree-plugin-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.551400 mkdocs-pagetree-plugin-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.551400 mkdocs-pagetree-plugin-0.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-13 18:50:26.555400 mkdocs-pagetree-plugin-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.551400 mkdocs-pagetree-plugin-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.551400 mkdocs-pagetree-plugin-0.0.9/docs/section_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/docs/section_1/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/docs/section_1/subpage_1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.551400 mkdocs-pagetree-plugin-0.0.9/docs/section_1/subsection_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/docs/section_1/subsection_1/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.551400 mkdocs-pagetree-plugin-0.0.9/docs/section_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/docs/section_2/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/docs/section_2/pagetree.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/docs/toplevelpage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.551400 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.555400 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/js/mkdocs_pagetree_plugin.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.555400 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/templates/nav_item.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/templates/nav_sub.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/templates/pagetree.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 18:50:26.555400 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-13 18:50:26.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-12-13 18:50:26.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 18:50:26.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-13 18:50:26.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-13 18:50:26.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 18:50:26.000000 mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-13 18:50:05.000000 mkdocs-pagetree-plugin-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 18:50:26.555400 mkdocs-pagetree-plugin-0.0.9/setup.cfg
```

### Comparing `mkdocs-pagetree-plugin-0.0.6/.github/workflows/deploy.yml` & `mkdocs-pagetree-plugin-0.0.9/.github/workflows/deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Thomas Breitner
+#
+# SPDX-License-Identifier: CC0-1.0
+
 name: Deploy Python Package
 
 on:
   release:
     types: [published]
 
 permissions:
@@ -20,19 +24,24 @@
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.11'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools wheel
-        python -m pip install --upgrade build twine
+    - name: Trigger a test build
+      run: |
+        python -m pip install .
+        mkdocs build --clean --verbose
+    - name: Deploy to github pages
+      run: |
+        python -m pip install .
+        mkdocs gh-deploy --force --clean --verbose
     - name: Build package
-      run: python -m build
+      run: |
+        python -m pip install --upgrade build twine
+        python -m build
     - name: Publish package to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
-    - name: Deploy to github pages
-      run: |
-        python -m pip install .
-        mkdocs gh-deploy --force --verbose
```

### Comparing `mkdocs-pagetree-plugin-0.0.6/LICENSE` & `mkdocs-pagetree-plugin-0.0.9/LICENSES/MIT.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 MIT License
 
-Copyright (c) 2023 Thomas Breitner
+Copyright (c) <year> <copyright holders>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mkdocs-pagetree-plugin-0.0.6/PKG-INFO` & `mkdocs-pagetree-plugin-0.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 Metadata-Version: 2.1
 Name: mkdocs-pagetree-plugin
-Version: 0.0.6
+Version: 0.0.9
 Summary: MkDocs plugin that allows you to display the page tree
 Author-email: Thomas Breitner <mail@thms.de>
-License: MIT License
-        
-        Copyright (c) 2023 Thomas Breitner
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+License: MIT
 Project-URL: Homepage, https://tombreit.github.io/mkdocs-pagetree-plugin/
 Project-URL: Documentation, https://github.com/tombreit/mkdocs-pagetree-plugin/blob/main/README.md
 Project-URL: Repository, https://github.com/tombreit/mkdocs-pagetree-plugin
 Project-URL: Issues, https://github.com/tombreit/mkdocs-pagetree-plugin/issues
 Classifier: Framework :: MkDocs
 Classifier: Topic :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSES/CC0-1.0.txt
+License-File: LICENSES/MIT.txt
 Requires-Dist: mkdocs>=1.5
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: reuse; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+
+<!--
+SPDX-FileCopyrightText: 2023 Thomas Breitner
+
+SPDX-License-Identifier: MIT
+-->
 
 # mkdocs-pagetree-plugin
 
 MkDocs plugin that allows you to display the page tree. Like `sitemap.xml`, but for humans.
 
+[![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-pagetree-plugin?color=rgb(17%2C%20148%2C%20223)&link=https%3A%2F%2Fpypi.org%2Fproject%2Fmkdocs-pagetree-plugin%2F)](https://pypi.org/project/mkdocs-pagetree-plugin/)
+[![REUSE status](https://api.reuse.software/badge/github.com/tombreit/mkdocs-pagetree-plugin)](https://api.reuse.software/info/github.com/tombreit/mkdocs-pagetree-plugin)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+![pre-commit enabled](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+
 ## Setup
 
 Install the plugin [PyPI package](https://pypi.org/project/mkdocs-pagetree-plugin/):
 
 ```bash
 pip install mkdocs-pagetree-plugin
 ```
@@ -54,14 +49,15 @@
 Configure `mkdocs.yml`:
 
 ```yaml
 plugins:
   - pagetree
 ```
 
-## Demo
-
-https://tombreit.github.io/mkdocs-pagetree-plugin/
-
 ## Usage
 
 Use `{{ pagetree }}` in your Markdown page(s) where the page tree should be rendered.
+
+## Demo & Docs
+
+https://tombreit.github.io/mkdocs-pagetree-plugin/
+
```

### Comparing `mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/js/mkdocs_pagetree_plugin.js` & `mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/js/mkdocs_pagetree_plugin.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,11 @@
+// SPDX-FileCopyrightText: 2023 Thomas Breitner
+//
+// SPDX-License-Identifier: MIT
+
 document.addEventListener("DOMContentLoaded", function(event) {
     console.log("Hi, I'm mkdocs-pagetree-plugin.");
 
     // Plugin CSS
     const style = document.createElement('style');
     style.appendChild(document.createTextNode(`
     /* Reset some default MkDocs styles */
```

### Comparing `mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/plugin.py` & `mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Thomas Breitner
+#
+# SPDX-License-Identifier: MIT
+
 """
 MkDocs Pagetree Plugin
 """
 
 from pathlib import Path
 from jinja2 import PackageLoader
 from mkdocs.plugins import BasePlugin, get_plugin_logger
@@ -9,15 +13,14 @@
 from mkdocs.commands.build import get_context
 
 
 log = get_plugin_logger(__name__)
 
 
 class PagetreePlugin(BasePlugin):
-
     def render_pagetree(self, pagetree, config, page):
         env = config.theme.get_env()
         env.loader = PackageLoader("mkdocs_pagetree_plugin")
         template = env.get_template("pagetree.html.j2")
         context = get_context(None, None, config, page=page, base_url="/")
         context["pagetree"] = pagetree
         return template.render(context)
```

### Comparing `mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin/templates/pagetree.html.j2` & `mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin/templates/pagetree.html.j2`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+<!--
+SPDX-FileCopyrightText: 2023 Thomas Breitner
+
+SPDX-License-Identifier: MIT
+-->
+
 {%- if pagetree|length>1 %}
 <div class="pagetree-container">
     <ul class="pagetree">
     {%- for nav_item in pagetree %}
     {%- if nav_item.children %}
         <li>
         <details open>
```

### Comparing `mkdocs-pagetree-plugin-0.0.6/mkdocs_pagetree_plugin.egg-info/PKG-INFO` & `mkdocs-pagetree-plugin-0.0.9/mkdocs_pagetree_plugin.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 Metadata-Version: 2.1
 Name: mkdocs-pagetree-plugin
-Version: 0.0.6
+Version: 0.0.9
 Summary: MkDocs plugin that allows you to display the page tree
 Author-email: Thomas Breitner <mail@thms.de>
-License: MIT License
-        
-        Copyright (c) 2023 Thomas Breitner
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+License: MIT
 Project-URL: Homepage, https://tombreit.github.io/mkdocs-pagetree-plugin/
 Project-URL: Documentation, https://github.com/tombreit/mkdocs-pagetree-plugin/blob/main/README.md
 Project-URL: Repository, https://github.com/tombreit/mkdocs-pagetree-plugin
 Project-URL: Issues, https://github.com/tombreit/mkdocs-pagetree-plugin/issues
 Classifier: Framework :: MkDocs
 Classifier: Topic :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSES/CC0-1.0.txt
+License-File: LICENSES/MIT.txt
 Requires-Dist: mkdocs>=1.5
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: reuse; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+
+<!--
+SPDX-FileCopyrightText: 2023 Thomas Breitner
+
+SPDX-License-Identifier: MIT
+-->
 
 # mkdocs-pagetree-plugin
 
 MkDocs plugin that allows you to display the page tree. Like `sitemap.xml`, but for humans.
 
+[![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-pagetree-plugin?color=rgb(17%2C%20148%2C%20223)&link=https%3A%2F%2Fpypi.org%2Fproject%2Fmkdocs-pagetree-plugin%2F)](https://pypi.org/project/mkdocs-pagetree-plugin/)
+[![REUSE status](https://api.reuse.software/badge/github.com/tombreit/mkdocs-pagetree-plugin)](https://api.reuse.software/info/github.com/tombreit/mkdocs-pagetree-plugin)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+![pre-commit enabled](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)
+
 ## Setup
 
 Install the plugin [PyPI package](https://pypi.org/project/mkdocs-pagetree-plugin/):
 
 ```bash
 pip install mkdocs-pagetree-plugin
 ```
@@ -54,14 +49,15 @@
 Configure `mkdocs.yml`:
 
 ```yaml
 plugins:
   - pagetree
 ```
 
-## Demo
-
-https://tombreit.github.io/mkdocs-pagetree-plugin/
-
 ## Usage
 
 Use `{{ pagetree }}` in your Markdown page(s) where the page tree should be rendered.
+
+## Demo & Docs
+
+https://tombreit.github.io/mkdocs-pagetree-plugin/
+
```

