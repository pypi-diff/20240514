# Comparing `tmp/ebilab-2.5.0.tar.gz` & `tmp/ebilab-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebilab-2.5.0.tar", last modified: Fri May 10 06:32:57 2024, max compression
+gzip compressed data, was "ebilab-2.6.0.tar", last modified: Tue May 14 10:08:17 2024, max compression
```

## Comparing `ebilab-2.5.0.tar` & `ebilab-2.6.0.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-10 06:32:46.000000 ebilab-2.5.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-10 06:32:46.000000 ebilab-2.5.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-10 06:32:46.000000 ebilab-2.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 06:32:46.000000 ebilab-2.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-10 06:32:46.000000 ebilab-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 06:32:46.000000 ebilab-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 06:32:46.000000 ebilab-2.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-10 06:32:57.304190 ebilab-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 06:32:46.000000 ebilab-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.292190 ebilab-2.5.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.experiment.devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.experiment.devices.visa.rst
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.project.rst
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/ebilab.rst
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/changelog-v2.0.0-pre.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/docs/source/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/docs/source/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/api.po
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/changelog.po
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/installation.po
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/modules.po
--rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/experiment_device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-10 06:32:46.000000 ebilab-2.5.0/docs/source/tutorial/version.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/ebilab/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/ebilab/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/analysis/_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/ebilab/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.296190 ebilab-2.5.0/ebilab/data/project-template/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/ebilab/data/project-template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/input/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/original/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/original/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/output/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/data/project-template/data/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/data/plot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/ebilab.ini
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/data/project-template/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/_experiment_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/_ui_tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/experiment/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/ebilab/experiment/devices/_visa/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/A707.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/E4980.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/K34411A.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/_visa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/devices/visa.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/experiment/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-10 06:32:46.000000 ebilab-2.5.0/ebilab/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/ebilab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 06:32:57.000000 ebilab-2.5.0/ebilab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 06:32:46.000000 ebilab-2.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/sample/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/cont_r.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/multimeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/random-walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/sample/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/recipes/do-nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/recipes/random-walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 06:32:46.000000 ebilab-2.5.0/sample/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:32:57.304190 ebilab-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-10 06:32:46.000000 ebilab-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.300190 ebilab-2.5.0/tests/sample/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.288190 ebilab-2.5.0/tests/sample/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/data/input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/data/original/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/data/original/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/data/output/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/ebilab.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:57.304190 ebilab-2.5.0/tests/sample/other_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/sample/other_dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-10 06:32:46.000000 ebilab-2.5.0/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 10:08:08.000000 ebilab-2.6.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-14 10:08:08.000000 ebilab-2.6.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-14 10:08:08.000000 ebilab-2.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 10:08:08.000000 ebilab-2.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 10:08:08.000000 ebilab-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 10:08:08.000000 ebilab-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 10:08:08.000000 ebilab-2.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 10:08:17.729264 ebilab-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-14 10:08:08.000000 ebilab-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.717264 ebilab-2.6.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.717264 ebilab-2.6.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.experiment.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.experiment.devices.visa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/changelog-v2.0.0-pre.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/docs/source/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/docs/source/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.717264 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/api.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/changelog.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/installation.po
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/modules.po
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/experiment_device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/version.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/ebilab/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/ebilab/data/project-template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/input/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/original/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/output/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/data/project-template/data/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/plot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/ebilab.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10644 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/_experiment_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22272 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/_ui_tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/experiment/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/experiment/devices/_visa/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/A707.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/E4980.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/K34411A.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/visa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/ebilab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 10:08:08.000000 ebilab-2.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/cont_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/multimeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/random-walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/sample/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/do-nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/raise-error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/random-walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:08:17.729264 ebilab-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-14 10:08:08.000000 ebilab-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/tests/sample/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/data/input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/data/original/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/data/output/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/ebilab.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/other_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/other_dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/test_paths.py
```

### Comparing `ebilab-2.5.0/.gitignore` & `ebilab-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/LICENSE` & `ebilab-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/PKG-INFO` & `ebilab-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebilab
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python package for my research
 Home-page: https://ebilab.readthedocs.io/
 Author: Yusuke Ebihara
 Author-email: yusuke@ebihara.me
 Project-URL: GitHub repository, https://github.com/ebiyuu1121/ebilab
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebilab-2.5.0/README.md` & `ebilab-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/Makefile` & `ebilab-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/make.bat` & `ebilab-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/api/ebilab.analysis.rst` & `ebilab-2.6.0/docs/source/api/ebilab.analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/changelog-v2.0.0-pre.rst` & `ebilab-2.6.0/docs/source/changelog-v2.0.0-pre.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/changelog.md` & `ebilab-2.6.0/docs/source/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 更新履歴
 ========
 
+v2.6.0 (May 14, 2024)
+---------------------
+
+### Features
+
+- `ebilab.experiment` にて、実験時にPython例外が発生しても適切に処理するようにしました。
+
 v2.5.0 (May 10, 2024)
 ---------------------
 
 ### Features
 
 - `ebilab.experiment.devices` にて、いくつかのデバイスに関するメソッドを追加しました。
     - `A707` に、すべてのスイッチを開放する `open_all()` メソッドを実装しました。
```

### Comparing `ebilab-2.5.0/docs/source/conf.py` & `ebilab-2.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/index.rst` & `ebilab-2.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/installation.rst` & `ebilab-2.6.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/api.po` & `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/api.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/changelog.po` & `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/changelog.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/index.po` & `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/installation.po` & `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/modules.po` & `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/modules.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/locale/en/LC_MESSAGES/tutorial.po` & `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/tutorial.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/tutorial/analysis.rst` & `ebilab-2.6.0/docs/source/tutorial/analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/tutorial/experiment.rst` & `ebilab-2.6.0/docs/source/tutorial/experiment.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/tutorial/experiment_device.rst` & `ebilab-2.6.0/docs/source/tutorial/experiment_device.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/docs/source/tutorial/version.rst` & `ebilab-2.6.0/docs/source/tutorial/version.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/__init__.py` & `ebilab-2.6.0/ebilab/__init__.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/_cli.py` & `ebilab-2.6.0/ebilab/_cli.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/analysis/_actions.py` & `ebilab-2.6.0/ebilab/analysis/_actions.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/analysis/_preprocess.py` & `ebilab-2.6.0/ebilab/analysis/_preprocess.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/analysis/_process.py` & `ebilab-2.6.0/ebilab/analysis/_process.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/data/project-template/.gitignore` & `ebilab-2.6.0/ebilab/data/project-template/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/experiment/_experiment_controller.py` & `ebilab-2.6.0/ebilab/experiment/_experiment_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 import matplotlib.pyplot as plt
 
 from .options import OptionField
 from ..project import get_current_project
 
 logger = getLogger(__name__)
 
+class ExperimentStoppedByUser(Exception):
+    """
+    Raised when user pressed 'stop' button
+    """
+    def __str__(self):
+        return "User has stopped the experiment"
+
 # dependencies of ExperimentController
 class ExperimentContextDelegate(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def experiment_ctx_delegate_send_row(self, row):
         raise NotImplementedError()
 
     @abc.abstractmethod
@@ -155,14 +162,17 @@
     def get_options(self) -> dict:
         raise NotImplementedError()
 
     @property
     def experiment_label(self) -> str:
         raise NotImplementedError()
 
+    def show_error(self, msg: str):
+        raise NotImplementedError()
+
 def prepare_experiments(experiments):
     for experiment in experiments:
         if isinstance(experiment, ExperimentProtocolGroup):
             prepare_experiments(experiment.protocols)
             continue
 
         if experiment.plotter_classes is None:
@@ -244,20 +254,29 @@
         self._file.write(comment_lines)
 
         header = ["t", "time"] + self._running_experiment.columns
         logger.debug("Header: " + str(header))
         self._csv_writer.writerow(header)
 
         def run():
-            self._running_experiment.steps(self._ctx)
-            logger.debug("running_experiment finished, waiting 1sec")
-            time.sleep(1)
-            self._running = False
-            self._ui.update_state("stopped")
-            logger.info("running_experiment finished")
+            try:
+                self._running_experiment.steps(self._ctx)
+            except ExperimentStoppedByUser:
+                logger.info("experiment stopped by user")
+            except Exception as e:
+                # print error info
+                self._ctx.log(f"Python error occured: {e}")
+                logger.exception("Python error occured during experiment")
+                self._ui.show_error(f"Python error occured: {e}")
+            finally:
+                logger.debug("running_experiment finished, waiting 1sec")
+                time.sleep(1)
+                self._running = False
+                self._ui.update_state("stopped")
+                logger.info("running_experiment finished")
 
         self._started_time = time.perf_counter()
         logger.debug(f"started_time: {self._started_time}")
         self._running = True
         self._experiment_thread = Thread(target=run)
         self._experiment_thread.daemon = True
         self._experiment_thread.start()
@@ -313,15 +332,15 @@
         return self._get_t()
 
     def experiment_ctx_delegate_get_options(self) -> dict:
         return self._options
 
     def experiment_ctx_delegate_loop(self) -> None:
         if not self._running:
-            sys.exit()
+            raise ExperimentStoppedByUser()
 
     # ExperimentUIDelegate
     def handle_ui_start(self, experiment: Type[ExperimentProtocol]):
         self._run(experiment)
 
     def handle_ui_stop(self):
         self._stop()
```

### Comparing `ebilab-2.5.0/ebilab/experiment/_ui_tkinter.py` & `ebilab-2.6.0/ebilab/experiment/_ui_tkinter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from logging import getLogger
 import queue
 import time
 from pathlib import Path
 from typing import List, Optional, Type, Dict
 import tkinter as tk
-from tkinter import ttk
+from tkinter import ttk, messagebox
 import tkinter.font as tkf
 
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
 from ._experiment_controller import ExperimentPlotter, IExperimentUI, ExperimentProtocol, PlotterContext, ExperimentProtocolGroup
@@ -574,7 +574,10 @@
 
     def get_options(self) -> dict:
         return self._protocol_options_pane.options
 
     @property
     def experiment_label(self) -> str:
         return self._experiment_label_var.get()
+
+    def show_error(self, msg: str):
+        messagebox.showerror("Error", msg)
```

### Comparing `ebilab-2.5.0/ebilab/experiment/devices/_visa/A707.py` & `ebilab-2.6.0/ebilab/experiment/devices/_visa/A707.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/experiment/devices/_visa/E4980.py` & `ebilab-2.6.0/ebilab/experiment/devices/_visa/E4980.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/experiment/devices/_visa/K34411A.py` & `ebilab-2.6.0/ebilab/experiment/devices/_visa/K34411A.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/experiment/devices/visa.py` & `ebilab-2.6.0/ebilab/experiment/devices/visa.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/experiment/options.py` & `ebilab-2.6.0/ebilab/experiment/options.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/icon.ico` & `ebilab-2.6.0/ebilab/icon.ico`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab/project.py` & `ebilab-2.6.0/ebilab/project.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/ebilab.egg-info/PKG-INFO` & `ebilab-2.6.0/ebilab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebilab
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python package for my research
 Home-page: https://ebilab.readthedocs.io/
 Author: Yusuke Ebihara
 Author-email: yusuke@ebihara.me
 Project-URL: GitHub repository, https://github.com/ebiyuu1121/ebilab
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebilab-2.5.0/ebilab.egg-info/SOURCES.txt` & `ebilab-2.6.0/ebilab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 sample/README.md
 sample/cont_r.py
 sample/multimeter.py
 sample/random-walk.py
 sample/voltage.py
 sample/recipes/__init__.py
 sample/recipes/do-nothing.py
+sample/recipes/raise-error.py
 sample/recipes/random-walk.py
 tests/test_paths.py
 tests/sample/ebilab.ini
 tests/sample/data/input/.gitkeep
 tests/sample/data/original/.gitkeep
 tests/sample/data/output/.gitkeep
 tests/sample/other_dir/.gitkeep
```

### Comparing `ebilab-2.5.0/sample/cont_r.py` & `ebilab-2.6.0/sample/cont_r.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/sample/random-walk.py` & `ebilab-2.6.0/sample/random-walk.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/sample/recipes/random-walk.py` & `ebilab-2.6.0/sample/recipes/random-walk.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/sample/voltage.py` & `ebilab-2.6.0/sample/voltage.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/setup.py` & `ebilab-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.5.0/tests/test_paths.py` & `ebilab-2.6.0/tests/test_paths.py`

 * *Files identical despite different names*

