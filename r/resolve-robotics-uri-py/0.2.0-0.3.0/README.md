# Comparing `tmp/resolve-robotics-uri-py-0.2.0.tar.gz` & `tmp/resolve_robotics_uri_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolve-robotics-uri-py-0.2.0.tar", last modified: Thu Feb 29 09:09:37 2024, max compression
+gzip compressed data, was "resolve_robotics_uri_py-0.3.0.tar", last modified: Tue May 14 13:16:48 2024, max compression
```

## Comparing `resolve-robotics-uri-py-0.2.0.tar` & `resolve_robotics_uri_py-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:09:37.832299 resolve-robotics-uri-py-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:09:37.828299 resolve-robotics-uri-py-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:09:37.828299 resolve-robotics-uri-py-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-02-29 09:09:37.832299 resolve-robotics-uri-py-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/ci_env.yml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-02-29 09:09:37.832299 resolve-robotics-uri-py-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:09:37.828299 resolve-robotics-uri-py-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:09:37.828299 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py/resolve_robotics_uri_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:09:37.832299 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-02-29 09:09:37.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-29 09:09:37.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:09:37.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-29 09:09:37.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:09:37.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-29 09:09:37.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-29 09:09:37.000000 resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:09:37.832299 resolve-robotics-uri-py-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-02-29 09:09:30.000000 resolve-robotics-uri-py-0.2.0/test/test_resolve_robotics_uri_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:48.164945 resolve_robotics_uri_py-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:48.160945 resolve_robotics_uri_py-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:48.164945 resolve_robotics_uri_py-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-14 13:16:48.164945 resolve_robotics_uri_py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/ci_env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-14 13:16:48.164945 resolve_robotics_uri_py-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:48.160945 resolve_robotics_uri_py-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:48.164945 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py/resolve_robotics_uri_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:48.164945 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-14 13:16:48.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 13:16:48.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:16:48.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 13:16:48.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:16:47.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 13:16:48.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 13:16:48.000000 resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:48.164945 resolve_robotics_uri_py-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-14 13:16:43.000000 resolve_robotics_uri_py-0.3.0/test/test_resolve_robotics_uri_py.py
```

### Comparing `resolve-robotics-uri-py-0.2.0/.github/workflows/ci.yml` & `resolve_robotics_uri_py-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `resolve-robotics-uri-py-0.2.0/.github/workflows/publish-to-pypi.yml` & `resolve_robotics_uri_py-0.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `resolve-robotics-uri-py-0.2.0/.gitignore` & `resolve_robotics_uri_py-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `resolve-robotics-uri-py-0.2.0/LICENSE` & `resolve_robotics_uri_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resolve-robotics-uri-py-0.2.0/PKG-INFO` & `resolve_robotics_uri_py-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resolve-robotics-uri-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pure python package to solve ROS-style package:// and Gazebo-style model:// URIs in absolute paths.
 Home-page: https://github.com/ami-iit/resolve-robotics-uri-py
 Author: Silvio Traversaro
 Author-email: silvio.traversaro@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/resolve-robotics-uri-py/releases
 Project-URL: Source, https://github.com/ami-iit/resolve-robotics-uri-py
```

### Comparing `resolve-robotics-uri-py-0.2.0/README.md` & `resolve_robotics_uri_py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `resolve-robotics-uri-py-0.2.0/setup.cfg` & `resolve_robotics_uri_py-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py/resolve_robotics_uri_py.py` & `resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py/resolve_robotics_uri_py.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,27 +72,40 @@
 
 
 # ===================
 # URI resolving logic
 # ===================
 
 
-def resolve_robotics_uri(uri: str) -> pathlib.Path:
+def resolve_robotics_uri(
+    uri: str, package_dirs: list[str] | None = None
+) -> pathlib.Path:
     """
     Resolve a robotics URI to an absolute filename.
 
     Args:
         uri: The URI to resolve.
+        package_dirs: A list of additional paths to look for the file.
 
     Returns:
         The absolute filename corresponding to the URI.
 
     Raises:
         FileNotFoundError: If no file corresponding to the URI is found.
+
+    Note:
+        By default the function will look for the file in the
+        default search paths specified by the environment variables in `SupportedEnvVars`.
+ 
+        If the `package_dirs` argument is provided, the model is also searched in the folders
+        specified in `package_dirs` . In particular if a file is specified by the uri
+        `package://ModelName/meshes/mesh.stl`, and the actual file is in 
+        `/usr/local/share/ModelName/meshes/mesh.stl`, the `package_dirs` should contain `/usr/local/share`.
     """
+    package_dirs = package_dirs if isinstance(package_dirs, list) else [package_dirs]
 
     # If the URI has no scheme, use by default file:// which maps the resolved input
     # path to a URI with empty authority
     if not any(uri.startswith(scheme) for scheme in SupportedSchemes):
         uri = f"file://{pathlib.Path(uri).resolve()}"
 
     # ================================================
@@ -100,16 +113,16 @@
     # ================================================
 
     # This is the file URI scheme as per RFC8089:
     # https://datatracker.ietf.org/doc/html/rfc8089
 
     if uri.startswith("file:"):
         # Strip the scheme from the URI
-        uri = uri.replace(f"file://", "")
-        uri = uri.replace(f"file:", "")
+        uri = uri.replace("file://", "")
+        uri = uri.replace("file:", "")
 
         # Create the file path, resolving symlinks and '..'
         uri_file_path = pathlib.Path(uri).resolve()
 
         # Check that the file exists
         if not uri_file_path.is_file():
             msg = "resolve-robotics-uri-py: No file corresponding to URI '{}' found"
@@ -141,15 +154,19 @@
     uri_path = uri
     uri_path = uri_path.replace(f"{parsed_uri.scheme}://", "")
 
     # List of matching resources found
     model_filenames = []
 
     # Search the resource in the path from the env variables
-    for folder in set(get_search_paths_from_envs(SupportedEnvVars)):
+    for folder in set(get_search_paths_from_envs(SupportedEnvVars)) | {
+        path
+        for directory in package_dirs
+        if directory and (path := pathlib.Path(directory)).exists()
+    }:
 
         # Join the folder from environment variable and the URI path
         candidate_file_name = folder / uri_path
 
         # Expand or resolve the file path (symlinks and ..)
         candidate_file_name = candidate_file_name.resolve()
 
@@ -177,19 +194,26 @@
 def main():
     parser = argparse.ArgumentParser(
         description="Utility resolve a robotics URI ({}) to an absolute filename.".format(
             ", ".join(f"{scheme}://" for scheme in SupportedSchemes)
         )
     )
     parser.add_argument("uri", metavar="URI", type=str, help="URI to resolve")
+    parser.add_argument(
+        "--package_dirs",
+        metavar="PATH",
+        type=str,
+        help="Additional paths to look for the file",
+        default=None,
+    )
 
     args = parser.parse_args()
 
     try:
-        result = resolve_robotics_uri(args.uri)
+        result = resolve_robotics_uri(args.uri, args.package_dirs)
     except FileNotFoundError as e:
         print(e, file=sys.stderr)
         sys.exit(1)
 
     print(result, file=sys.stdout)
     sys.exit(0)
```

### Comparing `resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/PKG-INFO` & `resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resolve-robotics-uri-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pure python package to solve ROS-style package:// and Gazebo-style model:// URIs in absolute paths.
 Home-page: https://github.com/ami-iit/resolve-robotics-uri-py
 Author: Silvio Traversaro
 Author-email: silvio.traversaro@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/resolve-robotics-uri-py/releases
 Project-URL: Source, https://github.com/ami-iit/resolve-robotics-uri-py
```

### Comparing `resolve-robotics-uri-py-0.2.0/src/resolve_robotics_uri_py.egg-info/SOURCES.txt` & `resolve_robotics_uri_py-0.3.0/src/resolve_robotics_uri_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resolve-robotics-uri-py-0.2.0/test/test_resolve_robotics_uri_py.py` & `resolve_robotics_uri_py-0.3.0/test/test_resolve_robotics_uri_py.py`

 * *Files 8% similar despite different names*

```diff
@@ -152,11 +152,33 @@
         temp_name = pathlib.Path(temp.name).resolve(strict=True)
         uri_file = f"{temp_name}"
         path_of_file = resolve_robotics_uri_py.resolve_robotics_uri(uri_file)
         assert path_of_file == path_of_file.resolve()
         assert path_of_file == temp_name
 
     # Try to find an existing file (the Python executable) without any file:/ scheme
-    path_of_python_executable = resolve_robotics_uri_py.resolve_robotics_uri(sys.executable)
+    path_of_python_executable = resolve_robotics_uri_py.resolve_robotics_uri(
+        sys.executable
+    )
     assert path_of_python_executable == pathlib.Path(sys.executable)
 
 
+def test_additional_search_path():
+
+    import tempfile
+    import pathlib
+    import resolve_robotics_uri_py
+
+    clear_env_vars()
+
+    uri = "model://my_model"
+
+    with tempfile.TemporaryDirectory() as temp_dir:
+
+        temp_dir_path = pathlib.Path(temp_dir).resolve()
+        temp_dir_path.mkdir(exist_ok=True)
+        top_level = temp_dir_path / "my_model"
+        top_level.touch(exist_ok=True)
+
+        # Test resolving a URI with an additional search path
+        result = resolve_robotics_uri_py.resolve_robotics_uri(uri, temp_dir)
+        assert result == temp_dir_path / "my_model"
```

