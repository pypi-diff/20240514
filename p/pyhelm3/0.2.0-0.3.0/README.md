# Comparing `tmp/pyhelm3-0.2.0.tar.gz` & `tmp/pyhelm3-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelm3-0.2.0.tar", last modified: Thu Nov  9 15:04:04 2023, max compression
+gzip compressed data, was "pyhelm3-0.3.0.tar", last modified: Tue May 14 15:50:33 2024, max compression
```

## Comparing `pyhelm3-0.2.0.tar` & `pyhelm3-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 15:04:04.146619 pyhelm3-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 15:04:04.142619 pyhelm3-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 15:04:04.142619 pyhelm3-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-09 15:04:04.146619 pyhelm3-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 15:04:04.142619 pyhelm3-0.2.0/pyhelm3/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/pyhelm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/pyhelm3/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32386 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/pyhelm3/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/pyhelm3/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/pyhelm3/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 15:04:04.146619 pyhelm3-0.2.0/pyhelm3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-09 15:04:04.000000 pyhelm3-0.2.0/pyhelm3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-11-09 15:04:04.000000 pyhelm3-0.2.0/pyhelm3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 15:04:04.000000 pyhelm3-0.2.0/pyhelm3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 15:04:03.000000 pyhelm3-0.2.0/pyhelm3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-09 15:04:04.000000 pyhelm3-0.2.0/pyhelm3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-09 15:04:04.000000 pyhelm3-0.2.0/pyhelm3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2023-11-09 15:04:04.146619 pyhelm3-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2023-11-09 15:03:53.000000 pyhelm3-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.990490 pyhelm3-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.990490 pyhelm3-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.990490 pyhelm3-0.3.0/pyhelm3/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32859 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/pyhelm3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/setup.py
```

### Comparing `pyhelm3-0.2.0/.github/workflows/pypi-publish.yaml` & `pyhelm3-0.3.0/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.2.0/PKG-INFO` & `pyhelm3-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelm3
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library for managing Helm releases using Helm 3.
 Home-page: https://github.com/stackhpc/pyhelm3
 Author: Matt Pryor
 Author-email: matt@stackhpc.com
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
@@ -27,14 +27,16 @@
 from pyhelm3 import Client
 
 
 # This will use the Kubernetes configuration from the environment
 client = Client()
 # Specify the kubeconfig file to use
 client = Client(kubeconfig = "/path/to/kubeconfig")
+# Specify the kubecontext to use
+client = Client(kubecontext = "kubecontext")
 # Specify a custom Helm executable (by default, we expect 'helm' to be on the PATH)
 client = Client(executable = "/path/to/helm")
 
 
 # List the deployed releases
 releases = await client.list_releases(all = True, all_namespaces = True)
 for release in releases:
```

### Comparing `pyhelm3-0.2.0/README.md` & `pyhelm3-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from pyhelm3 import Client
 
 
 # This will use the Kubernetes configuration from the environment
 client = Client()
 # Specify the kubeconfig file to use
 client = Client(kubeconfig = "/path/to/kubeconfig")
+# Specify the kubecontext to use
+client = Client(kubecontext = "kubecontext")
 # Specify a custom Helm executable (by default, we expect 'helm' to be on the PATH)
 client = Client(executable = "/path/to/helm")
 
 
 # List the deployed releases
 releases = await client.list_releases(all = True, all_namespaces = True)
 for release in releases:
```

### Comparing `pyhelm3-0.2.0/pyhelm3/client.py` & `pyhelm3-0.3.0/pyhelm3/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,22 +49,24 @@
         command: t.Optional[Command] = None,
         *,
         default_timeout: t.Union[int, str] = "5m",
         executable: str = "helm",
         history_max_revisions: int = 10,
         insecure_skip_tls_verify: bool = False,
         kubeconfig: t.Optional[pathlib.Path] = None,
+        kubecontext: t.Optional[str] = None,
         unpack_directory: t.Optional[str] = None
     ):
         self._command = command or Command(
             default_timeout = default_timeout,
             executable = executable,
             history_max_revisions = history_max_revisions,
             insecure_skip_tls_verify = insecure_skip_tls_verify,
             kubeconfig = kubeconfig,
+            kubecontext = kubecontext,
             unpack_directory = unpack_directory
         )
 
     async def get_chart(
         self,
         chart_ref: t.Union[pathlib.Path, str],
         *,
```

### Comparing `pyhelm3-0.2.0/pyhelm3/command.py` & `pyhelm3-0.3.0/pyhelm3/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,22 +140,24 @@
         self,
         *,
         default_timeout: t.Union[int, str] = "5m",
         executable: str = "helm",
         history_max_revisions: int = 10,
         insecure_skip_tls_verify: bool = False,
         kubeconfig: t.Optional[pathlib.Path] = None,
+        kubecontext: t.Optional[str] = None,
         unpack_directory: t.Optional[str] = None
     ):
         self._logger = logging.getLogger(__name__)
         self._default_timeout = default_timeout
         self._executable = executable
         self._history_max_revisions = history_max_revisions
         self._insecure_skip_tls_verify = insecure_skip_tls_verify
         self._kubeconfig = kubeconfig
+        self._kubecontext = kubecontext
         self._unpack_directory = unpack_directory
 
     def _log_format(self, argument):
         argument = str(argument)
         if argument == "-":
             return "<stdin>"
         elif "\n" in argument:
@@ -166,14 +168,16 @@
     async def run(self, command: t.List[str], input: t.Optional[bytes] = None) -> bytes:
         """
         Run the given Helm command with the given input as stdin and 
         """
         command = [self._executable] + command
         if self._kubeconfig:
             command.extend(["--kubeconfig", self._kubeconfig])
+        if self._kubecontext:
+            command.extend(["--kube-context", self._kubecontext])
         # The command must be made up of str and bytes, so convert anything that isn't
         shell_formatted_command = shlex.join(
             part if isinstance(part, (str, bytes)) else str(part)
             for part in command
         )
         log_formatted_command = shlex.join(self._log_format(part) for part in command)
         self._logger.info("running command: %s", log_formatted_command)
@@ -185,16 +189,22 @@
             stderr = asyncio.subprocess.PIPE
         )
         try:
             stdout, stderr = await proc.communicate(input)
         except asyncio.CancelledError:
             # If the asyncio task is cancelled, terminate the Helm process but let the
             # process handle the termination and exit
-            proc.terminate()
-            stdout, stderr = await proc.communicate()
+            # We occassionally see a ProcessLookupError here if the process finished between
+            # us being cancelled and terminating the process, which we ignore as that is our
+            # target state anyway
+            try:
+                proc.terminate()
+                _ = await proc.communicate()
+            except ProcessLookupError:
+                pass
             # Once the process has exited, re-raise the cancelled error
             raise
         if proc.returncode == 0:
             self._logger.info("command succeeded: %s", log_formatted_command)
             return stdout
         else:
             self._logger.warning("command failed: %s", log_formatted_command)
```

### Comparing `pyhelm3-0.2.0/pyhelm3/errors.py` & `pyhelm3-0.3.0/pyhelm3/errors.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.2.0/pyhelm3/models.py` & `pyhelm3-0.3.0/pyhelm3/models.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.2.0/pyhelm3.egg-info/PKG-INFO` & `pyhelm3-0.3.0/pyhelm3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelm3
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library for managing Helm releases using Helm 3.
 Home-page: https://github.com/stackhpc/pyhelm3
 Author: Matt Pryor
 Author-email: matt@stackhpc.com
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
@@ -27,14 +27,16 @@
 from pyhelm3 import Client
 
 
 # This will use the Kubernetes configuration from the environment
 client = Client()
 # Specify the kubeconfig file to use
 client = Client(kubeconfig = "/path/to/kubeconfig")
+# Specify the kubecontext to use
+client = Client(kubecontext = "kubecontext")
 # Specify a custom Helm executable (by default, we expect 'helm' to be on the PATH)
 client = Client(executable = "/path/to/helm")
 
 
 # List the deployed releases
 releases = await client.list_releases(all = True, all_namespaces = True)
 for release in releases:
```

