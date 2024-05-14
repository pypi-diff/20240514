# Comparing `tmp/mkdocs-material-igwn-0.1.1.tar.gz` & `tmp/mkdocs_material_igwn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-material-igwn-0.1.1.tar", last modified: Thu Oct  5 12:54:47 2023, max compression
+gzip compressed data, was "mkdocs_material_igwn-0.2.0.tar", last modified: Tue May 14 07:41:37 2024, max compression
```

## Comparing `mkdocs-material-igwn-0.1.1.tar` & `mkdocs_material_igwn-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.204753 mkdocs-material-igwn-0.1.1/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1568 2023-10-05 12:54:47.204753 mkdocs-material-igwn-0.1.1/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)      433 2022-09-02 14:49:33.000000 mkdocs-material-igwn-0.1.1/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.194753 mkdocs-material-igwn-0.1.1/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      376 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/docs/index.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)      374 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/docs/install.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)      320 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/docs/usage.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.194753 mkdocs-material-igwn-0.1.1/material_igwn/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      291 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/material_igwn/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      411 2023-10-05 12:54:47.000000 mkdocs-material-igwn-0.1.1/material_igwn/_version.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.194753 mkdocs-material-igwn-0.1.1/material_igwn/assets/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.204753 mkdocs-material-igwn-0.1.1/material_igwn/assets/images/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    32038 2022-04-29 18:32:48.000000 mkdocs-material-igwn-0.1.1/material_igwn/assets/images/favicon.ico
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14199 2022-04-29 18:32:48.000000 mkdocs-material-igwn-0.1.1/material_igwn/assets/images/kagra.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)    62176 2022-04-29 18:32:48.000000 mkdocs-material-igwn-0.1.1/material_igwn/assets/images/ligo.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9635 2022-04-29 18:32:48.000000 mkdocs-material-igwn-0.1.1/material_igwn/assets/images/logo.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)  3560416 2022-04-29 18:32:48.000000 mkdocs-material-igwn-0.1.1/material_igwn/assets/images/lsc.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24558 2022-04-29 18:32:48.000000 mkdocs-material-igwn-0.1.1/material_igwn/assets/images/virgo.png
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.204753 mkdocs-material-igwn-0.1.1/material_igwn/assets/stylesheets/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2097 2023-10-05 12:42:27.000000 mkdocs-material-igwn-0.1.1/material_igwn/assets/stylesheets/igwn-mkdocs-material.css
--rw-r--r--   0 duncan    (1000) duncan    (1000)      240 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/material_igwn/main.html
--rw-r--r--   0 duncan    (1000) duncan    (1000)      661 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/material_igwn/mkdocs_theme.yml
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.204753 mkdocs-material-igwn-0.1.1/material_igwn/partials/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1209 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/material_igwn/partials/acknowledgements.html
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1017 2022-09-02 14:49:33.000000 mkdocs-material-igwn-0.1.1/material_igwn/partials/copyright.html
--rw-r--r--   0 duncan    (1000) duncan    (1000)      527 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/mkdocs.yml
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-10-05 12:54:47.204753 mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1568 2023-10-05 12:54:47.000000 mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)      829 2023-10-05 12:54:47.000000 mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-10-05 12:54:47.000000 mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       46 2023-10-05 12:54:47.000000 mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/entry_points.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       53 2023-10-05 12:54:47.000000 mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       14 2023-10-05 12:54:47.000000 mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      221 2022-05-23 10:45:35.000000 mkdocs-material-igwn-0.1.1/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1360 2023-10-05 12:54:47.204753 mkdocs-material-igwn-0.1.1/setup.cfg
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1581 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      433 2022-09-02 14:49:33.000000 mkdocs_material_igwn-0.2.0/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      376 2022-05-23 10:45:35.000000 mkdocs_material_igwn-0.2.0/docs/index.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      374 2022-05-23 10:45:35.000000 mkdocs_material_igwn-0.2.0/docs/install.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      320 2022-05-23 10:45:35.000000 mkdocs_material_igwn-0.2.0/docs/usage.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/material_igwn/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      291 2022-05-23 10:45:35.000000 mkdocs_material_igwn-0.2.0/material_igwn/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      411 2024-05-14 07:41:37.000000 mkdocs_material_igwn-0.2.0/material_igwn/_version.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.531828 mkdocs_material_igwn-0.2.0/material_igwn/assets/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/material_igwn/assets/images/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    32038 2022-04-29 18:32:48.000000 mkdocs_material_igwn-0.2.0/material_igwn/assets/images/favicon.ico
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14199 2022-04-29 18:32:48.000000 mkdocs_material_igwn-0.2.0/material_igwn/assets/images/kagra.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    62176 2022-04-29 18:32:48.000000 mkdocs_material_igwn-0.2.0/material_igwn/assets/images/ligo.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9635 2022-04-29 18:32:48.000000 mkdocs_material_igwn-0.2.0/material_igwn/assets/images/logo.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)  3560416 2022-04-29 18:32:48.000000 mkdocs_material_igwn-0.2.0/material_igwn/assets/images/lsc.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24558 2022-04-29 18:32:48.000000 mkdocs_material_igwn-0.2.0/material_igwn/assets/images/virgo.png
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/material_igwn/assets/stylesheets/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2097 2023-10-05 12:42:27.000000 mkdocs_material_igwn-0.2.0/material_igwn/assets/stylesheets/igwn-mkdocs-material.css
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      240 2022-05-23 10:45:35.000000 mkdocs_material_igwn-0.2.0/material_igwn/main.html
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      661 2022-05-23 10:45:35.000000 mkdocs_material_igwn-0.2.0/material_igwn/mkdocs_theme.yml
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/material_igwn/partials/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1209 2022-05-23 10:45:35.000000 mkdocs_material_igwn-0.2.0/material_igwn/partials/acknowledgements.html
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1017 2022-09-02 14:49:33.000000 mkdocs_material_igwn-0.2.0/material_igwn/partials/copyright.html
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      540 2024-05-13 14:51:51.000000 mkdocs_material_igwn-0.2.0/mkdocs.yml
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1581 2024-05-14 07:41:37.000000 mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      819 2024-05-14 07:41:37.000000 mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2024-05-14 07:41:37.000000 mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       46 2024-05-14 07:41:37.000000 mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       53 2024-05-14 07:41:37.000000 mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       14 2024-05-14 07:41:37.000000 mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1693 2024-05-13 15:32:51.000000 mkdocs_material_igwn-0.2.0/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2024-05-14 07:41:37.541829 mkdocs_material_igwn-0.2.0/setup.cfg
```

### Comparing `mkdocs-material-igwn-0.1.1/PKG-INFO` & `mkdocs_material_igwn-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: mkdocs-material-igwn
-Version: 0.1.1
+Version: 0.2.0
 Summary: IGWN extensions to Material for MkDocs
-Author: Duncan Macleod
-Author-email: duncan.macleod@ligo.org
+Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: MIT
 Project-URL: Bug Tracker, https://git.ligo.org/computing/igwn-material/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/igwn-material/mkdocs/
-Project-URL: Source Code, https://git.ligo.org/computing/igwn-material.git
+Project-URL: Source Code, https://git.ligo.org/computing/igwn-material
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Documentation
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: mkdocs-material~=8.0
+Requires-Dist: mkdocs-material~=9.0
 Provides-Extra: docs
 Requires-Dist: markdown-include; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 
 # IGWN Material for MkDocs
 
 This project defines the IGWN Material theme for MkDocs, an extension of
```

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/assets/images/favicon.ico` & `mkdocs_material_igwn-0.2.0/material_igwn/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/assets/images/kagra.png` & `mkdocs_material_igwn-0.2.0/material_igwn/assets/images/kagra.png`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/assets/images/ligo.png` & `mkdocs_material_igwn-0.2.0/material_igwn/assets/images/ligo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/assets/images/logo.png` & `mkdocs_material_igwn-0.2.0/material_igwn/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/assets/images/lsc.png` & `mkdocs_material_igwn-0.2.0/material_igwn/assets/images/lsc.png`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/assets/images/virgo.png` & `mkdocs_material_igwn-0.2.0/material_igwn/assets/images/virgo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/assets/stylesheets/igwn-mkdocs-material.css` & `mkdocs_material_igwn-0.2.0/material_igwn/assets/stylesheets/igwn-mkdocs-material.css`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/mkdocs_theme.yml` & `mkdocs_material_igwn-0.2.0/material_igwn/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/partials/acknowledgements.html` & `mkdocs_material_igwn-0.2.0/material_igwn/partials/acknowledgements.html`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/material_igwn/partials/copyright.html` & `mkdocs_material_igwn-0.2.0/material_igwn/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `mkdocs-material-igwn-0.1.1/mkdocs.yml` & `mkdocs_material_igwn-0.2.0/mkdocs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 
 nav:
   - index.md
   - install.md
   - usage.md
 
 markdown_extensions:
-  - markdown.extensions.codehilite
   - markdown_include.include
+  - pymdownx.highlight
+  - pymdownx.superfences
```

### Comparing `mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/PKG-INFO` & `mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: mkdocs-material-igwn
-Version: 0.1.1
+Version: 0.2.0
 Summary: IGWN extensions to Material for MkDocs
-Author: Duncan Macleod
-Author-email: duncan.macleod@ligo.org
+Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: MIT
 Project-URL: Bug Tracker, https://git.ligo.org/computing/igwn-material/-/issues
 Project-URL: Documentation, https://computing.docs.ligo.org/igwn-material/mkdocs/
-Project-URL: Source Code, https://git.ligo.org/computing/igwn-material.git
+Project-URL: Source Code, https://git.ligo.org/computing/igwn-material
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Documentation
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: mkdocs-material~=8.0
+Requires-Dist: mkdocs-material~=9.0
 Provides-Extra: docs
 Requires-Dist: markdown-include; extra == "docs"
 Requires-Dist: mkdocs; extra == "docs"
 
 # IGWN Material for MkDocs
 
 This project defines the IGWN Material theme for MkDocs, an extension of
```

### Comparing `mkdocs-material-igwn-0.1.1/mkdocs_material_igwn.egg-info/SOURCES.txt` & `mkdocs_material_igwn-0.2.0/mkdocs_material_igwn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 mkdocs.yml
 pyproject.toml
-setup.cfg
 docs/index.md
 docs/install.md
 docs/usage.md
 material_igwn/__init__.py
 material_igwn/_version.py
 material_igwn/main.html
 material_igwn/mkdocs_theme.yml
```

### Comparing `mkdocs-material-igwn-0.1.1/setup.cfg` & `mkdocs_material_igwn-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,72 @@
-[metadata]
-name = mkdocs-material-igwn
-author = Duncan Macleod
-author_email = duncan.macleod@ligo.org
-description = IGWN extensions to Material for MkDocs
-license = MIT
-license_files = LICENSE
-long_description = file: README.md
-long_description_content_type = text/markdown
-urls = https://git.ligo.org/computing/igwn-material
-project_urls = 
-	Bug Tracker = https://git.ligo.org/computing/igwn-material/-/issues
-	Documentation = https://computing.docs.ligo.org/igwn-material/mkdocs/
-	Source Code = https://git.ligo.org/computing/igwn-material.git
-classifiers = 
-	Development Status :: 3 - Alpha
-	Intended Audience :: Science/Research
-	License :: OSI Approved :: MIT License
-	Natural Language :: English
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Topic :: Documentation
-	Topic :: Scientific/Engineering
-	Topic :: Scientific/Engineering :: Astronomy
-	Topic :: Scientific/Engineering :: Physics
-	Topic :: Software Development :: Documentation
-
-[options]
-packages = find:
-install_requires = 
-	mkdocs-material ~=8.0
-
-[options.entry_points]
-mkdocs.themes = 
-	material_igwn = material_igwn
-
-[options.extras_require]
-docs = 
-	markdown-include
-	mkdocs
-
-[options.package_data]
-material_igwn = 
-	*.html
-	mkdocs_theme.yml
-	partials/*.html
-	assets/stylesheets/*.css
-	assets/images/*.ico
-	assets/images/*.png
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
+name = "mkdocs-material-igwn"
+description = "IGWN extensions to Material for MkDocs"
+readme = "README.md"
+authors = [
+  { name = "Duncan Macleod", email = "duncan.macleod@ligo.org" },
+]
+license = { text = "MIT" }
+classifiers = [
+  "Development Status :: 3 - Alpha",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Topic :: Documentation",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Astronomy",
+  "Topic :: Scientific/Engineering :: Physics",
+  "Topic :: Software Development :: Documentation",
+]
+requires-python = ">=3.8"
+dependencies = [
+  "mkdocs-material ~=9.0",
+]
+dynamic = [
+  "version",
+]
+
+[project.entry-points."mkdocs.themes"]
+material_igwn = "material_igwn"
+
+[project.optional-dependencies]
+docs = [
+  "markdown-include",
+  "mkdocs",
+]
+
+[project.urls]
+"Bug Tracker" = "https://git.ligo.org/computing/igwn-material/-/issues"
+"Documentation" = "https://computing.docs.ligo.org/igwn-material/mkdocs/"
+"Source Code" = "https://git.ligo.org/computing/igwn-material"
+
+[tool.setuptools]
+license-files = [ "LICENSE" ]
+
+[tool.setuptools.packages.find]
+include = [
+  "material_igwn*",
+]
+
+[tool.setuptools.package-data]
+material_igwn = [
+  "*.html",
+  "mkdocs_theme.yml",
+  "partials/*.html",
+  "assets/stylesheets/*.css",
+  "assets/images/*.ico",
+  "assets/images/*.png",
+]
+
+[tool.setuptools_scm]
+root = ".."
+write_to = "mkdocs/material_igwn/_version.py"
```

