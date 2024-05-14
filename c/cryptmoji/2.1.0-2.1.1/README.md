# Comparing `tmp/cryptmoji-2.1.0.tar.gz` & `tmp/cryptmoji-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptmoji-2.1.0.tar", max compression
+gzip compressed data, was "cryptmoji-2.1.1.tar", max compression
```

## Comparing `cryptmoji-2.1.0.tar` & `cryptmoji-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      105 2023-04-26 03:44:58.000000 cryptmoji-2.1.0/cryptmoji/__init__.py
--rw-r--r--   0        0        0      736 2024-05-13 09:06:41.074540 cryptmoji-2.1.0/cryptmoji/cli.py
--rw-r--r--   0        0        0    13293 2022-09-15 07:14:58.000000 cryptmoji-2.1.0/cryptmoji/data.py
--rw-r--r--   0        0        0     1400 2024-05-13 07:18:19.674068 cryptmoji-2.1.0/cryptmoji/main.py
--rw-r--r--   0        0        0     1094 2022-09-04 12:17:16.000000 cryptmoji-2.1.0/LICENSE
--rw-r--r--   0        0        0     1569 2024-05-13 09:06:41.075540 cryptmoji-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1377 2024-05-13 09:06:41.074540 cryptmoji-2.1.0/README.md
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 cryptmoji-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-05-13 16:15:31.984887 cryptmoji-2.1.1/cryptmoji/__init__.py
+-rw-r--r--   0        0        0      816 2024-05-14 03:39:33.276065 cryptmoji-2.1.1/cryptmoji/cli.py
+-rw-r--r--   0        0        0    13293 2022-09-15 07:14:58.000000 cryptmoji-2.1.1/cryptmoji/data.py
+-rw-r--r--   0        0        0     1400 2024-05-13 07:18:19.674068 cryptmoji-2.1.1/cryptmoji/main.py
+-rw-r--r--   0        0        0       25 2024-05-14 03:39:49.259709 cryptmoji-2.1.1/cryptmoji/version.py
+-rw-r--r--   0        0        0     1094 2022-09-04 12:17:16.000000 cryptmoji-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1570 2024-05-14 03:40:12.020299 cryptmoji-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1399 2024-05-13 17:22:55.307088 cryptmoji-2.1.1/README.md
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 cryptmoji-2.1.1/PKG-INFO
```

### Comparing `cryptmoji-2.1.0/cryptmoji/cli.py` & `cryptmoji-2.1.1/cryptmoji/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from rich.console import Console
-from typer import Typer
+from typer import Typer, prompt
 
 from cryptmoji.main import decrypt, encrypt
+from cryptmoji.version import __version__
 
 app = Typer()
 console = Console()
 
 
 @app.command("encrypt")
 def cli_encrypt(text: str):
     """Encrypts a string as a string of emojis."""
-    key = console.input(
-        "Key (optional): ",
-        markup=False,
-        emoji=False,
-        password=True,
-    )
-
-    console.print(encrypt(text, key=key if key else None))
+    key = prompt("Enter key", default=None)
+    console.print(encrypt(text, key=key))
 
 
 @app.command("decrypt")
 def cli_decrypt(text: str):
     """Decrypts a string of emojis."""
-    key = console.input(
-        "Key (optional): ",
-        markup=False,
-        emoji=False,
-        password=True,
-    )
-    console.print(decrypt(text, key=key if key else None))
+    key = prompt("Enter key", default=None)
+    console.print(decrypt(text, key=key))
+
+
+@app.command("--version")
+def cli_version():
+    """Prints the version of the library."""
+    version = ".".join(str(i) for i in __version__)
+    console.print(f"cryptmoji v{version}")
+
+
+if __name__ == "__main__":
+    app()
```

### Comparing `cryptmoji-2.1.0/cryptmoji/data.py` & `cryptmoji-2.1.1/cryptmoji/data.py`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.1.0/cryptmoji/main.py` & `cryptmoji-2.1.1/cryptmoji/main.py`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.1.0/LICENSE` & `cryptmoji-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptmoji-2.1.0/pyproject.toml` & `cryptmoji-2.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 [tool.poetry]
 name = "cryptmoji"
-version = "2.1.0"
+version = "2.1.1"
 description = "Encrypt Text using emojis!"
 authors = ["Siddhesh Agarwal <siddhesh.agarwal@gmail.com>"]
 license = "MIT"
 readme = "./README.md"
 repository = "https://github.com/Siddhesh-Agarwal/cryptmoji"
-documentation = "https://siddhesh-agarwal.github.io/cryptmoji/"
+documentation = "https://github.com/Siddhesh-Agarwal/cryptmoji/wiki"
 keywords = ["encryption", "emoji", "cipher", "cryptography", "cryptmoji"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
+    "Intended Audience :: Information Technology",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
+    "Programming Language :: Python :: Implementation",
     "Topic :: Security",
     "Topic :: Security :: Cryptography",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 
 [tool.poetry.scripts]
 cryptmoji = "cryptmoji.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4.0"
-
-[tool.poetry.group.cli.dependencies]
 typer = {extras = ["all"], version = "^0.12.3"}
 rich = "^13.7.1"
 
 [build-system]
 requires = ["poetry-core>=2.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cryptmoji-2.1.0/README.md` & `cryptmoji-2.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,24 +38,18 @@
 decrypted = decrypt(encrypted, key=key)
 print(decrypted)
 # 'Hello, world!'
 ```
 
 ## Command line tool
 
-### Installation
-
-```sh
-pip install cryptmoji[cli]
-```
-
 ### Usage
 
 ```sh
-$ cryptmoji encrypt "Hello World"
-Key (optional):
+$ cryptmoji encrypt "Hello World" --key "test"
 🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪
 
-$ cryptmoji decrypt "🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪"
-Key (optional):
+$ cryptmoji decrypt "🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪" --key "test"
 Hello World
 ```
+
+> **NOTE**: key is an optional parameter. If not provided, the value defaults to `None`.
```

### Comparing `cryptmoji-2.1.0/PKG-INFO` & `cryptmoji-2.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: cryptmoji
-Version: 2.1.0
+Version: 2.1.1
 Summary: Encrypt Text using emojis!
 Home-page: https://github.com/Siddhesh-Agarwal/cryptmoji
 License: MIT
 Keywords: encryption,emoji,cipher,cryptography,cryptmoji
 Author: Siddhesh Agarwal
 Author-email: siddhesh.agarwal@gmail.com
 Requires-Python: >=3.7.0,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Programming Language :: Python :: Implementation
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Project-URL: Documentation, https://siddhesh-agarwal.github.io/cryptmoji/
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
+Project-URL: Documentation, https://github.com/Siddhesh-Agarwal/cryptmoji/wiki
 Project-URL: Repository, https://github.com/Siddhesh-Agarwal/cryptmoji
 Description-Content-Type: text/markdown
 
 # 🥷 Cryptmoji
 
 A simple emoji-based encryption-decryption library.
 
@@ -71,25 +74,19 @@
 decrypted = decrypt(encrypted, key=key)
 print(decrypted)
 # 'Hello, world!'
 ```
 
 ## Command line tool
 
-### Installation
-
-```sh
-pip install cryptmoji[cli]
-```
-
 ### Usage
 
 ```sh
-$ cryptmoji encrypt "Hello World"
-Key (optional):
+$ cryptmoji encrypt "Hello World" --key "test"
 🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪
 
-$ cryptmoji decrypt "🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪"
-Key (optional):
+$ cryptmoji decrypt "🎿🏑🏸🏹🐁🍻🏑🐁🐄🏤🏪" --key "test"
 Hello World
 ```
 
+> **NOTE**: key is an optional parameter. If not provided, the value defaults to `None`.
+
```

