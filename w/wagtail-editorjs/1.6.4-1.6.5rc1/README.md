# Comparing `tmp/wagtail_editorjs-1.6.4.tar.gz` & `tmp/wagtail_editorjs-1.6.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_editorjs-1.6.4.tar", last modified: Mon May 13 17:54:13 2024, max compression
+gzip compressed data, was "wagtail_editorjs-1.6.5rc1.tar", last modified: Mon May 13 23:37:04 2024, max compression
```

## Comparing `wagtail_editorjs-1.6.4.tar` & `wagtail_editorjs-1.6.5rc1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.157128 wagtail_editorjs-1.6.4/
--rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.4/LICENSE
--rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6666 2024-05-13 17:54:13.157128 wagtail_editorjs-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     5532 2024-05-13 16:18:48.000000 wagtail_editorjs-1.6.4/README.md
--rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.4/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2024-05-13 17:54:13.159154 wagtail_editorjs-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.916502 wagtail_editorjs-1.6.4/wagtail_editorjs/
--rw-rw-rw-   0        0        0      331 2024-05-13 17:54:10.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/__init__.py
--rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/apps.py
--rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/blocks.py
--rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/django_editor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.937425 wagtail_editorjs-1.6.4/wagtail_editorjs/features/
--rw-rw-rw-   0        0        0      668 2024-05-13 14:46:42.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/features/__init__.py
--rw-rw-rw-   0        0        0    15548 2024-05-13 17:39:24.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/features/blocks.py
--rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/features/documents.py
--rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/features/images.py
--rw-rw-rw-   0        0        0     7721 2024-05-01 07:39:27.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/features/inlines.py
--rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/features/lists.py
--rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/features/tunes.py
--rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/fields.py
--rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/forms.py
--rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.939426 wagtail_editorjs-1.6.4/wagtail_editorjs/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.940426 wagtail_editorjs-1.6.4/wagtail_editorjs/migrations/__pycache__/
--rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.945426 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/
--rw-rw-rw-   0        0        0      932 2024-05-13 14:22:20.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.966532 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/
--rw-rw-rw-   0        0        0      255 2024-05-13 14:22:16.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/__init__.py
--rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/attrs.py
--rw-rw-rw-   0        0        0     5110 2024-05-13 14:43:24.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/element.py
--rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/utils.py
--rw-rw-rw-   0        0        0     7265 2024-03-27 21:04:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/feature_registry.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.997851 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/
--rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/__init__.py
--rw-rw-rw-   0        0        0     7600 2024-05-13 15:20:31.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/base.py
--rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/basic.py
--rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/inlines.py
--rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/snippets_inlines.py
--rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/view.py
--rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/registry/value.py
--rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/render.py
--rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.877662 wagtail_editorjs-1.6.4/wagtail_editorjs/static/
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.880830 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.005499 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/css/
--rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
--rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.012548 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/
--rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
--rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
--rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.017552 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/init/
--rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
--rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.044396 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/
--rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.047912 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
--rw-rw-rw-   0        0        0     2661 2024-04-27 00:14:45.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
--rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
--rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
--rw-rw-rw-   0        0        0     3349 2024-05-13 17:36:51.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
--rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
--rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
--rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
--rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
--rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
--rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
--rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
--rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.883859 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.052945 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
--rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.101302 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
--rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
--rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
--rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
--rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
--rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
--rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
--rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
--rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
--rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
--rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
--rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
--rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
--rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
--rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
--rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
--rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
--rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
--rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
--rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
--rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
--rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
--rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.103302 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
--rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.110203 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
--rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
--rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.885101 wagtail_editorjs-1.6.4/wagtail_editorjs/templates/
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.113144 wagtail_editorjs-1.6.4/wagtail_editorjs/templates/wagtail_editorjs/
--rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.114932 wagtail_editorjs-1.6.4/wagtail_editorjs/templates/wagtail_editorjs/widgets/
--rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.118423 wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.121582 wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
--rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/editorjs.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.123202 wagtail_editorjs-1.6.4/wagtail_editorjs/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.129701 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/__init__.py
--rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.131297 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.141232 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/base.py
--rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_attrs.py
--rw-rw-rw-   0        0        0     2711 2024-05-13 17:36:20.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_inlines.py
--rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_render.py
--rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.150128 wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/settings.py
--rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/urls.py
--rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:13.156128 wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/
--rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/features.py
--rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-13 17:54:12.925082 wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/
--rw-rw-rw-   0        0        0     6666 2024-05-13 17:54:12.000000 wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6006 2024-05-13 17:54:12.000000 wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 17:54:12.000000 wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-13 17:54:12.000000 wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 17:54:12.000000 wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.665804 wagtail_editorjs-1.6.5rc1/
+-rw-rw-rw-   0        0        0    18429 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc1/LICENSE
+-rw-rw-rw-   0        0        0      272 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6784 2024-05-13 23:37:04.666802 wagtail_editorjs-1.6.5rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     5647 2024-05-13 23:33:57.000000 wagtail_editorjs-1.6.5rc1/README.md
+-rw-rw-rw-   0        0        0       90 2024-03-23 00:30:20.000000 wagtail_editorjs-1.6.5rc1/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-05-13 23:37:04.671348 wagtail_editorjs-1.6.5rc1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-27 00:40:18.000000 wagtail_editorjs-1.6.5rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.341616 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      334 2024-05-13 23:37:01.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/__init__.py
+-rw-rw-rw-   0        0        0      169 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/apps.py
+-rw-rw-rw-   0        0        0     1985 2024-03-29 17:31:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/blocks.py
+-rw-rw-rw-   0        0        0     2569 2024-04-08 19:06:41.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/django_editor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.370571 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/
+-rw-rw-rw-   0        0        0      668 2024-05-13 14:46:42.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/__init__.py
+-rw-rw-rw-   0        0        0    16033 2024-05-13 23:33:06.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/blocks.py
+-rw-rw-rw-   0        0        0     6818 2024-03-31 07:04:36.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/documents.py
+-rw-rw-rw-   0        0        0     9823 2024-04-16 19:24:08.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/images.py
+-rw-rw-rw-   0        0        0     7721 2024-05-01 07:39:27.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/inlines.py
+-rw-rw-rw-   0        0        0     5164 2024-03-27 20:40:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/lists.py
+-rw-rw-rw-   0        0        0     3983 2024-04-18 21:15:27.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/tunes.py
+-rw-rw-rw-   0        0        0     1785 2024-04-16 12:46:42.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/fields.py
+-rw-rw-rw-   0        0        0     6874 2024-04-26 08:34:08.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/forms.py
+-rw-rw-rw-   0        0        0      319 2024-03-27 21:25:26.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.373678 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.375693 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.381706 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/
+-rw-rw-rw-   0        0        0      932 2024-05-13 14:22:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.389963 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/
+-rw-rw-rw-   0        0        0      255 2024-05-13 14:22:16.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/__init__.py
+-rw-rw-rw-   0        0        0     2073 2024-03-28 19:01:37.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/attrs.py
+-rw-rw-rw-   0        0        0     5110 2024-05-13 14:43:24.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/element.py
+-rw-rw-rw-   0        0        0     1525 2024-03-27 14:19:36.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/utils.py
+-rw-rw-rw-   0        0        0     7337 2024-05-13 23:25:18.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/feature_registry.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.402732 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/
+-rw-rw-rw-   0        0        0      340 2024-04-18 21:14:51.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/__init__.py
+-rw-rw-rw-   0        0        0     7865 2024-05-13 23:22:22.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/base.py
+-rw-rw-rw-   0        0        0     2235 2024-04-18 09:40:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/basic.py
+-rw-rw-rw-   0        0        0     8877 2024-04-26 13:03:15.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/inlines.py
+-rw-rw-rw-   0        0        0      674 2024-04-18 21:56:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/snippets_inlines.py
+-rw-rw-rw-   0        0        0     1258 2024-03-27 20:13:06.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/view.py
+-rw-rw-rw-   0        0        0     3311 2024-04-16 12:34:49.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/value.py
+-rw-rw-rw-   0        0        0     5353 2024-04-18 10:11:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/render.py
+-rw-rw-rw-   0        0        0     1042 2024-04-08 19:04:03.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.288914 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.295065 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.408735 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/
+-rw-rw-rw-   0        0        0    10098 2024-04-26 12:36:15.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css
+-rw-rw-rw-   0        0        0    14154 2024-04-26 13:11:26.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.415902 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/
+-rw-rw-rw-   0        0        0     1371 2024-03-29 17:29:46.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js
+-rw-rw-rw-   0        0        0     1155 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js
+-rw-rw-rw-   0        0        0     2913 2024-04-26 11:54:42.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.421161 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/
+-rw-rw-rw-   0        0        0       86 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/drag-drop.js
+-rw-rw-rw-   0        0        0       94 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/init/undo-redo.js
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.455873 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/
+-rw-rw-rw-   0        0        0      364 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/attaches.js
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.462850 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/
+-rw-rw-rw-   0        0        0     2661 2024-04-27 00:14:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js
+-rw-rw-rw-   0        0        0     4464 2024-04-26 12:37:59.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js
+-rw-rw-rw-   0        0        0    12378 2024-04-18 09:49:54.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js
+-rw-rw-rw-   0        0        0     3876 2024-05-13 23:22:09.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js
+-rw-rw-rw-   0        0        0     5510 2024-04-18 21:24:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js
+-rw-rw-rw-   0        0        0     3595 2024-04-26 10:29:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js
+-rw-rw-rw-   0        0        0    11260 2024-04-18 09:47:53.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js
+-rw-rw-rw-   0        0        0     3277 2024-03-26 20:38:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js
+-rw-rw-rw-   0        0        0     7883 2024-04-18 08:43:02.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js
+-rw-rw-rw-   0        0        0    16447 2024-04-18 09:47:21.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js
+-rw-rw-rw-   0        0        0     4197 2024-04-26 12:35:50.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js
+-rw-rw-rw-   0        0        0     6225 2024-04-18 22:11:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.298807 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.470601 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/
+-rw-rw-rw-   0        0        0   208234 2024-03-28 10:17:35.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.561082 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/
+-rw-rw-rw-   0        0        0    34797 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js
+-rw-rw-rw-   0        0        0     7233 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js
+-rw-rw-rw-   0        0        0     3222 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js
+-rw-rw-rw-   0        0        0     1864 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js
+-rw-rw-rw-   0        0        0    10151 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js
+-rw-rw-rw-   0        0        0     6946 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js
+-rw-rw-rw-   0        0        0    29531 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js
+-rw-rw-rw-   0        0        0     2440 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js
+-rw-rw-rw-   0        0        0    33560 2024-03-27 17:16:55.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js
+-rw-rw-rw-   0        0        0    30466 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js
+-rw-rw-rw-   0        0        0     2550 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js
+-rw-rw-rw-   0        0        0    10575 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js
+-rw-rw-rw-   0        0        0     3142 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js
+-rw-rw-rw-   0        0        0     5481 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js
+-rw-rw-rw-   0        0        0     3198 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js
+-rw-rw-rw-   0        0        0    23954 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js
+-rw-rw-rw-   0        0        0     9463 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js
+-rw-rw-rw-   0        0        0     9644 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js
+-rw-rw-rw-   0        0        0     8007 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js
+-rw-rw-rw-   0        0        0    19237 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js
+-rw-rw-rw-   0        0        0     3713 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js
+-rw-rw-rw-   0        0        0    20734 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.567087 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/
+-rw-rw-rw-   0        0        0    44137 2024-04-16 19:19:37.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.579966 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE
+-rw-rw-rw-   0        0        0    20122 2024-04-23 14:51:23.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js
+-rw-rw-rw-   0        0        0    25717 2024-04-23 14:51:31.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.301865 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.583981 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/
+-rw-rw-rw-   0        0        0      123 2024-03-29 14:30:09.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/rich_text.html
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.586979 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/
+-rw-rw-rw-   0        0        0      555 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.592555 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-26 20:17:19.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.598516 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2024-03-28 09:30:45.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2309 2024-04-25 19:47:38.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1497 2024-04-25 19:47:36.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/editorjs.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.604068 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.609596 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/__init__.py
+-rw-rw-rw-   0        0        0      168 2024-04-08 18:30:48.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.612607 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.633541 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-26 23:51:58.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     2310 2024-04-08 19:05:43.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/base.py
+-rw-rw-rw-   0        0        0     2585 2024-04-08 18:38:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_attrs.py
+-rw-rw-rw-   0        0        0     2711 2024-05-13 17:36:20.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 18:42:47.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_inlines.py
+-rw-rw-rw-   0        0        0     5862 2024-04-08 18:58:38.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_render.py
+-rw-rw-rw-   0        0        0      707 2024-04-08 18:29:14.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.649798 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3826 2024-04-08 19:17:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/settings.py
+-rw-rw-rw-   0        0        0     1176 2024-04-08 18:42:23.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      429 2024-04-08 18:29:49.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.662799 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/
+-rw-rw-rw-   0        0        0       74 2024-04-16 12:19:31.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     7364 2024-04-26 09:19:37.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/features.py
+-rw-rw-rw-   0        0        0      646 2024-03-27 20:14:22.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0      777 2024-04-16 12:19:25.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-13 23:37:04.353846 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/
+-rw-rw-rw-   0        0        0     6784 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6006 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-13 23:37:04.000000 wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/top_level.txt
```

### Comparing `wagtail_editorjs-1.6.4/LICENSE` & `wagtail_editorjs-1.6.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/PKG-INFO` & `wagtail_editorjs-1.6.5rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_editorjs
-Version: 1.6.4
+Version: 1.6.5rc1
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -138,22 +138,23 @@
    dict_keys([... all registered features ...])
    ```
 
 ##  Register a Wagtail block as a feature
 
 It is also possible to register a Wagtail block as a feature.
 
-This may be a `Fieldblock` (like `Charblock`, or `TextBlock`), or a `StructBlock`.
+It is important to note that the block must be a `StructBlock` or a subclass of `StructBlock`.
 
 It is **not** allowed to be or include:
 
-* A `StreamBlock`
-* A `ListBlock`
-* Any type of `ChooserBlock`
-* A `RichTextBlock`
+* A `StreamBlock` (mainly due to styling issues)
+* A `ListBlock` (mainly due to styling issues)
+* A `RichTextBlock` (cannot initialize)
+
+*Help with these issues is highly appreciated!*
 
 Example:
 
 ```python
 from wagtail import hooks
 from wagtail_editorjs.features import (
     WagtailBlockFeature,
```

### Comparing `wagtail_editorjs-1.6.4/README.md` & `wagtail_editorjs-1.6.5rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -110,22 +110,23 @@
    dict_keys([... all registered features ...])
    ```
 
 ##  Register a Wagtail block as a feature
 
 It is also possible to register a Wagtail block as a feature.
 
-This may be a `Fieldblock` (like `Charblock`, or `TextBlock`), or a `StructBlock`.
+It is important to note that the block must be a `StructBlock` or a subclass of `StructBlock`.
 
 It is **not** allowed to be or include:
 
-* A `StreamBlock`
-* A `ListBlock`
-* Any type of `ChooserBlock`
-* A `RichTextBlock`
+* A `StreamBlock` (mainly due to styling issues)
+* A `ListBlock` (mainly due to styling issues)
+* A `RichTextBlock` (cannot initialize)
+
+*Help with these issues is highly appreciated!*
 
 Example:
 
 ```python
 from wagtail import hooks
 from wagtail_editorjs.features import (
     WagtailBlockFeature,
```

### Comparing `wagtail_editorjs-1.6.4/setup.cfg` & `wagtail_editorjs-1.6.5rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f65 6469 746f   = wagtail_edito
 00000020: 726a 730d 0a76 6572 7369 6f6e 203d 2031  rjs..version = 1
-00000030: 2e36 2e34 0d0a 6465 7363 7269 7074 696f  .6.4..descriptio
-00000040: 6e20 3d20 4564 6974 6f72 4a53 2061 7320  n = EditorJS as 
-00000050: 6120 7769 6467 6574 2066 6f72 2057 6167  a widget for Wag
-00000060: 7461 696c 2c20 7769 7468 2050 6167 652d  tail, with Page-
-00000070: 2061 6e64 2049 6d61 6765 2063 686f 6f73   and Image choos
-00000080: 6572 2073 7570 706f 7274 0d0a 6c6f 6e67  er support..long
-00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000a0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000c0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000d0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
-000000e0: 7574 686f 7220 3d20 4e69 6765 6c0d 0a61  uthor = Nigel..a
-000000f0: 7574 686f 725f 656d 6169 6c20 3d20 6e69  uthor_email = ni
-00000100: 6765 6c40 676f 6f64 6164 7669 6365 2e69  gel@goodadvice.i
-00000110: 740d 0a75 726c 203d 2068 7474 7073 3a2f  t..url = https:/
-00000120: 2f67 6974 6875 622e 636f 6d2f 4e69 6765  /github.com/Nige
-00000130: 6c32 3339 322f 7761 6774 6169 6c5f 6564  l2392/wagtail_ed
-00000140: 6974 6f72 6a73 0d0a 6c69 6365 6e73 6520  itorjs..license 
-00000150: 3d20 4750 4c2d 332e 302d 6f6e 6c79 0d0a  = GPL-3.0-only..
-00000160: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000170: 0945 6e76 6972 6f6e 6d65 6e74 203a 3a20  .Environment :: 
-00000180: 5765 6220 456e 7669 726f 6e6d 656e 740d  Web Environment.
-00000190: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-000001a0: 6a61 6e67 6f0d 0a09 4672 616d 6577 6f72  jango...Framewor
-000001b0: 6b20 3a3a 2044 6a61 6e67 6f20 3a3a 2034  k :: Django :: 4
-000001c0: 2e32 0d0a 0946 7261 6d65 776f 726b 203a  .2...Framework :
-000001d0: 3a20 5761 6774 6169 6c0d 0a09 4672 616d  : Wagtail...Fram
-000001e0: 6577 6f72 6b20 3a3a 2057 6167 7461 696c  ework :: Wagtail
-000001f0: 203a 3a20 350d 0a09 4672 616d 6577 6f72   :: 5...Framewor
-00000200: 6b20 3a3a 2057 6167 7461 696c 203a 3a20  k :: Wagtail :: 
-00000210: 360d 0a09 496e 7465 6e64 6564 2041 7564  6...Intended Aud
-00000220: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-00000230: 6572 730d 0a09 4c69 6365 6e73 6520 3a3a  ers...License ::
-00000240: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000250: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
-00000260: 6c69 6320 4c69 6365 6e73 6520 7633 206f  lic License v3 o
-00000270: 7220 6c61 7465 7220 2847 504c 7633 2b29  r later (GPLv3+)
-00000280: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000290: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000002a0: 6e64 656e 740d 0a09 5072 6f67 7261 6d6d  ndent...Programm
-000002b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002c0: 5079 7468 6f6e 0d0a 0950 726f 6772 616d  Python...Program
-000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002e0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-000002f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000300: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000310: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
-00000320: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000330: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000340: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-00000350: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000360: 686f 6e20 3a3a 2033 2e39 0d0a 0954 6f70  hon :: 3.9...Top
-00000370: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000380: 3a20 5757 572f 4854 5450 0d0a 0954 6f70  : WWW/HTTP...Top
-00000390: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-000003a0: 3a20 5757 572f 4854 5450 203a 3a20 4479  : WWW/HTTP :: Dy
-000003b0: 6e61 6d69 6320 436f 6e74 656e 740d 0a0d  namic Content...
-000003c0: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 636c  .[options]..incl
-000003d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-000003e0: 203d 2074 7275 650d 0a70 6163 6b61 6765   = true..package
-000003f0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000400: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000410: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
-00000420: 6972 6573 203d 200d 0a09 446a 616e 676f  ires = ...Django
-00000430: 203e 3d20 342e 320d 0a09 5761 6774 6169   >= 4.2...Wagtai
-00000440: 6c20 3e3d 2035 2e30 0d0a 0962 6561 7574  l >= 5.0...beaut
-00000450: 6966 756c 736f 7570 3420 3e3d 2034 2e39  ifulsoup4 >= 4.9
-00000460: 2e33 0d0a 0962 6c65 6163 6820 3e3d 2036  .3...bleach >= 6
-00000470: 2e30 2e30 0d0a 0d0a 5b65 6767 5f69 6e66  .0.0....[egg_inf
-00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000004a0: 0d0a                                     ..
+00000030: 2e36 2e35 7263 310d 0a64 6573 6372 6970  .6.5rc1..descrip
+00000040: 7469 6f6e 203d 2045 6469 746f 724a 5320  tion = EditorJS 
+00000050: 6173 2061 2077 6964 6765 7420 666f 7220  as a widget for 
+00000060: 5761 6774 6169 6c2c 2077 6974 6820 5061  Wagtail, with Pa
+00000070: 6765 2d20 616e 6420 496d 6167 6520 6368  ge- and Image ch
+00000080: 6f6f 7365 7220 7375 7070 6f72 740d 0a6c  ooser support..l
+00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+000000b0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+000000c0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+000000d0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+000000e0: 0d0a 6175 7468 6f72 203d 204e 6967 656c  ..author = Nigel
+000000f0: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000100: 206e 6967 656c 4067 6f6f 6461 6476 6963   nigel@goodadvic
+00000110: 652e 6974 0d0a 7572 6c20 3d20 6874 7470  e.it..url = http
+00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
+00000130: 6967 656c 3233 3932 2f77 6167 7461 696c  igel2392/wagtail
+00000140: 5f65 6469 746f 726a 730d 0a6c 6963 656e  _editorjs..licen
+00000150: 7365 203d 2047 504c 2d33 2e30 2d6f 6e6c  se = GPL-3.0-onl
+00000160: 790d 0a63 6c61 7373 6966 6965 7273 203d  y..classifiers =
+00000170: 200d 0a09 456e 7669 726f 6e6d 656e 7420   ...Environment 
+00000180: 3a3a 2057 6562 2045 6e76 6972 6f6e 6d65  :: Web Environme
+00000190: 6e74 0d0a 0946 7261 6d65 776f 726b 203a  nt...Framework :
+000001a0: 3a20 446a 616e 676f 0d0a 0946 7261 6d65  : Django...Frame
+000001b0: 776f 726b 203a 3a20 446a 616e 676f 203a  work :: Django :
+000001c0: 3a20 342e 320d 0a09 4672 616d 6577 6f72  : 4.2...Framewor
+000001d0: 6b20 3a3a 2057 6167 7461 696c 0d0a 0946  k :: Wagtail...F
+000001e0: 7261 6d65 776f 726b 203a 3a20 5761 6774  ramework :: Wagt
+000001f0: 6169 6c20 3a3a 2035 0d0a 0946 7261 6d65  ail :: 5...Frame
+00000200: 776f 726b 203a 3a20 5761 6774 6169 6c20  work :: Wagtail 
+00000210: 3a3a 2036 0d0a 0949 6e74 656e 6465 6420  :: 6...Intended 
+00000220: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000230: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
+00000240: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000250: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+00000260: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+00000270: 3320 6f72 206c 6174 6572 2028 4750 4c76  3 or later (GPLv
+00000280: 332b 290d 0a09 4f70 6572 6174 696e 6720  3+)...Operating 
+00000290: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000002a0: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
+000002b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002c0: 3a3a 2050 7974 686f 6e0d 0a09 5072 6f67  :: Python...Prog
+000002d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002e0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+000002f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000300: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000310: 203a 3a20 3320 3a3a 204f 6e6c 790d 0a09   :: 3 :: Only...
+00000320: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000330: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000340: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+00000350: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000360: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+00000370: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+00000380: 7420 3a3a 2057 5757 2f48 5454 500d 0a09  t :: WWW/HTTP...
+00000390: 546f 7069 6320 3a3a 2049 6e74 6572 6e65  Topic :: Interne
+000003a0: 7420 3a3a 2057 5757 2f48 5454 5020 3a3a  t :: WWW/HTTP ::
+000003b0: 2044 796e 616d 6963 2043 6f6e 7465 6e74   Dynamic Content
+000003c0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
+000003d0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+000003e0: 6174 6120 3d20 7472 7565 0d0a 7061 636b  ata = true..pack
+000003f0: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000400: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000410: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
+00000420: 6571 7569 7265 7320 3d20 0d0a 0944 6a61  equires = ...Dja
+00000430: 6e67 6f20 3e3d 2034 2e32 0d0a 0957 6167  ngo >= 4.2...Wag
+00000440: 7461 696c 203e 3d20 352e 300d 0a09 6265  tail >= 5.0...be
+00000450: 6175 7469 6675 6c73 6f75 7034 203e 3d20  autifulsoup4 >= 
+00000460: 342e 392e 330d 0a09 626c 6561 6368 203e  4.9.3...bleach >
+00000470: 3d20 362e 302e 300d 0a0d 0a5b 6567 675f  = 6.0.0....[egg_
+00000480: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000490: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000004a0: 300d 0a0d 0a                             0....
```

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/blocks.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/django_editor.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/django_editor.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/features/__init__.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/features/blocks.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -310,17 +310,14 @@
             allowed_attributes: dict[str, list[str]] = None,
             **kwargs
         ):
 
         if not isinstance(block, blocks.Block) and issubclass(block, blocks.Block):
             block = block()
 
-        if not isinstance(block, (blocks.StructBlock, blocks.FieldBlock)):
-            raise TypeError("block must be an instance of EditorJSFeatureStructBlock or FieldBlock")
-
         self.block = block
 
         self.block.set_name(
             self.block.__class__.__name__.lower()
         )
 
         super().__init__(
@@ -393,17 +390,33 @@
     
     def validate(self, data: Any):
         super().validate(data)
 
         if "block" not in data["data"]:
             raise forms.ValidationError("Invalid block value")
         
-        self.block.clean(
-            data["data"]["block"],
+        try:
+            data["data"]["block"] = self.block.get_prep_value(
+                self.block.clean(self.block.to_python(data["data"]["block"]))
+            )
+        except blocks.StreamBlockValidationError as e:
+            raise e
+        except blocks.list_block.ListBlockValidationError as e:
+            raise e
+        except blocks.struct_block.StructBlockValidationError as e:
+            raise e
+        except Exception as e:
+            raise e
+        
+    def value_for_form(self, value: dict) -> dict:
+        value = super().value_for_form(value)
+        value["data"]["block"] = self.block.get_form_state(
+            self.block.to_python(value["data"]["block"])
         )
+        return value
     
     def render_block_data(self, block: EditorJSBlock, context=None) -> EditorJSElement:
         value: blocks.StructValue = self.block.to_python(block["data"]["block"])
         return EditorJSSoupElement(f"<div class=\"{self.tool_name}\">{ self.block.render(value) }</div>")
     
     @classmethod
     def get_test_data(cls):
```

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/features/documents.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/documents.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/features/images.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/images.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/features/inlines.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/features/lists.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/lists.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/features/tunes.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/features/tunes.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/fields.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/forms.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/__init__.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/attrs.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/element.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/element.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/element/utils.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/element/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/feature_registry.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/feature_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             tunes = item.get("tunes", {})
             if tunes:
                 keys = list(tunes.keys())
                 for key in keys:
                     if key not in tools:
                         del tunes[key]
 
-            blocks[i] = item
+            blocks[i] = self[block_type].value_for_form(item)
 
         data["blocks"] = list(filter(None, blocks))
         return data
 
     def get_by_weight(self, tools: list[str]) -> OrderedDict[str, EditorJSFeature]:
         """
             Returns the tools sorted by weight.
@@ -228,11 +228,13 @@
                     if tune:
                         tool_mapping.validate(tune)
 
                 else:
                     if item["type"] == tool:
                         tool_mapping.validate(item)
 
+        data["blocks"] = block_list
+
         return data
```

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/base.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,22 @@
                     allowed_attributes[tag] = set(allowed_attributes.get(tag, []) + self.allowed_attributes)
             else:
                 raise ValueError("Invalid allowed attributes type, self.allowed_attributes must be dict or list")
 
         self.allowed_tags = set(allowed_tags)
         self.allowed_attributes = allowed_attributes
 
+    def value_for_form(self, value: dict) -> dict:
+        """
+            Prepare the value for the feature.
+            This is useful for when you need to modify the data
+            before it is passed to the frontend.
+        """
+        return value
+
     def init_static(self, css, js):
         css = css or []
         js = js or []
 
         if self.css:
             css.extend(self.css)
```

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/basic.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/basic.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/inlines.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/snippets_inlines.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/snippets_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/features/view.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/features/view.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/registry/value.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/registry/value.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/render.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/settings.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/editorjs-widget.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-block.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget-controller.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/editorjs-widget.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/tooltips/wagtail-tooltips.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-block.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -55,47 +55,58 @@
                 this.blockPrefix,
             );
 
             this.wrapperElement.innerHTML = html;
 
             const element = this.wrapperElement.querySelector(`#${this.blockPrefix}`);
             const id = element.id;
-
+            //
             if (!window.telepath) {
                 console.error('Telepath is not defined');
                 return;
             }
-
+            //
             // const dataValue = JSON.parse(element.getAttribute('data-w-block-data-value'));
             // const argumentsValue = JSON.parse(element.getAttribute('data-w-block-arguments-value'));
+            if (element.dataset.controller) {
+                delete element.dataset.controller;
+            }
             const dataValue = JSON.parse(element.dataset.wBlockDataValue);
             const argumentsValue = JSON.parse(element.dataset.wBlockArgumentsValue);
             this.blockDef = telepath.unpack(dataValue);
 
-            this.block = this.blockDef.render(
-                element, id, ...argumentsValue,
-            )
-
-            if (this.data) {
-                this.block.setState(this.data["block"]);
-            }
+            this.wrapperElement.addEventListener('DOMNodeInserted', (e) => {
+                if (!(e.relatedNode.firstElementChild == this.wrapperElement)) {
+                    return;
+                }
+
+                // Wait for the element block to be rendered by the browser
+                setTimeout(() => {
+                    this.block = this.blockDef.render(
+                        element, id, ...argumentsValue,
+                    )
+                    if (this.data) {
+                        this.block.setState(this.data["block"]);
+                    }
+                }, 0);
+            });
 
             return super.render();
         }
 
         validate(savedData) {
             return true;
         }
 
         save(blockContent) {
             this.data = super.save(blockContent);
             if (!this.block.getState) {
                 console.error('Block does not have a getState method', this.block)
             } else {
-                this.data["block"] = this.block.getState();
+                this.data["block"] = this.block.getValue();
             }
             return this.data || {};
         }
     }
 
     window[`WagtailBlockTool_${blockName}`] = WagtailBlockTool;
```

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-button-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-chooser-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-color-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-document.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image-row.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-inline-tool.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/js/tools/wagtail-link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/editorjs.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/attaches.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/checklist.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/delimiter.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/drag-drop.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/header.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/image.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/inline-code.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link-autocomplete.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/link.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/marker.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/nested-list.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/paragraph.umd.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/quote.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/raw.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/table.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-alignment.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/text-variant-tune.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/underline.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/undo-redo.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/tools/warning.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/editorjs/vendor.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/sortable/sortable.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/popper.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/static/wagtail_editorjs/vendor/tippy/tippy-bundle.min.js`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templates/wagtail_editorjs/widgets/editorjs.html`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/__pycache__/editorjs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/templatetags/editorjs.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/templatetags/editorjs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/base.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_attrs.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_blocks.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_inlines.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_inlines.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/core/tests/test_render.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/core/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/manage.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/settings.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/test/testapp/urls.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/features.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/features.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/urls.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs/wagtail_hooks/wagtail_fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/PKG-INFO` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-editorjs
-Version: 1.6.4
+Version: 1.6.5rc1
 Summary: EditorJS as a widget for Wagtail, with Page- and Image chooser support
 Home-page: https://github.com/Nigel2392/wagtail_editorjs
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -138,22 +138,23 @@
    dict_keys([... all registered features ...])
    ```
 
 ##  Register a Wagtail block as a feature
 
 It is also possible to register a Wagtail block as a feature.
 
-This may be a `Fieldblock` (like `Charblock`, or `TextBlock`), or a `StructBlock`.
+It is important to note that the block must be a `StructBlock` or a subclass of `StructBlock`.
 
 It is **not** allowed to be or include:
 
-* A `StreamBlock`
-* A `ListBlock`
-* Any type of `ChooserBlock`
-* A `RichTextBlock`
+* A `StreamBlock` (mainly due to styling issues)
+* A `ListBlock` (mainly due to styling issues)
+* A `RichTextBlock` (cannot initialize)
+
+*Help with these issues is highly appreciated!*
 
 Example:
 
 ```python
 from wagtail import hooks
 from wagtail_editorjs.features import (
     WagtailBlockFeature,
```

### Comparing `wagtail_editorjs-1.6.4/wagtail_editorjs.egg-info/SOURCES.txt` & `wagtail_editorjs-1.6.5rc1/wagtail_editorjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

