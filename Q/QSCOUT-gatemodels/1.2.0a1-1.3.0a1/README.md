# Comparing `tmp/QSCOUT-gatemodels-1.2.0a1.tar.gz` & `tmp/qscout_gatemodels-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/build-jaqal/qscout-gatemodels/dist/.tmp-tiobknl0/QSCOUT-gatemodels-1.2.0a1.tar", last modified: Fri May 19 23:36:28 2023, max compression
+gzip compressed data, was "qscout_gatemodels-1.3.0a1.tar", last modified: Tue May 14 11:02:07 2024, max compression
```

## Comparing `QSCOUT-gatemodels-1.2.0a1.tar` & `qscout_gatemodels-1.3.0a1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      197 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     2156 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1333 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/README.md
--rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1169 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2156 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      599 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/
--rw-rw-r--   0 root         (0) root         (0)     3205 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/jaqal_action.py
--rw-rw-r--   0 root         (0) root         (0)     2740 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/jaqal_gates.py
--rw-rw-r--   0 root         (0) root         (0)     5076 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/noisy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/stretched/
--rw-rw-r--   0 root         (0) root         (0)      167 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/stretched/jaqal_action.py
--rw-rw-r--   0 root         (0) root         (0)      890 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/stretched/jaqal_gates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/zz/
--rw-rw-r--   0 root         (0) root         (0)      781 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/zz/jaqal_action.py
--rw-rw-r--   0 root         (0) root         (0)      762 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/zz/jaqal_gates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:28.000000 QSCOUT-gatemodels-1.2.0a1/tests/parser/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/tests/parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8190 2023-05-19 20:38:38.000000 QSCOUT-gatemodels-1.2.0a1/tests/parser/test_jaqalpup_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1333 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/README.md
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-05-14 11:02:07.289428 qscout_gatemodels-1.3.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.281428 qscout_gatemodels-1.3.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-14 11:02:07.000000 qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-14 11:02:07.000000 qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 11:02:07.000000 qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-14 11:02:07.000000 qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-14 11:02:07.000000 qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.281428 qscout_gatemodels-1.3.0a1/src/qscout/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.281428 qscout_gatemodels-1.3.0a1/src/qscout/v1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/src/qscout/v1/std/
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/src/qscout/v1/std/jaqal_action.py
+-rw-r--r--   0 root         (0) root         (0)     4198 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/src/qscout/v1/std/jaqal_gates.py
+-rw-r--r--   0 root         (0) root         (0)     8539 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/src/qscout/v1/std/noisy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/src/qscout/v1/std/stretched/
+-rw-r--r--   0 root         (0) root         (0)      167 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/src/qscout/v1/std/stretched/jaqal_action.py
+-rw-r--r--   0 root         (0) root         (0)      890 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/src/qscout/v1/std/stretched/jaqal_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/src/qscout/v1/zz/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/src/qscout/v1/zz/jaqal_action.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/src/qscout/v1/zz/jaqal_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:02:07.285428 qscout_gatemodels-1.3.0a1/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/tests/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8190 2024-05-14 11:01:41.000000 qscout_gatemodels-1.3.0a1/tests/parser/test_jaqalpup_parser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `QSCOUT-gatemodels-1.2.0a1/LICENSE` & `qscout_gatemodels-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `QSCOUT-gatemodels-1.2.0a1/PKG-INFO` & `qscout_gatemodels-1.3.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QSCOUT-gatemodels
-Version: 1.2.0a1
+Version: 1.3.0a1
 Summary: QSCOUT Gate Models
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,17 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: JaqalPaq>=1.3.0a1
+Requires-Dist: numpy
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 
 QSCOUT Gate Models
 ------------------
 
 The [Quantum Scientific Computing Open User Testbed
 (QSCOUT)](https://qscout.sandia.gov/) is a five-year DOE program to build a
 quantum testbed based on trapped ions that is available to the research
```

### Comparing `QSCOUT-gatemodels-1.2.0a1/README.md` & `qscout_gatemodels-1.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `QSCOUT-gatemodels-1.2.0a1/setup.cfg` & `qscout_gatemodels-1.3.0a1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = QSCOUT-gatemodels
 author = Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 author_email = qscout@sandia.gov
 description = QSCOUT Gate Models
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache
-version = 1.2.0a1
+version = 1.3.0a1
 home_page = https://qscout.sandia.gov
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
@@ -18,15 +18,15 @@
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Unix
 
 [options]
 packages = find_namespace:
 package_dir = 
 	=src
-install_requires = JaqalPaq>=1.2.0a1; numpy
+install_requires = JaqalPaq>=1.3.0a1; numpy
 python_requires = >=3.6.5
 platforms = any
 
 [options.packages.find]
 include = 
 	qscout
 	qscout.*
```

### Comparing `QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/PKG-INFO` & `qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QSCOUT-gatemodels
-Version: 1.2.0a1
+Version: 1.3.0a1
 Summary: QSCOUT Gate Models
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,17 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: JaqalPaq>=1.3.0a1
+Requires-Dist: numpy
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 
 QSCOUT Gate Models
 ------------------
 
 The [Quantum Scientific Computing Open User Testbed
 (QSCOUT)](https://qscout.sandia.gov/) is a five-year DOE program to build a
 quantum testbed based on trapped ions that is available to the research
```

### Comparing `QSCOUT-gatemodels-1.2.0a1/src/QSCOUT_gatemodels.egg-info/SOURCES.txt` & `qscout_gatemodels-1.3.0a1/src/QSCOUT_gatemodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QSCOUT-gatemodels-1.2.0a1/src/qscout/v1/std/stretched/jaqal_gates.py` & `qscout_gatemodels-1.3.0a1/src/qscout/v1/std/stretched/jaqal_gates.py`

 * *Files identical despite different names*

### Comparing `QSCOUT-gatemodels-1.2.0a1/tests/parser/test_jaqalpup_parser.py` & `qscout_gatemodels-1.3.0a1/tests/parser/test_jaqalpup_parser.py`

 * *Files identical despite different names*

