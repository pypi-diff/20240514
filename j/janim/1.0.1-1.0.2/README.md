# Comparing `tmp/janim-1.0.1.tar.gz` & `tmp/janim-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-1.0.1.tar` & `janim-1.0.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0      165 2024-04-29 03:02:09.985896 janim-1.0.1/.gitignore
--rw-r--r--   0        0        0     1053 2024-04-17 15:49:03.633620 janim-1.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0      413 2024-04-28 10:20:10.624911 janim-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0      403 2023-10-12 06:08:14.650702 janim-1.0.1/.vscode/tasks.json
--rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.1/LICENSE
--rw-r--r--   0        0        0      966 2024-03-08 14:50:49.538193 janim-1.0.1/README.md
--rw-r--r--   0        0        0       71 2024-05-11 04:51:04.527148 janim-1.0.1/janim/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-17 03:59:08.847168 janim-1.0.1/janim/__main__.py
--rw-r--r--   0        0        0     4099 2024-05-10 15:16:50.978563 janim-1.0.1/janim/anims/animation.py
--rw-r--r--   0        0        0     6349 2024-05-10 15:15:49.989394 janim-1.0.1/janim/anims/composition.py
--rw-r--r--   0        0        0     5861 2024-04-29 03:02:09.993849 janim-1.0.1/janim/anims/creation.py
--rw-r--r--   0        0        0      721 2024-04-29 03:02:09.993849 janim-1.0.1/janim/anims/display.py
--rw-r--r--   0        0        0     3246 2024-04-29 03:02:09.993849 janim-1.0.1/janim/anims/fading.py
--rw-r--r--   0        0        0     3458 2024-05-10 01:15:31.092973 janim-1.0.1/janim/anims/growing.py
--rw-r--r--   0        0        0     9094 2024-05-11 01:59:04.880227 janim-1.0.1/janim/anims/indication.py
--rw-r--r--   0        0        0     1525 2024-05-11 01:34:20.294913 janim-1.0.1/janim/anims/rotation.py
--rw-r--r--   0        0        0    24756 2024-05-11 02:53:28.238786 janim-1.0.1/janim/anims/timeline.py
--rw-r--r--   0        0        0     8894 2024-04-29 03:02:10.001840 janim-1.0.1/janim/anims/transform.py
--rw-r--r--   0        0        0     9918 2024-05-10 15:49:08.746418 janim-1.0.1/janim/anims/updater.py
--rw-r--r--   0        0        0     4505 2024-04-29 03:02:10.001840 janim-1.0.1/janim/camera/camera.py
--rw-r--r--   0        0        0     2744 2024-03-05 11:28:56.434384 janim-1.0.1/janim/camera/camera_info.py
--rw-r--r--   0        0        0     6808 2024-04-28 10:19:08.668987 janim-1.0.1/janim/cli.py
--rw-r--r--   0        0        0     9221 2024-05-09 02:33:32.575199 janim-1.0.1/janim/components/component.py
--rw-r--r--   0        0        0     2408 2024-04-29 03:02:10.001840 janim-1.0.1/janim/components/data.py
--rw-r--r--   0        0        0     2609 2024-05-10 14:02:00.852109 janim-1.0.1/janim/components/depth.py
--rw-r--r--   0        0        0     1284 2024-04-29 03:02:10.001840 janim-1.0.1/janim/components/image.py
--rw-r--r--   0        0        0    30900 2024-05-10 09:03:24.673167 janim-1.0.1/janim/components/points.py
--rw-r--r--   0        0        0     2833 2024-04-29 04:16:18.595714 janim-1.0.1/janim/components/radius.py
--rw-r--r--   0        0        0     7922 2024-05-10 15:58:49.637620 janim-1.0.1/janim/components/rgbas.py
--rw-r--r--   0        0        0    22599 2024-05-10 01:20:31.753161 janim-1.0.1/janim/components/vpoints.py
--rw-r--r--   0        0        0      245 2024-05-09 02:35:19.291617 janim-1.0.1/janim/constants/__init__.py
--rw-r--r--   0        0        0      169 2024-01-12 15:55:35.365552 janim-1.0.1/janim/constants/alignment.py
--rw-r--r--   0        0        0     1333 2024-02-20 13:10:29.970716 janim-1.0.1/janim/constants/colors.py
--rw-r--r--   0        0        0      483 2024-03-05 11:28:56.458376 janim-1.0.1/janim/constants/coord.py
--rw-r--r--   0        0        0      179 2024-01-12 15:55:05.570414 janim-1.0.1/janim/constants/degrees.py
--rw-r--r--   0        0        0     4783 2024-04-29 03:02:10.009835 janim-1.0.1/janim/examples.py
--rw-r--r--   0        0        0     1723 2024-04-29 03:02:10.009835 janim-1.0.1/janim/exception.py
--rw-r--r--   0        0        0    40949 2024-05-09 06:44:12.976369 janim-1.0.1/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      330 2024-02-20 13:10:29.974744 janim-1.0.1/janim/gui/application.py
--rw-r--r--   0        0        0      797 2024-04-17 03:59:08.853145 janim-1.0.1/janim/gui/audio_player.py
--rw-r--r--   0        0        0     3181 2024-02-20 13:10:29.978729 janim-1.0.1/janim/gui/export.png
--rw-r--r--   0        0        0     1258 2024-02-20 13:10:29.978729 janim-1.0.1/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0      996 2024-05-11 04:50:05.051446 janim-1.0.1/janim/gui/glwidget.py
--rw-r--r--   0        0        0      903 2024-04-24 02:36:54.042754 janim-1.0.1/janim/gui/precise_timer.py
--rw-r--r--   0        0        0     5278 2024-03-26 14:54:35.926619 janim-1.0.1/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     8331 2024-04-29 03:02:10.017837 janim-1.0.1/janim/gui/selector.py
--rw-r--r--   0        0        0     1679 2024-05-10 01:25:26.525873 janim-1.0.1/janim/imports.py
--rw-r--r--   0        0        0     5727 2024-05-11 02:59:56.767613 janim-1.0.1/janim/items/audio.py
--rw-r--r--   0        0        0     4862 2024-03-08 02:47:13.255043 janim-1.0.1/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8745 2024-05-10 13:55:21.394170 janim-1.0.1/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2165 2024-05-09 02:35:32.318443 janim-1.0.1/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8330 2024-03-26 14:54:35.942576 janim-1.0.1/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8784 2024-04-28 10:29:47.798293 janim-1.0.1/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6729 2024-05-11 01:59:17.314024 janim-1.0.1/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     7917 2024-04-29 03:02:10.017837 janim-1.0.1/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5239 2024-05-10 14:00:42.241727 janim-1.0.1/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5277 2024-05-10 09:01:57.035941 janim-1.0.1/janim/items/image_item.py
--rw-r--r--   0        0        0    18848 2024-05-11 01:35:54.138307 janim-1.0.1/janim/items/item.py
--rw-r--r--   0        0        0     3262 2024-05-06 03:29:21.974646 janim-1.0.1/janim/items/points.py
--rw-r--r--   0        0        0     7660 2024-05-06 05:14:45.063804 janim-1.0.1/janim/items/relation.py
--rw-r--r--   0        0        0     2071 2024-04-28 10:20:10.634879 janim-1.0.1/janim/items/shape_matchers.py
--rw-r--r--   0        0        0     5955 2024-04-29 03:38:28.528237 janim-1.0.1/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1736 2024-03-14 06:39:26.930042 janim-1.0.1/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4377 2024-05-09 02:42:00.017699 janim-1.0.1/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     3090 2024-04-17 03:59:08.856138 janim-1.0.1/janim/items/svg/typst.py
--rw-r--r--   0        0        0       40 2024-05-09 06:47:34.328454 janim-1.0.1/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    16153 2024-05-09 03:09:50.338506 janim-1.0.1/janim/items/text/text.py
--rw-r--r--   0        0        0     1094 2024-04-29 03:02:10.025824 janim-1.0.1/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5357 2024-05-06 03:22:50.462994 janim-1.0.1/janim/items/vitem.py
--rw-r--r--   0        0        0      271 2024-01-17 04:53:39.682291 janim-1.0.1/janim/logger.py
--rw-r--r--   0        0        0     3054 2024-04-29 03:26:21.783167 janim-1.0.1/janim/render/base.py
--rw-r--r--   0        0        0     8845 2024-04-29 03:02:10.025824 janim-1.0.1/janim/render/impl.py
--rw-r--r--   0        0        0      448 2024-02-20 13:10:30.002762 janim-1.0.1/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1250 2024-04-01 15:20:38.430742 janim-1.0.1/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      325 2024-02-20 13:10:30.006723 janim-1.0.1/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      180 2024-03-05 11:28:56.506406 janim-1.0.1/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      350 2024-03-05 11:28:56.506406 janim-1.0.1/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6950 2024-04-12 03:01:12.197148 janim-1.0.1/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      203 2024-02-20 13:10:30.010722 janim-1.0.1/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0     1013 2024-05-10 08:16:24.365275 janim-1.0.1/janim/render/texture.py
--rw-r--r--   0        0        0     6787 2024-04-17 03:59:08.857134 janim-1.0.1/janim/render/writer.py
--rw-r--r--   0        0        0      964 2024-04-29 03:02:10.025824 janim-1.0.1/janim/typing.py
--rw-r--r--   0        0        0    17207 2024-03-26 14:54:35.966511 janim-1.0.1/janim/utils/bezier.py
--rw-r--r--   0        0        0     5515 2024-05-11 02:51:12.477563 janim-1.0.1/janim/utils/config.py
--rw-r--r--   0        0        0     5786 2024-04-29 03:02:10.025824 janim-1.0.1/janim/utils/data.py
--rw-r--r--   0        0        0      637 2024-03-26 14:54:35.970502 janim-1.0.1/janim/utils/dict_ops.py
--rw-r--r--   0        0        0     2483 2024-04-28 10:19:08.704857 janim-1.0.1/janim/utils/file_ops.py
--rw-r--r--   0        0        0     2995 2024-05-11 03:58:36.613133 janim-1.0.1/janim/utils/font.py
--rw-r--r--   0        0        0     6369 2024-03-05 11:28:56.522384 janim-1.0.1/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5973 2024-03-05 11:28:56.530408 janim-1.0.1/janim/utils/iterables.py
--rw-r--r--   0        0        0     1870 2024-02-20 13:10:30.022729 janim-1.0.1/janim/utils/paths.py
--rw-r--r--   0        0        0     2705 2024-01-31 12:46:51.074078 janim-1.0.1/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2651 2024-05-06 04:42:35.799305 janim-1.0.1/janim/utils/refresh.py
--rw-r--r--   0        0        0     8342 2024-04-29 08:39:07.489731 janim-1.0.1/janim/utils/signal.py
--rw-r--r--   0        0        0     2000 2024-03-05 11:28:56.538410 janim-1.0.1/janim/utils/simple_functions.py
--rw-r--r--   0        0        0    10068 2024-03-08 02:47:13.319071 janim-1.0.1/janim/utils/space_ops.py
--rw-r--r--   0        0        0    22970 2024-03-08 02:47:13.327041 janim-1.0.1/logo.png
--rw-r--r--   0        0        0     1018 2024-04-17 04:51:28.717344 janim-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-05-14 01:59:46.065562 janim-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1053 2024-04-17 15:49:03.633620 janim-1.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      413 2024-05-14 01:59:46.073570 janim-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      403 2023-10-12 06:08:14.650702 janim-1.0.2/.vscode/tasks.json
+-rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.2/LICENSE
+-rw-r--r--   0        0        0      966 2024-03-08 14:50:49.538193 janim-1.0.2/README.md
+-rw-r--r--   0        0        0       71 2024-05-14 02:28:31.447277 janim-1.0.2/janim/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-17 03:59:08.847168 janim-1.0.2/janim/__main__.py
+-rw-r--r--   0        0        0     4233 2024-05-14 01:59:46.170426 janim-1.0.2/janim/anims/animation.py
+-rw-r--r--   0        0        0     6349 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/composition.py
+-rw-r--r--   0        0        0     6034 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/creation.py
+-rw-r--r--   0        0        0      815 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/display.py
+-rw-r--r--   0        0        0     3454 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/fading.py
+-rw-r--r--   0        0        0     3954 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/growing.py
+-rw-r--r--   0        0        0    10342 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/indication.py
+-rw-r--r--   0        0        0     1547 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/rotation.py
+-rw-r--r--   0        0        0    25400 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/timeline.py
+-rw-r--r--   0        0        0     9210 2024-05-14 01:59:46.178428 janim-1.0.2/janim/anims/transform.py
+-rw-r--r--   0        0        0     9946 2024-05-14 01:59:46.186425 janim-1.0.2/janim/anims/updater.py
+-rw-r--r--   0        0        0     4505 2024-05-14 01:59:46.195654 janim-1.0.2/janim/camera/camera.py
+-rw-r--r--   0        0        0     2744 2024-03-05 11:28:56.434384 janim-1.0.2/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     6808 2024-05-14 01:59:46.203658 janim-1.0.2/janim/cli.py
+-rw-r--r--   0        0        0     9221 2024-05-14 01:59:46.211660 janim-1.0.2/janim/components/component.py
+-rw-r--r--   0        0        0     2408 2024-05-14 01:59:46.219687 janim-1.0.2/janim/components/data.py
+-rw-r--r--   0        0        0     2609 2024-05-14 01:59:46.227662 janim-1.0.2/janim/components/depth.py
+-rw-r--r--   0        0        0     1284 2024-05-14 01:59:46.235662 janim-1.0.2/janim/components/image.py
+-rw-r--r--   0        0        0    30900 2024-05-14 01:59:46.249633 janim-1.0.2/janim/components/points.py
+-rw-r--r--   0        0        0     2833 2024-05-14 01:59:46.265668 janim-1.0.2/janim/components/radius.py
+-rw-r--r--   0        0        0     7922 2024-05-14 01:59:46.273667 janim-1.0.2/janim/components/rgbas.py
+-rw-r--r--   0        0        0    22599 2024-05-14 01:59:46.281677 janim-1.0.2/janim/components/vpoints.py
+-rw-r--r--   0        0        0      245 2024-05-14 01:59:46.289685 janim-1.0.2/janim/constants/__init__.py
+-rw-r--r--   0        0        0      169 2024-01-12 15:55:35.365552 janim-1.0.2/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1542 2024-05-14 01:59:46.289685 janim-1.0.2/janim/constants/colors.py
+-rw-r--r--   0        0        0      483 2024-03-05 11:28:56.458376 janim-1.0.2/janim/constants/coord.py
+-rw-r--r--   0        0        0      179 2024-01-12 15:55:05.570414 janim-1.0.2/janim/constants/degrees.py
+-rw-r--r--   0        0        0     4900 2024-05-14 02:28:31.447277 janim-1.0.2/janim/examples.py
+-rw-r--r--   0        0        0     1723 2024-05-14 01:59:46.353641 janim-1.0.2/janim/exception.py
+-rw-r--r--   0        0        0    40949 2024-05-14 01:59:46.370826 janim-1.0.2/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      330 2024-02-20 13:10:29.974744 janim-1.0.2/janim/gui/application.py
+-rw-r--r--   0        0        0      797 2024-04-17 03:59:08.853145 janim-1.0.2/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-02-20 13:10:29.978729 janim-1.0.2/janim/gui/export.png
+-rw-r--r--   0        0        0     1258 2024-02-20 13:10:29.978729 janim-1.0.2/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0      996 2024-05-14 01:59:46.378840 janim-1.0.2/janim/gui/glwidget.py
+-rw-r--r--   0        0        0      903 2024-04-24 02:36:54.042754 janim-1.0.2/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5278 2024-03-26 14:54:35.926619 janim-1.0.2/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     8331 2024-05-14 01:59:46.386831 janim-1.0.2/janim/gui/selector.py
+-rw-r--r--   0        0        0     1679 2024-05-14 01:59:46.402832 janim-1.0.2/janim/imports.py
+-rw-r--r--   0        0        0     5727 2024-05-14 01:59:46.410834 janim-1.0.2/janim/items/audio.py
+-rw-r--r--   0        0        0     4862 2024-03-08 02:47:13.255043 janim-1.0.2/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8745 2024-05-14 01:59:46.425018 janim-1.0.2/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2165 2024-05-09 02:35:32.318443 janim-1.0.2/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8330 2024-03-26 14:54:35.942576 janim-1.0.2/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8784 2024-05-14 01:59:46.430120 janim-1.0.2/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6729 2024-05-14 01:59:46.446128 janim-1.0.2/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     7917 2024-05-14 01:59:46.462124 janim-1.0.2/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5239 2024-05-14 01:59:46.470125 janim-1.0.2/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5277 2024-05-14 01:59:46.486125 janim-1.0.2/janim/items/image_item.py
+-rw-r--r--   0        0        0    19084 2024-05-14 01:59:46.486125 janim-1.0.2/janim/items/item.py
+-rw-r--r--   0        0        0     3262 2024-05-14 01:59:46.494125 janim-1.0.2/janim/items/points.py
+-rw-r--r--   0        0        0     7660 2024-05-14 01:59:46.510125 janim-1.0.2/janim/items/relation.py
+-rw-r--r--   0        0        0     2071 2024-05-14 01:59:46.518127 janim-1.0.2/janim/items/shape_matchers.py
+-rw-r--r--   0        0        0     5955 2024-05-14 01:59:46.534124 janim-1.0.2/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1736 2024-03-14 06:39:26.930042 janim-1.0.2/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4377 2024-05-14 01:59:46.542125 janim-1.0.2/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     3090 2024-04-17 03:59:08.856138 janim-1.0.2/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       40 2024-05-09 06:47:34.328454 janim-1.0.2/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    16153 2024-05-14 01:59:46.558125 janim-1.0.2/janim/items/text/text.py
+-rw-r--r--   0        0        0     1094 2024-05-14 01:59:46.566125 janim-1.0.2/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5357 2024-05-14 01:59:46.582126 janim-1.0.2/janim/items/vitem.py
+-rw-r--r--   0        0        0      271 2024-01-17 04:53:39.682291 janim-1.0.2/janim/logger.py
+-rw-r--r--   0        0        0     3054 2024-04-29 03:26:21.783167 janim-1.0.2/janim/render/base.py
+-rw-r--r--   0        0        0     8845 2024-05-14 01:59:46.614125 janim-1.0.2/janim/render/impl.py
+-rw-r--r--   0        0        0      448 2024-02-20 13:10:30.002762 janim-1.0.2/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1250 2024-04-01 15:20:38.430742 janim-1.0.2/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      325 2024-02-20 13:10:30.006723 janim-1.0.2/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      180 2024-03-05 11:28:56.506406 janim-1.0.2/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      350 2024-03-05 11:28:56.506406 janim-1.0.2/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6950 2024-04-12 03:01:12.197148 janim-1.0.2/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      203 2024-02-20 13:10:30.010722 janim-1.0.2/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0     1013 2024-05-14 01:59:46.622126 janim-1.0.2/janim/render/texture.py
+-rw-r--r--   0        0        0     6787 2024-04-17 03:59:08.857134 janim-1.0.2/janim/render/writer.py
+-rw-r--r--   0        0        0      964 2024-05-14 01:59:46.638124 janim-1.0.2/janim/typing.py
+-rw-r--r--   0        0        0    17207 2024-03-26 14:54:35.966511 janim-1.0.2/janim/utils/bezier.py
+-rw-r--r--   0        0        0     5515 2024-05-14 01:59:46.646128 janim-1.0.2/janim/utils/config.py
+-rw-r--r--   0        0        0     5786 2024-05-14 01:59:46.662124 janim-1.0.2/janim/utils/data.py
+-rw-r--r--   0        0        0      637 2024-03-26 14:54:35.970502 janim-1.0.2/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0     2483 2024-05-14 01:59:46.678125 janim-1.0.2/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     2995 2024-05-14 01:59:46.694125 janim-1.0.2/janim/utils/font.py
+-rw-r--r--   0        0        0     6369 2024-03-05 11:28:56.522384 janim-1.0.2/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5973 2024-03-05 11:28:56.530408 janim-1.0.2/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1870 2024-02-20 13:10:30.022729 janim-1.0.2/janim/utils/paths.py
+-rw-r--r--   0        0        0     2705 2024-01-31 12:46:51.074078 janim-1.0.2/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2651 2024-05-14 01:59:46.710124 janim-1.0.2/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8342 2024-05-14 01:59:46.718125 janim-1.0.2/janim/utils/signal.py
+-rw-r--r--   0        0        0     2000 2024-03-05 11:28:56.538410 janim-1.0.2/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0    10068 2024-03-08 02:47:13.319071 janim-1.0.2/janim/utils/space_ops.py
+-rw-r--r--   0        0        0    22970 2024-03-08 02:47:13.327041 janim-1.0.2/logo.png
+-rw-r--r--   0        0        0     1018 2024-04-17 04:51:28.717344 janim-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.2/PKG-INFO
```

### Comparing `janim-1.0.1/.readthedocs.yaml` & `janim-1.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/LICENSE` & `janim-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/README.md` & `janim-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/__main__.py` & `janim-1.0.2/janim/__main__.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/anims/animation.py` & `janim-1.0.2/janim/anims/animation.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 if TYPE_CHECKING:   # pragma: no cover
     from janim.anims.composition import AnimGroup
     from janim.components.depth import Cmpt_Depth
 
 
 @dataclass
 class TimeRange:
+    '''
+    标识了从 ``at`` 开始，持续时间为 ``duration`` 的时间区段
+
+    ``end`` 即 ``at + duration``
+    '''
     at: float
     duration: float
 
     @property
     def end(self) -> float:
         return self.at + self.duration
```

### Comparing `janim-1.0.1/janim/anims/composition.py` & `janim-1.0.2/janim/anims/composition.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/anims/creation.py` & `janim-1.0.2/janim/anims/creation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 
 from typing import Callable
 
 import numpy as np
 
 from janim.anims.updater import DataUpdater, UpdaterParams
 from janim.components.vpoints import Cmpt_VPoints
-from janim.constants import NAN_POINT
+from janim.constants import (C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN,
+                             C_LABEL_ANIM_OUT, NAN_POINT)
 from janim.items.item import Item
 from janim.items.vitem import VItem
 from janim.typing import JAnimColor
 from janim.utils.bezier import integer_interpolate
 from janim.utils.rate_functions import RateFunc, double_smooth, linear
 
 
 class ShowPartial(DataUpdater):
     '''
     显示物件一部分的动画，显示的部分由 ``bound_func`` 决定
     '''
-    label_color = (54, 164, 186)
+    label_color = C_LABEL_ANIM_ABSTRACT
 
     def __init__(
         self,
         item: Item,
         bound_func: Callable[[UpdaterParams], tuple[int, int]],
         *,
         auto_close_path: bool = False,
@@ -67,22 +68,26 @@
         super().__init__(item, func, become_at_end=become_at_end, root_only=root_only, **kwargs)
 
 
 class Create(ShowPartial):
     '''
     显示物件的创建过程
     '''
+    label_color = C_LABEL_ANIM_IN
+
     def __init__(self, item: Item, auto_close_path: bool = True, **kwargs):
         super().__init__(item, lambda p: (0, p.alpha), auto_close_path=auto_close_path, **kwargs)
 
 
 class Uncreate(ShowPartial):
     '''
     显示物件的销毁过程（:class:`Create` 的倒放）
     '''
+    label_color = C_LABEL_ANIM_OUT
+
     def __init__(
         self,
         item: Item,
         show_at_end: bool = False,
         auto_close_path: bool = True,
         **kwargs
     ):
@@ -95,15 +100,15 @@
         )
 
 
 class DrawBorderThenFill(DataUpdater):
     '''
     画出边缘，然后填充颜色
     '''
-    label_color = (54, 164, 186)
+    label_color = C_LABEL_ANIM_IN
 
     def __init__(
         self,
         item: Item,
         *,
         duration: float = 2.0,
         stroke_radius: float = 0.01,
```

### Comparing `janim-1.0.1/janim/anims/fading.py` & `janim-1.0.2/janim/anims/fading.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 
 from abc import ABCMeta, abstractmethod
 
 import numpy as np
 
+from janim.anims.updater import DataUpdater, UpdaterParams
+from janim.components.rgbas import Cmpt_Rgbas
+from janim.constants import (C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN,
+                             C_LABEL_ANIM_OUT, ORIGIN)
 from janim.items.item import Item
 from janim.items.points import Points
-from janim.components.rgbas import Cmpt_Rgbas
-from janim.anims.updater import DataUpdater, UpdaterParams
 from janim.typing import Vect
-from janim.constants import ORIGIN
 
 
 class Fade(DataUpdater, metaclass=ABCMeta):
     '''
     :class:`FadeIn` 和 :class:`FadeOut` 的基类
     '''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
     def __init__(
         self,
         item: Item,
         shift: Vect = ORIGIN,
         scale: float = 1.0,
         *,
         about_point: Vect | None = None,
@@ -51,14 +54,16 @@
 class FadeIn(Fade):
     '''
     淡入
 
     - 可以使用 ``shift`` 指定淡入位移
     - 可以使用 ``scale`` 指定淡入缩放
     '''
+    label_color = C_LABEL_ANIM_IN
+
     def updater(self, data: Item, p: UpdaterParams) -> None:
         if not isinstance(data, Points):
             return
 
         for cmpt in data.components.values():
             if not isinstance(cmpt, Cmpt_Rgbas):
                 continue
@@ -78,14 +83,16 @@
 class FadeOut(Fade):
     '''
     淡出
 
     - 可以使用 ``shift`` 指定淡出位移
     - 可以使用 ``scale`` 指定淡出缩放
     '''
+    label_color = C_LABEL_ANIM_OUT
+
     def __init__(
         self,
         item: Item,
         shift: Vect = ORIGIN,
         scale: float = 1.0,
         show_at_end: float = False,
         **kwargs
```

### Comparing `janim-1.0.1/janim/anims/indication.py` & `janim-1.0.2/janim/anims/indication.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,32 @@
 
 from janim.anims.animation import Animation
 from janim.anims.composition import AnimGroup, Succession
 from janim.anims.creation import Create, ShowPartial
 from janim.anims.fading import FadeOut
 from janim.anims.updater import DataUpdater, UpdaterParams
 from janim.components.rgbas import Cmpt_Rgbas
-from janim.constants import GREY, ORIGIN, RIGHT, TAU, YELLOW
+from janim.constants import (C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_INDICATION,
+                             GREY, ORIGIN, RIGHT, TAU, YELLOW)
 from janim.items.geometry.arc import Circle, Dot
 from janim.items.geometry.line import Line
 from janim.items.item import Item
 from janim.items.points import Group, Points
 from janim.items.shape_matchers import SurroundingRect
 from janim.items.vitem import VItem
 from janim.typing import JAnimColor, Vect
 from janim.utils.bezier import interpolate
 from janim.utils.config import Config
 from janim.utils.rate_functions import RateFunc, there_and_back
 
 
 class FocusOn(DataUpdater[Dot]):
     '''展现一个逐渐聚焦到指定物件的圆形缩小动画'''
+    label_color = C_LABEL_ANIM_INDICATION
+
     def __init__(
         self,
         point_or_item: Vect | Points,
         *,
         about_edge: Vect = ORIGIN,
         color: JAnimColor = GREY,
         alpha: float = 0.2,
@@ -52,14 +55,16 @@
 
         super().__init__(dot1, updater, duration=duration, **kwargs)
         self.timeline.track(dot1)
 
 
 class Indicate(DataUpdater):
     '''展现指定物件以放大为黄色后回到原状的动画'''
+    label_color = C_LABEL_ANIM_INDICATION
+
     def __init__(
         self,
         item: Points,
         *,
         scale_factor: float = 1.2,
         color: JAnimColor = YELLOW,
         rate_func: RateFunc = there_and_back,
@@ -94,14 +99,22 @@
             if not isinstance(cmpt, Cmpt_Rgbas):
                 continue
             cmpt.set(self.color)
         return data_copy
 
 
 class CircleIndicate(DataUpdater[Circle]):
+    '''
+    展现以圆圈在指定物件周围淡入淡出进行强调的动画
+
+    - 可以使用 ``rate_func=there_and_back_with_pause`` 使得动画中间停留一段时间
+    - 可以传入 ``scale`` 指定缩放，例如 ``scale=1.2`` 即缩小的同时淡入，并且放大的同时淡出
+    '''
+    label_color = C_LABEL_ANIM_INDICATION
+
     def __init__(
         self,
         item: Points,
         *,
         color: JAnimColor = YELLOW,
         rate_func: RateFunc = there_and_back,
         scale: float = 1,
@@ -124,14 +137,19 @@
             show_at_end=False,
             become_at_end=False,
             **kwargs
         )
 
 
 class ShowPassingFlash(ShowPartial):
+    '''
+    基于 ``time_width`` 显示物件的一小段
+    '''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
     def __init__(
         self,
         item: Points,
         *,
         time_width: float = 0.1,
         auto_close_path: bool = False,
         **kwargs
@@ -152,36 +170,46 @@
             become_at_end=False,
             **kwargs
         )
 
 
 class ShowCreationThenDestruction(ShowPassingFlash):
     '''展现创建动画后展现销毁动画'''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
     def __init__(
         self,
         item: Points,
         *,
         time_width: float = 2.0,
         duration: float = 1,
         **kwargs
     ):
         super().__init__(item, time_width=time_width, duration=duration, **kwargs)
 
 
 class ShowCreationThenFadeOut(Succession):
     '''展现创建动画后展现淡出动画'''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
     def __init__(self, item: Points, create_kwargs: dict = {}, fadeout_kwargs: dict = {}, **kwargs):
         super().__init__(
             Create(item, **create_kwargs),
             FadeOut(item, **fadeout_kwargs),
             **kwargs
         )
 
 
 class AnimationOnSurroundingRect(AnimGroup):
+    '''
+    :class:`ShowPassingFlash`、:class:`ShowCreationThenDestructionAround`、
+    :class:`ShowCreationThenFadeAround` 的基类
+    '''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
     def __init__(
         self,
         item: Points,
         rect_anim: type[Animation],
         surrounding_rect_config: dict = {},
         **kwargs
     ):
@@ -211,34 +239,43 @@
         elif isinstance(anim, AnimGroup):
             for sub in anim.anims:
                 self.apply_updater(sub)
 
 
 class ShowPassingFlashAround(AnimationOnSurroundingRect):
     '''不完整线条在指定物件周围环绕一圈的动画'''
+    label_color = C_LABEL_ANIM_INDICATION
+
     def __init__(self, item: Points, **kwargs) -> None:
         super().__init__(item, ShowPassingFlash, **kwargs)
 
 
 class ShowCreationThenDestructionAround(AnimationOnSurroundingRect):
     '''在指定物件周围先创建出完整线条再销毁线条的动画'''
+    label_color = C_LABEL_ANIM_INDICATION
+
     def __init__(self, item: Points, **kwargs) -> None:
         super().__init__(item, ShowCreationThenDestruction, **kwargs)
 
 
 class ShowCreationThenFadeAround(AnimationOnSurroundingRect):
     '''在指定物件周围先创建出完整线条再淡出线条的动画'''
+    label_color = C_LABEL_ANIM_INDICATION
+
     def __init__(self, item: Points, **kwargs) -> None:
         super().__init__(item,
                          ShowCreationThenFadeOut,
                          create_kwargs=dict(auto_close_path=False),
                          **kwargs)
 
 
 class Flash(ShowCreationThenDestruction):
+    '''展现以放射状线条进行强调的动画'''
+    label_color = C_LABEL_ANIM_INDICATION
+
     def __init__(
         self,
         point_or_item: Vect | Points,
         *,
         color: JAnimColor = YELLOW,
         line_length: float = 0.2,
         num_lines: int = 12,
@@ -272,7 +309,13 @@
             line.points.shift((self.flash_radius - self.line_length) * RIGHT)
             line.points.rotate(angle, about_point=ORIGIN)
             lines.add(line)
         lines(VItem) \
             .stroke.set(self.color) \
             .r.radius.set(self.line_stroke_radius)
         return lines
+
+
+# TODO: ApplyWave
+# TODO: WiggleOutThenIn
+# TODO: TurnInsideOut
+# TODO: FlashyFadeIn
```

### Comparing `janim-1.0.1/janim/anims/rotation.py` & `janim-1.0.2/janim/anims/rotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 from janim.anims.updater import DataUpdater, UpdaterParams
 from janim.components.points import Cmpt_Points
-from janim.constants import ORIGIN, OUT
+from janim.constants import C_LABEL_ANIM_STAY, ORIGIN, OUT
 from janim.items.item import Item
 from janim.items.points import Points
 from janim.typing import Vect
 from janim.utils.rate_functions import linear
 
 
 class Rotate(DataUpdater):
     '''
     旋转，默认对角度进行平滑插值
     '''
-    label_color = (64, 181, 126)
+    label_color = C_LABEL_ANIM_STAY
 
     def __init__(
         self,
         item: Item,
         angle: float,
         *,
         axis: Vect = OUT,
```

### Comparing `janim-1.0.1/janim/anims/timeline.py` & `janim-1.0.2/janim/anims/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             self.token = config_ctx_var.set(lst)
             return self
 
         def __exit__(self, exc_type, exc_value, tb) -> None:
             config_ctx_var.reset(self.token)
 
     @classmethod
-    def with_config(cls) -> _WithConfig:
+    def _with_config(cls) -> _WithConfig:
         '''
         使用定义在 :class:`Timeline` 子类中的 config
         '''
         return cls._WithConfig(cls)
 
     # endregion
 
@@ -98,15 +98,15 @@
     ctx_var: ContextVar[Timeline | None] = ContextVar('Timeline.ctx_var', default=None)
 
     @staticmethod
     def get_context(raise_exc=True) -> Timeline | None:
         '''
         调用该方法可以得到当前正在构建的 :class:`Timeline` 对象
 
-        - 如果在 :meth:`construct` 方法外调用，且 ``raise_exc=True`` （默认），则抛出 ``LookupError``
+        - 如果在 :meth:`construct` 方法外调用，且 ``raise_exc=True`` （默认），则抛出 :class:`~.TimelineLookupError`
         '''
         obj = Timeline.ctx_var.get(None)
         if obj is None and raise_exc:
             f_back = inspect.currentframe().f_back
             raise TimelineLookupError(f'{f_back.f_code.co_qualname} 无法在 Timeline.construct 之外使用')
         return obj
 
@@ -176,15 +176,15 @@
         '''
         pass    # pragma: no cover
 
     def build(self, *, quiet=False) -> TimelineAnim:
         '''
         构建动画并返回
         '''
-        with self.with_config(), ContextSetter(self.ctx_var, self):
+        with self._with_config(), ContextSetter(self.ctx_var, self):
 
             self.config_getter = ConfigGetter(config_ctx_var.get())
             self.camera = Camera()
 
             self._build_frame = inspect.currentframe()
 
             if not quiet:   # pragma: no cover
@@ -276,14 +276,19 @@
         self.forward_to(t_range.end, _detect_changes=False)
 
     # endregion
 
     # region display
 
     def is_displaying(self, item: Item) -> None:
+        '''
+        判断特定的物件是否正在显示中
+
+        另见：:meth:`show`、:meth:`hide`
+        '''
         return item in self.item_display_times
 
     def _show(self, item: Item) -> None:
         self.item_display_times.setdefault(item, self.current_time)
 
     def show(self, *roots: Item, root_only=False) -> None:
         '''
@@ -353,22 +358,28 @@
                                       TimeRange(self.current_time + delay, duration),
                                       TimeRange(begin, duration))
         self.audio_infos.append(info)
 
         return info.range.copy()
 
     def has_audio(self) -> bool:
+        '''
+        是否有可以播放的音频
+        '''
         return len(self.audio_infos) != 0
 
     def get_audio_samples_of_frame(
         self,
         fps: float,
         framerate: int,
         frame: int
     ) -> np.ndarray:
+        '''
+        提取特定帧的音频流
+        '''
         begin = frame / fps
         end = (frame + 1) / fps
 
         output_sample_count = math.floor(end * framerate) - math.floor(begin * framerate)
         result = np.zeros(output_sample_count, dtype=np.int16)
 
         for info in self.audio_infos:
@@ -472,14 +483,20 @@
 
             self.schedule(range.at, subtitle_group.show)
             self.schedule(range.end, subtitle_group.hide)
 
         return range.copy()
 
     def place_subtitle(self, subtitle: Text, range: TimeRange) -> None:
+        '''
+        被 :meth:`subtitle` 调用以将字幕放置到合适的位置：
+
+        - 对于同一批添加的字幕 ``[a, b]``，则 ``a`` 放在 ``b`` 的上面
+        - 如果在上文所述的 ``[a, b]`` 仍存在时，又加入了一个 ``c``，则 ``c`` 放在最上面
+        '''
         for other in reversed(self.subtitle_infos):
             # 根据 TimelineView 中排列显示标签的经验
             # 这里加了一个 np.isclose 的判断
             # 如果不加可能导致前一个字幕消失但是后一个字幕凭空出现在更上面
             # （但是我没有测试过是否会出现这个bug，只是根据写 TimelineView 时的经验加了 np.isclose）
             if other.range.at <= range.at < other.range.end and not np.isclose(range.at, other.range.end):
                 subtitle.points.next_to(other.subtitle, UP, buff=SMALL_BUFF)
@@ -537,14 +554,17 @@
                 static = ih.history_without_dynamic.latest().data
             else:
                 static = item.store()
         ih.history.record_as_time(end, static, replaceable=static_replaceable)
         ih.history_without_dynamic.record_as_time(end, static, replaceable=static_replaceable)
 
     def item_current[T](self, item: T, *, as_time: float | None = None, skip_dynamic=False) -> T:
+        '''
+        另见 :meth:`~.Item.current`
+        '''
         ih = self.items_history[item]
         history = ih.history_without_dynamic if skip_dynamic else ih.history
         if not history.has_record():
             return item
 
         if as_time is None:
             params = updater_params_ctx.get(None)
```

### Comparing `janim-1.0.1/janim/anims/transform.py` & `janim-1.0.2/janim/anims/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from typing import Self
 
 from janim.anims.animation import Animation, RenderCall
 from janim.components.component import Component
-from janim.constants import ANIM_END_DELTA, OUT
+from janim.constants import ANIM_END_DELTA, OUT, C_LABEL_ANIM_STAY
 from janim.items.item import DynamicItem, Item
 from janim.logger import log
 from janim.typing import Vect
 from janim.utils.data import AlignedData
 from janim.utils.paths import PathFunc, path_along_arc, straight_path
 
 
 class Transform(Animation):
-    label_color = (208, 171, 67)
+    '''
+    创建从 ``src_item`` 至 ``target_item`` 的插值动画
+
+    - ``path_arc`` 和 ``path_arc_axis`` 可以指定插值的圆弧路径的角度，若不传入则是直线
+    - 也可以直接传入 ``path_func`` 来指定路径方法
+    '''
+    label_color = C_LABEL_ANIM_STAY
 
     def __init__(
         self,
         src_item: Item,
         target_item: Item,
         *,
         path_arc: float = 0,
@@ -139,15 +145,15 @@
 
 class MethodTransform(Transform):
     '''
     依据物件的变换而创建的补间过程
 
     具体参考 :meth:`~.Item.anim`
     '''
-    label_color = (196, 130, 69)
+    label_color = (196, 130, 69)    # C_LABEL_ANIM_STAY 的变体
 
     def __init__(self, item: Item, **kwargs):
         super().__init__(item, item, **kwargs)
         self.current_alpha = None
 
         self.timeline.detect_changes(item.walk_self_and_descendants())
```

### Comparing `janim-1.0.1/janim/anims/updater.py` & `janim-1.0.2/janim/anims/updater.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import inspect
 from contextvars import ContextVar
 from dataclasses import dataclass
 from typing import Any, Callable, Self
 
 from janim.anims.animation import Animation, RenderCall, TimeRange
-from janim.constants import ANIM_END_DELTA
+from janim.constants import ANIM_END_DELTA, C_LABEL_ANIM_ABSTRACT
 from janim.exception import UpdaterError
-from janim.items.item import Item, DynamicItem
+from janim.items.item import DynamicItem, Item
 from janim.utils.simple_functions import clip
 
 
 @dataclass
 class UpdaterParams:
     '''
     ``Updater`` 调用时会传递的参数，用于标注时间信息以及动画进度
@@ -56,15 +56,15 @@
                     )
                 )
 
     会产生一个“矩形从左侧旋转着移动到右侧”的动画
 
     另见：:class:`~.UpdaterExample`
     '''
-    label_color = (49, 155, 191)
+    label_color = C_LABEL_ANIM_ABSTRACT
 
     @dataclass
     class DataGroup:
         orig_data: Item
         data: Item
         extra_data: Any | None
 
@@ -209,15 +209,15 @@
 
     - 传入的 ``item`` 会在动画的末尾被替换为动画最后一帧 ``func`` 所返回的物件，传入 ``become_at_end=False`` 以禁用
     - 传入的 ``item`` 会在动画开始时隐藏，在动画结束后显示，传入 ``hide_at_begin=False`` 和 ``show_at_end=False`` 以禁用
     - 若传入 ``item=None``，则以上两点都无效
 
     另见：:class:`~.UpdaterExample`
     '''
-    label_color = DataUpdater.label_color
+    label_color = C_LABEL_ANIM_ABSTRACT
 
     def __init__(
         self,
         item: Item | None,
         func: Callable[[UpdaterParams], Item],
         *,
         hide_at_begin: bool = True,
```

### Comparing `janim-1.0.1/janim/camera/camera.py` & `janim-1.0.2/janim/camera/camera.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/camera/camera_info.py` & `janim-1.0.2/janim/camera/camera_info.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/cli.py` & `janim-1.0.2/janim/cli.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/component.py` & `janim-1.0.2/janim/components/component.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/data.py` & `janim-1.0.2/janim/components/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/depth.py` & `janim-1.0.2/janim/components/depth.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/image.py` & `janim-1.0.2/janim/components/image.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/points.py` & `janim-1.0.2/janim/components/points.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/radius.py` & `janim-1.0.2/janim/components/radius.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/rgbas.py` & `janim-1.0.2/janim/components/rgbas.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/components/vpoints.py` & `janim-1.0.2/janim/components/vpoints.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/examples.py` & `janim-1.0.2/janim/examples.py`

 * *Files 15% similar despite different names*

```diff
@@ -84,19 +84,22 @@
 
 
 class TypstExample(Timeline):
     def construct(self) -> None:
         doc = TypstDoc(typst_doc)
         typ = Typst('sum_(i=1)^n x_i')
 
-        self.show(doc)
+        # Applying animations on text is slow
+        self.play(Write(doc), duration=4)
         self.forward()
-        self.hide(doc)
-        self.show(typ)
+        self.play(FadeOut(doc))
+
+        self.play(Write(typ))
         self.forward()
+        self.play(FadeOut(typ))
 
 
 class AnimatingPiExample(Timeline):
     def construct(self) -> None:
         grid = Typst('pi') * 100
         grid.points.scale(2).arrange_in_grid(10, 10, buff=0.2)
         grid.show()
```

### Comparing `janim-1.0.1/janim/exception.py` & `janim-1.0.2/janim/exception.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/anim_viewer.py` & `janim-1.0.2/janim/gui/anim_viewer.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/audio_player.py` & `janim-1.0.2/janim/gui/audio_player.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/export.png` & `janim-1.0.2/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/fixed_ratio_widget.py` & `janim-1.0.2/janim/gui/fixed_ratio_widget.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/glwidget.py` & `janim-1.0.2/janim/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/precise_timer.py` & `janim-1.0.2/janim/gui/precise_timer.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/richtext_editor.py` & `janim-1.0.2/janim/gui/richtext_editor.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/gui/selector.py` & `janim-1.0.2/janim/gui/selector.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/imports.py` & `janim-1.0.2/janim/imports.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/audio.py` & `janim-1.0.2/janim/items/audio.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/boolean_ops.py` & `janim-1.0.2/janim/items/boolean_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/coordinate/coordinate_systems.py` & `janim-1.0.2/janim/items/coordinate/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/coordinate/functions.py` & `janim-1.0.2/janim/items/coordinate/functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/coordinate/number_line.py` & `janim-1.0.2/janim/items/coordinate/number_line.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/geometry/arc.py` & `janim-1.0.2/janim/items/geometry/arc.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/geometry/arrow.py` & `janim-1.0.2/janim/items/geometry/arrow.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/geometry/line.py` & `janim-1.0.2/janim/items/geometry/line.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/geometry/polygon.py` & `janim-1.0.2/janim/items/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/image_item.py` & `janim-1.0.2/janim/items/image_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/item.py` & `janim-1.0.2/janim/items/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,20 @@
             return False
         for key, cmpt in self.components.items():
             if not cmpt.not_changed(other.components[key]):
                 return False
         return True
 
     def current(self, *, as_time: float | None = None, skip_dynamic=False) -> Self:
+        '''
+        当前物件
+
+        - 如果此时在回放和 Updater 中，则返回对应时间的历史物件
+        - 在其余情况下，包括该物件没有历史记录的情况，则返回物件自身
+        '''
         return self.timeline.item_current(self, as_time=as_time, skip_dynamic=skip_dynamic)
 
     def copy(self, *, root_only=False) -> Self:
         '''
         复制物件
         '''
         copy_item = copy.copy(self)
```

### Comparing `janim-1.0.1/janim/items/points.py` & `janim-1.0.2/janim/items/points.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/relation.py` & `janim-1.0.2/janim/items/relation.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/shape_matchers.py` & `janim-1.0.2/janim/items/shape_matchers.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/svg/brace.py` & `janim-1.0.2/janim/items/svg/brace.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/svg/brace.svg` & `janim-1.0.2/janim/items/svg/brace.svg`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/svg/svg_item.py` & `janim-1.0.2/janim/items/svg/svg_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/svg/typst.py` & `janim-1.0.2/janim/items/svg/typst.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/text/text.py` & `janim-1.0.2/janim/items/text/text.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/value_tracker.py` & `janim-1.0.2/janim/items/value_tracker.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/items/vitem.py` & `janim-1.0.2/janim/items/vitem.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/render/base.py` & `janim-1.0.2/janim/render/base.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/render/impl.py` & `janim-1.0.2/janim/render/impl.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/render/shaders/dotcloud.geom.glsl` & `janim-1.0.2/janim/render/shaders/dotcloud.geom.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/render/shaders/vitem.frag.glsl` & `janim-1.0.2/janim/render/shaders/vitem.frag.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/render/texture.py` & `janim-1.0.2/janim/render/texture.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/render/writer.py` & `janim-1.0.2/janim/render/writer.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/typing.py` & `janim-1.0.2/janim/typing.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/bezier.py` & `janim-1.0.2/janim/utils/bezier.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/config.py` & `janim-1.0.2/janim/utils/config.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/data.py` & `janim-1.0.2/janim/utils/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/dict_ops.py` & `janim-1.0.2/janim/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/file_ops.py` & `janim-1.0.2/janim/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/font.py` & `janim-1.0.2/janim/utils/font.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/font_manager.py` & `janim-1.0.2/janim/utils/font_manager.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/iterables.py` & `janim-1.0.2/janim/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/paths.py` & `janim-1.0.2/janim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/rate_functions.py` & `janim-1.0.2/janim/utils/rate_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/refresh.py` & `janim-1.0.2/janim/utils/refresh.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/signal.py` & `janim-1.0.2/janim/utils/signal.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/simple_functions.py` & `janim-1.0.2/janim/utils/simple_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/janim/utils/space_ops.py` & `janim-1.0.2/janim/utils/space_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/logo.png` & `janim-1.0.2/logo.png`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/pyproject.toml` & `janim-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `janim-1.0.1/PKG-INFO` & `janim-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janim
-Version: 1.0.1
+Version: 1.0.2
 Summary: a library for simple animation effects
 Author: jkjkil4
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Requires-Dist: numpy
 Requires-Dist: scipy
```

