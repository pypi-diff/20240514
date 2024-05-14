# Comparing `tmp/smartdashboard-0.0.3.tar.gz` & `tmp/smartdashboard-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdashboard-0.0.3.tar", last modified: Thu Feb 15 18:45:28 2024, max compression
+gzip compressed data, was "smartdashboard-0.0.4.tar", last modified: Tue May 14 21:13:23 2024, max compression
```

## Comparing `smartdashboard-0.0.3.tar` & `smartdashboard-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:45:28.570256 smartdashboard-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-02-15 18:45:28.570256 smartdashboard-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 18:45:28.570256 smartdashboard-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:45:28.566256 smartdashboard-0.0.3/smartdashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/Experiment_Overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:45:28.566256 smartdashboard-0.0.3/smartdashboard/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/pages/3_Help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:45:28.566256 smartdashboard-0.0.3/smartdashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/static/SmartSim.png
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:45:28.570256 smartdashboard-0.0.3/smartdashboard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/LogReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/ManifestReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/StatusReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/pageSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    14781 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/view_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-02-15 18:45:08.000000 smartdashboard-0.0.3/smartdashboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 18:45:28.570256 smartdashboard-0.0.3/smartdashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-02-15 18:45:28.000000 smartdashboard-0.0.3/smartdashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-15 18:45:28.000000 smartdashboard-0.0.3/smartdashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 18:45:28.000000 smartdashboard-0.0.3/smartdashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-15 18:45:28.000000 smartdashboard-0.0.3/smartdashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-15 18:45:28.000000 smartdashboard-0.0.3/smartdashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-15 18:45:28.000000 smartdashboard-0.0.3/smartdashboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:13:23.010031 smartdashboard-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-14 21:13:23.010031 smartdashboard-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:13:23.010031 smartdashboard-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:13:23.002031 smartdashboard-0.0.4/smartdashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/Experiment_Overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:13:23.006031 smartdashboard-0.0.4/smartdashboard/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/pages/2_Database_Telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/pages/3_Help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/pages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:13:23.006031 smartdashboard-0.0.4/smartdashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/static/SmartSim.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:13:23.006031 smartdashboard-0.0.4/smartdashboard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/LogReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/ManifestReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/StatusReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/pageSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/view_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25037 2024-05-14 21:13:07.000000 smartdashboard-0.0.4/smartdashboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:13:23.006031 smartdashboard-0.0.4/smartdashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-14 21:13:22.000000 smartdashboard-0.0.4/smartdashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-14 21:13:22.000000 smartdashboard-0.0.4/smartdashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:13:22.000000 smartdashboard-0.0.4/smartdashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 21:13:22.000000 smartdashboard-0.0.4/smartdashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-14 21:13:22.000000 smartdashboard-0.0.4/smartdashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 21:13:22.000000 smartdashboard-0.0.4/smartdashboard.egg-info/top_level.txt
```

### Comparing `smartdashboard-0.0.3/LICENSE.md` & `smartdashboard-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/MANIFEST.in` & `smartdashboard-0.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/PKG-INFO` & `smartdashboard-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: smartdashboard
-Version: 0.0.3
+Version: 0.0.4
 Summary: Visualize SmartSim Experiments
 Author-email: "CrayLabs: a Hewlett Packard Enterprise OSS Organization" <craylabs@hpe.com>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://www.craylabs.org
 Project-URL: Documentation, https://github.com/CrayLabs/SmartDashboard
 Project-URL: Repository, https://github.com/CrayLabs/SmartDashboard
 Keywords: scientific,ai,workflow,hpc,analysis
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: altair>=5.2.0
 Requires-Dist: pandas>=2.0.0
-Requires-Dist: pydantic>=2.5.2
-Requires-Dist: streamlit>=1.28.0
+Requires-Dist: pydantic<2,>=1.10.14
+Requires-Dist: streamlit!=1.31.0,!=1.31.1,>=1.28.0
 Requires-Dist: watchdog>=3.0.0
 Provides-Extra: dev
 Requires-Dist: black>=20.8b1; extra == "dev"
 Requires-Dist: isort>=5.6.4; extra == "dev"
 Requires-Dist: pylint>=2.10.0; extra == "dev"
 Requires-Dist: pytest>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
@@ -37,24 +38,45 @@
 Requires-Dist: sphinx-book-theme==0.2.0; extra == "doc"
 Requires-Dist: nbsphinx>=0.8.2; extra == "doc"
 Requires-Dist: breathe==4.31.0; extra == "doc"
 Requires-Dist: jinja2==3.0.3; extra == "doc"
 
 # SmartDashboard
 
-SmartDashboard is an add-on to SmartSim that provides a dashboard to help users understand and monitor their SmartSim experiments in a visual way. Configuration, status, and logs are available for all launched entities within an experiment for easy inspection.
+SmartDashboard is an add-on to SmartSim that provides a dashboard to help users understand and monitor their SmartSim experiments in a visual way. Configuration, status, and logs are available for all launched entities within an experiment for easy inspection, along with memory and client data per shard for launched orchestrators.
 
-A ``Telemetry Monitor`` is a background process that is launched along with the experiment
-that produces the data displayed by SmartDashboard. The ``Telemetry Monitor`` can be disabled by
-adding ``export SMARTSIM_TELEMETRY_ENABLE=0`` as an environment variable. When disabled, SmartDashboard
-will not display any data. To re-enable, set the ``SMARTSIM_TELEMETRY_ENABLE`` environment variable to ``1``
-with ``export SMARTSIM_TELEMETRY_ENABLE=1``.
+A ``Telemetry Monitor`` is a background process that is launched alongside the experiment.
+It is responsible for generating the data displayed by SmartDashboard. The ``Telemetry Monitor`` can be disabled globally by
+adding ``export SMARTSIM_FLAG_TELEMETRY=0`` as an environment variable. When disabled, SmartDashboard
+will not display entity status data. To re-enable, set the ``SMARTSIM_FLAG_TELEMETRY`` environment variable to ``1``
+with ``export SMARTSIM_FLAG_TELEMETRY=1``. For workflows involving multiple experiments, SmartSim provides the attributes
+``Experiment.telemetry.enable`` and ``Experiment.telemetry.disable`` to manage the enabling or disabling of telemetry on a per-experiment basis.
+
+`Orchestrator` memory and client data can be collected by enabling database telemetry. To do so, add ``Orchestrator.telemetry.enable``
+after creating an `Orchestrator` within the driver script. Database telemetry is enabled per `Orchestrator`, so if there are multiple
+`Orchestrators` launched, they will each need to be enabled separately in the driver script.
 
-Experiment metadata is also stored in the ``.smartsim`` directory, a hidden folder for internal api use and used by the dashboard.
-Deletion of the experiment folder will remove all experiment metadata.
+```python
+# enabling telemetry example
+
+from smartsim import Experiment
+
+exp = Experiment("experiment", launcher="auto")
+exp.telemetry.enable()
+
+db = exp.create_database(db_nodes=3)
+db.telemetry.enable()
+
+exp.start(db, block=True)
+exp.stop(db)
+```
+
+Experiment metadata is stored in the ``.smartsim`` directory, a hidden folder used by the internal api and accessed by the dashboard.
+This folder can be found within the created experiment directory.
+Deletion of the experiment folder will remove all associated metadata.
 
 ## Installation
 
 It's important to note that SmartDashboard only works while using SmartSim, so SmartSim will need to be installed as well.
 SmartSim installation docs can be found [here](https://www.craylabs.org/docs/installation_instructions/basic.html).
 
 ### User Install
@@ -86,14 +108,15 @@
 ```
 
 ```python
 # hello_world.py
 from smartsim import Experiment
 
 exp = Experiment("hello_world_exp", launcher="auto")
+exp.telemetry.enable()
 run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
 run.set_tasks(60)
 run.set_tasks_per_node(20)
 
 model = exp.create_model("hello_world", run)
 exp.start(model, block=True, summary=True)
 ```
@@ -136,8 +159,13 @@
 
 ## Using SmartDashboard
 
 Once the dashboard is launched, a browser will open to `http://localhost:<port>`. SmartDashboard currently has two tabs on the left hand side.
   
 `Experiment Overview:` This tab is where configuration information, statuses, and logs are located for each launched entity of the experiment. The `Experiment` section displays configuration information for the overall experiment and its logs. In the `Applications` section, also known as SmartSim `Models`, select a launched application to see its status, what it was configured with, and its logs. The `Orchestrators` section also provides configuration and status information, as well as logs per shard for a selected orchestrator. Finally, in the `Ensembles` section, select an ensemble to see its status and configuration. Then select any of its members to see its status, configuration, and logs.
   
+`Database Telemetry:` This tab provides additional details about `Orchestrators`.
+The `Orchestrator Summary` section shows configuration and status information of the selected. The `Memory`
+section provides memory usage data per shard within the `Orchestrator`. The `Clients`
+section displays client data per shard within the `Orchestrator`.  
+
 `Help:` This tab links to SmartSim documentation and provides a SmartSim contact for support.
```

### Comparing `smartdashboard-0.0.3/pyproject.toml` & `smartdashboard-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,35 +28,36 @@
 [build-system]
 requires = ["setuptools", "wheel", "cmake>=3.13"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "smartdashboard"
-version = "0.0.3"
-requires-python = ">=3.8,<3.11"
+version = "0.0.4"
+requires-python = ">=3.9,<3.12"
 authors = [
   {name = "CrayLabs: a Hewlett Packard Enterprise OSS Organization", email = "craylabs@hpe.com"},
 ]
 description = "Visualize SmartSim Experiments"
 license = { text = "BSD 2-Clause License" }
 keywords = ["scientific", "ai", "workflow", "hpc", "analysis"]
 classifiers = [
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
 ]
 readme = "README.md"
 dependencies = [
+    "altair>=5.2.0",
     "pandas>=2.0.0",
-    "pydantic>=2.5.2",
-    "streamlit>=1.28.0",
+    "pydantic>=1.10.14, <2", # this is pinned to keep consistency with SmartSim
+    "streamlit>=1.28.0, !=1.31.0, !=1.31.1",
     "watchdog>=3.0.0",
 ]
 
 [project.urls]
 Homepage = "https://www.craylabs.org"
 Documentation = "https://github.com/CrayLabs/SmartDashboard"
 Repository = "https://github.com/CrayLabs/SmartDashboard"
@@ -100,15 +101,15 @@
 
 [tool.setuptools.exclude-package-data]
 tests = ["tests"]
 
 
 [tool.black]
 line-length = 88
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py39', 'py310', 'py311']
 exclude = '''
 (
   | \.egg
   | \.git
   | \.hg
   | \.mypy_cache
   | \.nox
@@ -165,14 +166,7 @@
 disallow_untyped_decorators = true
 
 # Safety/Upgrading Mypy
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_unused_configs = true
 show_error_codes = true
-
-
-[[tool.mypy.overrides]]
-# Ignore packages that are not used or not typed
-module = []
-ignore_missing_imports = true
-ignore_errors = true
```

### Comparing `smartdashboard-0.0.3/smartdashboard/__init__.py` & `smartdashboard-0.0.4/smartdashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/__main__.py` & `smartdashboard-0.0.4/smartdashboard/__main__.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/pages/3_Help.py` & `smartdashboard-0.0.4/smartdashboard/pages/3_Help.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,13 +59,23 @@
         - [Experiments](https://www.craylabs.org/docs/experiment.html#)
         - [Models](https://www.craylabs.org/docs/experiment.html#model)
         - [Orchestrators](https://www.craylabs.org/docs/orchestrator.html)
         - [Ensembles](https://www.craylabs.org/docs/experiment.html#ensemble)""")
 
 st.write("")
 
+with st.expander(label="Database Telemetry"):
+    st.markdown("""Gain deeper insights into your orchestrators in this section.
+        Select the orchestrator you want to analyze from the
+        orchestrator dropdown and find information about its memory usage and
+        clients per shard.""")
+    st.markdown("""
+        - [Orchestrators](https://www.craylabs.org/docs/orchestrator.html)""")
+
+st.write("")
+
 with st.expander(label="Support"):
     st.markdown("""Should you encounter any issues or require assistance while
         using the SmartSim Dashboard, we're here to help!""")
     st.markdown("""The complete SmartSim documentation can be found
         [here](https://www.craylabs.org/docs/overview.html).
         You can also contact us at craylabs@hpe.com.""")
```

### Comparing `smartdashboard-0.0.3/smartdashboard/pages/__init__.py` & `smartdashboard-0.0.4/smartdashboard/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/static/SmartSim.png` & `smartdashboard-0.0.4/smartdashboard/static/SmartSim.png`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/static/style.css` & `smartdashboard-0.0.4/smartdashboard/static/style.css`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/LogReader.py` & `smartdashboard-0.0.4/smartdashboard/utils/LogReader.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/ManifestReader.py` & `smartdashboard-0.0.4/smartdashboard/utils/ManifestReader.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,26 +23,28 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import io
 import itertools
 import json
+import os
+import pathlib
 import typing as t
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Dict, List
 
 from pydantic import ValidationError
 
 from smartdashboard.schemas.application import Application
 from smartdashboard.schemas.ensemble import Ensemble
 from smartdashboard.schemas.experiment import Experiment
 from smartdashboard.schemas.orchestrator import Orchestrator
-from smartdashboard.schemas.run import Run
+from smartdashboard.schemas.run import Run, RunContext
 from smartdashboard.utils.errors import (
     MalformedManifestError,
     ManifestError,
     VersionIncompatibilityError,
 )
 
 
@@ -56,86 +58,103 @@
     :type runs: List[Run]
     """
 
     experiment: Experiment
     runs: List[Run]
 
     @property
-    def apps_with_run_ctx(self) -> t.Iterable[t.Tuple[str, Application]]:
+    def apps_with_run_ctx(self) -> t.Iterable[RunContext[Application]]:
         return itertools.chain.from_iterable(run.apps_with_ctx for run in self.runs)
 
     @property
-    def orcs_with_run_ctx(self) -> t.Iterable[t.Tuple[str, Orchestrator]]:
+    def orcs_with_run_ctx(self) -> t.Iterable[RunContext[Orchestrator]]:
         return itertools.chain.from_iterable(run.orcs_with_ctx for run in self.runs)
 
     @property
-    def ensemble_with_run_ctx(self) -> t.Iterable[t.Tuple[str, Ensemble]]:
+    def ensemble_with_run_ctx(self) -> t.Iterable[RunContext[Ensemble]]:
         return itertools.chain.from_iterable(run.ensemble_with_ctx for run in self.runs)
 
 
 class ManifestReader(ABC):
     """Base class for a ManifestReader"""
 
     @abstractmethod
     def get_manifest(self) -> Manifest:
         """Abstract method to get the manifest from a ManifestReader subclass"""
 
 
 class ManifestFileReader(ManifestReader):
     """ManifestReader class for file-based manifests"""
 
-    def __init__(self, file_path: str) -> None:
+    def __init__(self, file_path: pathlib.Path) -> None:
         """Initialize a ManifestFileReader
 
         :param file_path: Path to the manifest file
-        :type file_path: str
+        :type file_path: pathlib.Path
         """
         self._file_path = file_path
+        self._last_modified = os.path.getmtime(self._file_path)
         self._data = self.from_file(self._file_path)
 
         try:
             version = self._data["schema info"]["version"]
         except KeyError as key:
             raise MalformedManifestError(
-                "Version data is malformed.", file=self._file_path, exception=key
+                "Version data is malformed.", file=str(self._file_path), exception=key
             ) from key
 
-        if version not in ("0.0.2", "0.0.3"):
+        if version not in ("0.0.2", "0.0.3", "0.0.4"):
             version_exception = Exception(
-                "SmartDashboard version 0.0.3 is unable to parse manifest "
+                "SmartDashboard version 0.0.4 is unable to parse manifest "
                 f"file at version {version}."
             )
             raise VersionIncompatibilityError(
                 title="Invalid Version Number",
-                file=file_path,
+                file=str(file_path),
                 exception=version_exception,
             )
 
+    @property
+    def has_changed(self) -> bool:
+        """Check if the manifest file has been modified
+
+        :return: If the file has been modified
+        :rtype: bool
+        """
+        return self._last_modified != os.path.getmtime(self._file_path)
+
     def get_manifest(self) -> Manifest:
         """Get the Manifest from self._data
 
         :return: Manifest
         :rtype: Manifest
         """
-        experiment = Experiment(**self._data.get("experiment", {}))
-        runs_data = self._data.get("runs", [])
+        try:
+            experiment = Experiment(**self._data.get("experiment", {}))
+            runs_data = self._data.get("runs", [])
 
-        runs = [Run(**run_data) for run_data in runs_data]
+            runs = [Run(**run_data) for run_data in runs_data]
 
-        return Manifest(
-            experiment=experiment,
-            runs=runs,
-        )
+            return Manifest(
+                experiment=experiment,
+                runs=runs,
+            )
+        except ValidationError as val:
+            raise MalformedManifestError(
+                title="Manifest file is malformed.",
+                file=str(self._file_path),
+                exception=val,
+            ) from val
 
     @classmethod
-    def from_file(cls, file_path: str) -> Dict[str, Any]:
+    def from_file(cls, file_path: pathlib.Path) -> Dict[str, Any]:
         """Initialize self._data
 
         :param file_path: File path of the manifest
-        :type file_path: str
+        :type file_path: pathlib.Path
         :return: self._data
         :rtype: Dict[str, Any]
         """
         with open(file_path, encoding="utf-8") as file:
             return cls.from_io_stream(file)
 
     @classmethod
@@ -147,35 +166,47 @@
         :return: self._data
         :rtype: Dict[str, Any]
         """
         data: Dict[str, Any] = json.loads(stream.read())
         return data
 
 
-def load_manifest(path: str) -> Manifest:
-    """Instantiate and call get_manifest
+def create_filereader(path: pathlib.Path) -> ManifestFileReader:
+    """Instantiate ManifestFileReader
 
     This is where we're checking for any errors
     that could occur when creating a manifest
     from file.
 
     :param path: Path to the manifest file
     :type path: str
-    :return: Manifest
-    :rtype: Optional[Manifest]
+    :return: ManifestFileReader
+    :rtype: ManifestFileReader
     """
     try:
         manifest_file_reader = ManifestFileReader(path)
-        manifest = manifest_file_reader.get_manifest()
     except FileNotFoundError as fnf:
         raise ManifestError(
-            title="Manifest file does not exist.", file=path, exception=fnf
+            title="Manifest file does not exist.", file=str(path), exception=fnf
         ) from fnf
     except json.decoder.JSONDecodeError as jde:
         raise ManifestError(
-            title="Manifest file could not be decoded.", file=path, exception=jde
+            title="Manifest file could not be decoded.", file=str(path), exception=jde
         ) from jde
-    except ValidationError as val:
-        raise MalformedManifestError(
-            title="Manifest file is malformed.", file=path, exception=val
-        ) from val
-    return manifest
+    return manifest_file_reader
+
+
+def get_manifest_path(directory: t.Optional[pathlib.Path]) -> pathlib.Path:
+    """Get the manifest path using the directory
+    path passed in from the command line arguments.
+
+    :param directory: An experiment directory
+    :type directory: t.Optional[pathlib.Path]
+    :return: Manifest path
+    :rtype: pathlib.Path
+    """
+
+    if directory is not None:
+        manifest_path = directory / ".smartsim/telemetry/manifest.json"
+    else:
+        manifest_path = pathlib.Path() / ".smartsim/telemetry/manifest.json"
+    return manifest_path.resolve()
```

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/StatusReader.py` & `smartdashboard-0.0.4/smartdashboard/utils/StatusReader.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/__init__.py` & `smartdashboard-0.0.4/smartdashboard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/errors.py` & `smartdashboard-0.0.4/smartdashboard/utils/errors.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/helpers.py` & `smartdashboard-0.0.4/smartdashboard/utils/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,29 @@
             "Warning! Shards within an Orchestrator should have the same port. "
             + ", ".join(map(str, sorted(orc.ports)))
         )
 
     return ""
 
 
+def format_interfaces(orc: t.Optional[Orchestrator]) -> str:
+    """Format the interfaces of an orchestrator
+
+    :param orc: Orchestrator
+    :type orc: Optional[Orchestrator]
+    :return: Formatted interfaces
+    :rtype: str
+    """
+
+    if orc:
+        return ", ".join(orc.interface)
+
+    return ""
+
+
 def flatten_nested_keyvalue_containers(
     dict_name: str,
     entity: t.Optional[t.Dict[str, t.Any]],
 ) -> t.List[t.Tuple[str, str]]:
     """Format dicts of all types to be displayed
 
     The dictionaries can have a combination of types attached, so
```

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/pageSetup.py` & `smartdashboard-0.0.4/smartdashboard/utils/pageSetup.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/utils/status.py` & `smartdashboard-0.0.4/smartdashboard/utils/status.py`

 * *Files identical despite different names*

### Comparing `smartdashboard-0.0.3/smartdashboard/view_builders.py` & `smartdashboard-0.0.4/smartdashboard/view_builders.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,30 +26,37 @@
 
 import traceback
 import typing as t
 
 import pandas as pd
 import streamlit as st
 
+from smartdashboard.schemas.orchestrator import Orchestrator
+from smartdashboard.schemas.shard import Shard
 from smartdashboard.utils.errors import SSDashboardError
 from smartdashboard.utils.helpers import (
     build_dataframe_generic,
     build_dataframe_loaded_entities,
     flatten_nested_keyvalue_containers,
     format_ensemble_params,
+    format_interfaces,
     get_port,
     render_dataframe,
     shard_log_spacing,
 )
 from smartdashboard.utils.ManifestReader import Manifest
 from smartdashboard.views import (
     ApplicationView,
+    ClientView,
+    DatabaseTelemetryView,
     EnsembleView,
     ErrorView,
     ExperimentView,
+    MemoryView,
+    OrchestratorSummaryView,
     OrchestratorView,
     OverviewView,
 )
 
 
 def error_builder(error: SSDashboardError) -> ErrorView:
     """Error view displayed when errors are caught
@@ -57,18 +64,20 @@
     :param error: Error to get information from
     :type error: SSDashboardError
     :return: An error view
     :rtype: ErrorView
     """
     view = ErrorView()
     st.header(str(error))
+    # fmt: off
     st.error(
         f"""Error found in file: {error.file}  
              Error Message: {error.exception}"""
     )
+    # fmt: on
 
     with st.expander(label="Traceback"):
         st.code(traceback.format_exc(), language="log")
 
     return view
 
 
@@ -107,78 +116,71 @@
     :type manifest: Manifest
     :return: An application view
     :rtype: ApplicationView
     """
     st.subheader("Application Configuration")
     col1, col2 = st.columns([4, 4])
     with col1:
-        selected_application_tuple = st.selectbox(
+        selected_application_context = st.selectbox(
             "Select an application:",
             manifest.apps_with_run_ctx,
-            format_func=lambda tup: f"{tup[1].name}: Run {tup[0]}",
+            format_func=lambda context: f"{context.entity.name}: Run {context.run_id}",
         )
 
-    if selected_application_tuple is not None:
-        _, selected_application = selected_application_tuple
+    if selected_application_context is not None:
+        selected_application = selected_application_context.entity
     else:
         selected_application = None
 
     view = ApplicationView(selected_application)
 
     st.write("")
     view.status_element = st.empty()
     st.write("Path: " + (view.application.path if view.application is not None else ""))
 
     st.write("")
     with st.expander(label="Executable Arguments"):
-        render_dataframe(
-            pd.DataFrame(
-                {
-                    "All Arguments": (
-                        selected_application.exe_args
-                        if selected_application is not None
-                        else []
-                    ),
-                }
-            )
+        arguments = (
+            selected_application.exe_args if selected_application is not None else []
         )
+        render_dataframe(pd.DataFrame(arguments, columns=["All Arguments"]))
 
     st.write("")
     with st.expander(label="Batch and Run Settings"):
         col1, col2 = st.columns([4, 4])
         build_dataframe_generic(
             column=col1,
             title="Batch Settings",
             dict_name="batch_settings",
-            entity=selected_application.model_dump() if selected_application else {},
+            entity=selected_application.dict() if selected_application else {},
             df_columns=["Name", "Value"],
         )
         build_dataframe_generic(
             column=col2,
             title="Run Settings",
             dict_name="run_settings",
-            entity=selected_application.model_dump() if selected_application else {},
+            entity=selected_application.dict() if selected_application else {},
             df_columns=["Name", "Value"],
         )
 
     st.write("")
     with st.expander(label="Parameters and Generator Files"):
         col1, col2 = st.columns([4, 4])
         build_dataframe_generic(
             column=col1,
             title="Parameters",
             dict_name="params",
-            entity=selected_application.model_dump() if selected_application else {},
+            entity=selected_application.dict() if selected_application else {},
             df_columns=["Name", "Value"],
         )
         build_dataframe_generic(
             column=col2,
             title="Files",
             dict_name="files",
-            entity=selected_application.model_dump() if selected_application else {},
+            entity=selected_application.dict() if selected_application else {},
             df_columns=["Type", "File"],
         )
 
     st.write("")
     with st.expander(label="Colocated Database"):
         with st.container():
             col1, col2 = st.columns([6, 6])
@@ -222,52 +224,42 @@
     :type manifest: Manifest
     :return: An orchestrator view
     :rtype: OrchestratorView
     """
     st.subheader("Orchestrator Configuration")
     col1, col2 = st.columns([4, 4])
     with col1:
-        selected_orchestrator_tuple = st.selectbox(
+        selected_orchestrator_context = st.selectbox(
             "Select an orchestrator:",
             manifest.orcs_with_run_ctx,
-            format_func=lambda tup: f"{tup[1].name}: Run {tup[0]}",
+            format_func=lambda context: f"{context.entity.name}: Run {context.run_id}",
         )
 
-    if selected_orchestrator_tuple is not None:
-        _, selected_orchestrator = selected_orchestrator_tuple
+    if selected_orchestrator_context is not None:
+        selected_orchestrator = selected_orchestrator_context.entity
     else:
         selected_orchestrator = None
 
     shards = selected_orchestrator.shards if selected_orchestrator else []
     view = OrchestratorView(selected_orchestrator, shards[0] if shards else None)
 
     st.write("")
     view.status_element = st.empty()
     st.write(
         "Type: "
         + (selected_orchestrator.type if selected_orchestrator is not None else "")
     )
     st.write("Port: " + get_port(selected_orchestrator))
-    st.write(
-        "Interface: " + ", ".join(selected_orchestrator.interface)
-        if selected_orchestrator
-        else ""
-    )
+    st.write("Interface: " + format_interfaces(selected_orchestrator))
 
     st.write("")
     with st.expander(label="Database Hosts"):
-        render_dataframe(
-            pd.DataFrame(
-                {
-                    "Hosts": (
-                        selected_orchestrator.db_hosts if selected_orchestrator else []
-                    ),
-                }
-            )
-        )
+        hosts = selected_orchestrator.db_hosts if selected_orchestrator else []
+        render_dataframe(pd.DataFrame(hosts, columns=["Hosts"]))
+
     st.write("")
     with st.expander(label="Logs"):
         col1, col2 = st.columns([6, 6])
         with col1:
             shard = st.selectbox(
                 "Select a shard:", shards, format_func=lambda shard: shard.name
             )
@@ -293,52 +285,44 @@
     :type manifest: Manifest
     :return: An ensemble view
     :rtype: EnsembleView
     """
     st.subheader("Ensemble Configuration")
     col1, col2 = st.columns([4, 4])
     with col1:
-        selected_ensemble_tuple = st.selectbox(
+        selected_ensemble_context = st.selectbox(
             "Select an ensemble:",
             manifest.ensemble_with_run_ctx,
-            format_func=lambda tup: f"{tup[1].name}: Run {tup[0]}",
+            format_func=lambda context: f"{context.entity.name}: Run {context.run_id}",
         )
 
-    if selected_ensemble_tuple is not None:
-        _, selected_ensemble = selected_ensemble_tuple
+    if selected_ensemble_context is not None:
+        selected_ensemble = selected_ensemble_context.entity
     else:
         selected_ensemble = None
 
     members = selected_ensemble.models if selected_ensemble else []
 
     view = EnsembleView(selected_ensemble, members[0] if members else None)
 
     st.write("")
     view.status_element = st.empty()
 
     st.write("")
     with st.expander(label="Batch Settings"):
-        render_dataframe(
-            pd.DataFrame(
-                flatten_nested_keyvalue_containers(
-                    "batch_settings",
-                    selected_ensemble.model_dump() if selected_ensemble else {},
-                ),
-                columns=["Name", "Value"],
-            )
+        batch = flatten_nested_keyvalue_containers(
+            "batch_settings",
+            selected_ensemble.dict() if selected_ensemble else {},
         )
+        render_dataframe(pd.DataFrame(batch, columns=["Name", "Value"]))
 
     st.write("")
     with st.expander(label="Parameters"):
-        render_dataframe(
-            pd.DataFrame(
-                format_ensemble_params(selected_ensemble),
-                columns=["Name", "Value"],
-            )
-        )
+        params = format_ensemble_params(selected_ensemble)
+        render_dataframe(pd.DataFrame(params, columns=["Name", "Value"]))
 
     st.write("#")
     if selected_ensemble is not None:
         st.subheader(selected_ensemble.name + " Member Configuration")
     else:
         st.subheader("Member Configuration")
 
@@ -351,53 +335,50 @@
     view.update_view_model(member)
 
     st.write("")
     view.member_status_element = st.empty()
     st.write("Path: " + (member.path if member else ""))
     st.write("")
     with st.expander(label="Executable Arguments"):
-        render_dataframe(
-            pd.DataFrame(
-                {"All Arguments": member.exe_args if member is not None else []}
-            ),
-        )
+        arguments = member.exe_args if member is not None else []
+        render_dataframe(pd.DataFrame(arguments, columns=["All Arguments"]))
 
     st.write("")
     with st.expander(label="Batch and Run Settings"):
         col1, col2 = st.columns([4, 4])
         build_dataframe_generic(
             column=col1,
             title="Batch Settings",
             dict_name="batch_settings",
-            entity=member.model_dump() if member else {},
+            entity=member.dict() if member else {},
             df_columns=["Name", "Value"],
         )
         build_dataframe_generic(
             column=col2,
             title="Run Settings",
             dict_name="run_settings",
-            entity=member.model_dump() if member else {},
+            entity=member.dict() if member else {},
             df_columns=["Name", "Value"],
         )
 
     st.write("")
     with st.expander(label="Parameters and Generator Files"):
         col1, col2 = st.columns([4, 4])
         build_dataframe_generic(
             column=col1,
             title="Parameters",
             dict_name="params",
-            entity=member.model_dump() if member else {},
+            entity=member.dict() if member else {},
             df_columns=["Name", "Value"],
         )
         build_dataframe_generic(
             column=col2,
             title="Files",
             dict_name="files",
-            entity=member.model_dump() if member else {},
+            entity=member.dict() if member else {},
             df_columns=["Type", "File"],
         )
 
     st.write("")
     with st.expander(label="Colocated Database"):
         with st.container():
             col1, col2 = st.columns([6, 6])
@@ -462,7 +443,156 @@
         orc_view = orc_builder(manifest)
 
     ### Ensembles ###
     with ensembles:
         ens_view = ens_builder(manifest)
 
     return OverviewView(exp_view, app_view, orc_view, ens_view)
+
+
+def db_telem_builder(manifest: Manifest) -> DatabaseTelemetryView:
+    """Database Telemetry page to be rendered
+
+    This function organizes the views within
+    the Database Telemetry page.
+
+    :param manifest: Manifest of the Experiment
+    :type manifest: Manifest
+    :return: View of the DB Telemetry Page
+    :rtype: TelemetryView
+    """
+    st.header("Database Telemetry")
+
+    st.write("")
+
+    col1, _ = st.columns([6, 6])
+    with col1:
+        selected_orchestrator_context = st.selectbox(
+            "Select an orchestrator:",
+            manifest.orcs_with_run_ctx,
+            format_func=lambda context: f"{context.entity.name}: Run {context.run_id}",
+        )
+
+    st.write("")
+
+    if selected_orchestrator_context is not None:
+        run_id = selected_orchestrator_context.run_id
+        selected_orchestrator = selected_orchestrator_context.entity
+        shards = selected_orchestrator.shards
+        st.subheader(f"{selected_orchestrator.name}: Run {run_id} Telemetry")
+    else:
+        run_id, selected_orchestrator = None, None
+        shards = []
+        st.subheader("No Orchestrator Selected")
+
+    st.write("")
+
+    ### Orchestrator Summary ###
+    orc_summary_view = orc_summary_builder(selected_orchestrator)
+    st.write("")
+
+    ### Memory ###
+    memory_view = memory_view_builder(shards)
+    st.write("")
+
+    ### Clients ###
+    client_view = client_view_builder(shards)
+    st.write("")
+
+    return DatabaseTelemetryView(orc_summary_view, memory_view, client_view)
+
+
+def memory_view_builder(shards: t.List[Shard]) -> MemoryView:
+    """Memory section of Database Telemetry page to be rendered
+
+    :param shards: Shards of the selected Orchestrator
+    :type shards: t.List[Shard]
+    :return: View of the memory portion of the DB Telemetry page
+    :rtype: MemoryView
+    """
+
+    with st.expander(label="Memory"):
+        col1, col2 = st.columns([0.4, 0.5])
+        with col1:
+            shard = st.selectbox(
+                "Select a shard:",
+                shards,
+                format_func=lambda shard: shard.name,
+                key="memory_shard",
+            )
+            memory_table_element = st.empty()
+        with col2:
+            st.write("")
+            st.write("")
+            st.write("")
+            memory_graph_element = st.empty()
+            _, colb = st.columns([0.85, 0.15])
+            with colb:
+                export_button = st.empty()
+
+    return MemoryView(shard, memory_table_element, memory_graph_element, export_button)
+
+
+def client_view_builder(shards: t.List[Shard]) -> ClientView:
+    """Client section of Database Telemetry page to be rendered
+
+    :param shards: Shards of the selected Orchestrator
+    :type shards: t.List[Shard]
+    :return: View of the client portion of the DB Telemetry page
+    :rtype: ClientView
+    """
+
+    with st.expander(label="Clients"):
+        col1, col2 = st.columns([0.4, 0.5])
+        with col1:
+            shard = st.selectbox(
+                "Select a shard:",
+                shards,
+                format_func=lambda shard: shard.name,
+                key="client_shard",
+            )
+            client_table_element = st.empty()
+        with col2:
+            st.write("")
+            st.write("")
+            st.write("")
+            client_graph_element = st.empty()
+            _, colb = st.columns([0.85, 0.15])
+            with colb:
+                export_button = st.empty()
+
+    return ClientView(shard, client_table_element, client_graph_element, export_button)
+
+
+def orc_summary_builder(
+    selected_orchestrator: t.Optional[Orchestrator],
+) -> OrchestratorSummaryView:
+    """Orchestrator summary section of Database Telemetry page to be rendered
+
+    :param selected_orchestrator: Selected Orchestrator
+    :type selected_orchestrator: t.Optional[Orchestrator]
+    :return: View of the summary portion of the DB Telemetry page
+    :rtype: OrchestratorSummaryView
+    """
+    view = OrchestratorSummaryView(selected_orchestrator)
+    data = selected_orchestrator.db_hosts if selected_orchestrator else []
+
+    with st.expander(label="Orchestrator Summary"):
+
+        st.write("")
+        view.status_element = st.empty()
+        st.write(
+            "Number of shards: "
+            + (str(len(selected_orchestrator.shards)) if selected_orchestrator else "")
+        )
+        st.write(
+            "Type: "
+            + (selected_orchestrator.type if selected_orchestrator is not None else "")
+        )
+        st.write("Port: " + get_port(selected_orchestrator))
+        st.write("Interface: " + format_interfaces(selected_orchestrator))
+
+        st.write("")
+
+        render_dataframe(pd.DataFrame(data, columns=["Hosts"]))
+
+    return view
```

### Comparing `smartdashboard-0.0.3/smartdashboard.egg-info/PKG-INFO` & `smartdashboard-0.0.4/smartdashboard.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: smartdashboard
-Version: 0.0.3
+Version: 0.0.4
 Summary: Visualize SmartSim Experiments
 Author-email: "CrayLabs: a Hewlett Packard Enterprise OSS Organization" <craylabs@hpe.com>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://www.craylabs.org
 Project-URL: Documentation, https://github.com/CrayLabs/SmartDashboard
 Project-URL: Repository, https://github.com/CrayLabs/SmartDashboard
 Keywords: scientific,ai,workflow,hpc,analysis
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: altair>=5.2.0
 Requires-Dist: pandas>=2.0.0
-Requires-Dist: pydantic>=2.5.2
-Requires-Dist: streamlit>=1.28.0
+Requires-Dist: pydantic<2,>=1.10.14
+Requires-Dist: streamlit!=1.31.0,!=1.31.1,>=1.28.0
 Requires-Dist: watchdog>=3.0.0
 Provides-Extra: dev
 Requires-Dist: black>=20.8b1; extra == "dev"
 Requires-Dist: isort>=5.6.4; extra == "dev"
 Requires-Dist: pylint>=2.10.0; extra == "dev"
 Requires-Dist: pytest>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.10.1; extra == "dev"
@@ -37,24 +38,45 @@
 Requires-Dist: sphinx-book-theme==0.2.0; extra == "doc"
 Requires-Dist: nbsphinx>=0.8.2; extra == "doc"
 Requires-Dist: breathe==4.31.0; extra == "doc"
 Requires-Dist: jinja2==3.0.3; extra == "doc"
 
 # SmartDashboard
 
-SmartDashboard is an add-on to SmartSim that provides a dashboard to help users understand and monitor their SmartSim experiments in a visual way. Configuration, status, and logs are available for all launched entities within an experiment for easy inspection.
+SmartDashboard is an add-on to SmartSim that provides a dashboard to help users understand and monitor their SmartSim experiments in a visual way. Configuration, status, and logs are available for all launched entities within an experiment for easy inspection, along with memory and client data per shard for launched orchestrators.
 
-A ``Telemetry Monitor`` is a background process that is launched along with the experiment
-that produces the data displayed by SmartDashboard. The ``Telemetry Monitor`` can be disabled by
-adding ``export SMARTSIM_TELEMETRY_ENABLE=0`` as an environment variable. When disabled, SmartDashboard
-will not display any data. To re-enable, set the ``SMARTSIM_TELEMETRY_ENABLE`` environment variable to ``1``
-with ``export SMARTSIM_TELEMETRY_ENABLE=1``.
+A ``Telemetry Monitor`` is a background process that is launched alongside the experiment.
+It is responsible for generating the data displayed by SmartDashboard. The ``Telemetry Monitor`` can be disabled globally by
+adding ``export SMARTSIM_FLAG_TELEMETRY=0`` as an environment variable. When disabled, SmartDashboard
+will not display entity status data. To re-enable, set the ``SMARTSIM_FLAG_TELEMETRY`` environment variable to ``1``
+with ``export SMARTSIM_FLAG_TELEMETRY=1``. For workflows involving multiple experiments, SmartSim provides the attributes
+``Experiment.telemetry.enable`` and ``Experiment.telemetry.disable`` to manage the enabling or disabling of telemetry on a per-experiment basis.
+
+`Orchestrator` memory and client data can be collected by enabling database telemetry. To do so, add ``Orchestrator.telemetry.enable``
+after creating an `Orchestrator` within the driver script. Database telemetry is enabled per `Orchestrator`, so if there are multiple
+`Orchestrators` launched, they will each need to be enabled separately in the driver script.
 
-Experiment metadata is also stored in the ``.smartsim`` directory, a hidden folder for internal api use and used by the dashboard.
-Deletion of the experiment folder will remove all experiment metadata.
+```python
+# enabling telemetry example
+
+from smartsim import Experiment
+
+exp = Experiment("experiment", launcher="auto")
+exp.telemetry.enable()
+
+db = exp.create_database(db_nodes=3)
+db.telemetry.enable()
+
+exp.start(db, block=True)
+exp.stop(db)
+```
+
+Experiment metadata is stored in the ``.smartsim`` directory, a hidden folder used by the internal api and accessed by the dashboard.
+This folder can be found within the created experiment directory.
+Deletion of the experiment folder will remove all associated metadata.
 
 ## Installation
 
 It's important to note that SmartDashboard only works while using SmartSim, so SmartSim will need to be installed as well.
 SmartSim installation docs can be found [here](https://www.craylabs.org/docs/installation_instructions/basic.html).
 
 ### User Install
@@ -86,14 +108,15 @@
 ```
 
 ```python
 # hello_world.py
 from smartsim import Experiment
 
 exp = Experiment("hello_world_exp", launcher="auto")
+exp.telemetry.enable()
 run = exp.create_run_settings(exe="echo", exe_args="Hello World!")
 run.set_tasks(60)
 run.set_tasks_per_node(20)
 
 model = exp.create_model("hello_world", run)
 exp.start(model, block=True, summary=True)
 ```
@@ -136,8 +159,13 @@
 
 ## Using SmartDashboard
 
 Once the dashboard is launched, a browser will open to `http://localhost:<port>`. SmartDashboard currently has two tabs on the left hand side.
   
 `Experiment Overview:` This tab is where configuration information, statuses, and logs are located for each launched entity of the experiment. The `Experiment` section displays configuration information for the overall experiment and its logs. In the `Applications` section, also known as SmartSim `Models`, select a launched application to see its status, what it was configured with, and its logs. The `Orchestrators` section also provides configuration and status information, as well as logs per shard for a selected orchestrator. Finally, in the `Ensembles` section, select an ensemble to see its status and configuration. Then select any of its members to see its status, configuration, and logs.
   
+`Database Telemetry:` This tab provides additional details about `Orchestrators`.
+The `Orchestrator Summary` section shows configuration and status information of the selected. The `Memory`
+section provides memory usage data per shard within the `Orchestrator`. The `Clients`
+section displays client data per shard within the `Orchestrator`.  
+
 `Help:` This tab links to SmartSim documentation and provides a SmartSim contact for support.
```

### Comparing `smartdashboard-0.0.3/smartdashboard.egg-info/SOURCES.txt` & `smartdashboard-0.0.4/smartdashboard.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 smartdashboard/views.py
 smartdashboard.egg-info/PKG-INFO
 smartdashboard.egg-info/SOURCES.txt
 smartdashboard.egg-info/dependency_links.txt
 smartdashboard.egg-info/entry_points.txt
 smartdashboard.egg-info/requires.txt
 smartdashboard.egg-info/top_level.txt
+smartdashboard/pages/2_Database_Telemetry.py
 smartdashboard/pages/3_Help.py
 smartdashboard/pages/__init__.py
 smartdashboard/static/SmartSim.png
 smartdashboard/static/style.css
 smartdashboard/utils/LogReader.py
 smartdashboard/utils/ManifestReader.py
 smartdashboard/utils/StatusReader.py
 smartdashboard/utils/__init__.py
+smartdashboard/utils/argparser.py
 smartdashboard/utils/errors.py
 smartdashboard/utils/helpers.py
 smartdashboard/utils/pageSetup.py
 smartdashboard/utils/status.py
```

