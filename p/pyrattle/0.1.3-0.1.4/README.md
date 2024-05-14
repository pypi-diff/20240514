# Comparing `tmp/pyrattle-0.1.3.tar.gz` & `tmp/pyrattle-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrattle-0.1.3.tar", max compression
+gzip compressed data, was "pyrattle-0.1.4.tar", max compression
```

## Comparing `pyrattle-0.1.3.tar` & `pyrattle-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      371 2024-05-14 12:31:47.963660 pyrattle-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.3/pyrattle/__init__.py
--rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.3/pyrattle/errors.py
--rw-r--r--   0        0        0     9310 2024-05-14 12:31:37.499781 pyrattle-0.1.3/pyrattle/pyrattle.py
--rw-r--r--   0        0        0     4253 2024-05-14 11:35:37.541695 pyrattle-0.1.3/README.md
--rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 pyrattle-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      371 2024-05-14 12:32:58.074819 pyrattle-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.4/pyrattle/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.4/pyrattle/errors.py
+-rw-r--r--   0        0        0     9356 2024-05-14 12:32:40.448153 pyrattle-0.1.4/pyrattle/pyrattle.py
+-rw-r--r--   0        0        0     4253 2024-05-14 11:35:37.541695 pyrattle-0.1.4/README.md
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 pyrattle-0.1.4/PKG-INFO
```

### Comparing `pyrattle-0.1.3/LICENSE.md` & `pyrattle-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.3/pyrattle/errors.py` & `pyrattle-0.1.4/pyrattle/errors.py`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.3/pyrattle/pyrattle.py` & `pyrattle-0.1.4/pyrattle/pyrattle.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,14 +228,15 @@
           return [line.split(": ")[1] for line in output.strip().split("\n")] 
 
      def listAllDynamicSignatures(self) -> List[str]:
           flags : List[str] = ['-ListAllDynamicSignatures']
 
           stdout, stderr , returncode = self._run_command(flags)
 
+          print("Return code: ", returncode)
           if (returncode != 0 and returncode != 2):
                print(stdout) 
                return []
           return self._parse_signatures(stdout)
 
      def removeDynamicSignature(self, signature_id: str) -> bool :
           if (signature_id == None):
```

### Comparing `pyrattle-0.1.3/README.md` & `pyrattle-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.3/PKG-INFO` & `pyrattle-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrattle
-Version: 0.1.3
+Version: 0.1.4
 Summary: Windows Defender wrapper
 Author: Yassine DAMIRI
 Author-email: yassine.damiri@epita.fr
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

