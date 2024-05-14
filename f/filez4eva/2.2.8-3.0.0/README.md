# Comparing `tmp/filez4eva-2.2.8.tar.gz` & `tmp/filez4eva-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filez4eva-2.2.8.tar", max compression
+gzip compressed data, was "filez4eva-3.0.0.tar", max compression
```

## Comparing `filez4eva-2.2.8.tar` & `filez4eva-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     1616 2024-04-26 04:48:22.060644 filez4eva-2.2.8/README.md
--rw-r--r--   0        0        0      168 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/__init__.py
--rw-r--r--   0        0        0       48 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/__main__.py
--rw-r--r--   0        0        0      288 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/command/__init__.py
--rw-r--r--   0        0        0      654 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/command/scan_command.py
--rw-r--r--   0        0        0     3261 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/command/stow_command.py
--rw-r--r--   0        0        0      730 2024-04-26 04:48:22.060644 filez4eva-2.2.8/filez4eva/directory_scanner.py
--rw-r--r--   0        0        0       42 2024-04-26 04:48:22.061644 filez4eva-2.2.8/filez4eva/error.py
--rw-r--r--   0        0        0     2487 2024-04-26 04:48:22.061644 filez4eva-2.2.8/filez4eva/file_mover.py
--rw-r--r--   0        0        0      585 2024-04-26 04:48:32.205571 filez4eva-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 filez4eva-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1616 2024-05-14 04:26:37.137152 filez4eva-3.0.0/README.md
+-rw-r--r--   0        0        0      168 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/__main__.py
+-rw-r--r--   0        0        0      291 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/command/__init__.py
+-rw-r--r--   0        0        0     2770 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/command/scan_command.py
+-rw-r--r--   0        0        0     3866 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/command/stow_command.py
+-rw-r--r--   0        0        0       42 2024-05-14 04:26:37.137152 filez4eva-3.0.0/filez4eva/error.py
+-rw-r--r--   0        0        0      585 2024-05-14 04:26:47.818143 filez4eva-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 filez4eva-3.0.0/PKG-INFO
```

### Comparing `filez4eva-2.2.8/README.md` & `filez4eva-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `filez4eva-2.2.8/filez4eva/command/stow_command.py` & `filez4eva-3.0.0/filez4eva/command/stow_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from datetime import datetime
+import os
 from pathlib import Path
 import re
+from subprocess import run
 import sys
+
 from wizlib.parser import WizParser
-from wizlib.ui import Chooser
-from wizlib.ui import Choice
+from wizlib.command import CommandCancellation
+from wizlib.ui.shell_ui import Emphasis
 
 from filez4eva.command import Filez4EvaCommand
 from filez4eva.error import Filez4EvaError
 
 
 FILE_PATTERN = re.compile(r'\d{8}\-([a-zA-Z0-9-]+)\.(\w+)')
 
@@ -26,20 +29,48 @@
     def add_args(cls, parser: WizParser):
         super().add_args(parser)
         parser.add_argument('--date', '-d')
         parser.add_argument('--account', '-a')
         parser.add_argument('--part', '-p')
         parser.add_argument('file')
 
+    def handle_vals(self):
+        super().handle_vals()
+        if not self.provided('date'):
+            while True:
+                self.date = self.app.ui.get_text('Date: ').strip()
+                if not self.date:
+                    self.app.ui.send('Date required', Emphasis.PRINCIPAL)
+                    raise CommandCancellation()
+                try:
+                    datetime.strptime(self.date, "%Y%m%d")
+                    break
+                except ValueError:
+                    self.app.ui.send('Date must match format YYYYMMDD',
+                                     Emphasis.PRINCIPAL)
+        if not self.provided('account'):
+            accounts = self.get_accounts()
+            self.account = self.app.ui.get_text('Account: ', accounts)
+            if not self.account:
+                self.app.ui.send('Account required', Emphasis.PRINCIPAL)
+                raise CommandCancellation()
+        if not self.provided('part'):
+            parts = self.get_parts(self.account)
+            self.part = self.app.ui.get_text('Part: ', parts)
+            if not self.part:
+                self.app.ui.send('Part required', Emphasis.PRINCIPAL)
+                raise CommandCancellation()
+
     def get_accounts(self) -> list:
         accounts = set()
         for year in self.targetdir.iterdir():
             if year.name.isdigit() and year.is_dir():
                 for dir in year.iterdir():
-                    accounts.add(dir.name)
+                    if dir.is_dir():
+                        accounts.add(dir.name)
         return sorted(accounts)
 
     def get_parts(self, sub: str) -> list:
         """Return a set of past filename parts"""
         parts = set()
         for year in self.targetdir.iterdir():
             if year.name.isdigit():
@@ -47,48 +78,31 @@
                 if subdir.is_dir():
                     for file in subdir.iterdir():
                         match = re.match(FILE_PATTERN, file.name)
                         if match:
                             parts.add(match.groups()[0])
         return sorted(parts)
 
-    def handle_vals(self):
-        super().handle_vals()
-        if not self.provided('date'):
-            while True:
-                self.date = self.ui.get_text('Date: ')
-                try:
-                    datetime.strptime(self.date, "%Y%m%d")
-                    break
-                except ValueError:
-                    print('Date must match format YYYYMMDD', file=sys.stderr)
-        if not self.provided('account'):
-            accounts = self.get_accounts()
-            self.account = self.ui.get_text('Account: ', accounts)
-        if not self.provided('part'):
-            parts = self.get_parts(self.account)
-            self.part = self.ui.get_text('Part: ', parts)
-
     @property
     def targetdir(self):
-        return Path(self.config.get('filez4eva-target'))
+        return Path(self.app.config.get('filez4eva-target'))
 
     @Filez4EvaCommand.wrap
     def execute(self):
-        sourcepath = Path(self.file).expanduser().absolute()
-        if not sourcepath.is_file():
-            raise Filez4EvaError(f"Missing file {sourcepath}")
-        extension = sourcepath.suffix
+        path = Path(self.file).expanduser().absolute()
+        if not path.is_file():
+            raise Filez4EvaError(f"File {path} must exist")
+        extension = path.suffix
         date = datetime.strptime(self.date, "%Y%m%d")
         dirpath = self.targetdir / str(date.year) / self.account
         if not dirpath.exists():
             # confirm = rlinput(f"Create {dirpath}? ", default="yes")
             # if confirm.startswith('y'):
             dirpath.mkdir(parents=True)
         targetpath = dirpath / \
             f"{date.strftime('%Y%m%d')}-{self.part}{extension}"
         if targetpath.exists():
             raise Filez4EvaError(f"File already exists at {targetpath}")
         # confirm = rlinput(f"Move file to {targetpath}? ", default="yes")
         # if confirm.startswith('y'):
-        sourcepath.rename(targetpath)
+        path.rename(targetpath)
         self.status = 'Done'
```

### Comparing `filez4eva-2.2.8/pyproject.toml` & `filez4eva-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "filez4eva"
 description = "Shift scans, photos, and other files into structured folders for permanent safekeeping"
 authors = ["Francis Potter <francis@steampunkwizard.ca>"]
 license = "MIT"
 readme = "README.md"
-version = "2.2.8"
+version = "3.0.0"
 
 [tool.poetry.dependencies]
 python = "~3.11"
 watchdog = "^3.0.0"
-wizlib = "2.0.18"
+wizlib = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pycodestyle = "^2.11.0"
 coverage = "^7.3.0"
 autopep8 = "^2.0.4"
 
 [build-system]
```

### Comparing `filez4eva-2.2.8/PKG-INFO` & `filez4eva-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: filez4eva
-Version: 2.2.8
+Version: 3.0.0
 Summary: Shift scans, photos, and other files into structured folders for permanent safekeeping
 License: MIT
 Author: Francis Potter
 Author-email: francis@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
-Requires-Dist: wizlib (==2.0.18)
+Requires-Dist: wizlib (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Filez4Eva
 
 Shift scans, photos, and other files into structured folders for permanent safekeeping
 ---
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: filez4eva Version: 2.2.8 Summary: Shift scans,
+Metadata-Version: 2.1 Name: filez4eva Version: 3.0.0 Summary: Shift scans,
 photos, and other files into structured folders for permanent safekeeping
 License: MIT Author: Francis Potter Author-email: francis@steampunkwizard.ca
 Requires-Python: >=3.11,<3.12 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: watchdog (>=3.0.0,<4.0.0) Requires-
-Dist: wizlib (==2.0.18) Description-Content-Type: text/markdown # Filez4Eva
-Shift scans, photos, and other files into structured folders for permanent
-safekeeping --- _E_l_e_p_h_a_n_t_ _i_c_o_n_ _c_r_e_a_t_e_d_ _b_y_ _F_l_a_t_ _I_c_o_n_s_ _-_ _F_l_a_t_i_c_o_n I keep files
-named and organized in a certain way in DropBox. This tool names new files
-correctly and puts them in the right directory. ## Installation It's best to
-install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if you
-need it. Then: ```bash pipx install filez4eva ``` ## Usage The directory
+Dist: wizlib (>=3.0.0,<4.0.0) Description-Content-Type: text/markdown #
+Filez4Eva Shift scans, photos, and other files into structured folders for
+permanent safekeeping --- _E_l_e_p_h_a_n_t_ _i_c_o_n_ _c_r_e_a_t_e_d_ _b_y_ _F_l_a_t_ _I_c_o_n_s_ _-_ _F_l_a_t_i_c_o_n I keep
+files named and organized in a certain way in DropBox. This tool names new
+files correctly and puts them in the right directory. ## Installation It's best
+to install using `pipx`. See [the pipx site](https://pypa.github.io/pipx/) if
+you need it. Then: ```bash pipx install filez4eva ``` ## Usage The directory
 pattern for account documents is: ``` ~/Dropbox/accounts///-. ``` Where: -
 `year` is the year of the document, typically from the date - `account` is the
 name of the account, all lower case, hyphen separated - `date` is the date on
 the document in `YYYYMMDD` format - `part` is the textual part of the name of
 the document, often starting with the account name, all lower case, hyphen
 separated - `extension` is the original filename extension, often `pdf` I have
 my browsers etc. set to download new files to Desktop, then it's easy to run
```

