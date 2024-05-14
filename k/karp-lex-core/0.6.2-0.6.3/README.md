# Comparing `tmp/karp_lex_core-0.6.2.tar.gz` & `tmp/karp_lex_core-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karp_lex_core-0.6.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `karp_lex_core-0.6.2.tar` & `karp_lex_core-0.6.3.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-01-24 11:23:49.331710 karp_lex_core-0.6.2/LICENSE
--rw-r--r--   0        0        0      239 2024-01-24 11:23:49.331710 karp_lex_core-0.6.2/README.md
--rw-r--r--   0        0        0      894 2024-01-24 11:23:49.331710 karp_lex_core-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      217 2024-01-24 11:23:49.331710 karp_lex_core-0.6.2/src/karp/lex_core/__init__.py
--rw-r--r--   0        0        0      236 2024-01-24 11:23:49.331710 karp_lex_core-0.6.2/src/karp/lex_core/alias_generators.py
--rw-r--r--   0        0        0     1075 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/commands/__init__.py
--rw-r--r--   0        0        0      890 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/commands/base.py
--rw-r--r--   0        0        0     1690 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/commands/entry_commands.py
--rw-r--r--   0        0        0      838 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/commands/entry_repo_commands.py
--rw-r--r--   0        0        0     3062 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/commands/resource_commands.py
--rw-r--r--   0        0        0      124 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/dtos/__init__.py
--rw-r--r--   0        0        0     1314 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/dtos/entry_dto.py
--rw-r--r--   0        0        0        0 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/py.typed
--rw-r--r--   0        0        0      229 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/value_objects/__init__.py
--rw-r--r--   0        0        0     3749 2024-01-24 11:23:49.335710 karp_lex_core-0.6.2/src/karp/lex_core/value_objects/unique_id.py
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 karp_lex_core-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/.bumpversion.cfg
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/Makefile
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/mypy.ini
+-rw-r--r--   0        0        0    32401 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/pdm.lock
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/ruff.toml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/src/karp/lex_core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/src/karp/lex_core/py.typed
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/src/karp/lex_core/commands/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/src/karp/lex_core/dtos/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/src/karp/lex_core/value_objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/tests/conftest.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/tests/entry_dto_unit_test.py
+-rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/tests/test_entry_commands.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/tests/test_entry_repo_commands.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/tests/test_resource_commands.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/tests/test_unique_id.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/LICENSE
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/README.md
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 karp_lex_core-0.6.3/PKG-INFO
```

### Comparing `karp_lex_core-0.6.2/LICENSE` & `karp_lex_core-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `karp_lex_core-0.6.2/pyproject.toml` & `karp_lex_core-0.6.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,44 @@
-[tool.poetry]
-name = "karp-lex-core"
-version = "0.6.2"
-description = "The core of karp-lex"
+[project]
 authors = [
-    "Språkbanken at the University of Gothenburg <sb-info@svenska.gu.se>",
-    "Kristoffer Andersson <kristoffer.andersson@gu.se>",
+    { name = "Språkbanken at the University of Gothenburg", email = "sb-info@svenska.gu.se" },
+    { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
-license = "MIT"
+license = { text = "MIT" }
+requires-python = ">=3.10,<4.0"
+dependencies = ["karp-lex-types>=0.6.2"]
+name = "karp-lex-core"
+version = "0.6.3"
+description = "The core of karp-lex"
 readme = "README.md"
-homepage = "https://spraakbanken.gu.se"
 
-documentation = "https://github.com/spraakbanken/karp-lex-core"
+[project.urls]
+"Bug Tracker" = "https://github.com/spraakbanken/karp-lex-core/issues"
+homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/karp-lex-core"
-packages = [{ include = "karp/lex_core", from = "src" }]
+documentation = "https://github.com/spraakbanken/karp-lex-core"
 
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/spraakbanken/karp-lex-core/issues"
 
-[tool.poetry.dependencies]
-python = "^3.10"
-pydantic = "^2.5.3"
-ulid-py = "^1.1.0"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
-bump2version = "^1.0.1"
-mypy = "^1.8.0"
-ruff = "^0.1.14"
+[tool.pdm.dev-dependencies]
+dev = [
+    "pytest<8.0.0,>=7.2.1",
+    "pytest-cov<5.0.0,>=4.0.0",
+    "bump2version<2.0.0,>=1.0.1",
+    "mypy<2.0.0,>=1.8.0",
+    "ruff<1.0.0,>=0.1.14",
+]
+
+[tool.pdm.build]
+includes = ["src/karp/lex_core"]
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.build.targets.sdist]
+exclude = ["/.github", "/docs"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/karp/"]
```

### Comparing `karp_lex_core-0.6.2/src/karp/lex_core/commands/__init__.py` & `karp_lex_core-0.6.3/src/karp/lex_core/commands/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 """Commands top-level module."""
-from .entry_commands import (
+
+from karp_lex_types.commands.entry_commands import (
     AddEntries,
     AddEntriesInChunks,
     AddEntry,
     DeleteEntry,
     EntryCommand,
     ExecuteBatchOfEntryCommands,
     GenericAddEntry,
     GenericUpdateEntry,
     ImportEntries,
     ImportEntriesInChunks,
     UpdateEntry,
 )
-from .entry_repo_commands import CreateEntryRepository
-from .resource_commands import (
+from karp_lex_types.commands.entry_repo_commands import CreateEntryRepository
+from karp_lex_types.commands.resource_commands import (
     CreateResource,
     DeleteResource,
+    EntityOrResourceIdMixin,
     GenericCreateResource,
     GenericUpdateResource,
     PublishResource,
     SetEntryRepoId,
     UpdateResource,
 )
 
 __all__ = [
     # Entry commands
     "AddEntries",
     "AddEntriesInChunks",
     "AddEntry",
-    "DeleteEntry",
-    "GenericAddEntry",
-    "GenericUpdateEntry",
-    "ImportEntries",
-    "ImportEntriesInChunks",
-    "UpdateEntry",
-    "EntryCommand",
-    "ExecuteBatchOfEntryCommands",
     # EntryRepo commands
     "CreateEntryRepository",
     # Resource commands
     "CreateResource",
+    "DeleteEntry",
     "DeleteResource",
+    "EntityOrResourceIdMixin",
+    "EntryCommand",
+    "ExecuteBatchOfEntryCommands",
+    "GenericAddEntry",
     "GenericCreateResource",
+    "GenericUpdateEntry",
     "GenericUpdateResource",
+    "ImportEntries",
+    "ImportEntriesInChunks",
     "PublishResource",
     "SetEntryRepoId",
+    "UpdateEntry",
     "UpdateResource",
 ]
```

