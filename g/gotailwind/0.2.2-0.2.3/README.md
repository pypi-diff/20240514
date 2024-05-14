# Comparing `tmp/gotailwind-0.2.2.tar.gz` & `tmp/gotailwind-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotailwind-0.2.2.tar", max compression
+gzip compressed data, was "gotailwind-0.2.3.tar", max compression
```

## Comparing `gotailwind-0.2.2.tar` & `gotailwind-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-12-18 19:25:03.824973 gotailwind-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     8325 2023-12-18 19:25:03.824973 gotailwind-0.2.2/README.md
--rw-r--r--   0        0        0     4083 2023-12-18 19:25:15.572934 gotailwind-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2223 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/__init__.py
--rw-r--r--   0        0        0    14480 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/cli/__init__.py
--rw-r--r--   0        0        0     6294 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/cli/async_typer.py
--rw-r--r--   0        0        0      174 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/cli/ruff.toml
--rw-r--r--   0        0        0      827 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/const.py
--rw-r--r--   0        0        0     1058 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/exceptions.py
--rw-r--r--   0        0        0     7773 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/models.py
--rw-r--r--   0        0        0        0 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/py.typed
--rw-r--r--   0        0        0     6869 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/tailwind.py
--rw-r--r--   0        0        0      269 2023-12-18 19:25:03.824973 gotailwind-0.2.2/src/gotailwind/util.py
--rw-r--r--   0        0        0     9835 1970-01-01 00:00:00.000000 gotailwind-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-14 07:30:31.265818 gotailwind-0.2.3/LICENSE.md
+-rw-r--r--   0        0        0     8335 2024-05-14 07:30:31.265818 gotailwind-0.2.3/README.md
+-rw-r--r--   0        0        0     4102 2024-05-14 07:30:44.645772 gotailwind-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2224 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/__init__.py
+-rw-r--r--   0        0        0    14481 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/cli/__init__.py
+-rw-r--r--   0        0        0     6278 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/cli/async_typer.py
+-rw-r--r--   0        0        0      179 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/cli/ruff.toml
+-rw-r--r--   0        0        0      827 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/const.py
+-rw-r--r--   0        0        0     1058 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/exceptions.py
+-rw-r--r--   0        0        0     7774 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/models.py
+-rw-r--r--   0        0        0        0 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/py.typed
+-rw-r--r--   0        0        0     6872 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/tailwind.py
+-rw-r--r--   0        0        0      269 2024-05-14 07:30:31.269818 gotailwind-0.2.3/src/gotailwind/util.py
+-rw-r--r--   0        0        0     9845 1970-01-01 00:00:00.000000 gotailwind-0.2.3/PKG-INFO
```

### Comparing `gotailwind-0.2.2/LICENSE.md` & `gotailwind-0.2.3/LICENSE.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2023 Franck Nijhof
+Copyright (c) 2023-2024 Franck Nijhof
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gotailwind-0.2.2/README.md` & `gotailwind-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 For a full list of all authors and contributors,
 check [the contributor's page][contributors].
 
 ## License
 
 MIT License
 
-Copyright (c) 2023 Franck Nijhof
+Copyright (c) 2023-2024 Franck Nijhof
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -223,15 +223,15 @@
 [devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
 [devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/frenck/python-gotailwind
 [frenck]: https://github.com/frenck
 [github-sponsors-shield]: https://frenck.dev/wp-content/uploads/2019/12/github_sponsor.png
 [github-sponsors]: https://github.com/sponsors/frenck
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/frenck/python-gotailwind.svg
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023-2024.svg
 [patreon-shield]: https://frenck.dev/wp-content/uploads/2019/12/patreon.png
 [patreon]: https://www.patreon.com/frenck
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
 [pypi]: https://pypi.org/project/gotailwind/
```

### Comparing `gotailwind-0.2.2/pyproject.toml` & `gotailwind-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 maintainers = ["Franck Nijhof <opensource@frenck.dev>"]
 name = "gotailwind"
 packages = [
   {include = "gotailwind", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/frenck/python-gotailwind"
-version = "0.2.2"
+version = "0.2.3"
 
 [tool.poetry.dependencies]
 aiohttp = ">=3.0.0"
 awesomeversion = ">=22.8.0"
 backoff = ">=2.2.1"
 mashumaro = ">=3.10"
 orjson = ">=3.9.8"
@@ -42,29 +42,29 @@
 tailwind = "gotailwind.cli:cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/frenck/python-gotailwind/issues"
 Changelog = "https://github.com/frenck/python-gotailwind/releases"
 
 [tool.poetry.group.dev.dependencies]
-aresponses = "2.1.6"
+aresponses = "3.0.0"
 codespell = "2.2.6"
 covdefaults = "2.3.0"
-coverage = {version = "7.3.3", extras = ["toml"]}
-mypy = "1.7.1"
-pre-commit = "3.6.0"
-pre-commit-hooks = "4.5.0"
-pylint = "3.0.3"
-pytest = "7.4.3"
-pytest-asyncio = "0.23.2"
-pytest-cov = "4.1.0"
-ruff = "0.1.8"
-safety = "2.4.0b2"
-syrupy = "4.6.0"
-yamllint = "1.33.0"
+coverage = {version = "7.5.1", extras = ["toml"]}
+mypy = "1.10.0"
+pre-commit = "3.7.1"
+pre-commit-hooks = "4.6.0"
+pylint = "3.1.1"
+pytest = "7.4.4"
+pytest-asyncio = "0.23.6"
+pytest-cov = "5.0.0"
+ruff = "0.4.4"
+safety = "3.2.0"
+syrupy = "4.6.1"
+yamllint = "1.35.1"
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["gotailwind"]
 
 [tool.coverage.report]
 show_missing = true
@@ -139,38 +139,38 @@
 [tool.pylint.FORMAT]
 max-line-length = 88
 
 [tool.pytest.ini_options]
 addopts = "--cov"
 asyncio_mode = "auto"
 
-[tool.ruff]
+[tool.ruff.lint]
 ignore = [
   "ANN101", # Self... explanatory
   "ANN401", # Opinioated warning on disallowing dynamically typed expressions
   "D203", # Conflicts with other rules
   "D213", # Conflicts with other rules
   "D417", # False positives in some occasions
   "PLR2004", # Just annoying, not really useful
 
   # Conflicts with the Ruff formatter
   "COM812",
   "ISC001",
 ]
 select = ["ALL"]
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["gotailwind"]
 
 [tool.ruff.lint.flake8-type-checking]
 runtime-evaluated-base-classes = ["mashumaro.mixins.orjson.DataClassORJSONMixin"]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 25
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `gotailwind-0.2.2/src/gotailwind/__init__.py` & `gotailwind-0.2.3/src/gotailwind/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Asynchronous Python client for Tailwind garage door openers."""
+
 from .const import (
     MIN_REQUIRED_FIRMWARE_VERSION,
     TailwindDoorOperationCommand,
     TailwindDoorState,
     TailwindRequestType,
     TailwindResponseResult,
 )
```

### Comparing `gotailwind-0.2.2/src/gotailwind/cli/__init__.py` & `gotailwind-0.2.3/src/gotailwind/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Asynchronous Python client for Tailwind garage door openers."""
+
 import asyncio
 import sys
 from typing import Annotated
 
 import typer
 from rich.console import Console
 from rich.live import Live
```

### Comparing `gotailwind-0.2.2/src/gotailwind/cli/async_typer.py` & `gotailwind-0.2.3/src/gotailwind/cli/async_typer.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,14 @@
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Call the typer app."""
         try:
             return super().__call__(*args, **kwargs)
         except Exit:
             raise
         # pylint: disable-next=broad-except
-        except Exception as e:  # noqa: BLE001
+        except Exception as e:
             if (
                 not hasattr(self, "error_handlers")
                 or (handler := self.error_handlers.get(type(e))) is None
             ):
                 raise
             return handler(e)
```

### Comparing `gotailwind-0.2.2/src/gotailwind/const.py` & `gotailwind-0.2.3/src/gotailwind/const.py`

 * *Files identical despite different names*

### Comparing `gotailwind-0.2.2/src/gotailwind/exceptions.py` & `gotailwind-0.2.3/src/gotailwind/exceptions.py`

 * *Files identical despite different names*

### Comparing `gotailwind-0.2.2/src/gotailwind/models.py` & `gotailwind-0.2.3/src/gotailwind/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Asynchronous Python client for Tailwind garage door openers."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, Generic, Self, TypeVar
 
 from mashumaro import field_options
 from mashumaro.config import BaseConfig
```

### Comparing `gotailwind-0.2.2/src/gotailwind/tailwind.py` & `gotailwind-0.2.3/src/gotailwind/tailwind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Asynchronous Python client for Tailwind garage door openers."""
+
 from __future__ import annotations
 
 import asyncio
 import socket
 from dataclasses import dataclass
 from typing import Any, Self, TypeVar
 
@@ -199,18 +200,20 @@
 
     async def __aenter__(self) -> Self:
         """Async enter.
 
         Returns
         -------
             The Tailwind object.
+
         """
         return self
 
     async def __aexit__(self, *_exc_info: object) -> None:
         """Async exit.
 
         Args:
         ----
             _exc_info: Exec type.
+
         """
         await self.close()
```

### Comparing `gotailwind-0.2.2/PKG-INFO` & `gotailwind-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotailwind
-Version: 0.2.2
+Version: 0.2.3
 Summary: Asynchronous Python client for Tailwind garage door openers.
 Home-page: https://github.com/frenck/python-gotailwind
 License: MIT
 Keywords: gotailwind,tailwind,iq3,myq,chamberlain,craftsman,liftmaster
 Author: Franck Nijhof
 Author-email: opensource@frenck.dev
 Maintainer: Franck Nijhof
@@ -227,15 +227,15 @@
 For a full list of all authors and contributors,
 check [the contributor's page][contributors].
 
 ## License
 
 MIT License
 
-Copyright (c) 2023 Franck Nijhof
+Copyright (c) 2023-2024 Franck Nijhof
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -259,15 +259,15 @@
 [devcontainer-shield]: https://img.shields.io/static/v1?label=Dev%20Containers&message=Open&color=blue&logo=visualstudiocode
 [devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/frenck/python-gotailwind
 [frenck]: https://github.com/frenck
 [github-sponsors-shield]: https://frenck.dev/wp-content/uploads/2019/12/github_sponsor.png
 [github-sponsors]: https://github.com/sponsors/frenck
 [keepchangelog]: http://keepachangelog.com/en/1.0.0/
 [license-shield]: https://img.shields.io/github/license/frenck/python-gotailwind.svg
-[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023-2024.svg
 [patreon-shield]: https://frenck.dev/wp-content/uploads/2019/12/patreon.png
 [patreon]: https://www.patreon.com/frenck
 [poetry-install]: https://python-poetry.org/docs/#installation
 [poetry]: https://python-poetry.org
 [pre-commit]: https://pre-commit.com/
 [project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
 [pypi]: https://pypi.org/project/gotailwind/
```

