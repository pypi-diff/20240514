# Comparing `tmp/sphinxcontrib_sqltable-2.1.0.0a2.tar.gz` & `tmp/sphinxcontrib_sqltable-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_sqltable-2.1.0.0a2.tar", last modified: Sun May  5 13:15:39 2024, max compression
+gzip compressed data, was "sphinxcontrib_sqltable-2.1.1.tar", last modified: Tue May 14 12:11:39 2024, max compression
```

## Comparing `sphinxcontrib_sqltable-2.1.0.0a2.tar` & `sphinxcontrib_sqltable-2.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.278709 sphinxcontrib_sqltable-2.1.0.0a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.282709 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.hgignore
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.hgtags
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/.mergify.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/announce.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.282709 sphinxcontrib_sqltable-2.1.0.0a2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/_static/.placeholder
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/customize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/example.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/docs/sampledata.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/sqltable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:15:39.286709 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 13:15:39.000000 sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-05 13:15:14.000000 sphinxcontrib_sqltable-2.1.0.0a2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:39.050220 sphinxcontrib_sqltable-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:39.042220 sphinxcontrib_sqltable-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:39.046220 sphinxcontrib_sqltable-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.hgignore
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.hgtags
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-14 12:11:39.050220 sphinxcontrib_sqltable-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/announce.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:39.046220 sphinxcontrib_sqltable-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:39.046220 sphinxcontrib_sqltable-2.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/_static/.placeholder
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/customize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/example.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/docs/sampledata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:11:39.050220 sphinxcontrib_sqltable-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:39.046220 sphinxcontrib_sqltable-2.1.1/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/sphinxcontrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/sphinxcontrib/sqltable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:11:39.046220 sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-14 12:11:39.000000 sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-14 12:11:39.000000 sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:11:39.000000 sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 12:11:39.000000 sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 12:11:39.000000 sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-14 12:11:18.000000 sphinxcontrib_sqltable-2.1.1/tox.ini
```

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/check.yml` & `sphinxcontrib_sqltable-2.1.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/python-publish.yaml` & `sphinxcontrib_sqltable-2.1.1/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/.github/workflows/test.yml` & `sphinxcontrib_sqltable-2.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/.hgtags` & `sphinxcontrib_sqltable-2.1.1/.hgtags`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/.mergify.yml` & `sphinxcontrib_sqltable-2.1.1/.mergify.yml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/LICENSE` & `sphinxcontrib_sqltable-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/Makefile` & `sphinxcontrib_sqltable-2.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/PKG-INFO` & `sphinxcontrib_sqltable-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib.sqltable
-Version: 2.1.0.0a2
+Version: 2.1.1
 Summary: Sphinx extension for embedding database content in documents
 Author-email: Doug Hellmann <doug@doughellmann.com>
 Project-URL: homepage, https://sphinxcontrib-sqltable.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/sphinx-contrib/sqltable
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -28,14 +28,17 @@
 Requires-Dist: flake8; extra == "linter"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: beautifulsoup4; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
+Provides-Extra: docs
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
 
 .. -*- mode: rst -*-
 
 ========================
  sphinxcontrib-sqltable
 ========================
```

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/README.rst` & `sphinxcontrib_sqltable-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/announce.rst` & `sphinxcontrib_sqltable-2.1.1/announce.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/docs/Makefile` & `sphinxcontrib_sqltable-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/docs/conf.py` & `sphinxcontrib_sqltable-2.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
+import importlib
 import os
 import sqlite3
 import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
@@ -50,15 +51,15 @@
 copyright = u'2012, Doug Hellmann'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.0'
+version = importlib.metadata.version('sphinxcontrib.sqltable')
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
@@ -93,15 +94,15 @@
 #modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
```

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/docs/customize.rst` & `sphinxcontrib_sqltable-2.1.1/docs/customize.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/docs/developers.rst` & `sphinxcontrib_sqltable-2.1.1/docs/developers.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/docs/example.rst` & `sphinxcontrib_sqltable-2.1.1/docs/example.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/docs/index.rst` & `sphinxcontrib_sqltable-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/docs/install.rst` & `sphinxcontrib_sqltable-2.1.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/pyproject.toml` & `sphinxcontrib_sqltable-2.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     "pytest",
     "beautifulsoup4",
 ]
 build = [
     "build",
     "twine",
 ]
+docs = [
+    "sphinx_rtd_theme",
+    "sphinx",
+]
 
 [tools.setuptools]
 packages = [
     "sphinxcontrib.sqltable",
 ]
 
 # https://github.com/pypa/setuptools_scm/
```

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib/sqltable.py` & `sphinxcontrib_sqltable-2.1.1/sphinxcontrib/sqltable.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,28 +67,28 @@
 
         # Run the query
         try:
             query = '\n'.join(self.content)
             LOG.info('Running query %r' % query)
             with engine.connect() as conn:
                 results = conn.execute(sqlalchemy.text(query))
+                table_headers = results.keys()
+                table_body = results.fetchall()
         except Exception as err:
             error = self.state_machine.reporter.error(
                 u'Error with query %s for sqltable: %s' % (
                     query,
                     err,
                 ),
                 nodes.literal_block(self.block_text, self.block_text),
                 line=self.lineno,
             )
             return [error]
 
         # Extract some values we need for building the table.
-        table_headers = results.keys()
-        table_body = results
         max_cols = len(table_headers)
 
         # Handle the width settings and title
         try:
             col_widths = self.get_column_widths(max_cols)
             title, messages = self.make_title()
         except SystemMessagePropagation as detail:
```

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/PKG-INFO` & `sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib.sqltable
-Version: 2.1.0.0a2
+Version: 2.1.1
 Summary: Sphinx extension for embedding database content in documents
 Author-email: Doug Hellmann <doug@doughellmann.com>
 Project-URL: homepage, https://sphinxcontrib-sqltable.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/sphinx-contrib/sqltable
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -28,14 +28,17 @@
 Requires-Dist: flake8; extra == "linter"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: beautifulsoup4; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
+Provides-Extra: docs
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
 
 .. -*- mode: rst -*-
 
 ========================
  sphinxcontrib-sqltable
 ========================
```

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/sphinxcontrib.sqltable.egg-info/SOURCES.txt` & `sphinxcontrib_sqltable-2.1.1/sphinxcontrib.sqltable.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 .hgignore
 .hgtags
 .mergify.yml
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 announce.rst
 pyproject.toml
 requirements.txt
@@ -17,15 +18,14 @@
 docs/conf.py
 docs/customize.rst
 docs/developers.rst
 docs/example.rst
 docs/history.rst
 docs/index.rst
 docs/install.rst
-docs/requirements.txt
 docs/sampledata.sql
 docs/_static/.placeholder
 sphinxcontrib/__init__.py
 sphinxcontrib/sqltable.py
 sphinxcontrib.sqltable.egg-info/PKG-INFO
 sphinxcontrib.sqltable.egg-info/SOURCES.txt
 sphinxcontrib.sqltable.egg-info/dependency_links.txt
```

### Comparing `sphinxcontrib_sqltable-2.1.0.0a2/tox.ini` & `sphinxcontrib_sqltable-2.1.1/tox.ini`

 * *Files identical despite different names*

