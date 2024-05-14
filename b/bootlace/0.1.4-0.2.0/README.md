# Comparing `tmp/bootlace-0.1.4.tar.gz` & `tmp/bootlace-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon May  6 04:18:23 2024, max compression
+gzip compressed data, last modified: Tue May 14 00:58:10 2024, max compression
```

## Comparing `bootlace-0.1.4.tar` & `bootlace-0.2.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      247 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/__about__.py
--rw-r--r--   0        0        0      384 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/__init__.py
--rw-r--r--   0        0        0      411 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/_version.py
--rw-r--r--   0        0        0     8751 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/breadcrumbs.py
--rw-r--r--   0        0        0     1447 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/extension.py
--rw-r--r--   0        0        0     1139 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/icon.py
--rw-r--r--   0        0        0      465 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/image.py
--rw-r--r--   0        0        0     2004 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/links.py
--rw-r--r--   0        0        0        0 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/py.typed
--rw-r--r--   0        0        0      669 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/size.py
--rw-r--r--   0        0        0     1217 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/style.py
--rw-r--r--   0        0        0     6950 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/util.py
--rw-r--r--   0        0        0        0 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/__init__.py
--rw-r--r--   0        0        0     3037 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/fields.py
--rw-r--r--   0        0        0      661 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/widgets.py
--rw-r--r--   0        0        0     1571 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/forms/templates/bootlace/_form.html
--rw-r--r--   0        0        0      109 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/__init__.py
--rw-r--r--   0        0        0     4638 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/bar.py
--rw-r--r--   0        0        0     5049 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/core.py
--rw-r--r--   0        0        0      427 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/elements.py
--rw-r--r--   0        0        0     2932 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/nav/nav.py
--rw-r--r--   0        0        0    70330 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203179 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51796 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115988 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70404 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203183 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51871 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116065 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12066 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129328 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10127 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51370 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12059 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129343 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10199 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63944 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107824 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267492 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85353 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180382 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107692 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267433 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85282 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180218 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   280814 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.css
--rw-r--r--   0        0        0   679012 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.css.map
--rw-r--r--   0        0        0   232949 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css
--rw-r--r--   0        0        0   589162 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280393 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   678857 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   233056 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   588696 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0    88585 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.css
--rw-r--r--   0        0        0    47188 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.json
--rw-r--r--   0        0        0   211136 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   972584 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.svg
--rw-r--r--   0        0        0   207731 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444287 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80664 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331887 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135747 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305153 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74155 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222463 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145313 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.js
--rw-r--r--   0        0        0   306321 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.js.map
--rw-r--r--   0        0        0    60578 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js
--rw-r--r--   0        0        0   220351 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js.map
--rw-r--r--   0        0        0      299 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/table/__init__.py
--rw-r--r--   0        0        0     4469 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/table/base.py
--rw-r--r--   0        0        0     2339 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/table/columns.py
--rw-r--r--   0        0        0       67 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/testing/__init__.py
--rw-r--r--   0        0        0     4910 2024-05-06 04:18:23.000000 bootlace-0.1.4/src/bootlace/testing/html.py
--rw-r--r--   0        0        0     1222 2024-05-06 04:18:23.000000 bootlace-0.1.4/.gitignore
--rw-r--r--   0        0        0     1096 2024-05-06 04:18:23.000000 bootlace-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      478 2024-05-06 04:18:23.000000 bootlace-0.1.4/README.md
--rw-r--r--   0        0        0     2613 2024-05-06 04:18:23.000000 bootlace-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1323 2024-05-06 04:18:23.000000 bootlace-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      247 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/__about__.py
+-rw-r--r--   0        0        0      384 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/_version.py
+-rw-r--r--   0        0        0     9054 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/breadcrumbs.py
+-rw-r--r--   0        0        0     1447 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/extension.py
+-rw-r--r--   0        0        0     1106 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/icon.py
+-rw-r--r--   0        0        0      465 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/image.py
+-rw-r--r--   0        0        0     2051 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/links.py
+-rw-r--r--   0        0        0        0 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/py.typed
+-rw-r--r--   0        0        0      669 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/size.py
+-rw-r--r--   0        0        0     1217 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/style.py
+-rw-r--r--   0        0        0     9893 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/util.py
+-rw-r--r--   0        0        0        0 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/forms/__init__.py
+-rw-r--r--   0        0        0     3037 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/forms/fields.py
+-rw-r--r--   0        0        0      661 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/forms/widgets.py
+-rw-r--r--   0        0        0     1571 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/forms/templates/bootlace/_form.html
+-rw-r--r--   0        0        0      109 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/nav/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/nav/bar.py
+-rw-r--r--   0        0        0     5442 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/nav/core.py
+-rw-r--r--   0        0        0      427 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/nav/elements.py
+-rw-r--r--   0        0        0     3197 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/nav/nav.py
+-rw-r--r--   0        0        0    70330 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203179 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51796 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115988 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70404 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203183 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51871 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116065 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12066 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129328 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10127 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51370 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12059 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129343 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10199 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63944 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107824 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267492 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85353 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180382 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107692 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267433 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85282 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180218 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   280814 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.css
+-rw-r--r--   0        0        0   679012 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232949 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589162 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280393 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   678857 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   233056 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   588696 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0    88585 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    47188 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.json
+-rw-r--r--   0        0        0   211136 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   972584 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.svg
+-rw-r--r--   0        0        0   207731 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444287 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80664 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331887 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135747 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305153 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74155 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222463 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145313 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.js
+-rw-r--r--   0        0        0   306321 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60578 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220351 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0      299 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/table/__init__.py
+-rw-r--r--   0        0        0     5096 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/table/base.py
+-rw-r--r--   0        0        0     2353 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/table/columns.py
+-rw-r--r--   0        0        0       67 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/testing/__init__.py
+-rw-r--r--   0        0        0     4939 2024-05-14 00:58:10.000000 bootlace-0.2.0/src/bootlace/testing/html.py
+-rw-r--r--   0        0        0     1222 2024-05-14 00:58:10.000000 bootlace-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1096 2024-05-14 00:58:10.000000 bootlace-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      478 2024-05-14 00:58:10.000000 bootlace-0.2.0/README.md
+-rw-r--r--   0        0        0     2613 2024-05-14 00:58:10.000000 bootlace-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1323 2024-05-14 00:58:10.000000 bootlace-0.2.0/PKG-INFO
```

### Comparing `bootlace-0.1.4/src/bootlace/breadcrumbs.py` & `bootlace-0.2.0/src/bootlace/breadcrumbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from flask import Flask
 from flask import request
 from flask import url_for
 from werkzeug.local import LocalProxy
 
 from .util import as_tag
 from .util import is_active_endpoint
+from .util import Tag
 
 __all__ = ["breadcrumbs", "Breadcrumb", "Breadcrumbs", "BreadcrumbEntry", "BreadcrumbExtension", "Endpoint"]
 
 
 class Named(Protocol):
 
     __name__: str
@@ -36,14 +37,18 @@
 def endpoint_name(instance: object, attribute: attrs.Attribute, value: str) -> None:
     if "." in value:
         raise ValueError("Endpoint names cannot contain dots")
 
 
 @attrs.define(frozen=True, init=False)
 class KeywordArguments(Mapping[str, Any]):
+    """
+    A mapping of keyword arguments for a URL endpoint,
+    which is frozen and hashable for use as a key in a dictionary.
+    """
 
     _arguments: frozenset[tuple[str, Any]]
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         arguments = frozenset(dict(*args, **kwargs).items())
         object.__setattr__(self, "_arguments", arguments)
 
@@ -116,43 +121,49 @@
 
     #: The title of the breadcrumb, displayed in text
     title: str
 
     #: The endpoint for the breadcrumb
     link: Endpoint
 
+    a: Tag = Tag(tags.a)
+
     @property
     def active(self) -> bool:
         """Whether the breadcrumb is the active view"""
         return self.link.active
 
     @property
     def url(self) -> str:
         """The URL for the breadcrumb"""
         return self.link.url
 
     def __tag__(self) -> dom_tag:
         if self.active:
             return text(self.title)
 
-        return tags.a(self.title, href=self.url)
+        return self.a(self.title, href=self.url)
 
 
 @attrs.define
 class Breadcrumbs:
     """The trail of breadcrumbs
 
     Supports the :func:`as_tag` protocol to render the breadcrumbs as HTML"""
 
     #: The list of breadcrumbs, in order from broadest to most specific
     crumbs: list[Breadcrumb] = attrs.field(factory=list)
 
     #: The divider to use between breadcrumbs
     divider: str = attrs.field(default=">")
 
+    nav: Tag = Tag(tags.nav)
+    ol: Tag = Tag(tags.ol, classes={"breadcrumb"})
+    li: Tag = Tag(tags.li, classes={"breadcrumb-item"})
+
     def __iter__(self) -> Iterator[Breadcrumb]:
         return iter(self.crumbs)
 
     def __len__(self) -> int:
         return len(self.crumbs)
 
     def __getitem__(self, index: int) -> Breadcrumb:
@@ -162,23 +173,25 @@
         """Add a new crumb to the beginning of the list"""
         self.crumbs.insert(0, crumb)
 
     def __tag__(self) -> dom_tag:
         if not self.crumbs:
             return text("")
 
-        nav = tags.nav(aria_label="breadcrumb")
+        nav = self.nav()
+        nav.aria["label"] = "breadcrumb"
+
         if self.divider != "/":
             nav["style"] = f"--breadcrumb-divider: '{self.divider:s}';"  # noqa: B907
 
-        ol = tags.ol(cls="breadcrumb")
+        ol = self.ol()
         for crumb in self:
-            item = tags.li(as_tag(crumb), cls="breadcrumb-item")
+            item = self.li(as_tag(crumb))
             if crumb.active:
-                item["aria-current"] = "page"
+                item.aria["current"] = "page"
                 item.classes.add("active")
             ol.add(item)
         nav.add(ol)
         return nav
 
 
 @attrs.define
```

### Comparing `bootlace-0.1.4/src/bootlace/extension.py` & `bootlace-0.2.0/src/bootlace/extension.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/icon.py` & `bootlace-0.2.0/src/bootlace/icon.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import ClassVar
 
 import attrs
-from dominate import svg
+from dominate import svg as svg_tag
 from dominate.dom_tag import dom_tag
 from flask import url_for
 
+from bootlace.util import Tag
+
 
 __all__ = ["Icon"]
 
 
 @attrs.define
 class Icon:
     """A Bootstrap icon
@@ -21,28 +23,24 @@
 
     #: Filename for the Bootstrap Icon SVG file
     filename: ClassVar[str] = "icons/bootstrap-icons.svg"
 
     #: Name of the icon
     name: str
 
-    #: Width of the icon
-    width: int = 16
+    svg: Tag = Tag(
+        svg_tag.svg,
+        attributes={"role": "img", "fill": "currentColor", "width": "16", "height": "16"},
+        classes={"bi", "me-1", "pe-none", "align-self-center"},
+    )
 
-    #: Height of the icon
-    height: int = 16
+    use: Tag = Tag(svg_tag.use)
 
     @property
     def url(self) -> str:
         """The URL for the SVG source for the icon"""
         return url_for(self.endpoint, filename=self.filename, _anchor=self.name)
 
     def __tag__(self) -> dom_tag:
-        classes = ["bi", "me-1", "pe-none", "align-self-center"]
-        return svg.svg(
-            svg.use(xlink_href=self.url),
-            cls=" ".join(classes),
-            role="img",
-            width=self.width,
-            height=self.height,
-            fill="currentColor",
+        return self.svg(
+            self.use(xlink_href=self.url),
         )
```

### Comparing `bootlace-0.1.4/src/bootlace/links.py` & `bootlace-0.2.0/src/bootlace/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 import attrs
 from dominate import tags
 from flask import url_for
 
 from .util import as_tag
 from .util import is_active_endpoint
 from .util import MaybeTaggable
+from .util import Tag
 
 __all__ = ["Link", "View"]
 
 
 @attrs.define(kw_only=True, frozen=True)
 class LinkBase(abc.ABC):
     text: MaybeTaggable
 
+    a: Tag = Tag(tags.a)
+
     @property
     @abc.abstractmethod
     def active(self) -> bool:
         raise NotImplementedError("LinkBase.active must be implemented in a subclass")
 
     @property
     @abc.abstractmethod
@@ -28,16 +31,15 @@
 
     @property
     @abc.abstractmethod
     def url(self) -> str:
         raise NotImplementedError("LinkBase.url must be implemented in a subclass")
 
     def __tag__(self) -> tags.html_tag:
-
-        return tags.a(as_tag(self.text), href=self.url)
+        return self.a(as_tag(self.text), href=self.url)
 
 
 @attrs.define(kw_only=True, frozen=True)
 class Link(LinkBase):
     """A raw link to a URL."""
 
     #: The URL to link to
```

### Comparing `bootlace-0.1.4/src/bootlace/size.py` & `bootlace-0.2.0/src/bootlace/size.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/style.py` & `bootlace-0.2.0/src/bootlace/style.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/util.py` & `bootlace-0.2.0/src/bootlace/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import functools
 import itertools
 import warnings
 from collections.abc import Callable
 from collections.abc import Iterable
 from collections.abc import Iterator
 from collections.abc import Mapping
+from collections.abc import MutableMapping
+from collections.abc import MutableSet
 from typing import Any
+from typing import Generic
 from typing import Protocol
 from typing import TypeAlias
 from typing import TypeVar
 
 import attrs
 from dominate import tags
 from dominate.dom_tag import dom_tag
@@ -39,14 +42,17 @@
 class BootlaceWarning(UserWarning):
     """A warning specific to Bootlace"""
 
 
 def _monkey_patch_dominate() -> None:
     """Monkey patch the dominate tags to support class attribute manipulation"""
     tags.html_tag.classes = property(lambda self: Classes(self))  # type: ignore
+    tags.html_tag.data = PrefixAccessor("data")  # type: ignore
+    tags.html_tag.aria = PrefixAccessor("aria")  # type: ignore
+    tags.html_tag.hx = PrefixAccessor("hx")  # type: ignore
 
 
 class Taggable(Protocol):
     """Protocol for objects that can be converted to a tag."""
 
     def __tag__(self) -> dom_tag:
         """Convert the object to a dominate tag.
@@ -121,53 +127,101 @@
     :param item: The item to render. See :func:`as_tag` for more information.
     :returns: A :class:`Markup` object, suitable for inserting into a :mod:`jinja` template.
 
     """
     return Markup(as_tag(item).render())
 
 
-class Classes:
+class Classes(MutableSet[str]):
     """A helper for manipulating the class attribute on a tag."""
 
     def __init__(self, tag: tags.html_tag) -> None:
         self.tag = tag
 
-    def __contains__(self, cls: str) -> bool:
+    def __contains__(self, cls: object) -> bool:
         return cls in self.tag.attributes.get("class", "").split()
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.tag.attributes.get("class", "").split())
 
-    def add(self, *classes: str) -> tags.html_tag:
+    def __len__(self) -> int:
+        return len(self.tag.attributes.get("class", "").split())
+
+    def add(self, *classes: str) -> tags.html_tag:  # type: ignore[override]
         current: list[str] = self.tag.attributes.get("class", "").split()
         for cls in classes:
             if cls not in current:
                 current.append(cls)
         self.tag.attributes["class"] = " ".join(current)
         return self.tag
 
-    def remove(self, *classes: str) -> tags.html_tag:
+    def remove(self, *classes: str) -> tags.html_tag:  # type: ignore[override]
         current: list[str] = self.tag.attributes.get("class", "").split()
         for cls in classes:
             if cls in current:
                 current.remove(cls)
         self.tag.attributes["class"] = " ".join(current)
         return self.tag
 
+    def discard(self, value: str) -> None:
+        self.remove(value)
+
     def swap(self, old: str, new: str) -> tags.html_tag:
         current: list[str] = self.tag.attributes.get("class", "").split()
         if old in current:
             current.remove(old)
         if new not in current:
             current.append(new)
         self.tag.attributes["class"] = " ".join(current)
         return self.tag
 
 
 @attrs.define
+class PrefixAccessor:
+    """A helper for accessing attributes with a prefix."""
+
+    prefix: str = attrs.field()
+
+    def __get__(self, instance: tags.html_tag, owner: type[tags.html_tag]) -> "PrefixAccess":
+        return PrefixAccess(self.prefix, instance)
+
+
+@attrs.define
+class PrefixAccess(MutableMapping[str, str]):
+
+    prefix: str = attrs.field()
+    tag: tags.html_tag = attrs.field()
+
+    def __getitem__(self, name: str) -> str:
+        return self.tag.attributes[f"{self.prefix}-{name}"]
+
+    def __setitem__(self, name: str, value: str) -> None:
+        self.tag.attributes[f"{self.prefix}-{name}"] = value
+
+    def __delitem__(self, name: str) -> None:
+        del self.tag.attributes[f"{self.prefix}-{name}"]
+
+    def __iter__(self) -> Iterator[str]:
+        for key in self.tag.attributes:
+            if key.startswith(f"{self.prefix}-"):
+                yield key[len(self.prefix) + 1 :]
+
+    def __len__(self) -> int:
+        return sum(1 for _ in self)
+
+    def set(self, name: str, value: str) -> tags.html_tag:
+        self[name] = value
+        return self.tag
+
+    def remove(self, name: str) -> tags.html_tag:
+        del self[name]
+        return self.tag
+
+
+@attrs.define
 class HtmlIDScope:
     """A helper for generating unique HTML IDs."""
 
     scopes: collections.defaultdict[str, itertools.count] = attrs.field(
         factory=lambda: collections.defaultdict(itertools.count)
     )
 
@@ -210,7 +264,49 @@
 
     if rule_url is None:  # pragma: no cover
         return False
 
     _, url = rule_url
 
     return url == request.path
+
+
+H = TypeVar("H", bound=tags.html_tag)
+
+
+@attrs.define
+class Tag(Generic[H]):
+    """A helper for creating tags.
+
+    Holds the tag type as well as attributes for the tag. This can be used
+    by calling the instance as a function to create a tag, or by calling the
+    :meth:`update` method to apply the attributes to an existing tag."""
+
+    #: The tag type
+    tag: type[H] = attrs.field()
+
+    #: The classes to apply to the tag
+    classes: set[str] = attrs.field(factory=set)
+
+    #: The attributes to apply to the tag
+    attributes: dict[str, str] = attrs.field(factory=dict)
+
+    def __tag__(self) -> H:
+        tag = self.tag(**self.attributes)
+        tag.classes.add(*self.classes)
+        return tag
+
+    def __call__(self, *args: Any, **kwds: Any) -> H:
+        tag = self.tag(*args, **{**self.attributes, **kwds})
+        tag.classes.add(*self.classes)
+        return tag
+
+    def __setitem__(self, name: str, value: str) -> None:
+        self.attributes[name] = value
+
+    def __getitem__(self, name: str) -> str:
+        return self.attributes[name]
+
+    def update(self, tag: H) -> H:
+        tag.classes.add(*self.classes)
+        tag.attributes.update(self.attributes)
+        return tag
```

### Comparing `bootlace-0.1.4/src/bootlace/forms/fields.py` & `bootlace-0.2.0/src/bootlace/forms/fields.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/forms/widgets.py` & `bootlace-0.2.0/src/bootlace/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/forms/templates/bootlace/_form.html` & `bootlace-0.2.0/src/bootlace/forms/templates/bootlace/_form.html`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/nav/bar.py` & `bootlace-0.2.0/src/bootlace/nav/bar.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .core import NavElement
 from .core import SubGroup
 from .nav import Nav
 from bootlace.size import SizeClass
 from bootlace.style import ColorClass
 from bootlace.util import as_tag
 from bootlace.util import ids as element_id
+from bootlace.util import Tag
 
 
 @attrs.define
 class NavBar(NavElement):
     """A navigation bar, typically at the top of the page
 
     This is usually the primary navigation for a site.
@@ -34,14 +35,17 @@
 
     #: The color of the navbar, if using a bootstrap color class
     color: ColorClass | None = ColorClass.TERTIARY
 
     #: Whether the navbar should be fluid (e.g. full width)
     fluid: bool = True
 
+    nav: Tag = Tag(tags.nav, classes={"navbar"})
+    container: Tag = Tag(tags.div, classes={"container"})
+
     def serialize(self) -> dict[str, Any]:
         data = super().serialize()
         data["items"] = [item.serialize() for item in self.items]
         data["expand"] = self.expand.value if self.expand else None
         data["color"] = self.color.value if self.color else None
         return data
 
@@ -49,23 +53,24 @@
     def deserialize(cls, data: dict[str, Any]) -> NavElement:
         data["items"] = [NavElement.deserialize(item) for item in data["items"]]
         data["expand"] = SizeClass(data["expand"]) if data["expand"] else None
         data["color"] = ColorClass(data["color"]) if data["color"] else None
         return cls(**data)
 
     def __tag__(self) -> tags.html_tag:
-        nav = tags.nav(cls="navbar")
+        nav = self.nav()
         if self.expand:
             nav.classes.add(self.expand.add_to_class("navbar-expand"))
         if self.color:
             nav.classes.add(self.color.add_to_class("bg-body"))
 
-        container = tags.div()
+        container = self.container()
         if self.fluid:
             container.classes.add("container-fluid")
+            container.classes.remove("container")
         else:
             container.classes.add("container")
 
         nav.add(container)
 
         for item in self.items:
             container.add(as_tag(item))
@@ -93,62 +98,67 @@
 
 @attrs.define
 class NavBarCollapse(SubGroup):
     """A collection of nav elements that can be collapsed"""
 
     id: str = attrs.field(factory=element_id.factory("navbar-collapse"))
 
+    button: Tag = Tag(tags.button, classes={"navbar-toggler"}, attributes={"type": "button"})
+    icon: Tag = Tag(tags.span, classes={"navbar-toggler-icon"})
+    container: Tag = Tag(tags.div, classes={"collapse", "navbar-collapse"})
+
     def __tag__(self) -> dom_tag:
-        button = tags.button(
-            type="button",
-            cls="navbar-toggler",
-            data_bs_toggle="collapse",
-            data_bs_target=f"#{self.id}",
-            aria_controls=f"{self.id}",
-            aria_expanded="false",
-            aria_label="Toggle navigation",
-        )
-        button.add(tags.span(cls="navbar-toggler-icon"))
-        div = tags.div(cls="collapse navbar-collapse", id=self.id)
+        button = self.button()
+        button.data["bs-toggle"] = "collapse"
+        button.data["bs-target"] = f"#{self.id}"
+        button.aria["controls"] = f"{self.id}"
+        button.aria["expanded"] = "false"
+        button.aria["label"] = "Toggle navigation"
+
+        button.add(self.icon())
+        div = self.container(id=self.id)
         for item in self.items:
             div.add(as_tag(item))
         return container(button, div)
 
 
 @attrs.define
 class NavBarNav(Nav):
     """Primary grouping of nav elements in the navbar"""
 
     id: str = attrs.field(factory=element_id.factory("navbar-nav"))
 
+    ul: Tag = Tag(tags.ul, classes={"navbar-nav"})
+    li: Tag = Tag(tags.li, classes={"nav-item"})
+
     def __tag__(self) -> tags.html_tag:
-        ul = tags.ul(cls="navbar-nav", id=self.id)
+        ul = self.ul(id=self.id)
         for item in self.items:
-            ul.add(tags.li(as_tag(item), cls="nav-item", __pretty=False))
+            ul.add(self.li(as_tag(item), __pretty=False))
         return ul
 
 
 @attrs.define
 class NavBarSearch(NavElement):
     """A search bar for the navbar"""
 
     id: str = attrs.field(factory=element_id.factory("navbar-search"))
 
     placeholder: str = "Search"
     action: str = "#"
     method: str = "GET"
     button: str | None = None
 
+    form: Tag = Tag(tags.form, classes={"d-flex"}, attributes={"role": "search"})
+    input: Tag = Tag(tags.input_, classes={"form-control", "me-2"}, attributes={"type": "search"})
+    button_tag: Tag = Tag(tags.button, classes={"btn", "btn-success"}, attributes={"type": "submit"})
+
     def __tag__(self) -> dom_tag:
-        form = tags.form(id=self.id)
-        form.classes.add("d-flex")
-        form["role"] = "search"
-
-        input = tags.input_(
-            type="search",
-            cls="form-control me-2",
+        form = self.form(id=self.id)
+
+        input = self.input(
             placeholder=self.placeholder,
-            aria_label=self.placeholder,
         )
+        input.aria["label"] = self.placeholder
         form.add(input)
-        form.add(tags.button(self.button or self.placeholder, cls="btn btn-success", type="submit"))
+        form.add(self.button_tag(self.button or self.placeholder))
         return self.element_state(form)
```

### Comparing `bootlace-0.1.4/src/bootlace/nav/core.py` & `bootlace-0.2.0/src/bootlace/nav/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dominate.dom_tag import dom_tag
 
 from bootlace import links
 from bootlace.image import Image
 from bootlace.util import as_tag
 from bootlace.util import BootlaceWarning
 from bootlace.util import ids as element_id
+from bootlace.util import Tag
 
 
 class NavStyle(enum.Enum):
     """Styles for the nav element"""
 
     PLAIN = ""
     TABS = "nav-tabs"
@@ -27,35 +28,44 @@
     """Alignment for the nav element"""
 
     DEFAULT = ""
     FILL = "nav-fill"
     JUSTIFIED = "nav-justified"
 
 
+def nav_serialize_filter(field: attrs.Attribute, value: Any) -> Any:
+    """Serialize the value of a NavElement"""
+    if isinstance(value, Tag):
+        return False
+
+    return True
+
+
 class NavElement:
     """Base class for nav components"""
 
     _NAV_ELEMENT_REGISTRY: dict[str, type["NavElement"]] = {}
 
     def __init_subclass__(cls) -> None:
         cls._NAV_ELEMENT_REGISTRY[cls.__name__] = cls
 
     def serialize(self) -> dict[str, Any]:
         """Serialize the element to a dictionary"""
-        data = attrs.asdict(self)  # type: ignore
+        data = attrs.asdict(self, filter=nav_serialize_filter)  # type: ignore
         data["__type__"] = self.__class__.__name__
         return data
 
     @classmethod
     def deserialize(cls, data: dict[str, Any]) -> "NavElement":
         """Deserialize an element from a dictionary"""
         if cls is NavElement:
             element_cls = cls._NAV_ELEMENT_REGISTRY.get(data["__type__"], NavElement)
             del data["__type__"]
             return element_cls.deserialize(data)
+
         return cls(**data)
 
     @property
     def active(self) -> bool:
         """Whether the element is active"""
         return False
 
@@ -71,35 +81,37 @@
     def element_state(self, tag: dom_tag) -> dom_tag:
         """Apply :attr:`active` and :attr:`enabled` states to the tag."""
         if not isinstance(tag, tags.html_tag):
             return tag
 
         if self.active:
             tag.classes.add("active")
-            tag.attributes["aria-current"] = "page"
+            tag.aria["current"] = "page"
 
         if not self.enabled:
             tag.classes.add("disabled")
-            tag["aria-disabled"] = "true"
+            tag.aria["disabled"] = "true"
         return tag
 
 
 @attrs.define
 class Link(NavElement):
     """A link in the nav bar, either for a view or a literal URL"""
 
     #: The link to display, either a URL or a view
     link: links.LinkBase
 
     #: The ID of the element
     id: str = attrs.field(factory=element_id.factory("nav-link"))
 
+    a: Tag = Tag(tags.a, classes={"nav-link"})
+
     def serialize(self) -> dict[str, Any]:
         data = super().serialize()
-        data["link"] = attrs.asdict(self.link)
+        data["link"] = attrs.asdict(self.link, filter=nav_serialize_filter)
         data["link"]["__type__"] = self.link.__class__.__name__
         return data
 
     @classmethod
     def deserialize(cls, data: dict[str, Any]) -> Self:
         link_cls = getattr(links, data["link"].pop("__type__"))
         data["link"] = link_cls(**data["link"])
@@ -130,39 +142,43 @@
         """The URL for the link."""
         return self.link.url
 
     def __tag__(self) -> dom_tag:
         a = as_tag(self.link)
         if isinstance(a, tags.html_tag):
             a["id"] = self.id
-            a.classes.add("nav-link")
+            self.a.update(a)
 
         return self.element_state(a)
 
 
 @attrs.define
 class Separator(NavElement):
     """A separator in dropdown menus"""
 
+    hr: Tag = Tag(tags.hr, classes={"dropdown-divider"})
+
     def __tag__(self) -> tags.html_tag:
-        return tags.hr(cls="dropdown-divider")
+        return self.hr()
 
 
 @attrs.define
 class Text(NavElement):
     """A text element in the nav bar"""
 
     text: str
 
+    span: Tag = Tag(tags.span, classes={"nav-link"})
+
     @property
     def enabled(self) -> bool:
         return False
 
     def __tag__(self) -> dom_tag:
-        tag = tags.span(self.text, cls="nav-link")
+        tag = self.span(self.text, cls="nav-link")
         return self.element_state(tag)
 
 
 @attrs.define
 class SubGroup(NavElement):
     """Any grouping of items in the nav bar"""
```

### Comparing `bootlace-0.1.4/src/bootlace/nav/nav.py` & `bootlace-0.2.0/src/bootlace/nav/nav.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .core import NavAlignment
 from .core import NavStyle
 from .core import SubGroup
 from bootlace.util import as_tag
 from bootlace.util import BootlaceWarning
 from bootlace.util import ids as element_id
+from bootlace.util import Tag
 
 
 @attrs.define
 class Nav(SubGroup):
     """A navigation bar"""
 
     #: The ID of the nav
@@ -22,75 +23,83 @@
 
     #: The style of the nav
     style: NavStyle = NavStyle.PLAIN
 
     #: The alignment of the elments in the nav
     alignment: NavAlignment = NavAlignment.DEFAULT
 
+    ul: Tag = Tag(tags.ul, classes={"nav"})
+    li: Tag = Tag(tags.li, classes={"nav-item"})
+
     def serialize(self) -> dict[str, Any]:
         data = super().serialize()
         data["style"] = self.style.name
         data["alignment"] = self.alignment.name
         return data
 
     @classmethod
     def deserialize(cls, data: dict[str, Any]) -> Self:
         data["style"] = NavStyle[data["style"]]
         data["alignment"] = NavAlignment[data["alignment"]]
         return super().deserialize(data)
 
     def __tag__(self) -> tags.html_tag:
         active_endpoint = next((item for item in self.items if item.active), None)
-        ul = tags.ul(cls="nav", id=self.id)
+        ul = self.ul(id=self.id)
 
         if (style := self.style.value) != "":
             ul.classes.add(style)
 
         if (alignment := self.alignment.value) != "":
             ul.classes.add(alignment)
 
         if (link := getattr(active_endpoint, "link", None)) is not None:
             if (endpoint := getattr(link, "endpoint", None)) is not None:
                 ul["data-endpoint"] = endpoint
 
         for item in self.items:
-            ul.add(tags.li(as_tag(item), cls="nav-item", __pretty=False))
+            ul.add(self.li(as_tag(item), __pretty=False))
 
         return ul
 
 
 @attrs.define
 class Dropdown(SubGroup):
     """A dropdown menu in the nav bar"""
 
     #: The title of the dropdown
     title: str = attrs.field(kw_only=True)
 
     #: The ID of the dropdown
     id: str = attrs.field(factory=element_id.factory("bs-dropdown"))
 
+    dropdown: Tag = Tag(tags.div, classes={"dropdown"})
+    ul: Tag = Tag(tags.ul, classes={"dropdown-menu"})
+    li: Tag = Tag(tags.li)
+    toggle: Tag = Tag(tags.a, classes={"nav-link", "dropdown-toggle"}, attributes={"role": "button"})
+
     def __tag__(self) -> tags.html_tag:
-        div = tags.div(cls="dropdown")
-        a = tags.a(
+        div = self.dropdown()
+        a = self.toggle(
             self.title,
             href="#",
-            cls="nav-link dropdown-toggle",
-            role="button",
             id=self.id,
-            aria_expanded="false",
-            data_bs_toggle="dropdown",
         )
+        a.aria["expanded"] = "false"
+        a.data["bs-toggle"] = "dropdown"
         div.add(a)
-        menu = tags.ul(cls="dropdown-menu", aria_labelledby=self.id)
+
+        menu = self.ul()
+        menu.aria["labelledby"] = self.id
         for item in self.items:
             tag = as_tag(item)
             if isinstance(tag, tags.html_tag):
                 tag.classes.remove("nav-link")
                 if not any(cls.startswith("dropdown-") for cls in tag.classes):
                     tag.classes.add("dropdown-item")
             else:
                 warnings.warn(
                     BootlaceWarning(f"Item {item!r} is not an html tag, may not display properly"), stacklevel=2
                 )
-            menu.add(tags.li(tag, __pretty=False))
+            menu.add(self.li(tag, __pretty=False))
         div.add(menu)
         return div
```

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/css/bootstrap.rtl.min.css.map` & `bootlace-0.2.0/src/bootlace/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.css` & `bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.json` & `bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.scss` & `bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/icons/bootstrap-icons.svg` & `bootlace-0.2.0/src/bootlace/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.js.map` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.bundle.min.js.map` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.js.map` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.esm.min.js.map` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.js` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.js.map` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/static/js/bootstrap.min.js.map` & `bootlace-0.2.0/src/bootlace/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/src/bootlace/table/base.py` & `bootlace-0.2.0/src/bootlace/table/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import attrs
 from dominate import tags
 from dominate.dom_tag import dom_tag
 
 from bootlace.icon import Icon
 from bootlace.util import as_tag
 from bootlace.util import maybe
+from bootlace.util import Tag
 
 
 @attrs.define
 class Heading:
     """A heading for a table column."""
 
     #: The text of the heading
@@ -38,31 +39,40 @@
     """Base class for table columns.
 
     Subclasses must implement the :meth:`cell` method."""
 
     #: The heading for the column
     heading: Heading = attrs.field(converter=maybe(Heading))  # type: ignore
 
-    _attribute: str | None = None
+    name: str | None = None
+
+    th = Tag(tags.th)
+    td = Tag(tags.td)
 
     def __set_name__(self, owner: type, name: str) -> None:
-        self._attribute = self._attribute or name
+        self.name = self.name or name
 
     @property
     def attribute(self) -> str:
         """The attribute name for the column."""
-        if self._attribute is None:
+        if self.name is None:
             raise ValueError("column must be named in Table or attribute= parameter must be provided")
-        return self._attribute
+        return self.name
 
     @abstractmethod
     def cell(self, value: Any) -> dom_tag:
         """Return the cell for the column as an HTML tag."""
         raise NotImplementedError("Subclasses must implement this method")
 
+    def __th__(self) -> dom_tag:
+        return self.th(as_tag(self.heading), scope="col", __pretty=False)
+
+    def __td__(self, value: Any) -> dom_tag:
+        return self.td(self.cell(value), __pretty=False)
+
 
 def is_instance_or_subclass(val: Any, class_: type) -> bool:
     """Return True if ``val`` is either a subclass or instance of ``class_``."""
     try:
         return issubclass(val, class_)
     except TypeError:
         return isinstance(val, class_)
@@ -114,35 +124,49 @@
         name = Column(Heading("Name"))
         age = Column(Heading("Age"))
 
     Use :meth:`render` to render a table from a list of items as
     :class:`dominate.tags.table`.
     """
 
-    decorated_classes: set[str] = set()
     columns: ClassVar[dict[str, ColumnBase]]
 
+    table = Tag(tags.table)
+    thead = Tag(tags.thead)
+    tbody = Tag(tags.tbody)
+    tr = Tag(tags.tr)
+
     def __init__(self, decorated_classes: Iterable[str] | None = None) -> None:
         if decorated_classes is None:
             self.decorated_classes = set()
         else:
             self.decorated_classes = set(decorated_classes)
 
-    def __call__(self, items: list[Any]) -> tags.html_tag:
-        table = tags.table(cls="table")
+    def __table__(self, items: list[Any]) -> tags.html_tag:
+        table = self.table(cls="table")
         table.classes.add(*self.decorated_classes)
-        thead = tags.thead()
-        tbody = tags.tbody()
+        table.add(self.__thead__())
+        table.add(self.__tbody__(items))
+        return table
 
-        for _, column in self.columns.items():
-            thead.add(tags.th(as_tag(column.heading), scope="col", __pretty=False))
-        table.add(thead)
+    def __thead__(self) -> tags.html_tag:
+        thead = self.thead()
+        for column in self.columns.values():
+            thead.add(column.__th__())
+        return thead
+
+    def __tr__(self, item: Any) -> tags.html_tag:
+        id = getattr(item, "id", None)
+        name = item.__class__.__name__.lower()
+        tr = self.tr(id=f"{name}-{id}" if id else None)
+        for column in self.columns.values():
+            tr.add(column.__td__(item))
+        return tr
 
+    def __tbody__(self, items: list[Any]) -> tags.html_tag:
+        tbody = self.tbody()
         for item in items:
-            id = getattr(item, "id", None)
-            tr = tags.tr(id=f"item-{id}" if id else None)
-            for column in self.columns.values():
-                cell = column.cell(item)
-                tr.add(tags.td(cell))
-            tbody.add(tr)
-        table.add(tbody)
-        return table
+            tbody.add(self.__tr__(item))
+        return tbody
+
+    def __call__(self, items: list[Any]) -> tags.html_tag:
+        return self.__table__(items)
```

### Comparing `bootlace-0.1.4/src/bootlace/table/columns.py` & `bootlace-0.2.0/src/bootlace/table/columns.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from dominate.dom_tag import dom_tag
 from dominate.util import text
 from flask import url_for
 
 from bootlace.icon import Icon
 from bootlace.table.base import ColumnBase
 from bootlace.util import as_tag
+from bootlace.util import Tag
 
 
 __all__ = ["Column", "EditColumn", "CheckColumn", "Datetime"]
 
 
 @attrs.define
 class Column(ColumnBase):
@@ -30,29 +31,31 @@
     """A column which links to an edit view for the value.
 
     This is commonly shown as e.g. the name of the item, which links to the edit view."""
 
     #: The endpoint for the edit view
     endpoint: str = attrs.field(default=".edit")
 
+    a: Tag = Tag(tags.a)
+
     def cell(self, value: Any) -> tags.html_tag:
         """Return the cell for the column as an HTML tag."""
         id = getattr(value, "id", None)
-        return tags.a(getattr(value, self.attribute), href=url_for(self.endpoint, id=id))
+        return self.a(getattr(value, self.attribute), href=url_for(self.endpoint, id=id))
 
 
 @attrs.define
 class CheckColumn(ColumnBase):
     """A column which shows a checkmark or X based on the value of the attribute."""
 
     #: The icon for a true value
-    yes: Icon = attrs.field(default=Icon("check", width=16, height=16))
+    yes: Icon = attrs.field(default=Icon("check"))
 
     #: The icon for a false value
-    no: Icon = attrs.field(default=Icon("x", width=16, height=16))
+    no: Icon = attrs.field(default=Icon("x"))
 
     def cell(self, value: Any) -> dom_tag:
         """Return the cell for the column as an HTML tag."""
         if getattr(value, self.attribute):
             return as_tag(self.yes)
         return as_tag(self.no)
```

### Comparing `bootlace-0.1.4/src/bootlace/testing/html.py` & `bootlace-0.2.0/src/bootlace/testing/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,10 +135,11 @@
                     differences.append(Difference(None, actual.attrib.get(attr), f"Attribute {attr} not expected"))
                     continue
 
         return differences
 
 
 def assert_same_html(expected_html: str, actual_html: str) -> None:
+    __tracebackhide__ = True
     diff = HTMLDiff(attributes=ATTRIBUTES)
     result = diff.compare(expected_html, actual_html)
     assert not result, str(result)
```

### Comparing `bootlace-0.1.4/.gitignore` & `bootlace-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/LICENSE.txt` & `bootlace-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/pyproject.toml` & `bootlace-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.4/PKG-INFO` & `bootlace-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bootlace
-Version: 0.1.4
+Version: 0.2.0
 Summary: Pythonic Bootstrap Utilities
 Project-URL: Documentation, https://github.com/alexrudy/bootlace#readme
 Project-URL: Issues, https://github.com/alexrudy/bootlace/issues
 Project-URL: Source, https://github.com/alexrudy/bootlace
 Author-email: Alex Rudy <github@alexrudy.net>
 License-Expression: MIT
 License-File: LICENSE.txt
```

