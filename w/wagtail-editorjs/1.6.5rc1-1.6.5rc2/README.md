# Comparing `tmp/wagtail_editorjs-1.6.5rc1.tar.gz` & `tmp/wagtail_editorjs-1.6.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_editorjs-1.6.5rc1.tar", last modified: Mon May 13 23:37:04 2024, max compression
+gzip compressed data, was "wagtail_editorjs-1.6.5rc2.tar", last modified: Tue May 14 00:50:25 2024, max compression
```

## Comparing `wagtail_editorjs-1.6.5rc1.tar` & `wagtail_editorjs-1.6.5rc2.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.665804 wagtail_editorjs-1.6.5rc1/
--rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc1/LICENSE
--rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc1/MANIFEST.in
--rw-rw-rw-   0        0        0     6784 2024-05-13 23:37:04.666802 wagtail_editorjs-1.6.5rc1/PKG-INFO
--rw-rw-rw-   0        0        0     5647 2024-05-13 23:33:57.000000 wagtail_editorjs-1.6.5rc1/README.md
--rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc1/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-05-13 23:37:04.671348 wagtail_editorjs-1.6.5rc1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.5rc1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.341616 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/
--rw-rw-rw-   0        0        0      334 2024-05-13 23:37:01.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/__init__.py
--rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/apps.py
--rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/blocks.py
--rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/django_editor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.370571 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/
--rw-rw-rw-   0        0        0      668 2024-05-13 14:46:42.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/__init__.py
--rw-rw-rw-   0        0        0    16033 2024-05-13 23:33:06.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/blocks.py
--rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/documents.py
--rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/images.py
--rw-rw-rw-   0        0        0     7721 2024-05-01 07:39:27.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/inlines.py
--rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/lists.py
--rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/tunes.py
--rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/fields.py
--rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/forms.py
--rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.373678 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.375693 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.381706 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/
--rw-rw-rw-   0        0        0      932 2024-05-13 14:22:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.389963 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/
--rw-rw-rw-   0        0        0      255 2024-05-13 14:22:16.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/__init__.py
--rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/attrs.py
--rw-rw-rw-   0        0        0     5110 2024-05-13 14:43:24.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/element.py
--rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/utils.py
--rw-rw-rw-   0        0        0     7337 2024-05-13 23:25:18.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/feature_registry.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.402732 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/
--rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/__init__.py
--rw-rw-rw-   0        0        0     7865 2024-05-13 23:22:22.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/base.py
--rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/basic.py
--rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/inlines.py
--rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/snippets_inlines.py
--rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/view.py
--rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/value.py
--rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/render.py
--rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.288914 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.295065 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.408735 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/
--rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
--rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.415902 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/
--rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
--rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
--rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.421161 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/
--rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
--rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.455873 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/
--rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.462850 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
--rw-rw-rw-   0        0        0     2661 2024-04-27 00:14:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
--rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
--rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
--rw-rw-rw-   0        0        0     3876 2024-05-13 23:22:09.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
--rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
--rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
--rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
--rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
--rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
--rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
--rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
--rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.298807 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.470601 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
--rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.561082 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
--rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
--rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
--rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
--rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
--rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
--rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
--rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
--rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
--rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
--rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
--rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
--rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
--rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
--rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
--rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
--rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
--rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
--rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
--rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
--rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
--rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
--rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.567087 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
--rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.579966 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.301865 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.583981 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/
--rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.586979 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/
--rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.592555 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.598516 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
--rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/editorjs.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.604068 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.609596 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/__init__.py
--rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.612607 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.633541 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/base.py
--rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_attrs.py
--rw-rw-rw-   0        0        0     2711 2024-05-13 17:36:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_inlines.py
--rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_render.py
--rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.649798 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/settings.py
--rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/urls.py
--rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.662799 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/
--rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/features.py
--rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.353846 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/
--rw-rw-rw-   0        0        0     6784 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6006 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.270301 wagtail_editorjs-1.6.5rc2/
+-rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc2/LICENSE
+-rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6784 2024-05-14 00:50:25.270301 wagtail_editorjs-1.6.5rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     5647 2024-05-13 23:33:57.000000 wagtail_editorjs-1.6.5rc2/README.md
+-rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc2/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-05-14 00:50:25.274308 wagtail_editorjs-1.6.5rc2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.5rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.035995 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      334 2024-05-14 00:50:21.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/apps.py
+-rw-rw-rw-   0        0        0     1985 2024-05-14 00:45:36.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/blocks.py
+-rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/django_editor.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.065542 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/
+-rw-rw-rw-   0        0        0      668 2024-05-13 14:46:42.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/__init__.py
+-rw-rw-rw-   0        0        0    16540 2024-05-14 00:29:32.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/blocks.py
+-rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/documents.py
+-rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/images.py
+-rw-rw-rw-   0        0        0     7721 2024-05-01 07:39:27.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/inlines.py
+-rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/lists.py
+-rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/tunes.py
+-rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/fields.py
+-rw-rw-rw-   0        0        0     6875 2024-05-14 00:47:04.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/forms.py
+-rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.067542 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.069539 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.076982 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/
+-rw-rw-rw-   0        0        0      932 2024-05-13 14:22:20.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.086507 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/
+-rw-rw-rw-   0        0        0      255 2024-05-13 14:22:16.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/__init__.py
+-rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/attrs.py
+-rw-rw-rw-   0        0        0     5110 2024-05-13 14:43:24.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/element.py
+-rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/utils.py
+-rw-rw-rw-   0        0        0     7527 2024-05-14 00:46:02.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/feature_registry.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.101148 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/
+-rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/__init__.py
+-rw-rw-rw-   0        0        0     8012 2024-05-14 00:21:24.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/base.py
+-rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/basic.py
+-rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/inlines.py
+-rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/snippets_inlines.py
+-rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/view.py
+-rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/value.py
+-rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/render.py
+-rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:24.982461 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:24.988470 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.106153 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/css/
+-rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
+-rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.114209 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/
+-rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
+-rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
+-rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.117205 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/init/
+-rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
+-rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.139443 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/
+-rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.145751 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
+-rw-rw-rw-   0        0        0     2661 2024-04-27 00:14:45.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
+-rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
+-rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+-rw-rw-rw-   0        0        0     3876 2024-05-13 23:22:09.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
+-rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
+-rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
+-rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
+-rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
+-rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
+-rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
+-rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
+-rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:24.991675 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.151302 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
+-rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.199235 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
+-rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
+-rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
+-rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
+-rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
+-rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
+-rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
+-rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
+-rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
+-rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
+-rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
+-rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
+-rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
+-rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
+-rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
+-rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
+-rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
+-rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
+-rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
+-rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
+-rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
+-rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
+-rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.200251 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
+-rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.208250 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:24.994669 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templates/
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.211338 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templates/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.213338 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templates/wagtail_editorjs/widgets/
+-rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.216334 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.220726 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/editorjs.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.225734 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.230256 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.232278 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.247773 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_attrs.py
+-rw-rw-rw-   0        0        0     3060 2024-05-14 00:17:57.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_inlines.py
+-rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_render.py
+-rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.259302 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/settings.py
+-rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.269292 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/
+-rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/features.py
+-rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-14 00:50:25.049407 wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/
+-rw-rw-rw-   0        0        0     6784 2024-05-14 00:50:24.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6006 2024-05-14 00:50:24.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 00:50:24.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-14 00:50:24.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-14 00:50:24.000000 wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/top_level.txt
```

### Comparing `wagtail_editorjs-1.6.5rc1/LICENSE` & `wagtail_editorjs-1.6.5rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/PKG-INFO` & `wagtail_editorjs-1.6.5rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_editorjs
-Version: 1.6.5rc1
+Version: 1.6.5rc2
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_editorjs-1.6.5rc1/README.md` & `wagtail_editorjs-1.6.5rc2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/setup.cfg` & `wagtail_editorjs-1.6.5rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f65 6469 746f   = wagtail_edito
 00000020: 726a 730d 0a76 6572 7369 6f6e 203d 2031  rjs..version = 1
-00000030: 2e36 2e35 7263 310d 0a64 6573 6372 6970  .6.5rc1..descrip
+00000030: 2e36 2e35 7263 320d 0a64 6573 6372 6970  .6.5rc2..descrip
 00000040: 7469 6f6e 203d 2045 6469 746f 724a 5320  tion = EditorJS 
 00000050: 6173 2061 2077 6964 6765 7420 666f 7220  as a widget for 
 00000060: 5761 6774 6169 6c2c 2077 6974 6820 5061  Wagtail, with Pa
 00000070: 6765 2d20 616e 6420 496d 6167 6520 6368  ge- and Image ch
 00000080: 6f6f 7365 7220 7375 7070 6f72 740d 0a6c  ooser support..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
```

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/blocks.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/django_editor.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/django_editor.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/__init__.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/blocks.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,64 @@
             "allowed_tags": allowed_tags,
             "allowed_attributes": allowed_attributes,
         })
 
         for _, block in self.child_blocks.items():
             if isinstance(block, (blocks.StreamBlock, blocks.ListBlock)):
                 raise ValueError("StreamBlock and ListBlock are not allowed in StructBlock children for the EditorJSFeatureStructBlock")
-        
+
+def get_allowed_tags(instance: EditorJSFeatureStructBlock, block: blocks.Block, l = None) -> list[str]:
+
+    if hasattr(block, "allowed_tags"):
+        l = block.allowed_tags
+    elif hasattr(block.meta, "allowed_tags"):
+        l = block.meta.allowed_tags
+
+    l = l or []
+
+    if isinstance(block, blocks.StructBlock):
+        for _, b in block.child_blocks.items():
+            l += get_allowed_tags(instance, b, l)
+
+    return list(set(list(l) + ["div"]))
+
+def get_allowed_attributes(instance: EditorJSFeatureStructBlock, block: blocks.Block, d = None) -> dict[str, list[str]]:
+    if hasattr(block, "allowed_attributes"):
+        obj_dict = block.allowed_attributes
+    elif hasattr(block.meta, "allowed_attributes"):
+        obj_dict = block.meta.allowed_attributes
+    else:
+        obj_dict = {}
+
+    if d is None:
+        d = obj_dict
+    else:
+        for key, value in obj_dict.items():
+            d[key] = set(list(d.get(key, [])) + list(value))
+    
+    if isinstance(d, list) and "class" not in d:
+        d.append("class")
+    elif isinstance(d, dict):
+        v = d.get("div", [])
+        if isinstance(v, list) and "class" not in v:
+            v.append("class")
+        elif isinstance(v, set) and "class" not in v:
+            v.add("class")
+        elif isinstance(v, str):
+            v = set(v.split(" "))
+            v.add("class")
+
+        d["div"] = v
+
+    if isinstance(block, blocks.StructBlock):
+        for _, b in block.child_blocks.items():
+            d = get_allowed_attributes(instance, b, d)
+
+    return d
+
 
 class WagtailBlockFeature(EditorJSFeature):
     def __init__(self, 
             tool_name: str,
             block: blocks.Block,
             klass: str = None,
             config: dict = None,
@@ -310,80 +359,52 @@
             allowed_attributes: dict[str, list[str]] = None,
             **kwargs
         ):
 
         if not isinstance(block, blocks.Block) and issubclass(block, blocks.Block):
             block = block()
 
+
         self.block = block
 
         self.block.set_name(
             self.block.__class__.__name__.lower()
         )
 
         super().__init__(
             tool_name, klass, None, None, None, config, weight, allowed_tags, allowed_attributes, **kwargs
         )
 
     def init_static(self, css, js):
         pass
 
+    def init_attrs(self, allowed_tags, allowed_attributes):
+        pass
+
     @cached_property
     def widget(self):
         return blocks.BlockWidget(self.block)
 
     def get_config(self, context: dict[str, Any] = None) -> dict:
         data = super().get_config(context)
         config = data.get("config", {})
         config["rendered"] = self.widget.render_with_errors(
             "__PREFIX__", self.block.get_default(),
         )
         data["config"] = config
         return data
     
     
-    @property
+    @cached_property
     def allowed_tags(self):
-        if hasattr(self.block, "allowed_tags"):
-            l = self.block.allowed_tags
-        elif hasattr(self.block.meta, "allowed_tags"):
-            l = self.block.meta.allowed_tags
-        else:
-            l = super().allowed_tags
-
-        l = l or []
+        return get_allowed_tags(self, self.block)
 
-        return list(set(list(l) + ["div"]))
-
-    @property
+    @cached_property
     def allowed_attributes(self):
-        if hasattr(self.block, "allowed_attributes"):
-            d = self.block.allowed_attributes
-        elif hasattr(self.block.meta, "allowed_attributes"):
-            d = self.block.meta.allowed_attributes
-        else:
-            d = super().allowed_attributes
-
-        d = d or {}
-        
-        if isinstance(d, list) and "class" not in d:
-            d.append("class")
-        elif isinstance(d, dict):
-            v = d.get("div", [])
-            if isinstance(v, list) and "class" not in v:
-                v.append("class")
-            elif isinstance(v, set) and "class" not in v:
-                v.add("class")
-            elif isinstance(v, str):
-                v = set(v.split(" "))
-                v.add("class")
-
-            d["div"] = v
-
-        return d
+        return get_allowed_attributes(self, self.block)
     
     @property
     def js(self):
         return [
             *self.widget.media._js,
             mark_safe(f"<script src=\"{ static('wagtail_editorjs/js/tools/wagtail-block.js') }\" data-name=\"{ self.block.name }\" data-title=\"{ self.block.label }\"></script>"),
         ]
@@ -435,21 +456,14 @@
 
     @css.setter
     def css(self, data: Any): pass
 
     @klass.setter
     def klass(self, data: Any): pass
 
-    @allowed_tags.setter
-    def allowed_tags(self, data: Any): pass
-
-    @allowed_attributes.setter
-    def allowed_attributes(self, data: Any): pass
-
-
     
 
 from wagtail.models import Page
 from wagtail.admin.widgets import AdminPageChooser
 
 
 class ButtonFeature(PageChooserURLsMixin, EditorJSFeature):
```

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/documents.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/documents.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/images.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/images.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/inlines.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/lists.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/lists.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/tunes.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/features/tunes.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/fields.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/forms.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         
         if isinstance(value, formfields.InvalidJSONInput):
             return value
         
         if not isinstance(value, dict):
             return value
         
-        value = EDITOR_JS_FEATURES.prepare_value(
+        value = EDITOR_JS_FEATURES.value_for_form(
             self.features, value
         )
 
         return super().prepare_value(value)
     
     def validate(self, value) -> None:
         super().validate(value)
```

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/__init__.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/attrs.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/element.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/element.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/utils.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/element/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/feature_registry.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/feature_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,18 +181,23 @@
             tunes = item.get("tunes", {})
             if tunes:
                 keys = list(tunes.keys())
                 for key in keys:
                     if key not in tools:
                         del tunes[key]
 
-            blocks[i] = self[block_type].value_for_form(item)
-
         data["blocks"] = list(filter(None, blocks))
         return data
+    
+    def value_for_form(self, tools: list[str], data: dict):
+        for i, item in enumerate(data["blocks"]):
+            block_type = item.get("type")
+            data["blocks"][i] = self[block_type].value_for_form(item)
+        return data
+
 
     def get_by_weight(self, tools: list[str]) -> OrderedDict[str, EditorJSFeature]:
         """
             Returns the tools sorted by weight.
             Items with the lowest weight are first.
         """
         self._look_for_features()
```

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/base.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,40 @@
         self.weight = weight
         self.include_template = include_template
 
         self.init_static(
             css, js,
         )
 
+        self.init_attrs(
+            allowed_tags, allowed_attributes,
+        )
+
+    def value_for_form(self, value: dict) -> dict:
+        """
+            Prepare the value for the feature.
+            This is useful for when you need to modify the data
+            before it is passed to the frontend.
+        """
+        return value
+
+    def init_static(self, css, js):
+        css = css or []
+        js = js or []
+
+        if self.css:
+            css.extend(self.css)
+
+        if self.js:
+            js.extend(self.js)
+            
+        self.js = js
+        self.css = css
+
+    def init_attrs(self, allowed_tags, allowed_attributes):
         if not isinstance(allowed_tags, (list, tuple, set)) and allowed_tags is not None:
             raise ValueError("allowed_tags must be a list, tuple or set")
         
         if not isinstance(allowed_attributes, dict) and allowed_attributes is not None:
             raise ValueError("allowed_attributes must be a dict")
 
         allowed_tags = allowed_tags or []
@@ -103,35 +129,14 @@
                     allowed_attributes[tag] = set(allowed_attributes.get(tag, []) + self.allowed_attributes)
             else:
                 raise ValueError("Invalid allowed attributes type, self.allowed_attributes must be dict or list")
 
         self.allowed_tags = set(allowed_tags)
         self.allowed_attributes = allowed_attributes
 
-    def value_for_form(self, value: dict) -> dict:
-        """
-            Prepare the value for the feature.
-            This is useful for when you need to modify the data
-            before it is passed to the frontend.
-        """
-        return value
-
-    def init_static(self, css, js):
-        css = css or []
-        js = js or []
-
-        if self.css:
-            css.extend(self.css)
-
-        if self.js:
-            js.extend(self.js)
-            
-        self.js = js
-        self.css = css
-
     def on_register(self, registry: "EditorJSFeatures"):
         """
             Called when the feature is registered.
             This can be used to say; register URLs
             required for this feature to work.
         """
         pass
```

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/basic.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/basic.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/inlines.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/snippets_inlines.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/snippets_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/view.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/features/view.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/value.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/registry/value.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/render.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/settings.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/editorjs.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/templatetags/editorjs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/base.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_attrs.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_blocks.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,39 @@
 from wagtail_editorjs.render import render_editorjs_html
 from wagtail_editorjs.registry import (
     EDITOR_JS_FEATURES,
 )
 
 from .base import BaseEditorJSTest
 
+class SubBlock(blocks.StructBlock):
+    sub_title = blocks.CharBlock()
+    sub_text = blocks.CharBlock()
+
+    class Meta:
+        allowed_tags = ["h3", "p"]
+        allowed_attributes = {
+            "h3": ["class"],
+            "p": ["class"],
+        }
 
 class TestWagtailBlockFeatureBlock(blocks.StructBlock):
     title = blocks.CharBlock()
-    text = blocks.CharBlock()
-    sub_block = blocks.StructBlock([
-        ("sub_title", blocks.CharBlock()),
-        ("sub_text", blocks.CharBlock()),
-    ])
+    subtitle = blocks.CharBlock()
+    sub_block = SubBlock()
 
     class Meta:
-        allowed_tags = ["h1", "h2", "p"]
+        allowed_tags = ["h1", "h2"]
+        allowed_attributes = {
+            "h1": ["class"],
+            "h2": ["class"],
+        }
 
     def render(self, value, context=None):
-        return f"<h1>{value['title']}</h1><p>{value['text']}</p><h2>{value['sub_block']['sub_title']}</h2><p>{value['sub_block']['sub_text']}</p>"
+        return f"<h1 class='test1'>{value['title']}</h1><h2 class='test2'>{value['subtitle']}</h2><h3 class='test3'>{value['sub_block']['sub_title']}</h3><p class='test4'>{value['sub_block']['sub_text']}</p>"
 
 
 class TestWagtailBlockFeature(BaseEditorJSTest):
 
     def setUp(self) -> None:
         super().setUp()
 
@@ -45,59 +56,59 @@
             self.feature,
         )
         
 
     def test_wagtail_block_feature(self):
         test_data = {
             "title": "Test Title",
-            "text": "Test Text",
+            "subtitle": "Test Text",
             "sub_block": {
                 "sub_title": "Sub Title",
                 "sub_text": "Sub Text",
             },
         }
 
         feature_value = {
             "type": "test_feature",
             "data": {
-                "__prefix__": "test_feature",
                 "block": test_data,
             }
         }
 
         editorjs_value = {
             "time": int(time.time()),
             "blocks": [feature_value],
             "version": "0.0.0",
         }
 
         html = render_editorjs_html(features=["test_feature"], data=editorjs_value)
         feature_html = str(self.feature.render_block_data(feature_value))
         
+        
         self.assertHTMLEqual(
             html,
             render_to_string(
                 "wagtail_editorjs/rich_text.html",
                 {"html": mark_safe(feature_html)}
             ),
         )
 
         self.assertInHTML(
-            "<h1>Test Title</h1>",
+            "<h1 class='test1'>Test Title</h1>",
             feature_html,
         )
 
         self.assertInHTML(
-            "<p>Test Text</p>",
+            "<h2 class='test2'>Test Text</h2>",
             feature_html,
         )
 
         self.assertInHTML(
-            "<h2>Sub Title</h2>",
+            "<h3 class='test3'>Sub Title</h3>",
             feature_html,
         )
 
         self.assertInHTML(
-            "<p>Sub Text</p>",
+            "<p class='test4'>Sub Text</p>",
             feature_html,
         )
```

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_inlines.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_render.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/core/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/manage.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/settings.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/urls.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/features.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/features.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/urls.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/PKG-INFO` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-editorjs
-Version: 1.6.5rc1
+Version: 1.6.5rc2
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/SOURCES.txt` & `wagtail_editorjs-1.6.5rc2/wagtail_editorjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

