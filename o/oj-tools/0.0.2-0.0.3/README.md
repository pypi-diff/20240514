# Comparing `tmp/oj_tools-0.0.2.tar.gz` & `tmp/oj_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oj_tools-0.0.2.tar", last modified: Tue May 14 11:50:45 2024, max compression
+gzip compressed data, was "oj_tools-0.0.3.tar", last modified: Tue May 14 15:00:44 2024, max compression
```

## Comparing `oj_tools-0.0.2.tar` & `oj_tools-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 11:50:45.165015 oj_tools-0.0.2/
--rw-r--r--   0 hepheir    (501) staff       (20)      878 2024-05-14 11:50:45.164816 oj_tools-0.0.2/PKG-INFO
--rw-r--r--   0 hepheir    (501) staff       (20)      392 2024-05-14 10:47:12.000000 oj_tools-0.0.2/README.md
--rw-r--r--   0 hepheir    (501) staff       (20)      489 2024-05-14 11:50:31.000000 oj_tools-0.0.2/pyproject.toml
--rw-r--r--   0 hepheir    (501) staff       (20)       38 2024-05-14 11:50:45.165058 oj_tools-0.0.2/setup.cfg
-drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 11:50:45.163535 oj_tools-0.0.2/src/
--rw-r--r--   0 hepheir    (501) staff       (20)     3200 2024-05-14 11:43:01.000000 oj_tools-0.0.2/src/oj.py
-drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 11:50:45.164531 oj_tools-0.0.2/src/oj_tools.egg-info/
--rw-r--r--   0 hepheir    (501) staff       (20)      878 2024-05-14 11:50:45.000000 oj_tools-0.0.2/src/oj_tools.egg-info/PKG-INFO
--rw-r--r--   0 hepheir    (501) staff       (20)      178 2024-05-14 11:50:45.000000 oj_tools-0.0.2/src/oj_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hepheir    (501) staff       (20)        1 2024-05-14 11:50:45.000000 oj_tools-0.0.2/src/oj_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hepheir    (501) staff       (20)        3 2024-05-14 11:50:45.000000 oj_tools-0.0.2/src/oj_tools.egg-info/top_level.txt
+drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 15:00:44.739927 oj_tools-0.0.3/
+-rw-r--r--   0 hepheir    (501) staff       (20)     1870 2024-05-14 15:00:44.739741 oj_tools-0.0.3/PKG-INFO
+-rw-r--r--   0 hepheir    (501) staff       (20)     1383 2024-05-14 11:57:20.000000 oj_tools-0.0.3/README.md
+-rw-r--r--   0 hepheir    (501) staff       (20)      489 2024-05-14 15:00:33.000000 oj_tools-0.0.3/pyproject.toml
+-rw-r--r--   0 hepheir    (501) staff       (20)       38 2024-05-14 15:00:44.739969 oj_tools-0.0.3/setup.cfg
+drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 15:00:44.738583 oj_tools-0.0.3/src/
+-rw-r--r--   0 hepheir    (501) staff       (20)     3446 2024-05-14 14:59:04.000000 oj_tools-0.0.3/src/oj.py
+drwxr-xr-x   0 hepheir    (501) staff       (20)        0 2024-05-14 15:00:44.739580 oj_tools-0.0.3/src/oj_tools.egg-info/
+-rw-r--r--   0 hepheir    (501) staff       (20)     1870 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hepheir    (501) staff       (20)      178 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hepheir    (501) staff       (20)        1 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hepheir    (501) staff       (20)        3 2024-05-14 15:00:44.000000 oj_tools-0.0.3/src/oj_tools.egg-info/top_level.txt
```

### Comparing `oj_tools-0.0.2/src/oj.py` & `oj_tools-0.0.3/src/oj.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,26 @@
         return {
             "spj": self.spj,
             "testcases": {
                 key: val.as_dict() for key, val in self.testcases.items()
             },
         }
 
-    def extract_as_zip(self, file="./problem.zip") -> None:
-        """Save problem as .zip file"""
+    @property
+    def default_zip_path(self) -> pathlib.Path:
+        return pathlib.Path(f'./{self.title}.zip')
+
+
+    def extract_as_zip(self, filename: typing.Optional[str]=None) -> None:
+        """Save problem as .zip file
+
+        filename: default is `./PROBLEM_TITLE.zip`
+        """
         with tempfile.TemporaryDirectory() as tmp_dir:
-            zip_path = pathlib.Path(file)
+            zip_path = pathlib.Path(filename) if filename is not None else self.default_zip_path
             dir_path = pathlib.Path(tmp_dir)
             info_filename = 'info'
 
             for testcase in self.testcases.values():
                 testcase.extract_as_file(dir=dir_path)
 
             with open(dir_path / info_filename, 'w') as f:
```

