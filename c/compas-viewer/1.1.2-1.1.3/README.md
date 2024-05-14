# Comparing `tmp/compas_viewer-1.1.2.tar.gz` & `tmp/compas_viewer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_viewer-1.1.2.tar", last modified: Mon Apr 22 15:21:04 2024, max compression
+gzip compressed data, was "compas_viewer-1.1.3.tar", last modified: Tue May 14 18:30:34 2024, max compression
```

## Comparing `compas_viewer-1.1.2.tar` & `compas_viewer-1.1.3.tar`

### file list

```diff
@@ -1,125 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.242399 compas_viewer-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-22 15:21:04.242399 compas_viewer-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 15:21:04.242399 compas_viewer-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.222399 compas_viewer-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.226399 compas_viewer-1.1.2/src/compas_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.230399 compas_viewer-1.1.2/src/compas_viewer/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/delete_selected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/select_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/viewmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/actions/zoom_selected.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.230399 compas_viewer-1.1.2/src/compas_viewer/components/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.230399 compas_viewer-1.1.2/src/compas_viewer/components/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14467 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    22454 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.230399 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/arrow.frag
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/arrow.vert
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/grid.frag
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/grid.vert
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/instance.frag
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/instance.vert
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/model.frag
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/model.vert
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/shader.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/tag.frag
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/tag.vert
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.230399 compas_viewer-1.1.2/src/compas_viewer/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/controller_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.234399 compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/controller.json
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/layout.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/renderer.json
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/viewer.json
--rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/layout_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/renderer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/configurations/viewer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.234399 compas_viewer-1.1.2/src/compas_viewer/controller/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/controller/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/controller/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/gl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.234399 compas_viewer-1.1.2/src/compas_viewer/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/camera_info.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/compas_icon_white.png
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/delete_selected.svg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/export_file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/gl_info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/import_file.svg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/selection_info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/view_front.svg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/view_perspective.svg
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/view_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/view_top.svg
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/icons/zoom_selected.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.238399 compas_viewer-1.1.2/src/compas_viewer/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/collapsiblebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/menubar.py
--rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/propertyform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/sidedock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/statusbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/treeform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/viewport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/layout/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/qt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.242399 compas_viewer-1.1.2/src/compas_viewer/scene/
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/boxobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/brepobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/capsuleobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/circleobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/collectionobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/coneobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/cylinderobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/ellipseobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/frameobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/geometryobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/graphobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/gridobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/lineobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/meshobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/nurbssurfaceobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/planeobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/pointobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/polygonobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/polylineobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)    19009 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/sceneobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/sphereobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/tagobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/torusobject.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/scene/vectorobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/src/compas_viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.242399 compas_viewer-1.1.2/src/compas_viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-22 15:21:04.000000 compas_viewer-1.1.2/src/compas_viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-22 15:21:04.000000 compas_viewer-1.1.2/src/compas_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:21:04.000000 compas_viewer-1.1.2/src/compas_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 15:21:04.000000 compas_viewer-1.1.2/src/compas_viewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-22 15:21:04.000000 compas_viewer-1.1.2/src/compas_viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 15:21:04.000000 compas_viewer-1.1.2/src/compas_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 15:21:04.242399 compas_viewer-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/tests/test_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 15:20:54.000000 compas_viewer-1.1.2/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.462638 compas_viewer-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.466638 compas_viewer-1.1.3/src/compas_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.466638 compas_viewer-1.1.3/src/compas_viewer/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/delete_selected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/select_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/viewmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/actions/zoom_selected.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.470638 compas_viewer-1.1.3/src/compas_viewer/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/button_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/component_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.470638 compas_viewer-1.1.3/src/compas_viewer/components/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.470638 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/arrow.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/arrow.vert
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/grid.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/grid.vert
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/instance.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/instance.vert
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/model.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/model.vert
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/shader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/tag.frag
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/tag.vert
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/setting_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/treeform_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/components/widget_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.474638 compas_viewer-1.1.3/src/compas_viewer/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/controller_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.474638 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/
+-rw-r--r--   0 runner    (1001) docker     (127)   714456 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/FreeSans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/controller.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/layout.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/renderer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/viewer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9158 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/layout_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/renderer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/configurations/viewer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.474638 compas_viewer-1.1.3/src/compas_viewer/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/controller/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/controller/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/gl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.478639 compas_viewer-1.1.3/src/compas_viewer/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/camera_info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/compas_icon_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/delete_selected.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/export_file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/gl_info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/import_file.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/selection_info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_front.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_perspective.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/view_top.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/icons/zoom_selected.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.478639 compas_viewer-1.1.3/src/compas_viewer/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/collapsiblebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/menubar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/propertyform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/sidedock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/treeform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/viewport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/layout/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/qt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.482638 compas_viewer-1.1.3/src/compas_viewer/scene/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/boxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/brepobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/capsuleobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/circleobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/collectionobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/coneobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/cylinderobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/ellipseobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/frameobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/geometryobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/graphobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/gridobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/groupobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/lineobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/meshobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/nurbscurveobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/nurbssurfaceobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/planeobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/pointcloudobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/pointobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/polygonobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/polyhedronobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/polylineobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18821 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/sceneobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/sphereobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/tagobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/torusobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/scene/vectorobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/src/compas_viewer/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/menubar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/ui/viewport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/src/compas_viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/src/compas_viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 18:30:34.000000 compas_viewer-1.1.3/src/compas_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:34.486638 compas_viewer-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/tests/test_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 18:30:20.000000 compas_viewer-1.1.3/tests/test_viewer.py
```

### Comparing `compas_viewer-1.1.2/LICENSE` & `compas_viewer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/PKG-INFO` & `compas_viewer-1.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_viewer
-Version: 1.1.2
+Version: 1.1.3
 Summary: Standalone viewer for COMPAS 2 based on PyOpenGL and PyQt6.
 Author-email: tom van mele <tom.v.mele@gmail.com>, Li Chen <li.chen@arch.ethz.ch>, Zac Zhuo Zhang <zhuo.zhang@arch.ethz.ch>
 License: MIT License
         
         COMPAS Association
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,15 +39,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: compas>=2.0.0
 Requires-Dist: freetype-py
 Requires-Dist: PyOpenGL
-Requires-Dist: PyOpenGL_accelerate
 Requires-Dist: PySide6==6.6.1
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: compas_invocations2; extra == "dev"
 Requires-Dist: compas_notebook; extra == "dev"
```

### Comparing `compas_viewer-1.1.2/README.md` & `compas_viewer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/pyproject.toml` & `compas_viewer-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 compas_viewer = ['config.json']
 "compas_viewer.icons" = ["*.svg", "*.png"]
 "compas_viewer.components.renderer.shaders" = ["*.vert", "*.frag"]
-"compas_viewer.configurations.default_config" = ["*.json", "*.tff"]
+"compas_viewer.configurations.default_config" = ["*.json", "*.ttf"]
 
 # ============================================================================
 # replace pytest.ini
 # ============================================================================
 
 [tool.pytest.ini_options]
 minversion = "6.0"
@@ -76,15 +76,15 @@
 ]
 
 # ============================================================================
 # replace bumpversion.cfg
 # ============================================================================
 
 [tool.bumpversion]
-current_version = "1.1.2"
+current_version = "1.1.3"
 message = "Bump version to {new_version}"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "src/compas_viewer/__init__.py"
 search = "{current_version}"
@@ -96,18 +96,18 @@
 replace = "[{new_version}] {now:%Y-%m-%d}"
 
 # ============================================================================
 # replace setup.cfg
 # ============================================================================
 
 [tool.black]
-line-length = 119
+line-length = 179
 
 [tool.ruff]
-line-length = 119
+line-length = 179
 indent-width = 4
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["E", "F", "I"]
 
 [tool.ruff.lint.per-file-ignores]
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/__init__.py` & `compas_viewer-1.1.3/src/compas_viewer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 
 
 __author__ = ["Li Chen"]
 __copyright__ = "COMPAS Association"
 __license__ = "MIT License"
 __email__ = "li.chen@arch.ethz.ch"
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 
 HERE = os.path.dirname(__file__)
 
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
 DATA = os.path.abspath(os.path.join(HOME, "data"))
 DOCS = os.path.abspath(os.path.join(HOME, "docs"))
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/__main__.py` & `compas_viewer-1.1.3/src/compas_viewer/__main__.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/actions/__init__.py` & `compas_viewer-1.1.3/src/compas_viewer/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/actions/action.py` & `compas_viewer-1.1.3/src/compas_viewer/actions/action.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from abc import abstractmethod
-from typing import TYPE_CHECKING
 
 from PySide6.QtCore import QObject
 from PySide6.QtCore import Signal
 
+from compas_viewer.base import Base
 from compas_viewer.configurations import ActionConfig
 
 from . import get_action_cls
 
-if TYPE_CHECKING:
-    from compas_viewer.viewer import Viewer
 
-
-class Action(QObject):
+class Action(QObject, Base):
     """
     Actions are functions that are called when a certain event happens, such as mouse and keyboard click.
 
     Parameters
     ----------
     name : str
         The name of the action. The key in the configuration dictionary should match the name.
@@ -42,23 +39,21 @@
     ----------
     * https://doc.qt.io/qtforpython-6/PySide6/QtCore/Signal.html
     """
 
     pressed = Signal()
     released = Signal()
 
-    def __new__(cls, name: str, viewer: "Viewer", config: ActionConfig, **kwargs):
+    def __new__(cls, name: str, config: ActionConfig, **kwargs):
         action_cls = get_action_cls(name)
         return super(Action, cls).__new__(action_cls, **kwargs)
 
-    def __init__(self, name: str, viewer: "Viewer", config: ActionConfig):
+    def __init__(self, name: str, config: ActionConfig):
         super().__init__()
         self.name = name
-        self.viewer = viewer
-        self.scene = viewer.scene
         self.config = config
         self.key = self.config.key
         self.modifier = self.config.modifier
         self.pressed.connect(self.pressed_action)
         self.released.connect(self.released_action)
 
     @abstractmethod
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/actions/info.py` & `compas_viewer-1.1.3/src/compas_viewer/actions/info.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/actions/io.py` & `compas_viewer-1.1.3/src/compas_viewer/actions/io.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/actions/viewmode.py` & `compas_viewer-1.1.3/src/compas_viewer/actions/viewmode.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/actions/zoom_selected.py` & `compas_viewer-1.1.3/src/compas_viewer/actions/zoom_selected.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from .action import Action
 
 
 class ZoomSelected(Action):
     """Look at action."""
 
     def pressed_action(self):
-        selected_objs = [obj for obj in self.scene.objects if obj.is_selected]
+        selected_objs = [obj for obj in self.viewer.scene.objects if obj.is_selected]
+        if len(selected_objs) == 0:
+            selected_objs = self.viewer.scene.objects
         extents = []
 
         for obj in selected_objs:
             if obj.bounding_box is not None:
                 obj._update_bounding_box()
                 extents.append(obj.bounding_box)
 
@@ -20,19 +22,15 @@
 
         if len(extents) == 0:
             return
 
         extents = extents.reshape(-1, 3)
         max_corner = extents.max(axis=0)
         min_corner = extents.min(axis=0)
-        self.viewer.renderer.camera.config.scale = float(
-            (norm(max_corner - min_corner)) / 10
-        )  # 10 is a tunned magic number
+        self.viewer.renderer.camera.scale = float((norm(max_corner - min_corner)) / 10)  # 10 is a tunned magic number
         center = (max_corner + min_corner) / 2
         distance = max(norm(max_corner - min_corner), 1)
 
         self.viewer.renderer.camera.target = center
-        vec = (self.viewer.renderer.camera.target - self.viewer.renderer.camera.position) / norm(
-            self.viewer.renderer.camera.target - self.viewer.renderer.camera.position
-        )
+        vec = (self.viewer.renderer.camera.target - self.viewer.renderer.camera.position) / norm(self.viewer.renderer.camera.target - self.viewer.renderer.camera.position)
         self.viewer.renderer.camera.position = self.viewer.renderer.camera.target - vec * distance
         self.viewer.renderer.update()
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/components/renderer/camera.py` & `compas_viewer-1.1.3/src/compas_viewer/components/renderer/camera.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,83 @@
 from math import atan2
 from math import radians
 from math import tan
 from typing import TYPE_CHECKING
-from typing import Callable
 from typing import Optional
 
 from numpy import array
 from numpy import asfortranarray
 from numpy import dot
 from numpy import float32
 from numpy import pi
 from numpy.linalg import det
 from numpy.linalg import norm
 
 from compas.geometry import Rotation
 from compas.geometry import Transformation
 from compas.geometry import Translation
 from compas.geometry import Vector
+from compas_viewer.base import Base
 
 if TYPE_CHECKING:
     # https://peps.python.org/pep-0484/#runtime-or-type-checking
-    from .renderer import Renderer
+    pass
 
 
 class Position(Vector):
-    """
-    The position of the camera.
-
-    Parameters
-    ----------
-    vector : tuple[float, float, float]
-        The position of the camera.
-    on_update : Callable
-        A callback function that is called when the position changes.
-
-    """
-
-    def __init__(self, vector: tuple[float, float, float], on_update: Optional[Callable] = None):
-        self.on_update = on_update
-        self.pause_update = True
+    def __init__(self, vector, on_update=None):
         super().__init__(*vector)
+        self.pause_update = False
+        if on_update:
+            self.on_update = on_update
+
+    def set(self, x, y, z, pause_update=False):
+        pause_update = pause_update or self.pause_update
+        if hasattr(self, "on_update") and not pause_update:
+            self.on_update([x, y, z])
+        self._x = x
+        self._y = y
+        self._z = z
 
     @property
     def x(self):
         return self._x
 
     @x.setter
     def x(self, x):
-        if self.on_update is not None and not self.pause_update:
+        if hasattr(self, "on_update") and not self.pause_update:
             self.on_update([x, self.y, self.z])
         self._x = float(x)
 
     @property
     def y(self):
         return self._y
 
     @y.setter
     def y(self, y):
-        if self.on_update is not None and not self.pause_update:
+        if hasattr(self, "on_update") and not self.pause_update:
             self.on_update([self.x, y, self.z])
         self._y = float(y)
 
     @property
     def z(self):
         return self._z
 
     @z.setter
     def z(self, z):
-        if self.on_update is not None and not self.pause_update:
+        if hasattr(self, "on_update") and not self.pause_update:
             self.on_update([self.x, self.y, z])
         self._z = float(z)
 
-    def set(self, x: float, y: float, z: float, pause_update: bool = False):
-        """Set the position of the camera."""
-        pause_update = pause_update or self.pause_update
-        if self.on_update is not None and not pause_update:
-            self.on_update([x, y, z])
-        self._x = x
-        self._y = y
-        self._z = z
-
 
 class RotationEuler(Position):
     pass
 
 
-class Camera:
+class Camera(Base):
     """Camera object for the default view.
 
     Parameters
     ----------
     renderer : :class:`compas_viewer.components.renderer.Renderer`,
         The parent renderer of the camera.
 
@@ -123,28 +111,41 @@
         Size of one rotation increment.
     pan_delta : float
         Size of one pan increment.
     scale : float
         The scale factor for camera's near, far and pan_delta.
     """
 
-    def __init__(self, renderer: "Renderer"):
-        self.renderer = renderer
-        self.config = renderer.config.camera
-        self._position = Position((0.0, 0.0, 10.0 * self.config.scale), on_update=self._on_position_update)
-        self._rotation = RotationEuler((0, 0, 0), on_update=self._on_rotation_update)
-        self._target = Position((0, 0, 0), on_update=self._on_target_update)
-        self._position.pause_update = False
-        self._rotation.pause_update = False
-        self._target.pause_update = False
-        # Camera position only modifiable in perspective view mode.
-        self.reset_position()
-        if self.renderer.config.viewmode == "perspective":
-            self.position = Position(self.config.position)
-        self.target = Position(self.config.target)
+    def __init__(
+        self,
+        fov: Optional[float] = 45.0,
+        near: Optional[float] = 0.1,
+        far: Optional[float] = 1000.0,
+        init_position: Optional[tuple] = [10.0, 10.0, 10.0],
+        init_target: Optional[tuple] = [0.0, 0.0, 0.0],
+        scale: Optional[float] = 1.0,
+        zoomdelta: Optional[float] = 0.05,
+        rotationdelta: Optional[float] = 0.01,
+        pan_delta: Optional[float] = 0.05,
+    ) -> None:
+        self.fov = fov
+        self.near = near
+        self.far = far
+        self.scale = scale
+        self.zoomdelta = zoomdelta
+        self.rotationdelta = rotationdelta
+        self.pan_delta = pan_delta
+
+        self._position = Position([0, 0, 10 * scale], on_update=self._on_position_update)
+        self._rotation = RotationEuler([0, 0, 0], on_update=self._on_rotation_update)
+        self._target = Position([0, 0, 0], on_update=self._on_target_update)
+
+        self.reset_position(viewmode="perspective")
+        self.target.set(*init_target)
+        self.position.set(*init_position)
 
     @property
     def position(self) -> Position:
         """The position of the camera."""
         return self._position
 
     @position.setter
@@ -273,17 +274,15 @@
 
         old_direction_xy /= old_direction_xy_distance or 1
         new_direction_xy /= new_direction_xy_distance or 1
         old_direction_pitch /= old_direction_pitch_distance
         new_direction_pitch /= new_direction_pitch_distance
 
         angle_z = atan2(det([old_direction_xy, new_direction_xy]), dot(old_direction_xy, new_direction_xy))
-        angle_x = -atan2(
-            det([old_direction_pitch, new_direction_pitch]), dot(old_direction_pitch, new_direction_pitch)
-        )
+        angle_x = -atan2(det([old_direction_pitch, new_direction_pitch]), dot(old_direction_pitch, new_direction_pitch))
 
         new_rotation = self.rotation + [angle_x or 0, 0, angle_z or 0]
         self.rotation.set(*new_rotation, pause_update=True)
 
     def _on_rotation_update(self, rotation):
         """Update camera position when rotation around target."""
         R = Rotation.from_euler_angles(rotation)
@@ -301,24 +300,26 @@
         M = (R * T).matrix
         vector = [M[i][3] for i in range(3)]
         position = Vector(*target) + Vector(*vector)
 
         self.target.set(*target, pause_update=True)
         self.position.set(*position, pause_update=True)
 
-    def reset_position(self):
+    def reset_position(self, viewmode: Optional[str] = None):
         """Reset the position of the camera based current view type."""
         self.target.set(0, 0, 0, False)
-        if self.renderer.viewmode == "perspective":
+        viewmode = viewmode or self.viewer.renderer.viewmode
+
+        if viewmode == "perspective":
             self.rotation.set(pi / 4, 0, -pi / 4, False)
-        if self.renderer.viewmode == "top":
+        if viewmode == "top":
             self.rotation.set(0, 0, 0, False)
-        if self.renderer.viewmode == "front":
+        if viewmode == "front":
             self.rotation.set(pi / 2, 0, 0, False)
-        if self.renderer.viewmode == "right":
+        if viewmode == "right":
             self.rotation.set(pi / 2, 0, pi / 2, False)
 
     def rotate(self, dx: float, dy: float):
         """Rotate the camera based on current mouse movement.
 
         Parameters
         ----------
@@ -331,48 +332,46 @@
 
         Notes
         -----
         Camera rotations are only available if the current view mode
         is a perspective view (``camera.renderer.config.viewmode == "perspective"``).
 
         """
-        if self.renderer.config.viewmode == "perspective":
-            self.rotation += [-self.config.rotationdelta * dy, 0, -self.config.rotationdelta * dx]
+        if self.viewer.renderer.config.viewmode == "perspective":
+            self.rotation += [-self.rotationdelta * dy, 0, -self.rotationdelta * dx]
 
     def pan(self, dx: float, dy: float):
         """Pan the camera based on current mouse movement.
 
         Parameters
         ----------
         dx : float
             Number of "pan" increments in the "X" direction of the current view,
             with each increment the size of :attr:`Camera.pan_delta`.
         dy : float
             Number of "pan" increments in the "Y" direction of the current view,
             with each increment the size of :attr:`Camera.pan_delta`.
         """
         R = Rotation.from_euler_angles(self.rotation)
-        T = Translation.from_vector(
-            [-dx * self.config.pan_delta * self.config.scale, dy * self.config.pan_delta * self.config.scale, 0]
-        )
+        T = Translation.from_vector([-dx * self.pan_delta * self.scale, dy * self.pan_delta * self.scale, 0])
         M = (R * T).matrix
         vector = [M[i][3] for i in range(3)]
         self.target += vector
 
     def zoom(self, steps: float = 1):
         """Zoom in or out.
 
         Parameters
         ----------
         steps : float
             The number of zoom increments, with each increment the size
             of :attr:`compas_viewer.components.renderer.Camera.config.zoomdelta`.
 
         """
-        self.distance -= steps * self.config.zoomdelta * self.distance
+        self.distance -= steps * self.zoomdelta * self.distance
 
     def projection(self, width: int, height: int) -> list[list[float]]:
         """Compute the projection matrix corresponding to the current camera settings.
 
         Parameters
         ----------
         width : int
@@ -387,26 +386,22 @@
 
         Notes
         -----
         The projection matrix transforms the scene from camera coordinates to screen coordinates.
 
         """
         aspect = width / height
-        if self.renderer.viewmode == "perspective":
-            P = self.perspective(
-                self.config.fov, aspect, self.config.near * self.config.scale, self.config.far * self.config.scale
-            )
+        if self.viewer.renderer.viewmode == "perspective":
+            P = self.perspective(self.fov, aspect, self.near * self.scale, self.far * self.scale)
         else:
             left = -self.distance
             right = self.distance
             bottom = -self.distance / aspect
             top = self.distance / aspect
-            P = self.ortho(
-                left, right, bottom, top, self.config.near * self.config.scale, self.config.far * self.config.scale
-            )
+            P = self.ortho(left, right, bottom, top, self.near * self.scale, self.far * self.scale)
         return list(asfortranarray(P, dtype=float32))
 
     def viewworld(self) -> list[list[float]]:
         """Compute the view-world matrix corresponding to the current camera settings.
 
         Returns
         -------
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/components/renderer/renderer.py` & `compas_viewer-1.1.3/src/compas_viewer/components/renderer/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,66 +9,64 @@
 from PySide6.QtGui import QKeyEvent
 from PySide6.QtGui import QMouseEvent
 from PySide6.QtGui import QWheelEvent
 from PySide6.QtOpenGLWidgets import QOpenGLWidget
 
 from compas.geometry import Frame
 from compas.geometry import transform_points_numpy
+from compas_viewer.base import Base
 from compas_viewer.configurations import RendererConfig
 from compas_viewer.scene import TagObject
-from compas_viewer.scene.collectionobject import CollectionObject
 from compas_viewer.scene.vectorobject import VectorObject
 
 from .camera import Camera
 from .selector import Selector
 from .shaders import Shader
 
 if TYPE_CHECKING:
     # https://peps.python.org/pep-0484/#runtime-or-type-checking
-    from compas_viewer import Viewer
+    # from compas_viewer import Viewer
     from compas_viewer.scene.gridobject import GridObject
     from compas_viewer.scene.meshobject import MeshObject
 
 
-class Renderer(QOpenGLWidget):
+class Renderer(QOpenGLWidget, Base):
     """
     Renderer class for 3D rendering of COMPAS geometry.
     We constantly use OpenGL version 2.1 and GLSL 120 with a Compatibility Profile at the moment.
     The width and height are not in its configuration since they are set by the parent layout.
 
     Parameters
     ----------
     viewer : :class:`compas_viewer.viewer.Viewer`
         The viewer instance.
     config : :class:`compas_viewer.configurations.RendererConfig`
         The renderer configuration.
     """
 
-    def __init__(self, viewer: "Viewer", config: RendererConfig):
+    def __init__(self, config: RendererConfig):
         super().__init__()
 
         self.config = config
-        self.viewer = viewer
-        self.scene = viewer.scene
 
         self._viewmode = self.config.viewmode
         self._rendermode = self.config.rendermode
         self._opacity = self.config.ghostopacity if self.rendermode == "ghosted" else 1.0
 
         self._frames = 0
         self._now = time.time()
 
         self.shader_model: Shader
         self.shader_tag: Shader
         self.shader_arrow: Shader
         self.shader_instance: Shader
         self.shader_grid: Shader
 
-        self.camera = Camera(self)
-        self.selector = Selector(self)
+        self.camera = Camera()
+        self.selector = Selector()
         self.grid: "GridObject"
 
         self.setFocusPolicy(QtCore.Qt.FocusPolicy.StrongFocus)
         self.grabGesture(QtCore.Qt.PinchGesture)
 
     @property
     def rendermode(self):
@@ -109,15 +107,15 @@
     @viewmode.setter
     def viewmode(self, viewmode):
         self._viewmode = viewmode
         self.config.viewmode = viewmode
         self.shader_model.bind()
         self.shader_model.uniform4x4(
             "projection",
-            self.camera.projection(self.viewer.layout.config.window.width, self.viewer.layout.config.window.height),
+            self.camera.projection(self.viewer.config.window.width, self.viewer.config.window.height),
         )
         self.shader_model.release()
         self.camera.reset_position()
         self.update_projection()
         self.update()
 
     @property
@@ -190,16 +188,16 @@
         This implements the virtual function of the OpenGL widget.
 
         References
         ----------
         * https://doc.qt.io/qtforpython-6/PySide6/QtOpenGL/QOpenGLWindow.html#PySide6.QtOpenGL.PySide6.QtOpenGL.QOpenGLWindow.resizeGL
 
         """
-        self.viewer.layout.config.window.width = w
-        self.viewer.layout.config.window.height = h
+        self.viewer.config.window.width = w
+        self.viewer.config.window.height = h
         GL.glViewport(0, 0, w, h)
         self.resize(w, h)
 
     def paintGL(self, is_instance: bool = False):
         """Paint the OpenGL canvas.
 
         Parameters
@@ -264,15 +262,15 @@
 
         References
         ----------
         * https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QWidget.html#PySide6.QtWidgets.PySide6.QtWidgets.QWidget.mouseMoveEvent
 
         """
         if self.isActiveWindow() and self.underMouse():
-            self.viewer.controller.mouse_move_action(self, event)
+            self.viewer.controller.mouse_move_action(event)
             self.update()
 
     def mousePressEvent(self, event: QMouseEvent):
         """
         Callback for the mouse press event which passes the event to the controller.
 
         Parameters
@@ -286,15 +284,15 @@
 
         References
         ----------
         * https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QWidget.html#PySide6.QtWidgets.PySide6.QtWidgets.QWidget.mousePressEvent
 
         """
         if self.isActiveWindow() and self.underMouse():
-            self.viewer.controller.mouse_press_action(self, event)
+            self.viewer.controller.mouse_press_action(event)
             self.update()
 
     def mouseReleaseEvent(self, event: QMouseEvent):
         """
         Callback for the release press event which passes the event to the controller.
 
         Parameters
@@ -308,15 +306,15 @@
 
         References
         ----------
         * https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QWidget.html#PySide6.QtWidgets.PySide6.QtWidgets.QWidget.mouseReleaseEvent
 
         """
         if self.isActiveWindow() and self.underMouse():
-            self.viewer.controller.mouse_release_action(self, event)
+            self.viewer.controller.mouse_release_action(event)
             self.update()
 
     def gestureEvent(self, event):
         """
         Callback for the gesture event which passes the event to the controller.
 
         Parameters
@@ -324,16 +322,19 @@
         event : :PySide6:`PySide6/QtCore/QEvent`
             The Qt event.
 
         """
         # Handle pinch gestures
         pinch = event.gesture(QtCore.Qt.PinchGesture)
         if pinch:
-            self.viewer.controller.pinch_action(self, pinch)
+            self.viewer.controller.pinch_action(pinch)
             self.update()
+            return True
+        else:
+            return False
 
     def wheelEvent(self, event: QWheelEvent):
         """
         Callback for the mouse wheel event which passes the event to the controller.
 
         Parameters
         ----------
@@ -346,15 +347,15 @@
 
         References
         ----------
         * https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QWidget.html#PySide6.QtWidgets.PySide6.QtWidgets.QWidget.wheelEvent
 
         """
         if self.isActiveWindow() and self.underMouse():
-            self.viewer.controller.wheel_action(self, event)
+            self.viewer.controller.wheel_action(event)
             self.update()
 
     def keyPressEvent(self, event: QKeyEvent):
         """
         Callback for the key press event which passes the event to the controller.
 
         Parameters
@@ -367,15 +368,15 @@
         :func:`compas_viewer.controller.Controller.key_press_action`
 
         References
         ----------
         * https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QWidget.html#PySide6.QtWidgets.PySide6.QtWidgets.QWidget.keyPressEvent
 
         """
-        self.viewer.controller.key_press_action(self, event)
+        self.viewer.controller.key_press_action(event)
 
     def keyReleaseEvent(self, event: QKeyEvent):
         """
         Callback for the key release event which passes the event to the controller.
 
         Parameters
         ----------
@@ -387,41 +388,39 @@
         :func:`compas_viewer.controller.Controller.key_release_action`
 
         References
         ----------
         * https://doc.qt.io/qtforpython-6/PySide6/QtWidgets/QWidget.html#PySide6.QtWidgets.PySide6.QtWidgets.QWidget.keyReleaseEvent
 
         """
-        self.viewer.controller.key_release_action(self, event)
+        self.viewer.controller.key_release_action(event)
 
     # ==========================================================================
     # view
     # ==========================================================================
 
     def init(self):
         """Initialize the renderer."""
 
         # Init the grid
-        self.grid: GridObject = self.scene.add(  # type: ignore
+        self.grid: GridObject = self.viewer.scene.add(  # type: ignore
             Frame.worldXY(),
             framesize=self.config.gridsize,
             show_framez=self.config.show_gridz,
             is_selected=False,
             is_locked=True,
             is_visible=self.config.show_grid,
         )
         self.grid.init()  # type: ignore
 
         # Init the buffers
-        for obj in self.scene.objects:
+        for obj in self.viewer.scene.objects:
             obj.init()
 
-        projection = self.camera.projection(
-            self.viewer.layout.config.window.width, self.viewer.layout.config.window.height
-        )
+        projection = self.camera.projection(self.viewer.config.window.width, self.viewer.config.window.height)
         viewworld = self.camera.viewworld()
         transform = list(identity(4, dtype=float32))
         # create the program
 
         self.shader_model = Shader(name="model")
         self.shader_model.bind()
         self.shader_model.uniform4x4("projection", projection)
@@ -442,17 +441,15 @@
 
         self.shader_arrow = Shader(name="arrow")
         self.shader_arrow.bind()
         self.shader_arrow.uniform4x4("projection", projection)
         self.shader_arrow.uniform4x4("viewworld", viewworld)
         self.shader_arrow.uniform4x4("transform", transform)
         self.shader_arrow.uniform1f("opacity", self.opacity)
-        self.shader_arrow.uniform1f(
-            "aspect", self.viewer.layout.config.window.width / self.viewer.layout.config.window.height
-        )
+        self.shader_arrow.uniform1f("aspect", self.viewer.config.window.width / self.viewer.config.window.height)
         self.shader_arrow.release()
 
         self.shader_instance = Shader(name="instance")
         self.shader_instance.bind()
         self.shader_instance.uniform4x4("projection", projection)
         self.shader_instance.uniform4x4("viewworld", viewworld)
         self.shader_instance.uniform4x4("transform", transform)
@@ -472,16 +469,16 @@
         Parameters
         ----------
         w : int, optional
             The width of the renderer, by default None.
         h : int, optional
             The height of the renderer, by default None.
         """
-        w = w or self.viewer.layout.config.window.width
-        h = h or self.viewer.layout.config.window.height
+        w = w or self.viewer.config.window.width
+        h = h or self.viewer.config.window.height
 
         projection = self.camera.projection(w, h)
         self.shader_model.bind()
         self.shader_model.uniform4x4("projection", projection)
         self.shader_model.release()
 
         self.shader_tag.bind()
@@ -542,17 +539,15 @@
         if transparent_objects:
             centers = transform_points_numpy(centers, viewworld)
             transparent_objects = sorted(zip(transparent_objects, centers), key=lambda pair: pair[1][2])
             transparent_objects, _ = zip(*transparent_objects)
         return opaque_objects + list(transparent_objects)
 
     @lru_cache(maxsize=3)
-    def sort_objects_from_category(
-        self, objs: tuple["MeshObject"]
-    ) -> tuple[list["TagObject"], list["VectorObject"], list["MeshObject"]]:
+    def sort_objects_from_category(self, objs: tuple["MeshObject"]) -> tuple[list["TagObject"], list["VectorObject"], list["MeshObject"]]:
         """Sort objects by their categories
 
         Returns
         -------
         tuple(list[:class:`compas_viewer.scene.tagobject.TagObject`],
         list[:class:`compas_viewer.scene.vectorobject.VectorObject`],
         list[:class:`compas_viewer.scene.sceneobject.MeshObject`])
@@ -576,18 +571,15 @@
                 tag_objs.append(obj)
             elif isinstance(obj, VectorObject):
                 vector_objs.append(obj)
             else:
                 mesh_objs.append(obj)
 
         for obj in objs:
-            if isinstance(obj, CollectionObject):
-                [sort(item) for item in obj.objects]
-            else:
-                sort(obj)
+            sort(obj)
 
         return tag_objs, vector_objs, mesh_objs
 
     def paint(self):
         """
         Paint all the items in the render, which only be called by the paintGL function
         and determines the performance of the renders
@@ -600,17 +592,15 @@
         :func:`compas_viewer.components.render.Render.paint_instance`
         """
 
         #  Matrix update
         viewworld = self.camera.viewworld()
         self.update_projection()
         # Object categorization
-        tag_objs, vector_objs, mesh_objs = self.sort_objects_from_category(
-            (obj for obj in self.scene.objects if obj.is_visible)
-        )
+        tag_objs, vector_objs, mesh_objs = self.sort_objects_from_category((obj for obj in self.viewer.scene.objects if obj.is_visible))
 
         # Draw model objects in the scene
         self.shader_model.bind()
         self.shader_model.uniform4x4("viewworld", viewworld)
         for obj in self.sort_objects_from_viewworld(mesh_objs, viewworld):
             obj.draw(self.shader_model, self.rendermode == "wireframe", self.rendermode == "lighted")
         self.shader_model.release()
@@ -626,24 +616,24 @@
         self.shader_tag.bind()
         self.shader_tag.uniform4x4("viewworld", viewworld)
         for obj in tag_objs:
             obj.draw(self.shader_tag, self.camera.position)
         self.shader_tag.release()
 
         # draw 2D box for multi-selection
-        if self.selector.on_drag_selection and self.selector.enable_selector:
+        if self.selector.on_drag_selection:
             self.shader_model.draw_2d_box(
                 (
                     self.selector.drag_start_pt.x(),
                     self.selector.drag_start_pt.y(),
                     self.viewer.controller.mouse.last_pos.x(),
                     self.viewer.controller.mouse.last_pos.y(),
                 ),
-                self.viewer.layout.config.window.width,
-                self.viewer.layout.config.window.height,
+                self.viewer.config.window.width,
+                self.viewer.config.window.height,
             )
 
     def paint_instance(self):
         """
         Independent drawing function for the  instance map,
         which is only called by the :class:`compas_viewer.components.render.Render.paintGL` function.
 
@@ -654,15 +644,15 @@
 
         """
 
         #  Matrix update
         viewworld = self.camera.viewworld()
         self.update_projection()
         # Object categorization
-        _, _, mesh_objs = self.sort_objects_from_category(tuple(self.scene.objects))
+        _, _, mesh_objs = self.sort_objects_from_category(tuple(self.viewer.scene.objects))
         # Draw instance maps
         GL.glDisable(GL.GL_POINT_SMOOTH)
         GL.glDisable(GL.GL_LINE_SMOOTH)
 
         self.shader_instance.bind()
         self.shader_instance.uniform4x4("viewworld", viewworld)
         for obj in mesh_objs:
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/components/renderer/selector.py` & `compas_viewer-1.1.3/src/compas_viewer/components/renderer/selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import TYPE_CHECKING
-
 from numpy import all
 from numpy import any
 from numpy import array
 from numpy import frombuffer
 from numpy import uint8
 from numpy import unique
 from OpenGL import GL
 from PySide6.QtCore import QObject
 from PySide6.QtCore import QPoint
 from PySide6.QtCore import Signal
 
-if TYPE_CHECKING:
-    from .renderer import Renderer
+from compas.colors import Color
+from compas_viewer.base import Base
 
 
-class Selector(QObject):
+class Selector(QObject, Base):
     """Selector class manages all selection operations for the viewer.
 
     Parameters
     ----------
     renderer : :class:`compas_viewer.components.renderer.Renderer`
         The renderer instance.
 
@@ -47,27 +45,17 @@
 
     select = Signal()
     deselect = Signal()
     multiselect = Signal()
     drag_selection = Signal()
     drag_deselection = Signal()
 
-    def __init__(
-        self,
-        renderer: "Renderer",
-    ):
-        self.enable_selector = renderer.config.selector.enable_selector
-        if not self.enable_selector:
-            return
+    def __init__(self):
         super().__init__()
-        self.renderer = renderer
-        self.viewer = renderer.viewer
-        self.scene = renderer.scene
-        self.controller = renderer.viewer.controller
-        self.selectioncolor = renderer.config.selector.selectioncolor
+        self.selectioncolor = Color(0, 0, 0)
 
         #  Drag selection
         self.on_drag_selection: bool = False
         self.drag_start_pt: QPoint
         self.drag_end_pt: QPoint
 
         self.select.connect(self.select_action)
@@ -76,110 +64,100 @@
         self.drag_selection.connect(self.drag_selection_action)
         self.drag_deselection.connect(self.drag_deselection_action)
 
     def select_action(self):
         """Select the object under the mouse cursor."""
 
         # Deselect all objects first
-        for _, obj in self.renderer.scene.instance_colors.items():
+        for _, obj in self.viewer.scene.instance_colors.items():
             obj.is_selected = False
 
-        x = self.controller.mouse.last_pos.x()
-        y = self.controller.mouse.last_pos.y()
+        x = self.viewer.controller.mouse.last_pos.x()
+        y = self.viewer.controller.mouse.last_pos.y()
         instance_color = self.read_instance_color((x, y, x, y))
         unique_color = unique(instance_color, axis=0, return_counts=False)
 
-        selected_obj = self.renderer.scene.instance_colors.get(tuple(unique_color[0]))  # type: ignore
+        selected_obj = self.viewer.scene.instance_colors.get(tuple(unique_color[0]))  # type: ignore
         if selected_obj:
             selected_obj.is_selected = True
 
         # Update the layout.
-        self.viewer.layout.update()
+        # TODO: This is a temporary solution to update the layout.
+        # self.viewer.layout.update()
 
     def deselect_action(self):
         """Deselect the object under the mouse cursor."""
 
-        x = self.controller.mouse.last_pos.x()
-        y = self.controller.mouse.last_pos.y()
+        x = self.viewer.controller.mouse.last_pos.x()
+        y = self.viewer.controller.mouse.last_pos.y()
         instance_color = self.read_instance_color((x, y, x, y))
         unique_color = unique(instance_color, axis=0, return_counts=False)
 
-        selected_obj = self.renderer.scene.instance_colors.get(tuple(unique_color[0]))  # type: ignore
+        selected_obj = self.viewer.scene.instance_colors.get(tuple(unique_color[0]))  # type: ignore
         if selected_obj:
             selected_obj.is_selected = False
 
     def multiselect_action(self):
         """Multiselect the object under the mouse cursor. Similar to the select action.
 
         See Also
         --------
         :func:`compas_viewer.components.renderer.selector.Selector.select_action`
         """
-        x = self.controller.mouse.last_pos.x()
-        y = self.controller.mouse.last_pos.y()
+        x = self.viewer.controller.mouse.last_pos.x()
+        y = self.viewer.controller.mouse.last_pos.y()
         instance_color = self.read_instance_color((x, y, x, y))
         unique_color = unique(instance_color, axis=0, return_counts=False)
 
-        selected_obj = self.renderer.scene.instance_colors.get(tuple(unique_color[0]))  # type: ignore
+        selected_obj = self.viewer.scene.instance_colors.get(tuple(unique_color[0]))  # type: ignore
         if selected_obj:
             selected_obj.is_selected = True
 
         # Update the layout.
         self.viewer.layout.update()
 
     def drag_selection_action(self):
         """Drag select the objects in the rectangle area."""
 
         # Ignore drag selection caused by small mouse shift.
-        if (
-            abs(self.drag_start_pt.x() - self.drag_end_pt.x()) * abs(self.drag_start_pt.y() - self.drag_end_pt.y())
-            <= 4
-        ):
+        if abs(self.drag_start_pt.x() - self.drag_end_pt.x()) * abs(self.drag_start_pt.y() - self.drag_end_pt.y()) <= 4:
             return
 
         # Deselect all objects first
-        for _, obj in self.renderer.scene.instance_colors.items():
+        for _, obj in self.viewer.scene.instance_colors.items():
             obj.is_selected = False
 
-        instance_color = self.read_instance_color(
-            (self.drag_start_pt.x(), self.drag_start_pt.y(), self.drag_end_pt.x(), self.drag_end_pt.y())
-        )
+        instance_color = self.read_instance_color((self.drag_start_pt.x(), self.drag_start_pt.y(), self.drag_end_pt.x(), self.drag_end_pt.y()))
         unique_colors = unique(instance_color, axis=0, return_counts=True)
-        unique_colors = array(
-            [unique_colors[0][i] for i, count in enumerate(unique_colors[1]) if count > self.ANTI_ALIASING_FACTOR]
-        )
+        unique_colors = array([unique_colors[0][i] for i, count in enumerate(unique_colors[1]) if count > self.ANTI_ALIASING_FACTOR])
 
         if len(unique_colors) == 0:
             return
 
-        for color, obj in self.renderer.scene.instance_colors.items():
+        for color, obj in self.viewer.scene.instance_colors.items():
             if any(all(color == unique_colors, axis=1)):
                 obj.is_selected = True
                 continue
 
     def drag_deselection_action(self):
         """Drag deselect the objects in the rectangle area. Similar to the drag selection action.
 
         See Also
         --------
         :func:`compas_viewer.components.renderer.selector.Selector.drag_selection_action`
         """
 
-        instance_color = self.read_instance_color(
-            (self.drag_start_pt.x(), self.drag_start_pt.y(), self.drag_end_pt.x(), self.drag_end_pt.y())
-        )
+        instance_color = self.read_instance_color((self.drag_start_pt.x(), self.drag_start_pt.y(), self.drag_end_pt.x(), self.drag_end_pt.y()))
         unique_colors = unique(instance_color, axis=0, return_counts=True)
-        unique_colors = array(
-            [unique_colors[0][i] for i, count in enumerate(unique_colors[1]) if count > self.ANTI_ALIASING_FACTOR]
-        )
+        unique_colors = array([unique_colors[0][i] for i, count in enumerate(unique_colors[1]) if count > self.ANTI_ALIASING_FACTOR])
 
         if len(unique_colors) == 0:
             return
 
-        for color, obj in self.renderer.scene.instance_colors.items():
+        for color, obj in self.viewer.scene.instance_colors.items():
             if any(all(color == unique_colors, axis=1)):
                 obj.is_selected = False
                 continue
 
     def read_instance_color(self, box: tuple[int, int, int, int]):
         """
         Paint the instance map quickly, and then read the color of the specified area.
@@ -213,22 +191,22 @@
         * https://doc.qt.io/qt-6/qscreen.html#devicePixelRatio-prop
         * https://registry.khronos.org/OpenGL-Refpages/gl4/html/glReadPixels.xhtml
         * https://doc.qt.io/qt-6/qopenglwidget.html#makeCurrent
         """
 
         # 0. Get the rectangle area.
         x1, y1, x2, y2 = box
-        x, y = min(x1, x2), self.viewer.layout.config.window.height - max(y1, y2)
+        x, y = min(x1, x2), self.viewer.config.window.height - max(y1, y2)
         width = max(self.PIXEL_SELECTION_INCREMENTAL, abs(x1 - x2))
         height = max(self.PIXEL_SELECTION_INCREMENTAL, abs(y1 - y2))
-        r = self.renderer.devicePixelRatio()
+        r = self.viewer.renderer.devicePixelRatio()
 
         # 1. Repaint the canvas with instance color.
-        self.renderer.makeCurrent()
-        self.renderer.paintGL(is_instance=True)
+        self.viewer.renderer.makeCurrent()
+        self.viewer.renderer.paintGL(is_instance=True)
 
         # 2. Read the instance buffer.
         instance_buffer = GL.glReadPixels(x * r, y * r, width * r, height * r, GL.GL_RGB, GL.GL_UNSIGNED_BYTE)
 
         # 3. Return the instance color.
         #      From 1-3, the canvas goes through a quick repaint process, which should be not noticeable to the user.
         instance_map = frombuffer(buffer=instance_buffer, dtype=uint8).reshape(-1, 3)
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/model.frag` & `compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/model.frag`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/components/renderer/shaders/shader.py` & `compas_viewer-1.1.3/src/compas_viewer/components/renderer/shaders/shader.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/config.py` & `compas_viewer-1.1.3/src/compas_viewer/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,24 @@
     up: list[float] = field(default_factory=lambda: [0, 0, 1])
     near: float = 0.1
     far: float = 1000
     fov: float = 50
 
 
 @dataclass
+class DisplayConfig(Base):
+    pointcolor: Color = field(default_factory=Color.black)
+    linecolor: Color = field(default_factory=Color.black)
+    surfacecolor: Color = field(default_factory=Color.grey)
+    pointsize: float = float(6.0)
+    linewidth: float = float(1.0)
+    opacity: float = float(1.0)
+
+
+@dataclass
 class View3dConfig(Base):
     viewport: Literal["top", "perspective"] = "perspective"
     background: Color = field(default_factory=lambda: Color.from_hex("#eeeeee"))
     show_grid: bool = True
     show_axes: bool = True
     camera: CameraConfig = field(default_factory=CameraConfig)
 
@@ -95,14 +105,15 @@
 @dataclass
 class UIConfig(Base):
     menubar: MenubarConfig = field(default_factory=MenubarConfig)
     toolbar: ToolbarConfig = field(default_factory=ToolbarConfig)
     statusbar: StatusbarConfig = field(default_factory=StatusbarConfig)
     sidebar: SidebarConfig = field(default_factory=SidebarConfig)
     view3d: View3dConfig = field(default_factory=View3dConfig)
+    display: DisplayConfig = field(default_factory=DisplayConfig)
 
 
 @dataclass
 class ControllerConfig(Base):
     pass
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/__init__.py` & `compas_viewer-1.1.3/src/compas_viewer/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/controller_config.py` & `compas_viewer-1.1.3/src/compas_viewer/configurations/controller_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,15 @@
         self.drag_deselection = MouseConfig(*drag_deselection)
         self.multiselect = MouseConfig(*multiselect)
         self.deselect = MouseConfig(*deselect)
         self.actions = {k: ActionConfig(*v) for k, v in actions.items()}
 
     @classmethod
     def from_default(cls) -> "ControllerConfig":
-        controller_config = ControllerConfig.from_json(
-            Path(HERE, "configurations", "default_config", "controller.json")
-        )
+        controller_config = ControllerConfig.from_json(Path(HERE, "configurations", "default_config", "controller.json"))
         if not isinstance(controller_config, ControllerConfig):
             raise TypeError(f"The {controller_config} is not a valid controller configuration file.")
         return controller_config
 
     @classmethod
     def from_json(cls, filepath) -> "ControllerConfig":
         controller_config = super().from_json(filepath)
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/controller.json` & `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/controller.json`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/layout.json` & `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/layout.json`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/renderer.json` & `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/renderer.json`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/default_config/viewer.json` & `compas_viewer-1.1.3/src/compas_viewer/configurations/default_config/viewer.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'data'": "{'linewidth': 1.0, 'pointsize': 10.0, delete: ['lineswidth', 'pointssize']}"}*

```diff
@@ -12,26 +12,26 @@
                 "alpha": 1.0,
                 "blue": 0.4,
                 "green": 0.4,
                 "red": 0.4
             },
             "dtype": "compas.colors/Color"
         },
-        "lineswidth": 1.0,
+        "linewidth": 1.0,
         "opacity": 1.0,
         "pointcolor": {
             "data": {
                 "alpha": 1.0,
                 "blue": 0.2,
                 "green": 0.2,
                 "red": 0.2
             },
             "dtype": "compas.colors/Color"
         },
-        "pointssize": 10.0,
+        "pointsize": 10.0,
         "show_faces": true,
         "show_framez": true,
         "show_lines": true,
         "show_points": true,
         "surfacecolor": {
             "data": {
                 "alpha": 1.0,
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/layout_config.py` & `compas_viewer-1.1.3/src/compas_viewer/configurations/layout_config.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/renderer_config.py` & `compas_viewer-1.1.3/src/compas_viewer/configurations/renderer_config.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/configurations/viewer_config.py` & `compas_viewer-1.1.3/src/compas_viewer/configurations/viewer_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,17 @@
         The default color of the surfaces.
     show_points : bool
         The default setting for showing the points.
     show_lines : bool
         The default setting for showing the lines.
     show_faces : bool
         The default setting for showing the faces.
-    lineswidth : float
+    linewidth : float
         The default width of the lines.
-    pointssize : float
+    pointsize : float
         The default size of the points.
     opacity : float
         The default opacity of the objects.
     hide_coplanaredges : bool
         The default setting for hiding the coplanar edges.
     use_vertexcolors : bool
         The default setting for using the vertex colors.
@@ -52,16 +52,16 @@
         self,
         pointcolor: Color,
         linecolor: Color,
         surfacecolor: Color,
         show_points: bool,
         show_lines: bool,
         show_faces: bool,
-        lineswidth: float,
-        pointssize: float,
+        linewidth: float,
+        pointsize: float,
         opacity: float,
         hide_coplanaredges: bool,
         use_vertexcolors: bool,
         framesize: tuple[float, int, float, int],
         show_framez: bool,
         vectorsize: float,
     ):
@@ -69,16 +69,16 @@
 
         self.pointcolor = pointcolor
         self.linecolor = linecolor
         self.surfacecolor = surfacecolor
         self.show_points = show_points
         self.show_lines = show_lines
         self.show_faces = show_faces
-        self.lineswidth = lineswidth
-        self.pointssize = pointssize
+        self.linewidth = linewidth
+        self.pointsize = pointsize
         self.opacity = opacity
         self.hide_coplanaredges = hide_coplanaredges
         self.use_vertexcolors = use_vertexcolors
         self.framesize = framesize
         self.show_framez = show_framez
         self.vectorsize = vectorsize
         if self.vectorsize < 0 or self.vectorsize > 1:
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/controller/controller.py` & `compas_viewer-1.1.3/src/compas_viewer/controller/controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from typing import TYPE_CHECKING
-
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QKeyEvent
 from PySide6.QtGui import QMouseEvent
 from PySide6.QtGui import QWheelEvent
 from PySide6.QtWidgets import QApplication
 from PySide6.QtWidgets import QPinchGesture
 
 from compas_viewer.actions import Action
+from compas_viewer.base import Base
 from compas_viewer.configurations import ControllerConfig
 
 from .mouse import Mouse
 
-if TYPE_CHECKING:
-    from compas_viewer.components import Renderer
-    from compas_viewer.viewer import Viewer
-
 
-class Controller:
+class Controller(Base):
     """
     The Controller class is the main entry of all the key and mouse events.
     It is used to manage actions and events in the viewer.
 
     Parameters
     ----------
     viewer : :class:`compas_viewer.viewer.Viewer`
@@ -35,27 +30,26 @@
         The viewer object.
     config : :class:`compas_viewer.configurations.controller_config.ControllerConfig`
         The controller configuration.
     mouse : :class:`compas_viewer.controller.mouse.Mouse`
         The mouse object.
     """
 
-    def __init__(self, viewer: "Viewer", config: ControllerConfig):
-        self.viewer = viewer
+    def __init__(self, config: ControllerConfig):
         self.config = config
         self.mouse = Mouse()
         self.actions: dict[str, Action] = {}
         for k, v in self.config.actions.items():
-            self.actions[k] = Action(k, self.viewer, v)
+            self.actions[k] = Action(k, v)
 
     # ==============================================================================
     # Actions
     # ==============================================================================
 
-    def mouse_move_action(self, renderer: "Renderer", event: QMouseEvent):
+    def mouse_move_action(self, event: QMouseEvent):
         """
         The mouse move action of the renderer object.
         This function introduces elif for different actions, meaning only one action can be performed at a time.
 
         Parameters
         ----------
         renderer : :class:`compas_viewer.components.renderer.Renderer`
@@ -67,144 +61,126 @@
         # Record mouse position
         self.mouse.pos = event.pos()
         # Compute displacement
         dx = self.mouse.dx()
         dy = self.mouse.dy()
 
         # Drag selection
-        if (
-            event.buttons() == self.config.drag_selection.mouse
-            and event.modifiers() == self.config.drag_selection.modifier
-        ):
-            renderer.selector.on_drag_selection = True
+        if event.buttons() == self.config.drag_selection.mouse and event.modifiers() == self.config.drag_selection.modifier:
+            self.viewer.renderer.selector.on_drag_selection = True
         # Drag deselection
-        elif (
-            event.buttons() == self.config.drag_deselection.mouse
-            and event.modifiers() == self.config.drag_deselection.modifier
-        ):
-            renderer.selector.on_drag_selection = True
+        elif event.buttons() == self.config.drag_deselection.mouse and event.modifiers() == self.config.drag_deselection.modifier:
+            self.viewer.renderer.selector.on_drag_selection = True
         # Pan
         elif event.buttons() == self.config.pan.mouse and event.modifiers() == self.config.pan.modifier:
-            renderer.camera.pan(dx, dy)
+            self.viewer.renderer.camera.pan(dx, dy)
         # Rotate
         elif event.buttons() == self.config.rotate.mouse and event.modifiers() == self.config.rotate.modifier:
-            renderer.camera.rotate(dx, dy)
+            self.viewer.renderer.camera.rotate(dx, dy)
 
         # Record mouse position
         self.mouse.last_pos = event.pos()
 
-    def mouse_press_action(self, renderer: "Renderer", event: QMouseEvent):
+    def mouse_press_action(self, event: QMouseEvent):
         """
         The mouse press action of the renderer object.
         This function introduces elif for different actions, meaning only one action can be performed at a time.
 
         Parameters
         ----------
         renderer : :class:`compas_viewer.components.renderer.Renderer`
             The renderer object.
         event : :PySide6:`PySide6/QtGui/QMouseEvent`
             The Qt event.
         """
         self.mouse.last_pos = event.pos()
 
         # Drag selection: not in the elif.
-        if (
-            event.buttons() == self.config.drag_selection.mouse
-            and event.modifiers() == self.config.drag_selection.modifier
-        ):
-            renderer.selector.drag_start_pt = event.pos()
+        if event.buttons() == self.config.drag_selection.mouse and event.modifiers() == self.config.drag_selection.modifier:
+            self.viewer.renderer.selector.drag_start_pt = event.pos()
         # Drag deselection
-        elif (
-            event.buttons() == self.config.drag_deselection.mouse
-            and event.modifiers() == self.config.drag_deselection.modifier
-        ):
-            renderer.selector.drag_start_pt = event.pos()
+        elif event.buttons() == self.config.drag_deselection.mouse and event.modifiers() == self.config.drag_deselection.modifier:
+            self.viewer.renderer.selector.drag_start_pt = event.pos()
 
         # Select: single left click.
         if event.buttons() == Qt.MouseButton.LeftButton and event.modifiers() == Qt.KeyboardModifier.NoModifier:
-            renderer.selector.select.emit()
+            self.viewer.renderer.selector.select.emit()
         # Multiselect
-        elif (
-            event.buttons() == self.config.multiselect.mouse and event.modifiers() == self.config.multiselect.modifier
-        ):
-            renderer.selector.multiselect.emit()
+        elif event.buttons() == self.config.multiselect.mouse and event.modifiers() == self.config.multiselect.modifier:
+            self.viewer.renderer.selector.multiselect.emit()
         # Deselect
         elif event.buttons() == self.config.deselect.mouse and event.modifiers() == self.config.deselect.modifier:
-            renderer.selector.deselect.emit()
+            self.viewer.renderer.selector.deselect.emit()
         # Pan
-        elif (
-            event.buttons() == self.config.pan.mouse
-            and event.modifiers() == self.config.pan.modifier
-            and event.modifiers() != self.config.rotate.modifier
-        ):
+        elif event.buttons() == self.config.pan.mouse and event.modifiers() == self.config.pan.modifier and event.modifiers() != self.config.rotate.modifier:
             QApplication.setOverrideCursor(Qt.CursorShape.OpenHandCursor)
         # Rotate
         elif event.buttons() == self.config.rotate.mouse and event.modifiers() == self.config.rotate.modifier:
             QApplication.setOverrideCursor(Qt.CursorShape.SizeAllCursor)
 
-    def mouse_release_action(self, renderer: "Renderer", event: QMouseEvent):
+    def mouse_release_action(self, event: QMouseEvent):
         """
         The mouse release action of the renderer object.
         This function introduces elif for different actions, meaning only one action can be performed at a time.
 
         Parameters
         ----------
         renderer : :class:`compas_viewer.components.renderer.Renderer`
             The renderer object.
         event : :PySide6:`PySide6/QtGui/QMouseEvent`
             The Qt event.
         """
 
         # Drag selection
-        if event.modifiers() == self.config.drag_selection.modifier and renderer.selector.on_drag_selection:
-            renderer.selector.on_drag_selection = False
-            renderer.selector.drag_end_pt = event.pos()
-            renderer.selector.drag_selection.emit()
+        if event.modifiers() == self.config.drag_selection.modifier and self.viewer.renderer.selector.on_drag_selection:
+            self.viewer.renderer.selector.on_drag_selection = False
+            self.viewer.renderer.selector.drag_end_pt = event.pos()
+            self.viewer.renderer.selector.drag_selection.emit()
         # Drag deselection
-        elif event.modifiers() == self.config.drag_deselection.modifier and renderer.selector.on_drag_selection:
-            renderer.selector.on_drag_selection = False
-            renderer.selector.drag_end_pt = event.pos()
-            renderer.selector.drag_deselection.emit()
+        elif event.modifiers() == self.config.drag_deselection.modifier and self.viewer.renderer.selector.on_drag_selection:
+            self.viewer.renderer.selector.on_drag_selection = False
+            self.viewer.renderer.selector.drag_end_pt = event.pos()
+            self.viewer.renderer.selector.drag_deselection.emit()
 
         if event.buttons() == Qt.KeyboardModifier.NoModifier or event.buttons() == Qt.MouseButton.NoButton:
             QApplication.restoreOverrideCursor()
 
-    def pinch_action(self, renderer: "Renderer", event: QPinchGesture):
+    def pinch_action(self, event: QPinchGesture):
         """
         The pinch action of the renderer object.
 
         Parameters
         ----------
         renderer : :class:`compas_viewer.components.renderer.Renderer`
             The renderer object.
         event : :PySide6:`PySide6/QtWidgets/QPinchGesture`
             The Qt event.
 
         """
         steps = event.scaleFactor() - 1
         steps *= 10
-        renderer.camera.zoom(steps)
+        self.viewer.renderer.camera.zoom(steps)
 
-    def wheel_action(self, renderer: "Renderer", event: QWheelEvent):
+    def wheel_action(self, event: QWheelEvent):
         """
         The wheel action of the renderer object.
         It is used from zooming action only.
 
         Parameters
         ----------
         renderer : :class:`compas_viewer.components.renderer.Renderer`
             The renderer object.
         event : :PySide6:`PySide6/QtGui/QWheelEvent`
             The Qt event.
         """
         degrees = event.angleDelta().y() / 8
         steps = degrees / 15
-        renderer.camera.zoom(steps)
+        self.viewer.renderer.camera.zoom(steps)
 
-    def key_press_action(self, renderer: "Renderer", event: QKeyEvent):
+    def key_press_action(self, event: QKeyEvent):
         """
         The key press action of the renderer object.
         This function introduces break for different actions, meaning only one action can be performed at a time.
 
         Parameters
         ----------
         renderer : :class:`compas_viewer.components.renderer.Renderer`
@@ -213,15 +189,15 @@
             The Qt event.
         """
         for action in self.actions.values():
             if event.key() == action.key and event.modifiers() == action.modifier:
                 action.pressed.emit()
                 break
 
-    def key_release_action(self, renderer: "Renderer", event: QKeyEvent):
+    def key_release_action(self, event: QKeyEvent):
         """
         The key release action of the renderer object.
         This function introduces break for different actions, meaning only one action can be performed at a time.
 
         Parameters
         ----------
         renderer : :class:`compas_viewer.components.renderer.Renderer`
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/controller/mouse.py` & `compas_viewer-1.1.3/src/compas_viewer/controller/mouse.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/gl.py` & `compas_viewer-1.1.3/src/compas_viewer/gl.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/icons/compas_icon_white.png` & `compas_viewer-1.1.3/src/compas_viewer/icons/compas_icon_white.png`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/icons/export_file.svg` & `compas_viewer-1.1.3/src/compas_viewer/icons/export_file.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/icons/import_file.svg` & `compas_viewer-1.1.3/src/compas_viewer/icons/import_file.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/icons/selection_info.svg` & `compas_viewer-1.1.3/src/compas_viewer/icons/selection_info.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/icons/view_right.svg` & `compas_viewer-1.1.3/src/compas_viewer/icons/view_right.svg`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/collapsiblebox.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/collapsiblebox.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/layout.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/layout.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/menubar.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/menubar.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/propertyform.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/propertyform.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,25 +312,25 @@
             minimum=0,
             maximum=1,
             step=0.1,
         )
 
         self.map_number(
             obj,
-            "pointssize",
+            "pointsize",
             collapsibleBox.content_area.layout(),  # type: ignore
             "Point Size",
             minimum=1,
             maximum=20,
             step=1,
         )
 
         self.map_number(
             obj,
-            "lineswidth",
+            "linewidth",
             collapsibleBox.content_area.layout(),  # type: ignore
             "Line Width",
             minimum=1,
             maximum=20,
             step=1,
         )
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/sidedock.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/sidedock.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/slider.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/slider.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/statusbar.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/statusbar.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/toolbar.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/toolbar.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/treeform.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/treeform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-from typing import TYPE_CHECKING
 from typing import Callable
 from typing import Optional
 
 from PySide6.QtGui import QColor
 from PySide6.QtWidgets import QTreeWidget
 from PySide6.QtWidgets import QTreeWidgetItem
 
 from compas.datastructures import Tree
 
-if TYPE_CHECKING:
-    from compas_viewer.viewer import Viewer
-
 
 class Treeform(QTreeWidget):
     """
     Class for displaying tree-like data.
     Treeform is an abstract class that could be placed in either the viewport or the sidedock.
 
     Parameters
@@ -61,17 +57,15 @@
 
         viewer = Viewer()
 
         for i in range(10):
             for j in range(10):
                 sp = viewer.scene.add(Sphere(0.1, Frame([i, j, 0], [1, 0, 0], [0, 1, 0])), name=f"Sphere_{i}_{j}")
 
-        viewer.layout.sidedock.add_element(
-            Treeform(viewer._tree, {"Name": (lambda o: o.object.name), "Object": (lambda o: o.object)})
-        )
+        viewer.layout.sidedock.add_element(Treeform(viewer._tree, {"Name": (lambda o: o.object.name), "Object": (lambda o: o.object)}))
 
         viewer.show()
 
     """
 
     def __init__(
         self,
@@ -79,15 +73,14 @@
         columns: dict[str, Callable],
         column_editable: list[bool] = [False],
         show_headers: bool = True,
         stretch: int = 2,
         backgrounds: Optional[dict[str, Callable]] = None,
     ):
         super().__init__()
-        self.viewer: "Viewer"
         self.columns = columns
         self.column_editable = column_editable + [False] * (len(columns) - len(column_editable))
         self.setColumnCount(len(columns))
         self.setHeaderLabels(list(self.columns.keys()))
         self.setHeaderHidden(not show_headers)
         self.stretch = stretch
         self._backgrounds = backgrounds
@@ -114,13 +107,11 @@
                 node.attributes["widget_item"] = QTreeWidgetItem(
                     node.parent.attributes["widget_item"],
                     strings,  # type: ignore
                 )
 
             if self._backgrounds:
                 for col, background in self._backgrounds.items():
-                    node.attributes["widget_item"].setBackground(
-                        list(self.columns.keys()).index(col), QColor(*background(node).rgb255)
-                    )
+                    node.attributes["widget_item"].setBackground(list(self.columns.keys()).index(col), QColor(*background(node).rgb255))
 
     def update(self):
         self.tree = self._tree
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/viewport.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/viewport.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/layout/window.py` & `compas_viewer-1.1.3/src/compas_viewer/layout/window.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/qt.py` & `compas_viewer-1.1.3/src/compas_viewer/qt.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/__init__.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """
 This package provides scene object plugins for visualizing COMPAS objects in `compas_viewer`.
 """
 
-from typing import Union
 from compas.scene import register
 from compas.plugins import plugin
 from compas.datastructures import Mesh
 from compas.datastructures import Graph
 from compas.geometry import (
     Point,
+    Pointcloud,
     Line,
     Vector,
     Circle,
     Box,
     Polyline,
     Torus,
     Polygon,
     Sphere,
     Plane,
     Cylinder,
     Ellipse,
     Cone,
     Capsule,
+    Polyhedron,
     Frame,
     NurbsSurface,
-    Geometry,
 )
 
 from .sceneobject import ViewerSceneObject
 from .meshobject import MeshObject
 from .graphobject import GraphObject
 from .pointobject import PointObject
+from .pointcloudobject import PointcloudObject
 from .lineobject import LineObject
 from .vectorobject import VectorObject
 from .tagobject import TagObject, Tag
 from .frameobject import FrameObject
 from .circleobject import CircleObject
 from .boxobject import BoxObject
 from .torusobject import TorusObject
@@ -42,17 +43,20 @@
 from .polygonobject import PolygonObject
 from .sphereobject import SphereObject
 from .planeobject import PlaneObject
 from .cylinderobject import CylinderObject
 from .ellipseobject import EllipseObject
 from .coneobject import ConeObject
 from .capsuleobject import CapsuleObject
-from .nurbssurfaceobject import NurbsSurfaceObject
-from .collectionobject import CollectionObject
+from .polyhedronobject import PolyhedronObject
 from .geometryobject import GeometryObject
+from .groupobject import Group
+from .groupobject import GroupObject
+from .collectionobject import Collection
+from .collectionobject import CollectionObject
 
 
 @plugin(category="drawing-utils", requires=["compas_viewer"])
 def clear(guids: list[str]):
     for obj in guids:
         del obj
 
@@ -63,14 +67,15 @@
 
 
 @plugin(category="factories", requires=["compas_viewer"])
 def register_scene_objects():
     register(Mesh, MeshObject, context="Viewer")
     register(Graph, GraphObject, context="Viewer")
     register(Point, PointObject, context="Viewer")
+    register(Pointcloud, PointcloudObject, context="Viewer")
     register(Line, LineObject, context="Viewer")
     register(Tag, TagObject, context="Viewer")
     register(Frame, FrameObject, context="Viewer")
     register(Vector, VectorObject, context="Viewer")
     register(Circle, CircleObject, context="Viewer")
     register(Box, BoxObject, context="Viewer")
     register(Polyline, PolylineObject, context="Viewer")
@@ -78,22 +83,29 @@
     register(Polygon, PolygonObject, context="Viewer")
     register(Sphere, SphereObject, context="Viewer")
     register(Plane, PlaneObject, context="Viewer")
     register(Cylinder, CylinderObject, context="Viewer")
     register(Ellipse, EllipseObject, context="Viewer")
     register(Cone, ConeObject, context="Viewer")
     register(Capsule, CapsuleObject, context="Viewer")
-    register(NurbsSurface, NurbsSurfaceObject, context="Viewer")
-    register(list[Union[Geometry, Mesh]], CollectionObject, context="Viewer")
+    register(Polyhedron, PolyhedronObject, context="Viewer")
+    register(list, GroupObject, context="Viewer")
+    register(Collection, CollectionObject, context="Viewer")
 
     try:
         from compas_occ.brep import OCCBrep
         from .brepobject import BRepObject
+        from .nurbssurfaceobject import NurbsSurfaceObject
+        from compas.geometry import NurbsCurve
+        from .nurbscurveobject import NurbsCurveObject
 
         register(OCCBrep, BRepObject, context="Viewer")
+        register(NurbsSurface, NurbsSurfaceObject, context="Viewer")
+        register(NurbsCurve, NurbsCurveObject, context="Viewer")
+
     except ImportError:
         pass
 
 
 __all__ = [
     "ViewerSceneObject",
     "Mesh",
@@ -129,8 +141,12 @@
     "Cone",
     "ConeObject",
     "Capsule",
     "CapsuleObject",
     "NurbsSurface",
     "NurbsSurfaceObject",
     "GeometryObject",
+    "Group",
+    "GroupObject",
+    "Collection",
+    "CollectionObject",
 ]
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/boxobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/boxobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/brepobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/brepobject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 from typing import Optional
 
+from compas_occ.brep import OCCBrep
+
 from compas.datastructures import Mesh
 from compas.geometry import Line
 from compas.geometry import Point
+from compas.itertools import pairwise
 from compas.scene import GeometryObject
 from compas.tolerance import TOL
-from compas.utilities import pairwise
 
 from .geometryobject import GeometryObject as ViewerGeometryObject
 
-try:
-    from compas_occ.brep import OCCBrep
-
-    class BRepObject(ViewerGeometryObject, GeometryObject):
-        """Viewer scene object for displaying COMPAS OCCBrep geometry.
 
-        Attributes
-        ----------
-        brep : :class:`compas_occ.brep.OCCBrep`
-            The compas_occ Brep object.
-        mesh : :class:`compas.datastructures.Mesh`
-            The mesh representation of the Brep.
-
-        See Also
-        --------
-        :class:`compas_occ.brep.Brep`
-        """
-
-        def __init__(self, brep: OCCBrep, **kwargs):
-            super().__init__(geometry=brep, **kwargs)
-            self.geometry: OCCBrep
-            self._viewmesh, self._boundaries = self.geometry.to_tesselation(TOL.lineardeflection)
-
-        @property
-        def points(self) -> Optional[list[Point]]:
-            """The points to be shown in the viewer."""
-            return self.geometry.points
-
-        @property
-        def lines(self) -> Optional[list[Line]]:
-            """The lines to be shown in the viewer."""
-            lines = []
-            for polyline in self._boundaries:
-                for pair in pairwise(polyline.points):
-                    lines.append(Line(*pair))
-
-            return lines
-
-        @property
-        def viewmesh(self) -> Mesh:
-            """The mesh volume to be shown in the viewer."""
-            return self._viewmesh
+class BRepObject(ViewerGeometryObject, GeometryObject):
+    """Viewer scene object for displaying COMPAS OCCBrep geometry.
 
-except ImportError:
-    pass
+    Attributes
+    ----------
+    brep : :class:`compas_occ.brep.OCCBrep`
+        The compas_occ Brep object.
+    mesh : :class:`compas.datastructures.Mesh`
+        The mesh representation of the Brep.
+
+    See Also
+    --------
+    :class:`compas_occ.brep.Brep`
+    """
+
+    def __init__(self, brep: OCCBrep, **kwargs):
+        super().__init__(geometry=brep, **kwargs)
+        self.geometry: OCCBrep
+        self._viewmesh, self._boundaries = self.geometry.to_tesselation(TOL.lineardeflection)
+
+    @property
+    def points(self) -> Optional[list[Point]]:
+        """The points to be shown in the viewer."""
+        return self.geometry.points
+
+    @property
+    def lines(self) -> Optional[list[Line]]:
+        """The lines to be shown in the viewer."""
+        lines = []
+        for polyline in self._boundaries:
+            for pair in pairwise(polyline.points):
+                lines.append(Line(*pair))
+
+        return lines
+
+    @property
+    def viewmesh(self) -> Mesh:
+        """The mesh volume to be shown in the viewer."""
+        return self._viewmesh
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/capsuleobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/capsuleobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/circleobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/circleobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from typing import Optional
 
 from compas.geometry import Circle
 from compas.geometry import Line
 from compas.geometry import Point
+from compas.itertools import pairwise
 from compas.scene import GeometryObject
-from compas.utilities import pairwise
 
 from .geometryobject import GeometryObject as ViewerGeometryObject
 
 
 class CircleObject(ViewerGeometryObject, GeometryObject):
     """Viewer scene object for displaying COMPAS Circle geometry.
 
@@ -39,18 +39,13 @@
     def points(self) -> Optional[list[Point]]:
         """The points to be shown in the viewer."""
         return [self.geometry.center]
 
     @property
     def lines(self) -> Optional[list[Line]]:
         """The lines to be shown in the viewer."""
-        return [
-            Line(*pair)
-            for pair in pairwise(
-                self._calculate_circle_points(self.geometry) + [self._calculate_circle_points(self.geometry)[0]]
-            )
-        ]
+        return [Line(*pair) for pair in pairwise(self._calculate_circle_points(self.geometry) + [self._calculate_circle_points(self.geometry)[0]])]
 
     @property
     def viewmesh(self):
         """The mesh volume to be shown in the viewer."""
         return None
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/collectionobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/collectionobject.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,101 +11,79 @@
 from .sceneobject import ShaderDataType
 from .sceneobject import ViewerSceneObject
 
 
 class Collection(Data):
     """Viewer scene object for displaying a collection of COMPAS geometries."""
 
-    def __init__(self, items: list[Union[Geometry, Mesh]], **kwargs):
+    def __init__(self, items: list[Union[Geometry, Mesh]] = None, **kwargs):
         super().__init__(**kwargs)
         self.items = items
 
     @property
     def __data__(self):
-        return self.items
+        return {"items": self.items}
 
 
 class CollectionObject(ViewerSceneObject, GeometryObject):
     """Viewer scene object for displaying a collection of COMPAS geometries."""
 
-    def __init__(self, items: list[Union[Geometry, Mesh]], **kwargs):
-        self.collection = Collection(items)
+    def __init__(self, collection: Collection, **kwargs):
+        self.collection = collection
         super().__init__(geometry=self.collection, **kwargs)
-        self.objects = [ViewerSceneObject(item=item, **kwargs) for item in self.collection.items]
+        self.objects = [ViewerSceneObject(item, **kwargs) for item in self.collection.items]
 
     def _read_points_data(self) -> ShaderDataType:
         positions = []
         colors = []
         elements = []
         count = 0
         for obj in self.objects:
             p, c, e = obj._read_points_data() or ([], [], [])
             positions += p
             colors += c
             elements += (array(e) + count).tolist()
             count += len(p)
+
         return positions, colors, elements
 
     def _read_lines_data(self) -> ShaderDataType:
         positions = []
         colors = []
         elements = []
         count = 0
         for obj in self.objects:
             p, c, e = obj._read_lines_data() or ([], [], [])
             positions += p
             colors += c
             elements += (array(e) + count).tolist()
             count += len(p)
+
         return positions, colors, elements
 
     def _read_frontfaces_data(self) -> ShaderDataType:
         positions = []
         colors = []
-        opacities = []
         elements = []
         count = 0
         for obj in self.objects:
-            if obj.use_rgba:
-                p, c, o, e = obj._read_frontfaces_data() or ([], [], [])
-                positions += p
-                colors += c
-                opacities += o
-                elements += (np.array(e) + count).tolist()
-                count += len(p)
-            else:
-                p, c, e = obj._read_frontfaces_data() or ([], [], [])
-                positions += p
-                colors += c
-                elements += (np.array(e) + count).tolist()
-                count += len(p)
-
-        if opacities:
-            return positions, colors, opacities, elements
-        else:
-            return positions, colors, elements
+            p, c, e = obj._read_frontfaces_data() or ([], [], [])
+            positions += p
+            colors += c
+            elements += (np.array(e) + count).tolist()
+            count += len(p)
+
+        return positions, colors, elements
 
     def _read_backfaces_data(self) -> ShaderDataType:
         positions = []
         colors = []
-        opacities = []
         elements = []
         count = 0
         for obj in self.objects:
-            if obj.use_rgba:
-                p, c, o, e = obj._read_backfaces_data() or ([], [], [])
-                positions += p
-                colors += c
-                opacities += o
-                elements += (np.array(e) + count).tolist()
-                count += len(p)
-            else:
-                p, c, e = obj._read_backfaces_data() or ([], [], [])
-                positions += p
-                colors += c
-                elements += (np.array(e) + count).tolist()
-                count += len(p)
-
-        if opacities:
-            return positions, colors, opacities, elements
-        else:
-            return positions, colors, elements
+            p, c, e = obj._read_backfaces_data() or ([], [], [])
+            positions += p
+            colors += c
+            elements += (np.array(e) + count).tolist()
+            count += len(p)
+
+        return positions, colors, elements
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/coneobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/coneobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/cylinderobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/cylinderobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/ellipseobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/ellipseobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/frameobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/frameobject.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,20 +52,20 @@
         framesize: Optional[tuple[float, int, float, int]] = None,
         linecolor: Optional[Color] = None,
         show_framez: Optional[bool] = None,
         **kwargs,
     ):
         super().__init__(item=frame, **kwargs)
         self.frame = frame
-        self.linecolor = linecolor or self.viewer.config.linecolor
-        self.dx = framesize[0] if framesize else self.viewer.config.framesize[0]
-        self.nx = framesize[1] if framesize else self.viewer.config.framesize[1]
-        self.dy = framesize[2] if framesize else self.viewer.config.framesize[2]
-        self.ny = framesize[3] if framesize else self.viewer.config.framesize[3]
-        self.show_framez = show_framez or self.viewer.config.show_framez
+        self.linecolor = linecolor if linecolor else Color(0.5, 0.5, 0.5)
+        self.dx = framesize[0] if framesize else float(0.1)
+        self.nx = framesize[1] if framesize else int(10)
+        self.dy = framesize[2] if framesize else float(0.1)
+        self.ny = framesize[3] if framesize else int(10)
+        self.show_framez = show_framez if show_framez else True
         if self.nx % 2 != 0 or self.ny % 2 != 0:
             raise ValueError("The number of grid cells in the X and Y directions must be even numbers.")
         self.show_lines = True
 
     def _read_lines_data(self) -> ShaderDataType:
         trans = Transformation.from_frame_to_frame(Frame.worldXY(), self.frame)
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/geometryobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/geometryobject.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,29 +51,34 @@
     --------
     :class:`compas.geometry.Geometry`
     """
 
     def __init__(
         self,
         geometry: Geometry,
-        u: int,
-        v: int,
-        pointcolor: Optional[Color] = None,
-        linecolor: Optional[Color] = None,
-        surfacecolor: Optional[Color] = None,
+        u: Optional[int] = 16,
+        v: Optional[int] = 16,
+        facecolor: Optional[Color] = None,
         **kwargs,
     ):
         super().__init__(geometry=geometry, **kwargs)
         self.geometry: Geometry
 
         self.u = u
         self.v = v
-        self.pointcolor = pointcolor or self.viewer.config.pointcolor
-        self.linecolor = linecolor or self.viewer.config.linecolor
-        self.surfacecolor = surfacecolor or self.viewer.config.surfacecolor
+        self.facecolor = facecolor or Color(0.9, 0.9, 0.9)
+
+    @property
+    def facecolor(self) -> Color:
+        """The color of the faces."""
+        return self.surfacecolor
+
+    @facecolor.setter
+    def facecolor(self, color: Color) -> None:
+        self.surfacecolor = color
 
     @property
     def points(self) -> Optional[list[Point]]:
         """The points to be shown in the viewer."""
         raise NotImplementedError
 
     @property
@@ -106,18 +111,18 @@
 
         return positions, colors, elements
 
     def _read_frontfaces_data(self) -> ShaderDataType:
         if self.viewmesh is None:
             return [], [], []
         positions, elements = self.viewmesh.to_vertices_and_faces()
-        colors = [self.surfacecolor] * 3 * len(positions)
+        colors = [self.facecolor] * 3 * len(positions)
         return positions, colors, elements  # type: ignore
 
     def _read_backfaces_data(self) -> ShaderDataType:
         if self.viewmesh is None:
             return [], [], []
         positions, elements = self.viewmesh.to_vertices_and_faces()
         for element in elements:
             element.reverse()
-        colors = [self.surfacecolor] * 3 * len(positions)
+        colors = [self.facecolor] * 3 * len(positions)
         return positions, colors, elements  # type: ignore
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/graphobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/graphobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/gridobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/gridobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/lineobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/lineobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/meshobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/meshobject.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Optional
 from typing import Union
 
 from compas.colors import Color
 from compas.datastructures import Mesh
 from compas.geometry import centroid_points
 from compas.geometry import is_coplanar
+from compas.itertools import pairwise
 from compas.scene import MeshObject as BaseMeshObject
-from compas.utilities import pairwise
 
 from .sceneobject import ShaderDataType
 from .sceneobject import ViewerSceneObject
 
 ColorDictValueType = Optional[Union[Dict[Any, Color], Color]]
 
 
@@ -49,52 +49,89 @@
     --------
     :class:`compas.datastructures.Mesh`
     """
 
     def __init__(
         self,
         mesh: Mesh,
-        vertexcolor: Optional[ColorDictValueType] = None,
-        edgecolor: Optional[ColorDictValueType] = None,
-        facecolor: Optional[ColorDictValueType] = None,
+        show_points: Optional[bool] = None,
+        show_lines: Optional[bool] = None,
+        pointcolor: Optional[Color] = None,
+        linecolor: Optional[Color] = None,
+        facecolor: Optional[Color] = None,
+        pointsize: Optional[float] = None,
+        linewidth: Optional[int] = None,
         hide_coplanaredges: Optional[bool] = None,
         use_vertexcolors: Optional[bool] = None,
         **kwargs,
     ):
         super().__init__(mesh=mesh, **kwargs)
 
         self.mesh: Mesh
 
-        self.hide_coplanaredges = (
-            hide_coplanaredges if hide_coplanaredges is not None else self.viewer.config.hide_coplanaredges
-        )
-        self.use_vertexcolors = (
-            use_vertexcolors if use_vertexcolors is not None else self.viewer.config.use_vertexcolors
-        )
-
-        if not vertexcolor:
-            self.vertexcolor = self.viewer.config.pointcolor
-            for vertex in self.mesh.vertices():
-                self.vertexcolor[vertex] = self.mesh.vertex_attribute(vertex, "color")  # type: ignore
-        else:
-            self.vertexcolor = vertexcolor
-
-        if not edgecolor:
-            self.edgecolor = self.viewer.config.linecolor
-            for u, v in self.mesh.edges():
-                self.edgecolor[(u, v)] = self.mesh.edge_attribute((u, v), "color")  # type: ignore
-        else:
-            self.edgecolor = edgecolor
-
-        if not facecolor:
-            self.facecolor = self.viewer.config.surfacecolor
-            for face in self.mesh.faces():
-                self.facecolor[face] = self.mesh.face_attribute(face, "color")  # type: ignore
-        else:
-            self.facecolor = facecolor
+        self.show_points = show_points if show_points is not None else False
+        self.show_lines = show_lines if show_lines is not None else True
+
+        self.pointcolor = pointcolor
+        self.linecolor = linecolor
+        self.facecolor = facecolor or Color(0.9, 0.9, 0.9)
+
+        self.pointsize = pointsize if pointsize is not None else 6.0
+        self.linewidth = linewidth if linewidth is not None else 1.0
+
+        self.hide_coplanaredges = hide_coplanaredges if hide_coplanaredges is not None else False
+        self.use_vertexcolors = use_vertexcolors if use_vertexcolors is not None else False
+
+    @property
+    def pointcolor(self) -> Color:
+        return self.vertexcolor
+
+    @pointcolor.setter
+    def pointcolor(self, color: Color):
+        self.vertexcolor = color
+
+    @property
+    def linecolor(self) -> Color:
+        return self.edgecolor
+
+    @linecolor.setter
+    def linecolor(self, color: Color):
+        self.edgecolor = color
+
+    @property
+    def show_points(self) -> bool:
+        return self.show_vertices
+
+    @show_points.setter
+    def show_points(self, show: bool):
+        self.show_vertices = show
+
+    @property
+    def show_lines(self) -> bool:
+        return self.show_edges
+
+    @show_lines.setter
+    def show_lines(self, show: bool):
+        self.show_edges = show
+
+    @property
+    def pointsize(self) -> float:
+        return self.vertexsize
+
+    @pointsize.setter
+    def pointsize(self, size: float):
+        self.vertexsize = size
+
+    @property
+    def linewidth(self) -> float:
+        return self.edgesize
+
+    @linewidth.setter
+    def linewidth(self, size: float):
+        self.edgesize = size
 
     def _read_points_data(self) -> ShaderDataType:
         positions = []
         colors = []
         elements = []
         i = 0
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/planeobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/planeobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/pointobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/pointobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/polygonobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/polylineobject.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from typing import Optional
 
 from compas.geometry import Line
 from compas.geometry import Point
-from compas.geometry import Polygon
+from compas.geometry import Polyline
 from compas.scene import GeometryObject
 
 from .geometryobject import GeometryObject as ViewerGeometryObject
 
 
-class PolygonObject(ViewerGeometryObject, GeometryObject):
-    """Viewer scene object for displaying COMPAS Polygon geometry.
+class PolylineObject(ViewerGeometryObject, GeometryObject):
+    """Viewer scene object for displaying COMPAS Polyline geometry.
 
     See Also
     --------
-    :class:`compas.geometry.Polygon`
+    :class:`compas.geometry.Polyline`
     """
 
-    def __init__(self, polygon: Polygon, **kwargs):
-        super().__init__(geometry=polygon, **kwargs)
-        self.geometry: Polygon
+    def __init__(self, polyline: Polyline, **kwargs):
+        super().__init__(geometry=polyline, **kwargs)
+        self.geometry: Polyline
         self.show_lines = True
 
     @property
     def points(self) -> Optional[list[Point]]:
         """The points to be shown in the viewer."""
         return self.geometry.points
 
     @property
     def lines(self) -> Optional[list[Line]]:
+        """The lines to be shown in the viewer."""
         return self.geometry.lines
 
     @property
     def viewmesh(self):
         """The mesh volume to be shown in the viewer."""
         return None
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/polylineobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/polygonobject.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from typing import Optional
 
+from compas.datastructures import Mesh
 from compas.geometry import Line
 from compas.geometry import Point
-from compas.geometry import Polyline
+from compas.geometry import Polygon
+from compas.geometry import earclip_polygon
 from compas.scene import GeometryObject
 
 from .geometryobject import GeometryObject as ViewerGeometryObject
 
 
-class PolylineObject(ViewerGeometryObject, GeometryObject):
-    """Viewer scene object for displaying COMPAS Polyline geometry.
+class PolygonObject(ViewerGeometryObject, GeometryObject):
+    """Viewer scene object for displaying COMPAS Polygon geometry.
 
     See Also
     --------
-    :class:`compas.geometry.Polyline`
+    :class:`compas.geometry.Polygon`
     """
 
-    def __init__(self, polyline: Polyline, **kwargs):
-        super().__init__(geometry=polyline, **kwargs)
-        self.geometry: Polyline
-        self.show_lines = True
+    def __init__(self, polygon: Polygon, **kwargs):
+        super().__init__(geometry=polygon, **kwargs)
+        self.geometry: Polygon
 
     @property
     def points(self) -> Optional[list[Point]]:
         """The points to be shown in the viewer."""
         return self.geometry.points
 
     @property
     def lines(self) -> Optional[list[Line]]:
-        """The lines to be shown in the viewer."""
         return self.geometry.lines
 
     @property
     def viewmesh(self):
         """The mesh volume to be shown in the viewer."""
-        return None
+        vertices = self.geometry.points
+        faces = earclip_polygon(self.geometry)
+        return Mesh.from_vertices_and_faces(vertices, faces)
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/scene.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/scene.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from random import randint
 from random import seed
-from typing import TYPE_CHECKING
 from typing import Any
 from typing import Generator
 from typing import Optional
 from typing import Union
 
 from compas.colors import Color
 from compas.datastructures import Datastructure
 from compas.geometry import Geometry
 from compas.scene import Scene
 
 from .sceneobject import ViewerSceneObject
 
-if TYPE_CHECKING:
-    from compas_viewer import Viewer
-
 
 def instance_colors_generator(i: int = 0) -> Generator:
     """
     Generate a set of non-repetitive random colors for instance colors.
 
     Parameters
     ----------
@@ -65,17 +61,16 @@
         The context of the scene.
 
     See Also
     --------
     :class:`compas.scene.Scene`
     """
 
-    def __init__(self, viewer: "Viewer", name: str, context: str):
-        super(ViewerScene, self).__init__(name=name, context=context)
-        self.viewer = viewer
+    def __init__(self, name: str = "ViewerScene", context: str = "Viewer"):
+        super().__init__(name=name, context=context)
 
         #  Primitive
         self.objects: list[ViewerSceneObject]
 
         #  Selection
         self.instance_colors: dict[tuple[int, int, int], ViewerSceneObject] = {}
         self._instance_colors_generator = instance_colors_generator()
@@ -88,20 +83,19 @@
         is_locked: bool = False,
         is_visible: bool = True,
         show_points: Optional[bool] = None,
         show_lines: Optional[bool] = None,
         show_faces: Optional[bool] = None,
         pointcolor: Optional[Color] = None,
         linecolor: Optional[Color] = None,
-        surfacecolor: Optional[Color] = None,
         vertexcolor: Optional[Union[Color, dict[Any, Color]]] = None,
         edgecolor: Optional[Union[Color, dict[Any, Color]]] = None,
         facecolor: Optional[Union[Color, dict[Any, Color]]] = None,
-        lineswidth: Optional[float] = None,
-        pointssize: Optional[float] = None,
+        linewidth: Optional[float] = None,
+        pointsize: Optional[float] = None,
         opacity: Optional[float] = None,
         hide_coplanaredges: Optional[bool] = None,
         use_vertexcolors: Optional[bool] = None,
         v: int = 16,
         u: int = 16,
         **kwargs,
     ) -> ViewerSceneObject:
@@ -131,25 +125,23 @@
             Whether to show lines/edges of the object.
         show_faces : bool, optional
             Whether to show faces of the object.
         pointcolor : :class:`compas.colors.Color`, optional
             The single color of colors of the points in the COMPAS Geometry.
         linecolor : :class:`compas.colors.Color`, optional
             The single color of colors of the lines in the COMPAS Geometry.
-        surfacecolor : :class:`compas.colors.Color`, optional
-            The single color of colors the surfaces in the COMPAS Geometry.
         vertexcolor : Union[:class:`compas.colors.Color`, dict[Any, :class:`compas.colors.Color`], optional
             The color or the dict of colors of the vertices in the COMPAS Mesh.
         edgecolor : Union[:class:`compas.colors.Color`, dict[Any, :class:`compas.colors.Color`], optional
             The color or the dict of colors of the edges in the COMPAS Mesh.
         facecolor : Union[:class:`compas.colors.Color`, dict[Any, :class:`compas.colors.Color`], optional
             The color or the dict of colors of the faces in the COMPAS Mesh.
-        lineswidth : float, optional
+        linewidth : float, optional
             The line width to be drawn on screen
-        pointssize : float, optional
+        pointsize : float, optional
             The point size to be drawn on screen
         opacity : float, optional
             The opacity of the object.
         hide_coplanaredges : bool, optional
             Whether to hide the coplanar edges of the mesh.
         use_vertexcolors : bool, optional
             Whether to use vertex color.
@@ -165,29 +157,27 @@
         :class:`compas_viewer.scene.ViewerSceneObject`
             The scene object.
         """
 
         sceneobject: ViewerSceneObject = super().add(  # type: ignore
             item=item,
             parent=parent,
-            viewer=self.viewer,
             is_selected=is_selected,
             is_visible=is_visible,
             is_locked=is_locked,
             show_points=show_points,
             show_lines=show_lines,
             show_faces=show_faces,
             pointcolor=pointcolor,
             linecolor=linecolor,
             facecolor=facecolor,
-            surfacecolor=surfacecolor,
             vertexcolor=vertexcolor,
             edgecolor=edgecolor,
-            lineswidth=lineswidth,
-            pointssize=pointssize,
+            linewidth=linewidth,
+            pointsize=pointsize,
             opacity=opacity,
             hide_coplanaredges=hide_coplanaredges,
             use_vertexcolors=use_vertexcolors,
             v=v,
             u=u,
             **kwargs,
         )
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/sceneobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/sceneobject.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-from typing import TYPE_CHECKING
 from typing import Any
 from typing import Optional
 
 from numpy import array
 from numpy import average
 from numpy import identity
 
 from compas.colors import Color
 from compas.geometry import Point
 from compas.geometry import Transformation
 from compas.geometry import transform_points_numpy
+from compas.itertools import flatten
 from compas.scene import SceneObject
-from compas.utilities import flatten
+from compas_viewer.base import Base
 from compas_viewer.components.renderer.shaders import Shader
 from compas_viewer.gl import make_index_buffer
 from compas_viewer.gl import make_vertex_buffer
 from compas_viewer.gl import update_index_buffer
 from compas_viewer.gl import update_vertex_buffer
 
-if TYPE_CHECKING:
-    from compas_viewer import Viewer
-
-
 # Type template of point/line/face data for generating the buffers.
 ShaderDataType = tuple[list[Point], list[Color], list[list[int]]]
 
 
-class ViewerSceneObject(SceneObject):
+class ViewerSceneObject(SceneObject, Base):
     """
     Base class for all Viewer scene objects
     which also includes the  GL buffer creation and drawing methods.
 
     Parameters
     ----------
     viewer : :class:`compas_viewer.viewer.Viewer`
@@ -43,18 +39,18 @@
         Whether to show object. Default is True.
     show_points : bool, optional
         Whether to show points/vertices of the object. Default is the value of `show_points` in `viewer.config`.
     show_lines : bool, optional
         Whether to show lines/edges of the object. Default is the value of `show_lines` in `viewer.config`.
     show_faces : bool, optional
         Whether to show faces of the object. Default is the value of `show_faces` in `viewer.config`.
-    lineswidth : float, optional
-        The line width to be drawn on screen. Default is the value of `lineswidth` in `viewer.config`.
-    pointssize : float, optional
-        The point size to be drawn on screen. Default is the value of `pointssize` in `viewer.config`.
+    linewidth : float, optional
+        The line width to be drawn on screen. Default is the value of `linewidth` in `viewer.config`.
+    pointsize : float, optional
+        The point size to be drawn on screen. Default is the value of `pointsize` in `viewer.config`.
     opacity : float, optional
         The opacity of the object. Default is the value of `opacity` in `viewer.config`.
     **kwargs : dict, optional
         Additional visualization options for :class:`compas.scene.SceneObject`.
 
     Attributes
     ----------
@@ -67,17 +63,17 @@
         Whether to show object.
     show_points : bool
         Whether to show points/vertices of the object.
     show_lines : bool
         Whether to show lines/edges of the object.
     show_faces : bool
         Whether to show faces of the object.
-    lineswidth : float
+    linewidth : float
         The line width to be drawn on screen
-    pointssize : float
+    pointsize : float
         The point size to be drawn on screen.
     opacity : float
         The opacity of the object.
     background : bool
         Whether the object is drawn on the background with depth test disabled.
     bounding_box : list[float], read-only
         The min and max corners of object bounding box, as a numpy array of shape (2, 3).
@@ -87,57 +83,53 @@
     See Also
     --------
     :class:`compas.scene.SceneObject`
     """
 
     def __init__(
         self,
-        viewer: "Viewer",
         is_selected: bool = False,
         is_locked: bool = False,
         is_visible: bool = True,
         show_points: Optional[bool] = None,
         show_lines: Optional[bool] = None,
         show_faces: Optional[bool] = None,
-        lineswidth: Optional[float] = None,
-        pointssize: Optional[float] = None,
+        linewidth: Optional[float] = None,
+        pointsize: Optional[float] = None,
         opacity: Optional[float] = None,
         use_rgba: bool = False,
         **kwargs,
     ):
         #  Basic
         super().__init__(**kwargs)
-        self.viewer = viewer
-        self.scene = viewer.scene
-        self.renderer = viewer.renderer
         self.is_visible = is_visible
-        self.show_points = self.viewer.config.show_points if show_points is None else show_points
-        self.show_lines = self.viewer.config.show_lines if show_lines is None else show_lines
-        self.show_faces = self.viewer.config.show_faces if show_faces is None else show_faces
-        self.lineswidth = lineswidth or self.viewer.config.lineswidth
-        self.pointssize = pointssize or self.viewer.config.pointssize
-        self.opacity = opacity or self.viewer.config.opacity
+        self.show_points = show_points if show_points is not None else False
+        self.show_lines = show_lines if show_lines is not None else True
+        self.show_faces = show_faces if show_faces is not None else True
+        self.linewidth = linewidth if linewidth is not None else self.viewer.config.ui.display.linewidth
+        self.pointsize = pointsize if pointsize is not None else self.viewer.config.ui.display.pointsize
+        self.opacity = opacity if opacity is not None else self.viewer.config.ui.display.opacity
 
         #  Selection
         self._is_locked = is_locked
         self.is_selected = not is_locked and is_selected
-        self.instance_color = Color.from_rgb255(*next(self.scene._instance_colors_generator))
+        # TODO scene
+        self.instance_color = Color.from_rgb255(*next(self.viewer.scene._instance_colors_generator))
         if not is_locked:
-            self.scene.instance_colors[self.instance_color.rgb255] = self
+            self.viewer.scene.instance_colors[self.instance_color.rgb255] = self
 
         #  Visual
         self.background: bool = False
         self.use_rgba = use_rgba
 
         #  Geometric
         self.transformation: Optional[Transformation] = None
         self._matrix_buffer: Optional[list[list[float]]] = None
         self._bounding_box: Optional[list[float]] = None
         self._bounding_box_center: Optional[Point] = None
-        self._is_collection = False
 
         #  Primitive
         self._points_data: Optional[ShaderDataType] = None
         self._lines_data: Optional[ShaderDataType] = None
         self._frontfaces_data: Optional[ShaderDataType] = None
         self._backfaces_data: Optional[ShaderDataType] = None
         self._points_buffer: [dict[str, Any]] = None  # type: ignore
@@ -150,14 +142,15 @@
         return self._is_locked
 
     @is_locked.setter
     def is_locked(self, value: bool):
         self._is_locked = value
         if value:
             self.is_selected = False
+            # scene parent
             self.scene.instance_colors.pop(self.instance_color.rgb255)
         else:
             self.scene.instance_colors[self.instance_color.rgb255] = self
 
     @property
     def bounding_box(self):
         return self._bounding_box
@@ -343,15 +336,15 @@
                 self._backfaces_buffer,
                 update_positions,
                 update_colors,
                 update_elements,
             )
 
         #  Update the canvas.
-        self.renderer.update()
+        self.viewer.renderer.update()
 
     def _update_bounding_box(self, positions: Optional[list[Point]] = None):
         """Update the bounding box of the object"""
         if positions is None:
             positions = []
             if self._points_data is not None:
                 positions += self._points_data[0]
@@ -359,17 +352,15 @@
                 positions += self._lines_data[0]
             if self._frontfaces_data is not None:
                 positions += self._frontfaces_data[0]
             if not positions:
                 return
 
         _positions = array(positions)
-        self._bounding_box = list(
-            transform_points_numpy(array([_positions.min(axis=0), _positions.max(axis=0)]), self.worldtransformation)
-        )
+        self._bounding_box = list(transform_points_numpy(array([_positions.min(axis=0), _positions.max(axis=0)]), self.worldtransformation))
         self._bounding_box_center = Point(*list(average(a=array(self.bounding_box), axis=0)))
 
     def draw(self, shader: Shader, wireframe: bool, is_lighted: bool):
         """Draw the object from its buffers"""
         shader.enable_attribute("position")
         shader.enable_attribute("color")
         shader.uniform1i("is_selected", self.is_selected)
@@ -388,36 +379,34 @@
                 n=self._frontfaces_buffer["n"],
                 background=self.background,
             )
         # Backfaces
         if self._backfaces_buffer is not None and not wireframe and self.show_faces:
             shader.bind_attribute("position", self._backfaces_buffer["positions"])
             shader.bind_attribute("color", self._backfaces_buffer["colors"], step=4)
-            shader.draw_triangles(
-                elements=self._backfaces_buffer["elements"], n=self._backfaces_buffer["n"], background=self.background
-            )
+            shader.draw_triangles(elements=self._backfaces_buffer["elements"], n=self._backfaces_buffer["n"], background=self.background)
         shader.uniform1i("is_lighted", False)
         shader.uniform1i("element_type", 1)
         # Lines
         if self._lines_buffer is not None and self.show_lines:
             shader.bind_attribute("position", self._lines_buffer["positions"])
             shader.bind_attribute("color", self._lines_buffer["colors"], step=4)
             shader.draw_lines(
-                width=self.lineswidth,
+                width=self.linewidth,
                 elements=self._lines_buffer["elements"],
                 n=self._lines_buffer["n"],
                 background=self.background,
             )
         shader.uniform1i("element_type", 0)
         # Points
         if self._points_buffer is not None and self.show_points:
             shader.bind_attribute("position", self._points_buffer["positions"])
             shader.bind_attribute("color", self._points_buffer["colors"], step=4)
             shader.draw_points(
-                size=self.pointssize,
+                size=self.pointsize,
                 elements=self._points_buffer["elements"],
                 n=self._points_buffer["n"],
                 background=self.background,
             )
         # Reset
         shader.uniform1i("is_selected", 0)
         shader.uniform1f("object_opacity", 1)
@@ -432,22 +421,20 @@
         shader.uniform3f("instance_color", self.instance_color.rgb)
         # Matrix
         if self._matrix_buffer is not None:
             shader.uniform4x4("transform", self._matrix_buffer)
         # Points
         if self._points_buffer is not None and self.show_points:
             shader.bind_attribute("position", self._points_buffer["positions"])
-            shader.draw_points(
-                size=self.pointssize, elements=self._points_buffer["elements"], n=self._points_buffer["n"]
-            )
+            shader.draw_points(size=self.pointsize, elements=self._points_buffer["elements"], n=self._points_buffer["n"])
         # Lines
         if self._lines_buffer is not None and (self.show_lines or wireframe):
             shader.bind_attribute("position", self._lines_buffer["positions"])
             shader.draw_lines(
-                width=self.lineswidth + self.renderer.selector.PIXEL_SELECTION_INCREMENTAL,
+                width=self.linewidth + self.viewer.renderer.selector.PIXEL_SELECTION_INCREMENTAL,
                 elements=self._lines_buffer["elements"],
                 n=self._lines_buffer["n"],
             )
         # Frontfaces
         if self._frontfaces_buffer is not None and not wireframe and self.show_faces:
             shader.bind_attribute("position", self._frontfaces_buffer["positions"])
             shader.draw_triangles(elements=self._frontfaces_buffer["elements"], n=self._frontfaces_buffer["n"])
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/sphereobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/sphereobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/tagobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/tagobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,23 +198,15 @@
             GL.GL_UNSIGNED_BYTE,
             string_buffer,
         )
         return texture
 
     def _calculate_text_height(self, camera_position):
         if self.geometry.absolute_height:
-            return int(
-                (10 * self.geometry.height)
-                / float(
-                    linalg.norm(
-                        array(self.geometry.position)
-                        - array([camera_position.x, camera_position.y, camera_position.z])
-                    )
-                )
-            )
+            return int((10 * self.geometry.height) / float(linalg.norm(array(self.geometry.position) - array([camera_position.x, camera_position.y, camera_position.z]))))
 
         else:
             return self.geometry.height
 
     def draw(self, shader, camera_position):
         """Draw the object from its buffers"""
         shader.enable_attribute("position")
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/torusobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/torusobject.py`

 * *Files identical despite different names*

### Comparing `compas_viewer-1.1.2/src/compas_viewer/scene/vectorobject.py` & `compas_viewer-1.1.3/src/compas_viewer/scene/vectorobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         Default is the origin point.
     **kwargs : dict, optional
         Additional options for the :class:`compas_viewer.scene.ViewerSceneObject`.
 
     Notes
     -----
     The frame object is always unselectable.
-    Apart from the :attr:`compas_viewer.scene.vectorobject.VectorObject.config.lineswidth`
+    Apart from the :attr:`compas_viewer.scene.vectorobject.VectorObject.config.linewidth`
     that controls the width of the vector,
     the :attr:`compas_viewer.scene.vectorobject.VectorObject.config.vectorsize`
     (float 0-1) controls the size of the arrow.
 
     See Also
     --------
     :class:`compas.geometry.Vector`
@@ -71,13 +71,11 @@
 
         if self.worldtransformation is not None:
             shader.uniform4x4("transform", self.worldtransformation.matrix)
         shader.enable_attribute("position")
         shader.enable_attribute("color")
         shader.bind_attribute("position", self._lines_buffer["positions"])
         shader.bind_attribute("color", self._lines_buffer["colors"], step=4)
-        shader.draw_arrows(
-            elements=self._lines_buffer["elements"], n=self._lines_buffer["n"], width=self.lineswidth, background=True
-        )
+        shader.draw_arrows(elements=self._lines_buffer["elements"], n=self._lines_buffer["n"], width=self.linewidth, background=True)
         shader.draw_triangles(elements=self.arrow_buffer["elements"], n=self.arrow_buffer["n"], background=True)
         shader.disable_attribute("position")
         shader.disable_attribute("color")
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer.egg-info/PKG-INFO` & `compas_viewer-1.1.3/src/compas_viewer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_viewer
-Version: 1.1.2
+Version: 1.1.3
 Summary: Standalone viewer for COMPAS 2 based on PyOpenGL and PyQt6.
 Author-email: tom van mele <tom.v.mele@gmail.com>, Li Chen <li.chen@arch.ethz.ch>, Zac Zhuo Zhang <zhuo.zhang@arch.ethz.ch>
 License: MIT License
         
         COMPAS Association
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -39,15 +39,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: compas>=2.0.0
 Requires-Dist: freetype-py
 Requires-Dist: PyOpenGL
-Requires-Dist: PyOpenGL_accelerate
 Requires-Dist: PySide6==6.6.1
 Provides-Extra: dev
 Requires-Dist: attrs>=17.4; extra == "dev"
 Requires-Dist: black>=22.12.0; extra == "dev"
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: compas_invocations2; extra == "dev"
 Requires-Dist: compas_notebook; extra == "dev"
```

### Comparing `compas_viewer-1.1.2/src/compas_viewer.egg-info/SOURCES.txt` & `compas_viewer-1.1.3/src/compas_viewer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 src/compas_viewer/__init__.py
 src/compas_viewer/__main__.py
+src/compas_viewer/base.py
 src/compas_viewer/config.json
 src/compas_viewer/config.py
 src/compas_viewer/gl.py
 src/compas_viewer/qt.py
+src/compas_viewer/singleton.py
 src/compas_viewer/viewer.py
 src/compas_viewer.egg-info/PKG-INFO
 src/compas_viewer.egg-info/SOURCES.txt
 src/compas_viewer.egg-info/dependency_links.txt
 src/compas_viewer.egg-info/not-zip-safe
 src/compas_viewer.egg-info/requires.txt
 src/compas_viewer.egg-info/top_level.txt
@@ -21,14 +23,19 @@
 src/compas_viewer/actions/delete_selected.py
 src/compas_viewer/actions/info.py
 src/compas_viewer/actions/io.py
 src/compas_viewer/actions/select_all.py
 src/compas_viewer/actions/viewmode.py
 src/compas_viewer/actions/zoom_selected.py
 src/compas_viewer/components/__init__.py
+src/compas_viewer/components/button_factory.py
+src/compas_viewer/components/component_manager.py
+src/compas_viewer/components/setting_components.py
+src/compas_viewer/components/treeform_components.py
+src/compas_viewer/components/widget_tools.py
 src/compas_viewer/components/renderer/__init__.py
 src/compas_viewer/components/renderer/camera.py
 src/compas_viewer/components/renderer/renderer.py
 src/compas_viewer/components/renderer/selector.py
 src/compas_viewer/components/renderer/shaders/__init__.py
 src/compas_viewer/components/renderer/shaders/arrow.frag
 src/compas_viewer/components/renderer/shaders/arrow.vert
@@ -43,14 +50,15 @@
 src/compas_viewer/components/renderer/shaders/tag.vert
 src/compas_viewer/configurations/__init__.py
 src/compas_viewer/configurations/config.py
 src/compas_viewer/configurations/controller_config.py
 src/compas_viewer/configurations/layout_config.py
 src/compas_viewer/configurations/renderer_config.py
 src/compas_viewer/configurations/viewer_config.py
+src/compas_viewer/configurations/default_config/FreeSans.ttf
 src/compas_viewer/configurations/default_config/controller.json
 src/compas_viewer/configurations/default_config/layout.json
 src/compas_viewer/configurations/default_config/renderer.json
 src/compas_viewer/configurations/default_config/viewer.json
 src/compas_viewer/controller/__init__.py
 src/compas_viewer/controller/controller.py
 src/compas_viewer/controller/mouse.py
@@ -87,22 +95,33 @@
 src/compas_viewer/scene/coneobject.py
 src/compas_viewer/scene/cylinderobject.py
 src/compas_viewer/scene/ellipseobject.py
 src/compas_viewer/scene/frameobject.py
 src/compas_viewer/scene/geometryobject.py
 src/compas_viewer/scene/graphobject.py
 src/compas_viewer/scene/gridobject.py
+src/compas_viewer/scene/groupobject.py
 src/compas_viewer/scene/lineobject.py
 src/compas_viewer/scene/meshobject.py
+src/compas_viewer/scene/nurbscurveobject.py
 src/compas_viewer/scene/nurbssurfaceobject.py
 src/compas_viewer/scene/planeobject.py
+src/compas_viewer/scene/pointcloudobject.py
 src/compas_viewer/scene/pointobject.py
 src/compas_viewer/scene/polygonobject.py
+src/compas_viewer/scene/polyhedronobject.py
 src/compas_viewer/scene/polylineobject.py
 src/compas_viewer/scene/scene.py
 src/compas_viewer/scene/sceneobject.py
 src/compas_viewer/scene/sphereobject.py
 src/compas_viewer/scene/tagobject.py
 src/compas_viewer/scene/torusobject.py
 src/compas_viewer/scene/vectorobject.py
+src/compas_viewer/ui/__init__.py
+src/compas_viewer/ui/mainwindow.py
+src/compas_viewer/ui/menubar.py
+src/compas_viewer/ui/statusbar.py
+src/compas_viewer/ui/toolbar.py
+src/compas_viewer/ui/ui.py
+src/compas_viewer/ui/viewport.py
 tests/test_placeholder.py
 tests/test_viewer.py
```

