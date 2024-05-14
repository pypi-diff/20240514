# Comparing `tmp/zntrack-0.7.2.tar.gz` & `tmp/zntrack-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zntrack-0.7.2.tar", max compression
+gzip compressed data, was "zntrack-0.7.3.tar", max compression
```

## Comparing `zntrack-0.7.2.tar` & `zntrack-0.7.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.7.2/LICENSE
--rw-r--r--   0        0        0     6531 2023-11-09 13:20:12.826008 zntrack-0.7.2/README.md
--rw-r--r--   0        0        0     2507 2023-12-19 12:01:44.157602 zntrack-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1147 2023-11-09 13:20:12.836008 zntrack-0.7.2/zntrack/__init__.py
--rw-r--r--   0        0        0     3201 2023-11-09 13:20:12.836008 zntrack-0.7.2/zntrack/cli/__init__.py
--rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.7.2/zntrack/core/__init__.py
--rw-r--r--   0        0        0     4641 2023-12-19 13:11:50.471836 zntrack-0.7.2/zntrack/core/load.py
--rw-r--r--   0        0        0    15550 2023-12-19 13:34:39.777050 zntrack-0.7.2/zntrack/core/node.py
--rw-r--r--   0        0        0    14012 2023-11-09 10:06:42.602104 zntrack-0.7.2/zntrack/core/nodify.py
--rw-r--r--   0        0        0     7285 2023-12-19 12:01:44.167602 zntrack-0.7.2/zntrack/examples/__init__.py
--rw-r--r--   0        0        0     2079 2023-12-18 14:23:21.590313 zntrack-0.7.2/zntrack/exceptions/__init__.py
--rw-r--r--   0        0        0      195 2023-08-16 15:28:21.013916 zntrack-0.7.2/zntrack/fields/__init__.py
--rw-r--r--   0        0        0    10977 2023-11-09 10:50:26.663685 zntrack-0.7.2/zntrack/fields/dependency.py
--rw-r--r--   0        0        0     2019 2023-11-09 10:06:42.682103 zntrack-0.7.2/zntrack/fields/dvc/__init__.py
--rw-r--r--   0        0        0     5156 2023-12-19 12:01:44.167602 zntrack-0.7.2/zntrack/fields/dvc/options.py
--rw-r--r--   0        0        0    10088 2023-11-09 10:06:42.702103 zntrack-0.7.2/zntrack/fields/field.py
--rw-r--r--   0        0        0     4591 2023-11-09 10:06:42.702103 zntrack-0.7.2/zntrack/fields/fields.py
--rw-r--r--   0        0        0     3559 2023-11-09 10:06:42.722102 zntrack-0.7.2/zntrack/fields/meta/__init__.py
--rw-r--r--   0        0        0     1073 2023-09-22 15:57:25.294219 zntrack-0.7.2/zntrack/fields/zn/__init__.py
--rw-r--r--   0        0        0    18848 2023-11-09 10:50:31.823629 zntrack-0.7.2/zntrack/fields/zn/options.py
--rw-r--r--   0        0        0     2649 2023-11-09 10:06:42.762102 zntrack-0.7.2/zntrack/notebooks/jupyter.py
--rw-r--r--   0        0        0      160 2023-11-09 10:06:42.762102 zntrack-0.7.2/zntrack/project/__init__.py
--rw-r--r--   0        0        0    16932 2023-12-19 13:34:39.777050 zntrack-0.7.2/zntrack/project/zntrack_project.py
--rw-r--r--   0        0        0     1823 2023-11-09 10:06:42.772102 zntrack-0.7.2/zntrack/tools/__init__.py
--rw-r--r--   0        0        0     8735 2023-12-19 12:01:44.167602 zntrack-0.7.2/zntrack/utils/__init__.py
--rw-r--r--   0        0        0     3908 2023-11-09 13:20:12.836008 zntrack-0.7.2/zntrack/utils/cli.py
--rw-r--r--   0        0        0     3882 2023-12-19 12:01:44.167602 zntrack-0.7.2/zntrack/utils/config.py
--rw-r--r--   0        0        0     4777 2023-11-09 10:06:42.832101 zntrack-0.7.2/zntrack/utils/file_io.py
--rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.7.2/zntrack/utils/node_wd.py
--rw-r--r--   0        0        0     7703 1970-01-01 00:00:00.000000 zntrack-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-31 09:35:21.669596 zntrack-0.7.3/LICENSE
+-rw-r--r--   0        0        0     6885 2024-02-23 09:23:56.246870 zntrack-0.7.3/README.md
+-rw-r--r--   0        0        0     2452 2024-02-23 09:23:56.416868 zntrack-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1198 2024-05-14 14:41:45.763068 zntrack-0.7.3/zntrack/__init__.py
+-rw-r--r--   0        0        0     3524 2024-05-14 14:41:45.763068 zntrack-0.7.3/zntrack/cli/__init__.py
+-rw-r--r--   0        0        0       30 2023-03-16 14:38:52.662721 zntrack-0.7.3/zntrack/core/__init__.py
+-rw-r--r--   0        0        0     4641 2023-12-19 13:11:50.471836 zntrack-0.7.3/zntrack/core/load.py
+-rw-r--r--   0        0        0    16778 2024-05-14 14:41:45.763068 zntrack-0.7.3/zntrack/core/node.py
+-rw-r--r--   0        0        0    14012 2023-11-09 10:06:42.602104 zntrack-0.7.3/zntrack/core/nodify.py
+-rw-r--r--   0        0        0     8273 2024-05-14 14:41:45.763068 zntrack-0.7.3/zntrack/examples/__init__.py
+-rw-r--r--   0        0        0     2080 2024-01-20 21:51:57.498587 zntrack-0.7.3/zntrack/exceptions/__init__.py
+-rw-r--r--   0        0        0      195 2023-08-16 15:28:21.013916 zntrack-0.7.3/zntrack/fields/__init__.py
+-rw-r--r--   0        0        0    10977 2023-11-09 10:50:26.663685 zntrack-0.7.3/zntrack/fields/dependency.py
+-rw-r--r--   0        0        0     2019 2023-11-09 10:06:42.682103 zntrack-0.7.3/zntrack/fields/dvc/__init__.py
+-rw-r--r--   0        0        0     5156 2023-12-19 12:01:44.167602 zntrack-0.7.3/zntrack/fields/dvc/options.py
+-rw-r--r--   0        0        0    10088 2023-11-09 10:06:42.702103 zntrack-0.7.3/zntrack/fields/field.py
+-rw-r--r--   0        0        0     4591 2023-11-09 10:06:42.702103 zntrack-0.7.3/zntrack/fields/fields.py
+-rw-r--r--   0        0        0     3559 2023-11-09 10:06:42.722102 zntrack-0.7.3/zntrack/fields/meta/__init__.py
+-rw-r--r--   0        0        0     1073 2023-09-22 15:57:25.294219 zntrack-0.7.3/zntrack/fields/zn/__init__.py
+-rw-r--r--   0        0        0    18848 2023-11-09 10:50:31.823629 zntrack-0.7.3/zntrack/fields/zn/options.py
+-rw-r--r--   0        0        0     2649 2023-11-09 10:06:42.762102 zntrack-0.7.3/zntrack/notebooks/jupyter.py
+-rw-r--r--   0        0        0      160 2023-11-09 10:06:42.762102 zntrack-0.7.3/zntrack/project/__init__.py
+-rw-r--r--   0        0        0    18470 2024-05-14 14:41:45.773068 zntrack-0.7.3/zntrack/project/zntrack_project.py
+-rw-r--r--   0        0        0     1823 2023-11-09 10:06:42.772102 zntrack-0.7.3/zntrack/tools/__init__.py
+-rw-r--r--   0        0        0     9095 2024-05-14 14:06:11.145240 zntrack-0.7.3/zntrack/utils/__init__.py
+-rw-r--r--   0        0        0      639 2024-05-14 14:41:45.773068 zntrack-0.7.3/zntrack/utils/apply.py
+-rw-r--r--   0        0        0     3908 2023-11-09 13:20:12.836008 zntrack-0.7.3/zntrack/utils/cli.py
+-rw-r--r--   0        0        0     3882 2023-12-19 12:01:44.167602 zntrack-0.7.3/zntrack/utils/config.py
+-rw-r--r--   0        0        0     4777 2023-11-09 10:06:42.832101 zntrack-0.7.3/zntrack/utils/file_io.py
+-rw-r--r--   0        0        0     1500 2023-03-17 15:52:43.708117 zntrack-0.7.3/zntrack/utils/node_wd.py
+-rw-r--r--   0        0        0     8039 1970-01-01 00:00:00.000000 zntrack-0.7.3/PKG-INFO
```

### Comparing `zntrack-0.7.2/LICENSE` & `zntrack-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/README.md` & `zntrack-0.7.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![codecov](https://codecov.io/gh/zincware/ZnTrack/branch/main/graph/badge.svg?token=ZQ67FXN1IT)](https://codecov.io/gh/zincware/ZnTrack)
 [![Maintainability](https://api.codeclimate.com/v1/badges/f25e119bbd5d5ec74e2c/maintainability)](https://codeclimate.com/github/zincware/ZnTrack/maintainability)
 ![PyTest](https://github.com/zincware/ZnTrack/actions/workflows/test.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/zntrack.svg)](https://badge.fury.io/py/zntrack)
 [![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Documentation](https://readthedocs.org/projects/zntrack/badge/?version=latest)](https://zntrack.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnTrack/HEAD)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6472850.svg)](https://doi.org/10.5281/zenodo.6472850)
+[![DOI](https://img.shields.io/badge/arXiv-2401.10603-red)](https://arxiv.org/abs/2401.10603)
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 ![Logo](https://raw.githubusercontent.com/zincware/ZnTrack/main/docs/source/_static/logo_ZnTrack.png)
 
 # ZnTrack: A Parameter Tracking Package for Python
 
@@ -131,14 +131,28 @@
 On a fundamental level the ZnTrack package provides an easy-to-use interface for
 DVC directly from Python. It handles all the computational overhead of reading
 config files, defining outputs in the `dvc.yaml` as well as in the script and
 much more.
 
 For more information on DVC visit their [homepage](https://dvc.org/doc).
 
+# References
+
+If you use ZnTrack in your research and find it helpful please cite us.
+
+```bibtex
+@misc{zillsZnTrackDataCode2024,
+  title = {{{ZnTrack}} -- {{Data}} as {{Code}}},
+  author = {Zills, Fabian and Sch{\"a}fer, Moritz and Tovey, Samuel and K{\"a}stner, Johannes and Holm, Christian},
+  year = {2024},
+  eprint={2401.10603},
+  archivePrefix={arXiv},
+}
+```
+
 # Copyright
 
 This project is distributed under the
 [Apache License Version 2.0](https://github.com/zincware/ZnTrack/blob/main/LICENSE).
 
 ## Similar Tools
```

### Comparing `zntrack-0.7.2/pyproject.toml` & `zntrack-0.7.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 [tool.poetry]
 name = "ZnTrack"
-version = "0.7.2"
+version = "0.7.3"
 description = "Create, Run and Benchmark DVC Pipelines in Python"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "data-version-control", "machine-learning", "reproducibility", "collaboration"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0.0"
-dvc = "^3.2.2"
-pyyaml = "^6.0"
-tqdm = "^4.64.0"
+python = ">=3.9,<4.0.0"
+dvc = "^3.3"
+pyyaml = "^6"
+tqdm = "^4"
 pandas = "^2"
-typer = "^0.7.0"
+typer = "^0.7"
 
-dot4dict = "^0.1.1"
-zninit = "^0.1.11"
-znjson = "^0.2.2"
-znflow = "^0.1.14"
-typing-extensions = "^4.8.0"
+dot4dict = "^0.1"
+zninit = "^0.1"
+znjson = "^0.2"
+znflow = "^0.1"
+varname = "^0.13"
+# for Python3.12 compatibliity
+pyzmq = "^25"
 
 
 [tool.poetry.urls]
 documentation = "https://zntrack.readthedocs.io"
 repository = "https://github.com/zincware/ZnTrack"
 
 
 [tool.poetry.scripts]
 zntrack = "zntrack.cli:app"
 
 [tool.poetry.group.dev.dependencies]
-pytest-benchmark = "^3.4.1"
-pytest = "^7.1.2"
-numpy = "^1.23"
-matplotlib = "^3.5.2"
-ase = "^3.22.1"
-pre-commit = ">=2.20,<4.0"
-coverage = "^6.4"
-pytest-xdist = "^2.5.0"
-optuna = "^3.1.1"
-scikit-learn = "^1.2.2"
-nbmake = "1.4.3"
+pytest-benchmark = "^3"
+pytest = "^7"
+numpy = "^1"
+matplotlib = "^3"
+ase = "^3"
+pre-commit = "^2"
+coverage = "^6"
+pytest-xdist = "^2"
+optuna = "^3"
+scikit-learn = "^1"
+nbmake = "^1"
 
 [tool.poetry.group.notebook.dependencies]
-jupyterlab = "^3.4.3"
+jupyterlab = "^3"
 
 [tool.poetry.group.docs.dependencies]
-furo = "^2022.12.7"
-sphinx-copybutton = "^0.5.1"
-sphinx = "^6.1.3"
-nbsphinx = "^0.8.12"
-nbsphinx-link = "^1.3.0"
+furo = "^2022"
+sphinx-copybutton = "^0.5"
+sphinx = "^6"
+nbsphinx = "^0.8"
+nbsphinx-link = "^1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
```

### Comparing `zntrack-0.7.2/zntrack/__init__.py` & `zntrack-0.7.3/zntrack/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     params,
     params_path,
     plots,
     plots_path,
 )
 from zntrack.project import Project
 from zntrack.utils import config
+from zntrack.utils.apply import apply
 from zntrack.utils.node_wd import nwd
 
 __version__ = importlib.metadata.version("zntrack")
 
 __all__ = [
     "Node",
     "dvc",
@@ -41,14 +42,15 @@
     "FieldGroup",
     "nodify",
     "NodeConfig",
     "tools",
     "exceptions",
     "from_rev",
     "get_nodes",
+    "apply",
 ]
 
 __all__ += [
     "outs",
     "metrics",
     "params",
     "deps",
```

### Comparing `zntrack-0.7.2/zntrack/cli/__init__.py` & `zntrack-0.7.3/zntrack/cli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,18 +43,31 @@
     ),
 ) -> None:
     """ZnTrack CLI main callback."""
     _ = version  # this would be greyed out otherwise
 
 
 @app.command()
-def run(node: str, name: str = None, meta_only: bool = False) -> None:
+def run(
+    node: str, name: str = None, meta_only: bool = False, method: str = "run"
+) -> None:
     """Execute a ZnTrack Node.
 
     Use as 'zntrack run module.Node --name node_name'.
+
+    Arguments:
+    ---------
+    node : str
+        The node to run.
+    name : str
+        The name of the node.
+    meta_only : bool
+        Save only the metadata.
+    method : str, default 'run'
+        The method to run on the node.
     """
     env_file = pathlib.Path("env.yaml")
     if env_file.exists():
         env = yaml.safe_load(env_file.read_text())
         os.environ.update(env.get("global", {}))
 
         for key, value in env.get("stages", {}).get(name, {}).items():
@@ -74,18 +87,19 @@
 
     cls = getattr(module, cls)
 
     if getattr(cls, "is_node", False):
         cls(exec_func=True)
     elif issubclass(cls, Node):
         node: Node = cls.from_rev(name=name, results=False)
+        node.save(meta_only=True)
         if not meta_only:
-            node.run()
+            # dynamic version of node.run()
+            getattr(node, method)()
             node.save(parameter=False)
-        node.save(meta_only=True)
     else:
         raise ValueError(f"Node {node} is not a ZnTrack Node.")
 
 
 @app.command()
 def init(
     name: str = "New Project",
```

### Comparing `zntrack-0.7.2/zntrack/core/load.py` & `zntrack-0.7.3/zntrack/core/load.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/core/node.py` & `zntrack-0.7.3/zntrack/core/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import dvc.api
 import dvc.cli
 import dvc.utils.strictyaml
 import znflow
 import zninit
 import znjson
+from varname import VarnameException, varname
 
 from zntrack import exceptions
 from zntrack.notebooks.jupyter import jupyter_class_to_file
 from zntrack.utils import (
     DISABLE_TMP_PATH,
     NodeName,
     NodeStatusResults,
@@ -63,14 +64,15 @@
     loaded: bool
     results: "NodeStatusResults"
     remote: str = None
     rev: str = None
     tmp_path: pathlib.Path = dataclasses.field(
         default=DISABLE_TMP_PATH, init=False, repr=False
     )
+    _run_count: int = dataclasses.field(default=0, init=False, repr=False)
 
     @functools.cached_property
     def fs(self) -> dvc.api.DVCFileSystem:
         """Get the file system of the Node."""
         for _ in range(10):
             try:
                 return dvc.api.DVCFileSystem(
@@ -140,14 +142,28 @@
                 finally:
                     files = list(self.tmp_path.glob("**/*"))
                     log.debug(
                         f"Deleting temporary directory {self.tmp_path} containing {files}"
                     )
                     self.tmp_path = None
 
+    def _increment_run_count(self) -> None:
+        """Increment the run count."""
+        self._run_count += 1
+
+    @property
+    def run_count(self) -> int:
+        """Get the run count."""
+        return self._run_count
+
+    @property
+    def restarted(self) -> bool:
+        """Whether the node was restarted."""
+        return self._run_count > 1
+
 
 class _NameDescriptor(zninit.Descriptor):
     """A descriptor for the name attribute."""
 
     def __get__(self, instance, owner=None):
         if instance is None:
             return self
@@ -157,16 +173,20 @@
 
     def __set__(self, instance, value):
         if value is None:
             return
         if isinstance(value, NodeName):
             if not instance._external_:
                 value.update_suffix(instance._graph_.project, instance)
+            with contextlib.suppress(VarnameException):
+                value.varname = varname(frame=4)
             instance._name_ = value
         elif isinstance(getattr(instance, "_name_"), NodeName):
+            with contextlib.suppress(VarnameException):
+                instance._name_.varname = varname(frame=4)
             instance._name_.name = value
             instance._name_.suffix = 0
             instance._name_.update_suffix(instance._graph_.project, instance)
         else:
             # This should only happen if an instance is loaded.
             instance._name_ = value
 
@@ -251,15 +271,17 @@
         self, parameter: bool = True, results: bool = True, meta_only: bool = False
     ) -> None:
         """Save the node's output to disk."""
         if meta_only:
             # the meta data will only be written here.
             import json
 
-            (self.nwd / "node-meta.json").write_text(json.dumps({"uuid": str(self.uuid)}))
+            (self.nwd / "node-meta.json").write_text(
+                json.dumps({"uuid": str(self.uuid), "run_count": self.state.run_count})
+            )
             return
 
         # TODO have an option to save and run dvc commit afterwards.
 
         # TODO: check if there is a difference in saving
         # a loaded node vs a new node and why
         from zntrack.fields import Field, FieldGroup
@@ -313,22 +335,23 @@
                 for attr in zninit.get_descriptors(Field, self=self):
                     if attr.group == FieldGroup.RESULT and not results:
                         continue
                     attr.load(self)
         except KeyError as err:
             raise exceptions.NodeNotAvailableError(self) from err
 
-        if results:
-            with contextlib.suppress(FileNotFoundError):
-                # If the uuid is available, we can assume that all data for
-                #  this Node is available.
-                with self.state.fs.open(get_nwd(self) / "node-meta.json") as f:
-                    node_meta = json.load(f)
-                    self._uuid = uuid.UUID(node_meta["uuid"])
-                    self.state.results = NodeStatusResults.AVAILABLE
+        with contextlib.suppress(FileNotFoundError):
+            # If the uuid is available, we can assume that all data for
+            #  this Node is available.
+            with self.state.fs.open(get_nwd(self) / "node-meta.json") as f:
+                node_meta = json.load(f)
+                self._uuid = uuid.UUID(node_meta["uuid"])
+                self.state._run_count = node_meta.get("run_count", -1)
+                # in older versions, the run_count was not saved.
+                self.state.results = NodeStatusResults.AVAILABLE
         # TODO: documentation about _post_init and _post_load_ and when they are called
 
         zntrack_config = json.loads(self.state.fs.read_text(config.files.zntrack))
 
         if self.name not in zntrack_config:
             raise exceptions.NodeNotAvailableError(self)
 
@@ -364,14 +387,20 @@
             node.load(results=results)
 
         if remote is not None or rev is not None:
             # by default, tmp_path is disabled.
             # if remote or rev is set, we enable it.
             node.state.tmp_path = None
 
+        if not results:
+            # if a node is loaded without results and saved afterwards,
+            #  we count this as a run.
+            node.state._increment_run_count()
+            log.debug(f"Setting run count to {node.state.run_count} for {node}")
+
         return node
 
 
 def get_dvc_cmd(
     node: Node,
     git_only_repo: bool,
     quiet: bool = False,
@@ -410,15 +439,21 @@
 
     if git_only_repo:
         cmd += ["--metrics-no-cache", f"{(get_nwd(node) /'node-meta.json').as_posix()}"]
     else:
         cmd += ["--outs", f"{(get_nwd(node) /'node-meta.json').as_posix()}"]
 
     module = module_handler(node.__class__)
-    cmd += [f"zntrack run {module}.{node.__class__.__name__} --name {node.name}"]
+
+    zntrack_run = f"zntrack run {module}.{node.__class__.__name__} --name {node.name}"
+    if hasattr(node, "_method"):
+        zntrack_run += f" --method {node._method}"
+
+    cmd += [zntrack_run]
+
     optionals = [x for x in optionals if x]  # remove empty entries []
     return [cmd] + optionals
 
 
 @dataclasses.dataclass
 class NodeIdentifier:
     """All information that uniquely identifies a node."""
```

### Comparing `zntrack-0.7.2/zntrack/core/nodify.py` & `zntrack-0.7.3/zntrack/core/nodify.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/examples/__init__.py` & `zntrack-0.7.3/zntrack/examples/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     params = zntrack.params()
     outs = zntrack.outs()
 
     def run(self) -> None:
         """Save params to outs."""
         self.outs = self.params
 
+    def join(self) -> None:
+        """Join the results."""
+        self.outs = "-".join(self.params)
+
 
 class ParamsToMetrics(zntrack.Node):
     """Save params to metrics."""
 
     params = zntrack.params()
     metrics = zntrack.metrics()
 
@@ -145,15 +149,15 @@
             return pathlib.Path(self.outs).read_text()
 
 
 class WriteDVCOutsSequence(zntrack.Node):
     """Write an output file."""
 
     params: list = zntrack.params()
-    outs: list | tuple | set | dict = zntrack.outs_path()
+    outs: t.Union[list, tuple, set, dict] = zntrack.outs_path()
 
     def run(self):
         """Write an output file."""
         for value, path in zip(self.params, self.outs):
             pathlib.Path(path).write_text(str(value))
 
     def get_outs_content(self):
@@ -271,7 +275,39 @@
         self.result = sum(x.get_random_number() for x in self.numbers)
 
 
 class SumRandomNumbersNamed(SumRandomNumbers):
     """Same as SumRandomNumbers but with a custom name."""
 
     _name_ = "custom_SumRandomNumbers"
+
+
+class NodeWithRestart(zntrack.Node):
+    """Node that restarts."""
+
+    start: int = zntrack.params()
+    raise_exception_until: int = zntrack.params(0)
+
+    count: int = zntrack.outs()
+
+    def run(self) -> None:
+        """Run the node.
+
+        Increments the count by one, for each run.
+        Check that the restart flag is set.
+        """
+        self.count = self.start + self.state.run_count
+        if self.state.run_count > 1:
+            assert self.state.restarted
+        if self.state.run_count < self.raise_exception_until:
+            raise ValueError("This is a test exception, simulating killing the Node.")
+
+
+class OptionalDeps(zntrack.Node):
+    """Node with optional dependencies."""
+
+    value: float = zntrack.deps(None)
+    result: float = zntrack.outs()
+
+    def run(self) -> None:
+        """Run the node."""
+        self.result = self.value or 0.0
```

### Comparing `zntrack-0.7.2/zntrack/exceptions/__init__.py` & `zntrack-0.7.3/zntrack/exceptions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """All ZnTrack exceptions."""
 
+
 class NodeNotAvailableError(Exception):
     """Raised when a node is not available."""
 
     def __init__(self, arg):
         """Initialize the exception.
 
         Parameters
```

### Comparing `zntrack-0.7.2/zntrack/fields/dependency.py` & `zntrack-0.7.3/zntrack/fields/dependency.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/fields/dvc/__init__.py` & `zntrack-0.7.3/zntrack/fields/dvc/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/fields/dvc/options.py` & `zntrack-0.7.3/zntrack/fields/dvc/options.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/fields/field.py` & `zntrack-0.7.3/zntrack/fields/field.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/fields/fields.py` & `zntrack-0.7.3/zntrack/fields/fields.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/fields/meta/__init__.py` & `zntrack-0.7.3/zntrack/fields/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/fields/zn/__init__.py` & `zntrack-0.7.3/zntrack/fields/zn/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/fields/zn/options.py` & `zntrack-0.7.3/zntrack/fields/zn/options.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/notebooks/jupyter.py` & `zntrack-0.7.3/zntrack/notebooks/jupyter.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/project/zntrack_project.py` & `zntrack-0.7.3/zntrack/project/zntrack_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,33 +67,39 @@
     graph : znflow.DiGraph
         the znflow graph of the project.
     initialize : bool, default = True
         If True, initialize a git repository and a dvc repository.
     remove_existing_graph : bool, default = False
         If True, remove 'dvc.yaml', 'zntrack.json' and 'params.yaml'
             before writing new nodes.
-    automatic_node_names : bool, default = False
+    automatic_node_names : bool, default = True
         If True, automatically add a number to the node name if the name is already
             used in the graph.
     git_only_repo : bool, default = True
         The DVC graph relies on file outputs for connecting stages.
         ZnTrack will use a '--metrics-no-cache' file output for each stage by default.
         Contrary to '--outs-no-cache', this will keep the DVC run cache available.
         If a project has a DVC remote available, '--outs' can be used instead.
         This will require a DVC remote to be setup.
     force : bool, default = False
         overwrite existing nodes.
+    magic_names : bool, default = False
+        If True, use magic names for the nodes. This will use the variable name of the
+        node as the node name. E.g. `node = Node()` will result in a node name of 'node'.
+        If used within a group, the group name will be added to the node name. E.g.
+        `group.name = Grp1` and `model = Node()` will result in a name of 'Grp1_model'.
     """
 
     graph: ZnTrackGraph = dataclasses.field(default_factory=ZnTrackGraph, init=False)
     initialize: bool = True
     remove_existing_graph: bool = False
-    automatic_node_names: bool = False
+    automatic_node_names: bool = True
     git_only_repo: bool = True
     force: bool = False
+    magic_names: bool = False
 
     _groups: dict[str, NodeGroup] = dataclasses.field(
         default_factory=dict, init=False, repr=False
     )
 
     def __post_init__(self):
         """Initialize the Project.
@@ -112,14 +118,19 @@
         if self.remove_existing_graph:
             # we remove the files that typically contain the graph definition
             config.files.zntrack.unlink(missing_ok=True)
             config.files.dvc.unlink(missing_ok=True)
             config.files.params.unlink(missing_ok=True)
             shutil.rmtree("nodes", ignore_errors=True)
 
+        if self.automatic_node_names and self.magic_names:
+            raise ValueError(
+                "automatic_node_names and magic_names can not be True at the same time"
+            )
+
     def __enter__(self, *args, **kwargs):
         """Enter the graph context."""
         self.graph.__enter__(*args, **kwargs)
         return self
 
     def __exit__(self, *args, **kwargs):
         """Exit the graph context."""
@@ -272,15 +283,18 @@
             node.nwd  # create the node working directory (property-access will create it)
             if node._external_:
                 continue
             if eager:
                 # update connectors
                 log.info(f"Running node {node}")
                 self.graph._update_node_attributes(node, UpdateConnectors())
-                node.run()
+                if hasattr(node, "_method"):
+                    getattr(node, node._method)()
+                else:
+                    node.run()
                 if save:
                     node.save()
                 node.state.loaded = True
             else:
                 log.info(f"Adding node {node}")
                 cmd = get_dvc_cmd(
                     node, git_only_repo=self.git_only_repo, **optional.get(node.name, {})
@@ -476,14 +490,36 @@
 class NodeGroup:
     """A group of nodes."""
 
     name: tuple[str]
     nwd: pathlib.Path
     nodes: list[Node]
 
-    def __contains__(self, item: Node) -> bool:
+    def _get_name_with_prefix(self, name: str) -> str:
+        """Get the name with the group prefix."""
+        if name.startswith(self.name):
+            return name
+        return f"{self.name}_{name}"
+
+    def __contains__(self, item: typing.Union[Node, str]) -> bool:
         """Check if the Node is in the group."""
-        return item in self.nodes
+        if isinstance(item, Node):
+            item = item.name
+        else:
+            item = self._get_name_with_prefix(item)
+        return item in [node.name for node in self.nodes]
+
+    def __iter__(self) -> typing.Iterator[Node]:
+        """Iterate over the nodes in the group."""
+        return iter(self.nodes)
+
+    def __getitem__(self, name: int) -> Node:
+        """Get the Node from the group."""
+        name = self._get_name_with_prefix(name)
+        for node in self.nodes:
+            if node.name == name:
+                return node
+        raise KeyError(f"Node {name} not in group {self.name}")
 
     def __len__(self) -> int:
         """Get the number of nodes in the group."""
         return len(self.nodes)
```

### Comparing `zntrack-0.7.2/zntrack/tools/__init__.py` & `zntrack-0.7.3/zntrack/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/utils/__init__.py` & `zntrack-0.7.3/zntrack/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,36 +223,44 @@
 
 @dataclasses.dataclass
 class NodeName:
     """The name of a node."""
 
     groups: list[str]
     name: str
+    varname: str = None
     suffix: int = 0
+    use_varname: bool = False
 
     def __str__(self) -> str:
         """Get the node name."""
         name = []
         if self.groups is not None:
             name.extend(self.groups)
-        name.append(self.name)
+        if self.use_varname:
+            name.append(self.varname)
+        else:
+            name.append(self.name)
+        if self.suffix > 0 and self.use_varname:
+            raise ValueError("Suffixes are not supported for magic names (varnames).")
         if self.suffix > 0:
             name.append(str(self.suffix))
         return "_".join(name)
 
     def get_name_without_groups(self) -> str:
         """Get the node name without the groups."""
-        name = self.name
+        name = self.varname if self.use_varname else self.name
         if self.suffix > 0:
             name += f"_{self.suffix}"
         return name
 
     def update_suffix(self, project: "Project", node: "Node") -> None:
         """Update the suffix."""
         node_names = [x["value"].name for x in project.graph.nodes.values()]
+        self.use_varname = project.magic_names
 
         node_names = []
         for node_uuid in project.graph.nodes:
             if node_uuid == node.uuid:
                 continue
             node_names.append(project.graph.nodes[node_uuid]["value"].name)
```

### Comparing `zntrack-0.7.2/zntrack/utils/cli.py` & `zntrack-0.7.3/zntrack/utils/cli.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/utils/config.py` & `zntrack-0.7.3/zntrack/utils/config.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/utils/file_io.py` & `zntrack-0.7.3/zntrack/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/zntrack/utils/node_wd.py` & `zntrack-0.7.3/zntrack/utils/node_wd.py`

 * *Files identical despite different names*

### Comparing `zntrack-0.7.2/PKG-INFO` & `zntrack-0.7.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: ZnTrack
-Version: 0.7.2
+Version: 0.7.3
 Summary: Create, Run and Benchmark DVC Pipelines in Python
 License: Apache-2.0
 Keywords: data-science,data-version-control,machine-learning,reproducibility,collaboration
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
-Requires-Python: >=3.8,<4.0.0
+Requires-Python: >=3.9,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dot4dict (>=0.1.1,<0.2.0)
-Requires-Dist: dvc (>=3.2.2,<4.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dot4dict (>=0.1,<0.2)
+Requires-Dist: dvc (>=3.3,<4.0)
 Requires-Dist: pandas (>=2,<3)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: tqdm (>=4.64.0,<5.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
-Requires-Dist: znflow (>=0.1.14,<0.2.0)
-Requires-Dist: zninit (>=0.1.11,<0.2.0)
-Requires-Dist: znjson (>=0.2.2,<0.3.0)
+Requires-Dist: pyyaml (>=6,<7)
+Requires-Dist: pyzmq (>=25,<26)
+Requires-Dist: tqdm (>=4,<5)
+Requires-Dist: typer (>=0.7,<0.8)
+Requires-Dist: varname (>=0.13,<0.14)
+Requires-Dist: znflow (>=0.1,<0.2)
+Requires-Dist: zninit (>=0.1,<0.2)
+Requires-Dist: znjson (>=0.2,<0.3)
 Project-URL: documentation, https://zntrack.readthedocs.io
 Project-URL: repository, https://github.com/zincware/ZnTrack
 Description-Content-Type: text/markdown
 
 [![coeralls](https://coveralls.io/repos/github/zincware/ZnTrack/badge.svg)](https://coveralls.io/github/zincware/ZnTrack)
 [![codecov](https://codecov.io/gh/zincware/ZnTrack/branch/main/graph/badge.svg?token=ZQ67FXN1IT)](https://codecov.io/gh/zincware/ZnTrack)
 [![Maintainability](https://api.codeclimate.com/v1/badges/f25e119bbd5d5ec74e2c/maintainability)](https://codeclimate.com/github/zincware/ZnTrack/maintainability)
 ![PyTest](https://github.com/zincware/ZnTrack/actions/workflows/test.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/zntrack.svg)](https://badge.fury.io/py/zntrack)
 [![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Documentation](https://readthedocs.org/projects/zntrack/badge/?version=latest)](https://zntrack.readthedocs.io/en/latest/?badge=latest)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnTrack/HEAD)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6472850.svg)](https://doi.org/10.5281/zenodo.6472850)
+[![DOI](https://img.shields.io/badge/arXiv-2401.10603-red)](https://arxiv.org/abs/2401.10603)
 [![ZnTrack](https://img.shields.io/badge/Powered%20by-ZnTrack-%23007CB0)](https://zntrack.readthedocs.io/en/latest/)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 ![Logo](https://raw.githubusercontent.com/zincware/ZnTrack/main/docs/source/_static/logo_ZnTrack.png)
 
 # ZnTrack: A Parameter Tracking Package for Python
 
@@ -160,14 +161,28 @@
 On a fundamental level the ZnTrack package provides an easy-to-use interface for
 DVC directly from Python. It handles all the computational overhead of reading
 config files, defining outputs in the `dvc.yaml` as well as in the script and
 much more.
 
 For more information on DVC visit their [homepage](https://dvc.org/doc).
 
+# References
+
+If you use ZnTrack in your research and find it helpful please cite us.
+
+```bibtex
+@misc{zillsZnTrackDataCode2024,
+  title = {{{ZnTrack}} -- {{Data}} as {{Code}}},
+  author = {Zills, Fabian and Sch{\"a}fer, Moritz and Tovey, Samuel and K{\"a}stner, Johannes and Holm, Christian},
+  year = {2024},
+  eprint={2401.10603},
+  archivePrefix={arXiv},
+}
+```
+
 # Copyright
 
 This project is distributed under the
 [Apache License Version 2.0](https://github.com/zincware/ZnTrack/blob/main/LICENSE).
 
 ## Similar Tools
```

