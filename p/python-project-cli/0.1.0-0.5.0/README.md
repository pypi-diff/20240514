# Comparing `tmp/python_project_cli-0.1.0.tar.gz` & `tmp/python_project_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_cli-0.1.0.tar", max compression
+gzip compressed data, was "python_project_cli-0.5.0.tar", max compression
```

## Comparing `python_project_cli-0.1.0.tar` & `python_project_cli-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-05-12 14:19:08.095314 python_project_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     3774 2024-05-12 15:42:44.234749 python_project_cli-0.1.0/README.md
--rw-r--r--   0        0        0     2475 2024-05-13 10:21:58.786584 python_project_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-12 14:19:08.099314 python_project_cli-0.1.0/src/python_project_cli/__init__.py
--rw-r--r--   0        0        0     1858 2024-05-13 10:14:43.426987 python_project_cli-0.1.0/src/python_project_cli/main.py
--rw-r--r--   0        0        0     4691 1970-01-01 00:00:00.000000 python_project_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-14 16:27:47.722836 python_project_cli-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3775 2024-05-14 16:27:47.722836 python_project_cli-0.5.0/README.md
+-rw-r--r--   0        0        0     2455 2024-05-14 16:27:48.694848 python_project_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-14 16:27:47.726836 python_project_cli-0.5.0/src/python_project_cli/__init__.py
+-rw-r--r--   0        0        0     1858 2024-05-14 16:27:48.694848 python_project_cli-0.5.0/src/python_project_cli/main.py
+-rw-r--r--   0        0        0     4579 1970-01-01 00:00:00.000000 python_project_cli-0.5.0/PKG-INFO
```

### Comparing `python_project_cli-0.1.0/LICENSE` & `python_project_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_project_cli-0.1.0/README.md` & `python_project_cli-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -98,11 +98,12 @@
 ```
 
 - Upload new version to pypi 
 ```bash
 twine upload --repository testpypi dist/*
 ```
 
+
 ## License
 
 PYTHON-PROJECT-CLI is unlicensed, as found in the
 [LICENSE](https://github.com/MentorMate/python-project-cli/blob/development/LICENSE) file.
```

### Comparing `python_project_cli-0.1.0/pyproject.toml` & `python_project_cli-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python_project_cli"
-version = "0.1.0"
+version = "0.5.0"
 authors = ["alexandermentormate"]
 description = "CLI for building base djang and fastapi based projects"
 readme = "README.md"
 homepage = "https://github.com/MentorMate/python-project-cli/"
 repository = "https://github.com/MentorMate/python-project-cli/"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: The Unlicense (Unlicense)",
     "Operating System :: OS Independent",
 ]
 packages = [{ include = "python_project_cli", from = "src" }]
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/MentorMate/python-project-cli/blob/main/CHANGELOG.md"
 
@@ -40,19 +40,17 @@
 
 # for development purpose, in order to check for a new potential release
 # when using `semantic-release version`
 [tool.semantic_release.branches.feature]
 match = "feature/*"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
+python = ">=3.11,<4.0"
 typer = "^0.12.3"
 cookiecutter = "^2.6.0"
-build = "^1.2.1"
-twine = "^5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.9.0"
 pre-commit = "^3.5.0"
 python-semantic-release = "^9.4.1"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
```

### Comparing `python_project_cli-0.1.0/src/python_project_cli/main.py` & `python_project_cli-0.5.0/src/python_project_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from subprocess import run
 from rich.console import Console
 from rich.table import Table
 from rich import print
 import typer
 from typing_extensions import Annotated
 
-__version__ = '0.1.0'
+__version__ = '0.5.0'
 
 app = typer.Typer(add_completion=False)
 console = Console()
 
 
 class Frameworks(StrEnum):
     django = 'Django'
```

### Comparing `python_project_cli-0.1.0/PKG-INFO` & `python_project_cli-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: python_project_cli
-Version: 0.1.0
+Version: 0.5.0
 Summary: CLI for building base djang and fastapi based projects
 Home-page: https://github.com/MentorMate/python-project-cli/
 Author: alexandermentormate
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: build (>=1.2.1,<2.0.0)
 Requires-Dist: cookiecutter (>=2.6.0,<3.0.0)
-Requires-Dist: twine (>=5.0.0,<6.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Changelog, https://github.com/MentorMate/python-project-cli/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/MentorMate/python-project-cli/
 Description-Content-Type: text/markdown
 
 # MentorMate Python CLI
 A CLI tool for generating Django and FastAPI projects.
@@ -119,12 +116,13 @@
 ```
 
 - Upload new version to pypi 
 ```bash
 twine upload --repository testpypi dist/*
 ```
 
+
 ## License
 
 PYTHON-PROJECT-CLI is unlicensed, as found in the
 [LICENSE](https://github.com/MentorMate/python-project-cli/blob/development/LICENSE) file.
```

