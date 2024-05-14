# Comparing `tmp/meetlify-0.1.3.tar.gz` & `tmp/meetlify-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetlify-0.1.3.tar", last modified: Mon May 13 00:52:47 2024, max compression
+gzip compressed data, was "meetlify-0.1.4.tar", last modified: Tue May 14 00:41:15 2024, max compression
```

## Comparing `meetlify-0.1.3.tar` & `meetlify-0.1.4.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:47.020125 meetlify-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-13 00:52:34.000000 meetlify-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-13 00:52:34.000000 meetlify-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-13 00:52:47.020125 meetlify-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-13 00:52:34.000000 meetlify-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 00:52:34.000000 meetlify-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 00:52:47.020125 meetlify-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-13 00:52:34.000000 meetlify-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.988125 meetlify-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.992125 meetlify-0.1.3/src/meetlify/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/meetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.992125 meetlify-0.1.3/src/meetlify/share/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/configs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.988125 meetlify-0.1.3/src/meetlify/share/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.992125 meetlify-0.1.3/src/meetlify/share/content/images/
--rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/images/fatureimage.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.996125 meetlify-0.1.3/src/meetlify/share/content/meetups/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/meetups/0001.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/meetups/0002.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/meetups/0003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.996125 meetlify-0.1.3/src/meetlify/share/content/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/pages/contact.md
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/pages/home.md
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/pages/privacy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/content/pages/terms.md
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/share/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.988125 meetlify-0.1.3/src/meetlify/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.988125 meetlify-0.1.3/src/meetlify/themes/lindau/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.988125 meetlify-0.1.3/src/meetlify/themes/lindau/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:46.996125 meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/about.png
--rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/author.png
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:47.008125 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:47.008125 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   237143 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:47.016125 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/static/js/scripts.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:47.016125 meetlify-0.1.3/src/meetlify/themes/lindau/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/templates/meetup.html
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/templates/meetups.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/themes/lindau/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-13 00:52:34.000000 meetlify-0.1.3/src/meetlify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:47.016125 meetlify-0.1.3/src/meetlify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-05-13 00:52:46.000000 meetlify-0.1.3/src/meetlify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-13 00:52:46.000000 meetlify-0.1.3/src/meetlify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:52:46.000000 meetlify-0.1.3/src/meetlify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 00:52:46.000000 meetlify-0.1.3/src/meetlify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:52:46.000000 meetlify-0.1.3/src/meetlify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 00:52:46.000000 meetlify-0.1.3/src/meetlify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 00:52:46.000000 meetlify-0.1.3/src/meetlify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:52:47.016125 meetlify-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-13 00:52:34.000000 meetlify-0.1.3/tests/test_meetups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 00:41:04.000000 meetlify-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 00:41:04.000000 meetlify-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-14 00:41:15.655336 meetlify-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-14 00:41:04.000000 meetlify-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 00:41:04.000000 meetlify-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 00:41:15.655336 meetlify-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-14 00:41:04.000000 meetlify-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.627336 meetlify-0.1.4/src/meetlify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/meetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/configs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/share/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/content/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/images/fatureimage.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/content/meetups/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/meetups/0001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/meetups/0002.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/meetups/0003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/content/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/contact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/privacy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/terms.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/themes/lindau/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/themes/lindau/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/author.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.647336 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/cookiealert.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.647336 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   238335 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.651336 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/cookiealert.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/scripts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/src/meetlify/themes/lindau/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetups.html
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/src/meetlify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-14 00:41:04.000000 meetlify-0.1.4/tests/test_meetups.py
```

### Comparing `meetlify-0.1.3/LICENSE` & `meetlify-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/PKG-INFO` & `meetlify-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.3.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.4.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -37,14 +37,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: markdown
 Requires-Dist: Jinja2
+Requires-Dist: python-slugify
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: python-language-server[all]; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -54,24 +55,24 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
 Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: setuptools; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: black; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
 Requires-Dist: mkdocstrings[python]; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
+Requires-Dist: wheel; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -90,17 +91,17 @@
 
 ### Using Command Line Interface (CLI)
 
 Create an empty folder on your computer or move to a desired location where you want to create the Meetup Website. 
 
 1. Now execute ``meetlify init`` which will crate an empty configuration file (JSON) in the folder. Feel free to edit it as per your need. Content of the configuration file are self explanatory.  
 
-2. Now execute ```meetlify setup`` which will setup the all folders as per your configurations. 
+2. Now execute ``meetlify setup`` which will setup the all folders as per your configurations. 
 
-3. Now execute ```meetlify make`` which will generate full website in output folder.
+3. Now execute ``meetlify make`` which will generate full website in output folder.
 
 
 ### Using Application Programming Interface (API)
 
 You can embed ```meetilify`` into your existing workflow easily. Here is a sample snippet.
 
 ```python
```

### Comparing `meetlify-0.1.3/README.md` & `meetlify-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 ### Using Command Line Interface (CLI)
 
 Create an empty folder on your computer or move to a desired location where you want to create the Meetup Website. 
 
 1. Now execute ``meetlify init`` which will crate an empty configuration file (JSON) in the folder. Feel free to edit it as per your need. Content of the configuration file are self explanatory.  
 
-2. Now execute ```meetlify setup`` which will setup the all folders as per your configurations. 
+2. Now execute ``meetlify setup`` which will setup the all folders as per your configurations. 
 
-3. Now execute ```meetlify make`` which will generate full website in output folder.
+3. Now execute ``meetlify make`` which will generate full website in output folder.
 
 
 ### Using Application Programming Interface (API)
 
 You can embed ```meetilify`` into your existing workflow easily. Here is a sample snippet.
 
 ```python
```

### Comparing `meetlify-0.1.3/setup.py` & `meetlify-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     % __version__,
     license="MIT",
     keywords=["meetups", "static-site-generators", "seo", "python"],
     scripts=[],
     include_package_data=True,
     python_requires=">=3.{MINOR:d}".format(MINOR=python_minor_min),
     setup_requires=[],
-    install_requires=["click", "markdown", "Jinja2"],
+    install_requires=["click", "markdown", "Jinja2", "python-slugify"],
     extras_require=extras_require,
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "meetlify = meetlify.cli:main",
         ],
     },
```

### Comparing `meetlify-0.1.3/src/meetlify/__init__.py` & `meetlify-0.1.4/src/meetlify/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/api.py` & `meetlify-0.1.4/src/meetlify/api.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/cli.py` & `meetlify-0.1.4/src/meetlify/cli.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/configs.py` & `meetlify-0.1.4/src/meetlify/configs.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/constants.py` & `meetlify-0.1.4/src/meetlify/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,10 +33,10 @@
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # DATABASE/CONSTANTS LIST
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
-VERSION_REVISION = 3
+VERSION_REVISION = 4
 
 FULL_VERSION = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_REVISION}"
```

### Comparing `meetlify-0.1.3/src/meetlify/meetup.py` & `meetlify-0.1.4/src/meetlify/meetup.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import markdown
+from slugify import slugify
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
@@ -75,19 +76,27 @@
 
         Returns:
             Meetup: Return Constructed Meetup Object
         """
         _md = markdown.Markdown(extensions=["meta", "attr_list"])
         with codecs.open(meetup_, "r", encoding="utf-8") as f:
             data = f.read()
+            content_ = _md.convert(data)
+
+            slug_ = (
+                "".join(_md.Meta["slug"])
+                if _md.Meta.get("slug")
+                else slugify("".join(_md.Meta["title"]))
+            )
+
             return cls(
-                content=_md.convert(data),
+                content=content_,
                 id="".join(_md.Meta["id"]),
                 date="".join(_md.Meta["date"]),
                 author="".join(_md.Meta["author"]),
                 title="".join(_md.Meta["title"]),
                 description="".join(_md.Meta["description"]),
-                slug="".join(_md.Meta["slug"]),
+                slug=slug_,
                 featureimage="".join(_md.Meta["featureimage"]),
                 address="".join(_md.Meta["address"]),
                 status="".join(_md.Meta["status"]),
             )
```

### Comparing `meetlify-0.1.3/src/meetlify/page.py` & `meetlify-0.1.4/src/meetlify/page.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/__init__.py` & `meetlify-0.1.4/src/meetlify/share/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/configs.json` & `meetlify-0.1.4/src/meetlify/share/configs.json`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/images/fatureimage.png` & `meetlify-0.1.4/src/meetlify/share/content/images/fatureimage.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/meetups/0001.md` & `meetlify-0.1.4/src/meetlify/share/content/meetups/0001.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/meetups/0002.md` & `meetlify-0.1.4/src/meetlify/share/content/meetups/0002.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/meetups/0003.md` & `meetlify-0.1.4/src/meetlify/share/content/meetups/0003.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/pages/contact.md` & `meetlify-0.1.4/src/meetlify/share/content/pages/contact.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/pages/home.md` & `meetlify-0.1.4/src/meetlify/share/content/pages/home.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/pages/privacy.md` & `meetlify-0.1.4/src/meetlify/share/content/pages/privacy.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/share/content/pages/terms.md` & `meetlify-0.1.4/src/meetlify/share/content/pages/terms.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/about.png` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/about.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/author.png` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/author.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/banner.png` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/banner.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/favicon.png` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/assets/logo.png` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/logo.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-icons.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/css/styles.css` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/styles.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 @charset "UTF-8";
+
 /*!
 * Start Bootstrap - Modern Business v5.0.7 (https://startbootstrap.com/template-overviews/modern-business)
 * Copyright 2013-2023 Start Bootstrap
 * Licensed under MIT (https://github.com/StartBootstrap/startbootstrap-modern-business/blob/master/LICENSE)
 */
 /*!
  * Bootstrap  v5.2.3 (https://getbootstrap.com/)
@@ -108,76 +109,105 @@
   margin: 1rem 0;
   color: inherit;
   border: 0;
   border-top: 1px solid;
   opacity: 0.25;
 }
 
-h6, .h6, h5, .h5, h4, .h4, h3, .h3, h2, .h2, h1, .h1 {
+h6,
+.h6,
+h5,
+.h5,
+h4,
+.h4,
+h3,
+.h3,
+h2,
+.h2,
+h1,
+.h1 {
   margin-top: 0;
   margin-bottom: 0.5rem;
   font-weight: 500;
   line-height: 1.2;
 }
 
-h1, .h1 {
+h1,
+.h1 {
   font-size: calc(1.375rem + 1.5vw);
 }
+
 @media (min-width: 1200px) {
-  h1, .h1 {
+
+  h1,
+  .h1 {
     font-size: 2.5rem;
   }
 }
 
-h2, .h2 {
+h2,
+.h2 {
   font-size: calc(1.325rem + 0.9vw);
 }
+
 @media (min-width: 1200px) {
-  h2, .h2 {
+
+  h2,
+  .h2 {
     font-size: 2rem;
   }
 }
 
-h3, .h3 {
+h3,
+.h3 {
   font-size: calc(1.3rem + 0.6vw);
 }
+
 @media (min-width: 1200px) {
-  h3, .h3 {
+
+  h3,
+  .h3 {
     font-size: 1.75rem;
   }
 }
 
-h4, .h4 {
+h4,
+.h4 {
   font-size: calc(1.275rem + 0.3vw);
 }
+
 @media (min-width: 1200px) {
-  h4, .h4 {
+
+  h4,
+  .h4 {
     font-size: 1.5rem;
   }
 }
 
-h5, .h5 {
+h5,
+.h5 {
   font-size: 1.25rem;
 }
 
-h6, .h6 {
+h6,
+.h6 {
   font-size: 1rem;
 }
 
 p {
   margin-top: 0;
   margin-bottom: 1rem;
 }
 
 abbr[title] {
   -webkit-text-decoration: underline dotted;
-          text-decoration: underline dotted;
+  text-decoration: underline dotted;
   cursor: help;
   -webkit-text-decoration-skip-ink: none;
-          text-decoration-skip-ink: none;
+  text-decoration-skip-ink: none;
 }
 
 address {
   margin-bottom: 1rem;
   font-style: normal;
   line-height: inherit;
 }
@@ -215,19 +245,21 @@
 }
 
 b,
 strong {
   font-weight: bolder;
 }
 
-small, .small {
+small,
+.small {
   font-size: 0.875em;
 }
 
-mark, .mark {
+mark,
+.mark {
   padding: 0.1875em;
   background-color: var(--bs-highlight-bg);
 }
 
 sub,
 sup {
   position: relative;
@@ -244,19 +276,21 @@
   top: -0.5em;
 }
 
 a {
   color: var(--bs-link-color);
   text-decoration: underline;
 }
+
 a:hover {
   color: var(--bs-link-hover-color);
 }
 
-a:not([href]):not([class]), a:not([href]):not([class]):hover {
+a:not([href]):not([class]),
+a:not([href]):not([class]):hover {
   color: inherit;
   text-decoration: none;
 }
 
 pre,
 code,
 kbd,
@@ -268,36 +302,39 @@
 pre {
   display: block;
   margin-top: 0;
   margin-bottom: 1rem;
   overflow: auto;
   font-size: 0.875em;
 }
+
 pre code {
   font-size: inherit;
   color: inherit;
   word-break: normal;
 }
 
 code {
   font-size: 0.875em;
   color: var(--bs-code-color);
   word-wrap: break-word;
 }
-a > code {
+
+a>code {
   color: inherit;
 }
 
 kbd {
   padding: 0.1875rem 0.375rem;
   font-size: 0.875em;
   color: var(--bs-body-bg);
   background-color: var(--bs-body-color);
   border-radius: 0.25rem;
 }
+
 kbd kbd {
   padding: 0;
   font-size: 1em;
 }
 
 figure {
   margin: 0 0 1rem;
@@ -367,28 +404,30 @@
 [role=button] {
   cursor: pointer;
 }
 
 select {
   word-wrap: normal;
 }
+
 select:disabled {
   opacity: 1;
 }
 
 [list]:not([type=date]):not([type=datetime-local]):not([type=month]):not([type=week]):not([type=time])::-webkit-calendar-picker-indicator {
   display: none !important;
 }
 
 button,
 [type=button],
 [type=reset],
 [type=submit] {
   -webkit-appearance: button;
 }
+
 button:not(:disabled),
 [type=button]:not(:disabled),
 [type=reset]:not(:disabled),
 [type=submit]:not(:disabled) {
   cursor: pointer;
 }
 
@@ -412,20 +451,22 @@
   float: left;
   width: 100%;
   padding: 0;
   margin-bottom: 0.5rem;
   font-size: calc(1.275rem + 0.3vw);
   line-height: inherit;
 }
+
 @media (min-width: 1200px) {
   legend {
     font-size: 1.5rem;
   }
 }
-legend + * {
+
+legend+* {
   clear: left;
 }
 
 ::-webkit-datetime-edit-fields-wrapper,
 ::-webkit-datetime-edit-text,
 ::-webkit-datetime-edit-minute,
 ::-webkit-datetime-edit-hour-field,
@@ -492,69 +533,75 @@
 }
 
 .display-1 {
   font-size: calc(1.625rem + 4.5vw);
   font-weight: 300;
   line-height: 1.2;
 }
+
 @media (min-width: 1200px) {
   .display-1 {
     font-size: 5rem;
   }
 }
 
 .display-2 {
   font-size: calc(1.575rem + 3.9vw);
   font-weight: 300;
   line-height: 1.2;
 }
+
 @media (min-width: 1200px) {
   .display-2 {
     font-size: 4.5rem;
   }
 }
 
 .display-3 {
   font-size: calc(1.525rem + 3.3vw);
   font-weight: 300;
   line-height: 1.2;
 }
+
 @media (min-width: 1200px) {
   .display-3 {
     font-size: 4rem;
   }
 }
 
 .display-4 {
   font-size: calc(1.475rem + 2.7vw);
   font-weight: 300;
   line-height: 1.2;
 }
+
 @media (min-width: 1200px) {
   .display-4 {
     font-size: 3.5rem;
   }
 }
 
 .display-5 {
   font-size: calc(1.425rem + 2.1vw);
   font-weight: 300;
   line-height: 1.2;
 }
+
 @media (min-width: 1200px) {
   .display-5 {
     font-size: 3rem;
   }
 }
 
 .display-6 {
   font-size: calc(1.375rem + 1.5vw);
   font-weight: 300;
   line-height: 1.2;
 }
+
 @media (min-width: 1200px) {
   .display-6 {
     font-size: 2.5rem;
   }
 }
 
 .list-unstyled {
@@ -566,37 +613,40 @@
   padding-left: 0;
   list-style: none;
 }
 
 .list-inline-item {
   display: inline-block;
 }
+
 .list-inline-item:not(:last-child) {
   margin-right: 0.5rem;
 }
 
 .initialism {
   font-size: 0.875em;
   text-transform: uppercase;
 }
 
 .blockquote {
   margin-bottom: 1rem;
   font-size: 1.25rem;
 }
-.blockquote > :last-child {
+
+.blockquote> :last-child {
   margin-bottom: 0;
 }
 
 .blockquote-footer {
   margin-top: -1rem;
   margin-bottom: 1rem;
   font-size: 0.875em;
   color: #6c757d;
 }
+
 .blockquote-footer::before {
   content: "— ";
 }
 
 .img-fluid {
   max-width: 100%;
   height: auto;
@@ -638,91 +688,117 @@
   padding-right: calc(var(--bs-gutter-x) * 0.5);
   padding-left: calc(var(--bs-gutter-x) * 0.5);
   margin-right: auto;
   margin-left: auto;
 }
 
 @media (min-width: 576px) {
-  .container-sm, .container {
+
+  .container-sm,
+  .container {
     max-width: 540px;
   }
 }
+
 @media (min-width: 768px) {
-  .container-md, .container-sm, .container {
+
+  .container-md,
+  .container-sm,
+  .container {
     max-width: 720px;
   }
 }
+
 @media (min-width: 992px) {
-  .container-lg, .container-md, .container-sm, .container {
+
+  .container-lg,
+  .container-md,
+  .container-sm,
+  .container {
     max-width: 960px;
   }
 }
+
 @media (min-width: 1200px) {
-  .container-xl, .container-lg, .container-md, .container-sm, .container {
+
+  .container-xl,
+  .container-lg,
+  .container-md,
+  .container-sm,
+  .container {
     max-width: 1140px;
   }
 }
+
 @media (min-width: 1400px) {
-  .container-xxl, .container-xl, .container-lg, .container-md, .container-sm, .container {
+
+  .container-xxl,
+  .container-xl,
+  .container-lg,
+  .container-md,
+  .container-sm,
+  .container {
     max-width: 1320px;
   }
 }
+
 .row {
   --bs-gutter-x: 1.5rem;
   --bs-gutter-y: 0;
   display: flex;
   flex-wrap: wrap;
   margin-top: calc(-1 * var(--bs-gutter-y));
   margin-right: calc(-0.5 * var(--bs-gutter-x));
   margin-left: calc(-0.5 * var(--bs-gutter-x));
 }
-.row > * {
+
+.row>* {
   flex-shrink: 0;
   width: 100%;
   max-width: 100%;
   padding-right: calc(var(--bs-gutter-x) * 0.5);
   padding-left: calc(var(--bs-gutter-x) * 0.5);
   margin-top: var(--bs-gutter-y);
 }
 
 .col {
   flex: 1 0 0%;
 }
 
-.row-cols-auto > * {
+.row-cols-auto>* {
   flex: 0 0 auto;
   width: auto;
 }
 
-.row-cols-1 > * {
+.row-cols-1>* {
   flex: 0 0 auto;
   width: 100%;
 }
 
-.row-cols-2 > * {
+.row-cols-2>* {
   flex: 0 0 auto;
   width: 50%;
 }
 
-.row-cols-3 > * {
+.row-cols-3>* {
   flex: 0 0 auto;
   width: 33.3333333333%;
 }
 
-.row-cols-4 > * {
+.row-cols-4>* {
   flex: 0 0 auto;
   width: 25%;
 }
 
-.row-cols-5 > * {
+.row-cols-5>* {
   flex: 0 0 auto;
   width: 20%;
 }
 
-.row-cols-6 > * {
+.row-cols-6>* {
   flex: 0 0 auto;
   width: 16.6666666667%;
 }
 
 .col-auto {
   flex: 0 0 auto;
   width: auto;
@@ -892,855 +968,1080 @@
   --bs-gutter-y: 3rem;
 }
 
 @media (min-width: 576px) {
   .col-sm {
     flex: 1 0 0%;
   }
-  .row-cols-sm-auto > * {
+
+  .row-cols-sm-auto>* {
     flex: 0 0 auto;
     width: auto;
   }
-  .row-cols-sm-1 > * {
+
+  .row-cols-sm-1>* {
     flex: 0 0 auto;
     width: 100%;
   }
-  .row-cols-sm-2 > * {
+
+  .row-cols-sm-2>* {
     flex: 0 0 auto;
     width: 50%;
   }
-  .row-cols-sm-3 > * {
+
+  .row-cols-sm-3>* {
     flex: 0 0 auto;
     width: 33.3333333333%;
   }
-  .row-cols-sm-4 > * {
+
+  .row-cols-sm-4>* {
     flex: 0 0 auto;
     width: 25%;
   }
-  .row-cols-sm-5 > * {
+
+  .row-cols-sm-5>* {
     flex: 0 0 auto;
     width: 20%;
   }
-  .row-cols-sm-6 > * {
+
+  .row-cols-sm-6>* {
     flex: 0 0 auto;
     width: 16.6666666667%;
   }
+
   .col-sm-auto {
     flex: 0 0 auto;
     width: auto;
   }
+
   .col-sm-1 {
     flex: 0 0 auto;
     width: 8.33333333%;
   }
+
   .col-sm-2 {
     flex: 0 0 auto;
     width: 16.66666667%;
   }
+
   .col-sm-3 {
     flex: 0 0 auto;
     width: 25%;
   }
+
   .col-sm-4 {
     flex: 0 0 auto;
     width: 33.33333333%;
   }
+
   .col-sm-5 {
     flex: 0 0 auto;
     width: 41.66666667%;
   }
+
   .col-sm-6 {
     flex: 0 0 auto;
     width: 50%;
   }
+
   .col-sm-7 {
     flex: 0 0 auto;
     width: 58.33333333%;
   }
+
   .col-sm-8 {
     flex: 0 0 auto;
     width: 66.66666667%;
   }
+
   .col-sm-9 {
     flex: 0 0 auto;
     width: 75%;
   }
+
   .col-sm-10 {
     flex: 0 0 auto;
     width: 83.33333333%;
   }
+
   .col-sm-11 {
     flex: 0 0 auto;
     width: 91.66666667%;
   }
+
   .col-sm-12 {
     flex: 0 0 auto;
     width: 100%;
   }
+
   .offset-sm-0 {
     margin-left: 0;
   }
+
   .offset-sm-1 {
     margin-left: 8.33333333%;
   }
+
   .offset-sm-2 {
     margin-left: 16.66666667%;
   }
+
   .offset-sm-3 {
     margin-left: 25%;
   }
+
   .offset-sm-4 {
     margin-left: 33.33333333%;
   }
+
   .offset-sm-5 {
     margin-left: 41.66666667%;
   }
+
   .offset-sm-6 {
     margin-left: 50%;
   }
+
   .offset-sm-7 {
     margin-left: 58.33333333%;
   }
+
   .offset-sm-8 {
     margin-left: 66.66666667%;
   }
+
   .offset-sm-9 {
     margin-left: 75%;
   }
+
   .offset-sm-10 {
     margin-left: 83.33333333%;
   }
+
   .offset-sm-11 {
     margin-left: 91.66666667%;
   }
+
   .g-sm-0,
   .gx-sm-0 {
     --bs-gutter-x: 0;
   }
+
   .g-sm-0,
   .gy-sm-0 {
     --bs-gutter-y: 0;
   }
+
   .g-sm-1,
   .gx-sm-1 {
     --bs-gutter-x: 0.25rem;
   }
+
   .g-sm-1,
   .gy-sm-1 {
     --bs-gutter-y: 0.25rem;
   }
+
   .g-sm-2,
   .gx-sm-2 {
     --bs-gutter-x: 0.5rem;
   }
+
   .g-sm-2,
   .gy-sm-2 {
     --bs-gutter-y: 0.5rem;
   }
+
   .g-sm-3,
   .gx-sm-3 {
     --bs-gutter-x: 1rem;
   }
+
   .g-sm-3,
   .gy-sm-3 {
     --bs-gutter-y: 1rem;
   }
+
   .g-sm-4,
   .gx-sm-4 {
     --bs-gutter-x: 1.5rem;
   }
+
   .g-sm-4,
   .gy-sm-4 {
     --bs-gutter-y: 1.5rem;
   }
+
   .g-sm-5,
   .gx-sm-5 {
     --bs-gutter-x: 3rem;
   }
+
   .g-sm-5,
   .gy-sm-5 {
     --bs-gutter-y: 3rem;
   }
 }
+
 @media (min-width: 768px) {
   .col-md {
     flex: 1 0 0%;
   }
-  .row-cols-md-auto > * {
+
+  .row-cols-md-auto>* {
     flex: 0 0 auto;
     width: auto;
   }
-  .row-cols-md-1 > * {
+
+  .row-cols-md-1>* {
     flex: 0 0 auto;
     width: 100%;
   }
-  .row-cols-md-2 > * {
+
+  .row-cols-md-2>* {
     flex: 0 0 auto;
     width: 50%;
   }
-  .row-cols-md-3 > * {
+
+  .row-cols-md-3>* {
     flex: 0 0 auto;
     width: 33.3333333333%;
   }
-  .row-cols-md-4 > * {
+
+  .row-cols-md-4>* {
     flex: 0 0 auto;
     width: 25%;
   }
-  .row-cols-md-5 > * {
+
+  .row-cols-md-5>* {
     flex: 0 0 auto;
     width: 20%;
   }
-  .row-cols-md-6 > * {
+
+  .row-cols-md-6>* {
     flex: 0 0 auto;
     width: 16.6666666667%;
   }
+
   .col-md-auto {
     flex: 0 0 auto;
     width: auto;
   }
+
   .col-md-1 {
     flex: 0 0 auto;
     width: 8.33333333%;
   }
+
   .col-md-2 {
     flex: 0 0 auto;
     width: 16.66666667%;
   }
+
   .col-md-3 {
     flex: 0 0 auto;
     width: 25%;
   }
+
   .col-md-4 {
     flex: 0 0 auto;
     width: 33.33333333%;
   }
+
   .col-md-5 {
     flex: 0 0 auto;
     width: 41.66666667%;
   }
+
   .col-md-6 {
     flex: 0 0 auto;
     width: 50%;
   }
+
   .col-md-7 {
     flex: 0 0 auto;
     width: 58.33333333%;
   }
+
   .col-md-8 {
     flex: 0 0 auto;
     width: 66.66666667%;
   }
+
   .col-md-9 {
     flex: 0 0 auto;
     width: 75%;
   }
+
   .col-md-10 {
     flex: 0 0 auto;
     width: 83.33333333%;
   }
+
   .col-md-11 {
     flex: 0 0 auto;
     width: 91.66666667%;
   }
+
   .col-md-12 {
     flex: 0 0 auto;
     width: 100%;
   }
+
   .offset-md-0 {
     margin-left: 0;
   }
+
   .offset-md-1 {
     margin-left: 8.33333333%;
   }
+
   .offset-md-2 {
     margin-left: 16.66666667%;
   }
+
   .offset-md-3 {
     margin-left: 25%;
   }
+
   .offset-md-4 {
     margin-left: 33.33333333%;
   }
+
   .offset-md-5 {
     margin-left: 41.66666667%;
   }
+
   .offset-md-6 {
     margin-left: 50%;
   }
+
   .offset-md-7 {
     margin-left: 58.33333333%;
   }
+
   .offset-md-8 {
     margin-left: 66.66666667%;
   }
+
   .offset-md-9 {
     margin-left: 75%;
   }
+
   .offset-md-10 {
     margin-left: 83.33333333%;
   }
+
   .offset-md-11 {
     margin-left: 91.66666667%;
   }
+
   .g-md-0,
   .gx-md-0 {
     --bs-gutter-x: 0;
   }
+
   .g-md-0,
   .gy-md-0 {
     --bs-gutter-y: 0;
   }
+
   .g-md-1,
   .gx-md-1 {
     --bs-gutter-x: 0.25rem;
   }
+
   .g-md-1,
   .gy-md-1 {
     --bs-gutter-y: 0.25rem;
   }
+
   .g-md-2,
   .gx-md-2 {
     --bs-gutter-x: 0.5rem;
   }
+
   .g-md-2,
   .gy-md-2 {
     --bs-gutter-y: 0.5rem;
   }
+
   .g-md-3,
   .gx-md-3 {
     --bs-gutter-x: 1rem;
   }
+
   .g-md-3,
   .gy-md-3 {
     --bs-gutter-y: 1rem;
   }
+
   .g-md-4,
   .gx-md-4 {
     --bs-gutter-x: 1.5rem;
   }
+
   .g-md-4,
   .gy-md-4 {
     --bs-gutter-y: 1.5rem;
   }
+
   .g-md-5,
   .gx-md-5 {
     --bs-gutter-x: 3rem;
   }
+
   .g-md-5,
   .gy-md-5 {
     --bs-gutter-y: 3rem;
   }
 }
+
 @media (min-width: 992px) {
   .col-lg {
     flex: 1 0 0%;
   }
-  .row-cols-lg-auto > * {
+
+  .row-cols-lg-auto>* {
     flex: 0 0 auto;
     width: auto;
   }
-  .row-cols-lg-1 > * {
+
+  .row-cols-lg-1>* {
     flex: 0 0 auto;
     width: 100%;
   }
-  .row-cols-lg-2 > * {
+
+  .row-cols-lg-2>* {
     flex: 0 0 auto;
     width: 50%;
   }
-  .row-cols-lg-3 > * {
+
+  .row-cols-lg-3>* {
     flex: 0 0 auto;
     width: 33.3333333333%;
   }
-  .row-cols-lg-4 > * {
+
+  .row-cols-lg-4>* {
     flex: 0 0 auto;
     width: 25%;
   }
-  .row-cols-lg-5 > * {
+
+  .row-cols-lg-5>* {
     flex: 0 0 auto;
     width: 20%;
   }
-  .row-cols-lg-6 > * {
+
+  .row-cols-lg-6>* {
     flex: 0 0 auto;
     width: 16.6666666667%;
   }
+
   .col-lg-auto {
     flex: 0 0 auto;
     width: auto;
   }
+
   .col-lg-1 {
     flex: 0 0 auto;
     width: 8.33333333%;
   }
+
   .col-lg-2 {
     flex: 0 0 auto;
     width: 16.66666667%;
   }
+
   .col-lg-3 {
     flex: 0 0 auto;
     width: 25%;
   }
+
   .col-lg-4 {
     flex: 0 0 auto;
     width: 33.33333333%;
   }
+
   .col-lg-5 {
     flex: 0 0 auto;
     width: 41.66666667%;
   }
+
   .col-lg-6 {
     flex: 0 0 auto;
     width: 50%;
   }
+
   .col-lg-7 {
     flex: 0 0 auto;
     width: 58.33333333%;
   }
+
   .col-lg-8 {
     flex: 0 0 auto;
     width: 66.66666667%;
   }
+
   .col-lg-9 {
     flex: 0 0 auto;
     width: 75%;
   }
+
   .col-lg-10 {
     flex: 0 0 auto;
     width: 83.33333333%;
   }
+
   .col-lg-11 {
     flex: 0 0 auto;
     width: 91.66666667%;
   }
+
   .col-lg-12 {
     flex: 0 0 auto;
     width: 100%;
   }
+
   .offset-lg-0 {
     margin-left: 0;
   }
+
   .offset-lg-1 {
     margin-left: 8.33333333%;
   }
+
   .offset-lg-2 {
     margin-left: 16.66666667%;
   }
+
   .offset-lg-3 {
     margin-left: 25%;
   }
+
   .offset-lg-4 {
     margin-left: 33.33333333%;
   }
+
   .offset-lg-5 {
     margin-left: 41.66666667%;
   }
+
   .offset-lg-6 {
     margin-left: 50%;
   }
+
   .offset-lg-7 {
     margin-left: 58.33333333%;
   }
+
   .offset-lg-8 {
     margin-left: 66.66666667%;
   }
+
   .offset-lg-9 {
     margin-left: 75%;
   }
+
   .offset-lg-10 {
     margin-left: 83.33333333%;
   }
+
   .offset-lg-11 {
     margin-left: 91.66666667%;
   }
+
   .g-lg-0,
   .gx-lg-0 {
     --bs-gutter-x: 0;
   }
+
   .g-lg-0,
   .gy-lg-0 {
     --bs-gutter-y: 0;
   }
+
   .g-lg-1,
   .gx-lg-1 {
     --bs-gutter-x: 0.25rem;
   }
+
   .g-lg-1,
   .gy-lg-1 {
     --bs-gutter-y: 0.25rem;
   }
+
   .g-lg-2,
   .gx-lg-2 {
     --bs-gutter-x: 0.5rem;
   }
+
   .g-lg-2,
   .gy-lg-2 {
     --bs-gutter-y: 0.5rem;
   }
+
   .g-lg-3,
   .gx-lg-3 {
     --bs-gutter-x: 1rem;
   }
+
   .g-lg-3,
   .gy-lg-3 {
     --bs-gutter-y: 1rem;
   }
+
   .g-lg-4,
   .gx-lg-4 {
     --bs-gutter-x: 1.5rem;
   }
+
   .g-lg-4,
   .gy-lg-4 {
     --bs-gutter-y: 1.5rem;
   }
+
   .g-lg-5,
   .gx-lg-5 {
     --bs-gutter-x: 3rem;
   }
+
   .g-lg-5,
   .gy-lg-5 {
     --bs-gutter-y: 3rem;
   }
 }
+
 @media (min-width: 1200px) {
   .col-xl {
     flex: 1 0 0%;
   }
-  .row-cols-xl-auto > * {
+
+  .row-cols-xl-auto>* {
     flex: 0 0 auto;
     width: auto;
   }
-  .row-cols-xl-1 > * {
+
+  .row-cols-xl-1>* {
     flex: 0 0 auto;
     width: 100%;
   }
-  .row-cols-xl-2 > * {
+
+  .row-cols-xl-2>* {
     flex: 0 0 auto;
     width: 50%;
   }
-  .row-cols-xl-3 > * {
+
+  .row-cols-xl-3>* {
     flex: 0 0 auto;
     width: 33.3333333333%;
   }
-  .row-cols-xl-4 > * {
+
+  .row-cols-xl-4>* {
     flex: 0 0 auto;
     width: 25%;
   }
-  .row-cols-xl-5 > * {
+
+  .row-cols-xl-5>* {
     flex: 0 0 auto;
     width: 20%;
   }
-  .row-cols-xl-6 > * {
+
+  .row-cols-xl-6>* {
     flex: 0 0 auto;
     width: 16.6666666667%;
   }
+
   .col-xl-auto {
     flex: 0 0 auto;
     width: auto;
   }
+
   .col-xl-1 {
     flex: 0 0 auto;
     width: 8.33333333%;
   }
+
   .col-xl-2 {
     flex: 0 0 auto;
     width: 16.66666667%;
   }
+
   .col-xl-3 {
     flex: 0 0 auto;
     width: 25%;
   }
+
   .col-xl-4 {
     flex: 0 0 auto;
     width: 33.33333333%;
   }
+
   .col-xl-5 {
     flex: 0 0 auto;
     width: 41.66666667%;
   }
+
   .col-xl-6 {
     flex: 0 0 auto;
     width: 50%;
   }
+
   .col-xl-7 {
     flex: 0 0 auto;
     width: 58.33333333%;
   }
+
   .col-xl-8 {
     flex: 0 0 auto;
     width: 66.66666667%;
   }
+
   .col-xl-9 {
     flex: 0 0 auto;
     width: 75%;
   }
+
   .col-xl-10 {
     flex: 0 0 auto;
     width: 83.33333333%;
   }
+
   .col-xl-11 {
     flex: 0 0 auto;
     width: 91.66666667%;
   }
+
   .col-xl-12 {
     flex: 0 0 auto;
     width: 100%;
   }
+
   .offset-xl-0 {
     margin-left: 0;
   }
+
   .offset-xl-1 {
     margin-left: 8.33333333%;
   }
+
   .offset-xl-2 {
     margin-left: 16.66666667%;
   }
+
   .offset-xl-3 {
     margin-left: 25%;
   }
+
   .offset-xl-4 {
     margin-left: 33.33333333%;
   }
+
   .offset-xl-5 {
     margin-left: 41.66666667%;
   }
+
   .offset-xl-6 {
     margin-left: 50%;
   }
+
   .offset-xl-7 {
     margin-left: 58.33333333%;
   }
+
   .offset-xl-8 {
     margin-left: 66.66666667%;
   }
+
   .offset-xl-9 {
     margin-left: 75%;
   }
+
   .offset-xl-10 {
     margin-left: 83.33333333%;
   }
+
   .offset-xl-11 {
     margin-left: 91.66666667%;
   }
+
   .g-xl-0,
   .gx-xl-0 {
     --bs-gutter-x: 0;
   }
+
   .g-xl-0,
   .gy-xl-0 {
     --bs-gutter-y: 0;
   }
+
   .g-xl-1,
   .gx-xl-1 {
     --bs-gutter-x: 0.25rem;
   }
+
   .g-xl-1,
   .gy-xl-1 {
     --bs-gutter-y: 0.25rem;
   }
+
   .g-xl-2,
   .gx-xl-2 {
     --bs-gutter-x: 0.5rem;
   }
+
   .g-xl-2,
   .gy-xl-2 {
     --bs-gutter-y: 0.5rem;
   }
+
   .g-xl-3,
   .gx-xl-3 {
     --bs-gutter-x: 1rem;
   }
+
   .g-xl-3,
   .gy-xl-3 {
     --bs-gutter-y: 1rem;
   }
+
   .g-xl-4,
   .gx-xl-4 {
     --bs-gutter-x: 1.5rem;
   }
+
   .g-xl-4,
   .gy-xl-4 {
     --bs-gutter-y: 1.5rem;
   }
+
   .g-xl-5,
   .gx-xl-5 {
     --bs-gutter-x: 3rem;
   }
+
   .g-xl-5,
   .gy-xl-5 {
     --bs-gutter-y: 3rem;
   }
 }
+
 @media (min-width: 1400px) {
   .col-xxl {
     flex: 1 0 0%;
   }
-  .row-cols-xxl-auto > * {
+
+  .row-cols-xxl-auto>* {
     flex: 0 0 auto;
     width: auto;
   }
-  .row-cols-xxl-1 > * {
+
+  .row-cols-xxl-1>* {
     flex: 0 0 auto;
     width: 100%;
   }
-  .row-cols-xxl-2 > * {
+
+  .row-cols-xxl-2>* {
     flex: 0 0 auto;
     width: 50%;
   }
-  .row-cols-xxl-3 > * {
+
+  .row-cols-xxl-3>* {
     flex: 0 0 auto;
     width: 33.3333333333%;
   }
-  .row-cols-xxl-4 > * {
+
+  .row-cols-xxl-4>* {
     flex: 0 0 auto;
     width: 25%;
   }
-  .row-cols-xxl-5 > * {
+
+  .row-cols-xxl-5>* {
     flex: 0 0 auto;
     width: 20%;
   }
-  .row-cols-xxl-6 > * {
+
+  .row-cols-xxl-6>* {
     flex: 0 0 auto;
     width: 16.6666666667%;
   }
+
   .col-xxl-auto {
     flex: 0 0 auto;
     width: auto;
   }
+
   .col-xxl-1 {
     flex: 0 0 auto;
     width: 8.33333333%;
   }
+
   .col-xxl-2 {
     flex: 0 0 auto;
     width: 16.66666667%;
   }
+
   .col-xxl-3 {
     flex: 0 0 auto;
     width: 25%;
   }
+
   .col-xxl-4 {
     flex: 0 0 auto;
     width: 33.33333333%;
   }
+
   .col-xxl-5 {
     flex: 0 0 auto;
     width: 41.66666667%;
   }
+
   .col-xxl-6 {
     flex: 0 0 auto;
     width: 50%;
   }
+
   .col-xxl-7 {
     flex: 0 0 auto;
     width: 58.33333333%;
   }
+
   .col-xxl-8 {
     flex: 0 0 auto;
     width: 66.66666667%;
   }
+
   .col-xxl-9 {
     flex: 0 0 auto;
     width: 75%;
   }
+
   .col-xxl-10 {
     flex: 0 0 auto;
     width: 83.33333333%;
   }
+
   .col-xxl-11 {
     flex: 0 0 auto;
     width: 91.66666667%;
   }
+
   .col-xxl-12 {
     flex: 0 0 auto;
     width: 100%;
   }
+
   .offset-xxl-0 {
     margin-left: 0;
   }
+
   .offset-xxl-1 {
     margin-left: 8.33333333%;
   }
+
   .offset-xxl-2 {
     margin-left: 16.66666667%;
   }
+
   .offset-xxl-3 {
     margin-left: 25%;
   }
+
   .offset-xxl-4 {
     margin-left: 33.33333333%;
   }
+
   .offset-xxl-5 {
     margin-left: 41.66666667%;
   }
+
   .offset-xxl-6 {
     margin-left: 50%;
   }
+
   .offset-xxl-7 {
     margin-left: 58.33333333%;
   }
+
   .offset-xxl-8 {
     margin-left: 66.66666667%;
   }
+
   .offset-xxl-9 {
     margin-left: 75%;
   }
+
   .offset-xxl-10 {
     margin-left: 83.33333333%;
   }
+
   .offset-xxl-11 {
     margin-left: 91.66666667%;
   }
+
   .g-xxl-0,
   .gx-xxl-0 {
     --bs-gutter-x: 0;
   }
+
   .g-xxl-0,
   .gy-xxl-0 {
     --bs-gutter-y: 0;
   }
+
   .g-xxl-1,
   .gx-xxl-1 {
     --bs-gutter-x: 0.25rem;
   }
+
   .g-xxl-1,
   .gy-xxl-1 {
     --bs-gutter-y: 0.25rem;
   }
+
   .g-xxl-2,
   .gx-xxl-2 {
     --bs-gutter-x: 0.5rem;
   }
+
   .g-xxl-2,
   .gy-xxl-2 {
     --bs-gutter-y: 0.5rem;
   }
+
   .g-xxl-3,
   .gx-xxl-3 {
     --bs-gutter-x: 1rem;
   }
+
   .g-xxl-3,
   .gy-xxl-3 {
     --bs-gutter-y: 1rem;
   }
+
   .g-xxl-4,
   .gx-xxl-4 {
     --bs-gutter-x: 1.5rem;
   }
+
   .g-xxl-4,
   .gy-xxl-4 {
     --bs-gutter-y: 1.5rem;
   }
+
   .g-xxl-5,
   .gx-xxl-5 {
     --bs-gutter-x: 3rem;
   }
+
   .g-xxl-5,
   .gy-xxl-5 {
     --bs-gutter-y: 3rem;
   }
 }
+
 .table {
   --bs-table-color: var(--bs-body-color);
   --bs-table-bg: transparent;
   --bs-table-border-color: var(--bs-border-color);
   --bs-table-accent-bg: transparent;
   --bs-table-striped-color: var(--bs-body-color);
   --bs-table-striped-bg: rgba(0, 0, 0, 0.05);
@@ -1750,69 +2051,74 @@
   --bs-table-hover-bg: rgba(0, 0, 0, 0.075);
   width: 100%;
   margin-bottom: 1rem;
   color: var(--bs-table-color);
   vertical-align: top;
   border-color: var(--bs-table-border-color);
 }
-.table > :not(caption) > * > * {
+
+.table> :not(caption)>*>* {
   padding: 0.5rem 0.5rem;
   background-color: var(--bs-table-bg);
   border-bottom-width: 1px;
   box-shadow: inset 0 0 0 9999px var(--bs-table-accent-bg);
 }
-.table > tbody {
+
+.table>tbody {
   vertical-align: inherit;
 }
-.table > thead {
+
+.table>thead {
   vertical-align: bottom;
 }
 
 .table-group-divider {
   border-top: 2px solid currentcolor;
 }
 
 .caption-top {
   caption-side: top;
 }
 
-.table-sm > :not(caption) > * > * {
+.table-sm> :not(caption)>*>* {
   padding: 0.25rem 0.25rem;
 }
 
-.table-bordered > :not(caption) > * {
+.table-bordered> :not(caption)>* {
   border-width: 1px 0;
 }
-.table-bordered > :not(caption) > * > * {
+
+.table-bordered> :not(caption)>*>* {
   border-width: 0 1px;
 }
 
-.table-borderless > :not(caption) > * > * {
+.table-borderless> :not(caption)>*>* {
   border-bottom-width: 0;
 }
-.table-borderless > :not(:first-child) {
+
+.table-borderless> :not(:first-child) {
   border-top-width: 0;
 }
 
-.table-striped > tbody > tr:nth-of-type(odd) > * {
+.table-striped>tbody>tr:nth-of-type(odd)>* {
   --bs-table-accent-bg: var(--bs-table-striped-bg);
   color: var(--bs-table-striped-color);
 }
 
-.table-striped-columns > :not(caption) > tr > :nth-child(even) {
+.table-striped-columns> :not(caption)>tr> :nth-child(even) {
   --bs-table-accent-bg: var(--bs-table-striped-bg);
   color: var(--bs-table-striped-color);
 }
 
 .table-active {
   --bs-table-accent-bg: var(--bs-table-active-bg);
   color: var(--bs-table-active-color);
 }
 
-.table-hover > tbody > tr:hover > * {
+.table-hover>tbody>tr:hover>* {
   --bs-table-accent-bg: var(--bs-table-hover-bg);
   color: var(--bs-table-hover-color);
 }
 
 .table-primary {
   --bs-table-color: #000;
   --bs-table-bg: #cfe2ff;
@@ -1932,38 +2238,43 @@
 
 @media (max-width: 575.98px) {
   .table-responsive-sm {
     overflow-x: auto;
     -webkit-overflow-scrolling: touch;
   }
 }
+
 @media (max-width: 767.98px) {
   .table-responsive-md {
     overflow-x: auto;
     -webkit-overflow-scrolling: touch;
   }
 }
+
 @media (max-width: 991.98px) {
   .table-responsive-lg {
     overflow-x: auto;
     -webkit-overflow-scrolling: touch;
   }
 }
+
 @media (max-width: 1199.98px) {
   .table-responsive-xl {
     overflow-x: auto;
     -webkit-overflow-scrolling: touch;
   }
 }
+
 @media (max-width: 1399.98px) {
   .table-responsive-xxl {
     overflow-x: auto;
     -webkit-overflow-scrolling: touch;
   }
 }
+
 .form-label {
   margin-bottom: 0.5rem;
 }
 
 .col-form-label {
   padding-top: calc(0.375rem + 1px);
   padding-bottom: calc(0.375rem + 1px);
@@ -1998,72 +2309,83 @@
   font-weight: 400;
   line-height: 1.5;
   color: #212529;
   background-color: #fff;
   background-clip: padding-box;
   border: 1px solid #ced4da;
   -webkit-appearance: none;
-     -moz-appearance: none;
-          appearance: none;
+  -moz-appearance: none;
+  appearance: none;
   border-radius: 0.375rem;
   transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .form-control {
     transition: none;
   }
 }
+
 .form-control[type=file] {
   overflow: hidden;
 }
+
 .form-control[type=file]:not(:disabled):not([readonly]) {
   cursor: pointer;
 }
+
 .form-control:focus {
   color: #212529;
   background-color: #fff;
   border-color: #86b7fe;
   outline: 0;
   box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
+
 .form-control::-webkit-date-and-time-value {
   height: 1.5em;
 }
+
 .form-control::-moz-placeholder {
   color: #6c757d;
   opacity: 1;
 }
+
 .form-control::placeholder {
   color: #6c757d;
   opacity: 1;
 }
+
 .form-control:disabled {
   background-color: #e9ecef;
   opacity: 1;
 }
+
 .form-control::file-selector-button {
   padding: 0.375rem 0.75rem;
   margin: -0.375rem -0.75rem;
   -webkit-margin-end: 0.75rem;
-          margin-inline-end: 0.75rem;
+  margin-inline-end: 0.75rem;
   color: #212529;
   background-color: #e9ecef;
   pointer-events: none;
   border-color: inherit;
   border-style: solid;
   border-width: 0;
   border-inline-end-width: 1px;
   border-radius: 0;
   transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .form-control::file-selector-button {
     transition: none;
   }
 }
+
 .form-control:hover:not(:disabled):not([readonly])::file-selector-button {
   background-color: #dde0e3;
 }
 
 .form-control-plaintext {
   display: block;
   width: 100%;
@@ -2071,76 +2393,88 @@
   margin-bottom: 0;
   line-height: 1.5;
   color: #212529;
   background-color: transparent;
   border: solid transparent;
   border-width: 1px 0;
 }
+
 .form-control-plaintext:focus {
   outline: 0;
 }
-.form-control-plaintext.form-control-sm, .form-control-plaintext.form-control-lg {
+
+.form-control-plaintext.form-control-sm,
+.form-control-plaintext.form-control-lg {
   padding-right: 0;
   padding-left: 0;
 }
 
 .form-control-sm {
   min-height: calc(1.5em + 0.5rem + 2px);
   padding: 0.25rem 0.5rem;
   font-size: 0.875rem;
   border-radius: 0.25rem;
 }
+
 .form-control-sm::file-selector-button {
   padding: 0.25rem 0.5rem;
   margin: -0.25rem -0.5rem;
   -webkit-margin-end: 0.5rem;
-          margin-inline-end: 0.5rem;
+  margin-inline-end: 0.5rem;
 }
 
 .form-control-lg {
   min-height: calc(1.5em + 1rem + 2px);
   padding: 0.5rem 1rem;
   font-size: 1.25rem;
   border-radius: 0.5rem;
 }
+
 .form-control-lg::file-selector-button {
   padding: 0.5rem 1rem;
   margin: -0.5rem -1rem;
   -webkit-margin-end: 1rem;
-          margin-inline-end: 1rem;
+  margin-inline-end: 1rem;
 }
 
 textarea.form-control {
   min-height: calc(1.5em + 0.75rem + 2px);
 }
+
 textarea.form-control-sm {
   min-height: calc(1.5em + 0.5rem + 2px);
 }
+
 textarea.form-control-lg {
   min-height: calc(1.5em + 1rem + 2px);
 }
 
 .form-control-color {
   width: 3rem;
   height: calc(1.5em + 0.75rem + 2px);
   padding: 0.375rem;
 }
+
 .form-control-color:not(:disabled):not([readonly]) {
   cursor: pointer;
 }
+
 .form-control-color::-moz-color-swatch {
   border: 0 !important;
   border-radius: 0.375rem;
 }
+
 .form-control-color::-webkit-color-swatch {
   border-radius: 0.375rem;
 }
+
 .form-control-color.form-control-sm {
   height: calc(1.5em + 0.5rem + 2px);
 }
+
 .form-control-color.form-control-lg {
   height: calc(1.5em + 1rem + 2px);
 }
 
 .form-select {
   display: block;
   width: 100%;
@@ -2155,34 +2489,40 @@
   background-repeat: no-repeat;
   background-position: right 0.75rem center;
   background-size: 16px 12px;
   border: 1px solid #ced4da;
   border-radius: 0.375rem;
   transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   -webkit-appearance: none;
-     -moz-appearance: none;
-          appearance: none;
+  -moz-appearance: none;
+  appearance: none;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .form-select {
     transition: none;
   }
 }
+
 .form-select:focus {
   border-color: #86b7fe;
   outline: 0;
   box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
-.form-select[multiple], .form-select[size]:not([size="1"]) {
+
+.form-select[multiple],
+.form-select[size]:not([size="1"]) {
   padding-right: 0.75rem;
   background-image: none;
 }
+
 .form-select:disabled {
   background-color: #e9ecef;
 }
+
 .form-select:-moz-focusring {
   color: transparent;
   text-shadow: 0 0 0 #212529;
 }
 
 .form-select-sm {
   padding-top: 0.25rem;
@@ -2202,24 +2542,26 @@
 
 .form-check {
   display: block;
   min-height: 1.5rem;
   padding-left: 1.5em;
   margin-bottom: 0.125rem;
 }
+
 .form-check .form-check-input {
   float: left;
   margin-left: -1.5em;
 }
 
 .form-check-reverse {
   padding-right: 1.5em;
   padding-left: 0;
   text-align: right;
 }
+
 .form-check-reverse .form-check-input {
   float: right;
   margin-right: -1.5em;
   margin-left: 0;
 }
 
 .form-check-input {
@@ -2229,85 +2571,102 @@
   vertical-align: top;
   background-color: #fff;
   background-repeat: no-repeat;
   background-position: center;
   background-size: contain;
   border: 1px solid rgba(0, 0, 0, 0.25);
   -webkit-appearance: none;
-     -moz-appearance: none;
-          appearance: none;
+  -moz-appearance: none;
+  appearance: none;
   -webkit-print-color-adjust: exact;
-          print-color-adjust: exact;
+  print-color-adjust: exact;
 }
+
 .form-check-input[type=checkbox] {
   border-radius: 0.25em;
 }
+
 .form-check-input[type=radio] {
   border-radius: 50%;
 }
+
 .form-check-input:active {
   filter: brightness(90%);
 }
+
 .form-check-input:focus {
   border-color: #86b7fe;
   outline: 0;
   box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
+
 .form-check-input:checked {
   background-color: #0d6efd;
   border-color: #0d6efd;
 }
+
 .form-check-input:checked[type=checkbox] {
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='m6 10 3 3 6-6'/%3e%3c/svg%3e");
 }
+
 .form-check-input:checked[type=radio] {
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='2' fill='%23fff'/%3e%3c/svg%3e");
 }
+
 .form-check-input[type=checkbox]:indeterminate {
   background-color: #0d6efd;
   border-color: #0d6efd;
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 20 20'%3e%3cpath fill='none' stroke='%23fff' stroke-linecap='round' stroke-linejoin='round' stroke-width='3' d='M6 10h8'/%3e%3c/svg%3e");
 }
+
 .form-check-input:disabled {
   pointer-events: none;
   filter: none;
   opacity: 0.5;
 }
-.form-check-input[disabled] ~ .form-check-label, .form-check-input:disabled ~ .form-check-label {
+
+.form-check-input[disabled]~.form-check-label,
+.form-check-input:disabled~.form-check-label {
   cursor: default;
   opacity: 0.5;
 }
 
 .form-switch {
   padding-left: 2.5em;
 }
+
 .form-switch .form-check-input {
   width: 2em;
   margin-left: -2.5em;
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='rgba%280, 0, 0, 0.25%29'/%3e%3c/svg%3e");
   background-position: left center;
   border-radius: 2em;
   transition: background-position 0.15s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .form-switch .form-check-input {
     transition: none;
   }
 }
+
 .form-switch .form-check-input:focus {
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%2386b7fe'/%3e%3c/svg%3e");
 }
+
 .form-switch .form-check-input:checked {
   background-position: right center;
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='-4 -4 8 8'%3e%3ccircle r='3' fill='%23fff'/%3e%3c/svg%3e");
 }
+
 .form-switch.form-check-reverse {
   padding-right: 2.5em;
   padding-left: 0;
 }
+
 .form-switch.form-check-reverse .form-check-input {
   margin-right: -2.5em;
   margin-left: 0;
 }
 
 .form-check-inline {
   display: inline-block;
@@ -2315,120 +2674,139 @@
 }
 
 .btn-check {
   position: absolute;
   clip: rect(0, 0, 0, 0);
   pointer-events: none;
 }
-.btn-check[disabled] + .btn, .btn-check:disabled + .btn {
+
+.btn-check[disabled]+.btn,
+.btn-check:disabled+.btn {
   pointer-events: none;
   filter: none;
   opacity: 0.65;
 }
 
 .form-range {
   width: 100%;
   height: 1.5rem;
   padding: 0;
   background-color: transparent;
   -webkit-appearance: none;
-     -moz-appearance: none;
-          appearance: none;
+  -moz-appearance: none;
+  appearance: none;
 }
+
 .form-range:focus {
   outline: 0;
 }
+
 .form-range:focus::-webkit-slider-thumb {
   box-shadow: 0 0 0 1px #fff, 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
+
 .form-range:focus::-moz-range-thumb {
   box-shadow: 0 0 0 1px #fff, 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
 }
+
 .form-range::-moz-focus-outer {
   border: 0;
 }
+
 .form-range::-webkit-slider-thumb {
   width: 1rem;
   height: 1rem;
   margin-top: -0.25rem;
   background-color: #0d6efd;
   border: 0;
   border-radius: 1rem;
   -webkit-transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   -webkit-appearance: none;
-          appearance: none;
+  appearance: none;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .form-range::-webkit-slider-thumb {
     -webkit-transition: none;
     transition: none;
   }
 }
+
 .form-range::-webkit-slider-thumb:active {
   background-color: #b6d4fe;
 }
+
 .form-range::-webkit-slider-runnable-track {
   width: 100%;
   height: 0.5rem;
   color: transparent;
   cursor: pointer;
   background-color: #dee2e6;
   border-color: transparent;
   border-radius: 1rem;
 }
+
 .form-range::-moz-range-thumb {
   width: 1rem;
   height: 1rem;
   background-color: #0d6efd;
   border: 0;
   border-radius: 1rem;
   -moz-transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   transition: background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
   -moz-appearance: none;
-       appearance: none;
+  appearance: none;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .form-range::-moz-range-thumb {
     -moz-transition: none;
     transition: none;
   }
 }
+
 .form-range::-moz-range-thumb:active {
   background-color: #b6d4fe;
 }
+
 .form-range::-moz-range-track {
   width: 100%;
   height: 0.5rem;
   color: transparent;
   cursor: pointer;
   background-color: #dee2e6;
   border-color: transparent;
   border-radius: 1rem;
 }
+
 .form-range:disabled {
   pointer-events: none;
 }
+
 .form-range:disabled::-webkit-slider-thumb {
   background-color: #adb5bd;
 }
+
 .form-range:disabled::-moz-range-thumb {
   background-color: #adb5bd;
 }
 
 .form-floating {
   position: relative;
 }
-.form-floating > .form-control,
-.form-floating > .form-control-plaintext,
-.form-floating > .form-select {
+
+.form-floating>.form-control,
+.form-floating>.form-control-plaintext,
+.form-floating>.form-select {
   height: calc(3.5rem + 2px);
   line-height: 1.25;
 }
-.form-floating > label {
+
+.form-floating>label {
   position: absolute;
   top: 0;
   left: 0;
   width: 100%;
   height: 100%;
   padding: 1rem 0.75rem;
   overflow: hidden;
@@ -2436,92 +2814,111 @@
   text-overflow: ellipsis;
   white-space: nowrap;
   pointer-events: none;
   border: 1px solid transparent;
   transform-origin: 0 0;
   transition: opacity 0.1s ease-in-out, transform 0.1s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
-  .form-floating > label {
+  .form-floating>label {
     transition: none;
   }
 }
-.form-floating > .form-control,
-.form-floating > .form-control-plaintext {
+
+.form-floating>.form-control,
+.form-floating>.form-control-plaintext {
   padding: 1rem 0.75rem;
 }
-.form-floating > .form-control::-moz-placeholder, .form-floating > .form-control-plaintext::-moz-placeholder {
+
+.form-floating>.form-control::-moz-placeholder,
+.form-floating>.form-control-plaintext::-moz-placeholder {
   color: transparent;
 }
-.form-floating > .form-control::placeholder,
-.form-floating > .form-control-plaintext::placeholder {
+
+.form-floating>.form-control::placeholder,
+.form-floating>.form-control-plaintext::placeholder {
   color: transparent;
 }
-.form-floating > .form-control:not(:-moz-placeholder-shown), .form-floating > .form-control-plaintext:not(:-moz-placeholder-shown) {
+
+.form-floating>.form-control:not(:-moz-placeholder-shown),
+.form-floating>.form-control-plaintext:not(:-moz-placeholder-shown) {
   padding-top: 1.625rem;
   padding-bottom: 0.625rem;
 }
-.form-floating > .form-control:focus, .form-floating > .form-control:not(:placeholder-shown),
-.form-floating > .form-control-plaintext:focus,
-.form-floating > .form-control-plaintext:not(:placeholder-shown) {
+
+.form-floating>.form-control:focus,
+.form-floating>.form-control:not(:placeholder-shown),
+.form-floating>.form-control-plaintext:focus,
+.form-floating>.form-control-plaintext:not(:placeholder-shown) {
   padding-top: 1.625rem;
   padding-bottom: 0.625rem;
 }
-.form-floating > .form-control:-webkit-autofill,
-.form-floating > .form-control-plaintext:-webkit-autofill {
+
+.form-floating>.form-control:-webkit-autofill,
+.form-floating>.form-control-plaintext:-webkit-autofill {
   padding-top: 1.625rem;
   padding-bottom: 0.625rem;
 }
-.form-floating > .form-select {
+
+.form-floating>.form-select {
   padding-top: 1.625rem;
   padding-bottom: 0.625rem;
 }
-.form-floating > .form-control:not(:-moz-placeholder-shown) ~ label {
+
+.form-floating>.form-control:not(:-moz-placeholder-shown)~label {
   opacity: 0.65;
   transform: scale(0.85) translateY(-0.5rem) translateX(0.15rem);
 }
-.form-floating > .form-control:focus ~ label,
-.form-floating > .form-control:not(:placeholder-shown) ~ label,
-.form-floating > .form-control-plaintext ~ label,
-.form-floating > .form-select ~ label {
+
+.form-floating>.form-control:focus~label,
+.form-floating>.form-control:not(:placeholder-shown)~label,
+.form-floating>.form-control-plaintext~label,
+.form-floating>.form-select~label {
   opacity: 0.65;
   transform: scale(0.85) translateY(-0.5rem) translateX(0.15rem);
 }
-.form-floating > .form-control:-webkit-autofill ~ label {
+
+.form-floating>.form-control:-webkit-autofill~label {
   opacity: 0.65;
   transform: scale(0.85) translateY(-0.5rem) translateX(0.15rem);
 }
-.form-floating > .form-control-plaintext ~ label {
+
+.form-floating>.form-control-plaintext~label {
   border-width: 1px 0;
 }
 
 .input-group {
   position: relative;
   display: flex;
   flex-wrap: wrap;
   align-items: stretch;
   width: 100%;
 }
-.input-group > .form-control,
-.input-group > .form-select,
-.input-group > .form-floating {
+
+.input-group>.form-control,
+.input-group>.form-select,
+.input-group>.form-floating {
   position: relative;
   flex: 1 1 auto;
   width: 1%;
   min-width: 0;
 }
-.input-group > .form-control:focus,
-.input-group > .form-select:focus,
-.input-group > .form-floating:focus-within {
+
+.input-group>.form-control:focus,
+.input-group>.form-select:focus,
+.input-group>.form-floating:focus-within {
   z-index: 5;
 }
+
 .input-group .btn {
   position: relative;
   z-index: 2;
 }
+
 .input-group .btn:focus {
   z-index: 5;
 }
 
 .input-group-text {
   display: flex;
   align-items: center;
@@ -2533,58 +2930,61 @@
   text-align: center;
   white-space: nowrap;
   background-color: #e9ecef;
   border: 1px solid #ced4da;
   border-radius: 0.375rem;
 }
 
-.input-group-lg > .form-control,
-.input-group-lg > .form-select,
-.input-group-lg > .input-group-text,
-.input-group-lg > .btn {
+.input-group-lg>.form-control,
+.input-group-lg>.form-select,
+.input-group-lg>.input-group-text,
+.input-group-lg>.btn {
   padding: 0.5rem 1rem;
   font-size: 1.25rem;
   border-radius: 0.5rem;
 }
 
-.input-group-sm > .form-control,
-.input-group-sm > .form-select,
-.input-group-sm > .input-group-text,
-.input-group-sm > .btn {
+.input-group-sm>.form-control,
+.input-group-sm>.form-select,
+.input-group-sm>.input-group-text,
+.input-group-sm>.btn {
   padding: 0.25rem 0.5rem;
   font-size: 0.875rem;
   border-radius: 0.25rem;
 }
 
-.input-group-lg > .form-select,
-.input-group-sm > .form-select {
+.input-group-lg>.form-select,
+.input-group-sm>.form-select {
   padding-right: 3rem;
 }
 
-.input-group:not(.has-validation) > :not(:last-child):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),
-.input-group:not(.has-validation) > .dropdown-toggle:nth-last-child(n+3),
-.input-group:not(.has-validation) > .form-floating:not(:last-child) > .form-control,
-.input-group:not(.has-validation) > .form-floating:not(:last-child) > .form-select {
+.input-group:not(.has-validation)> :not(:last-child):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),
+.input-group:not(.has-validation)>.dropdown-toggle:nth-last-child(n+3),
+.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-control,
+.input-group:not(.has-validation)>.form-floating:not(:last-child)>.form-select {
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
 }
-.input-group.has-validation > :nth-last-child(n+3):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),
-.input-group.has-validation > .dropdown-toggle:nth-last-child(n+4),
-.input-group.has-validation > .form-floating:nth-last-child(n+3) > .form-control,
-.input-group.has-validation > .form-floating:nth-last-child(n+3) > .form-select {
+
+.input-group.has-validation> :nth-last-child(n+3):not(.dropdown-toggle):not(.dropdown-menu):not(.form-floating),
+.input-group.has-validation>.dropdown-toggle:nth-last-child(n+4),
+.input-group.has-validation>.form-floating:nth-last-child(n+3)>.form-control,
+.input-group.has-validation>.form-floating:nth-last-child(n+3)>.form-select {
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
 }
-.input-group > :not(:first-child):not(.dropdown-menu):not(.valid-tooltip):not(.valid-feedback):not(.invalid-tooltip):not(.invalid-feedback) {
+
+.input-group> :not(:first-child):not(.dropdown-menu):not(.valid-tooltip):not(.valid-feedback):not(.invalid-tooltip):not(.invalid-feedback) {
   margin-left: -1px;
   border-top-left-radius: 0;
   border-bottom-left-radius: 0;
 }
-.input-group > .form-floating:not(:first-child) > .form-control,
-.input-group > .form-floating:not(:first-child) > .form-select {
+
+.input-group>.form-floating:not(:first-child)>.form-control,
+.input-group>.form-floating:not(:first-child)>.form-select {
   border-top-left-radius: 0;
   border-bottom-left-radius: 0;
 }
 
 .valid-feedback {
   display: none;
   width: 100%;
@@ -2603,79 +3003,99 @@
   margin-top: 0.1rem;
   font-size: 0.875rem;
   color: #fff;
   background-color: rgba(25, 135, 84, 0.9);
   border-radius: 0.375rem;
 }
 
-.was-validated :valid ~ .valid-feedback,
-.was-validated :valid ~ .valid-tooltip,
-.is-valid ~ .valid-feedback,
-.is-valid ~ .valid-tooltip {
+.was-validated :valid~.valid-feedback,
+.was-validated :valid~.valid-tooltip,
+.is-valid~.valid-feedback,
+.is-valid~.valid-tooltip {
   display: block;
 }
 
-.was-validated .form-control:valid, .form-control.is-valid {
+.was-validated .form-control:valid,
+.form-control.is-valid {
   border-color: #198754;
   padding-right: calc(1.5em + 0.75rem);
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");
   background-repeat: no-repeat;
   background-position: right calc(0.375em + 0.1875rem) center;
   background-size: calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
-.was-validated .form-control:valid:focus, .form-control.is-valid:focus {
+
+.was-validated .form-control:valid:focus,
+.form-control.is-valid:focus {
   border-color: #198754;
   box-shadow: 0 0 0 0.25rem rgba(25, 135, 84, 0.25);
 }
 
-.was-validated textarea.form-control:valid, textarea.form-control.is-valid {
+.was-validated textarea.form-control:valid,
+textarea.form-control.is-valid {
   padding-right: calc(1.5em + 0.75rem);
   background-position: top calc(0.375em + 0.1875rem) right calc(0.375em + 0.1875rem);
 }
 
-.was-validated .form-select:valid, .form-select.is-valid {
+.was-validated .form-select:valid,
+.form-select.is-valid {
   border-color: #198754;
 }
-.was-validated .form-select:valid:not([multiple]):not([size]), .was-validated .form-select:valid:not([multiple])[size="1"], .form-select.is-valid:not([multiple]):not([size]), .form-select.is-valid:not([multiple])[size="1"] {
+
+.was-validated .form-select:valid:not([multiple]):not([size]),
+.was-validated .form-select:valid:not([multiple])[size="1"],
+.form-select.is-valid:not([multiple]):not([size]),
+.form-select.is-valid:not([multiple])[size="1"] {
   padding-right: 4.125rem;
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"), url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8 8'%3e%3cpath fill='%23198754' d='M2.3 6.73.6 4.53c-.4-1.04.46-1.4 1.1-.8l1.1 1.4 3.4-3.8c.6-.63 1.6-.27 1.2.7l-4 4.6c-.43.5-.8.4-1.1.1z'/%3e%3c/svg%3e");
   background-position: right 0.75rem center, center right 2.25rem;
   background-size: 16px 12px, calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
-.was-validated .form-select:valid:focus, .form-select.is-valid:focus {
+
+.was-validated .form-select:valid:focus,
+.form-select.is-valid:focus {
   border-color: #198754;
   box-shadow: 0 0 0 0.25rem rgba(25, 135, 84, 0.25);
 }
 
-.was-validated .form-control-color:valid, .form-control-color.is-valid {
+.was-validated .form-control-color:valid,
+.form-control-color.is-valid {
   width: calc(3rem + calc(1.5em + 0.75rem));
 }
 
-.was-validated .form-check-input:valid, .form-check-input.is-valid {
+.was-validated .form-check-input:valid,
+.form-check-input.is-valid {
   border-color: #198754;
 }
-.was-validated .form-check-input:valid:checked, .form-check-input.is-valid:checked {
+
+.was-validated .form-check-input:valid:checked,
+.form-check-input.is-valid:checked {
   background-color: #198754;
 }
-.was-validated .form-check-input:valid:focus, .form-check-input.is-valid:focus {
+
+.was-validated .form-check-input:valid:focus,
+.form-check-input.is-valid:focus {
   box-shadow: 0 0 0 0.25rem rgba(25, 135, 84, 0.25);
 }
-.was-validated .form-check-input:valid ~ .form-check-label, .form-check-input.is-valid ~ .form-check-label {
+
+.was-validated .form-check-input:valid~.form-check-label,
+.form-check-input.is-valid~.form-check-label {
   color: #198754;
 }
 
-.form-check-inline .form-check-input ~ .valid-feedback {
+.form-check-inline .form-check-input~.valid-feedback {
   margin-left: 0.5em;
 }
 
-.was-validated .input-group > .form-control:not(:focus):valid, .input-group > .form-control:not(:focus).is-valid,
-.was-validated .input-group > .form-select:not(:focus):valid,
-.input-group > .form-select:not(:focus).is-valid,
-.was-validated .input-group > .form-floating:not(:focus-within):valid,
-.input-group > .form-floating:not(:focus-within).is-valid {
+.was-validated .input-group>.form-control:not(:focus):valid,
+.input-group>.form-control:not(:focus).is-valid,
+.was-validated .input-group>.form-select:not(:focus):valid,
+.input-group>.form-select:not(:focus).is-valid,
+.was-validated .input-group>.form-floating:not(:focus-within):valid,
+.input-group>.form-floating:not(:focus-within).is-valid {
   z-index: 3;
 }
 
 .invalid-feedback {
   display: none;
   width: 100%;
   margin-top: 0.25rem;
@@ -2693,79 +3113,99 @@
   margin-top: 0.1rem;
   font-size: 0.875rem;
   color: #fff;
   background-color: rgba(220, 53, 69, 0.9);
   border-radius: 0.375rem;
 }
 
-.was-validated :invalid ~ .invalid-feedback,
-.was-validated :invalid ~ .invalid-tooltip,
-.is-invalid ~ .invalid-feedback,
-.is-invalid ~ .invalid-tooltip {
+.was-validated :invalid~.invalid-feedback,
+.was-validated :invalid~.invalid-tooltip,
+.is-invalid~.invalid-feedback,
+.is-invalid~.invalid-tooltip {
   display: block;
 }
 
-.was-validated .form-control:invalid, .form-control.is-invalid {
+.was-validated .form-control:invalid,
+.form-control.is-invalid {
   border-color: #dc3545;
   padding-right: calc(1.5em + 0.75rem);
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");
   background-repeat: no-repeat;
   background-position: right calc(0.375em + 0.1875rem) center;
   background-size: calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
-.was-validated .form-control:invalid:focus, .form-control.is-invalid:focus {
+
+.was-validated .form-control:invalid:focus,
+.form-control.is-invalid:focus {
   border-color: #dc3545;
   box-shadow: 0 0 0 0.25rem rgba(220, 53, 69, 0.25);
 }
 
-.was-validated textarea.form-control:invalid, textarea.form-control.is-invalid {
+.was-validated textarea.form-control:invalid,
+textarea.form-control.is-invalid {
   padding-right: calc(1.5em + 0.75rem);
   background-position: top calc(0.375em + 0.1875rem) right calc(0.375em + 0.1875rem);
 }
 
-.was-validated .form-select:invalid, .form-select.is-invalid {
+.was-validated .form-select:invalid,
+.form-select.is-invalid {
   border-color: #dc3545;
 }
-.was-validated .form-select:invalid:not([multiple]):not([size]), .was-validated .form-select:invalid:not([multiple])[size="1"], .form-select.is-invalid:not([multiple]):not([size]), .form-select.is-invalid:not([multiple])[size="1"] {
+
+.was-validated .form-select:invalid:not([multiple]):not([size]),
+.was-validated .form-select:invalid:not([multiple])[size="1"],
+.form-select.is-invalid:not([multiple]):not([size]),
+.form-select.is-invalid:not([multiple])[size="1"] {
   padding-right: 4.125rem;
   background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23343a40' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='m2 5 6 6 6-6'/%3e%3c/svg%3e"), url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 12 12' width='12' height='12' fill='none' stroke='%23dc3545'%3e%3ccircle cx='6' cy='6' r='4.5'/%3e%3cpath stroke-linejoin='round' d='M5.8 3.6h.4L6 6.5z'/%3e%3ccircle cx='6' cy='8.2' r='.6' fill='%23dc3545' stroke='none'/%3e%3c/svg%3e");
   background-position: right 0.75rem center, center right 2.25rem;
   background-size: 16px 12px, calc(0.75em + 0.375rem) calc(0.75em + 0.375rem);
 }
-.was-validated .form-select:invalid:focus, .form-select.is-invalid:focus {
+
+.was-validated .form-select:invalid:focus,
+.form-select.is-invalid:focus {
   border-color: #dc3545;
   box-shadow: 0 0 0 0.25rem rgba(220, 53, 69, 0.25);
 }
 
-.was-validated .form-control-color:invalid, .form-control-color.is-invalid {
+.was-validated .form-control-color:invalid,
+.form-control-color.is-invalid {
   width: calc(3rem + calc(1.5em + 0.75rem));
 }
 
-.was-validated .form-check-input:invalid, .form-check-input.is-invalid {
+.was-validated .form-check-input:invalid,
+.form-check-input.is-invalid {
   border-color: #dc3545;
 }
-.was-validated .form-check-input:invalid:checked, .form-check-input.is-invalid:checked {
+
+.was-validated .form-check-input:invalid:checked,
+.form-check-input.is-invalid:checked {
   background-color: #dc3545;
 }
-.was-validated .form-check-input:invalid:focus, .form-check-input.is-invalid:focus {
+
+.was-validated .form-check-input:invalid:focus,
+.form-check-input.is-invalid:focus {
   box-shadow: 0 0 0 0.25rem rgba(220, 53, 69, 0.25);
 }
-.was-validated .form-check-input:invalid ~ .form-check-label, .form-check-input.is-invalid ~ .form-check-label {
+
+.was-validated .form-check-input:invalid~.form-check-label,
+.form-check-input.is-invalid~.form-check-label {
   color: #dc3545;
 }
 
-.form-check-inline .form-check-input ~ .invalid-feedback {
+.form-check-inline .form-check-input~.invalid-feedback {
   margin-left: 0.5em;
 }
 
-.was-validated .input-group > .form-control:not(:focus):invalid, .input-group > .form-control:not(:focus).is-invalid,
-.was-validated .input-group > .form-select:not(:focus):invalid,
-.input-group > .form-select:not(:focus).is-invalid,
-.was-validated .input-group > .form-floating:not(:focus-within):invalid,
-.input-group > .form-floating:not(:focus-within).is-invalid {
+.was-validated .input-group>.form-control:not(:focus):invalid,
+.input-group>.form-control:not(:focus).is-invalid,
+.was-validated .input-group>.form-select:not(:focus):invalid,
+.input-group>.form-select:not(:focus).is-invalid,
+.was-validated .input-group>.form-floating:not(:focus-within):invalid,
+.input-group>.form-floating:not(:focus-within).is-invalid {
   z-index: 4;
 }
 
 .btn {
   --bs-btn-padding-x: 0.75rem;
   --bs-btn-padding-y: 0.375rem;
   --bs-btn-font-family: ;
@@ -2789,57 +3229,75 @@
   line-height: var(--bs-btn-line-height);
   color: var(--bs-btn-color);
   text-align: center;
   text-decoration: none;
   vertical-align: middle;
   cursor: pointer;
   -webkit-user-select: none;
-     -moz-user-select: none;
-          user-select: none;
+  -moz-user-select: none;
+  user-select: none;
   border: var(--bs-btn-border-width) solid var(--bs-btn-border-color);
   border-radius: var(--bs-btn-border-radius);
   background-color: var(--bs-btn-bg);
   transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .btn {
     transition: none;
   }
 }
+
 .btn:hover {
   color: var(--bs-btn-hover-color);
   background-color: var(--bs-btn-hover-bg);
   border-color: var(--bs-btn-hover-border-color);
 }
-.btn-check + .btn:hover {
+
+.btn-check+.btn:hover {
   color: var(--bs-btn-color);
   background-color: var(--bs-btn-bg);
   border-color: var(--bs-btn-border-color);
 }
+
 .btn:focus-visible {
   color: var(--bs-btn-hover-color);
   background-color: var(--bs-btn-hover-bg);
   border-color: var(--bs-btn-hover-border-color);
   outline: 0;
   box-shadow: var(--bs-btn-focus-box-shadow);
 }
-.btn-check:focus-visible + .btn {
+
+.btn-check:focus-visible+.btn {
   border-color: var(--bs-btn-hover-border-color);
   outline: 0;
   box-shadow: var(--bs-btn-focus-box-shadow);
 }
-.btn-check:checked + .btn, :not(.btn-check) + .btn:active, .btn:first-child:active, .btn.active, .btn.show {
+
+.btn-check:checked+.btn,
+:not(.btn-check)+.btn:active,
+.btn:first-child:active,
+.btn.active,
+.btn.show {
   color: var(--bs-btn-active-color);
   background-color: var(--bs-btn-active-bg);
   border-color: var(--bs-btn-active-border-color);
 }
-.btn-check:checked + .btn:focus-visible, :not(.btn-check) + .btn:active:focus-visible, .btn:first-child:active:focus-visible, .btn.active:focus-visible, .btn.show:focus-visible {
+
+.btn-check:checked+.btn:focus-visible,
+:not(.btn-check)+.btn:active:focus-visible,
+.btn:first-child:active:focus-visible,
+.btn.active:focus-visible,
+.btn.show:focus-visible {
   box-shadow: var(--bs-btn-focus-box-shadow);
 }
-.btn:disabled, .btn.disabled, fieldset:disabled .btn {
+
+.btn:disabled,
+.btn.disabled,
+fieldset:disabled .btn {
   color: var(--bs-btn-disabled-color);
   pointer-events: none;
   background-color: var(--bs-btn-disabled-bg);
   border-color: var(--bs-btn-disabled-border-color);
   opacity: var(--bs-btn-disabled-opacity);
 }
 
@@ -3126,66 +3584,75 @@
   --bs-btn-active-border-color: transparent;
   --bs-btn-disabled-color: #6c757d;
   --bs-btn-disabled-border-color: transparent;
   --bs-btn-box-shadow: none;
   --bs-btn-focus-shadow-rgb: 49, 132, 253;
   text-decoration: underline;
 }
+
 .btn-link:focus-visible {
   color: var(--bs-btn-color);
 }
+
 .btn-link:hover {
   color: var(--bs-btn-hover-color);
 }
 
-.btn-lg, .btn-group-lg > .btn {
+.btn-lg,
+.btn-group-lg>.btn {
   --bs-btn-padding-y: 0.5rem;
   --bs-btn-padding-x: 1rem;
   --bs-btn-font-size: 1.25rem;
   --bs-btn-border-radius: 0.5rem;
 }
 
-.btn-sm, .btn-group-sm > .btn {
+.btn-sm,
+.btn-group-sm>.btn {
   --bs-btn-padding-y: 0.25rem;
   --bs-btn-padding-x: 0.5rem;
   --bs-btn-font-size: 0.875rem;
   --bs-btn-border-radius: 0.25rem;
 }
 
 .fade {
   transition: opacity 0.15s linear;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .fade {
     transition: none;
   }
 }
+
 .fade:not(.show) {
   opacity: 0;
 }
 
 .collapse:not(.show) {
   display: none;
 }
 
 .collapsing {
   height: 0;
   overflow: hidden;
   transition: height 0.35s ease;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .collapsing {
     transition: none;
   }
 }
+
 .collapsing.collapse-horizontal {
   width: 0;
   height: auto;
   transition: width 0.35s ease;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .collapsing.collapse-horizontal {
     transition: none;
   }
 }
 
 .dropup,
@@ -3196,24 +3663,26 @@
 .dropdown-center {
   position: relative;
 }
 
 .dropdown-toggle {
   white-space: nowrap;
 }
+
 .dropdown-toggle::after {
   display: inline-block;
   margin-left: 0.255em;
   vertical-align: 0.255em;
   content: "";
   border-top: 0.3em solid;
   border-right: 0.3em solid transparent;
   border-bottom: 0;
   border-left: 0.3em solid transparent;
 }
+
 .dropdown-toggle:empty::after {
   margin-left: 0;
 }
 
 .dropdown-menu {
   --bs-dropdown-zindex: 1000;
   --bs-dropdown-min-width: 10rem;
@@ -3252,188 +3721,221 @@
   text-align: left;
   list-style: none;
   background-color: var(--bs-dropdown-bg);
   background-clip: padding-box;
   border: var(--bs-dropdown-border-width) solid var(--bs-dropdown-border-color);
   border-radius: var(--bs-dropdown-border-radius);
 }
+
 .dropdown-menu[data-bs-popper] {
   top: 100%;
   left: 0;
   margin-top: var(--bs-dropdown-spacer);
 }
 
 .dropdown-menu-start {
   --bs-position: start;
 }
+
 .dropdown-menu-start[data-bs-popper] {
   right: auto;
   left: 0;
 }
 
 .dropdown-menu-end {
   --bs-position: end;
 }
+
 .dropdown-menu-end[data-bs-popper] {
   right: 0;
   left: auto;
 }
 
 @media (min-width: 576px) {
   .dropdown-menu-sm-start {
     --bs-position: start;
   }
+
   .dropdown-menu-sm-start[data-bs-popper] {
     right: auto;
     left: 0;
   }
+
   .dropdown-menu-sm-end {
     --bs-position: end;
   }
+
   .dropdown-menu-sm-end[data-bs-popper] {
     right: 0;
     left: auto;
   }
 }
+
 @media (min-width: 768px) {
   .dropdown-menu-md-start {
     --bs-position: start;
   }
+
   .dropdown-menu-md-start[data-bs-popper] {
     right: auto;
     left: 0;
   }
+
   .dropdown-menu-md-end {
     --bs-position: end;
   }
+
   .dropdown-menu-md-end[data-bs-popper] {
     right: 0;
     left: auto;
   }
 }
+
 @media (min-width: 992px) {
   .dropdown-menu-lg-start {
     --bs-position: start;
   }
+
   .dropdown-menu-lg-start[data-bs-popper] {
     right: auto;
     left: 0;
   }
+
   .dropdown-menu-lg-end {
     --bs-position: end;
   }
+
   .dropdown-menu-lg-end[data-bs-popper] {
     right: 0;
     left: auto;
   }
 }
+
 @media (min-width: 1200px) {
   .dropdown-menu-xl-start {
     --bs-position: start;
   }
+
   .dropdown-menu-xl-start[data-bs-popper] {
     right: auto;
     left: 0;
   }
+
   .dropdown-menu-xl-end {
     --bs-position: end;
   }
+
   .dropdown-menu-xl-end[data-bs-popper] {
     right: 0;
     left: auto;
   }
 }
+
 @media (min-width: 1400px) {
   .dropdown-menu-xxl-start {
     --bs-position: start;
   }
+
   .dropdown-menu-xxl-start[data-bs-popper] {
     right: auto;
     left: 0;
   }
+
   .dropdown-menu-xxl-end {
     --bs-position: end;
   }
+
   .dropdown-menu-xxl-end[data-bs-popper] {
     right: 0;
     left: auto;
   }
 }
+
 .dropup .dropdown-menu[data-bs-popper] {
   top: auto;
   bottom: 100%;
   margin-top: 0;
   margin-bottom: var(--bs-dropdown-spacer);
 }
+
 .dropup .dropdown-toggle::after {
   display: inline-block;
   margin-left: 0.255em;
   vertical-align: 0.255em;
   content: "";
   border-top: 0;
   border-right: 0.3em solid transparent;
   border-bottom: 0.3em solid;
   border-left: 0.3em solid transparent;
 }
+
 .dropup .dropdown-toggle:empty::after {
   margin-left: 0;
 }
 
 .dropend .dropdown-menu[data-bs-popper] {
   top: 0;
   right: auto;
   left: 100%;
   margin-top: 0;
   margin-left: var(--bs-dropdown-spacer);
 }
+
 .dropend .dropdown-toggle::after {
   display: inline-block;
   margin-left: 0.255em;
   vertical-align: 0.255em;
   content: "";
   border-top: 0.3em solid transparent;
   border-right: 0;
   border-bottom: 0.3em solid transparent;
   border-left: 0.3em solid;
 }
+
 .dropend .dropdown-toggle:empty::after {
   margin-left: 0;
 }
+
 .dropend .dropdown-toggle::after {
   vertical-align: 0;
 }
 
 .dropstart .dropdown-menu[data-bs-popper] {
   top: 0;
   right: 100%;
   left: auto;
   margin-top: 0;
   margin-right: var(--bs-dropdown-spacer);
 }
+
 .dropstart .dropdown-toggle::after {
   display: inline-block;
   margin-left: 0.255em;
   vertical-align: 0.255em;
   content: "";
 }
+
 .dropstart .dropdown-toggle::after {
   display: none;
 }
+
 .dropstart .dropdown-toggle::before {
   display: inline-block;
   margin-right: 0.255em;
   vertical-align: 0.255em;
   content: "";
   border-top: 0.3em solid transparent;
   border-right: 0.3em solid;
   border-bottom: 0.3em solid transparent;
 }
+
 .dropstart .dropdown-toggle:empty::after {
   margin-left: 0;
 }
+
 .dropstart .dropdown-toggle::before {
   vertical-align: 0;
 }
 
 .dropdown-divider {
   height: 0;
   margin: var(--bs-dropdown-divider-margin-y) 0;
@@ -3451,24 +3953,30 @@
   color: var(--bs-dropdown-link-color);
   text-align: inherit;
   text-decoration: none;
   white-space: nowrap;
   background-color: transparent;
   border: 0;
 }
-.dropdown-item:hover, .dropdown-item:focus {
+
+.dropdown-item:hover,
+.dropdown-item:focus {
   color: var(--bs-dropdown-link-hover-color);
   background-color: var(--bs-dropdown-link-hover-bg);
 }
-.dropdown-item.active, .dropdown-item:active {
+
+.dropdown-item.active,
+.dropdown-item:active {
   color: var(--bs-dropdown-link-active-color);
   text-decoration: none;
   background-color: var(--bs-dropdown-link-active-bg);
 }
-.dropdown-item.disabled, .dropdown-item:disabled {
+
+.dropdown-item.disabled,
+.dropdown-item:disabled {
   color: var(--bs-dropdown-link-disabled-color);
   pointer-events: none;
   background-color: transparent;
 }
 
 .dropdown-menu.show {
   display: block;
@@ -3506,104 +4014,120 @@
 
 .btn-group,
 .btn-group-vertical {
   position: relative;
   display: inline-flex;
   vertical-align: middle;
 }
-.btn-group > .btn,
-.btn-group-vertical > .btn {
+
+.btn-group>.btn,
+.btn-group-vertical>.btn {
   position: relative;
   flex: 1 1 auto;
 }
-.btn-group > .btn-check:checked + .btn,
-.btn-group > .btn-check:focus + .btn,
-.btn-group > .btn:hover,
-.btn-group > .btn:focus,
-.btn-group > .btn:active,
-.btn-group > .btn.active,
-.btn-group-vertical > .btn-check:checked + .btn,
-.btn-group-vertical > .btn-check:focus + .btn,
-.btn-group-vertical > .btn:hover,
-.btn-group-vertical > .btn:focus,
-.btn-group-vertical > .btn:active,
-.btn-group-vertical > .btn.active {
+
+.btn-group>.btn-check:checked+.btn,
+.btn-group>.btn-check:focus+.btn,
+.btn-group>.btn:hover,
+.btn-group>.btn:focus,
+.btn-group>.btn:active,
+.btn-group>.btn.active,
+.btn-group-vertical>.btn-check:checked+.btn,
+.btn-group-vertical>.btn-check:focus+.btn,
+.btn-group-vertical>.btn:hover,
+.btn-group-vertical>.btn:focus,
+.btn-group-vertical>.btn:active,
+.btn-group-vertical>.btn.active {
   z-index: 1;
 }
 
 .btn-toolbar {
   display: flex;
   flex-wrap: wrap;
   justify-content: flex-start;
 }
+
 .btn-toolbar .input-group {
   width: auto;
 }
 
 .btn-group {
   border-radius: 0.375rem;
 }
-.btn-group > :not(.btn-check:first-child) + .btn,
-.btn-group > .btn-group:not(:first-child) {
+
+.btn-group> :not(.btn-check:first-child)+.btn,
+.btn-group>.btn-group:not(:first-child) {
   margin-left: -1px;
 }
-.btn-group > .btn:not(:last-child):not(.dropdown-toggle),
-.btn-group > .btn.dropdown-toggle-split:first-child,
-.btn-group > .btn-group:not(:last-child) > .btn {
+
+.btn-group>.btn:not(:last-child):not(.dropdown-toggle),
+.btn-group>.btn.dropdown-toggle-split:first-child,
+.btn-group>.btn-group:not(:last-child)>.btn {
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
 }
-.btn-group > .btn:nth-child(n+3),
-.btn-group > :not(.btn-check) + .btn,
-.btn-group > .btn-group:not(:first-child) > .btn {
+
+.btn-group>.btn:nth-child(n+3),
+.btn-group> :not(.btn-check)+.btn,
+.btn-group>.btn-group:not(:first-child)>.btn {
   border-top-left-radius: 0;
   border-bottom-left-radius: 0;
 }
 
 .dropdown-toggle-split {
   padding-right: 0.5625rem;
   padding-left: 0.5625rem;
 }
-.dropdown-toggle-split::after, .dropup .dropdown-toggle-split::after, .dropend .dropdown-toggle-split::after {
+
+.dropdown-toggle-split::after,
+.dropup .dropdown-toggle-split::after,
+.dropend .dropdown-toggle-split::after {
   margin-left: 0;
 }
+
 .dropstart .dropdown-toggle-split::before {
   margin-right: 0;
 }
 
-.btn-sm + .dropdown-toggle-split, .btn-group-sm > .btn + .dropdown-toggle-split {
+.btn-sm+.dropdown-toggle-split,
+.btn-group-sm>.btn+.dropdown-toggle-split {
   padding-right: 0.375rem;
   padding-left: 0.375rem;
 }
 
-.btn-lg + .dropdown-toggle-split, .btn-group-lg > .btn + .dropdown-toggle-split {
+.btn-lg+.dropdown-toggle-split,
+.btn-group-lg>.btn+.dropdown-toggle-split {
   padding-right: 0.75rem;
   padding-left: 0.75rem;
 }
 
 .btn-group-vertical {
   flex-direction: column;
   align-items: flex-start;
   justify-content: center;
 }
-.btn-group-vertical > .btn,
-.btn-group-vertical > .btn-group {
+
+.btn-group-vertical>.btn,
+.btn-group-vertical>.btn-group {
   width: 100%;
 }
-.btn-group-vertical > .btn:not(:first-child),
-.btn-group-vertical > .btn-group:not(:first-child) {
+
+.btn-group-vertical>.btn:not(:first-child),
+.btn-group-vertical>.btn-group:not(:first-child) {
   margin-top: -1px;
 }
-.btn-group-vertical > .btn:not(:last-child):not(.dropdown-toggle),
-.btn-group-vertical > .btn-group:not(:last-child) > .btn {
+
+.btn-group-vertical>.btn:not(:last-child):not(.dropdown-toggle),
+.btn-group-vertical>.btn-group:not(:last-child)>.btn {
   border-bottom-right-radius: 0;
   border-bottom-left-radius: 0;
 }
-.btn-group-vertical > .btn ~ .btn,
-.btn-group-vertical > .btn-group:not(:first-child) > .btn {
+
+.btn-group-vertical>.btn~.btn,
+.btn-group-vertical>.btn-group:not(:first-child)>.btn {
   border-top-left-radius: 0;
   border-top-right-radius: 0;
 }
 
 .nav {
   --bs-nav-link-padding-x: 1rem;
   --bs-nav-link-padding-y: 0.5rem;
@@ -3623,22 +4147,26 @@
   padding: var(--bs-nav-link-padding-y) var(--bs-nav-link-padding-x);
   font-size: var(--bs-nav-link-font-size);
   font-weight: var(--bs-nav-link-font-weight);
   color: var(--bs-nav-link-color);
   text-decoration: none;
   transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .nav-link {
     transition: none;
   }
 }
-.nav-link:hover, .nav-link:focus {
+
+.nav-link:hover,
+.nav-link:focus {
   color: var(--bs-nav-link-hover-color);
 }
+
 .nav-link.disabled {
   color: var(--bs-nav-link-disabled-color);
   pointer-events: none;
   cursor: default;
 }
 
 .nav-tabs {
@@ -3647,85 +4175,96 @@
   --bs-nav-tabs-border-radius: 0.375rem;
   --bs-nav-tabs-link-hover-border-color: #e9ecef #e9ecef #dee2e6;
   --bs-nav-tabs-link-active-color: #495057;
   --bs-nav-tabs-link-active-bg: #fff;
   --bs-nav-tabs-link-active-border-color: #dee2e6 #dee2e6 #fff;
   border-bottom: var(--bs-nav-tabs-border-width) solid var(--bs-nav-tabs-border-color);
 }
+
 .nav-tabs .nav-link {
   margin-bottom: calc(-1 * var(--bs-nav-tabs-border-width));
   background: none;
   border: var(--bs-nav-tabs-border-width) solid transparent;
   border-top-left-radius: var(--bs-nav-tabs-border-radius);
   border-top-right-radius: var(--bs-nav-tabs-border-radius);
 }
-.nav-tabs .nav-link:hover, .nav-tabs .nav-link:focus {
+
+.nav-tabs .nav-link:hover,
+.nav-tabs .nav-link:focus {
   isolation: isolate;
   border-color: var(--bs-nav-tabs-link-hover-border-color);
 }
-.nav-tabs .nav-link.disabled, .nav-tabs .nav-link:disabled {
+
+.nav-tabs .nav-link.disabled,
+.nav-tabs .nav-link:disabled {
   color: var(--bs-nav-link-disabled-color);
   background-color: transparent;
   border-color: transparent;
 }
+
 .nav-tabs .nav-link.active,
 .nav-tabs .nav-item.show .nav-link {
   color: var(--bs-nav-tabs-link-active-color);
   background-color: var(--bs-nav-tabs-link-active-bg);
   border-color: var(--bs-nav-tabs-link-active-border-color);
 }
+
 .nav-tabs .dropdown-menu {
   margin-top: calc(-1 * var(--bs-nav-tabs-border-width));
   border-top-left-radius: 0;
   border-top-right-radius: 0;
 }
 
 .nav-pills {
   --bs-nav-pills-border-radius: 0.375rem;
   --bs-nav-pills-link-active-color: #fff;
   --bs-nav-pills-link-active-bg: #0d6efd;
 }
+
 .nav-pills .nav-link {
   background: none;
   border: 0;
   border-radius: var(--bs-nav-pills-border-radius);
 }
+
 .nav-pills .nav-link:disabled {
   color: var(--bs-nav-link-disabled-color);
   background-color: transparent;
   border-color: transparent;
 }
+
 .nav-pills .nav-link.active,
-.nav-pills .show > .nav-link {
+.nav-pills .show>.nav-link {
   color: var(--bs-nav-pills-link-active-color);
   background-color: var(--bs-nav-pills-link-active-bg);
 }
 
-.nav-fill > .nav-link,
+.nav-fill>.nav-link,
 .nav-fill .nav-item {
   flex: 1 1 auto;
   text-align: center;
 }
 
-.nav-justified > .nav-link,
+.nav-justified>.nav-link,
 .nav-justified .nav-item {
   flex-basis: 0;
   flex-grow: 1;
   text-align: center;
 }
 
 .nav-fill .nav-item .nav-link,
 .nav-justified .nav-item .nav-link {
   width: 100%;
 }
 
-.tab-content > .tab-pane {
+.tab-content>.tab-pane {
   display: none;
 }
-.tab-content > .active {
+
+.tab-content>.active {
   display: block;
 }
 
 .navbar {
   --bs-navbar-padding-x: 0;
   --bs-navbar-padding-y: 0.5rem;
   --bs-navbar-color: rgba(0, 0, 0, 0.55);
@@ -3749,36 +4288,40 @@
   position: relative;
   display: flex;
   flex-wrap: wrap;
   align-items: center;
   justify-content: space-between;
   padding: var(--bs-navbar-padding-y) var(--bs-navbar-padding-x);
 }
-.navbar > .container,
-.navbar > .container-fluid,
-.navbar > .container-sm,
-.navbar > .container-md,
-.navbar > .container-lg,
-.navbar > .container-xl,
-.navbar > .container-xxl {
+
+.navbar>.container,
+.navbar>.container-fluid,
+.navbar>.container-sm,
+.navbar>.container-md,
+.navbar>.container-lg,
+.navbar>.container-xl,
+.navbar>.container-xxl {
   display: flex;
   flex-wrap: inherit;
   align-items: center;
   justify-content: space-between;
 }
+
 .navbar-brand {
   padding-top: var(--bs-navbar-brand-padding-y);
   padding-bottom: var(--bs-navbar-brand-padding-y);
   margin-right: var(--bs-navbar-brand-margin-end);
   font-size: var(--bs-navbar-brand-font-size);
   color: var(--bs-navbar-brand-color);
   text-decoration: none;
   white-space: nowrap;
 }
-.navbar-brand:hover, .navbar-brand:focus {
+
+.navbar-brand:hover,
+.navbar-brand:focus {
   color: var(--bs-navbar-brand-hover-color);
 }
 
 .navbar-nav {
   --bs-nav-link-padding-x: 0;
   --bs-nav-link-padding-y: 0.5rem;
   --bs-nav-link-font-weight: ;
@@ -3787,27 +4330,30 @@
   --bs-nav-link-disabled-color: var(--bs-navbar-disabled-color);
   display: flex;
   flex-direction: column;
   padding-left: 0;
   margin-bottom: 0;
   list-style: none;
 }
-.navbar-nav .show > .nav-link,
+
+.navbar-nav .show>.nav-link,
 .navbar-nav .nav-link.active {
   color: var(--bs-navbar-active-color);
 }
+
 .navbar-nav .dropdown-menu {
   position: static;
 }
 
 .navbar-text {
   padding-top: 0.5rem;
   padding-bottom: 0.5rem;
   color: var(--bs-navbar-color);
 }
+
 .navbar-text a,
 .navbar-text a:hover,
 .navbar-text a:focus {
   color: var(--bs-navbar-active-color);
 }
 
 .navbar-collapse {
@@ -3822,22 +4368,25 @@
   line-height: 1;
   color: var(--bs-navbar-color);
   background-color: transparent;
   border: var(--bs-border-width) solid var(--bs-navbar-toggler-border-color);
   border-radius: var(--bs-navbar-toggler-border-radius);
   transition: var(--bs-navbar-toggler-transition);
 }
+
 @media (prefers-reduced-motion: reduce) {
   .navbar-toggler {
     transition: none;
   }
 }
+
 .navbar-toggler:hover {
   text-decoration: none;
 }
+
 .navbar-toggler:focus {
   text-decoration: none;
   outline: 0;
   box-shadow: 0 0 0 var(--bs-navbar-toggler-focus-width);
 }
 
 .navbar-toggler-icon {
@@ -3857,283 +4406,342 @@
 }
 
 @media (min-width: 576px) {
   .navbar-expand-sm {
     flex-wrap: nowrap;
     justify-content: flex-start;
   }
+
   .navbar-expand-sm .navbar-nav {
     flex-direction: row;
   }
+
   .navbar-expand-sm .navbar-nav .dropdown-menu {
     position: absolute;
   }
+
   .navbar-expand-sm .navbar-nav .nav-link {
     padding-right: var(--bs-navbar-nav-link-padding-x);
     padding-left: var(--bs-navbar-nav-link-padding-x);
   }
+
   .navbar-expand-sm .navbar-nav-scroll {
     overflow: visible;
   }
+
   .navbar-expand-sm .navbar-collapse {
     display: flex !important;
     flex-basis: auto;
   }
+
   .navbar-expand-sm .navbar-toggler {
     display: none;
   }
+
   .navbar-expand-sm .offcanvas {
     position: static;
     z-index: auto;
     flex-grow: 1;
     width: auto !important;
     height: auto !important;
     visibility: visible !important;
     background-color: transparent !important;
     border: 0 !important;
     transform: none !important;
     transition: none;
   }
+
   .navbar-expand-sm .offcanvas .offcanvas-header {
     display: none;
   }
+
   .navbar-expand-sm .offcanvas .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
   }
 }
+
 @media (min-width: 768px) {
   .navbar-expand-md {
     flex-wrap: nowrap;
     justify-content: flex-start;
   }
+
   .navbar-expand-md .navbar-nav {
     flex-direction: row;
   }
+
   .navbar-expand-md .navbar-nav .dropdown-menu {
     position: absolute;
   }
+
   .navbar-expand-md .navbar-nav .nav-link {
     padding-right: var(--bs-navbar-nav-link-padding-x);
     padding-left: var(--bs-navbar-nav-link-padding-x);
   }
+
   .navbar-expand-md .navbar-nav-scroll {
     overflow: visible;
   }
+
   .navbar-expand-md .navbar-collapse {
     display: flex !important;
     flex-basis: auto;
   }
+
   .navbar-expand-md .navbar-toggler {
     display: none;
   }
+
   .navbar-expand-md .offcanvas {
     position: static;
     z-index: auto;
     flex-grow: 1;
     width: auto !important;
     height: auto !important;
     visibility: visible !important;
     background-color: transparent !important;
     border: 0 !important;
     transform: none !important;
     transition: none;
   }
+
   .navbar-expand-md .offcanvas .offcanvas-header {
     display: none;
   }
+
   .navbar-expand-md .offcanvas .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
   }
 }
+
 @media (min-width: 992px) {
   .navbar-expand-lg {
     flex-wrap: nowrap;
     justify-content: flex-start;
   }
+
   .navbar-expand-lg .navbar-nav {
     flex-direction: row;
   }
+
   .navbar-expand-lg .navbar-nav .dropdown-menu {
     position: absolute;
   }
+
   .navbar-expand-lg .navbar-nav .nav-link {
     padding-right: var(--bs-navbar-nav-link-padding-x);
     padding-left: var(--bs-navbar-nav-link-padding-x);
   }
+
   .navbar-expand-lg .navbar-nav-scroll {
     overflow: visible;
   }
+
   .navbar-expand-lg .navbar-collapse {
     display: flex !important;
     flex-basis: auto;
   }
+
   .navbar-expand-lg .navbar-toggler {
     display: none;
   }
+
   .navbar-expand-lg .offcanvas {
     position: static;
     z-index: auto;
     flex-grow: 1;
     width: auto !important;
     height: auto !important;
     visibility: visible !important;
     background-color: transparent !important;
     border: 0 !important;
     transform: none !important;
     transition: none;
   }
+
   .navbar-expand-lg .offcanvas .offcanvas-header {
     display: none;
   }
+
   .navbar-expand-lg .offcanvas .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
   }
 }
+
 @media (min-width: 1200px) {
   .navbar-expand-xl {
     flex-wrap: nowrap;
     justify-content: flex-start;
   }
+
   .navbar-expand-xl .navbar-nav {
     flex-direction: row;
   }
+
   .navbar-expand-xl .navbar-nav .dropdown-menu {
     position: absolute;
   }
+
   .navbar-expand-xl .navbar-nav .nav-link {
     padding-right: var(--bs-navbar-nav-link-padding-x);
     padding-left: var(--bs-navbar-nav-link-padding-x);
   }
+
   .navbar-expand-xl .navbar-nav-scroll {
     overflow: visible;
   }
+
   .navbar-expand-xl .navbar-collapse {
     display: flex !important;
     flex-basis: auto;
   }
+
   .navbar-expand-xl .navbar-toggler {
     display: none;
   }
+
   .navbar-expand-xl .offcanvas {
     position: static;
     z-index: auto;
     flex-grow: 1;
     width: auto !important;
     height: auto !important;
     visibility: visible !important;
     background-color: transparent !important;
     border: 0 !important;
     transform: none !important;
     transition: none;
   }
+
   .navbar-expand-xl .offcanvas .offcanvas-header {
     display: none;
   }
+
   .navbar-expand-xl .offcanvas .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
   }
 }
+
 @media (min-width: 1400px) {
   .navbar-expand-xxl {
     flex-wrap: nowrap;
     justify-content: flex-start;
   }
+
   .navbar-expand-xxl .navbar-nav {
     flex-direction: row;
   }
+
   .navbar-expand-xxl .navbar-nav .dropdown-menu {
     position: absolute;
   }
+
   .navbar-expand-xxl .navbar-nav .nav-link {
     padding-right: var(--bs-navbar-nav-link-padding-x);
     padding-left: var(--bs-navbar-nav-link-padding-x);
   }
+
   .navbar-expand-xxl .navbar-nav-scroll {
     overflow: visible;
   }
+
   .navbar-expand-xxl .navbar-collapse {
     display: flex !important;
     flex-basis: auto;
   }
+
   .navbar-expand-xxl .navbar-toggler {
     display: none;
   }
+
   .navbar-expand-xxl .offcanvas {
     position: static;
     z-index: auto;
     flex-grow: 1;
     width: auto !important;
     height: auto !important;
     visibility: visible !important;
     background-color: transparent !important;
     border: 0 !important;
     transform: none !important;
     transition: none;
   }
+
   .navbar-expand-xxl .offcanvas .offcanvas-header {
     display: none;
   }
+
   .navbar-expand-xxl .offcanvas .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
   }
 }
+
 .navbar-expand {
   flex-wrap: nowrap;
   justify-content: flex-start;
 }
+
 .navbar-expand .navbar-nav {
   flex-direction: row;
 }
+
 .navbar-expand .navbar-nav .dropdown-menu {
   position: absolute;
 }
+
 .navbar-expand .navbar-nav .nav-link {
   padding-right: var(--bs-navbar-nav-link-padding-x);
   padding-left: var(--bs-navbar-nav-link-padding-x);
 }
+
 .navbar-expand .navbar-nav-scroll {
   overflow: visible;
 }
+
 .navbar-expand .navbar-collapse {
   display: flex !important;
   flex-basis: auto;
 }
+
 .navbar-expand .navbar-toggler {
   display: none;
 }
+
 .navbar-expand .offcanvas {
   position: static;
   z-index: auto;
   flex-grow: 1;
   width: auto !important;
   height: auto !important;
   visibility: visible !important;
   background-color: transparent !important;
   border: 0 !important;
   transform: none !important;
   transition: none;
 }
+
 .navbar-expand .offcanvas .offcanvas-header {
   display: none;
 }
+
 .navbar-expand .offcanvas .offcanvas-body {
   display: flex;
   flex-grow: 0;
   padding: 0;
   overflow-y: visible;
 }
 
@@ -4173,34 +4781,39 @@
   height: var(--bs-card-height);
   word-wrap: break-word;
   background-color: var(--bs-card-bg);
   background-clip: border-box;
   border: var(--bs-card-border-width) solid var(--bs-card-border-color);
   border-radius: var(--bs-card-border-radius);
 }
-.card > hr {
+
+.card>hr {
   margin-right: 0;
   margin-left: 0;
 }
-.card > .list-group {
+
+.card>.list-group {
   border-top: inherit;
   border-bottom: inherit;
 }
-.card > .list-group:first-child {
+
+.card>.list-group:first-child {
   border-top-width: 0;
   border-top-left-radius: var(--bs-card-inner-border-radius);
   border-top-right-radius: var(--bs-card-inner-border-radius);
 }
-.card > .list-group:last-child {
+
+.card>.list-group:last-child {
   border-bottom-width: 0;
   border-bottom-right-radius: var(--bs-card-inner-border-radius);
   border-bottom-left-radius: var(--bs-card-inner-border-radius);
 }
-.card > .card-header + .list-group,
-.card > .list-group + .card-footer {
+
+.card>.card-header+.list-group,
+.card>.list-group+.card-footer {
   border-top: 0;
 }
 
 .card-body {
   flex: 1 1 auto;
   padding: var(--bs-card-spacer-y) var(--bs-card-spacer-x);
   color: var(--bs-card-color);
@@ -4215,45 +4828,48 @@
   margin-bottom: 0;
 }
 
 .card-text:last-child {
   margin-bottom: 0;
 }
 
-.card-link + .card-link {
+.card-link+.card-link {
   margin-left: var(--bs-card-spacer-x);
 }
 
 .card-header {
   padding: var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);
   margin-bottom: 0;
   color: var(--bs-card-cap-color);
   background-color: var(--bs-card-cap-bg);
   border-bottom: var(--bs-card-border-width) solid var(--bs-card-border-color);
 }
+
 .card-header:first-child {
   border-radius: var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius) 0 0;
 }
 
 .card-footer {
   padding: var(--bs-card-cap-padding-y) var(--bs-card-cap-padding-x);
   color: var(--bs-card-cap-color);
   background-color: var(--bs-card-cap-bg);
   border-top: var(--bs-card-border-width) solid var(--bs-card-border-color);
 }
+
 .card-footer:last-child {
   border-radius: 0 0 var(--bs-card-inner-border-radius) var(--bs-card-inner-border-radius);
 }
 
 .card-header-tabs {
   margin-right: calc(-0.5 * var(--bs-card-cap-padding-x));
   margin-bottom: calc(-1 * var(--bs-card-cap-padding-y));
   margin-left: calc(-0.5 * var(--bs-card-cap-padding-x));
   border-bottom: 0;
 }
+
 .card-header-tabs .nav-link.active {
   background-color: var(--bs-card-bg);
   border-bottom-color: var(--bs-card-bg);
 }
 
 .card-header-pills {
   margin-right: calc(-0.5 * var(--bs-card-cap-padding-x));
@@ -4284,52 +4900,61 @@
 
 .card-img,
 .card-img-bottom {
   border-bottom-right-radius: var(--bs-card-inner-border-radius);
   border-bottom-left-radius: var(--bs-card-inner-border-radius);
 }
 
-.card-group > .card {
+.card-group>.card {
   margin-bottom: var(--bs-card-group-margin);
 }
+
 @media (min-width: 576px) {
   .card-group {
     display: flex;
     flex-flow: row wrap;
   }
-  .card-group > .card {
+
+  .card-group>.card {
     flex: 1 0 0%;
     margin-bottom: 0;
   }
-  .card-group > .card + .card {
+
+  .card-group>.card+.card {
     margin-left: 0;
     border-left: 0;
   }
-  .card-group > .card:not(:last-child) {
+
+  .card-group>.card:not(:last-child) {
     border-top-right-radius: 0;
     border-bottom-right-radius: 0;
   }
-  .card-group > .card:not(:last-child) .card-img-top,
-  .card-group > .card:not(:last-child) .card-header {
+
+  .card-group>.card:not(:last-child) .card-img-top,
+  .card-group>.card:not(:last-child) .card-header {
     border-top-right-radius: 0;
   }
-  .card-group > .card:not(:last-child) .card-img-bottom,
-  .card-group > .card:not(:last-child) .card-footer {
+
+  .card-group>.card:not(:last-child) .card-img-bottom,
+  .card-group>.card:not(:last-child) .card-footer {
     border-bottom-right-radius: 0;
   }
-  .card-group > .card:not(:first-child) {
+
+  .card-group>.card:not(:first-child) {
     border-top-left-radius: 0;
     border-bottom-left-radius: 0;
   }
-  .card-group > .card:not(:first-child) .card-img-top,
-  .card-group > .card:not(:first-child) .card-header {
+
+  .card-group>.card:not(:first-child) .card-img-top,
+  .card-group>.card:not(:first-child) .card-header {
     border-top-left-radius: 0;
   }
-  .card-group > .card:not(:first-child) .card-img-bottom,
-  .card-group > .card:not(:first-child) .card-footer {
+
+  .card-group>.card:not(:first-child) .card-img-bottom,
+  .card-group>.card:not(:first-child) .card-footer {
     border-bottom-left-radius: 0;
   }
 }
 
 .accordion {
   --bs-accordion-color: #212529;
   --bs-accordion-bg: #fff;
@@ -4366,47 +4991,54 @@
   text-align: left;
   background-color: var(--bs-accordion-btn-bg);
   border: 0;
   border-radius: 0;
   overflow-anchor: none;
   transition: var(--bs-accordion-transition);
 }
+
 @media (prefers-reduced-motion: reduce) {
   .accordion-button {
     transition: none;
   }
 }
+
 .accordion-button:not(.collapsed) {
   color: var(--bs-accordion-active-color);
   background-color: var(--bs-accordion-active-bg);
   box-shadow: inset 0 calc(-1 * var(--bs-accordion-border-width)) 0 var(--bs-accordion-border-color);
 }
+
 .accordion-button:not(.collapsed)::after {
   background-image: var(--bs-accordion-btn-active-icon);
   transform: var(--bs-accordion-btn-icon-transform);
 }
+
 .accordion-button::after {
   flex-shrink: 0;
   width: var(--bs-accordion-btn-icon-width);
   height: var(--bs-accordion-btn-icon-width);
   margin-left: auto;
   content: "";
   background-image: var(--bs-accordion-btn-icon);
   background-repeat: no-repeat;
   background-size: var(--bs-accordion-btn-icon-width);
   transition: var(--bs-accordion-btn-icon-transition);
 }
+
 @media (prefers-reduced-motion: reduce) {
   .accordion-button::after {
     transition: none;
   }
 }
+
 .accordion-button:hover {
   z-index: 2;
 }
+
 .accordion-button:focus {
   z-index: 3;
   border-color: var(--bs-accordion-btn-focus-border-color);
   outline: 0;
   box-shadow: var(--bs-accordion-btn-focus-box-shadow);
 }
 
@@ -4415,57 +5047,68 @@
 }
 
 .accordion-item {
   color: var(--bs-accordion-color);
   background-color: var(--bs-accordion-bg);
   border: var(--bs-accordion-border-width) solid var(--bs-accordion-border-color);
 }
+
 .accordion-item:first-of-type {
   border-top-left-radius: var(--bs-accordion-border-radius);
   border-top-right-radius: var(--bs-accordion-border-radius);
 }
+
 .accordion-item:first-of-type .accordion-button {
   border-top-left-radius: var(--bs-accordion-inner-border-radius);
   border-top-right-radius: var(--bs-accordion-inner-border-radius);
 }
+
 .accordion-item:not(:first-of-type) {
   border-top: 0;
 }
+
 .accordion-item:last-of-type {
   border-bottom-right-radius: var(--bs-accordion-border-radius);
   border-bottom-left-radius: var(--bs-accordion-border-radius);
 }
+
 .accordion-item:last-of-type .accordion-button.collapsed {
   border-bottom-right-radius: var(--bs-accordion-inner-border-radius);
   border-bottom-left-radius: var(--bs-accordion-inner-border-radius);
 }
+
 .accordion-item:last-of-type .accordion-collapse {
   border-bottom-right-radius: var(--bs-accordion-border-radius);
   border-bottom-left-radius: var(--bs-accordion-border-radius);
 }
 
 .accordion-body {
   padding: var(--bs-accordion-body-padding-y) var(--bs-accordion-body-padding-x);
 }
 
 .accordion-flush .accordion-collapse {
   border-width: 0;
 }
+
 .accordion-flush .accordion-item {
   border-right: 0;
   border-left: 0;
   border-radius: 0;
 }
+
 .accordion-flush .accordion-item:first-child {
   border-top: 0;
 }
+
 .accordion-flush .accordion-item:last-child {
   border-bottom: 0;
 }
-.accordion-flush .accordion-item .accordion-button, .accordion-flush .accordion-item .accordion-button.collapsed {
+
+.accordion-flush .accordion-item .accordion-button,
+.accordion-flush .accordion-item .accordion-button.collapsed {
   border-radius: 0;
 }
 
 .breadcrumb {
   --bs-breadcrumb-padding-x: 0;
   --bs-breadcrumb-padding-y: 0;
   --bs-breadcrumb-margin-bottom: 1rem;
@@ -4480,23 +5123,27 @@
   margin-bottom: var(--bs-breadcrumb-margin-bottom);
   font-size: var(--bs-breadcrumb-font-size);
   list-style: none;
   background-color: var(--bs-breadcrumb-bg);
   border-radius: var(--bs-breadcrumb-border-radius);
 }
 
-.breadcrumb-item + .breadcrumb-item {
+.breadcrumb-item+.breadcrumb-item {
   padding-left: var(--bs-breadcrumb-item-padding-x);
 }
-.breadcrumb-item + .breadcrumb-item::before {
+
+.breadcrumb-item+.breadcrumb-item::before {
   float: left;
   padding-right: var(--bs-breadcrumb-item-padding-x);
   color: var(--bs-breadcrumb-divider-color);
-  content: var(--bs-breadcrumb-divider, "/") /* rtl: var(--bs-breadcrumb-divider, "/") */;
+  content: var(--bs-breadcrumb-divider, "/")
+    /* rtl: var(--bs-breadcrumb-divider, "/") */
+  ;
 }
+
 .breadcrumb-item.active {
   color: var(--bs-breadcrumb-item-active-color);
 }
 
 .pagination {
   --bs-pagination-padding-x: 0.75rem;
   --bs-pagination-padding-y: 0.375rem;
@@ -4530,52 +5177,61 @@
   font-size: var(--bs-pagination-font-size);
   color: var(--bs-pagination-color);
   text-decoration: none;
   background-color: var(--bs-pagination-bg);
   border: var(--bs-pagination-border-width) solid var(--bs-pagination-border-color);
   transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out, border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .page-link {
     transition: none;
   }
 }
+
 .page-link:hover {
   z-index: 2;
   color: var(--bs-pagination-hover-color);
   background-color: var(--bs-pagination-hover-bg);
   border-color: var(--bs-pagination-hover-border-color);
 }
+
 .page-link:focus {
   z-index: 3;
   color: var(--bs-pagination-focus-color);
   background-color: var(--bs-pagination-focus-bg);
   outline: 0;
   box-shadow: var(--bs-pagination-focus-box-shadow);
 }
-.page-link.active, .active > .page-link {
+
+.page-link.active,
+.active>.page-link {
   z-index: 3;
   color: var(--bs-pagination-active-color);
   background-color: var(--bs-pagination-active-bg);
   border-color: var(--bs-pagination-active-border-color);
 }
-.page-link.disabled, .disabled > .page-link {
+
+.page-link.disabled,
+.disabled>.page-link {
   color: var(--bs-pagination-disabled-color);
   pointer-events: none;
   background-color: var(--bs-pagination-disabled-bg);
   border-color: var(--bs-pagination-disabled-border-color);
 }
 
 .page-item:not(:first-child) .page-link {
   margin-left: -1px;
 }
+
 .page-item:first-child .page-link {
   border-top-left-radius: var(--bs-pagination-border-radius);
   border-bottom-left-radius: var(--bs-pagination-border-radius);
 }
+
 .page-item:last-child .page-link {
   border-top-right-radius: var(--bs-pagination-border-radius);
   border-bottom-right-radius: var(--bs-pagination-border-radius);
 }
 
 .pagination-lg {
   --bs-pagination-padding-x: 1.5rem;
@@ -4605,14 +5261,15 @@
   line-height: 1;
   color: var(--bs-badge-color);
   text-align: center;
   white-space: nowrap;
   vertical-align: baseline;
   border-radius: var(--bs-badge-border-radius);
 }
+
 .badge:empty {
   display: none;
 }
 
 .btn .badge {
   position: relative;
   top: -1px;
@@ -4643,99 +5300,109 @@
 .alert-link {
   font-weight: 700;
 }
 
 .alert-dismissible {
   padding-right: 3rem;
 }
+
 .alert-dismissible .btn-close {
   position: absolute;
   top: 0;
   right: 0;
   z-index: 2;
   padding: 1.25rem 1rem;
 }
 
 .alert-primary {
   --bs-alert-color: #084298;
   --bs-alert-bg: #cfe2ff;
   --bs-alert-border-color: #b6d4fe;
 }
+
 .alert-primary .alert-link {
   color: #06357a;
 }
 
 .alert-secondary {
   --bs-alert-color: #41464b;
   --bs-alert-bg: #e2e3e5;
   --bs-alert-border-color: #d3d6d8;
 }
+
 .alert-secondary .alert-link {
   color: #34383c;
 }
 
 .alert-success {
   --bs-alert-color: #0f5132;
   --bs-alert-bg: #d1e7dd;
   --bs-alert-border-color: #badbcc;
 }
+
 .alert-success .alert-link {
   color: #0c4128;
 }
 
 .alert-info {
   --bs-alert-color: #055160;
   --bs-alert-bg: #cff4fc;
   --bs-alert-border-color: #b6effb;
 }
+
 .alert-info .alert-link {
   color: #04414d;
 }
 
 .alert-warning {
   --bs-alert-color: #664d03;
   --bs-alert-bg: #fff3cd;
   --bs-alert-border-color: #ffecb5;
 }
+
 .alert-warning .alert-link {
   color: #523e02;
 }
 
 .alert-danger {
   --bs-alert-color: #842029;
   --bs-alert-bg: #f8d7da;
   --bs-alert-border-color: #f5c2c7;
 }
+
 .alert-danger .alert-link {
   color: #6a1a21;
 }
 
 .alert-light {
   --bs-alert-color: #636464;
   --bs-alert-bg: #fefefe;
   --bs-alert-border-color: #fdfdfe;
 }
+
 .alert-light .alert-link {
   color: #4f5050;
 }
 
 .alert-dark {
   --bs-alert-color: #141619;
   --bs-alert-bg: #d3d3d4;
   --bs-alert-border-color: #bcbebf;
 }
+
 .alert-dark .alert-link {
   color: #101214;
 }
 
 @keyframes progress-bar-stripes {
   0% {
     background-position-x: 1rem;
   }
 }
+
 .progress {
   --bs-progress-height: 1rem;
   --bs-progress-font-size: 0.75rem;
   --bs-progress-bg: #e9ecef;
   --bs-progress-border-radius: 0.375rem;
   --bs-progress-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.075);
   --bs-progress-bar-color: #fff;
@@ -4756,28 +5423,30 @@
   overflow: hidden;
   color: var(--bs-progress-bar-color);
   text-align: center;
   white-space: nowrap;
   background-color: var(--bs-progress-bar-bg);
   transition: var(--bs-progress-bar-transition);
 }
+
 @media (prefers-reduced-motion: reduce) {
   .progress-bar {
     transition: none;
   }
 }
 
 .progress-bar-striped {
   background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
   background-size: var(--bs-progress-height) var(--bs-progress-height);
 }
 
 .progress-bar-animated {
   animation: 1s linear infinite progress-bar-stripes;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .progress-bar-animated {
     animation: none;
   }
 }
 
 .list-group {
@@ -4805,330 +5474,402 @@
   border-radius: var(--bs-list-group-border-radius);
 }
 
 .list-group-numbered {
   list-style-type: none;
   counter-reset: section;
 }
-.list-group-numbered > .list-group-item::before {
+
+.list-group-numbered>.list-group-item::before {
   content: counters(section, ".") ". ";
   counter-increment: section;
 }
 
 .list-group-item-action {
   width: 100%;
   color: var(--bs-list-group-action-color);
   text-align: inherit;
 }
-.list-group-item-action:hover, .list-group-item-action:focus {
+
+.list-group-item-action:hover,
+.list-group-item-action:focus {
   z-index: 1;
   color: var(--bs-list-group-action-hover-color);
   text-decoration: none;
   background-color: var(--bs-list-group-action-hover-bg);
 }
+
 .list-group-item-action:active {
   color: var(--bs-list-group-action-active-color);
   background-color: var(--bs-list-group-action-active-bg);
 }
 
 .list-group-item {
   position: relative;
   display: block;
   padding: var(--bs-list-group-item-padding-y) var(--bs-list-group-item-padding-x);
   color: var(--bs-list-group-color);
   text-decoration: none;
   background-color: var(--bs-list-group-bg);
   border: var(--bs-list-group-border-width) solid var(--bs-list-group-border-color);
 }
+
 .list-group-item:first-child {
   border-top-left-radius: inherit;
   border-top-right-radius: inherit;
 }
+
 .list-group-item:last-child {
   border-bottom-right-radius: inherit;
   border-bottom-left-radius: inherit;
 }
-.list-group-item.disabled, .list-group-item:disabled {
+
+.list-group-item.disabled,
+.list-group-item:disabled {
   color: var(--bs-list-group-disabled-color);
   pointer-events: none;
   background-color: var(--bs-list-group-disabled-bg);
 }
+
 .list-group-item.active {
   z-index: 2;
   color: var(--bs-list-group-active-color);
   background-color: var(--bs-list-group-active-bg);
   border-color: var(--bs-list-group-active-border-color);
 }
-.list-group-item + .list-group-item {
+
+.list-group-item+.list-group-item {
   border-top-width: 0;
 }
-.list-group-item + .list-group-item.active {
+
+.list-group-item+.list-group-item.active {
   margin-top: calc(-1 * var(--bs-list-group-border-width));
   border-top-width: var(--bs-list-group-border-width);
 }
 
 .list-group-horizontal {
   flex-direction: row;
 }
-.list-group-horizontal > .list-group-item:first-child:not(:last-child) {
+
+.list-group-horizontal>.list-group-item:first-child:not(:last-child) {
   border-bottom-left-radius: var(--bs-list-group-border-radius);
   border-top-right-radius: 0;
 }
-.list-group-horizontal > .list-group-item:last-child:not(:first-child) {
+
+.list-group-horizontal>.list-group-item:last-child:not(:first-child) {
   border-top-right-radius: var(--bs-list-group-border-radius);
   border-bottom-left-radius: 0;
 }
-.list-group-horizontal > .list-group-item.active {
+
+.list-group-horizontal>.list-group-item.active {
   margin-top: 0;
 }
-.list-group-horizontal > .list-group-item + .list-group-item {
+
+.list-group-horizontal>.list-group-item+.list-group-item {
   border-top-width: var(--bs-list-group-border-width);
   border-left-width: 0;
 }
-.list-group-horizontal > .list-group-item + .list-group-item.active {
+
+.list-group-horizontal>.list-group-item+.list-group-item.active {
   margin-left: calc(-1 * var(--bs-list-group-border-width));
   border-left-width: var(--bs-list-group-border-width);
 }
 
 @media (min-width: 576px) {
   .list-group-horizontal-sm {
     flex-direction: row;
   }
-  .list-group-horizontal-sm > .list-group-item:first-child:not(:last-child) {
+
+  .list-group-horizontal-sm>.list-group-item:first-child:not(:last-child) {
     border-bottom-left-radius: var(--bs-list-group-border-radius);
     border-top-right-radius: 0;
   }
-  .list-group-horizontal-sm > .list-group-item:last-child:not(:first-child) {
+
+  .list-group-horizontal-sm>.list-group-item:last-child:not(:first-child) {
     border-top-right-radius: var(--bs-list-group-border-radius);
     border-bottom-left-radius: 0;
   }
-  .list-group-horizontal-sm > .list-group-item.active {
+
+  .list-group-horizontal-sm>.list-group-item.active {
     margin-top: 0;
   }
-  .list-group-horizontal-sm > .list-group-item + .list-group-item {
+
+  .list-group-horizontal-sm>.list-group-item+.list-group-item {
     border-top-width: var(--bs-list-group-border-width);
     border-left-width: 0;
   }
-  .list-group-horizontal-sm > .list-group-item + .list-group-item.active {
+
+  .list-group-horizontal-sm>.list-group-item+.list-group-item.active {
     margin-left: calc(-1 * var(--bs-list-group-border-width));
     border-left-width: var(--bs-list-group-border-width);
   }
 }
+
 @media (min-width: 768px) {
   .list-group-horizontal-md {
     flex-direction: row;
   }
-  .list-group-horizontal-md > .list-group-item:first-child:not(:last-child) {
+
+  .list-group-horizontal-md>.list-group-item:first-child:not(:last-child) {
     border-bottom-left-radius: var(--bs-list-group-border-radius);
     border-top-right-radius: 0;
   }
-  .list-group-horizontal-md > .list-group-item:last-child:not(:first-child) {
+
+  .list-group-horizontal-md>.list-group-item:last-child:not(:first-child) {
     border-top-right-radius: var(--bs-list-group-border-radius);
     border-bottom-left-radius: 0;
   }
-  .list-group-horizontal-md > .list-group-item.active {
+
+  .list-group-horizontal-md>.list-group-item.active {
     margin-top: 0;
   }
-  .list-group-horizontal-md > .list-group-item + .list-group-item {
+
+  .list-group-horizontal-md>.list-group-item+.list-group-item {
     border-top-width: var(--bs-list-group-border-width);
     border-left-width: 0;
   }
-  .list-group-horizontal-md > .list-group-item + .list-group-item.active {
+
+  .list-group-horizontal-md>.list-group-item+.list-group-item.active {
     margin-left: calc(-1 * var(--bs-list-group-border-width));
     border-left-width: var(--bs-list-group-border-width);
   }
 }
+
 @media (min-width: 992px) {
   .list-group-horizontal-lg {
     flex-direction: row;
   }
-  .list-group-horizontal-lg > .list-group-item:first-child:not(:last-child) {
+
+  .list-group-horizontal-lg>.list-group-item:first-child:not(:last-child) {
     border-bottom-left-radius: var(--bs-list-group-border-radius);
     border-top-right-radius: 0;
   }
-  .list-group-horizontal-lg > .list-group-item:last-child:not(:first-child) {
+
+  .list-group-horizontal-lg>.list-group-item:last-child:not(:first-child) {
     border-top-right-radius: var(--bs-list-group-border-radius);
     border-bottom-left-radius: 0;
   }
-  .list-group-horizontal-lg > .list-group-item.active {
+
+  .list-group-horizontal-lg>.list-group-item.active {
     margin-top: 0;
   }
-  .list-group-horizontal-lg > .list-group-item + .list-group-item {
+
+  .list-group-horizontal-lg>.list-group-item+.list-group-item {
     border-top-width: var(--bs-list-group-border-width);
     border-left-width: 0;
   }
-  .list-group-horizontal-lg > .list-group-item + .list-group-item.active {
+
+  .list-group-horizontal-lg>.list-group-item+.list-group-item.active {
     margin-left: calc(-1 * var(--bs-list-group-border-width));
     border-left-width: var(--bs-list-group-border-width);
   }
 }
+
 @media (min-width: 1200px) {
   .list-group-horizontal-xl {
     flex-direction: row;
   }
-  .list-group-horizontal-xl > .list-group-item:first-child:not(:last-child) {
+
+  .list-group-horizontal-xl>.list-group-item:first-child:not(:last-child) {
     border-bottom-left-radius: var(--bs-list-group-border-radius);
     border-top-right-radius: 0;
   }
-  .list-group-horizontal-xl > .list-group-item:last-child:not(:first-child) {
+
+  .list-group-horizontal-xl>.list-group-item:last-child:not(:first-child) {
     border-top-right-radius: var(--bs-list-group-border-radius);
     border-bottom-left-radius: 0;
   }
-  .list-group-horizontal-xl > .list-group-item.active {
+
+  .list-group-horizontal-xl>.list-group-item.active {
     margin-top: 0;
   }
-  .list-group-horizontal-xl > .list-group-item + .list-group-item {
+
+  .list-group-horizontal-xl>.list-group-item+.list-group-item {
     border-top-width: var(--bs-list-group-border-width);
     border-left-width: 0;
   }
-  .list-group-horizontal-xl > .list-group-item + .list-group-item.active {
+
+  .list-group-horizontal-xl>.list-group-item+.list-group-item.active {
     margin-left: calc(-1 * var(--bs-list-group-border-width));
     border-left-width: var(--bs-list-group-border-width);
   }
 }
+
 @media (min-width: 1400px) {
   .list-group-horizontal-xxl {
     flex-direction: row;
   }
-  .list-group-horizontal-xxl > .list-group-item:first-child:not(:last-child) {
+
+  .list-group-horizontal-xxl>.list-group-item:first-child:not(:last-child) {
     border-bottom-left-radius: var(--bs-list-group-border-radius);
     border-top-right-radius: 0;
   }
-  .list-group-horizontal-xxl > .list-group-item:last-child:not(:first-child) {
+
+  .list-group-horizontal-xxl>.list-group-item:last-child:not(:first-child) {
     border-top-right-radius: var(--bs-list-group-border-radius);
     border-bottom-left-radius: 0;
   }
-  .list-group-horizontal-xxl > .list-group-item.active {
+
+  .list-group-horizontal-xxl>.list-group-item.active {
     margin-top: 0;
   }
-  .list-group-horizontal-xxl > .list-group-item + .list-group-item {
+
+  .list-group-horizontal-xxl>.list-group-item+.list-group-item {
     border-top-width: var(--bs-list-group-border-width);
     border-left-width: 0;
   }
-  .list-group-horizontal-xxl > .list-group-item + .list-group-item.active {
+
+  .list-group-horizontal-xxl>.list-group-item+.list-group-item.active {
     margin-left: calc(-1 * var(--bs-list-group-border-width));
     border-left-width: var(--bs-list-group-border-width);
   }
 }
+
 .list-group-flush {
   border-radius: 0;
 }
-.list-group-flush > .list-group-item {
+
+.list-group-flush>.list-group-item {
   border-width: 0 0 var(--bs-list-group-border-width);
 }
-.list-group-flush > .list-group-item:last-child {
+
+.list-group-flush>.list-group-item:last-child {
   border-bottom-width: 0;
 }
 
 .list-group-item-primary {
   color: #084298;
   background-color: #cfe2ff;
 }
-.list-group-item-primary.list-group-item-action:hover, .list-group-item-primary.list-group-item-action:focus {
+
+.list-group-item-primary.list-group-item-action:hover,
+.list-group-item-primary.list-group-item-action:focus {
   color: #084298;
   background-color: #bacbe6;
 }
+
 .list-group-item-primary.list-group-item-action.active {
   color: #fff;
   background-color: #084298;
   border-color: #084298;
 }
 
 .list-group-item-secondary {
   color: #41464b;
   background-color: #e2e3e5;
 }
-.list-group-item-secondary.list-group-item-action:hover, .list-group-item-secondary.list-group-item-action:focus {
+
+.list-group-item-secondary.list-group-item-action:hover,
+.list-group-item-secondary.list-group-item-action:focus {
   color: #41464b;
   background-color: #cbccce;
 }
+
 .list-group-item-secondary.list-group-item-action.active {
   color: #fff;
   background-color: #41464b;
   border-color: #41464b;
 }
 
 .list-group-item-success {
   color: #0f5132;
   background-color: #d1e7dd;
 }
-.list-group-item-success.list-group-item-action:hover, .list-group-item-success.list-group-item-action:focus {
+
+.list-group-item-success.list-group-item-action:hover,
+.list-group-item-success.list-group-item-action:focus {
   color: #0f5132;
   background-color: #bcd0c7;
 }
+
 .list-group-item-success.list-group-item-action.active {
   color: #fff;
   background-color: #0f5132;
   border-color: #0f5132;
 }
 
 .list-group-item-info {
   color: #055160;
   background-color: #cff4fc;
 }
-.list-group-item-info.list-group-item-action:hover, .list-group-item-info.list-group-item-action:focus {
+
+.list-group-item-info.list-group-item-action:hover,
+.list-group-item-info.list-group-item-action:focus {
   color: #055160;
   background-color: #badce3;
 }
+
 .list-group-item-info.list-group-item-action.active {
   color: #fff;
   background-color: #055160;
   border-color: #055160;
 }
 
 .list-group-item-warning {
   color: #664d03;
   background-color: #fff3cd;
 }
-.list-group-item-warning.list-group-item-action:hover, .list-group-item-warning.list-group-item-action:focus {
+
+.list-group-item-warning.list-group-item-action:hover,
+.list-group-item-warning.list-group-item-action:focus {
   color: #664d03;
   background-color: #e6dbb9;
 }
+
 .list-group-item-warning.list-group-item-action.active {
   color: #fff;
   background-color: #664d03;
   border-color: #664d03;
 }
 
 .list-group-item-danger {
   color: #842029;
   background-color: #f8d7da;
 }
-.list-group-item-danger.list-group-item-action:hover, .list-group-item-danger.list-group-item-action:focus {
+
+.list-group-item-danger.list-group-item-action:hover,
+.list-group-item-danger.list-group-item-action:focus {
   color: #842029;
   background-color: #dfc2c4;
 }
+
 .list-group-item-danger.list-group-item-action.active {
   color: #fff;
   background-color: #842029;
   border-color: #842029;
 }
 
 .list-group-item-light {
   color: #636464;
   background-color: #fefefe;
 }
-.list-group-item-light.list-group-item-action:hover, .list-group-item-light.list-group-item-action:focus {
+
+.list-group-item-light.list-group-item-action:hover,
+.list-group-item-light.list-group-item-action:focus {
   color: #636464;
   background-color: #e5e5e5;
 }
+
 .list-group-item-light.list-group-item-action.active {
   color: #fff;
   background-color: #636464;
   border-color: #636464;
 }
 
 .list-group-item-dark {
   color: #141619;
   background-color: #d3d3d4;
 }
-.list-group-item-dark.list-group-item-action:hover, .list-group-item-dark.list-group-item-action:focus {
+
+.list-group-item-dark.list-group-item-action:hover,
+.list-group-item-dark.list-group-item-action:focus {
   color: #141619;
   background-color: #bebebf;
 }
+
 .list-group-item-dark.list-group-item-action.active {
   color: #fff;
   background-color: #141619;
   border-color: #141619;
 }
 
 .btn-close {
@@ -5138,29 +5879,33 @@
   padding: 0.25em 0.25em;
   color: #000;
   background: transparent url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='%23000'%3e%3cpath d='M.293.293a1 1 0 0 1 1.414 0L8 6.586 14.293.293a1 1 0 1 1 1.414 1.414L9.414 8l6.293 6.293a1 1 0 0 1-1.414 1.414L8 9.414l-6.293 6.293a1 1 0 0 1-1.414-1.414L6.586 8 .293 1.707a1 1 0 0 1 0-1.414z'/%3e%3c/svg%3e") center/1em auto no-repeat;
   border: 0;
   border-radius: 0.375rem;
   opacity: 0.5;
 }
+
 .btn-close:hover {
   color: #000;
   text-decoration: none;
   opacity: 0.75;
 }
+
 .btn-close:focus {
   outline: 0;
   box-shadow: 0 0 0 0.25rem rgba(13, 110, 253, 0.25);
   opacity: 1;
 }
-.btn-close:disabled, .btn-close.disabled {
+
+.btn-close:disabled,
+.btn-close.disabled {
   pointer-events: none;
   -webkit-user-select: none;
-     -moz-user-select: none;
-          user-select: none;
+  -moz-user-select: none;
+  user-select: none;
   opacity: 0.25;
 }
 
 .btn-close-white {
   filter: invert(1) grayscale(100%) brightness(200%);
 }
 
@@ -5187,45 +5932,49 @@
   pointer-events: auto;
   background-color: var(--bs-toast-bg);
   background-clip: padding-box;
   border: var(--bs-toast-border-width) solid var(--bs-toast-border-color);
   box-shadow: var(--bs-toast-box-shadow);
   border-radius: var(--bs-toast-border-radius);
 }
+
 .toast.showing {
   opacity: 0;
 }
+
 .toast:not(.show) {
   display: none;
 }
 
 .toast-container {
   --bs-toast-zindex: 1090;
   position: absolute;
   z-index: var(--bs-toast-zindex);
   width: -moz-max-content;
   width: max-content;
   max-width: 100%;
   pointer-events: none;
 }
-.toast-container > :not(:last-child) {
+
+.toast-container> :not(:last-child) {
   margin-bottom: var(--bs-toast-spacing);
 }
 
 .toast-header {
   display: flex;
   align-items: center;
   padding: var(--bs-toast-padding-y) var(--bs-toast-padding-x);
   color: var(--bs-toast-header-color);
   background-color: var(--bs-toast-header-bg);
   background-clip: padding-box;
   border-bottom: var(--bs-toast-border-width) solid var(--bs-toast-header-border-color);
   border-top-left-radius: calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width));
   border-top-right-radius: calc(var(--bs-toast-border-radius) - var(--bs-toast-border-width));
 }
+
 .toast-header .btn-close {
   margin-right: calc(-0.5 * var(--bs-toast-padding-x));
   margin-left: var(--bs-toast-padding-x);
 }
 
 .toast-body {
   padding: var(--bs-toast-padding-x);
@@ -5268,37 +6017,43 @@
 
 .modal-dialog {
   position: relative;
   width: auto;
   margin: var(--bs-modal-margin);
   pointer-events: none;
 }
+
 .modal.fade .modal-dialog {
   transition: transform 0.3s ease-out;
   transform: translate(0, -50px);
 }
+
 @media (prefers-reduced-motion: reduce) {
   .modal.fade .modal-dialog {
     transition: none;
   }
 }
+
 .modal.show .modal-dialog {
   transform: none;
 }
+
 .modal.modal-static .modal-dialog {
   transform: scale(1.02);
 }
 
 .modal-dialog-scrollable {
   height: calc(100% - var(--bs-modal-margin) * 2);
 }
+
 .modal-dialog-scrollable .modal-content {
   max-height: 100%;
   overflow: hidden;
 }
+
 .modal-dialog-scrollable .modal-body {
   overflow-y: auto;
 }
 
 .modal-dialog-centered {
   display: flex;
   align-items: center;
@@ -5327,31 +6082,34 @@
   top: 0;
   left: 0;
   z-index: var(--bs-backdrop-zindex);
   width: 100vw;
   height: 100vh;
   background-color: var(--bs-backdrop-bg);
 }
+
 .modal-backdrop.fade {
   opacity: 0;
 }
+
 .modal-backdrop.show {
   opacity: var(--bs-backdrop-opacity);
 }
 
 .modal-header {
   display: flex;
   flex-shrink: 0;
   align-items: center;
   justify-content: space-between;
   padding: var(--bs-modal-header-padding);
   border-bottom: var(--bs-modal-header-border-width) solid var(--bs-modal-header-border-color);
   border-top-left-radius: var(--bs-modal-inner-border-radius);
   border-top-right-radius: var(--bs-modal-inner-border-radius);
 }
+
 .modal-header .btn-close {
   padding: calc(var(--bs-modal-header-padding-y) * 0.5) calc(var(--bs-modal-header-padding-x) * 0.5);
   margin: calc(-0.5 * var(--bs-modal-header-padding-y)) calc(-0.5 * var(--bs-modal-header-padding-x)) calc(-0.5 * var(--bs-modal-header-padding-y)) auto;
 }
 
 .modal-title {
   margin-bottom: 0;
@@ -5372,162 +6130,192 @@
   justify-content: flex-end;
   padding: calc(var(--bs-modal-padding) - var(--bs-modal-footer-gap) * 0.5);
   background-color: var(--bs-modal-footer-bg);
   border-top: var(--bs-modal-footer-border-width) solid var(--bs-modal-footer-border-color);
   border-bottom-right-radius: var(--bs-modal-inner-border-radius);
   border-bottom-left-radius: var(--bs-modal-inner-border-radius);
 }
-.modal-footer > * {
+
+.modal-footer>* {
   margin: calc(var(--bs-modal-footer-gap) * 0.5);
 }
 
 @media (min-width: 576px) {
   .modal {
     --bs-modal-margin: 1.75rem;
     --bs-modal-box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);
   }
+
   .modal-dialog {
     max-width: var(--bs-modal-width);
     margin-right: auto;
     margin-left: auto;
   }
+
   .modal-sm {
     --bs-modal-width: 300px;
   }
 }
+
 @media (min-width: 992px) {
+
   .modal-lg,
   .modal-xl {
     --bs-modal-width: 800px;
   }
 }
+
 @media (min-width: 1200px) {
   .modal-xl {
     --bs-modal-width: 1140px;
   }
 }
+
 .modal-fullscreen {
   width: 100vw;
   max-width: none;
   height: 100%;
   margin: 0;
 }
+
 .modal-fullscreen .modal-content {
   height: 100%;
   border: 0;
   border-radius: 0;
 }
+
 .modal-fullscreen .modal-header,
 .modal-fullscreen .modal-footer {
   border-radius: 0;
 }
+
 .modal-fullscreen .modal-body {
   overflow-y: auto;
 }
 
 @media (max-width: 575.98px) {
   .modal-fullscreen-sm-down {
     width: 100vw;
     max-width: none;
     height: 100%;
     margin: 0;
   }
+
   .modal-fullscreen-sm-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
+
   .modal-fullscreen-sm-down .modal-header,
   .modal-fullscreen-sm-down .modal-footer {
     border-radius: 0;
   }
+
   .modal-fullscreen-sm-down .modal-body {
     overflow-y: auto;
   }
 }
+
 @media (max-width: 767.98px) {
   .modal-fullscreen-md-down {
     width: 100vw;
     max-width: none;
     height: 100%;
     margin: 0;
   }
+
   .modal-fullscreen-md-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
+
   .modal-fullscreen-md-down .modal-header,
   .modal-fullscreen-md-down .modal-footer {
     border-radius: 0;
   }
+
   .modal-fullscreen-md-down .modal-body {
     overflow-y: auto;
   }
 }
+
 @media (max-width: 991.98px) {
   .modal-fullscreen-lg-down {
     width: 100vw;
     max-width: none;
     height: 100%;
     margin: 0;
   }
+
   .modal-fullscreen-lg-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
+
   .modal-fullscreen-lg-down .modal-header,
   .modal-fullscreen-lg-down .modal-footer {
     border-radius: 0;
   }
+
   .modal-fullscreen-lg-down .modal-body {
     overflow-y: auto;
   }
 }
+
 @media (max-width: 1199.98px) {
   .modal-fullscreen-xl-down {
     width: 100vw;
     max-width: none;
     height: 100%;
     margin: 0;
   }
+
   .modal-fullscreen-xl-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
+
   .modal-fullscreen-xl-down .modal-header,
   .modal-fullscreen-xl-down .modal-footer {
     border-radius: 0;
   }
+
   .modal-fullscreen-xl-down .modal-body {
     overflow-y: auto;
   }
 }
+
 @media (max-width: 1399.98px) {
   .modal-fullscreen-xxl-down {
     width: 100vw;
     max-width: none;
     height: 100%;
     margin: 0;
   }
+
   .modal-fullscreen-xxl-down .modal-content {
     height: 100%;
     border: 0;
     border-radius: 0;
   }
+
   .modal-fullscreen-xxl-down .modal-header,
   .modal-fullscreen-xxl-down .modal-footer {
     border-radius: 0;
   }
+
   .modal-fullscreen-xxl-down .modal-body {
     overflow-y: auto;
   }
 }
+
 .tooltip {
   --bs-tooltip-zindex: 1080;
   --bs-tooltip-max-width: 200px;
   --bs-tooltip-padding-x: 0.5rem;
   --bs-tooltip-padding-y: 0.25rem;
   --bs-tooltip-margin: ;
   --bs-tooltip-font-size: 0.875rem;
@@ -5555,67 +6343,82 @@
   white-space: normal;
   word-spacing: normal;
   line-break: auto;
   font-size: var(--bs-tooltip-font-size);
   word-wrap: break-word;
   opacity: 0;
 }
+
 .tooltip.show {
   opacity: var(--bs-tooltip-opacity);
 }
+
 .tooltip .tooltip-arrow {
   display: block;
   width: var(--bs-tooltip-arrow-width);
   height: var(--bs-tooltip-arrow-height);
 }
+
 .tooltip .tooltip-arrow::before {
   position: absolute;
   content: "";
   border-color: transparent;
   border-style: solid;
 }
 
-.bs-tooltip-top .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow {
+.bs-tooltip-top .tooltip-arrow,
+.bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow {
   bottom: 0;
 }
-.bs-tooltip-top .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow::before {
+
+.bs-tooltip-top .tooltip-arrow::before,
+.bs-tooltip-auto[data-popper-placement^=top] .tooltip-arrow::before {
   top: -1px;
   border-width: var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * 0.5) 0;
   border-top-color: var(--bs-tooltip-bg);
 }
 
 /* rtl:begin:ignore */
-.bs-tooltip-end .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow {
+.bs-tooltip-end .tooltip-arrow,
+.bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow {
   left: 0;
   width: var(--bs-tooltip-arrow-height);
   height: var(--bs-tooltip-arrow-width);
 }
-.bs-tooltip-end .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow::before {
+
+.bs-tooltip-end .tooltip-arrow::before,
+.bs-tooltip-auto[data-popper-placement^=right] .tooltip-arrow::before {
   right: -1px;
   border-width: calc(var(--bs-tooltip-arrow-width) * 0.5) var(--bs-tooltip-arrow-height) calc(var(--bs-tooltip-arrow-width) * 0.5) 0;
   border-right-color: var(--bs-tooltip-bg);
 }
 
 /* rtl:end:ignore */
-.bs-tooltip-bottom .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow {
+.bs-tooltip-bottom .tooltip-arrow,
+.bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow {
   top: 0;
 }
-.bs-tooltip-bottom .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow::before {
+
+.bs-tooltip-bottom .tooltip-arrow::before,
+.bs-tooltip-auto[data-popper-placement^=bottom] .tooltip-arrow::before {
   bottom: -1px;
   border-width: 0 calc(var(--bs-tooltip-arrow-width) * 0.5) var(--bs-tooltip-arrow-height);
   border-bottom-color: var(--bs-tooltip-bg);
 }
 
 /* rtl:begin:ignore */
-.bs-tooltip-start .tooltip-arrow, .bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow {
+.bs-tooltip-start .tooltip-arrow,
+.bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow {
   right: 0;
   width: var(--bs-tooltip-arrow-height);
   height: var(--bs-tooltip-arrow-width);
 }
-.bs-tooltip-start .tooltip-arrow::before, .bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow::before {
+
+.bs-tooltip-start .tooltip-arrow::before,
+.bs-tooltip-auto[data-popper-placement^=left] .tooltip-arrow::before {
   left: -1px;
   border-width: calc(var(--bs-tooltip-arrow-width) * 0.5) 0 calc(var(--bs-tooltip-arrow-width) * 0.5) var(--bs-tooltip-arrow-height);
   border-left-color: var(--bs-tooltip-bg);
 }
 
 /* rtl:end:ignore */
 .tooltip-inner {
@@ -5668,101 +6471,142 @@
   font-size: var(--bs-popover-font-size);
   word-wrap: break-word;
   background-color: var(--bs-popover-bg);
   background-clip: padding-box;
   border: var(--bs-popover-border-width) solid var(--bs-popover-border-color);
   border-radius: var(--bs-popover-border-radius);
 }
+
 .popover .popover-arrow {
   display: block;
   width: var(--bs-popover-arrow-width);
   height: var(--bs-popover-arrow-height);
 }
-.popover .popover-arrow::before, .popover .popover-arrow::after {
+
+.popover .popover-arrow::before,
+.popover .popover-arrow::after {
   position: absolute;
   display: block;
   content: "";
   border-color: transparent;
   border-style: solid;
   border-width: 0;
 }
 
-.bs-popover-top > .popover-arrow, .bs-popover-auto[data-popper-placement^=top] > .popover-arrow {
+.bs-popover-top>.popover-arrow,
+.bs-popover-auto[data-popper-placement^=top]>.popover-arrow {
   bottom: calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));
 }
-.bs-popover-top > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=top] > .popover-arrow::before, .bs-popover-top > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=top] > .popover-arrow::after {
+
+.bs-popover-top>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=top]>.popover-arrow::before,
+.bs-popover-top>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=top]>.popover-arrow::after {
   border-width: var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * 0.5) 0;
 }
-.bs-popover-top > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=top] > .popover-arrow::before {
+
+.bs-popover-top>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=top]>.popover-arrow::before {
   bottom: 0;
   border-top-color: var(--bs-popover-arrow-border);
 }
-.bs-popover-top > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=top] > .popover-arrow::after {
+
+.bs-popover-top>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=top]>.popover-arrow::after {
   bottom: var(--bs-popover-border-width);
   border-top-color: var(--bs-popover-bg);
 }
 
 /* rtl:begin:ignore */
-.bs-popover-end > .popover-arrow, .bs-popover-auto[data-popper-placement^=right] > .popover-arrow {
+.bs-popover-end>.popover-arrow,
+.bs-popover-auto[data-popper-placement^=right]>.popover-arrow {
   left: calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));
   width: var(--bs-popover-arrow-height);
   height: var(--bs-popover-arrow-width);
 }
-.bs-popover-end > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=right] > .popover-arrow::before, .bs-popover-end > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=right] > .popover-arrow::after {
+
+.bs-popover-end>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=right]>.popover-arrow::before,
+.bs-popover-end>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=right]>.popover-arrow::after {
   border-width: calc(var(--bs-popover-arrow-width) * 0.5) var(--bs-popover-arrow-height) calc(var(--bs-popover-arrow-width) * 0.5) 0;
 }
-.bs-popover-end > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=right] > .popover-arrow::before {
+
+.bs-popover-end>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=right]>.popover-arrow::before {
   left: 0;
   border-right-color: var(--bs-popover-arrow-border);
 }
-.bs-popover-end > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=right] > .popover-arrow::after {
+
+.bs-popover-end>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=right]>.popover-arrow::after {
   left: var(--bs-popover-border-width);
   border-right-color: var(--bs-popover-bg);
 }
 
 /* rtl:end:ignore */
-.bs-popover-bottom > .popover-arrow, .bs-popover-auto[data-popper-placement^=bottom] > .popover-arrow {
+.bs-popover-bottom>.popover-arrow,
+.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow {
   top: calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));
 }
-.bs-popover-bottom > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=bottom] > .popover-arrow::before, .bs-popover-bottom > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=bottom] > .popover-arrow::after {
+
+.bs-popover-bottom>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow::before,
+.bs-popover-bottom>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow::after {
   border-width: 0 calc(var(--bs-popover-arrow-width) * 0.5) var(--bs-popover-arrow-height);
 }
-.bs-popover-bottom > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=bottom] > .popover-arrow::before {
+
+.bs-popover-bottom>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow::before {
   top: 0;
   border-bottom-color: var(--bs-popover-arrow-border);
 }
-.bs-popover-bottom > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=bottom] > .popover-arrow::after {
+
+.bs-popover-bottom>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=bottom]>.popover-arrow::after {
   top: var(--bs-popover-border-width);
   border-bottom-color: var(--bs-popover-bg);
 }
-.bs-popover-bottom .popover-header::before, .bs-popover-auto[data-popper-placement^=bottom] .popover-header::before {
+
+.bs-popover-bottom .popover-header::before,
+.bs-popover-auto[data-popper-placement^=bottom] .popover-header::before {
   position: absolute;
   top: 0;
   left: 50%;
   display: block;
   width: var(--bs-popover-arrow-width);
   margin-left: calc(-0.5 * var(--bs-popover-arrow-width));
   content: "";
   border-bottom: var(--bs-popover-border-width) solid var(--bs-popover-header-bg);
 }
 
 /* rtl:begin:ignore */
-.bs-popover-start > .popover-arrow, .bs-popover-auto[data-popper-placement^=left] > .popover-arrow {
+.bs-popover-start>.popover-arrow,
+.bs-popover-auto[data-popper-placement^=left]>.popover-arrow {
   right: calc(-1 * (var(--bs-popover-arrow-height)) - var(--bs-popover-border-width));
   width: var(--bs-popover-arrow-height);
   height: var(--bs-popover-arrow-width);
 }
-.bs-popover-start > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=left] > .popover-arrow::before, .bs-popover-start > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=left] > .popover-arrow::after {
+
+.bs-popover-start>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=left]>.popover-arrow::before,
+.bs-popover-start>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=left]>.popover-arrow::after {
   border-width: calc(var(--bs-popover-arrow-width) * 0.5) 0 calc(var(--bs-popover-arrow-width) * 0.5) var(--bs-popover-arrow-height);
 }
-.bs-popover-start > .popover-arrow::before, .bs-popover-auto[data-popper-placement^=left] > .popover-arrow::before {
+
+.bs-popover-start>.popover-arrow::before,
+.bs-popover-auto[data-popper-placement^=left]>.popover-arrow::before {
   right: 0;
   border-left-color: var(--bs-popover-arrow-border);
 }
-.bs-popover-start > .popover-arrow::after, .bs-popover-auto[data-popper-placement^=left] > .popover-arrow::after {
+
+.bs-popover-start>.popover-arrow::after,
+.bs-popover-auto[data-popper-placement^=left]>.popover-arrow::after {
   right: var(--bs-popover-border-width);
   border-left-color: var(--bs-popover-bg);
 }
 
 /* rtl:end:ignore */
 .popover-header {
   padding: var(--bs-popover-header-padding-y) var(--bs-popover-header-padding-x);
@@ -5770,14 +6614,15 @@
   font-size: var(--bs-popover-header-font-size);
   color: var(--bs-popover-header-color);
   background-color: var(--bs-popover-header-bg);
   border-bottom: var(--bs-popover-border-width) solid var(--bs-popover-border-color);
   border-top-left-radius: var(--bs-popover-inner-border-radius);
   border-top-right-radius: var(--bs-popover-inner-border-radius);
 }
+
 .popover-header:empty {
   display: none;
 }
 
 .popover-body {
   padding: var(--bs-popover-body-padding-y) var(--bs-popover-body-padding-x);
   color: var(--bs-popover-body-color);
@@ -5792,30 +6637,32 @@
 }
 
 .carousel-inner {
   position: relative;
   width: 100%;
   overflow: hidden;
 }
+
 .carousel-inner::after {
   display: block;
   clear: both;
   content: "";
 }
 
 .carousel-item {
   position: relative;
   display: none;
   float: left;
   width: 100%;
   margin-right: -100%;
   -webkit-backface-visibility: hidden;
-          backface-visibility: hidden;
+  backface-visibility: hidden;
   transition: transform 0.6s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .carousel-item {
     transition: none;
   }
 }
 
 .carousel-item.active,
@@ -5835,27 +6682,31 @@
 }
 
 .carousel-fade .carousel-item {
   opacity: 0;
   transition-property: opacity;
   transform: none;
 }
+
 .carousel-fade .carousel-item.active,
 .carousel-fade .carousel-item-next.carousel-item-start,
 .carousel-fade .carousel-item-prev.carousel-item-end {
   z-index: 1;
   opacity: 1;
 }
+
 .carousel-fade .active.carousel-item-start,
 .carousel-fade .active.carousel-item-end {
   z-index: 0;
   opacity: 0;
   transition: opacity 0s 0.6s;
 }
+
 @media (prefers-reduced-motion: reduce) {
+
   .carousel-fade .active.carousel-item-start,
   .carousel-fade .active.carousel-item-end {
     transition: none;
   }
 }
 
 .carousel-control-prev,
@@ -5872,21 +6723,25 @@
   color: #fff;
   text-align: center;
   background: none;
   border: 0;
   opacity: 0.5;
   transition: opacity 0.15s ease;
 }
+
 @media (prefers-reduced-motion: reduce) {
+
   .carousel-control-prev,
   .carousel-control-next {
     transition: none;
   }
 }
-.carousel-control-prev:hover, .carousel-control-prev:focus,
+
+.carousel-control-prev:hover,
+.carousel-control-prev:focus,
 .carousel-control-next:hover,
 .carousel-control-next:focus {
   color: #fff;
   text-decoration: none;
   outline: 0;
   opacity: 0.9;
 }
@@ -5935,14 +6790,15 @@
   justify-content: center;
   padding: 0;
   margin-right: 15%;
   margin-bottom: 1rem;
   margin-left: 15%;
   list-style: none;
 }
+
 .carousel-indicators [data-bs-target] {
   box-sizing: content-box;
   flex: 0 1 auto;
   width: 30px;
   height: 3px;
   padding: 0;
   margin-right: 3px;
@@ -5953,19 +6809,21 @@
   background-clip: padding-box;
   border: 0;
   border-top: 10px solid transparent;
   border-bottom: 10px solid transparent;
   opacity: 0.5;
   transition: opacity 0.6s ease;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .carousel-indicators [data-bs-target] {
     transition: none;
   }
 }
+
 .carousel-indicators .active {
   opacity: 1;
 }
 
 .carousel-caption {
   position: absolute;
   right: 15%;
@@ -5977,17 +6835,19 @@
   text-align: center;
 }
 
 .carousel-dark .carousel-control-prev-icon,
 .carousel-dark .carousel-control-next-icon {
   filter: invert(1) grayscale(100);
 }
+
 .carousel-dark .carousel-indicators [data-bs-target] {
   background-color: #000;
 }
+
 .carousel-dark .carousel-caption {
   color: #000;
 }
 
 .spinner-grow,
 .spinner-border {
   display: inline-block;
@@ -5996,17 +6856,20 @@
   vertical-align: var(--bs-spinner-vertical-align);
   border-radius: 50%;
   animation: var(--bs-spinner-animation-speed) linear infinite var(--bs-spinner-animation-name);
 }
 
 @keyframes spinner-border {
   to {
-    transform: rotate(360deg) /* rtl:ignore */;
+    transform: rotate(360deg)
+      /* rtl:ignore */
+    ;
   }
 }
+
 .spinner-border {
   --bs-spinner-width: 2rem;
   --bs-spinner-height: 2rem;
   --bs-spinner-vertical-align: -0.125em;
   --bs-spinner-border-width: 0.25em;
   --bs-spinner-animation-speed: 0.75s;
   --bs-spinner-animation-name: spinner-border;
@@ -6020,19 +6883,21 @@
   --bs-spinner-border-width: 0.2em;
 }
 
 @keyframes spinner-grow {
   0% {
     transform: scale(0);
   }
+
   50% {
     opacity: 1;
     transform: none;
   }
 }
+
 .spinner-grow {
   --bs-spinner-width: 2rem;
   --bs-spinner-height: 2rem;
   --bs-spinner-vertical-align: -0.125em;
   --bs-spinner-animation-speed: 0.75s;
   --bs-spinner-animation-name: spinner-grow;
   background-color: currentcolor;
@@ -6041,20 +6906,27 @@
 
 .spinner-grow-sm {
   --bs-spinner-width: 1rem;
   --bs-spinner-height: 1rem;
 }
 
 @media (prefers-reduced-motion: reduce) {
+
   .spinner-border,
   .spinner-grow {
     --bs-spinner-animation-speed: 1.5s;
   }
 }
-.offcanvas, .offcanvas-xxl, .offcanvas-xl, .offcanvas-lg, .offcanvas-md, .offcanvas-sm {
+
+.offcanvas,
+.offcanvas-xxl,
+.offcanvas-xl,
+.offcanvas-lg,
+.offcanvas-md,
+.offcanvas-sm {
   --bs-offcanvas-zindex: 1045;
   --bs-offcanvas-width: 400px;
   --bs-offcanvas-height: 30vh;
   --bs-offcanvas-padding-x: 1rem;
   --bs-offcanvas-padding-y: 1rem;
   --bs-offcanvas-color: ;
   --bs-offcanvas-bg: #fff;
@@ -6075,77 +6947,92 @@
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
     transition: transform 0.3s ease-in-out;
   }
 }
+
 @media (max-width: 575.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-sm {
     transition: none;
   }
 }
+
 @media (max-width: 575.98px) {
   .offcanvas-sm.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
 }
+
 @media (max-width: 575.98px) {
   .offcanvas-sm.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
 }
+
 @media (max-width: 575.98px) {
   .offcanvas-sm.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
 }
+
 @media (max-width: 575.98px) {
   .offcanvas-sm.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
 }
+
 @media (max-width: 575.98px) {
-  .offcanvas-sm.showing, .offcanvas-sm.show:not(.hiding) {
+
+  .offcanvas-sm.showing,
+  .offcanvas-sm.show:not(.hiding) {
     transform: none;
   }
 }
+
 @media (max-width: 575.98px) {
-  .offcanvas-sm.showing, .offcanvas-sm.hiding, .offcanvas-sm.show {
+
+  .offcanvas-sm.showing,
+  .offcanvas-sm.hiding,
+  .offcanvas-sm.show {
     visibility: visible;
   }
 }
+
 @media (min-width: 576px) {
   .offcanvas-sm {
     --bs-offcanvas-height: auto;
     --bs-offcanvas-border-width: 0;
     background-color: transparent !important;
   }
+
   .offcanvas-sm .offcanvas-header {
     display: none;
   }
+
   .offcanvas-sm .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
     background-color: transparent !important;
   }
@@ -6163,77 +7050,92 @@
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
     transition: transform 0.3s ease-in-out;
   }
 }
+
 @media (max-width: 767.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-md {
     transition: none;
   }
 }
+
 @media (max-width: 767.98px) {
   .offcanvas-md.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
 }
+
 @media (max-width: 767.98px) {
   .offcanvas-md.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
 }
+
 @media (max-width: 767.98px) {
   .offcanvas-md.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
 }
+
 @media (max-width: 767.98px) {
   .offcanvas-md.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
 }
+
 @media (max-width: 767.98px) {
-  .offcanvas-md.showing, .offcanvas-md.show:not(.hiding) {
+
+  .offcanvas-md.showing,
+  .offcanvas-md.show:not(.hiding) {
     transform: none;
   }
 }
+
 @media (max-width: 767.98px) {
-  .offcanvas-md.showing, .offcanvas-md.hiding, .offcanvas-md.show {
+
+  .offcanvas-md.showing,
+  .offcanvas-md.hiding,
+  .offcanvas-md.show {
     visibility: visible;
   }
 }
+
 @media (min-width: 768px) {
   .offcanvas-md {
     --bs-offcanvas-height: auto;
     --bs-offcanvas-border-width: 0;
     background-color: transparent !important;
   }
+
   .offcanvas-md .offcanvas-header {
     display: none;
   }
+
   .offcanvas-md .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
     background-color: transparent !important;
   }
@@ -6251,77 +7153,92 @@
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
     transition: transform 0.3s ease-in-out;
   }
 }
+
 @media (max-width: 991.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-lg {
     transition: none;
   }
 }
+
 @media (max-width: 991.98px) {
   .offcanvas-lg.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
 }
+
 @media (max-width: 991.98px) {
   .offcanvas-lg.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
 }
+
 @media (max-width: 991.98px) {
   .offcanvas-lg.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
 }
+
 @media (max-width: 991.98px) {
   .offcanvas-lg.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
 }
+
 @media (max-width: 991.98px) {
-  .offcanvas-lg.showing, .offcanvas-lg.show:not(.hiding) {
+
+  .offcanvas-lg.showing,
+  .offcanvas-lg.show:not(.hiding) {
     transform: none;
   }
 }
+
 @media (max-width: 991.98px) {
-  .offcanvas-lg.showing, .offcanvas-lg.hiding, .offcanvas-lg.show {
+
+  .offcanvas-lg.showing,
+  .offcanvas-lg.hiding,
+  .offcanvas-lg.show {
     visibility: visible;
   }
 }
+
 @media (min-width: 992px) {
   .offcanvas-lg {
     --bs-offcanvas-height: auto;
     --bs-offcanvas-border-width: 0;
     background-color: transparent !important;
   }
+
   .offcanvas-lg .offcanvas-header {
     display: none;
   }
+
   .offcanvas-lg .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
     background-color: transparent !important;
   }
@@ -6339,77 +7256,92 @@
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
     transition: transform 0.3s ease-in-out;
   }
 }
+
 @media (max-width: 1199.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-xl {
     transition: none;
   }
 }
+
 @media (max-width: 1199.98px) {
   .offcanvas-xl.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
 }
+
 @media (max-width: 1199.98px) {
   .offcanvas-xl.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
 }
+
 @media (max-width: 1199.98px) {
   .offcanvas-xl.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
 }
+
 @media (max-width: 1199.98px) {
   .offcanvas-xl.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
 }
+
 @media (max-width: 1199.98px) {
-  .offcanvas-xl.showing, .offcanvas-xl.show:not(.hiding) {
+
+  .offcanvas-xl.showing,
+  .offcanvas-xl.show:not(.hiding) {
     transform: none;
   }
 }
+
 @media (max-width: 1199.98px) {
-  .offcanvas-xl.showing, .offcanvas-xl.hiding, .offcanvas-xl.show {
+
+  .offcanvas-xl.showing,
+  .offcanvas-xl.hiding,
+  .offcanvas-xl.show {
     visibility: visible;
   }
 }
+
 @media (min-width: 1200px) {
   .offcanvas-xl {
     --bs-offcanvas-height: auto;
     --bs-offcanvas-border-width: 0;
     background-color: transparent !important;
   }
+
   .offcanvas-xl .offcanvas-header {
     display: none;
   }
+
   .offcanvas-xl .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
     background-color: transparent !important;
   }
@@ -6427,77 +7359,92 @@
     visibility: hidden;
     background-color: var(--bs-offcanvas-bg);
     background-clip: padding-box;
     outline: 0;
     transition: transform 0.3s ease-in-out;
   }
 }
+
 @media (max-width: 1399.98px) and (prefers-reduced-motion: reduce) {
   .offcanvas-xxl {
     transition: none;
   }
 }
+
 @media (max-width: 1399.98px) {
   .offcanvas-xxl.offcanvas-start {
     top: 0;
     left: 0;
     width: var(--bs-offcanvas-width);
     border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(-100%);
   }
 }
+
 @media (max-width: 1399.98px) {
   .offcanvas-xxl.offcanvas-end {
     top: 0;
     right: 0;
     width: var(--bs-offcanvas-width);
     border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateX(100%);
   }
 }
+
 @media (max-width: 1399.98px) {
   .offcanvas-xxl.offcanvas-top {
     top: 0;
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(-100%);
   }
 }
+
 @media (max-width: 1399.98px) {
   .offcanvas-xxl.offcanvas-bottom {
     right: 0;
     left: 0;
     height: var(--bs-offcanvas-height);
     max-height: 100%;
     border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
     transform: translateY(100%);
   }
 }
+
 @media (max-width: 1399.98px) {
-  .offcanvas-xxl.showing, .offcanvas-xxl.show:not(.hiding) {
+
+  .offcanvas-xxl.showing,
+  .offcanvas-xxl.show:not(.hiding) {
     transform: none;
   }
 }
+
 @media (max-width: 1399.98px) {
-  .offcanvas-xxl.showing, .offcanvas-xxl.hiding, .offcanvas-xxl.show {
+
+  .offcanvas-xxl.showing,
+  .offcanvas-xxl.hiding,
+  .offcanvas-xxl.show {
     visibility: visible;
   }
 }
+
 @media (min-width: 1400px) {
   .offcanvas-xxl {
     --bs-offcanvas-height: auto;
     --bs-offcanvas-border-width: 0;
     background-color: transparent !important;
   }
+
   .offcanvas-xxl .offcanvas-header {
     display: none;
   }
+
   .offcanvas-xxl .offcanvas-body {
     display: flex;
     flex-grow: 0;
     padding: 0;
     overflow-y: visible;
     background-color: transparent !important;
   }
@@ -6513,79 +7460,92 @@
   color: var(--bs-offcanvas-color);
   visibility: hidden;
   background-color: var(--bs-offcanvas-bg);
   background-clip: padding-box;
   outline: 0;
   transition: transform 0.3s ease-in-out;
 }
+
 @media (prefers-reduced-motion: reduce) {
   .offcanvas {
     transition: none;
   }
 }
+
 .offcanvas.offcanvas-start {
   top: 0;
   left: 0;
   width: var(--bs-offcanvas-width);
   border-right: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
   transform: translateX(-100%);
 }
+
 .offcanvas.offcanvas-end {
   top: 0;
   right: 0;
   width: var(--bs-offcanvas-width);
   border-left: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
   transform: translateX(100%);
 }
+
 .offcanvas.offcanvas-top {
   top: 0;
   right: 0;
   left: 0;
   height: var(--bs-offcanvas-height);
   max-height: 100%;
   border-bottom: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
   transform: translateY(-100%);
 }
+
 .offcanvas.offcanvas-bottom {
   right: 0;
   left: 0;
   height: var(--bs-offcanvas-height);
   max-height: 100%;
   border-top: var(--bs-offcanvas-border-width) solid var(--bs-offcanvas-border-color);
   transform: translateY(100%);
 }
-.offcanvas.showing, .offcanvas.show:not(.hiding) {
+
+.offcanvas.showing,
+.offcanvas.show:not(.hiding) {
   transform: none;
 }
-.offcanvas.showing, .offcanvas.hiding, .offcanvas.show {
+
+.offcanvas.showing,
+.offcanvas.hiding,
+.offcanvas.show {
   visibility: visible;
 }
 
 .offcanvas-backdrop {
   position: fixed;
   top: 0;
   left: 0;
   z-index: 1040;
   width: 100vw;
   height: 100vh;
   background-color: #000;
 }
+
 .offcanvas-backdrop.fade {
   opacity: 0;
 }
+
 .offcanvas-backdrop.show {
   opacity: 0.5;
 }
 
 .offcanvas-header {
   display: flex;
   align-items: center;
   justify-content: space-between;
   padding: var(--bs-offcanvas-padding-y) var(--bs-offcanvas-padding-x);
 }
+
 .offcanvas-header .btn-close {
   padding: calc(var(--bs-offcanvas-padding-y) * 0.5) calc(var(--bs-offcanvas-padding-x) * 0.5);
   margin-top: calc(-0.5 * var(--bs-offcanvas-padding-y));
   margin-right: calc(-0.5 * var(--bs-offcanvas-padding-x));
   margin-bottom: calc(-0.5 * var(--bs-offcanvas-padding-y));
 }
 
@@ -6604,14 +7564,15 @@
   display: inline-block;
   min-height: 1em;
   vertical-align: middle;
   cursor: wait;
   background-color: currentcolor;
   opacity: 0.5;
 }
+
 .placeholder.btn::before {
   display: inline-block;
   content: "";
 }
 
 .placeholder-xs {
   min-height: 0.6em;
@@ -6630,28 +7591,30 @@
 }
 
 @keyframes placeholder-glow {
   50% {
     opacity: 0.2;
   }
 }
+
 .placeholder-wave {
   -webkit-mask-image: linear-gradient(130deg, #000 55%, rgba(0, 0, 0, 0.8) 75%, #000 95%);
-          mask-image: linear-gradient(130deg, #000 55%, rgba(0, 0, 0, 0.8) 75%, #000 95%);
+  mask-image: linear-gradient(130deg, #000 55%, rgba(0, 0, 0, 0.8) 75%, #000 95%);
   -webkit-mask-size: 200% 100%;
-          mask-size: 200% 100%;
+  mask-size: 200% 100%;
   animation: placeholder-wave 2s linear infinite;
 }
 
 @keyframes placeholder-wave {
   100% {
     -webkit-mask-position: -200% 0%;
-            mask-position: -200% 0%;
+    mask-position: -200% 0%;
   }
 }
+
 .clearfix::after {
   display: block;
   clear: both;
   content: "";
 }
 
 .text-bg-primary {
@@ -6693,77 +7656,95 @@
   color: #fff !important;
   background-color: RGBA(33, 37, 41, var(--bs-bg-opacity, 1)) !important;
 }
 
 .link-primary {
   color: #0d6efd !important;
 }
-.link-primary:hover, .link-primary:focus {
+
+.link-primary:hover,
+.link-primary:focus {
   color: #0a58ca !important;
 }
 
 .link-secondary {
   color: #6c757d !important;
 }
-.link-secondary:hover, .link-secondary:focus {
+
+.link-secondary:hover,
+.link-secondary:focus {
   color: #565e64 !important;
 }
 
 .link-success {
   color: #198754 !important;
 }
-.link-success:hover, .link-success:focus {
+
+.link-success:hover,
+.link-success:focus {
   color: #146c43 !important;
 }
 
 .link-info {
   color: #0dcaf0 !important;
 }
-.link-info:hover, .link-info:focus {
+
+.link-info:hover,
+.link-info:focus {
   color: #3dd5f3 !important;
 }
 
 .link-warning {
   color: #ffc107 !important;
 }
-.link-warning:hover, .link-warning:focus {
+
+.link-warning:hover,
+.link-warning:focus {
   color: #ffcd39 !important;
 }
 
 .link-danger {
   color: #dc3545 !important;
 }
-.link-danger:hover, .link-danger:focus {
+
+.link-danger:hover,
+.link-danger:focus {
   color: #b02a37 !important;
 }
 
 .link-light {
   color: #f8f9fa !important;
 }
-.link-light:hover, .link-light:focus {
+
+.link-light:hover,
+.link-light:focus {
   color: #f9fafb !important;
 }
 
 .link-dark {
   color: #212529 !important;
 }
-.link-dark:hover, .link-dark:focus {
+
+.link-dark:hover,
+.link-dark:focus {
   color: #1a1e21 !important;
 }
 
 .ratio {
   position: relative;
   width: 100%;
 }
+
 .ratio::before {
   display: block;
   padding-top: var(--bs-aspect-ratio);
   content: "";
 }
-.ratio > * {
+
+.ratio>* {
   position: absolute;
   top: 0;
   left: 0;
   width: 100%;
   height: 100%;
 }
 
@@ -6813,68 +7794,78 @@
 
 @media (min-width: 576px) {
   .sticky-sm-top {
     position: sticky;
     top: 0;
     z-index: 1020;
   }
+
   .sticky-sm-bottom {
     position: sticky;
     bottom: 0;
     z-index: 1020;
   }
 }
+
 @media (min-width: 768px) {
   .sticky-md-top {
     position: sticky;
     top: 0;
     z-index: 1020;
   }
+
   .sticky-md-bottom {
     position: sticky;
     bottom: 0;
     z-index: 1020;
   }
 }
+
 @media (min-width: 992px) {
   .sticky-lg-top {
     position: sticky;
     top: 0;
     z-index: 1020;
   }
+
   .sticky-lg-bottom {
     position: sticky;
     bottom: 0;
     z-index: 1020;
   }
 }
+
 @media (min-width: 1200px) {
   .sticky-xl-top {
     position: sticky;
     top: 0;
     z-index: 1020;
   }
+
   .sticky-xl-bottom {
     position: sticky;
     bottom: 0;
     z-index: 1020;
   }
 }
+
 @media (min-width: 1400px) {
   .sticky-xxl-top {
     position: sticky;
     top: 0;
     z-index: 1020;
   }
+
   .sticky-xxl-bottom {
     position: sticky;
     bottom: 0;
     z-index: 1020;
   }
 }
+
 .hstack {
   display: flex;
   flex-direction: row;
   align-items: center;
   align-self: stretch;
 }
 
@@ -8206,28 +9197,28 @@
 
 .bg-gradient {
   background-image: var(--bs-gradient) !important;
 }
 
 .user-select-all {
   -webkit-user-select: all !important;
-     -moz-user-select: all !important;
-          user-select: all !important;
+  -moz-user-select: all !important;
+  user-select: all !important;
 }
 
 .user-select-auto {
   -webkit-user-select: auto !important;
-     -moz-user-select: auto !important;
-          user-select: auto !important;
+  -moz-user-select: auto !important;
+  user-select: auto !important;
 }
 
 .user-select-none {
   -webkit-user-select: none !important;
-     -moz-user-select: none !important;
-          user-select: none !important;
+  -moz-user-select: none !important;
+  user-select: none !important;
 }
 
 .pe-none {
   pointer-events: none !important;
 }
 
 .pe-auto {
@@ -8298,2536 +9289,3330 @@
   visibility: hidden !important;
 }
 
 @media (min-width: 576px) {
   .float-sm-start {
     float: left !important;
   }
+
   .float-sm-end {
     float: right !important;
   }
+
   .float-sm-none {
     float: none !important;
   }
+
   .d-sm-inline {
     display: inline !important;
   }
+
   .d-sm-inline-block {
     display: inline-block !important;
   }
+
   .d-sm-block {
     display: block !important;
   }
+
   .d-sm-grid {
     display: grid !important;
   }
+
   .d-sm-table {
     display: table !important;
   }
+
   .d-sm-table-row {
     display: table-row !important;
   }
+
   .d-sm-table-cell {
     display: table-cell !important;
   }
+
   .d-sm-flex {
     display: flex !important;
   }
+
   .d-sm-inline-flex {
     display: inline-flex !important;
   }
+
   .d-sm-none {
     display: none !important;
   }
+
   .flex-sm-fill {
     flex: 1 1 auto !important;
   }
+
   .flex-sm-row {
     flex-direction: row !important;
   }
+
   .flex-sm-column {
     flex-direction: column !important;
   }
+
   .flex-sm-row-reverse {
     flex-direction: row-reverse !important;
   }
+
   .flex-sm-column-reverse {
     flex-direction: column-reverse !important;
   }
+
   .flex-sm-grow-0 {
     flex-grow: 0 !important;
   }
+
   .flex-sm-grow-1 {
     flex-grow: 1 !important;
   }
+
   .flex-sm-shrink-0 {
     flex-shrink: 0 !important;
   }
+
   .flex-sm-shrink-1 {
     flex-shrink: 1 !important;
   }
+
   .flex-sm-wrap {
     flex-wrap: wrap !important;
   }
+
   .flex-sm-nowrap {
     flex-wrap: nowrap !important;
   }
+
   .flex-sm-wrap-reverse {
     flex-wrap: wrap-reverse !important;
   }
+
   .justify-content-sm-start {
     justify-content: flex-start !important;
   }
+
   .justify-content-sm-end {
     justify-content: flex-end !important;
   }
+
   .justify-content-sm-center {
     justify-content: center !important;
   }
+
   .justify-content-sm-between {
     justify-content: space-between !important;
   }
+
   .justify-content-sm-around {
     justify-content: space-around !important;
   }
+
   .justify-content-sm-evenly {
     justify-content: space-evenly !important;
   }
+
   .align-items-sm-start {
     align-items: flex-start !important;
   }
+
   .align-items-sm-end {
     align-items: flex-end !important;
   }
+
   .align-items-sm-center {
     align-items: center !important;
   }
+
   .align-items-sm-baseline {
     align-items: baseline !important;
   }
+
   .align-items-sm-stretch {
     align-items: stretch !important;
   }
+
   .align-content-sm-start {
     align-content: flex-start !important;
   }
+
   .align-content-sm-end {
     align-content: flex-end !important;
   }
+
   .align-content-sm-center {
     align-content: center !important;
   }
+
   .align-content-sm-between {
     align-content: space-between !important;
   }
+
   .align-content-sm-around {
     align-content: space-around !important;
   }
+
   .align-content-sm-stretch {
     align-content: stretch !important;
   }
+
   .align-self-sm-auto {
     align-self: auto !important;
   }
+
   .align-self-sm-start {
     align-self: flex-start !important;
   }
+
   .align-self-sm-end {
     align-self: flex-end !important;
   }
+
   .align-self-sm-center {
     align-self: center !important;
   }
+
   .align-self-sm-baseline {
     align-self: baseline !important;
   }
+
   .align-self-sm-stretch {
     align-self: stretch !important;
   }
+
   .order-sm-first {
     order: -1 !important;
   }
+
   .order-sm-0 {
     order: 0 !important;
   }
+
   .order-sm-1 {
     order: 1 !important;
   }
+
   .order-sm-2 {
     order: 2 !important;
   }
+
   .order-sm-3 {
     order: 3 !important;
   }
+
   .order-sm-4 {
     order: 4 !important;
   }
+
   .order-sm-5 {
     order: 5 !important;
   }
+
   .order-sm-last {
     order: 6 !important;
   }
+
   .m-sm-0 {
     margin: 0 !important;
   }
+
   .m-sm-1 {
     margin: 0.25rem !important;
   }
+
   .m-sm-2 {
     margin: 0.5rem !important;
   }
+
   .m-sm-3 {
     margin: 1rem !important;
   }
+
   .m-sm-4 {
     margin: 1.5rem !important;
   }
+
   .m-sm-5 {
     margin: 3rem !important;
   }
+
   .m-sm-auto {
     margin: auto !important;
   }
+
   .mx-sm-0 {
     margin-right: 0 !important;
     margin-left: 0 !important;
   }
+
   .mx-sm-1 {
     margin-right: 0.25rem !important;
     margin-left: 0.25rem !important;
   }
+
   .mx-sm-2 {
     margin-right: 0.5rem !important;
     margin-left: 0.5rem !important;
   }
+
   .mx-sm-3 {
     margin-right: 1rem !important;
     margin-left: 1rem !important;
   }
+
   .mx-sm-4 {
     margin-right: 1.5rem !important;
     margin-left: 1.5rem !important;
   }
+
   .mx-sm-5 {
     margin-right: 3rem !important;
     margin-left: 3rem !important;
   }
+
   .mx-sm-auto {
     margin-right: auto !important;
     margin-left: auto !important;
   }
+
   .my-sm-0 {
     margin-top: 0 !important;
     margin-bottom: 0 !important;
   }
+
   .my-sm-1 {
     margin-top: 0.25rem !important;
     margin-bottom: 0.25rem !important;
   }
+
   .my-sm-2 {
     margin-top: 0.5rem !important;
     margin-bottom: 0.5rem !important;
   }
+
   .my-sm-3 {
     margin-top: 1rem !important;
     margin-bottom: 1rem !important;
   }
+
   .my-sm-4 {
     margin-top: 1.5rem !important;
     margin-bottom: 1.5rem !important;
   }
+
   .my-sm-5 {
     margin-top: 3rem !important;
     margin-bottom: 3rem !important;
   }
+
   .my-sm-auto {
     margin-top: auto !important;
     margin-bottom: auto !important;
   }
+
   .mt-sm-0 {
     margin-top: 0 !important;
   }
+
   .mt-sm-1 {
     margin-top: 0.25rem !important;
   }
+
   .mt-sm-2 {
     margin-top: 0.5rem !important;
   }
+
   .mt-sm-3 {
     margin-top: 1rem !important;
   }
+
   .mt-sm-4 {
     margin-top: 1.5rem !important;
   }
+
   .mt-sm-5 {
     margin-top: 3rem !important;
   }
+
   .mt-sm-auto {
     margin-top: auto !important;
   }
+
   .me-sm-0 {
     margin-right: 0 !important;
   }
+
   .me-sm-1 {
     margin-right: 0.25rem !important;
   }
+
   .me-sm-2 {
     margin-right: 0.5rem !important;
   }
+
   .me-sm-3 {
     margin-right: 1rem !important;
   }
+
   .me-sm-4 {
     margin-right: 1.5rem !important;
   }
+
   .me-sm-5 {
     margin-right: 3rem !important;
   }
+
   .me-sm-auto {
     margin-right: auto !important;
   }
+
   .mb-sm-0 {
     margin-bottom: 0 !important;
   }
+
   .mb-sm-1 {
     margin-bottom: 0.25rem !important;
   }
+
   .mb-sm-2 {
     margin-bottom: 0.5rem !important;
   }
+
   .mb-sm-3 {
     margin-bottom: 1rem !important;
   }
+
   .mb-sm-4 {
     margin-bottom: 1.5rem !important;
   }
+
   .mb-sm-5 {
     margin-bottom: 3rem !important;
   }
+
   .mb-sm-auto {
     margin-bottom: auto !important;
   }
+
   .ms-sm-0 {
     margin-left: 0 !important;
   }
+
   .ms-sm-1 {
     margin-left: 0.25rem !important;
   }
+
   .ms-sm-2 {
     margin-left: 0.5rem !important;
   }
+
   .ms-sm-3 {
     margin-left: 1rem !important;
   }
+
   .ms-sm-4 {
     margin-left: 1.5rem !important;
   }
+
   .ms-sm-5 {
     margin-left: 3rem !important;
   }
+
   .ms-sm-auto {
     margin-left: auto !important;
   }
+
   .p-sm-0 {
     padding: 0 !important;
   }
+
   .p-sm-1 {
     padding: 0.25rem !important;
   }
+
   .p-sm-2 {
     padding: 0.5rem !important;
   }
+
   .p-sm-3 {
     padding: 1rem !important;
   }
+
   .p-sm-4 {
     padding: 1.5rem !important;
   }
+
   .p-sm-5 {
     padding: 3rem !important;
   }
+
   .px-sm-0 {
     padding-right: 0 !important;
     padding-left: 0 !important;
   }
+
   .px-sm-1 {
     padding-right: 0.25rem !important;
     padding-left: 0.25rem !important;
   }
+
   .px-sm-2 {
     padding-right: 0.5rem !important;
     padding-left: 0.5rem !important;
   }
+
   .px-sm-3 {
     padding-right: 1rem !important;
     padding-left: 1rem !important;
   }
+
   .px-sm-4 {
     padding-right: 1.5rem !important;
     padding-left: 1.5rem !important;
   }
+
   .px-sm-5 {
     padding-right: 3rem !important;
     padding-left: 3rem !important;
   }
+
   .py-sm-0 {
     padding-top: 0 !important;
     padding-bottom: 0 !important;
   }
+
   .py-sm-1 {
     padding-top: 0.25rem !important;
     padding-bottom: 0.25rem !important;
   }
+
   .py-sm-2 {
     padding-top: 0.5rem !important;
     padding-bottom: 0.5rem !important;
   }
+
   .py-sm-3 {
     padding-top: 1rem !important;
     padding-bottom: 1rem !important;
   }
+
   .py-sm-4 {
     padding-top: 1.5rem !important;
     padding-bottom: 1.5rem !important;
   }
+
   .py-sm-5 {
     padding-top: 3rem !important;
     padding-bottom: 3rem !important;
   }
+
   .pt-sm-0 {
     padding-top: 0 !important;
   }
+
   .pt-sm-1 {
     padding-top: 0.25rem !important;
   }
+
   .pt-sm-2 {
     padding-top: 0.5rem !important;
   }
+
   .pt-sm-3 {
     padding-top: 1rem !important;
   }
+
   .pt-sm-4 {
     padding-top: 1.5rem !important;
   }
+
   .pt-sm-5 {
     padding-top: 3rem !important;
   }
+
   .pe-sm-0 {
     padding-right: 0 !important;
   }
+
   .pe-sm-1 {
     padding-right: 0.25rem !important;
   }
+
   .pe-sm-2 {
     padding-right: 0.5rem !important;
   }
+
   .pe-sm-3 {
     padding-right: 1rem !important;
   }
+
   .pe-sm-4 {
     padding-right: 1.5rem !important;
   }
+
   .pe-sm-5 {
     padding-right: 3rem !important;
   }
+
   .pb-sm-0 {
     padding-bottom: 0 !important;
   }
+
   .pb-sm-1 {
     padding-bottom: 0.25rem !important;
   }
+
   .pb-sm-2 {
     padding-bottom: 0.5rem !important;
   }
+
   .pb-sm-3 {
     padding-bottom: 1rem !important;
   }
+
   .pb-sm-4 {
     padding-bottom: 1.5rem !important;
   }
+
   .pb-sm-5 {
     padding-bottom: 3rem !important;
   }
+
   .ps-sm-0 {
     padding-left: 0 !important;
   }
+
   .ps-sm-1 {
     padding-left: 0.25rem !important;
   }
+
   .ps-sm-2 {
     padding-left: 0.5rem !important;
   }
+
   .ps-sm-3 {
     padding-left: 1rem !important;
   }
+
   .ps-sm-4 {
     padding-left: 1.5rem !important;
   }
+
   .ps-sm-5 {
     padding-left: 3rem !important;
   }
+
   .gap-sm-0 {
     gap: 0 !important;
   }
+
   .gap-sm-1 {
     gap: 0.25rem !important;
   }
+
   .gap-sm-2 {
     gap: 0.5rem !important;
   }
+
   .gap-sm-3 {
     gap: 1rem !important;
   }
+
   .gap-sm-4 {
     gap: 1.5rem !important;
   }
+
   .gap-sm-5 {
     gap: 3rem !important;
   }
+
   .text-sm-start {
     text-align: left !important;
   }
+
   .text-sm-end {
     text-align: right !important;
   }
+
   .text-sm-center {
     text-align: center !important;
   }
 }
+
 @media (min-width: 768px) {
   .float-md-start {
     float: left !important;
   }
+
   .float-md-end {
     float: right !important;
   }
+
   .float-md-none {
     float: none !important;
   }
+
   .d-md-inline {
     display: inline !important;
   }
+
   .d-md-inline-block {
     display: inline-block !important;
   }
+
   .d-md-block {
     display: block !important;
   }
+
   .d-md-grid {
     display: grid !important;
   }
+
   .d-md-table {
     display: table !important;
   }
+
   .d-md-table-row {
     display: table-row !important;
   }
+
   .d-md-table-cell {
     display: table-cell !important;
   }
+
   .d-md-flex {
     display: flex !important;
   }
+
   .d-md-inline-flex {
     display: inline-flex !important;
   }
+
   .d-md-none {
     display: none !important;
   }
+
   .flex-md-fill {
     flex: 1 1 auto !important;
   }
+
   .flex-md-row {
     flex-direction: row !important;
   }
+
   .flex-md-column {
     flex-direction: column !important;
   }
+
   .flex-md-row-reverse {
     flex-direction: row-reverse !important;
   }
+
   .flex-md-column-reverse {
     flex-direction: column-reverse !important;
   }
+
   .flex-md-grow-0 {
     flex-grow: 0 !important;
   }
+
   .flex-md-grow-1 {
     flex-grow: 1 !important;
   }
+
   .flex-md-shrink-0 {
     flex-shrink: 0 !important;
   }
+
   .flex-md-shrink-1 {
     flex-shrink: 1 !important;
   }
+
   .flex-md-wrap {
     flex-wrap: wrap !important;
   }
+
   .flex-md-nowrap {
     flex-wrap: nowrap !important;
   }
+
   .flex-md-wrap-reverse {
     flex-wrap: wrap-reverse !important;
   }
+
   .justify-content-md-start {
     justify-content: flex-start !important;
   }
+
   .justify-content-md-end {
     justify-content: flex-end !important;
   }
+
   .justify-content-md-center {
     justify-content: center !important;
   }
+
   .justify-content-md-between {
     justify-content: space-between !important;
   }
+
   .justify-content-md-around {
     justify-content: space-around !important;
   }
+
   .justify-content-md-evenly {
     justify-content: space-evenly !important;
   }
+
   .align-items-md-start {
     align-items: flex-start !important;
   }
+
   .align-items-md-end {
     align-items: flex-end !important;
   }
+
   .align-items-md-center {
     align-items: center !important;
   }
+
   .align-items-md-baseline {
     align-items: baseline !important;
   }
+
   .align-items-md-stretch {
     align-items: stretch !important;
   }
+
   .align-content-md-start {
     align-content: flex-start !important;
   }
+
   .align-content-md-end {
     align-content: flex-end !important;
   }
+
   .align-content-md-center {
     align-content: center !important;
   }
+
   .align-content-md-between {
     align-content: space-between !important;
   }
+
   .align-content-md-around {
     align-content: space-around !important;
   }
+
   .align-content-md-stretch {
     align-content: stretch !important;
   }
+
   .align-self-md-auto {
     align-self: auto !important;
   }
+
   .align-self-md-start {
     align-self: flex-start !important;
   }
+
   .align-self-md-end {
     align-self: flex-end !important;
   }
+
   .align-self-md-center {
     align-self: center !important;
   }
+
   .align-self-md-baseline {
     align-self: baseline !important;
   }
+
   .align-self-md-stretch {
     align-self: stretch !important;
   }
+
   .order-md-first {
     order: -1 !important;
   }
+
   .order-md-0 {
     order: 0 !important;
   }
+
   .order-md-1 {
     order: 1 !important;
   }
+
   .order-md-2 {
     order: 2 !important;
   }
+
   .order-md-3 {
     order: 3 !important;
   }
+
   .order-md-4 {
     order: 4 !important;
   }
+
   .order-md-5 {
     order: 5 !important;
   }
+
   .order-md-last {
     order: 6 !important;
   }
+
   .m-md-0 {
     margin: 0 !important;
   }
+
   .m-md-1 {
     margin: 0.25rem !important;
   }
+
   .m-md-2 {
     margin: 0.5rem !important;
   }
+
   .m-md-3 {
     margin: 1rem !important;
   }
+
   .m-md-4 {
     margin: 1.5rem !important;
   }
+
   .m-md-5 {
     margin: 3rem !important;
   }
+
   .m-md-auto {
     margin: auto !important;
   }
+
   .mx-md-0 {
     margin-right: 0 !important;
     margin-left: 0 !important;
   }
+
   .mx-md-1 {
     margin-right: 0.25rem !important;
     margin-left: 0.25rem !important;
   }
+
   .mx-md-2 {
     margin-right: 0.5rem !important;
     margin-left: 0.5rem !important;
   }
+
   .mx-md-3 {
     margin-right: 1rem !important;
     margin-left: 1rem !important;
   }
+
   .mx-md-4 {
     margin-right: 1.5rem !important;
     margin-left: 1.5rem !important;
   }
+
   .mx-md-5 {
     margin-right: 3rem !important;
     margin-left: 3rem !important;
   }
+
   .mx-md-auto {
     margin-right: auto !important;
     margin-left: auto !important;
   }
+
   .my-md-0 {
     margin-top: 0 !important;
     margin-bottom: 0 !important;
   }
+
   .my-md-1 {
     margin-top: 0.25rem !important;
     margin-bottom: 0.25rem !important;
   }
+
   .my-md-2 {
     margin-top: 0.5rem !important;
     margin-bottom: 0.5rem !important;
   }
+
   .my-md-3 {
     margin-top: 1rem !important;
     margin-bottom: 1rem !important;
   }
+
   .my-md-4 {
     margin-top: 1.5rem !important;
     margin-bottom: 1.5rem !important;
   }
+
   .my-md-5 {
     margin-top: 3rem !important;
     margin-bottom: 3rem !important;
   }
+
   .my-md-auto {
     margin-top: auto !important;
     margin-bottom: auto !important;
   }
+
   .mt-md-0 {
     margin-top: 0 !important;
   }
+
   .mt-md-1 {
     margin-top: 0.25rem !important;
   }
+
   .mt-md-2 {
     margin-top: 0.5rem !important;
   }
+
   .mt-md-3 {
     margin-top: 1rem !important;
   }
+
   .mt-md-4 {
     margin-top: 1.5rem !important;
   }
+
   .mt-md-5 {
     margin-top: 3rem !important;
   }
+
   .mt-md-auto {
     margin-top: auto !important;
   }
+
   .me-md-0 {
     margin-right: 0 !important;
   }
+
   .me-md-1 {
     margin-right: 0.25rem !important;
   }
+
   .me-md-2 {
     margin-right: 0.5rem !important;
   }
+
   .me-md-3 {
     margin-right: 1rem !important;
   }
+
   .me-md-4 {
     margin-right: 1.5rem !important;
   }
+
   .me-md-5 {
     margin-right: 3rem !important;
   }
+
   .me-md-auto {
     margin-right: auto !important;
   }
+
   .mb-md-0 {
     margin-bottom: 0 !important;
   }
+
   .mb-md-1 {
     margin-bottom: 0.25rem !important;
   }
+
   .mb-md-2 {
     margin-bottom: 0.5rem !important;
   }
+
   .mb-md-3 {
     margin-bottom: 1rem !important;
   }
+
   .mb-md-4 {
     margin-bottom: 1.5rem !important;
   }
+
   .mb-md-5 {
     margin-bottom: 3rem !important;
   }
+
   .mb-md-auto {
     margin-bottom: auto !important;
   }
+
   .ms-md-0 {
     margin-left: 0 !important;
   }
+
   .ms-md-1 {
     margin-left: 0.25rem !important;
   }
+
   .ms-md-2 {
     margin-left: 0.5rem !important;
   }
+
   .ms-md-3 {
     margin-left: 1rem !important;
   }
+
   .ms-md-4 {
     margin-left: 1.5rem !important;
   }
+
   .ms-md-5 {
     margin-left: 3rem !important;
   }
+
   .ms-md-auto {
     margin-left: auto !important;
   }
+
   .p-md-0 {
     padding: 0 !important;
   }
+
   .p-md-1 {
     padding: 0.25rem !important;
   }
+
   .p-md-2 {
     padding: 0.5rem !important;
   }
+
   .p-md-3 {
     padding: 1rem !important;
   }
+
   .p-md-4 {
     padding: 1.5rem !important;
   }
+
   .p-md-5 {
     padding: 3rem !important;
   }
+
   .px-md-0 {
     padding-right: 0 !important;
     padding-left: 0 !important;
   }
+
   .px-md-1 {
     padding-right: 0.25rem !important;
     padding-left: 0.25rem !important;
   }
+
   .px-md-2 {
     padding-right: 0.5rem !important;
     padding-left: 0.5rem !important;
   }
+
   .px-md-3 {
     padding-right: 1rem !important;
     padding-left: 1rem !important;
   }
+
   .px-md-4 {
     padding-right: 1.5rem !important;
     padding-left: 1.5rem !important;
   }
+
   .px-md-5 {
     padding-right: 3rem !important;
     padding-left: 3rem !important;
   }
+
   .py-md-0 {
     padding-top: 0 !important;
     padding-bottom: 0 !important;
   }
+
   .py-md-1 {
     padding-top: 0.25rem !important;
     padding-bottom: 0.25rem !important;
   }
+
   .py-md-2 {
     padding-top: 0.5rem !important;
     padding-bottom: 0.5rem !important;
   }
+
   .py-md-3 {
     padding-top: 1rem !important;
     padding-bottom: 1rem !important;
   }
+
   .py-md-4 {
     padding-top: 1.5rem !important;
     padding-bottom: 1.5rem !important;
   }
+
   .py-md-5 {
     padding-top: 3rem !important;
     padding-bottom: 3rem !important;
   }
+
   .pt-md-0 {
     padding-top: 0 !important;
   }
+
   .pt-md-1 {
     padding-top: 0.25rem !important;
   }
+
   .pt-md-2 {
     padding-top: 0.5rem !important;
   }
+
   .pt-md-3 {
     padding-top: 1rem !important;
   }
+
   .pt-md-4 {
     padding-top: 1.5rem !important;
   }
+
   .pt-md-5 {
     padding-top: 3rem !important;
   }
+
   .pe-md-0 {
     padding-right: 0 !important;
   }
+
   .pe-md-1 {
     padding-right: 0.25rem !important;
   }
+
   .pe-md-2 {
     padding-right: 0.5rem !important;
   }
+
   .pe-md-3 {
     padding-right: 1rem !important;
   }
+
   .pe-md-4 {
     padding-right: 1.5rem !important;
   }
+
   .pe-md-5 {
     padding-right: 3rem !important;
   }
+
   .pb-md-0 {
     padding-bottom: 0 !important;
   }
+
   .pb-md-1 {
     padding-bottom: 0.25rem !important;
   }
+
   .pb-md-2 {
     padding-bottom: 0.5rem !important;
   }
+
   .pb-md-3 {
     padding-bottom: 1rem !important;
   }
+
   .pb-md-4 {
     padding-bottom: 1.5rem !important;
   }
+
   .pb-md-5 {
     padding-bottom: 3rem !important;
   }
+
   .ps-md-0 {
     padding-left: 0 !important;
   }
+
   .ps-md-1 {
     padding-left: 0.25rem !important;
   }
+
   .ps-md-2 {
     padding-left: 0.5rem !important;
   }
+
   .ps-md-3 {
     padding-left: 1rem !important;
   }
+
   .ps-md-4 {
     padding-left: 1.5rem !important;
   }
+
   .ps-md-5 {
     padding-left: 3rem !important;
   }
+
   .gap-md-0 {
     gap: 0 !important;
   }
+
   .gap-md-1 {
     gap: 0.25rem !important;
   }
+
   .gap-md-2 {
     gap: 0.5rem !important;
   }
+
   .gap-md-3 {
     gap: 1rem !important;
   }
+
   .gap-md-4 {
     gap: 1.5rem !important;
   }
+
   .gap-md-5 {
     gap: 3rem !important;
   }
+
   .text-md-start {
     text-align: left !important;
   }
+
   .text-md-end {
     text-align: right !important;
   }
+
   .text-md-center {
     text-align: center !important;
   }
 }
+
 @media (min-width: 992px) {
   .float-lg-start {
     float: left !important;
   }
+
   .float-lg-end {
     float: right !important;
   }
+
   .float-lg-none {
     float: none !important;
   }
+
   .d-lg-inline {
     display: inline !important;
   }
+
   .d-lg-inline-block {
     display: inline-block !important;
   }
+
   .d-lg-block {
     display: block !important;
   }
+
   .d-lg-grid {
     display: grid !important;
   }
+
   .d-lg-table {
     display: table !important;
   }
+
   .d-lg-table-row {
     display: table-row !important;
   }
+
   .d-lg-table-cell {
     display: table-cell !important;
   }
+
   .d-lg-flex {
     display: flex !important;
   }
+
   .d-lg-inline-flex {
     display: inline-flex !important;
   }
+
   .d-lg-none {
     display: none !important;
   }
+
   .flex-lg-fill {
     flex: 1 1 auto !important;
   }
+
   .flex-lg-row {
     flex-direction: row !important;
   }
+
   .flex-lg-column {
     flex-direction: column !important;
   }
+
   .flex-lg-row-reverse {
     flex-direction: row-reverse !important;
   }
+
   .flex-lg-column-reverse {
     flex-direction: column-reverse !important;
   }
+
   .flex-lg-grow-0 {
     flex-grow: 0 !important;
   }
+
   .flex-lg-grow-1 {
     flex-grow: 1 !important;
   }
+
   .flex-lg-shrink-0 {
     flex-shrink: 0 !important;
   }
+
   .flex-lg-shrink-1 {
     flex-shrink: 1 !important;
   }
+
   .flex-lg-wrap {
     flex-wrap: wrap !important;
   }
+
   .flex-lg-nowrap {
     flex-wrap: nowrap !important;
   }
+
   .flex-lg-wrap-reverse {
     flex-wrap: wrap-reverse !important;
   }
+
   .justify-content-lg-start {
     justify-content: flex-start !important;
   }
+
   .justify-content-lg-end {
     justify-content: flex-end !important;
   }
+
   .justify-content-lg-center {
     justify-content: center !important;
   }
+
   .justify-content-lg-between {
     justify-content: space-between !important;
   }
+
   .justify-content-lg-around {
     justify-content: space-around !important;
   }
+
   .justify-content-lg-evenly {
     justify-content: space-evenly !important;
   }
+
   .align-items-lg-start {
     align-items: flex-start !important;
   }
+
   .align-items-lg-end {
     align-items: flex-end !important;
   }
+
   .align-items-lg-center {
     align-items: center !important;
   }
+
   .align-items-lg-baseline {
     align-items: baseline !important;
   }
+
   .align-items-lg-stretch {
     align-items: stretch !important;
   }
+
   .align-content-lg-start {
     align-content: flex-start !important;
   }
+
   .align-content-lg-end {
     align-content: flex-end !important;
   }
+
   .align-content-lg-center {
     align-content: center !important;
   }
+
   .align-content-lg-between {
     align-content: space-between !important;
   }
+
   .align-content-lg-around {
     align-content: space-around !important;
   }
+
   .align-content-lg-stretch {
     align-content: stretch !important;
   }
+
   .align-self-lg-auto {
     align-self: auto !important;
   }
+
   .align-self-lg-start {
     align-self: flex-start !important;
   }
+
   .align-self-lg-end {
     align-self: flex-end !important;
   }
+
   .align-self-lg-center {
     align-self: center !important;
   }
+
   .align-self-lg-baseline {
     align-self: baseline !important;
   }
+
   .align-self-lg-stretch {
     align-self: stretch !important;
   }
+
   .order-lg-first {
     order: -1 !important;
   }
+
   .order-lg-0 {
     order: 0 !important;
   }
+
   .order-lg-1 {
     order: 1 !important;
   }
+
   .order-lg-2 {
     order: 2 !important;
   }
+
   .order-lg-3 {
     order: 3 !important;
   }
+
   .order-lg-4 {
     order: 4 !important;
   }
+
   .order-lg-5 {
     order: 5 !important;
   }
+
   .order-lg-last {
     order: 6 !important;
   }
+
   .m-lg-0 {
     margin: 0 !important;
   }
+
   .m-lg-1 {
     margin: 0.25rem !important;
   }
+
   .m-lg-2 {
     margin: 0.5rem !important;
   }
+
   .m-lg-3 {
     margin: 1rem !important;
   }
+
   .m-lg-4 {
     margin: 1.5rem !important;
   }
+
   .m-lg-5 {
     margin: 3rem !important;
   }
+
   .m-lg-auto {
     margin: auto !important;
   }
+
   .mx-lg-0 {
     margin-right: 0 !important;
     margin-left: 0 !important;
   }
+
   .mx-lg-1 {
     margin-right: 0.25rem !important;
     margin-left: 0.25rem !important;
   }
+
   .mx-lg-2 {
     margin-right: 0.5rem !important;
     margin-left: 0.5rem !important;
   }
+
   .mx-lg-3 {
     margin-right: 1rem !important;
     margin-left: 1rem !important;
   }
+
   .mx-lg-4 {
     margin-right: 1.5rem !important;
     margin-left: 1.5rem !important;
   }
+
   .mx-lg-5 {
     margin-right: 3rem !important;
     margin-left: 3rem !important;
   }
+
   .mx-lg-auto {
     margin-right: auto !important;
     margin-left: auto !important;
   }
+
   .my-lg-0 {
     margin-top: 0 !important;
     margin-bottom: 0 !important;
   }
+
   .my-lg-1 {
     margin-top: 0.25rem !important;
     margin-bottom: 0.25rem !important;
   }
+
   .my-lg-2 {
     margin-top: 0.5rem !important;
     margin-bottom: 0.5rem !important;
   }
+
   .my-lg-3 {
     margin-top: 1rem !important;
     margin-bottom: 1rem !important;
   }
+
   .my-lg-4 {
     margin-top: 1.5rem !important;
     margin-bottom: 1.5rem !important;
   }
+
   .my-lg-5 {
     margin-top: 3rem !important;
     margin-bottom: 3rem !important;
   }
+
   .my-lg-auto {
     margin-top: auto !important;
     margin-bottom: auto !important;
   }
+
   .mt-lg-0 {
     margin-top: 0 !important;
   }
+
   .mt-lg-1 {
     margin-top: 0.25rem !important;
   }
+
   .mt-lg-2 {
     margin-top: 0.5rem !important;
   }
+
   .mt-lg-3 {
     margin-top: 1rem !important;
   }
+
   .mt-lg-4 {
     margin-top: 1.5rem !important;
   }
+
   .mt-lg-5 {
     margin-top: 3rem !important;
   }
+
   .mt-lg-auto {
     margin-top: auto !important;
   }
+
   .me-lg-0 {
     margin-right: 0 !important;
   }
+
   .me-lg-1 {
     margin-right: 0.25rem !important;
   }
+
   .me-lg-2 {
     margin-right: 0.5rem !important;
   }
+
   .me-lg-3 {
     margin-right: 1rem !important;
   }
+
   .me-lg-4 {
     margin-right: 1.5rem !important;
   }
+
   .me-lg-5 {
     margin-right: 3rem !important;
   }
+
   .me-lg-auto {
     margin-right: auto !important;
   }
+
   .mb-lg-0 {
     margin-bottom: 0 !important;
   }
+
   .mb-lg-1 {
     margin-bottom: 0.25rem !important;
   }
+
   .mb-lg-2 {
     margin-bottom: 0.5rem !important;
   }
+
   .mb-lg-3 {
     margin-bottom: 1rem !important;
   }
+
   .mb-lg-4 {
     margin-bottom: 1.5rem !important;
   }
+
   .mb-lg-5 {
     margin-bottom: 3rem !important;
   }
+
   .mb-lg-auto {
     margin-bottom: auto !important;
   }
+
   .ms-lg-0 {
     margin-left: 0 !important;
   }
+
   .ms-lg-1 {
     margin-left: 0.25rem !important;
   }
+
   .ms-lg-2 {
     margin-left: 0.5rem !important;
   }
+
   .ms-lg-3 {
     margin-left: 1rem !important;
   }
+
   .ms-lg-4 {
     margin-left: 1.5rem !important;
   }
+
   .ms-lg-5 {
     margin-left: 3rem !important;
   }
+
   .ms-lg-auto {
     margin-left: auto !important;
   }
+
   .p-lg-0 {
     padding: 0 !important;
   }
+
   .p-lg-1 {
     padding: 0.25rem !important;
   }
+
   .p-lg-2 {
     padding: 0.5rem !important;
   }
+
   .p-lg-3 {
     padding: 1rem !important;
   }
+
   .p-lg-4 {
     padding: 1.5rem !important;
   }
+
   .p-lg-5 {
     padding: 3rem !important;
   }
+
   .px-lg-0 {
     padding-right: 0 !important;
     padding-left: 0 !important;
   }
+
   .px-lg-1 {
     padding-right: 0.25rem !important;
     padding-left: 0.25rem !important;
   }
+
   .px-lg-2 {
     padding-right: 0.5rem !important;
     padding-left: 0.5rem !important;
   }
+
   .px-lg-3 {
     padding-right: 1rem !important;
     padding-left: 1rem !important;
   }
+
   .px-lg-4 {
     padding-right: 1.5rem !important;
     padding-left: 1.5rem !important;
   }
+
   .px-lg-5 {
     padding-right: 3rem !important;
     padding-left: 3rem !important;
   }
+
   .py-lg-0 {
     padding-top: 0 !important;
     padding-bottom: 0 !important;
   }
+
   .py-lg-1 {
     padding-top: 0.25rem !important;
     padding-bottom: 0.25rem !important;
   }
+
   .py-lg-2 {
     padding-top: 0.5rem !important;
     padding-bottom: 0.5rem !important;
   }
+
   .py-lg-3 {
     padding-top: 1rem !important;
     padding-bottom: 1rem !important;
   }
+
   .py-lg-4 {
     padding-top: 1.5rem !important;
     padding-bottom: 1.5rem !important;
   }
+
   .py-lg-5 {
     padding-top: 3rem !important;
     padding-bottom: 3rem !important;
   }
+
   .pt-lg-0 {
     padding-top: 0 !important;
   }
+
   .pt-lg-1 {
     padding-top: 0.25rem !important;
   }
+
   .pt-lg-2 {
     padding-top: 0.5rem !important;
   }
+
   .pt-lg-3 {
     padding-top: 1rem !important;
   }
+
   .pt-lg-4 {
     padding-top: 1.5rem !important;
   }
+
   .pt-lg-5 {
     padding-top: 3rem !important;
   }
+
   .pe-lg-0 {
     padding-right: 0 !important;
   }
+
   .pe-lg-1 {
     padding-right: 0.25rem !important;
   }
+
   .pe-lg-2 {
     padding-right: 0.5rem !important;
   }
+
   .pe-lg-3 {
     padding-right: 1rem !important;
   }
+
   .pe-lg-4 {
     padding-right: 1.5rem !important;
   }
+
   .pe-lg-5 {
     padding-right: 3rem !important;
   }
+
   .pb-lg-0 {
     padding-bottom: 0 !important;
   }
+
   .pb-lg-1 {
     padding-bottom: 0.25rem !important;
   }
+
   .pb-lg-2 {
     padding-bottom: 0.5rem !important;
   }
+
   .pb-lg-3 {
     padding-bottom: 1rem !important;
   }
+
   .pb-lg-4 {
     padding-bottom: 1.5rem !important;
   }
+
   .pb-lg-5 {
     padding-bottom: 3rem !important;
   }
+
   .ps-lg-0 {
     padding-left: 0 !important;
   }
+
   .ps-lg-1 {
     padding-left: 0.25rem !important;
   }
+
   .ps-lg-2 {
     padding-left: 0.5rem !important;
   }
+
   .ps-lg-3 {
     padding-left: 1rem !important;
   }
+
   .ps-lg-4 {
     padding-left: 1.5rem !important;
   }
+
   .ps-lg-5 {
     padding-left: 3rem !important;
   }
+
   .gap-lg-0 {
     gap: 0 !important;
   }
+
   .gap-lg-1 {
     gap: 0.25rem !important;
   }
+
   .gap-lg-2 {
     gap: 0.5rem !important;
   }
+
   .gap-lg-3 {
     gap: 1rem !important;
   }
+
   .gap-lg-4 {
     gap: 1.5rem !important;
   }
+
   .gap-lg-5 {
     gap: 3rem !important;
   }
+
   .text-lg-start {
     text-align: left !important;
   }
+
   .text-lg-end {
     text-align: right !important;
   }
+
   .text-lg-center {
     text-align: center !important;
   }
 }
+
 @media (min-width: 1200px) {
   .float-xl-start {
     float: left !important;
   }
+
   .float-xl-end {
     float: right !important;
   }
+
   .float-xl-none {
     float: none !important;
   }
+
   .d-xl-inline {
     display: inline !important;
   }
+
   .d-xl-inline-block {
     display: inline-block !important;
   }
+
   .d-xl-block {
     display: block !important;
   }
+
   .d-xl-grid {
     display: grid !important;
   }
+
   .d-xl-table {
     display: table !important;
   }
+
   .d-xl-table-row {
     display: table-row !important;
   }
+
   .d-xl-table-cell {
     display: table-cell !important;
   }
+
   .d-xl-flex {
     display: flex !important;
   }
+
   .d-xl-inline-flex {
     display: inline-flex !important;
   }
+
   .d-xl-none {
     display: none !important;
   }
+
   .flex-xl-fill {
     flex: 1 1 auto !important;
   }
+
   .flex-xl-row {
     flex-direction: row !important;
   }
+
   .flex-xl-column {
     flex-direction: column !important;
   }
+
   .flex-xl-row-reverse {
     flex-direction: row-reverse !important;
   }
+
   .flex-xl-column-reverse {
     flex-direction: column-reverse !important;
   }
+
   .flex-xl-grow-0 {
     flex-grow: 0 !important;
   }
+
   .flex-xl-grow-1 {
     flex-grow: 1 !important;
   }
+
   .flex-xl-shrink-0 {
     flex-shrink: 0 !important;
   }
+
   .flex-xl-shrink-1 {
     flex-shrink: 1 !important;
   }
+
   .flex-xl-wrap {
     flex-wrap: wrap !important;
   }
+
   .flex-xl-nowrap {
     flex-wrap: nowrap !important;
   }
+
   .flex-xl-wrap-reverse {
     flex-wrap: wrap-reverse !important;
   }
+
   .justify-content-xl-start {
     justify-content: flex-start !important;
   }
+
   .justify-content-xl-end {
     justify-content: flex-end !important;
   }
+
   .justify-content-xl-center {
     justify-content: center !important;
   }
+
   .justify-content-xl-between {
     justify-content: space-between !important;
   }
+
   .justify-content-xl-around {
     justify-content: space-around !important;
   }
+
   .justify-content-xl-evenly {
     justify-content: space-evenly !important;
   }
+
   .align-items-xl-start {
     align-items: flex-start !important;
   }
+
   .align-items-xl-end {
     align-items: flex-end !important;
   }
+
   .align-items-xl-center {
     align-items: center !important;
   }
+
   .align-items-xl-baseline {
     align-items: baseline !important;
   }
+
   .align-items-xl-stretch {
     align-items: stretch !important;
   }
+
   .align-content-xl-start {
     align-content: flex-start !important;
   }
+
   .align-content-xl-end {
     align-content: flex-end !important;
   }
+
   .align-content-xl-center {
     align-content: center !important;
   }
+
   .align-content-xl-between {
     align-content: space-between !important;
   }
+
   .align-content-xl-around {
     align-content: space-around !important;
   }
+
   .align-content-xl-stretch {
     align-content: stretch !important;
   }
+
   .align-self-xl-auto {
     align-self: auto !important;
   }
+
   .align-self-xl-start {
     align-self: flex-start !important;
   }
+
   .align-self-xl-end {
     align-self: flex-end !important;
   }
+
   .align-self-xl-center {
     align-self: center !important;
   }
+
   .align-self-xl-baseline {
     align-self: baseline !important;
   }
+
   .align-self-xl-stretch {
     align-self: stretch !important;
   }
+
   .order-xl-first {
     order: -1 !important;
   }
+
   .order-xl-0 {
     order: 0 !important;
   }
+
   .order-xl-1 {
     order: 1 !important;
   }
+
   .order-xl-2 {
     order: 2 !important;
   }
+
   .order-xl-3 {
     order: 3 !important;
   }
+
   .order-xl-4 {
     order: 4 !important;
   }
+
   .order-xl-5 {
     order: 5 !important;
   }
+
   .order-xl-last {
     order: 6 !important;
   }
+
   .m-xl-0 {
     margin: 0 !important;
   }
+
   .m-xl-1 {
     margin: 0.25rem !important;
   }
+
   .m-xl-2 {
     margin: 0.5rem !important;
   }
+
   .m-xl-3 {
     margin: 1rem !important;
   }
+
   .m-xl-4 {
     margin: 1.5rem !important;
   }
+
   .m-xl-5 {
     margin: 3rem !important;
   }
+
   .m-xl-auto {
     margin: auto !important;
   }
+
   .mx-xl-0 {
     margin-right: 0 !important;
     margin-left: 0 !important;
   }
+
   .mx-xl-1 {
     margin-right: 0.25rem !important;
     margin-left: 0.25rem !important;
   }
+
   .mx-xl-2 {
     margin-right: 0.5rem !important;
     margin-left: 0.5rem !important;
   }
+
   .mx-xl-3 {
     margin-right: 1rem !important;
     margin-left: 1rem !important;
   }
+
   .mx-xl-4 {
     margin-right: 1.5rem !important;
     margin-left: 1.5rem !important;
   }
+
   .mx-xl-5 {
     margin-right: 3rem !important;
     margin-left: 3rem !important;
   }
+
   .mx-xl-auto {
     margin-right: auto !important;
     margin-left: auto !important;
   }
+
   .my-xl-0 {
     margin-top: 0 !important;
     margin-bottom: 0 !important;
   }
+
   .my-xl-1 {
     margin-top: 0.25rem !important;
     margin-bottom: 0.25rem !important;
   }
+
   .my-xl-2 {
     margin-top: 0.5rem !important;
     margin-bottom: 0.5rem !important;
   }
+
   .my-xl-3 {
     margin-top: 1rem !important;
     margin-bottom: 1rem !important;
   }
+
   .my-xl-4 {
     margin-top: 1.5rem !important;
     margin-bottom: 1.5rem !important;
   }
+
   .my-xl-5 {
     margin-top: 3rem !important;
     margin-bottom: 3rem !important;
   }
+
   .my-xl-auto {
     margin-top: auto !important;
     margin-bottom: auto !important;
   }
+
   .mt-xl-0 {
     margin-top: 0 !important;
   }
+
   .mt-xl-1 {
     margin-top: 0.25rem !important;
   }
+
   .mt-xl-2 {
     margin-top: 0.5rem !important;
   }
+
   .mt-xl-3 {
     margin-top: 1rem !important;
   }
+
   .mt-xl-4 {
     margin-top: 1.5rem !important;
   }
+
   .mt-xl-5 {
     margin-top: 3rem !important;
   }
+
   .mt-xl-auto {
     margin-top: auto !important;
   }
+
   .me-xl-0 {
     margin-right: 0 !important;
   }
+
   .me-xl-1 {
     margin-right: 0.25rem !important;
   }
+
   .me-xl-2 {
     margin-right: 0.5rem !important;
   }
+
   .me-xl-3 {
     margin-right: 1rem !important;
   }
+
   .me-xl-4 {
     margin-right: 1.5rem !important;
   }
+
   .me-xl-5 {
     margin-right: 3rem !important;
   }
+
   .me-xl-auto {
     margin-right: auto !important;
   }
+
   .mb-xl-0 {
     margin-bottom: 0 !important;
   }
+
   .mb-xl-1 {
     margin-bottom: 0.25rem !important;
   }
+
   .mb-xl-2 {
     margin-bottom: 0.5rem !important;
   }
+
   .mb-xl-3 {
     margin-bottom: 1rem !important;
   }
+
   .mb-xl-4 {
     margin-bottom: 1.5rem !important;
   }
+
   .mb-xl-5 {
     margin-bottom: 3rem !important;
   }
+
   .mb-xl-auto {
     margin-bottom: auto !important;
   }
+
   .ms-xl-0 {
     margin-left: 0 !important;
   }
+
   .ms-xl-1 {
     margin-left: 0.25rem !important;
   }
+
   .ms-xl-2 {
     margin-left: 0.5rem !important;
   }
+
   .ms-xl-3 {
     margin-left: 1rem !important;
   }
+
   .ms-xl-4 {
     margin-left: 1.5rem !important;
   }
+
   .ms-xl-5 {
     margin-left: 3rem !important;
   }
+
   .ms-xl-auto {
     margin-left: auto !important;
   }
+
   .p-xl-0 {
     padding: 0 !important;
   }
+
   .p-xl-1 {
     padding: 0.25rem !important;
   }
+
   .p-xl-2 {
     padding: 0.5rem !important;
   }
+
   .p-xl-3 {
     padding: 1rem !important;
   }
+
   .p-xl-4 {
     padding: 1.5rem !important;
   }
+
   .p-xl-5 {
     padding: 3rem !important;
   }
+
   .px-xl-0 {
     padding-right: 0 !important;
     padding-left: 0 !important;
   }
+
   .px-xl-1 {
     padding-right: 0.25rem !important;
     padding-left: 0.25rem !important;
   }
+
   .px-xl-2 {
     padding-right: 0.5rem !important;
     padding-left: 0.5rem !important;
   }
+
   .px-xl-3 {
     padding-right: 1rem !important;
     padding-left: 1rem !important;
   }
+
   .px-xl-4 {
     padding-right: 1.5rem !important;
     padding-left: 1.5rem !important;
   }
+
   .px-xl-5 {
     padding-right: 3rem !important;
     padding-left: 3rem !important;
   }
+
   .py-xl-0 {
     padding-top: 0 !important;
     padding-bottom: 0 !important;
   }
+
   .py-xl-1 {
     padding-top: 0.25rem !important;
     padding-bottom: 0.25rem !important;
   }
+
   .py-xl-2 {
     padding-top: 0.5rem !important;
     padding-bottom: 0.5rem !important;
   }
+
   .py-xl-3 {
     padding-top: 1rem !important;
     padding-bottom: 1rem !important;
   }
+
   .py-xl-4 {
     padding-top: 1.5rem !important;
     padding-bottom: 1.5rem !important;
   }
+
   .py-xl-5 {
     padding-top: 3rem !important;
     padding-bottom: 3rem !important;
   }
+
   .pt-xl-0 {
     padding-top: 0 !important;
   }
+
   .pt-xl-1 {
     padding-top: 0.25rem !important;
   }
+
   .pt-xl-2 {
     padding-top: 0.5rem !important;
   }
+
   .pt-xl-3 {
     padding-top: 1rem !important;
   }
+
   .pt-xl-4 {
     padding-top: 1.5rem !important;
   }
+
   .pt-xl-5 {
     padding-top: 3rem !important;
   }
+
   .pe-xl-0 {
     padding-right: 0 !important;
   }
+
   .pe-xl-1 {
     padding-right: 0.25rem !important;
   }
+
   .pe-xl-2 {
     padding-right: 0.5rem !important;
   }
+
   .pe-xl-3 {
     padding-right: 1rem !important;
   }
+
   .pe-xl-4 {
     padding-right: 1.5rem !important;
   }
+
   .pe-xl-5 {
     padding-right: 3rem !important;
   }
+
   .pb-xl-0 {
     padding-bottom: 0 !important;
   }
+
   .pb-xl-1 {
     padding-bottom: 0.25rem !important;
   }
+
   .pb-xl-2 {
     padding-bottom: 0.5rem !important;
   }
+
   .pb-xl-3 {
     padding-bottom: 1rem !important;
   }
+
   .pb-xl-4 {
     padding-bottom: 1.5rem !important;
   }
+
   .pb-xl-5 {
     padding-bottom: 3rem !important;
   }
+
   .ps-xl-0 {
     padding-left: 0 !important;
   }
+
   .ps-xl-1 {
     padding-left: 0.25rem !important;
   }
+
   .ps-xl-2 {
     padding-left: 0.5rem !important;
   }
+
   .ps-xl-3 {
     padding-left: 1rem !important;
   }
+
   .ps-xl-4 {
     padding-left: 1.5rem !important;
   }
+
   .ps-xl-5 {
     padding-left: 3rem !important;
   }
+
   .gap-xl-0 {
     gap: 0 !important;
   }
+
   .gap-xl-1 {
     gap: 0.25rem !important;
   }
+
   .gap-xl-2 {
     gap: 0.5rem !important;
   }
+
   .gap-xl-3 {
     gap: 1rem !important;
   }
+
   .gap-xl-4 {
     gap: 1.5rem !important;
   }
+
   .gap-xl-5 {
     gap: 3rem !important;
   }
+
   .text-xl-start {
     text-align: left !important;
   }
+
   .text-xl-end {
     text-align: right !important;
   }
+
   .text-xl-center {
     text-align: center !important;
   }
 }
+
 @media (min-width: 1400px) {
   .float-xxl-start {
     float: left !important;
   }
+
   .float-xxl-end {
     float: right !important;
   }
+
   .float-xxl-none {
     float: none !important;
   }
+
   .d-xxl-inline {
     display: inline !important;
   }
+
   .d-xxl-inline-block {
     display: inline-block !important;
   }
+
   .d-xxl-block {
     display: block !important;
   }
+
   .d-xxl-grid {
     display: grid !important;
   }
+
   .d-xxl-table {
     display: table !important;
   }
+
   .d-xxl-table-row {
     display: table-row !important;
   }
+
   .d-xxl-table-cell {
     display: table-cell !important;
   }
+
   .d-xxl-flex {
     display: flex !important;
   }
+
   .d-xxl-inline-flex {
     display: inline-flex !important;
   }
+
   .d-xxl-none {
     display: none !important;
   }
+
   .flex-xxl-fill {
     flex: 1 1 auto !important;
   }
+
   .flex-xxl-row {
     flex-direction: row !important;
   }
+
   .flex-xxl-column {
     flex-direction: column !important;
   }
+
   .flex-xxl-row-reverse {
     flex-direction: row-reverse !important;
   }
+
   .flex-xxl-column-reverse {
     flex-direction: column-reverse !important;
   }
+
   .flex-xxl-grow-0 {
     flex-grow: 0 !important;
   }
+
   .flex-xxl-grow-1 {
     flex-grow: 1 !important;
   }
+
   .flex-xxl-shrink-0 {
     flex-shrink: 0 !important;
   }
+
   .flex-xxl-shrink-1 {
     flex-shrink: 1 !important;
   }
+
   .flex-xxl-wrap {
     flex-wrap: wrap !important;
   }
+
   .flex-xxl-nowrap {
     flex-wrap: nowrap !important;
   }
+
   .flex-xxl-wrap-reverse {
     flex-wrap: wrap-reverse !important;
   }
+
   .justify-content-xxl-start {
     justify-content: flex-start !important;
   }
+
   .justify-content-xxl-end {
     justify-content: flex-end !important;
   }
+
   .justify-content-xxl-center {
     justify-content: center !important;
   }
+
   .justify-content-xxl-between {
     justify-content: space-between !important;
   }
+
   .justify-content-xxl-around {
     justify-content: space-around !important;
   }
+
   .justify-content-xxl-evenly {
     justify-content: space-evenly !important;
   }
+
   .align-items-xxl-start {
     align-items: flex-start !important;
   }
+
   .align-items-xxl-end {
     align-items: flex-end !important;
   }
+
   .align-items-xxl-center {
     align-items: center !important;
   }
+
   .align-items-xxl-baseline {
     align-items: baseline !important;
   }
+
   .align-items-xxl-stretch {
     align-items: stretch !important;
   }
+
   .align-content-xxl-start {
     align-content: flex-start !important;
   }
+
   .align-content-xxl-end {
     align-content: flex-end !important;
   }
+
   .align-content-xxl-center {
     align-content: center !important;
   }
+
   .align-content-xxl-between {
     align-content: space-between !important;
   }
+
   .align-content-xxl-around {
     align-content: space-around !important;
   }
+
   .align-content-xxl-stretch {
     align-content: stretch !important;
   }
+
   .align-self-xxl-auto {
     align-self: auto !important;
   }
+
   .align-self-xxl-start {
     align-self: flex-start !important;
   }
+
   .align-self-xxl-end {
     align-self: flex-end !important;
   }
+
   .align-self-xxl-center {
     align-self: center !important;
   }
+
   .align-self-xxl-baseline {
     align-self: baseline !important;
   }
+
   .align-self-xxl-stretch {
     align-self: stretch !important;
   }
+
   .order-xxl-first {
     order: -1 !important;
   }
+
   .order-xxl-0 {
     order: 0 !important;
   }
+
   .order-xxl-1 {
     order: 1 !important;
   }
+
   .order-xxl-2 {
     order: 2 !important;
   }
+
   .order-xxl-3 {
     order: 3 !important;
   }
+
   .order-xxl-4 {
     order: 4 !important;
   }
+
   .order-xxl-5 {
     order: 5 !important;
   }
+
   .order-xxl-last {
     order: 6 !important;
   }
+
   .m-xxl-0 {
     margin: 0 !important;
   }
+
   .m-xxl-1 {
     margin: 0.25rem !important;
   }
+
   .m-xxl-2 {
     margin: 0.5rem !important;
   }
+
   .m-xxl-3 {
     margin: 1rem !important;
   }
+
   .m-xxl-4 {
     margin: 1.5rem !important;
   }
+
   .m-xxl-5 {
     margin: 3rem !important;
   }
+
   .m-xxl-auto {
     margin: auto !important;
   }
+
   .mx-xxl-0 {
     margin-right: 0 !important;
     margin-left: 0 !important;
   }
+
   .mx-xxl-1 {
     margin-right: 0.25rem !important;
     margin-left: 0.25rem !important;
   }
+
   .mx-xxl-2 {
     margin-right: 0.5rem !important;
     margin-left: 0.5rem !important;
   }
+
   .mx-xxl-3 {
     margin-right: 1rem !important;
     margin-left: 1rem !important;
   }
+
   .mx-xxl-4 {
     margin-right: 1.5rem !important;
     margin-left: 1.5rem !important;
   }
+
   .mx-xxl-5 {
     margin-right: 3rem !important;
     margin-left: 3rem !important;
   }
+
   .mx-xxl-auto {
     margin-right: auto !important;
     margin-left: auto !important;
   }
+
   .my-xxl-0 {
     margin-top: 0 !important;
     margin-bottom: 0 !important;
   }
+
   .my-xxl-1 {
     margin-top: 0.25rem !important;
     margin-bottom: 0.25rem !important;
   }
+
   .my-xxl-2 {
     margin-top: 0.5rem !important;
     margin-bottom: 0.5rem !important;
   }
+
   .my-xxl-3 {
     margin-top: 1rem !important;
     margin-bottom: 1rem !important;
   }
+
   .my-xxl-4 {
     margin-top: 1.5rem !important;
     margin-bottom: 1.5rem !important;
   }
+
   .my-xxl-5 {
     margin-top: 3rem !important;
     margin-bottom: 3rem !important;
   }
+
   .my-xxl-auto {
     margin-top: auto !important;
     margin-bottom: auto !important;
   }
+
   .mt-xxl-0 {
     margin-top: 0 !important;
   }
+
   .mt-xxl-1 {
     margin-top: 0.25rem !important;
   }
+
   .mt-xxl-2 {
     margin-top: 0.5rem !important;
   }
+
   .mt-xxl-3 {
     margin-top: 1rem !important;
   }
+
   .mt-xxl-4 {
     margin-top: 1.5rem !important;
   }
+
   .mt-xxl-5 {
     margin-top: 3rem !important;
   }
+
   .mt-xxl-auto {
     margin-top: auto !important;
   }
+
   .me-xxl-0 {
     margin-right: 0 !important;
   }
+
   .me-xxl-1 {
     margin-right: 0.25rem !important;
   }
+
   .me-xxl-2 {
     margin-right: 0.5rem !important;
   }
+
   .me-xxl-3 {
     margin-right: 1rem !important;
   }
+
   .me-xxl-4 {
     margin-right: 1.5rem !important;
   }
+
   .me-xxl-5 {
     margin-right: 3rem !important;
   }
+
   .me-xxl-auto {
     margin-right: auto !important;
   }
+
   .mb-xxl-0 {
     margin-bottom: 0 !important;
   }
+
   .mb-xxl-1 {
     margin-bottom: 0.25rem !important;
   }
+
   .mb-xxl-2 {
     margin-bottom: 0.5rem !important;
   }
+
   .mb-xxl-3 {
     margin-bottom: 1rem !important;
   }
+
   .mb-xxl-4 {
     margin-bottom: 1.5rem !important;
   }
+
   .mb-xxl-5 {
     margin-bottom: 3rem !important;
   }
+
   .mb-xxl-auto {
     margin-bottom: auto !important;
   }
+
   .ms-xxl-0 {
     margin-left: 0 !important;
   }
+
   .ms-xxl-1 {
     margin-left: 0.25rem !important;
   }
+
   .ms-xxl-2 {
     margin-left: 0.5rem !important;
   }
+
   .ms-xxl-3 {
     margin-left: 1rem !important;
   }
+
   .ms-xxl-4 {
     margin-left: 1.5rem !important;
   }
+
   .ms-xxl-5 {
     margin-left: 3rem !important;
   }
+
   .ms-xxl-auto {
     margin-left: auto !important;
   }
+
   .p-xxl-0 {
     padding: 0 !important;
   }
+
   .p-xxl-1 {
     padding: 0.25rem !important;
   }
+
   .p-xxl-2 {
     padding: 0.5rem !important;
   }
+
   .p-xxl-3 {
     padding: 1rem !important;
   }
+
   .p-xxl-4 {
     padding: 1.5rem !important;
   }
+
   .p-xxl-5 {
     padding: 3rem !important;
   }
+
   .px-xxl-0 {
     padding-right: 0 !important;
     padding-left: 0 !important;
   }
+
   .px-xxl-1 {
     padding-right: 0.25rem !important;
     padding-left: 0.25rem !important;
   }
+
   .px-xxl-2 {
     padding-right: 0.5rem !important;
     padding-left: 0.5rem !important;
   }
+
   .px-xxl-3 {
     padding-right: 1rem !important;
     padding-left: 1rem !important;
   }
+
   .px-xxl-4 {
     padding-right: 1.5rem !important;
     padding-left: 1.5rem !important;
   }
+
   .px-xxl-5 {
     padding-right: 3rem !important;
     padding-left: 3rem !important;
   }
+
   .py-xxl-0 {
     padding-top: 0 !important;
     padding-bottom: 0 !important;
   }
+
   .py-xxl-1 {
     padding-top: 0.25rem !important;
     padding-bottom: 0.25rem !important;
   }
+
   .py-xxl-2 {
     padding-top: 0.5rem !important;
     padding-bottom: 0.5rem !important;
   }
+
   .py-xxl-3 {
     padding-top: 1rem !important;
     padding-bottom: 1rem !important;
   }
+
   .py-xxl-4 {
     padding-top: 1.5rem !important;
     padding-bottom: 1.5rem !important;
   }
+
   .py-xxl-5 {
     padding-top: 3rem !important;
     padding-bottom: 3rem !important;
   }
+
   .pt-xxl-0 {
     padding-top: 0 !important;
   }
+
   .pt-xxl-1 {
     padding-top: 0.25rem !important;
   }
+
   .pt-xxl-2 {
     padding-top: 0.5rem !important;
   }
+
   .pt-xxl-3 {
     padding-top: 1rem !important;
   }
+
   .pt-xxl-4 {
     padding-top: 1.5rem !important;
   }
+
   .pt-xxl-5 {
     padding-top: 3rem !important;
   }
+
   .pe-xxl-0 {
     padding-right: 0 !important;
   }
+
   .pe-xxl-1 {
     padding-right: 0.25rem !important;
   }
+
   .pe-xxl-2 {
     padding-right: 0.5rem !important;
   }
+
   .pe-xxl-3 {
     padding-right: 1rem !important;
   }
+
   .pe-xxl-4 {
     padding-right: 1.5rem !important;
   }
+
   .pe-xxl-5 {
     padding-right: 3rem !important;
   }
+
   .pb-xxl-0 {
     padding-bottom: 0 !important;
   }
+
   .pb-xxl-1 {
     padding-bottom: 0.25rem !important;
   }
+
   .pb-xxl-2 {
     padding-bottom: 0.5rem !important;
   }
+
   .pb-xxl-3 {
     padding-bottom: 1rem !important;
   }
+
   .pb-xxl-4 {
     padding-bottom: 1.5rem !important;
   }
+
   .pb-xxl-5 {
     padding-bottom: 3rem !important;
   }
+
   .ps-xxl-0 {
     padding-left: 0 !important;
   }
+
   .ps-xxl-1 {
     padding-left: 0.25rem !important;
   }
+
   .ps-xxl-2 {
     padding-left: 0.5rem !important;
   }
+
   .ps-xxl-3 {
     padding-left: 1rem !important;
   }
+
   .ps-xxl-4 {
     padding-left: 1.5rem !important;
   }
+
   .ps-xxl-5 {
     padding-left: 3rem !important;
   }
+
   .gap-xxl-0 {
     gap: 0 !important;
   }
+
   .gap-xxl-1 {
     gap: 0.25rem !important;
   }
+
   .gap-xxl-2 {
     gap: 0.5rem !important;
   }
+
   .gap-xxl-3 {
     gap: 1rem !important;
   }
+
   .gap-xxl-4 {
     gap: 1.5rem !important;
   }
+
   .gap-xxl-5 {
     gap: 3rem !important;
   }
+
   .text-xxl-start {
     text-align: left !important;
   }
+
   .text-xxl-end {
     text-align: right !important;
   }
+
   .text-xxl-center {
     text-align: center !important;
   }
 }
+
 @media (min-width: 1200px) {
   .fs-1 {
     font-size: 2.5rem !important;
   }
+
   .fs-2 {
     font-size: 2rem !important;
   }
+
   .fs-3 {
     font-size: 1.75rem !important;
   }
+
   .fs-4 {
     font-size: 1.5rem !important;
   }
 }
+
 @media print {
   .d-print-inline {
     display: inline !important;
   }
+
   .d-print-inline-block {
     display: inline-block !important;
   }
+
   .d-print-block {
     display: block !important;
   }
+
   .d-print-grid {
     display: grid !important;
   }
+
   .d-print-table {
     display: table !important;
   }
+
   .d-print-table-row {
     display: table-row !important;
   }
+
   .d-print-table-cell {
     display: table-cell !important;
   }
+
   .d-print-flex {
     display: flex !important;
   }
+
   .d-print-inline-flex {
     display: inline-flex !important;
   }
+
   .d-print-none {
     display: none !important;
   }
 }
+
 body,
 html {
   height: 100%;
 }
 
 .feature {
   display: inline-flex;
@@ -10841,8 +12626,36 @@
 .bg-featured-blog {
   height: 100%;
   width: 100%;
   background-size: cover;
   background-position: center;
   background-repeat: no-repeat;
   min-height: 15rem;
+}
+
+.sidebar {
+  position: -webkit-sticky;
+  position: sticky;
+  top: 0;
+}
+
+p,
+ul {
+  --bs-text-opacity: 1;
+  color: #6c757d !important;
+  font-weight: 400 !important;
+  margin-bottom: 1.15rem !important;
+  font-size: 1.15rem;
+  margin-top: 0;
+  margin-bottom: 1rem;
+}
+
+h1,
+h2,
+h3,
+h4,
+h5,
+h6 {
+  font-weight: bolder !important;
+  margin-bottom: 1.12rem !important;
+  font-size: 1.75rem;
 }
```

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.js` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.js` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.js.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.min.js` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/static/js/scripts.js` & `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/scripts.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/templates/404.html` & `meetlify-0.1.4/src/meetlify/themes/lindau/templates/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
                 <div class="card h-100 shadow border-0">
                     <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.featureimage}}"
                         alt="Feature Image for Meetup">
                     <div class="card-body p-4">
                         <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
                         <a class="text-decoration-none link-dark stretched-link"
                             href="{{meta.URL}}/meetups/{{meetup.slug}}/">
-                            <h5 class="card-title mb-3">Meetup # {{meetup.id}} -
-                                {{meetup.title}}
+                            <h5 class="card-title mb-3"> {{meetup.title}}
                             </h5>
                         </a>
                         <p class="card-text mb-0">Agenda: {{meetup.description}}</p>
                     </div>
                     <div class="card-footer p-4 pt-0 bg-transparent border-top-0">
                         <div class="d-flex align-items-end justify-content-between">
                             <div class="d-flex align-items-center">
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 _H_o_m_e _M_e_e_t_u_p_s
 [{{meta.name}} about us banner]
 ********** MMeeeettuuppss **********
 Here is the list of upcoming meetups organized by {{meta.name}}.
 {% for meetup in meetups%}
 [Feature Image for Meetup]
 Meetup
-_**_**_ _MM_ee_ee_tt_uu_pp_ _##_ _{{_{{_mm_ee_ee_tt_uu_pp_.._ii_dd_}}_}}_ _--_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
+_**_**_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
 Agenda: {{meetup.description}}
 Date: {{meetup.date}} Â· Status: {{{{mmeeeettuupp..ssttaattuuss}}}}
 Location: {{meetup.address}}
 Organizer: {{meetup.author}}
 {% endfor%}
 _O_l_d_e_r_ _M_e_e_t_u_p_s
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/templates/index.html` & `meetlify-0.1.4/src/meetlify/themes/lindau/templates/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 <header class="bg-dark py-5" id="home">
     <div class="container px-5">
         <div class="row gx-5 align-items-center justify-content-center">
             <div class="col-lg-8 col-xl-7 col-xxl-6">
                 <div class="my-5 text-center text-xl-start">
                     <h1 class="display-5 fw-bolder text-white mb-2">{{meta.title}}
                     </h1>
-                    <p class="lead fw-normal text-white-50 mb-4"> Our next meetup is in <em
-                            class="lead fw-normal text-white mb-4">Lindau am Bodensee</em> on
-                        <em class="lead fw-normal text-white mb-4"> {{meetups[0].date}}</em>. Drop us an email at <em
-                            class="lead fw-normal text-white mb-4">{{meta.email}}</em>
-                        if you plan to join. This will help to for better organization of the
-                        event.
+                    <p class="text-white-50 mb-4"> Our next meetup is in <em class="text-white mb-4">Wangen im
+                            Allgäu</em> on
+                        <em class="text-white mb-4"> {{meetups[0].date}}</em>.
+                    </p>
+                    <p class="text-white-50 mb-4">
+                        Drop us an email at <em class="text-white mb-4">{{meta.email}}</em>
+                        if you plan to join. This will help to better organize the event.
                     </p>
                     <div class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xl-start">
                         <a class="btn btn-primary btn-lg px-4 me-sm-3"
                             href="{{meta.URL}}/meetups/{{meetups[0].slug}}/">More Details</a>
                         <a class="btn btn-outline-light btn-lg px-4" href="{{meta.URL}}/meetups/">Future Meetups</a>
                     </div>
                 </div>
@@ -49,31 +50,30 @@
 
 <section class="py-5 bg-light" id="meetups">
     <div class="container px-5 my-5">
         <div class="row gx-5 justify-content-left">
             <div class="col-lg-12">
                 <div class="text-left">
                     <h2 class="fw-bolder  mb-4">Meetups</h2>
-                    <p class="lead fw-normal text-muted mb-5">Here is the list of upcoming meetups organized by
+                    <p class="mb-5">Here is the list of upcoming meetups organized by
                         PyBodensee. </p>
                 </div>
             </div>
         </div>
         <div class="row gx-5">
             {% for meetup in meetups%}
             <div class="col-lg-4 mb-5">
                 <div class="card h-100 shadow border-0">
                     <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.featureimage}}"
                         alt="Feature Image for Meetup">
                     <div class="card-body p-4">
                         <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
                         <a class="text-decoration-none link-dark stretched-link"
                             href="{{meta.URL}}/meetups/{{meetup.slug}}/">
-                            <h5 class="card-title mb-3">Meetup # {{meetup.id}} -
-                                {{meetup.title}}
+                            <h5 class="card-title mb-3"> {{meetup.title}}
                             </h5>
                         </a>
                         <p class="card-text mb-0">Agenda: {{meetup.description}}</p>
                     </div>
                     <div class="card-footer p-4 pt-0 bg-transparent border-top-0">
                         <div class="d-flex align-items-end justify-content-between">
                             <div class="d-flex align-items-center">
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 {% extends "base.html" %} {% block main_header %}
 {% endblock main_header %} {% block main_content %}
 ************ {{{{mmeettaa..ttiittllee}}}} ************
-Our next meetup is in LLiinnddaauu aamm BBooddeennsseeee on {{{{mmeeeettuuppss[[00]]..ddaattee}}}}. Drop us an
-email at {{{{mmeettaa..eemmaaiill}}}} if you plan to join. This will help to for better
-organization of the event.
+Our next meetup is in WWaannggeenn iimm AAllllgg?Ã?¤uu on {{{{mmeeeettuuppss[[00]]..ddaattee}}}}.
+Drop us an email at {{{{mmeettaa..eemmaaiill}}}} if you plan to join. This will help to
+better organize the event.
 _M_o_r_e_ _D_e_t_a_i_l_s _F_u_t_u_r_e_ _M_e_e_t_u_p_s
 [{{meta.name}} about us banner]
 [{{meta.author}} image]
 {{home_content}}
 ********** MMeeeettuuppss **********
 Here is the list of upcoming meetups organized by PyBodensee.
 {% for meetup in meetups%}
 [Feature Image for Meetup]
 Meetup
-_**_**_ _MM_ee_ee_tt_uu_pp_ _##_ _{{_{{_mm_ee_ee_tt_uu_pp_.._ii_dd_}}_}}_ _--_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
+_**_**_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
 Agenda: {{meetup.description}}
 Date: {{meetup.date}} Â· Status: {{{{mmeeeettuupp..ssttaattuuss}}}}
 Location: {{meetup.address}}
 Organizer: {{meetup.author}}
 {% endfor%}
 _O_l_d_e_r_ _M_e_e_t_u_p_s
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/templates/meetup.html` & `meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetup.html`

 * *Files 23% similar despite different names*

```diff
@@ -8,58 +8,69 @@
 {% endblock main_header %}
 
 {% block main_content %}
 <!-- Page Content-->
 <section class="py-5">
     <div class="container px-5 my-5">
         <div class="row gx-5">
-            <div class="col-lg-3">
-                <div class="d-flex align-items-center mt-lg-5 mb-4">
-                    <img class="img-fluid rounded-circle" src="{{meta.URL}}/static/assets/author.png" width="40"
-                        height="40" alt="{{meta.author}} Image" />
-                    <div class="ms-3">
-                        <div class="fw-bold">{{front.author}}</div>
-                        <div class="text-muted">Organizer</div>
-                    </div>
-                </div>
-                <!-- Post meta content-->
-                <div class="row">
-                    <div class="text-muted mb-2">Event Date: <div class="fw-bold">{{front.date}}</div>
-                    </div>
-                    <div class="text-muted mb-2">Event Location: <div class="fw-bold">{{front.address}}</div>
-                    </div>
-                </div>
-                <div class="card border-0 bg-light mt-xl-5">
-                    <div class="card-body p-4 py-lg-5">
-                        <div class="d-flex align-items-center justify-content-center">
-                            <div class="text-center">
-                                <div class="h6 fw-bolder">Have more questions?</div>
-                                <p class="text-muted mb-4">
-                                    Check out our <a href=" {{meta.URL}}/contact/">Contact us</a> page for differnt
-                                    methods to get in touch.
-                                </p>
-                            </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-
-            <div class="col-lg-9">
+            <div class="col-lg-8">
                 <!-- Post content-->
                 <article>
                     <!-- Post header-->
                     <header class="mb-4">
                         <!-- Post title-->
-                        <h1 class="fw-bolder mb-1">Meetup # {{front.id}} - {{front.title}}</h1>
+                        <h1 class="fw-bolder mb-1">{{front.title}}</h1>
                         <!-- Post categories-->
-                        <a class="badge bg-secondary text-decoration-none link-light" href="/">Python</a>
-                        <a class="badge bg-secondary text-decoration-none link-light" href="/">Meetup</a>
+                        <a class="badge bg-secondary text-decoration-none link-light mt-3" href="/">Python</a>
+                        <a class="badge bg-secondary text-decoration-none link-light mt-3" href="/">Meetup</a>
                     </header>
                     <section class="mb-5">
                         {{ content }}
                     </section>
                 </article>
             </div>
+            <div class="col-lg-4">
+                <div class="py-2 sidebar">
+                    <div class="d-flex align-items-center mt-lg-4 mb-4">
+                        <img class="img-fluid rounded-circle" src="{{meta.URL}}/static/assets/author.png" width="60"
+                            height="60" alt="{{meta.author}} Image" />
+                        <div class="ms-3">
+                            <h4 class="fw-bold">{{front.author}} </h4>
+                            <div class="text-muted">Organizer</div>
+                        </div>
+                    </div>
+                    <div class="card border-0 bg-light mt-xl-3">
+                        <div class="card-body p-4 py-lg-4">
+                            <div class="text-muted mb-2">Meetup Date: <div class="fw-bold">{{front.date}}</div>
+                            </div>
+                            <div class="text-muted mb-2">Meetup Location: <div class="fw-bold">{{front.address}}</div>
+                            </div>
+                        </div>
+                    </div>
+
+                    <div class="card border-0 bg-light mt-xl-3">
+                        <div class="card-body p-4 py-lg-4">
+                            <img class="img-fluid rounded mb-5 mb-lg-0" src="{{meta.URL}}/images/{{front.featureimage}}"
+                                alt="{{meta.author}} image">
+                        </div>
+                    </div>
+
+                    <div class="card border-0 bg-light mt-xl-3">
+                        <div class="card-body p-4 py-lg-4">
+                            <div class="d-flex align-items-center justify-content-center">
+                                <div class="text-center">
+                                    <div class="h6 fw-bolder">Have more questions?</div>
+                                    <p class="text-muted mb-4">
+                                        Check out our <a href=" {{meta.URL}}/contact/">Contact us</a> page to get in
+                                        touch
+                                        or to get in touch send us an email at <code>pybodensee at gmail dot com</code>
+                                    </p>
+                                </div>
+                            </div>
+                        </div>
+                    </div>
+                </div>
+            </div>
         </div>
     </div>
 </section>
 {% endblock main_content %}
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 {% extends "base.html" %} {% block main_header %}
 {% endblock main_header %} {% block main_content %}
+************ {{{{ffrroonntt..ttiittllee}}}} ************
+_P_y_t_h_o_n _M_e_e_t_u_p {{ content }}
 [{{meta.author}} Image]
-{{front.author}}
+****** {{{{ffrroonntt..aauutthhoorr}}}} ******
 Organizer
-Event Date:
+Meetup Date:
 {{front.date}}
-Event Location:
+Meetup Location:
 {{front.address}}
+[{{meta.author}} image]
 Have more questions?
-Check out our _C_o_n_t_a_c_t_ _u_s page for differnt methods to get in touch.
-************ MMeeeettuupp ## {{{{ffrroonntt..iidd}}}} -- {{{{ffrroonntt..ttiittllee}}}} ************
-_P_y_t_h_o_n _M_e_e_t_u_p {{ content }}
+Check out our _C_o_n_t_a_c_t_ _u_s page to get in touch or to get in touch send us an
+email at pybodensee at gmail dot com
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.3/src/meetlify/themes/lindau/templates/meetups.html` & `meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetups.html`

 * *Files 14% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 <meta name="author" content="{{meta.author}}" />
 <link href="{{meta.URL}}/meetups/" rel="canonical" />
 <title>Python Meetups in Bodensee Regions</title>
 {% endblock main_header %}
 
 {% block main_content %}
 <!-- Page Content-->
-<section class="py-5">
+<section class="py-5 bg-light">
     <div class="container px-5">
-        <h1 class="fw-bolder fs-5 mb-4">Next Meetup</h1>
+        <h1 class="fw-bolder mb-4">Next Meetup</h1>
         <div class="card border-0 shadow rounded-3 overflow-hidden">
             <div class="card-body p-0">
                 <div class="row gx-0">
                     <div class="col-lg-6 col-xl-5 py-lg-5">
                         <div class="p-4 p-md-5">
                             <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
-                            <div class="h2 fw-bolder">Meetup # {{meetups[0].id}} -
-                                {{meetups[0].title}}</div>
+                            <div class="h2 fw-bolder"> {{meetups[0].title}}</div>
                             <p>{{meetups[0].description}}</p>
                             <a class="stretched-link text-decoration-none"
                                 href="{{meta.URL}}/meetups/{{meetups[0].slug}}/">
                                 Read more <i class="bi bi-arrow-right"></i>
                             </a>
                         </div>
                     </div>
@@ -37,27 +36,26 @@
         </div>
     </div>
 </section>
 
 <!-- Meetup preview section-->
 <section class="py-5">
     <div class="container px-5">
-        <h2 class="fw-bolder fs-5 mb-4">Recent Meetups</h2>
+        <h2 class="fw-bolder mb-4">Recent Meetups</h2>
         <div class="row gx-5">
             {% for meetup in meetups[1:]%}
             <div class="col-lg-4 mb-5">
                 <div class="card h-100 shadow border-0">
                     <img class="card-img-top" src="{{meta.URL}}/images/{{meetup.featureimage}}"
                         alt="Feautre Image for Meetup">
                     <div class="card-body p-4">
                         <div class="badge bg-primary bg-gradient rounded-pill mb-2">Meetup</div>
                         <a class="text-decoration-none link-dark stretched-link"
                             href="{{meta.URL}}/meetups/{{meetup.slug}}/">
-                            <h5 class="card-title mb-3">Meetup # {{meetup.id}} -
-                                {{meetup.title}}
+                            <h5 class="card-title mb-3">{{meetup.title}}
                             </h5>
                         </a>
                         <p class="card-text mb-0">Agenda: {{meetup.description}}</p>
                     </div>
                     <div class="card-footer p-4 pt-0 bg-transparent border-top-0">
                         <div class="d-flex align-items-end justify-content-between">
                             <div class="d-flex align-items-center">
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 {% extends "base.html" %} {% block main_header %}
 {% endblock main_header %} {% block main_content %}
 ************ NNeexxtt MMeeeettuupp ************
 Meetup
-Meetup # {{meetups[0].id}} - {{meetups[0].title}}
+{{meetups[0].title}}
 {{meetups[0].description}}
 _R_e_a_d_ _m_o_r_e
 ********** RReecceenntt MMeeeettuuppss **********
 {% for meetup in meetups[1:]%}
 [Feautre Image for Meetup]
 Meetup
-_**_**_ _MM_ee_ee_tt_uu_pp_ _##_ _{{_{{_mm_ee_ee_tt_uu_pp_.._ii_dd_}}_}}_ _--_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
+_**_**_ _{{_{{_mm_ee_ee_tt_uu_pp_.._tt_ii_tt_ll_ee_}}_}}_ _**_**
 Agenda: {{meetup.description}}
 Date: {{meetup.date}} Â· Status: {{{{mmeeeettuupp..ssttaattuuss}}}}
 Location: {{meetup.address}}
 Organizer: {{meetup.author}}
 {% endfor%}
 {% endblock main_content %}
```

### Comparing `meetlify-0.1.3/src/meetlify/utils.py` & `meetlify-0.1.4/src/meetlify/utils.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.3/src/meetlify.egg-info/PKG-INFO` & `meetlify-0.1.4/src/meetlify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.3.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.4.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -37,14 +37,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: markdown
 Requires-Dist: Jinja2
+Requires-Dist: python-slugify
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: python-language-server[all]; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
@@ -54,24 +55,24 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
-Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
 Requires-Dist: pymdown-extensions; extra == "all"
 Requires-Dist: setuptools; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: black; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
 Requires-Dist: mkdocstrings[python]; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
+Requires-Dist: wheel; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -90,17 +91,17 @@
 
 ### Using Command Line Interface (CLI)
 
 Create an empty folder on your computer or move to a desired location where you want to create the Meetup Website. 
 
 1. Now execute ``meetlify init`` which will crate an empty configuration file (JSON) in the folder. Feel free to edit it as per your need. Content of the configuration file are self explanatory.  
 
-2. Now execute ```meetlify setup`` which will setup the all folders as per your configurations. 
+2. Now execute ``meetlify setup`` which will setup the all folders as per your configurations. 
 
-3. Now execute ```meetlify make`` which will generate full website in output folder.
+3. Now execute ``meetlify make`` which will generate full website in output folder.
 
 
 ### Using Application Programming Interface (API)
 
 You can embed ```meetilify`` into your existing workflow easily. Here is a sample snippet.
 
 ```python
```

### Comparing `meetlify-0.1.3/src/meetlify.egg-info/SOURCES.txt` & `meetlify-0.1.4/src/meetlify.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 src/meetlify/themes/lindau/static/css/bootstrap.css.map
 src/meetlify/themes/lindau/static/css/bootstrap.min.css
 src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
 src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
+src/meetlify/themes/lindau/static/css/cookiealert.css
 src/meetlify/themes/lindau/static/css/styles.css
 src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
 src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
 src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
@@ -79,14 +80,15 @@
 src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
 src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
 src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
 src/meetlify/themes/lindau/static/js/bootstrap.js
 src/meetlify/themes/lindau/static/js/bootstrap.js.map
 src/meetlify/themes/lindau/static/js/bootstrap.min.js
 src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
+src/meetlify/themes/lindau/static/js/cookiealert.js
 src/meetlify/themes/lindau/static/js/scripts.js
 src/meetlify/themes/lindau/templates/404.html
 src/meetlify/themes/lindau/templates/base.html
 src/meetlify/themes/lindau/templates/index.html
 src/meetlify/themes/lindau/templates/meetup.html
 src/meetlify/themes/lindau/templates/meetups.html
 src/meetlify/themes/lindau/templates/page.html
```

### Comparing `meetlify-0.1.3/tests/test_meetups.py` & `meetlify-0.1.4/tests/test_meetups.py`

 * *Files identical despite different names*

