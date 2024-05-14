# Comparing `tmp/feno-0.2.2.tar.gz` & `tmp/feno-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.2.2.tar", last modified: Thu Apr 25 14:39:42 2024, max compression
+gzip compressed data, was "feno-0.2.3.tar", last modified: Thu Apr 25 16:27:46 2024, max compression
```

## Comparing `feno-0.2.2.tar` & `feno-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.163656 feno-0.2.2/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.2.2/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.2.2/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2569 2024-04-25 14:39:42.163656 feno-0.2.2/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1716 2024-04-25 13:45:39.000000 feno-0.2.2/Readme.md
--rw-r--r--   0 lion      (1000) lion      (1000)     1396 2024-04-25 13:38:45.000000 feno-0.2.2/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      305 2024-04-25 14:08:21.000000 feno-0.2.2/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-25 14:39:42.163656 feno-0.2.2/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3157 2024-04-25 14:00:40.000000 feno-0.2.2/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.150322 feno-0.2.2/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.160322 feno-0.2.2/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-25 13:23:50.000000 feno-0.2.2/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2345 2024-04-25 14:26:59.000000 feno-0.2.2/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5534 2024-04-25 14:31:38.000000 feno-0.2.2/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.2.2/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.2.2/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.2.2/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9189 2024-04-19 14:04:18.000000 feno-0.2.2/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8932 2024-04-25 14:27:57.000000 feno-0.2.2/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4378 2024-04-08 17:28:46.000000 feno-0.2.2/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.2.2/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4907 2024-04-08 23:40:15.000000 feno-0.2.2/src/feno/lock.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.2.2/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11894 2024-04-08 15:58:02.000000 feno-0.2.2/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5043 2024-04-25 14:31:56.000000 feno-0.2.2/src/feno/remote_md.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 14:39:42.160322 feno-0.2.2/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2569 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      192 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-25 14:39:42.000000 feno-0.2.2/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 16:27:46.956692 feno-0.2.3/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.2.3/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.2.3/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2569 2024-04-25 16:27:46.956692 feno-0.2.3/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1716 2024-04-25 13:45:39.000000 feno-0.2.3/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     1396 2024-04-25 13:38:45.000000 feno-0.2.3/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      305 2024-04-25 14:08:21.000000 feno-0.2.3/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-25 16:27:46.956692 feno-0.2.3/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3157 2024-04-25 14:00:40.000000 feno-0.2.3/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 16:27:46.943359 feno-0.2.3/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 16:27:46.953359 feno-0.2.3/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-25 16:27:40.000000 feno-0.2.3/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2345 2024-04-25 14:26:59.000000 feno-0.2.3/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5534 2024-04-25 14:31:38.000000 feno-0.2.3/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.2.3/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.2.3/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.2.3/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9189 2024-04-25 16:11:18.000000 feno-0.2.3/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8932 2024-04-25 14:27:57.000000 feno-0.2.3/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4378 2024-04-08 17:28:46.000000 feno-0.2.3/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.2.3/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4907 2024-04-08 23:40:15.000000 feno-0.2.3/src/feno/lock.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.2.3/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11949 2024-04-25 16:13:59.000000 feno-0.2.3/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5043 2024-04-25 14:31:56.000000 feno-0.2.3/src/feno/remote_md.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-25 16:27:46.956692 feno-0.2.3/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2569 2024-04-25 16:27:46.000000 feno-0.2.3/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-25 16:27:46.000000 feno-0.2.3/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-25 16:27:46.000000 feno-0.2.3/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      192 2024-04-25 16:27:46.000000 feno-0.2.3/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-25 16:27:46.000000 feno-0.2.3/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-25 16:27:46.000000 feno-0.2.3/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.2.2/LICENSE` & `feno-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/PKG-INFO` & `feno-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.2.2
+Version: 0.2.3
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.2.2/Readme.md` & `feno-0.2.3/Readme.md`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/changelog.md` & `feno-0.2.3/changelog.md`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/setup.py` & `feno-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/__main__.py` & `feno-0.2.3/src/feno/__main__.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/actions.py` & `feno-0.2.3/src/feno/actions.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/cases.py` & `feno-0.2.3/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/check.py` & `feno-0.2.3/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/css_style.py` & `feno-0.2.3/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/filter.py` & `feno-0.2.3/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/html.py` & `feno-0.2.3/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/indexer.py` & `feno-0.2.3/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/jsontools.py` & `feno-0.2.3/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/lock.py` & `feno-0.2.3/src/feno/lock.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno/mdpp.py` & `feno-0.2.3/src/feno/mdpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
                 entries = sorted(os.listdir(directory))
                 for entry in entries:
                     full_path = os.path.join(directory, entry)
                     if os.path.isdir(full_path):
                         output += "  " * depth + "- " + entry + "\n"
                         output += traverse_directory(full_path, depth + 1)
                     else:
-                        output += "  " * depth + "- [" + entry + "](" + os.path.relpath(full_path, readme_dir) + ")\n"
+                        path = os.path.relpath(full_path, readme_dir).replace("\\", "/")
+                        output += "  " * depth + "- [" + entry + "](" + path + ")\n"
             return output
         
         origin = os.path.join(readme_dir, filter_dir)
         return traverse_directory(origin)
 
     @staticmethod
     def execute(path, content: str, action: Action = Action.RUN) -> str:
```

### Comparing `feno-0.2.2/src/feno/remote_md.py` & `feno-0.2.3/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.2.2/src/feno.egg-info/PKG-INFO` & `feno-0.2.3/src/feno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.2.2
+Version: 0.2.3
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.2.2/src/feno.egg-info/SOURCES.txt` & `feno-0.2.3/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

