# Comparing `tmp/omuplugin_obssync-0.3.1.tar.gz` & `tmp/omuplugin_obssync-0.3.2.tar.gz`

## Comparing `omuplugin_obssync-0.3.1.tar` & `omuplugin_obssync-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/src/omuplugin_obssync/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/src/omuplugin_obssync/__main__.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/src/omuplugin_obssync/plugin.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/src/omuplugin_obssync/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/__main__.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/src/omuplugin_obssync/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.2/PKG-INFO
```

### Comparing `omuplugin_obssync-0.3.1/src/omuplugin_obssync/plugin.py` & `omuplugin_obssync-0.3.2/src/omuplugin_obssync/plugin.py`

 * *Files identical despite different names*

### Comparing `omuplugin_obssync-0.3.1/pyproject.toml` & `omuplugin_obssync-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_obssync"
-version = "0.3.1"
+version = "0.3.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9", "psutil>=5.9.8"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

