# Comparing `tmp/rms-vicar-1.0.4.tar.gz` & `tmp/rms_vicar-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-vicar-1.0.4.tar", last modified: Fri Mar  1 17:44:08 2024, max compression
+gzip compressed data, was "rms_vicar-1.0.5.tar", last modified: Tue May 14 19:07:42 2024, max compression
```

## Comparing `rms-vicar-1.0.4.tar` & `rms_vicar-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:44:08.372589 rms-vicar-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:44:08.356589 rms-vicar-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:44:08.360589 rms-vicar-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-03-01 17:44:08.372589 rms-vicar-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:44:08.372589 rms-vicar-1.0.4/rms_vicar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-03-01 17:44:08.000000 rms-vicar-1.0.4/rms_vicar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-01 17:44:08.000000 rms-vicar-1.0.4/rms_vicar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 17:44:08.000000 rms-vicar-1.0.4/rms_vicar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-01 17:44:08.000000 rms-vicar-1.0.4/rms_vicar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-01 17:44:08.000000 rms-vicar-1.0.4/rms_vicar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-01 17:44:08.372589 rms-vicar-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:44:08.364589 rms-vicar-1.0.4/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)   831488 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/test_files/C0532836239R.IMG
--rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/test_files/C2069302_GEOMA.DAT
--rw-r--r--   0 runner    (1001) docker     (127)  2002000 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/test_files/C2069302_GEOMED.IMG
--rw-r--r--   0 runner    (1001) docker     (127)   823296 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/test_files/C2069302_RAW.IMG
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/test_files/C2069302_RESLOC.DAT
--rwxr-xr-x   0 runner    (1001) docker     (127)  4202496 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/test_files/N1536633072_1_CALIB.IMG
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:44:08.368589 rms-vicar-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/tests/test_LABEL_GRAMMAR.py
--rw-r--r--   0 runner    (1001) docker     (127)    23629 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/tests/test_vicarimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/tests/test_vicarlabel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 17:44:08.372589 rms-vicar-1.0.4/vicar/
--rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/vicar/_LABEL_GRAMMAR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/vicar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-01 17:44:08.000000 rms-vicar-1.0.4/vicar/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    29610 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/vicar/vicarimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-03-01 17:43:57.000000 rms-vicar-1.0.4/vicar/vicarlabel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.734450 rms_vicar-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.734450 rms_vicar-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/rms_vicar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/rms_vicar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.742450 rms_vicar-1.0.5/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   831488 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C0532836239R.IMG
+-rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_GEOMA.DAT
+-rw-r--r--   0 runner    (1001) docker     (127)  2002000 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_GEOMED.IMG
+-rw-r--r--   0 runner    (1001) docker     (127)   823296 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_RAW.IMG
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/C2069302_RESLOC.DAT
+-rwxr-xr-x   0 runner    (1001) docker     (127)  4202496 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/test_files/N1536633072_1_CALIB.IMG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.746450 rms_vicar-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/test_LABEL_GRAMMAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23629 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/test_vicarimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/tests/test_vicarlabel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:07:42.750450 rms_vicar-1.0.5/vicar/
+-rw-r--r--   0 runner    (1001) docker     (127)     9925 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/_LABEL_GRAMMAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:07:42.000000 rms_vicar-1.0.5/vicar/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29610 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/vicarimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51298 2024-05-14 19:07:31.000000 rms_vicar-1.0.5/vicar/vicarlabel.py
```

### Comparing `rms-vicar-1.0.4/.github/workflows/publish_to_pypi.yml` & `rms_vicar-1.0.5/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/.github/workflows/publish_to_test_pypi.yml` & `rms_vicar-1.0.5/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/.github/workflows/run-tests.yml` & `rms_vicar-1.0.5/.github/workflows/run-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 jobs:
   test:
     name: Test vicar
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [ '3.7', '3.8', '3.9', '3.10', '3.11', '3.12' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
       fail-fast: false
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
```

### Comparing `rms-vicar-1.0.4/.gitignore` & `rms_vicar-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/LICENSE` & `rms_vicar-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/PKG-INFO` & `rms_vicar-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-vicar
-Version: 1.0.4
+Version: 1.0.5
 Summary: Routines for converting to and from VICAR image files
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-vicar
 Project-URL: Repository, https://github.com/SETI/rms-vicar
 Project-URL: Source, https://github.com/SETI/rms-vicar
 Project-URL: Issues, https://github.com/SETI/rms-vicar/issues
@@ -54,15 +54,15 @@
 [![Number of GitHub stars](https://img.shields.io/github/stars/SETI/rms-vicar)](https://github.com/SETI/rms-vicar/stargazers)
 ![GitHub forks](https://img.shields.io/github/forks/SETI/rms-vicar)
 
 # rms-vicar
 
 PDS Ring-Moon Systems Node, SETI Institute
 
-Supported versions: Python >= 3.7
+Supported versions: Python >= 3.8
 
 Classes and methods to read and write JPL's VICAR-format data files:
 
     VicarLabel      class for reading, writing, and parsing of VICAR labels.
     VicarImage      class for handling VICAR image (and other) data files.
     VicarError      extension of class ValueError to contain exceptions.
```

### Comparing `rms-vicar-1.0.4/README.md` & `rms_vicar-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 [![Number of GitHub stars](https://img.shields.io/github/stars/SETI/rms-vicar)](https://github.com/SETI/rms-vicar/stargazers)
 ![GitHub forks](https://img.shields.io/github/forks/SETI/rms-vicar)
 
 # rms-vicar
 
 PDS Ring-Moon Systems Node, SETI Institute
 
-Supported versions: Python >= 3.7
+Supported versions: Python >= 3.8
 
 Classes and methods to read and write JPL's VICAR-format data files:
 
     VicarLabel      class for reading, writing, and parsing of VICAR labels.
     VicarImage      class for handling VICAR image (and other) data files.
     VicarError      extension of class ValueError to contain exceptions.
```

### Comparing `rms-vicar-1.0.4/pyproject.toml` & `rms_vicar-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/rms_vicar.egg-info/PKG-INFO` & `rms_vicar-1.0.5/rms_vicar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-vicar
-Version: 1.0.4
+Version: 1.0.5
 Summary: Routines for converting to and from VICAR image files
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-vicar
 Project-URL: Repository, https://github.com/SETI/rms-vicar
 Project-URL: Source, https://github.com/SETI/rms-vicar
 Project-URL: Issues, https://github.com/SETI/rms-vicar/issues
@@ -54,15 +54,15 @@
 [![Number of GitHub stars](https://img.shields.io/github/stars/SETI/rms-vicar)](https://github.com/SETI/rms-vicar/stargazers)
 ![GitHub forks](https://img.shields.io/github/forks/SETI/rms-vicar)
 
 # rms-vicar
 
 PDS Ring-Moon Systems Node, SETI Institute
 
-Supported versions: Python >= 3.7
+Supported versions: Python >= 3.8
 
 Classes and methods to read and write JPL's VICAR-format data files:
 
     VicarLabel      class for reading, writing, and parsing of VICAR labels.
     VicarImage      class for handling VICAR image (and other) data files.
     VicarError      extension of class ValueError to contain exceptions.
```

### Comparing `rms-vicar-1.0.4/rms_vicar.egg-info/SOURCES.txt` & `rms_vicar-1.0.5/rms_vicar.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 .coveragerc
 .flake8
 .gitignore
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/publish_to_pypi.yml
 .github/workflows/publish_to_test_pypi.yml
```

### Comparing `rms-vicar-1.0.4/test_files/C0532836239R.IMG` & `rms_vicar-1.0.5/test_files/C0532836239R.IMG`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/test_files/C2069302_GEOMA.DAT` & `rms_vicar-1.0.5/test_files/C2069302_GEOMA.DAT`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/test_files/C2069302_GEOMED.IMG` & `rms_vicar-1.0.5/test_files/C2069302_GEOMED.IMG`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/test_files/C2069302_RAW.IMG` & `rms_vicar-1.0.5/test_files/C2069302_RAW.IMG`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/test_files/C2069302_RESLOC.DAT` & `rms_vicar-1.0.5/test_files/C2069302_RESLOC.DAT`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/test_files/N1536633072_1_CALIB.IMG` & `rms_vicar-1.0.5/test_files/N1536633072_1_CALIB.IMG`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/tests/__init__.py` & `rms_vicar-1.0.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/tests/test_LABEL_GRAMMAR.py` & `rms_vicar-1.0.5/tests/test_LABEL_GRAMMAR.py`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/tests/test_vicarimage.py` & `rms_vicar-1.0.5/tests/test_vicarimage.py`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/tests/test_vicarlabel.py` & `rms_vicar-1.0.5/tests/test_vicarlabel.py`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/vicar/_LABEL_GRAMMAR.py` & `rms_vicar-1.0.5/vicar/_LABEL_GRAMMAR.py`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/vicar/__init__.py` & `rms_vicar-1.0.5/vicar/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/vicar/vicarimage.py` & `rms_vicar-1.0.5/vicar/vicarimage.py`

 * *Files identical despite different names*

### Comparing `rms-vicar-1.0.4/vicar/vicarlabel.py` & `rms_vicar-1.0.5/vicar/vicarlabel.py`

 * *Files identical despite different names*

