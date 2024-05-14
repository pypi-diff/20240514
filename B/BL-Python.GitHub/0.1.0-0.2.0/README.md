# Comparing `tmp/BL_Python.GitHub-0.1.0.tar.gz` & `tmp/bl_python_github-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BL_Python.GitHub-0.1.0.tar", last modified: Wed Feb  7 18:58:25 2024, max compression
+gzip compressed data, was "bl_python_github-0.2.0.tar", last modified: Tue May 14 21:36:25 2024, max compression
```

## Comparing `BL_Python.GitHub-0.1.0.tar` & `bl_python_github-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:25.060805 BL_Python.GitHub-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:25.056805 BL_Python.GitHub-0.1.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:25.060805 BL_Python.GitHub-0.1.0/BL_Python/GitHub/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-07 18:58:09.000000 BL_Python.GitHub-0.1.0/BL_Python/GitHub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-02-07 18:58:09.000000 BL_Python.GitHub-0.1.0/BL_Python/GitHub/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:25.060805 BL_Python.GitHub-0.1.0/BL_Python.GitHub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-07 18:58:25.000000 BL_Python.GitHub-0.1.0/BL_Python.GitHub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-07 18:58:25.000000 BL_Python.GitHub-0.1.0/BL_Python.GitHub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:58:25.000000 BL_Python.GitHub-0.1.0/BL_Python.GitHub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-07 18:58:25.000000 BL_Python.GitHub-0.1.0/BL_Python.GitHub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-07 18:58:25.000000 BL_Python.GitHub-0.1.0/BL_Python.GitHub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-07 18:58:09.000000 BL_Python.GitHub-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-07 18:58:09.000000 BL_Python.GitHub-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-07 18:58:25.060805 BL_Python.GitHub-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-07 18:58:09.000000 BL_Python.GitHub-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:58:09.000000 BL_Python.GitHub-0.1.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-02-07 18:58:09.000000 BL_Python.GitHub-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 18:58:25.060805 BL_Python.GitHub-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:36:25.955795 bl_python_github-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:36:25.951795 bl_python_github-0.2.0/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:36:25.955795 bl_python_github-0.2.0/BL_Python/GitHub/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 21:36:18.000000 bl_python_github-0.2.0/BL_Python/GitHub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-14 21:36:18.000000 bl_python_github-0.2.0/BL_Python/GitHub/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:36:25.955795 bl_python_github-0.2.0/BL_Python.GitHub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 21:36:25.000000 bl_python_github-0.2.0/BL_Python.GitHub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-14 21:36:25.000000 bl_python_github-0.2.0/BL_Python.GitHub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:36:25.000000 bl_python_github-0.2.0/BL_Python.GitHub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 21:36:25.000000 bl_python_github-0.2.0/BL_Python.GitHub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 21:36:25.000000 bl_python_github-0.2.0/BL_Python.GitHub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:36:18.000000 bl_python_github-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 21:36:18.000000 bl_python_github-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-14 21:36:25.955795 bl_python_github-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 21:36:18.000000 bl_python_github-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:36:18.000000 bl_python_github-0.2.0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 21:36:18.000000 bl_python_github-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:36:25.955795 bl_python_github-0.2.0/setup.cfg
```

### Comparing `BL_Python.GitHub-0.1.0/BL_Python/GitHub/api.py` & `bl_python_github-0.2.0/BL_Python/GitHub/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,15 @@
     ):
         ## repo = organization.get_repo(repository_name)
         ## can't use repo.organization because of this
         ## https://github.com/PyGithub/PyGithub/issues/1598
         repository = self._client.get_repo(f"{organization_name}/{repository_name}")
         organization: Organization = self._client.get_organization(organization_name)
         # fixes the PyGithub API URLs for working with the organiztion owning the repository
-        cast(
-            Any, repository._organization  # pyright: ignore[reportPrivateUsage]
-        )._value = organization
+        cast(Any, repository._organization)._value = organization  # pyright: ignore[reportPrivateUsage]
         return repository
 
     def create_repository(
         self,
         name: str,
         description: str,
         organization_name: str | None = None,
```

### Comparing `BL_Python.GitHub-0.1.0/BL_Python.GitHub.egg-info/PKG-INFO` & `bl_python_github-0.2.0/BL_Python.GitHub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.GitHub
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for working with the GitHub API in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `BL_Python.GitHub-0.1.0/LICENSE.md` & `bl_python_github-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `BL_Python.GitHub-0.1.0/PKG-INFO` & `bl_python_github-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.GitHub
-Version: 0.1.0
+Version: 0.2.0
 Summary: Libraries for working with the GitHub API in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `BL_Python.GitHub-0.1.0/pyproject.toml` & `bl_python_github-0.2.0/pyproject.toml`

 * *Files identical despite different names*

