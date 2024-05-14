# Comparing `tmp/wild_code-0.4.3.tar.gz` & `tmp/wild_code-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_code-0.4.3.tar", last modified: Sun May 12 22:22:37 2024, max compression
+gzip compressed data, was "wild_code-0.4.4.tar", last modified: Tue May 14 20:08:52 2024, max compression
```

## Comparing `wild_code-0.4.3.tar` & `wild_code-0.4.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:59.203994 wild_code-0.4.3/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-12 22:19:33.000000 wild_code-0.4.3/.dockerignore
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.216561 wild_code-0.4.3/.github/
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.216113 wild_code-0.4.3/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_contract.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_test.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-12 22:19:33.000000 wild_code-0.4.3/.github/ISSUE_TEMPLATE/model_eval_request.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-12 22:19:33.000000 wild_code-0.4.3/.gitignore
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-12 22:19:33.000000 wild_code-0.4.3/.pre-commit-config.yaml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-12 22:19:33.000000 wild_code-0.4.3/CITATION.cff
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      757 2024-05-12 22:19:33.000000 wild_code-0.4.3/Dockerfile
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-12 22:19:33.000000 wild_code-0.4.3/LICENSE
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-12 22:19:33.000000 wild_code-0.4.3/MANIFEST.in
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10938 2024-05-12 22:19:59.196091 wild_code-0.4.3/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9825 2024-05-12 22:19:33.000000 wild_code-0.4.3/README.md
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-12 22:19:33.000000 wild_code-0.4.3/pyproject.toml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-12 22:19:33.000000 wild_code-0.4.3/release.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      156 2024-05-12 22:19:33.000000 wild_code-0.4.3/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1348 2024-05-12 22:19:33.000000 wild_code-0.4.3/run.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-12 22:19:59.220794 wild_code-0.4.3/setup.cfg
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.221269 wild_code-0.4.3/tests/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-12 22:19:33.000000 wild_code-0.4.3/tests/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-12 22:19:33.000000 wild_code-0.4.3/tests/test_legacy_sanitizer.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-12 22:19:33.000000 wild_code-0.4.3/tests/test_treesitter_sanitizer.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:59.169551 wild_code-0.4.3/wild_code.egg-info/
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10938 2024-05-12 22:19:57.000000 wild_code-0.4.3/wild_code.egg-info/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/SOURCES.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/dependency_links.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/entry_points.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/requires.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-12 22:19:58.000000 wild_code-0.4.3/wild_code.egg-info/top_level.txt
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.255855 wild_code-0.4.3/wildcode/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-12 22:19:57.000000 wild_code-0.4.3/wildcode/_version.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.244229 wild_code-0.4.3/wildcode/data/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/data/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/data/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/data/wildcodebench.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.250298 wild_code-0.4.3/wildcode/eval/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7214 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/eval/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/eval/_special_oracle.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5715 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/eval/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8279 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/evaluate.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.267472 wild_code-0.4.3/wildcode/gen/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/__init__.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 22:19:58.266954 wild_code-0.4.3/wildcode/gen/util/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2159 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/util/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/util/anthropic_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/gen/util/openai_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5558 2024-05-12 22:19:33.000000 wild_code-0.4.3/wildcode/generate.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/inspect.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/lecacy_sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/model.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-12 22:19:34.000000 wild_code-0.4.3/wildcode/syncheck.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:12.539648 wild_code-0.4.4/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-14 19:57:47.000000 wild_code-0.4.4/.dockerignore
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.730029 wild_code-0.4.4/.github/
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.729630 wild_code-0.4.4/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_contract.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_test.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-14 19:57:47.000000 wild_code-0.4.4/.github/ISSUE_TEMPLATE/model_eval_request.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-14 19:57:47.000000 wild_code-0.4.4/.gitignore
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-14 19:57:47.000000 wild_code-0.4.4/.pre-commit-config.yaml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-14 19:57:47.000000 wild_code-0.4.4/CITATION.cff
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      757 2024-05-14 19:57:47.000000 wild_code-0.4.4/Dockerfile
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-14 19:57:47.000000 wild_code-0.4.4/LICENSE
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-14 19:57:47.000000 wild_code-0.4.4/MANIFEST.in
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10932 2024-05-14 20:06:12.534059 wild_code-0.4.4/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9819 2024-05-14 19:57:47.000000 wild_code-0.4.4/README.md
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-14 19:57:47.000000 wild_code-0.4.4/pyproject.toml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-14 20:05:59.000000 wild_code-0.4.4/release.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      156 2024-05-14 19:57:47.000000 wild_code-0.4.4/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1348 2024-05-14 19:57:47.000000 wild_code-0.4.4/run.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-14 20:06:12.551049 wild_code-0.4.4/setup.cfg
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.735305 wild_code-0.4.4/tests/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-14 19:57:47.000000 wild_code-0.4.4/tests/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-14 19:57:47.000000 wild_code-0.4.4/tests/test_legacy_sanitizer.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-14 19:57:47.000000 wild_code-0.4.4/tests/test_treesitter_sanitizer.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:12.516879 wild_code-0.4.4/wild_code.egg-info/
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10932 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/entry_points.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/requires.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-14 20:06:11.000000 wild_code-0.4.4/wild_code.egg-info/top_level.txt
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.772721 wild_code-0.4.4/wildcode/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-14 20:06:11.000000 wild_code-0.4.4/wildcode/_version.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.757082 wild_code-0.4.4/wildcode/data/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/data/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/data/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/data/wildcodebench.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.764430 wild_code-0.4.4/wildcode/eval/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7216 2024-05-14 19:58:38.000000 wild_code-0.4.4/wildcode/eval/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/eval/_special_oracle.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7110 2024-05-14 19:59:36.000000 wild_code-0.4.4/wildcode/eval/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8190 2024-05-14 20:01:25.000000 wild_code-0.4.4/wildcode/evaluate.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.782491 wild_code-0.4.4/wildcode/gen/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/gen/__init__.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-14 20:06:11.781970 wild_code-0.4.4/wildcode/gen/util/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2202 2024-05-14 20:00:46.000000 wild_code-0.4.4/wildcode/gen/util/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/gen/util/anthropic_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/gen/util/openai_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5558 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/generate.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/inspect.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/lecacy_sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/model.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-14 19:57:47.000000 wild_code-0.4.4/wildcode/syncheck.py
```

### Comparing `wild_code-0.4.3/.dockerignore` & `wild_code-0.4.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_contract.yml` & `wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_contract.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/.github/ISSUE_TEMPLATE/buggy_test.yml` & `wild_code-0.4.4/.github/ISSUE_TEMPLATE/buggy_test.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/.github/ISSUE_TEMPLATE/model_eval_request.yml` & `wild_code-0.4.4/.github/ISSUE_TEMPLATE/model_eval_request.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/.gitignore` & `wild_code-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/Dockerfile` & `wild_code-0.4.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/LICENSE` & `wild_code-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/PKG-INFO` & `wild_code-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.3
+Version: 0.4.4
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -187,15 +187,15 @@
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
 # mount the current directory to the container
-docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl --check-gt-only
+docker run -v $(pwd):/wildcode terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
 # ...Or locally ⚠️
 wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.3 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.4 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -89,19 +89,19 @@
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```shell # mount the current
-directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
-dataset wildcodebench --samples samples.jsonl --check-gt-only # ...Or locally
-â ï¸ wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ```
-...Or if you want to try it locally regardless of the risks â ï¸: First,
-install the dependencies for WildCodeBench: ```shell pip install -r https://
+directory to the container docker run -v $(pwd):/wildcode terryzho/wildcode:
+latest --dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
+you want to try it locally regardless of the risks â ï¸: First, install the
+dependencies for WildCodeBench: ```shell pip install -r https://
 raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
 requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
 dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
 very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
 OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
 solution's runtime. > > Additionally, you are **NOT** encouraged to make your
 test-bed over stressed while running evaluation. > For example, using `--
```

### Comparing `wild_code-0.4.3/README.md` & `wild_code-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
 # mount the current directory to the container
-docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl --check-gt-only
+docker run -v $(pwd):/wildcode terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
 # ...Or locally ⚠️
 wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
```

#### html2text {}

```diff
@@ -74,19 +74,19 @@
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```shell # mount the current
-directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
-dataset wildcodebench --samples samples.jsonl --check-gt-only # ...Or locally
-â ï¸ wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ```
-...Or if you want to try it locally regardless of the risks â ï¸: First,
-install the dependencies for WildCodeBench: ```shell pip install -r https://
+directory to the container docker run -v $(pwd):/wildcode terryzho/wildcode:
+latest --dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
+you want to try it locally regardless of the risks â ï¸: First, install the
+dependencies for WildCodeBench: ```shell pip install -r https://
 raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
 requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
 dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
 very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
 OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
 solution's runtime. > > Additionally, you are **NOT** encouraged to make your
 test-bed over stressed while running evaluation. > For example, using `--
```

### Comparing `wild_code-0.4.3/release.sh` & `wild_code-0.4.4/release.sh`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/run.sh` & `wild_code-0.4.4/run.sh`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/setup.cfg` & `wild_code-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/tests/test_legacy_sanitizer.py` & `wild_code-0.4.4/tests/test_legacy_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/tests/test_treesitter_sanitizer.py` & `wild_code-0.4.4/tests/test_treesitter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wild_code.egg-info/PKG-INFO` & `wild_code-0.4.4/wild_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.4.3
+Version: 0.4.4
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -187,15 +187,15 @@
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
 # mount the current directory to the container
-docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl --check-gt-only
+docker run -v $(pwd):/wildcode terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
 # ...Or locally ⚠️
 wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.4.3 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.4 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -89,19 +89,19 @@
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```shell # mount the current
-directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
-dataset wildcodebench --samples samples.jsonl --check-gt-only # ...Or locally
-â ï¸ wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ```
-...Or if you want to try it locally regardless of the risks â ï¸: First,
-install the dependencies for WildCodeBench: ```shell pip install -r https://
+directory to the container docker run -v $(pwd):/wildcode terryzho/wildcode:
+latest --dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
+you want to try it locally regardless of the risks â ï¸: First, install the
+dependencies for WildCodeBench: ```shell pip install -r https://
 raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
 requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
 dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
 very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
 OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
 solution's runtime. > > Additionally, you are **NOT** encouraged to make your
 test-bed over stressed while running evaluation. > For example, using `--
```

### Comparing `wild_code-0.4.3/wild_code.egg-info/SOURCES.txt` & `wild_code-0.4.4/wild_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/data/utils.py` & `wild_code-0.4.4/wildcode/data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/data/wildcodebench.py` & `wild_code-0.4.4/wildcode/data/wildcodebench.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/eval/__init__.py` & `wild_code-0.4.4/wildcode/eval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,16 @@
         import shutil
         import builtins
         
         rmtree = shutil.rmtree
         rmdir = os.rmdir
         chdir = os.chdir
         # Disable functionalities that can make destructive changes to the test.
-        # allow only 32GB memory usage
-        maximum_memory_bytes = 32 * 1024 * 1024 * 1024
+        # allow only 128GB memory usage
+        maximum_memory_bytes = 128 * 1024 * 1024 * 1024
         reliability_guard(maximum_memory_bytes=maximum_memory_bytes)
         module_name = "__test__"
         new_module = types.ModuleType(module_name)
         # Set necessary attributes for the module
         new_module.__dict__.update({
             '__builtins__': builtins,
             '__file__': f"{module_name}.py",
```

### Comparing `wild_code-0.4.3/wildcode/eval/utils.py` & `wild_code-0.4.4/wildcode/eval/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -105,14 +105,51 @@
         yield
     except BaseException as exc:
         raise exc
     finally:
         os.chdir(cwd)
 
 
+@contextlib.contextmanager
+def safe_environment():
+    # Save original functions
+    original_kill = os.kill
+    original_subprocess_call = subprocess.call
+    original_check_output = subprocess.check_output
+
+    def safe_kill(pid, sig):
+        print(f"Prevented attempt to kill PID {pid} with signal {sig}")
+        # Prevent killing any process, or you can add your logic to allow killing non-critical processes
+
+    def safe_subprocess_call(command, *args, **kwargs):
+        print(f"Intercepted subprocess call: {command}")
+        if 'killall' in command:
+            return 0  # Simulate successful execution without doing anything
+        return original_subprocess_call(command, *args, **kwargs)
+
+    def safe_check_output(command, *args, **kwargs):
+        print(f"Intercepted command: {command}")
+        if 'ps' in command:
+            return b""  # Simulate no processes found
+        return original_check_output(command, *args, **kwargs)
+
+    # Override the risky functions with the safe versions
+    os.kill = safe_kill
+    subprocess.call = safe_subprocess_call
+    subprocess.check_output = safe_check_output
+
+    try:
+        yield
+    finally:
+        # Restore original functions after the block
+        os.kill = original_kill
+        subprocess.call = original_subprocess_call
+        subprocess.check_output = original_check_output
+
+
 class TimeoutException(Exception):
     pass
 
 
 class WriteOnlyStringIO(io.StringIO):
     """StringIO that throws an exception when it's read from"""
```

### Comparing `wild_code-0.4.3/wildcode/evaluate.py` & `wild_code-0.4.4/wildcode/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,19 +146,17 @@
                 )
                 remainings.add(sample["_identifier"])
                 args = (
                     flags.dataset,
                     completion_id[task_id],
                     problems[task_id],
                     solution,
-                    # problems[task_id]["canonical_solution"],
                     sample["_identifier"],
                     flags.min_time_limit,
-                    # expected_time[task_id],
-                    120
+                    expected_time[task_id],
                 )
                 futures.append(executor.submit(check_correctness, *args))
                 completion_id[task_id] += 1
                 n_samples += 1
 
             assert n_samples == len(remainings), "Missing problems in unfinished"
             assert len(completion_id) == len(problems), "Missing problems in samples"
```

### Comparing `wild_code-0.4.3/wildcode/gen/__init__.py` & `wild_code-0.4.4/wildcode/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/gen/util/__init__.py` & `wild_code-0.4.4/wildcode/gen/util/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from copy import deepcopy
 
 from wildcode.eval.utils import (
     create_tempdir,
     reliability_guard,
     swallow_io,
     time_limit,
+    safe_environment,
 )
 def trusted_exec(code, test_code, task_id):
     """Execute trusted code in place."""
     
     with create_tempdir():
         import os
         import shutil
         import builtins
         
         rmtree = shutil.rmtree
         rmdir = os.rmdir
         chdir = os.chdir
         module_name = "__test__"
         new_module = types.ModuleType(module_name)
-        maximum_memory_bytes = 32 * 1024 * 1024 * 1024
+        maximum_memory_bytes = 128 * 1024 * 1024 * 1024
         reliability_guard(maximum_memory_bytes=maximum_memory_bytes)
         # Set necessary attributes for the module
         new_module.__dict__.update({
             '__builtins__': builtins,
             '__file__': f"{module_name}.py",
             '__package__': None,
             '__doc__': None,
@@ -46,15 +47,15 @@
         exec(compile(full_code, f"{module_name}.py", 'exec'), new_module.__dict__)
         sys.modules[module_name] = new_module
         TestCases = getattr(new_module, 'TestCases')
         loader = unittest.TestLoader()
         suite = loader.loadTestsFromTestCase(TestCases)
         test_result = unittest.TestResult()
         start = time.time()
-        with swallow_io():
+        with safe_environment(), swallow_io():
             suite.run(test_result)
         for test, trace in test_result.failures + test_result.errors:
             print(trace)
         # Needed for cleaning up.
         shutil.rmtree = rmtree
         os.rmdir = rmdir
         os.chdir = chdir
```

### Comparing `wild_code-0.4.3/wildcode/gen/util/anthropic_request.py` & `wild_code-0.4.4/wildcode/gen/util/anthropic_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/gen/util/openai_request.py` & `wild_code-0.4.4/wildcode/gen/util/openai_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/generate.py` & `wild_code-0.4.4/wildcode/generate.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/inspect.py` & `wild_code-0.4.4/wildcode/inspect.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/lecacy_sanitize.py` & `wild_code-0.4.4/wildcode/lecacy_sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/model.py` & `wild_code-0.4.4/wildcode/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     prompt = f"""\
 Please provide a self-contained Python script that solves the following problem in a markdown code block:
 ```
 {prompt.strip()}
 ```
 """
     response = f"""\
-Below is a Python script with a self-contained function that solves the problem and passes correpsonding tests:
+Below is a Python script with a self-contained function that solves the problem and passes corresponding tests:
 ```python
 {_MAGIC_SPLITTER_}
 ```
 """
     prompt = tokenizer.apply_chat_template(
         [
             {"role": "user", "content": prompt},
```

### Comparing `wild_code-0.4.3/wildcode/sanitize.py` & `wild_code-0.4.4/wildcode/sanitize.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.4.3/wildcode/syncheck.py` & `wild_code-0.4.4/wildcode/syncheck.py`

 * *Files identical despite different names*

