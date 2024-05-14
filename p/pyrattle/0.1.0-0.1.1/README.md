# Comparing `tmp/pyrattle-0.1.0.tar.gz` & `tmp/pyrattle-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrattle-0.1.0.tar", max compression
+gzip compressed data, was "pyrattle-0.1.1.tar", max compression
```

## Comparing `pyrattle-0.1.0.tar` & `pyrattle-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.0/LICENSE.md
--rw-r--r--   0        0        0      347 2024-05-14 09:44:44.957378 pyrattle-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.0/pyrattle/__init__.py
--rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.0/pyrattle/errors.py
--rw-r--r--   0        0        0     9082 2024-05-14 09:43:11.926011 pyrattle-0.1.0/pyrattle/pyrattle.py
--rw-r--r--   0        0        0     4252 2024-05-14 09:55:47.190387 pyrattle-0.1.0/README.md
--rw-r--r--   0        0        0     4410 1970-01-01 00:00:00.000000 pyrattle-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0      371 2024-05-14 12:24:28.758241 pyrattle-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.1/pyrattle/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.1/pyrattle/errors.py
+-rw-r--r--   0        0        0     9517 2024-05-14 12:22:45.339004 pyrattle-0.1.1/pyrattle/pyrattle.py
+-rw-r--r--   0        0        0     4253 2024-05-14 11:35:37.541695 pyrattle-0.1.1/README.md
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 pyrattle-0.1.1/PKG-INFO
```

### Comparing `pyrattle-0.1.0/LICENSE.md` & `pyrattle-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.0/pyrattle/errors.py` & `pyrattle-0.1.1/pyrattle/errors.py`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.0/pyrattle/pyrattle.py` & `pyrattle-0.1.1/pyrattle/pyrattle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
-import subprocess
+import os
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import List, Tuple
 
+
 from pyrattle.errors import BadArgument, FileNotPresent, ScanFailed, ScanParsingFailed
 
 class ScanType(Enum):
     DEFAULT = 0
     QUICK  = 1
     FULL = 2
     CUSTOM = 3
@@ -40,17 +41,32 @@
 
  
 @dataclass
 class PyDefender :
      executable_path: str = "C:\\Program Files\\Windows Defender\\MpCmdRun.exe"
         
      def _run_command(self, args) -> Tuple[str, str, int]:
-          command = [self.executable_path] + args
-          result = subprocess.run(command, capture_output=True, text=True)
-          return result.stdout, result.stderr, result.returncode
+          command = [f'"{self.executable_path}"'] + args
+          command_str = ' '.join(command)
+          
+          # Open pipes to capture stdout and stderr
+          stdout_pipe = os.popen(f"{command_str} 2>&1")
+          stdout = stdout_pipe.read()
+          returncode = stdout_pipe.close()
+          
+          if returncode is None:
+               returncode = 0
+          else:
+               returncode = 124
+          
+          # In this simple example, stderr will be empty as it's redirected to stdout
+          stderr = ""
+
+          return stdout, stderr, returncode
+
      
      def _parse_scan(self, output : str):
           threat = re.search(r"Threat\s+:\s*(.*)", output).group(1).strip()
           ressources = int(re.search(r"Ressources\s+:\s*([0-9]+)\stotal", output).group(1))
           file = re.search(r"file\s*:(.*)", output).group(1).strip()
 
           return ScanResult(True, threat, ressources, file)
@@ -218,14 +234,15 @@
 
      def listAllDynamicSignatures(self) -> List[str]:
           flags : List[str] = ['-ListAllDynamicSignatures']
 
           stdout, stderr , returncode = self._run_command(flags)
 
           if (returncode != 0 and returncode != 2 or stderr != None):
+               print(stdout)
                return []
           return self._parse_signatures(stdout)
 
      def removeDynamicSignature(self, signature_id: str) -> bool :
           if (signature_id == None):
                raise BadArgument
```

### Comparing `pyrattle-0.1.0/README.md` & `pyrattle-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```
 scanner = PyDefender()
 # or
 scanner = PyDefender(executable_path="C:\\Program Files\\Windows Defender\\MpCmdRun.exe")
 ```
 
 ## Performing a Scan
-It can perform multiple king of scan:
+It can perform multiple kinds of scan:
 - **Quick Scan**
     ```
     scan_result = scanner.scan(scan_type=ScanType.QUICK)
     ```
 - **Full Scan**
     ```
     scan_result = scanner.scan(scan_type=ScanType.FULL)
```

### Comparing `pyrattle-0.1.0/PKG-INFO` & `pyrattle-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyrattle
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Windows Defender wrapper
 Author: Yassine DAMIRI
 Author-email: yassine.damiri@epita.fr
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
@@ -39,15 +39,15 @@
 ```
 scanner = PyDefender()
 # or
 scanner = PyDefender(executable_path="C:\\Program Files\\Windows Defender\\MpCmdRun.exe")
 ```
 
 ## Performing a Scan
-It can perform multiple king of scan:
+It can perform multiple kinds of scan:
 - **Quick Scan**
     ```
     scan_result = scanner.scan(scan_type=ScanType.QUICK)
     ```
 - **Full Scan**
     ```
     scan_result = scanner.scan(scan_type=ScanType.FULL)
```

