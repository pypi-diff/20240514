# Comparing `tmp/astrosampler-0.0.2.tar.gz` & `tmp/astrosampler-0.0.3.tar.gz`

## Comparing `astrosampler-0.0.2.tar` & `astrosampler-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 astrosampler-0.0.2/.release.sh
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 astrosampler-0.0.2/.github/workflows/pr-validation.yml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 astrosampler-0.0.2/.github/workflows/test-and-release.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 astrosampler-0.0.2/astrosampler/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrosampler-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 astrosampler-0.0.2/tests/sampler_test.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 astrosampler-0.0.2/.gitignore
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 astrosampler-0.0.2/LICENSE
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 astrosampler-0.0.2/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 astrosampler-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 astrosampler-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 astrosampler-0.0.3/.github/workflows/pr-validation.yml
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 astrosampler-0.0.3/.github/workflows/test-and-release.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 astrosampler-0.0.3/astrosampler/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astrosampler-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 astrosampler-0.0.3/tests/sampler_test.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 astrosampler-0.0.3/.gitignore
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 astrosampler-0.0.3/LICENSE
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 astrosampler-0.0.3/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 astrosampler-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 astrosampler-0.0.3/PKG-INFO
```

### Comparing `astrosampler-0.0.2/.github/workflows/test-and-release.yml` & `astrosampler-0.0.3/.github/workflows/test-and-release.yml`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       uses: actions/create-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ steps.version.outputs.v-version }}
         release_name: Release ${{ steps.version.outputs.version }}
         body: |
-          Release: ${{ steps.version.outputs.version }}
+          See https://pypi.org/project/astrosampler/${{ steps.version.outputs.version }}/
         draft: false
         prerelease: false
     - name: Update Version in File
       id: update_version
       run: |
         sed -i "s/{{VERSION_NUMBER}}/${{ steps.version.outputs.version }}/" pyproject.toml
     - name: Build Project
```

### Comparing `astrosampler-0.0.2/LICENSE` & `astrosampler-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astrosampler-0.0.2/pyproject.toml` & `astrosampler-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="astrosampler"
-version="0.0.2"
+version="0.0.3"
 authors = [
     { name="Matthew Whitaker", email="sub6resources@gmail.com" },
 ]
 dependencies = [
     "numpy",
 ]
 description="A package for sampling typical distributions in astronomy"
```

### Comparing `astrosampler-0.0.2/PKG-INFO` & `astrosampler-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astrosampler
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for sampling typical distributions in astronomy
 Project-URL: Homepage, https://github.com/Sub6Resources/astro-sampler
 Project-URL: Issues, https://github.com/Sub6Resources/astro-sampler/issues
 Author-email: Matthew Whitaker <sub6resources@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

