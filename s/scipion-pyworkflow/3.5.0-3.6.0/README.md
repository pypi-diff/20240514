# Comparing `tmp/scipion-pyworkflow-3.5.0.tar.gz` & `tmp/scipion_pyworkflow-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-pyworkflow-3.5.0.tar", last modified: Mon Mar 18 08:34:58 2024, max compression
+gzip compressed data, was "scipion_pyworkflow-3.6.0.tar", last modified: Tue May 14 08:21:37 2024, max compression
```

## Comparing `scipion-pyworkflow-3.5.0.tar` & `scipion_pyworkflow-3.6.0.tar`

### file list

```diff
@@ -1,183 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.161612 scipion-pyworkflow-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-18 08:34:58.161612 scipion-pyworkflow-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.133612 scipion-pyworkflow-3.5.0/pyworkflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.137612 scipion-pyworkflow-3.5.0/pyworkflow/apps/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_protocol_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_protocol_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_schedule_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_sync_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19081 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.141612 scipion-pyworkflow-3.5.0/pyworkflow/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25379 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    41175 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)    35654 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)   103376 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/graph_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/matplotlib_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.141612 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    19197 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/searchprotocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/searchrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    22545 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewprojects.py
--rw-r--r--   0 runner    (1001) docker     (127)    83036 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewprotocols.py
--rw-r--r--   0 runner    (1001) docker     (127)    21278 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewprotocols_extra.py
--rw-r--r--   0 runner    (1001) docker     (127)    28483 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)    23023 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.141612 scipion-pyworkflow-3.5.0/pyworkflow/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/mapper/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    62044 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/mapper/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/mapper/sqlite_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/mapper/xmlmapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    54000 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/object.py
--rw-r--r--   0 runner    (1001) docker     (127)    28507 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.145612 scipion-pyworkflow-3.5.0/pyworkflow/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    81601 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.145612 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/clean_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2942 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/edit_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/fix_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      941 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/stack2volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.145612 scipion-pyworkflow-3.5.0/pyworkflow/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/package.py
--rw-r--r--   0 runner    (1001) docker     (127)    26337 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    95033 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.153612 scipion-pyworkflow-3.5.0/pyworkflow/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/Imagej.png
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/chimera.png
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/fa-exclamation-triangle_alert.png
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/fa-info-circle_alert.png
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/fa-search.png
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/fa-times-circle_alert.png
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/file_vol.png
--rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/loading.gif
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/no-image128.png
--rw-r--r--   0 runner    (1001) docker     (127)   113916 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_bn.png
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)   126140 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon_proj.png
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon_projs.png
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon_prot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_logo_normal.png
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_logo_small.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.153612 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/arrowDown.png
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/arrowUp.png
--rw-r--r--   0 runner    (1001) docker     (127)   284666 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/background_section.png
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/colRowModeOff.png
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/colRowModeOn.png
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/delete.png
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/doc_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/download_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/enabled_gallery.png
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/galleryViewOff.png
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/galleryViewOn.png
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/goto.png
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/menu.png
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/separator.png
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/tableViewOff.png
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/tableViewOn.png
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/volumeOff.png
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/volumeOn.png
--rw-r--r--   0 runner    (1001) docker     (127)    53903 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/sprites.png
--rw-r--r--   0 runner    (1001) docker     (127)    93331 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/sprites.xcf
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/resources/wait.gif
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.157612 scipion-pyworkflow-3.5.0/pyworkflow/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.157612 scipion-pyworkflow-3.5.0/pyworkflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14943 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/echo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    23223 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)    25979 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/utils/which.py
--rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.157612 scipion-pyworkflow-3.5.0/pyworkflow/webservices/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/webservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/webservices/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/webservices/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/webservices/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflow/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.157612 scipion-pyworkflow-3.5.0/pyworkflowtests/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.161612 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_canvas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1624 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_mappers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18393 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_protocol_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_protocol_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_protocol_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:34:58.161612 scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-18 08:34:58.000000 scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-03-18 08:34:58.000000 scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-18 08:34:58.000000 scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-18 08:34:58.000000 scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-18 08:34:58.000000 scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-18 08:34:58.000000 scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 08:34:58.161612 scipion-pyworkflow-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-03-18 08:34:49.000000 scipion-pyworkflow-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.746500 scipion_pyworkflow-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-14 08:21:37.746500 scipion_pyworkflow-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.718500 scipion_pyworkflow-3.6.0/pyworkflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.718500 scipion_pyworkflow-3.6.0/pyworkflow/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_protocol_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_protocol_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_schedule_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_sync_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20747 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.722500 scipion_pyworkflow-3.6.0/pyworkflow/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25590 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41175 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34982 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103376 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/graph_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20629 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/matplotlib_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.726500 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18672 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/searchprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/searchrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22516 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewprojects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83036 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewprotocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewprotocols_extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28483 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23023 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.726500 scipion_pyworkflow-3.6.0/pyworkflow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/mapper/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63145 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/mapper/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/mapper/sqlite_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/mapper/xmlmapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53991 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29371 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.726500 scipion_pyworkflow-3.6.0/pyworkflow/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81601 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.730500 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/clean_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2942 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/edit_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/fix_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      941 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/stack2volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.730500 scipion_pyworkflow-3.6.0/pyworkflow/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26337 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95369 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.734500 scipion_pyworkflow-3.6.0/pyworkflow/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/Imagej.png
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/chimera.png
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/fa-exclamation-triangle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/fa-info-circle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/fa-search.png
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/fa-times-circle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/file_vol.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16824 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/no-image128.png
+-rw-r--r--   0 runner    (1001) docker     (127)   113916 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_bn.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   126140 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon_proj.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon_projs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon_prot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_logo_normal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_logo_small.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.738500 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/arrowDown.png
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/arrowUp.png
+-rw-r--r--   0 runner    (1001) docker     (127)   284666 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/background_section.png
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/colRowModeOff.png
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/colRowModeOn.png
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/doc_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/download_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/enabled_gallery.png
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/galleryViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/galleryViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/goto.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/separator.png
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/tableViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/tableViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/volumeOff.png
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/volumeOn.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53903 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/sprites.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93331 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/sprites.xcf
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/resources/wait.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.738500 scipion_pyworkflow-3.6.0/pyworkflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.742500 scipion_pyworkflow-3.6.0/pyworkflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14943 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26319 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/utils/which.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.742500 scipion_pyworkflow-3.6.0/pyworkflow/webservices/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/webservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/webservices/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/webservices/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/webservices/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflow/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.742500 scipion_pyworkflow-3.6.0/pyworkflowtests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.746500 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_canvas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1624 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16170 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_mappers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18494 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_protocol_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_protocol_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_protocol_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:21:37.746500 scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-14 08:21:37.000000 scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-14 08:21:37.000000 scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 08:21:37.000000 scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 08:21:37.000000 scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-14 08:21:37.000000 scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 08:21:37.000000 scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:21:37.746500 scipion_pyworkflow-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-14 08:21:29.000000 scipion_pyworkflow-3.6.0/setup.py
```

### Comparing `scipion-pyworkflow-3.5.0/LICENSE.txt` & `scipion_pyworkflow-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/PKG-INFO` & `scipion_pyworkflow-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-pyworkflow
-Version: 3.5.0
+Version: 3.6.0
 Summary: Simple workflow platform used in scientific applications, initially developed within the Scipion framework for image processing in Electron Microscopy.
 Home-page: https://github.com/scipion-em/scipion-pyworkflow
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-pyworkflow/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-pyworkflow/
 Keywords: workflows science electron-microscopy cryo-em structural-biology image-processing scipion
```

### Comparing `scipion-pyworkflow-3.5.0/README.rst` & `scipion_pyworkflow-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_manager.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_plot.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_plot.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_project.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_protocol_list.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_protocol_list.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_protocol_run.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_protocol_run.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_run_tests.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_run_tests.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_schedule_run.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_schedule_run.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_sleep.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_sleep.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_sync_data.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_sync_data.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/apps/pw_viewer.py` & `scipion_pyworkflow-3.6.0/pyworkflow/apps/pw_viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/config.py` & `scipion_pyworkflow-3.6.0/pyworkflow/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import enum
 import logging
+
 logger = logging.getLogger(__file__)
 import ast
 import importlib
 import inspect
-import json
 import os
 import shutil
 import sys
 import types
 from .constants import *
 
 HOME = os.path.abspath(os.path.dirname(__file__))
@@ -61,75 +60,115 @@
 
 
 def getModuleFolder(moduleName):
     """ Returns the path of a module without importing it"""
     spec = importlib.util.find_spec(moduleName)
     return os.path.dirname(spec.origin)
 
-class VarTypes(enum.Enum):
-    STRING = 1
-    INTEGER = 2
-    BOOLEAN = 3
-    PATH = 4
-
-class Variable(object):
-    """ Class for variables of the Config class."""
-    def __init__(self, value, varType:VarTypes=VarTypes.STRING):
-        """
-        :param value: Value of the variable
-        :param type: Type of the variable"""
-        super().__init__()
+
+def validColor(colorname):
+    """ If it can be converted to rgb is a valid color"""
+    from matplotlib.colors import to_rgb
+    to_rgb(colorname)
+    return colorname
+
+class VarTypes(Enum):
+    STRING = 0
+    BOOLEAN = 1
+    PATH = 2  # Any Path: Folder or file
+    INTEGER = 3
+    DECIMAL = 4
+    FILENAME = 5  # Just the base name of a file
+    FOLDER = 6  # A folder
+
+class Variable:
+    def __init__(self, name, description, source, value, default, var_type: VarTypes = VarTypes.STRING, isDefault=None):
+        self.name = name
+        self.description = description
+        self.source = source
         self.value = value
-        self.varType = varType
-    def __bool__(self):
-        return bool(self.value)
-
-    def __int__(self):
-        return int(self.value)
-    def __str__(self):
-        return str(self.value)
-
-    def __eq__(self, other):
-        return other == self.value
-
-    def __repr__(self):
-        return self.__str__()
-
-    def __fspath__(self):
-        return self.__str__()
-
-    " We migth need to imlement more like this--> https://docs.python.org/3.3/reference/datamodel.html#object.__truediv__"
-    def __truediv__(self, other):
-        return float(self.value)/other
-
-    def __rtruediv__(self, other):
-        return  other / float(self.value)
-
-    def __add__(self, other):
-        return self.value+other
-    def __radd__(self, other):
-        return other+self.value
+        self.default = default
+        self.var_type = var_type
+        self.isDefault = isDefault if isDefault is not None else value==default
+    def setToDefault(self):
+        self.isDefault=True
+        self.value=self.default
+
+class VariablesRegistry:
+    _variables={}
+
+    def __init__(self):
+        raise RuntimeError("Variables class doesn't need to be instantiated.")
+    @classmethod
+    def register(cls, variable: Variable):
+        cls._variables[variable.name] = variable
+
+    @classmethod
+    def variables(cls):
+        return cls._variables
+
+    @classmethod
+    def __iter__(cls):
+        """ Iterate alphabetically"""
+        for key in sorted(cls._variables):
+            yield cls._variables[key]
+
+    @classmethod
+    def save(cls, path):
+        """ Saves the variables in the path specified """
+        from pyworkflow.utils import backup
+        backup(path)
+
+        with open(path,"w") as fh:
+            # Save the section as in any python config file format.
+            fh.write("[PYWORKFLOW]\n")
+            for var in cls.__iter__():
+                if var.source == "pyworkflow" and not var.isDefault:
+                    fh.write("%s=%s\n" % (var.name, var.value))
+
+            fh.write("\n[PLUGINS]\n")
+            for var in cls._variables.values():
+                if var.source != "pyworkflow" and not var.isDefault:
+                    fh.write("%s=%s\n" % (var.name, var.value))
+
 
 class Config:
     """ Main Config for pyworkflow. It contains the main Scipion configuration variables
     providing default values or, if present, taking them from the environment.
     Necessary value is SCIPION_HOME and has to be present in the environment"""
 
     @staticmethod
-    def __get(key, default):
-        value = os.environ.get(key, default)
+    def __get(key, default, description=None, caster=None, var_type:VarTypes=VarTypes.STRING, source="pyworkflow"):
+
+        if key in os.environ:
+            value = os.environ.get(key)
+            isDefault = (value==default)
+        else:
+            isDefault = True
+            value = default
 
+        # If the caster is passed do the casting, if fails go back to default
+        if caster:
+            try:
+                value=caster(value)
+            except:
+                logger.warning("Variable %s has this value %s that can't be casted to the right type (%s). Using %s (default value)" %
+                               (key,value, caster, default))
+                value = default
         # If empty use default value
         if value == "" != default:
             logger.warning("%s variable is empty, falling back to default value (%s)" % (key, default))
             value = default
+
         # Expand user and variables if string value
         if isinstance(value, str):
             value = os.path.expandvars(os.path.expanduser(value))
 
+        # Register the variable
+        VariablesRegistry.register(Variable(key,description, source, value, default, var_type=var_type, isDefault=isDefault))
         return value
 
     class Root:
         """ Simple helper to return path from a root. """
 
         def __init__(self, root):
             self._root = root
@@ -139,187 +178,186 @@
             expanded = os.path.expanduser(os.path.join(*path))
 
             # join will not join if expanded is absolute
             return os.path.join(self._root, expanded)
 
     # Home for scipion
     _get = __get.__func__
-    SCIPION_HOME = os.path.abspath(_get(SCIPION_HOME_VAR, ''))
-    "Path where Scipion is installed. Other paths are based on this like SCIPION_SOFTWARE, SCIPION_TESTS,... unless specified"
+    SCIPION_HOME = os.path.abspath(_get(SCIPION_HOME_VAR, '',
+    "Path where Scipion is installed. Other paths are based on this like SCIPION_SOFTWARE, SCIPION_TESTS,... unless specified"))
 
-    # Actual SCIPION_HOME
-    SCIPION_HOME_DEFINED = _get(SCIPION_HOME_VAR, False)
-    "False if SCIPION_HOME is not found in the environment"
+    # False if SCIPION_HOME is not found in the environment. To distinguish API documentation generation execution.
+    SCIPION_HOME_DEFINED = SCIPION_HOME != ''
 
     _root = Root(str(SCIPION_HOME))
     _join = _root.join
 
     # Internal cached variables, use __ so they are not returned in getVars
     __activeColor = None
 
-    CONDA_ACTIVATION_CMD = _get(CONDA_ACTIVATION_CMD_VAR,'')
-    "str: Command to activate/initialize conda itself. Do not confuse it with 'conda activate'. It should be defined at installation time. It looks like this: eval \"$(/extra/miniconda3/bin/conda shell.bash hook)\""
+    CONDA_ACTIVATION_CMD = _get(CONDA_ACTIVATION_CMD_VAR,'',
+    "str: Command to activate/initialize conda itself. Do not confuse it with 'conda activate'. It should be defined at installation time. It looks like this: eval \"$(/extra/miniconda3/bin/conda shell.bash hook)\"")
 
     # SCIPION PATHS
-    SCIPION_SOFTWARE = _join(_get('SCIPION_SOFTWARE', 'software'))
-    "Path where Scipion will install the software. Defaults to SCIPION_HOME/software."
+    SCIPION_SOFTWARE = _get('SCIPION_SOFTWARE', _join('software'),
+    "Path where Scipion will install the software. Defaults to SCIPION_HOME/software.", var_type=VarTypes.FOLDER)
 
-    SCIPION_TESTS = _join(_get('SCIPION_TESTS', os.path.join('data', 'tests')))
-    "Path where to find/download test data. Defaults to SCIPION_HOME/data/tests."
+    SCIPION_TESTS = _get('SCIPION_TESTS', _join('data', 'tests'),
+    "Path where to find/download test data. Defaults to SCIPION_HOME/data/tests.", var_type=VarTypes.FOLDER)
 
     # User dependent paths
-    SCIPION_USER_DATA = _get('SCIPION_USER_DATA', '~/ScipionUserData')
-    "Path where Scipion projects are or will be created. Defaults to ~/ScipionUserData"
-
-    SCIPION_TMP = _get('SCIPION_TMP', _join(SCIPION_USER_DATA, 'tmp'))
-    "General purpose scipion tmp folder. Defaults to SCIPION_USER_DATA/tmp"
+    SCIPION_USER_DATA = _get('SCIPION_USER_DATA', '~/ScipionUserData',
+    "Path where Scipion projects are or will be created. Defaults to ~/ScipionUserData", var_type=VarTypes.FOLDER)
 
     # LOGGING variables
-    SCIPION_LOGS = _get('SCIPION_LOGS', _join(SCIPION_USER_DATA, 'logs'))
-    "Path for Scipion logs folder used by the GUI. Defaults to SCIPION_USER_DATA/logs."
+    SCIPION_LOGS = _get('SCIPION_LOGS', _join(SCIPION_USER_DATA, 'logs'),
+    "Folder for Scipion logs used by the GUI. Defaults to SCIPION_USER_DATA/logs.", var_type=VarTypes.FOLDER)
 
-    SCIPION_LOG_CONFIG = _get('SCIPION_LOG_CONFIG', None)
-    "Optional. Path to a python logging configuration file fine tune the logging."
+    SCIPION_LOG_CONFIG = _get('SCIPION_LOG_CONFIG', None,
+    "Optional. Path to a python logging configuration file to fine tune the logging.", var_type=VarTypes.PATH)
 
-    SCIPION_LOG = _join(SCIPION_LOGS, 'scipion.log')
-    "Path to the file where scipion will write GUI logging messages. Defaults to SCIPION_LOGS/scipion.log"
+    SCIPION_LOG = _get('SCIPION_LOG', _join(SCIPION_LOGS, 'scipion.log'),
+    "Path to the file where scipion will write GUI logging messages. Defaults to SCIPION_LOGS/scipion.log", var_type=VarTypes.PATH)
 
-    SCIPION_LOG_FORMAT = _get('SCIPION_LOG_FORMAT', "%(message)s")
-    "str: Format for all the log lines, defaults to %(message)s. To compose the format see https://docs.python.org/3/library/logging.html#logrecord-attributes"
+    SCIPION_LOG_FORMAT = _get('SCIPION_LOG_FORMAT', "%(message)s",
+    "str: Format for all the log lines, defaults to %(message)s. To compose the format see https://docs.python.org/3/library/logging.html#logrecord-attributes")
 
-    SCIPION_LOG_LEVEL = _get(SCIPION_LOG_LEVEL, 'INFO')
-    "Default logging level. String among CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET. Default value is INFO."
+    SCIPION_LOG_LEVEL = _get(SCIPION_LOG_LEVEL, 'INFO',
+    "Default logging level. String among CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET. Default value is INFO.")
 
-    NO_COLOR = _get('NO_COLOR', '')
-    "str: Comply with https://no-color.org/ initiative. Set it to something different than '' to deactivate colors in the output."
+    NO_COLOR = _get('NO_COLOR', '',
+    "str: Comply with https://no-color.org/ initiative. Set it to something different than '' to deactivate colors in the output.")
 
-    SCIPION_SCRATCH = _get(SCIPION_SCRATCH, None)
-    "Optional. Path to a location mounted in a scratch drive (SSD,...)"
+    SCIPION_SCRATCH = _get(SCIPION_SCRATCH, None,
+    "Optional. Path to a location mounted in a scratch drive (SSD,...)")
 
-    SCIPION_TESTS_OUTPUT = _get('SCIPION_TESTS_OUTPUT', _join(SCIPION_USER_DATA, 'Tests'))
-    "Path to a folder Where the output of the tests will be written. Defaults to SCIPION_USER_DATA/Tests."
+    SCIPION_TESTS_OUTPUT = _get('SCIPION_TESTS_OUTPUT', _join(SCIPION_USER_DATA, 'Tests'),
+    "Path to a folder where the output of the tests will be written. Defaults to SCIPION_USER_DATA/Tests.", var_type=VarTypes.FOLDER)
 
-    SCIPION_TEST_NOSYNC = _get('SCIPION_TEST_NOSYNC', FALSE_STR) != FALSE_STR
-    "Set it to 1, True, Yes or y to cancel test dataset synchronization. Needed when updating files in a dataset."
+    SCIPION_TEST_NOSYNC = _get('SCIPION_TEST_NOSYNC', FALSE_STR,
+    "Set it to 1, True, Yes or y to cancel test dataset synchronization. Needed when updating files in a dataset.") != FALSE_STR
 
-    SCIPION_SUPPORT_EMAIL = _get('SCIPION_SUPPORT_EMAIL', 'scipion@cnb.csic.es')
+    SCIPION_SUPPORT_EMAIL = 'scipion@cnb.csic.es'
 
     # Config variables
-    SCIPION_CONFIG = _get('SCIPION_CONFIG', 'scipion.conf')
-    "Path to the scipion configuration file where all this variables could be defined."
+    SCIPION_CONFIG = _get('SCIPION_CONFIG', _join('config','scipion.conf'),
+    "Path to the scipion configuration file where all this variables could be defined.", var_type=VarTypes.PATH)
 
-    SCIPION_LOCAL_CONFIG = _get('SCIPION_LOCAL_CONFIG', SCIPION_CONFIG)
-    "Path to an optional/extra/user configuration file meant to overwrite default variables."
+    SCIPION_LOCAL_CONFIG = _get('SCIPION_LOCAL_CONFIG', SCIPION_CONFIG,
+    "Path to an optional/extra/user configuration file meant to overwrite default variables.", var_type=VarTypes.PATH)
 
-    SCIPION_HOSTS = _get('SCIPION_HOSTS', 'hosts.conf')
-    "Path to the host.cof file to allow scipion to use queue engines and run in HPC environments."
+    SCIPION_HOSTS = _get('SCIPION_HOSTS', _join('config','hosts.conf'),
+    "Path to the host.cof file to allow scipion to use queue engines and run in HPC environments.")
 
-    SCIPION_PROTOCOLS = _get('SCIPION_PROTOCOLS', 'protocols.conf')
-    ""
+    SCIPION_PROTOCOLS = _get('SCIPION_PROTOCOLS', _join('config','protocols.conf'),
+    "Custom conf file to extend the protocols tree view panel (panel on the left)")
 
-    SCIPION_PLUGIN_JSON = _get('SCIPION_PLUGIN_JSON', None)
-    "Optional. Path to get the json file with all the plugins available for Scipion."
+    SCIPION_PLUGIN_JSON = _get('SCIPION_PLUGIN_JSON', None,
+    "Optional. Path to get the json file with all the plugins available for Scipion.")
 
     SCIPION_PLUGIN_REPO_URL = _get('SCIPION_PLUGIN_REPO_URL',
-                                   'http://scipion.i2pc.es/getplugins/')
-    "Url from where to get the list of plugins."
+                                   'https://scipion.i2pc.es/getplugins/',
+    "Url from where to get the list of plugins.")
 
     # REMOTE Section
-    SCIPION_URL = _get('SCIPION_URL', 'http://scipion.cnb.csic.es/downloads/scipion')
-    SCIPION_URL_SOFTWARE = _get('SCIPION_URL_SOFTWARE', SCIPION_URL + '/software')
-    SCIPION_URL_TESTDATA = _get('SCIPION_URL_TESTDATA', SCIPION_URL + '/data/tests')
+    SCIPION_URL = 'https://scipion.cnb.csic.es/downloads/scipion'
+    SCIPION_URL_SOFTWARE = SCIPION_URL + '/software'
+    SCIPION_URL_TESTDATA = SCIPION_URL + '/data/tests'
 
     # Scipion Notes
-    SCIPION_NOTES_FILE = _get(SCIPION_NOTES_FILE, 'notes.txt')
-    "Name of the file where to write per project notes."
+    SCIPION_NOTES_FILE = _get(SCIPION_NOTES_FILE, 'notes.txt',
+    "Name of the file where to write per project notes.")
 
-    SCIPION_NOTES_PROGRAM = _get(SCIPION_NOTES_PROGRAM, None)
-    "Command or program to use to open the notes file. Otherwise system will extension association will take place."
+    SCIPION_NOTES_PROGRAM = _get(SCIPION_NOTES_PROGRAM, None,
+    "Command or program to use to open the notes file. Otherwise system will extension association will take place.")
 
     SCIPION_NOTES_ARGS = _get(SCIPION_NOTES_ARGS, None)
 
     # Aspect
-    SCIPION_FONT_NAME = _get('SCIPION_FONT_NAME', "Helvetica")
-    "Name of the font to use in Scipion GUI. Defaults to Helvetica."
+    SCIPION_FONT_NAME = _get('SCIPION_FONT_NAME', "Helvetica",
+    "Name of the font to use in Scipion GUI. Defaults to Helvetica.")
 
-    SCIPION_FONT_SIZE = int(_get('SCIPION_FONT_SIZE', SCIPION_DEFAULT_FONT_SIZE))
-    "Size of the 'normal' font to be used in Scipion GUI. Defaults to 10."
+    SCIPION_FONT_SIZE = _get('SCIPION_FONT_SIZE', SCIPION_DEFAULT_FONT_SIZE,
+    "Size of the 'normal' font to be used in Scipion GUI. Defaults to 10.", caster=int)
 
-    SCIPION_MAIN_COLOR = _get('SCIPION_MAIN_COLOR', Color.MAIN_COLOR)
-    "str: Main color of the GUI. Background will be white, so for better contrast choose a dark color. Probably any name here will work: https://matplotlib.org/stable/gallery/color/named_colors.html"
+    SCIPION_MAIN_COLOR = _get('SCIPION_MAIN_COLOR', Color.MAIN_COLOR,
+    "str: Main color of the GUI. Background will be white, so for better contrast choose a dark color. Probably any name here will work: https://matplotlib.org/stable/gallery/color/named_colors.html",
+                              caster=validColor)
 
-    SCIPION_BG_COLOR = _get('SCIPION_BG_COLOR', Color.BG_COLOR)
-    "str: Main background color of the GUI. Default is white, chose a light one. Probably any name here will work: https://matplotlib.org/stable/gallery/color/named_colors.html"
+    SCIPION_BG_COLOR = _get('SCIPION_BG_COLOR', Color.BG_COLOR,
+    "str: Main background color of the GUI. Default is white, chose a light one. Probably any name here will work: https://matplotlib.org/stable/gallery/color/named_colors.html",
+                            validColor)
 
-    WIZARD_MASK_COLOR = _get('WIZARD_MASK_COLOR', '[0.125, 0.909, 0.972]')
-    "Color to use in some wizards."
+    SCIPION_CONTRAST_COLOR = _get('SCIPION_CONTRAST_COLOR', 'cyan',
+    "Color used to highlight features over grayscaled images.", caster=validColor)
 
-    SCIPION_SPRITES_FILE = _get('SCIPION_SPRITES_FILE', _join(getResourcesPath(),'sprites.png'))
-    "File (png) with the icons in a collage. Default is found at pyworkflow/resources/sprites.png. And a GIMP file could be found at the same folder in the github repo."
+    SCIPION_SPRITES_FILE = _get('SCIPION_SPRITES_FILE', _join(getResourcesPath(),'sprites.png'),
+    "File (png) with the icons in a collage. Default is found at pyworkflow/resources/sprites.png. And a GIMP file could be found at the same folder in the github repo.")
 
-    SCIPION_SHOW_TEXT_IN_TOOLBAR = _get('SCIPION_SHOW_TEXT_IN_TOOLBAR', TRUE_STR) == TRUE_STR
-    "Define it to anything else except False to show the label of the icons. It will take more space."
+    SCIPION_SHOW_TEXT_IN_TOOLBAR = _get('SCIPION_SHOW_TEXT_IN_TOOLBAR', TRUE_STR,
+    "Define it to anything else except False to show the label of the icons. It will take more space.") == TRUE_STR
 
-    SCIPION_ICON_ZOOM = int(_get('SCIPION_ICON_ZOOM', 50))
-    "Define it to anything else except False to show the label of the icons. It will take more space."
+    SCIPION_ICON_ZOOM = _get('SCIPION_ICON_ZOOM', 50,
+    "Define it to anything else except False to show the label of the icons. It will take more space.", var_type=VarTypes.INTEGER, caster=int)
 
     # Notification
-    SCIPION_NOTIFY = _get('SCIPION_NOTIFY', TRUE_STR) == TRUE_STR
-    "If set to False, Scipion developers will know almost nothing about Scipion usage and will have less information to improve it."
+    SCIPION_NOTIFY = _get('SCIPION_NOTIFY', TRUE_STR,
+    "If set to False, Scipion developers will know almost nothing about Scipion usage and will have less information to improve it.") == TRUE_STR
 
     # *** Execution variables ***
-    SCIPION_CWD = _get('SCIPION_CWD', os.path.abspath(os.getcwd()))
-    "Directory when scipion was launched"
+    SCIPION_CWD = _get('SCIPION_CWD', os.path.abspath(os.getcwd()),
+    "Directory when scipion was launched")
 
-    SCIPION_GUI_REFRESH_IN_THREAD = _get('SCIPION_GUI_REFRESH_IN_THREAD', FALSE_STR) != FALSE_STR
-    "True to refresh the runs graph with a thread. Unstable."
+    SCIPION_GUI_REFRESH_IN_THREAD = _get('SCIPION_GUI_REFRESH_IN_THREAD', FALSE_STR,
+    "True to refresh the runs graph with a thread. Unstable.") != FALSE_STR
 
-    SCIPION_GUI_REFRESH_INITIAL_WAIT = int(_get("SCIPION_GUI_REFRESH_INITIAL_WAIT", 5))
-    "Seconds to wait after a manual refresh"
+    SCIPION_GUI_REFRESH_INITIAL_WAIT = _get("SCIPION_GUI_REFRESH_INITIAL_WAIT", 5,
+    "Seconds to wait after a manual refresh", caster=int)
 
-    SCIPION_GUI_CANCEL_AUTO_REFRESH = _get("SCIPION_GUI_CANCEL_AUTO_REFRESH",FALSE_STR) != FALSE_STR
-    "Set it to True to cancel automatic refresh of the runs."
+    SCIPION_GUI_CANCEL_AUTO_REFRESH = _get("SCIPION_GUI_CANCEL_AUTO_REFRESH",FALSE_STR,
+    "Set it to True to cancel automatic refresh of the runs.") != FALSE_STR
 
     # Cancel shutil fast copy. In GPFS, shutil.copy does fail when trying a fastcopy and does not
-    # fallback on the slow copy. For legacy reasons None is also False.
-    SCIPION_CANCEL_FASTCOPY = _get('SCIPION_CANCEL_FASTCOPY', FALSE_STR) not in [NONE_STR, FALSE_STR]
+    # fall back on the slow copy. For legacy reasons None is also False.
+    SCIPION_CANCEL_FASTCOPY = _get('SCIPION_CANCEL_FASTCOPY', FALSE_STR,
     "Cancel fast copy done by shutil (copying files) when it fails. Has happened in GPFS environments. Defaults to False. None is also False otherwise fastcopy is cancelled."
+                                   ) not in [NONE_STR, FALSE_STR]
 
     # Priority package list: This variable is used in the view protocols in
     # order to load first the plugins that contains the main protocols.conf
     # sections, so other plugins can define only their sections avoiding
     # duplicating all the sections in all plugins. Scipion app is currently defining it for em tomo and chem
     SCIPION_PRIORITY_PACKAGE_LIST = _get('SCIPION_PRIORITY_PACKAGE_LIST', EMPTY_STR)
 
-    SCIPION_STEPS_CHECK_SEC = int(_get('SCIPION_STEPS_CHECK_SEC', 5))
-    "Number of seconds to wait before checking if new input is available in streamified protocols."
+    SCIPION_STEPS_CHECK_SEC = _get('SCIPION_STEPS_CHECK_SEC', 5,
+    "Number of seconds to wait before checking if new input is available in streamified protocols.", caster=int)
 
-    SCIPION_UPDATE_SET_ATTEMPTS = int(_get('SCIPION_UPDATE_SET_ATTEMPTS', 3))
-    "Number of attempts to modify the protocol output before failing. The default value is 3"
+    SCIPION_UPDATE_SET_ATTEMPTS = _get('SCIPION_UPDATE_SET_ATTEMPTS', 3,
+    "Number of attempts to modify the protocol output before failing. The default value is 3", caster=int)
 
-    SCIPION_UPDATE_SET_ATTEMPT_WAIT = int(_get('SCIPION_UPDATE_SET_ATTEMPT_WAIT', 2))
-    "Time in seconds to wait until the next attempt when checking new outputs. The default value is 2 seconds"
+    SCIPION_UPDATE_SET_ATTEMPT_WAIT = _get('SCIPION_UPDATE_SET_ATTEMPT_WAIT', 2,
+    "Time in seconds to wait until the next attempt when checking new outputs. The default value is 2 seconds", caster=int)
 
-    SCIPION_USE_QUEUE = _get("SCIPION_USE_QUEUE", FALSE_STR) != FALSE_STR
-    "Default value for using the queue. By default is False. ANY value will be True except and empty value. \"False\" or \"0\" will be True too."
+    SCIPION_USE_QUEUE = _get("SCIPION_USE_QUEUE", FALSE_STR,
+    "Default value for using the queue. By default is False. ANY value will be True except and empty value. \"False\" or \"0\" will be True too.")!= FALSE_STR
 
-    SCIPION_DEFAULT_EXECUTION_ACTION = int(_get('SCIPION_DEFAULT_EXECUTION_ACTION', DEFAULT_EXECUTION_ACTION_ASK))
+    SCIPION_DEFAULT_EXECUTION_ACTION = _get('SCIPION_DEFAULT_EXECUTION_ACTION', DEFAULT_EXECUTION_ACTION_ASK,
     """Ask if you want to launch a single protocol or a sub-workflow. The default value is 1
        1: Scipion always ask
        2: Run a single protocol
-       3: Run a sub-workflow """
+       3: Run a sub-workflow """, caster=int)
 
     try:
-        VIEWERS = ast.literal_eval(_get('VIEWERS', "{}"))
+        VIEWERS = ast.literal_eval(_get('VIEWERS', "{}", "Json string to define which viewer are the default ones per output type."))
     except Exception as e:
         VIEWERS = {}
         logger.error("ERROR loading preferred viewers, VIEWERS variable will be ignored", exc_info=e)
 
-    SCIPION_DOMAIN = _get(SCIPION_DOMAIN, None)
-    SCIPION_TESTS_CMD = _get(SCIPION_TESTS_CMD, getTestsScript())
+    SCIPION_DOMAIN = _get(SCIPION_DOMAIN, None, "Domain base class. Ignore.")
+    SCIPION_TESTS_CMD = _get(SCIPION_TESTS_CMD, getTestsScript(), "Command to run tests")
 
     # ---- Getters ---- #
     # Getters are alternatives to offer a variable, but preventing it to be stored in the config
     @classmethod
     def getLibFolder(cls):
         """
         :return: Folder where libraries must be placed in case a binding needs them
@@ -355,25 +393,19 @@
         """
         configVars = dict()
         # For each variable, also in base classes
         for baseCls in inspect.getmro(cls):
             for name, value in vars(baseCls).items():
                 # Skip methods and internal attributes starting with __
                 # (e.g __doc__, __module__, etc)
-                if isinstance(value, (str, int, Variable)) and not name.startswith('__'):
+                if isinstance(value, (str, int)) and not name.startswith('__'):
                     configVars[name] = str(value)
         return configVars
 
     @classmethod
-    def printVars(cls):
-        """ Print the variables' dict, mostly for debugging. """
-        from .utils import prettyDict
-        prettyDict(cls.getVars())
-
-    @classmethod
     def getDomain(cls):
         """ Import domain module from path or name defined in SCIPION_DOMAIN.
         """
         value = cls.SCIPION_DOMAIN
 
         if not value:
             return None
@@ -427,15 +459,17 @@
 
     @classmethod
     def getExternalJsonTemplates(cls):
         return os.path.dirname(cls.SCIPION_CONFIG)
 
     @classmethod
     def getWizardMaskColor(cls):
-        return json.loads(cls.WIZARD_MASK_COLOR)
+        """ Color is a name"""
+        from matplotlib.colors import to_rgb
+        return list(to_rgb(cls.SCIPION_CONTRAST_COLOR))
 
     @classmethod
     def getPriorityPackageList(cls):
         if cls.SCIPION_PRIORITY_PACKAGE_LIST != EMPTY_STR:
             return cls.SCIPION_PRIORITY_PACKAGE_LIST.split(" ")
         else:
             return []
@@ -459,24 +493,17 @@
 
 
     @classmethod
     def getActiveColor(cls):
         """ Returns a color lighter than the SCIPION_MAIN_COLOR"""
 
         if cls.__activeColor is None:
-            import matplotlib.colors
             from pyworkflow.utils import lighter, rgb_to_hex
-            try:
-                rgb_main = matplotlib.colors.to_rgb(cls.SCIPION_MAIN_COLOR)
-            except Exception:
-                logger.error("Cannot convert SCIPION_MAIN_COLOR (%s) string to a color to compute the lighter color."
-                             " Falling back to %s" % (Config.SCIPION_MAIN_COLOR, Color.MAIN_COLOR))
-                cls.SCIPION_MAIN_COLOR = Color.MAIN_COLOR
-                rgb_main = matplotlib.colors.to_rgb(cls.SCIPION_MAIN_COLOR)
-
+            from matplotlib.colors import to_rgb
+            rgb_main = to_rgb(cls.SCIPION_MAIN_COLOR)
             rgb_main = (rgb_main[0] * 255, rgb_main[1] * 255, rgb_main[2] * 255)
             rgb_active = lighter(rgb_main, 0.3)
             cls.__activeColor = rgb_to_hex(rgb_active)
 
         return cls.__activeColor
 
     @classmethod
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/constants.py` & `scipion_pyworkflow-3.6.0/pyworkflow/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 CORE_VERSION = '3.0.0'
 
 # Versions
 VERSION_1 = '1.0.0'
 VERSION_1_1 = '1.1.0'
 VERSION_1_2 = '1.2.0'
 VERSION_2_0 = '2.0.0'
-VERSION_3_0 = '3.5.0'
+VERSION_3_0 = '3.6.0'
 
 # For a new release, define a new constant and assign it to LAST_VERSION
 # The existing one has to be added to OLD_VERSIONS list.
 LAST_VERSION = VERSION_3_0
 OLD_VERSIONS = (VERSION_1, VERSION_1_1, VERSION_1_2, VERSION_2_0)
 
 # STATUS
@@ -178,15 +178,15 @@
 
 class DOCSITEURLS:
     """Documentation site URL useful when exceptions happen and you want to point to some pages"""
     HOME = 'https://scipion-em.github.io/docs/release-3.0.0/'
     DOCS = HOME + 'docs/'
     CONFIG = DOCS + 'scipion-modes/scipion-configuration.html'
     CONFIG_SECTION = CONFIG + '#%s'
-    CONTACTUS = 'http://scipion.i2pc.es/contact'
+    CONTACTUS = 'https://scipion.i2pc.es/contact'
     USER = DOCS + 'user/'
     GUI = USER + 'scipion-gui.html'
     WAIT_FOR = GUI + '#waiting-for-other-protocols'
     PLUGIN_MANAGER = USER + 'plugin-manager.html'
     HOST_CONFIG = DOCS + "scipion-modes/host-configuration.html"
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/browser.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,15 +328,15 @@
                 # Do not add hidden files if not requested
                 if not self._showHidden and f.startswith('.'):
                     continue
 
                 # All ok...add item.
                 fileInfoList.append(FileInfo(self._currentDir, f))
         except Exception as e:
-            logger.error("Can't list files at " + self._currentDir, e)
+            logger.info("Can't list files at " + self._currentDir, e)
 
         # Sort objects
         fileInfoList.sort(key=self.fileKey, reverse=not self.isSortingAscending())
 
         return fileInfoList
 
     def fileKey(self, f):
@@ -357,15 +357,15 @@
 SELECT_NONE = 0  # No selection, just browse files
 SELECT_FILE = 1
 SELECT_FOLDER = 2
 SELECT_PATH = 3  # Can be either file or folder
 
 
 class FileBrowser(ObjectBrowser):
-    """ The FileBrowser is a particular class of ObjectBrowser
+    """ The FileBrowser is a particular class of ObjectBrowser (Tk.Frame)
     where the "objects" are just files and directories.
     """
 
     _lastSelectedFile = None
     "Class scope attribute to keep the lastSelected file"
 
     _fileSelectedAtLoading = None
@@ -413,21 +413,21 @@
         self.showInfo = showInfo or self._showInfo
 
         ObjectBrowser.__init__(self, parent, self._provider)
 
         # focuses on the browser in order to allow to move with the keyboard
         self._goDir(os.path.abspath(initialDir))
 
-        if selectionType == SELECT_NONE:
-            selectButton = None
-
         buttonsFrame = tk.Frame(self)
         self._fillButtonsFrame(buttonsFrame)
         buttonsFrame.grid(row=1, column=0)
 
+        # Callback to be called "on Select" button key press
+        self.onSelect=None
+
     def _showInfo(self, msg):
         """ Default way (logger.info to console) to show a message with a given info.
         """
         logger.info(msg)
 
     def _fillLeftPanel(self, frame):
         """ Redefine this method to include a buttons toolbar and
@@ -631,15 +631,18 @@
         self.onClose()
 
     def _select(self, e=None):
 
         self._lastSelected = self.getSelected()
 
         if self._lastSelected is not None:
-            self.onSelect(self._lastSelected)
+            if self.onSelect:
+                self.onSelect(self._lastSelected)
+            else:
+                self.onClose()
         else:
             self.showInfo('Select a valid file/folder')
 
     def getEntryValue(self):
         return self.entryVar.get()
 
     def getCurrentDir(self):
@@ -683,14 +686,15 @@
     fnLower = filename.lower()
     return any(fnLower.endswith(ext) for ext in STANDARD_IMAGE_EXTENSIONS)
 
 
 class FileBrowserWindow(BrowserWindow):
     """ Windows to hold a file browser frame inside. """
 
+    lastValue=None
     def __init__(self, title, master=None, path=None,
                  onSelect=None, shortCuts=None, **kwargs):
         BrowserWindow.__init__(self, title, master, **kwargs)
         self.registerHandlers()
         browser = FileBrowser(self.root, path,
                               showInfo=lambda msg: self.showInfo(msg, "Info"),
                               shortCuts=shortCuts,
@@ -703,14 +707,16 @@
             browser.onSelect = selected
         browser.onClose = self.close
         self.setBrowser(browser)
 
     def getEntryValue(self):
         return self.browser.getEntryValue()
 
+    def getLastSelection(self):
+        return self.browser._lastSelected.getPath()
     def getCurrentDir(self):
         return self.browser.getCurrentDir()
 
     def registerHandlers(self):
         register = FileTreeProvider.registerFileHandler  # shortcut
 
         register(TextFileHandler(pwutils.Icon.TXT_FILE),
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/canvas.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 import logging
 logger = logging.getLogger(__name__)
 import math
 import tkinter as tk
 import operator
 
 from pyworkflow import Config
-from pyworkflow.gui import gui, getDefaultFont, cfgFontSize
+from pyworkflow.gui import gui, getDefaultFont
 from pyworkflow.gui.widgets import Scrollable
 
 DEFAULT_ZOOM = 100
 
-DEFAULT_FONT_SIZE = cfgFontSize
+DEFAULT_FONT_SIZE = Config.SCIPION_FONT_SIZE
 
 DEFAULT_CONNECTOR_FILL = "blue"
 DEFAULT_CONNECTOR_OUTLINE = "black"
 
 
 class Canvas(tk.Canvas, Scrollable):
     """Canvas to draw some objects.
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/dialog.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 Module to handling Dialogs
 some code was taken from tkSimpleDialog
 """
+import os.path
 import tkinter as tk
 import traceback
 from tkcolorpicker import askcolor as _askColor
 from pyworkflow import Config
 from pyworkflow.exceptions import PyworkflowException
 from pyworkflow.utils import Message, Icon, Color
 from . import gui, Window, widgets, configureWeigths, LIST_TREEVIEW, defineStyle, ToolTip
@@ -85,14 +86,15 @@
         if parent.winfo_viewable() and lockGui:
             self.transient(parent)
 
         if title:
             self.title(title)
 
         self.parent = parent
+
         # Default to CANCEL so if window is "Closed" behaves the same.
         self.result = RESULT_CANCEL
         self.initial_focus = None
 
         bodyFrame = tk.Frame(self)
         # Call subclass method body to create that region
         self.body(bodyFrame)
@@ -141,14 +143,17 @@
         # window ".139897767953072.139897384058440" was deleted before its visibility changed
         # wait for window to appear on screen before calling grab_set
         self.wait_visibility()
         if lockGui:
             self.grab_set()
         self.wait_window(self)
 
+    def getRoot(self):
+        return self
+
     def destroy(self):
         """Destroy the window"""
         self.initial_focus = None
         tk.Toplevel.destroy(self)
 
     #
     # construction hooks
@@ -255,14 +260,28 @@
     def resultCancel(self):
         return self.result == RESULT_CANCEL
 
     def info(self, message):
         """ Shows a info message for long running processes to inform the user GUI is not frozen"""
         self.floatingMessage.config(text=message)
 
+    ### Basic GUI helper methods
+    def _addButton(self, frame, callback, text="", icon=None, row=0, col=0, tooltip=None, shortcut=""):
+        """ Adds a label button"""
+        btn = tk.Label(frame, text=text,
+                       image=self.getImage(icon),
+                       compound=tk.LEFT, cursor='hand2')
+        btn.grid(row=row, column=col, sticky='nw', padx=(5, 0), pady=(5, 0))
+        btn.bind('<Button-1>', callback)
+        if tooltip:
+            tooltip = tooltip + ' (%s)' % shortcut if shortcut else tooltip
+            ToolTip(btn, tooltip, delay=150)
+        if shortcut:
+            self.bind(shortcut, callback)
+
 
 def fillMessageText(text, message):
     # Insert lines of text
     if isinstance(message, list):
         lines = message
     else:
         lines = message.splitlines()
@@ -551,14 +570,26 @@
 
 
 def askColor(parent, defaultColor='black'):
     (rgbcolor, hexcolor) = _askColor(defaultColor, parent=parent)
     return hexcolor
 
 
+def askPath(title="Browse files", msg="Select a file of a folder", path=".", onlyFolders=False, master=None, returnBaseName=False):
+    from pyworkflow.gui.browser import FileBrowserWindow
+
+    browserW = FileBrowserWindow(title, master=master, path=path, onlyFolders=onlyFolders)
+    browserW.show(modal=True)
+
+    result = browserW.getLastSelection()
+    if returnBaseName:
+        result=os.path.basename(result)
+
+    return result
+
 class ListDialog(Dialog):
     """
     Dialog to select an element from a list.
     It is implemented using the Tree widget.
     """
 
     def __init__(self, parent, title, provider, message=None, **kwargs):
@@ -579,23 +610,24 @@
         self.validateSelectionCallback = kwargs.get('validateSelectionCallback', None)
         self.previewCallBack = kwargs.get('previewCallback', None)
 
         self._selectmode = kwargs.get('selectmode', 'extended')
         self._selectOnDoubleClick = kwargs.get('selectOnDoubleClick', False)
         self._allowsEmptySelection = kwargs.get('allowsEmptySelection', False)
 
-        buttons = []
-        if kwargs.get('allowSelect', True):
-            buttons.append(('Select', RESULT_YES))
-        if kwargs.get('cancelButton', False):
-            buttons.append(('Close', RESULT_CLOSE))
-        else:
-            buttons.append(('Cancel', RESULT_CANCEL))
-
-        Dialog.__init__(self, parent, title, buttons=buttons, **kwargs)
+        if "buttons" not in kwargs:
+            buttons=[]
+            if kwargs.get('allowSelect', True):
+                buttons.append(('Select', RESULT_YES))
+            if kwargs.get('cancelButton', False):
+                buttons.append(('Close', RESULT_CLOSE))
+            else:
+                buttons.append(('Cancel', RESULT_CANCEL))
+            kwargs['buttons'] = buttons
+        Dialog.__init__(self, parent, title, **kwargs)
 
     def body(self, bodyFrame):
         bodyFrame.config()
         gui.configureWeigths(bodyFrame)
         dialogFrame = tk.Frame(bodyFrame)
         dialogFrame.grid(row=0, column=0, sticky='news', padx=5, pady=5)
         dialogFrame.config()
@@ -740,31 +772,22 @@
 
         subBody = tk.Frame(bodyFrame)
         subBody.grid(row=1, column=0, sticky='news', padx=5, pady=5)
         ListDialog.body(self, subBody)
 
         if self.toolbarButtons:
             for i, b in enumerate(self.toolbarButtons):
-                self._addButton(b, i)
+                self.addButton(b, i)
 
         if self._itemDoubleClick:
             self.tree.itemDoubleClick = self._itemDoubleClick
 
-    def _addButton(self, button, col):
-        btn = tk.Label(self.toolbarFrame, text=button.text,
-                       image=self.getImage(button.icon),
-                       compound=tk.LEFT, cursor='hand2')
-        btn.grid(row=0, column=col, sticky='nw', padx=(5, 0), pady=(5, 0))
-        btn.bind('<Button-1>', button.command)
-        if button.tooltip:
-            tooltip = button.tooltip + ' (%s)' % button.shortcut if button.shortcut else button.tooltip
-            self.bind(button.shortcut, button.command)
-            ToolTip(btn, tooltip, delay=150)
-        if button.shortcut:
-            self.bind(button.shortcut, button.command)
+    def addButton(self, button, col):
+
+        self._addButton(self.toolbarFrame, button.command, icon=button.icon, col=col, tooltip=button.tooltip, shortcut=button.shortcut)
 
 
 class FlashMessage:
     def __init__(self, master, msg, delay=5, relief='solid', func=None):
         self.root = tk.Toplevel(master=master)
         # hides until know geometry
         self.root.withdraw()
@@ -809,51 +832,14 @@
     def show(self):
         self.floatingMessage.update_idletasks()
 
     def close(self):
         self.floatingMessage.destroy()
 
 
-class FileBrowseDialog(Dialog):
-    """Dialog to select files from the filesystem."""
-
-    def __init__(self, parent, title, provider, message=None, **args):
-        """ From args:
-                message: message tooltip to show when browsing.
-                selected: the item that should be selected.
-        """
-        self.value = None
-        self.provider = provider
-        self.message = args.get('message', None)
-        Dialog.__init__(self, parent, title,
-                        buttons=[('Select', RESULT_YES), ('Cancel', RESULT_CANCEL)])
-
-    def body(self, bodyFrame):
-        bodyFrame.config(bg=Config.SCIPION_BG_COLOR)
-        gui.configureWeigths(bodyFrame)
-        self._createTree(bodyFrame)
-        if self.message:
-            label = tk.Label(bodyFrame, text=self.message, bg=Config.SCIPION_BG_COLOR,
-                             image=self.getImage(Icon.LIGHTBULB), compound=tk.LEFT)
-            label.grid(row=1, column=0, sticky='nw', padx=5, pady=5)
-        self.initial_focus = self.tree
-
-    def _createTree(self, parent):
-        self.tree = BoundTree(parent, self.provider)
-
-    def apply(self):
-        index = self.tree.index(self.tree.getFirst())
-        self.value = self.tree._objects[index]
-
-    def validate(self):
-        if self.tree.getFirst() is None:
-            showError("Validation error", "Please select an element", self)
-            return False
-        return True
-
 
 class SearchBaseWindow(Window):
     """ Base window for searching in a list
     You are going to implement several elements:
 
         columnsConfig: a dictionary with elements with this structure:
             <column-key>: (<title>,{kwargs for tree.column method}, weight, <casting_method>(optional, otherwise str))
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/form.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/form.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/graph.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/graph.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/graph_layout.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/graph_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import logging
 
-from pyworkflow.gui import cfgFontSize
-
 logger = logging.getLogger(__name__)
 
 from pyworkflow import Config, SCIPION_DEFAULT_FONT_SIZE
 
 
 
 class GraphLayout(object):
@@ -54,15 +52,15 @@
     def getFontScaleFactor(self):
         """
         :return: The scale factor between default font size 10, and current one
 
         """
         if self._fontScaleFactor is None:
 
-            self._fontScaleFactor = cfgFontSize/SCIPION_DEFAULT_FONT_SIZE
+            self._fontScaleFactor = Config.SCIPION_FONT_SIZE/SCIPION_DEFAULT_FONT_SIZE
 
         return self._fontScaleFactor
 
     def draw(self, graph, **kwargs):
         """ Setup the nodes position in the plane. """
         pass
 
@@ -87,15 +85,15 @@
         
         # Setup empty layout for each node
         for node in graph.getNodes():
             node._layout = {}
 
         visitDict = dict()
         # Do some level initialization on each node
-        self._setLayoutLevel(rootNode,  1, None, visitDict)
+        self._setLayoutLevel(rootNode,  1, visitDict)
         self._computeNodeOffsets(rootNode, 1)
         # Compute extreme left limit
         m = 9999
         for left, _ in rootNode._layout['hLimits']:
             m = min(m, left)
         
         self._applyNodeOffsets(rootNode, -m + self.getY())
@@ -103,54 +101,48 @@
         # Clean temporary _layout attributes
         for node in graph.getNodes():
             del node._layout
 
     def _isNewNode(self, node):
         return node.x == 0 or node.y == 0 or node.isRoot()
         
-    def _setLayoutLevel(self, node, level, parent, visitDict=None, ancestors=[]):
+    def _setLayoutLevel(self, node, level, parent,  ancestors=[]):
         """ Iterate over all nodes and set _layout dict.
         Also set the node level, which is defined
         as the max level of a parent + 1
         """
-        if visitDict is None:
-            visitDict = {}
-
-        if node.getName() not in visitDict:
-            visitDict[node.getName()] = True
+        if level > self.maxLevel:
+            return
 
-            if level > self.maxLevel:
-                return
+        layout = node._layout
 
-            layout = node._layout
-
-            if level > layout.get('level', 0):
-                # Calculate the y-position depending on the level
-                # and the delta-Y (DY)
-                if not self.partial or self._isNewNode(node):
-                    node.y = level * self.getY()
-                layout['level'] = level
-                layout['parent'] = parent
-                if hasattr(node, 'width'):
-                    half = node.width / 2
-                else:
-                    half = 50
-                layout['half'] = half
-                layout['hLimits'] = [[-half, half]]
-                layout['offset'] = 0
-
-                if self.__isNodeExpanded(node):
-                    ancestors.append(node.getName())
-                    for child in node.getChilds():
-                        if child.getName() in ancestors:
-                            logger.warning("WARNING: There might be a cyclic redundancy error in this protocol: %s (%s)" %(child.getLabel(),
-                                                                                                                           child.getName()))
-                        if Config.debugOn():
-                            print("%s: Setting layout for child %s" % ("-" * level, child), flush=True)
-                        self._setLayoutLevel(child, level+1, node, visitDict, ancestors.copy())
+        if level > layout.get('level', 0):
+            # Calculate the y-position depending on the level
+            # and the delta-Y (DY)
+            if not self.partial or self._isNewNode(node):
+                node.y = level * self.getY()
+            layout['level'] = level
+            layout['parent'] = parent
+            if hasattr(node, 'width'):
+                half = node.width / 2
+            else:
+                half = 50
+            layout['half'] = half
+            layout['hLimits'] = [[-half, half]]
+            layout['offset'] = 0
+
+            if self.__isNodeExpanded(node):
+                ancestors.append(node.getName())
+                for child in node.getChilds():
+                    if child.getName() in ancestors:
+                        logger.warning("WARNING: There might be a cyclic redundancy error in this protocol: %s (%s)" %(child.getLabel(),
+                                                                                                                       child.getName()))
+                    if Config.debugOn():
+                        print("%s: Setting layout for child %s" % ("-" * level, child), flush=True)
+                    self._setLayoutLevel(child, level+1, node, ancestors.copy())
 
     def __isNodeExpanded(self, node):
         """ Check if the status of the node is expanded or collapsed. """
         return getattr(node, 'expanded', True)
         
     def __setNodeOffset(self, node, offset):
         node._layout['offset'] = offset
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/gui.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,29 +42,27 @@
 
 # --------------- GUI CONFIGURATION parameters -----------------------
 # TODO: read font size and name from config file
 FONT_ITALIC = 'fontItalic'
 FONT_NORMAL = 'fontNormal'
 FONT_BOLD = 'fontBold'
 FONT_BIG = 'fontBig'
-cfgFontName = pw.Config.SCIPION_FONT_NAME
-cfgFontSize = pw.Config.SCIPION_FONT_SIZE
-cfgFontBigSize = cfgFontSize + 8
 # TextColor
 # cfgCitationTextColor = "dark olive green"
 # cfgLabelTextColor = "black"
 # cfgSectionTextColor = "blue4"
 # Background Color
 # cfgBgColor = "light grey"
 # cfgLabelBgColor = "white"
 # cfgHighlightBgColor = cfgBgColor
+#This with trigger the validation of the color falling back the firebrick if fails
+cfgButtonActiveBgColor = pw.Config.getActiveColor()
 cfgButtonFgColor = pw.Config.SCIPION_BG_COLOR
 cfgButtonActiveFgColor = pw.Config.SCIPION_BG_COLOR
 cfgButtonBgColor = pw.Config.SCIPION_MAIN_COLOR
-cfgButtonActiveBgColor = pw.Config.getActiveColor()
 cfgEntryBgColor = "lemon chiffon"
 # cfgExpertLabelBgColor = "light salmon"
 # cfgSectionBgColor = cfgButtonBgColor
 # Color
 # cfgListSelectColor = "DeepSkyBlue4"
 # cfgBooleanSelectColor = "white"
 # cfgButtonSelectColor = "DeepSkyBlue2"
@@ -134,33 +132,30 @@
 def getBigFont():
     return getNamedFont(FONT_BIG)
 
 
 def setCommonFonts(windows=None):
     """Set some predefined common fonts.
     Same conditions of setFont applies here."""
-    f = setFont(FONT_NORMAL, family=cfgFontName, size=cfgFontSize)
+    f = setFont(FONT_NORMAL, family=pw.Config.SCIPION_FONT_NAME, size=pw.Config.SCIPION_FONT_SIZE)
     aliasFont('fontButton', FONT_NORMAL)
 
     # Set default font size
     default_font = getDefaultFont()
-    default_font.configure(size=cfgFontSize, family=cfgFontName)
+    default_font.configure(size=pw.Config.SCIPION_FONT_SIZE, family=pw.Config.SCIPION_FONT_NAME)
 
-    fb = setFont(FONT_BOLD, family=cfgFontName, size=cfgFontSize,
+    fb = setFont(FONT_BOLD, family=pw.Config.SCIPION_FONT_NAME, size=pw.Config.SCIPION_FONT_SIZE,
                  weight='bold')
-    fi = setFont(FONT_ITALIC, family=cfgFontName, size=cfgFontSize,
+    fi = setFont(FONT_ITALIC, family=pw.Config.SCIPION_FONT_NAME, size=pw.Config.SCIPION_FONT_SIZE,
                  slant='italic')
 
-    setFont(FONT_BIG, family=cfgFontName, size=cfgFontBigSize)
-
-    # not used?
-    # setFont('fontLabel', family=cfgFontName, size=cfgFontSize+1, weight='bold')
+    setFont(FONT_BIG, family=pw.Config.SCIPION_FONT_NAME, size=pw.Config.SCIPION_FONT_SIZE+8)
 
     if windows:
-        windows.fontBig = tkFont.Font(size=cfgFontSize + 2, family=cfgFontName,
+        windows.fontBig = tkFont.Font(size=pw.Config.SCIPION_FONT_SIZE + 2, family=pw.Config.SCIPION_FONT_NAME,
                                       weight='bold')
         windows.font = f
         windows.fontBold = fb
         windows.fontItalic = fi
 
         # This adds the default value for the listbox inside a combo box
         # Which seems to not react to default font!!
@@ -332,15 +327,15 @@
         minsize: a minimum size for height and width
         icon: if not None, set the windows icon
         """
         # Init gui plugins
         pw.Config.getDomain()._discoverGUIPlugins()
 
         if masterWindow is None:
-            Window._root = self
+            # Unused?? Window._root = self
             self._images = {}
             # If a window which isn't the main Scipion window is generated from another main window, e. g. with Scipion
             # template after the refactoring of the kickoff, in which a dialog is launched and then a form, being it
             # called from the command line, so there's no Scipion main window. In that case, a tk.Tk() exists because if
             # a tk.TopLevel(), as the dialog, is directly launched, it automatically generates a main tk.Tk(). Thus,
             # after that first auto-tk.Tk(), another tk.Tk() was created here, and so the previous information was lost.
             # Solution proposed is to generate the root as an invisible window if it doesn't exist previously, and make
@@ -351,16 +346,16 @@
             # invoke the button on the return key
             root.bind_class("Button", "<Key-Return>", lambda event: event.widget.invoke())
 
             self._class = kwargs.get("_class", DEFAULT_WINDOW_CLASS)
             self.root = tk.Toplevel(class_=self._class)  # Toplevel of main window
         else:
             class_ = masterWindow._class if hasattr(masterWindow, "_class") else DEFAULT_WINDOW_CLASS
-            self.root = tk.Toplevel(masterWindow.root, class_=class_)
-            self.root.group(masterWindow.root)
+            self.root = tk.Toplevel(masterWindow.getRoot(), class_=class_)
+            self.root.group(masterWindow.getRoot())
             self._images = masterWindow._images
 
         self.root.withdraw()
         self.root.title(title)
 
         if weight:
             configureWeigths(self.root)
@@ -437,28 +432,33 @@
         """Override this method to respond to resize events."""
         pass
 
     def handleMove(self):
         """Override this method to respond to move events."""
         pass
 
-    def show(self, center=True):
+    def show(self, center=True, modal=False):
         """This function will enter in the Tk mainloop"""
         if center:
             if self.master is None:
                 refw = None
             else:
-                refw = self.master.root
+                refw = self.master.getRoot()
             centerWindows(self.root, dim=self.desiredDimensions(),
                           refWindows=refw)
+
         self.root.deiconify()
         self.root.focus_set()
         if self.queue is not None:
             self._queueTimer = self.root.after(1000, self.__processQueue)
-        self.root.mainloop()
+
+        if modal:
+            self.root.wait_window(self.root)
+        else:
+            self.root.mainloop()
 
     def close(self, e=None):
         self.root.destroy()
         # JMRT: For some reason when Tkinter has an exception
         # it does not exit the application as expected and
         # remains in the mainloop, so here we are forcing
         # to exit the whole system (only applies for the main window)
@@ -467,15 +467,15 @@
             sys.exit()
 
     def _onClosing(self):
         """Do some cleaning before closing."""
         if self.master is None:
             pass
         else:
-            self.master.root.focus_set()
+            self.master.getRoot().focus_set()
         if self.queue is not None:
             self.root.after_cancel(self._queueTimer)
         self.close()
 
     def getImage(self, imgName, percent=100, maxheight=None):
         return getImage(imgName, percent=percent,
                         maxheight=maxheight)
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/matplotlib_image.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/matplotlib_image.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/plotter.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/base.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import webbrowser
 import tkinter as tk
 
 import pyworkflow as pw
 from pyworkflow.gui import Window, Message, Color, getBigFont, defineStyle
 from pyworkflow.gui.widgets import GradientFrame
 from pyworkflow.utils.properties import Icon
+from pyworkflow.gui.project.variables import VariablesDialog
 
 from .viewprojects import ProjectsView
 from .viewprotocols import ProtocolsView
 from .viewdata import ProjectDataView
 
 VIEW_PROJECTS = Message.VIEW_PROJECTS
 VIEW_PROTOCOLS = Message.VIEW_PROTOCOLS
@@ -173,17 +174,19 @@
             "It integrates several software packages with a unified interface. "
             "This way you can combine them in a single workflow, while all the "
             "formats and conversions are taken care of automatically.\n\n"
             "*Scipion* is developed by a multidisciplinary group of engineers, "
             "physicists, mathematicians, biologists and computer scientists. "
             "It is produced mainly by people at the "
             "[[http://biocomputingunit.es//][CNB Biocomputing Unit]], "
-            "[[https://www.scilifelab.se/][SciLifeLab]] and "
             "[[https://www2.mrc-lmb.cam.ac.uk/][MRC LMB]], "
             "but with many contributions across the globe.")
 
     def onContactSupport(self):
         # Help -> Contact support
         email = pw.Config.SCIPION_SUPPORT_EMAIL
         self.showInfo("Please, do contact us at [[mailto:%s][%s]] for any "
                       "feedback, bug, idea, anything that will make Scipion "
                       "better.""" % (email, email))
+
+    def onConfiguration(self):
+        VariablesDialog(self.root)
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/constants.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/labels.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 # *
 # **************************************************************************
 """
 Tree widget implementation.
 """
         
 import tkinter as tk
+
+
 from pyworkflow import Config
 from pyworkflow.project import Label
-from pyworkflow.gui import Icon, configureWeigths
+from pyworkflow.gui import Icon, configureWeigths, getDefaultFont
 from pyworkflow.gui.tree import TreeProvider
 import pyworkflow.gui.dialog as dialog
 
 
 class LabelsTreeProvider(TreeProvider):
     """ Populate Tree from Labels. """
     def __init__(self, objList=None):
@@ -158,15 +160,15 @@
         # Label
         label_text = tk.Label(bodyFrame, text="Name", bg=Config.SCIPION_BG_COLOR, bd=0)
         label_text.grid(row=0, column=0, sticky='nw', padx=(15, 10), pady=15)
         # Label box
         var = tk.StringVar()
         var.set(self.label.getName())
         self.textVar = var
-        self.textLabel = tk.Entry(bodyFrame, width=20, textvariable=var)
+        self.textLabel = tk.Entry(bodyFrame, width=20, font=getDefaultFont(), textvariable=var)
         self.textLabel.grid(row=0, column=1, sticky='news', padx=5, pady=5)
 
         # Comment
         colorLabel = tk.Label(bodyFrame, text='Color \n(Click to change)',
                               bg=Config.SCIPION_BG_COLOR, bd=0)
         colorLabel.grid(row=1, column=0, sticky='nw', padx=(15, 10), pady=15)
         self.colorVar = tk.StringVar()
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/project.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 It is composed by three panels:
 1. Left: protocol tree.
 2. Right upper: VIEWS (Data/Protocols)
 3. Summary/Details
 """
 
 import logging
+
+from .variables import VariablesDialog
+
 logger = logging.getLogger(__name__)
 import os
 import threading
 import shlex
 import subprocess
 import socketserver
 import tempfile
@@ -92,16 +95,18 @@
         projMenu.addSubMenu('Locate a protocol', 'locate protocol',
                             shortCut="Ctrl+l")
         projMenu.addSubMenu('', '')  # add separator
         projMenu.addSubMenu('Import workflow', 'load_workflow',
                             icon=Icon.DOWNLOAD)
         projMenu.addSubMenu('Search workflow', 'search_workflow',
                             icon=Icon.ACTION_SEARCH)
-        if pw.Config.debugOn():
-            projMenu.addSubMenu('Export tree graph', 'export_tree')
+
+        projMenu.addSubMenu('Configuration', 'configuration',
+                            icon=Icon.SETTINGS)
+
         projMenu.addSubMenu('', '')  # add separator
         projMenu.addSubMenu('Debug Mode', 'debug mode',
                             shortCut="Ctrl+D", icon=Icon.DEBUG)
         projMenu.addSubMenu('', '')  # add separator
         projMenu.addSubMenu('Notes', 'notes', icon=Icon.ACTION_EDIT)
         projMenu.addSubMenu('', '')  # add separator
         projMenu.addSubMenu('Exit', 'exit', icon=Icon.ACTION_OUT)
@@ -243,28 +248,14 @@
                           onSelect=self._loadWorkflow,
                           selectButton='Import'
                           ).show()
 
     def onSearchWorkflow(self):
         WorkflowRepository().search()
 
-    def onExportTreeGraph(self):
-        runsGraph = self.project.getRunsGraph()
-        useId = not pwutils.envVarOn('SCIPION_TREE_NAME')
-        dotStr = runsGraph.printDot(useId=useId)
-        with tempfile.NamedTemporaryFile(suffix='.gv', mode="w") as dotFile:
-            dotFile.write(dotStr)
-            dotFile.flush()
-            openTextFileEditor(dotFile.name)
-
-        if useId:
-            logger.info("\nexport SCIPION_TREE_NAME=1 # to use names instead of ids")
-        else:
-            logger.info("\nexport SCIPION_TREE_NAME=0 # to use ids instead of names")
-
     def onToggleColorMode(self):
         self.getViewWidget()._toggleColorScheme(None)
 
     def onSelectAllProtocols(self):
         self.getViewWidget()._selectAllProtocols(None)
 
     def onAddAProtocol(self):
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/searchprotocol.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/searchprotocol.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/searchrun.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/searchrun.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/steps.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/steps.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/utils.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewdata.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewdata.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewprojects.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewprojects.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 import pyworkflow as pw
 from pyworkflow.project import Project
 from pyworkflow.utils.utils import prettyDate, prettyTime
 from pyworkflow.utils.path import getHomePath
 
 from pyworkflow.project import Manager
-import pyworkflow.gui as pwgui
 from pyworkflow.gui.text import TaggedText
 from pyworkflow.gui.dialog import askString, askYesNo, showError
 
 from pyworkflow.gui import Message, Window, cfgEntryBgColor, ToolTip
 from pyworkflow.gui.browser import FileBrowserWindow
 from pyworkflow.gui.widgets import IconButton, HotButton, Button
 from pyworkflow.utils.properties import Icon
@@ -55,19 +54,18 @@
         self.windows = windows
         self.manager = windows.manager
         self.root = windows.root
         self.lastLoad = None
 
         # Bind to root "focus in"
         self.root.bind("<FocusIn>", self._onWindowFocusIn)
-        bigSize = pwgui.cfgFontSize + 2
-        smallSize = pwgui.cfgFontSize - 2
-        fontName = pwgui.cfgFontName
+        smallSize = pw.Config.SCIPION_FONT_SIZE - 2
+        fontName = pw.Config.SCIPION_FONT_NAME
 
-        self.projNameFont = tkFont.Font(size=bigSize, family=fontName,
+        self.projNameFont = tkFont.Font(size=pw.Config.SCIPION_FONT_SIZE+2, family=fontName,
                                         weight='bold')
         self.projDateFont = tkFont.Font(size=smallSize, family=fontName)
         self.projDelFont = tkFont.Font(size=smallSize, family=fontName,
                                        weight='bold')
         self.manager = Manager()
 
         self.filter = tk.StringVar()
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewprotocols.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewprotocols.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/project/viewprotocols_extra.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/project/viewprotocols_extra.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,16 +500,15 @@
                     protocolsConfPath = os.path.join(
                         pluginDict[pluginName].__path__[0],
                         cls.PLUGIN_CONFIG_PROTOCOLS)
                     cls.__addProtocolsFromConf(protocols, protocolsConfPath)
 
             except Exception as e:
                 print('Failed to read settings. The reported error was:\n  %s\n'
-                      'To solve it, fix %s and run again.' % (
-                          e, os.path.abspath(protocolsConfPath)))
+                      'To solve it, fix %s and run again.' % e)
 
         # Clean empty sections
         cls._hideEmptySections(protocols)
 
         # Add all protocols to All view
         cls.__addAllProtocols(domain, protocols)
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/text.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/text.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/tooltip.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/tree.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/tree.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/gui/widgets.py` & `scipion_pyworkflow-3.6.0/pyworkflow/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/mapper/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/mapper/mapper.py` & `scipion_pyworkflow-3.6.0/pyworkflow/mapper/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,15 @@
             self.warning("Class '%s' not found in mapper dict. Ignored. "
                          % className)
             return None
         
         objClass = self.dictClasses[className]
         
         if not issubclass(objClass, obj.Object):
-            print("WARNING: Class '%s' is not a subclass of Object. Ignored. "
-                  % className)
+            logger.warning("WARNING: Class '%s' is not a subclass of Object. Ignored. " % className)
             return None
 
         try:
             instance = self.dictClasses[className](**kwargs)
         except Exception as e:
             clazz = self.dictClasses._default
             logger.error('Class %s could not be created. Replacing it with %s ' % (className, clazz.__name__), exc_info=e)
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/mapper/sqlite.py` & `scipion_pyworkflow-3.6.0/pyworkflow/mapper/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # *
 # **************************************************************************
 import logging
 logger = logging.getLogger(__name__)
 import re
 from collections import OrderedDict
 
-from pyworkflow.utils import replaceExt, joinExt
+from pyworkflow.utils import replaceExt, joinExt, valueToList
 from .sqlite_db import SqliteDb, OperationalError
 from .mapper import Mapper
 
 ID = 'id'
 CREATION = 'creation'
 PARENT_ID = 'parent_id'
 CLASSNAME = 'classname'
@@ -903,14 +903,18 @@
         return obj
 
     def __loadObjDict(self):
         """ Load object properties and classes from db. """
         # Create a template object for retrieving stored ones
         columnList = []
         rows = self.db.getClassRows()
+
+        # Adds common fields to the mapping
+        self.db.addCommonFieldsToMap()
+
         attrClasses = {}
         self._objBuildList = []
 
         for r in rows:
             label = r['label_property']
 
             if label == SELF:
@@ -1043,23 +1047,26 @@
         # If there is only one label,
         if len(labels) == 1:
             return result[labels[0]]
         else:
             return result
 
     def aggregate(self, operations, operationLabel, groupByLabels=None):
+
+        operations = valueToList(operations)
+        groupByLabels = valueToList(groupByLabels)
+
         rows = self.db.aggregate(operations, operationLabel, groupByLabels)
+
+        # Transform the sql row into a disconnected list of dictionaries
         results = []
         for row in rows:
             values = {}
-            for label in operations:
-                values[label] = row[label]
-            if groupByLabels is not None:
-                for label in groupByLabels:
-                    values[label] = row[label]
+            for key in row.keys():
+                values[key] = row[key]
             results.append(values)
 
         return results
 
     def count(self):
         return 0 if self.doCreateTables else self.db.count()
 
@@ -1287,17 +1294,25 @@
             colName = 'c%02d' % c
             self._columnsMapping[k] = colName
             c += 1
             if k != SELF:
                 self.INSERT_OBJECT += ',%s' % colName
                 self.UPDATE_OBJECT += ', %s=?' % colName
 
+        self.addCommonFieldsToMap()
+
         self.INSERT_OBJECT += ") VALUES (?,?,?,?, datetime('now')" + ',?' * (c-1) + ')'
         self.UPDATE_OBJECT += ' WHERE id=?'
 
+    def addCommonFieldsToMap(self):
+
+        # Add common fields to the mapping
+        self._columnsMapping["id"] = "id"
+        self._columnsMapping["_objId"] = "id"
+
     def getClassRows(self):
         """ Create a dictionary with names of the attributes
         of the columns. """
         self.executeCommand(self.SELECT_CLASS)
         return self._results(iterate=False)
 
     def getSelfClassName(self):
@@ -1389,15 +1404,15 @@
         >>> _micId=3 OR _micId=4
         """
         if where is None:
             return
 
         whereStr = where
         # Split by valid where operators: =, <, >
-        result = re.split('<=|<=|=|<|>|AND|OR', where)
+        result = re.split('<=|>=|=|<|>|AND|OR', where)
         # For each item
         for term in result:
             # trim it
             term = term.strip()
             whereRealCol = self._getRealCol(term)
             if whereRealCol is not  None:
                 whereStr = whereStr.replace(term, whereRealCol)
@@ -1426,25 +1441,45 @@
         if whereStr is not None:
             sqlCommand += " WHERE " + whereStr
 
         self.executeCommand(sqlCommand)
         return self._results(iterate=False)
 
     def aggregate(self, operations, operationLabel, groupByLabels=None):
+        """
+
+        :param operations: string or LIST of operations: MIN, MAX, AVG, COUNT, SUM, TOTAL, GROUP_CONCAT. Any single argument function
+        defined for sqlite at https://www.sqlite.org/lang_aggfunc.html
+        :param operationLabel: string or LIST of attributes to apply the functions on
+        :param groupByLabels: (Optional) attribute or list of attributes to group by the data
+        :return:
+        """
         # let us count for testing
         selectStr = 'SELECT '
         separator = ' '
+
+        operations = valueToList(operations)
+        operationLabel = valueToList(operationLabel)
+        groupByLabels = valueToList(groupByLabels)
+
         # This cannot be like the following line should be expressed in terms
         # of C1, C2 etc....
-        for operation in operations:
-            selectStr += "%s %s(%s) AS %s" % (separator, operation,
-                                              self._columnsMapping[operationLabel],
-                                              operation)
-            separator = ', '
-        if groupByLabels is not None:
+        for index,label in enumerate(operationLabel):
+            for operation in operations:
+
+                if index==0:
+                    alias = operation
+                else:
+                    alias = operation + label
+
+                selectStr += "%s %s(%s) AS %s" % (separator, operation,
+                                                  self._columnsMapping[label],
+                                                  alias)
+                separator = ', '
+        if groupByLabels:
             groupByStr = 'GROUP BY '
             separator = ' '
             for groupByLabel in groupByLabels:
                 groupByCol = self._columnsMapping[groupByLabel]
                 selectStr += ', %(groupByCol)s as "%(groupByLabel)s"' % locals()
                 groupByStr += "%s %s" % (separator, groupByCol)
                 separator = ', '
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/mapper/sqlite_db.py` & `scipion_pyworkflow-3.6.0/pyworkflow/mapper/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/mapper/xmlmapper.py` & `scipion_pyworkflow-3.6.0/pyworkflow/mapper/xmlmapper.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/object.py` & `scipion_pyworkflow-3.6.0/pyworkflow/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,22 +581,22 @@
     
     def printAll(self, name=None, level=0):
         """Print object and all its attributes.
         Mainly for debugging"""
         tab = ' ' * (level*3)
         idStr = ''  # ' (id = %s, pid = %s)' % (self.getObjId(), self._objParentId)
         if name is None:
-            logger.info("%s %s %s" % (tab, self.getClassName(), idStr))
+            logger.info(f"{tab} {self.getClassName()} {idStr}")
         else:
             if name == 'submitTemplate':  # Skip this because very large value
                 value = '...'
             else:
                 value = self.getObjValue()
                 
-            logger.info(tab, '%s = %s' % (name, value), idStr)
+            logger.info(f"{tab} {name} = {value} {idStr}")
         for k, v in self.getAttributes():
             v.printAll(k, level + 1)
             
     def printObjDict(self, includeClasses=False):
         """Print object dictionary. Mainly for debugging"""
         import pprint
         pp = pprint.PrettyPrinter(indent=4)
@@ -1159,15 +1159,15 @@
             
     def aggregate(self, operations, operationLabel, groupByLabels=None):
         """
          This method operate on sets of values. They are used with a
          GROUP BY clause to group values into subsets
         :param operations: list of aggregate function such as COUNT, MAX, MIN,...
         :param operationLabel: label to use by the aggregate function
-        :param groupByLabels: list of labels to group
+        :param groupByLabels: list of labels to group by
         :return: the aggregated value of each group
         """
         return self._getMapper().aggregate(operations, operationLabel, groupByLabels)
 
     def setMapperClass(self, MapperClass):
         """ Set the mapper to be used for storage. """
         if MapperClass is None:
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/plugin.py` & `scipion_pyworkflow-3.6.0/pyworkflow/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import logging
 import sys
 
+from pyworkflow import Variable, VariablesRegistry, VarTypes
 from .protocol import Protocol
 from .viewer import Viewer
 from .wizard import Wizard
 
 logger = logging.getLogger(__name__)
 import glob
 import os
@@ -80,16 +81,21 @@
         """ Register a new plugin. This function should only be called when
         creating a class with __metaclass__=PluginMeta that will trigger this.
         """
         try:
             m = importlib.import_module(name)
 
             # Define variables
-            m.Plugin._defineVariables()
             m._pluginInstance = m.Plugin()
+            # This needs an explanation. _defineVariables() are classmethods, therfore we need a class variable and thus .name can't be used.
+            # Ideally, since Plugin class is instantiated we could transform _defineVariables methods into instance methods and only then we
+            # could use .name.
+            Plugin._tmpName = name
+            m._pluginInstance.name = name
+            m._pluginInstance._defineVariables()
 
             m.Domain = cls  # Register the domain class for this module
             # TODO avoid loading bibtex here and make a lazy load like the rest.
             # Load bibtex
             m._bibtex = {}
             bib = cls.__getSubmodule(name, 'bibtex')
             if bib is not None:
@@ -535,28 +541,32 @@
 
     _vars = {}
     _homeVar = ''  # Change in subclasses to define the "home" variable
     _pathVars = []
     _supportedVersions = []
     _url = ""  # For the plugin
     _condaActivationCmd = None
+    _tmpName = None # This would be temporary. It will hold the plugin name during the call to defineVariables
 
     def __init__(self):
         self._path = None
         self._inDevelMode = None
         self._name = None
 
     @classmethod
-    def _defineVar(cls, varName, defaultValue):
+    def _defineVar(cls, varName, defaultValue, description="Missing", var_type:VarTypes=None):
         """ Internal method to define variables trying to get it from the environment first. """
-        cls._addVar(varName, os.environ.get(varName, defaultValue))
+        cls._addVar(varName, os.environ.get(varName, defaultValue), default=defaultValue, description=description, var_type=var_type)
 
     @classmethod
-    def _addVar(cls, varName, value):
+    def _addVar(cls, varName, value, default=None, description="Missing", var_type:VarTypes=None):
         """ Adds a variable to the local variable dictionary directly. Avoiding the environment"""
+
+        var = Variable(varName, description, cls._tmpName, value, default, var_type=var_type)
+        VariablesRegistry.register(var)
         cls._vars[varName] = value
 
     @classmethod
     @abstractmethod
     def getEnviron(cls):
         """ Set up the environment variables needed to launch programs. """
         pass
@@ -572,15 +582,14 @@
             elif condaActivationCmd[-1] not in [";", "&"]:
                 condaActivationCmd += "&&"
 
             cls._condaActivationCmd = condaActivationCmd
 
         return cls._condaActivationCmd
 
-    @classmethod
     @abstractmethod
     def _defineVariables(cls):
         """ Method to define variables and their default values.
         It will use the method _defineVar that will take a variable value
         from the environment or from an optional default value.
 
         This method is not supposed to be called from client code,
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/config.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/manager.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/project.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/clean_projects.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/clean_projects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/config.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/create.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/create.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/edit_workflow.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/edit_workflow.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/fix_links.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/fix_links.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/load.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/load.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/refresh.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/refresh.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/schedule.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/schedule.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/stack2volume.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/stack2volume.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/project/scripts/stop.py` & `scipion_pyworkflow-3.6.0/pyworkflow/project/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/bibtex.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/constants.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/executor.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/executor.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/hosts.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/hosts.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/launch.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/launch.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/package.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/package.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/params.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/params.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/protocol/protocol.py` & `scipion_pyworkflow-3.6.0/pyworkflow/protocol/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,17 +709,20 @@
 
           - Iterate over the main attributes of the set
             - if attribute is a pointer then we add the pointed protocol to the ids list
         """
         protocolIds = []
         protocol = None
         for key, attrInput in self.iterInputAttributes():
+            outputs = []
             output = attrInput.get()
             if isinstance(output, Protocol):  # case A
                 protocol = output
+                for _, protOutput in protocol.iterOutputAttributes():
+                    outputs.append(protOutput)  # for case A store all the protocols outputs
             else:
                 if attrInput.hasExtended():  # case B
                     protocol = attrInput.getObjValue()
                 else:  # case C
 
                     if self.getProject() is not None:
                         protocol = self.getProject().getRunsGraph(refresh=True).getNode(str(output.getObjParentId())).run
@@ -732,29 +735,35 @@
                         # (without extended): hopefully this will only be
                         # created from tests
                         logger.warning("Can't get %s info from %s."
                               " This could render unexpected results when "
                               "scheduling protocols. Value: %s" % (key, self, attrInput))
                         continue
 
-                # If there is output
                 if output is not None:
+                    outputs.append(output)
+
+            # If there is output
+            if outputs:
+                # Iter over all the outputs
+                for output in outputs:
                     # For each output attribute: Looking for pointers like SetOfCoordinates.micrographs
                     for k, attr in output.getAttributes():
                         # If it's a pointer
                         if isinstance(attr, Pointer):
                             logger.debug("Pointer found in output: %s.%s (%s)" % (output, k, attr))
                             prot = attr.getObjValue()
                             if prot is not None:
                                 if isinstance(prot, Protocol):
                                     protocolIds.append(prot.getObjId())
                                 else:
                                     logger.warning(f"We have found that {output}.{key} points to {attr} "
                                                    f"and is a direct pointer. Direct pointers are less reliable "
                                                    f"in streaming scenarios. Developers should avoid them.")
+
             protocolIds.append(protocol.getObjId())
 
         return protocolIds
 
     def getInputStatus(self):
         """ Returns if any input pointer is not ready yet and if there is
          any pointer to an open set
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/Imagej.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/Imagej.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/chimera.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/chimera.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/fa-exclamation-triangle_alert.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/fa-exclamation-triangle_alert.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/fa-info-circle_alert.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/fa-info-circle_alert.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/fa-times-circle_alert.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/fa-times-circle_alert.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/file_vol.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/file_vol.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/loading.gif` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/loading.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/no-image128.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/no-image128.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_bn.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_bn.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon.svg` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon.svg`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon_proj.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon_proj.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon_projs.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon_projs.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_icon_prot.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_icon_prot.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_logo.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_logo_normal.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_logo_normal.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/scipion_logo_small.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/scipion_logo_small.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/background_section.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/background_section.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/delete.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/delete.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/doc_icon.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/doc_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/download_icon.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/download_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/menu.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/menu.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/volumeOff.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/volumeOff.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/showj/volumeOn.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/showj/volumeOn.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/sprites.png` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/sprites.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/sprites.xcf` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/sprites.xcf`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/resources/wait.gif` & `scipion_pyworkflow-3.6.0/pyworkflow/resources/wait.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/template.py` & `scipion_pyworkflow-3.6.0/pyworkflow/template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Module to host templates classes"""
 import collections
 import glob
 import os
 import tempfile
 from datetime import datetime
-from pyworkflow import SCIPION_JSON_TEMPLATES, Config
+from pyworkflow import SCIPION_JSON_TEMPLATES, Config, VarTypes
 from pyworkflow.utils import greenStr
 
 
 class Template:
     def __init__(self, pluginName, tempPath):
         self.pluginName = pluginName
         # Tidy up templates names: removing .json.template and .json (when passed as parameter)
@@ -134,15 +134,15 @@
 
 
 class TemplateParam(object):
     def __init__(self, index, title, value=None, varType=None, alias=None):
         self._index = index
         self._title = title
         self._value = value
-        self._type = varType
+        self._type = int(varType)
         self._alias = alias
 
     def getTitle(self):
         return self._title
 
     def getIndex(self):
         return self._index
@@ -163,37 +163,29 @@
         return Validations.check(self._value, self._type)
 
 
 class Validations:
 
     """ FIELDS VALIDATION """
     """ FIELDS TYPES"""
-    FIELD_TYPE_STR = "0"
-    FIELD_TYPE_BOOLEAN = "1"
-    FIELD_TYPE_PATH = "2"
-    FIELD_TYPE_INTEGER = "3"
-    FIELD_TYPE_DECIMAL = "4"
-
     @classmethod
     def check(cls, value, fieldType):
-        if fieldType == cls.FIELD_TYPE_BOOLEAN:
+        if fieldType == VarTypes.BOOLEAN.value:
             return cls.validBoolean(value)
-        elif fieldType == cls.FIELD_TYPE_DECIMAL:
+        elif fieldType == VarTypes.DECIMAL.value:
             return cls.validDecimal(value)
-        elif fieldType == cls.FIELD_TYPE_INTEGER:
+        elif fieldType == VarTypes.INTEGER.value:
             return cls.validInteger(value)
-        elif fieldType == cls.FIELD_TYPE_PATH:
+        elif fieldType == VarTypes.PATH.value:
             return cls.validPath(value)
-        elif fieldType == cls.FIELD_TYPE_STR:
+        elif fieldType == VarTypes.STRING.value:
             return cls.validString(value)
 
         else:
-            print("Type %s for %s not recognized. Review the template."
-                  % (type, value))
-            return
+            return "Type %s for %s not recognized. Review the template." % (fieldType, value)
 
     @staticmethod
     def validString(value):
         if value is None:
             return "String does not accept None/empty values."
 
     @staticmethod
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/tests/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/tests/tests.py` & `scipion_pyworkflow-3.6.0/pyworkflow/tests/tests.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/dataset.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/echo.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/echo.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/graph.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/graph.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/log.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/log.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/path.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 """
 This module contains the PATH related utilities
 inside the utils module
 """
 
 import logging
 
+from pyworkflow.utils import yellow
+
 logger = logging.getLogger(__name__)
 
 import os
 import shutil
 import sys
 from glob import glob
 import datetime
@@ -495,7 +497,31 @@
     if it doesn't exist. """
     if os.path.exists(fn):
         ts = os.path.getmtime(fn)
         return datetime.datetime.fromtimestamp(ts)
     else:
         logger.info(fn + " does not exist!!. Can't check last modification date.")
         return None
+
+
+def backup(fpath):
+    """
+    Create directory "backup" if necessary and back up the file.
+
+    :param fpath:
+    :return: None
+
+    """
+    BACKUPS="backup"
+
+    dname = os.path.dirname(fpath)
+
+    if not os.path.exists(dname):
+        os.makedirs(dname)
+
+    elif os.path.exists(fpath):
+        if not os.path.exists(os.path.join(dname, BACKUPS)):
+            os.makedirs(os.path.join(dname, BACKUPS))
+        backupFn = os.path.join(dname, BACKUPS,
+                      '%s.%s' % (os.path.basename(fpath), datetime.datetime.now().strftime("%Y%m%d%H%M%S")))
+        logger.info(yellow("* Creating backup: %s" % backupFn))
+        os.rename(fpath, backupFn)
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/process.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/profiler.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/progressbar.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/progressbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,63 +30,66 @@
 import sys
 import re
 
 
 class ProgressBar(object):
     """ Text progress bar class for Python.
 
-    A text progress bar is typically used to display the progress of a long
-    running operation, providing a visual cue that processing is underway.
+    A text progress bar is typically used to display the progress of a long-running
+    operation, providing a visual cue that processing is underway.
 
     Example::
 
         N = 1000
         pb = ProgressBar(N, fmt=ProgressBar.FULL)
         pb.start()
         for x in range(N):
             pb.update(x+1)
             sleep(0.1)
         pb.finish()
 
+    Optionally you can pass a step param (default to 10000) and call increase in each loop. Only when the step is reached, the progress is printed.
     """
     DEFAULT = 'Progress: %(bar)s %(percent)3d%%'
     FULL = '%(bar)s %(current)d/%(total)d (%(percent)3d%%) %(remaining)d to go'
     # scipion uses variable fonts so the bar size changes
     # since the space width is different from the = width
     NOBAR = '%(current)d/%(total)d (%(percent)3d%%) %(remaining)d to go'
     OBJID = '%(bar)s %(current)d/%(total)d (%(percent)3d%%) (objectId=%(objectId)d)'
     DOT = '.'
 
     def __init__(self, total, width=40, fmt=DEFAULT, symbol='=',
-                 output=None, extraArgs=None):
+                 output=None, extraArgs=None, step=10000):
         """
         Create a new ProgressBar object.
 
         :param total: The total amount that will be running the progress bar.
             The value in the update() method can no go greater than this value.
         :param width: progress bar width (without the percentage and number of
             iterations loop)
         :param fmt: predefined format string, so far DEFAULT, FULL, OBJID and
             DOT are defined.
         :param symbol: progress bar is made with this symbol
         :param output:
         :param extraArgs: Additional arguments that can be passed to be used
             the fmt format. (e.g extraArgs={'objectId': 1} for fmt=OBJID
+        :param step: interval between printing progress. Use in combination with "increase"
         """
         if len(symbol) != 1:
             raise Exception("Symbol should be only 1 character length. ")
 
         self._total = total
         self._width = width
         self._symbol = symbol
         self._output = output or sys.stdout
         self._current = -1
         self._extraArgs = extraArgs or {}
         self._fmt = fmt
         self._directPrint = fmt == self.DOT
+        self.step = step
 
         if not self._directPrint:
             # This line computes the number of digits
             # in total and rewrites the fmt string
             # so if total = 100, %d is converted to %3d
             self._fmt = re.sub(r'(?P<name>%\(.+?\))d',
                                r'\g<name>%dd' % len(str(total)), fmt)
@@ -129,14 +132,22 @@
         if value < 0 or value <= self._current or value > self._total:
             raise Exception("Incorrect value provided. It should be greater "
                             "than previous value and between 0 and total. ")
         self._current = value
         self._output.write(self.__getStr())
         self._output.flush()
 
+    def increase(self):
+        """ Increase the value by 1. Is new value matches the step. update is called"""
+        nextValue = self._current + 1
+        if (nextValue) % self.step == 0:
+            self.update(nextValue)
+        else:
+            self._current=nextValue
+
     def finish(self, printNewLine=True):
         """ Finalize the progress and
         print last update with 100% complete message """
         if self._current < self._total:
             self.update(self._total)
         # print a new line
         if printNewLine:
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/properties.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,16 @@
     ACTION_VISUALIZE = ACTION_RESULTS
     ACTION_WIZ = SpriteImage(32,288,'fa-magic.png')
     ACTION_HELP = SpriteImage(32,160,'fa-question-circle.png')
     ACTION_REFERENCES = SpriteImage(48,256,'link')
     ACTION_EXPORT = ACTION_REFERENCES
     ACTION_EXPORT_UPLOAD = SpriteImage(16,96, 'fa-upload.png')
     ACTION_SEARCH = SpriteImage(32,96, 'fa-search.png')
-    ACTION_EXECUTE = SpriteImage(48,304,'fa-cogs.png')
+    SETTINGS = SpriteImage(48,304,'fa-cogs.png')
+    ACTION_EXECUTE = SETTINGS
     ACTION_IN = SpriteImage(16,304,'fa-sign-in.png')
     ACTION_OUT = SpriteImage(16,288,'fa-sign-out.png')
     ACTION_FIND_NEXT = SpriteImage(32,208,'fa-next.png')
     ACTION_FIND_PREVIOUS = SpriteImage(32,192,'fa-previous.png')
     ACTION_COLLAPSE = SpriteImage(32,240,'fa-minus-square.png')
     ACTION_EXPAND = SpriteImage(32,224,'fa-plus-square.png')
     ACTION_CIRCLE = SpriteImage(48,192,'circle.png')
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/reflection.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/reflection.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/utils.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,15 +568,19 @@
     '1 1 2x2 4 4' -> ['1', '1', '2', '2', '4', '4']
     '2x3, 3x4, 1' -> ['3', '3', '4', '4', '4', '1']
 
     """
     result = []
     valuesStr = valuesStr.replace(","," ")
     for chunk in valuesStr.split():
-        values = chunk.split('x')
+        if caster != str:
+            values = chunk.split('x')
+        else:
+            values=[chunk]
+
         n = len(values)
         if n == 1:  # 'x' is not present in the chunk, single value
             result += [caster(values[0])]
         elif n == 2:  # multiple the values by the number after 'x'
             result += [caster(values[1])] * int(values[0])
         else:
             raise Exception("More than one 'x' is not allowed in list string value.")
@@ -860,7 +864,17 @@
 
     @classmethod
     def WLSfile2Windows(cls, file):
         # Links in WSL are not valid in windows
         file = os.path.realpath(file).replace("/", "\\")
         file = ("\\\\wsl.localhost\\" + cls.getWLSNAME() + file)
         return file
+
+
+def valueToList(value):
+    """ Returns a list containing value, unless value is already a list. If value is None returns an empty list"""
+    if value is None:
+        return []
+    elif isinstance(value, list):
+        return value
+    else:
+        return [value]
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/utils/which.py` & `scipion_pyworkflow-3.6.0/pyworkflow/utils/which.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/viewer.py` & `scipion_pyworkflow-3.6.0/pyworkflow/viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/webservices/config.py` & `scipion_pyworkflow-3.6.0/pyworkflow/webservices/config.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/webservices/notifier.py` & `scipion_pyworkflow-3.6.0/pyworkflow/webservices/notifier.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/webservices/repository.py` & `scipion_pyworkflow-3.6.0/pyworkflow/webservices/repository.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflow/wizard.py` & `scipion_pyworkflow-3.6.0/pyworkflow/wizard.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/__init__.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/bibtex.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/objects.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/protocols.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/protocols.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_canvas.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_domain.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_logs.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_mappers.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_mappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -262,14 +262,15 @@
         self.assertEqual(0, mapper.maxId())
         n = 10
 
         indexes = list(range(1, n + 1))
         for i in indexes:
             img = MockImage()
             img.setLocation(i, IMAGES_STK)
+            img.setSamplingRate(i%2)
             mapper.insert(img)
 
         self.assertEqual(n, mapper.count())
         self.assertEqual(n, mapper.maxId())
 
         # Store one more image with bigger id
         img = MockImage()
@@ -322,14 +323,35 @@
 
         self.assertEqual(mapper2.getProperty('samplingRate'), '3.0')
         self.assertEqual(mapper2.getProperty('defocusU'), '2000')
 
         # Make sure that maxId() returns the proper value after loading db
         self.assertEqual(bigId + 1, mapper2.maxId())
 
+        # test aggregation
+        result = mapper2.aggregate("COUNT", "id")  # As strings
+        self.assertEqual(result[0]["COUNT"], 12, "Aggregation fo count does not work")
+
+        result = mapper2.aggregate(["COUNT"], ["id"])  # As lists
+        self.assertEqual(result[0]["COUNT"], 12, "Aggregation as list of count does not work")
+
+        result = mapper2.aggregate(["MAX","AVG"], "id")
+        self.assertEqual(result[0]["MAX"], bigId+1, "Aggregation  max, avg does not work")
+        self.assertAlmostEqual(result[0]["AVG"], 171.33, places=2, msg="Aggregation  max, avg does not work")
+
+        result = mapper2.aggregate(["MAX", "COUNT"], "_samplingRate", "id")
+        self.assertEqual(result[0]["MAX"], 1, "Aggregation max, grouped does not work")
+        self.assertEqual(result[0]["COUNT"], 1, "Aggregation  max, count does not work")
+        self.assertEqual(result[0]["id"], 1, "Aggregation  group field not returned")
+
+        # Aggregation on more than one field
+        result = mapper2.aggregate(["MAX"], ["id","_samplingRate"])
+        self.assertEqual(result[0]["MAX"], 1001, "Aggregation max, grouped does not work")
+        self.assertEqual(result[0]["MAX_samplingRate"], 1.0, "Aggregation  max, count does not work")
+
     def test_emtpySet(self):
         dbName = self.getOutputPath('empty.sqlite')
         print(">>> test empty set: dbName = '%s'" % dbName)
         # Check that writing an emtpy set do not fail
         objSet = pwobj.Set(filename=dbName)
         objSet.write()
         objSet.close()
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_object.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,17 @@
         self.assertEqual(s2.getListFromValues(caster=float), [1.,2.,3.,4.])
         self.assertEqual(s2.getListFromRange(), [1, 2, 3, 4])
 
         # Values ...
         s2.set("2x4, 4, 7")
         self.assertEqual(s2.getListFromValues(), [4, 4, 4, 7])
 
+        # Values ...
+        self.assertEqual(s2.getListFromValues(caster=str), ["2x4", "4", "7"])
+
         # Ranges
         s2.set("2-8, 1-2, 7")
         self.assertEqual(s2.getListFromRange(), [2, 3, 4, 5, 6, 7, 8, 1, 2, 7])
 
     def test_Pointer(self):
         c = Complex.createComplex()
         p = pwobj.Pointer()
@@ -326,30 +329,30 @@
         # Request id list
         result = imgSet.getUniqueValues(ID)
         # Here we should have 10 values
         self.assertEqual(len(result), 10, "Unique values with ID")
 
         # Use creation timestamp
         # Request id list
-        result = imgSet.getUniqueValues(ID, where="%s>=%s" % (CREATION , imgSet.fmtDate(halfTimeStamp)))
+        result = imgSet.getUniqueValues(ID, where="%s>=%s" % (CREATION, imgSet.fmtDate(halfTimeStamp)))
         self.assertEqual(len(result), 5, "Unique values after a time stamp does not work")
 
         # Test getIdSet
         ids = imgSet.getIdSet()
         self.assertIsInstance(ids, set, "getIdSet does not return a set")
         self.assertIsInstance(next(iter(ids)), int, "getIdSet items are not integer")
         self.assertEqual(len(ids), 10, "getIdSet does not return 10 items")
 
         # Request item by id
         item = imgSet[1]
-        self.assertEqual(item.getObjId(), 1, "Item accesed by [] and id does not work")
+        self.assertEqual(item.getObjId(), 1, "Item accessed by [] and id does not work")
 
         # Request item by field
         item = imgSet.getItem("id", 2)
-        self.assertEqual(item.getObjId(), 2, "Item accesed field id does not work")
+        self.assertEqual(item.getObjId(), 2, "Item accessed field id does not work")
 
         # Test load properties queries
         from pyworkflow.mapper.sqlite_db import logger
         logger.setLevel(DEBUG)
         lastResort.setLevel(DEBUG)
         imgSetVerbose = MockSetOfImages(filename=fn)
         imgSetVerbose.loadAllProperties()
```

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_project.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_protocol_execution.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_protocol_execution.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_protocol_export.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_protocol_export.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_protocol_output.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_protocol_output.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_streaming.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_streaming.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/pyworkflowtests/tests/test_utils.py` & `scipion_pyworkflow-3.6.0/pyworkflowtests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/requirements.txt` & `scipion_pyworkflow-3.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/PKG-INFO` & `scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-pyworkflow
-Version: 3.5.0
+Version: 3.6.0
 Summary: Simple workflow platform used in scientific applications, initially developed within the Scipion framework for image processing in Electron Microscopy.
 Home-page: https://github.com/scipion-em/scipion-pyworkflow
 Author: J.M. De la Rosa Trevin, Roberto Marabini, Grigory Sharov, Josue Gomez Blanco, Pablo Conesa, Yunior Fonseca Reyna
 Author-email: delarosatrevin@scilifelab.se, roberto@cnb.csic.es, gsharov@mrc-lmb.cam.ac.uk, josue.gomez-blanco@mcgill.ca, pconesa@cnb.csic.es, fonsecareyna@cnb.csic.es
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-pyworkflow/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-pyworkflow/
 Keywords: workflows science electron-microscopy cryo-em structural-biology image-processing scipion
```

### Comparing `scipion-pyworkflow-3.5.0/scipion_pyworkflow.egg-info/SOURCES.txt` & `scipion_pyworkflow-3.6.0/scipion_pyworkflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 pyworkflow/gui/project/constants.py
 pyworkflow/gui/project/labels.py
 pyworkflow/gui/project/project.py
 pyworkflow/gui/project/searchprotocol.py
 pyworkflow/gui/project/searchrun.py
 pyworkflow/gui/project/steps.py
 pyworkflow/gui/project/utils.py
+pyworkflow/gui/project/variables.py
 pyworkflow/gui/project/viewdata.py
 pyworkflow/gui/project/viewprojects.py
 pyworkflow/gui/project/viewprotocols.py
 pyworkflow/gui/project/viewprotocols_extra.py
 pyworkflow/mapper/__init__.py
 pyworkflow/mapper/mapper.py
 pyworkflow/mapper/sqlite.py
```

### Comparing `scipion-pyworkflow-3.5.0/setup.py` & `scipion_pyworkflow-3.6.0/setup.py`

 * *Files identical despite different names*

