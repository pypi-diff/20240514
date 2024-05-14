# Comparing `tmp/pytest-retry-1.6.2.tar.gz` & `tmp/pytest_retry-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-retry-1.6.2.tar", last modified: Sun Feb  4 22:21:28 2024, max compression
+gzip compressed data, was "pytest_retry-1.6.3.tar", last modified: Tue May 14 03:56:20 2024, max compression
```

## Comparing `pytest-retry-1.6.2.tar` & `pytest_retry-1.6.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-02-04 22:21:28.433576 pytest-retry-1.6.2/
--rw-r--r--   0 silasj     (501) staff       (20)      113 2023-06-07 21:09:24.000000 pytest-retry-1.6.2/.gitignore
--rw-r--r--   0 silasj     (501) staff       (20)     1062 2023-06-07 21:09:24.000000 pytest-retry-1.6.2/LICENSE
--rw-r--r--   0 silasj     (501) staff       (20)       94 2023-06-07 21:09:24.000000 pytest-retry-1.6.2/MANIFEST.in
--rw-r--r--   0 silasj     (501) staff       (20)    10857 2024-02-04 22:21:28.433446 pytest-retry-1.6.2/PKG-INFO
--rw-r--r--   0 silasj     (501) staff       (20)     8716 2023-12-31 19:53:06.000000 pytest-retry-1.6.2/README.md
--rw-r--r--   0 silasj     (501) staff       (20)       68 2023-06-07 21:09:24.000000 pytest-retry-1.6.2/dev-requirements.txt
--rw-r--r--   0 silasj     (501) staff       (20)     1220 2024-02-04 22:13:29.000000 pytest-retry-1.6.2/pyproject.toml
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-02-04 22:21:28.431331 pytest-retry-1.6.2/pytest_retry/
--rw-r--r--   0 silasj     (501) staff       (20)      125 2023-06-07 21:09:24.000000 pytest-retry-1.6.2/pytest_retry/__init__.py
--rw-r--r--   0 silasj     (501) staff       (20)     1751 2023-10-04 18:03:36.000000 pytest-retry-1.6.2/pytest_retry/configs.py
--rw-r--r--   0 silasj     (501) staff       (20)     1187 2023-07-31 08:07:21.000000 pytest-retry-1.6.2/pytest_retry/hooks.py
--rw-r--r--   0 silasj     (501) staff       (20)        0 2023-06-07 21:09:24.000000 pytest-retry-1.6.2/pytest_retry/py.typed
--rw-r--r--   0 silasj     (501) staff       (20)    14323 2024-02-04 22:13:29.000000 pytest-retry-1.6.2/pytest_retry/retry_plugin.py
--rw-r--r--   0 silasj     (501) staff       (20)     1926 2024-01-04 20:58:29.000000 pytest-retry-1.6.2/pytest_retry/server.py
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-02-04 22:21:28.432980 pytest-retry-1.6.2/pytest_retry.egg-info/
--rw-r--r--   0 silasj     (501) staff       (20)    10857 2024-02-04 22:21:28.000000 pytest-retry-1.6.2/pytest_retry.egg-info/PKG-INFO
--rw-r--r--   0 silasj     (501) staff       (20)      536 2024-02-04 22:21:28.000000 pytest-retry-1.6.2/pytest_retry.egg-info/SOURCES.txt
--rw-r--r--   0 silasj     (501) staff       (20)        1 2024-02-04 22:21:28.000000 pytest-retry-1.6.2/pytest_retry.egg-info/dependency_links.txt
--rw-r--r--   0 silasj     (501) staff       (20)       52 2024-02-04 22:21:28.000000 pytest-retry-1.6.2/pytest_retry.egg-info/entry_points.txt
--rw-r--r--   0 silasj     (501) staff       (20)        1 2024-02-04 22:21:28.000000 pytest-retry-1.6.2/pytest_retry.egg-info/not-zip-safe
--rw-r--r--   0 silasj     (501) staff       (20)       45 2024-02-04 22:21:28.000000 pytest-retry-1.6.2/pytest_retry.egg-info/requires.txt
--rw-r--r--   0 silasj     (501) staff       (20)       13 2024-02-04 22:21:28.000000 pytest-retry-1.6.2/pytest_retry.egg-info/top_level.txt
--rw-r--r--   0 silasj     (501) staff       (20)       40 2023-12-31 19:53:06.000000 pytest-retry-1.6.2/requirements.txt
--rw-r--r--   0 silasj     (501) staff       (20)      301 2024-02-04 22:21:28.433827 pytest-retry-1.6.2/setup.cfg
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-02-04 22:21:28.432553 pytest-retry-1.6.2/tests/
--rw-r--r--   0 silasj     (501) staff       (20)    23527 2024-02-04 22:13:29.000000 pytest-retry-1.6.2/tests/test_retry_plugin.py
--rw-r--r--   0 silasj     (501) staff       (20)      554 2023-10-04 18:03:36.000000 pytest-retry-1.6.2/tox.ini
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-05-14 03:56:20.110192 pytest_retry-1.6.3/
+-rw-r--r--   0 silasj     (501) staff       (20)      113 2023-06-07 21:09:24.000000 pytest_retry-1.6.3/.gitignore
+-rw-r--r--   0 silasj     (501) staff       (20)     1062 2023-06-07 21:09:24.000000 pytest_retry-1.6.3/LICENSE
+-rw-r--r--   0 silasj     (501) staff       (20)       94 2023-06-07 21:09:24.000000 pytest_retry-1.6.3/MANIFEST.in
+-rw-r--r--   0 silasj     (501) staff       (20)    10892 2024-05-14 03:56:20.110020 pytest_retry-1.6.3/PKG-INFO
+-rw-r--r--   0 silasj     (501) staff       (20)     8751 2024-05-12 23:24:30.000000 pytest_retry-1.6.3/README.md
+-rw-r--r--   0 silasj     (501) staff       (20)       68 2023-06-07 21:09:24.000000 pytest_retry-1.6.3/dev-requirements.txt
+-rw-r--r--   0 silasj     (501) staff       (20)     1220 2024-05-14 03:50:19.000000 pytest_retry-1.6.3/pyproject.toml
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-05-14 03:56:20.107758 pytest_retry-1.6.3/pytest_retry/
+-rw-r--r--   0 silasj     (501) staff       (20)      125 2023-06-07 21:09:24.000000 pytest_retry-1.6.3/pytest_retry/__init__.py
+-rw-r--r--   0 silasj     (501) staff       (20)     1751 2023-10-04 18:03:36.000000 pytest_retry-1.6.3/pytest_retry/configs.py
+-rw-r--r--   0 silasj     (501) staff       (20)     1187 2023-07-31 08:07:21.000000 pytest_retry-1.6.3/pytest_retry/hooks.py
+-rw-r--r--   0 silasj     (501) staff       (20)        0 2023-06-07 21:09:24.000000 pytest_retry-1.6.3/pytest_retry/py.typed
+-rw-r--r--   0 silasj     (501) staff       (20)    14377 2024-05-14 03:45:11.000000 pytest_retry-1.6.3/pytest_retry/retry_plugin.py
+-rw-r--r--   0 silasj     (501) staff       (20)     1926 2024-01-04 20:58:29.000000 pytest_retry-1.6.3/pytest_retry/server.py
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-05-14 03:56:20.109514 pytest_retry-1.6.3/pytest_retry.egg-info/
+-rw-r--r--   0 silasj     (501) staff       (20)    10892 2024-05-14 03:56:20.000000 pytest_retry-1.6.3/pytest_retry.egg-info/PKG-INFO
+-rw-r--r--   0 silasj     (501) staff       (20)      536 2024-05-14 03:56:20.000000 pytest_retry-1.6.3/pytest_retry.egg-info/SOURCES.txt
+-rw-r--r--   0 silasj     (501) staff       (20)        1 2024-05-14 03:56:20.000000 pytest_retry-1.6.3/pytest_retry.egg-info/dependency_links.txt
+-rw-r--r--   0 silasj     (501) staff       (20)       52 2024-05-14 03:56:20.000000 pytest_retry-1.6.3/pytest_retry.egg-info/entry_points.txt
+-rw-r--r--   0 silasj     (501) staff       (20)        1 2024-05-14 03:56:19.000000 pytest_retry-1.6.3/pytest_retry.egg-info/not-zip-safe
+-rw-r--r--   0 silasj     (501) staff       (20)       45 2024-05-14 03:56:20.000000 pytest_retry-1.6.3/pytest_retry.egg-info/requires.txt
+-rw-r--r--   0 silasj     (501) staff       (20)       13 2024-05-14 03:56:20.000000 pytest_retry-1.6.3/pytest_retry.egg-info/top_level.txt
+-rw-r--r--   0 silasj     (501) staff       (20)       40 2023-12-31 19:53:06.000000 pytest_retry-1.6.3/requirements.txt
+-rw-r--r--   0 silasj     (501) staff       (20)      301 2024-05-14 03:56:20.110467 pytest_retry-1.6.3/setup.cfg
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2024-05-14 03:56:20.109003 pytest_retry-1.6.3/tests/
+-rw-r--r--   0 silasj     (501) staff       (20)    24029 2024-05-14 03:45:11.000000 pytest_retry-1.6.3/tests/test_retry_plugin.py
+-rw-r--r--   0 silasj     (501) staff       (20)      554 2023-10-04 18:03:36.000000 pytest_retry-1.6.3/tox.ini
```

### Comparing `pytest-retry-1.6.2/LICENSE` & `pytest_retry-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-retry-1.6.2/PKG-INFO` & `pytest_retry-1.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-retry
-Version: 1.6.2
+Version: 1.6.3
 Summary: Adds the ability to retry flaky tests in CI environments
 Author: str0zzapreti
 License: MIT License
         
         Copyright (c) 2022 Silas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,108 +55,108 @@
 
 pytest-retry is designed for the latest versions of Python and Pytest. Python 3.9+
 and pytest 7.0.0+ are required. 
 
 ## Installation
 
 Use pip to install pytest-retry:
-```
+```bash
 $ pip install pytest-retry
 ```
 
 ## Usage
 
 There are two main ways to use pytest-retry:
 
 ### 1. Global settings
 
 Once installed, pytest-retry adds new command line and ini config options for pytest.
 Run Pytest with the command line argument --retries in order to retry every test in 
 the event of a failure. The following example will retry each failed up to two times
 before proceeding to the next test:
 
-```
+```bash
 $ python -m pytest --retries 2
 ```
 
 An optional delay can be specified using the --retry-delay argument. This will insert
 a fixed delay (in seconds) between each attempt when a test fails. This can be useful
 if the test failures are due to intermittent environment issues which clear up after
 a few seconds
 
-```
+```bash
 $ python -m pytest --retries 2 --retry-delay 5
 ```
 
 #### Advanced Options:
 There are two custom hooks provided for the purpose of setting global exception
 filters for your entire Pytest suite. `pytest_set_filtered_exceptions`
 and `pytest_set_excluded_exceptions`. You can define either of them in your 
 conftest.py file and return a list of exception types. Note: these hooks are 
 mutually exclusive and cannot both be defined at the same time.
 
 Example:
-```
+```py
 def pytest_set_excluded_exceptions():
     """
     All tests will be retried unless they fail due to an AssertionError or CustomError
     """
     return [AssertionError, CustomError]
 ```
 
 There is a command line option to specify the test timing method, which can either
 be `overwrite` (default) or `cumulative`. With cumulative timing, the duration of 
 each test attempt is summed for the reported overall test duration. The default
 behavior simply reports the timing of the final attempt.
 
-```
+```bash
 $ python -m pytest --retries 2 --cumulative-timing 1
 ```
 
 If you're not sure which to use, stick with the default `overwrite` method. This
 generally plays nicer with time-based test splitting algorithms and will result in
 more even splits.
 
 Instead of command line arguments, you can set any of these config options in your
 pytest.ini, tox.ini, or pyproject.toml file. Any command line arguments will take
 precedence over options specified in one of these config files. Here are some
 sample configs that you can copy into your project to get started:
 
 _pyproject.toml_
-```
+```toml
 [tool.pytest.ini_options]
 retries = 2
 retry_delay = 0.5
 cumulative_timing = false
 ```
 
 _config.ini/tox.ini_
-```
+```ini
 [pytest]
 retries = 2
 retry_delay = 0.5
 cumulative_timing = false
 ```
 
 ### 2. Pytest flaky mark
 
 Mark individual tests as 'flaky' to retry them when they fail. If no command line
 arguments are passed, only the marked tests will be retried. The default values
 are 1 retry attempt with a 0-second delay
 
-```
+```py
 @pytest.mark.flaky
 def test_unreliable_service():
     ...
 ```
 
 The number of times each test will be retried and/or the delay can be manually
 specified as well
 
-```
+```py
 @pytest.mark.flaky(retries=3, delay=1)
 def test_unreliable_service():
     # This test will be retried up to 3 times (4 attempts total) with a
     # one second delay between each attempt
     ...
 ```
 
@@ -169,39 +169,39 @@
 one of the listed exceptions. A test with a list of `exclude` exceptions will
 only be retried if it fails with an exception which does not match any of the
 listed exceptions.
 
 If the exception for a subsequent attempt changes and no longer matches the filter,
 no further attempts will be made and the test will immediately fail.
 
-```
+```py
 @pytest.mark.flaky(retries=2, only_on=[ValueError, IndexError])
 def test_unreliable_service():
     # This test will only be retried if it fails due to raising a ValueError
     # or an IndexError. e.g., an AssertionError will fail without retrying
     ...
 ```
 
 If you want some other generalized condition to control whether a test is retried, use the
 `condition` argument. Any statement which results in a bool can be used here to add granularity
 to your retries. The test will only be retried if `condition` is `True`. Note, there is no
 matching command line option for `condition`, but if you need to globally apply this type of logic
 to all of your tests, consider invoking the `pytest_collection_modifyitems` hook.
 
-```
+```py
 @pytest.mark.flaky(retries=2, condition=sys.platform.startswith('win32'))
 def test_only_flaky_on_some_systems():
     # This test will only be retried if sys.platform.startswith('win32') evaluates to `True`
 ```
 
 Finally, there is a flaky mark argument for the test timing method, which can either
 be `overwrite` (default) or `cumulative`. See **Command Line** > **Advanced Options** 
 for more information
 
-```
+```py
 @pytest.mark.flaky(timing='overwrite')
 def test_unreliable_service():
     ...
 ```
 
 A flaky mark will override any command line options and exception filter hooks
 specified when running Pytest.
```

### Comparing `pytest-retry-1.6.2/README.md` & `pytest_retry-1.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,108 +8,108 @@
 
 pytest-retry is designed for the latest versions of Python and Pytest. Python 3.9+
 and pytest 7.0.0+ are required. 
 
 ## Installation
 
 Use pip to install pytest-retry:
-```
+```bash
 $ pip install pytest-retry
 ```
 
 ## Usage
 
 There are two main ways to use pytest-retry:
 
 ### 1. Global settings
 
 Once installed, pytest-retry adds new command line and ini config options for pytest.
 Run Pytest with the command line argument --retries in order to retry every test in 
 the event of a failure. The following example will retry each failed up to two times
 before proceeding to the next test:
 
-```
+```bash
 $ python -m pytest --retries 2
 ```
 
 An optional delay can be specified using the --retry-delay argument. This will insert
 a fixed delay (in seconds) between each attempt when a test fails. This can be useful
 if the test failures are due to intermittent environment issues which clear up after
 a few seconds
 
-```
+```bash
 $ python -m pytest --retries 2 --retry-delay 5
 ```
 
 #### Advanced Options:
 There are two custom hooks provided for the purpose of setting global exception
 filters for your entire Pytest suite. `pytest_set_filtered_exceptions`
 and `pytest_set_excluded_exceptions`. You can define either of them in your 
 conftest.py file and return a list of exception types. Note: these hooks are 
 mutually exclusive and cannot both be defined at the same time.
 
 Example:
-```
+```py
 def pytest_set_excluded_exceptions():
     """
     All tests will be retried unless they fail due to an AssertionError or CustomError
     """
     return [AssertionError, CustomError]
 ```
 
 There is a command line option to specify the test timing method, which can either
 be `overwrite` (default) or `cumulative`. With cumulative timing, the duration of 
 each test attempt is summed for the reported overall test duration. The default
 behavior simply reports the timing of the final attempt.
 
-```
+```bash
 $ python -m pytest --retries 2 --cumulative-timing 1
 ```
 
 If you're not sure which to use, stick with the default `overwrite` method. This
 generally plays nicer with time-based test splitting algorithms and will result in
 more even splits.
 
 Instead of command line arguments, you can set any of these config options in your
 pytest.ini, tox.ini, or pyproject.toml file. Any command line arguments will take
 precedence over options specified in one of these config files. Here are some
 sample configs that you can copy into your project to get started:
 
 _pyproject.toml_
-```
+```toml
 [tool.pytest.ini_options]
 retries = 2
 retry_delay = 0.5
 cumulative_timing = false
 ```
 
 _config.ini/tox.ini_
-```
+```ini
 [pytest]
 retries = 2
 retry_delay = 0.5
 cumulative_timing = false
 ```
 
 ### 2. Pytest flaky mark
 
 Mark individual tests as 'flaky' to retry them when they fail. If no command line
 arguments are passed, only the marked tests will be retried. The default values
 are 1 retry attempt with a 0-second delay
 
-```
+```py
 @pytest.mark.flaky
 def test_unreliable_service():
     ...
 ```
 
 The number of times each test will be retried and/or the delay can be manually
 specified as well
 
-```
+```py
 @pytest.mark.flaky(retries=3, delay=1)
 def test_unreliable_service():
     # This test will be retried up to 3 times (4 attempts total) with a
     # one second delay between each attempt
     ...
 ```
 
@@ -122,39 +122,39 @@
 one of the listed exceptions. A test with a list of `exclude` exceptions will
 only be retried if it fails with an exception which does not match any of the
 listed exceptions.
 
 If the exception for a subsequent attempt changes and no longer matches the filter,
 no further attempts will be made and the test will immediately fail.
 
-```
+```py
 @pytest.mark.flaky(retries=2, only_on=[ValueError, IndexError])
 def test_unreliable_service():
     # This test will only be retried if it fails due to raising a ValueError
     # or an IndexError. e.g., an AssertionError will fail without retrying
     ...
 ```
 
 If you want some other generalized condition to control whether a test is retried, use the
 `condition` argument. Any statement which results in a bool can be used here to add granularity
 to your retries. The test will only be retried if `condition` is `True`. Note, there is no
 matching command line option for `condition`, but if you need to globally apply this type of logic
 to all of your tests, consider invoking the `pytest_collection_modifyitems` hook.
 
-```
+```py
 @pytest.mark.flaky(retries=2, condition=sys.platform.startswith('win32'))
 def test_only_flaky_on_some_systems():
     # This test will only be retried if sys.platform.startswith('win32') evaluates to `True`
 ```
 
 Finally, there is a flaky mark argument for the test timing method, which can either
 be `overwrite` (default) or `cumulative`. See **Command Line** > **Advanced Options** 
 for more information
 
-```
+```py
 @pytest.mark.flaky(timing='overwrite')
 def test_unreliable_service():
     ...
 ```
 
 A flaky mark will override any command line options and exception filter hooks
 specified when running Pytest.
```

### Comparing `pytest-retry-1.6.2/pyproject.toml` & `pytest_retry-1.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-retry"
-version = "1.6.2"
+version = "1.6.3"
 description = "Adds the ability to retry flaky tests in CI environments"
 readme = "README.md"
 authors = [{ name = "str0zzapreti" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `pytest-retry-1.6.2/pytest_retry/configs.py` & `pytest_retry-1.6.3/pytest_retry/configs.py`

 * *Files identical despite different names*

### Comparing `pytest-retry-1.6.2/pytest_retry/hooks.py` & `pytest_retry-1.6.3/pytest_retry/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest-retry-1.6.2/pytest_retry/retry_plugin.py` & `pytest_retry-1.6.3/pytest_retry/retry_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """
     Stores statistics and reports for flaky tests and fixtures which have
     failed at least once during the test session and need to be retried
     """
 
     def __init__(self) -> None:
         self.reporter: ReportHandler = OfflineReporter()
-        self.trace_limit: Optional[int] = -1
+        self.trace_limit: Optional[int] = 1
         self.node_stats: dict[str, dict] = {}
         self.messages = (
             " failed on attempt {attempt}! Retrying!\n\t",
             " failed after {attempt} attempts!\n\t",
             " teardown failed on attempt {attempt}! Exiting immediately!\n\t",
             " passed on attempt {attempt}!\n\t",
         )
@@ -294,17 +294,18 @@
         "markers",
         "flaky(retries=1, delay=0, only_on=..., exclude=..., condition=...): indicate a flaky "
         "test which will be retried the number of times specified with an (optional) specified "
         "delay between each attempt. Collections of one or more exceptions can be passed so "
         "that the test is retried only on those exceptions, or excluding those exceptions. "
         "Any statement which returns a bool can be used as a condition",
     )
-    if config.getoption("verbose"):
-        # if pytest config has -v enabled, then don't limit traceback length
-        retry_manager.trace_limit = None
+    verbosity = config.getoption("verbose")
+    if verbosity:
+        # set trace limit according to verbosity count, or unlimited if 5
+        retry_manager.trace_limit = verbosity if verbosity < 5 else None
     Defaults.configure(config)
     Defaults.add("FILTERED_EXCEPTIONS", config.hook.pytest_set_filtered_exceptions() or [])
     Defaults.add("EXCLUDED_EXCEPTIONS", config.hook.pytest_set_excluded_exceptions() or [])
     if config.pluginmanager.has_plugin("xdist") and config.getoption("numprocesses", False):
         config.pluginmanager.register(XdistHook())
         retry_manager.reporter = ReportServer()
         config.stash[server_port_key] = retry_manager.reporter.initialize_server()
```

### Comparing `pytest-retry-1.6.2/pytest_retry/server.py` & `pytest_retry-1.6.3/pytest_retry/server.py`

 * *Files identical despite different names*

### Comparing `pytest-retry-1.6.2/pytest_retry.egg-info/PKG-INFO` & `pytest_retry-1.6.3/pytest_retry.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-retry
-Version: 1.6.2
+Version: 1.6.3
 Summary: Adds the ability to retry flaky tests in CI environments
 Author: str0zzapreti
 License: MIT License
         
         Copyright (c) 2022 Silas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,108 +55,108 @@
 
 pytest-retry is designed for the latest versions of Python and Pytest. Python 3.9+
 and pytest 7.0.0+ are required. 
 
 ## Installation
 
 Use pip to install pytest-retry:
-```
+```bash
 $ pip install pytest-retry
 ```
 
 ## Usage
 
 There are two main ways to use pytest-retry:
 
 ### 1. Global settings
 
 Once installed, pytest-retry adds new command line and ini config options for pytest.
 Run Pytest with the command line argument --retries in order to retry every test in 
 the event of a failure. The following example will retry each failed up to two times
 before proceeding to the next test:
 
-```
+```bash
 $ python -m pytest --retries 2
 ```
 
 An optional delay can be specified using the --retry-delay argument. This will insert
 a fixed delay (in seconds) between each attempt when a test fails. This can be useful
 if the test failures are due to intermittent environment issues which clear up after
 a few seconds
 
-```
+```bash
 $ python -m pytest --retries 2 --retry-delay 5
 ```
 
 #### Advanced Options:
 There are two custom hooks provided for the purpose of setting global exception
 filters for your entire Pytest suite. `pytest_set_filtered_exceptions`
 and `pytest_set_excluded_exceptions`. You can define either of them in your 
 conftest.py file and return a list of exception types. Note: these hooks are 
 mutually exclusive and cannot both be defined at the same time.
 
 Example:
-```
+```py
 def pytest_set_excluded_exceptions():
     """
     All tests will be retried unless they fail due to an AssertionError or CustomError
     """
     return [AssertionError, CustomError]
 ```
 
 There is a command line option to specify the test timing method, which can either
 be `overwrite` (default) or `cumulative`. With cumulative timing, the duration of 
 each test attempt is summed for the reported overall test duration. The default
 behavior simply reports the timing of the final attempt.
 
-```
+```bash
 $ python -m pytest --retries 2 --cumulative-timing 1
 ```
 
 If you're not sure which to use, stick with the default `overwrite` method. This
 generally plays nicer with time-based test splitting algorithms and will result in
 more even splits.
 
 Instead of command line arguments, you can set any of these config options in your
 pytest.ini, tox.ini, or pyproject.toml file. Any command line arguments will take
 precedence over options specified in one of these config files. Here are some
 sample configs that you can copy into your project to get started:
 
 _pyproject.toml_
-```
+```toml
 [tool.pytest.ini_options]
 retries = 2
 retry_delay = 0.5
 cumulative_timing = false
 ```
 
 _config.ini/tox.ini_
-```
+```ini
 [pytest]
 retries = 2
 retry_delay = 0.5
 cumulative_timing = false
 ```
 
 ### 2. Pytest flaky mark
 
 Mark individual tests as 'flaky' to retry them when they fail. If no command line
 arguments are passed, only the marked tests will be retried. The default values
 are 1 retry attempt with a 0-second delay
 
-```
+```py
 @pytest.mark.flaky
 def test_unreliable_service():
     ...
 ```
 
 The number of times each test will be retried and/or the delay can be manually
 specified as well
 
-```
+```py
 @pytest.mark.flaky(retries=3, delay=1)
 def test_unreliable_service():
     # This test will be retried up to 3 times (4 attempts total) with a
     # one second delay between each attempt
     ...
 ```
 
@@ -169,39 +169,39 @@
 one of the listed exceptions. A test with a list of `exclude` exceptions will
 only be retried if it fails with an exception which does not match any of the
 listed exceptions.
 
 If the exception for a subsequent attempt changes and no longer matches the filter,
 no further attempts will be made and the test will immediately fail.
 
-```
+```py
 @pytest.mark.flaky(retries=2, only_on=[ValueError, IndexError])
 def test_unreliable_service():
     # This test will only be retried if it fails due to raising a ValueError
     # or an IndexError. e.g., an AssertionError will fail without retrying
     ...
 ```
 
 If you want some other generalized condition to control whether a test is retried, use the
 `condition` argument. Any statement which results in a bool can be used here to add granularity
 to your retries. The test will only be retried if `condition` is `True`. Note, there is no
 matching command line option for `condition`, but if you need to globally apply this type of logic
 to all of your tests, consider invoking the `pytest_collection_modifyitems` hook.
 
-```
+```py
 @pytest.mark.flaky(retries=2, condition=sys.platform.startswith('win32'))
 def test_only_flaky_on_some_systems():
     # This test will only be retried if sys.platform.startswith('win32') evaluates to `True`
 ```
 
 Finally, there is a flaky mark argument for the test timing method, which can either
 be `overwrite` (default) or `cumulative`. See **Command Line** > **Advanced Options** 
 for more information
 
-```
+```py
 @pytest.mark.flaky(timing='overwrite')
 def test_unreliable_service():
     ...
 ```
 
 A flaky mark will override any command line options and exception filter hooks
 specified when running Pytest.
```

### Comparing `pytest-retry-1.6.2/pytest_retry.egg-info/SOURCES.txt` & `pytest_retry-1.6.3/pytest_retry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-retry-1.6.2/tests/test_retry_plugin.py` & `pytest_retry-1.6.3/tests/test_retry_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -920,14 +920,30 @@
         """
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=2, failed=1, retried=2)
 
 
+@mark.parametrize('verbosity', ['vv', 'vvv', 'vvvv'])
+def test_stack_trace_depth_uses_verbosity_count(testdir, verbosity):
+    testdir.makepyfile(
+        """
+        a = []
+        def test_eventually_passes():
+            a.append(1)
+            assert len(a) > 1
+        """
+    )
+    result = testdir.runpytest("--retries", "1", f"-{verbosity}")
+
+    assert_outcomes(result, passed=1, retried=1)
+    assert len([line for line in result.outlines if line.startswith('\t  File')]) == len(verbosity)
+
+
 @mark.skipif(xdist_installed is False, reason="Only run if xdist is installed locally")
 def test_xdist_reporting_compatability(testdir):
     testdir.makepyfile(
         """
         import pytest
 
         a = 0
```

### Comparing `pytest-retry-1.6.2/tox.ini` & `pytest_retry-1.6.3/tox.ini`

 * *Files identical despite different names*

