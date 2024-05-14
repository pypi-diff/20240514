# Comparing `tmp/tox-ipdb-plugin-0.3.tar.gz` & `tmp/tox_ipdb_plugin-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-ipdb-plugin-0.3.tar", last modified: Thu Feb  2 13:39:29 2023, max compression
+gzip compressed data, was "tox_ipdb_plugin-1.0.tar", last modified: Tue May 14 07:25:40 2024, max compression
```

## Comparing `tox-ipdb-plugin-0.3.tar` & `tox_ipdb_plugin-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-02-02 13:39:29.852937 tox-ipdb-plugin-0.3/
--rw-r--r--   0 tomas     (1000) tomas     (1000)      305 2023-02-02 13:38:16.000000 tox-ipdb-plugin-0.3/CHANGELOG.rst
--rw-r--r--   0 tomas     (1000) tomas     (1000)    35149 2023-02-02 13:31:21.000000 tox-ipdb-plugin-0.3/LICENSE
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1585 2023-02-02 13:39:29.852937 tox-ipdb-plugin-0.3/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)      278 2023-02-02 13:32:23.000000 tox-ipdb-plugin-0.3/README.rst
--rw-r--r--   0 tomas     (1000) tomas     (1000)       81 2023-02-02 13:31:21.000000 tox-ipdb-plugin-0.3/pyproject.toml
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1593 2023-02-02 13:39:29.852937 tox-ipdb-plugin-0.3/setup.cfg
--rw-r--r--   0 tomas     (1000) tomas     (1000)      129 2023-02-02 13:31:21.000000 tox-ipdb-plugin-0.3/setup.py
--rw-r--r--   0 tomas     (1000) tomas     (1000)     2617 2023-02-02 13:32:29.000000 tox-ipdb-plugin-0.3/tox_ipdb.py
-drwxr-xr-x   0 tomas     (1000) tomas     (1000)        0 2023-02-02 13:39:29.852937 tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/
--rw-r--r--   0 tomas     (1000) tomas     (1000)     1585 2023-02-02 13:39:29.000000 tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/PKG-INFO
--rw-r--r--   0 tomas     (1000) tomas     (1000)      314 2023-02-02 13:39:29.000000 tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        1 2023-02-02 13:39:29.000000 tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       22 2023-02-02 13:39:29.000000 tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/entry_points.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)       61 2023-02-02 13:39:29.000000 tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/requires.txt
--rw-r--r--   0 tomas     (1000) tomas     (1000)        9 2023-02-02 13:39:29.000000 tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 vzima     (1000) vzima     (1000)        0 2024-05-14 07:25:40.564376 tox_ipdb_plugin-1.0/
+-rw-r--r--   0 vzima     (1000) vzima     (1000)      478 2024-05-14 07:22:59.000000 tox_ipdb_plugin-1.0/CHANGELOG.rst
+-rw-r--r--   0 vzima     (1000) vzima     (1000)    35149 2020-02-26 09:37:27.000000 tox_ipdb_plugin-1.0/LICENSE
+-rw-r--r--   0 vzima     (1000) vzima     (1000)     1954 2024-05-14 07:25:40.564376 tox_ipdb_plugin-1.0/PKG-INFO
+-rw-r--r--   0 vzima     (1000) vzima     (1000)      278 2020-02-26 10:35:46.000000 tox_ipdb_plugin-1.0/README.rst
+-rw-r--r--   0 vzima     (1000) vzima     (1000)      572 2024-05-13 07:56:06.000000 tox_ipdb_plugin-1.0/pyproject.toml
+-rw-r--r--   0 vzima     (1000) vzima     (1000)     1410 2024-05-14 07:25:40.568376 tox_ipdb_plugin-1.0/setup.cfg
+-rw-r--r--   0 vzima     (1000) vzima     (1000)      129 2022-10-13 07:05:30.000000 tox_ipdb_plugin-1.0/setup.py
+-rw-r--r--   0 vzima     (1000) vzima     (1000)     2749 2024-05-14 07:24:38.000000 tox_ipdb_plugin-1.0/tox_ipdb.py
+drwxr-xr-x   0 vzima     (1000) vzima     (1000)        0 2024-05-14 07:25:40.564376 tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/
+-rw-r--r--   0 vzima     (1000) vzima     (1000)     1954 2024-05-14 07:25:40.000000 tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vzima     (1000) vzima     (1000)      314 2024-05-14 07:25:40.000000 tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vzima     (1000) vzima     (1000)        1 2024-05-14 07:25:40.000000 tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vzima     (1000) vzima     (1000)       22 2024-05-14 07:25:40.000000 tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 vzima     (1000) vzima     (1000)       35 2024-05-14 07:25:40.000000 tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/requires.txt
+-rw-r--r--   0 vzima     (1000) vzima     (1000)        9 2024-05-14 07:25:40.000000 tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/top_level.txt
```

### Comparing `tox-ipdb-plugin-0.3/LICENSE` & `tox_ipdb_plugin-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-ipdb-plugin-0.3/PKG-INFO` & `tox_ipdb_plugin-1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: tox-ipdb-plugin
-Version: 0.3
+Version: 1.0
 Summary: Tox plugin which installs ipdb in tox environments.
 Home-page: https://github.com/CZ-NIC/tox-ipdb-plugin
 Author: Vlastimil Zíma
 Author-email: vlastimil.zima@nic.cz
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Plugins
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: ~=3.7
-Provides-Extra: quality
+Requires-Python: ~=3.8
 License-File: LICENSE
+Requires-Dist: tox>=3.0
+Provides-Extra: quality
+Requires-Dist: doc8; extra == "quality"
+Requires-Dist: mypy; extra == "quality"
+Requires-Dist: ruff; extra == "quality"
 
 tox-ipdb-plugin
 ===============
 
 Tox plugin which installs ipdb in tox environments.
 This is useful for local development, if you don't want to modify the tox.ini.
 
@@ -38,14 +43,23 @@
 ChangeLog
 =========
 
 .. contents:: Releases
    :backlinks: none
    :local:
 
+1.0 (2024-05-14)
+----------------
+
+* Drop support for python 3.7.
+* Add support for python 3.11.
+* Add support for python 3.12.
+* Fix for tox 4.15.
+* Update project setup.
+
 0.3 (2023-02-02)
 ----------------
 
 * Update for tox v4.
 
 0.2 (2022-10-13)
 ----------------
```

### Comparing `tox-ipdb-plugin-0.3/setup.cfg` & `tox_ipdb_plugin-1.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,63 @@
 [metadata]
 name = tox-ipdb-plugin
-version = 0.3
+version = 1.0
 url = https://github.com/CZ-NIC/tox-ipdb-plugin
 author = Vlastimil Zíma
 author_email = vlastimil.zima@nic.cz
 description = Tox plugin which installs ipdb in tox environments.
 long_description = file: README.rst, CHANGELOG.rst
 license = GPLv3+
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Environment :: Plugins
 	Framework :: tox
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Debuggers
 	Topic :: Software Development :: Testing
 
 [options]
 py_modules = 
 	tox_ipdb
-python_requires = ~=3.7
+python_requires = ~=3.8
 install_requires = 
 	tox>=3.0
 
 [options.entry_points]
 tox = 
 	ipdb = tox_ipdb
 
 [options.extras_require]
 quality = 
-	bandit
 	doc8
-	flake8
-	isort
 	mypy
-	pydocstyle
+	ruff
 
 [doc8]
 max-line-length = 120
 allow-long-titles = true
 
-[flake8]
-max-line-length = 120
-max-complexity = 10
-
-[isort]
-line_length = 120
-combine_as_imports = true
-
 [mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_ignores = false
 
 [mypy-tests]
 disallow_untyped_defs = false
 
-[pydocstyle]
-convention = google
-add_ignore = D105,D106,D107
-add_select = D204,D400,D401
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tox-ipdb-plugin-0.3/tox_ipdb.py` & `tox_ipdb_plugin-1.0/tox_ipdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Tox plugin which installs ipdb in tox environments."""
 import logging
-from distutils.version import LooseVersion
 
 import tox
 
-__version__ = '0.3'
+__version__ = '1.0'
 _LOGGER = logging.getLogger(__name__)
 
 
-if LooseVersion(tox.__version__) < LooseVersion('4.0.0'):
+if tox.__version__ < '4':
     # TOX 3
     from tox import hookimpl  # type: ignore[attr-defined]
     from tox.action import Action
     from tox.config import Config, DepConfig  # type: ignore[attr-defined]
     from tox.venv import VirtualEnv
 
     @hookimpl
@@ -55,11 +54,15 @@
             # It's not a provision env, add ipdb.
             new_deps = old_deps + ['ipdb']
             _LOGGER.debug("tox-ipdb-plugin[%s]: Appending ipdb to environment dependencies.", env_conf.name)
 
         _LOGGER.debug("tox-ipdb-plugin[%s]: New deps: %s", env_conf.name, new_deps)
 
         override = Override('{}.deps={}'.format(env_conf.name, '\n'.join(new_deps)))
-        env_conf.loaders[0].overrides[override.key] = override
+        # API changed in tox 4.15.0
+        if tox.__version__ < '4.15':
+            env_conf.loaders[0].overrides[override.key] = override  # type: ignore[assignment]
+        else:
+            env_conf.loaders[0].overrides.setdefault(override.key, []).append(override)
 
         # Clear cache
         env_conf._defined['deps']._cache = _PLACE_HOLDER  # type: ignore[attr-defined]  # _cache is not public API
```

### Comparing `tox-ipdb-plugin-0.3/tox_ipdb_plugin.egg-info/PKG-INFO` & `tox_ipdb_plugin-1.0/tox_ipdb_plugin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: tox-ipdb-plugin
-Version: 0.3
+Version: 1.0
 Summary: Tox plugin which installs ipdb in tox environments.
 Home-page: https://github.com/CZ-NIC/tox-ipdb-plugin
 Author: Vlastimil Zíma
 Author-email: vlastimil.zima@nic.cz
 License: GPLv3+
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Plugins
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: ~=3.7
-Provides-Extra: quality
+Requires-Python: ~=3.8
 License-File: LICENSE
+Requires-Dist: tox>=3.0
+Provides-Extra: quality
+Requires-Dist: doc8; extra == "quality"
+Requires-Dist: mypy; extra == "quality"
+Requires-Dist: ruff; extra == "quality"
 
 tox-ipdb-plugin
 ===============
 
 Tox plugin which installs ipdb in tox environments.
 This is useful for local development, if you don't want to modify the tox.ini.
 
@@ -38,14 +43,23 @@
 ChangeLog
 =========
 
 .. contents:: Releases
    :backlinks: none
    :local:
 
+1.0 (2024-05-14)
+----------------
+
+* Drop support for python 3.7.
+* Add support for python 3.11.
+* Add support for python 3.12.
+* Fix for tox 4.15.
+* Update project setup.
+
 0.3 (2023-02-02)
 ----------------
 
 * Update for tox v4.
 
 0.2 (2022-10-13)
 ----------------
```

