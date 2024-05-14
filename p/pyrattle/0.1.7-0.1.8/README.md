# Comparing `tmp/pyrattle-0.1.7.tar.gz` & `tmp/pyrattle-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrattle-0.1.7.tar", max compression
+gzip compressed data, was "pyrattle-0.1.8.tar", max compression
```

## Comparing `pyrattle-0.1.7.tar` & `pyrattle-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.7/LICENSE.md
--rw-r--r--   0        0        0      371 2024-05-14 15:04:05.769558 pyrattle-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.7/pyrattle/__init__.py
--rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.7/pyrattle/errors.py
--rw-r--r--   0        0        0     9460 2024-05-14 15:03:41.242889 pyrattle-0.1.7/pyrattle/pyrattle.py
--rw-r--r--   0        0        0     4253 2024-05-14 11:35:37.541695 pyrattle-0.1.7/README.md
--rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 pyrattle-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     9680 2024-05-14 09:56:55.256347 pyrattle-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0      371 2024-05-14 15:08:56.861621 pyrattle-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-05-14 09:37:22.431681 pyrattle-0.1.8/pyrattle/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-14 09:18:43.736466 pyrattle-0.1.8/pyrattle/errors.py
+-rw-r--r--   0        0        0     9460 2024-05-14 15:09:14.147728 pyrattle-0.1.8/pyrattle/pyrattle.py
+-rw-r--r--   0        0        0     4253 2024-05-14 11:35:37.541695 pyrattle-0.1.8/README.md
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 pyrattle-0.1.8/PKG-INFO
```

### Comparing `pyrattle-0.1.7/LICENSE.md` & `pyrattle-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.7/pyrattle/errors.py` & `pyrattle-0.1.8/pyrattle/errors.py`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.7/pyrattle/pyrattle.py` & `pyrattle-0.1.8/pyrattle/pyrattle.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -130,24 +130,24 @@
                scan_result = scanner.scan(scan_type=ScanType.QUICK)
           ```
           """
 
           if (scan_type == ScanType.CUSTOM and file == None):
                raise FileNotPresent("When using Custom ScanType, a file or directory path should be provided")
           flags : List[str] = ["-Scan"]
-          if (file):
-               flags.append("-File")
           if (boot_sector_scan):
                flags.append("-BootSectorScan")
           if (timeout != 30):
                flags.append(f"-Timeout {timeout}")
           if (is_cancel):
                flags.append("-Cancel")
           if (disable_remediation):
                flags.append("-DisableRemediation")
+          if (file):
+               flags.append("-File")
           
           stdout, stderr, returncode = self._run_command(flags)
 
           print("Stdout: ", stdout)
           print("Return code :", returncode)
           if (returncode != 0 and returncode != 2):
                raise ScanFailed
```

### Comparing `pyrattle-0.1.7/README.md` & `pyrattle-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyrattle-0.1.7/PKG-INFO` & `pyrattle-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrattle
-Version: 0.1.7
+Version: 0.1.8
 Summary: Windows Defender wrapper
 Author: Yassine DAMIRI
 Author-email: yassine.damiri@epita.fr
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

