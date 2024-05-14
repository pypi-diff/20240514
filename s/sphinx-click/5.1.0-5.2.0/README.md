# Comparing `tmp/sphinx-click-5.1.0.tar.gz` & `tmp/sphinx_click-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-click-5.1.0.tar", last modified: Tue Nov 21 16:42:06 2023, max compression
+gzip compressed data, was "sphinx_click-5.2.0.tar", last modified: Tue May 14 11:44:32 2024, max compression
```

## Comparing `sphinx-click-5.1.0.tar` & `sphinx_click-5.2.0.tar`

### file list

```diff
@@ -1,70 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.970311 sphinx-click-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.962311 sphinx-click-5.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.962311 sphinx-click-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2023-11-21 16:42:06.970311 sphinx-click-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/examples/commandcollections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/examples/commands.rst
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/examples/groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/examples/commandcollections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/examples/commandcollections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/examples/commandcollections/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/examples/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/examples/commands/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/examples/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/examples/groups/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/examples/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.962311 sphinx-click-5.1.0/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-11-21 16:42:06.970311 sphinx-click-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.966311 sphinx-click-5.1.0/sphinx_click/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/sphinx_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18285 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/sphinx_click/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.970311 sphinx-click-5.1.0/sphinx_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/sphinx_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/sphinx_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/sphinx_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/sphinx_click.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/sphinx_click.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/sphinx_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-21 16:42:06.000000 sphinx-click-5.1.0/sphinx_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.970311 sphinx-click-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.962311 sphinx-click-5.1.0/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.970311 sphinx-click-5.1.0/tests/roots/basics/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/roots/basics/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/roots/basics/greet.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/roots/basics/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:42:06.970311 sphinx-click-5.1.0/tests/roots/nested-full/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/roots/nested-full/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/roots/nested-full/greet.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/roots/nested-full/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    24485 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-21 16:41:57.000000 sphinx-click-5.1.0/tox.ini
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.976758 sphinx_click-5.2.0/
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      640 2018-10-03 13:49:15.000000 sphinx_click-5.2.0/.editorconfig
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/.github/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      428 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/.github/workflows/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     2537 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/.github/workflows/ci.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1116 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/.pre-commit-config.yaml
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1355 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/AUTHORS
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     6503 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/ChangeLog
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1095 2018-01-02 16:35:12.000000 sphinx_click-5.2.0/LICENSE
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     3425 2024-05-14 11:44:32.976758 sphinx_click-5.2.0/PKG-INFO
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     2122 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/README.rst
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/docs/
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       61 2018-10-03 13:49:15.000000 sphinx_click-5.2.0/docs/changelog.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1819 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/conf.py
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1200 2018-10-03 13:49:15.000000 sphinx_click-5.2.0/docs/contributing.rst
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/docs/examples/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      611 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/commandcollections.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      509 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/commands.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      490 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/groups.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       93 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/index.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      580 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/index.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      536 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/installation.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    10068 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/usage.rst
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/examples/
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/examples/commandcollections/
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        0 2022-04-07 12:52:39.000000 sphinx_click-5.2.0/examples/commandcollections/__init__.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      828 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/examples/commandcollections/cli.py
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/examples/commands/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      710 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/examples/commands/cli.py
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/examples/groups/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      477 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/examples/groups/cli.py
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      153 2022-04-07 12:52:39.000000 sphinx_click-5.2.0/examples/setup.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      193 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/pyproject.toml
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.972758 sphinx_click-5.2.0/releasenotes/
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/releasenotes/notes/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      351 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      573 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      247 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      265 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-show_default-from-context-support-ab4aeffcc513502d.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       88 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       65 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       65 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/python-3.12-support-f2ed1dc438bd42ee.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      208 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/show-typer-arg-help-text-fae802f6878fa100.yaml
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       32 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/requirements.txt
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1497 2024-05-14 11:44:32.976758 sphinx_click-5.2.0/setup.cfg
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      110 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/setup.py
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/sphinx_click/
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       43 2022-04-07 12:52:39.000000 sphinx_click-5.2.0/sphinx_click/__init__.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    18823 2024-05-14 11:44:21.000000 sphinx_click-5.2.0/sphinx_click/ext.py
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/sphinx_click.egg-info/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     3425 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/PKG-INFO
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1728 2024-05-14 11:44:32.000000 sphinx_click-5.2.0/sphinx_click.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        1 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        1 2018-07-13 13:58:30.000000 sphinx_click-5.2.0/sphinx_click.egg-info/not-zip-safe
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       46 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/pbr.json
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       32 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/requires.txt
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       13 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/top_level.txt
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/
+-rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        0 2018-01-02 16:35:12.000000 sphinx_click-5.2.0/tests/__init__.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      855 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/conftest.py
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.972758 sphinx_click-5.2.0/tests/roots/
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/roots/basics/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      160 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/basics/conf.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      445 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/basics/greet.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       54 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/basics/index.rst
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/roots/commands/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      116 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/commands/conf.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      357 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/commands/greet.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       78 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/commands/index.rst
+drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/roots/nested-full/
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      116 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/nested-full/conf.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      357 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/nested-full/greet.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       85 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/nested-full/index.rst
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     4516 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/test_extension.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    26664 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/test_formatter.py
+-rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      785 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tox.ini
```

### Comparing `sphinx-click-5.1.0/.editorconfig` & `sphinx_click-5.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/.github/workflows/ci.yaml` & `sphinx_click-5.2.0/.github/workflows/ci.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 jobs:
   lint:
     name: Run linters
     runs-on: ubuntu-latest
     steps:
       - name: Checkout source code
         uses: actions/checkout@v3
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         uses: actions/setup-python@v4
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: python -m pip install tox
       - name: Run tox
         run: tox -e style
   test:
     name: Run unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python: ["3.8", "3.9", "3.10", "3.11"]
+        python: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: Checkout source code
         uses: actions/checkout@v3
         # We need history to build the package
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python }}
@@ -44,18 +44,18 @@
     runs-on: ubuntu-latest
     steps:
       - name: Checkout source code
         uses: actions/checkout@v3
         # We need history for release notes
         with:
           fetch-depth: 0
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         uses: actions/setup-python@v4
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: python -m pip install tox
       - name: Build docs (via tox)
         run: tox -e docs
       - name: Archive build results
         uses: actions/upload-artifact@v3
         with:
@@ -69,18 +69,18 @@
     if: github.event_name == 'push'
     steps:
       - name: Checkout source code
         uses: actions/checkout@v3
         # We need history to build the package
         with:
           fetch-depth: 0
-      - name: Set up Python 3.11
+      - name: Set up Python 3.12
         uses: actions/setup-python@v4
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: Install dependencies
         run: python -m pip install build
       - name: Build a binary wheel and a source tarball
         run: python -m build --sdist --wheel --outdir dist/ .
       - name: Publish distribution to PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@master
```

### Comparing `sphinx-click-5.1.0/.pre-commit-config.yaml` & `sphinx_click-5.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/AUTHORS` & `sphinx_click-5.2.0/AUTHORS`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 A Wegner <AWegnerGitHub@users.noreply.github.com>
 Adam Dangoor <adamdangoor@gmail.com>
 Adam Liddell <git@aliddell.com>
 Ahmed Masud <ahmed.masud@trustifier.com>
 AlexTereshenkov <50622389+AlexTereshenkov@users.noreply.github.com>
+Andreas Eisenbarth <andreas.eisenbarth@embl.de>
 Andy Wegner <andy@andrewwegner.com>
 Arie Bovenberg <a.c.bovenberg@gmail.com>
 Giel van Schijndel <giel@mortis.eu>
 Giel van Schijndel <me@mortis.eu>
 Hugo Osvaldo Barrera <hugo@barrera.io>
 James Ennis <james.ennis@codethink.com>
 Jared Dillard <jared.dillard+github@gmail.com>
@@ -26,7 +27,8 @@
 William Jamir Silva <williamjamir@gmail.com>
 coloursofnoise <coloursofthenoise@gmail.com>
 frostming <mianghong@gmail.com>
 jtrakk <43392409+jtrakk@users.noreply.github.com>
 oleg.hoefling <oleg.hoefling@gmail.com>
 pdmurray <peynmurray@gmail.com>
 tomMoral <thomas.moreau.2010@gmail.com>
+u-shiori <u.shiori1010@gmail.com>
```

### Comparing `sphinx-click-5.1.0/ChangeLog` & `sphinx_click-5.2.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+5.2.0
+-----
+
+* Fix show\_default with context\_settings
+* tests: Add tests for 'commands' option
+* Add support, testing for Python 3.12
+* Add release note for typer arg help text feature
+* Interpret help for arguments
+* typing: Update for latest types-docutils
+
 5.1.0
 -----
 
 * tox: Remove py37 entries
 * Add support for mocking modules
 * docs: Fix indentation
 * setup: Add Sphinx classifier
```

### Comparing `sphinx-click-5.1.0/LICENSE` & `sphinx_click-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/PKG-INFO` & `sphinx_click-5.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-click
-Version: 5.1.0
+Version: 5.2.0
 Summary: Sphinx extension that automatically documents click applications
 Home-page: https://github.com/click-contrib/sphinx-click
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/click-contrib/sphinx-click/issues
 Project-URL: Documentation, https://sphinx-click.readthedocs.io/en/latest
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
+License-File: AUTHORS
 Requires-Dist: sphinx>=2.0
 Requires-Dist: click>=7.0
 Requires-Dist: docutils
 
 ============
 sphinx-click
 ============
```

### Comparing `sphinx-click-5.1.0/README.rst` & `sphinx_click-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/docs/conf.py` & `sphinx_click-5.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/docs/contributing.rst` & `sphinx_click-5.2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/docs/examples/commandcollections.rst` & `sphinx_click-5.2.0/docs/examples/commandcollections.rst`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/docs/index.rst` & `sphinx_click-5.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/docs/installation.rst` & `sphinx_click-5.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/docs/usage.rst` & `sphinx_click-5.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/examples/commandcollections/cli.py` & `sphinx_click-5.2.0/examples/commandcollections/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/examples/commands/cli.py` & `sphinx_click-5.2.0/examples/commands/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml` & `sphinx_click-5.2.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/setup.cfg` & `sphinx_click-5.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/sphinx_click/ext.py` & `sphinx_click-5.2.0/sphinx_click/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from sphinx.ext.autodoc import mock
 
 LOG = logging.getLogger(__name__)
 
 NESTED_FULL = 'full'
 NESTED_SHORT = 'short'
 NESTED_NONE = 'none'
+NestedT = ty.Literal['full', 'short', 'none', None]
 
 ANSI_ESC_SEQ_RE = re.compile(r'\x1B\[\d+(;\d+){0,2}m', flags=re.MULTILINE)
 
 _T_Formatter = ty.Callable[[click.Context], ty.Generator[str, None, None]]
 
 
 def _process_lines(event_name: str) -> ty.Callable[[_T_Formatter], _T_Formatter]:
@@ -58,15 +59,15 @@
     """Alternative, non-prefixed version of 'get_usage'."""
     formatter = ctx.make_formatter()
     pieces = ctx.command.collect_usage_pieces(ctx)
     formatter.write_usage(ctx.command_path, ' '.join(pieces), prefix='')
     return formatter.getvalue().rstrip('\n')  # type: ignore
 
 
-def _get_help_record(opt: click.Option) -> ty.Tuple[str, str]:
+def _get_help_record(ctx: click.Context, opt: click.Option) -> ty.Tuple[str, str]:
     """Re-implementation of click.Opt.get_help_record.
 
     The variant of 'get_help_record' found in Click makes uses of slashes to
     separate multiple opts, and formats option arguments using upper case. This
     is not compatible with Sphinx's 'option' directive, which expects
     comma-separated opts and option arguments surrounded by angle brackets [1].
 
@@ -94,20 +95,25 @@
             out.append(opt.help)
     else:
         if opt.required:
             out.append('**Required**')
 
     extras = []
 
-    if isinstance(opt.show_default, str):
+    if opt.show_default is not None:
+        show_default = opt.show_default
+    else:
+        show_default = ctx.show_default
+
+    if isinstance(show_default, str):
         # Starting from Click 7.0 show_default can be a string. This is
         # mostly useful when the default is not a constant and
         # documentation thus needs a manually written string.
-        extras.append(':default: ``%s``' % opt.show_default)
-    elif opt.default is not None and opt.show_default:
+        extras.append(':default: ``%s``' % show_default)
+    elif opt.default is not None and show_default:
         extras.append(
             ':default: ``%s``'
             % (
                 ', '.join(str(d) for d in opt.default)
                 if isinstance(opt.default, (list, tuple))
                 else opt.default,
             )
@@ -160,17 +166,19 @@
     yield '.. code-block:: shell'
     yield ''
     for line in _get_usage(ctx).splitlines():
         yield _indent(line)
     yield ''
 
 
-def _format_option(opt: click.Option) -> ty.Generator[str, None, None]:
+def _format_option(
+    ctx: click.Context, opt: click.Option
+) -> ty.Generator[str, None, None]:
     """Format the output for a `click.Option`."""
-    opt_help = _get_help_record(opt)
+    opt_help = _get_help_record(ctx, opt)
 
     yield '.. option:: {}'.format(opt_help[0])
     if opt_help[1]:
         yield ''
         bar_enabled = False
         for line in statemachine.string2lines(
             ANSI_ESC_SEQ_RE.sub('', opt_help[1]), tab_width=4, convert_whitespace=True
@@ -191,28 +199,34 @@
     params = [
         param
         for param in ctx.command.params
         if isinstance(param, click.Option) and not getattr(param, 'hidden', False)
     ]
 
     for param in params:
-        for line in _format_option(param):
+        for line in _format_option(ctx, param):
             yield line
         yield ''
 
 
 def _format_argument(arg: click.Argument) -> ty.Generator[str, None, None]:
     """Format the output of a `click.Argument`."""
     yield '.. option:: {}'.format(arg.human_readable_name)
     yield ''
     yield _indent(
         '{} argument{}'.format(
             'Required' if arg.required else 'Optional', '(s)' if arg.nargs != 1 else ''
         )
     )
+    # Subclasses of click.Argument may add a `help` attribute (like typer.main.TyperArgument)
+    if hasattr(arg, 'help'):
+        yield ''
+        help_string = ANSI_ESC_SEQ_RE.sub('', getattr(arg, 'help'))
+        for line in _format_help(help_string):
+            yield _indent(line)
 
 
 @_process_lines("sphinx-click-process-arguments")
 def _format_arguments(ctx: click.Context) -> ty.Generator[str, None, None]:
     """Format all `click.Argument` for a `click.Command`."""
     params = [x for x in ctx.command.params if isinstance(x, click.Argument)]
 
@@ -311,15 +325,15 @@
         return sorted(lookup.values(), key=lambda item: item.name)
 
     return [lookup[command] for command in commands if command in lookup]
 
 
 def _format_command(
     ctx: click.Context,
-    nested: str,
+    nested: NestedT,
     commands: ty.Optional[ty.List[str]] = None,
 ) -> ty.Generator[str, None, None]:
     """Format the output of `click.Command`."""
     if ctx.command.hidden:
         return None
 
     # description
@@ -387,24 +401,24 @@
             continue
 
         for line in _format_subcommand(command_obj):
             yield line
         yield ''
 
 
-def nested(argument: ty.Optional[str]) -> ty.Optional[str]:
+def nested(argument: ty.Optional[str]) -> NestedT:
     values = (NESTED_FULL, NESTED_SHORT, NESTED_NONE, None)
 
     if argument not in values:
         raise ValueError(
             "%s is not a valid value for ':nested:'; allowed values: %s"
-            % directives.format_values(values)
+            % directives.format_values(values)  # type: ignore
         )
 
-    return argument
+    return ty.cast(NestedT, argument)
 
 
 class ClickDirective(rst.Directive):
     has_content = False
     required_arguments = 1
     option_spec = {
         'prog': directives.unchanged_required,
@@ -452,15 +466,15 @@
         return parser
 
     def _generate_nodes(
         self,
         name: str,
         command: click.Command,
         parent: ty.Optional[click.Context],
-        nested: str,
+        nested: NestedT,
         commands: ty.Optional[ty.List[str]] = None,
         semantic_group: bool = False,
     ) -> ty.List[nodes.section]:
         """Generate the relevant Sphinx nodes.
 
         Format a `click.Group` or `click.Command`.
 
@@ -486,15 +500,15 @@
             nodes.title(text=name),
             ids=[nodes.make_id(ctx.command_path)],
             names=[nodes.fully_normalize_name(ctx.command_path)],
         )
 
         # Summary
         source_name = ctx.command_path
-        result = statemachine.ViewList()
+        result = statemachine.StringList()
 
         ctx.meta["sphinx-click-env"] = self.env
         if semantic_group:
             lines = _format_description(ctx)
         else:
             lines = _format_command(ctx, nested, commands)
 
@@ -526,23 +540,23 @@
                         self._generate_nodes(
                             command.name, command, parent=parent, nested=nested
                         )
                     )
 
         return [section]
 
-    def run(self) -> ty.Iterable[nodes.section]:
+    def run(self) -> ty.Sequence[nodes.section]:
         self.env = self.state.document.settings.env
 
         command = self._load_module(self.arguments[0])
 
         if 'prog' not in self.options:
             raise self.error(':prog: must be specified')
 
-        prog_name = self.options.get('prog')
+        prog_name = self.options['prog']
         show_nested = 'show-nested' in self.options
         nested = self.options.get('nested')
 
         if show_nested:
             if nested:
                 raise self.error(
                     "':nested:' and ':show-nested:' are mutually exclusive"
@@ -553,15 +567,15 @@
                     DeprecationWarning,
                 )
                 nested = NESTED_FULL if show_nested else NESTED_SHORT
 
         commands = None
         if self.options.get('commands'):
             commands = [
-                command.strip() for command in self.options.get('commands').split(',')
+                command.strip() for command in self.options['commands'].split(',')
             ]
 
         return self._generate_nodes(prog_name, command, None, nested, commands)
 
 
 def setup(app: application.Sphinx) -> ty.Dict[str, ty.Any]:
     # Need autodoc to support mocking modules
```

### Comparing `sphinx-click-5.1.0/sphinx_click.egg-info/PKG-INFO` & `sphinx_click-5.2.0/sphinx_click.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-click
-Version: 5.1.0
+Version: 5.2.0
 Summary: Sphinx extension that automatically documents click applications
 Home-page: https://github.com/click-contrib/sphinx-click
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/click-contrib/sphinx-click/issues
 Project-URL: Documentation, https://sphinx-click.readthedocs.io/en/latest
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
+License-File: AUTHORS
 Requires-Dist: sphinx>=2.0
 Requires-Dist: click>=7.0
 Requires-Dist: docutils
 
 ============
 sphinx-click
 ============
```

### Comparing `sphinx-click-5.1.0/sphinx_click.egg-info/SOURCES.txt` & `sphinx_click-5.2.0/sphinx_click.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,19 @@
 examples/commandcollections/__init__.py
 examples/commandcollections/cli.py
 examples/commands/cli.py
 examples/groups/cli.py
 releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
 releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
 releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
+releasenotes/notes/add-show_default-from-context-support-ab4aeffcc513502d.yaml
 releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
 releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
+releasenotes/notes/python-3.12-support-f2ed1dc438bd42ee.yaml
+releasenotes/notes/show-typer-arg-help-text-fae802f6878fa100.yaml
 sphinx_click/__init__.py
 sphinx_click/ext.py
 sphinx_click.egg-info/PKG-INFO
 sphinx_click.egg-info/SOURCES.txt
 sphinx_click.egg-info/dependency_links.txt
 sphinx_click.egg-info/not-zip-safe
 sphinx_click.egg-info/pbr.json
@@ -43,10 +46,13 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_extension.py
 tests/test_formatter.py
 tests/roots/basics/conf.py
 tests/roots/basics/greet.py
 tests/roots/basics/index.rst
+tests/roots/commands/conf.py
+tests/roots/commands/greet.py
+tests/roots/commands/index.rst
 tests/roots/nested-full/conf.py
 tests/roots/nested-full/greet.py
 tests/roots/nested-full/index.rst
```

### Comparing `sphinx-click-5.1.0/tests/conftest.py` & `sphinx_click-5.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx-click-5.1.0/tests/test_extension.py` & `sphinx_click-5.2.0/tests/test_extension.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,16 +40,58 @@
     assert section[1].astext() == 'A sample command group.'
     assert isinstance(section[2], nodes.literal_block)
 
     assert isinstance(section[3], nodes.rubric)
     assert section[3].astext() == 'Commands'
     assert isinstance(section[4], sphinx_nodes.index)
     assert isinstance(section[5], sphinx_nodes.desc)
+    assert section[5].astext() == 'hello\n\nGreet a user.'
     assert isinstance(section[6], sphinx_nodes.index)
     assert isinstance(section[7], sphinx_nodes.desc)
+    assert section[7].astext() == 'world\n\nGreet the world.'
+
+
+def test_commands(make_app, rootdir):
+    srcdir = rootdir / 'commands'
+    app = make_app('xml', srcdir=srcdir)
+    app.build()
+
+    # TODO: rather than using the pickled doctree, we should decode the XML
+    content = pickle.loads((app.doctreedir / 'index.doctree').read_bytes())
+
+    # doc has format like so:
+    #
+    # document:
+    #   section:
+    #     title:
+    #     section:
+    #       title:
+    #       paragraph:
+    #       literal_block:
+    #       rubric:
+    #       index:
+    #       desc:
+    #         desc_signature:
+    #         desc_signature:
+
+    section = content[0][1]
+    assert isinstance(section, nodes.section)
+
+    assert isinstance(section[0], nodes.title)
+    assert section[0].astext() == 'greet'
+    assert isinstance(section[1], nodes.paragraph)
+    assert section[1].astext() == 'A sample command group.'
+    assert isinstance(section[2], nodes.literal_block)
+
+    # we should only show a single command, 'world'
+    assert isinstance(section[3], nodes.rubric)
+    assert section[3].astext() == 'Commands'
+    assert isinstance(section[4], sphinx_nodes.index)
+    assert isinstance(section[5], sphinx_nodes.desc)
+    assert section[5].astext() == 'world\n\nGreet the world.'
 
 
 def test_nested_full(make_app, rootdir):
     srcdir = rootdir / 'nested-full'
     app = make_app('xml', srcdir=srcdir)
     app.build()
```

### Comparing `sphinx-click-5.1.0/tests/test_formatter.py` & `sphinx_click-5.2.0/tests/test_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,14 +166,65 @@
 
         A sample epilog.
         """
             ).lstrip(),
             '\n'.join(output),
         )
 
+    def test_help_argument(self):
+        """Validate a help text for arguments.
+
+        While click only provides the help attribute for options, but not for arguments,
+        it allows customization with subclasses.
+        """
+
+        class CustomArgument(click.Argument):
+            def __init__(self, *args, help=None, **kwargs):
+                super().__init__(*args, **kwargs)
+                self.help = help
+
+        @click.command()
+        @click.option('--option', help='A sample option')
+        @click.argument('ARG', help='A sample argument', cls=CustomArgument)
+        def foobar(bar):
+            """A sample command."""
+            pass
+
+        ctx = click.Context(foobar, info_name='foobar')
+        output = list(ext._format_command(ctx, nested='short'))
+
+        self.assertEqual(
+            textwrap.dedent(
+                """
+        A sample command.
+
+        .. program:: foobar
+        .. code-block:: shell
+
+            foobar [OPTIONS] ARG
+
+        .. rubric:: Options
+
+        .. option:: --option <option>
+
+            A sample option
+
+        .. rubric:: Arguments
+
+        .. option:: ARG
+
+            Required argument
+
+            A sample argument
+
+        """
+            ).lstrip(),
+            '\n'.join(output),
+        )
+
     def test_defaults(self):
         """Validate formatting of user documented defaults."""
 
         @click.command()
         @click.option('--num-param', type=int, default=42, show_default=True)
         @click.option(
             '--param',
@@ -227,14 +278,48 @@
 
             :default: ``Some default computed at runtime!``
         """
             ).lstrip(),
             '\n'.join(output),
         )
 
+    def test_show_default(self):
+        """Validate formatting of show_default via context_settings."""
+
+        @click.command(context_settings={"show_default": True})
+        @click.option('--no-set', default=0)
+        @click.option('--set-false', default=0, show_default=False)
+        def foobar():
+            """A sample command."""
+            pass
+
+        ctx = click.Context(foobar, info_name='foobar', show_default=True)
+        output = list(ext._format_command(ctx, nested='short'))
+        self.assertEqual(
+            textwrap.dedent(
+                """
+        A sample command.
+
+        .. program:: foobar
+        .. code-block:: shell
+
+            foobar [OPTIONS]
+
+        .. rubric:: Options
+
+        .. option:: --no-set <no_set>
+
+            :default: ``0``
+
+        .. option:: --set-false <set_false>
+        """
+            ).lstrip(),
+            '\n'.join(output),
+        )
+
     def test_hidden(self):
         """Validate a `click.Command` with the `hidden` flag."""
 
         @click.command(hidden=True)
         def foobar():
             """A sample command."""
             pass
```

### Comparing `sphinx-click-5.1.0/tox.ini` & `sphinx_click-5.2.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 minversion = 2.0
-envlist = py{38,39}-click{7,8,8-async},py{310,311}-click{8,8-async},style,docs
+envlist = py{38,39}-click{7,8,8-async},py{310,311,312}-click{8,8-async},style,docs
 
 [testenv]
 setenv =
     PYTHONDEVMODE = 1
     PYTHONWARNINGS = all
     PYTEST_ADDOPTS = {env:PYTEST_ADDOPTS:} --color yes
 deps =
```

