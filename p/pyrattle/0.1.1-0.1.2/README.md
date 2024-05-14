# Comparing `tmp/pyrattle-0.1.1.tar.gz` & `tmp/pyrattle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrattle-0.1.1.tar", max compression
+gzip compressed data, was "pyrattle-0.1.2.tar", max compression
```

## Comparing `pyrattle-0.1.1.tar` & `pyrattle-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      371 2024-05-14 12:24:28.758241 pyrattle-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.1/pyrattle/__init__.py
--rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.1/pyrattle/errors.py
--rw-r--r--   0        0        0     9517 2024-05-14 12:22:45.339004 pyrattle-0.1.1/pyrattle/pyrattle.py
--rw-r--r--   0        0        0     4253 2024-05-14 11:35:37.541695 pyrattle-0.1.1/README.md
--rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 pyrattle-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      371 2024-05-14 12:29:58.241802 pyrattle-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.2/pyrattle/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.2/pyrattle/errors.py
+-rw-r--r--   0        0        0     9386 2024-05-14 12:29:39.673780 pyrattle-0.1.2/pyrattle/pyrattle.py
+-rw-r--r--   0        0        0     4253 2024-05-14 11:35:37.541695 pyrattle-0.1.2/README.md
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 pyrattle-0.1.2/PKG-INFO
```

### Comparing `pyrattle-0.1.1/LICENSE.md` & `pyrattle-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.1/pyrattle/errors.py` & `pyrattle-0.1.2/pyrattle/errors.py`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.1/pyrattle/pyrattle.py` & `pyrattle-0.1.2/pyrattle/pyrattle.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,20 +48,15 @@
           command = [f'"{self.executable_path}"'] + args
           command_str = ' '.join(command)
           
           # Open pipes to capture stdout and stderr
           stdout_pipe = os.popen(f"{command_str} 2>&1")
           stdout = stdout_pipe.read()
           returncode = stdout_pipe.close()
-          
-          if returncode is None:
-               returncode = 0
-          else:
-               returncode = 124
-          
+      
           # In this simple example, stderr will be empty as it's redirected to stdout
           stderr = ""
 
           return stdout, stderr, returncode
 
      
      def _parse_scan(self, output : str):
```

### Comparing `pyrattle-0.1.1/README.md` & `pyrattle-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.1/PKG-INFO` & `pyrattle-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrattle
-Version: 0.1.1
+Version: 0.1.2
 Summary: Windows Defender wrapper
 Author: Yassine DAMIRI
 Author-email: yassine.damiri@epita.fr
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

