# Comparing `tmp/sphinx_click-5.2.0.tar.gz` & `tmp/sphinx_click-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_click-5.2.0.tar", last modified: Tue May 14 11:44:32 2024, max compression
+gzip compressed data, was "sphinx_click-5.2.2.tar", last modified: Tue May 14 12:09:01 2024, max compression
```

## Comparing `sphinx_click-5.2.0.tar` & `sphinx_click-5.2.2.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.976758 sphinx_click-5.2.0/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      640 2018-10-03 13:49:15.000000 sphinx_click-5.2.0/.editorconfig
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/.github/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      428 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/.github/workflows/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     2537 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1116 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1355 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/AUTHORS
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     6503 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/ChangeLog
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1095 2018-01-02 16:35:12.000000 sphinx_click-5.2.0/LICENSE
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     3425 2024-05-14 11:44:32.976758 sphinx_click-5.2.0/PKG-INFO
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     2122 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/README.rst
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/docs/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       61 2018-10-03 13:49:15.000000 sphinx_click-5.2.0/docs/changelog.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1819 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/conf.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1200 2018-10-03 13:49:15.000000 sphinx_click-5.2.0/docs/contributing.rst
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/docs/examples/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      611 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/commandcollections.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      509 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/commands.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      490 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/groups.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       93 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/examples/index.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      580 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/index.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      536 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/installation.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    10068 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/docs/usage.rst
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.973758 sphinx_click-5.2.0/examples/
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/examples/commandcollections/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        0 2022-04-07 12:52:39.000000 sphinx_click-5.2.0/examples/commandcollections/__init__.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      828 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/examples/commandcollections/cli.py
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/examples/commands/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      710 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/examples/commands/cli.py
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/examples/groups/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      477 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/examples/groups/cli.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      153 2022-04-07 12:52:39.000000 sphinx_click-5.2.0/examples/setup.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      193 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/pyproject.toml
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.972758 sphinx_click-5.2.0/releasenotes/
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/releasenotes/notes/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      351 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      573 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      247 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      265 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/add-show_default-from-context-support-ab4aeffcc513502d.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       88 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       65 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       65 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/python-3.12-support-f2ed1dc438bd42ee.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      208 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/releasenotes/notes/show-typer-arg-help-text-fae802f6878fa100.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       32 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/requirements.txt
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1497 2024-05-14 11:44:32.976758 sphinx_click-5.2.0/setup.cfg
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      110 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/setup.py
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.974758 sphinx_click-5.2.0/sphinx_click/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       43 2022-04-07 12:52:39.000000 sphinx_click-5.2.0/sphinx_click/__init__.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    18823 2024-05-14 11:44:21.000000 sphinx_click-5.2.0/sphinx_click/ext.py
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/sphinx_click.egg-info/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     3425 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/PKG-INFO
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1728 2024-05-14 11:44:32.000000 sphinx_click-5.2.0/sphinx_click.egg-info/SOURCES.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        1 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/dependency_links.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        1 2018-07-13 13:58:30.000000 sphinx_click-5.2.0/sphinx_click.egg-info/not-zip-safe
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       46 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/pbr.json
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       32 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/requires.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       13 2024-05-14 11:44:31.000000 sphinx_click-5.2.0/sphinx_click.egg-info/top_level.txt
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        0 2018-01-02 16:35:12.000000 sphinx_click-5.2.0/tests/__init__.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      855 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/conftest.py
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.972758 sphinx_click-5.2.0/tests/roots/
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/roots/basics/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      160 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/basics/conf.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      445 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/basics/greet.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       54 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/basics/index.rst
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/roots/commands/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      116 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/commands/conf.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      357 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/commands/greet.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       78 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/commands/index.rst
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2024-05-14 11:44:32.975758 sphinx_click-5.2.0/tests/roots/nested-full/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      116 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/nested-full/conf.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      357 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/nested-full/greet.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       85 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/roots/nested-full/index.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     4516 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/test_extension.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    26664 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tests/test_formatter.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      785 2024-04-05 10:10:43.000000 sphinx_click-5.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/commandcollections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/examples/commandcollections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/commandcollections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/commandcollections/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.298283 sphinx_click-5.2.2/examples/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/commands/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.302283 sphinx_click-5.2.2/examples/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/groups/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/examples/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.294283 sphinx_click-5.2.2/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.302283 sphinx_click-5.2.2/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-auto_envvar_prefix-support-a08e68aba792ee26.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-mock-modules-support-d4663c3265eeba5e.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/add-show_default-from-context-support-ab4aeffcc513502d.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/drop-python-3-7-support-3d3cab951fc6ae82.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/python-3.11-support-64013e70ae9926f4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/python-3.12-support-f2ed1dc438bd42ee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/releasenotes/notes/show-typer-arg-help-text-fae802f6878fa100.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.302283 sphinx_click-5.2.2/sphinx_click/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/sphinx_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18813 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/sphinx_click/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/sphinx_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 12:09:01.000000 sphinx_click-5.2.2/sphinx_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.294283 sphinx_click-5.2.2/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/roots/basics/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/basics/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/basics/greet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/basics/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/roots/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/commands/greet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/commands/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:01.306283 sphinx_click-5.2.2/tests/roots/nested-full/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/nested-full/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/nested-full/greet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/roots/nested-full/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-14 12:08:56.000000 sphinx_click-5.2.2/tox.ini
```

### Comparing `sphinx_click-5.2.0/.editorconfig` & `sphinx_click-5.2.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/.github/workflows/ci.yaml` & `sphinx_click-5.2.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/.pre-commit-config.yaml` & `sphinx_click-5.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/AUTHORS` & `sphinx_click-5.2.2/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Ahmed Masud <ahmed.masud@trustifier.com>
 AlexTereshenkov <50622389+AlexTereshenkov@users.noreply.github.com>
 Andreas Eisenbarth <andreas.eisenbarth@embl.de>
 Andy Wegner <andy@andrewwegner.com>
 Arie Bovenberg <a.c.bovenberg@gmail.com>
 Giel van Schijndel <giel@mortis.eu>
 Giel van Schijndel <me@mortis.eu>
+Hood Chatham <roberthoodchatham@gmail.com>
 Hugo Osvaldo Barrera <hugo@barrera.io>
 James Ennis <james.ennis@codethink.com>
 Jared Dillard <jared.dillard+github@gmail.com>
 JeremyB <jeremybillheimer@gmail.com>
 Jiri Kuncar <jiri.kuncar@gmail.com>
 José Sánchez-Gallego <gallegoj@uw.edu>
 Kevin Deldycke <kevin@deldycke.com>
```

### Comparing `sphinx_click-5.2.0/ChangeLog` & `sphinx_click-5.2.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+5.2.2
+-----
+
+* FIX If the \`help\` of an argument is \`None\`, don't fail
+* Add defusedxml to tox deps
+* Add defusedxml as test requirement
+* typing: Remove unused ignore
+* Add readthedocs config file
+
 5.2.0
 -----
 
 * Fix show\_default with context\_settings
 * tests: Add tests for 'commands' option
 * Add support, testing for Python 3.12
 * Add release note for typer arg help text feature
```

### Comparing `sphinx_click-5.2.0/LICENSE` & `sphinx_click-5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/PKG-INFO` & `sphinx_click-5.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-click
-Version: 5.2.0
+Version: 5.2.2
 Summary: Sphinx extension that automatically documents click applications
 Home-page: https://github.com/click-contrib/sphinx-click
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/click-contrib/sphinx-click/issues
 Project-URL: Documentation, https://sphinx-click.readthedocs.io/en/latest
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
-License-File: AUTHORS
 Requires-Dist: sphinx>=2.0
 Requires-Dist: click>=7.0
 Requires-Dist: docutils
 
 ============
 sphinx-click
 ============
```

### Comparing `sphinx_click-5.2.0/README.rst` & `sphinx_click-5.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/docs/conf.py` & `sphinx_click-5.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/docs/contributing.rst` & `sphinx_click-5.2.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/docs/examples/commandcollections.rst` & `sphinx_click-5.2.2/docs/examples/commandcollections.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/docs/index.rst` & `sphinx_click-5.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/docs/installation.rst` & `sphinx_click-5.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/docs/usage.rst` & `sphinx_click-5.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/examples/commandcollections/cli.py` & `sphinx_click-5.2.2/examples/commandcollections/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/examples/commands/cli.py` & `sphinx_click-5.2.2/examples/commands/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml` & `sphinx_click-5.2.2/releasenotes/notes/add-event-support-e55edb86d86d1082.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/setup.cfg` & `sphinx_click-5.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/sphinx_click/ext.py` & `sphinx_click-5.2.2/sphinx_click/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,17 +214,18 @@
     yield ''
     yield _indent(
         '{} argument{}'.format(
             'Required' if arg.required else 'Optional', '(s)' if arg.nargs != 1 else ''
         )
     )
     # Subclasses of click.Argument may add a `help` attribute (like typer.main.TyperArgument)
-    if hasattr(arg, 'help'):
+    help = getattr(arg, 'help', None)
+    if help:
         yield ''
-        help_string = ANSI_ESC_SEQ_RE.sub('', getattr(arg, 'help'))
+        help_string = ANSI_ESC_SEQ_RE.sub('', help)
         for line in _format_help(help_string):
             yield _indent(line)
 
 
 @_process_lines("sphinx-click-process-arguments")
 def _format_arguments(ctx: click.Context) -> ty.Generator[str, None, None]:
     """Format all `click.Argument` for a `click.Command`."""
@@ -407,15 +408,15 @@
 
 def nested(argument: ty.Optional[str]) -> NestedT:
     values = (NESTED_FULL, NESTED_SHORT, NESTED_NONE, None)
 
     if argument not in values:
         raise ValueError(
             "%s is not a valid value for ':nested:'; allowed values: %s"
-            % directives.format_values(values)  # type: ignore
+            % directives.format_values(values)
         )
 
     return ty.cast(NestedT, argument)
 
 
 class ClickDirective(rst.Directive):
     has_content = False
```

### Comparing `sphinx_click-5.2.0/sphinx_click.egg-info/PKG-INFO` & `sphinx_click-5.2.2/sphinx_click.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-click
-Version: 5.2.0
+Version: 5.2.2
 Summary: Sphinx extension that automatically documents click applications
 Home-page: https://github.com/click-contrib/sphinx-click
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/click-contrib/sphinx-click/issues
 Project-URL: Documentation, https://sphinx-click.readthedocs.io/en/latest
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
-License-File: AUTHORS
 Requires-Dist: sphinx>=2.0
 Requires-Dist: click>=7.0
 Requires-Dist: docutils
 
 ============
 sphinx-click
 ============
```

### Comparing `sphinx_click-5.2.0/sphinx_click.egg-info/SOURCES.txt` & `sphinx_click-5.2.2/sphinx_click.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .editorconfig
 .pre-commit-config.yaml
+.readthedocs.yaml
 AUTHORS
 ChangeLog
 LICENSE
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
```

### Comparing `sphinx_click-5.2.0/tests/conftest.py` & `sphinx_click-5.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/tests/test_extension.py` & `sphinx_click-5.2.2/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `sphinx_click-5.2.0/tests/test_formatter.py` & `sphinx_click-5.2.2/tests/test_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
             def __init__(self, *args, help=None, **kwargs):
                 super().__init__(*args, **kwargs)
                 self.help = help
 
         @click.command()
         @click.option('--option', help='A sample option')
         @click.argument('ARG', help='A sample argument', cls=CustomArgument)
+        @click.argument('ARG_NO_HELP', cls=CustomArgument)
         def foobar(bar):
             """A sample command."""
             pass
 
         ctx = click.Context(foobar, info_name='foobar')
         output = list(ext._format_command(ctx, nested='short'))
 
@@ -196,15 +197,15 @@
             textwrap.dedent(
                 """
         A sample command.
 
         .. program:: foobar
         .. code-block:: shell
 
-            foobar [OPTIONS] ARG
+            foobar [OPTIONS] ARG ARG_NO_HELP
 
         .. rubric:: Options
 
         .. option:: --option <option>
 
             A sample option
 
@@ -212,14 +213,18 @@
 
         .. option:: ARG
 
             Required argument
 
             A sample argument
 
+
+        .. option:: ARG_NO_HELP
+
+            Required argument
         """
             ).lstrip(),
             '\n'.join(output),
         )
 
     def test_defaults(self):
         """Validate formatting of user documented defaults."""
```

### Comparing `sphinx_click-5.2.0/tox.ini` & `sphinx_click-5.2.2/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,19 @@
     PYTHONDEVMODE = 1
     PYTHONWARNINGS = all
     PYTEST_ADDOPTS = {env:PYTEST_ADDOPTS:} --color yes
 deps =
     pytest
     pytest-cov
     coverage
+    defusedxml
     click7: click>=7.0,<8.0
     click8: click>=8.0,<9.0
     click8-async: asyncclick>=8.0,<9.0
+    defusedxml
 commands =
     python -m pytest --cov {toxinidir}/sphinx_click {posargs}
 pip_pre =
     pre: true
 
 [testenv:coverage]
 commands =
```

