# Comparing `tmp/earthkit-0.5.0.tar.gz` & `tmp/earthkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-0.5.0.tar", last modified: Fri Apr 26 13:48:54 2024, max compression
+gzip compressed data, was "earthkit-0.5.1.tar", last modified: Tue May 14 17:43:02 2024, max compression
```

## Comparing `earthkit-0.5.0.tar` & `earthkit-0.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.394324 earthkit-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.386324 earthkit-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-26 13:48:44.000000 earthkit-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-26 13:48:44.000000 earthkit-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-26 13:48:44.000000 earthkit-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 13:48:44.000000 earthkit-0.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-04-26 13:48:44.000000 earthkit-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-26 13:48:44.000000 earthkit-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-26 13:48:54.394324 earthkit-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-26 13:48:44.000000 earthkit-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/_ext/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    60639 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/_static/earthkit.png
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/components_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    73703 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/examples/01_grib_file.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    52548 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/examples/02_grib_fdb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/licence.rst
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 13:48:44.000000 earthkit-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/earthkit/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-26 13:48:44.000000 earthkit-0.5.0/earthkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.394324 earthkit-0.5.0/earthkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 13:48:54.000000 earthkit-0.5.0/earthkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 13:48:44.000000 earthkit-0.5.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-26 13:48:44.000000 earthkit-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 13:48:44.000000 earthkit-0.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-26 13:48:54.394324 earthkit-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:48:54.390324 earthkit-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 13:48:44.000000 earthkit-0.5.0/tests/environment-docs-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-26 13:48:44.000000 earthkit-0.5.0/tests/environment-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-26 13:48:44.000000 earthkit-0.5.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.954032 earthkit-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.954032 earthkit-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-14 17:42:53.000000 earthkit-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-14 17:42:53.000000 earthkit-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-14 17:42:53.000000 earthkit-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 17:42:53.000000 earthkit-0.5.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-14 17:42:53.000000 earthkit-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 17:42:53.000000 earthkit-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-14 17:43:02.958032 earthkit-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 17:42:53.000000 earthkit-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/_ext/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    60639 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/_static/earthkit.png
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/components_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    73703 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/examples/01_grib_file.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    52548 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/examples/02_grib_fdb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 17:42:53.000000 earthkit-0.5.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/earthkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 17:42:53.000000 earthkit-0.5.1/earthkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 17:43:02.000000 earthkit-0.5.1/earthkit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/earthkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-14 17:43:02.000000 earthkit-0.5.1/earthkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-14 17:43:02.000000 earthkit-0.5.1/earthkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:43:02.000000 earthkit-0.5.1/earthkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-14 17:43:02.000000 earthkit-0.5.1/earthkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 17:43:02.000000 earthkit-0.5.1/earthkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-14 17:42:53.000000 earthkit-0.5.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-14 17:42:53.000000 earthkit-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 17:42:53.000000 earthkit-0.5.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-14 17:43:02.958032 earthkit-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:43:02.958032 earthkit-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-14 17:42:53.000000 earthkit-0.5.1/tests/environment-docs-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 17:42:53.000000 earthkit-0.5.1/tests/environment-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-14 17:42:53.000000 earthkit-0.5.1/tests/test_version.py
```

### Comparing `earthkit-0.5.0/.github/workflows/ci.yml` & `earthkit-0.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/.gitignore` & `earthkit-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/.pre-commit-config.yaml` & `earthkit-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/LICENSE` & `earthkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/PKG-INFO` & `earthkit-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit
-Version: 0.5.0
+Version: 0.5.1
 Home-page: https://github.com/ecmwf/earthkit
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: earthkit-data[all]>=0.7.0
 Requires-Dist: earthkit-geo>=0.1.0
 Requires-Dist: earthkit-maps>=0.0.18
 Requires-Dist: earthkit-meteo>=0.1.0
 Requires-Dist: earthkit-plots>=0.0.6
-Requires-Dist: earthkit-regrid>=0.3.0
+Requires-Dist: earthkit-regrid>=0.3.1
 
 # earthkit
 
 <img src="docs/_static/earthkit.png" width="120">
 
 [![PyPI version fury.io](https://badge.fury.io/py/earthkit.svg)](https://pypi.python.org/pypi/earthkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit.svg)](https://pypi.python.org/pypi/earthkit/)
```

### Comparing `earthkit-0.5.0/README.md` & `earthkit-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/Makefile` & `earthkit-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/_ext/xref.py` & `earthkit-0.5.1/docs/_ext/xref.py`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/_static/earthkit.png` & `earthkit-0.5.1/docs/_static/earthkit.png`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/_static/style.css` & `earthkit-0.5.1/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/components_overview.rst` & `earthkit-0.5.1/docs/components_overview.rst`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/conf.py` & `earthkit-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/examples/01_grib_file.ipynb` & `earthkit-0.5.1/docs/examples/01_grib_file.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/examples/02_grib_fdb.ipynb` & `earthkit-0.5.1/docs/examples/02_grib_fdb.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/index.rst` & `earthkit-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/docs/install.rst` & `earthkit-0.5.1/docs/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 ..     conda install earthkit -c conda-forge
 
 .. This will bring in some necessary binary dependencies for you.
 
 Installing the binary dependencies
 --------------------------------------
 
-This is the list of components with have binary dependencies. Please click on the links to see the installation instructions.
+This is the list of components with binary dependencies. Please click on the links to see the installation instructions.
 
 -  `eartkit-data <https://earthkit-data.readthedocs.io/en/latest/install.html#installing-the-binary-dependencies>`_
```

### Comparing `earthkit-0.5.0/docs/licence.rst` & `earthkit-0.5.1/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/earthkit/__init__.py` & `earthkit-0.5.1/earthkit/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/earthkit.egg-info/PKG-INFO` & `earthkit-0.5.1/earthkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit
-Version: 0.5.0
+Version: 0.5.1
 Home-page: https://github.com/ecmwf/earthkit
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: earthkit-data[all]>=0.7.0
 Requires-Dist: earthkit-geo>=0.1.0
 Requires-Dist: earthkit-maps>=0.0.18
 Requires-Dist: earthkit-meteo>=0.1.0
 Requires-Dist: earthkit-plots>=0.0.6
-Requires-Dist: earthkit-regrid>=0.3.0
+Requires-Dist: earthkit-regrid>=0.3.1
 
 # earthkit
 
 <img src="docs/_static/earthkit.png" width="120">
 
 [![PyPI version fury.io](https://badge.fury.io/py/earthkit.svg)](https://pypi.python.org/pypi/earthkit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit.svg)](https://pypi.python.org/pypi/earthkit/)
```

### Comparing `earthkit-0.5.0/earthkit.egg-info/SOURCES.txt` & `earthkit-0.5.1/earthkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthkit-0.5.0/setup.cfg` & `earthkit-0.5.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 packages = find_namespace:
 install_requires = 
 	earthkit-data[all]>=0.7.0
 	earthkit-geo>=0.1.0
 	earthkit-maps>=0.0.18
 	earthkit-meteo>=0.1.0
 	earthkit-plots>=0.0.6
-	earthkit-regrid>=0.3.0
+	earthkit-regrid>=0.3.1
 
 [options.packages.find]
 include = earthkit, earthkit.*
 
 [flake8]
 max-line-length = 110
 extend-ignore = E203, W503
```

### Comparing `earthkit-0.5.0/tests/test_version.py` & `earthkit-0.5.1/tests/test_version.py`

 * *Files identical despite different names*

