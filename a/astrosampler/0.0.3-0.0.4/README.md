# Comparing `tmp/astrosampler-0.0.3.tar.gz` & `tmp/astrosampler-0.0.4.tar.gz`

## Comparing `astrosampler-0.0.3.tar` & `astrosampler-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 astrosampler-0.0.3/.github/workflows/pr-validation.yml
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 astrosampler-0.0.3/.github/workflows/test-and-release.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 astrosampler-0.0.3/astrosampler/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrosampler-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 astrosampler-0.0.3/tests/sampler_test.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 astrosampler-0.0.3/.gitignore
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 astrosampler-0.0.3/LICENSE
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 astrosampler-0.0.3/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 astrosampler-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 astrosampler-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 astrosampler-0.0.4/.github/workflows/pr-validation.yml
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 astrosampler-0.0.4/.github/workflows/test-and-release.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 astrosampler-0.0.4/astrosampler/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrosampler-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 astrosampler-0.0.4/tests/sampler_test.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 astrosampler-0.0.4/.gitignore
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 astrosampler-0.0.4/LICENSE
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 astrosampler-0.0.4/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 astrosampler-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 astrosampler-0.0.4/PKG-INFO
```

### Comparing `astrosampler-0.0.3/.github/workflows/test-and-release.yml` & `astrosampler-0.0.4/.github/workflows/test-and-release.yml`

 * *Files identical despite different names*

### Comparing `astrosampler-0.0.3/LICENSE` & `astrosampler-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astrosampler-0.0.3/pyproject.toml` & `astrosampler-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="astrosampler"
-version="0.0.3"
+version="0.0.4"
 authors = [
     { name="Matthew Whitaker", email="sub6resources@gmail.com" },
 ]
 dependencies = [
     "numpy",
 ]
 description="A package for sampling typical distributions in astronomy"
```

### Comparing `astrosampler-0.0.3/PKG-INFO` & `astrosampler-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astrosampler
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for sampling typical distributions in astronomy
 Project-URL: Homepage, https://github.com/Sub6Resources/astro-sampler
 Project-URL: Issues, https://github.com/Sub6Resources/astro-sampler/issues
 Author-email: Matthew Whitaker <sub6resources@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

