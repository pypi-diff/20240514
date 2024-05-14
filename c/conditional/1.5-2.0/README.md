# Comparing `tmp/conditional-1.5.tar.gz` & `tmp/conditional-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conditional-1.5.tar", last modified: Thu Sep 14 13:31:35 2023, max compression
+gzip compressed data, was "conditional-2.0.tar", last modified: Tue May 14 10:47:50 2024, max compression
```

## Comparing `conditional-1.5.tar` & `conditional-2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-09-14 13:31:35.929237 conditional-1.5/
--rw-r--r--   0 stefan     (501) staff       (20)     1140 2023-09-14 13:28:17.000000 conditional-1.5/CHANGES.rst
--rw-r--r--   0 stefan     (501) staff       (20)     1288 2023-09-08 08:06:19.000000 conditional-1.5/LICENSE
--rw-r--r--   0 stefan     (501) staff       (20)      115 2023-09-11 18:30:47.000000 conditional-1.5/MANIFEST.in
--rw-r--r--   0 stefan     (501) staff       (20)     3381 2023-09-14 13:31:35.929438 conditional-1.5/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)     1374 2023-09-11 18:30:47.000000 conditional-1.5/README.rst
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-09-14 13:31:35.924090 conditional-1.5/conditional/
--rw-r--r--   0 stefan     (501) staff       (20)      157 2023-09-10 07:10:21.000000 conditional-1.5/conditional/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)      717 2023-09-11 18:30:47.000000 conditional-1.5/conditional/conditional.py
--rw-r--r--   0 stefan     (501) staff       (20)      769 2023-09-11 18:30:47.000000 conditional-1.5/conditional/conditional.pyi
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-09-14 13:31:35.927779 conditional-1.5/conditional/examples/
--rw-r--r--   0 stefan     (501) staff       (20)        0 2023-09-11 18:30:47.000000 conditional-1.5/conditional/examples/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)     4773 2023-09-11 18:30:47.000000 conditional-1.5/conditional/examples/example.py
--rw-r--r--   0 stefan     (501) staff       (20)        0 2023-09-11 18:30:47.000000 conditional-1.5/conditional/py.typed
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-09-14 13:31:35.928644 conditional-1.5/conditional/tests/
--rw-r--r--   0 stefan     (501) staff       (20)        0 2019-03-04 22:33:22.000000 conditional-1.5/conditional/tests/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)     2126 2022-03-07 18:58:58.000000 conditional-1.5/conditional/tests/test_conditional.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-09-14 13:31:35.926975 conditional-1.5/conditional.egg-info/
--rw-r--r--   0 stefan     (501) staff       (20)     3381 2023-09-14 13:31:35.000000 conditional-1.5/conditional.egg-info/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)      525 2023-09-14 13:31:35.000000 conditional-1.5/conditional.egg-info/SOURCES.txt
--rw-r--r--   0 stefan     (501) staff       (20)        1 2023-09-14 13:31:35.000000 conditional-1.5/conditional.egg-info/dependency_links.txt
--rw-r--r--   0 stefan     (501) staff       (20)        1 2023-08-22 18:06:19.000000 conditional-1.5/conditional.egg-info/not-zip-safe
--rw-r--r--   0 stefan     (501) staff       (20)       79 2023-09-14 13:31:35.000000 conditional-1.5/conditional.egg-info/requires.txt
--rw-r--r--   0 stefan     (501) staff       (20)       12 2023-09-14 13:31:35.000000 conditional-1.5/conditional.egg-info/top_level.txt
--rw-r--r--   0 stefan     (501) staff       (20)       90 2022-03-07 18:47:34.000000 conditional-1.5/pyproject.toml
--rw-r--r--   0 stefan     (501) staff       (20)     1249 2023-09-14 13:31:35.930684 conditional-1.5/setup.cfg
--rw-r--r--   0 stefan     (501) staff       (20)       38 2022-03-07 18:47:34.000000 conditional-1.5/setup.py
--rw-r--r--   0 stefan     (501) staff       (20)      763 2023-09-11 18:30:47.000000 conditional-1.5/tox.ini
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2024-05-14 10:47:50.369286 conditional-2.0/
+-rw-r--r--   0 stefan     (501) staff       (20)     1289 2024-05-14 10:36:30.000000 conditional-2.0/CHANGES.rst
+-rw-r--r--   0 stefan     (501) staff       (20)     1288 2024-05-14 10:22:53.000000 conditional-2.0/LICENSE
+-rw-r--r--   0 stefan     (501) staff       (20)      115 2023-09-11 18:30:47.000000 conditional-2.0/MANIFEST.in
+-rw-r--r--   0 stefan     (501) staff       (20)     3838 2024-05-14 10:47:50.369067 conditional-2.0/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)     1536 2024-05-14 10:22:53.000000 conditional-2.0/README.rst
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2024-05-14 10:47:50.362671 conditional-2.0/conditional/
+-rw-r--r--   0 stefan     (501) staff       (20)      118 2024-05-14 10:22:53.000000 conditional-2.0/conditional/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)     1003 2024-05-14 10:22:53.000000 conditional-2.0/conditional/conditional.py
+-rw-r--r--   0 stefan     (501) staff       (20)     1111 2024-05-14 10:22:53.000000 conditional-2.0/conditional/conditional.pyi
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2024-05-14 10:47:50.366542 conditional-2.0/conditional/examples/
+-rw-r--r--   0 stefan     (501) staff       (20)        0 2023-09-11 18:30:47.000000 conditional-2.0/conditional/examples/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)     5441 2024-05-14 10:22:53.000000 conditional-2.0/conditional/examples/example.py
+-rw-r--r--   0 stefan     (501) staff       (20)        0 2023-09-11 18:30:47.000000 conditional-2.0/conditional/py.typed
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2024-05-14 10:47:50.367317 conditional-2.0/conditional/tests/
+-rw-r--r--   0 stefan     (501) staff       (20)        0 2019-03-04 22:33:22.000000 conditional-2.0/conditional/tests/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)     4500 2024-05-14 10:22:53.000000 conditional-2.0/conditional/tests/test_conditional.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2024-05-14 10:47:50.365762 conditional-2.0/conditional.egg-info/
+-rw-r--r--   0 stefan     (501) staff       (20)     3838 2024-05-14 10:47:50.000000 conditional-2.0/conditional.egg-info/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)      525 2024-05-14 10:47:50.000000 conditional-2.0/conditional.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        1 2024-05-14 10:47:50.000000 conditional-2.0/conditional.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        1 2023-08-22 18:06:19.000000 conditional-2.0/conditional.egg-info/not-zip-safe
+-rw-r--r--   0 stefan     (501) staff       (20)       79 2024-05-14 10:47:50.000000 conditional-2.0/conditional.egg-info/requires.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       12 2024-05-14 10:47:50.000000 conditional-2.0/conditional.egg-info/top_level.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       90 2024-05-14 08:29:18.000000 conditional-2.0/pyproject.toml
+-rw-r--r--   0 stefan     (501) staff       (20)     1196 2024-05-14 10:47:50.370214 conditional-2.0/setup.cfg
+-rw-r--r--   0 stefan     (501) staff       (20)       38 2022-03-07 18:47:34.000000 conditional-2.0/setup.py
+-rw-r--r--   0 stefan     (501) staff       (20)      731 2024-05-14 10:22:53.000000 conditional-2.0/tox.ini
```

### Comparing `conditional-1.5/CHANGES.rst` & `conditional-2.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+2.0 - 2024-05-14
+----------------
+
+- Support asynchronous context managers. Thanks to Dawid Wolski.
+  [stefan]
+
+- Require Python >= 3.5.
+  [stefan]
+
 1.5 - 2023-09-14
 ----------------
 
 - Add type annotations to the context manager.
   [stefan]
 
 - Update tox.ini for latest tox.
```

### Comparing `conditional-1.5/LICENSE` & `conditional-2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2012-2023 Stefan H. Holek
+Copyright (c) 2012-2024 Stefan H. Holek
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `conditional-1.5/PKG-INFO` & `conditional-2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: conditional
-Version: 1.5
+Version: 2.0
 Summary: Conditionally enter a context manager
 Home-page: https://github.com/stefanholek/conditional
 Author: Stefan H. Holek
 Author-email: stefan@epy.co.at
 License: BSD-2-Clause
 Project-URL: Documentation, https://conditional.readthedocs.io/en/stable/
-Keywords: conditional,context manager,with
+Keywords: conditional,context manager,contextmanager,with,async,async with,enter,exit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7
+Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: testing
+Requires-Dist: flexmock; extra == "testing"
 Provides-Extra: mypy
+Requires-Dist: mypy; extra == "mypy"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "docs"
 
 ===========
 conditional
 ===========
 -------------------------------------------------------------------
 Conditionally enter a context manager
 -------------------------------------------------------------------
@@ -55,18 +58,28 @@
 Consider replacing it with:
 
 .. code-block:: python
 
     with conditional(CONDITION, CONTEXTMANAGER()):
         BODY()
 
+Async
+=====
+
+`conditional` supports asynchronous context managers:
+
+.. code-block:: python
+
+    async with conditional(CONDITION, ASYNCCONTEXTMANAGER()):
+        BODY()
+
 Typing
 ======
 
-The context manager ships with type annotations. Type checkers and IDEs can
+The package ships with type annotations. Type checkers and IDEs can
 use this information to implement type safety and auto completion.
 
 Examples
 ========
 
 Say we want to ignore signals when a pager application is in the
 foreground, but not otherwise:
@@ -85,14 +98,23 @@
 
 .. _`API Documentation`: https://conditional.readthedocs.io/en/stable/
 
 
 Changelog
 =========
 
+2.0 - 2024-05-14
+----------------
+
+- Support asynchronous context managers. Thanks to Dawid Wolski.
+  [stefan]
+
+- Require Python >= 3.5.
+  [stefan]
+
 1.5 - 2023-09-14
 ----------------
 
 - Add type annotations to the context manager.
   [stefan]
 
 - Update tox.ini for latest tox.
```

### Comparing `conditional-1.5/README.rst` & `conditional-2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,28 @@
 Consider replacing it with:
 
 .. code-block:: python
 
     with conditional(CONDITION, CONTEXTMANAGER()):
         BODY()
 
+Async
+=====
+
+`conditional` supports asynchronous context managers:
+
+.. code-block:: python
+
+    async with conditional(CONDITION, ASYNCCONTEXTMANAGER()):
+        BODY()
+
 Typing
 ======
 
-The context manager ships with type annotations. Type checkers and IDEs can
+The package ships with type annotations. Type checkers and IDEs can
 use this information to implement type safety and auto completion.
 
 Examples
 ========
 
 Say we want to ignore signals when a pager application is in the
 foreground, but not otherwise:
```

### Comparing `conditional-1.5/conditional/conditional.pyi` & `conditional-2.0/conditional/conditional.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import sys
 
-from typing import Any, ContextManager, Optional, Type, TypeVar
+from typing import Any, AsyncContextManager, ContextManager, Optional, Type, TypeVar
 from types import TracebackType
 
 if sys.version_info >= (3, 9):
     from types import GenericAlias
 
 _T = TypeVar("_T")
 
 
-class conditional(ContextManager[_T]):
+class conditional(ContextManager[_T], AsyncContextManager[_T]):
     condition: Optional[Any]
-    contextmanager: ContextManager[_T]
+    contextmanager: ContextManager[_T] | AsyncContextManager[_T]
 
     def __init__(
         self,
         condition: Optional[Any],
-        contextmanager: ContextManager[_T],
+        contextmanager: ContextManager[_T] | AsyncContextManager[_T],
     ) -> None: ...
 
     def __enter__(self) -> _T: ...
 
+    async def __aenter__(self) -> _T: ...
+
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> Optional[bool]: ...
 
+    async def __aexit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> Optional[bool]: ...
+
     if sys.version_info >= (3, 9):
         def __class_getitem__(cls, params: Any) -> GenericAlias: ...
```

### Comparing `conditional-1.5/conditional/examples/example.py` & `conditional-2.0/conditional/examples/example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from typing import TYPE_CHECKING
-from typing import Any, ContextManager, Iterator, Optional, TypeVar
+from typing import Any, AsyncContextManager, ContextManager, Iterator, Optional, TypeVar
 
 from contextlib import contextmanager
 from conditional import conditional
 
 
 @contextmanager
 def setstr(key: str, value: str) -> Iterator[str]:
@@ -66,14 +66,28 @@
 
         def __enter__(self) -> setfloat:
             return self
 
         def __exit__(self, *exc_info: object) -> Optional[bool]:
             return None
 
+    class asetfloat(AsyncContextManager[asetfloat]):
+        key: str
+        value: float
+        saved: Optional[str]
+
+        def __init__(self, key: str, value: float) -> None:
+            pass
+
+        async def __aenter__(self) -> asetfloat:
+            return self
+
+        async def __aexit__(self, *exc_info: object) -> Optional[bool]:
+            return None
+
 
 # Inherit from conditional
 _T = TypeVar('_T')
 
 
 class inverted(conditional[_T]):
     def __init__(self, condition: Optional[Any], contextmanager: ContextManager[_T]) -> None:
@@ -154,14 +168,24 @@
         c.key == 'quux'
         c.value == 42.0
         c.saved == None
         c.saved == ''
         c.__enter__
         c.__exit__
 
+    async def a() -> None:
+        async with conditional(True, asetfloat('quux', 42.0)) as c:
+            c == None
+            c.key == 'quux'
+            c.value == 42.0
+            c.saved == None
+            c.saved == ''
+            c.__aenter__
+            c.__aexit__
+
 
 if TYPE_CHECKING:
     conditional.__class_getitem__(None)
     inverted.__class_getitem__(None)
 
 
 def g() -> None:
```

### Comparing `conditional-1.5/conditional.egg-info/PKG-INFO` & `conditional-2.0/conditional.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: conditional
-Version: 1.5
+Version: 2.0
 Summary: Conditionally enter a context manager
 Home-page: https://github.com/stefanholek/conditional
 Author: Stefan H. Holek
 Author-email: stefan@epy.co.at
 License: BSD-2-Clause
 Project-URL: Documentation, https://conditional.readthedocs.io/en/stable/
-Keywords: conditional,context manager,with
+Keywords: conditional,context manager,contextmanager,with,async,async with,enter,exit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,>=2.7
+Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: testing
+Requires-Dist: flexmock; extra == "testing"
 Provides-Extra: mypy
+Requires-Dist: mypy; extra == "mypy"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "docs"
 
 ===========
 conditional
 ===========
 -------------------------------------------------------------------
 Conditionally enter a context manager
 -------------------------------------------------------------------
@@ -55,18 +58,28 @@
 Consider replacing it with:
 
 .. code-block:: python
 
     with conditional(CONDITION, CONTEXTMANAGER()):
         BODY()
 
+Async
+=====
+
+`conditional` supports asynchronous context managers:
+
+.. code-block:: python
+
+    async with conditional(CONDITION, ASYNCCONTEXTMANAGER()):
+        BODY()
+
 Typing
 ======
 
-The context manager ships with type annotations. Type checkers and IDEs can
+The package ships with type annotations. Type checkers and IDEs can
 use this information to implement type safety and auto completion.
 
 Examples
 ========
 
 Say we want to ignore signals when a pager application is in the
 foreground, but not otherwise:
@@ -85,14 +98,23 @@
 
 .. _`API Documentation`: https://conditional.readthedocs.io/en/stable/
 
 
 Changelog
 =========
 
+2.0 - 2024-05-14
+----------------
+
+- Support asynchronous context managers. Thanks to Dawid Wolski.
+  [stefan]
+
+- Require Python >= 3.5.
+  [stefan]
+
 1.5 - 2023-09-14
 ----------------
 
 - Add type annotations to the context manager.
   [stefan]
 
 - Update tox.ini for latest tox.
```

### Comparing `conditional-1.5/conditional.egg-info/SOURCES.txt` & `conditional-2.0/conditional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conditional-1.5/setup.cfg` & `conditional-2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [metadata]
 name = conditional
-version = 1.5
+version = 2.0
 description = Conditionally enter a context manager
 long_description = file: README.rst, CHANGES.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 2
 	Programming Language :: Python :: 3
-keywords = conditional, context manager, with
+keywords = conditional, context manager, contextmanager, with, async, async with, enter, exit
 author = Stefan H. Holek
 author_email = stefan@epy.co.at
 url = https://github.com/stefanholek/conditional
 project_urls = 
 	Documentation = https://conditional.readthedocs.io/en/stable/
 license = BSD-2-Clause
 
 [options]
 packages = find:
 include_package_data = false
 zip_safe = false
-python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*
+python_requires = >=3.5
 
 [options.packages.find]
 exclude = 
 	conditional.examples
 	conditional.tests
 
 [options.package_data]
@@ -45,15 +44,12 @@
 	sphinx == 5.3.0
 	sphinx-rtd-theme == 1.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
 
-[bdist_wheel]
-universal = true
-
 [build_sphinx]
 source_dir = docs
 build_dir = docs/_build
 all_files = true
```

### Comparing `conditional-1.5/tox.ini` & `conditional-2.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported Python versions. To use it,
 # "pip install tox" and then run "tox" from this directory.
 
 [tox]
-envlist = py27, py36, py37, py38, py39, py310, py311, py312, pypy27, pypy38, mypy
-requires = virtualenv<20.22.0
+envlist = py37, py38, py39, py310, py311, py312, pypy38, mypy
+requires = tox>=4
 
 [testenv]
 package = wheel
 wheel_build_env = .pkg
 extras = testing
 commands = python -m unittest discover {posargs}
```

