# Comparing `tmp/hairydogm-0.2.7.tar.gz` & `tmp/hairydogm-0.3.0.tar.gz`

## Comparing `hairydogm-0.2.7.tar` & `hairydogm-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hairydogm-0.2.7/.editorconfig
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 hairydogm-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hairydogm-0.2.7/.readthedocs.yaml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 hairydogm-0.2.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/Makefile
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/conf.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/filters.base.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/filters.callback_data.rst
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/filters.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/i18n.context.rst
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/i18n.core.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/i18n.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/index.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/keyboard.rst
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hairydogm-0.2.7/docs/source/mixins.rst
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/__init__.py
--rw-r--r--   0        0        0    13697 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/keyboard.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/mixins.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/filters/__init__.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/filters/base.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/filters/callback_data.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/i18n/__init__.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/i18n/context.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 hairydogm-0.2.7/src/hairydogm/i18n/core.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hairydogm-0.2.7/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hairydogm-0.2.7/LICENSE
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hairydogm-0.2.7/README.md
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 hairydogm-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 hairydogm-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 hairydogm-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 hairydogm-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hairydogm-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 hairydogm-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/filters.base.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/filters.callback_data.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/filters.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/i18n.context.rst
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/i18n.core.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/i18n.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/keyboard.rst
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 hairydogm-0.3.0/docs/source/mixins.rst
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/__init__.py
+-rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/chat_action.py
+-rw-r--r--   0        0        0    13849 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/keyboard.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/mixins.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/filters/__init__.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/filters/base.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/filters/callback_data.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/i18n/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/i18n/context.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 hairydogm-0.3.0/src/hairydogm/i18n/core.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hairydogm-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hairydogm-0.3.0/LICENSE
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hairydogm-0.3.0/README.md
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 hairydogm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 hairydogm-0.3.0/PKG-INFO
```

### Comparing `hairydogm-0.2.7/.pre-commit-config.yaml` & `hairydogm-0.3.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
-    hooks:
-      - id: check-merge-conflict
-      - id: detect-private-key
-      - id: end-of-file-fixer
-      - id: trailing-whitespace
-      - id: mixed-line-ending
-      - id: check-toml
-      - id: check-yaml
+    - repo: https://github.com/pre-commit/pre-commit-hooks
+      rev: v4.5.0
+      hooks:
+          - id: check-merge-conflict
+          - id: detect-private-key
+          - id: end-of-file-fixer
+          - id: trailing-whitespace
+          - id: mixed-line-ending
+          - id: check-toml
+          - id: check-yaml
 
-  - repo: https://github.com/numpy/numpydoc
-    rev: v1.6.0
-    hooks:
-      - id: numpydoc-validation
+    - repo: https://github.com/numpy/numpydoc
+      rev: v1.7.0
+      hooks:
+          - id: numpydoc-validation
 
-  - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
-    hooks:
-      - id: ruff-format
-      - id: ruff
-        args: [--fix, --exit-non-zero-on-fix]
+    - repo: https://github.com/astral-sh/ruff-pre-commit
+      rev: v0.4.4
+      hooks:
+          - id: ruff-format
+          - id: ruff
+            args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `hairydogm-0.2.7/.github/workflows/python-publish.yml` & `hairydogm-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hairydogm-0.2.7/docs/Makefile` & `hairydogm-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hairydogm-0.2.7/docs/source/conf.py` & `hairydogm-0.3.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-import datetime
+# SPDX-License-Identifier: BSD-3-Clause
+# Copyright (c) 2024 Hitalo M. <https://github.com/HitaloM>
+
 import sys
+from datetime import UTC, datetime
 from pathlib import Path
 
 docs_dir = Path(__file__).parent.parent
 sys.path.insert(0, Path("../../src").resolve().as_posix())
 
 import hairydogm  # noqa: E402
 
 project = "hairydogm"
 author = "Hitalo M."
-copyright = f"{datetime.date.today().year}, {author}"
+date_time = datetime.now(tz=UTC)
+date = date_time.date()
+copyright = f"{date.year}, {author}"
 release = hairydogm.__version__
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
@@ -44,17 +49,15 @@
 
 napoleon_use_admonition_for_examples = True
 
 autodoc_typehints = "none"
 
 html_theme = "furo"
 html_title = f"{project} Docs - {release}"
-html_last_updated_fmt = (
-    f"{datetime.datetime.now(tz=datetime.UTC).strftime('%d/%m/%Y, %H:%M:%S')} UTC"
-)
+html_last_updated_fmt = f"{date_time.strftime("%d/%m/%Y, %H:%M:%S")} UTC"
 html_copy_source = False
 
 html_theme_options = {
     "navigation_with_keys": True,
     "footer_icons": [  # these icons are getten from: https://react-icons.github.io/react-icons/
         {
             "name": "Telegram Channel",
```

### Comparing `hairydogm-0.2.7/src/hairydogm/keyboard.py` & `hairydogm-0.3.0/src/hairydogm/keyboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2017-2023 Alex Root Junior <https://github.com/JrooTJunior>
 # Copyright (c) 2023-present Hitalo M. <https://github.com/HitaloM>
 
 from __future__ import annotations
 
-from collections.abc import Generator
 from copy import deepcopy
 from itertools import chain, cycle
 from typing import (
+    TYPE_CHECKING,
     Any,
     Generic,
     TypeVar,
     cast,
 )
 
 from hydrogram.types import (
     InlineKeyboardButton,
     InlineKeyboardMarkup,
 )
 
 from hairydogm.filters.callback_data import CallbackData
 
+if TYPE_CHECKING:
+    from collections.abc import Generator
+
 ButtonType = TypeVar("ButtonType", bound=InlineKeyboardButton)
 T = TypeVar("T")
 
 
 class InlineKeyboardBuilder(Generic[ButtonType]):
     """
     A builder class for creating inline keyboards.
@@ -47,15 +50,15 @@
 
     def __init__(
         self,
         button_type: type[ButtonType] = InlineKeyboardButton,
         markup: list[list[ButtonType]] | None = None,
     ) -> None:
         self._button_type: type[ButtonType] = button_type
-        self._markup: list[list[ButtonType]] = markup if markup else []
+        self._markup: list[list[ButtonType]] = markup or []
         if markup:
             self._validate_markup(markup)
 
     @property
     def buttons(self) -> Generator[ButtonType, None, None]:
         """
         A generator that yields all the buttons in the keyboard.
@@ -85,17 +88,16 @@
         Raises
         ------
         ValueError
             If the button is not of the correct type.
         """
         allowed = self._button_type
         if not isinstance(button, allowed):
-            raise ValueError(
-                f"{button!r} should be type {allowed.__name__!r} not {type(button).__name__!r}"
-            )
+            msg = f"{button!r} should be type {allowed.__name__!r} not {type(button).__name__!r}"
+            raise ValueError(msg)
 
     def _validate_buttons(self, *buttons: ButtonType) -> bool:
         """
         Validate if a list of buttons are of the correct type.
 
         This method checks if a list of buttons are of the correct type.
         It iterates over each button in the list and calls the `_validate_button`
@@ -128,20 +130,22 @@
 
         Raises
         ------
         ValueError
             If the row is not of the correct type or length.
         """
         if not isinstance(row, list):
-            raise ValueError(
+            msg = (
                 f"Row {row!r} should be type 'List[{self._button_type.__name__}]' "
                 f"not type {type(row).__name__}"
             )
+            raise ValueError(msg)
         if len(row) > self.max_width:
-            raise ValueError(f"Row {row!r} is too long (max width: {self.max_width})")
+            msg = f"Row {row!r} is too long (max width: {self.max_width})"
+            raise ValueError(msg)
         self._validate_buttons(*row)
 
     def _validate_markup(self, markup: list[list[ButtonType]]) -> None:
         """
         Validate if the markup of the keyboard is of the correct type and structure.
 
         This method validates if the markup of the keyboard is of the correct type and structure.
@@ -154,21 +158,23 @@
 
         Raises
         ------
         ValueError
             If the markup is not of the correct type or structure.
         """
         if not isinstance(markup, list):
-            raise ValueError(
+            msg = (
                 f"Markup should be type 'List[List[{self._button_type.__name__}]]' "
                 f"not type {type(markup).__name__!r}"
             )
+            raise ValueError(msg)
         count = sum(len(row) for row in markup)
         if count > self.max_buttons:
-            raise ValueError(f"Too much buttons detected Max allowed count - {self.max_buttons}")
+            msg = f"Too much buttons detected Max allowed count - {self.max_buttons}"
+            raise ValueError(msg)
         for row in markup:
             self._validate_row(row)
 
     def _validate_size(self, size: Any) -> None:
         """
         Validate if a size is a valid row size.
 
@@ -182,19 +188,19 @@
 
         Raises
         ------
         ValueError
             If the size is not a valid row size.
         """
         if not isinstance(size, int):
-            raise ValueError("Only int sizes are allowed")
+            msg = "Only int sizes are allowed"
+            raise ValueError(msg)
         if size not in range(self.min_width, self.max_width + 1):
-            raise ValueError(
-                f"Row size {size} is not allowed, range: [{self.min_width}, {self.max_width}]"
-            )
+            msg = f"Row size {size} is not allowed, range: [{self.min_width}, {self.max_width}]"
+            raise ValueError(msg)
 
     def copy(self: InlineKeyboardBuilder[ButtonType]) -> InlineKeyboardBuilder[ButtonType]:
         """
         Create a copy of the current InlineKeyboardBuilder instance.
 
         This method creates a new instance of the InlineKeyboardBuilder class with the
         same button type and markup as the current instance.
@@ -404,13 +410,14 @@
 
         Raises
         ------
         ValueError
             If the button types of the builders do not match.
         """
         if builder._button_type is not self._button_type:
-            raise ValueError(
+            msg = (
                 f"Only builders with same button type can be attached, "
                 f"not {self._button_type.__name__} and {builder._button_type.__name__}"
             )
+            raise ValueError(msg)
         self._markup.extend(builder.export())
         return self
```

### Comparing `hairydogm-0.2.7/src/hairydogm/mixins.py` & `hairydogm-0.3.0/src/hairydogm/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,16 @@
 
         Raises
         ------
         TypeError
             If the provided value is not an instance of the expected type.
         """
         if not isinstance(value, cls):
-            raise TypeError(
-                f"Value should be instance of {cls.__name__!r} not {type(value).__name__!r}"
-            )
+            msg = f"Value should be instance of {cls.__name__!r} not {type(value).__name__!r}"
+            raise TypeError(msg)
         return cls.__context_instance.set(value)  # type: ignore
 
     @classmethod
     def reset_current(cls, token: contextvars.Token[ContextInstance]) -> None:
         """
         Reset the current context instance.
```

### Comparing `hairydogm-0.2.7/src/hairydogm/filters/base.py` & `hairydogm-0.3.0/src/hairydogm/filters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
         -------
         str
             A string representation of the filter signature.
         """
         items = [repr(arg) for arg in args]
         items.extend([f"{k}={v!r}" for k, v in kwargs.items() if v is not None])
 
-        return f"{type(self).__name__}({', '.join(items)})"
+        return f"{type(self).__name__}({", ".join(items)})"
```

### Comparing `hairydogm-0.2.7/src/hairydogm/filters/callback_data.py` & `hairydogm-0.3.0/src/hairydogm/filters/callback_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,24 @@
     Any,
     ClassVar,
     Literal,
     TypeVar,
 )
 from uuid import UUID
 
-from hydrogram import Client
 from hydrogram.types import CallbackQuery
-from magic_filter import MagicFilter
 from pydantic import BaseModel
-from pydantic.fields import FieldInfo
 
 from hairydogm.filters.base import BaseFilter
 
+if typing.TYPE_CHECKING:
+    from hydrogram import Client
+    from magic_filter import MagicFilter
+    from pydantic.fields import FieldInfo
+
 T = TypeVar("T", bound="CallbackData")
 
 MAX_CALLBACK_LENGTH: int = 64
 
 
 class CallbackData(BaseModel):
     """
@@ -44,29 +46,30 @@
     """
 
     __separator__: ClassVar[str]
     __prefix__: ClassVar[str]
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         if "prefix" not in kwargs:
-            raise ValueError(
+            msg = (
                 f"prefix required, usage example: "
                 f"`class {cls.__name__}(CallbackData, prefix='my_callback'): ...`"
             )
+            raise ValueError(msg)
         separator = kwargs.get("sep", ":")
         prefix = kwargs.get("prefix")
         if separator in prefix:
-            raise ValueError(
-                f"Separator symbol {separator!r} can not be used " f"inside prefix {prefix!r}"
-            )
+            msg = f"Separator symbol {separator!r} can not be used " f"inside prefix {prefix!r}"
+            raise ValueError(msg)
         cls.__separator__ = kwargs.pop("sep", ":")
         cls.__prefix__ = kwargs.pop("prefix")
         super().__init_subclass__(**kwargs)
 
-    def _encode_value(self, key: str, value: Any) -> str:
+    @staticmethod
+    def _encode_value(key: str, value: Any) -> str:
         """
         Encode the value to a string representation.
 
         This method is used to encode the value to a string representation.
 
         Parameters
         ----------
@@ -98,19 +101,20 @@
             float: str,
             Decimal: str,
             Fraction: str,
         }
 
         try:
             return type_to_str[type(value)](value)
-        except KeyError:
-            raise ValueError(
+        except KeyError as err:
+            msg = (
                 f"Attribute {key}={value!r} of type {type(value).__name__!r}"
                 f" can not be packed to callback data"
             )
+            raise ValueError(msg) from err
 
     def pack(self) -> str:
         """
         Generate callback data string.
 
         This method is used to generate callback data string.
 
@@ -125,25 +129,27 @@
             If the resulted callback data is too long.
         """
 
         result = [self.__prefix__]
         for key, value in self.model_dump(mode="json").items():
             encoded = self._encode_value(key, value)
             if self.__separator__ in encoded:
-                raise ValueError(
+                msg = (
                     f"Separator symbol {self.__separator__!r} can not be used "
                     f"in value {key}={encoded!r}"
                 )
+                raise ValueError(msg)
             result.append(encoded)
         callback_data = self.__separator__.join(result)
         if len(callback_data.encode()) > MAX_CALLBACK_LENGTH:
-            raise ValueError(
+            msg = (
                 f"Resulted callback data is too long! "
                 f"len({callback_data!r}.encode()) > {MAX_CALLBACK_LENGTH}"
             )
+            raise ValueError(msg)
         return callback_data
 
     @classmethod
     def unpack(cls: type[T], value: str | bytes) -> T:
         """
         Parse callback data string.
 
@@ -167,26 +173,29 @@
         ValueError
             If the prefix in the callback data does not match the prefix in CallbackData.
         """
 
         prefix, *parts = str(value).split(cls.__separator__)
         names = cls.model_fields.keys()
         if len(parts) != len(names):
-            raise TypeError(
+            msg = (
                 f"Callback data {cls.__name__!r} takes {len(names)} arguments "
                 f"but {len(parts)} were given"
             )
+            raise TypeError(msg)
         if prefix != cls.__prefix__:
-            raise ValueError(f"Bad prefix ({prefix!r} != {cls.__prefix__!r})")
+            msg = f"Bad prefix ({prefix!r} != {cls.__prefix__!r})"
+            raise ValueError(msg)
 
         nullable_fields = {
             k for k, field in cls.model_fields.items() if _check_field_is_nullable(field)
         }
         payload = {
-            k: v if v != "" or k not in nullable_fields else None for k, v in zip(names, parts)
+            k: v if v or k not in nullable_fields else None
+            for k, v in zip(names, parts, strict=False)
         }
 
         return cls(**payload)
 
     @classmethod
     def filter(cls, rule: MagicFilter | None = None) -> CallbackQueryFilter:
         """
```

### Comparing `hairydogm-0.2.7/src/hairydogm/i18n/context.py` & `hairydogm-0.3.0/src/hairydogm/i18n/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
     Raises
     ------
     LookupError
         If the I18n context is not set.
     """
     if (i18n := I18n.get_current(no_error=True)) is None:
-        raise LookupError("I18n context is not set")
+        msg = "I18n context is not set"
+        raise LookupError(msg)
     return i18n
 
 
 def gettext(*args: Any, **kwargs: Any) -> str:
     """
     Get the translated string for the given message.
```

### Comparing `hairydogm-0.2.7/src/hairydogm/i18n/core.py` & `hairydogm-0.3.0/src/hairydogm/i18n/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,16 @@
                 continue
 
             mo_path = locale_path / "LC_MESSAGES" / f"{self.domain}.mo"
             if mo_path.exists():
                 with mo_path.open("rb") as fp:
                     translations[name] = gettext.GNUTranslations(fp)
             elif mo_path.with_suffix(".po").exists():
-                raise RuntimeError(f"Found locale '{name}' but this language is not compiled!")
+                msg = f"Found locale '{name}' but this language is not compiled!"
+                raise RuntimeError(msg)
 
         return translations
 
     def reload(self) -> None:
         """
         Reload the locales for the i18n core.
```

### Comparing `hairydogm-0.2.7/LICENSE` & `hairydogm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hairydogm-0.2.7/pyproject.toml` & `hairydogm-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "hairydogm"
 dynamic = ["version"]
 description = "Some utilities from AIOgram adapted to be used with Hydrogram."
 authors = [{ name = "Hitalo" }]
 dependencies = [
     "hydrogram>=0.1.4",
-    "babel>=2.14.0",
+    "babel>=2.15.0",
     "magic-filter>=1.0.12",
-    "pydantic>=2.5.3",
+    "pydantic>=2.7.1",
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.12"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -34,59 +34,78 @@
 tracker = "https://github.com/HitaloM/hairydogm/issues"
 community = "https://t.me/HitaloProjects"
 source = "https://github.com/HitaloM/hairydogm"
 documentation = "https://hairydogm.readthedocs.io/"
 
 [project.optional-dependencies]
 docs = [
-    "Sphinx>=7.2.6",
-    "furo>=2023.9.10",
-    "sphinx-autobuild>=2021.3.14",
+    "Sphinx>=7.3.7",
+    "furo>=2024.5.6",
+    "sphinx-autobuild>=2024.4.16",
     "sphinx-copybutton>=0.5.2",
-    "pygments>=2.17.2",
+    "pygments>=2.18.0",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
-dev-dependencies = ["pre-commit>=3.6.0", "ruff>=0.1.14"]
+dev-dependencies = ["pre-commit>=3.7.1", "ruff>=0.4.4"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.ruff]
 line-length = 99
 target-version = "py312"
+
+[tool.ruff.lint]
 select = [
-    "I",    # isort
+    "B",    # flake8-bugbear
+    "C4",   # flake8-comprehensions
+    "C90",  # mccabe
+    "CPY",  # flake8-copyright
+    "DTZ",  # flake8-datetimez
     "E",    # pycodestyle
-    "W",    # pycodestyle
-    "UP",   # pyupgrade
+    "EM",   # flake8-errmsg
     "F",    # pyflakes
-    "PERF", # perflint
+    "FURB", # refurb
+    "G",    # flake8-logging-format
+    "I",    # isort
     "N",    # pep8-naming
+    "PERF", # perflint
+    "PL",   # pylint
+    "PTH",  # flake8-use-pathlib
+    "RET",  # flake8-return
     "RUF",  # ruff
-    "FURB", # refurb
     "SIM",  # flake8-simplify
-    "RET",  # flake8-return
-    "C4",   # flake8-comprehensions
-    "PTH",  # flake8-use-pathlib
-    "G",    # flake8-logging-format
+    "TCH",  # flake8-type-checking
     "TID",  # flake8-tidy-imports
+    "UP",   # pyupgrade
+    "W",    # pycodestyle
+]
+ignore = [
+    "RUF001",
+    "RUF002",
+    "RUF003",
+    "PLR0913",
+    "PLR2004",
+    "PLW2901",
+    "PLW1641",
 ]
 preview = true
 
-[tool.ruff.isort]
-known-first-party = ["src"]
-
 [tool.ruff.format]
 docstring-code-format = true
+preview = true
+
+[tool.ruff.lint.isort]
+known-first-party = ["src"]
 
 [tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/hairydogm"]
```

### Comparing `hairydogm-0.2.7/PKG-INFO` & `hairydogm-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hairydogm
-Version: 0.2.7
+Version: 0.3.0
 Summary: Some utilities from AIOgram adapted to be used with Hydrogram.
 Project-URL: homepage, https://github.com/HitaloM/hairydogm
 Project-URL: tracker, https://github.com/HitaloM/hairydogm/issues
 Project-URL: community, https://t.me/HitaloProjects
 Project-URL: source, https://github.com/HitaloM/hairydogm
 Project-URL: documentation, https://hairydogm.readthedocs.io/
 Author: Hitalo
@@ -35,24 +35,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.12
-Requires-Dist: babel>=2.14.0
+Requires-Dist: babel>=2.15.0
 Requires-Dist: hydrogram>=0.1.4
 Requires-Dist: magic-filter>=1.0.12
-Requires-Dist: pydantic>=2.5.3
+Requires-Dist: pydantic>=2.7.1
 Provides-Extra: docs
-Requires-Dist: furo>=2023.9.10; extra == 'docs'
-Requires-Dist: pygments>=2.17.2; extra == 'docs'
-Requires-Dist: sphinx-autobuild>=2021.3.14; extra == 'docs'
+Requires-Dist: furo>=2024.5.6; extra == 'docs'
+Requires-Dist: pygments>=2.18.0; extra == 'docs'
+Requires-Dist: sphinx-autobuild>=2024.4.16; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
-Requires-Dist: sphinx>=7.2.6; extra == 'docs'
+Requires-Dist: sphinx>=7.3.7; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # hairydogm
 
 Hairydogm is a library that brings some of the powerful features of [AIOgram](https://github.com/aiogram/aiogram) to [Hydrogram](https://github.com/Hydrogram/Hydrogram). It is named "hairydogm" as an anagram of "Hydrogram" and "AIOgram".
 
 Primarily designed to be used in:
```

