# Comparing `tmp/tempit-0.1.5.tar.gz` & `tmp/tempit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempit-0.1.5.tar", last modified: Mon May 13 16:41:37 2024, max compression
+gzip compressed data, was "tempit-0.1.6.tar", last modified: Tue May 14 09:52:36 2024, max compression
```

## Comparing `tempit-0.1.5.tar` & `tempit-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.622376 tempit-0.1.5/
--rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     7236 2024-05-13 16:41:37.621372 tempit-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6577 2024-05-13 16:35:58.000000 tempit-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 16:41:37.622376 tempit-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-13 14:57:01.000000 tempit-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.602375 tempit-0.1.5/tempit/
--rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.5/tempit/__init__.py
--rw-rw-rw-   0        0        0    11238 2024-05-13 16:16:07.000000 tempit-0.1.5/tempit/core.py
--rw-rw-rw-   0        0        0     5498 2024-05-10 06:26:45.000000 tempit-0.1.5/tempit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.618377 tempit-0.1.5/tempit.egg-info/
--rw-rw-rw-   0        0        0     7236 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 16:41:37.000000 tempit-0.1.5/tempit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 16:41:37.616373 tempit-0.1.5/tests/
--rw-rw-rw-   0        0        0    12928 2024-05-13 16:32:13.000000 tempit-0.1.5/tests/test_tempit.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:52:36.886048 tempit-0.1.6/
+-rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     7657 2024-05-14 09:52:36.885044 tempit-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7002 2024-05-14 09:50:44.000000 tempit-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 09:52:36.887048 tempit-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-14 07:35:54.000000 tempit-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:52:36.870047 tempit-0.1.6/tempit/
+-rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.6/tempit/__init__.py
+-rw-rw-rw-   0        0        0    11238 2024-05-13 16:16:07.000000 tempit-0.1.6/tempit/core.py
+-rw-rw-rw-   0        0        0     5498 2024-05-10 06:26:45.000000 tempit-0.1.6/tempit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 09:52:36.883046 tempit-0.1.6/tempit.egg-info/
+-rw-rw-rw-   0        0        0     7657 2024-05-14 09:52:36.000000 tempit-0.1.6/tempit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-14 09:52:36.000000 tempit-0.1.6/tempit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 09:52:36.000000 tempit-0.1.6/tempit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-14 09:52:36.000000 tempit-0.1.6/tempit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-14 09:52:36.000000 tempit-0.1.6/tempit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 09:52:36.881076 tempit-0.1.6/tests/
+-rw-rw-rw-   0        0        0    12853 2024-05-14 06:44:50.000000 tempit-0.1.6/tests/test_tempit.py
```

### Comparing `tempit-0.1.5/LICENSE.txt` & `tempit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tempit-0.1.5/PKG-INFO` & `tempit-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.5
+Version: 0.1.6
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 Requires-Dist: joblib==1.4.2
 
+
 # Tempit
 
+![PyPI](https://img.shields.io/pypi/v/tempit?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tempit)
+
+## Overview
+
 Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
 
 ## Installation
 
 You can install Tempit using pip:
 
 ```bash
 pip install tempit
 ```
 
 ## Usage
 
+Tempit decorator should only be used for benchmarking; it is not intended for production code.
+
 Below are some examples demonstrating Tempit's usage:
 
 ### Basic Usage
 
 ```python
 from tempit import tempit
 
@@ -77,15 +85,15 @@
         Max: 1.0000Âµs
         Standard deviation: 0.2828Âµs
         Sum time: 3.5000Âµs
         Real time: 965.1000Âµs
 ***** End of tempit data. *****
 ```
 
-More examples can be found in the [examples.py](examples/examples.py) script.
+More examples can be found in the [examples.py](https://github.com/mcrespoae/tempit/blob/main/tests/test_tempit.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
 - Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
@@ -166,20 +174,20 @@
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
 3. Create a new branch for your changes.
 4. Implement your changes and commit them.
 5. Push your changes to your forked repository.
 6. Submit a pull request.
 
-You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](Makefile) to know more about commands.
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/tempit/blob/main/Makefile) to know more about commands.
 
 ## Testing
 
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](tests).
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/tempit/tree/main/tests).
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE.txt).
+This project is licensed under the [MIT License](https://github.com/mcrespoae/tempit/blob/main/LICENSE).
 
 ## Contributors
 
 - [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `tempit-0.1.5/README.md` & `tempit-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+
 # Tempit
 
+![PyPI](https://img.shields.io/pypi/v/tempit?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tempit)
+
+## Overview
+
 Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
 
 ## Installation
 
 You can install Tempit using pip:
 
 ```bash
 pip install tempit
 ```
 
 ## Usage
 
+Tempit decorator should only be used for benchmarking; it is not intended for production code.
+
 Below are some examples demonstrating Tempit's usage:
 
 ### Basic Usage
 
 ```python
 from tempit import tempit
 
@@ -59,15 +67,15 @@
         Max: 1.0000µs
         Standard deviation: 0.2828µs
         Sum time: 3.5000µs
         Real time: 965.1000µs
 ***** End of tempit data. *****
 ```
 
-More examples can be found in the [examples.py](examples/examples.py) script.
+More examples can be found in the [examples.py](https://github.com/mcrespoae/tempit/blob/main/tests/test_tempit.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
 - Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
@@ -148,20 +156,20 @@
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
 3. Create a new branch for your changes.
 4. Implement your changes and commit them.
 5. Push your changes to your forked repository.
 6. Submit a pull request.
 
-You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](Makefile) to know more about commands.
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/tempit/blob/main/Makefile) to know more about commands.
 
 ## Testing
 
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](tests).
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/tempit/tree/main/tests).
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE.txt).
+This project is licensed under the [MIT License](https://github.com/mcrespoae/tempit/blob/main/LICENSE).
 
 ## Contributors
 
 - [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `tempit-0.1.5/setup.py` & `tempit-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 setup(
     name="tempit",
     version=VERSION,
     author="mcrespoae",
     author_email="info@mariocrespo.es",
     packages=["tempit"],
     description="A dead simple time decorator",
```

### Comparing `tempit-0.1.5/tempit/core.py` & `tempit-0.1.6/tempit/core.py`

 * *Files identical despite different names*

### Comparing `tempit-0.1.5/tempit/utils.py` & `tempit-0.1.6/tempit/utils.py`

 * *Files identical despite different names*

### Comparing `tempit-0.1.5/tempit.egg-info/PKG-INFO` & `tempit-0.1.6/tempit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.5
+Version: 0.1.6
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 Requires-Dist: joblib==1.4.2
 
+
 # Tempit
 
+![PyPI](https://img.shields.io/pypi/v/tempit?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/tempit)
+
+## Overview
+
 Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
 
 ## Installation
 
 You can install Tempit using pip:
 
 ```bash
 pip install tempit
 ```
 
 ## Usage
 
+Tempit decorator should only be used for benchmarking; it is not intended for production code.
+
 Below are some examples demonstrating Tempit's usage:
 
 ### Basic Usage
 
 ```python
 from tempit import tempit
 
@@ -77,15 +85,15 @@
         Max: 1.0000Âµs
         Standard deviation: 0.2828Âµs
         Sum time: 3.5000Âµs
         Real time: 965.1000Âµs
 ***** End of tempit data. *****
 ```
 
-More examples can be found in the [examples.py](examples/examples.py) script.
+More examples can be found in the [examples.py](https://github.com/mcrespoae/tempit/blob/main/tests/test_tempit.py) script.
 
 ## Features
 
 - Simplified usage.
 - Accurate measurement of function execution time.
 - Support for functions, methods, `classmethod`, `staticmethods` and classes.
 - Parallel execution mode for performance measurement.
@@ -166,20 +174,20 @@
 1. Fork the repository.
 2. Use `make install` to install all depedencies.
 3. Create a new branch for your changes.
 4. Implement your changes and commit them.
 5. Push your changes to your forked repository.
 6. Submit a pull request.
 
-You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](Makefile) to know more about commands.
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](https://github.com/mcrespoae/tempit/blob/main/Makefile) to know more about commands.
 
 ## Testing
 
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](tests).
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](https://github.com/mcrespoae/tempit/tree/main/tests).
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE.txt).
+This project is licensed under the [MIT License](https://github.com/mcrespoae/tempit/blob/main/LICENSE).
 
 ## Contributors
 
 - [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `tempit-0.1.5/tests/test_tempit.py` & `tempit-0.1.6/tests/test_tempit.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,14 @@
         execution_time_concurrent = end_time - start_time
 
         start_time = time.perf_counter()
         result_sequential = my_sequential_function(20_000_000, n=16)
         end_time = time.perf_counter()
         execution_time_sequential = end_time - start_time
 
-        # self.assertGreaterEqual(execution_time_sequential, lower_bound)
         self.assertLessEqual(
             execution_time_concurrent, (execution_time_sequential / 3) + (execution_time_sequential * 0.2)
         )
 
         self.assertEqual(result_concurrent, 987)
         self.assertEqual(result_sequential, 987)
```

