# Comparing `tmp/frequenz-client-base-0.3.0.tar.gz` & `tmp/frequenz-client-base-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-client-base-0.3.0.tar", last modified: Mon Mar 11 11:35:28 2024, max compression
+gzip compressed data, was "frequenz-client-base-0.4.0.tar", last modified: Tue May 14 13:46:18 2024, max compression
```

## Comparing `frequenz-client-base-0.3.0.tar` & `frequenz-client-base-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/src/frequenz/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/src/frequenz/client/base/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/src/frequenz/client/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/src/frequenz/client/base/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/src/frequenz/client/base/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/src/frequenz/client/base/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/src/frequenz/client/base/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-11 11:35:20.000000 frequenz-client-base-0.3.0/src/frequenz/client/base/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 11:35:28.519207 frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-11 11:35:28.000000 frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-11 11:35:28.000000 frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 11:35:28.000000 frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-11 11:35:28.000000 frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 11:35:28.000000 frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:46:18.885347 frequenz-client-base-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-14 13:46:18.885347 frequenz-client-base-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:46:18.885347 frequenz-client-base-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:46:18.881348 frequenz-client-base-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:46:18.881348 frequenz-client-base-0.4.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:46:18.881348 frequenz-client-base-0.4.0/src/frequenz/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:46:18.885347 frequenz-client-base-0.4.0/src/frequenz/client/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/_grpchacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-14 13:46:08.000000 frequenz-client-base-0.4.0/src/frequenz/client/base/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:46:18.885347 frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-14 13:46:18.000000 frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-14 13:46:18.000000 frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:46:18.000000 frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-14 13:46:18.000000 frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 13:46:18.000000 frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/top_level.txt
```

### Comparing `frequenz-client-base-0.3.0/LICENSE` & `frequenz-client-base-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-client-base-0.3.0/PKG-INFO` & `frequenz-client-base-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-base
-Version: 0.3.0
+Version: 0.4.0
 Summary: Utilities for writing Frequenz API clients
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-base-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-base-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-base-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-base-python
@@ -15,14 +15,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: grpcio
+Provides-Extra: grpclib
 Provides-Extra: dev-flake8
 Provides-Extra: dev-formatting
 Provides-Extra: dev-mkdocs
 Provides-Extra: dev-mypy
 Provides-Extra: dev-noxfile
 Provides-Extra: dev-pylint
 Provides-Extra: dev-pytest
```

### Comparing `frequenz-client-base-0.3.0/README.md` & `frequenz-client-base-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-client-base-0.3.0/pyproject.toml` & `frequenz-client-base-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
 requires = [
   "setuptools == 68.1.0",
   "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[lib] == 0.9.1",
+  "frequenz-repo-config[lib] == 0.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-client-base"
 description = "Utilities for writing Frequenz API clients"
 readme = "README.md"
 license = { text = "MIT" }
 keywords = ["frequenz", "python", "lib", "library", "client-base"]
-# TODO(cookiecutter): Remove and add more classifiers if appropriate
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
-# TODO(cookiecutter): Remove and add more dependencies if appropriate
 dependencies = [
   "frequenz-channels >= v1.0.0-rc1, < 2",
-  "grpcio >= 1.54.2, < 2",
-  "protobuf >= 4.21.6, < 5",
+  "protobuf >= 4.21.6, < 6",
   "typing-extensions >= 4.5.0, < 5",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
-# TODO(cookiecutter): Remove and add more optional dependencies if appropriate
 [project.optional-dependencies]
+grpcio = ["grpcio >= 1.54.2, < 2"]
+grpclib = ["grpclib >= 0.4.0, < 0.5"]
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
-  "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
+  "flake8-pyproject == 1.2.3",            # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
+  "frequenz-client-base[grpclib,grpcio]",
 ]
-dev-formatting = ["black == 24.2.0", "isort == 5.13.2"]
+dev-formatting = ["black == 24.4.2", "isort == 5.13.2"]
 dev-mkdocs = [
-  "black == 24.2.0",
-  "Markdown==3.5.2",
+  "black == 24.4.2",
+  "Markdown==3.6",
   "mike == 2.0.0",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
   "mkdocs-macros-plugin == 1.0.5",
-  "mkdocs-material == 9.5.12",
-  "mkdocstrings[python] == 0.24.1",
-  "frequenz-repo-config[lib] == 0.9.1",
+  "mkdocs-material == 9.5.20",
+  "mkdocstrings[python] == 0.25.0",
+  "frequenz-repo-config[lib] == 0.9.2",
+  "frequenz-client-base[grpclib,grpcio]",
 ]
 dev-mypy = [
-  "mypy == 1.8.0",
-  "types-Markdown == 3.5.0.20240129",
-  "types-protobuf == 4.24.0.20240129",
+  "mypy == 1.10.0",
+  "types-Markdown == 3.6.0.20240316",
+  "types-protobuf == 5.26.0.20240422",
   "grpc-stubs == 1.53.0.5",            # This dependency introduces breaking changes in patch releases
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-base[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.9.1"]
+dev-noxfile = ["nox == 2024.4.15", "frequenz-repo-config[lib] == 0.9.2"]
 dev-pylint = [
   "pylint == 3.1.0",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-base[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
-  "pytest == 8.0.2",
-  "frequenz-repo-config[extra-lint-examples] == 0.9.1",
-  "pytest-mock == 3.12.0",
-  "pytest-asyncio == 0.23.5",
-  "async-solipsism == 0.5",
-  "hypothesis == 6.98.15",
+  "pytest == 8.2.0",
+  "frequenz-repo-config[extra-lint-examples] == 0.9.2",
+  "pytest-mock == 3.14.0",
+  "pytest-asyncio == 0.23.6",
+  "async-solipsism == 0.6",
+  "hypothesis == 6.100.2",
+  "frequenz-client-base[grpclib,grpcio]",
 ]
 dev = [
   "frequenz-client-base[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Documentation = "https://frequenz-floss.github.io/frequenz-client-base-python/"
@@ -137,14 +138,16 @@
   "unsubscriptable-object",
   # Checked by flake8
   "redefined-outer-name",
   "unused-import",
   "line-too-long",
   "unused-variable",
   "unnecessary-lambda-assignment",
+  # Checked by mypy
+  "no-member",
 ]
 
 [tool.pytest.ini_options]
 testpaths = ["tests", "src"]
 asyncio_mode = "auto"
 required_plugins = ["pytest-asyncio", "pytest-mock"]
```

### Comparing `frequenz-client-base-0.3.0/src/frequenz/client/base/conversion.py` & `frequenz-client-base-0.4.0/src/frequenz/client/base/conversion.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-base-0.3.0/src/frequenz/client/base/retry.py` & `frequenz-client-base-0.4.0/src/frequenz/client/base/retry.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-base-0.3.0/src/frequenz/client/base/streaming.py` & `frequenz-client-base-0.4.0/src/frequenz/client/base/streaming.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 """Implementation of the grpc streaming helper."""
 
 import asyncio
 import logging
-from typing import Any, Callable, Generic, TypeVar
-
-import grpc.aio
+from collections.abc import AsyncIterator, Callable
+from typing import Generic, TypeVar
 
 from frequenz import channels
 
 from . import retry
+from ._grpchacks import GrpcioError, GrpclibError
 
 _logger = logging.getLogger(__name__)
 
 
 InputT = TypeVar("InputT")
 """The input type of the stream."""
 
@@ -25,15 +25,15 @@
 
 class GrpcStreamBroadcaster(Generic[InputT, OutputT]):
     """Helper class to handle grpc streaming methods."""
 
     def __init__(
         self,
         stream_name: str,
-        stream_method: Callable[[], grpc.aio.UnaryStreamCall[Any, InputT]],
+        stream_method: Callable[[], AsyncIterator[InputT]],
         transform: Callable[[InputT], OutputT],
         retry_strategy: retry.Strategy | None = None,
     ):
         """Initialize the streaming helper.
 
         Args:
             stream_name: A name to identify the stream in the logs.
@@ -78,33 +78,34 @@
         await self._channel.close()
 
     async def _run(self) -> None:
         """Run the streaming helper."""
         sender = self._channel.new_sender()
 
         while True:
-            _logger.debug("Making call to grpc streaming method: %s", self._stream_name)
-
+            error: Exception | None = None
+            _logger.info("%s: starting to stream", self._stream_name)
             try:
                 call = self._stream_method()
                 async for msg in call:
                     await sender.send(self._transform(msg))
-            except grpc.aio.AioRpcError:
-                _logger.exception(
-                    "Error in grpc streaming method: %s", self._stream_name
-                )
-            if interval := self._retry_strategy.next_interval():
-                _logger.warning(
-                    "`%s`, connection ended, retrying %s in %0.3f seconds.",
-                    self._stream_name,
-                    self._retry_strategy.get_progress(),
-                    interval,
-                )
-                await asyncio.sleep(interval)
-            else:
-                _logger.warning(
-                    "`%s`, connection ended, retry limit exceeded %s.",
+            except (GrpcioError, GrpclibError) as err:
+                error = err
+            error_str = f"Error: {error}" if error else "Stream exhausted"
+            interval = self._retry_strategy.next_interval()
+            if interval is None:
+                _logger.error(
+                    "%s: connection ended, retry limit exceeded (%s), giving up. %s.",
                     self._stream_name,
                     self._retry_strategy.get_progress(),
+                    error_str,
                 )
                 await self._channel.close()
                 break
+            _logger.warning(
+                "%s: connection ended, retrying %s in %0.3f seconds. %s.",
+                self._stream_name,
+                self._retry_strategy.get_progress(),
+                interval,
+                error_str,
+            )
+            await asyncio.sleep(interval)
```

### Comparing `frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/PKG-INFO` & `frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-base
-Version: 0.3.0
+Version: 0.4.0
 Summary: Utilities for writing Frequenz API clients
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-base-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-base-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-base-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-base-python
@@ -15,14 +15,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: grpcio
+Provides-Extra: grpclib
 Provides-Extra: dev-flake8
 Provides-Extra: dev-formatting
 Provides-Extra: dev-mkdocs
 Provides-Extra: dev-mypy
 Provides-Extra: dev-noxfile
 Provides-Extra: dev-pylint
 Provides-Extra: dev-pytest
```

### Comparing `frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/SOURCES.txt` & `frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 RELEASE_NOTES.md
 pyproject.toml
 src/frequenz/client/base/__init__.py
+src/frequenz/client/base/_grpchacks.py
+src/frequenz/client/base/channel.py
 src/frequenz/client/base/conftest.py
 src/frequenz/client/base/conversion.py
 src/frequenz/client/base/py.typed
 src/frequenz/client/base/retry.py
 src/frequenz/client/base/streaming.py
 src/frequenz_client_base.egg-info/PKG-INFO
 src/frequenz_client_base.egg-info/SOURCES.txt
```

### Comparing `frequenz-client-base-0.3.0/src/frequenz_client_base.egg-info/requires.txt` & `frequenz-client-base-0.4.0/src/frequenz_client_base.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 frequenz-channels<2,>=v1.0.0-rc1
-grpcio<2,>=1.54.2
-protobuf<5,>=4.21.6
+protobuf<6,>=4.21.6
 typing-extensions<5,>=4.5.0
 
 [dev]
 frequenz-client-base[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==7.0.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
 pydoclint==0.4.1
 pydocstyle==6.3.0
+frequenz-client-base[grpcio,grpclib]
 
 [dev-formatting]
-black==24.2.0
+black==24.4.2
 isort==5.13.2
 
 [dev-mkdocs]
-black==24.2.0
-Markdown==3.5.2
+black==24.4.2
+Markdown==3.6
 mike==2.0.0
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
 mkdocs-macros-plugin==1.0.5
-mkdocs-material==9.5.12
-mkdocstrings[python]==0.24.1
-frequenz-repo-config[lib]==0.9.1
+mkdocs-material==9.5.20
+mkdocstrings[python]==0.25.0
+frequenz-repo-config[lib]==0.9.2
+frequenz-client-base[grpcio,grpclib]
 
 [dev-mypy]
-mypy==1.8.0
-types-Markdown==3.5.0.20240129
-types-protobuf==4.24.0.20240129
+mypy==1.10.0
+types-Markdown==3.6.0.20240316
+types-protobuf==5.26.0.20240422
 grpc-stubs==1.53.0.5
 frequenz-client-base[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-noxfile]
-nox==2023.4.22
-frequenz-repo-config[lib]==0.9.1
+nox==2024.4.15
+frequenz-repo-config[lib]==0.9.2
 
 [dev-pylint]
 pylint==3.1.0
 frequenz-client-base[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-pytest]
-pytest==8.0.2
-frequenz-repo-config[extra-lint-examples]==0.9.1
-pytest-mock==3.12.0
-pytest-asyncio==0.23.5
-async-solipsism==0.5
-hypothesis==6.98.15
+pytest==8.2.0
+frequenz-repo-config[extra-lint-examples]==0.9.2
+pytest-mock==3.14.0
+pytest-asyncio==0.23.6
+async-solipsism==0.6
+hypothesis==6.100.2
+frequenz-client-base[grpcio,grpclib]
+
+[grpcio]
+grpcio<2,>=1.54.2
+
+[grpclib]
+grpclib<0.5,>=0.4.0
```

