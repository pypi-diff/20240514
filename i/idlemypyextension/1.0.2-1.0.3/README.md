# Comparing `tmp/idlemypyextension-1.0.2.tar.gz` & `tmp/idlemypyextension-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idlemypyextension-1.0.2.tar", last modified: Mon Mar 11 08:24:45 2024, max compression
+gzip compressed data, was "idlemypyextension-1.0.3.tar", last modified: Tue May 14 01:15:32 2024, max compression
```

## Comparing `idlemypyextension-1.0.2.tar` & `idlemypyextension-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:24:45.619375 idlemypyextension-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46456 2024-03-11 08:24:45.619375 idlemypyextension-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 08:24:45.619375 idlemypyextension-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:24:45.611375 idlemypyextension-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:24:45.615375 idlemypyextension-1.0.2/src/idlemypyextension/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31106 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18701 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/ast_annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24117 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/moduleguard.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/tktrio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20762 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/src/idlemypyextension/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:24:45.619375 idlemypyextension-1.0.2/src/idlemypyextension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46456 2024-03-11 08:24:45.000000 idlemypyextension-1.0.2/src/idlemypyextension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-11 08:24:45.000000 idlemypyextension-1.0.2/src/idlemypyextension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 08:24:45.000000 idlemypyextension-1.0.2/src/idlemypyextension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-11 08:24:45.000000 idlemypyextension-1.0.2/src/idlemypyextension.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-11 08:24:45.000000 idlemypyextension-1.0.2/src/idlemypyextension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 08:24:45.000000 idlemypyextension-1.0.2/src/idlemypyextension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 08:24:45.619375 idlemypyextension-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    25979 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-11 08:24:41.000000 idlemypyextension-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:15:32.118843 idlemypyextension-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46457 2024-05-14 01:15:32.118843 idlemypyextension-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 01:15:32.118843 idlemypyextension-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:15:32.110843 idlemypyextension-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:15:32.114843 idlemypyextension-1.0.3/src/idlemypyextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33058 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18701 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/ast_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/moduleguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/tktrio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20762 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/src/idlemypyextension/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:15:32.118843 idlemypyextension-1.0.3/src/idlemypyextension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46457 2024-05-14 01:15:32.000000 idlemypyextension-1.0.3/src/idlemypyextension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-14 01:15:32.000000 idlemypyextension-1.0.3/src/idlemypyextension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 01:15:32.000000 idlemypyextension-1.0.3/src/idlemypyextension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 01:15:32.000000 idlemypyextension-1.0.3/src/idlemypyextension.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 01:15:32.000000 idlemypyextension-1.0.3/src/idlemypyextension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-14 01:15:32.000000 idlemypyextension-1.0.3/src/idlemypyextension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 01:15:32.114843 idlemypyextension-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    26591 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-14 01:15:27.000000 idlemypyextension-1.0.3/tests/test_utils.py
```

### Comparing `idlemypyextension-1.0.2/LICENSE` & `idlemypyextension-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/PKG-INFO` & `idlemypyextension-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlemypyextension
-Version: 1.0.2
+Version: 1.0.3
 Summary: Mypy daemon extension for Python IDLE
 Author-email: CoolCat467 <CoolCat467@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,16 +696,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: IDLE
 Classifier: Framework :: Trio
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mypy~=1.9.0
-Requires-Dist: trio~=0.24.0
+Requires-Dist: mypy~=1.10.0
+Requires-Dist: trio~=0.25.0
 Requires-Dist: mttkinter~=0.6.1
 Provides-Extra: user
 Requires-Dist: idleuserextend~=0.0.1; extra == "user"
 
 # IdleMypyExtension
 Python IDLE extension to perform mypy analysis on an open file
```

### Comparing `idlemypyextension-1.0.2/README.md` & `idlemypyextension-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/pyproject.toml` & `idlemypyextension-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     "Operating System :: OS Independent",
     "Framework :: IDLE",
     "Framework :: Trio",
     "Typing :: Typed",
 ]
 keywords = ["mypy", "dmypy", "idle", "extension", "development", "daemon"]
 dependencies = [
-    "mypy~=1.9.0",
-    "trio~=0.24.0",
+    "mypy~=1.10.0",
+    "trio~=0.25.0",
     "mttkinter~=0.6.1",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "idlemypyextension.__init__.__version__"}
 
 [project.optional-dependencies]
```

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/__init__.py` & `idlemypyextension-1.0.3/src/idlemypyextension/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 __title__ = "idlemypyextension"
 __author__ = "CoolCat467"
 __license__ = "GNU General Public License Version 3"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 
 from idlemypyextension import utils
 from idlemypyextension.extension import idlemypyextension as idlemypyextension
 
 
 def check_installed() -> bool:
```

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/annotate.py` & `idlemypyextension-1.0.3/src/idlemypyextension/annotate.py`

 * *Files 8% similar despite different names*

```diff
@@ -527,14 +527,16 @@
         args.append(get_typevalue_repr(arg, ignore_modules))
     if not args:
         if name:
             return name
         return "[]"
     if name == "Union":
         return " | ".join(args)
+    if name == "__hacks_DictItem":
+        return ": ".join(args)
     values = ", ".join(args)
     return f"{name}[{values}]"
 
 
 class TypeValue:
     """A type value, potentially collection of multiple."""
 
@@ -592,18 +594,55 @@
         types = []
         while self.lookup() not in (")", "]"):
             typ = self.parse_type()
             types.append(typ)
             string = self.lookup()
             if string == ",":
                 self.expect(",")
-            elif string not in {")", "]"}:
-                self.fail(f"Expected ) or ], got {string!r}")
+                continue
+            self.expect_option((")", "]"))
+            self.back()
         return types
 
+    def parse_type_dict_or_set(self) -> list[TypeValue]:
+        """Parse dict or set type list."""
+        types = []
+        # 0 -> Unknown
+        # 1 -> dict
+        # 2 -> set
+        which = 0
+        while self.lookup() != "}":
+            typ = self.parse_type()
+            if which == 0:
+                which = 1 if self.lookup() == ":" else 2
+            if which == 1:  # dict
+                self.expect(":")
+                types.append(
+                    TypeValue("__hacks_DictItem", (typ, self.parse_type())),
+                )
+            if which == 2:  # set
+                types.append(typ)
+            if self.lookup() == ",":
+                self.expect(",")
+                continue
+            self.expect("}")
+            self.back()
+        return types
+
+    def parse_type_collection(self, start_collection: str) -> list[TypeValue]:
+        """Parse default argument type list."""
+        if start_collection in ("(", "["):
+            return self.parse_type_list()
+        if start_collection == "{":
+            return self.parse_type_dict_or_set()
+        # Fail is a NoReturn, making RET503 irrelevant
+        self.fail(  # pragma: nocover  # noqa: RET503
+            "Unhandled collection start: {start_collection!r}",
+        )
+
     def parse_union_list(self) -> list[TypeValue]:
         """Parse | separated union list."""
         types = []
         while True:
             typ = self.parse_single()
             types.append(typ)
             if self.lookup() != "|":
@@ -698,14 +737,23 @@
 
     def next(self) -> Token:
         """Get next token."""
         token = self.peek()
         self.i += 1
         return token
 
+    def expect_option(self, options: Collection[str]) -> str:
+        """Expect next token text to be one of options. Return matching text."""
+        got = self.next().text
+        if got not in options:
+            expected = list_or(tuple(map(repr, options)))
+            self.fail(f"Expected {expected}, got {got!r}")
+        assert got is not None
+        return got
+
     def expect(self, text: str) -> None:
         """Expect next token text to be text."""
         got = self.next().text
         if got != text:
             self.fail(f"Expected {text!r}, got {got!r}")
 
     def expect_type(
@@ -865,16 +913,23 @@
                     type_value,
                     ignore_modules,
                 )
             if isinstance(parser.peek(), DefaultDef):
                 parser.expect("=")
                 type_text += " = "
                 if isinstance(parser.peek(), EndSeparator):
-                    type_text += f"{parser.next().text}"
-                    type_text += ", ".join(map(str, parser.parse_type_list()))
+                    start_collection = parser.next().text
+                    assert start_collection is not None
+                    type_text += start_collection
+                    type_text += ", ".join(
+                        map(
+                            str,
+                            parser.parse_type_collection(start_collection),
+                        ),
+                    )
                     type_text += f"{parser.next().text}"
                 else:
                     type_text += str(parser.parse_type())
             # debug(f"{name}{type_text}")
             new_lines += f"{name}{type_text}"
             argument += 1
             arg_place += 1
```

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/ast_annotate.py` & `idlemypyextension-1.0.3/src/idlemypyextension/ast_annotate.py`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/client.py` & `idlemypyextension-1.0.3/src/idlemypyextension/client.py`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/extension.py` & `idlemypyextension-1.0.3/src/idlemypyextension/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,25 +438,31 @@
             return client.Response(
                 {"out": "", "err": "Error: Could not start mypy daemon"},
             )
         flags = self.flags
         flags += [file]
         # debug(f"check {flags = }")
         command = " ".join(
-            [
+            x
+            for x in [
                 "dmypy",
                 f'--status-file="{self.status_file}"',
                 "run",
-                f"--timeout={self.daemon_timeout}",
+                (
+                    f"--timeout={self.action_timeout}"
+                    if self.action_timeout
+                    else ""
+                ),
                 f'--log-file="{self.log_file}"',
                 "--export-types",
                 f'"{file}"',
                 "--",
                 *self.flags,
-            ],
+            ]
+            if x
         )
         debug(f"{command = }")
         return await client.run(
             self.status_file,
             flags=flags,
             timeout=self.action_timeout,
             daemon_timeout=self.daemon_timeout,
@@ -749,9 +755,23 @@
         self.reload()
 
         # Find comment
         self.find_next_extension_comment(self.search_wrap == "True")
 
         return "break"
 
-    # def close(self) -> None:
-    #    """Called when any idle editor window closes"""
+    def unregister_async_events(self) -> None:
+        """Unregister asynchronous event handlers."""
+        for attr_name in dir(self):
+            if attr_name.startswith("_"):
+                continue
+            if attr_name.endswith("_event_async"):
+                bind_name = "-".join(attr_name.split("_")[:-2]).lower()
+                self.text.event_delete(f"<<{bind_name}>>")
+
+    def close(self) -> None:
+        """Extension cleanup before IDLE window closes."""
+        # Wrapped in try except so failure doesn't cause zombie windows.
+        try:
+            self.unregister_async_events()
+        except Exception as exc:
+            traceback.print_exception(exc)
```

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/moduleguard.py` & `idlemypyextension-1.0.3/src/idlemypyextension/moduleguard.py`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/tktrio.py` & `idlemypyextension-1.0.3/src/idlemypyextension/tktrio.py`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension/utils.py` & `idlemypyextension-1.0.3/src/idlemypyextension/utils.py`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension.egg-info/PKG-INFO` & `idlemypyextension-1.0.3/src/idlemypyextension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlemypyextension
-Version: 1.0.2
+Version: 1.0.3
 Summary: Mypy daemon extension for Python IDLE
 Author-email: CoolCat467 <CoolCat467@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,16 +696,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: IDLE
 Classifier: Framework :: Trio
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mypy~=1.9.0
-Requires-Dist: trio~=0.24.0
+Requires-Dist: mypy~=1.10.0
+Requires-Dist: trio~=0.25.0
 Requires-Dist: mttkinter~=0.6.1
 Provides-Extra: user
 Requires-Dist: idleuserextend~=0.0.1; extra == "user"
 
 # IdleMypyExtension
 Python IDLE extension to perform mypy analysis on an open file
```

### Comparing `idlemypyextension-1.0.2/src/idlemypyextension.egg-info/SOURCES.txt` & `idlemypyextension-1.0.3/src/idlemypyextension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idlemypyextension-1.0.2/tests/test_annotate.py` & `idlemypyextension-1.0.3/tests/test_annotate.py`

 * *Files 4% similar despite different names*

```diff
@@ -590,14 +590,32 @@
                 "dots and boxes:Sequence[dots and boxes.Sequence[int]]",
                 "dots and boxes:Sequence[dots and boxes.Sequence[int]]",
             ],
             "dots and boxes:Generator[dots and boxes.Action, None, None]",
             "def valid_moves(turn: bool, lines: Sequence[Sequence[int]], boxes: Sequence[Sequence[int]]) -> Generator[Action, None, None]:",
             "dots and boxes",
         ),
+        (
+            """def bad_default_arg(name_map = {"jerald": "cat", "luigi": "person"}):""",
+            [
+                "dict[str, str]",
+            ],
+            "str",
+            """def bad_default_arg(name_map: dict[str, str] = {"jerald": "cat", "luigi": "person"}) -> str:""",
+            None,
+        ),
+        (
+            """def bad_default_arg(name_map = {"jerald", "cat", "bob"}):""",
+            [
+                "set[str]",
+            ],
+            "str",
+            """def bad_default_arg(name_map: set[str] = {"jerald", "cat", "bob"}) -> str:""",
+            None,
+        ),
     ],
 )
 def test_get_annotation(
     function_text: str,
     arg_types: Sequence[str],
     return_type: str,
     result: str,
@@ -758,15 +776,15 @@
 
 def test_parse_type_list_no_close_failure() -> None:
     parser = annotate.Parser(
         [annotate.DottedName("int"), annotate.Separator("notend")],
     )
     with pytest.raises(
         annotate.ParseError,
-        match="Expected \\) or \\], got 'notend'",
+        match="Expected '\\)' or '\\]', got 'notend'",
     ):
         parser.parse_type_list()
 
 
 def test_parse_union_list() -> None:
     parser = annotate.Parser(
         [
```

### Comparing `idlemypyextension-1.0.2/tests/test_utils.py` & `idlemypyextension-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

