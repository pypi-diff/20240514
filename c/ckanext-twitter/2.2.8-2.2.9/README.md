# Comparing `tmp/ckanext-twitter-2.2.8.tar.gz` & `tmp/ckanext_twitter-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-twitter-2.2.8.tar", last modified: Mon Jul 17 08:22:54 2023, max compression
+gzip compressed data, was "ckanext_twitter-2.2.9.tar", last modified: Tue May 14 10:47:08 2024, max compression
```

## Comparing `ckanext-twitter-2.2.8.tar` & `ckanext_twitter-2.2.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/cache_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/config_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/lib/twitter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/routes/tweet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/ajax_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/package/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/package/base.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/package/read_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:22:54.000000 ckanext-twitter-2.2.8/ckanext_twitter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.970515 ckanext-twitter-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:22:54.974515 ckanext-twitter-2.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-17 08:22:43.000000 ckanext-twitter-2.2.8/tests/test_templatehelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.789521 ckanext_twitter-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-14 10:47:08.789521 ckanext_twitter-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/twitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/twitter/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/lib/cache_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/lib/config_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/lib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/lib/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/lib/twitter_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/twitter/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/routes/tweet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.781521 ckanext_twitter-2.2.9/ckanext/twitter/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/twitter/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.781521 ckanext_twitter-2.2.9/ckanext/twitter/theme/assets/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/twitter/theme/assets/scripts/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/theme/assets/webassets.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.781521 ckanext_twitter-2.2.9/ckanext/twitter/theme/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/twitter/theme/templates/ajax_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.785521 ckanext_twitter-2.2.9/ckanext/twitter/theme/templates/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/theme/templates/package/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/ckanext/twitter/theme/templates/package/read_base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.789521 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-14 10:47:08.000000 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-14 10:47:08.000000 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:47:08.000000 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-14 10:47:08.000000 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:47:08.000000 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 10:47:08.000000 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 10:47:08.000000 ckanext_twitter-2.2.9/ckanext_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.781521 ckanext_twitter-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.789521 ckanext_twitter-2.2.9/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:47:08.789521 ckanext_twitter-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:47:08.789521 ckanext_twitter-2.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/tests/test_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/tests/test_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-14 10:47:04.000000 ckanext_twitter-2.2.9/tests/test_templatehelpers.py
```

### Comparing `ckanext-twitter-2.2.8/LICENSE` & `ckanext_twitter-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/PKG-INFO` & `ckanext_twitter-2.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-twitter
-Version: 2.2.8
+Version: 2.2.9
 Summary: A CKAN extension that enables users to post a tweet every time a dataset is created or updated.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-twitter
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-twitter/blob/main/CHANGELOG.md
 Keywords: CKAN,data,twitter
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,16 +12,30 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: oauth2==1.9.0.post1
+Requires-Dist: ckantools>=0.3.0
+Provides-Extra: test
+Requires-Dist: mock; extra == "test"
+Requires-Dist: pytest>=4.6.5; extra == "test"
+Requires-Dist: pytest-cov>=2.7.1; extra == "test"
+Requires-Dist: coveralls; extra == "test"
+
+<!--notices-start-->
+> **Warning**
+> ## This extension is now deprecated.
+>
+> Due to the API changes Twitter/X introduced in 2023, this extension no longer works and will not be fixed. There will not be any further releases, new features, or bugfixes.
+
+<!--notices-end-->
 
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-twitter
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-twitter/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-twitter/actions/workflows/main.yml)
```

### Comparing `ckanext-twitter-2.2.8/README.md` & `ckanext_twitter-2.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+<!--notices-start-->
+> **Warning**
+> ## This extension is now deprecated.
+>
+> Due to the API changes Twitter/X introduced in 2023, this extension no longer works and will not be fixed. There will not be any further releases, new features, or bugfixes.
+
+<!--notices-end-->
+
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-twitter
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-twitter/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-twitter/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-twitter/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-twitter)
```

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/lib/cache_helpers.py` & `ckanext_twitter-2.2.9/ckanext/twitter/lib/cache_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/lib/config_helpers.py` & `ckanext_twitter-2.2.9/ckanext/twitter/lib/config_helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/lib/helpers.py` & `ckanext_twitter-2.2.9/ckanext/twitter/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/lib/parsers.py` & `ckanext_twitter-2.2.9/ckanext/twitter/lib/parsers.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/lib/twitter_api.py` & `ckanext_twitter-2.2.9/ckanext/twitter/lib/twitter_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     """
     Attempts to create a client for accessing the twitter API using the credentials
     specified in the configuration file. Does not test for success. Caches the resulting
     client in the 'twitter' cache.
 
     :return: oauth2.Client
     """
+    logger.info('ckanext-twitter has been deprecated; please consider removing it')
+
     (
         consumer_key,
         consumer_secret,
         token_key,
         token_secret,
     ) = config_helpers.twitter_get_credentials()
     consumer = oauth2.Consumer(consumer_key, consumer_secret)
@@ -38,14 +40,16 @@
 def twitter_authenticate():
     """
     Verifies that the client is able to connect to the twitter API.
 
     Refreshes any unauthenticated cached client.
     :return: boolean
     """
+    logger.info('ckanext-twitter has been deprecated; please consider removing it')
+
     authenticated = False
     while not authenticated:
         client = twitter_client()
         url = 'https://api.twitter.com/1.1/account/verify_credentials.json'
         response, content = client.request(url, 'GET')
         authenticated = response.status == 200
         if not authenticated:
@@ -71,14 +75,16 @@
 
     :param tweet_text: The text to post. This is passed in rather than
     generated inside the method to allow users to change the tweet before
     posting (if enabled).
     :param pkg_id: The package ID (for caching).
     :return: boolean, str
     """
+    logger.info('ckanext-twitter has been deprecated; please consider removing it')
+
     if config_helpers.twitter_is_debug():
         logger.debug(f'Not posted (debug): {tweet_text}')
         return False, 'debug'
 
     # if not enough time has passed since the last tweet
     if not cache_helpers.expired(pkg_id):
         logger.debug(f'Not posted (insufficient rest period): {tweet_text}')
```

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/plugin.py` & `ckanext_twitter-2.2.9/ckanext/twitter/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/routes/tweet.py` & `ckanext_twitter-2.2.9/ckanext/twitter/routes/tweet.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js` & `ckanext_twitter-2.2.9/ckanext/twitter/theme/assets/scripts/modules/confirm-tweet.js`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html` & `ckanext_twitter-2.2.9/ckanext/twitter/theme/templates/ajax_snippets/edit_tweet.html`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/ckanext_twitter.egg-info/PKG-INFO` & `ckanext_twitter-2.2.9/ckanext_twitter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-twitter
-Version: 2.2.8
+Version: 2.2.9
 Summary: A CKAN extension that enables users to post a tweet every time a dataset is created or updated.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-twitter
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-twitter/blob/main/CHANGELOG.md
 Keywords: CKAN,data,twitter
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,16 +12,30 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: oauth2==1.9.0.post1
+Requires-Dist: ckantools>=0.3.0
+Provides-Extra: test
+Requires-Dist: mock; extra == "test"
+Requires-Dist: pytest>=4.6.5; extra == "test"
+Requires-Dist: pytest-cov>=2.7.1; extra == "test"
+Requires-Dist: coveralls; extra == "test"
+
+<!--notices-start-->
+> **Warning**
+> ## This extension is now deprecated.
+>
+> Due to the API changes Twitter/X introduced in 2023, this extension no longer works and will not be fixed. There will not be any further releases, new features, or bugfixes.
+
+<!--notices-end-->
 
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-twitter
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-twitter/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-twitter/actions/workflows/main.yml)
```

### Comparing `ckanext-twitter-2.2.8/ckanext_twitter.egg-info/SOURCES.txt` & `ckanext_twitter-2.2.9/ckanext_twitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/docs/_scripts/gen_api_pages.py` & `ckanext_twitter-2.2.9/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/pyproject.toml` & `ckanext_twitter-2.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ckanext-twitter"
-version = "2.2.8"
+version = "2.2.9"
 description = "A CKAN extension that enables users to post a tweet every time a dataset is created or updated."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
@@ -52,20 +52,21 @@
 exclude = ["tests", "docs"]
 
 [tool.setuptools.package-data]
 "ckanext.twitter.theme" = ["*", "**/*"]
 
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.2.8"
+version = "2.2.9"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
-    "pyproject.toml:version"
+    "pyproject.toml:version",
+    "CITATION.cff:^version"
 ]
 
 [tool.black]
 line-length = 88
 skip_string_normalization = true
 
 [tool.pylint]
```

### Comparing `ckanext-twitter-2.2.8/tests/test_authentication.py` & `ckanext_twitter-2.2.9/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/tests/test_config.py` & `ckanext_twitter-2.2.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/tests/test_controller.py` & `ckanext_twitter-2.2.9/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/tests/test_dataset.py` & `ckanext_twitter-2.2.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/tests/test_generation.py` & `ckanext_twitter-2.2.9/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/tests/test_routes.py` & `ckanext_twitter-2.2.9/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `ckanext-twitter-2.2.8/tests/test_templatehelpers.py` & `ckanext_twitter-2.2.9/tests/test_templatehelpers.py`

 * *Files identical despite different names*

