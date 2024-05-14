# Comparing `tmp/tableofcontents-2.6.0.tar.gz` & `tmp/tableofcontents-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableofcontents-2.6.0.tar", last modified: Sat Mar 16 21:35:02 2024, max compression
+gzip compressed data, was "tableofcontents-2.7.0.tar", last modified: Tue May 14 07:32:55 2024, max compression
```

## Comparing `tableofcontents-2.6.0.tar` & `tableofcontents-2.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:35:02.078689 tableofcontents-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-16 21:35:02.078689 tableofcontents-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 21:35:02.078689 tableofcontents-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:35:02.078689 tableofcontents-2.6.0/tableofcontents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-16 21:35:02.000000 tableofcontents-2.6.0/tableofcontents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-16 21:35:02.000000 tableofcontents-2.6.0/tableofcontents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 21:35:02.000000 tableofcontents-2.6.0/tableofcontents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-16 21:35:02.000000 tableofcontents-2.6.0/tableofcontents.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-16 21:35:02.000000 tableofcontents-2.6.0/tableofcontents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-16 21:35:02.000000 tableofcontents-2.6.0/tableofcontents.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:35:02.074689 tableofcontents-2.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/tests/test_toc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 21:35:02.074689 tableofcontents-2.6.0/toc/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/toc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5484 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/toc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    31002 2024-03-16 21:34:51.000000 tableofcontents-2.6.0/toc/toc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:32:55.887897 tableofcontents-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-14 07:32:55.887897 tableofcontents-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:32:55.887897 tableofcontents-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:32:55.887897 tableofcontents-2.7.0/tableofcontents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-14 07:32:55.000000 tableofcontents-2.7.0/tableofcontents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-14 07:32:55.000000 tableofcontents-2.7.0/tableofcontents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:32:55.000000 tableofcontents-2.7.0/tableofcontents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 07:32:55.000000 tableofcontents-2.7.0/tableofcontents.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 07:32:55.000000 tableofcontents-2.7.0/tableofcontents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-14 07:32:55.000000 tableofcontents-2.7.0/tableofcontents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:32:55.883897 tableofcontents-2.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/tests/test_toc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:32:55.887897 tableofcontents-2.7.0/toc/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/toc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5766 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/toc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35130 2024-05-14 07:32:45.000000 tableofcontents-2.7.0/toc/toc.py
```

### Comparing `tableofcontents-2.6.0/LICENSE` & `tableofcontents-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tableofcontents-2.6.0/PKG-INFO` & `tableofcontents-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableofcontents
-Version: 2.6.0
+Version: 2.7.0
 Summary: Generate a table of contents from the comments of a file
 Author: AlphaJack
 Project-URL: Homepage, https://github.com/AlphaJack/toc
 Project-URL: Issues, https://github.com/AlphaJack/toc/issues
 Project-URL: Repository, https://github.com/AlphaJack/toc
 Project-URL: Changelog, https://github.com/AlphaJack/toc/blob/master/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tableofcontents-2.6.0/README.md` & `tableofcontents-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tableofcontents-2.6.0/pyproject.toml` & `tableofcontents-2.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [tool.setuptools]
 packages = ["toc"]
 
 # ################################################################ Project
 
 [project]
 name = "tableofcontents"
-version = "2.6.0"
+version = "2.7.0"
 authors = [
   { name="AlphaJack" },
 ]
 description = "Generate a table of contents from the comments of a file"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `tableofcontents-2.6.0/tableofcontents.egg-info/PKG-INFO` & `tableofcontents-2.7.0/tableofcontents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableofcontents
-Version: 2.6.0
+Version: 2.7.0
 Summary: Generate a table of contents from the comments of a file
 Author: AlphaJack
 Project-URL: Homepage, https://github.com/AlphaJack/toc
 Project-URL: Issues, https://github.com/AlphaJack/toc/issues
 Project-URL: Repository, https://github.com/AlphaJack/toc
 Project-URL: Changelog, https://github.com/AlphaJack/toc/blob/master/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tableofcontents-2.6.0/tests/test_cli.py` & `tableofcontents-2.7.0/tests/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # current directory
 from pathlib import Path
 
 # load local module rather than system installed version
 import sys
 
 project_root = Path(__file__).resolve().parent.parent
-sys.path.insert(0, project_root)
+sys.path.insert(0, str(project_root))
 
 # module to test
 from toc.cli import main
 
 # from toc.__version__ import __version__
 
 # ################################################################ TEST CLASSES
@@ -120,14 +120,55 @@
             with patch.object(sys, "argv", test_args):
                 output = StringIO()
                 with redirect_stdout(output):
                     main()
                     print("output: '" + output.getvalue() + "'")
                     self.assertIn("Contents of stdin.html", output.getvalue())
 
+    def test_depth(self):
+        test_args = [f"{self.p / 'toc' / 'cli.py'}", "-e", "html", "-d", "1", "-"]
+        stdin_content = """
+<html>
+<html>
+<h1>Title</h1>
+<h2>Subtitle</h2>
+</html>
+"""
+        with patch("sys.stdin", StringIO(stdin_content)):
+            with patch.object(sys, "argv", test_args):
+                output = StringIO()
+                with redirect_stdout(output):
+                    main()
+                    print("output: '" + output.getvalue() + "'")
+                    self.assertNotIn("Subtitle", output.getvalue())
+
+    def test_line_numbers_html(self):
+        test_args = [f"{self.p / 'toc' / 'cli.py'}", "-e", "html", "-n", "-"]
+        stdin_content = "<h1>Title</h1>"
+        with patch("sys.stdin", StringIO(stdin_content)):
+            with patch.object(sys, "argv", test_args):
+                output = StringIO()
+                with redirect_stdout(output):
+                    main()
+                    print("output: '" + output.getvalue() + "'")
+                    self.assertIn("Title 1", output.getvalue())
+
+    def test_line_numbers_generic(self):
+        test_args = [f"{self.p / 'toc' / 'cli.py'}", "-e", "tex", "-n", "-"]
+        stdin_content = """
+% ################################################################ Preamble
+"""
+        with patch("sys.stdin", StringIO(stdin_content)):
+            with patch.object(sys, "argv", test_args):
+                output = StringIO()
+                with redirect_stdout(output):
+                    main()
+                    print("output: '" + output.getvalue() + "'")
+                    self.assertIn("Preamble 2", output.getvalue())
+
     def test_output(self):
         test_args = [
             f"{self.p / 'toc' / 'cli.py'}",
             "-o",
             f"{self.o / 'output.txt'}",
             f"{self.p / 'README.md'}",
         ]
```

### Comparing `tableofcontents-2.6.0/tests/test_toc.py` & `tableofcontents-2.7.0/tests/test_toc.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
 # clean output path if existing
 import shutil
 
 # current directory
 from pathlib import Path
 
+# fake files
+from unittest.mock import patch
+
 # load local module rather than system installed version
 import sys
 
 project_root = Path(__file__).resolve().parent.parent
-sys.path.insert(0, project_root)
-
-# fake files
-from unittest.mock import patch, mock_open
+sys.path.insert(0, str(project_root))
 
 # module to test
 from toc.toc import Toc
 
 # ################################################################ TEST CLASSES
 # ################################ SINGLE METHODS
 
@@ -42,23 +42,23 @@
 # example test
 class TestTocMethods(unittest.TestCase):
     def test_set_extension(self):
         test_cases = [
             ("file.c", "c"),
             ("file.ini", "ini"),
             (".", ""),
-            ("./../", "/"),
+            ("./../", ""),
             ("file.unknown", "unknown"),
             ("file.", ""),
         ]
         for input_file, expected_extension in test_cases:
             with self.subTest(
                 input_file=input_file, expected_extension=expected_extension
             ):
-                t = Toc(input_file)
+                t = Toc(Path(input_file))
                 actual_extension = t.extension
                 self.assertEqual(
                     actual_extension,
                     expected_extension,
                     f'Unexpected extension "{actual_extension}" for file "{input_file}"',
                 )
 
@@ -72,15 +72,15 @@
             ("file.", "#"),
             ("file", "#"),
         ]
         for input_file, expected_character in test_cases:
             with self.subTest(
                 input_file=input_file, expected_character=expected_character
             ):
-                t = Toc(input_file)
+                t = Toc(Path(input_file))
                 actual_character = t.set_character()
                 self.assertEqual(
                     actual_character,
                     expected_character,
                     f'Unexpected comment character "{actual_character}" for file "{input_file}"',
                 )
 
@@ -88,47 +88,51 @@
         test_cases = {
             "c": ([], []),
             "css": (["/*"], ["*/"]),
             "ml": (["(*"], ["*)"]),
             "": ([], []),
         }
         for extension, (expected_prefix, expected_suffix) in test_cases.items():
-            t = Toc("mock.txt")
+            input_file = Path("mock.txt")
+            t = Toc(input_file)
             t.extension = extension
             actual_prefix, actual_suffix = t._toc_prefix_suffix()
             comparison = (
                 True
                 if actual_prefix == expected_prefix and actual_suffix == expected_suffix
                 else False
             )
             with self.subTest(comparison=comparison):
                 self.assertTrue(
                     comparison,
                     f'Unexpected prefix or suffix "{actual_prefix, actual_suffix}" for extension "{extension}"',
                 )
 
     def test_process_generic_1(self):
-        t = Toc("mock.txt")
+        input_file = Path("mock.txt")
+        t = Toc(input_file)
         lines = [
             "# ################################################################ Heading 1"
         ]
         expected = ["# ├── Heading 1"]
         result = t._process_generic(lines)
         self.assertEqual(result, expected)
 
     def test_process_generic_2n(self):
-        t = Toc("mock.beancount")
+        input_file = Path("mock.beancount")
+        t = Toc(input_file)
         t.set_character()
         lines = ["*** Transactions"]
         expected = ["; │     └── Transactions"]
         result = t._process_increasing(lines, "*")
         self.assertEqual(result, expected)
 
     def test_prettify_connectors(self):
-        t = Toc("mock.txt")
+        input_file = Path("mock.txt")
+        t = Toc(input_file)
         input_list = [
             "# ├── MODULES",
             "# ├── CLASS",
             "# │  └── PUBLIC METHODS",
             "# │     └── COMMENT CHARACTER",
             "# │     └── TOC OUTPUT",
             "# │        └── STDOUT",
@@ -175,15 +179,16 @@
         self.assertEqual(output_list, expected_list)
 
     def test_read_file(self):
         with patch(
             "builtins.open",
             side_effect=UnicodeDecodeError("utf-8", b"", 1, 2, "mock reason"),
         ):
-            t = Toc("mock.txt")
+            input_file = Path("mock.txt")
+            t = Toc(input_file)
             data = t._read_file()
             self.assertEqual(data, "")
             self.assertEqual(t.err, "binary")
 
 
 # ################################ FILE PROCESSING
 
@@ -214,17 +219,18 @@
             # print("output_file: " + str(output_file))
             # print("reference_file: " + str(reference_file))
             t = Toc(input_file)
             t.set_character()
             t.lineNumbers = True if file.name == "latex_linenumbers.tex" else False
             t.to_file(output_file)
             if output_file.is_file() and reference_file.is_file():
-                with open(output_file, "r") as output, open(
-                    reference_file, "r"
-                ) as reference:
+                with (
+                    open(output_file, "r") as output,
+                    open(reference_file, "r") as reference,
+                ):
                     output_content, reference_content = output.read(), reference.read()
                     comparison = True if output_content == reference_content else False
                     with self.subTest(comparison=comparison):
                         self.assertTrue(
                             comparison,
                             f'Unexpected content (should be different) processing "{file.name}", please run `diff {output_file} {reference_file}`',
                         )
```

### Comparing `tableofcontents-2.6.0/toc/cli.py` & `tableofcontents-2.7.0/toc/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 # heredoc in help epilog
 from argparse import RawDescriptionHelpFormatter
 
 # stderr
 import sys
 
 # glob expansion
-import glob
+# import glob
 
 # version
 from importlib_metadata import version
 
+# robust file handling
+from pathlib import Path
+
 # toc library
 from toc.toc import Toc
 
 # needed for cprofile, pprofile and memray
-#from toc import Toc
+# from toc import Toc
 
 # ################################################################ FUNCTIONS
 # ################################ ARGUMENTS
 
 
 def parse_args():
     # read user-provided arguments
@@ -61,24 +64,25 @@
         epilog=example_usage,
         formatter_class=RawDescriptionHelpFormatter,
     )
     group = parser.add_mutually_exclusive_group()
     parser.add_argument(
         "files",
         nargs="*",
+        type=Path,
         help="files or lists of files to process. use '-' to read from stdin",
     )
     parser.add_argument(
         "-c",
         action="store",
         dest="character",
         type=str,
         help="set an arbitrary comment character (e.g. //)",
     )
-    group.add_argument("-d", "--depth", type=int, help="maximum toc depth")
+    parser.add_argument("-d", "--depth", type=int, help="maximum toc depth")
     parser.add_argument(
         "-e",
         action="store",
         dest="extension",
         type=str,
         help="interpret input as a file with this extension (e.g. html)",
     )
@@ -97,58 +101,61 @@
     parser.add_argument(
         "-n", "--line-numbers", action="store_true", help="print line numbers in toc"
     )
     group.add_argument(
         "-o",
         action="store",
         dest="output_file",
-        type=str,
+        type=Path,
         help="print output to an arbitrary file",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version="%(prog)s " + version("tableofcontents"),
         help="show the current version and exit",
     )
     args = parser.parse_args()
     return args
 
 
-def get_files(args) -> list:
+def get_files(args) -> list[Path]:
     # consider all files as lists
     if args.from_list:
         files = []
         for fileList in args.files:
-            try:
+            # try:
+            if True:
                 with open(fileList, "r") as list_content:
                     for line in list_content.read().splitlines():
-                        if not line.startswith("#"):
+                        if not line.startswith("#") and line != "":
                             # glob expansion
                             files += [
+                                # globMatch for globMatch in glob.glob(line, recursive=True)
                                 globMatch
-                                for globMatch in glob.glob(line, recursive=True)
+                                for globMatch in Path.cwd().glob(line)
+                                if globMatch.exists() and globMatch.is_file()
                             ]
             # cannot open that list
-            except BaseException:
-                print(f'Skipping list "{fileList}"', file=sys.stderr)
+            # except BaseException:
+            #    print(f'Skipping list "{fileList}"', file=sys.stderr)
     # only consider the first file
     elif args.output_file:
         files = [args.files[0]]
     # consider all files
     else:
         files = args.files
     return files
 
 
 # ################################ PROCESS FILE
 
 
-def process_file(inputFile: str, args):
+def process_file(inputFile: Path, args):
     # initialize instance
     t = Toc(inputFile)
     # set comment character and line numbers
     t.extension = args.extension if args.extension else t.extension
     t.character = args.character if args.character else t.set_character()
     t.depth = args.depth if args.depth else t.depth
     t.lineNumbers = args.line_numbers if args.line_numbers else False
```

### Comparing `tableofcontents-2.6.0/toc/toc.py` & `tableofcontents-2.7.0/toc/toc.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,52 +36,106 @@
 
 # regex
 import re
 
 # stderr
 import sys
 
+# files
+from pathlib import Path
+
 
 # ################################################################ CLASSES
 
 
 class Toc:
-    def __init__(
-        self,
-        inputFile: str = "",
-        outputFile: str | None = None,
-        lineNumbers: bool = False,
-        character: str = "#",
-    ):
-        self.inputFile = "stdin" if str(inputFile) == "-" else str(inputFile)
-        self.outputFile = outputFile
-        self.extension = (
-            self.inputFile.split(".")[-1].lower() if "." in self.inputFile else ""
-        )
-        self.lineNumbers = lineNumbers
-        self.character = character
-        self.depth = 0
+    def __init__(self, inputFile: Path):
+        print(f"inputFile: {inputFile}", file=sys.stderr)
+        self.inputFile: Path = inputFile
+        self.outputFile: Path | None = None
+        self.extension: str = self.inputFile.suffix.lower().replace(".", "")
+        self.lineNumbers: bool = False
+        self.updated: bool = False
+        self.character: str = "#"
+        self.depth: int = 0
         self.err: str | None = None
-        self.updated = False
         self.innerTocBegin: str | None = None
         self.innerTocTitle: str | None = None
         self.innerTocEnd: str | None = None
         # n=2**(7−l), l=7−math.log(n,2)
-        self.levels = {64: 1, 32: 2, 16: 3, 8: 4, 4: 5, 2: 6}
+        self.levels: dict[int, int] = {64: 1, 32: 2, 16: 3, 8: 4, 4: 5, 2: 6}
 
     # ################################ PUBLIC METHODS
 
     # ################ COMMENT CHARACTER
 
     def set_character(self) -> str:
         # automatically select the comment type from its extension, if not already set
         match self.extension:
-            case "ad" | "adoc" | "asc" | "asciidoc" | "c" | "carbon" | "cc" | "coffee" | "cpp" | "cs" | "css" | "d" | "dart" | "go" | "h" | "hpp" | "htm" | "html" | "hxx" | "java" | "js" | "jsx" | "kt" | "md" | "mdx" | "qmd" | "rmd" | "pas" | "php" | "pp" | "proto" | "qs" | "rs" | "scala" | "sc" | "swift" | "ts" | "typ" | "xml" | "zig":
+            case (
+                "ad"
+                | "adoc"
+                | "asc"
+                | "asciidoc"
+                | "c"
+                | "carbon"
+                | "cc"
+                | "coffee"
+                | "cpp"
+                | "cs"
+                | "css"
+                | "cu"
+                | "d"
+                | "dart"
+                | "go"
+                | "h"
+                | "hpp"
+                | "htm"
+                | "html"
+                | "hxx"
+                | "java"
+                | "js"
+                | "jsx"
+                | "kt"
+                | "md"
+                | "mdx"
+                | "qmd"
+                | "rmd"
+                | "pas"
+                | "php"
+                | "pp"
+                | "proto"
+                | "qs"
+                | "rs"
+                | "scala"
+                | "sc"
+                | "swift"
+                | "ts"
+                | "typ"
+                | "xml"
+                | "zig"
+            ):
                 self.character = "//"
-            case "ahk" | "asm" | "beancount" | "cl" | "clj" | "cljs" | "cljc" | "edn" | "fasl" | "ini" | "lisp" | "lsp" | "rkt" | "scm" | "ss":
+            case (
+                "ahk"
+                | "asm"
+                | "beancount"
+                | "cl"
+                | "clj"
+                | "cljs"
+                | "cljc"
+                | "edn"
+                | "fasl"
+                | "ini"
+                | "lisp"
+                | "lsp"
+                | "rkt"
+                | "scm"
+                | "ss"
+            ):
                 self.character = ";"
             case "bib" | "cls" | "erl" | "hrl" | "mat" | "sty" | "tex":
                 self.character = "%"
             case "adb" | "ads" | "elm" | "hs" | "lua" | "sql":
                 self.character = "--"
             # https://www.gnu.org/software/groff/manual/, https://manpages.bsd.lv/mdoc.html
             case "1" | "1m" | "2" | "3" | "4" | "5" | "6" | "7" | "8" | "n":
@@ -117,56 +171,72 @@
     # ################ TOC OUTPUT
     # ######## STDOUT
 
     def to_stdout(self) -> None:
         _, _outerToc = self._generate_toc()
         if _outerToc == "":
             # skip error if we already set self.err
-            print(
-                f'Could not generate a "{self.character}" toc from "{self.inputFile}"',
-                file=sys.stderr,
-            ) if self.err is None else None
+            (
+                print(
+                    f'Could not generate a "{self.character}" toc from "{self.inputFile}"',
+                    file=sys.stderr,
+                )
+                if self.err is None
+                else None
+            )
             self.err = "empty"
         else:
             print(_outerToc)
 
     # ######## FILE
 
-    def to_file(self, output: str | None = None) -> None:
+    def to_file(self, output: Path | None = None) -> None:
         # if file has been specified, print there instead of the original file (useful for testing)
         if self.outputFile is None:
             self.outputFile = output if output else self.inputFile
-        if self.inputFile == "stdin":
-            print(
-                "Cannot write to stdin", file=sys.stderr
-            ) if self.err is None else None
+        if self.inputFile == Path("-"):
+            (
+                print("Cannot write to stdin", file=sys.stderr)
+                if self.err is None
+                else None
+            )
             self.err = "stdin"
         else:
             # run twice because updating the toc with self.lineNumbers == True may shift everything down
             n = 2 if self.lineNumbers else 1
             for _ in range(n):
                 self._add_or_update()
 
     # ################################ INTERNAL METHODS
     # ################ TOC OUTPUT
 
     def _add_or_update(self) -> None:
         _innerToc, _outerToc = self._generate_toc()
         # do not write an empty file
         if _outerToc == "":
-            print(
-                f'Could not generate a "{self.character}" toc from "{self.inputFile}"',
-                file=sys.stderr,
-            ) if self.err is None else None
+            (
+                print(
+                    f'Could not generate a "{self.character}" toc from "{self.inputFile}"',
+                    file=sys.stderr,
+                )
+                if self.err is None
+                else None
+            )
             self.err = "empty"
         else:
             # if the file does not contain a toc, add it, otherwise update it
             # re.MULTILINE: https://docs.python.org/3/library/re.html#re.M
+            # match also file name, results in a second toc if file is renamed
+            # self.pattern = re.compile(
+            #    rf"{self.innerTocBegin}\n{self.innerTocTitle}(.*?){self.innerTocEnd}",
+            #    re.DOTALL,
+            # )
+            # does not match file name, replacing toc even if file gets renamed
             self.pattern = re.compile(
-                rf"{self.innerTocBegin}\n{self.innerTocTitle}(.*?){self.innerTocEnd}",
+                rf"{self.innerTocBegin}\n{self.character} │ Contents of (.*?){self.innerTocEnd}",
                 re.DOTALL,
             )
             # print(self.pattern)
             _data = self._read_file()
             # print(_data)
             if re.search(self.pattern, _data):
                 self._update_toc(_innerToc)
@@ -176,23 +246,32 @@
     def _write_toc(self, data: str) -> None:
         # common function to rewrite file
         if data and self.outputFile is not None:
             try:
                 with open(self.outputFile, "w") as f:
                     f.write(data)
             except PermissionError:
-                print(
-                    f'Skipping write-protected "{self.outputFile}"', file=sys.stderr
-                ) if self.err is None else None
+                (
+                    print(
+                        f'Skipping write-protected "{self.outputFile}"', file=sys.stderr
+                    )
+                    if self.err is None
+                    else None
+                )
                 self.err = "write"
                 self.updated = True
             except BaseException:
-                print(
-                    f'Unknown error while writing "{self.outputFile}"', file=sys.stderr
-                ) if self.err is None else None
+                (
+                    print(
+                        f'Unknown error while writing "{self.outputFile}"',
+                        file=sys.stderr,
+                    )
+                    if self.err is None
+                    else None
+                )
                 self.err = "unknownw"
                 self.updated = True
         elif not self.updated:
             # data should never be empty if self.updated = False, but in case least we prevented cleaning the file
             print(f'Skipping writing "{self.outputFile}"', file=sys.stderr)
             self.updated = True
         # elif self.updated: we skipped replacing the same toc
@@ -214,35 +293,68 @@
         if _firstLine == "":
             # if _firstLine was be empty, re.sub would destroy the original file by inserting an outerToc between every character
             _data = outerToc + "\n" + _data
         else:
             match self.extension:
                 case "md":
                     # multi line yaml, toml, js frontmatter for markdown
-                    _frontmatter_yaml = re.search(r"^---\n.*?\n---", _data, re.DOTALL)
-                    _frontmatter_toml = re.search(
-                        r"^\+\+\+\n.*?\n\+\+\+", _data, re.DOTALL
-                    )
-                    _frontmatter_json = re.search(r"^\{\n.*?\n\}", _data, re.DOTALL)
-                    if _frontmatter_yaml is not None:
-                        _frontmatter = _frontmatter_yaml.group(0)
-                    elif _frontmatter_toml is not None:
-                        _frontmatter = _frontmatter_toml.group(0)
-                    elif _frontmatter_json is not None:
-                        _frontmatter = _frontmatter_json.group(0)
+                    _firstline_yaml = re.search(r"^---$", _firstLine)
+                    _firstline_toml = re.search(r"^\+\+\+$", _firstLine)
+                    _firstline_json = re.search(r"^{$", _firstLine)
+                    if _firstline_yaml is not None:
+                        _frontmatters_yaml = re.search(
+                            r"^---\n.*?\n---", _data, re.DOTALL
+                        )
+                        if _frontmatters_yaml is not None:
+                            _frontmatter = _frontmatters_yaml.group(0)
+                        else:
+                            _frontmatter = None
+                    elif _firstline_toml is not None:
+                        _frontmatters_toml = re.search(
+                            r"^\+\+\+\n.*?\n\+\+\+", _data, re.DOTALL
+                        )
+                        if _frontmatters_toml is not None:
+                            _frontmatter = _frontmatters_toml.group(0)
+                        else:
+                            _frontmatter = None
+                    elif _firstline_json is not None:
+                        _frontmatters_json = re.search(
+                            r"^\{\n.*?\n\}", _data, re.DOTALL
+                        )
+                        if _frontmatters_json is not None:
+                            _frontmatter = _frontmatters_json.group(0)
+                        else:
+                            _frontmatter = None
                     else:
                         _frontmatter = None
-                    _firstLine = _frontmatter if _frontmatter else _firstLine
-                    _firstFewLines = (
-                        _firstLine + "\n\n" + outerToc
-                        if _frontmatter
-                        else outerToc + "\n\n" + _firstLine
-                    )
+                    if _frontmatter is not None:
+                        _firstLine = _frontmatter
+                        _firstFewLines = _firstLine + "\n\n" + outerToc
+                    else:
+                        _firstFewLines = outerToc + "\n\n" + _firstLine
                     # print(_frontmatter)
                     # print(_firstFewLines)
+                case "py":
+                    # need to match shebang also here since we have a switch/case by extension
+                    _firstline_shebang = re.search(r"^#\!", _firstLine)
+                    # module docstring for python
+                    _firstline_docstring = re.search(r'^"""$', _firstLine)
+                    if _firstline_shebang is not None:
+                        _firstFewLines = _firstLine + "\n\n" + outerToc
+                    else:
+                        if _firstline_docstring is not None:
+                            _docstrings = re.search(r'^"""\n.*?\n"""', _data, re.DOTALL)
+                            if _docstrings is not None:
+                                _docstring = _docstrings.group(0)
+                                _firstLine = _docstring
+                                _firstFewLines = _firstLine + "\n\n" + outerToc
+                            else:
+                                _firstFewLines = outerToc + "\n\n" + _firstLine
+                        else:
+                            _firstFewLines = outerToc + "\n\n" + _firstLine
                 case _:
                     # single line shebang, xml, html, vim, emacs, perl pod
                     if (
                         re.search(r"^#\!", _firstLine)
                         or re.search(r"<\?xml", _firstLine, re.IGNORECASE)
                         or re.search(r"<!doctype", _firstLine, re.IGNORECASE)
                         or re.search(
@@ -338,16 +450,16 @@
                 _tocSuffix = []
         return _tocPrefix, _tocSuffix
 
     # ######## HEADER
 
     def _toc_header(self) -> list:
         # begin the toc with the file name, truncating it if necessary
-        _filename = self.inputFile.split("/")[-1]
-        if self.inputFile == "stdin":
+        _filename = self.inputFile.name
+        if self.inputFile == Path("-"):
             _truncated_filename = (
                 f"stdin.{self.extension}" if self.extension != "" else "stdin"
             )
         else:
             _truncated_filename = (
                 (_filename[:46] + "...") if len(_filename) > 46 else _filename
             )
@@ -438,19 +550,25 @@
                     f"{_match.group(2)} {n+1}" if self.lineNumbers else _match.group(2)
                 )
                 _newtoc.append(self._add_heading(_heading_level, _heading_text))
                 # print(_newtoc)
         return _newtoc
 
     # #### HTML
-
-    # every time an html page is parsed with regex, a software engineer dies
     def _process_html(self, data: str) -> list:
         _newtoc = []
-        _pattern = re.compile(r"<h(\d).*?>(?:<.*?>)?(.*?)</.*?h\d", re.MULTILINE)
+        # every time an html page is parsed with regex, a software engineer dies
+        # _pattern = re.compile(r"<h(\d).*?>(?:<.*?>)?(.*?)</.*?h\d", re.MULTILINE)
+        # https://learnbyexample.github.io/python-regex-possessive-quantifier/
+        # _pattern = re.compile(r"<h(\d)(?>.*?)>?(?:\s)*(?:<.*?>)?(?:\s)*(.*?)(?:\s)*</(.*?)h\d>", re.MULTILINE)
+        # _pattern = re.compile(r"<h(\d).*?>.*?>?(?:\s)*(?:<.*?>)?(?:\s)*(.*?)(?:\s)*</.*?h\d>", re.DOTALL)
+        _pattern = re.compile(
+            r"<[hH](\d).*?>.*?>?(?:\s)*(?:<.*?>)?(?:\s)*(.*?)(?:\s)*</[hH]\d>",
+            re.DOTALL,
+        )
         # _matches = _pattern.finditer(data)
         # print(sum(1 for _ in _matches))
         # for _match in _matches:
         # sometimes it fails if not using list()
         # _matches = list(_pattern.finditer(data))
         # print(len(_matches))
         # print(_matches)
@@ -458,15 +576,16 @@
         _fromLastMatch = 0
         n = 1
         for _match in _pattern.finditer(data):
             # indicates character, not line number
             _heading_level = int(_match.group(1))
             # in case there are fancy tags or other elements inside the title, we remove them
             # blood for the blood god
-            _heading_text = re.sub(r"<.*?>", "", _match.group(2).strip())
+            _heading_text = re.sub(r"<.*?>", "", _match.group(2)).strip()
+            # print(f"Heading text: '{_heading_text}'")
             if self.lineNumbers:
                 # return the character number, not the line number
                 _untilCurrentMatch = _match.start(0)
                 # to calculate the line number, let's count the number of "\n" up to the match start, and add 1 to the result
                 n += data.count("\n", _fromLastMatch, _untilCurrentMatch)
                 _heading_text = _heading_text + " " + str(n)
                 # update with the position of the current match
@@ -642,44 +761,56 @@
     # ################ TOC INPUT
 
     def _read_file(self) -> str:
         # read file content and process it accordingly
         # display alert for common errors
         _data = ""
         try:
-            if self.inputFile == "stdin":
+            if self.inputFile == Path("-"):
                 _data = sys.stdin.read()
             else:
                 with open(self.inputFile, "r") as f:
                     _data = f.read()
         except FileNotFoundError:
-            print(
-                f'Skipping non-existing "{self.inputFile}"', file=sys.stderr
-            ) if self.err is None else None
+            (
+                print(f'Skipping non-existing "{self.inputFile}"', file=sys.stderr)
+                if self.err is None
+                else None
+            )
             _data = ""
             self.err = "notfound"
         except PermissionError:
-            print(
-                f'Skipping read-protected "{self.inputFile}"', file=sys.stderr
-            ) if self.err is None else None
+            (
+                print(f'Skipping read-protected "{self.inputFile}"', file=sys.stderr)
+                if self.err is None
+                else None
+            )
             _data = ""
             self.err = "read"
         except IsADirectoryError:
-            print(
-                f'Skipping directory "{self.inputFile}"', file=sys.stderr
-            ) if self.err is None else None
+            (
+                print(f'Skipping directory "{self.inputFile}"', file=sys.stderr)
+                if self.err is None
+                else None
+            )
             _data = ""
             self.err = "directory"
         except UnicodeDecodeError:
-            print(
-                f'Skipping binary "{self.inputFile}"', file=sys.stderr
-            ) if self.err is None else None
+            (
+                print(f'Skipping binary "{self.inputFile}"', file=sys.stderr)
+                if self.err is None
+                else None
+            )
             _data = ""
             self.err = "binary"
         except BaseException:
-            print(
-                f'Unknown error while reading "{self.inputFile}"', file=sys.stderr
-            ) if self.err is None else None
+            (
+                print(
+                    f'Unknown error while reading "{self.inputFile}"', file=sys.stderr
+                )
+                if self.err is None
+                else None
+            )
             _data = ""
             self.err = "unknownr"
         finally:
             return _data
```

