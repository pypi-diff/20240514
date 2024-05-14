# Comparing `tmp/rich_click-1.8.1.tar.gz` & `tmp/rich_click-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich_click-1.8.1.tar", last modified: Tue May  7 13:05:34 2024, max compression
+gzip compressed data, was "rich_click-1.8.2.tar", last modified: Tue May 14 12:44:05 2024, max compression
```

## Comparing `rich_click-1.8.1.tar` & `rich_click-1.8.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.737436 rich_click-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 13:05:30.000000 rich_click-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-07 13:05:34.737436 rich_click-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-07 13:05:30.000000 rich_click-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-07 13:05:30.000000 rich_click-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:05:34.737436 rich_click-1.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.733436 rich_click-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.733436 rich_click-1.8.1/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31289 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-07 13:05:30.000000 rich_click-1.8.1/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.737436 rich_click-1.8.1/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 13:05:34.000000 rich_click-1.8.1/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:05:34.737436 rich_click-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-07 13:05:30.000000 rich_click-1.8.1/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:44:05.866353 rich_click-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 12:44:01.000000 rich_click-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-14 12:44:05.866353 rich_click-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-14 12:44:01.000000 rich_click-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-14 12:44:01.000000 rich_click-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:44:05.866353 rich_click-1.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:44:05.862353 rich_click-1.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:44:05.862353 rich_click-1.8.2/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31289 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-14 12:44:01.000000 rich_click-1.8.2/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:44:05.866353 rich_click-1.8.2/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-14 12:44:05.000000 rich_click-1.8.2/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-14 12:44:05.000000 rich_click-1.8.2/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:44:05.000000 rich_click-1.8.2/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 12:44:05.000000 rich_click-1.8.2/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-14 12:44:05.000000 rich_click-1.8.2/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 12:44:05.000000 rich_click-1.8.2/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:44:05.866353 rich_click-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-14 12:44:01.000000 rich_click-1.8.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-14 12:44:01.000000 rich_click-1.8.2/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-05-14 12:44:01.000000 rich_click-1.8.2/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-14 12:44:01.000000 rich_click-1.8.2/tests/test_rich_click_cli.py
```

### Comparing `rich_click-1.8.1/LICENSE` & `rich_click-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/PKG-INFO` & `rich_click-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.1
+Version: 1.8.2
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich_click-1.8.1/README.md` & `rich_click-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/pyproject.toml` & `rich_click-1.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/__init__.py` & `rich_click-1.8.2/src/rich_click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.1"
+__version__ = "1.8.2"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich_click-1.8.1/src/rich_click/_compat_click.py` & `rich_click-1.8.2/src/rich_click/_compat_click.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/cli.py` & `rich_click-1.8.2/src/rich_click/cli.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/decorators.py` & `rich_click-1.8.2/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/patch.py` & `rich_click-1.8.2/src/rich_click/patch.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/rich_click.py` & `rich_click-1.8.2/src/rich_click/rich_click.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/rich_command.py` & `rich_click-1.8.2/src/rich_click/rich_command.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/rich_context.py` & `rich_click-1.8.2/src/rich_click/rich_context.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/rich_help_configuration.py` & `rich_click-1.8.2/src/rich_click/rich_help_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,25 +168,27 @@
         ]
     )
     """Patterns to use with the option highlighter."""
 
     legacy_windows: Optional[bool] = field(default=None)
 
     def __post_init__(self) -> None:  # noqa: D105
-        if self.highlighter is not None:
-            import warnings
+        # Todo: Fix this so that the deprecation warning works properly.
 
-            warnings.warn(
-                "`highlighter` kwarg is deprecated in RichHelpConfiguration."
-                " Please do one of the following instead: either set highlighter_patterns=[...] if you want"
-                " to use regex; or for more advanced use cases where you'd like to use a different type"
-                " of rich.highlighter.Highlighter, subclass the `RichHelpFormatter` and update its `highlighter`.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
+        # if self.highlighter is not None:
+        #     import warnings
+        #
+        #     warnings.warn(
+        #         "`highlighter` kwarg is deprecated in RichHelpConfiguration."
+        #         " Please do one of the following instead: either set highlighter_patterns=[...] if you want"
+        #         " to use regex; or for more advanced use cases where you'd like to use a different type"
+        #         " of rich.highlighter.Highlighter, subclass the `RichHelpFormatter` and update its `highlighter`.",
+        #         DeprecationWarning,
+        #         stacklevel=2,
+        #     )
 
         self.__dataclass_fields__.pop("highlighter", None)
 
     @classmethod
     def load_from_globals(cls, module: Optional[ModuleType] = None, **extra: Any) -> "RichHelpConfiguration":
         """
         Build a RichHelpConfiguration from globals in rich_click.rich_click.
```

### Comparing `rich_click-1.8.1/src/rich_click/rich_help_formatter.py` & `rich_click-1.8.2/src/rich_click/rich_help_formatter.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/rich_help_rendering.py` & `rich_click-1.8.2/src/rich_click/rich_help_rendering.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click/utils.py` & `rich_click-1.8.2/src/rich_click/utils.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/src/rich_click.egg-info/PKG-INFO` & `rich_click-1.8.2/src/rich_click.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.1
+Version: 1.8.2
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich_click-1.8.1/src/rich_click.egg-info/SOURCES.txt` & `rich_click-1.8.2/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/tests/test_config.py` & `rich_click-1.8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/tests/test_exit_code.py` & `rich_click-1.8.2/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/tests/test_help.py` & `rich_click-1.8.2/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich_click-1.8.1/tests/test_rich_click_cli.py` & `rich_click-1.8.2/tests/test_rich_click_cli.py`

 * *Files identical despite different names*

