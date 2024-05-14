# Comparing `tmp/sphinx-immaterial-igwn-0.1.1.tar.gz` & `tmp/sphinx_immaterial_igwn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-immaterial-igwn-0.1.1.tar", last modified: Thu Oct  5 12:54:57 2023, max compression
+gzip compressed data, was "sphinx_immaterial_igwn-0.2.0.tar", last modified: Tue May 14 07:41:42 2024, max compression
```

## Comparing `sphinx-immaterial-igwn-0.1.1.tar` & `sphinx_immaterial_igwn-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.704761 sphinx-immaterial-igwn-0.1.1/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1734 2023-10-05 12:54:57.704761 sphinx-immaterial-igwn-0.1.1/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)      476 2023-10-05 12:42:27.000000 sphinx-immaterial-igwn-0.1.1/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.694761 sphinx-immaterial-igwn-0.1.1/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      799 2023-10-05 12:42:24.000000 sphinx-immaterial-igwn-0.1.1/docs/conf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      439 2023-10-05 12:42:24.000000 sphinx-immaterial-igwn-0.1.1/docs/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      359 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/docs/install.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      538 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/docs/usage.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      230 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1512 2023-10-05 12:54:57.704761 sphinx-immaterial-igwn-0.1.1/setup.cfg
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.694761 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1143 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      411 2023-10-05 12:54:57.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/_version.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1162 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/defaults.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      438 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/layout.html
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.694761 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/partials/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1209 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/partials/acknowledgements.html
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1444 2022-09-02 14:49:33.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/partials/copyright.html
--rw-r--r--   0 duncan    (1000) duncan    (1000)      257 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/partials/source-file.html
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.694761 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.704761 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    32038 2022-04-29 18:32:48.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/favicon.ico
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14199 2022-04-29 18:32:48.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/kagra.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)    62176 2022-04-29 18:32:48.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/ligo.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9635 2022-04-29 18:32:48.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/logo.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)  3560416 2022-04-29 18:32:48.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/lsc.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24558 2022-04-29 18:32:48.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/virgo.png
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.704761 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/stylesheets/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2097 2023-10-05 12:42:27.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/stylesheets/igwn-mkdocs-material.css
--rw-r--r--   0 duncan    (1000) duncan    (1000)       36 2022-05-23 10:45:35.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/theme.conf
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:57.694761 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1734 2023-10-05 12:54:57.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1043 2023-10-05 12:54:57.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-10-05 12:54:57.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       69 2023-10-05 12:54:57.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/entry_points.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       51 2023-10-05 12:54:57.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       23 2023-10-05 12:54:57.000000 sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/top_level.txt
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1751 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      476 2023-10-05 12:42:27.000000 sphinx_immaterial_igwn-0.2.0/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      799 2023-10-05 12:42:24.000000 sphinx_immaterial_igwn-0.2.0/docs/conf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      439 2023-10-05 12:42:24.000000 sphinx_immaterial_igwn-0.2.0/docs/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      359 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/docs/install.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      538 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/docs/usage.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1866 2024-05-13 15:06:32.000000 sphinx_immaterial_igwn-0.2.0/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/setup.cfg
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1143 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      411 2024-05-14 07:41:42.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/_version.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1162 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/defaults.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      438 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/layout.html
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/partials/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1209 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/partials/acknowledgements.html
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1444 2022-09-02 14:49:33.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/partials/copyright.html
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      257 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/partials/source-file.html
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    32038 2022-04-29 18:32:48.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/favicon.ico
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14199 2022-04-29 18:32:48.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/kagra.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    62176 2022-04-29 18:32:48.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/ligo.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9635 2022-04-29 18:32:48.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/logo.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)  3560416 2022-04-29 18:32:48.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/lsc.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24558 2022-04-29 18:32:48.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/virgo.png
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/stylesheets/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2097 2023-10-05 12:42:27.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/stylesheets/igwn-mkdocs-material.css
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       36 2022-05-23 10:45:35.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/theme.conf
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:42.322182 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1751 2024-05-14 07:41:42.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1033 2024-05-14 07:41:42.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2024-05-14 07:41:42.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       69 2024-05-14 07:41:42.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       51 2024-05-14 07:41:42.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       23 2024-05-14 07:41:42.000000 sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/top_level.txt
```

### Comparing `sphinx-immaterial-igwn-0.1.1/PKG-INFO` & `sphinx_immaterial_igwn-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: sphinx-immaterial-igwn
-Version: 0.1.1
+Version: 0.2.0
 Summary: IGWN extensions to sphinx-immaterial
-Author: Duncan Macleod
-Author-email: duncan.macleod@ligo.org
+Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: MIT
 Project-URL: Bug Tracker, https://git.ligo.org/computing/igwn-mkdocs-material-theme/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/igwn-mkdocs-material-theme/sphinx/
 Project-URL: Source Code, https://git.ligo.org/computing/igwn-mkdocs-material-theme.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Documentation
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sphinx-immaterial
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-immaterial; extra == "docs"
 
 # sphinx-immaterial-igwn
```

### Comparing `sphinx-immaterial-igwn-0.1.1/docs/conf.py` & `sphinx_immaterial_igwn-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/docs/usage.rst` & `sphinx_immaterial_igwn-0.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/setup.cfg` & `sphinx_immaterial_igwn-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,75 @@
-[metadata]
-name = sphinx-immaterial-igwn
-author = Duncan Macleod
-author_email = duncan.macleod@ligo.org
-description = IGWN extensions to sphinx-immaterial
-license = MIT
-license_files = LICENSE
-long_description = file: README.md
-long_description_content_type = text/markdown
-urls = https://git.ligo.org/computing/igwn-mkdocs-material-theme
-project_urls = 
-	Bug Tracker = https://git.ligo.org/computing/igwn-mkdocs-material-theme/-/issues
-	Documentation = https://computing.docs.ligo.org/igwn-mkdocs-material-theme/sphinx/
-	Source Code = https://git.ligo.org/computing/igwn-mkdocs-material-theme.git
-classifiers = 
-	Development Status :: 3 - Alpha
-	Framework :: Sphinx :: Theme
-	Intended Audience :: Science/Research
-	License :: OSI Approved :: MIT License
-	Natural Language :: English
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Topic :: Documentation
-	Topic :: Documentation :: Sphinx
-	Topic :: Scientific/Engineering
-	Topic :: Scientific/Engineering :: Astronomy
-	Topic :: Scientific/Engineering :: Physics
-	Topic :: Software Development :: Documentation
-
-[options]
-packages = find:
-install_requires = 
-	sphinx-immaterial
-
-[options.entry_points]
-sphinx.html_themes = 
-	sphinx_immaterial_igwn = sphinx_immaterial_igwn
-
-[options.extras_require]
-docs = 
-	sphinx
-	sphinx-immaterial
-
-[options.package_data]
-sphinx_immaterial_igwn = 
-	*.html
-	layout.html
-	partials/*.html
-	static/images/*.ico
-	static/images/*.png
-	static/stylesheets/*.css
-	theme.conf
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+[build-system]
+requires = [
+    "setuptools>=61.0.0",
+    "setuptools_scm[toml]>=3.4.3",
+    "wheel",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "sphinx-immaterial-igwn"
+description = "IGWN extensions to sphinx-immaterial"
+readme = "README.md"
+authors = [
+  { name = "Duncan Macleod", email = "duncan.macleod@ligo.org" },
+]
+license = { text = "MIT" }
+classifiers = [
+  "Development Status :: 3 - Alpha",
+  "Framework :: Sphinx :: Theme",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Topic :: Documentation",
+  "Topic :: Documentation :: Sphinx",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Astronomy",
+  "Topic :: Scientific/Engineering :: Physics",
+  "Topic :: Software Development :: Documentation",
+]
+requires-python = ">=3.8"
+dependencies = [
+  "sphinx-immaterial",
+]
+dynamic = [
+  "version",
+]
+
+[project.optional-dependencies]
+docs = [
+  "sphinx",
+  "sphinx-immaterial",
+]
+
+[project.entry-points."sphinx.html_themes"]
+sphinx_immaterial_igwn = "sphinx_immaterial_igwn"
+
+[project.urls]
+"Bug Tracker" = "https://git.ligo.org/computing/igwn-mkdocs-material-theme/-/issues"
+"Documentation" = "https://computing.docs.ligo.org/igwn-mkdocs-material-theme/sphinx/"
+"Source Code" = "https://git.ligo.org/computing/igwn-mkdocs-material-theme.git"
+
+[tool.setuptools]
+license-files = [ "LICENSE" ]
+
+[tool.setuptools.packages.find]
+include = [
+  "sphinx_immaterial_igwn*",
+]
+
+[tool.setuptools.package-data]
+sphinx_immaterial_igwn = [
+  "*.html",
+  "layout.html",
+  "partials/*.html",
+  "static/images/*.ico",
+  "static/images/*.png",
+  "static/stylesheets/*.css",
+  "theme.conf",
+]
+
+[tool.setuptools_scm]
+root = ".."
+write_to = "sphinx/sphinx_immaterial_igwn/_version.py"
```

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/__init__.py` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/defaults.py` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/defaults.py`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/partials/acknowledgements.html` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/partials/acknowledgements.html`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/partials/copyright.html` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/favicon.ico` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/kagra.png` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/kagra.png`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/ligo.png` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/ligo.png`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/logo.png` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/lsc.png` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/lsc.png`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/images/virgo.png` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/images/virgo.png`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn/static/stylesheets/igwn-mkdocs-material.css` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn/static/stylesheets/igwn-mkdocs-material.css`

 * *Files identical despite different names*

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/PKG-INFO` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: sphinx-immaterial-igwn
-Version: 0.1.1
+Version: 0.2.0
 Summary: IGWN extensions to sphinx-immaterial
-Author: Duncan Macleod
-Author-email: duncan.macleod@ligo.org
+Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: MIT
 Project-URL: Bug Tracker, https://git.ligo.org/computing/igwn-mkdocs-material-theme/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/igwn-mkdocs-material-theme/sphinx/
 Project-URL: Source Code, https://git.ligo.org/computing/igwn-mkdocs-material-theme.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Intended Audience :: Science/Research
@@ -17,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Documentation
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sphinx-immaterial
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-immaterial; extra == "docs"
 
 # sphinx-immaterial-igwn
```

### Comparing `sphinx-immaterial-igwn-0.1.1/sphinx_immaterial_igwn.egg-info/SOURCES.txt` & `sphinx_immaterial_igwn-0.2.0/sphinx_immaterial_igwn.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 README.md
 pyproject.toml
-setup.cfg
 docs/conf.py
 docs/index.rst
 docs/install.rst
 docs/usage.rst
 sphinx_immaterial_igwn/__init__.py
 sphinx_immaterial_igwn/_version.py
 sphinx_immaterial_igwn/defaults.py
```

