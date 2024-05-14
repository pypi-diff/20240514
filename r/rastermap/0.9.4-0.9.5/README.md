# Comparing `tmp/rastermap-0.9.4.tar.gz` & `tmp/rastermap-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastermap-0.9.4.tar", last modified: Sat Aug  5 17:21:59 2023, max compression
+gzip compressed data, was "rastermap-0.9.5.tar", last modified: Tue May 14 17:53:29 2024, max compression
```

## Comparing `rastermap-0.9.4.tar` & `rastermap-0.9.5.tar`

### file list

```diff
@@ -1,66 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.937479 rastermap-0.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.941479 rastermap-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-05 17:21:48.000000 rastermap-0.9.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-05 17:21:48.000000 rastermap-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-05 17:21:48.000000 rastermap-0.9.4/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-05 17:21:48.000000 rastermap-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-08-05 17:21:59.945479 rastermap-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17350 2023-08-05 17:21:48.000000 rastermap-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-05 17:21:48.000000 rastermap-0.9.4/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-05 17:21:48.000000 rastermap-0.9.4/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.941479 rastermap-0.9.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_largescale.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_singleneurons.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_widefield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/rastermap_zebrafish.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-08-05 17:21:48.000000 rastermap-0.9.4/notebooks/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.941479 rastermap-0.9.4/paper/
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig3.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig4.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig5.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig5.py
--rw-r--r--   0 runner    (1001) docker     (123)    14408 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/fig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/other_upsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/qrdqn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-08-05 17:21:48.000000 rastermap-0.9.4/paper/splitting.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/rastermap/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/rastermap/gui/
--rw-r--r--   0 runner    (1001) docker     (123)   118393 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/guiparts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/gui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-08-05 17:21:48.000000 rastermap-0.9.4/rastermap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/rastermap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 17:21:59.000000 rastermap-0.9.4/rastermap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:21:59.945479 rastermap-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-05 17:21:48.000000 rastermap-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:21:59.945479 rastermap-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 17:21:48.000000 rastermap-0.9.4/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-05 17:21:48.000000 rastermap-0.9.4/tests/test_rastermap.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-05 17:21:48.000000 rastermap-0.9.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.391025 rastermap-0.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.379025 rastermap-0.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.383025 rastermap-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-14 17:53:20.000000 rastermap-0.9.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-14 17:53:20.000000 rastermap-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 17:53:20.000000 rastermap-0.9.5/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-14 17:53:20.000000 rastermap-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20204 2024-05-14 17:53:29.391025 rastermap-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-05-14 17:53:20.000000 rastermap-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-14 17:53:20.000000 rastermap-0.9.5/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-14 17:53:20.000000 rastermap-0.9.5/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.383025 rastermap-0.9.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    17385 2024-05-14 17:53:20.000000 rastermap-0.9.5/notebooks/rastermap_interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12301 2024-05-14 17:53:20.000000 rastermap-0.9.5/notebooks/rastermap_largescale.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-14 17:53:20.000000 rastermap-0.9.5/notebooks/rastermap_singleneurons.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-05-14 17:53:20.000000 rastermap-0.9.5/notebooks/rastermap_widefield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-14 17:53:20.000000 rastermap-0.9.5/notebooks/rastermap_zebrafish.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27221 2024-05-14 17:53:20.000000 rastermap-0.9.5/notebooks/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.387025 rastermap-0.9.5/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35906 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16334 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig6.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig7.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8525 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig8.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/fig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12314 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/other_upsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/qrdqn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27815 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/splitting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-14 17:53:20.000000 rastermap-0.9.5/paper/svca.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.387025 rastermap-0.9.5/rastermap/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.391025 rastermap-0.9.5/rastermap/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)   118393 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/gui/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28154 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/gui/guiparts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17603 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/gui/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/gui/menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7177 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/gui/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/gui/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23074 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15429 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-14 17:53:20.000000 rastermap-0.9.5/rastermap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.391025 rastermap-0.9.5/rastermap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20204 2024-05-14 17:53:29.000000 rastermap-0.9.5/rastermap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-14 17:53:29.000000 rastermap-0.9.5/rastermap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:53:29.000000 rastermap-0.9.5/rastermap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 17:53:29.000000 rastermap-0.9.5/rastermap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 17:53:29.000000 rastermap-0.9.5/rastermap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:53:29.391025 rastermap-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-14 17:53:20.000000 rastermap-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:53:29.391025 rastermap-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 17:53:20.000000 rastermap-0.9.5/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-14 17:53:20.000000 rastermap-0.9.5/tests/test_rastermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 17:53:20.000000 rastermap-0.9.5/tox.ini
```

### Comparing `rastermap-0.9.4/.github/workflows/test_and_deploy.yml` & `rastermap-0.9.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/.gitignore` & `rastermap-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/LICENSE` & `rastermap-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/PKG-INFO` & `rastermap-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 Metadata-Version: 2.1
 Name: rastermap
-Version: 0.9.4
+Version: 0.9.5
 Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
 Home-page: https://github.com/MouseLand/rastermap
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: carsen.stringer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: gui
 License-File: LICENSE
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: numba>=0.57.0
+Requires-Dist: natsort
+Requires-Dist: tqdm
+Provides-Extra: gui
+Requires-Dist: pyqtgraph>=0.11.0rc0; extra == "gui"
+Requires-Dist: pyqt6; extra == "gui"
+Requires-Dist: pyqt6.sip; extra == "gui"
+Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: superqt; extra == "gui"
 
 # Rastermap
 
 ![tests](https://github.com/mouseland/rastermap/actions/workflows/test_and_deploy.yml/badge.svg)
 [![codecov](https://codecov.io/gh/MouseLand/rastermap/branch/main/graph/badge.svg?token=9FFo4zNtYP)](https://codecov.io/gh/MouseLand/rastermap)
 [![PyPI version](https://badge.fury.io/py/rastermap.svg)](https://badge.fury.io/py/rastermap)
-[![Downloads](https://pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
-[![Downloads](https://pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
+[![Downloads](https://static.pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
+[![Downloads](https://static.pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
 [![Python version](https://img.shields.io/pypi/pyversions/rastermap)](https://pypistats.org/packages/rastermap)
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/blob/main/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
 Rastermap is a discovery algorithm for neural data. The algorithm was written by Carsen Stringer and Marius Pachitariu. For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation). If you use Rastermap in your work, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.07.25.550571v1):
 
-Stringer C., Zhong L., Syeda A., Du F., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
+Stringer C., Zhong L., Syeda A., Du F., Kesa M., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
 
 Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
-* [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
+* [rastermap_interactive.ipynb](notebooks/rastermap_interactive.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_interactive.ipynb) allows running Rastermap in an interactive way without a local installation
+* [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations. See the student/teacher versions [here](https://github.com/MouseLand/course-materials/tree/main/behavior_encoding).
 
 All demo data available [here](https://osf.io/xn4cm/).
 
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
 <img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
@@ -50,15 +62,15 @@
 
 # Installation
 
 ## Local installation (< 2 minutes)
 
 ### System requirements
 
-Linux, Windows and Mac OS are supported for running the code. For running the graphical interface you will need a Mac OS later than Yosemite. At least 8GB of RAM is recommended to run the software. 16GB-32GB may be required for larger datasets. The software has been heavily tested on Windows 10 and Ubuntu 20.04 and less well-tested on Mac OS. Please open an [issue](https://github.com/MouseLand/rastermap/issues) if you have problems with installation.
+Linux, Windows and Mac OS are supported for running the code. For running the graphical interface in Mac, you will need a Mac OS later than Yosemite. At least 8GB of RAM is recommended to run the software. 16GB-32GB may be required for larger datasets. The software has been heavily tested on Windows 10 and Ubuntu 20.04 and less well-tested on Mac OS. Please open an [issue](https://github.com/MouseLand/rastermap/issues) if you have problems with installation.
 
 ### Instructions
 
 Recommended to install an [Anaconda](https://www.anaconda.com/download/) distribution of Python -- Choose **Python 3.x** and your operating system. Note you might need to use an anaconda prompt (windows) if you did not add anaconda to the path. Open an anaconda prompt / command prompt with **python 3** in the path, then:
 
 ~~~sh
 pip install rastermap
@@ -145,20 +157,20 @@
 
 # spks is neurons by time
 spks = np.load("spks.npy").astype("float32")
 spks = zscore(spks, axis=1)
 
 # fit rastermap
 model = Rastermap(n_PCs=200, n_clusters=100, 
-                  locality=0.75, time_lag_window=5).fit(spks)
+                  locality=0.75, time_lag_window=5).fit(spks, compute_X_embedding=True)
 y = model.embedding # neurons x 1
 isort = model.isort
 
-# bin over neurons
-X_embedding = zscore(utils.bin1d(spks, bin_size=25, axis=0), axis=1)
+# visualize binning over neurons
+X_embedding = model.X_embedding
 
 # plot
 fig = plt.figure(figsize=(12,5))
 ax = fig.add_subplot(111)
 ax.imshow(X_embedding, vmin=0, vmax=1.5, cmap="gray_r", aspect="auto")
 ```
 
@@ -174,14 +186,34 @@
 
 Save an "ops.npy" file with the parameters and a "spks.npy" file with a matrix of neurons by time, and run
 
 ~~~sh
 python -m rastermap --S spks.npy --ops ops.npy
 ~~~
 
+## From MATLAB
+If you have an existing MATLAB analysis pipeline (and are using MATLAB version R2021b or newer), you can use MATLAB's Python interface to call Rastermap. First you need to tell MATLAB where your Python enviroment with Rastermap is (more details: https://www.mathworks.com/help/matlab/matlab_external/install-supported-python-implementation.html). Create or modify the "PYTHONHOME" environmental variable in your OS to point to the Rastermap environment root folder. Then in MATLAB run the following statement, modified for the specific path to your Rastermap environment pythonw executable:
+
+```
+pyenv('Version','C:\Users\admin\.conda\envs\rastermap\pythonw.exe', 'ExecutionMode', 'OutOfProcess')
+```
+Then you should be able to see your environment details in MATLAB after typing "pyenv" (the intepreter will not actually load until you try to run a Python statement). An example function to call Rastermap and return the sort order back as a MATLAB array is:
+```
+function [sortIdx] = rastermapSort(shankDataToSort)
+% wrapper to convert to numpy array, call Rastermap, and then convert back to MATLAB array
+
+ data = shankDataToSort.zScoredFiringRates; 
+ dataNdArray = py.numpy.array(data);
+ pyrun("from rastermap import Rastermap") %load interpreter, import main function
+ rmModel = pyrun("model = Rastermap(locality=0.5, time_lag_window=50).fit(spks)", "model", spks=dataNdArray);
+ sortIdx = int16(py.memoryview(rmModel.isort.data)) + 1; %back to MATLAB array, 1-indexing
+
+end
+```
+
 # Inputs
 
 Most of the time you will input to `Rastermap().fit` a matrix of neurons by time. For more details, these are all the inputs to the function:
 
 * **data** : array, shape (n_samples, n_features) (optional, default None) 
             this matrix is usually neurons/voxels by time, or None if using decomposition, 
             e.g. as in widefield imaging
```

### Comparing `rastermap-0.9.4/README.md` & `rastermap-0.9.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # Rastermap
 
 ![tests](https://github.com/mouseland/rastermap/actions/workflows/test_and_deploy.yml/badge.svg)
 [![codecov](https://codecov.io/gh/MouseLand/rastermap/branch/main/graph/badge.svg?token=9FFo4zNtYP)](https://codecov.io/gh/MouseLand/rastermap)
 [![PyPI version](https://badge.fury.io/py/rastermap.svg)](https://badge.fury.io/py/rastermap)
-[![Downloads](https://pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
-[![Downloads](https://pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
+[![Downloads](https://static.pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
+[![Downloads](https://static.pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
 [![Python version](https://img.shields.io/pypi/pyversions/rastermap)](https://pypistats.org/packages/rastermap)
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/blob/main/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
 Rastermap is a discovery algorithm for neural data. The algorithm was written by Carsen Stringer and Marius Pachitariu. For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation). If you use Rastermap in your work, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.07.25.550571v1):
 
-Stringer C., Zhong L., Syeda A., Du F., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
+Stringer C., Zhong L., Syeda A., Du F., Kesa M., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
 
 Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
-* [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
+* [rastermap_interactive.ipynb](notebooks/rastermap_interactive.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_interactive.ipynb) allows running Rastermap in an interactive way without a local installation
+* [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations. See the student/teacher versions [here](https://github.com/MouseLand/course-materials/tree/main/behavior_encoding).
 
 All demo data available [here](https://osf.io/xn4cm/).
 
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
 <img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
@@ -36,15 +37,15 @@
 
 # Installation
 
 ## Local installation (< 2 minutes)
 
 ### System requirements
 
-Linux, Windows and Mac OS are supported for running the code. For running the graphical interface you will need a Mac OS later than Yosemite. At least 8GB of RAM is recommended to run the software. 16GB-32GB may be required for larger datasets. The software has been heavily tested on Windows 10 and Ubuntu 20.04 and less well-tested on Mac OS. Please open an [issue](https://github.com/MouseLand/rastermap/issues) if you have problems with installation.
+Linux, Windows and Mac OS are supported for running the code. For running the graphical interface in Mac, you will need a Mac OS later than Yosemite. At least 8GB of RAM is recommended to run the software. 16GB-32GB may be required for larger datasets. The software has been heavily tested on Windows 10 and Ubuntu 20.04 and less well-tested on Mac OS. Please open an [issue](https://github.com/MouseLand/rastermap/issues) if you have problems with installation.
 
 ### Instructions
 
 Recommended to install an [Anaconda](https://www.anaconda.com/download/) distribution of Python -- Choose **Python 3.x** and your operating system. Note you might need to use an anaconda prompt (windows) if you did not add anaconda to the path. Open an anaconda prompt / command prompt with **python 3** in the path, then:
 
 ~~~sh
 pip install rastermap
@@ -131,20 +132,20 @@
 
 # spks is neurons by time
 spks = np.load("spks.npy").astype("float32")
 spks = zscore(spks, axis=1)
 
 # fit rastermap
 model = Rastermap(n_PCs=200, n_clusters=100, 
-                  locality=0.75, time_lag_window=5).fit(spks)
+                  locality=0.75, time_lag_window=5).fit(spks, compute_X_embedding=True)
 y = model.embedding # neurons x 1
 isort = model.isort
 
-# bin over neurons
-X_embedding = zscore(utils.bin1d(spks, bin_size=25, axis=0), axis=1)
+# visualize binning over neurons
+X_embedding = model.X_embedding
 
 # plot
 fig = plt.figure(figsize=(12,5))
 ax = fig.add_subplot(111)
 ax.imshow(X_embedding, vmin=0, vmax=1.5, cmap="gray_r", aspect="auto")
 ```
 
@@ -160,14 +161,34 @@
 
 Save an "ops.npy" file with the parameters and a "spks.npy" file with a matrix of neurons by time, and run
 
 ~~~sh
 python -m rastermap --S spks.npy --ops ops.npy
 ~~~
 
+## From MATLAB
+If you have an existing MATLAB analysis pipeline (and are using MATLAB version R2021b or newer), you can use MATLAB's Python interface to call Rastermap. First you need to tell MATLAB where your Python enviroment with Rastermap is (more details: https://www.mathworks.com/help/matlab/matlab_external/install-supported-python-implementation.html). Create or modify the "PYTHONHOME" environmental variable in your OS to point to the Rastermap environment root folder. Then in MATLAB run the following statement, modified for the specific path to your Rastermap environment pythonw executable:
+
+```
+pyenv('Version','C:\Users\admin\.conda\envs\rastermap\pythonw.exe', 'ExecutionMode', 'OutOfProcess')
+```
+Then you should be able to see your environment details in MATLAB after typing "pyenv" (the intepreter will not actually load until you try to run a Python statement). An example function to call Rastermap and return the sort order back as a MATLAB array is:
+```
+function [sortIdx] = rastermapSort(shankDataToSort)
+% wrapper to convert to numpy array, call Rastermap, and then convert back to MATLAB array
+
+ data = shankDataToSort.zScoredFiringRates; 
+ dataNdArray = py.numpy.array(data);
+ pyrun("from rastermap import Rastermap") %load interpreter, import main function
+ rmModel = pyrun("model = Rastermap(locality=0.5, time_lag_window=50).fit(spks)", "model", spks=dataNdArray);
+ sortIdx = int16(py.memoryview(rmModel.isort.data)) + 1; %back to MATLAB array, 1-indexing
+
+end
+```
+
 # Inputs
 
 Most of the time you will input to `Rastermap().fit` a matrix of neurons by time. For more details, these are all the inputs to the function:
 
 * **data** : array, shape (n_samples, n_features) (optional, default None) 
             this matrix is usually neurons/voxels by time, or None if using decomposition, 
             e.g. as in widefield imaging
```

### Comparing `rastermap-0.9.4/conftest.py` & `rastermap-0.9.5/conftest.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/notebooks/rastermap_largescale.ipynb` & `rastermap-0.9.5/notebooks/rastermap_largescale.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/notebooks/rastermap_singleneurons.ipynb` & `rastermap-0.9.5/notebooks/rastermap_singleneurons.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/notebooks/rastermap_widefield.ipynb` & `rastermap-0.9.5/notebooks/rastermap_widefield.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/notebooks/rastermap_zebrafish.ipynb` & `rastermap-0.9.5/notebooks/rastermap_zebrafish.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/notebooks/tutorial.ipynb` & `rastermap-0.9.5/notebooks/tutorial.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999850657108722%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(6, '\\n'), (7, 'from rastermap import utils, "*

 * *            "Rastermap\\n')]}}}"}*

```diff
@@ -64,14 +64,16 @@
                 "import os # os stands for \"operating system\" and includes read/write routines etc. \n",
                 "import numpy as np # by far the most used library for everyday computation\n",
                 "from scipy import stats # here we import a whole sub-library of stats functions\n",
                 "from matplotlib import pyplot as plt # all of our plotting is done with plt\n",
                 "%matplotlib inline \n",
                 "# %matplotlib notebook # if you need to zoom into a figure, this is the \"interactive\" mode of IPython\n",
                 "\n",
+                "from rastermap import utils, Rastermap\n",
+                "\n",
                 "# download the spontaneous activity recording\n",
                 "filename = utils.download_data(data_type=\"spont2\")\n",
                 "\n",
                 "# load the neural data and the processed behavioral data\n",
                 "dat = np.load(filename)\n",
                 "spks, U, sv, V = dat[\"spks\"], dat[\"U\"], dat[\"sv\"], dat[\"V\"]\n",
                 "xpos, ypos = dat[\"xpos\"], dat[\"ypos\"]\n",
```

### Comparing `rastermap-0.9.4/paper/fig1.ipynb` & `rastermap-0.9.5/paper/fig8.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9029988344988346%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(1, 'import matplotlib.pyplot as plt\\n'), (3, 'from "*

 * *            "scipy.stats import zscore \\n'), (5, 'from rastermap import Rastermap, utils\\n'), "*

 * *            "(7, '# path to paper code\\n'), (8, 'sys.path.insert(0, "*

 * *            '"/github/rastermap/paper")\\n\'), (9, \'import simulations, metrics, fig8\\n\'), (10, '*

 * *            "'from loaders import load_visual_data, load_alexnet_data\\n'), (13, '\\n'), (14, "*

 * *            '\'os.makedirs(os.path.join(root, "simula […]*

```diff
@@ -2,225 +2,228 @@
     "cells": [
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import matplotlib.pyplot as plt\n",
-                "\n",
                 "import numpy as np\n",
-                "from scipy.ndimage import gaussian_filter1d\n",
-                "from rastermap.svd import SVD\n",
+                "import matplotlib.pyplot as plt\n",
                 "import sys, os\n",
-                "from rastermap import Rastermap\n",
-                "from scipy.stats import zscore\n",
-                "from rastermap.utils import bin1d\n",
+                "from scipy.stats import zscore \n",
                 "\n",
+                "from rastermap import Rastermap, utils\n",
                 "\n",
-                "sys.path.insert(0, '/github/rastermap/paper/')\n",
-                "import metrics, simulations, fig1\n",
+                "# path to paper code\n",
+                "sys.path.insert(0, \"/github/rastermap/paper\")\n",
+                "import simulations, metrics, fig8\n",
+                "from loaders import load_visual_data, load_alexnet_data\n",
                 "\n",
                 "root = \"/media/carsen/ssd2/rastermap_paper/\"\n",
-                "os.makedirs(os.path.join(root, \"simulations/\"), exist_ok=True)\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### make simulations"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "\n",
-                "n_per_module = 1000\n",
-                "for random_state in range(0, 10):\n",
-                "    out = simulations.make_full_simulation(n_per_module=n_per_module, random_state=random_state)\n",
-                "    spks, xi_all, stim_times_all, psth, psth_spont, iperm = out\n",
-                "    np.savez(os.path.join(root, \"simulations/\", f\"sim_{random_state}.npz\"), \n",
-                "                spks=spks, xi_all=xi_all, \n",
-                "                stim_times_all=np.array(stim_times_all, dtype=object), \n",
-                "                psth=psth, psth_spont=psth_spont, iperm=iperm)\n",
-                "\n"
+                "os.makedirs(os.path.join(root, \"simulations/\"), exist_ok=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### run embedding algorithms and benchmark performance"
+                "### 2D simulations"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "imp.reload(simulations)\n",
-                "simulations.embedding_performance(root, save=True)"
+                "\n",
+                "filename = os.path.join(root, \"simulations\", \"sim2D.npz\")\n",
+                "if not os.path.exists(filename):\n",
+                "    # create simulated data with intrinsic dimensionality of 2\n",
+                "    simulations.make_2D_simulation(filename)\n",
+                "\n",
+                "dat = np.load(filename)\n",
+                "spks = dat[\"spks\"]\n",
+                "xi = dat[\"xi\"]\n",
+                "\n",
+                "### run algorithms\n",
+                "model = Rastermap(n_clusters=100, n_splits=0, n_PCs=400).fit(spks, normalize=False)\n",
+                "isort0 = model.isort \n",
+                "\n",
+                "model = Rastermap(n_clusters=100, n_splits=3, n_PCs=400).fit(spks, normalize=False)\n",
+                "isort_split = model.isort \n",
+                "X_embedding = model.X_embedding\n",
+                "\n",
+                "perplexities = [[10, 100], [10], [30], [100], [300]]\n",
+                "isorts_tsne = []\n",
+                "for i, perplexity in enumerate(perplexities):\n",
+                "    print(perplexity)\n",
+                "    y_tsne = metrics.run_TSNE(model.Usv, perplexities=perplexity, verbose=False)\n",
+                "    if i==0:\n",
+                "        isort_tsne = y_tsne[:,0].argsort()\n",
+                "    isorts_tsne.append(y_tsne[:,0].argsort())\n",
+                "\n",
+                "isorts = [isort0, isort_split, *isorts_tsne]\n",
+                "\n",
+                "### benchmark\n",
+                "knn_score, knn, rhos = simulations.benchmark_2D(xi, isorts)\n",
+                "        \n",
+                "np.savez(os.path.join(root, \"simulations\", \"sim2D_results.npz\"),\n",
+                "         X_embedding=X_embedding, isorts=np.array(isorts), \n",
+                "         knn_score=knn_score, knn=knn, rhos=rhos, \n",
+                "         xi=xi)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### make figure"
+                "### visual cortex data\n",
+                "\n",
+                "(this data will be shared upon publication)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# root path has folder \"simulations\" with saved results\n",
-                "# will save figures to \"figures\" folder\n",
-                "os.makedirs(os.path.join(root, \"figures/\"), exist_ok=True)\n",
-                "fig1.fig1(root, save_figure=True)   "
+                "filename = os.path.join(root, \"data/\", \"TX61_3x.npz\")\n",
+                "stim_filename = os.path.join(root, \"data/\", \"text5k_3x.mat\")\n",
+                "\n",
+                "out = load_visual_data(filename, stim_filename)\n",
+                "spks, istim, stim_times, xpos, ypos, run, ex_stim, img_pca, img_U, Ly, Lx = out\n",
+                "\n",
+                "# run rastermap \n",
+                "# neuron bin in rastermap\n",
+                "n_neurons = spks.shape[0]\n",
+                "n_bins = 500\n",
+                "bin_size = n_neurons // n_bins\n",
+                "model = Rastermap(n_clusters=100, n_splits=3, nc_splits=25, locality=0., bin_size=bin_size,\n",
+                "                             n_PCs=400, mean_time=True).fit(spks, compute_X_embedding=True)\n",
+                "isort = model.isort\n",
+                "\n",
+                "X_embedding = model.X_embedding\n",
+                "\n",
+                "# compute stimulus responses sresp and average over the three repeats\n",
+                "iss = np.zeros((3,5000), \"int\")\n",
+                "for j in range(5000):\n",
+                "    iss[:,j] = (istim==j).nonzero()[0][:3]\n",
+                "sresp = spks[:, stim_times]\n",
+                "sresp = sresp[:, iss].transpose((1,0,2))\n",
+                "snr_neurons = (zscore(sresp[0], axis=-1) * zscore(sresp[1], axis=-1)).mean(axis=1)\n",
+                "\n",
+                "# bin rastermap by neurons\n",
+                "n_stim = sresp.shape[-1]\n",
+                "n_bins = 500\n",
+                "bin_size = n_neurons // n_bins\n",
+                "x = sresp[:, isort[:(n_neurons // bin_size) * bin_size]]\n",
+                "x = x.reshape(3, -1, bin_size, n_stim).mean(axis=2)\n",
+                "n_bins = x.shape[1]\n",
+                "snr = (zscore(x[0], axis=-1) * zscore(x[1], axis=-1)).mean(axis=-1)\n",
+                "\n",
+                "isort2 = []\n",
+                "\n",
+                "# mean over 3 repeats\n",
+                "sresp = sresp.mean(axis=0)\n",
+                "sresp = zscore(sresp, axis=1)\n",
+                "x = x.mean(axis=0)\n",
+                "x = zscore(x, axis=-1)\n",
+                "\n",
+                "# ridge regression from 200 image PCs to 1000 rastermap components\n",
+                "itrain = np.arange(5000)%5>0\n",
+                "itest  = ~itrain\n",
+                "\n",
+                "# ridge regression on training data with regularizer of 1e4\n",
+                "imgTimg = (img_pca[itrain].T @ img_pca[itrain])/itrain.sum()\n",
+                "imgTx   = (img_pca[itrain].T @ x[:, itrain].T)/itrain.sum()\n",
+                "B       = np.linalg.solve(imgTimg + 1e4 * np.eye(200), imgTx)\n",
+                "\n",
+                "# reconstruct the receptive fields from the PCs\n",
+                "rfs = B.T @ img_U\n",
+                "rfs = np.reshape(rfs, (n_bins, Ly, Lx))\n",
+                "\n",
+                "# evaluate model on test data\n",
+                "rpred = img_pca[itest] @ B\n",
+                "cpred = (zscore(rpred.T, 1) * zscore(x[:,itest], 1)).mean(1)\n",
+                "\n",
+                "print(f\"mean r on test data {cpred.mean()}\")\n",
+                "\n",
+                "np.savez(os.path.join(root, \"results\", \"v1stimresp_proc.npz\"),\n",
+                "         X_embedding=X_embedding, bin_size=bin_size, isort=isort, isort2=isort2, \n",
+                "         xpos=xpos, ypos=ypos, x=x,\n",
+                "         stim_times=stim_times, run=run, ex_stim=ex_stim, rfs=rfs)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "#d = 0\n",
-                "#div_map = [[5, 42], [43, 108], [109, 136], [136, 170], [176, 200]]\n",
-                "#plt.figure(figsize=(12,3))\n",
-                "#plt.imshow(X_emb[div_map[d][0] : div_map[d][1],:8000], aspect=\"auto\", vmax=2, vmin=0)"
+                "\n",
+                "np.savez(os.path.join(root, \"results\", \"v1stimresp_proc.npz\"),\n",
+                "         X_embedding=X_embedding, bin_size=bin_size, isort=isort, isort2=np.zeros(len(isort)), \n",
+                "         xpos=xpos, ypos=ypos, x=x,\n",
+                "         stim_times=stim_times, run=run, ex_stim=ex_stim, rfs=rfs)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### supplementary analyses"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# run t-SNE with different perplexities\n",
-                "knn = np.array([10,50,100,200,500])\n",
-                "mnn_all = np.zeros((10, 7, len(knn)))\n",
-                "rho_all = np.zeros((10, 7))\n",
-                "embs_all = np.zeros((10, 7, 6000, 1))\n",
-                "scores_all = np.zeros((10, 2, 8, 5))\n",
-                "for random_state in range(10):\n",
-                "    print(random_state)\n",
-                "    dat = np.load(os.path.join(root, \"simulations\", f\"sim_{random_state}.npz\"), allow_pickle=True)\n",
-                "    spks = dat[\"spks\"]\n",
-                "    # run rastermap to get PCs\n",
-                "    model = Rastermap(n_clusters=100, n_PCs=200, locality=0.8,\n",
-                "                    time_lag_window=10, time_bin=10).fit(spks)   \n",
-                "    perplexities = []\n",
-                "    j = 0\n",
-                "    for perplexity in [10,30,60,100,200]:\n",
-                "        M = metrics.run_TSNE(model.Usv, perplexities=[perplexity])\n",
-                "        embs_all[random_state, j] = M\n",
-                "        j += 1\n",
-                "        perplexities.append([perplexity, 0])\n",
-                "        if perplexity > 60:\n",
-                "            M = metrics.run_TSNE(model.Usv, perplexities=[30, perplexity])\n",
-                "            embs_all[random_state, j] = M\n",
-                "            j += 1\n",
-                "            perplexities.append([30, perplexity])\n",
-                "    contamination_scores, triplet_scores = metrics.benchmarks(dat[\"xi_all\"], embs_all[random_state])\n",
-                "    mnn, rho = metrics.embedding_quality_gt(dat[\"xi_all\"], embs_all[random_state], knn=knn.copy())\n",
-                "    mnn_all[random_state], rho_all[random_state] = mnn, rho\n",
-                "    scores_all[random_state] = np.stack((contamination_scores, triplet_scores), \n",
-                "                                            axis=0)\n",
-                "    \n",
-                "np.savez(os.path.join(root, \"simulations\", \"sim_performance_tsne.npz\"), \n",
-                "         embs_all=embs_all, scores_all=scores_all, \n",
-                "         mnn_all=mnn_all, rho_all=rho_all, knn=knn,\n",
-                "         perplexities=perplexities)"
+                "### alexnet activations to same images\n",
+                "\n",
+                "(this data will be shared upon publication)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# run UMAP with different n_neighbors\n",
-                "knn = np.array([10,50,100,200,500])\n",
-                "n_neighbors = np.array([5, 15, 30, 60, 100, 200])\n",
-                "mnn_all = np.zeros((10, 6, len(knn)))\n",
-                "rho_all = np.zeros((10, 6))\n",
-                "embs_all = np.zeros((10, 6, 6000, 1))\n",
-                "scores_all = np.zeros((10, 2, 7, 5))\n",
-                "for random_state in range(10):\n",
-                "    print(random_state)\n",
-                "    dat = np.load(os.path.join(root, \"simulations\", f\"sim_{random_state}.npz\"), allow_pickle=True)\n",
-                "    spks = dat[\"spks\"]\n",
-                "    # run rastermap to get PCs\n",
-                "    model = Rastermap(n_clusters=100, n_PCs=200, locality=0.8,\n",
-                "                    time_lag_window=10, time_bin=10).fit(spks)   \n",
-                "    j = 0\n",
-                "    for nneigh in n_neighbors:\n",
-                "        M = metrics.run_UMAP(model.Usv, n_neighbors=nneigh)\n",
-                "        embs_all[random_state, j] = M\n",
-                "        j += 1\n",
-                "        print(j)\n",
-                "    contamination_scores, triplet_scores = metrics.benchmarks(dat[\"xi_all\"], embs_all[random_state])\n",
-                "    mnn, rho = metrics.embedding_quality_gt(dat[\"xi_all\"], embs_all[random_state], knn=knn.copy())\n",
-                "    mnn_all[random_state], rho_all[random_state] = mnn, rho\n",
-                "    scores_all[random_state] = np.stack((contamination_scores, triplet_scores), \n",
-                "                                            axis=0)\n",
-                "    \n",
-                "np.savez(os.path.join(root, \"simulations\", \"sim_performance_umap.npz\"), \n",
-                "         embs_all=embs_all, scores_all=scores_all, \n",
-                "         mnn_all=mnn_all, rho_all=rho_all, knn=knn,\n",
-                "         n_neighbors=n_neighbors)"
+                "filename = os.path.join(root, \"data\", \"ann_fvs_Grayscale(224)_TX61_3X.npz\")\n",
+                "sresp, ilayer, ipos, iconv, nmax = load_alexnet_data(filename)\n",
+                "\n",
+                "# run rastermap\n",
+                "bin_size = 24\n",
+                "model = Rastermap(n_clusters=100, n_splits=3, nc_splits=25, locality=0., bin_size=bin_size,\n",
+                "                             n_PCs=400, mean_time=True).fit(sresp, compute_X_embedding=True)\n",
+                "isort = model.isort\n",
+                "\n",
+                "isort2 = np.zeros(len(isort))\n",
+                "\n",
+                "np.savez(os.path.join(root, \"results\", \"alexnet_proc.npz\"),\n",
+                "         X_embedding=model.X_embedding, bin_size=bin_size, isort=isort, isort2=isort2,\n",
+                "         ilayer=ilayer, ipos=ipos, iconv=iconv, nmax=nmax)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# compute neighbor scores for original embeddings\n",
-                "d2 = np.load(os.path.join(root, \"simulations\", \"sim_performance.npz\"), allow_pickle=True) \n",
-                "mnn_all = np.zeros((10, 5, len(knn)))\n",
-                "rho_all = np.zeros((10, 5))\n",
-                "for random_state in range(10):\n",
-                "    dat = np.load(os.path.join(root, \"simulations\", f\"sim_{random_state}.npz\"), allow_pickle=True)\n",
-                "    embs = d2[\"embs_all\"][random_state].squeeze()\n",
-                "    mnn, rho = metrics.embedding_quality_gt(dat[\"xi_all\"], embs, knn=knn.copy())\n",
-                "    mnn_all[random_state], rho_all[random_state] = mnn, rho\n",
-                "np.savez(os.path.join(root, \"simulations\", \"sim_performance_neigh.npz\"), \n",
-                "         mnn_all=mnn_all, rho_all=rho_all, knn=knn)\n"
+                "### make figure"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fig1.suppfig_scores(root)"
+                "fig8.fig_all(root, False)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.9.16 ('rastermap')",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -228,15 +231,50 @@
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.16"
         },
-        "orig_nbformat": 4,
+        "varInspector": {
+            "cols": {
+                "lenName": 16,
+                "lenType": 16,
+                "lenVar": 40
+            },
+            "kernels_config": {
+                "python": {
+                    "delete_cmd_postfix": "",
+                    "delete_cmd_prefix": "del ",
+                    "library": "var_list.py",
+                    "varRefreshCmd": "print(var_dic_list())"
+                },
+                "r": {
+                    "delete_cmd_postfix": ") ",
+                    "delete_cmd_prefix": "rm(",
+                    "library": "var_list.r",
+                    "varRefreshCmd": "cat(var_dic_list()) "
+                }
+            },
+            "position": {
+                "height": "546px",
+                "left": "845px",
+                "right": "20px",
+                "top": "120px",
+                "width": "344px"
+            },
+            "types_to_exclude": [
+                "module",
+                "function",
+                "builtin_function_or_method",
+                "instance",
+                "_Feature"
+            ],
+            "window_display": false
+        },
         "vscode": {
             "interpreter": {
                 "hash": "998540cc2fc2836a46e99cd3ca3c37c375205941b23fd1eb4b203c48f2be758f"
             }
         }
     },
     "nbformat": 4,
```

### Comparing `rastermap-0.9.4/paper/fig1.py` & `rastermap-0.9.5/paper/fig4.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,509 +1,522 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
-import matplotlib.pyplot as plt 
 import os
-import numpy as np
-from rastermap.utils import bin1d
-from rastermap.sort import compute_BBt, compute_BBt_mask
-import metrics
 from fig_utils import *
+from matplotlib import patches
 
-alg_cols = plt.get_cmap("tab20b")(np.linspace(0,1.,20))[::4]
-alg_cols = alg_cols[[1,0,2,3]]
-alg_cols = np.concatenate((np.array([0,0,0,1])[np.newaxis,:],
-                           alg_cols), axis=0)
-alg_names = ["rastermap", "t-SNE", "UMAP", "isomap", "laplacian\neigenmaps"]
-mod_names = ["tuning", "sustained", "sequence 1", "sequence 2", "power-law"]
-
-def panels_schematic(fig, grid, il, cc_tdelay, tshifts, BBt_log, BBt_travel, 
-                     U_nodes, U_upsampled, kmeans_img):
-    dx = 0.1
-    dy = 0.1
-    xpad = 0.96 / 5
-    transl = mtransforms.ScaledTranslation(-18 / 72, 7 / 72, fig.dpi_scale_trans)
-    
-    ### schematics
-    ax_kmeans = plt.subplot(grid[0,0])
-    ax_kmeans.axis("off")
-    il = plot_label(ltr, il, ax_kmeans, transl, fs_title)
-    pos = ax_kmeans.get_position().bounds
-    x0 = pos[0]-(xpad-dx)/4
-    #print(x0)
-    ax_kmeans_img = fig.add_axes([x0+pos[2]*0.15, pos[1]+0.55*pos[3], pos[2]*0.3, pos[3]*0.3])
-    ax_crosscorr = fig.add_axes([pos[0]+0.6*pos[2], pos[1]+0.25*pos[3], pos[2]*0.3, pos[3]*0.3])
-
-    # plot kmeans illustration
-    ax_kmeans_img.imshow(kmeans_img)
-    ax_kmeans_img.set_title("k-means\nclustering")
-    ax_kmeans_img.axis("off")
-
-    # plot example crosscorr
-    c0, c1 = 5, 7
-    ax_crosscorr.plot(tshifts, cc_tdelay[c0,c1], color=[0.5,0.5,0.5], zorder=1)
-    ax_crosscorr.set_ylabel("corr")
-    ax_crosscorr.set_xlabel("time lag ($\delta$t)")
-    ax_crosscorr.set_xlim([tshifts.min(), tshifts.max()])
-    ax_crosscorr.set_title(f"cross-corr\nclusters {c0}, {c1}")
-    ix = cc_tdelay[c0,c1].argmax()
-    ax_crosscorr.scatter(tshifts[ix], cc_tdelay[c0,c1,ix], marker="*", lw=0.5, color=[1,0.5,0], s=40, zorder=2)
-    ax_crosscorr.text(tshifts[ix]+5, cc_tdelay[c0,c1,ix], "max", color=[1,0.5,0], va="center")
-    ax_crosscorr.set_ylim([-0.2,0.9])
-
-    nshow=20
-    ax = plt.subplot(grid[0,1]) 
-    il = plot_label(ltr, il, ax, transl, fs_title)
+def brain_plot(ax, x, y, cweights, cmap, theta=np.pi*0.77, subsample=5, 
+                vmin=None, vmax=None, brain_axes=True):
     pos = ax.get_position().bounds
+    xvox = x*np.cos(theta) - y*np.sin(theta)
+    yvox = x*np.sin(theta) + y*np.cos(theta)
+    im = ax.scatter(-xvox[::subsample], yvox[::subsample], 
+                cmap=cmap, c=cweights[::subsample], rasterized=True,
+                s=1, alpha=1, marker=".", vmin=vmin, vmax=vmax)
+    if brain_axes:
+        il = add_apml(ax, 210*np.ones(1), 45*np.ones(1), dx=80, dy=80, tp=10)
     ax.axis("off")
-    ax.set_title("time-lagged correlations")
+    ax.set_xlim([0, (-xvox).max()*1.1])
+    ax.set_ylim([-3*yvox.max(), 2*yvox.max()])
+    if isinstance(cmap, str):
+        cax = ax.figure.add_axes([pos[0]+pos[2]*0.3, pos[1]+pos[3]*.35, 
+                                    pos[2]*0.5, pos[3]*0.04])
+        plt.colorbar(im, cax=cax, orientation="horizontal")
+        if cmap=="viridis":
+            cax.set_xlabel("var. exp.")
+        else:
+            cax.set_xticks([-0.2,0,0.2])
+            cax.set_xticklabels(["-0.2  ", "0", "  0.2"])
+            cax.set_xlabel("diff. in \nvar. exp.")
+
+    #ax.axis("square")
+
+def panels_hippocampus(fig, grid, il, spks, pyr_cells, speed, loc2d, tcurves, isort,
+                        cc_nodes, isort2, xmin=1000, xmax=2000, bin_sec=0.2):
+    ax = plt.subplot(grid[0,:3])
     pos = ax.get_position().bounds
-    dym=0.02
-    dxm = dym
-    np.random.seed(2)
-    isort = np.random.permutation(nshow)
-    for i in range(3):
-        axi = fig.add_axes([pos[0]+(2-i)*dxm-0.1*pos[2], pos[1]+(-i)*dym+0.3*pos[3], pos[2]*0.7, pos[3]*0.7])
-        im=axi.imshow(cc_tdelay[c0:c0+nshow, c0:c0+nshow,11+(2-i)][np.ix_(isort, isort)],#[:nshow,:nshow], 
-                        vmin=-1, vmax=1, cmap="RdBu_r")
-        axi.set_yticks([])
-        axi.set_xticks([])
-        axi.spines["right"].set_visible(True)
-        axi.spines["top"].set_visible(True)
-        axi.text(1.05, -0.0, f"$\delta$t = {2-i}", transform=axi.transAxes, ha="left")
-        if i==0:
-            posi = axi.get_position().bounds
-            #divider = make_axes_locatable(ax)
-            cax = fig.add_axes([posi[0]+posi[2]+0.005, posi[1]+posi[3]*0.75, posi[2]*0.05, posi[3]*0.25])
-            plt.colorbar(im, cax)
-        elif i==2:
-            axi.text(-.15,0.5,"clusters", transform=axi.transAxes, rotation=90, va="center")
-            axi.text(0.5,-0.15,"clusters", transform=axi.transAxes, ha="center")
+    ax.set_position([pos[0], pos[1]+pos[3]*0.1, pos[2], pos[3]*0.9])
+    grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(8,5, subplot_spec=ax, 
+                                                            wspace=0.3, hspace=0.1)
+    ax.remove()
+
+    nn = spks.shape[0]
+    xr = xmax - xmin
+    padding = 0.025
+
+    ax = plt.subplot(grid1[0,:-1])
+    sp = loc2d[xmin:xmax].copy()
+    sp -= sp.min()
+    spm = sp.max()
+    sp /= spm
+    sp[:,1] += sp[:,0].mean() - sp[:,1].mean()
+    d = -0.005*xr
+    for j in range(2):
+        ax.plot(sp[:,j], color=kp_colors[j+2])
+        ax.text(0.06+j*.01, 0.9-j*0.34,"x-position" if j==0 else "y-position", 
+                transform=ax.transAxes, color=kp_colors[j+2])
+    ax.plot(d*np.ones(2), [0,1/(spm)], color="k")
+    ht=ax.text(-0.008*xr, 0.15, "1 m", ha="right")
+    ht.set_rotation(90)
+    ax.set_xlim([-0.008*xr, xr])
+    ax.axis("off")
 
-    ax = plt.subplot(grid[0,2])
+    ### title
+    ax.text(0, 1.45, "rat hippocampus ephys recording, 1.6m linear track (Grosmark & Buzsaki, 2016)", 
+                    transform=ax.transAxes, fontsize="large")
+    transl = mtransforms.ScaledTranslation(-15 / 72, 14/ 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, ax, transl, fs_title)
-    ax.set_title("matching matrix")
+
+    ax = plt.subplot(grid1[1,:-1])
+    sp = speed[xmin:xmax].copy()
+    spm = sp.max()
+    sp /= spm
+    ax.fill_between(np.arange(0, xr), sp, color=kp_colors[0])
+    d = -0.005*xr
+    ax.plot(d*np.ones(2), [0, 0.5/(spm/bin_sec)], color="k")
+    ht=ax.text(-0.008*xr, -0.15, "0.5 m/s", ha="right")
+    ht.set_rotation(90)
+    ax.set_xlim([-0.008*xr, xr])
+    ax.text(0.08, 0.75, "running speed", transform=ax.transAxes, color=kp_colors[0])
     ax.axis("off")
-    pos = ax.get_position().bounds
-    xi = np.arange(0, nshow, 1, "float32") / nshow
-    BBt_log = compute_BBt(xi, xi)
-    BBt_log = np.triu(BBt_log)
-    BBt_log /= BBt_log.sum()
-    BBt_travel = compute_BBt_mask(xi, xi)
-    BBt_travel = np.triu(BBt_travel)
-    BBt_travel /= BBt_travel.sum() 
-    vmax = 2e-2
-    for i,mat in enumerate([BBt_log, BBt_travel]):
-        axi = fig.add_axes([pos[0]+dx*0.2+i*dx*1, 
-                            pos[1]+pos[3]*0.3, pos[2]*0.5, pos[3]*0.5])
-        axi.imshow(mat[:nshow,:nshow], vmin=-vmax, vmax=vmax, cmap="RdBu_r")
-        axi.set_yticks([])
-        axi.set_xticks([])
-        axi.spines["right"].set_visible(True)
-        axi.spines["top"].set_visible(True)
-        axi.set_title(["global", "local"][i])
-        if i==0:
-            axi.text(1.07,0.5, "+",transform=axi.transAxes, fontsize=default_font+6)
-            axi.text(1.3,0.5, "w",transform=axi.transAxes, fontsize=default_font+2)
-            axi.text(-0.05,0.5, "(1-w)",transform=axi.transAxes, 
-                        fontsize=default_font+2, ha="right")
-        else:
-            axi.text(1.2,0.4, "=",transform=axi.transAxes, fontsize=default_font+6)
 
-    ax = plt.subplot(grid[0,3])
+    ax = plt.subplot(grid1[2:,:-1])
     pos = ax.get_position().bounds
-    ax.set_position([pos[0]+dx*0.2, pos[1]+pos[3]*0.3, pos[2]*0.5, pos[3]*0.5])
-    im = ax.imshow(BBt_log[:nshow, :nshow]/2 + BBt_travel[:nshow, :nshow]/2, 
-                    vmin=-vmax, vmax=vmax, cmap="RdBu_r")
-    ax.set_yticks([])
-    ax.set_xticks([])
-    ax.spines["right"].set_visible(True)
-    ax.spines["top"].set_visible(True)
-    posi = ax.get_position().bounds
-    #divider = make_axes_locatable(ax)
-    cax = fig.add_axes([posi[0]+posi[2]*1.1, posi[1]+posi[3]*0.6, posi[2]*0.07, posi[3]*0.4])
-    plt.colorbar(im, cax)
-
-    ax = plt.subplot(grid[0,4])
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    for i in range(3):
-        nshow=20
-        du = 0.4
-        p = ax.plot(np.linspace(0, len(U_upsampled[c0:c0+nshow*10,i]), 
-                                            len(U_nodes[c0:c0+nshow+1,i])), 
-                            U_nodes[c0:c0+nshow+1,i] + du*(2-i) + (i==2)*0.08, "x", 
-                            markersize=6, 
-                            color=np.ones(3)*(0.25*i),
-                            lw=4)
-        ax.plot(U_upsampled[c0*10:(c0+nshow)*10,i] + du*(2-i) + (i==2)*0.08, 
-                color=p[0].get_color(), lw=1)
-        ax.text(20*10, du*(2-i) + du*0.05 + U_nodes[c0:c0+nshow,i].max(), f"PC {i+1:d}", 
-                         color=p[0].get_color(), ha="right")
-    ax.set_ylim([-du*0.8,du*2.4])
+    xw = pos[2]*0.05
+    cax = fig.add_axes([pos[0]+pos[2]-xw, pos[1]-pos[3]*0.015, xw, pos[3]*0.025])
+    plot_raster(ax, spks[isort], xmin, xmax, nper=1, n_neurons=20, padding=padding,
+                n_sec=10, fs=1/bin_sec, label=True, cax=cax)
+
+    cax = fig.add_axes([pos[0]+pos[2]*1.01, pos[1], pos[2]*0.01, pos[3]])
+    cols = np.zeros((nn, 3))
+    cols[pyr_cells] = np.array([0,1,0])
+    cols[~pyr_cells] = np.array([0,0,1])
+    cax.imshow(cols[isort,np.newaxis], aspect="auto")
+    cax.text(1.1, 0.93, "FS", transform=cax.transAxes, color=[0,0,1])
+    cax.text(1.1, 0.75, "RS", transform=cax.transAxes, color=[0,1,0])
+    cax.set_ylim([0, (1+padding)*nn])
+    cax.invert_yaxis()
+    cax.axis("off")
+
+    ax = plt.subplot(grid1[2:, -1])
+    n_pos = tcurves.shape[1]//2
+    x = np.arange(0, n_pos)
+    dy = 2
+    xpad = n_pos/10
+    for t in range(len(tcurves)):
+        ax.plot(x, tcurves[isort[t], :n_pos]*dy + (1+padding)*nn - t, 
+                color="k", lw=0.5)
+        ax.plot(x+n_pos+xpad, tcurves[isort[t], n_pos:]*dy + (1+padding)*nn - t, 
+                color="k", lw=0.5)
+    for j in range(2):
+        xstr = "position\n(left run)" if j==0 else "position\n(right run)"
+        ax.text(n_pos/2 + j*(n_pos+xpad), -18, xstr, ha="center")
+        ax.text(j*(n_pos+xpad), -3, "0")
+        ax.text(n_pos + j*(n_pos+xpad), -3, "1.6", ha="right")
+
+    ax.set_title("single-neuron\ntuning curves", loc="center")
+    ax.set_ylim([0,nn*(1+padding)])
+    ax.set_xlim([0.05, 2*n_pos-0.05])
     ax.axis("off")
-    ax.text(0,0.1, "clusters sorted x", transform=ax.transAxes)
-    ax.text(0,0., "upsampled nodes -", transform=ax.transAxes)
-    ax.text(-0.1,0.5, "weights", rotation=90, transform=ax.transAxes, va="center")
-    ax.set_title("upsampling")
 
     return il
 
-def panels_raster(fig, grid, il, yratio, X_embs, cc_embs, div_map, mod_names, emb_cols):
-    transl = mtransforms.ScaledTranslation(-18 / 72, 7 / 72, fig.dpi_scale_trans)
-    
-    titles = [" simulated neurons sorted by rastermap", " simulated neurons sorted by t-SNE"]
-    mod_names_sort = np.array(mod_names.copy())[np.array([3, 4, 0, 2, 1])]#[2,0,3,4,1])]
-    for k in range(2):
-        ax = plt.subplot(grid[k+1,0:3])
-        pos = ax.get_position().bounds
-        ax.set_position([pos[0], pos[1], pos[2]*0.94, pos[3]])
-        pos = ax.get_position().bounds
-        if k==0:
-            il = plot_label(ltr, il, ax, transl, fs_title)
-            cax = fig.add_axes([pos[0]+pos[2]-pos[3]*0.25, pos[1]-pos[3]*0.05, pos[3]*0.25, pos[2]*0.01])
-        else:
-            cax = None
-        plot_raster(ax, X_embs[k], xmin=0, xmax=8000, label=1-k, cax=cax)
-        if cax is not None:
-            cax.set_xlabel("")
-            cax.text(-0.15,-2, "z-scored", transform=cax.transAxes, ha="right")
-        #ax.text(0.05, 1.02, titles[k], transform=ax.transAxes, ha="left", fontsize="large")
-        ax.set_title(titles[k])
-        if k==0: 
-            # create bar with colors 
-            cax = fig.add_axes([pos[0]+pos[2]*1.01, pos[1], pos[2]*0.01, pos[3]])
-            nn = X_embs[k].shape[0]
-            cax.imshow(emb_cols[:,np.newaxis], aspect="auto")
-            cax.set_ylim([0, nn*1.025])
-            cax.invert_yaxis()
-            cax.axis("off")
-
-            # create bar with ticks 
-            cax = fig.add_axes([pos[0]+pos[2]*1.03, pos[1], pos[2]*0.01, pos[3]])
-            for d in range(len(div_map)):
-                cax.plot([0,0], [div_map[d][0], div_map[d][1]], marker=0, color="k")
-                cax.text(0.08, (div_map[d][1]-div_map[d][0])/2 + div_map[d][0], 
-                         mod_names_sort[d], va="center")
-            cax.set_ylim([0, nn*1.025])
-            cax.invert_yaxis()
-            cax.axis("off")
-
-        ax = plt.subplot(grid[k+1,3])
-        pos2 = ax.get_position().bounds
-        ax.set_position([pos2[0], pos2[1], pos[3]/yratio, pos[3]])
-        vmax = 0.3
-        cc = cc_embs[k].copy()
-        im = ax.imshow(cc, vmin=-vmax, vmax=vmax, cmap="RdBu_r")
-        ax.spines["right"].set_visible(True)
-        ax.spines["top"].set_visible(True)
-        ax.set_yticks([])
-        ax.set_xticks([])
-        ax.set_ylim([0, nn*1.025])
-        posi = ax.get_position().bounds
-        if k==0:
-            ax.set_title("asymmetric similarity")
+def panels_widefield(fig, grid, il, stim_times_0, stim_times_1, 
+                    stim_times_2, stim_times_3, 
+                    stim_labels, reward_times, sn, sn_pred, sn_pred_beh, 
+                     bin_size, itest, ypos, xpos, isort, 
+                    xmin=820, xmax=1730):
+    stim_times = [stim_times_0, stim_times_1, stim_times_2, stim_times_3]
+
+    titles = ["(i) widefield imaging during a decision-making task \n      (Musall, Kaufman et al, 2019)",
+                "(ii) prediction of activity from task and behavior variables",
+                "(iii) prediction of activity from behavior variables only",
+                "(iv) difference between (ii) and (iii)"]
+
+    ax = plt.subplot(grid[:,3:])
+    pos = ax.get_position().bounds 
+    ax.set_position([pos[0], pos[1]-0.01, pos[2], pos[3]])
+    grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(4,5, subplot_spec=ax, 
+                                                            wspace=0.25, hspace=0.2)
+    ax.remove()
+
+    nn = sn.shape[0]
+    padding = 0.03
+
+    ven = 1 - (((sn[:,itest] - sn_pred)**2).mean(axis=1) / 
+                (sn**2).mean(axis=1))
 
+    ven_beh = 1 - (((sn[:,itest] - sn_pred_beh)**2).mean(axis=1) / 
+                    (sn**2).mean(axis=1))
+
+    memb = np.zeros_like(isort)
+    memb[isort] = np.arange(0, len(isort))
+    subsample = 10
+
+    ns = (len(ypos)//bin_size) * bin_size
+    ven_t = np.repeat(ven, bin_size).T.flatten()
+    ven_beh_t = np.repeat(ven_beh, bin_size).T.flatten()
+
+    ypos_sort = ypos[isort][:ns]
+    xpos_sort = xpos[isort][:ns]
+    transl = mtransforms.ScaledTranslation(-15 / 72, 22 / 72, fig.dpi_scale_trans)
+    for j in range(4):
+        ax = plt.subplot(grid1[j,0])
+        if j==0:
+            cweights=memb
+            cmap = cmap_emb
+            vmin, vmax = 0, len(isort)
+        elif j<3:
+            vmin, vmax = 0, 0.55
+            cmap = "viridis"
+            cweights = ven_t if j==1 else ven_beh_t
+        else:
+            vmin, vmax = -0.2, 0.2
+            cmap = "RdBu_r"
+            cweights = ven_t - ven_beh_t 
+        brain_plot(ax, ypos_sort if j>0 else ypos, xpos_sort if j>0 else xpos, 
+                    cweights=cweights, cmap=cmap, subsample=subsample, 
+                    vmin=vmin, vmax=vmax, brain_axes=(j==0))
+        ax.set_title(titles[j])
+        if j==0:
             il = plot_label(ltr, il, ax, transl, fs_title)
-            cax = fig.add_axes([posi[0], posi[1]-posi[3]*0.05, posi[3]*0.25, posi[2]*0.05])
-            plt.colorbar(im, cax, orientation="horizontal")
-            cax.set_xticks([-0.3,0,0.3])
-        ax.set_ylim([0, nn*1.025])
-        ax.set_xlim([0, nn*1.025])
-        ax.invert_yaxis()
-        ax.axis("off")
 
+
+    for j in range(4):
+        if j==0:
+            X = sn[:, itest]
+        elif j==1:
+            X = sn_pred
+            ve = ven
+        elif j==2:
+            X = sn_pred_beh 
+            ve = ven_beh
+        else:
+            X = sn_pred - sn_pred_beh
+            ve = ven - ven_beh
+        vmax=1.1
+        ax = plt.subplot(grid1[j,1:])
+        poss = ax.get_position().bounds
+        ax.set_position([poss[0], poss[1], poss[2]*0.9, poss[3]])
+        poss = ax.get_position().bounds
+        cax = fig.add_axes([poss[0]+poss[2]*1.06, poss[1]+0.05*poss[3], 
+                            poss[2]*0.02, 0.2*poss[3]])
+        plot_raster(ax, X, xmin, xmax, n_neurons=None, fs=30, n_sec=5,
+                    padding=padding, cax=cax, cax_orientation="vertical",
+                    cax_label="left",   vmax=vmax,
+                    symmetric=(j==3), label=(j==0))
+
+        if j < 3:
+            nn = sn.shape[0]
+            reward_color = [0,0.5,0]
+            fcolor = np.array([[0,0.5,1], 
+                            [0,1,1], 
+                            [1,0,0], 
+                            [1,0.5,0],
+                            [0.8,0.5,0.7]])
+            for k in range(len(stim_times)):
+                starts = stim_times[k] - itest[0]
+                if j==0:
+                    ax.text(1.02,0.95-k*0.1, stim_labels[k], 
+                            color=fcolor[k], transform=ax.transAxes)
+                for n in range(len(starts)-1):
+                    start = starts[n]+1
+                    width = 1.6*30
+                    # add stimulus patch
+                    ax.add_patch(
+                            patches.Rectangle(xy=(start, 0), width=width,
+                                    height=nn, facecolor=fcolor[k], 
+                                    edgecolor=None, alpha=0.2))
+                    
+            for reward_time in reward_times:
+                ax.plot([reward_time, reward_time], [0, nn],
+                            color=reward_color, lw=2)
+            if j==0:
+                ax.text(1.02,0.95-(k+1)*0.1, "reward", 
+                            color=reward_color, transform=ax.transAxes)
+
+        cax = fig.add_axes([poss[0]-poss[2]*0.04, poss[1], poss[2]*0.02, poss[3]])
+        cols = cmap_emb(np.linspace(0, 1, nn))
+        if j==0:
+            cax.imshow(cols[:,np.newaxis], aspect="auto")
+        else:
+            if j<3:
+                vmin, vmax = 0, 0.55
+                cmap = "viridis"
+            else:
+                vmin, vmax = -0.2, 0.2
+                cmap = "RdBu_r"
+            cax.imshow(ve[:,np.newaxis], cmap=cmap, vmin=vmin, vmax=vmax, aspect="auto")
+            
+        cax.set_ylim([0, (1+padding)*nn])
+        cax.invert_yaxis()
+        cax.axis("off")
+        cax.add_patch(patches.Rectangle(xy=(-0.5, 0), width=0.99, height=nn*1, 
+                                fill=False, edgecolor="k", lw=1))
     return il
 
-def panels_responses(grid, transl, il, div_map, seqcurves0, seqcurves1, tcurves, xresp, 
-                     emb_cols, mod_names):
-    mod_names_sort = np.array(mod_names.copy())[np.array([3, 4, 0, 2, 1])]
-    ax = plt.subplot(grid[1:3, 4])
-    pos = ax.get_position().bounds
-    ax.set_position([pos[0]-0.02, pos[1]+pos[3]*0.1, pos[2]+0.03, pos[3]*0.82])
-    ax.axis("off")
-    grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(2,2, subplot_spec=ax, 
-                                                        wspace=0.1, hspace=0.6)
-    ax.remove()
 
-    ids = [3, 2, 0, 4]#[0, 1, 2, 4]
-    nsp = [4, 3, 4, 4]
-    xlabels = ["position", "stim id", "position", "time (sec.)"]
-    for a in range(4):
-        ax = plt.subplot(grid1[a//2,a%2])
-        if a==0:
-            il = plot_label(ltr, il, ax, transl, fs_title)
-        dt = ids[a]
-        n_x = div_map[dt][1] - div_map[dt][0]
-        if a==0 or a==2:
-            tc = seqcurves0.copy() if a==0 else seqcurves1.copy()
-            tc = tc[div_map[dt][0] : div_map[dt][1]]
-            ax.set_xticks([0,25,50])
-        elif a==1:
-            tc = tcurves[div_map[dt][0] : div_map[dt][1]].copy()
-            ax.set_xticks(np.arange(0,16,5))
-        elif a==3:
-            tc = xresp[div_map[dt][0] : div_map[dt][1]].copy()
-            tc = bin1d(tc, 10, axis=1)
-            ax.set_xticks([0, 20])
-            ax.set_xticklabels(["0", "10"])
-        tc -= tc.min(axis=0)
-        if a < 3:
-            tc /= tc.max(axis=0)
-        for i, c in enumerate(tc[(a<3)::nsp[a]]):
-            ax.plot(c, lw=1, color=emb_cols[div_map[dt][0] + i*nsp[a] + (a<3)]);
-        ax.set_xlabel(xlabels[a])
-        ax.set_title(mod_names_sort[dt], fontsize="medium")
-        ax.set_yticks([])
-        ax.spines["left"].set_visible(False)
-        if a==0: 
-            ax.text(1., 1.3, "superneuron responses", transform=ax.transAxes, 
-                    ha="center", fontsize="large")
-    return il 
+def panels_fish(fig, grid1, il, sn, swimming, eyepos, 
+                stims, xyz, isort, isort2, cc_nodes):
+    nn = sn.shape[0]
+    nx = 3
+    ny = 6
+    nxy = nx * ny
+
+    xi = np.hstack((np.arange(5700, 6500), np.arange(7300,7860)))
+    stims = stims[xi]
+    #xmin=5600, xmax=7900
 
-def panels_embs(grid, transl, il, xi_all, embs_all, alg_cols, mod_names):
-    ax = plt.subplot(grid[3, :3])
-    pos = ax.get_position().bounds
-    ax.set_position([pos[0]-0.0, pos[1]-0.02, pos[2]-0.02, pos[3]])
+    ax = plt.subplot(grid1[0,:-1])
+    pos = ax.get_position().bounds 
     ax.remove()
-    grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(1, 6, subplot_spec=ax, 
-                                                    wspace=0.11, hspace=0.2)
-    xip = xi_all.copy()
-    embs = embs_all[0].squeeze().copy()
-    xip = metrics.emb_to_idx(xip)
-    ax = plt.subplot(grid1[0])
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    ht=ax.text(0, 3000, "ground-truth", va="center")
-    ht.set_rotation(90)
-    ax.text(0, 7000, "benchmarking embedding algorithms", fontsize="large")
-    for k in range(5):
-        ax.text(len(xip), 6000 - (1000*k + 500 + 500*(k>3)), mod_names[k], ha="right")
-        #ax.plot([0, len(xip)], (i+1) * 1000 * np.ones(2), "--", color="k")
-    #ax.axis("square")
-    ax.set_ylim([0, len(xip)])
-    ax.set_xlim([0, len(xip)])
+
+    yh = 0.09*pos[3]
+    yh2 = 0.05*pos[3]
+    ypad = 0.01*pos[3]
+    xp = 0.025*pos[2]
+    ax_neural = fig.add_axes([pos[0], pos[1]+2*yh+2*ypad, 
+                        pos[2]-xp, pos[3]-(2*yh+yh2+3*ypad)])
+    pos_neural = ax_neural.get_position().bounds
+
+    ### eyepos
+    ax = fig.add_axes([pos_neural[0], pos[1], pos_neural[2], yh])
+    eye_color = [[0,0.95,0], [0,0.5,0.]]
+    for i in range(2):
+        ax.plot(eyepos[xi,i], color=eye_color[i])
+        ax.text(320+130*i, eyepos[xi].max()*(0.8), 
+                "left" if i==0 else "right", color=eye_color[i])
+    ax.text(0, eyepos[xi].max()*0.8, "eye pos.", 
+                color="k")
+    ax.plot([0, 60], (-1+eyepos[xi].min())*np.ones(2), 
+                color="k")
+    ax.text(0, -5, "30 sec.")
+    ax.set_xlim([0, len(xi)])
     ax.axis("off")
     
-    subsample = 5
-    for k in range(5):
-        ax = plt.subplot(grid1[k+1])
-        idx = metrics.emb_to_idx(embs[k])
-        ax.scatter(5999 - idx[::subsample], 5999 - xip[::subsample], s=1, alpha=0.15, 
-                    color=alg_cols[k], rasterized=True)
-        for i in range(4):
-            ax.plot([0, len(xip)], 6000 - ((i+1) * 1000 * np.ones(2)), "--", color="k", lw=0.5)
-        ax.set_yticks([])
-        ax.set_xticks([])
-        ax.spines["right"].set_visible(True)
-        ax.spines["top"].set_visible(True)
-        ax.set_title(alg_names[k], color=alg_cols[k], fontsize="medium")
-        ax.set_ylim([0, len(xip)])
-        ax.set_xlim([0, len(xip)])
-        if k==2:
-            ax.text(0.5, -0.15, "embedding position", transform=ax.transAxes, ha="center")
+    ### swimming
+    swim_color = np.array([[0,1,1,1],
+                           [0,0,1,1],
+                           [1.0,0.0,0,1],
+                           [0.8,1.0,0,1]])
+
+    ax = fig.add_axes([pos_neural[0], pos[1] + yh + ypad, 
+                        pos_neural[2], yh])
+    for i in range(2):
+        ax.plot(swimming[xi,i], color=swim_color[i])
+        ax.text(0+320+130*i, swimming[xi].max()*(0.6), 
+                "left" if i==0 else "right", color=swim_color[i])
+    ax.text(0, swimming[xi].max()*0.6,"swimming", 
+                color="k")
+    ax.set_ylim([swimming[xi].min(), swimming[xi].max()])
+    ax.set_xlim([0, len(xi)])
+    ax.axis("off")
 
-    return il
+    ### neuron activity
+    ax_neural.imshow(sn[:, xi], vmin=0, vmax=1, 
+                  cmap="gray_r", aspect="auto")
+    ax_neural.axis("off")
+    ax = fig.add_axes([-pos_neural[2]*0.01+pos_neural[0], pos_neural[1], 
+                        0.01*pos_neural[2], pos_neural[3]])
+    ax.plot(np.ones(2), [0, 40], 
+                color="k")
+    ax.text(-2.5, 0, "2000 neurons", transform=ax.transAxes, rotation=90, ha="left")
+    ax.axis("off")
+    ax.set_ylim([0, nn])
 
-def panels_scores(grid, transl, il, scores_all, alg_cols, mod_names):
-    ts = 100 * scores_all[:,1].mean(axis=0)
-    ts_sem = 100 * scores_all[:,1].std(axis=0) / (scores_all.shape[0]-1)**0.5
-    cs = 100 * scores_all[:,0].mean(axis=0)
-    cs_sem = 100 * scores_all[:,0].std(axis=0) / (scores_all.shape[0]-1)**0.5
+    ### stims
+    ax_stim = fig.add_axes([pos_neural[0],pos_neural[1]+pos_neural[3]+ypad,
+                            pos_neural[2], yh2])
+
+    fcolor = plt.get_cmap("hsv")(np.linspace(0,1,stims.max()+1))[::-1]
+    fcolor[0] = np.array([0., 0.5, 1.0, 1.0])
+    fcolor[1] = np.array([1.0, 0.0, 1.0, 1.0])
+    fcolor[2] = np.array([1., 1., 1., 1.])
+    fcolor[8] = swim_color[2]
+    fcolor[9] = swim_color[3]
+    fcolor[10] = swim_color[1]
+    fcolor[11] = swim_color[0]
+    
+    starts = np.nonzero(np.diff(stims))
+    starts = np.append(np.array([0]), starts)
+    starts = np.append(starts, np.array([len(stims)-1]))
+    for n in range(len(starts)-1):
+        start = starts[n]+1
+        stype = stims[start]
+        if stype!=3:
+            width = starts[n+1] - start
+            width += min(0, start)
+            start = max(0, start)
+            width = min(width, len(xi) - start)
+            ax_neural.add_patch(
+                    patches.Rectangle(xy=(start, 0), width=width,
+                                height=nn, facecolor=fcolor[stype], 
+                                edgecolor=None, alpha=0.15*(stype!=2)))
+
+            if stype==11 or stype==10:
+                if stype==11:
+                    ax_stim.arrow(start+0.2*width, 0, width*0.75, 0, width=0.04, 
+                                    head_length=10, length_includes_head=True,
+                                    facecolor=fcolor[stype], edgecolor='none')
+                else:
+                    ax_stim.arrow(start+width*0.8, 0, -width*0.75, 0, width=0.04, 
+                                    head_length=10, length_includes_head=True,
+                                    facecolor=fcolor[stype], edgecolor='none')
+                pim = np.ones((12,12))
+                ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==9 or stype==8:
+                if stype==9:
+                    ax_stim.arrow(start+width*0.5, -0.06, 0, 0.13*1.2, width=8,
+                                    head_length=0.08, length_includes_head=True,
+                                    facecolor=fcolor[stype], edgecolor='none')      
+                else:
+                    ax_stim.arrow(start+width*0.5, 0.08, 0, -0.13*1.2, width=8,
+                                head_length=0.08, length_includes_head=True,
+                                facecolor=fcolor[stype], edgecolor='none')
+                pim = np.ones((12,width))
+                ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==1:
+                pim = np.ones((12,width))
+                ax_stim.text(start+width/2, -0.07, "L", fontsize="small",
+                                ha="center", va="bottom", color=fcolor[stype])
+                ax_stim.imshow(pim, extent=(start, start+width+1, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==0:
+                pim = np.ones((12,width))
+                ax_stim.text(start+width/2, -0.07, "R", fontsize="small",
+                                ha="center", va="bottom", color=fcolor[stype])
+                ax_stim.imshow(pim, extent=(start, start+width+1, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+            elif stype==2:
+                pim = np.ones((12,width))
+                ax_stim.imshow(pim, extent=(start, start+width+2, -0.1, 0.1), 
+                            aspect="auto", cmap="gray", vmin=0, vmax=1)
+
+    ax_stim.set_xlim([0, len(xi)])
+    ax_stim.axis("off")
+
+    ax_stim.text(0., 1.1, "phototactic stimuli", 
+        transform=ax_stim.transAxes, ha="left")
+    ax_stim.text(0.55, 1.1, "optomotor response stimuli", 
+        transform=ax_stim.transAxes, ha="center")
+
+    ### title
+    ax_stim.text(0, 2, "zebrafish brainwide recording (Chen, Mu, Hu, Kuan et al, 2018)", 
+                    transform=ax_stim.transAxes, fontsize="large")
+    transl = mtransforms.ScaledTranslation(-15 / 72, 14/ 72, fig.dpi_scale_trans)
+    il = plot_label(ltr, il, ax_stim, transl, fs_title)
 
-    ax = plt.subplot(grid[3,3])
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    for k in range(5):
-        ax.errorbar(np.arange(5), ts[k], ts_sem[k], lw=2,
-                    color=alg_cols[k], zorder=0 if k>0 else 5)
-    ax.plot(100 * np.ones(5) / 3., color="k", linestyle="--")
-    ax.text(0, 33, "chance", va="top")
-    ax.set_ylabel("% correct triplets")
-    ax.set_ylim([28, 83])
-    ax.set_xticks(np.arange(0, 5))
-    ax.set_xticklabels(mod_names, 
-                        rotation=30, ha="right", rotation_mode="anchor")
+    
+    colors = cmap_emb(np.linspace(0, 1, nxy))
 
-    ax = plt.subplot(grid[3,4])
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    for k in range(5):
-        ax.errorbar(np.arange(5), cs[k], cs_sem[k], lw=2, 
-                    color=alg_cols[k], zorder=0 if k>0 else 5)
-    ax.plot(100 * np.array([5./6, 5./6, 5./6, 5./6, 2./3]), color="k", linestyle="--")
-    ax.text(0, 85, "chance")
-    ax.set_ylabel("% contamination")
-    ax.set_xticks(np.arange(0, 5))
-    ax.set_xticklabels(mod_names, 
-                        rotation=30, ha="right", rotation_mode="anchor")
-    ax.set_ylim([0, 85])
+    ### colorbar
+    ax = fig.add_axes([pos_neural[2]*1.01+pos_neural[0], pos_neural[1], 
+                        0.015*pos_neural[2], pos_neural[3]])
+    ax.imshow(colors[:,np.newaxis])
+    ax.yaxis.set_label_position("right")
+    ax.yaxis.tick_right()
+    ax.spines["right"].set_visible(True)
+    ax.spines["top"].set_visible(True)
+    ax.set_yticks(np.arange(0,nx*ny+1), 
+            labels=[str(i) for i in np.arange(1, nx*ny+2)])
+    ax.set_xticks([])
+    ax.axis("tight")
+
+    ### neuron locations
+    ax = plt.subplot(grid1[0,-1])
+    grid2 = matplotlib.gridspec.GridSpecFromSubplotSpec(ny, nx, subplot_spec=ax, 
+                                                        wspace=0.25, hspace=0.1)
+    ax.remove()
+    n_neurons = len(isort)
+    snp = np.linspace(0, n_neurons, nx*ny+1).astype(int)
+    for j in range(nx):
+        for k in range(ny):
+            ax = plt.subplot(grid2[k,j])
+            # plot all neurons
+            subsample = 50
+            ax.scatter(xyz[:,1][::subsample], xyz[:,0][::subsample], s=2, alpha=1, 
+                        color=0.9*np.ones(3), rasterized=True)
+            snmin = snp[j + k*nx]
+            snmax = snp[j+1 + k*nx]
+            ix = isort[snmin : snmax]
+            subsample = 3
+            ax.scatter(xyz[ix,1][::subsample], xyz[ix,0][::subsample],
+                        s=0.5, alpha=0.3, color=colors[j+k*nx])
+            ax.axis("off")
+            ax.text(0.1,0,str(j+k*nx+1), transform=ax.transAxes, ha="right")
+            if j==0 and k==0:
+                axin = ax.inset_axes([-0.25, 0.75, 0.2, 0.2])
+                add_apml(axin, xyz[:,0], xyz[:,1])
+                axin.axis("off")
+                axin.axis("tight")
     return il
 
-def _fig1(kmeans_img, xi_all, cc_tdelay, tshifts, BBt_log, BBt_travel, 
-        seqcurves0, seqcurves1, tcurves, xresp, 
-        U_nodes, U_upsampled, X_embs, cc_embs,cc_embs_max,
-        csig, scores_all, embs_all):
+def fig4(root, save_figure=True):
     
     fig = plt.figure(figsize=(14,10))
     yratio = 14 / 10
-    grid = plt.GridSpec(4,5, figure=fig, left=0.04, right=0.98, top=0.96, bottom=0.07, 
-                        wspace = 0.35, hspace = 0.25)
-
-    
-    # divide up plot into modules
-    #div_map = [[0, 35], [35, 63], [67, 102], [106, 172], [174, 196]]
-    #mod_names = ["tuning", "sustained", "sequence 1", "sequence 2", "power-law"]
-    div_map = [[5, 42], [43, 108], [109, 136], [136, 170], [174, 199]]
-    
+    grid = plt.GridSpec(2,5, figure=fig, left=0.02, right=0.98, top=0.96, bottom=0.02, 
+                    wspace = 0.2, hspace = 0.08)
     il = 0
-    il = panels_schematic(fig, grid, il, cc_tdelay, tshifts, BBt_log, BBt_travel, 
-                         U_nodes, U_upsampled, kmeans_img)
-
-    emb_cols = plt.get_cmap("gist_ncar")(np.linspace(0.05, 0.95, X_embs[0].shape[0]))[::-1]
-    il = panels_raster(fig, grid, il, yratio, X_embs, cc_embs_max, div_map, mod_names, emb_cols)
-
-    transl = mtransforms.ScaledTranslation(-18 / 72, 30 / 72, fig.dpi_scale_trans)
-    il = panels_responses(grid, transl, il, div_map, seqcurves0, seqcurves1, tcurves, xresp, 
-                        emb_cols, mod_names)
 
-    transl = mtransforms.ScaledTranslation(-18 / 72, 26 / 72, fig.dpi_scale_trans)
-    il = panels_embs(grid, transl, il, xi_all, embs_all, alg_cols, mod_names)
-
-    transl = mtransforms.ScaledTranslation(-40 / 72, 4 / 72, fig.dpi_scale_trans)
-    panels_scores(grid, transl, il, scores_all, alg_cols, mod_names)
+    try:
+        d = np.load(os.path.join(root, "results", "hippocampus_proc.npz"))
+        il = panels_hippocampus(fig, grid, il, **d)    
+    except:
+        print("hippocampus data not processed")
 
-    return fig 
+    ax = plt.subplot(grid[1,:3])
+    grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(1,4, subplot_spec=ax, 
+                                                            wspace=0.3, hspace=0.15)
+    ax.remove()
+    try:
+        d = np.load(os.path.join(root, "results", "fish_proc.npz"))
+        il = panels_fish(fig, grid1, il, **d) 
+    except:
+        print("fish data not processed")
 
-def fig1(root, save_figure=True):
-    d1 = np.load(os.path.join(root, "simulations", "sim_results.npz"), allow_pickle=True) 
-    d2 = np.load(os.path.join(root, "simulations", "sim_performance.npz"), allow_pickle=True) 
     try:
-        kmeans_img = plt.imread(os.path.join(root, "figures", "manifold_kmeans.png"))
+        d = np.load(os.path.join(root, "results", "widefield_proc.npz"))
+        il = panels_widefield(fig, grid, il, **d)
     except:
-        kmeans_img = np.zeros((50,50))
+        print("widefield data not processed")
 
-    fig = _fig1(kmeans_img, **d1, **d2);
     if save_figure:
-        fig.savefig(os.path.join(root, "figures", "fig1.pdf"), dpi=200)
-
-            
+        fig.savefig(os.path.join(root, "figures", "fig4.pdf"), dpi=200)
 
-def panel_mnn(ax, mnn_all, knn, cols):
-    ms = 100 * mnn_all.mean(axis=0)
-    ms_sem = 100 * mnn_all.std(axis=0) / (mnn_all.shape[0]-1)**0.5
-    #il = plot_label(ltr, il, ax, transl, fs_title)
-    for k in range(len(ms)):
-        ax.errorbar(knn/2000*100, ms[k], ms_sem[k], lw=2,
-                    color=cols[k], zorder=0 if k>0 else 5)
-    ax.set_ylim([10, 65])
-    ax.set_ylabel("% neighbors preserved")
-    ax.set_xlabel("top n % of neighbors")
-
-def panels_scores_tsne_umap(fig, grid, il, transl, scores_all, mnn_all, knn, 
-                            cols, perplexities=None, n_neighbors=None, g0=0):
-    legend = ["rastermap"]
-    extra = ["", "(default)"]
-    if perplexities is not None:
-        for p in perplexities:
-            if p[1]>0:
-                legend.append(f"t-SNE $P$ = [{p[0]}, {p[1]}]")
-            else:
-                legend.append(f"t-SNE $P$ = {p[0]} {extra[p[0]==30]}")
-    elif n_neighbors is not None:
-        for nn in n_neighbors:
-            legend.append(f"UMAP $nn$ = {nn} {extra[nn==15]}")
+def suppfig_timesort(root, save_figure=True):
 
-    ax = plt.subplot(grid[0, 2+2*g0])
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    panel_mnn(ax, mnn_all, knn, cols)
-
-    ax = plt.subplot(grid[0, 3+2*g0])
-    for k, l in enumerate(legend):
-        ax.text(-0.3, 0.9-0.12*k, l, transform=ax.transAxes,
-                 ha="left", color=cols[k])
-    ax.axis("off")
-    
-    ts = 100 * scores_all[:,1].mean(axis=0)
-    ts_sem = 100 * scores_all[:,1].std(axis=0) / (scores_all.shape[0]-1)**0.5
-    ax = plt.subplot(grid[1, 2+2*g0])
-    #il = plot_label(ltr, il, ax, transl, fs_title)
-    for k in range(len(ts)-1):
-        ax.errorbar(np.arange(5), ts[k], ts_sem[k], lw=2,
-                    color=cols[k], zorder=0 if k>0 else 5)
-    ax.plot(100 * np.ones(5) / 3., color="k", linestyle="--")
-    ax.text(0, 33, "chance", va="top")
-    ax.set_ylabel("% correct triplets")
-    ax.set_ylim([28, 83])
-    ax.set_xticks(np.arange(0, 5))
-    ax.set_xticklabels(mod_names, 
-                        rotation=30, ha="right", rotation_mode="anchor")
-
-    cs = 100 * scores_all[:,0].mean(axis=0)
-    cs_sem = 100 * scores_all[:,0].std(axis=0) / (scores_all.shape[0]-1)**0.5
-    ax = plt.subplot(grid[1, 3+2*g0])
-    #il = plot_label(ltr, il, ax, transl, fs_title)
-    for k in range(len(cs)-1):
-        ax.errorbar(np.arange(5), cs[k], cs_sem[k], lw=2, 
-                    color=cols[k]   , zorder=0 if k>0 else 5)
-    ax.plot(100 * np.array([5./6, 5./6, 5./6, 5./6, 2./3]), color="k", linestyle="--")
-    ax.text(0, 85, "chance")
-    ax.set_ylabel("% contamination")
-    ax.set_ylim([0, 85])
-    ax.set_xticks(np.arange(0, 5))
-    ax.set_xticklabels(mod_names, 
-                        rotation=30, ha="right", rotation_mode="anchor")
-    return il
-        
-def suppfig_scores(root, save_figure=True):
-    tsne_cols = plt.get_cmap("Greens")(np.linspace(0.4,1,8))
-    tsne_cols = np.concatenate((np.array([0,0,0,1])[np.newaxis,:],
-                                tsne_cols), axis=0)
-    tsne_cols[2] = alg_cols[1]
-
-    umap_cols = plt.get_cmap("Blues")(np.linspace(0.3,1,8))
-    umap_cols = np.concatenate((np.array([0,0,0,1])[np.newaxis,:],
-                                umap_cols), axis=0)
-    umap_cols[2] = alg_cols[2]
-
-    d2 = np.load(os.path.join(root, "simulations", "sim_performance.npz"), allow_pickle=True) 
-    dtsne = np.load(os.path.join(root, "simulations", "sim_performance_tsne.npz"))
-    dumap = np.load(os.path.join(root, "simulations", "sim_performance_umap.npz"))
-    dneigh = np.load(os.path.join(root, "simulations", "sim_performance_neigh.npz"))
-
-    fig = plt.figure(figsize=(14,5))
-    grid = plt.GridSpec(2, 6, figure=fig, left=0.06, right=0.98, top=0.94, bottom=0.15, 
-                        wspace = 0.5, hspace = 0.4)
-    transl = mtransforms.ScaledTranslation(-45 / 72, 5 / 72, fig.dpi_scale_trans)
+    fig = plt.figure(figsize=(14,8))
+    yratio = 14 / 8
+    grid = plt.GridSpec(2,2, figure=fig, left=0.05, right=0.98, top=0.95, bottom=0.06, 
+                    wspace = 0.2, hspace = 0.25)
     il = 0
 
-    mnn_all = dneigh["mnn_all"]
-    knn = dneigh["knn"]
-    ax = plt.subplot(grid[0, 0])
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    panel_mnn(ax, mnn_all, knn, alg_cols)
-
-    ax = plt.subplot(grid[0, 1])
-    for k, l in enumerate(alg_names):
-        ax.text(-0.3, 0.9-0.12*k, l, transform=ax.transAxes,
-                    ha="left", va="top", color=alg_cols[k])
-    ax.axis("off")
-
-
-    scores_rmap = d2["scores_all"][:,:,0]
-    mnn_rmap = dneigh["mnn_all"][:,0]
-    knn = dneigh["knn"]
-
-    mnn_all = dtsne["mnn_all"]
-    mnn_all = np.concatenate((mnn_rmap[:,np.newaxis], mnn_all), axis=1)
-    scores_all = dtsne["scores_all"]
-    scores_all = np.concatenate((scores_rmap[:,:,np.newaxis], scores_all), axis=2)
-    perplexities = dtsne["perplexities"]
-    il = panels_scores_tsne_umap(fig, grid, il, transl, scores_all, mnn_all, 
-                            knn, tsne_cols, perplexities=perplexities, g0=0)
-
-    mnn_all = dumap["mnn_all"]
-    mnn_all = np.concatenate((mnn_rmap[:,np.newaxis], mnn_all), axis=1)
-    scores_all = dumap["scores_all"]
-    scores_all = np.concatenate((scores_rmap[:,:,np.newaxis], scores_all), axis=2)
-    n_neighbors = dumap["n_neighbors"]
-    il = panels_scores_tsne_umap(fig, grid, il, transl, scores_all, mnn_all, 
-                            knn, umap_cols, n_neighbors=n_neighbors, g0=1)
+    titles = ["spontaneous activity", "virtual reality task", "rat hippocampus, linear track",
+                "fish wholebrain, visual stimuli"]
+    tstr = ["spont", "corridor", "hippocampus", "fish"]
+    transl = mtransforms.ScaledTranslation(-20 / 72, 10/ 72, fig.dpi_scale_trans)
+        
+    for j in range(4):
+        d = np.load(os.path.join(root, "results", f"{tstr[j]}_proc.npz"))
+        ax = plt.subplot(grid[j//2, j%2])
+        il = plot_label(ltr, il, ax, transl, fs_title)
+        if j!=2:
+            isort2 = d["isort2"]
+            sn = d["sn"]
+            sp = sn[:,isort2]
+        else:
+            isort = d["isort"]
+            isort2 = d["isort2"]
+            spks = d["spks"]
+            sp = spks[isort][:,isort2]
+
+        ax.imshow(sp, vmin=0, vmax=1.5, aspect="auto", cmap="gray_r")
+        ax.set_xlabel("time sorted")
+        ax.set_ylabel("superneurons" if j!=2 else "neurons")
+        ax.set_title(titles[j])
 
     if save_figure:
-        fig.savefig(os.path.join(root, "figures", "suppfig_scores.pdf"), dpi=200)
+        fig.savefig(os.path.join(root, "figures", "suppfig_timesort.pdf"), dpi=200)
```

### Comparing `rastermap-0.9.4/paper/fig2.ipynb` & `rastermap-0.9.5/paper/fig5.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9078125%*

 * *Differences: {"'cells'": "{1: {'source': ['## Download dataset and required packages if necessary\\n', '!pip "*

 * *            "install git+https://github.com/neurallatents/nlb_tools.git\\n', '!pip install "*

 * *            "dandi\\n', '!dandi download https://gui.dandiarchive.org/#/dandiset/000130']}, 2: "*

 * *            "{'source': ['load dataset']}, 3: {'source': ['import sys\\n', 'import numpy as "*

 * *            "np\\n', 'import pandas as pd\\n', 'import matplotlib.pyplot as plt\\n', 'from "*

 * *            "nlb_tools.nwb_interface  […]*

```diff
@@ -1,203 +1,207 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# DMFC recordings in macaque (Sohn, Narain et al 2019)\n",
+                "\n",
+                "original data-loading notebook from: https://neurallatents.github.io/datasets#dmfcrsg"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import sys, os\n",
-                "import numpy as np\n",
-                "import torch\n",
-                "from scipy.stats import zscore\n",
-                "from neuropop import nn_prediction\n",
-                "from rastermap import Rastermap, utils\n",
-                "\n",
-                "### use cuda version of torch if available\n",
-                "device = torch.device('cuda')\n",
-                "\n",
-                "# path to paper code\n",
-                "sys.path.insert(0, '/github/rastermap/paper')\n",
-                "import fig2\n",
-                "\n",
-                "# path to directory with data etc\n",
-                "### *** CHANGE THIS TO WHEREEVER YOU ARE DOWNLOADING THE DATA ***\n",
-                "root = \"/media/carsen/ssd2/rastermap_paper/\"\n",
-                "# (in this folder we have a \"data\" folder and a \"results\" folder)\n",
-                "os.makedirs(os.path.join(root, \"data\"), exist_ok=True)\n",
-                "os.makedirs(os.path.join(root, \"results\"), exist_ok=True)"
+                "## Download dataset and required packages if necessary\n",
+                "!pip install git+https://github.com/neurallatents/nlb_tools.git\n",
+                "!pip install dandi\n",
+                "!dandi download https://gui.dandiarchive.org/#/dandiset/000130"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### load spont data\n",
-                "\n",
-                "(this data will be available upon publication of the paper)\n"
+                "load dataset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "dat = np.load(os.path.join(root, \"data/\", \"spont_data.npz\"))\n",
-                "spks, U, sv, V = dat[\"spks\"], dat[\"U\"], dat[\"sv\"], dat[\"V\"]\n",
-                "xpos, ypos = dat[\"xpos\"], dat[\"ypos\"]\n",
-                "tcam, tneural = dat[\"tcam\"], dat[\"tneural\"]\n",
-                "run, beh, beh_names = dat[\"run\"], dat[\"beh\"], dat[\"beh_names\"]"
+                "import sys\n",
+                "import numpy as np\n",
+                "import pandas as pd\n",
+                "import matplotlib.pyplot as plt\n",
+                "from nlb_tools.nwb_interface import NWBDataset\n",
+                "from scipy.stats import zscore\n",
+                "\n",
+                "sys.path.insert(0, \"/github/rastermap/paper\")\n",
+                "import fig5\n",
+                "\n",
+                "# path to directory with data etc\n",
+                "### *** CHANGE THIS TO WHEREEVER YOU ARE SAVING YOUR DATA OUTPUTS ***\n",
+                "root = \"/media/carsen/ssd2/rastermap_paper/\"\n",
+                "\n",
+                "## Load dataset\n",
+                "dataset = NWBDataset(\"000130/sub-Haydn/\", \"*train\", split_heldout=False)\n",
+                "\n",
+                "# bin at 20ms\n",
+                "dataset.resample(20)\n",
+                "\n",
+                "# convert neural times from nanoseconds to seconds \n",
+                "neural_time = (dataset.data.index.to_numpy() / 1e3).astype(\"float\") / 1e6\n",
+                "\n",
+                "# convert task times from nanoseconds to seconds for valid trials\n",
+                "# (valid trials = set_time at least 3 second after start of exp and before end of exp)\n",
+                "igood = ~dataset.trial_info.ready_time.isna()\n",
+                "igood *= ~dataset.trial_info.set_time.isna()\n",
+                "igood *= ~dataset.trial_info.go_time.isna()\n",
+                "\n",
+                "ready_time = (dataset.trial_info.ready_time.to_numpy() / 1e3).astype(\"float\") / 1e6\n",
+                "set_time = (dataset.trial_info.set_time.to_numpy() / 1e3).astype(\"float\") / 1e6\n",
+                "go_time = (dataset.trial_info.go_time.to_numpy() / 1e3).astype(\"float\") / 1e6\n",
+                "\n",
+                "nt_sec = 3\n",
+                "igood *= (set_time - nt_sec) > 0\n",
+                "igood *= (set_time + nt_sec - neural_time[-1]) < 0\n",
+                "\n",
+                "ready_time = ready_time[igood]\n",
+                "set_time = set_time[igood]\n",
+                "go_time = go_time[igood]\n",
+                "is_short = dataset.trial_info.is_short.to_numpy()[igood]\n",
+                "is_eye = dataset.trial_info.is_eye.to_numpy()[igood]\n",
+                "iti = dataset.trial_info.iti.to_numpy()[igood]\n",
+                "\n",
+                "print(f\"number of trials: {len(set_time)}\")\n",
+                "\n",
+                "print(len(is_eye), len(is_short))\n",
+                "\n",
+                "# some spike timebins are NaN, replace with nearby values\n",
+                "spks = dataset.data.to_numpy().T.copy()\n",
+                "spks = spks.astype(\"float32\")\n",
+                "ibad = np.isnan(spks[0])\n",
+                "nbad = np.arange(0, spks.shape[-1])[~ibad]\n",
+                "ibad = np.nonzero(ibad)[0]\n",
+                "ireplace = np.array([nbad[np.abs(nbad - ibad[i]).argmin()] for i in range(len(ibad))])\n",
+                "spks[:, ibad] = spks[:, ireplace]\n",
+                "print(spks.shape)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### predict neural activity from behavior and run rastermap"
+                "### run rastermap"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "np.random.seed(0)\n",
-                "torch.manual_seed(0)\n",
-                "torch.cuda.manual_seed(0)\n",
-                "\n",
-                "### fit linear and non-linear model from behavior to neural activity\n",
-                "Vfit = V.copy() * sv\n",
-                "for i in range(2):\n",
-                "    if i==1:\n",
-                "        pred_model = nn_prediction.PredictionNetwork(n_in=beh.shape[-1], n_kp=22, identity=False, \n",
-                "                                                n_filt=10, n_latents=0,\n",
-                "                                n_out=Vfit.shape[-1], n_core_layers=1,\n",
-                "                                relu_wavelets=False, relu_latents=False)\n",
-                "    else:\n",
-                "        pred_model = nn_prediction.PredictionNetwork(n_in=beh.shape[-1], n_kp=22, n_out=Vfit.shape[-1], )\n",
-                "    pred_model.to(device)\n",
-                "\n",
-                "    y_pred_all, ve_all, itest = pred_model.train_model(beh, Vfit, tcam, tneural, delay=-1,\n",
-                "                                                        learning_rate=1e-3, n_iter=400,\n",
-                "                                                    device=device, verbose=True)\n",
-                "    if i==1:\n",
-                "        y_pred_nn = y_pred_all.copy()\n",
-                "\n",
-                "### run rastermap\n",
-                "model = Rastermap(n_clusters=100, \n",
-                "                    n_PCs=128, \n",
-                "                    locality=0.75,\n",
-                "                    time_lag_window=5,\n",
-                "                    ).fit(spks)\n",
-                "cc_nodes = model.cc.copy()\n",
-                "isort = model.isort\n",
-                "\n",
-                "### bin full data into superneurons\n",
-                "nbin = 200\n",
-                "sn = zscore(utils.bin1d(spks[isort], nbin, axis=0), axis=1)\n",
-                "np.random.seed(0)\n",
-                "sn_rand = zscore(utils.bin1d(spks[np.random.permutation(spks.shape[0])], nbin, axis=0), axis=1)\n",
-                "\n",
-                "# sort in time\n",
-                "model2 = Rastermap(n_clusters=100, locality=0.,\n",
-                "                    n_PCs=128).fit(sn.T)\n",
-                "isort2 = model2.isort\n",
-                "\n",
-                "### bin test data and prediction into superneurons\n",
-                "sn_test = utils.bin1d(spks[isort][:,itest.flatten()], nbin, axis=0)\n",
-                "sn_pred_test = utils.bin1d(U[isort] @ y_pred_nn.T, nbin, axis=0)\n",
-                "sn_pred_test -= sn_test.mean(axis=1, keepdims=True)\n",
-                "sn_pred_test /= sn_test.std(axis=1, keepdims=True)\n",
-                "sn_test = zscore(sn_test, axis=1)\n",
-                "cc_pred = (sn_test * zscore(sn_pred_test, axis=1)).mean(axis=1)\n",
-                "# sort and bin PCs for maxstim estimation\n",
-                "U_sn = utils.bin1d(U[isort], nbin)\n",
-                "\n",
-                "### maxstim estimation for superneurons (receptive fields)\n",
-                "np.random.seed(0)\n",
-                "torch.manual_seed(0)\n",
-                "torch.cuda.manual_seed(0)\n",
-                "ms_model = nn_prediction.MaxStimModel(pred_model)\n",
-                "ms_model.requires_grad = False\n",
-                "u = torch.from_numpy(U_sn).to(device)\n",
-                "u.requires_grad = False\n",
-                "xr = ms_model.train_batch(u, n_iter=200, learning_rate=1e-2)\n",
-                "rfs = xr.detach().cpu().numpy()\n",
-                "\n",
-                "\n",
-                "# save results\n",
-                "np.savez(os.path.join(root, \"results\", \"spont_proc.npz\"), sn_test=sn_test, \n",
-                "            sn_pred_test=sn_pred_test, itest=itest, \n",
-                "            sn=sn, sn_rand=sn_rand, isort2=isort2,\n",
-                "            rfs=rfs, isort=isort, cc_nodes=cc_nodes,\n",
-                "            xpos=xpos, ypos=ypos,\n",
-                "            tcam=tcam, tneural=tneural, \n",
-                "            run=run, beh=beh, beh_names=beh_names)\n"
+                "from rastermap import Rastermap\n",
+                "model = Rastermap(n_clusters=None, # None turns off clustering and sorts single neurons\n",
+                "                  n_PCs=48, # use fewer PCs than neurons\n",
+                "                  locality=0.5, # some locality in sorting (this is a value from 0-1)\n",
+                "                  time_lag_window=20, # use future timepoints to compute correlation\n",
+                "                  grid_upsample=0, # 0 turns off upsampling since we're using single neurons\n",
+                "                  mean_time=True,\n",
+                "                  bin_size=1,\n",
+                "                  time_bin=1\n",
+                "                ).fit(spks, compute_X_embedding=True)\n",
+                "y = model.embedding # neurons x 1\n",
+                "isort = model.isort"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### make figure"
+                "reshape spks into trials"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# root path has folder \"results\" with saved results\n",
-                "# will save figures to \"figures\" folder\n",
-                "os.makedirs(os.path.join(root, \"figures/\"), exist_ok=True)\n",
-                "fig2.fig2(root, save_figure=True)"
+                "set_idx = np.array([np.abs(neural_time - set_time[i]).argmin() for i in range(len(set_time))])\n",
+                "nt = int(nt_sec/.02)\n",
+                "print(nt)\n",
+                "set_idx = np.arange(-nt, nt+1) + set_idx[:,np.newaxis]\n",
+                "spks_trials = spks[:, set_idx].copy()\n",
+                "\n",
+                "\n",
+                "# split trials into short and long prior blocks, and by set_time bins\n",
+                "ttypes = [is_short, ~is_short]\n",
+                "ttypes = [(is_eye)*(is_short), (is_eye)*(~is_short), (~is_eye)*(is_short), (~is_eye)*(~is_short)]\n",
+                "bins = list(np.linspace(0.46, 0.85, 6))\n",
+                "bins.extend(list(np.arange(0.95, 1.3, 0.1)))\n",
+                "sr = np.digitize(set_time - ready_time, bins) - 1\n",
+                "ttypes = [sr==i for i in range(9)]\n",
+                "ttypes.insert(4, (sr==4)*(is_short))\n",
+                "ttypes[5] = (sr==4)*(~is_short)\n",
+                "rts = np.array(bins) + 0.05\n",
+                "rts = (nt - rts/0.02).astype(\"int\")\n",
+                "rts = list(rts)\n",
+                "rts.insert(4, rts[4])\n",
+                "gts = np.array([(go_time[ttypes[k]] - set_time[ttypes[k]]).mean() for k in range(len(ttypes))])\n",
+                "gts = (nt + gts/0.02).astype(\"int\")\n",
+                "\n",
+                "psths = []\n",
+                "for k in range(len(ttypes)):\n",
+                "    psths.append(spks_trials[isort][:,ttypes[k]].mean(axis=1))\n",
+                "psths = np.array(psths)\n",
+                "psths = psths.transpose(1,0,2).reshape(spks.shape[0], -1)\n",
+                "psths = zscore(psths, axis=1)\n",
+                "psths = psths.reshape(spks.shape[0], len(ttypes), -1).transpose(1,0,2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### make supp fig "
+                "### make figure"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "fig2.suppfig_random(root, save_figure=True)"
+                "os.makedirs(os.path.join(root, \"figures/\"), exist_ok=True)\n",
+                "fig5.fig5(root, psths, rts, gts, save_figure=True)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.9.16 ('rastermap')",
+            "display_name": "rastermap",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.16"
-        },
-        "orig_nbformat": 4,
-        "vscode": {
-            "interpreter": {
-                "hash": "998540cc2fc2836a46e99cd3ca3c37c375205941b23fd1eb4b203c48f2be758f"
-            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `rastermap-0.9.4/paper/fig2.py` & `rastermap-0.9.5/paper/fig3.py`

 * *Files 19% similar despite different names*

```diff
@@ -72,19 +72,20 @@
     transl = mtransforms.ScaledTranslation(-15 / 72, 38 / 72, grid.figure.dpi_scale_trans)
     il = plot_label(ltr, il, ax, transl, fs_title)
         
     dy = 300
     dx = 1.
     l = np.array([0,1,2])
     npl = len(ipl)
+    h = 4
     for i in range(npl):
         ir = ipl[i]
         rf = rfs[ir, 201-100:201+100].copy() / dx
         for k in range(rfs.shape[-1]):
-            ax.plot(np.arange(0,rf.shape[-2]) + k*dy, rf[:,k]*-1 + ir, color=kp_colors[k], lw=1)
+            ax.plot(np.arange(0,rf.shape[-2]) + k*dy, rf[:,k]*-h + ir, color=kp_colors[k], lw=1)
     ax.set_ylim([0, nn*(1+padding)])
     ax.invert_yaxis()
     ax.axis("off")
     ax.text(0.01,1.09, "behavioral receptive fields", transform=ax.transAxes, fontsize="large")
     for k in range(len(kp_colors)):
         ax.text(k/len(kp_colors),1.005,beh_names[k], color=kp_colors[k], 
                 rotation=45, transform=ax.transAxes, size="small")
@@ -125,22 +126,22 @@
     for k in range(2):
         ax = plt.subplot(grid[5*k + 1 : 5*k + 4])
         pos = ax.get_position().bounds
         ax.axis("off")
         ax.remove()
 
         # run raster
+        padding_x = 0.01
         ax = fig.add_axes([pos[0]+0.02*(k==0), pos[1]+pos[3]*(yh+0.01), pos[2], pos[3]*(1-yh-0.01)])     
         ax.fill_between(np.arange(0, xr), run[itest.flatten()][xmin:xmax], 
                         color=kp_colors[0])
-        ax.set_xlim([0, 1.008*xr])
+        ax.set_xlim([0*xr, xr*(1+padding_x*2)])
+        #ax.set_xlim([0, 1.008*xr])
         ax.set_ylim([0,1.2])
-        ax.spines["left"].set_visible(False)
-        ax.set_yticks([])
-        ax.set_xticks([])
+        ax.axis("off")
         transl = mtransforms.ScaledTranslation(-15 / 72, 12 / 72, fig.dpi_scale_trans)
         il = plot_label(ltr, il, ax, transl, fs_title)
         if k==0:
             il+=2
 
         if k==0:
             ax.text(0.75,0.8,"running speed", transform=ax.transAxes, color=kp_colors[0])
@@ -153,16 +154,17 @@
         xw = pos[2]*0.1
         if k==0:
             cax = fig.add_axes([pos[0]+0.02, pos[1]-pos[3]*0.005, xw, pos[3]*0.01])
         else: 
             cax = None
         plot_raster(ax, sn_test if k==0 else sn_pred_test, 
                     xmin=xmin, xmax=xmax, vmax=1.5, fs=3.38, 
-                    nper=200, n_neurons=5000, label=k==1, 
-                    padding=padding, padding_x=0.01, cax=cax, label_pos="right")    
+                    nper=50, n_neurons=5000, label=k==1, 
+                    padding=padding, padding_x=padding_x, 
+                    cax=cax, label_pos="right")    
         if k==0:
             cax = fig.add_axes([pos[0]+0.02-pos[2]*0.02, pos[1], pos[2]*0.01, pos[3]*yh])
             nn = sn_test.shape[0]
             cols = cmap_emb(np.linspace(0, 1, nn))
             cax.imshow(cols[:,np.newaxis], aspect="auto")
             cax.set_ylim([0, (1+padding)*nn])
             cax.invert_yaxis()
@@ -173,32 +175,34 @@
                 xy0 = (0,ir)
                 xy1 = (xr,ir)
                 con = patches.ConnectionPatch(xyA=xy0, xyB=xy1, coordsA="data", coordsB="data",
                                     axesA=ax0, axesB=ax, color=.5*np.ones(3), lw=0.5)
                 ax.add_artist(con)
     return il
             
-def _fig2(brain_img, face_img, xpos, ypos, isort, 
+def _fig3(brain_img, face_img, xpos, ypos, isort, 
             isort2, sn, cc_nodes, sn_rand,
             beh, beh_names, tcam, tneural, 
             itest, rfs, run, sn_test, sn_pred_test):
     fig = plt.figure(figsize=(14,7))
     yratio = 14 / 7
     grid = plt.GridSpec(1,9, figure=fig, left=0.02, right=0.98, top=0.94, bottom=0.07, 
                         wspace = 0.35, hspace = 0.3)
 
 
-    xmin = 185 
+    #xmin = 185 
+    xmin = 688*4
     xmax = xmin+500
     padding = 0.015
     yh = 0.94 # fraction raster vs run
 
-    npl = 15
+    npl = 18
     nn = rfs.shape[0]
-    ipl = np.linspace(npl//3, nn-npl//3, npl).astype("int")
+    ipl = np.linspace(8, nn-8, npl).astype("int")
+    print(ipl)
 
     ax = fig.add_subplot(grid[0])
     ax.axis("off")
     grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(3,1, subplot_spec=ax, 
                                                         wspace=0.2, hspace=0.5)
     ax.remove()
     il = 0
@@ -213,29 +217,26 @@
     il = panels_rfs(grid, il, yh, padding, ipl, rfs, beh_names)
         
     il-=3
     il = panels_rasters(fig, grid, il, yh, padding, ipl, sn_test, sn_pred_test, 
                         run, itest, xmin, xmax)
     return fig
 
-def fig2(root, save_figure=True):
+def fig3(root, save_figure=True):
     d = np.load(os.path.join(root, "results", "spont_proc.npz"), allow_pickle=True) 
     try:
         brain_img = plt.imread(os.path.join(root, "figures", "brain_windows.png"))
         face_img = plt.imread(os.path.join(root, "figures", "mouse_face_labeled.png"))
     except:
         brain_img = np.zeros((50,50))
         face_img = np.zeros((50,50))
 
-    fig = _fig2(brain_img, face_img, **d);
+    fig = _fig3(brain_img, face_img, **d);
     if save_figure:
-        fig.savefig(os.path.join(root, "figures", "fig2.pdf"), dpi=200)
-
-            
-
+        fig.savefig(os.path.join(root, "figures", "fig3.pdf"), dpi=200)
 
 def suppfig_random(root, save_figure=True):
     d = np.load(os.path.join(root, "results", "spont_proc.npz"), allow_pickle=True) 
     sn = d["sn"]
     sn_rand = d["sn_rand"]
     run = d["run"]
     itest = d["itest"]
@@ -245,15 +246,15 @@
     grid = plt.GridSpec(1,2, figure=fig, left=0.02, right=0.99, top=0.9, bottom=0.13, 
                         wspace = 0.15, hspace = 0.3)
     il = 0
 
     titles = ["random sorting", 
             "Rastermap sorting"]
 
-    xmin = 185 
+    xmin = 688*4
     xmax = xmin+500
     padding = 0.015
     yh = 0.94 # fraction raster vs run
     xr = xmax - xmin
 
     for k in range(2):
         ax = plt.subplot(grid[k])
@@ -284,13 +285,138 @@
         xw = pos[2]*0.1
         if k==0:
             cax = fig.add_axes([pos[0]+0.02, pos[1]-pos[3]*0.005, xw, pos[3]*0.01])
         else: 
             cax = None
         plot_raster(ax, sn_rand[:,itest.flatten()] if k==0 else sn[:, itest.flatten()], 
                     xmin=xmin, xmax=xmax, vmax=1.5, fs=3.38, label=k==0, 
-                    nper=200, n_neurons=5000,
+                    nper=50, n_neurons=5000,
                     padding=padding, padding_x=0.01, cax=cax, label_pos="right")    
-
     
     if save_figure:
         fig.savefig(os.path.join(root, "figures", "suppfig_random.pdf"))
+
+
+def suppfig_locality(root, save_figure=True):
+    d = np.load(os.path.join(root, "results", "asym_vr_spont.npz"), allow_pickle=True) 
+    ccs_vr = d["ccs_vr"]
+    ccs_spont = d["ccs_spont"]
+    localities = d["localities"]
+    scores_vr = d["scores_vr"]
+    scores_spont = d["scores_spont"]
+
+    fig = plt.figure(figsize=(14,6))
+    grid = plt.GridSpec(2,5, figure=fig, left=0.01, right=0.99, top=0.86, bottom=0.01, 
+                                wspace = 0.2, hspace = 0.45)
+    transl = mtransforms.ScaledTranslation(-15 / 72, 38 / 72, fig.dpi_scale_trans)
+    il = 0
+
+    xmin = 185 
+    xmax = xmin+500
+    xr = xmax - xmin
+    yh = 0.9
+    padding_x = 0.008
+    nbin = 200
+
+    vmax = 0.75
+    tstrs = ["neural activity in virtual reality", "spontaneous neural activity"]
+    for j in range(2):
+        ccs = ccs_vr.copy() if j==0 else ccs_spont.copy()
+        scores = scores_vr.copy() if j==0 else scores_spont.copy()
+        for k in range(5):
+            ax = plt.subplot(grid[j, k])
+            cc = ccs[k].copy()
+            cc -= np.diag(np.diag(cc))
+            im = ax.imshow(cc, vmin=-vmax, vmax=vmax, cmap="RdBu_r")
+            ax.axis("off")
+            
+            if k==0:
+                ax.text(0., 1.05, f"locality = {localities[k]}\nscores (global / local): {scores[k][0]:.2f} / {scores[k][1]:.2f}", transform=ax.transAxes,
+                    fontsize="medium")#, ha="center")
+                il = plot_label(ltr, il, ax, transl, fs_title)
+                ax.set_title(f"{tstrs[j]} - asymmetric similarity matrix", 
+                            y=1.22)
+                cax = ax.inset_axes([1.05, 0.55, 0.05, 0.3])
+                plt.colorbar(im, cax=cax)
+            else:
+                ax.text(0., 1.05, f"locality = {localities[k]}\nscores: {scores[k][0]:.2f} / {scores[k][1]:.2f}", transform=ax.transAxes,
+                    fontsize="medium")#, ha="center")
+
+    if save_figure:
+        fig.savefig(os.path.join(root, "figures", "suppfig_asym.pdf"))
+
+def suppfig_beh(root, save_figure=True):
+    d = np.load(os.path.join(root, "results", "spont_proc.npz"), allow_pickle=True) 
+    sn = d["sn"]
+    itest = d["itest"]
+    dbeh = np.load(os.path.join(root, "results", "spont_corrs_beh.npz"), allow_pickle=True) 
+    sn_beh = dbeh["sn_beh"]
+    vars = dbeh["vars"]
+
+    fig = plt.figure(figsize=(14,3.7))
+    grid = plt.GridSpec(1,5, figure=fig, left=0.02, right=0.99, top=0.82, bottom=0.04, 
+                                wspace = 0.2, hspace = 0.5)
+    transl = mtransforms.ScaledTranslation(-15 / 72, 20 / 72, fig.dpi_scale_trans)
+    il = 0
+
+    xmin = 688*4
+    xmax = xmin+500
+    xr = xmax - xmin
+    yh = 0.9
+    padding_x = 0.008
+    nbin = 50
+
+    padding = 0.015
+    ax = plt.subplot(grid[0, 0])
+    pos = ax.get_position().bounds
+    ax.axis("off")
+    ax.remove()
+    ax = fig.add_axes([pos[0], pos[1]+pos[3]*(yh+0.03), pos[2], pos[3]*(1-yh-0.01)])     
+    ax.text(0, 1.4, "Spontaneous neural activity\nRastermap sorting",
+                    fontsize="large", transform=ax.transAxes, fontstyle="italic")
+    il = plot_label(ltr, il, ax, transl, fs_title)        
+    ax.axis("off")
+
+    ax = fig.add_axes([pos[0], pos[1], pos[2], pos[3]*yh])     
+    plot_raster(ax, sn[:,itest.flatten()], 
+                    xmin=xmin, xmax=xmax, vmax=1.5, fs=3.38, 
+                    nper=nbin, n_neurons=5000, label=True, 
+                    padding=padding, padding_x=padding_x)
+    
+    titles = ["running speed", "whisking speed", "nose speed", "eye area"]
+    vmax = [0.2, 0.1, 0.1, 0.2]
+    ylim = [[0, 1.2], [0, 3], [0, 3], [-1.5, 3]]
+    for k in range(4):
+        ax = plt.subplot(grid[0, k+1])
+        pos = ax.get_position().bounds
+        ax.axis("off")
+        ax.remove()
+
+        # beh plot
+        ax = fig.add_axes([pos[0], pos[1]+pos[3]*(yh+0.03), pos[2], pos[3]*(1-yh-0.01)])     
+        if k<3:
+            ax.fill_between(np.arange(0, xr), vars[itest.flatten(),k][xmin:xmax], 
+                            color=kp_colors[[0,2,4]][k])
+            ax.set_ylim(ylim[k])
+        else:
+            ax.plot(np.arange(0, xr), vars[itest.flatten(),k][xmin:xmax], color=kp_colors[1])
+        ax.set_xlim([-2*padding_x*xr, xr])
+        ax.axis("off")
+        ax.set_title(titles[k], color=kp_colors[[0,2,4,1]][k], fontsize="medium", y=0.8)
+        if k==0:
+            il = plot_label(ltr, il, ax, transl, fs_title)        
+        elif k==1:
+            ax.text(1, 1.8, "sorting by correlation with behavioral variables", ha="center",
+                    fontsize="large", transform=ax.transAxes, fontstyle="italic")
+
+        # spk raster
+        sn_test = sn_beh[k][::-1]
+        #isort = isorts_beh[k][::-1].copy()
+        #sn_test = zscore(utils.bin1d(spks[isort][:,itest.flatten()], nbin, axis=0), axis=1)
+        ax = fig.add_axes([pos[0], pos[1], pos[2], pos[3]*yh])     
+        plot_raster(ax, sn_test, 
+                    xmin=xmin, xmax=xmax, vmax=1.5, fs=3.38, 
+                    nper=nbin, n_neurons=5000, label=False, 
+                    padding=padding, padding_x=padding_x)
+        
+    if save_figure:
+        fig.savefig(os.path.join(root, "figures/suppfig_beh.pdf"), dpi=200)
```

### Comparing `rastermap-0.9.4/paper/fig3.ipynb` & `rastermap-0.9.5/paper/fig2.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993529411764706%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(8, 'import fig2\\n')], delete: [8]}}, 6: {'source': "*

 * *            "{insert: [(3, 'fig2.fig2(root)')], delete: [3]}}}"}*

```diff
@@ -10,15 +10,15 @@
                 "import numpy as np\n",
                 "from scipy.stats import zscore\n",
                 "from rastermap import Rastermap, utils\n",
                 "\n",
                 "# path to paper code\n",
                 "sys.path.insert(0, '/github/rastermap/paper')\n",
                 "from loaders import tuning_curves_VR\n",
-                "import fig3\n",
+                "import fig2\n",
                 "\n",
                 "# path to directory with data etc\n",
                 "### *** CHANGE THIS TO WHEREEVER YOU ARE DOWNLOADING THE DATA ***\n",
                 "root = \"/media/carsen/ssd2/rastermap_paper/\"\n",
                 "# (in this folder we have a \"data\" folder and a \"results\" folder)\n",
                 "os.makedirs(os.path.join(root, \"data\"), exist_ok=True)\n",
                 "os.makedirs(os.path.join(root, \"results\"), exist_ok=True)"
@@ -89,15 +89,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# root path has folder \"results\" with saved results\n",
                 "# will save figures to \"figures\" folder\n",
                 "os.makedirs(os.path.join(root, \"figures/\"), exist_ok=True)\n",
-                "fig3.fig3(root)"
+                "fig2.fig2(root)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### supplementary analysis"
```

### Comparing `rastermap-0.9.4/paper/fig3.py` & `rastermap-0.9.5/paper/fig2.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     il = plot_label(ltr, il, ax, transl, fs_title)
     
     cax = grid.figure.add_axes([poss[0]+poss[2]*1.02, poss[1]+poss[3]*0.75, 
                         poss[2]*0.03, poss[3]*0.25])
     plt.colorbar(im, cax)
     return il
 
-def _fig3(brain_img, sn, xpos, ypos, isort, isort2, cc_nodes,
+def _fig2(brain_img, sn, xpos, ypos, isort, isort2, cc_nodes,
          corridor_starts, corridor_widths, 
          corridor_tuning, corridor_imgs, VRpos,
          reward_inds, sound_inds, lick_inds, run):
     fig = plt.figure(figsize=(14,7))
     yratio = 14 / 7
     grid = plt.GridSpec(3,5, figure=fig, left=0.02, right=0.98, top=0.98, bottom=0.02, 
                         wspace = 0.3, hspace = 0.15)
@@ -195,15 +195,15 @@
 
     il = panel_cc(grid, il, yratio, cc_nodes)
     
     ax = plt.subplot(grid[:,1:])
     pos = ax.get_position().bounds
     ax.remove()
 
-    xmin = 1410
+    xmin = 0
     xmax=xmin+520
 
     nn = sn.shape[0]
     xr = xmax - xmin
     y0 = pos[1]
     x0 = pos[0]
     padding=0.025
@@ -235,25 +235,25 @@
         fig.add_axes([poss[0]+poss[2]+xpad+xpadt+dxt, poss[1], dxt, poss[3]])]
     
     il = panels_tuning(axs, il, padding, corridor_tuning)
 
     return fig
 
 
-def fig3(root, save_figure=True):
+def fig2(root, save_figure=True):
     d = np.load(os.path.join(root, "results", "corridor_proc.npz"), allow_pickle=True) 
     d2 = np.load(os.path.join(root, "data", "corridor_behavior.npz"), allow_pickle=True) 
     try:
         brain_img = plt.imread(os.path.join(root, "figures", "brain_window_visual.png"))
     except:
         brain_img = np.zeros((50,50))
 
-    fig = _fig3(brain_img, **d, **d2)
+    fig = _fig2(brain_img, **d, **d2)
     if save_figure:
-        fig.savefig(os.path.join(root, "figures", "fig3.pdf"), dpi=200)
+        fig.savefig(os.path.join(root, "figures", "fig2.pdf"), dpi=200)
 
           
 def _suppfig_vr_algs(snys, ctunings,
         corridor_starts, corridor_widths, reward_inds):
         
     fig = plt.figure(figsize=(12,12))
     grid = plt.GridSpec(2,1, figure=fig, left=0.06, right=0.96, top=0.96, bottom=0.04,
```

### Comparing `rastermap-0.9.4/paper/fig4.ipynb` & `rastermap-0.9.5/paper/fig4.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996031746031746%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(3, 'import imp\\n'), (4, 'imp.reload(fig4)\\n')]}}}"}*

```diff
@@ -178,14 +178,16 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# root path has folder \"results\" with saved results\n",
                 "# will save figures to \"figures\" folder\n",
                 "# will ignore panels that aren't processed\n",
+                "import imp\n",
+                "imp.reload(fig4)\n",
                 "os.makedirs(os.path.join(root, \"figures/\"), exist_ok=True)\n",
                 "fig4.fig4(root)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `rastermap-0.9.4/paper/fig5.ipynb` & `rastermap-0.9.5/paper/fig7.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974383503401361%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(16, 'import fig7\\n')], delete: [16]}}, 2: {'source': "*

 * *            "{insert: [(2, 'qrdqn.run_qrdqn(model_folder, root, env_id=env_ids[0], "*

 * *            "n_seeds=n_seeds, device=device)')], delete: [2]}}, 6: {'source': {insert: [(3, "*

 * *            "'fig7.fig7(root)')], delete: [3]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.16'}}"}*

```diff
@@ -22,15 +22,15 @@
                 "# install torch with cuda support\n",
                 "device = torch.device('cuda')\n",
                 "num_threads = 16\n",
                 "torch.set_num_threads(num_threads)\n",
                 "\n",
                 "sys.path.insert(0, \"/github/rastermap/paper\")\n",
                 "import qrdqn # has functions that wrap rl-baselines3-zoo and stable_baselines3\n",
-                "import fig5 \n",
+                "import fig7\n",
                 "\n",
                 "# path to directory with data etc\n",
                 "### *** CHANGE THIS TO WHEREEVER YOU ARE SAVING YOUR MODEL OUTPUTS ***\n",
                 "root = \"/media/carsen/ssd2/rastermap_paper/\"\n",
                 "# (in this folder we have a \"simulations\" folder)\n",
                 "os.makedirs(os.path.join(root, \"simulations\"), exist_ok=True)\n",
                 "\n",
@@ -54,15 +54,15 @@
             "execution_count": null,
             "id": "78e816ab",
             "metadata": {},
             "outputs": [],
             "source": [
                 "### IMPORTANT:\n",
                 "### need to run one game at a time then restart notebook because hooks stick around\n",
-                "# qrdqn.run_qrdqn(model_folder, root, env_id=env_ids[0], n_seeds=n_seeds, device=device)"
+                "qrdqn.run_qrdqn(model_folder, root, env_id=env_ids[0], n_seeds=n_seeds, device=device)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "acf413db",
             "metadata": {},
             "source": [
@@ -101,15 +101,15 @@
                 "outputId": "7dc6125b-ec4a-4983-f6c5-e6b8402fe3a2"
             },
             "outputs": [],
             "source": [
                 "# root path has folder \"simulations\" with saved results\n",
                 "# will save figures to \"figures\" folder\n",
                 "os.makedirs(os.path.join(root, \"figures/\"), exist_ok=True)\n",
-                "fig5.fig5(root)"
+                "fig7.fig7(root)"
             ]
         }
     ],
     "metadata": {
         "colab": {
             "name": "atari_pretrained.ipynb",
             "provenance": []
@@ -125,15 +125,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.17"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "cdf17a3778e5017f066e6f3db18157f3af3a0506de593e09339227d49ead1beb"
             }
         }
     },
```

### Comparing `rastermap-0.9.4/paper/fig5.py` & `rastermap-0.9.5/paper/fig7.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import numpy as np
 import matplotlib.pyplot as plt 
 
 from fig_utils import *
 
 
-def fig5(root, save_figure=True):
+def fig7(root, save_figure=True):
     env_ids = ["PongNoFrameskip-v4", "SpaceInvadersNoFrameskip-v4", 
                "EnduroNoFrameskip-v4", "SeaquestNoFrameskip-v4"]
     fig = plt.figure(figsize=(14,7))
     grid = plt.GridSpec(2,6, figure=fig, left=0.04, right=0.98, top=0.96, bottom=0.07, 
                         wspace = 0.15, hspace = 0.25)
     transl = mtransforms.ScaledTranslation(-13 / 72, 20 / 72, fig.dpi_scale_trans)
     il = 0
@@ -69,8 +69,8 @@
             ax.set_title(f"frame {iframes[k]}", fontsize="medium", color="b")
             ax.axis("off")
             if k==0:
                 ax.text(0, 1.23, env_id[:-14], fontsize="large", transform=ax.transAxes)
                 il = plot_label(ltr, il, ax, transl, fs_title)
 
     if save_figure:
-        fig.savefig(os.path.join(root, "figures", "fig5.pdf"), dpi=200)
+        fig.savefig(os.path.join(root, "figures", "fig7.pdf"), dpi=200)
```

### Comparing `rastermap-0.9.4/paper/fig_splitting.py` & `rastermap-0.9.5/paper/fig8.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,59 +38,64 @@
     #ax.set_facecolor("k")
     ax.spines["left"].set_visible(False)
     ax.spines["bottom"].set_visible(False)
     ax.axis("square")
     return line
 
 def panels_sim2d(fig, grid, il, xi, X_embedding, isorts, 
-                 knn_score, knn, rhos):
+                 knn_score, knn, rhos, g0=2):
     perplexities = [[10, 100], [10], [30], [100], [300]]
 
+    ax = plt.subplot(grid[g0,:-1])
+    grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(1,5, subplot_spec=ax, 
+                                                        wspace=0.3, hspace=0.6)
+    ax.remove()
     gs = plt.get_cmap("Greens")(np.linspace(0.3, 0.7, knn_score.shape[1]-1))[::-1,:3]
     colors = np.stack((0.*np.ones(3), np.array([0.5,0,0]), 
                         np.array([0,0,1]), *gs), axis=0)
 
 
     isort0, isort_split, isort_tsne = isorts[:3]
 
-    dx = 0.01
-    ax = plt.subplot(grid[0,0])
+    dx = 0.02
+    ax = plt.subplot(grid1[0,0])
     pos = ax.get_position().bounds
     ax.set_position([pos[0]+2*dx, pos[1], pos[2], pos[3]])
-    transl = mtransforms.ScaledTranslation(-40 / 72, 10 / 72, fig.dpi_scale_trans)
+    transl = mtransforms.ScaledTranslation(-40/ 72, 28 / 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, ax, transl, fs_title)
     line = plot_sorting2d(ax, xi, isort0, label=True)
-    ax.text(-0.15, 1.07, "sorting by: ", fontweight="bold", transform=ax.transAxes)
+    ax.text(-0.2, 1.2, "2D simulation", transform=ax.transAxes, fontsize="large")
+    ax.text(-0.25, 1.05, "sorting by: ", fontweight="bold", transform=ax.transAxes)
     ax.set_title("   rastermap", fontsize="medium", 
                 color=colors[0], loc="center")#, fontweight="bold")
     cax = ax.inset_axes([-0.04, 0.0, 0.03, 0.3])
     cmap = cmap_emb(np.linspace(0.1,1.0,50))[:,np.newaxis,:3]
     cax.imshow(cmap, aspect="auto")
     #cax.axis("off")
     cax.set_xticks([])
     cax.set_yticks([0, 50])
     cax.set_yticklabels(["1st", "last"])
 
-    ax = plt.subplot(grid[0,1])
+    ax = plt.subplot(grid1[0,1])
     pos = ax.get_position().bounds
     ax.set_position([pos[0]+dx/2, pos[1], pos[2], pos[3]])
     plot_sorting2d(ax, xi, isort_split)
     ax.set_title("rastermap + splitting", fontsize="medium",
                 color=colors[1], loc="center")#, fontweight="bold")
 
-    ax = plt.subplot(grid[0,2])
+    ax = plt.subplot(grid1[0,2])
     pos = ax.get_position().bounds
     ax.set_position([pos[0]-dx, pos[1], pos[2], pos[3]])
     plot_sorting2d(ax, xi, isort_tsne)
     ax.set_title("t-SNE multi-perplexity", fontsize="medium", 
                 color=colors[2], loc="center")#, fontweight="bold")
 
-    ax = plt.subplot(grid[0,3])
+    ax = plt.subplot(grid1[0,3])
     pos = ax.get_position().bounds
-    ax.set_position([pos[0]+dx, pos[1]+0.03, pos[2]-dx, pos[3]])
+    ax.set_position([pos[0], pos[1]+0.03, pos[2], pos[2]*14/8])
     transl = mtransforms.ScaledTranslation(-40 / 72, 2 / 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, ax, transl, fs_title)
     titles = ["rastermap", "+ splitting", "t-SNE multi-$P$"]
     for perplexity in perplexities[1:]:
         titles.append(f"{perplexity[0]}")
     ax.text(1, 0.35, "t-SNE $P$ =     ", color=colors[3], transform=ax.transAxes, ha="right")
     for i in range(knn_score.shape[1]):
@@ -99,18 +104,18 @@
     ax.set_ylim([0, 68])
     ax.set_ylabel("% neighbors preserved")
     ax.set_xlabel("neighborhood size")
     ax.set_xticks([10,100,1000])
     ax.set_xticklabels(["10","100","1000"])
     #plot_raster(ax, X_embedding, 200, 275, vmax=2)
 
-    ax = plt.subplot(grid[0,4])
+    ax = plt.subplot(grid1[0,4])
     pos = ax.get_position().bounds
-    ax.set_position([pos[0]+dx, pos[1]+0.01, pos[2]-dx, pos[3]])
-    transl = mtransforms.ScaledTranslation(-20 / 72, 5 / 72, fig.dpi_scale_trans)
+    ax.set_position([pos[0], pos[1]+0.03, pos[2], pos[2]*14/8])
+    transl = mtransforms.ScaledTranslation(-20 / 72, 2 / 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, ax, transl, fs_title)
     im = ax.imshow(X_embedding[:, 230:320], vmin=0, vmax=2, 
                 cmap="gray_r", aspect="auto")
     ax.set_title("sorted activity", fontsize="medium")
     ax.set_xlabel("time")
     ax.set_ylabel("superneurons")
     ax.set_xticks([])
@@ -118,23 +123,23 @@
     ax.spines["left"].set_visible(False)
     ax.spines["bottom"].set_visible(False)
 
     return il
 
 def panels_v1stimresp(fig, grid, il, yratio, areas, X_embedding, bin_size,
                       isort, xpos, ypos, stim_times, run, ex_stim, 
-                      isort2, x, rfs, g0=1):
+                      isort2, x, rfs, g0=0):
     subsample = 5
     xpos_sub = xpos[::subsample]
     ypos_sub = ypos[::subsample]
 
     ax = plt.subplot(grid[g0,0])
     pos = ax.get_position().bounds
     pos_ratio = (ypos.max() - ypos.min()) / (xpos.max() - xpos.min())
-    ax.set_position([pos[0]+0.01, pos[1]-0.07, pos[2]*0.9, pos[2]*0.9*yratio*pos_ratio])    
+    ax.set_position([pos[0]+0.01, pos[1]-0.04, pos[2]*0.89, pos[2]*0.89*yratio*pos_ratio])    
     memb = np.zeros_like(isort)
     memb[isort] = np.arange(0, len(isort))
     memb = memb[::subsample]
     ax.scatter(xpos_sub, -ypos_sub, s=2.5, 
             c=memb, cmap=cmap_emb, alpha=0.15, rasterized=True)
     iarea = [21, 23, 27, 3, 5]
     xw = 10
@@ -183,26 +188,27 @@
 
     xmin = 5000
     xmax = 5400
     padding_x = 0.005
     
     ax = plt.subplot(grid[g0,1:4])
     pos = ax.get_position().bounds
-    ax.set_position([pos[0], pos[1]-0.03, pos[2], pos[3]*0.9])    
-    axs = fig.add_axes([pos[0], pos[1]-0.03 + pos[3]*1.07, pos[2], pos[3]*0.05])
+    ax.set_position([pos[0], pos[1]-0.03, pos[2]-0.015, pos[3]*0.9])    
+    axs = fig.add_axes([pos[0], pos[1]-0.03 + pos[3]*1.07, pos[2]-0.015, pos[3]*0.05])
     axs.text(0, 1.1, "visual stim.", transform=axs.transAxes)
     st = stim_times[np.logical_and(stim_times < xmax, stim_times >= xmin)] - xmin
+    print(len(st))
     axs.plot([0, xmax-xmin], [0, 0], color="k")
     axs.scatter(st, np.zeros(len(st)), color="k", marker=2, rasterized=True)
     axs.set_xlim([0, (xmax-xmin)*(1+padding_x*2)])
     axs.set_ylim([0, 1])
     axs.axis("off")
     transl = mtransforms.ScaledTranslation(-15 / 72, -2 / 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, axs, transl, fs_title)
-    axr = fig.add_axes([pos[0], pos[1]-0.03 + pos[3]*0.92, pos[2], pos[3]*0.13])
+    axr = fig.add_axes([pos[0], pos[1]-0.03 + pos[3]*0.92, pos[2]-0.015, pos[3]*0.13])
     axr.fill_between(np.arange(0, xmax-xmin), run[xmin : xmax], color=kp_colors[0])
     axr.text(0, 0.55, "running speed", color=kp_colors[0], 
             transform=axr.transAxes)
     axr.set_xlim([0, (xmax-xmin)*(1+padding_x*2)])
     axr.axis("off")
     pos = ax.get_position().bounds
     cax = fig.add_axes([pos[0]+0.6*pos[2], pos[1]-pos[3]*0.05, 
@@ -215,53 +221,45 @@
     nn = X_embedding.shape[0]
     emb_cols = plt.get_cmap("gist_ncar")(np.linspace(0.05, 0.95, nn))[::-1]
     cax.imshow(emb_cols[:,np.newaxis], aspect="auto")
     cax.set_ylim([0, nn*1.025])
     cax.invert_yaxis()
     cax.axis("off")
 
-    ax = plt.subplot(grid[g0+1,1:4])
-    pos = ax.get_position().bounds
-    ax.set_position([pos[0], pos[1]-0.02, pos[2], pos[3]*0.9])    
-    transl = mtransforms.ScaledTranslation(-15 / 72, 5 / 72, fig.dpi_scale_trans)
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    plot_raster(ax, x[:,isort2][:,::10], xmin=0, xmax=500, vmax=1.5, padding=0.04,
-                padding_x=padding_x, nper=bin_size, n_neurons=5000, xlabel="stim.",
-                label_pos="right", label=True, fs=1, n_sec=20)
-    ax.set_title("responses sorted across stimuli", fontsize="medium")
-
-    ax = plt.subplot(grid[g0:g0+4, 4])
+    ax = plt.subplot(grid[:, -1])
     pos = ax.get_position().bounds
-    ax.set_position([pos[0], pos[1]-0.07, pos[2], pos[3]+0.05])    
+    ax.set_position([pos[0], pos[1]-0.03, pos[2], pos[3]+0.01])    
     ny, nx = 30, 8
     grid1 = matplotlib.gridspec.GridSpecFromSubplotSpec(ny,nx, subplot_spec=ax, 
                                                                 wspace=0.15, hspace=0.1)
     ax.remove()
     dj = nn // (nx*ny)
     vmax = 1e-4
     rfj = np.linspace(0, nn-1, nx*ny).astype("int")
     for j in range(nx*ny):
         ax = plt.subplot(grid1[j//nx, j%nx])
-        rfi = rfj[nx*ny - 1 - j]
+        rfi = rfj[j]#nx*ny - 1 - j]
         ax.imshow(rfs[rfi], vmin = -vmax, vmax = vmax, cmap = 'RdBu_r', rasterized=True)
         if j==0:
             ax.text(0, 2.5, "superneuron receptive fields", transform=ax.transAxes)
             transl = mtransforms.ScaledTranslation(-15 / 72, 15 / 72, fig.dpi_scale_trans)
             il = plot_label(ltr, il, ax, transl, fs_title)
         ax.axis('off')
         if j<2 or j>nx*ny-3:
-            ax.text(0.5, 1.1, f"{nn - rfi}", ha="center", transform=ax.transAxes)
+            ax.text(0.5, 1.1, f"{rfi+1}", ha="center", transform=ax.transAxes, 
+                    fontsize="small")
         elif j==2 or j==nx*ny-3:
-            ax.text(0.5, 1.5, f"...", ha="center", transform=ax.transAxes)
+            ax.text(0.5, 1.4, f"...", ha="center", transform=ax.transAxes, 
+                    fontsize="small")
 
 
     return il
 
 def panels_alexnet(fig, grid, il, X_embedding, bin_size, 
-                   isort, isort2, ipos, ilayer, iconv, nmax, g0=2):
+                   isort, isort2, ipos, ilayer, iconv, nmax, g0=1):
     
     memb = np.zeros(len(isort))
     memb[isort] = np.arange(len(isort))
     ax = plt.subplot(grid[g0,0])
     transl = mtransforms.ScaledTranslation(-15 / 72, -12 / 72, fig.dpi_scale_trans)
     il = plot_label(ltr, il, ax, transl, fs_title)
     ypre = 0
@@ -277,71 +275,72 @@
         ypre += (yp.max() + 4)
     ax.axis("square")
     ax.axis("off")
     ax.set_title("Alexnet convolutional layer responses", y=0.88)
 
     ax = plt.subplot(grid[g0,1:4])
     xmin = 2200
-    xmax = 2700
+    xmax = xmin + 188 #2700
     padding_x = 0.005
     pos = ax.get_position().bounds
-    ax.set_position([pos[0], pos[1]-0.01, pos[2], pos[3]*0.9]) 
+    ax.set_position([pos[0], pos[1]-0.01, pos[2]-0.015, pos[3]*0.9]) 
     pos = ax.get_position().bounds
     cax = fig.add_axes([pos[0]+0.6*pos[2], pos[1]-pos[3]*0.05, 
                         pos[2]*0.06, pos[3]*0.03])
     plot_raster(ax, X_embedding, xmin, xmax, cax=cax, cax_label="left", 
                 vmax=2, padding=0.04, padding_x=padding_x, 
                 nper=bin_size, n_neurons=1000, xlabel="stim.",
-                fs=1, n_sec=20, label=True, label_pos="right")
+                fs=1, n_sec=10, label=True, label_pos="right")
     #ax.set_title("Alexnet responses to visual stimuli")
     cax = fig.add_axes([pos[0]-pos[2]*0.03, pos[1], pos[2]*0.015, pos[3]])
     nn = X_embedding.shape[0]
     emb_cols = plt.get_cmap("gist_ncar")(np.linspace(0.05, 0.95, nn))[::-1]
     cax.imshow(emb_cols[:,np.newaxis], aspect="auto")
     cax.set_ylim([0, nn*1.025])
     cax.invert_yaxis()
     cax.axis("off")
 
-    ax = plt.subplot(grid[g0+1,1:4])
-    pos = ax.get_position().bounds
-    ax.set_position([pos[0], pos[1]-0.0, pos[2], pos[3]*0.9])    
-    transl = mtransforms.ScaledTranslation(-15 / 72, 5 / 72, fig.dpi_scale_trans)
-    il = plot_label(ltr, il, ax, transl, fs_title)
-    plot_raster(ax, X_embedding[:,isort2][:,::10], xmin=0, xmax=500, vmax=1.5, padding=0.04,
-                padding_x=padding_x, nper=bin_size, n_neurons=5000, xlabel="stim.",
-                label_pos="right", label=True, fs=1, n_sec=20)
-    ax.set_title("responses sorted across stimuli", fontsize="medium")
-
-
     return il
 
     
 def fig_all(root, save_figure=True):
     
     fig = plt.figure(figsize=(14,8))
     yratio = 14 / 8
     grid = plt.GridSpec(3,5, figure=fig, left=0.01, right=0.99, top=0.94, bottom=0.055, 
                     wspace = 0.15, hspace = 0.25)
     il = 0
 
-    try:
-        d = np.load(os.path.join(root, "simulations", "sim2D_results.npz"))
-        il = panels_sim2d(fig, grid, il, **d)
-    except:
-        print("simulation data not available")
+    ax = plt.subplot(grid[:, -1])
+    pos = ax.get_position().bounds
+    ax.set_position([pos[0], pos[1]-0.03, pos[2], pos[3]+0.01])    
+    pos = ax.get_position().bounds
+    ax.remove()
 
     try:
         areas = loadmat(os.path.join(root, "figures", "ctxOutlines.mat"), 
                         squeeze_me=True)["coords"]
         d = np.load(os.path.join(root, "results", "v1stimresp_proc.npz"))
         il = panels_v1stimresp(fig, grid, il, yratio, areas, **d)
+        ax = fig.add_axes([pos[0]-0.045, pos[1], 0.04, pos[3]])
+        ax.plot([0, 1], [0.71, 0], color=0.5*np.ones(3), lw=1)
+        ax.plot([0, 1], [0.96, 1], color=0.5*np.ones(3), lw=1)
+        ax.set_ylim([0, 1])
+        ax.set_xlim([0, 1])
+        ax.axis("off")
     except:
         print("visual data not available")
 
     try:
         d = np.load(os.path.join(root, "results", "alexnet_proc.npz"))
         il = panels_alexnet(fig, grid, il, **d)  
     except:
         print("alexnet data not available")
 
+    try:
+        d = np.load(os.path.join(root, "simulations", "sim2D_results.npz"))
+        il = panels_sim2d(fig, grid, il, **d)
+    except:
+        print("simulation data not available")
+
     if save_figure:
-        fig.savefig(os.path.join(root, "figures", "fig6.pdf"), dpi=200)
+        fig.savefig(os.path.join(root, "figures", "fig8.pdf"), dpi=200)
```

### Comparing `rastermap-0.9.4/paper/fig_utils.py` & `rastermap-0.9.5/paper/fig_utils.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/paper/loaders.py` & `rastermap-0.9.5/paper/loaders.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/paper/metrics.py` & `rastermap-0.9.5/paper/metrics.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/paper/other_upsampling.py` & `rastermap-0.9.5/paper/other_upsampling.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/paper/qrdqn.py` & `rastermap-0.9.5/paper/qrdqn.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/paper/splitting.ipynb` & `rastermap-0.9.5/paper/splitting.ipynb`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/__main__.py` & `rastermap-0.9.5/rastermap/__main__.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/cluster.py` & `rastermap-0.9.5/rastermap/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,20 +111,19 @@
         cluster centers found by kmeans
     imax : array (n_samples)
         best cluster for each data point
 
     """
     n_samples, n_features = X.shape
     # initialize with kmeans++
+    np.random.seed(random_state)
     if init == "kmeans++":
-        np.random.seed(random_state)
         X_nodes = _scaled_kmeans_init(X, n_clusters=n_clusters, 
                                         n_local_trials=n_local_trials)
     else:
-        np.random.seed(random_state)
         X_nodes = np.random.randn(n_clusters, n_features) * (X**2).sum(axis=0)**0.5
     X_nodes = X_nodes / (1e-4 + (X_nodes**2).sum(axis=1)[:, np.newaxis])**.5
     
     # iterate and reassign neurons
     for j in range(n_iter):
         cc = X @ X_nodes.T
         imax = np.argmax(cc, axis=1)
@@ -154,15 +153,15 @@
 
 def kmeans(X, n_clusters=100, random_state=0):
     np.random.seed(random_state)
     #X_nodes = (np.random.randn(n_clusters, n_features) /
     #                            (1 + np.arange(n_features))**0.5)
     #X_nodes = X_nodes / (1e-4 + (X_nodes**2).sum(axis=1)[:,np.newaxis])**.5
     model = KMeans(n_init=1, init="k-means++", n_clusters=n_clusters,
-                   random_state=0).fit(X)
+                   random_state=random_state).fit(X)
     X_nodes = model.cluster_centers_
     X_nodes = X_nodes / (1e-10 + ((X_nodes**2).sum(axis=1))[:, np.newaxis])**.5
     imax = model.labels_
     X_nodes = X_nodes[X_nodes[:, 0].argsort()]
     cc = X @ X_nodes.T
     imax = cc.argmax(axis=1)
     return X_nodes, imax
```

### Comparing `rastermap-0.9.4/rastermap/gui/colormaps.py` & `rastermap-0.9.5/rastermap/gui/colormaps.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/gui/gui.py` & `rastermap-0.9.5/rastermap/gui/gui.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/gui/guiparts.py` & `rastermap-0.9.5/rastermap/gui/guiparts.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/gui/io.py` & `rastermap-0.9.5/rastermap/gui/io.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/gui/menus.py` & `rastermap-0.9.5/rastermap/gui/menus.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/gui/run.py` & `rastermap-0.9.5/rastermap/gui/run.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/gui/views.py` & `rastermap-0.9.5/rastermap/gui/views.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/io.py` & `rastermap-0.9.5/rastermap/io.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/rastermap.py` & `rastermap-0.9.5/rastermap/rastermap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 Copright © 2023 Howard Hughes Medical Institute, Authored by Carsen Stringer and Marius Pachitariu.
 """
 import time
 import numpy as np
 import warnings
 from scipy.stats import zscore
+import logging
+import sys 
 
 from .cluster import kmeans, scaled_kmeans, compute_cc_tdelay
 from .sort import traveling_salesman, compute_BBt, matrix_matching
 from .upsample import grid_upsampling
 from .utils import bin1d
 from .svd import SVD
 
+rmap_logger = logging.getLogger(__name__)
+
 def default_settings():
     """ default settings for main algorithm settings """
     settings = {}
     settings["n_clusters"] = 100
     settings["n_PCs"] = 200
     settings["time_lag_window"] = 0
     settings["locality"] = 0.0
@@ -23,15 +27,14 @@
     settings["time_bin"] = 0
     settings["grid_upsample"] = 10
     settings["mean_time"] = True
     settings["verbose"] = True
     settings["verbose_sorting"] = False
     return settings
 
-
 def sequence_settings():
     """ good for data with sequences """
     settings = default_settings()
     settings["time_lag_window"] = 10
     settings["locality"] = 0.75
     return settings
 
@@ -135,41 +138,51 @@
         clusters (recommended to not change, instead use locality to change sorting)
     
     """
 
     def __init__(self, n_clusters=100, n_PCs=200, time_lag_window=0.0, locality=0.0,
                  grid_upsample=10, time_bin=0, normalize=True, mean_time=True, n_splits=0,
                  run_scaled_kmeans=True, verbose=True, verbose_sorting=False, 
-                 keep_norm_X=True, bin_size=0, symmetric=False, 
+                 keep_norm_X=True, bin_size=0, symmetric=False, random_state=0,
                  sticky=True, nc_splits=None, smoothness=1):
 
         self.n_clusters = n_clusters
         self.n_PCs = n_PCs
         self.time_lag_window = time_lag_window
         self.locality = locality
         self.grid_upsample = grid_upsample
         self.time_bin = time_bin
         self.normalize = normalize
         self.mean_time = mean_time
         self.n_splits = n_splits
         self.run_scaled_kmeans = run_scaled_kmeans
         self.verbose = verbose
         self.verbose_sorting = verbose_sorting
+        self.random_state = random_state
 
         self.keep_norm_X = keep_norm_X
         self.bin_size = bin_size                
         self.symmetric = symmetric
         self.sticky = sticky
         self.nc_splits = nc_splits
         self.smoothness = smoothness
         
         self.sorting_algorithm = "travelling_salesman"
         
+        if self.verbose:
+            logging.basicConfig(
+                level=logging.INFO, format="%(asctime)s [%(levelname)s] %(message)s",
+                handlers=[logging.StreamHandler(sys.stdout)])
+        else:
+            logging.basicConfig(
+                level=logging.WARN, format="%(asctime)s [%(levelname)s] %(message)s",
+                handlers=[logging.StreamHandler(sys.stdout)])
+
     def fit(self, data=None, Usv=None, Vsv=None, U_nodes=None, itrain=None,
-            compute_X_embedding=False):
+            compute_X_embedding=True, BBt=None):
         """ sorts data or singular value decomposition of data by first axis
 
         can use full data matrix, or use singular value decomposition, to reduce RAM 
         requirements, it is recommended to use float32. see Rastermap class for 
         parameter information (`Rastermap?`)
 
         example usage:
@@ -184,18 +197,16 @@
         spks = zscore(spks, axis=1)
 
         # fit rastermap
         model = Rastermap(n_PCs=200, n_clusters=100, 
                         locality=0.75, time_lag_window=5).fit(spks)
         y = model.embedding # neurons x 1
         isort = model.isort
-
-        # bin over neurons
-        X_embedding = zscore(utils.bin1d(spks, bin_size=25, axis=0), axis=1)
-
+        X_embedding = model.X_embedding # neurons by time
+        
         # plot
         fig = plt.figure(figsize=(12,5))
         ax = fig.add_subplot(111)
         ax.imshow(X_embedding, vmin=0, vmax=1.5, cmap="gray_r", aspect="auto")
         ```
 
         Inputs
@@ -207,14 +218,18 @@
             singular vectors U times singular values sv
         Vsv : array, shape (n_features, n_PCs) (optional, default None)
             singular vectors U times singular values sv
         U_nodes : array, shape (n_clusters, n_PCs) (optional, default None)
             cluster centers in PC space, if you have precomputed them
         itrain : array, shape (n_features,) (optional, default None)
             fit embedding on timepoints itrain only
+        compute_X_emebdding : bool (optional, default True)
+            compute binning over neurons in X_embedding
+        BBt : array, shape (n_clusters, n_clusters) (optional, default None)
+            use user-specified matching matrix (not recommended for most users)
 
         Assigns
         ----------
         embedding : array, shape (n_samples, 1)
             embedding of each neuron / voxel
         isort : sorting along first dimension of input matrix
             use this to get neuron / voxel sorting
@@ -249,114 +264,113 @@
         normed = False
         if data is not None:
             if self.normalize:
                 if hasattr(self, "X"):
                     warnings.warn("not renormalizing / subtracting mean, using previous normalization")
                     X = self.X 
                 else:
-                    print("normalizing data across axis=1")
+                    rmap_logger.info("normalizing data across axis=1")
                     X = data.copy() 
                     if self.time_bin > 1:
-                        print(f"binning in time with time_bin = {self.time_bin}")
+                        rmap_logger.info(f"binning in time with time_bin = {self.time_bin}")
                         X = bin1d(X, bin_size=self.time_bin, axis=1)
                     X -= X.mean(axis=1)[:,np.newaxis]
                     stdx = X.std(axis=1)
                     X /= stdx[:,np.newaxis]
                     normed = True
             else:
                 if self.time_bin > 1:
                     X = bin1d(data.copy(), bin_size=self.time_bin, axis=1)
                 else:
                     X = data
             if self.mean_time:
                 if hasattr(self, "X"):
-                    warnings.warn("not renormalizing / subtracting mean, using previous normalization")
+                    rmap_logger.warn("not renormalizing / subtracting mean, using previous normalization")
                     X = self.X 
                 else:
-                    print("projecting out mean along axis=0")
+                    rmap_logger.info("projecting out mean along axis=0")
                     X_mean = np.nanmean(X, axis=0, keepdims=True).T
                     X_mean /= (X_mean**2).sum()**0.5
                     w_mean = X @ X_mean
                     X -= w_mean @ X_mean.T
                     normed = True
             if self.keep_norm_X and (self.mean_time or self.normalize):
                 self.X = X
         elif hasattr(self, "X"):
             X = self.X
             Vsv_sub = Vsv.copy()
             if self.normalize or self.mean_time:
-                warnings.warn("not renormalizing / subtracting mean, using previous normalization")
+                rmap_logger.warn("not renormalizing / subtracting mean, using previous normalization")
         else:
             if self.mean_time:
                 V_mean = Vsv.mean(axis=1, keepdims=True)
                 V_mean /= (V_mean**2).sum()**0.5
                 self.V_mean = V_mean
                 proj_mean = V_mean @ (V_mean.T @ Vsv)
                 Vsv_sub = Vsv.copy() - proj_mean
                 normed = True
             else:
                 Vsv_sub = Vsv.copy()
             stdx = Usv.std(axis=1) if stdx is None else stdx
         if normed:
-            print(f"data normalized, {time.time()-t0:0.2f}sec")    
+            rmap_logger.info(f"data normalized, {time.time()-t0:0.2f}sec")    
 
         stdx = X.std(axis=1) if stdx is None else stdx
         igood = np.logical_and(igood, stdx > 0)
         n_samples = igood.sum() 
         n_time = data.shape[1] if data is not None else Vsv.shape[0]
-        print(f"sorting activity: {n_samples} valid samples by {n_time} timepoints")
-        
+        rmap_logger.info(f"sorting activity: {n_samples} valid samples by {n_time} timepoints")
 
         ### ------------- PCA ------------------------------------------------------ ###        
         if not hasattr(self, "Usv"):
             if Usv is None:
                 tic = time.time()
-                Usv_valid = SVD(X[igood][:, itrain] if itrain is not None else X, 
+                Usv_valid = SVD(X[igood][:, itrain] if itrain is not None else X[igood], 
                                n_components=self.n_PCs)            
                 Usv = np.nan * np.zeros((len(igood), Usv_valid.shape[1]), "float32")
                 Usv[igood] = Usv_valid
                 self.Usv = Usv
                 self.n_PCs = Usv.shape[1]
                 pc_time = time.time() - tic
-                print(f"n_PCs = {self.n_PCs} computed, {time.time()-t0:0.2f}sec")    
+                rmap_logger.info(f"n_PCs = {self.n_PCs} computed, {time.time()-t0:0.2f}sec")    
             elif Usv is not None:
                 self.Usv = Usv
                 pc_time = 0
                 self.n_PCs = self.Usv.shape[1]
         self.sv = np.nansum((self.Usv**2), axis=0)**0.5
         if not hasattr(self, "Vsv"):
             if Vsv is None:
                 U = self.Usv.copy() / self.sv
                 self.Vsv = X.T @ U 
             elif Vsv is not None:
-                self.Vsv = Vsv_sub
+                self.Vsv = Vsv
 
         ### ------------- clustering ----------------------------------------------- ###
         if self.run_scaled_kmeans:
             kmeans_func = scaled_kmeans
         else:
             kmeans_func = kmeans
 
         if ((U_nodes is None and self.Usv.shape[0] <= 50) or 
             (self.Usv.shape[0] <= 200 and self.n_clusters is None)):
             # number of neurons / voxels <= 50, skip clustering
             if U_nodes is None and self.Usv.shape[0] <= 50:
                 warnings.warn("""data has <= 50 samples, \n
                                 going to skip clustering and sort samples""")
             elif (self.Usv.shape[0] <= 200 and self.n_clusters is None):
-                print("skipping clustering, n_clusters is None")
+                rmap_logger.info("skipping clustering, n_clusters is None")
             U_nodes = self.Usv[igood].copy()
             imax = np.arange(0, U_nodes.shape[0])
         elif self.n_clusters is None:
             raise ValueError("n_clusters set to None")
         elif self.n_clusters >= 200:
             raise ValueError("n_clusters cannot be greater than 200")
         elif not hasattr(self, "U_nodes") and U_nodes is not None:
             # use user input for clusters
-            print("using cluster input from user")
+            rmap_logger.info("using cluster input from user")
             cu = self.Usv[igood] @ U_nodes.T
             imax = cu.argmax(axis=1)
         elif hasattr(self, "U_nodes") and self.U_nodes is not None:
             # skip clustering as it was run before
             if self.n_splits==1:
                 U_nodes = self.U_nodes
                 imax = self.embedding_clust
@@ -364,29 +378,31 @@
             else:
                 raise ValueError("""cannot rerun if n_splits > 0\n 
                                     need to set model.U_nodes = None first or \n 
                                     reset model = Rastermap(...) """)
         else:
             # run clustering
             self.n_clusters = min(self.Usv.shape[0]//2, self.n_clusters)
-            U_nodes, imax = kmeans_func(self.Usv[igood], n_clusters=self.n_clusters)
-            print(f"{U_nodes.shape[0]} clusters computed, time {time.time() - t0:0.2f}sec")
+            U_nodes = kmeans_func(self.Usv[igood], n_clusters=self.n_clusters,
+                                  random_state=self.random_state)[0]
+            rmap_logger.info(f"{U_nodes.shape[0]} clusters computed, time {time.time() - t0:0.2f}sec")
 
         # compute correlation matrix across clusters
         if self.time_lag_window > 0:
             cc = compute_cc_tdelay(self.Vsv / self.sv, U_nodes, 
                                    time_lag_window=self.time_lag_window,
                                    symmetric=self.symmetric)
         else:
             cc = U_nodes @ U_nodes.T
 
         ### ---------------- sorting ----------------------------------------------- ###
-        cc, inds = traveling_salesman(cc, verbose=self.verbose_sorting, 
-                                       locality=self.locality,
-                                        n_skip=None)[:2]
+        cc, inds, BBt = traveling_salesman(cc, verbose=self.verbose_sorting, 
+                                            locality=self.locality,
+                                            n_skip=None, BBt=BBt)[:3]
+        self.BBt = BBt
         U_nodes = U_nodes[inds]
         ineurons = (self.Usv[igood] @ U_nodes.T).argmax(axis=1)
         self.cc = cc
         Y_nodes = np.arange(0, U_nodes.shape[0])[:, np.newaxis]
 
         # split and recluster and sort
         if self.n_splits > 0:
@@ -423,27 +439,27 @@
                 n_nodes = U_nodes_new.shape[0]
                 U_nodes = U_nodes_new.copy()
                 ineurons = ineurons_new.copy()
             if not self.sticky:
                 ineurons = (self.Usv[igood] @ U_nodes.T).argmax(axis=1)
             Y_nodes = np.arange(0, U_nodes.shape[0])[:, np.newaxis]
 
-        print(f"clusters sorted, time {time.time() - t0:0.2f}sec")
+        rmap_logger.info(f"clusters sorted, time {time.time() - t0:0.2f}sec")
         
         ### ---------------- upsample ---------------------------------------------- ###
         self.n_clusters = U_nodes.shape[0]
         if self.grid_upsample > 0:
             self.n_X = int(self.n_clusters * max(2, self.grid_upsample))
             n_neighbors = max(min(8, self.n_clusters - 1), self.n_clusters // 5)
             e_neighbor = max(1, min(self.smoothness, n_neighbors - 1))
 
             Y, corr, g, Xrec = grid_upsampling(self.Usv[igood], U_nodes, Y_nodes, n_X=self.n_X,
                                             n_neighbors=n_neighbors,
                                             e_neighbor=e_neighbor)
-            print(f"clusters upsampled, time {time.time() - t0:0.2f}sec")
+            rmap_logger.info(f"clusters upsampled, time {time.time() - t0:0.2f}sec")
         else:
             if len(U_nodes) == n_samples:
                 Y = np.zeros(n_samples, "int")
                 Y[inds] = np.arange(0, n_samples)
             else:
                 Y = np.zeros(n_samples, "int")
                 Y[ineurons.argsort()] = np.arange(0, n_samples)
@@ -467,18 +483,19 @@
         self.igood = igood
         self.embedding = np.nan * np.zeros((len(self.igood),1))
         self.embedding[igood] = self.embedding_valid
         self.isort = self.embedding[:,0].argsort()
         
         ### ----------- bin across embedding --------------------------------------- ###
         if data is not None and compute_X_embedding:
+            bin_size=self.bin_size
             if (bin_size==0 or n_samples < bin_size or 
                 (bin_size == 50 and n_samples < 1000)):
                 bin_size = max(1, n_samples // 500)
             self.X_embedding = zscore(bin1d(X[igood][self.isort], bin_size, axis=0), axis=1)
 
-        print(f"rastermap complete, time {time.time() - t0:0.2f}sec")
+        rmap_logger.info(f"rastermap complete, time {time.time() - t0:0.2f}sec")
 
         self.runtime = time.time() - t0
         self.pc_time = pc_time
 
         return self
```

### Comparing `rastermap-0.9.4/rastermap/sort.py` & `rastermap-0.9.5/rastermap/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
         Kx, fx = create_ND_basis(1, nclust, K, flag)
         S = np.zeros((S0.shape[0], K, S0.shape[1], nclust), np.float64)
         fxx = np.zeros((S0.shape[0], K))
         for kx in range(K):
             for ky in range(S0.shape[0]):
                 S[ky, kx, :, :] = np.outer(S0[ky, :], Kx[kx, :])
                 fxx[ky, kx] = ((0 + fy[ky])**2 + (0 + fx[kx])**2)**0.5
-                #fxx[ky,kx] = fy[ky] + fx[kx]
-                #fxx[ky,kx] = max(fy[ky], fx[kx]) + min(fy[ky], fx[kx])/1000.
         S = np.reshape(S, (K * S0.shape[0], nclust * S0.shape[1]))
     fxx = fxx.flatten()
     ix = np.argsort(fxx)
     S = S[ix, :]
     fxx = fxx[ix]
     return S, fxx
 
@@ -174,29 +172,30 @@
                 start_pos[k] = i0
                 end_pos[k] = inode
                 flipped[k] = ordering
     return cc, inds, seg_len, start_pos, end_pos, flipped
 
 
 def traveling_salesman(cc, n_iter=400, locality=0.0, circular=False,
-                         n_skip=None, verbose=False):
+                         n_skip=None, BBt=None, verbose=False):
     """ matches correlation matrix cc to B@B.T basis functions """
     n_nodes = (cc.shape[0])
     if n_skip is None:
         n_skip = max(1, n_nodes // 30)
     cc = cc.astype(np.float32)
 
     n_components = 1
 
     x = np.arange(0, 1.0, 1.0 / n_nodes)[:n_nodes]
-    BBt = compute_BBt(x, x, locality=locality, circular=circular)
-    if np.isinf(locality):
-        BBt = np.ones((n_nodes, n_nodes))
-        BBt = np.tril(np.triu(BBt, -1), 1)
-    BBt = np.triu(BBt)
+    if BBt is None:
+        BBt = compute_BBt(x, x, locality=locality, circular=circular)
+        if np.isinf(locality):
+            BBt = np.ones((n_nodes, n_nodes))
+            BBt = np.tril(np.triu(BBt, -1), 1)
+        BBt = np.triu(BBt)
 
     n_iter = np.int64(n_iter)
 
     cc, inds, seg_len, start_pos, end_pos, flipped = tsp_fast(
         cc, n_iter, n_nodes, n_skip, BBt.astype(np.float32), verbose)
     iter_completed = np.nonzero(seg_len == -1)[0][0]
     seg_len = seg_len[:iter_completed]
@@ -209,15 +208,15 @@
         iter_completed = np.nonzero(seg_len2 == -1)[0][0]
         seg_len = np.append(seg_len, seg_len2[:iter_completed])
         start_pos = np.append(start_pos, start_pos2[:iter_completed])
         end_pos = np.append(end_pos, end_pos2[:iter_completed])
         flipped = np.append(flipped, flipped2[:iter_completed])
         inds = inds[inds2]
 
-    return cc, inds, seg_len, start_pos, end_pos, flipped
+    return cc, inds, BBt, seg_len, start_pos, end_pos, flipped
 
 
 @njit("int32[:] (int64, int64, int64, int64, int64)", nogil=True, cache=True)
 def shift_inds_sub(i0, i1, inode, isforward, n_nodes):
     """ shift segment from i0->i1 to position inode"""
     n_seg = i1 - i0 + 1
     inds = np.arange(0, n_nodes, 1, np.int32)
@@ -353,33 +352,49 @@
 
 def compute_BBt_mask(xi, yi):
     sigma = 0.5 * (xi[1] - xi[0])
     gaussian = np.exp(-(xi[:, np.newaxis] - yi)**2 / (2 * sigma**2))
     gaussian[(xi[:, np.newaxis] - yi) == 0] = 0
     return gaussian
 
-
-def compute_BBt(xi, yi, locality=0, circular=False):
-    if locality > 0:
-        BBt0 = compute_BBt(xi, xi, locality=0)
-        BBt_norm = BBt0.sum()
-        BBt_mask_norm = compute_BBt_mask(xi, xi).sum()
+def compute_BBt(xi, yi, locality=0, circular=False, alpha=1):
+    """ can change alpha but only if not splitting """
+    #if locality > 0:
+    #    BBt0 = compute_BBt(xi, yi, locality=0)
+    #    BBt_norm = BBt0.sum()
+    #    BBt_mask_norm = compute_BBt_mask(xi, yi).sum()
     eps = 1e-3
+    
     if not circular:
-        ds = np.abs(xi[:, np.newaxis] - yi)
-        ds[ds == 0] = 1 - eps
-        BBt = -np.log(eps + ds)
+        if alpha==1:
+            ds = np.abs(xi[:, np.newaxis] - yi)
+            ds[ds == 0] = 1 - eps
+            BBt = -np.log(eps + ds)
+        else:
+            n_nodes = len(xi)
+            B, plaw = create_ND_basis(1, n_nodes, 5 * n_nodes, flag=False)
+            B = B[1:]
+            plaw = plaw[1:]
+            B /= plaw[:,np.newaxis] ** (alpha/2)
+            B_norm = (B**2).sum(axis=0)**0.5
+            B = B / B_norm
+            BBt0 = B.T @ B
     else:
         ds = np.abs(xi[len(xi)//2] - yi)
         ds[ds == 0] = 1 - eps
         BBt0 = -np.log(eps + ds)
         BBt = np.zeros((len(xi), len(yi)), "float32")
         for k in range(len(xi)):
             BBt[k] = np.roll(BBt0, -len(xi)//2 + k)
+    
+    BBt_norm = BBt.mean()
+    BBt /= BBt_norm
+        
     if locality > 0:
         BBt_mask = compute_BBt_mask(xi, yi)
         # need to make BBt and BBt_mask on same scale
-        BBt /= BBt_norm
+        BBt_mask_norm = BBt_mask.mean()
         BBt_mask /= BBt_mask_norm
         BBt = BBt * (1 - locality) + BBt_mask * locality
-        BBt *= BBt_norm
+        #BBt *= BBt_norm
+    
     return BBt
```

### Comparing `rastermap-0.9.4/rastermap/svd.py` & `rastermap-0.9.5/rastermap/svd.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/upsample.py` & `rastermap-0.9.5/rastermap/upsample.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/rastermap/utils.py` & `rastermap-0.9.5/rastermap/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from pathlib import Path
 
 def bin1d(X, bin_size, axis=0):
     """ mean bin over axis of data with bin bin_size """
     if bin_size > 0:
         size = list(X.shape)
         Xb = X.swapaxes(0, axis)
-        Xb = Xb[:size[axis]//bin_size*bin_size].reshape((size[axis]//bin_size, bin_size, -1)).mean(axis=1)
+        size_new = Xb.shape
+        Xb = Xb[:size[axis]//bin_size*bin_size].reshape((size[axis]//bin_size, bin_size, *size_new[1:])).mean(axis=1)
         Xb = Xb.swapaxes(axis, 0)
-        size[axis] = Xb.shape[axis]
-        Xb = Xb.reshape(size)
         return Xb
     else:
         return X
 
 def split_traintest(n_t, frac=0.25, n_segs=20, pad=3, split_time=False):
     """this returns deterministic split of train and test in time chunks
```

### Comparing `rastermap-0.9.4/rastermap.egg-info/PKG-INFO` & `rastermap-0.9.5/rastermap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 Metadata-Version: 2.1
 Name: rastermap
-Version: 0.9.4
+Version: 0.9.5
 Summary: Unsupervised clustering algorithm for 2D data (neurons by time)
 Home-page: https://github.com/MouseLand/rastermap
 Author: Marius Pachitariu and Carsen Stringer
 Author-email: carsen.stringer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: gui
 License-File: LICENSE
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: numba>=0.57.0
+Requires-Dist: natsort
+Requires-Dist: tqdm
+Provides-Extra: gui
+Requires-Dist: pyqtgraph>=0.11.0rc0; extra == "gui"
+Requires-Dist: pyqt6; extra == "gui"
+Requires-Dist: pyqt6.sip; extra == "gui"
+Requires-Dist: qtpy; extra == "gui"
+Requires-Dist: superqt; extra == "gui"
 
 # Rastermap
 
 ![tests](https://github.com/mouseland/rastermap/actions/workflows/test_and_deploy.yml/badge.svg)
 [![codecov](https://codecov.io/gh/MouseLand/rastermap/branch/main/graph/badge.svg?token=9FFo4zNtYP)](https://codecov.io/gh/MouseLand/rastermap)
 [![PyPI version](https://badge.fury.io/py/rastermap.svg)](https://badge.fury.io/py/rastermap)
-[![Downloads](https://pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
-[![Downloads](https://pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
+[![Downloads](https://static.pepy.tech/badge/rastermap)](https://pepy.tech/project/rastermap)
+[![Downloads](https://static.pepy.tech/badge/rastermap/month)](https://pepy.tech/project/rastermap)
 [![Python version](https://img.shields.io/pypi/pyversions/rastermap)](https://pypistats.org/packages/rastermap)
 [![Licence: GPL v3](https://img.shields.io/github/license/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/blob/main/LICENSE)
 [![Contributors](https://img.shields.io/github/contributors-anon/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/graphs/contributors)
 [![repo size](https://img.shields.io/github/repo-size/MouseLand/rastermap)](https://github.com/MouseLand/rastermap/)
 [![GitHub stars](https://img.shields.io/github/stars/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 [![GitHub forks](https://img.shields.io/github/forks/MouseLand/rastermap?style=social)](https://github.com/MouseLand/rastermap/)
 
 
 Rastermap is a discovery algorithm for neural data. The algorithm was written by Carsen Stringer and Marius Pachitariu. For support,  please open an [issue](https://github.com/MouseLand/rastermap/issues). Please see install instructions [below](README.md/#Installation). If you use Rastermap in your work, please cite the [paper](https://www.biorxiv.org/content/10.1101/2023.07.25.550571v1):
 
-Stringer C., Zhong L., Syeda A., Du F., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
+Stringer C., Zhong L., Syeda A., Du F., Kesa M., & Pachitariu M. (2023). Rastermap: a discovery method for neural population recordings. *bioRxiv* 2023.07.25.550571; doi: https://doi.org/10.1101/2023.07.25.550571
 
 Rastermap runs in python 3.8+ and has a graphical user interface (GUI) for running it easily. Rastermap can also be run in a jupyter notebook locally or on google colab, see these demos:
 * [rastermap_largescale.ipynb](notebooks/rastermap_largescale.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_largescale.ipynb) shows how to use it with large-scale data from mouse cortex (> 200 neurons) 
 * [rastermap_singleneurons.ipynb](notebooks/rastermap_singleneurons.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_singleneurons.ipynb) shows how to use it with small to medium sized data (< 200 neurons), in this case recorded from rat hippocampus 
 * [rastermap_zebrafish.ipynb](notebooks/rastermap_zebrafish.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_zebrafish.ipynb) shows how to use it with large-scale data from zebrafish 
 * [rastermap_widefield.ipynb](notebooks/rastermap_widefield.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_widefield.ipynb) shows how to use it with widefield imaging data, or other types of datasets that are too large to fit into memory 
-* [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations 
+* [rastermap_interactive.ipynb](notebooks/rastermap_interactive.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/rastermap_interactive.ipynb) allows running Rastermap in an interactive way without a local installation
+* [tutorial.ipynb](notebooks/tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MouseLand/rastermap/blob/main/notebooks/tutorial.ipynb) is a guided tutorial for integrating rastermap and facemap to visualize behavioral representations. See the student/teacher versions [here](https://github.com/MouseLand/course-materials/tree/main/behavior_encoding).
 
 All demo data available [here](https://osf.io/xn4cm/).
 
 Here is what the output looks like for a segment of a mesoscope recording in a mouse during spontaneous activity (3.2Hz sampling rate), compared to random neural sorting:
 
 <img src="https://www.suite2p.org/static/images/rastermap_spont.png" width="800" alt="random sorting and rastermap sorting of spontaneous activity"/>
 
@@ -50,15 +62,15 @@
 
 # Installation
 
 ## Local installation (< 2 minutes)
 
 ### System requirements
 
-Linux, Windows and Mac OS are supported for running the code. For running the graphical interface you will need a Mac OS later than Yosemite. At least 8GB of RAM is recommended to run the software. 16GB-32GB may be required for larger datasets. The software has been heavily tested on Windows 10 and Ubuntu 20.04 and less well-tested on Mac OS. Please open an [issue](https://github.com/MouseLand/rastermap/issues) if you have problems with installation.
+Linux, Windows and Mac OS are supported for running the code. For running the graphical interface in Mac, you will need a Mac OS later than Yosemite. At least 8GB of RAM is recommended to run the software. 16GB-32GB may be required for larger datasets. The software has been heavily tested on Windows 10 and Ubuntu 20.04 and less well-tested on Mac OS. Please open an [issue](https://github.com/MouseLand/rastermap/issues) if you have problems with installation.
 
 ### Instructions
 
 Recommended to install an [Anaconda](https://www.anaconda.com/download/) distribution of Python -- Choose **Python 3.x** and your operating system. Note you might need to use an anaconda prompt (windows) if you did not add anaconda to the path. Open an anaconda prompt / command prompt with **python 3** in the path, then:
 
 ~~~sh
 pip install rastermap
@@ -145,20 +157,20 @@
 
 # spks is neurons by time
 spks = np.load("spks.npy").astype("float32")
 spks = zscore(spks, axis=1)
 
 # fit rastermap
 model = Rastermap(n_PCs=200, n_clusters=100, 
-                  locality=0.75, time_lag_window=5).fit(spks)
+                  locality=0.75, time_lag_window=5).fit(spks, compute_X_embedding=True)
 y = model.embedding # neurons x 1
 isort = model.isort
 
-# bin over neurons
-X_embedding = zscore(utils.bin1d(spks, bin_size=25, axis=0), axis=1)
+# visualize binning over neurons
+X_embedding = model.X_embedding
 
 # plot
 fig = plt.figure(figsize=(12,5))
 ax = fig.add_subplot(111)
 ax.imshow(X_embedding, vmin=0, vmax=1.5, cmap="gray_r", aspect="auto")
 ```
 
@@ -174,14 +186,34 @@
 
 Save an "ops.npy" file with the parameters and a "spks.npy" file with a matrix of neurons by time, and run
 
 ~~~sh
 python -m rastermap --S spks.npy --ops ops.npy
 ~~~
 
+## From MATLAB
+If you have an existing MATLAB analysis pipeline (and are using MATLAB version R2021b or newer), you can use MATLAB's Python interface to call Rastermap. First you need to tell MATLAB where your Python enviroment with Rastermap is (more details: https://www.mathworks.com/help/matlab/matlab_external/install-supported-python-implementation.html). Create or modify the "PYTHONHOME" environmental variable in your OS to point to the Rastermap environment root folder. Then in MATLAB run the following statement, modified for the specific path to your Rastermap environment pythonw executable:
+
+```
+pyenv('Version','C:\Users\admin\.conda\envs\rastermap\pythonw.exe', 'ExecutionMode', 'OutOfProcess')
+```
+Then you should be able to see your environment details in MATLAB after typing "pyenv" (the intepreter will not actually load until you try to run a Python statement). An example function to call Rastermap and return the sort order back as a MATLAB array is:
+```
+function [sortIdx] = rastermapSort(shankDataToSort)
+% wrapper to convert to numpy array, call Rastermap, and then convert back to MATLAB array
+
+ data = shankDataToSort.zScoredFiringRates; 
+ dataNdArray = py.numpy.array(data);
+ pyrun("from rastermap import Rastermap") %load interpreter, import main function
+ rmModel = pyrun("model = Rastermap(locality=0.5, time_lag_window=50).fit(spks)", "model", spks=dataNdArray);
+ sortIdx = int16(py.memoryview(rmModel.isort.data)) + 1; %back to MATLAB array, 1-indexing
+
+end
+```
+
 # Inputs
 
 Most of the time you will input to `Rastermap().fit` a matrix of neurons by time. For more details, these are all the inputs to the function:
 
 * **data** : array, shape (n_samples, n_features) (optional, default None) 
             this matrix is usually neurons/voxels by time, or None if using decomposition, 
             e.g. as in widefield imaging
```

### Comparing `rastermap-0.9.4/rastermap.egg-info/SOURCES.txt` & `rastermap-0.9.5/rastermap.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE
 README.md
 codecov.yml
 conftest.py
 setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
+notebooks/rastermap_interactive.ipynb
 notebooks/rastermap_largescale.ipynb
 notebooks/rastermap_singleneurons.ipynb
 notebooks/rastermap_widefield.ipynb
 notebooks/rastermap_zebrafish.ipynb
 notebooks/tutorial.ipynb
 paper/fig1.ipynb
 paper/fig1.py
@@ -18,22 +19,28 @@
 paper/fig2.py
 paper/fig3.ipynb
 paper/fig3.py
 paper/fig4.ipynb
 paper/fig4.py
 paper/fig5.ipynb
 paper/fig5.py
-paper/fig_splitting.py
+paper/fig6.ipynb
+paper/fig6.py
+paper/fig7.ipynb
+paper/fig7.py
+paper/fig8.ipynb
+paper/fig8.py
 paper/fig_utils.py
 paper/loaders.py
 paper/metrics.py
 paper/other_upsampling.py
 paper/qrdqn.py
 paper/simulations.py
 paper/splitting.ipynb
+paper/svca.ipynb
 rastermap/__init__.py
 rastermap/__main__.py
 rastermap/cluster.py
 rastermap/io.py
 rastermap/rastermap.py
 rastermap/sort.py
 rastermap/svd.py
```

### Comparing `rastermap-0.9.4/setup.py` & `rastermap-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/tests/test_rastermap.py` & `rastermap-0.9.5/tests/test_rastermap.py`

 * *Files identical despite different names*

### Comparing `rastermap-0.9.4/tox.ini` & `rastermap-0.9.5/tox.ini`

 * *Files identical despite different names*

