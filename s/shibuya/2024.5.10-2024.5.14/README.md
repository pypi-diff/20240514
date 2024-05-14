# Comparing `tmp/shibuya-2024.5.10.tar.gz` & `tmp/shibuya-2024.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shibuya-2024.5.10.tar", last modified: Fri May 10 06:14:22 2024, max compression
+gzip compressed data, was "shibuya-2024.5.14.tar", last modified: Tue May 14 12:21:34 2024, max compression
```

## Comparing `shibuya-2024.5.10.tar` & `shibuya-2024.5.14.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.358519 shibuya-2024.5.10/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-10 06:14:13.000000 shibuya-2024.5.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-10 06:14:13.000000 shibuya-2024.5.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-10 06:14:22.358519 shibuya-2024.5.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 06:14:13.000000 shibuya-2024.5.10/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-10 06:14:13.000000 shibuya-2024.5.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:14:22.358519 shibuya-2024.5.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 06:14:13.000000 shibuya-2024.5.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.350519 shibuya-2024.5.10/src/shibuya/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.346519 shibuya-2024.5.10/src/shibuya/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.354519 shibuya-2024.5.10/src/shibuya/theme/shibuya/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.354519 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/alternate-links.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/discussion-link.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/foot-copyright.html
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/foot-socials.html
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/meta-opengraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/nav-languages.html
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/nav-links.html
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/nav-socials.html
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/nav-versions.html
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/site-foot.html
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/site-head.html
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/components/theme-switch.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.354519 shibuya-2024.5.10/src/shibuya/theme/shibuya/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/extensions/buysellads.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.354519 shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/compact.html
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/default.html
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/landing.html
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/simple.html
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.358519 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/banner.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/extra-head.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/globaltoc-above.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/page-bottom.html
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/partials/webfonts.html
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/relations.html
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.358519 shibuya-2024.5.10/src/shibuya/theme/shibuya/sidebars/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/sidebars/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/sidebars/repo-stats.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.358519 shibuya-2024.5.10/src/shibuya/theme/shibuya/static/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/static/print.css
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)   229176 2024-05-10 06:14:18.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/static/shibuya.css
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-10 06:14:16.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/static/shibuya.js
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-10 06:14:13.000000 shibuya-2024.5.10/src/shibuya/theme/shibuya/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:14:22.358519 shibuya-2024.5.10/src/shibuya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-10 06:14:22.000000 shibuya-2024.5.10/src/shibuya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-10 06:14:22.000000 shibuya-2024.5.10/src/shibuya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:14:22.000000 shibuya-2024.5.10/src/shibuya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 06:14:22.000000 shibuya-2024.5.10/src/shibuya.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 06:14:22.000000 shibuya-2024.5.10/src/shibuya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 06:14:22.000000 shibuya-2024.5.10/src/shibuya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.771084 shibuya-2024.5.14/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-14 12:21:23.000000 shibuya-2024.5.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 12:21:23.000000 shibuya-2024.5.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 12:21:34.771084 shibuya-2024.5.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-14 12:21:23.000000 shibuya-2024.5.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-14 12:21:23.000000 shibuya-2024.5.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:21:34.771084 shibuya-2024.5.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 12:21:23.000000 shibuya-2024.5.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.759084 shibuya-2024.5.14/src/shibuya/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.763084 shibuya-2024.5.14/src/shibuya/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.755084 shibuya-2024.5.14/src/shibuya/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.763084 shibuya-2024.5.14/src/shibuya/theme/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/alternate-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/discussion-link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/foot-copyright.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/foot-socials.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/meta-opengraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-languages.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-socials.html
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/site-foot.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/site-head.html
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/components/theme-switch.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/extensions/buysellads.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/compact.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/default.html
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/landing.html
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/extra-head.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/globaltoc-above.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/page-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/partials/webfonts.html
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/relations.html
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/carbon-ads.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/repo-stats.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.767084 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/print.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)   229960 2024-05-14 12:21:31.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-14 12:21:29.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.js
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-14 12:21:23.000000 shibuya-2024.5.14/src/shibuya/theme/shibuya/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:21:34.771084 shibuya-2024.5.14/src/shibuya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 12:21:34.000000 shibuya-2024.5.14/src/shibuya.egg-info/top_level.txt
```

### Comparing `shibuya-2024.5.10/LICENSE` & `shibuya-2024.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/PKG-INFO` & `shibuya-2024.5.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2024.5.10
+Version: 2024.5.14
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2024.5.10/README.md` & `shibuya-2024.5.14/README.md`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/pyproject.toml` & `shibuya-2024.5.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/__init__.py` & `shibuya-2024.5.14/src/shibuya/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     create_edit_source_link,
 )
 from ._sphinx import (
     WrapperPostTransform,
     WrapLineFormatter,
 )
 
-__version__ = "2024.5.10"
+__version__ = "2024.5.14"
 
 shibuya_version = __version__
 
 ROOT_PATH = Path(__file__).parent
 THEME_PATH = (ROOT_PATH / "theme" / "shibuya").resolve()
```

### Comparing `shibuya-2024.5.10/src/shibuya/_sphinx.py` & `shibuya-2024.5.14/src/shibuya/_sphinx.py`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/context.py` & `shibuya-2024.5.14/src/shibuya/context.py`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/ja/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/ko/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/zh/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo` & `shibuya-2024.5.14/src/shibuya/locale/zh_TW/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/base.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/base.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/breadcrumbs.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/discussion-link.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/discussion-link.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/foot-socials.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/foot-socials.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/meta-opengraph.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/meta-opengraph.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/nav-links.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-links.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/nav-socials.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-socials.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/nav-versions.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/nav-versions.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/navigation.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/navigation.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/components/site-head.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/components/site-head.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/extensions/buysellads.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/extensions/buysellads.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/compact.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/compact.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/layout/default.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/layout/default.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/layout.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/layout.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/sidebars/repo-stats.html` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/sidebars/repo-stats.html`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/static/print.css` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/print.css`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/static/pygments.css` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/pygments.css`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/static/shibuya.css` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.css`

 * *Files 1% similar despite different names*

```diff
@@ -11975,2350 +11975,2399 @@
 0002ec60: 6469 6e67 293b 666f 6e74 2d77 6569 6768  ding);font-weigh
 0002ec70: 743a 3630 303b 6d61 7267 696e 2d74 6f70  t:600;margin-top
 0002ec80: 3a31 2e35 656d 3b6d 6172 6769 6e2d 626f  :1.5em;margin-bo
 0002ec90: 7474 6f6d 3a2e 3565 6d3b 6c69 6e65 2d68  ttom:.5em;line-h
 0002eca0: 6569 6768 743a 312e 357d 2e79 7565 2068  eight:1.5}.yue h
 0002ecb0: 3420 7374 726f 6e67 7b66 6f6e 742d 7765  4 strong{font-we
 0002ecc0: 6967 6874 3a37 3030 3b63 6f6c 6f72 3a69  ight:700;color:i
-0002ecd0: 6e68 6572 6974 7d2e 7975 6520 696d 677b  nherit}.yue img{
-0002ece0: 6469 7370 6c61 793a 696e 6c69 6e65 3b6d  display:inline;m
-0002ecf0: 6172 6769 6e2d 746f 703a 3265 6d3b 6d61  argin-top:2em;ma
-0002ed00: 7267 696e 2d62 6f74 746f 6d3a 3265 6d7d  rgin-bottom:2em}
-0002ed10: 2e79 7565 2069 6d67 2e72 6f75 6e64 6564  .yue img.rounded
-0002ed20: 7b62 6f72 6465 722d 7261 6469 7573 3a2e  {border-radius:.
-0002ed30: 3572 656d 7d2e 7975 6520 613e 696d 672c  5rem}.yue a>img,
-0002ed40: 2e79 7565 2066 6967 7572 6520 696d 672c  .yue figure img,
-0002ed50: 2e79 7565 2066 6967 7572 653e 2a7b 6d61  .yue figure>*{ma
-0002ed60: 7267 696e 2d74 6f70 3a30 3b6d 6172 6769  rgin-top:0;margi
-0002ed70: 6e2d 626f 7474 6f6d 3a30 7d2e 7975 6520  n-bottom:0}.yue 
-0002ed80: 6669 6763 6170 7469 6f6e 7b63 6f6c 6f72  figcaption{color
-0002ed90: 3a76 6172 282d 2d79 7565 2d63 2d63 6170  :var(--yue-c-cap
-0002eda0: 7469 6f6e 293b 666f 6e74 2d73 697a 653a  tion);font-size:
-0002edb0: 2e38 3735 656d 3b6c 696e 652d 6865 6967  .875em;line-heig
-0002edc0: 6874 3a31 2e34 3238 3537 3134 3b6d 6172  ht:1.4285714;mar
-0002edd0: 6769 6e2d 746f 703a 2e38 3537 3134 3239  gin-top:.8571429
-0002ede0: 656d 7d2e 7975 6520 6669 6763 6170 7469  em}.yue figcapti
-0002edf0: 6f6e 3e70 7b6d 6172 6769 6e2d 746f 703a  on>p{margin-top:
-0002ee00: 307d 2e79 7565 2063 6f64 657b 636f 6c6f  0}.yue code{colo
-0002ee10: 723a 7661 7228 2d2d 7975 652d 632d 636f  r:var(--yue-c-co
-0002ee20: 6465 2d74 6578 7429 3b66 6f6e 742d 7765  de-text);font-we
-0002ee30: 6967 6874 3a36 3030 3b66 6f6e 742d 7369  ight:600;font-si
-0002ee40: 7a65 3a2e 3837 3565 6d7d 2e79 7565 2061  ze:.875em}.yue a
-0002ee50: 2063 6f64 652c 2e79 7565 2062 6c6f 636b   code,.yue block
-0002ee60: 7175 6f74 6520 636f 6465 2c2e 7975 6520  quote code,.yue 
-0002ee70: 6831 2063 6f64 652c 2e79 7565 2068 3220  h1 code,.yue h2 
-0002ee80: 636f 6465 2c2e 7975 6520 6833 2063 6f64  code,.yue h3 cod
-0002ee90: 652c 2e79 7565 2068 3420 636f 6465 2c2e  e,.yue h4 code,.
-0002eea0: 7975 6520 7468 2063 6f64 657b 636f 6c6f  yue th code{colo
-0002eeb0: 723a 696e 6865 7269 747d 2e79 7565 2068  r:inherit}.yue h
-0002eec0: 3220 636f 6465 7b66 6f6e 742d 7369 7a65  2 code{font-size
-0002eed0: 3a2e 3837 3565 6d7d 2e79 7565 206c 693e  :.875em}.yue li>
-0002eee0: 636f 6465 2c2e 7975 6520 703e 636f 6465  code,.yue p>code
-0002eef0: 7b70 6164 6469 6e67 3a32 7078 2034 7078  {padding:2px 4px
-0002ef00: 3b62 6f72 6465 722d 7261 6469 7573 3a33  ;border-radius:3
-0002ef10: 7078 3b66 6f6e 742d 7765 6967 6874 3a35  px;font-weight:5
-0002ef20: 3030 3b62 6163 6b67 726f 756e 642d 636f  00;background-co
-0002ef30: 6c6f 723a 7661 7228 2d2d 7975 652d 632d  lor:var(--yue-c-
-0002ef40: 636f 6465 2d62 6163 6b67 726f 756e 6429  code-background)
-0002ef50: 7d2e 7975 6520 6833 2063 6f64 657b 666f  }.yue h3 code{fo
-0002ef60: 6e74 2d73 697a 653a 2e39 656d 7d2e 7975  nt-size:.9em}.yu
-0002ef70: 6520 6b62 647b 666f 6e74 2d66 616d 696c  e kbd{font-famil
-0002ef80: 793a 7661 7228 2d2d 7379 2d66 2d6d 6f6e  y:var(--sy-f-mon
-0002ef90: 6f29 7d2e 7975 6520 6669 6775 7265 2c2e  o)}.yue figure,.
-0002efa0: 7975 6520 7669 6465 6f7b 6d61 7267 696e  yue video{margin
-0002efb0: 2d74 6f70 3a32 656d 3b6d 6172 6769 6e2d  -top:2em;margin-
-0002efc0: 626f 7474 6f6d 3a32 656d 7d2e 7975 6520  bottom:2em}.yue 
-0002efd0: 6c69 7b6d 6172 6769 6e2d 746f 703a 2e35  li{margin-top:.5
-0002efe0: 656d 3b6d 6172 6769 6e2d 626f 7474 6f6d  em;margin-bottom
-0002eff0: 3a2e 3565 6d7d 2e79 7565 206f 6c3e 6c69  :.5em}.yue ol>li
-0002f000: 2c2e 7975 6520 756c 3e6c 697b 7061 6464  ,.yue ul>li{padd
-0002f010: 696e 672d 6c65 6674 3a2e 3337 3565 6d7d  ing-left:.375em}
-0002f020: 2e79 7565 206f 6c20 6f6c 2c2e 7975 6520  .yue ol ol,.yue 
-0002f030: 6f6c 2075 6c2c 2e79 7565 2075 6c20 6f6c  ol ul,.yue ul ol
-0002f040: 2c2e 7975 6520 756c 2075 6c7b 6d61 7267  ,.yue ul ul{marg
-0002f050: 696e 2d74 6f70 3a2e 3735 656d 3b6d 6172  in-top:.75em;mar
-0002f060: 6769 6e2d 626f 7474 6f6d 3a2e 3735 656d  gin-bottom:.75em
-0002f070: 7d2e 7975 6520 6832 2b2a 2c2e 7975 6520  }.yue h2+*,.yue 
-0002f080: 6833 2b2a 2c2e 7975 6520 6834 2b2a 2c2e  h3+*,.yue h4+*,.
-0002f090: 7975 6520 6872 2b2a 7b6d 6172 6769 6e2d  yue hr+*{margin-
-0002f0a0: 746f 703a 307d 2e79 7565 2074 6162 6c65  top:0}.yue table
-0002f0b0: 7b77 6964 7468 3a31 3030 253b 7461 626c  {width:100%;tabl
-0002f0c0: 652d 6c61 796f 7574 3a61 7574 6f3b 7465  e-layout:auto;te
-0002f0d0: 7874 2d61 6c69 676e 3a6c 6566 743b 6d61  xt-align:left;ma
-0002f0e0: 7267 696e 2d74 6f70 3a32 656d 3b6d 6172  rgin-top:2em;mar
-0002f0f0: 6769 6e2d 626f 7474 6f6d 3a32 656d 3b66  gin-bottom:2em;f
-0002f100: 6f6e 742d 7369 7a65 3a2e 3836 656d 3b6c  ont-size:.86em;l
-0002f110: 696e 652d 6865 6967 6874 3a31 2e37 7d2e  ine-height:1.7}.
-0002f120: 7975 6520 7461 626c 653e 6361 7074 696f  yue table>captio
-0002f130: 6e7b 6d61 7267 696e 2d62 6f74 746f 6d3a  n{margin-bottom:
-0002f140: 2e34 7265 6d3b 636f 6c6f 723a 7661 7228  .4rem;color:var(
-0002f150: 2d2d 7975 652d 632d 6361 7074 696f 6e29  --yue-c-caption)
-0002f160: 7d2e 7975 6520 7468 6561 6420 7472 7b62  }.yue thead tr{b
-0002f170: 6f72 6465 722d 626f 7474 6f6d 2d77 6964  order-bottom-wid
-0002f180: 7468 3a31 7078 3b62 6f72 6465 722d 626f  th:1px;border-bo
-0002f190: 7474 6f6d 2d63 6f6c 6f72 3a76 6172 282d  ttom-color:var(-
-0002f1a0: 2d79 7565 2d63 2d74 682d 626f 7264 6572  -yue-c-th-border
-0002f1b0: 297d 2e79 7565 2074 6865 6164 2074 687b  )}.yue thead th{
-0002f1c0: 636f 6c6f 723a 7661 7228 2d2d 7975 652d  color:var(--yue-
-0002f1d0: 632d 6865 6164 696e 6729 3b66 6f6e 742d  c-heading);font-
-0002f1e0: 7765 6967 6874 3a36 3030 3b76 6572 7469  weight:600;verti
-0002f1f0: 6361 6c2d 616c 6967 6e3a 6d69 6464 6c65  cal-align:middle
-0002f200: 7d2e 7975 6520 7462 6f64 7920 7472 7b62  }.yue tbody tr{b
-0002f210: 6f72 6465 722d 626f 7474 6f6d 2d77 6964  order-bottom-wid
-0002f220: 7468 3a31 7078 3b62 6f72 6465 722d 626f  th:1px;border-bo
-0002f230: 7474 6f6d 2d63 6f6c 6f72 3a76 6172 282d  ttom-color:var(-
-0002f240: 2d79 7565 2d63 2d74 642d 626f 7264 6572  -yue-c-td-border
-0002f250: 297d 2e79 7565 2074 626f 6479 2074 723a  )}.yue tbody tr:
-0002f260: 6c61 7374 2d63 6869 6c64 7b62 6f72 6465  last-child{borde
-0002f270: 722d 626f 7474 6f6d 2d77 6964 7468 3a30  r-bottom-width:0
-0002f280: 7d2e 7975 6520 7462 6f64 7920 7464 7b76  }.yue tbody td{v
-0002f290: 6572 7469 6361 6c2d 616c 6967 6e3a 6d69  ertical-align:mi
-0002f2a0: 6464 6c65 7d2e 7975 6520 7466 6f6f 747b  ddle}.yue tfoot{
-0002f2b0: 626f 7264 6572 2d74 6f70 2d77 6964 7468  border-top-width
-0002f2c0: 3a31 7078 3b62 6f72 6465 722d 746f 702d  :1px;border-top-
-0002f2d0: 636f 6c6f 723a 7661 7228 2d2d 7975 652d  color:var(--yue-
-0002f2e0: 632d 7468 2d62 6f72 6465 7229 7d2e 7975  c-th-border)}.yu
-0002f2f0: 6520 7466 6f6f 7420 7464 7b76 6572 7469  e tfoot td{verti
-0002f300: 6361 6c2d 616c 6967 6e3a 746f 707d 2e79  cal-align:top}.y
-0002f310: 7565 2074 643e 707b 6d61 7267 696e 3a2e  ue td>p{margin:.
-0002f320: 3235 7265 6d20 307d 2e79 7565 2074 6865  25rem 0}.yue the
-0002f330: 6164 2074 683e 707b 6d61 7267 696e 3a30  ad th>p{margin:0
-0002f340: 7d2e 7975 6520 7462 6f64 7920 7464 2c2e  }.yue tbody td,.
-0002f350: 7975 6520 7466 6f6f 7420 7464 2c2e 7975  yue tfoot td,.yu
-0002f360: 6520 7468 6561 6420 7468 7b70 6164 6469  e thead th{paddi
-0002f370: 6e67 3a2e 3572 656d 7d2e 7975 6520 7365  ng:.5rem}.yue se
-0002f380: 6374 696f 6e3e 6469 767b 6d61 7267 696e  ction>div{margin
-0002f390: 2d62 6f74 746f 6d3a 3272 656d 7d2e 7975  -bottom:2rem}.yu
-0002f3a0: 6520 6464 3e70 3a66 6972 7374 2d63 6869  e dd>p:first-chi
-0002f3b0: 6c64 7b6d 6172 6769 6e2d 746f 703a 307d  ld{margin-top:0}
-0002f3c0: 2e79 7565 2070 2e6c 6561 647b 666f 6e74  .yue p.lead{font
-0002f3d0: 2d73 697a 653a 312e 3272 656d 3b63 6f6c  -size:1.2rem;col
-0002f3e0: 6f72 3a76 6172 282d 2d73 792d 632d 6c69  or:var(--sy-c-li
-0002f3f0: 6768 7429 3b6d 6172 6769 6e2d 626f 7474  ght);margin-bott
-0002f400: 6f6d 3a30 7d2e 7975 6520 702e 6c65 6164  om:0}.yue p.lead
-0002f410: 2b68 727b 6d61 7267 696e 2d74 6f70 3a31  +hr{margin-top:1
-0002f420: 7265 6d7d 2e79 7565 2070 2e72 7562 7269  rem}.yue p.rubri
-0002f430: 637b 636f 6c6f 723a 7661 7228 2d2d 7975  c{color:var(--yu
-0002f440: 652d 632d 6865 6164 696e 6729 3b66 6f6e  e-c-heading);fon
-0002f450: 742d 7765 6967 6874 3a36 3030 3b66 6f6e  t-weight:600;fon
-0002f460: 742d 7369 7a65 3a31 2e32 3565 6d3b 6d61  t-size:1.25em;ma
-0002f470: 7267 696e 2d74 6f70 3a32 656d 7d2e 7975  rgin-top:2em}.yu
-0002f480: 6520 646c 2e73 696d 706c 653e 6464 3e70  e dl.simple>dd>p
-0002f490: 2c2e 7975 6520 6f6c 2e73 696d 706c 653e  ,.yue ol.simple>
-0002f4a0: 6c69 3e70 2c2e 7975 6520 756c 2e73 696d  li>p,.yue ul.sim
-0002f4b0: 706c 653e 6c69 3e70 7b6d 6172 6769 6e3a  ple>li>p{margin:
-0002f4c0: 307d 2e79 7565 2061 2e68 6561 6465 726c  0}.yue a.headerl
-0002f4d0: 696e 6b7b 7669 7369 6269 6c69 7479 3a68  ink{visibility:h
-0002f4e0: 6964 6465 6e3b 6d61 7267 696e 2d6c 6566  idden;margin-lef
-0002f4f0: 743a 3670 783b 636f 6c6f 723a 7661 7228  t:6px;color:var(
-0002f500: 2d2d 7379 2d63 2d6c 6967 6874 293b 666f  --sy-c-light);fo
-0002f510: 6e74 2d77 6569 6768 743a 3330 303b 666f  nt-weight:300;fo
-0002f520: 6e74 2d73 697a 653a 3538 253b 666f 6e74  nt-size:58%;font
-0002f530: 2d66 616d 696c 793a 7661 7228 2d2d 7379  -family:var(--sy
-0002f540: 2d66 2d6d 6f6e 6f29 3b2d 2d69 636f 6e2d  -f-mono);--icon-
-0002f550: 7572 6c3a 7661 7228 2d2d 6c75 6369 6465  url:var(--lucide
-0002f560: 2d6c 696e 6b2d 7572 6c29 3b2d 7765 626b  -link-url);-webk
-0002f570: 6974 2d6d 6173 6b3a 7661 7228 2d2d 6963  it-mask:var(--ic
-0002f580: 6f6e 2d75 726c 2920 6e6f 2d72 6570 6561  on-url) no-repea
-0002f590: 743b 6d61 736b 3a76 6172 282d 2d69 636f  t;mask:var(--ico
-0002f5a0: 6e2d 7572 6c29 206e 6f2d 7265 7065 6174  n-url) no-repeat
-0002f5b0: 3b2d 7765 626b 6974 2d6d 6173 6b2d 7369  ;-webkit-mask-si
-0002f5c0: 7a65 3a31 3030 2520 3130 3025 3b6d 6173  ze:100% 100%;mas
-0002f5d0: 6b2d 7369 7a65 3a31 3030 2520 3130 3025  k-size:100% 100%
-0002f5e0: 3b77 6964 7468 3a31 656d 3b68 6569 6768  ;width:1em;heigh
-0002f5f0: 743a 3165 6d3b 6469 7370 6c61 793a 696e  t:1em;display:in
-0002f600: 6c69 6e65 2d62 6c6f 636b 3b76 6572 7469  line-block;verti
-0002f610: 6361 6c2d 616c 6967 6e3a 6d69 6464 6c65  cal-align:middle
-0002f620: 3b66 6f6e 742d 7374 796c 653a 6e6f 726d  ;font-style:norm
-0002f630: 616c 3b62 6163 6b67 726f 756e 642d 636f  al;background-co
-0002f640: 6c6f 723a 6375 7272 656e 7443 6f6c 6f72  lor:currentColor
-0002f650: 7d2e 7975 6520 2e6d 6174 6820 612e 6865  }.yue .math a.he
-0002f660: 6164 6572 6c69 6e6b 2c68 313a 686f 7665  aderlink,h1:hove
-0002f670: 7220 612e 6865 6164 6572 6c69 6e6b 2c68  r a.headerlink,h
-0002f680: 323a 686f 7665 7220 612e 6865 6164 6572  2:hover a.header
-0002f690: 6c69 6e6b 2c68 333a 686f 7665 7220 612e  link,h3:hover a.
-0002f6a0: 6865 6164 6572 6c69 6e6b 2c68 343a 686f  headerlink,h4:ho
-0002f6b0: 7665 7220 612e 6865 6164 6572 6c69 6e6b  ver a.headerlink
-0002f6c0: 2c68 353a 686f 7665 7220 612e 6865 6164  ,h5:hover a.head
-0002f6d0: 6572 6c69 6e6b 2c68 363a 686f 7665 7220  erlink,h6:hover 
-0002f6e0: 612e 6865 6164 6572 6c69 6e6b 7b76 6973  a.headerlink{vis
-0002f6f0: 6962 696c 6974 793a 7669 7369 626c 657d  ibility:visible}
-0002f700: 2e79 7565 202e 746f 6374 7265 652d 7772  .yue .toctree-wr
-0002f710: 6170 7065 7220 612c 2e79 7565 2061 2e69  apper a,.yue a.i
-0002f720: 6d61 6765 2d72 6566 6572 656e 6365 7b62  mage-reference{b
-0002f730: 6f72 6465 722d 626f 7474 6f6d 3a6e 6f6e  order-bottom:non
-0002f740: 657d 2e79 7565 202e 746f 6374 7265 652d  e}.yue .toctree-
-0002f750: 7772 6170 7065 7220 702e 6361 7074 696f  wrapper p.captio
-0002f760: 6e7b 666f 6e74 2d73 697a 653a 2e38 3672  n{font-size:.86r
-0002f770: 656d 3b66 6f6e 742d 7765 6967 6874 3a35  em;font-weight:5
-0002f780: 3030 3b66 6f6e 742d 6661 6d69 6c79 3a76  00;font-family:v
-0002f790: 6172 282d 2d73 792d 662d 6865 6164 696e  ar(--sy-f-headin
-0002f7a0: 6729 3b63 6f6c 6f72 3a76 6172 282d 2d73  g);color:var(--s
-0002f7b0: 792d 632d 6c69 6768 7429 3b74 6578 742d  y-c-light);text-
-0002f7c0: 7472 616e 7366 6f72 6d3a 7570 7065 7263  transform:upperc
-0002f7d0: 6173 653b 6c65 7474 6572 2d73 7061 6369  ase;letter-spaci
-0002f7e0: 6e67 3a2e 3470 783b 7061 6464 696e 673a  ng:.4px;padding:
-0002f7f0: 2e38 7265 6d20 3020 2e34 7265 6d3b 626f  .8rem 0 .4rem;bo
-0002f800: 7264 6572 2d62 6f74 746f 6d3a 3170 7820  rder-bottom:1px 
-0002f810: 736f 6c69 6420 7661 7228 2d2d 7379 2d63  solid var(--sy-c
-0002f820: 2d64 6976 6964 6572 297d 2e79 7565 202e  -divider)}.yue .
-0002f830: 616c 6967 6e2d 6365 6e74 6572 7b64 6973  align-center{dis
-0002f840: 706c 6179 3a62 6c6f 636b 3b74 6578 742d  play:block;text-
-0002f850: 616c 6967 6e3a 6365 6e74 6572 7d2e 7975  align:center}.yu
-0002f860: 6520 2e61 6c69 676e 2d63 656e 7465 722c  e .align-center,
-0002f870: 2e79 7565 2066 6967 7572 652e 616c 6967  .yue figure.alig
-0002f880: 6e2d 6365 6e74 6572 2069 6d67 7b6d 6172  n-center img{mar
-0002f890: 6769 6e2d 6c65 6674 3a61 7574 6f3b 6d61  gin-left:auto;ma
-0002f8a0: 7267 696e 2d72 6967 6874 3a61 7574 6f7d  rgin-right:auto}
-0002f8b0: 612e 666f 6f74 6e6f 7465 2d72 6566 6572  a.footnote-refer
-0002f8c0: 656e 6365 7b66 6f6e 742d 7369 7a65 3a2e  ence{font-size:.
-0002f8d0: 3635 7265 6d3b 7665 7274 6963 616c 2d61  65rem;vertical-a
-0002f8e0: 6c69 676e 3a74 6f70 7d61 7369 6465 2e66  lign:top}aside.f
-0002f8f0: 6f6f 746e 6f74 653e 7370 616e 2c64 6976  ootnote>span,div
-0002f900: 2e63 6974 6174 696f 6e3e 7370 616e 7b66  .citation>span{f
-0002f910: 6c6f 6174 3a6c 6566 743b 666f 6e74 2d77  loat:left;font-w
-0002f920: 6569 6768 743a 3530 303b 7061 6464 696e  eight:500;paddin
-0002f930: 672d 7269 6768 743a 2e32 3572 656d 7d61  g-right:.25rem}a
-0002f940: 7369 6465 2e66 6f6f 746e 6f74 653e 702c  side.footnote>p,
-0002f950: 6469 762e 6369 7461 7469 6f6e 3e70 7b6d  div.citation>p{m
-0002f960: 6172 6769 6e2d 626f 7474 6f6d 3a2e 3572  argin-bottom:.5r
-0002f970: 656d 3b6d 6172 6769 6e2d 746f 703a 2e35  em;margin-top:.5
-0002f980: 7265 6d3b 6d61 7267 696e 2d6c 6566 743a  rem;margin-left:
-0002f990: 3272 656d 7d2e 7975 6520 6b62 642e 6b62  2rem}.yue kbd.kb
-0002f9a0: 643a 6e6f 7428 2e63 6f6d 706f 756e 6429  d:not(.compound)
-0002f9b0: 7b66 6f6e 742d 7369 7a65 3a2e 3836 7265  {font-size:.86re
-0002f9c0: 6d3b 7061 6464 696e 673a 3270 7820 3570  m;padding:2px 5p
-0002f9d0: 783b 626f 7264 6572 2d72 6164 6975 733a  x;border-radius:
-0002f9e0: 3370 783b 6d61 7267 696e 2d72 6967 6874  3px;margin-right
-0002f9f0: 3a2e 3235 7265 6d7d 2e79 7565 206b 6264  :.25rem}.yue kbd
-0002fa00: 2e63 6f6d 706f 756e 643e 6b62 647b 6d61  .compound>kbd{ma
-0002fa10: 7267 696e 2d6c 6566 743a 2e32 3572 656d  rgin-left:.25rem
-0002fa20: 7d2e 6c69 6768 7420 2e73 6561 7263 6862  }.light .searchb
-0002fa30: 6f78 206b 6264 2c2e 6c69 6768 7420 2e79  ox kbd,.light .y
-0002fa40: 7565 206b 6264 2e6b 6264 3a6e 6f74 282e  ue kbd.kbd:not(.
-0002fa50: 636f 6d70 6f75 6e64 297b 626f 7264 6572  compound){border
-0002fa60: 3a30 3b62 6163 6b67 726f 756e 643a 6c69  :0;background:li
-0002fa70: 6e65 6172 2d67 7261 6469 656e 7428 2d32  near-gradient(-2
-0002fa80: 3235 6465 672c 2365 3665 3665 362c 2366  25deg,#e6e6e6,#f
-0002fa90: 3866 3866 3829 3b62 6f78 2d73 6861 646f  8f8f8);box-shado
-0002faa0: 773a 696e 7365 7420 3020 2d32 7078 2023  w:inset 0 -2px #
-0002fab0: 6462 6462 6462 2c69 6e73 6574 2030 2030  dbdbdb,inset 0 0
-0002fac0: 2031 7078 2031 7078 2023 6666 662c 3020   1px 1px #fff,0 
-0002fad0: 3170 7820 3270 7820 3170 7820 2335 3035  1px 2px 1px #505
-0002fae0: 3035 3036 367d 2e64 6172 6b20 2e73 6561  05066}.dark .sea
-0002faf0: 7263 6862 6f78 206b 6264 2c2e 6461 726b  rchbox kbd,.dark
-0002fb00: 202e 7975 6520 6b62 642e 6b62 643a 6e6f   .yue kbd.kbd:no
-0002fb10: 7428 2e63 6f6d 706f 756e 6429 7b62 6f72  t(.compound){bor
-0002fb20: 6465 723a 303b 6261 636b 6772 6f75 6e64  der:0;background
-0002fb30: 3a6c 696e 6561 722d 6772 6164 6965 6e74  :linear-gradient
-0002fb40: 282d 3232 3564 6567 2c23 3335 3334 3334  (-225deg,#353434
-0002fb50: 2c23 3134 3134 3134 293b 626f 782d 7368  ,#141414);box-sh
-0002fb60: 6164 6f77 3a69 6e73 6574 2030 202d 3270  adow:inset 0 -2p
-0002fb70: 7820 2333 3733 3733 372c 696e 7365 7420  x #373737,inset 
-0002fb80: 3020 3020 3170 7820 3170 7820 2332 3232  0 0 1px 1px #222
-0002fb90: 2c30 2031 7078 2032 7078 2031 7078 2023  ,0 1px 2px 1px #
-0002fba0: 3030 307d 2e68 6c69 7374 2074 647b 7665  000}.hlist td{ve
-0002fbb0: 7274 6963 616c 2d61 6c69 676e 3a74 6f70  rtical-align:top
-0002fbc0: 7d70 2e63 656e 7465 7265 647b 7465 7874  }p.centered{text
-0002fbd0: 2d61 6c69 676e 3a63 656e 7465 727d 2e64  -align:center}.d
-0002fbe0: 6172 6b20 2e64 6172 6b2d 6869 6464 656e  ark .dark-hidden
-0002fbf0: 2c2e 6461 726b 202e 6c69 6768 742d 6f6e  ,.dark .light-on
-0002fc00: 6c79 2c2e 6c69 6768 7420 2e64 6172 6b2d  ly,.light .dark-
-0002fc10: 6f6e 6c79 2c2e 6c69 6768 7420 2e6c 6967  only,.light .lig
-0002fc20: 6874 2d68 6964 6465 6e7b 6469 7370 6c61  ht-hidden{displa
-0002fc30: 793a 6e6f 6e65 7d2e 7975 6520 2e67 656e  y:none}.yue .gen
-0002fc40: 696e 6465 782d 6a75 6d70 626f 782c 2e79  index-jumpbox,.y
-0002fc50: 7565 202e 6d6f 6469 6e64 6578 2d6a 756d  ue .modindex-jum
-0002fc60: 7062 6f78 7b62 6f72 6465 722d 746f 703a  pbox{border-top:
-0002fc70: 3170 7820 736f 6c69 6420 7661 7228 2d2d  1px solid var(--
-0002fc80: 7379 2d63 2d62 6f72 6465 7229 3b62 6f72  sy-c-border);bor
-0002fc90: 6465 722d 626f 7474 6f6d 3a31 7078 2073  der-bottom:1px s
-0002fca0: 6f6c 6964 2076 6172 282d 2d73 792d 632d  olid var(--sy-c-
-0002fcb0: 626f 7264 6572 293b 7061 6464 696e 673a  border);padding:
-0002fcc0: 3270 7820 2e34 7265 6d7d 2e79 7565 2074  2px .4rem}.yue t
-0002fcd0: 6162 6c65 2e6d 6f64 696e 6465 7874 6162  able.modindextab
-0002fce0: 6c65 2074 643a 6669 7273 742d 6f66 2d74  le td:first-of-t
-0002fcf0: 7970 657b 7769 6474 683a 3238 7078 7d2e  ype{width:28px}.
-0002fd00: 7975 6520 7461 626c 652e 6d6f 6469 6e64  yue table.modind
-0002fd10: 6578 7461 626c 6520 696d 672e 746f 6767  extable img.togg
-0002fd20: 6c65 727b 6d61 7267 696e 3a30 7d2e 7975  ler{margin:0}.yu
-0002fd30: 6520 7461 626c 652e 6d6f 6469 6e64 6578  e table.modindex
-0002fd40: 7461 626c 6520 7472 2e63 6170 7b66 6f6e  table tr.cap{fon
-0002fd50: 742d 7369 7a65 3a31 2e31 3272 656d 3b62  t-size:1.12rem;b
-0002fd60: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
-0002fd70: 7379 2d63 2d73 7572 6661 6365 293b 666f  sy-c-surface);fo
-0002fd80: 6e74 2d66 616d 696c 793a 7661 7228 2d2d  nt-family:var(--
-0002fd90: 7379 2d66 2d6d 6f6e 6f29 7d2e 7975 6520  sy-f-mono)}.yue 
-0002fda0: 6832 2b74 6162 6c65 2e69 6e64 6578 7461  h2+table.indexta
-0002fdb0: 626c 652c 2e79 7565 2074 6162 6c65 2e69  ble,.yue table.i
-0002fdc0: 6e64 6578 7461 626c 6520 756c 7b6d 6172  ndextable ul{mar
-0002fdd0: 6769 6e2d 746f 703a 307d 3a72 6f6f 747b  gin-top:0}:root{
-0002fde0: 2d2d 6174 7465 6e74 696f 6e2d 6963 6f6e  --attention-icon
-0002fdf0: 3a76 6172 282d 2d6c 7563 6964 652d 616c  :var(--lucide-al
-0002fe00: 6572 742d 7572 6c29 3b2d 2d61 7474 656e  ert-url);--atten
-0002fe10: 7469 6f6e 2d31 3a76 6172 282d 2d63 7269  tion-1:var(--cri
-0002fe20: 6d73 6f6e 2d73 7572 6661 6365 293b 2d2d  mson-surface);--
-0002fe30: 6174 7465 6e74 696f 6e2d 323a 7661 7228  attention-2:var(
-0002fe40: 2d2d 6372 696d 736f 6e2d 6133 293b 2d2d  --crimson-a3);--
-0002fe50: 6174 7465 6e74 696f 6e2d 333a 7661 7228  attention-3:var(
-0002fe60: 2d2d 6372 696d 736f 6e2d 3929 3b2d 2d61  --crimson-9);--a
-0002fe70: 7474 656e 7469 6f6e 2d34 3a76 6172 282d  ttention-4:var(-
-0002fe80: 2d63 7269 6d73 6f6e 2d61 3131 293b 2d2d  -crimson-a11);--
-0002fe90: 6361 7574 696f 6e2d 6963 6f6e 3a76 6172  caution-icon:var
-0002fea0: 282d 2d6c 7563 6964 652d 7a61 702d 7572  (--lucide-zap-ur
-0002feb0: 6c29 3b2d 2d63 6175 7469 6f6e 2d31 3a76  l);--caution-1:v
-0002fec0: 6172 282d 2d61 6d62 6572 2d73 7572 6661  ar(--amber-surfa
-0002fed0: 6365 293b 2d2d 6361 7574 696f 6e2d 323a  ce);--caution-2:
-0002fee0: 7661 7228 2d2d 616d 6265 722d 6133 293b  var(--amber-a3);
-0002fef0: 2d2d 6361 7574 696f 6e2d 333a 7661 7228  --caution-3:var(
-0002ff00: 2d2d 616d 6265 722d 3929 3b2d 2d63 6175  --amber-9);--cau
-0002ff10: 7469 6f6e 2d34 3a76 6172 282d 2d61 6d62  tion-4:var(--amb
-0002ff20: 6572 2d31 3129 3b2d 2d64 616e 6765 722d  er-11);--danger-
-0002ff30: 6963 6f6e 3a76 6172 282d 2d6c 7563 6964  icon:var(--lucid
-0002ff40: 652d 736b 756c 6c2d 7572 6c29 3b2d 2d64  e-skull-url);--d
-0002ff50: 616e 6765 722d 313a 7661 7228 2d2d 7275  anger-1:var(--ru
-0002ff60: 6279 2d73 7572 6661 6365 293b 2d2d 6461  by-surface);--da
-0002ff70: 6e67 6572 2d32 3a76 6172 282d 2d72 7562  nger-2:var(--rub
-0002ff80: 792d 6133 293b 2d2d 6461 6e67 6572 2d33  y-a3);--danger-3
-0002ff90: 3a76 6172 282d 2d72 7562 792d 3929 3b2d  :var(--ruby-9);-
-0002ffa0: 2d64 616e 6765 722d 343a 7661 7228 2d2d  -danger-4:var(--
-0002ffb0: 7275 6279 2d61 3131 293b 2d2d 6572 726f  ruby-a11);--erro
-0002ffc0: 722d 6963 6f6e 3a76 6172 282d 2d6c 7563  r-icon:var(--luc
-0002ffd0: 6964 652d 636c 6f73 652d 7572 6c29 3b2d  ide-close-url);-
-0002ffe0: 2d65 7272 6f72 2d31 3a76 6172 282d 2d72  -error-1:var(--r
-0002fff0: 6564 2d73 7572 6661 6365 293b 2d2d 6572  ed-surface);--er
-00030000: 726f 722d 323a 7661 7228 2d2d 7265 642d  ror-2:var(--red-
-00030010: 6133 293b 2d2d 6572 726f 722d 333a 7661  a3);--error-3:va
-00030020: 7228 2d2d 7265 642d 3929 3b2d 2d65 7272  r(--red-9);--err
-00030030: 6f72 2d34 3a76 6172 282d 2d72 6564 2d61  or-4:var(--red-a
-00030040: 3131 293b 2d2d 6869 6e74 2d69 636f 6e3a  11);--hint-icon:
-00030050: 7661 7228 2d2d 6c75 6369 6465 2d62 656c  var(--lucide-bel
-00030060: 6c2d 7572 6c29 3b2d 2d68 696e 742d 313a  l-url);--hint-1:
-00030070: 7661 7228 2d2d 6379 616e 2d73 7572 6661  var(--cyan-surfa
-00030080: 6365 293b 2d2d 6869 6e74 2d32 3a76 6172  ce);--hint-2:var
-00030090: 282d 2d63 7961 6e2d 6133 293b 2d2d 6869  (--cyan-a3);--hi
-000300a0: 6e74 2d33 3a76 6172 282d 2d63 7961 6e2d  nt-3:var(--cyan-
-000300b0: 3929 3b2d 2d68 696e 742d 343a 7661 7228  9);--hint-4:var(
-000300c0: 2d2d 6379 616e 2d61 3131 293b 2d2d 696d  --cyan-a11);--im
-000300d0: 706f 7274 616e 742d 6963 6f6e 3a76 6172  portant-icon:var
-000300e0: 282d 2d6c 7563 6964 652d 666c 616d 652d  (--lucide-flame-
-000300f0: 7572 6c29 3b2d 2d69 6d70 6f72 7461 6e74  url);--important
-00030100: 2d31 3a76 6172 282d 2d76 696f 6c65 742d  -1:var(--violet-
-00030110: 7375 7266 6163 6529 3b2d 2d69 6d70 6f72  surface);--impor
-00030120: 7461 6e74 2d32 3a76 6172 282d 2d76 696f  tant-2:var(--vio
-00030130: 6c65 742d 6133 293b 2d2d 696d 706f 7274  let-a3);--import
-00030140: 616e 742d 333a 7661 7228 2d2d 7669 6f6c  ant-3:var(--viol
-00030150: 6574 2d39 293b 2d2d 696d 706f 7274 616e  et-9);--importan
-00030160: 742d 343a 7661 7228 2d2d 7669 6f6c 6574  t-4:var(--violet
-00030170: 2d61 3131 293b 2d2d 6e6f 7465 2d69 636f  -a11);--note-ico
-00030180: 6e3a 7661 7228 2d2d 6c75 6369 6465 2d63  n:var(--lucide-c
-00030190: 616c 656e 6461 722d 7572 6c29 3b2d 2d6e  alendar-url);--n
-000301a0: 6f74 652d 313a 7661 7228 2d2d 626c 7565  ote-1:var(--blue
-000301b0: 2d73 7572 6661 6365 293b 2d2d 6e6f 7465  -surface);--note
-000301c0: 2d32 3a76 6172 282d 2d62 6c75 652d 6133  -2:var(--blue-a3
-000301d0: 293b 2d2d 6e6f 7465 2d33 3a76 6172 282d  );--note-3:var(-
-000301e0: 2d62 6c75 652d 3929 3b2d 2d6e 6f74 652d  -blue-9);--note-
-000301f0: 343a 7661 7228 2d2d 626c 7565 2d61 3131  4:var(--blue-a11
-00030200: 293b 2d2d 7469 702d 6963 6f6e 3a76 6172  );--tip-icon:var
-00030210: 282d 2d6c 7563 6964 652d 726f 636b 6574  (--lucide-rocket
-00030220: 2d75 726c 293b 2d2d 7469 702d 313a 7661  -url);--tip-1:va
-00030230: 7228 2d2d 6772 6565 6e2d 7375 7266 6163  r(--green-surfac
-00030240: 6529 3b2d 2d74 6970 2d32 3a76 6172 282d  e);--tip-2:var(-
-00030250: 2d67 7265 656e 2d61 3329 3b2d 2d74 6970  -green-a3);--tip
-00030260: 2d33 3a76 6172 282d 2d67 7265 656e 2d39  -3:var(--green-9
-00030270: 293b 2d2d 7469 702d 343a 7661 7228 2d2d  );--tip-4:var(--
-00030280: 6772 6565 6e2d 6131 3129 3b2d 2d77 6172  green-a11);--war
-00030290: 6e69 6e67 2d69 636f 6e3a 7661 7228 2d2d  ning-icon:var(--
-000302a0: 6c75 6369 6465 2d7a 6170 2d75 726c 293b  lucide-zap-url);
-000302b0: 2d2d 7761 726e 696e 672d 313a 7661 7228  --warning-1:var(
-000302c0: 2d2d 6f72 616e 6765 2d73 7572 6661 6365  --orange-surface
-000302d0: 293b 2d2d 7761 726e 696e 672d 323a 7661  );--warning-2:va
-000302e0: 7228 2d2d 6f72 616e 6765 2d61 3329 3b2d  r(--orange-a3);-
-000302f0: 2d77 6172 6e69 6e67 2d33 3a76 6172 282d  -warning-3:var(-
-00030300: 2d6f 7261 6e67 652d 3929 3b2d 2d77 6172  -orange-9);--war
-00030310: 6e69 6e67 2d34 3a76 6172 282d 2d6f 7261  ning-4:var(--ora
-00030320: 6e67 652d 6131 3129 3b2d 2d73 6565 616c  nge-a11);--seeal
-00030330: 736f 2d69 636f 6e3a 7661 7228 2d2d 6c75  so-icon:var(--lu
-00030340: 6369 6465 2d6c 696e 6b2d 7572 6c29 3b2d  cide-link-url);-
-00030350: 2d73 6565 616c 736f 2d31 3a76 6172 282d  -seealso-1:var(-
-00030360: 2d67 6f6c 642d 7375 7266 6163 6529 3b2d  -gold-surface);-
-00030370: 2d73 6565 616c 736f 2d32 3a76 6172 282d  -seealso-2:var(-
-00030380: 2d67 6f6c 642d 6133 293b 2d2d 7365 6561  -gold-a3);--seea
-00030390: 6c73 6f2d 333a 7661 7228 2d2d 676f 6c64  lso-3:var(--gold
-000303a0: 2d39 293b 2d2d 7365 6561 6c73 6f2d 343a  -9);--seealso-4:
-000303b0: 7661 7228 2d2d 676f 6c64 2d61 3131 293b  var(--gold-a11);
-000303c0: 2d2d 746f 646f 2d69 636f 6e3a 7661 7228  --todo-icon:var(
-000303d0: 2d2d 6c75 6369 6465 2d62 6f6f 6b6d 6172  --lucide-bookmar
-000303e0: 6b2d 7572 6c29 3b2d 2d74 6f64 6f2d 313a  k-url);--todo-1:
-000303f0: 7661 7228 2d2d 6272 6f6e 7a65 2d73 7572  var(--bronze-sur
-00030400: 6661 6365 293b 2d2d 746f 646f 2d32 3a76  face);--todo-2:v
-00030410: 6172 282d 2d62 726f 6e7a 652d 6133 293b  ar(--bronze-a3);
-00030420: 2d2d 746f 646f 2d33 3a76 6172 282d 2d62  --todo-3:var(--b
-00030430: 726f 6e7a 652d 3929 3b2d 2d74 6f64 6f2d  ronze-9);--todo-
-00030440: 343a 7661 7228 2d2d 6272 6f6e 7a65 2d61  4:var(--bronze-a
-00030450: 3131 293b 2d2d 7665 7273 696f 6e61 6464  11);--versionadd
-00030460: 6564 2d31 3a76 6172 282d 2d67 7265 656e  ed-1:var(--green
-00030470: 2d73 7572 6661 6365 293b 2d2d 7665 7273  -surface);--vers
-00030480: 696f 6e61 6464 6564 2d32 3a76 6172 282d  ionadded-2:var(-
-00030490: 2d67 7265 656e 2d39 293b 2d2d 7665 7273  -green-9);--vers
-000304a0: 696f 6e63 6861 6e67 6564 2d31 3a76 6172  ionchanged-1:var
-000304b0: 282d 2d61 6d62 6572 2d73 7572 6661 6365  (--amber-surface
-000304c0: 293b 2d2d 7665 7273 696f 6e63 6861 6e67  );--versionchang
-000304d0: 6564 2d32 3a76 6172 282d 2d61 6d62 6572  ed-2:var(--amber
-000304e0: 2d39 293b 2d2d 6465 7072 6563 6174 6564  -9);--deprecated
-000304f0: 2d31 3a76 6172 282d 2d72 6564 2d73 7572  -1:var(--red-sur
-00030500: 6661 6365 293b 2d2d 6465 7072 6563 6174  face);--deprecat
-00030510: 6564 2d32 3a76 6172 282d 2d72 6564 2d39  ed-2:var(--red-9
-00030520: 297d 2e61 646d 6f6e 6974 696f 6e7b 2d2d  )}.admonition{--
-00030530: 6963 6f6e 2d75 726c 3a76 6172 282d 2d6c  icon-url:var(--l
-00030540: 7563 6964 652d 6265 6c6c 2d75 726c 293b  ucide-bell-url);
-00030550: 2d2d 636f 6c6f 722d 313a 7661 7228 2d2d  --color-1:var(--
-00030560: 636f 6c6f 722d 7375 7266 6163 652d 6163  color-surface-ac
-00030570: 6365 6e74 293b 2d2d 636f 6c6f 722d 323a  cent);--color-2:
-00030580: 7661 7228 2d2d 6163 6365 6e74 2d61 3329  var(--accent-a3)
-00030590: 3b2d 2d63 6f6c 6f72 2d33 3a76 6172 282d  ;--color-3:var(-
-000305a0: 2d61 6363 656e 742d 3929 3b2d 2d63 6f6c  -accent-9);--col
-000305b0: 6f72 2d34 3a76 6172 282d 2d61 6363 656e  or-4:var(--accen
-000305c0: 742d 6131 3129 3b70 6f73 6974 696f 6e3a  t-a11);position:
-000305d0: 7265 6c61 7469 7665 3b70 6164 6469 6e67  relative;padding
-000305e0: 3a30 2031 3670 7820 2e38 7265 6d3b 6d61  :0 16px .8rem;ma
-000305f0: 7267 696e 2d74 6f70 3a31 7265 6d3b 6d61  rgin-top:1rem;ma
-00030600: 7267 696e 2d62 6f74 746f 6d3a 3172 656d  rgin-bottom:1rem
-00030610: 3b62 6f72 6465 722d 6c65 6674 3a34 7078  ;border-left:4px
-00030620: 2073 6f6c 6964 2076 6172 282d 2d63 6f6c   solid var(--col
-00030630: 6f72 2d33 293b 6261 636b 6772 6f75 6e64  or-3);background
-00030640: 2d63 6f6c 6f72 3a76 6172 282d 2d63 6f6c  -color:var(--col
-00030650: 6f72 2d31 297d 2e61 646d 6f6e 6974 696f  or-1)}.admonitio
-00030660: 6e3a 6265 666f 7265 7b70 6f73 6974 696f  n:before{positio
-00030670: 6e3a 6162 736f 6c75 7465 3b63 6f6e 7465  n:absolute;conte
-00030680: 6e74 3a22 223b 746f 703a 3670 783b 6c65  nt:"";top:6px;le
-00030690: 6674 3a2d 3132 7078 3b77 6964 7468 3a32  ft:-12px;width:2
-000306a0: 3070 783b 6865 6967 6874 3a32 3070 783b  0px;height:20px;
-000306b0: 626f 7264 6572 2d72 6164 6975 733a 3130  border-radius:10
-000306c0: 3025 3b62 6163 6b67 726f 756e 642d 636f  0%;background-co
-000306d0: 6c6f 723a 7661 7228 2d2d 636f 6c6f 722d  lor:var(--color-
-000306e0: 3329 7d2e 6164 6d6f 6e69 7469 6f6e 2070  3)}.admonition p
-000306f0: 2e61 646d 6f6e 6974 696f 6e2d 7469 746c  .admonition-titl
-00030700: 657b 706f 7369 7469 6f6e 3a72 656c 6174  e{position:relat
-00030710: 6976 653b 6d61 7267 696e 3a30 202d 3136  ive;margin:0 -16
-00030720: 7078 202e 3872 656d 202d 3139 7078 3b70  px .8rem -19px;p
-00030730: 6164 6469 6e67 3a34 7078 2031 3870 783b  adding:4px 18px;
-00030740: 666f 6e74 2d73 697a 653a 2e38 3572 656d  font-size:.85rem
-00030750: 3b66 6f6e 742d 7765 6967 6874 3a36 3030  ;font-weight:600
-00030760: 3b6c 696e 652d 6865 6967 6874 3a31 2e37  ;line-height:1.7
-00030770: 323b 636f 6c6f 723a 7661 7228 2d2d 636f  2;color:var(--co
-00030780: 6c6f 722d 3429 3b62 6163 6b67 726f 756e  lor-4);backgroun
-00030790: 642d 636f 6c6f 723a 7661 7228 2d2d 636f  d-color:var(--co
-000307a0: 6c6f 722d 3229 3b2d 2d79 7565 2d63 2d63  lor-2);--yue-c-c
-000307b0: 6f64 653a 7661 7228 2d2d 636f 6c6f 722d  ode:var(--color-
-000307c0: 3429 3b2d 2d79 7565 2d63 2d62 6f6c 643a  4);--yue-c-bold:
-000307d0: 7661 7228 2d2d 636f 6c6f 722d 3429 7d2e  var(--color-4)}.
-000307e0: 6164 6d6f 6e69 7469 6f6e 2070 2e61 646d  admonition p.adm
-000307f0: 6f6e 6974 696f 6e2d 7469 746c 6520 7376  onition-title sv
-00030800: 677b 6469 7370 6c61 793a 696e 6c69 6e65  g{display:inline
-00030810: 2d62 6c6f 636b 7d2e 6164 6d6f 6e69 7469  -block}.admoniti
-00030820: 6f6e 2d74 6974 6c65 3a62 6566 6f72 657b  on-title:before{
-00030830: 706f 7369 7469 6f6e 3a61 6273 6f6c 7574  position:absolut
-00030840: 653b 636f 6e74 656e 743a 2222 3b74 6f70  e;content:"";top
-00030850: 3a31 3070 783b 6c65 6674 3a2d 3570 783b  :10px;left:-5px;
-00030860: 2d77 6562 6b69 742d 6d61 736b 3a76 6172  -webkit-mask:var
-00030870: 282d 2d69 636f 6e2d 7572 6c29 206e 6f2d  (--icon-url) no-
-00030880: 7265 7065 6174 3b6d 6173 6b3a 7661 7228  repeat;mask:var(
-00030890: 2d2d 6963 6f6e 2d75 726c 2920 6e6f 2d72  --icon-url) no-r
-000308a0: 6570 6561 743b 2d77 6562 6b69 742d 6d61  epeat;-webkit-ma
-000308b0: 736b 2d73 697a 653a 3130 3025 2031 3030  sk-size:100% 100
-000308c0: 253b 6d61 736b 2d73 697a 653a 3130 3025  %;mask-size:100%
-000308d0: 2031 3030 253b 666f 6e74 2d73 7479 6c65   100%;font-style
-000308e0: 3a6e 6f72 6d61 6c3b 7769 6474 683a 3132  :normal;width:12
-000308f0: 7078 3b68 6569 6768 743a 3132 7078 3b62  px;height:12px;b
-00030900: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00030910: 2366 6666 7d2e 6164 6d6f 6e69 7469 6f6e  #fff}.admonition
-00030920: 2e61 7474 656e 7469 6f6e 7b2d 2d69 636f  .attention{--ico
-00030930: 6e2d 7572 6c3a 7661 7228 2d2d 6174 7465  n-url:var(--atte
-00030940: 6e74 696f 6e2d 6963 6f6e 293b 2d2d 636f  ntion-icon);--co
-00030950: 6c6f 722d 313a 7661 7228 2d2d 6174 7465  lor-1:var(--atte
-00030960: 6e74 696f 6e2d 3129 3b2d 2d63 6f6c 6f72  ntion-1);--color
-00030970: 2d32 3a76 6172 282d 2d61 7474 656e 7469  -2:var(--attenti
-00030980: 6f6e 2d32 293b 2d2d 636f 6c6f 722d 333a  on-2);--color-3:
-00030990: 7661 7228 2d2d 6174 7465 6e74 696f 6e2d  var(--attention-
-000309a0: 3329 3b2d 2d63 6f6c 6f72 2d34 3a76 6172  3);--color-4:var
-000309b0: 282d 2d61 7474 656e 7469 6f6e 2d34 297d  (--attention-4)}
-000309c0: 2e61 646d 6f6e 6974 696f 6e2e 6361 7574  .admonition.caut
-000309d0: 696f 6e7b 2d2d 6963 6f6e 2d75 726c 3a76  ion{--icon-url:v
-000309e0: 6172 282d 2d63 6175 7469 6f6e 2d69 636f  ar(--caution-ico
-000309f0: 6e29 3b2d 2d63 6f6c 6f72 2d31 3a76 6172  n);--color-1:var
-00030a00: 282d 2d63 6175 7469 6f6e 2d31 293b 2d2d  (--caution-1);--
-00030a10: 636f 6c6f 722d 323a 7661 7228 2d2d 6361  color-2:var(--ca
-00030a20: 7574 696f 6e2d 3229 3b2d 2d63 6f6c 6f72  ution-2);--color
-00030a30: 2d33 3a76 6172 282d 2d63 6175 7469 6f6e  -3:var(--caution
-00030a40: 2d33 293b 2d2d 636f 6c6f 722d 343a 7661  -3);--color-4:va
-00030a50: 7228 2d2d 6361 7574 696f 6e2d 3429 7d2e  r(--caution-4)}.
-00030a60: 6164 6d6f 6e69 7469 6f6e 2e64 616e 6765  admonition.dange
-00030a70: 727b 2d2d 6963 6f6e 2d75 726c 3a76 6172  r{--icon-url:var
-00030a80: 282d 2d64 616e 6765 722d 6963 6f6e 293b  (--danger-icon);
-00030a90: 2d2d 636f 6c6f 722d 313a 7661 7228 2d2d  --color-1:var(--
-00030aa0: 6461 6e67 6572 2d31 293b 2d2d 636f 6c6f  danger-1);--colo
-00030ab0: 722d 323a 7661 7228 2d2d 6461 6e67 6572  r-2:var(--danger
-00030ac0: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
-00030ad0: 7228 2d2d 6461 6e67 6572 2d33 293b 2d2d  r(--danger-3);--
-00030ae0: 636f 6c6f 722d 343a 7661 7228 2d2d 6461  color-4:var(--da
-00030af0: 6e67 6572 2d34 297d 2e61 646d 6f6e 6974  nger-4)}.admonit
-00030b00: 696f 6e2e 6572 726f 727b 2d2d 6963 6f6e  ion.error{--icon
-00030b10: 2d75 726c 3a76 6172 282d 2d65 7272 6f72  -url:var(--error
-00030b20: 2d69 636f 6e29 3b2d 2d63 6f6c 6f72 2d31  -icon);--color-1
-00030b30: 3a76 6172 282d 2d65 7272 6f72 2d31 293b  :var(--error-1);
-00030b40: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
-00030b50: 6572 726f 722d 3229 3b2d 2d63 6f6c 6f72  error-2);--color
-00030b60: 2d33 3a76 6172 282d 2d65 7272 6f72 2d33  -3:var(--error-3
-00030b70: 293b 2d2d 636f 6c6f 722d 343a 7661 7228  );--color-4:var(
-00030b80: 2d2d 6572 726f 722d 3429 7d2e 6164 6d6f  --error-4)}.admo
-00030b90: 6e69 7469 6f6e 2e68 696e 747b 2d2d 6963  nition.hint{--ic
-00030ba0: 6f6e 2d75 726c 3a76 6172 282d 2d68 696e  on-url:var(--hin
-00030bb0: 742d 6963 6f6e 293b 2d2d 636f 6c6f 722d  t-icon);--color-
-00030bc0: 313a 7661 7228 2d2d 6869 6e74 2d31 293b  1:var(--hint-1);
-00030bd0: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
-00030be0: 6869 6e74 2d32 293b 2d2d 636f 6c6f 722d  hint-2);--color-
-00030bf0: 333a 7661 7228 2d2d 6869 6e74 2d33 293b  3:var(--hint-3);
-00030c00: 2d2d 636f 6c6f 722d 343a 7661 7228 2d2d  --color-4:var(--
-00030c10: 6869 6e74 2d34 297d 2e61 646d 6f6e 6974  hint-4)}.admonit
-00030c20: 696f 6e2e 696d 706f 7274 616e 747b 2d2d  ion.important{--
-00030c30: 6963 6f6e 2d75 726c 3a76 6172 282d 2d69  icon-url:var(--i
-00030c40: 6d70 6f72 7461 6e74 2d69 636f 6e29 3b2d  mportant-icon);-
-00030c50: 2d63 6f6c 6f72 2d31 3a76 6172 282d 2d69  -color-1:var(--i
-00030c60: 6d70 6f72 7461 6e74 2d31 293b 2d2d 636f  mportant-1);--co
-00030c70: 6c6f 722d 323a 7661 7228 2d2d 696d 706f  lor-2:var(--impo
-00030c80: 7274 616e 742d 3229 3b2d 2d63 6f6c 6f72  rtant-2);--color
-00030c90: 2d33 3a76 6172 282d 2d69 6d70 6f72 7461  -3:var(--importa
-00030ca0: 6e74 2d33 293b 2d2d 636f 6c6f 722d 343a  nt-3);--color-4:
-00030cb0: 7661 7228 2d2d 696d 706f 7274 616e 742d  var(--important-
-00030cc0: 3429 7d2e 6164 6d6f 6e69 7469 6f6e 2e6e  4)}.admonition.n
-00030cd0: 6f74 657b 2d2d 6963 6f6e 2d75 726c 3a76  ote{--icon-url:v
-00030ce0: 6172 282d 2d6e 6f74 652d 6963 6f6e 293b  ar(--note-icon);
-00030cf0: 2d2d 636f 6c6f 722d 313a 7661 7228 2d2d  --color-1:var(--
-00030d00: 6e6f 7465 2d31 293b 2d2d 636f 6c6f 722d  note-1);--color-
-00030d10: 323a 7661 7228 2d2d 6e6f 7465 2d32 293b  2:var(--note-2);
-00030d20: 2d2d 636f 6c6f 722d 333a 7661 7228 2d2d  --color-3:var(--
-00030d30: 6e6f 7465 2d33 293b 2d2d 636f 6c6f 722d  note-3);--color-
-00030d40: 343a 7661 7228 2d2d 6e6f 7465 2d34 297d  4:var(--note-4)}
-00030d50: 2e61 646d 6f6e 6974 696f 6e2e 7469 707b  .admonition.tip{
-00030d60: 2d2d 6963 6f6e 2d75 726c 3a76 6172 282d  --icon-url:var(-
-00030d70: 2d74 6970 2d69 636f 6e29 3b2d 2d63 6f6c  -tip-icon);--col
-00030d80: 6f72 2d31 3a76 6172 282d 2d74 6970 2d31  or-1:var(--tip-1
-00030d90: 293b 2d2d 636f 6c6f 722d 323a 7661 7228  );--color-2:var(
-00030da0: 2d2d 7469 702d 3229 3b2d 2d63 6f6c 6f72  --tip-2);--color
-00030db0: 2d33 3a76 6172 282d 2d74 6970 2d33 293b  -3:var(--tip-3);
-00030dc0: 2d2d 636f 6c6f 722d 343a 7661 7228 2d2d  --color-4:var(--
-00030dd0: 7469 702d 3429 7d2e 6164 6d6f 6e69 7469  tip-4)}.admoniti
-00030de0: 6f6e 2e77 6172 6e69 6e67 7b2d 2d69 636f  on.warning{--ico
-00030df0: 6e2d 7572 6c3a 7661 7228 2d2d 7761 726e  n-url:var(--warn
-00030e00: 696e 672d 6963 6f6e 293b 2d2d 636f 6c6f  ing-icon);--colo
-00030e10: 722d 313a 7661 7228 2d2d 7761 726e 696e  r-1:var(--warnin
-00030e20: 672d 3129 3b2d 2d63 6f6c 6f72 2d32 3a76  g-1);--color-2:v
-00030e30: 6172 282d 2d77 6172 6e69 6e67 2d32 293b  ar(--warning-2);
-00030e40: 2d2d 636f 6c6f 722d 333a 7661 7228 2d2d  --color-3:var(--
-00030e50: 7761 726e 696e 672d 3329 3b2d 2d63 6f6c  warning-3);--col
-00030e60: 6f72 2d34 3a76 6172 282d 2d77 6172 6e69  or-4:var(--warni
-00030e70: 6e67 2d34 297d 2e61 646d 6f6e 6974 696f  ng-4)}.admonitio
-00030e80: 6e2e 7365 6561 6c73 6f7b 2d2d 6963 6f6e  n.seealso{--icon
-00030e90: 2d75 726c 3a76 6172 282d 2d73 6565 616c  -url:var(--seeal
-00030ea0: 736f 2d69 636f 6e29 3b2d 2d63 6f6c 6f72  so-icon);--color
-00030eb0: 2d31 3a76 6172 282d 2d73 6565 616c 736f  -1:var(--seealso
-00030ec0: 2d31 293b 2d2d 636f 6c6f 722d 323a 7661  -1);--color-2:va
-00030ed0: 7228 2d2d 7365 6561 6c73 6f2d 3229 3b2d  r(--seealso-2);-
-00030ee0: 2d63 6f6c 6f72 2d33 3a76 6172 282d 2d73  -color-3:var(--s
-00030ef0: 6565 616c 736f 2d33 293b 2d2d 636f 6c6f  eealso-3);--colo
-00030f00: 722d 343a 7661 7228 2d2d 7365 6561 6c73  r-4:var(--seeals
-00030f10: 6f2d 3429 7d2e 6164 6d6f 6e69 7469 6f6e  o-4)}.admonition
-00030f20: 2e61 646d 6f6e 6974 696f 6e2d 746f 646f  .admonition-todo
-00030f30: 7b2d 2d69 636f 6e2d 7572 6c3a 7661 7228  {--icon-url:var(
-00030f40: 2d2d 746f 646f 2d69 636f 6e29 3b2d 2d63  --todo-icon);--c
-00030f50: 6f6c 6f72 2d31 3a76 6172 282d 2d74 6f64  olor-1:var(--tod
-00030f60: 6f2d 3129 3b2d 2d63 6f6c 6f72 2d32 3a76  o-1);--color-2:v
-00030f70: 6172 282d 2d74 6f64 6f2d 3229 3b2d 2d63  ar(--todo-2);--c
-00030f80: 6f6c 6f72 2d33 3a76 6172 282d 2d74 6f64  olor-3:var(--tod
-00030f90: 6f2d 3329 3b2d 2d63 6f6c 6f72 2d34 3a76  o-3);--color-4:v
-00030fa0: 6172 282d 2d74 6f64 6f2d 3429 7d2e 6164  ar(--todo-4)}.ad
-00030fb0: 6d6f 6e69 7469 6f6e 2070 2e61 646d 6f6e  monition p.admon
-00030fc0: 6974 696f 6e2d 7469 746c 652b 707b 6d61  ition-title+p{ma
-00030fd0: 7267 696e 2d74 6f70 3a30 7d2e 6164 6d6f  rgin-top:0}.admo
-00030fe0: 6e69 7469 6f6e 3e3a 6c61 7374 2d63 6869  nition>:last-chi
-00030ff0: 6c64 7b6d 6172 6769 6e2d 626f 7474 6f6d  ld{margin-bottom
-00031000: 3a30 7d73 7061 6e2e 7665 7273 696f 6e6d  :0}span.versionm
-00031010: 6f64 6966 6965 647b 636f 6c6f 723a 7661  odified{color:va
-00031020: 7228 2d2d 7379 2d63 2d62 6f6c 6429 3b66  r(--sy-c-bold);f
-00031030: 6f6e 742d 7765 6967 6874 3a36 3030 7d64  ont-weight:600}d
-00031040: 6976 2e64 6570 7265 6361 7465 642c 6469  iv.deprecated,di
-00031050: 762e 7665 7273 696f 6e61 6464 6564 2c64  v.versionadded,d
-00031060: 6976 2e76 6572 7369 6f6e 6368 616e 6765  iv.versionchange
-00031070: 647b 706f 7369 7469 6f6e 3a72 656c 6174  d{position:relat
-00031080: 6976 653b 7061 6464 696e 673a 3670 7820  ive;padding:6px 
-00031090: 3172 656d 3b6d 6172 6769 6e3a 3172 656d  1rem;margin:1rem
-000310a0: 2030 3b62 6f72 6465 722d 6c65 6674 3a34   0;border-left:4
-000310b0: 7078 2073 6f6c 6964 2076 6172 282d 2d63  px solid var(--c
-000310c0: 6f6c 6f72 2d32 293b 6261 636b 6772 6f75  olor-2);backgrou
-000310d0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d63  nd-color:var(--c
-000310e0: 6f6c 6f72 2d31 293b 6c69 6e65 2d68 6569  olor-1);line-hei
-000310f0: 6768 743a 312e 3732 7d64 6976 2e64 6570  ght:1.72}div.dep
-00031100: 7265 6361 7465 643a 6265 666f 7265 2c64  recated:before,d
-00031110: 6976 2e76 6572 7369 6f6e 6164 6465 643a  iv.versionadded:
-00031120: 6265 666f 7265 2c64 6976 2e76 6572 7369  before,div.versi
-00031130: 6f6e 6368 616e 6765 643a 6265 666f 7265  onchanged:before
-00031140: 7b70 6f73 6974 696f 6e3a 6162 736f 6c75  {position:absolu
-00031150: 7465 3b63 6f6e 7465 6e74 3a76 6172 282d  te;content:var(-
-00031160: 2d76 6572 7369 6f6e 2d69 636f 6e29 3b74  -version-icon);t
-00031170: 6f70 3a31 3070 783b 6c65 6674 3a2d 3132  op:10px;left:-12
-00031180: 7078 3b63 6f6c 6f72 3a23 6666 663b 7769  px;color:#fff;wi
-00031190: 6474 683a 3230 7078 3b68 6569 6768 743a  dth:20px;height:
-000311a0: 3230 7078 3b62 6f72 6465 722d 7261 6469  20px;border-radi
-000311b0: 7573 3a31 3030 253b 6261 636b 6772 6f75  us:100%;backgrou
-000311c0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d63  nd-color:var(--c
-000311d0: 6f6c 6f72 2d32 293b 7465 7874 2d61 6c69  olor-2);text-ali
-000311e0: 676e 3a63 656e 7465 723b 666f 6e74 3a6e  gn:center;font:n
-000311f0: 6f72 6d61 6c20 3730 3020 3134 7078 2f32  ormal 700 14px/2
-00031200: 3070 7820 7661 7228 2d2d 7379 2d66 2d6d  0px var(--sy-f-m
-00031210: 6f6e 6f29 7d64 6976 2e76 6572 7369 6f6e  ono)}div.version
-00031220: 6164 6465 647b 2d2d 636f 6c6f 722d 313a  added{--color-1:
-00031230: 7661 7228 2d2d 7665 7273 696f 6e61 6464  var(--versionadd
-00031240: 6564 2d31 293b 2d2d 636f 6c6f 722d 323a  ed-1);--color-2:
-00031250: 7661 7228 2d2d 7665 7273 696f 6e61 6464  var(--versionadd
-00031260: 6564 2d32 293b 2d2d 7665 7273 696f 6e2d  ed-2);--version-
-00031270: 6963 6f6e 3a22 2322 7d64 6976 2e76 6572  icon:"#"}div.ver
-00031280: 7369 6f6e 6368 616e 6765 647b 2d2d 636f  sionchanged{--co
-00031290: 6c6f 722d 313a 7661 7228 2d2d 7665 7273  lor-1:var(--vers
-000312a0: 696f 6e63 6861 6e67 6564 2d31 293b 2d2d  ionchanged-1);--
-000312b0: 636f 6c6f 722d 323a 7661 7228 2d2d 7665  color-2:var(--ve
-000312c0: 7273 696f 6e63 6861 6e67 6564 2d32 293b  rsionchanged-2);
-000312d0: 2d2d 7665 7273 696f 6e2d 6963 6f6e 3a22  --version-icon:"
-000312e0: 2522 7d64 6976 2e64 6570 7265 6361 7465  %"}div.deprecate
-000312f0: 647b 2d2d 636f 6c6f 722d 313a 7661 7228  d{--color-1:var(
-00031300: 2d2d 6465 7072 6563 6174 6564 2d31 293b  --deprecated-1);
-00031310: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
-00031320: 6465 7072 6563 6174 6564 2d32 293b 2d2d  deprecated-2);--
-00031330: 7665 7273 696f 6e2d 6963 6f6e 3a22 2122  version-icon:"!"
-00031340: 7d64 6976 2e64 6570 7265 6361 7465 643e  }div.deprecated>
-00031350: 702c 6469 762e 7665 7273 696f 6e61 6464  p,div.versionadd
-00031360: 6564 3e70 2c64 6976 2e76 6572 7369 6f6e  ed>p,div.version
-00031370: 6368 616e 6765 643e 707b 6d61 7267 696e  changed>p{margin
-00031380: 3a30 7d2e 7975 6520 626c 6f63 6b71 756f  :0}.yue blockquo
-00031390: 7465 2e65 7069 6772 6170 687b 7061 6464  te.epigraph{padd
-000313a0: 696e 673a 3172 656d 2032 2e34 7265 6d3b  ing:1rem 2.4rem;
-000313b0: 626f 7264 6572 2d6c 6566 743a 303b 7465  border-left:0;te
-000313c0: 7874 2d61 6c69 676e 3a63 656e 7465 727d  xt-align:center}
-000313d0: 2e79 7565 2062 6c6f 636b 7175 6f74 652e  .yue blockquote.
-000313e0: 6869 6768 6c69 6768 7473 7b62 6f72 6465  highlights{borde
-000313f0: 722d 6c65 6674 2d77 6964 7468 3a34 7078  r-left-width:4px
-00031400: 3b70 6164 6469 6e67 2d74 6f70 3a2e 3272  ;padding-top:.2r
-00031410: 656d 3b70 6164 6469 6e67 2d62 6f74 746f  em;padding-botto
-00031420: 6d3a 2e32 7265 6d3b 6261 636b 6772 6f75  m:.2rem;backgrou
-00031430: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d73  nd-color:var(--s
-00031440: 792d 632d 7375 7266 6163 6529 7d2e 7975  y-c-surface)}.yu
-00031450: 6520 626c 6f63 6b71 756f 7465 2e70 756c  e blockquote.pul
-00031460: 6c2d 7175 6f74 657b 706f 7369 7469 6f6e  l-quote{position
-00031470: 3a72 656c 6174 6976 653b 666f 6e74 2d73  :relative;font-s
-00031480: 697a 653a 312e 3234 7265 6d3b 7061 6464  ize:1.24rem;padd
-00031490: 696e 673a 322e 3472 656d 2033 2e36 7265  ing:2.4rem 3.6re
-000314a0: 6d20 312e 3272 656d 3b62 6f72 6465 722d  m 1.2rem;border-
-000314b0: 6c65 6674 3a30 7d2e 7975 6520 626c 6f63  left:0}.yue bloc
-000314c0: 6b71 756f 7465 2e70 756c 6c2d 7175 6f74  kquote.pull-quot
-000314d0: 653a 6265 666f 7265 7b63 6f6e 7465 6e74  e:before{content
-000314e0: 3a22 5c32 3031 6322 3b70 6f73 6974 696f  :"\201c";positio
-000314f0: 6e3a 6162 736f 6c75 7465 3b74 6f70 3a30  n:absolute;top:0
-00031500: 3b6c 6566 743a 2e35 7265 6d3b 636f 6c6f  ;left:.5rem;colo
-00031510: 723a 7661 7228 2d2d 7975 652d 632d 7175  r:var(--yue-c-qu
-00031520: 6f74 652d 7379 6d62 6f6c 293b 666f 6e74  ote-symbol);font
-00031530: 3a37 3030 2034 7265 6d2f 3120 5469 6d65  :700 4rem/1 Time
-00031540: 7320 4e65 7720 526f 6d61 6e2c 4765 6f72  s New Roman,Geor
-00031550: 6769 612c 5061 6c61 7469 6e6f 2c54 696d  gia,Palatino,Tim
-00031560: 6573 2c73 6572 6966 7d2e 7975 6520 626c  es,serif}.yue bl
-00031570: 6f63 6b71 756f 7465 2e70 756c 6c2d 7175  ockquote.pull-qu
-00031580: 6f74 6520 2e61 7474 7269 6275 7469 6f6e  ote .attribution
-00031590: 7b74 6578 742d 616c 6967 6e3a 7269 6768  {text-align:righ
-000315a0: 747d 7072 652e 6c69 7465 7261 6c2d 626c  t}pre.literal-bl
-000315b0: 6f63 6b7b 6c69 6e65 2d68 6569 6768 743a  ock{line-height:
-000315c0: 312e 3438 3b70 6164 6469 6e67 3a31 7265  1.48;padding:1re
-000315d0: 6d3b 666f 6e74 2d73 697a 653a 2e39 3672  m;font-size:.96r
-000315e0: 656d 3b62 6163 6b67 726f 756e 642d 636f  em;background-co
-000315f0: 6c6f 723a 7661 7228 2d2d 7379 6e74 6178  lor:var(--syntax
-00031600: 2d70 7265 2d62 6729 3b62 6f72 6465 722d  -pre-bg);border-
-00031610: 7261 6469 7573 3a36 7078 3b6f 7665 7266  radius:6px;overf
-00031620: 6c6f 773a 6175 746f 7d2e 6869 6768 6c69  low:auto}.highli
-00031630: 6768 742c 2e6c 6974 6572 616c 2d62 6c6f  ght,.literal-blo
-00031640: 636b 2d77 7261 7070 6572 7b2d 2d6d 6172  ck-wrapper{--mar
-00031650: 6769 6e3a 3172 656d 3b2d 2d72 6164 6975  gin:1rem;--radiu
-00031660: 733a 3670 787d 2e68 6967 686c 6967 6874  s:6px}.highlight
-00031670: 3e70 7265 7b6c 696e 652d 6865 6967 6874  >pre{line-height
-00031680: 3a31 2e34 383b 7061 6464 696e 673a 7661  :1.48;padding:va
-00031690: 7228 2d2d 6d61 7267 696e 293b 666f 6e74  r(--margin);font
-000316a0: 2d73 697a 653a 2e39 3672 656d 3b66 6f6e  -size:.96rem;fon
-000316b0: 742d 6661 6d69 6c79 3a76 6172 282d 2d73  t-family:var(--s
-000316c0: 792d 662d 6d6f 6e6f 293b 6261 636b 6772  y-f-mono);backgr
-000316d0: 6f75 6e64 2d63 6f6c 6f72 3a76 6172 282d  ound-color:var(-
-000316e0: 2d73 796e 7461 782d 7072 652d 6267 293b  -syntax-pre-bg);
-000316f0: 626f 7264 6572 2d72 6164 6975 733a 7661  border-radius:va
-00031700: 7228 2d2d 7261 6469 7573 293b 6f76 6572  r(--radius);over
-00031710: 666c 6f77 3a61 7574 6f7d 2e77 696e 202e  flow:auto}.win .
-00031720: 6869 6768 6c69 6768 743e 7072 657b 666f  highlight>pre{fo
-00031730: 6e74 2d66 616d 696c 793a 2254 7765 6d6f  nt-family:"Twemo
-00031740: 6a69 2043 6f75 6e74 7279 2046 6c61 6773  ji Country Flags
-00031750: 222c 7661 7228 2d2d 7379 2d66 2d6d 6f6e  ",var(--sy-f-mon
-00031760: 6f29 7d2e 6869 6768 6c69 6768 7420 2e6c  o)}.highlight .l
-00031770: 696e 656e 6f73 7b64 6973 706c 6179 3a69  inenos{display:i
-00031780: 6e6c 696e 652d 626c 6f63 6b3b 626f 782d  nline-block;box-
-00031790: 7368 6164 6f77 3a2d 2e30 3572 656d 2030  shadow:-.05rem 0
-000317a0: 2076 6172 282d 2d73 796e 7461 782d 6c69   var(--syntax-li
-000317b0: 6e65 6e6f 732d 6469 7669 6465 7229 2069  nenos-divider) i
-000317c0: 6e73 6574 3b2d 7765 626b 6974 2d75 7365  nset;-webkit-use
-000317d0: 722d 7365 6c65 6374 3a6e 6f6e 653b 2d6d  r-select:none;-m
-000317e0: 6f7a 2d75 7365 722d 7365 6c65 6374 3a6e  oz-user-select:n
-000317f0: 6f6e 653b 7573 6572 2d73 656c 6563 743a  one;user-select:
-00031800: 6e6f 6e65 3b6d 6172 6769 6e2d 7269 6768  none;margin-righ
-00031810: 743a 2e38 7265 6d3b 7061 6464 696e 672d  t:.8rem;padding-
-00031820: 7269 6768 743a 2e38 7265 6d3b 6f70 6163  right:.8rem;opac
-00031830: 6974 793a 2e36 7d2e 6869 6768 6c69 6768  ity:.6}.highligh
-00031840: 7420 2e68 6c6c 7b6d 6172 6769 6e2d 6c65  t .hll{margin-le
-00031850: 6674 3a63 616c 6328 3072 656d 202d 2076  ft:calc(0rem - v
-00031860: 6172 282d 2d6d 6172 6769 6e29 293b 6d61  ar(--margin));ma
-00031870: 7267 696e 2d72 6967 6874 3a63 616c 6328  rgin-right:calc(
-00031880: 3072 656d 202d 2076 6172 282d 2d6d 6172  0rem - var(--mar
-00031890: 6769 6e29 293b 7061 6464 696e 673a 3020  gin));padding:0 
-000318a0: 7661 7228 2d2d 6d61 7267 696e 297d 2e63  var(--margin)}.c
-000318b0: 6f64 652d 626c 6f63 6b2d 6361 7074 696f  ode-block-captio
-000318c0: 6e7b 666f 6e74 2d73 697a 653a 2e38 3472  n{font-size:.84r
-000318d0: 656d 3b66 6f6e 742d 7765 6967 6874 3a36  em;font-weight:6
-000318e0: 3030 3b63 6f6c 6f72 3a76 6172 282d 2d73  00;color:var(--s
-000318f0: 796e 7461 782d 7465 7874 293b 6261 636b  yntax-text);back
-00031900: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
-00031910: 282d 2d73 796e 7461 782d 6361 702d 6267  (--syntax-cap-bg
-00031920: 293b 7061 6464 696e 673a 2e34 7265 6d20  );padding:.4rem 
-00031930: 7661 7228 2d2d 6d61 7267 696e 293b 626f  var(--margin);bo
-00031940: 7264 6572 2d72 6164 6975 733a 7661 7228  rder-radius:var(
-00031950: 2d2d 7261 6469 7573 2920 7661 7228 2d2d  --radius) var(--
-00031960: 7261 6469 7573 2920 3020 307d 2e63 6f64  radius) 0 0}.cod
-00031970: 652d 626c 6f63 6b2d 6361 7074 696f 6e2b  e-block-caption+
-00031980: 6469 763e 2e68 6967 686c 6967 6874 3e70  div>.highlight>p
-00031990: 7265 7b62 6f72 6465 722d 746f 702d 6c65  re{border-top-le
-000319a0: 6674 2d72 6164 6975 733a 303b 626f 7264  ft-radius:0;bord
-000319b0: 6572 2d74 6f70 2d72 6967 6874 2d72 6164  er-top-right-rad
-000319c0: 6975 733a 307d 6469 765b 636c 6173 735e  ius:0}div[class^
-000319d0: 3d68 6967 686c 6967 6874 5d3e 2e68 6967  =highlight]>.hig
-000319e0: 686c 6967 6874 3e70 7265 7b64 6973 706c  hlight>pre{displ
-000319f0: 6179 3a67 7269 647d 2e79 7565 202e 7461  ay:grid}.yue .ta
-00031a00: 626c 652d 7772 6170 7065 727b 7769 6474  ble-wrapper{widt
-00031a10: 683a 3130 3025 3b6f 7665 7266 6c6f 772d  h:100%;overflow-
-00031a20: 783a 6175 746f 3b6d 6172 6769 6e2d 746f  x:auto;margin-to
-00031a30: 703a 3272 656d 3b6d 6172 6769 6e2d 626f  p:2rem;margin-bo
-00031a40: 7474 6f6d 3a32 7265 6d3b 626f 7264 6572  ttom:2rem;border
-00031a50: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
-00031a60: 2d79 7565 2d63 2d74 6162 6c65 2d62 6f72  -yue-c-table-bor
-00031a70: 6465 7229 3b62 6f72 6465 722d 7261 6469  der);border-radi
-00031a80: 7573 3a36 7078 7d2e 7975 6520 2e74 6162  us:6px}.yue .tab
-00031a90: 6c65 2d77 7261 7070 6572 3e74 6162 6c65  le-wrapper>table
-00031aa0: 7b6d 6172 6769 6e3a 307d 2e79 7565 202e  {margin:0}.yue .
-00031ab0: 7461 626c 652d 7772 6170 7065 7220 7468  table-wrapper th
-00031ac0: 6561 6420 7472 7b62 6f72 6465 722d 746f  ead tr{border-to
-00031ad0: 703a 3170 7820 736f 6c69 6420 7661 7228  p:1px solid var(
-00031ae0: 2d2d 7975 652d 632d 7464 2d62 6f72 6465  --yue-c-td-borde
-00031af0: 7229 7d2e 7975 6520 2e74 6162 6c65 2d77  r)}.yue .table-w
-00031b00: 7261 7070 6572 2074 6865 6164 2074 723a  rapper thead tr:
-00031b10: 6669 7273 742d 6368 696c 647b 626f 7264  first-child{bord
-00031b20: 6572 2d74 6f70 3a30 7d2e 7975 6520 2e74  er-top:0}.yue .t
-00031b30: 6162 6c65 2d77 7261 7070 6572 2074 687b  able-wrapper th{
-00031b40: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00031b50: 3a76 6172 282d 2d79 7565 2d63 2d74 682d  :var(--yue-c-th-
-00031b60: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
-00031b70: 6572 2d6c 6566 743a 3170 7820 736f 6c69  er-left:1px soli
-00031b80: 6420 7661 7228 2d2d 7975 652d 632d 7464  d var(--yue-c-td
-00031b90: 2d62 6f72 6465 7229 3b70 6164 6469 6e67  -border);padding
-00031ba0: 3a2e 3732 3572 656d 2031 7265 6d7d 2e79  :.725rem 1rem}.y
-00031bb0: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
-00031bc0: 7220 7464 7b62 6f72 6465 722d 6c65 6674  r td{border-left
-00031bd0: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
-00031be0: 2d79 7565 2d63 2d74 642d 626f 7264 6572  -yue-c-td-border
-00031bf0: 293b 7061 6464 696e 673a 2e35 7265 6d20  );padding:.5rem 
-00031c00: 3172 656d 7d2e 7975 6520 2e74 6162 6c65  1rem}.yue .table
-00031c10: 2d77 7261 7070 6572 2074 723e 7464 3a66  -wrapper tr>td:f
-00031c20: 6972 7374 2d63 6869 6c64 2c2e 7975 6520  irst-child,.yue 
-00031c30: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
-00031c40: 723e 7468 3a66 6972 7374 2d63 6869 6c64  r>th:first-child
-00031c50: 7b62 6f72 6465 722d 6c65 6674 3a30 7d2e  {border-left:0}.
-00031c60: 7975 6520 2e74 6162 6c65 2d77 7261 7070  yue .table-wrapp
-00031c70: 6572 2063 6170 7469 6f6e 7b70 6164 6469  er caption{paddi
-00031c80: 6e67 3a2e 3572 656d 3b6d 6172 6769 6e3a  ng:.5rem;margin:
-00031c90: 303b 626f 7264 6572 2d62 6f74 746f 6d3a  0;border-bottom:
-00031ca0: 3170 7820 736f 6c69 6420 7661 7228 2d2d  1px solid var(--
-00031cb0: 7975 652d 632d 7468 2d62 6f72 6465 7229  yue-c-th-border)
-00031cc0: 7d2e 7975 6520 2e74 6162 6c65 2d77 7261  }.yue .table-wra
-00031cd0: 7070 6572 2074 626f 6479 2074 722e 726f  pper tbody tr.ro
-00031ce0: 772d 6f64 647b 6261 636b 6772 6f75 6e64  w-odd{background
-00031cf0: 2d63 6f6c 6f72 3a76 6172 282d 2d79 7565  -color:var(--yue
-00031d00: 2d63 2d72 6f77 2d62 6163 6b67 726f 756e  -c-row-backgroun
-00031d10: 6429 7d2e 7975 6520 7461 626c 652e 686c  d)}.yue table.hl
-00031d20: 6973 7420 7464 7b76 6572 7469 6361 6c2d  ist td{vertical-
-00031d30: 616c 6967 6e3a 746f 707d 2e74 6162 6c65  align:top}.table
-00031d40: 2d77 7261 7070 6572 7b6f 7665 7266 6c6f  -wrapper{overflo
-00031d50: 772d 783a 6175 746f 3b73 6372 6f6c 6c62  w-x:auto;scrollb
-00031d60: 6172 2d67 7574 7465 723a 6175 746f 7d2e  ar-gutter:auto}.
-00031d70: 7461 626c 652d 7772 6170 7065 723a 3a2d  table-wrapper::-
-00031d80: 7765 626b 6974 2d73 6372 6f6c 6c62 6172  webkit-scrollbar
-00031d90: 7b68 6569 6768 743a 2e37 3572 656d 3b77  {height:.75rem;w
-00031da0: 6964 7468 3a2e 3735 7265 6d7d 2e74 6162  idth:.75rem}.tab
-00031db0: 6c65 2d77 7261 7070 6572 3a3a 2d77 6562  le-wrapper::-web
-00031dc0: 6b69 742d 7363 726f 6c6c 6261 722d 7468  kit-scrollbar-th
-00031dd0: 756d 627b 626f 7264 6572 2d72 6164 6975  umb{border-radiu
-00031de0: 733a 3130 7078 7d2e 7461 626c 652d 7772  s:10px}.table-wr
-00031df0: 6170 7065 723a 3a2d 7765 626b 6974 2d73  apper::-webkit-s
-00031e00: 6372 6f6c 6c62 6172 2d74 7261 636b 7b62  crollbar-track{b
-00031e10: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00031e20: 696e 6974 6961 6c7d 2e74 6162 6c65 2d77  initial}.table-w
-00031e30: 7261 7070 6572 3a68 6f76 6572 3a3a 2d77  rapper:hover::-w
-00031e40: 6562 6b69 742d 7363 726f 6c6c 6261 722d  ebkit-scrollbar-
-00031e50: 7468 756d 627b 6261 636b 6772 6f75 6e64  thumb{background
-00031e60: 2d63 6f6c 6f72 3a23 3962 3962 3962 3333  -color:#9b9b9b33
-00031e70: 3b62 6163 6b67 726f 756e 642d 636c 6970  ;background-clip
-00031e80: 3a63 6f6e 7465 6e74 2d62 6f78 3b62 6f72  :content-box;bor
-00031e90: 6465 723a 3370 7820 736f 6c69 6420 2330  der:3px solid #0
-00031ea0: 3030 307d 2e79 7565 2074 6162 6c65 2e67  000}.yue table.g
-00031eb0: 686f 7374 2074 642c 2e79 7565 2074 6162  host td,.yue tab
-00031ec0: 6c65 2e67 686f 7374 2074 687b 626f 7264  le.ghost th{bord
-00031ed0: 6572 2d6c 6566 743a 303b 626f 7264 6572  er-left:0;border
-00031ee0: 2d72 6967 6874 3a30 3b62 6163 6b67 726f  -right:0;backgro
-00031ef0: 756e 642d 636f 6c6f 723a 696e 6974 6961  und-color:initia
-00031f00: 6c7d 2e79 7565 2074 6162 6c65 2e67 686f  l}.yue table.gho
-00031f10: 7374 2063 6170 7469 6f6e 7b6d 6172 6769  st caption{margi
-00031f20: 6e2d 626f 7474 6f6d 3a30 3b70 6164 6469  n-bottom:0;paddi
-00031f30: 6e67 2d62 6f74 746f 6d3a 2e35 7265 6d3b  ng-bottom:.5rem;
-00031f40: 626f 7264 6572 2d62 6f74 746f 6d3a 3370  border-bottom:3p
-00031f50: 7820 736f 6c69 6420 7661 7228 2d2d 7975  x solid var(--yu
-00031f60: 652d 632d 7464 2d62 6f72 6465 7229 7d2e  e-c-td-border)}.
-00031f70: 7975 6520 7461 626c 652e 6768 6f73 7420  yue table.ghost 
-00031f80: 7468 6561 6420 7472 3a66 6972 7374 2d63  thead tr:first-c
-00031f90: 6869 6c64 7b62 6f72 6465 722d 746f 703a  hild{border-top:
-00031fa0: 303b 626f 7264 6572 2d62 6f74 746f 6d2d  0;border-bottom-
-00031fb0: 7769 6474 683a 3370 787d 2e79 7565 202e  width:3px}.yue .
-00031fc0: 7461 626c 652d 7772 6170 7065 722e 6768  table-wrapper.gh
-00031fd0: 6f73 747b 626f 7264 6572 3a30 7d3a 726f  ost{border:0}:ro
-00031fe0: 6f74 7b2d 2d73 6967 2d70 726f 7065 7274  ot{--sig-propert
-00031ff0: 793a 7661 7228 2d2d 7379 6e74 6178 2d6b  y:var(--syntax-k
-00032000: 6579 776f 7264 293b 2d2d 7369 672d 6e61  eyword);--sig-na
-00032010: 6d65 3a76 6172 282d 2d73 796e 7461 782d  me:var(--syntax-
-00032020: 7072 6f70 6572 7479 293b 2d2d 7369 672d  property);--sig-
-00032030: 7479 7065 6869 6e74 3a76 6172 282d 2d73  typehint:var(--s
-00032040: 796e 7461 782d 636f 6e73 7461 6e74 293b  yntax-constant);
-00032050: 2d2d 7369 672d 7061 7261 6d3a 7661 7228  --sig-param:var(
-00032060: 2d2d 7379 6e74 6178 2d6d 6574 6129 7d64  --syntax-meta)}d
-00032070: 742e 7369 677b 706f 7369 7469 6f6e 3a72  t.sig{position:r
-00032080: 656c 6174 6976 653b 666f 6e74 2d73 697a  elative;font-siz
-00032090: 653a 2e39 3272 656d 3b70 6164 6469 6e67  e:.92rem;padding
-000320a0: 3a2e 3235 7265 6d20 2e35 7265 6d20 2e32  :.25rem .5rem .2
-000320b0: 3572 656d 2033 7265 6d3b 7465 7874 2d69  5rem 3rem;text-i
-000320c0: 6e64 656e 743a 2d32 2e34 7265 6d3b 626f  ndent:-2.4rem;bo
-000320d0: 7264 6572 2d72 6164 6975 733a 3670 787d  rder-radius:6px}
-000320e0: 6474 2e73 6967 3a61 6674 6572 7b63 6f6e  dt.sig:after{con
-000320f0: 7465 6e74 3a22 223b 6469 7370 6c61 793a  tent:"";display:
-00032100: 7461 626c 653b 636c 6561 723a 626f 7468  table;clear:both
-00032110: 7d64 742e 7369 673a 686f 7665 727b 6261  }dt.sig:hover{ba
-00032120: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
-00032130: 792d 632d 7375 7266 6163 6529 7d64 742e  y-c-surface)}dt.
-00032140: 7369 672b 6464 7b66 6f6e 742d 7369 7a65  sig+dd{font-size
-00032150: 3a2e 3932 7265 6d3b 6d61 7267 696e 2d6c  :.92rem;margin-l
-00032160: 6566 743a 3272 656d 7d64 742e 7369 673e  eft:2rem}dt.sig>
-00032170: 656d 2e70 726f 7065 7274 793a 6669 7273  em.property:firs
-00032180: 742d 6368 696c 647b 636f 6c6f 723a 7661  t-child{color:va
-00032190: 7228 2d2d 7369 672d 7072 6f70 6572 7479  r(--sig-property
-000321a0: 297d 646c 2e66 6965 6c64 2d6c 6973 7420  )}dl.field-list 
-000321b0: 617b 666f 6e74 2d77 6569 6768 743a 3430  a{font-weight:40
-000321c0: 307d 6474 2e73 6967 2b64 643e 6469 767b  0}dt.sig+dd>div{
-000321d0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3172  margin-bottom:1r
-000321e0: 656d 7d64 742e 7369 672b 6464 3e64 6c2e  em}dt.sig+dd>dl.
-000321f0: 6669 656c 642d 6c69 7374 3e64 747b 7465  field-list>dt{te
-00032200: 7874 2d74 7261 6e73 666f 726d 3a75 7070  xt-transform:upp
-00032210: 6572 6361 7365 3b66 6f6e 742d 7369 7a65  ercase;font-size
-00032220: 3a2e 3736 7265 6d7d 656d 2e70 726f 7065  :.76rem}em.prope
-00032230: 7274 792c 656d 2e73 6967 2d70 6172 616d  rty,em.sig-param
-00032240: 7b66 6f6e 742d 7374 796c 653a 6e6f 726d  {font-style:norm
-00032250: 616c 7d65 6d2e 7369 672d 7061 7261 6d7b  al}em.sig-param{
-00032260: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
-00032270: 2d6c 6967 6874 297d 7370 616e 2e73 6967  -light)}span.sig
-00032280: 2d6e 616d 652c 7370 616e 2e73 6967 2d70  -name,span.sig-p
-00032290: 7265 6e61 6d65 7b63 6f6c 6f72 3a76 6172  rename{color:var
-000322a0: 282d 2d73 6967 2d6e 616d 6529 7d73 7061  (--sig-name)}spa
-000322b0: 6e2e 7369 672d 6e61 6d65 7b66 6f6e 742d  n.sig-name{font-
-000322c0: 7765 6967 6874 3a36 3030 7d73 7061 6e2e  weight:600}span.
-000322d0: 7369 672d 7265 7475 726e 2d69 636f 6e7b  sig-return-icon{
-000322e0: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
-000322f0: 2d6c 6967 6874 297d 7370 616e 2e73 6967  -light)}span.sig
-00032300: 2d72 6574 7572 6e2d 7479 7065 6869 6e74  -return-typehint
-00032310: 2c73 7061 6e2e 7369 672d 7265 7475 726e  ,span.sig-return
-00032320: 2d74 7970 6568 696e 743e 617b 636f 6c6f  -typehint>a{colo
-00032330: 723a 7661 7228 2d2d 7369 672d 7479 7065  r:var(--sig-type
-00032340: 6869 6e74 297d 7370 616e 2e70 7265 2c73  hint)}span.pre,s
-00032350: 7061 6e2e 7369 672d 7061 7265 6e7b 666f  pan.sig-paren{fo
-00032360: 6e74 2d66 616d 696c 793a 7661 7228 2d2d  nt-family:var(--
-00032370: 7379 2d66 2d6d 6f6e 6f29 7d64 742e 7369  sy-f-mono)}dt.si
-00032380: 673e 612e 696e 7465 726e 616c 7b66 6f6e  g>a.internal{fon
-00032390: 742d 7369 7a65 3a2e 3832 7265 6d3b 626f  t-size:.82rem;bo
-000323a0: 7264 6572 3a30 3b63 6f6c 6f72 3a76 6172  rder:0;color:var
-000323b0: 282d 2d73 792d 632d 6c69 6768 7429 7d64  (--sy-c-light)}d
-000323c0: 742e 7369 673e 612e 696e 7465 726e 616c  t.sig>a.internal
-000323d0: 3a62 6566 6f72 657b 636f 6e74 656e 743a  :before{content:
-000323e0: 225c 6122 3b77 6869 7465 2d73 7061 6365  "\a";white-space
-000323f0: 3a70 7265 7d2e 7669 6577 636f 6465 2d62  :pre}.viewcode-b
-00032400: 6c6f 636b 7b70 6f73 6974 696f 6e3a 7265  lock{position:re
-00032410: 6c61 7469 7665 7d2e 7669 6577 636f 6465  lative}.viewcode
-00032420: 2d62 6163 6b7b 706f 7369 7469 6f6e 3a61  -back{position:a
-00032430: 6273 6f6c 7574 653b 746f 703a 2d31 2e35  bsolute;top:-1.5
-00032440: 7265 6d3b 666f 6e74 2d73 697a 653a 2e38  rem;font-size:.8
-00032450: 7265 6d7d 2e63 6c61 7373 6966 6965 727b  rem}.classifier{
-00032460: 666f 6e74 2d73 7479 6c65 3a6f 626c 6971  font-style:obliq
-00032470: 7565 3b66 6f6e 742d 7765 6967 6874 3a34  ue;font-weight:4
-00032480: 3030 7d2e 636c 6173 7369 6669 6572 3a62  00}.classifier:b
-00032490: 6566 6f72 657b 666f 6e74 2d73 7479 6c65  efore{font-style
-000324a0: 3a6e 6f72 6d61 6c3b 6d61 7267 696e 2d6c  :normal;margin-l
-000324b0: 6566 743a 2e31 7265 6d3b 6d61 7267 696e  eft:.1rem;margin
-000324c0: 2d72 6967 6874 3a2e 3572 656d 3b63 6f6e  -right:.5rem;con
-000324d0: 7465 6e74 3a22 3a22 3b64 6973 706c 6179  tent:":";display
-000324e0: 3a69 6e6c 696e 652d 626c 6f63 6b7d 2e79  :inline-block}.y
-000324f0: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
-00032500: 722e 6175 746f 7375 6d6d 6172 797b 626f  r.autosummary{bo
-00032510: 7264 6572 2d6c 6566 743a 303b 626f 7264  rder-left:0;bord
-00032520: 6572 2d72 6967 6874 3a30 3b62 6f72 6465  er-right:0;borde
-00032530: 722d 7261 6469 7573 3a30 7d2e 7975 6520  r-radius:0}.yue 
-00032540: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
-00032550: 6162 6c65 2e61 7574 6f73 756d 6d61 7279  able.autosummary
-00032560: 2074 647b 626f 7264 6572 3a6e 6f6e 653b   td{border:none;
-00032570: 7061 6464 696e 672d 746f 703a 2e32 3572  padding-top:.25r
-00032580: 656d 3b70 6164 6469 6e67 2d62 6f74 746f  em;padding-botto
-00032590: 6d3a 2e32 3572 656d 7d2e 7975 6520 702e  m:.25rem}.yue p.
-000325a0: 7275 6272 6963 2b64 6976 2e61 7574 6f73  rubric+div.autos
-000325b0: 756d 6d61 7279 7b6d 6172 6769 6e2d 746f  ummary{margin-to
-000325c0: 703a 307d 3a72 6f6f 747b 2d2d 7379 6e74  p:0}:root{--synt
-000325d0: 6178 2d70 7265 2d62 673a 7661 7228 2d2d  ax-pre-bg:var(--
-000325e0: 6163 6365 6e74 2d61 3229 3b2d 2d73 796e  accent-a2);--syn
-000325f0: 7461 782d 6361 702d 6267 3a76 6172 282d  tax-cap-bg:var(-
-00032600: 2d61 6363 656e 742d 6133 293b 2d2d 7379  -accent-a3);--sy
-00032610: 6e74 6178 2d68 6967 686c 6967 6874 2d62  ntax-highlight-b
-00032620: 673a 7661 7228 2d2d 6163 6365 6e74 2d61  g:var(--accent-a
-00032630: 3329 3b2d 2d73 796e 7461 782d 6c69 6e65  3);--syntax-line
-00032640: 6e6f 732d 6469 7669 6465 723a 7661 7228  nos-divider:var(
-00032650: 2d2d 6772 6179 2d61 3629 3b2d 2d73 796e  --gray-a6);--syn
-00032660: 7461 782d 6c69 6768 742d 7465 7874 3a23  tax-light-text:#
-00032670: 3234 3239 3266 3b2d 2d73 796e 7461 782d  24292f;--syntax-
-00032680: 6c69 6768 742d 6d65 7461 3a23 3830 3763  light-meta:#807c
-00032690: 3837 3b2d 2d73 796e 7461 782d 6c69 6768  87;--syntax-ligh
-000326a0: 742d 636f 6d6d 656e 743a 2336 6537 3738  t-comment:#6e778
-000326b0: 313b 2d2d 7379 6e74 6178 2d6c 6967 6874  1;--syntax-light
-000326c0: 2d63 6f6e 7374 616e 743a 2330 3535 3061  -constant:#0550a
-000326d0: 653b 2d2d 7379 6e74 6178 2d6c 6967 6874  e;--syntax-light
-000326e0: 2d65 6e74 6974 793a 2332 3638 6264 323b  -entity:#268bd2;
-000326f0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d70  --syntax-light-p
-00032700: 726f 7065 7274 793a 2338 3235 3064 663b  roperty:#8250df;
-00032710: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d64  --syntax-light-d
-00032720: 6566 696e 6974 696f 6e3a 2332 3432 3932  efinition:#24292
-00032730: 663b 2d2d 7379 6e74 6178 2d6c 6967 6874  f;--syntax-light
-00032740: 2d74 6167 3a23 3038 353b 2d2d 7379 6e74  -tag:#085;--synt
-00032750: 6178 2d6c 6967 6874 2d62 7569 6c74 696e  ax-light-builtin
-00032760: 3a23 6235 3839 3030 3b2d 2d73 796e 7461  :#b58900;--synta
-00032770: 782d 6c69 6768 742d 6b65 7977 6f72 643a  x-light-keyword:
-00032780: 2363 6632 3232 653b 2d2d 7379 6e74 6178  #cf222e;--syntax
-00032790: 2d6c 6967 6874 2d65 7863 6570 7469 6f6e  -light-exception
-000327a0: 3a23 6536 3231 3265 3b2d 2d73 796e 7461  :#e6212e;--synta
-000327b0: 782d 6c69 6768 742d 7374 7269 6e67 3a23  x-light-string:#
-000327c0: 3061 3330 3639 3b2d 2d73 796e 7461 782d  0a3069;--syntax-
-000327d0: 6c69 6768 742d 7265 6765 7870 3a23 6534  light-regexp:#e4
-000327e0: 303b 2d2d 7379 6e74 6178 2d6c 6967 6874  0;--syntax-light
-000327f0: 2d76 6172 6961 626c 653a 2361 3434 3830  -variable:#a4480
-00032800: 663b 2d2d 7379 6e74 6178 2d6c 6967 6874  f;--syntax-light
-00032810: 2d69 6e76 616c 6964 2d69 6c6c 6567 616c  -invalid-illegal
-00032820: 2d74 6578 743a 2366 3666 3866 613b 2d2d  -text:#f6f8fa;--
-00032830: 7379 6e74 6178 2d6c 6967 6874 2d69 6e76  syntax-light-inv
-00032840: 616c 6964 2d69 6c6c 6567 616c 2d62 673a  alid-illegal-bg:
-00032850: 2338 3230 3731 653b 2d2d 7379 6e74 6178  #82071e;--syntax
-00032860: 2d6c 6967 6874 2d6d 6172 6b75 702d 6865  -light-markup-he
-00032870: 6164 696e 673a 2330 3535 3061 653b 2d2d  ading:#0550ae;--
-00032880: 7379 6e74 6178 2d6c 6967 6874 2d6d 6172  syntax-light-mar
-00032890: 6b75 702d 6974 616c 6963 3a23 3234 3239  kup-italic:#2429
-000328a0: 3266 3b2d 2d73 796e 7461 782d 6c69 6768  2f;--syntax-ligh
-000328b0: 742d 6d61 726b 7570 2d62 6f6c 643a 2332  t-markup-bold:#2
-000328c0: 3432 3932 663b 2d2d 7379 6e74 6178 2d6c  4292f;--syntax-l
-000328d0: 6967 6874 2d6d 6172 6b75 702d 6465 6c65  ight-markup-dele
-000328e0: 7465 642d 7465 7874 3a23 3832 3037 3165  ted-text:#82071e
-000328f0: 3b2d 2d73 796e 7461 782d 6c69 6768 742d  ;--syntax-light-
-00032900: 6d61 726b 7570 2d64 656c 6574 6564 2d62  markup-deleted-b
-00032910: 673a 2366 6665 6265 393b 2d2d 7379 6e74  g:#ffebe9;--synt
-00032920: 6178 2d6c 6967 6874 2d6d 6172 6b75 702d  ax-light-markup-
-00032930: 696e 7365 7274 6564 2d74 6578 743a 2331  inserted-text:#1
-00032940: 3136 3332 393b 2d2d 7379 6e74 6178 2d6c  16329;--syntax-l
-00032950: 6967 6874 2d6d 6172 6b75 702d 696e 7365  ight-markup-inse
-00032960: 7274 6564 2d62 673a 2364 6166 6265 313b  rted-bg:#dafbe1;
-00032970: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00032980: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
-00032990: 7874 3a23 3935 3338 3030 3b2d 2d73 796e  xt:#953800;--syn
-000329a0: 7461 782d 6c69 6768 742d 6d61 726b 7570  tax-light-markup
-000329b0: 2d63 6861 6e67 6564 2d62 673a 2366 6664  -changed-bg:#ffd
-000329c0: 3862 353b 2d2d 7379 6e74 6178 2d6c 6967  8b5;--syntax-lig
-000329d0: 6874 2d6d 6172 6b75 702d 6967 6e6f 7265  ht-markup-ignore
-000329e0: 642d 7465 7874 3a23 6561 6565 6632 3b2d  d-text:#eaeef2;-
-000329f0: 2d73 796e 7461 782d 6c69 6768 742d 6d61  -syntax-light-ma
-00032a00: 726b 7570 2d69 676e 6f72 6564 2d62 673a  rkup-ignored-bg:
-00032a10: 2330 3535 3061 653b 2d2d 7379 6e74 6178  #0550ae;--syntax
-00032a20: 2d6c 6967 6874 2d6d 6574 612d 6469 6666  -light-meta-diff
-00032a30: 2d72 616e 6765 3a23 3832 3530 6466 3b2d  -range:#8250df;-
-00032a40: 2d73 796e 7461 782d 6c69 6768 742d 7370  -syntax-light-sp
-00032a50: 6563 6961 6c2d 6267 3a23 6463 6361 6661  ecial-bg:#dccafa
-00032a60: 3b2d 2d73 796e 7461 782d 6461 726b 2d74  ;--syntax-dark-t
-00032a70: 6578 743a 2363 3964 3164 393b 2d2d 7379  ext:#c9d1d9;--sy
-00032a80: 6e74 6178 2d64 6172 6b2d 6d65 7461 3a23  ntax-dark-meta:#
-00032a90: 3665 3737 3831 3b2d 2d73 796e 7461 782d  6e7781;--syntax-
-00032aa0: 6461 726b 2d63 6f6d 6d65 6e74 3a23 3862  dark-comment:#8b
-00032ab0: 3934 3965 3b2d 2d73 796e 7461 782d 6461  949e;--syntax-da
-00032ac0: 726b 2d63 6f6e 7374 616e 743a 2337 3963  rk-constant:#79c
-00032ad0: 3066 663b 2d2d 7379 6e74 6178 2d64 6172  0ff;--syntax-dar
-00032ae0: 6b2d 656e 7469 7479 3a23 3437 6230 6661  k-entity:#47b0fa
-00032af0: 3b2d 2d73 796e 7461 782d 6461 726b 2d70  ;--syntax-dark-p
-00032b00: 726f 7065 7274 793a 2364 3261 3866 663b  roperty:#d2a8ff;
-00032b10: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6465  --syntax-dark-de
-00032b20: 6669 6e69 7469 6f6e 3a23 6339 6431 6439  finition:#c9d1d9
-00032b30: 3b2d 2d73 796e 7461 782d 6461 726b 2d74  ;--syntax-dark-t
-00032b40: 6167 3a23 3765 6537 3837 3b2d 2d73 796e  ag:#7ee787;--syn
-00032b50: 7461 782d 6461 726b 2d62 7569 6c74 696e  tax-dark-builtin
-00032b60: 3a23 6666 6433 3463 3b2d 2d73 796e 7461  :#ffd34c;--synta
-00032b70: 782d 6461 726b 2d6b 6579 776f 7264 3a23  x-dark-keyword:#
-00032b80: 6666 3762 3732 3b2d 2d73 796e 7461 782d  ff7b72;--syntax-
-00032b90: 6461 726b 2d65 7863 6570 7469 6f6e 3a23  dark-exception:#
-00032ba0: 6461 3437 3363 3b2d 2d73 796e 7461 782d  da473c;--syntax-
-00032bb0: 6461 726b 2d73 7472 696e 673a 2361 3564  dark-string:#a5d
-00032bc0: 3666 663b 2d2d 7379 6e74 6178 2d64 6172  6ff;--syntax-dar
-00032bd0: 6b2d 7265 6765 7870 3a23 6566 3935 3465  k-regexp:#ef954e
-00032be0: 3b2d 2d73 796e 7461 782d 6461 726b 2d76  ;--syntax-dark-v
-00032bf0: 6172 6961 626c 653a 2366 6661 3635 373b  ariable:#ffa657;
-00032c00: 2d2d 7379 6e74 6178 2d64 6172 6b2d 696e  --syntax-dark-in
-00032c10: 7661 6c69 642d 696c 6c65 6761 6c2d 7465  valid-illegal-te
-00032c20: 7874 3a23 6630 6636 6663 3b2d 2d73 796e  xt:#f0f6fc;--syn
-00032c30: 7461 782d 6461 726b 2d69 6e76 616c 6964  tax-dark-invalid
-00032c40: 2d69 6c6c 6567 616c 2d62 673a 2338 6531  -illegal-bg:#8e1
-00032c50: 3531 393b 2d2d 7379 6e74 6178 2d64 6172  519;--syntax-dar
-00032c60: 6b2d 6d61 726b 7570 2d68 6561 6469 6e67  k-markup-heading
-00032c70: 3a23 3166 3666 6562 3b2d 2d73 796e 7461  :#1f6feb;--synta
-00032c80: 782d 6461 726b 2d6d 6172 6b75 702d 6974  x-dark-markup-it
-00032c90: 616c 6963 3a23 6339 6431 6439 3b2d 2d73  alic:#c9d1d9;--s
-00032ca0: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
-00032cb0: 702d 626f 6c64 3a23 6339 6431 6439 3b2d  p-bold:#c9d1d9;-
-00032cc0: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-00032cd0: 6b75 702d 6465 6c65 7465 642d 7465 7874  kup-deleted-text
-00032ce0: 3a23 6666 6463 6437 3b2d 2d73 796e 7461  :#ffdcd7;--synta
-00032cf0: 782d 6461 726b 2d6d 6172 6b75 702d 6465  x-dark-markup-de
-00032d00: 6c65 7465 642d 6267 3a23 3637 3036 3063  leted-bg:#67060c
-00032d10: 3b2d 2d73 796e 7461 782d 6461 726b 2d6d  ;--syntax-dark-m
-00032d20: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
-00032d30: 6578 743a 2361 6666 3562 343b 2d2d 7379  ext:#aff5b4;--sy
-00032d40: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
-00032d50: 2d69 6e73 6572 7465 642d 6267 3a23 3033  -inserted-bg:#03
-00032d60: 3361 3136 3b2d 2d73 796e 7461 782d 6461  3a16;--syntax-da
-00032d70: 726b 2d6d 6172 6b75 702d 6368 616e 6765  rk-markup-change
-00032d80: 642d 7465 7874 3a23 6666 6466 6236 3b2d  d-text:#ffdfb6;-
-00032d90: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-00032da0: 6b75 702d 6368 616e 6765 642d 6267 3a23  kup-changed-bg:#
-00032db0: 3561 3165 3032 3b2d 2d73 796e 7461 782d  5a1e02;--syntax-
-00032dc0: 6461 726b 2d6d 6172 6b75 702d 6967 6e6f  dark-markup-igno
-00032dd0: 7265 642d 7465 7874 3a23 6339 6431 6439  red-text:#c9d1d9
-00032de0: 3b2d 2d73 796e 7461 782d 6461 726b 2d6d  ;--syntax-dark-m
-00032df0: 6172 6b75 702d 6967 6e6f 7265 642d 6267  arkup-ignored-bg
-00032e00: 3a23 3131 3538 6337 3b2d 2d73 796e 7461  :#1158c7;--synta
-00032e10: 782d 6461 726b 2d6d 6574 612d 6469 6666  x-dark-meta-diff
-00032e20: 2d72 616e 6765 3a23 6432 6138 6666 3b2d  -range:#d2a8ff;-
-00032e30: 2d73 796e 7461 782d 6461 726b 2d73 7065  -syntax-dark-spe
-00032e40: 6369 616c 2d62 673a 2334 6634 3235 647d  cial-bg:#4f425d}
-00032e50: 3a72 6f6f 742c 6874 6d6c 2e6c 6967 6874  :root,html.light
-00032e60: 7b2d 2d73 796e 7461 782d 7465 7874 3a76  {--syntax-text:v
-00032e70: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-00032e80: 742d 7465 7874 293b 2d2d 7379 6e74 6178  t-text);--syntax
-00032e90: 2d6d 6574 613a 7661 7228 2d2d 7379 6e74  -meta:var(--synt
-00032ea0: 6178 2d6c 6967 6874 2d6d 6574 6129 3b2d  ax-light-meta);-
-00032eb0: 2d73 796e 7461 782d 636f 6d6d 656e 743a  -syntax-comment:
-00032ec0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00032ed0: 6874 2d63 6f6d 6d65 6e74 293b 2d2d 7379  ht-comment);--sy
-00032ee0: 6e74 6178 2d63 6f6e 7374 616e 743a 7661  ntax-constant:va
-00032ef0: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
-00032f00: 2d63 6f6e 7374 616e 7429 3b2d 2d73 796e  -constant);--syn
-00032f10: 7461 782d 656e 7469 7479 3a76 6172 282d  tax-entity:var(-
-00032f20: 2d73 796e 7461 782d 6c69 6768 742d 656e  -syntax-light-en
-00032f30: 7469 7479 293b 2d2d 7379 6e74 6178 2d70  tity);--syntax-p
-00032f40: 726f 7065 7274 793a 7661 7228 2d2d 7379  roperty:var(--sy
-00032f50: 6e74 6178 2d6c 6967 6874 2d70 726f 7065  ntax-light-prope
-00032f60: 7274 7929 3b2d 2d73 796e 7461 782d 6465  rty);--syntax-de
-00032f70: 6669 6e69 7469 6f6e 3a76 6172 282d 2d73  finition:var(--s
-00032f80: 796e 7461 782d 6c69 6768 742d 6465 6669  yntax-light-defi
-00032f90: 6e69 7469 6f6e 293b 2d2d 7379 6e74 6178  nition);--syntax
-00032fa0: 2d74 6167 3a76 6172 282d 2d73 796e 7461  -tag:var(--synta
-00032fb0: 782d 6c69 6768 742d 7461 6729 3b2d 2d73  x-light-tag);--s
-00032fc0: 796e 7461 782d 6275 696c 7469 6e3a 7661  yntax-builtin:va
-00032fd0: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
-00032fe0: 2d62 7569 6c74 696e 293b 2d2d 7379 6e74  -builtin);--synt
-00032ff0: 6178 2d6b 6579 776f 7264 3a76 6172 282d  ax-keyword:var(-
-00033000: 2d73 796e 7461 782d 6c69 6768 742d 6b65  -syntax-light-ke
-00033010: 7977 6f72 6429 3b2d 2d73 796e 7461 782d  yword);--syntax-
-00033020: 6578 6365 7074 696f 6e3a 7661 7228 2d2d  exception:var(--
-00033030: 7379 6e74 6178 2d6c 6967 6874 2d65 7863  syntax-light-exc
-00033040: 6570 7469 6f6e 293b 2d2d 7379 6e74 6178  eption);--syntax
-00033050: 2d73 7472 696e 673a 7661 7228 2d2d 7379  -string:var(--sy
-00033060: 6e74 6178 2d6c 6967 6874 2d73 7472 696e  ntax-light-strin
-00033070: 6729 3b2d 2d73 796e 7461 782d 7265 6765  g);--syntax-rege
-00033080: 7870 3a76 6172 282d 2d73 796e 7461 782d  xp:var(--syntax-
-00033090: 6c69 6768 742d 7265 6765 7870 293b 2d2d  light-regexp);--
-000330a0: 7379 6e74 6178 2d76 6172 6961 626c 653a  syntax-variable:
-000330b0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-000330c0: 6874 2d76 6172 6961 626c 6529 3b2d 2d73  ht-variable);--s
-000330d0: 796e 7461 782d 696e 7661 6c69 642d 696c  yntax-invalid-il
-000330e0: 6c65 6761 6c2d 7465 7874 3a76 6172 282d  legal-text:var(-
-000330f0: 2d73 796e 7461 782d 6c69 6768 742d 696e  -syntax-light-in
-00033100: 7661 6c69 642d 696c 6c65 6761 6c2d 7465  valid-illegal-te
-00033110: 7874 293b 2d2d 7379 6e74 6178 2d69 6e76  xt);--syntax-inv
-00033120: 616c 6964 2d69 6c6c 6567 616c 2d62 673a  alid-illegal-bg:
-00033130: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00033140: 6874 2d69 6e76 616c 6964 2d69 6c6c 6567  ht-invalid-illeg
-00033150: 616c 2d62 6729 3b2d 2d73 796e 7461 782d  al-bg);--syntax-
-00033160: 6d61 726b 7570 2d68 6561 6469 6e67 3a76  markup-heading:v
-00033170: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-00033180: 742d 6d61 726b 7570 2d68 6561 6469 6e67  t-markup-heading
-00033190: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-000331a0: 702d 6974 616c 6963 3a76 6172 282d 2d73  p-italic:var(--s
-000331b0: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-000331c0: 7570 2d69 7461 6c69 6329 3b2d 2d73 796e  up-italic);--syn
-000331d0: 7461 782d 6d61 726b 7570 2d62 6f6c 643a  tax-markup-bold:
-000331e0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-000331f0: 6874 2d6d 6172 6b75 702d 626f 6c64 293b  ht-markup-bold);
-00033200: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
-00033210: 6465 6c65 7465 642d 7465 7874 3a76 6172  deleted-text:var
-00033220: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
-00033230: 6d61 726b 7570 2d64 656c 6574 6564 2d74  markup-deleted-t
-00033240: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033250: 726b 7570 2d64 656c 6574 6564 2d62 673a  rkup-deleted-bg:
-00033260: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00033270: 6874 2d6d 6172 6b75 702d 6465 6c65 7465  ht-markup-delete
-00033280: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-00033290: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
-000332a0: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
-000332b0: 2d6c 6967 6874 2d6d 6172 6b75 702d 696e  -light-markup-in
-000332c0: 7365 7274 6564 2d74 6578 7429 3b2d 2d73  serted-text);--s
-000332d0: 796e 7461 782d 6d61 726b 7570 2d69 6e73  yntax-markup-ins
-000332e0: 6572 7465 642d 6267 3a76 6172 282d 2d73  erted-bg:var(--s
-000332f0: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-00033300: 7570 2d69 6e73 6572 7465 642d 6267 293b  up-inserted-bg);
-00033310: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
-00033320: 6368 616e 6765 642d 7465 7874 3a76 6172  changed-text:var
-00033330: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
-00033340: 6d61 726b 7570 2d63 6861 6e67 6564 2d74  markup-changed-t
-00033350: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033360: 726b 7570 2d63 6861 6e67 6564 2d62 673a  rkup-changed-bg:
-00033370: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00033380: 6874 2d6d 6172 6b75 702d 6368 616e 6765  ht-markup-change
-00033390: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-000333a0: 6172 6b75 702d 6967 6e6f 7265 642d 7465  arkup-ignored-te
-000333b0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-000333c0: 6c69 6768 742d 6d61 726b 7570 2d69 676e  light-markup-ign
-000333d0: 6f72 6564 2d74 6578 7429 3b2d 2d73 796e  ored-text);--syn
-000333e0: 7461 782d 6d61 726b 7570 2d69 676e 6f72  tax-markup-ignor
-000333f0: 6564 2d62 673a 7661 7228 2d2d 7379 6e74  ed-bg:var(--synt
-00033400: 6178 2d6c 6967 6874 2d6d 6172 6b75 702d  ax-light-markup-
-00033410: 6967 6e6f 7265 642d 6267 293b 2d2d 7379  ignored-bg);--sy
-00033420: 6e74 6178 2d6d 6574 612d 6469 6666 2d72  ntax-meta-diff-r
-00033430: 616e 6765 3a76 6172 282d 2d73 796e 7461  ange:var(--synta
-00033440: 782d 6c69 6768 742d 6d65 7461 2d64 6966  x-light-meta-dif
-00033450: 662d 7261 6e67 6529 3b2d 2d73 796e 7461  f-range);--synta
-00033460: 782d 7370 6563 6961 6c2d 6267 3a76 6172  x-special-bg:var
-00033470: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
-00033480: 7370 6563 6961 6c2d 6267 297d 406d 6564  special-bg)}@med
-00033490: 6961 2028 7072 6566 6572 732d 636f 6c6f  ia (prefers-colo
-000334a0: 722d 7363 6865 6d65 3a64 6172 6b29 7b3a  r-scheme:dark){:
-000334b0: 726f 6f74 7b2d 2d73 796e 7461 782d 7465  root{--syntax-te
-000334c0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-000334d0: 6461 726b 2d74 6578 7429 3b2d 2d73 796e  dark-text);--syn
-000334e0: 7461 782d 6d65 7461 3a76 6172 282d 2d73  tax-meta:var(--s
-000334f0: 796e 7461 782d 6461 726b 2d6d 6574 6129  yntax-dark-meta)
-00033500: 3b2d 2d73 796e 7461 782d 636f 6d6d 656e  ;--syntax-commen
-00033510: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
-00033520: 6172 6b2d 636f 6d6d 656e 7429 3b2d 2d73  ark-comment);--s
-00033530: 796e 7461 782d 636f 6e73 7461 6e74 3a76  yntax-constant:v
-00033540: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00033550: 2d63 6f6e 7374 616e 7429 3b2d 2d73 796e  -constant);--syn
-00033560: 7461 782d 656e 7469 7479 3a76 6172 282d  tax-entity:var(-
-00033570: 2d73 796e 7461 782d 6461 726b 2d65 6e74  -syntax-dark-ent
-00033580: 6974 7929 3b2d 2d73 796e 7461 782d 7072  ity);--syntax-pr
-00033590: 6f70 6572 7479 3a76 6172 282d 2d73 796e  operty:var(--syn
-000335a0: 7461 782d 6461 726b 2d70 726f 7065 7274  tax-dark-propert
-000335b0: 7929 3b2d 2d73 796e 7461 782d 6465 6669  y);--syntax-defi
-000335c0: 6e69 7469 6f6e 3a76 6172 282d 2d73 796e  nition:var(--syn
-000335d0: 7461 782d 6461 726b 2d64 6566 696e 6974  tax-dark-definit
-000335e0: 696f 6e29 3b2d 2d73 796e 7461 782d 7461  ion);--syntax-ta
-000335f0: 673a 7661 7228 2d2d 7379 6e74 6178 2d64  g:var(--syntax-d
-00033600: 6172 6b2d 7461 6729 3b2d 2d73 796e 7461  ark-tag);--synta
-00033610: 782d 6275 696c 7469 6e3a 7661 7228 2d2d  x-builtin:var(--
-00033620: 7379 6e74 6178 2d64 6172 6b2d 6275 696c  syntax-dark-buil
-00033630: 7469 6e29 3b2d 2d73 796e 7461 782d 6b65  tin);--syntax-ke
-00033640: 7977 6f72 643a 7661 7228 2d2d 7379 6e74  yword:var(--synt
-00033650: 6178 2d64 6172 6b2d 6b65 7977 6f72 6429  ax-dark-keyword)
-00033660: 3b2d 2d73 796e 7461 782d 6578 6365 7074  ;--syntax-except
-00033670: 696f 6e3a 7661 7228 2d2d 7379 6e74 6178  ion:var(--syntax
-00033680: 2d64 6172 6b2d 6578 6365 7074 696f 6e29  -dark-exception)
-00033690: 3b2d 2d73 796e 7461 782d 7374 7269 6e67  ;--syntax-string
-000336a0: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-000336b0: 726b 2d73 7472 696e 6729 3b2d 2d73 796e  rk-string);--syn
-000336c0: 7461 782d 7265 6765 7870 3a76 6172 282d  tax-regexp:var(-
-000336d0: 2d73 796e 7461 782d 6461 726b 2d72 6567  -syntax-dark-reg
-000336e0: 6578 7029 3b2d 2d73 796e 7461 782d 7661  exp);--syntax-va
-000336f0: 7269 6162 6c65 3a76 6172 282d 2d73 796e  riable:var(--syn
-00033700: 7461 782d 6461 726b 2d76 6172 6961 626c  tax-dark-variabl
-00033710: 6529 3b2d 2d73 796e 7461 782d 696e 7661  e);--syntax-inva
-00033720: 6c69 642d 696c 6c65 6761 6c2d 7465 7874  lid-illegal-text
-00033730: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-00033740: 726b 2d69 6e76 616c 6964 2d69 6c6c 6567  rk-invalid-illeg
-00033750: 616c 2d74 6578 7429 3b2d 2d73 796e 7461  al-text);--synta
-00033760: 782d 696e 7661 6c69 642d 696c 6c65 6761  x-invalid-illega
-00033770: 6c2d 6267 3a76 6172 282d 2d73 796e 7461  l-bg:var(--synta
-00033780: 782d 6461 726b 2d69 6e76 616c 6964 2d69  x-dark-invalid-i
-00033790: 6c6c 6567 616c 2d62 6729 3b2d 2d73 796e  llegal-bg);--syn
-000337a0: 7461 782d 6d61 726b 7570 2d68 6561 6469  tax-markup-headi
-000337b0: 6e67 3a76 6172 282d 2d73 796e 7461 782d  ng:var(--syntax-
-000337c0: 6461 726b 2d6d 6172 6b75 702d 6865 6164  dark-markup-head
-000337d0: 696e 6729 3b2d 2d73 796e 7461 782d 6d61  ing);--syntax-ma
-000337e0: 726b 7570 2d69 7461 6c69 633a 7661 7228  rkup-italic:var(
-000337f0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-00033800: 726b 7570 2d69 7461 6c69 6329 3b2d 2d73  rkup-italic);--s
-00033810: 796e 7461 782d 6d61 726b 7570 2d62 6f6c  yntax-markup-bol
-00033820: 643a 7661 7228 2d2d 7379 6e74 6178 2d64  d:var(--syntax-d
-00033830: 6172 6b2d 6d61 726b 7570 2d62 6f6c 6429  ark-markup-bold)
-00033840: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00033850: 2d64 656c 6574 6564 2d74 6578 743a 7661  -deleted-text:va
-00033860: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-00033870: 6d61 726b 7570 2d64 656c 6574 6564 2d74  markup-deleted-t
-00033880: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033890: 726b 7570 2d64 656c 6574 6564 2d62 673a  rkup-deleted-bg:
-000338a0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-000338b0: 6b2d 6d61 726b 7570 2d64 656c 6574 6564  k-markup-deleted
-000338c0: 2d62 6729 3b2d 2d73 796e 7461 782d 6d61  -bg);--syntax-ma
-000338d0: 726b 7570 2d69 6e73 6572 7465 642d 7465  rkup-inserted-te
-000338e0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-000338f0: 6461 726b 2d6d 6172 6b75 702d 696e 7365  dark-markup-inse
-00033900: 7274 6564 2d74 6578 7429 3b2d 2d73 796e  rted-text);--syn
-00033910: 7461 782d 6d61 726b 7570 2d69 6e73 6572  tax-markup-inser
-00033920: 7465 642d 6267 3a76 6172 282d 2d73 796e  ted-bg:var(--syn
-00033930: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
-00033940: 696e 7365 7274 6564 2d62 6729 3b2d 2d73  inserted-bg);--s
-00033950: 796e 7461 782d 6d61 726b 7570 2d63 6861  yntax-markup-cha
-00033960: 6e67 6564 2d74 6578 743a 7661 7228 2d2d  nged-text:var(--
-00033970: 7379 6e74 6178 2d64 6172 6b2d 6d61 726b  syntax-dark-mark
-00033980: 7570 2d63 6861 6e67 6564 2d74 6578 7429  up-changed-text)
-00033990: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-000339a0: 2d63 6861 6e67 6564 2d62 673a 7661 7228  -changed-bg:var(
-000339b0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-000339c0: 726b 7570 2d63 6861 6e67 6564 2d62 6729  rkup-changed-bg)
-000339d0: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-000339e0: 2d69 676e 6f72 6564 2d74 6578 743a 7661  -ignored-text:va
-000339f0: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-00033a00: 6d61 726b 7570 2d69 676e 6f72 6564 2d74  markup-ignored-t
-00033a10: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
-00033a20: 726b 7570 2d69 676e 6f72 6564 2d62 673a  rkup-ignored-bg:
-00033a30: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033a40: 6b2d 6d61 726b 7570 2d69 676e 6f72 6564  k-markup-ignored
-00033a50: 2d62 6729 3b2d 2d73 796e 7461 782d 6d65  -bg);--syntax-me
-00033a60: 7461 2d64 6966 662d 7261 6e67 653a 7661  ta-diff-range:va
-00033a70: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-00033a80: 6d65 7461 2d64 6966 662d 7261 6e67 6529  meta-diff-range)
-00033a90: 3b2d 2d73 796e 7461 782d 7370 6563 6961  ;--syntax-specia
-00033aa0: 6c2d 6267 3a76 6172 282d 2d73 796e 7461  l-bg:var(--synta
-00033ab0: 782d 6461 726b 2d73 7065 6369 616c 2d62  x-dark-special-b
-00033ac0: 6729 7d7d 6874 6d6c 2e64 6172 6b7b 2d2d  g)}}html.dark{--
-00033ad0: 7379 6e74 6178 2d74 6578 743a 7661 7228  syntax-text:var(
-00033ae0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 7465  --syntax-dark-te
-00033af0: 7874 293b 2d2d 7379 6e74 6178 2d6d 6574  xt);--syntax-met
-00033b00: 613a 7661 7228 2d2d 7379 6e74 6178 2d64  a:var(--syntax-d
-00033b10: 6172 6b2d 6d65 7461 293b 2d2d 7379 6e74  ark-meta);--synt
-00033b20: 6178 2d63 6f6d 6d65 6e74 3a76 6172 282d  ax-comment:var(-
-00033b30: 2d73 796e 7461 782d 6461 726b 2d63 6f6d  -syntax-dark-com
-00033b40: 6d65 6e74 293b 2d2d 7379 6e74 6178 2d63  ment);--syntax-c
-00033b50: 6f6e 7374 616e 743a 7661 7228 2d2d 7379  onstant:var(--sy
-00033b60: 6e74 6178 2d64 6172 6b2d 636f 6e73 7461  ntax-dark-consta
-00033b70: 6e74 293b 2d2d 7379 6e74 6178 2d65 6e74  nt);--syntax-ent
-00033b80: 6974 793a 7661 7228 2d2d 7379 6e74 6178  ity:var(--syntax
-00033b90: 2d64 6172 6b2d 656e 7469 7479 293b 2d2d  -dark-entity);--
-00033ba0: 7379 6e74 6178 2d70 726f 7065 7274 793a  syntax-property:
+0002ecd0: 6e68 6572 6974 7d2e 7975 6520 6835 2c2e  nherit}.yue h5,.
+0002ece0: 7975 6520 6836 7b63 6f6c 6f72 3a76 6172  yue h6{color:var
+0002ecf0: 282d 2d79 7565 2d63 2d68 6561 6469 6e67  (--yue-c-heading
+0002ed00: 293b 666f 6e74 2d77 6569 6768 743a 3630  );font-weight:60
+0002ed10: 307d 2e79 7565 2069 6d67 7b64 6973 706c  0}.yue img{displ
+0002ed20: 6179 3a69 6e6c 696e 653b 6d61 7267 696e  ay:inline;margin
+0002ed30: 2d74 6f70 3a32 656d 3b6d 6172 6769 6e2d  -top:2em;margin-
+0002ed40: 626f 7474 6f6d 3a32 656d 7d2e 7975 6520  bottom:2em}.yue 
+0002ed50: 696d 672e 726f 756e 6465 647b 626f 7264  img.rounded{bord
+0002ed60: 6572 2d72 6164 6975 733a 2e35 7265 6d7d  er-radius:.5rem}
+0002ed70: 2e79 7565 2061 3e69 6d67 2c2e 7975 6520  .yue a>img,.yue 
+0002ed80: 6669 6775 7265 2069 6d67 2c2e 7975 6520  figure img,.yue 
+0002ed90: 6669 6775 7265 3e2a 7b6d 6172 6769 6e2d  figure>*{margin-
+0002eda0: 746f 703a 303b 6d61 7267 696e 2d62 6f74  top:0;margin-bot
+0002edb0: 746f 6d3a 307d 2e79 7565 2066 6967 6361  tom:0}.yue figca
+0002edc0: 7074 696f 6e7b 636f 6c6f 723a 7661 7228  ption{color:var(
+0002edd0: 2d2d 7975 652d 632d 6361 7074 696f 6e29  --yue-c-caption)
+0002ede0: 3b66 6f6e 742d 7369 7a65 3a2e 3837 3565  ;font-size:.875e
+0002edf0: 6d3b 6c69 6e65 2d68 6569 6768 743a 312e  m;line-height:1.
+0002ee00: 3432 3835 3731 343b 6d61 7267 696e 2d74  4285714;margin-t
+0002ee10: 6f70 3a2e 3835 3731 3432 3965 6d7d 2e79  op:.8571429em}.y
+0002ee20: 7565 2066 6967 6361 7074 696f 6e3e 707b  ue figcaption>p{
+0002ee30: 6d61 7267 696e 2d74 6f70 3a30 7d2e 7975  margin-top:0}.yu
+0002ee40: 6520 636f 6465 7b63 6f6c 6f72 3a76 6172  e code{color:var
+0002ee50: 282d 2d79 7565 2d63 2d63 6f64 652d 7465  (--yue-c-code-te
+0002ee60: 7874 293b 666f 6e74 2d77 6569 6768 743a  xt);font-weight:
+0002ee70: 3630 303b 666f 6e74 2d73 697a 653a 2e38  600;font-size:.8
+0002ee80: 3735 656d 7d2e 7975 6520 6120 636f 6465  75em}.yue a code
+0002ee90: 2c2e 7975 6520 626c 6f63 6b71 756f 7465  ,.yue blockquote
+0002eea0: 2063 6f64 652c 2e79 7565 2068 3120 636f   code,.yue h1 co
+0002eeb0: 6465 2c2e 7975 6520 6832 2063 6f64 652c  de,.yue h2 code,
+0002eec0: 2e79 7565 2068 3320 636f 6465 2c2e 7975  .yue h3 code,.yu
+0002eed0: 6520 6834 2063 6f64 652c 2e79 7565 2074  e h4 code,.yue t
+0002eee0: 6820 636f 6465 7b63 6f6c 6f72 3a69 6e68  h code{color:inh
+0002eef0: 6572 6974 7d2e 7975 6520 6832 2063 6f64  erit}.yue h2 cod
+0002ef00: 657b 666f 6e74 2d73 697a 653a 2e38 3735  e{font-size:.875
+0002ef10: 656d 7d2e 7975 6520 6c69 3e63 6f64 652c  em}.yue li>code,
+0002ef20: 2e79 7565 2070 3e63 6f64 657b 7061 6464  .yue p>code{padd
+0002ef30: 696e 673a 3270 7820 3470 783b 626f 7264  ing:2px 4px;bord
+0002ef40: 6572 2d72 6164 6975 733a 3370 783b 666f  er-radius:3px;fo
+0002ef50: 6e74 2d77 6569 6768 743a 3530 303b 6261  nt-weight:500;ba
+0002ef60: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+0002ef70: 6172 282d 2d79 7565 2d63 2d63 6f64 652d  ar(--yue-c-code-
+0002ef80: 6261 636b 6772 6f75 6e64 297d 2e79 7565  background)}.yue
+0002ef90: 2068 3320 636f 6465 7b66 6f6e 742d 7369   h3 code{font-si
+0002efa0: 7a65 3a2e 3965 6d7d 2e79 7565 206b 6264  ze:.9em}.yue kbd
+0002efb0: 7b66 6f6e 742d 6661 6d69 6c79 3a76 6172  {font-family:var
+0002efc0: 282d 2d73 792d 662d 6d6f 6e6f 297d 2e79  (--sy-f-mono)}.y
+0002efd0: 7565 2066 6967 7572 652c 2e79 7565 2076  ue figure,.yue v
+0002efe0: 6964 656f 7b6d 6172 6769 6e2d 746f 703a  ideo{margin-top:
+0002eff0: 3265 6d3b 6d61 7267 696e 2d62 6f74 746f  2em;margin-botto
+0002f000: 6d3a 3265 6d7d 2e79 7565 206c 697b 6d61  m:2em}.yue li{ma
+0002f010: 7267 696e 2d74 6f70 3a2e 3565 6d3b 6d61  rgin-top:.5em;ma
+0002f020: 7267 696e 2d62 6f74 746f 6d3a 2e35 656d  rgin-bottom:.5em
+0002f030: 7d2e 7975 6520 6f6c 3e6c 692c 2e79 7565  }.yue ol>li,.yue
+0002f040: 2075 6c3e 6c69 7b70 6164 6469 6e67 2d6c   ul>li{padding-l
+0002f050: 6566 743a 2e33 3735 656d 7d2e 7975 6520  eft:.375em}.yue 
+0002f060: 6f6c 206f 6c2c 2e79 7565 206f 6c20 756c  ol ol,.yue ol ul
+0002f070: 2c2e 7975 6520 756c 206f 6c2c 2e79 7565  ,.yue ul ol,.yue
+0002f080: 2075 6c20 756c 7b6d 6172 6769 6e2d 746f   ul ul{margin-to
+0002f090: 703a 2e37 3565 6d3b 6d61 7267 696e 2d62  p:.75em;margin-b
+0002f0a0: 6f74 746f 6d3a 2e37 3565 6d7d 2e79 7565  ottom:.75em}.yue
+0002f0b0: 2068 322b 2a2c 2e79 7565 2068 332b 2a2c   h2+*,.yue h3+*,
+0002f0c0: 2e79 7565 2068 342b 2a2c 2e79 7565 2068  .yue h4+*,.yue h
+0002f0d0: 722b 2a7b 6d61 7267 696e 2d74 6f70 3a30  r+*{margin-top:0
+0002f0e0: 7d2e 7975 6520 7461 626c 657b 7769 6474  }.yue table{widt
+0002f0f0: 683a 3130 3025 3b74 6162 6c65 2d6c 6179  h:100%;table-lay
+0002f100: 6f75 743a 6175 746f 3b74 6578 742d 616c  out:auto;text-al
+0002f110: 6967 6e3a 6c65 6674 3b6d 6172 6769 6e2d  ign:left;margin-
+0002f120: 746f 703a 3265 6d3b 6d61 7267 696e 2d62  top:2em;margin-b
+0002f130: 6f74 746f 6d3a 3265 6d3b 666f 6e74 2d73  ottom:2em;font-s
+0002f140: 697a 653a 2e38 3665 6d3b 6c69 6e65 2d68  ize:.86em;line-h
+0002f150: 6569 6768 743a 312e 377d 2e79 7565 2074  eight:1.7}.yue t
+0002f160: 6162 6c65 3e63 6170 7469 6f6e 7b6d 6172  able>caption{mar
+0002f170: 6769 6e2d 626f 7474 6f6d 3a2e 3472 656d  gin-bottom:.4rem
+0002f180: 3b63 6f6c 6f72 3a76 6172 282d 2d79 7565  ;color:var(--yue
+0002f190: 2d63 2d63 6170 7469 6f6e 297d 2e79 7565  -c-caption)}.yue
+0002f1a0: 2074 6865 6164 2074 727b 626f 7264 6572   thead tr{border
+0002f1b0: 2d62 6f74 746f 6d2d 7769 6474 683a 3170  -bottom-width:1p
+0002f1c0: 783b 626f 7264 6572 2d62 6f74 746f 6d2d  x;border-bottom-
+0002f1d0: 636f 6c6f 723a 7661 7228 2d2d 7975 652d  color:var(--yue-
+0002f1e0: 632d 7468 2d62 6f72 6465 7229 7d2e 7975  c-th-border)}.yu
+0002f1f0: 6520 7468 6561 6420 7468 7b63 6f6c 6f72  e thead th{color
+0002f200: 3a76 6172 282d 2d79 7565 2d63 2d68 6561  :var(--yue-c-hea
+0002f210: 6469 6e67 293b 666f 6e74 2d77 6569 6768  ding);font-weigh
+0002f220: 743a 3630 303b 7665 7274 6963 616c 2d61  t:600;vertical-a
+0002f230: 6c69 676e 3a6d 6964 646c 657d 2e79 7565  lign:middle}.yue
+0002f240: 2074 626f 6479 2074 727b 626f 7264 6572   tbody tr{border
+0002f250: 2d62 6f74 746f 6d2d 7769 6474 683a 3170  -bottom-width:1p
+0002f260: 783b 626f 7264 6572 2d62 6f74 746f 6d2d  x;border-bottom-
+0002f270: 636f 6c6f 723a 7661 7228 2d2d 7975 652d  color:var(--yue-
+0002f280: 632d 7464 2d62 6f72 6465 7229 7d2e 7975  c-td-border)}.yu
+0002f290: 6520 7462 6f64 7920 7472 3a6c 6173 742d  e tbody tr:last-
+0002f2a0: 6368 696c 647b 626f 7264 6572 2d62 6f74  child{border-bot
+0002f2b0: 746f 6d2d 7769 6474 683a 307d 2e79 7565  tom-width:0}.yue
+0002f2c0: 2074 626f 6479 2074 647b 7665 7274 6963   tbody td{vertic
+0002f2d0: 616c 2d61 6c69 676e 3a6d 6964 646c 657d  al-align:middle}
+0002f2e0: 2e79 7565 2074 666f 6f74 7b62 6f72 6465  .yue tfoot{borde
+0002f2f0: 722d 746f 702d 7769 6474 683a 3170 783b  r-top-width:1px;
+0002f300: 626f 7264 6572 2d74 6f70 2d63 6f6c 6f72  border-top-color
+0002f310: 3a76 6172 282d 2d79 7565 2d63 2d74 682d  :var(--yue-c-th-
+0002f320: 626f 7264 6572 297d 2e79 7565 2074 666f  border)}.yue tfo
+0002f330: 6f74 2074 647b 7665 7274 6963 616c 2d61  ot td{vertical-a
+0002f340: 6c69 676e 3a74 6f70 7d2e 7975 6520 7464  lign:top}.yue td
+0002f350: 3e70 7b6d 6172 6769 6e3a 2e32 3572 656d  >p{margin:.25rem
+0002f360: 2030 7d2e 7975 6520 7468 6561 6420 7468   0}.yue thead th
+0002f370: 3e70 7b6d 6172 6769 6e3a 307d 2e79 7565  >p{margin:0}.yue
+0002f380: 2074 626f 6479 2074 642c 2e79 7565 2074   tbody td,.yue t
+0002f390: 666f 6f74 2074 642c 2e79 7565 2074 6865  foot td,.yue the
+0002f3a0: 6164 2074 687b 7061 6464 696e 673a 2e35  ad th{padding:.5
+0002f3b0: 7265 6d7d 2e79 7565 2073 6563 7469 6f6e  rem}.yue section
+0002f3c0: 7b63 6c65 6172 3a62 6f74 687d 2e79 7565  {clear:both}.yue
+0002f3d0: 2073 6563 7469 6f6e 3e64 6976 7b6d 6172   section>div{mar
+0002f3e0: 6769 6e2d 626f 7474 6f6d 3a32 7265 6d7d  gin-bottom:2rem}
+0002f3f0: 2e79 7565 2064 643e 703a 6669 7273 742d  .yue dd>p:first-
+0002f400: 6368 696c 647b 6d61 7267 696e 2d74 6f70  child{margin-top
+0002f410: 3a30 7d2e 7975 6520 702e 6c65 6164 7b66  :0}.yue p.lead{f
+0002f420: 6f6e 742d 7369 7a65 3a31 2e32 7265 6d3b  ont-size:1.2rem;
+0002f430: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
+0002f440: 2d6c 6967 6874 293b 6d61 7267 696e 2d62  -light);margin-b
+0002f450: 6f74 746f 6d3a 307d 2e79 7565 2070 2e6c  ottom:0}.yue p.l
+0002f460: 6561 642b 6872 7b6d 6172 6769 6e2d 746f  ead+hr{margin-to
+0002f470: 703a 3172 656d 7d2e 7975 6520 702e 7275  p:1rem}.yue p.ru
+0002f480: 6272 6963 7b63 6f6c 6f72 3a76 6172 282d  bric{color:var(-
+0002f490: 2d79 7565 2d63 2d68 6561 6469 6e67 293b  -yue-c-heading);
+0002f4a0: 666f 6e74 2d77 6569 6768 743a 3630 303b  font-weight:600;
+0002f4b0: 6d61 7267 696e 2d74 6f70 3a32 7265 6d7d  margin-top:2rem}
+0002f4c0: 2e79 7565 202e 7369 6465 6261 727b 6261  .yue .sidebar{ba
+0002f4d0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+0002f4e0: 6172 282d 2d73 792d 632d 7375 7266 6163  ar(--sy-c-surfac
+0002f4f0: 6529 3b62 6f72 6465 723a 3170 7820 736f  e);border:1px so
+0002f500: 6c69 6420 7661 7228 2d2d 7379 2d63 2d62  lid var(--sy-c-b
+0002f510: 6f72 6465 7229 3b62 6f72 6465 722d 7261  order);border-ra
+0002f520: 6469 7573 3a36 7078 3b63 6c65 6172 3a72  dius:6px;clear:r
+0002f530: 6967 6874 3b66 6c6f 6174 3a72 6967 6874  ight;float:right
+0002f540: 3b6d 6172 6769 6e2d 6c65 6674 3a31 7265  ;margin-left:1re
+0002f550: 6d3b 6d61 7267 696e 2d62 6f74 746f 6d3a  m;margin-bottom:
+0002f560: 3172 656d 3b6d 6172 6769 6e2d 7269 6768  1rem;margin-righ
+0002f570: 743a 303b 7769 6474 683a 3330 257d 2e79  t:0;width:30%}.y
+0002f580: 7565 202e 7369 6465 6261 723e 2a7b 7061  ue .sidebar>*{pa
+0002f590: 6464 696e 672d 6c65 6674 3a31 7265 6d3b  dding-left:1rem;
+0002f5a0: 7061 6464 696e 672d 7269 6768 743a 3172  padding-right:1r
+0002f5b0: 656d 7d2e 7975 6520 2e73 6964 6562 6172  em}.yue .sidebar
+0002f5c0: 2069 6d67 7b6d 6172 6769 6e2d 746f 703a   img{margin-top:
+0002f5d0: 3172 656d 3b6d 6172 6769 6e2d 626f 7474  1rem;margin-bott
+0002f5e0: 6f6d 3a31 7265 6d7d 2e79 7565 202e 7369  om:1rem}.yue .si
+0002f5f0: 6465 6261 722d 7469 746c 657b 666f 6e74  debar-title{font
+0002f600: 2d77 6569 6768 743a 3530 303b 626f 7264  -weight:500;bord
+0002f610: 6572 2d62 6f74 746f 6d3a 3170 7820 736f  er-bottom:1px so
+0002f620: 6c69 6420 7661 7228 2d2d 7379 2d63 2d62  lid var(--sy-c-b
+0002f630: 6f72 6465 7229 3b6d 6172 6769 6e3a 303b  order);margin:0;
+0002f640: 7061 6464 696e 672d 746f 703a 2e35 7265  padding-top:.5re
+0002f650: 6d3b 7061 6464 696e 672d 626f 7474 6f6d  m;padding-bottom
+0002f660: 3a2e 3572 656d 7d2e 7975 6520 646c 2e73  :.5rem}.yue dl.s
+0002f670: 696d 706c 653e 6464 3e70 2c2e 7975 6520  imple>dd>p,.yue 
+0002f680: 6f6c 2e73 696d 706c 653e 6c69 3e70 2c2e  ol.simple>li>p,.
+0002f690: 7975 6520 756c 2e73 696d 706c 653e 6c69  yue ul.simple>li
+0002f6a0: 3e70 7b6d 6172 6769 6e3a 307d 2e79 7565  >p{margin:0}.yue
+0002f6b0: 2061 2e68 6561 6465 726c 696e 6b7b 7669   a.headerlink{vi
+0002f6c0: 7369 6269 6c69 7479 3a68 6964 6465 6e3b  sibility:hidden;
+0002f6d0: 6d61 7267 696e 2d6c 6566 743a 3670 783b  margin-left:6px;
+0002f6e0: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
+0002f6f0: 2d6c 6967 6874 293b 666f 6e74 2d77 6569  -light);font-wei
+0002f700: 6768 743a 3330 303b 666f 6e74 2d73 697a  ght:300;font-siz
+0002f710: 653a 3538 253b 666f 6e74 2d66 616d 696c  e:58%;font-famil
+0002f720: 793a 7661 7228 2d2d 7379 2d66 2d6d 6f6e  y:var(--sy-f-mon
+0002f730: 6f29 3b2d 2d69 636f 6e2d 7572 6c3a 7661  o);--icon-url:va
+0002f740: 7228 2d2d 6c75 6369 6465 2d6c 696e 6b2d  r(--lucide-link-
+0002f750: 7572 6c29 3b2d 7765 626b 6974 2d6d 6173  url);-webkit-mas
+0002f760: 6b3a 7661 7228 2d2d 6963 6f6e 2d75 726c  k:var(--icon-url
+0002f770: 2920 6e6f 2d72 6570 6561 743b 6d61 736b  ) no-repeat;mask
+0002f780: 3a76 6172 282d 2d69 636f 6e2d 7572 6c29  :var(--icon-url)
+0002f790: 206e 6f2d 7265 7065 6174 3b2d 7765 626b   no-repeat;-webk
+0002f7a0: 6974 2d6d 6173 6b2d 7369 7a65 3a31 3030  it-mask-size:100
+0002f7b0: 2520 3130 3025 3b6d 6173 6b2d 7369 7a65  % 100%;mask-size
+0002f7c0: 3a31 3030 2520 3130 3025 3b77 6964 7468  :100% 100%;width
+0002f7d0: 3a31 656d 3b68 6569 6768 743a 3165 6d3b  :1em;height:1em;
+0002f7e0: 6469 7370 6c61 793a 696e 6c69 6e65 2d62  display:inline-b
+0002f7f0: 6c6f 636b 3b76 6572 7469 6361 6c2d 616c  lock;vertical-al
+0002f800: 6967 6e3a 6d69 6464 6c65 3b66 6f6e 742d  ign:middle;font-
+0002f810: 7374 796c 653a 6e6f 726d 616c 3b62 6163  style:normal;bac
+0002f820: 6b67 726f 756e 642d 636f 6c6f 723a 6375  kground-color:cu
+0002f830: 7272 656e 7443 6f6c 6f72 7d2e 7975 6520  rrentColor}.yue 
+0002f840: 2e6d 6174 6820 612e 6865 6164 6572 6c69  .math a.headerli
+0002f850: 6e6b 2c68 313a 686f 7665 7220 612e 6865  nk,h1:hover a.he
+0002f860: 6164 6572 6c69 6e6b 2c68 323a 686f 7665  aderlink,h2:hove
+0002f870: 7220 612e 6865 6164 6572 6c69 6e6b 2c68  r a.headerlink,h
+0002f880: 333a 686f 7665 7220 612e 6865 6164 6572  3:hover a.header
+0002f890: 6c69 6e6b 2c68 343a 686f 7665 7220 612e  link,h4:hover a.
+0002f8a0: 6865 6164 6572 6c69 6e6b 2c68 353a 686f  headerlink,h5:ho
+0002f8b0: 7665 7220 612e 6865 6164 6572 6c69 6e6b  ver a.headerlink
+0002f8c0: 2c68 363a 686f 7665 7220 612e 6865 6164  ,h6:hover a.head
+0002f8d0: 6572 6c69 6e6b 7b76 6973 6962 696c 6974  erlink{visibilit
+0002f8e0: 793a 7669 7369 626c 657d 2e79 7565 202e  y:visible}.yue .
+0002f8f0: 746f 6374 7265 652d 7772 6170 7065 7220  toctree-wrapper 
+0002f900: 612c 2e79 7565 2061 2e69 6d61 6765 2d72  a,.yue a.image-r
+0002f910: 6566 6572 656e 6365 7b62 6f72 6465 722d  eference{border-
+0002f920: 626f 7474 6f6d 3a6e 6f6e 657d 2e79 7565  bottom:none}.yue
+0002f930: 202e 746f 6374 7265 652d 7772 6170 7065   .toctree-wrappe
+0002f940: 7220 702e 6361 7074 696f 6e7b 666f 6e74  r p.caption{font
+0002f950: 2d73 697a 653a 2e38 3672 656d 3b66 6f6e  -size:.86rem;fon
+0002f960: 742d 7765 6967 6874 3a35 3030 3b66 6f6e  t-weight:500;fon
+0002f970: 742d 6661 6d69 6c79 3a76 6172 282d 2d73  t-family:var(--s
+0002f980: 792d 662d 6865 6164 696e 6729 3b63 6f6c  y-f-heading);col
+0002f990: 6f72 3a76 6172 282d 2d73 792d 632d 6c69  or:var(--sy-c-li
+0002f9a0: 6768 7429 3b74 6578 742d 7472 616e 7366  ght);text-transf
+0002f9b0: 6f72 6d3a 7570 7065 7263 6173 653b 6c65  orm:uppercase;le
+0002f9c0: 7474 6572 2d73 7061 6369 6e67 3a2e 3470  tter-spacing:.4p
+0002f9d0: 783b 7061 6464 696e 673a 2e38 7265 6d20  x;padding:.8rem 
+0002f9e0: 3020 2e34 7265 6d3b 626f 7264 6572 2d62  0 .4rem;border-b
+0002f9f0: 6f74 746f 6d3a 3170 7820 736f 6c69 6420  ottom:1px solid 
+0002fa00: 7661 7228 2d2d 7379 2d63 2d64 6976 6964  var(--sy-c-divid
+0002fa10: 6572 297d 2e79 7565 202e 616c 6967 6e2d  er)}.yue .align-
+0002fa20: 6c65 6674 7b63 6c65 6172 3a6c 6566 743b  left{clear:left;
+0002fa30: 666c 6f61 743a 6c65 6674 3b6d 6172 6769  float:left;margi
+0002fa40: 6e3a 3020 3172 656d 2031 7265 6d7d 2e79  n:0 1rem 1rem}.y
+0002fa50: 7565 202e 616c 6967 6e2d 7269 6768 747b  ue .align-right{
+0002fa60: 636c 6561 723a 7269 6768 743b 666c 6f61  clear:right;floa
+0002fa70: 743a 7269 6768 743b 6d61 7267 696e 3a30  t:right;margin:0
+0002fa80: 2031 7265 6d20 3172 656d 7d2e 7975 6520   1rem 1rem}.yue 
+0002fa90: 2e61 6c69 676e 2d63 656e 7465 727b 6469  .align-center{di
+0002faa0: 7370 6c61 793a 626c 6f63 6b3b 7465 7874  splay:block;text
+0002fab0: 2d61 6c69 676e 3a63 656e 7465 727d 2e79  -align:center}.y
+0002fac0: 7565 202e 616c 6967 6e2d 6365 6e74 6572  ue .align-center
+0002fad0: 2c2e 7975 6520 6669 6775 7265 2e61 6c69  ,.yue figure.ali
+0002fae0: 676e 2d63 656e 7465 7220 696d 677b 6d61  gn-center img{ma
+0002faf0: 7267 696e 2d6c 6566 743a 6175 746f 3b6d  rgin-left:auto;m
+0002fb00: 6172 6769 6e2d 7269 6768 743a 6175 746f  argin-right:auto
+0002fb10: 7d61 2e66 6f6f 746e 6f74 652d 7265 6665  }a.footnote-refe
+0002fb20: 7265 6e63 657b 666f 6e74 2d73 697a 653a  rence{font-size:
+0002fb30: 2e36 3572 656d 3b76 6572 7469 6361 6c2d  .65rem;vertical-
+0002fb40: 616c 6967 6e3a 746f 707d 6173 6964 652e  align:top}aside.
+0002fb50: 666f 6f74 6e6f 7465 3e73 7061 6e2c 6469  footnote>span,di
+0002fb60: 762e 6369 7461 7469 6f6e 3e73 7061 6e7b  v.citation>span{
+0002fb70: 666c 6f61 743a 6c65 6674 3b66 6f6e 742d  float:left;font-
+0002fb80: 7765 6967 6874 3a35 3030 3b70 6164 6469  weight:500;paddi
+0002fb90: 6e67 2d72 6967 6874 3a2e 3235 7265 6d7d  ng-right:.25rem}
+0002fba0: 6173 6964 652e 666f 6f74 6e6f 7465 3e70  aside.footnote>p
+0002fbb0: 2c64 6976 2e63 6974 6174 696f 6e3e 707b  ,div.citation>p{
+0002fbc0: 6d61 7267 696e 2d62 6f74 746f 6d3a 2e35  margin-bottom:.5
+0002fbd0: 7265 6d3b 6d61 7267 696e 2d74 6f70 3a2e  rem;margin-top:.
+0002fbe0: 3572 656d 3b6d 6172 6769 6e2d 6c65 6674  5rem;margin-left
+0002fbf0: 3a32 7265 6d7d 2e79 7565 206b 6264 2e6b  :2rem}.yue kbd.k
+0002fc00: 6264 3a6e 6f74 282e 636f 6d70 6f75 6e64  bd:not(.compound
+0002fc10: 297b 666f 6e74 2d73 697a 653a 2e38 3672  ){font-size:.86r
+0002fc20: 656d 3b70 6164 6469 6e67 3a32 7078 2035  em;padding:2px 5
+0002fc30: 7078 3b62 6f72 6465 722d 7261 6469 7573  px;border-radius
+0002fc40: 3a33 7078 3b6d 6172 6769 6e2d 7269 6768  :3px;margin-righ
+0002fc50: 743a 2e32 3572 656d 7d2e 7975 6520 6b62  t:.25rem}.yue kb
+0002fc60: 642e 636f 6d70 6f75 6e64 3e6b 6264 7b6d  d.compound>kbd{m
+0002fc70: 6172 6769 6e2d 6c65 6674 3a2e 3235 7265  argin-left:.25re
+0002fc80: 6d7d 2e79 7565 202e 6d65 6e75 7365 6c65  m}.yue .menusele
+0002fc90: 6374 696f 6e7b 666f 6e74 2d77 6569 6768  ction{font-weigh
+0002fca0: 743a 3530 303b 666f 6e74 2d73 697a 653a  t:500;font-size:
+0002fcb0: 2e38 3672 656d 7d2e 6c69 6768 7420 2e73  .86rem}.light .s
+0002fcc0: 6561 7263 6862 6f78 206b 6264 2c2e 6c69  earchbox kbd,.li
+0002fcd0: 6768 7420 2e79 7565 206b 6264 2e6b 6264  ght .yue kbd.kbd
+0002fce0: 3a6e 6f74 282e 636f 6d70 6f75 6e64 297b  :not(.compound){
+0002fcf0: 626f 7264 6572 3a30 3b62 6163 6b67 726f  border:0;backgro
+0002fd00: 756e 643a 6c69 6e65 6172 2d67 7261 6469  und:linear-gradi
+0002fd10: 656e 7428 2d32 3235 6465 672c 2365 3665  ent(-225deg,#e6e
+0002fd20: 3665 362c 2366 3866 3866 3829 3b62 6f78  6e6,#f8f8f8);box
+0002fd30: 2d73 6861 646f 773a 696e 7365 7420 3020  -shadow:inset 0 
+0002fd40: 2d32 7078 2023 6462 6462 6462 2c69 6e73  -2px #dbdbdb,ins
+0002fd50: 6574 2030 2030 2031 7078 2031 7078 2023  et 0 0 1px 1px #
+0002fd60: 6666 662c 3020 3170 7820 3270 7820 3170  fff,0 1px 2px 1p
+0002fd70: 7820 2335 3035 3035 3036 367d 2e64 6172  x #50505066}.dar
+0002fd80: 6b20 2e73 6561 7263 6862 6f78 206b 6264  k .searchbox kbd
+0002fd90: 2c2e 6461 726b 202e 7975 6520 6b62 642e  ,.dark .yue kbd.
+0002fda0: 6b62 643a 6e6f 7428 2e63 6f6d 706f 756e  kbd:not(.compoun
+0002fdb0: 6429 7b62 6f72 6465 723a 303b 6261 636b  d){border:0;back
+0002fdc0: 6772 6f75 6e64 3a6c 696e 6561 722d 6772  ground:linear-gr
+0002fdd0: 6164 6965 6e74 282d 3232 3564 6567 2c23  adient(-225deg,#
+0002fde0: 3335 3334 3334 2c23 3134 3134 3134 293b  353434,#141414);
+0002fdf0: 626f 782d 7368 6164 6f77 3a69 6e73 6574  box-shadow:inset
+0002fe00: 2030 202d 3270 7820 2333 3733 3733 372c   0 -2px #373737,
+0002fe10: 696e 7365 7420 3020 3020 3170 7820 3170  inset 0 0 1px 1p
+0002fe20: 7820 2332 3232 2c30 2031 7078 2032 7078  x #222,0 1px 2px
+0002fe30: 2031 7078 2023 3030 307d 2e79 7565 2070   1px #000}.yue p
+0002fe40: 2e63 656e 7465 7265 647b 7465 7874 2d61  .centered{text-a
+0002fe50: 6c69 676e 3a63 656e 7465 727d 2e68 6c69  lign:center}.hli
+0002fe60: 7374 2074 647b 7665 7274 6963 616c 2d61  st td{vertical-a
+0002fe70: 6c69 676e 3a74 6f70 7d2e 6461 726b 202e  lign:top}.dark .
+0002fe80: 6461 726b 2d68 6964 6465 6e2c 2e64 6172  dark-hidden,.dar
+0002fe90: 6b20 2e6c 6967 6874 2d6f 6e6c 792c 2e6c  k .light-only,.l
+0002fea0: 6967 6874 202e 6461 726b 2d6f 6e6c 792c  ight .dark-only,
+0002feb0: 2e6c 6967 6874 202e 6c69 6768 742d 6869  .light .light-hi
+0002fec0: 6464 656e 7b64 6973 706c 6179 3a6e 6f6e  dden{display:non
+0002fed0: 657d 2e79 7565 202e 6765 6e69 6e64 6578  e}.yue .genindex
+0002fee0: 2d6a 756d 7062 6f78 2c2e 7975 6520 2e6d  -jumpbox,.yue .m
+0002fef0: 6f64 696e 6465 782d 6a75 6d70 626f 787b  odindex-jumpbox{
+0002ff00: 626f 7264 6572 2d74 6f70 3a31 7078 2073  border-top:1px s
+0002ff10: 6f6c 6964 2076 6172 282d 2d73 792d 632d  olid var(--sy-c-
+0002ff20: 626f 7264 6572 293b 626f 7264 6572 2d62  border);border-b
+0002ff30: 6f74 746f 6d3a 3170 7820 736f 6c69 6420  ottom:1px solid 
+0002ff40: 7661 7228 2d2d 7379 2d63 2d62 6f72 6465  var(--sy-c-borde
+0002ff50: 7229 3b70 6164 6469 6e67 3a32 7078 202e  r);padding:2px .
+0002ff60: 3472 656d 7d2e 7975 6520 7461 626c 652e  4rem}.yue table.
+0002ff70: 6d6f 6469 6e64 6578 7461 626c 6520 7464  modindextable td
+0002ff80: 3a66 6972 7374 2d6f 662d 7479 7065 7b77  :first-of-type{w
+0002ff90: 6964 7468 3a32 3870 787d 2e79 7565 2074  idth:28px}.yue t
+0002ffa0: 6162 6c65 2e6d 6f64 696e 6465 7874 6162  able.modindextab
+0002ffb0: 6c65 2069 6d67 2e74 6f67 676c 6572 7b6d  le img.toggler{m
+0002ffc0: 6172 6769 6e3a 307d 2e79 7565 2074 6162  argin:0}.yue tab
+0002ffd0: 6c65 2e6d 6f64 696e 6465 7874 6162 6c65  le.modindextable
+0002ffe0: 2074 722e 6361 707b 666f 6e74 2d73 697a   tr.cap{font-siz
+0002fff0: 653a 312e 3132 7265 6d3b 6261 636b 6772  e:1.12rem;backgr
+00030000: 6f75 6e64 3a76 6172 282d 2d73 792d 632d  ound:var(--sy-c-
+00030010: 7375 7266 6163 6529 3b66 6f6e 742d 6661  surface);font-fa
+00030020: 6d69 6c79 3a76 6172 282d 2d73 792d 662d  mily:var(--sy-f-
+00030030: 6d6f 6e6f 297d 2e79 7565 2068 322b 7461  mono)}.yue h2+ta
+00030040: 626c 652e 696e 6465 7874 6162 6c65 2c2e  ble.indextable,.
+00030050: 7975 6520 7461 626c 652e 696e 6465 7874  yue table.indext
+00030060: 6162 6c65 2075 6c7b 6d61 7267 696e 2d74  able ul{margin-t
+00030070: 6f70 3a30 7d3a 726f 6f74 7b2d 2d61 7474  op:0}:root{--att
+00030080: 656e 7469 6f6e 2d69 636f 6e3a 7661 7228  ention-icon:var(
+00030090: 2d2d 6c75 6369 6465 2d61 6c65 7274 2d75  --lucide-alert-u
+000300a0: 726c 293b 2d2d 6174 7465 6e74 696f 6e2d  rl);--attention-
+000300b0: 313a 7661 7228 2d2d 6372 696d 736f 6e2d  1:var(--crimson-
+000300c0: 7375 7266 6163 6529 3b2d 2d61 7474 656e  surface);--atten
+000300d0: 7469 6f6e 2d32 3a76 6172 282d 2d63 7269  tion-2:var(--cri
+000300e0: 6d73 6f6e 2d61 3329 3b2d 2d61 7474 656e  mson-a3);--atten
+000300f0: 7469 6f6e 2d33 3a76 6172 282d 2d63 7269  tion-3:var(--cri
+00030100: 6d73 6f6e 2d39 293b 2d2d 6174 7465 6e74  mson-9);--attent
+00030110: 696f 6e2d 343a 7661 7228 2d2d 6372 696d  ion-4:var(--crim
+00030120: 736f 6e2d 6131 3129 3b2d 2d63 6175 7469  son-a11);--cauti
+00030130: 6f6e 2d69 636f 6e3a 7661 7228 2d2d 6c75  on-icon:var(--lu
+00030140: 6369 6465 2d7a 6170 2d75 726c 293b 2d2d  cide-zap-url);--
+00030150: 6361 7574 696f 6e2d 313a 7661 7228 2d2d  caution-1:var(--
+00030160: 616d 6265 722d 7375 7266 6163 6529 3b2d  amber-surface);-
+00030170: 2d63 6175 7469 6f6e 2d32 3a76 6172 282d  -caution-2:var(-
+00030180: 2d61 6d62 6572 2d61 3329 3b2d 2d63 6175  -amber-a3);--cau
+00030190: 7469 6f6e 2d33 3a76 6172 282d 2d61 6d62  tion-3:var(--amb
+000301a0: 6572 2d39 293b 2d2d 6361 7574 696f 6e2d  er-9);--caution-
+000301b0: 343a 7661 7228 2d2d 616d 6265 722d 3131  4:var(--amber-11
+000301c0: 293b 2d2d 6461 6e67 6572 2d69 636f 6e3a  );--danger-icon:
+000301d0: 7661 7228 2d2d 6c75 6369 6465 2d73 6b75  var(--lucide-sku
+000301e0: 6c6c 2d75 726c 293b 2d2d 6461 6e67 6572  ll-url);--danger
+000301f0: 2d31 3a76 6172 282d 2d72 7562 792d 7375  -1:var(--ruby-su
+00030200: 7266 6163 6529 3b2d 2d64 616e 6765 722d  rface);--danger-
+00030210: 323a 7661 7228 2d2d 7275 6279 2d61 3329  2:var(--ruby-a3)
+00030220: 3b2d 2d64 616e 6765 722d 333a 7661 7228  ;--danger-3:var(
+00030230: 2d2d 7275 6279 2d39 293b 2d2d 6461 6e67  --ruby-9);--dang
+00030240: 6572 2d34 3a76 6172 282d 2d72 7562 792d  er-4:var(--ruby-
+00030250: 6131 3129 3b2d 2d65 7272 6f72 2d69 636f  a11);--error-ico
+00030260: 6e3a 7661 7228 2d2d 6c75 6369 6465 2d63  n:var(--lucide-c
+00030270: 6c6f 7365 2d75 726c 293b 2d2d 6572 726f  lose-url);--erro
+00030280: 722d 313a 7661 7228 2d2d 7265 642d 7375  r-1:var(--red-su
+00030290: 7266 6163 6529 3b2d 2d65 7272 6f72 2d32  rface);--error-2
+000302a0: 3a76 6172 282d 2d72 6564 2d61 3329 3b2d  :var(--red-a3);-
+000302b0: 2d65 7272 6f72 2d33 3a76 6172 282d 2d72  -error-3:var(--r
+000302c0: 6564 2d39 293b 2d2d 6572 726f 722d 343a  ed-9);--error-4:
+000302d0: 7661 7228 2d2d 7265 642d 6131 3129 3b2d  var(--red-a11);-
+000302e0: 2d68 696e 742d 6963 6f6e 3a76 6172 282d  -hint-icon:var(-
+000302f0: 2d6c 7563 6964 652d 6265 6c6c 2d75 726c  -lucide-bell-url
+00030300: 293b 2d2d 6869 6e74 2d31 3a76 6172 282d  );--hint-1:var(-
+00030310: 2d63 7961 6e2d 7375 7266 6163 6529 3b2d  -cyan-surface);-
+00030320: 2d68 696e 742d 323a 7661 7228 2d2d 6379  -hint-2:var(--cy
+00030330: 616e 2d61 3329 3b2d 2d68 696e 742d 333a  an-a3);--hint-3:
+00030340: 7661 7228 2d2d 6379 616e 2d39 293b 2d2d  var(--cyan-9);--
+00030350: 6869 6e74 2d34 3a76 6172 282d 2d63 7961  hint-4:var(--cya
+00030360: 6e2d 6131 3129 3b2d 2d69 6d70 6f72 7461  n-a11);--importa
+00030370: 6e74 2d69 636f 6e3a 7661 7228 2d2d 6c75  nt-icon:var(--lu
+00030380: 6369 6465 2d66 6c61 6d65 2d75 726c 293b  cide-flame-url);
+00030390: 2d2d 696d 706f 7274 616e 742d 313a 7661  --important-1:va
+000303a0: 7228 2d2d 7669 6f6c 6574 2d73 7572 6661  r(--violet-surfa
+000303b0: 6365 293b 2d2d 696d 706f 7274 616e 742d  ce);--important-
+000303c0: 323a 7661 7228 2d2d 7669 6f6c 6574 2d61  2:var(--violet-a
+000303d0: 3329 3b2d 2d69 6d70 6f72 7461 6e74 2d33  3);--important-3
+000303e0: 3a76 6172 282d 2d76 696f 6c65 742d 3929  :var(--violet-9)
+000303f0: 3b2d 2d69 6d70 6f72 7461 6e74 2d34 3a76  ;--important-4:v
+00030400: 6172 282d 2d76 696f 6c65 742d 6131 3129  ar(--violet-a11)
+00030410: 3b2d 2d6e 6f74 652d 6963 6f6e 3a76 6172  ;--note-icon:var
+00030420: 282d 2d6c 7563 6964 652d 6361 6c65 6e64  (--lucide-calend
+00030430: 6172 2d75 726c 293b 2d2d 6e6f 7465 2d31  ar-url);--note-1
+00030440: 3a76 6172 282d 2d62 6c75 652d 7375 7266  :var(--blue-surf
+00030450: 6163 6529 3b2d 2d6e 6f74 652d 323a 7661  ace);--note-2:va
+00030460: 7228 2d2d 626c 7565 2d61 3329 3b2d 2d6e  r(--blue-a3);--n
+00030470: 6f74 652d 333a 7661 7228 2d2d 626c 7565  ote-3:var(--blue
+00030480: 2d39 293b 2d2d 6e6f 7465 2d34 3a76 6172  -9);--note-4:var
+00030490: 282d 2d62 6c75 652d 6131 3129 3b2d 2d74  (--blue-a11);--t
+000304a0: 6970 2d69 636f 6e3a 7661 7228 2d2d 6c75  ip-icon:var(--lu
+000304b0: 6369 6465 2d72 6f63 6b65 742d 7572 6c29  cide-rocket-url)
+000304c0: 3b2d 2d74 6970 2d31 3a76 6172 282d 2d67  ;--tip-1:var(--g
+000304d0: 7265 656e 2d73 7572 6661 6365 293b 2d2d  reen-surface);--
+000304e0: 7469 702d 323a 7661 7228 2d2d 6772 6565  tip-2:var(--gree
+000304f0: 6e2d 6133 293b 2d2d 7469 702d 333a 7661  n-a3);--tip-3:va
+00030500: 7228 2d2d 6772 6565 6e2d 3929 3b2d 2d74  r(--green-9);--t
+00030510: 6970 2d34 3a76 6172 282d 2d67 7265 656e  ip-4:var(--green
+00030520: 2d61 3131 293b 2d2d 7761 726e 696e 672d  -a11);--warning-
+00030530: 6963 6f6e 3a76 6172 282d 2d6c 7563 6964  icon:var(--lucid
+00030540: 652d 7a61 702d 7572 6c29 3b2d 2d77 6172  e-zap-url);--war
+00030550: 6e69 6e67 2d31 3a76 6172 282d 2d6f 7261  ning-1:var(--ora
+00030560: 6e67 652d 7375 7266 6163 6529 3b2d 2d77  nge-surface);--w
+00030570: 6172 6e69 6e67 2d32 3a76 6172 282d 2d6f  arning-2:var(--o
+00030580: 7261 6e67 652d 6133 293b 2d2d 7761 726e  range-a3);--warn
+00030590: 696e 672d 333a 7661 7228 2d2d 6f72 616e  ing-3:var(--oran
+000305a0: 6765 2d39 293b 2d2d 7761 726e 696e 672d  ge-9);--warning-
+000305b0: 343a 7661 7228 2d2d 6f72 616e 6765 2d61  4:var(--orange-a
+000305c0: 3131 293b 2d2d 7365 6561 6c73 6f2d 6963  11);--seealso-ic
+000305d0: 6f6e 3a76 6172 282d 2d6c 7563 6964 652d  on:var(--lucide-
+000305e0: 6c69 6e6b 2d75 726c 293b 2d2d 7365 6561  link-url);--seea
+000305f0: 6c73 6f2d 313a 7661 7228 2d2d 676f 6c64  lso-1:var(--gold
+00030600: 2d73 7572 6661 6365 293b 2d2d 7365 6561  -surface);--seea
+00030610: 6c73 6f2d 323a 7661 7228 2d2d 676f 6c64  lso-2:var(--gold
+00030620: 2d61 3329 3b2d 2d73 6565 616c 736f 2d33  -a3);--seealso-3
+00030630: 3a76 6172 282d 2d67 6f6c 642d 3929 3b2d  :var(--gold-9);-
+00030640: 2d73 6565 616c 736f 2d34 3a76 6172 282d  -seealso-4:var(-
+00030650: 2d67 6f6c 642d 6131 3129 3b2d 2d74 6f64  -gold-a11);--tod
+00030660: 6f2d 6963 6f6e 3a76 6172 282d 2d6c 7563  o-icon:var(--luc
+00030670: 6964 652d 626f 6f6b 6d61 726b 2d75 726c  ide-bookmark-url
+00030680: 293b 2d2d 746f 646f 2d31 3a76 6172 282d  );--todo-1:var(-
+00030690: 2d62 726f 6e7a 652d 7375 7266 6163 6529  -bronze-surface)
+000306a0: 3b2d 2d74 6f64 6f2d 323a 7661 7228 2d2d  ;--todo-2:var(--
+000306b0: 6272 6f6e 7a65 2d61 3329 3b2d 2d74 6f64  bronze-a3);--tod
+000306c0: 6f2d 333a 7661 7228 2d2d 6272 6f6e 7a65  o-3:var(--bronze
+000306d0: 2d39 293b 2d2d 746f 646f 2d34 3a76 6172  -9);--todo-4:var
+000306e0: 282d 2d62 726f 6e7a 652d 6131 3129 3b2d  (--bronze-a11);-
+000306f0: 2d76 6572 7369 6f6e 6164 6465 642d 313a  -versionadded-1:
+00030700: 7661 7228 2d2d 6772 6565 6e2d 7375 7266  var(--green-surf
+00030710: 6163 6529 3b2d 2d76 6572 7369 6f6e 6164  ace);--versionad
+00030720: 6465 642d 323a 7661 7228 2d2d 6772 6565  ded-2:var(--gree
+00030730: 6e2d 3929 3b2d 2d76 6572 7369 6f6e 6368  n-9);--versionch
+00030740: 616e 6765 642d 313a 7661 7228 2d2d 616d  anged-1:var(--am
+00030750: 6265 722d 7375 7266 6163 6529 3b2d 2d76  ber-surface);--v
+00030760: 6572 7369 6f6e 6368 616e 6765 642d 323a  ersionchanged-2:
+00030770: 7661 7228 2d2d 616d 6265 722d 3929 3b2d  var(--amber-9);-
+00030780: 2d64 6570 7265 6361 7465 642d 313a 7661  -deprecated-1:va
+00030790: 7228 2d2d 7265 642d 7375 7266 6163 6529  r(--red-surface)
+000307a0: 3b2d 2d64 6570 7265 6361 7465 642d 323a  ;--deprecated-2:
+000307b0: 7661 7228 2d2d 7265 642d 3929 7d2e 6164  var(--red-9)}.ad
+000307c0: 6d6f 6e69 7469 6f6e 7b2d 2d69 636f 6e2d  monition{--icon-
+000307d0: 7572 6c3a 7661 7228 2d2d 6c75 6369 6465  url:var(--lucide
+000307e0: 2d62 656c 6c2d 7572 6c29 3b2d 2d63 6f6c  -bell-url);--col
+000307f0: 6f72 2d31 3a76 6172 282d 2d63 6f6c 6f72  or-1:var(--color
+00030800: 2d73 7572 6661 6365 2d61 6363 656e 7429  -surface-accent)
+00030810: 3b2d 2d63 6f6c 6f72 2d32 3a76 6172 282d  ;--color-2:var(-
+00030820: 2d61 6363 656e 742d 6133 293b 2d2d 636f  -accent-a3);--co
+00030830: 6c6f 722d 333a 7661 7228 2d2d 6163 6365  lor-3:var(--acce
+00030840: 6e74 2d39 293b 2d2d 636f 6c6f 722d 343a  nt-9);--color-4:
+00030850: 7661 7228 2d2d 6163 6365 6e74 2d61 3131  var(--accent-a11
+00030860: 293b 706f 7369 7469 6f6e 3a72 656c 6174  );position:relat
+00030870: 6976 653b 7061 6464 696e 673a 3020 3136  ive;padding:0 16
+00030880: 7078 202e 3872 656d 3b6d 6172 6769 6e2d  px .8rem;margin-
+00030890: 746f 703a 3172 656d 3b6d 6172 6769 6e2d  top:1rem;margin-
+000308a0: 626f 7474 6f6d 3a31 7265 6d3b 626f 7264  bottom:1rem;bord
+000308b0: 6572 2d6c 6566 743a 3470 7820 736f 6c69  er-left:4px soli
+000308c0: 6420 7661 7228 2d2d 636f 6c6f 722d 3329  d var(--color-3)
+000308d0: 3b62 6163 6b67 726f 756e 642d 636f 6c6f  ;background-colo
+000308e0: 723a 7661 7228 2d2d 636f 6c6f 722d 3129  r:var(--color-1)
+000308f0: 7d2e 6164 6d6f 6e69 7469 6f6e 3a62 6566  }.admonition:bef
+00030900: 6f72 657b 706f 7369 7469 6f6e 3a61 6273  ore{position:abs
+00030910: 6f6c 7574 653b 636f 6e74 656e 743a 2222  olute;content:""
+00030920: 3b74 6f70 3a36 7078 3b6c 6566 743a 2d31  ;top:6px;left:-1
+00030930: 3270 783b 7769 6474 683a 3230 7078 3b68  2px;width:20px;h
+00030940: 6569 6768 743a 3230 7078 3b62 6f72 6465  eight:20px;borde
+00030950: 722d 7261 6469 7573 3a31 3030 253b 6261  r-radius:100%;ba
+00030960: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+00030970: 6172 282d 2d63 6f6c 6f72 2d33 297d 2e61  ar(--color-3)}.a
+00030980: 646d 6f6e 6974 696f 6e20 702e 6164 6d6f  dmonition p.admo
+00030990: 6e69 7469 6f6e 2d74 6974 6c65 7b70 6f73  nition-title{pos
+000309a0: 6974 696f 6e3a 7265 6c61 7469 7665 3b6d  ition:relative;m
+000309b0: 6172 6769 6e3a 3020 2d31 3670 7820 2e38  argin:0 -16px .8
+000309c0: 7265 6d20 2d31 3970 783b 7061 6464 696e  rem -19px;paddin
+000309d0: 673a 3470 7820 3138 7078 3b66 6f6e 742d  g:4px 18px;font-
+000309e0: 7369 7a65 3a2e 3835 7265 6d3b 666f 6e74  size:.85rem;font
+000309f0: 2d77 6569 6768 743a 3630 303b 6c69 6e65  -weight:600;line
+00030a00: 2d68 6569 6768 743a 312e 3732 3b63 6f6c  -height:1.72;col
+00030a10: 6f72 3a76 6172 282d 2d63 6f6c 6f72 2d34  or:var(--color-4
+00030a20: 293b 6261 636b 6772 6f75 6e64 2d63 6f6c  );background-col
+00030a30: 6f72 3a76 6172 282d 2d63 6f6c 6f72 2d32  or:var(--color-2
+00030a40: 293b 2d2d 7975 652d 632d 636f 6465 3a76  );--yue-c-code:v
+00030a50: 6172 282d 2d63 6f6c 6f72 2d34 293b 2d2d  ar(--color-4);--
+00030a60: 7975 652d 632d 626f 6c64 3a76 6172 282d  yue-c-bold:var(-
+00030a70: 2d63 6f6c 6f72 2d34 297d 2e61 646d 6f6e  -color-4)}.admon
+00030a80: 6974 696f 6e20 702e 6164 6d6f 6e69 7469  ition p.admoniti
+00030a90: 6f6e 2d74 6974 6c65 2073 7667 7b64 6973  on-title svg{dis
+00030aa0: 706c 6179 3a69 6e6c 696e 652d 626c 6f63  play:inline-bloc
+00030ab0: 6b7d 2e61 646d 6f6e 6974 696f 6e2d 7469  k}.admonition-ti
+00030ac0: 746c 653a 6265 666f 7265 7b70 6f73 6974  tle:before{posit
+00030ad0: 696f 6e3a 6162 736f 6c75 7465 3b63 6f6e  ion:absolute;con
+00030ae0: 7465 6e74 3a22 223b 746f 703a 3130 7078  tent:"";top:10px
+00030af0: 3b6c 6566 743a 2d35 7078 3b2d 7765 626b  ;left:-5px;-webk
+00030b00: 6974 2d6d 6173 6b3a 7661 7228 2d2d 6963  it-mask:var(--ic
+00030b10: 6f6e 2d75 726c 2920 6e6f 2d72 6570 6561  on-url) no-repea
+00030b20: 743b 6d61 736b 3a76 6172 282d 2d69 636f  t;mask:var(--ico
+00030b30: 6e2d 7572 6c29 206e 6f2d 7265 7065 6174  n-url) no-repeat
+00030b40: 3b2d 7765 626b 6974 2d6d 6173 6b2d 7369  ;-webkit-mask-si
+00030b50: 7a65 3a31 3030 2520 3130 3025 3b6d 6173  ze:100% 100%;mas
+00030b60: 6b2d 7369 7a65 3a31 3030 2520 3130 3025  k-size:100% 100%
+00030b70: 3b66 6f6e 742d 7374 796c 653a 6e6f 726d  ;font-style:norm
+00030b80: 616c 3b77 6964 7468 3a31 3270 783b 6865  al;width:12px;he
+00030b90: 6967 6874 3a31 3270 783b 6261 636b 6772  ight:12px;backgr
+00030ba0: 6f75 6e64 2d63 6f6c 6f72 3a23 6666 667d  ound-color:#fff}
+00030bb0: 2e61 646d 6f6e 6974 696f 6e2e 6174 7465  .admonition.atte
+00030bc0: 6e74 696f 6e7b 2d2d 6963 6f6e 2d75 726c  ntion{--icon-url
+00030bd0: 3a76 6172 282d 2d61 7474 656e 7469 6f6e  :var(--attention
+00030be0: 2d69 636f 6e29 3b2d 2d63 6f6c 6f72 2d31  -icon);--color-1
+00030bf0: 3a76 6172 282d 2d61 7474 656e 7469 6f6e  :var(--attention
+00030c00: 2d31 293b 2d2d 636f 6c6f 722d 323a 7661  -1);--color-2:va
+00030c10: 7228 2d2d 6174 7465 6e74 696f 6e2d 3229  r(--attention-2)
+00030c20: 3b2d 2d63 6f6c 6f72 2d33 3a76 6172 282d  ;--color-3:var(-
+00030c30: 2d61 7474 656e 7469 6f6e 2d33 293b 2d2d  -attention-3);--
+00030c40: 636f 6c6f 722d 343a 7661 7228 2d2d 6174  color-4:var(--at
+00030c50: 7465 6e74 696f 6e2d 3429 7d2e 6164 6d6f  tention-4)}.admo
+00030c60: 6e69 7469 6f6e 2e63 6175 7469 6f6e 7b2d  nition.caution{-
+00030c70: 2d69 636f 6e2d 7572 6c3a 7661 7228 2d2d  -icon-url:var(--
+00030c80: 6361 7574 696f 6e2d 6963 6f6e 293b 2d2d  caution-icon);--
+00030c90: 636f 6c6f 722d 313a 7661 7228 2d2d 6361  color-1:var(--ca
+00030ca0: 7574 696f 6e2d 3129 3b2d 2d63 6f6c 6f72  ution-1);--color
+00030cb0: 2d32 3a76 6172 282d 2d63 6175 7469 6f6e  -2:var(--caution
+00030cc0: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
+00030cd0: 7228 2d2d 6361 7574 696f 6e2d 3329 3b2d  r(--caution-3);-
+00030ce0: 2d63 6f6c 6f72 2d34 3a76 6172 282d 2d63  -color-4:var(--c
+00030cf0: 6175 7469 6f6e 2d34 297d 2e61 646d 6f6e  aution-4)}.admon
+00030d00: 6974 696f 6e2e 6461 6e67 6572 7b2d 2d69  ition.danger{--i
+00030d10: 636f 6e2d 7572 6c3a 7661 7228 2d2d 6461  con-url:var(--da
+00030d20: 6e67 6572 2d69 636f 6e29 3b2d 2d63 6f6c  nger-icon);--col
+00030d30: 6f72 2d31 3a76 6172 282d 2d64 616e 6765  or-1:var(--dange
+00030d40: 722d 3129 3b2d 2d63 6f6c 6f72 2d32 3a76  r-1);--color-2:v
+00030d50: 6172 282d 2d64 616e 6765 722d 3229 3b2d  ar(--danger-2);-
+00030d60: 2d63 6f6c 6f72 2d33 3a76 6172 282d 2d64  -color-3:var(--d
+00030d70: 616e 6765 722d 3329 3b2d 2d63 6f6c 6f72  anger-3);--color
+00030d80: 2d34 3a76 6172 282d 2d64 616e 6765 722d  -4:var(--danger-
+00030d90: 3429 7d2e 6164 6d6f 6e69 7469 6f6e 2e65  4)}.admonition.e
+00030da0: 7272 6f72 7b2d 2d69 636f 6e2d 7572 6c3a  rror{--icon-url:
+00030db0: 7661 7228 2d2d 6572 726f 722d 6963 6f6e  var(--error-icon
+00030dc0: 293b 2d2d 636f 6c6f 722d 313a 7661 7228  );--color-1:var(
+00030dd0: 2d2d 6572 726f 722d 3129 3b2d 2d63 6f6c  --error-1);--col
+00030de0: 6f72 2d32 3a76 6172 282d 2d65 7272 6f72  or-2:var(--error
+00030df0: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
+00030e00: 7228 2d2d 6572 726f 722d 3329 3b2d 2d63  r(--error-3);--c
+00030e10: 6f6c 6f72 2d34 3a76 6172 282d 2d65 7272  olor-4:var(--err
+00030e20: 6f72 2d34 297d 2e61 646d 6f6e 6974 696f  or-4)}.admonitio
+00030e30: 6e2e 6869 6e74 7b2d 2d69 636f 6e2d 7572  n.hint{--icon-ur
+00030e40: 6c3a 7661 7228 2d2d 6869 6e74 2d69 636f  l:var(--hint-ico
+00030e50: 6e29 3b2d 2d63 6f6c 6f72 2d31 3a76 6172  n);--color-1:var
+00030e60: 282d 2d68 696e 742d 3129 3b2d 2d63 6f6c  (--hint-1);--col
+00030e70: 6f72 2d32 3a76 6172 282d 2d68 696e 742d  or-2:var(--hint-
+00030e80: 3229 3b2d 2d63 6f6c 6f72 2d33 3a76 6172  2);--color-3:var
+00030e90: 282d 2d68 696e 742d 3329 3b2d 2d63 6f6c  (--hint-3);--col
+00030ea0: 6f72 2d34 3a76 6172 282d 2d68 696e 742d  or-4:var(--hint-
+00030eb0: 3429 7d2e 6164 6d6f 6e69 7469 6f6e 2e69  4)}.admonition.i
+00030ec0: 6d70 6f72 7461 6e74 7b2d 2d69 636f 6e2d  mportant{--icon-
+00030ed0: 7572 6c3a 7661 7228 2d2d 696d 706f 7274  url:var(--import
+00030ee0: 616e 742d 6963 6f6e 293b 2d2d 636f 6c6f  ant-icon);--colo
+00030ef0: 722d 313a 7661 7228 2d2d 696d 706f 7274  r-1:var(--import
+00030f00: 616e 742d 3129 3b2d 2d63 6f6c 6f72 2d32  ant-1);--color-2
+00030f10: 3a76 6172 282d 2d69 6d70 6f72 7461 6e74  :var(--important
+00030f20: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
+00030f30: 7228 2d2d 696d 706f 7274 616e 742d 3329  r(--important-3)
+00030f40: 3b2d 2d63 6f6c 6f72 2d34 3a76 6172 282d  ;--color-4:var(-
+00030f50: 2d69 6d70 6f72 7461 6e74 2d34 297d 2e61  -important-4)}.a
+00030f60: 646d 6f6e 6974 696f 6e2e 6e6f 7465 7b2d  dmonition.note{-
+00030f70: 2d69 636f 6e2d 7572 6c3a 7661 7228 2d2d  -icon-url:var(--
+00030f80: 6e6f 7465 2d69 636f 6e29 3b2d 2d63 6f6c  note-icon);--col
+00030f90: 6f72 2d31 3a76 6172 282d 2d6e 6f74 652d  or-1:var(--note-
+00030fa0: 3129 3b2d 2d63 6f6c 6f72 2d32 3a76 6172  1);--color-2:var
+00030fb0: 282d 2d6e 6f74 652d 3229 3b2d 2d63 6f6c  (--note-2);--col
+00030fc0: 6f72 2d33 3a76 6172 282d 2d6e 6f74 652d  or-3:var(--note-
+00030fd0: 3329 3b2d 2d63 6f6c 6f72 2d34 3a76 6172  3);--color-4:var
+00030fe0: 282d 2d6e 6f74 652d 3429 7d2e 6164 6d6f  (--note-4)}.admo
+00030ff0: 6e69 7469 6f6e 2e74 6970 7b2d 2d69 636f  nition.tip{--ico
+00031000: 6e2d 7572 6c3a 7661 7228 2d2d 7469 702d  n-url:var(--tip-
+00031010: 6963 6f6e 293b 2d2d 636f 6c6f 722d 313a  icon);--color-1:
+00031020: 7661 7228 2d2d 7469 702d 3129 3b2d 2d63  var(--tip-1);--c
+00031030: 6f6c 6f72 2d32 3a76 6172 282d 2d74 6970  olor-2:var(--tip
+00031040: 2d32 293b 2d2d 636f 6c6f 722d 333a 7661  -2);--color-3:va
+00031050: 7228 2d2d 7469 702d 3329 3b2d 2d63 6f6c  r(--tip-3);--col
+00031060: 6f72 2d34 3a76 6172 282d 2d74 6970 2d34  or-4:var(--tip-4
+00031070: 297d 2e61 646d 6f6e 6974 696f 6e2e 7761  )}.admonition.wa
+00031080: 726e 696e 677b 2d2d 6963 6f6e 2d75 726c  rning{--icon-url
+00031090: 3a76 6172 282d 2d77 6172 6e69 6e67 2d69  :var(--warning-i
+000310a0: 636f 6e29 3b2d 2d63 6f6c 6f72 2d31 3a76  con);--color-1:v
+000310b0: 6172 282d 2d77 6172 6e69 6e67 2d31 293b  ar(--warning-1);
+000310c0: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
+000310d0: 7761 726e 696e 672d 3229 3b2d 2d63 6f6c  warning-2);--col
+000310e0: 6f72 2d33 3a76 6172 282d 2d77 6172 6e69  or-3:var(--warni
+000310f0: 6e67 2d33 293b 2d2d 636f 6c6f 722d 343a  ng-3);--color-4:
+00031100: 7661 7228 2d2d 7761 726e 696e 672d 3429  var(--warning-4)
+00031110: 7d2e 6164 6d6f 6e69 7469 6f6e 2e73 6565  }.admonition.see
+00031120: 616c 736f 7b2d 2d69 636f 6e2d 7572 6c3a  also{--icon-url:
+00031130: 7661 7228 2d2d 7365 6561 6c73 6f2d 6963  var(--seealso-ic
+00031140: 6f6e 293b 2d2d 636f 6c6f 722d 313a 7661  on);--color-1:va
+00031150: 7228 2d2d 7365 6561 6c73 6f2d 3129 3b2d  r(--seealso-1);-
+00031160: 2d63 6f6c 6f72 2d32 3a76 6172 282d 2d73  -color-2:var(--s
+00031170: 6565 616c 736f 2d32 293b 2d2d 636f 6c6f  eealso-2);--colo
+00031180: 722d 333a 7661 7228 2d2d 7365 6561 6c73  r-3:var(--seeals
+00031190: 6f2d 3329 3b2d 2d63 6f6c 6f72 2d34 3a76  o-3);--color-4:v
+000311a0: 6172 282d 2d73 6565 616c 736f 2d34 297d  ar(--seealso-4)}
+000311b0: 2e61 646d 6f6e 6974 696f 6e2e 6164 6d6f  .admonition.admo
+000311c0: 6e69 7469 6f6e 2d74 6f64 6f7b 2d2d 6963  nition-todo{--ic
+000311d0: 6f6e 2d75 726c 3a76 6172 282d 2d74 6f64  on-url:var(--tod
+000311e0: 6f2d 6963 6f6e 293b 2d2d 636f 6c6f 722d  o-icon);--color-
+000311f0: 313a 7661 7228 2d2d 746f 646f 2d31 293b  1:var(--todo-1);
+00031200: 2d2d 636f 6c6f 722d 323a 7661 7228 2d2d  --color-2:var(--
+00031210: 746f 646f 2d32 293b 2d2d 636f 6c6f 722d  todo-2);--color-
+00031220: 333a 7661 7228 2d2d 746f 646f 2d33 293b  3:var(--todo-3);
+00031230: 2d2d 636f 6c6f 722d 343a 7661 7228 2d2d  --color-4:var(--
+00031240: 746f 646f 2d34 297d 2e61 646d 6f6e 6974  todo-4)}.admonit
+00031250: 696f 6e20 702e 6164 6d6f 6e69 7469 6f6e  ion p.admonition
+00031260: 2d74 6974 6c65 2b70 7b6d 6172 6769 6e2d  -title+p{margin-
+00031270: 746f 703a 307d 2e61 646d 6f6e 6974 696f  top:0}.admonitio
+00031280: 6e3e 3a6c 6173 742d 6368 696c 647b 6d61  n>:last-child{ma
+00031290: 7267 696e 2d62 6f74 746f 6d3a 307d 7370  rgin-bottom:0}sp
+000312a0: 616e 2e76 6572 7369 6f6e 6d6f 6469 6669  an.versionmodifi
+000312b0: 6564 7b63 6f6c 6f72 3a76 6172 282d 2d73  ed{color:var(--s
+000312c0: 792d 632d 626f 6c64 293b 666f 6e74 2d77  y-c-bold);font-w
+000312d0: 6569 6768 743a 3630 307d 6469 762e 6465  eight:600}div.de
+000312e0: 7072 6563 6174 6564 2c64 6976 2e76 6572  precated,div.ver
+000312f0: 7369 6f6e 6164 6465 642c 6469 762e 7665  sionadded,div.ve
+00031300: 7273 696f 6e63 6861 6e67 6564 7b70 6f73  rsionchanged{pos
+00031310: 6974 696f 6e3a 7265 6c61 7469 7665 3b70  ition:relative;p
+00031320: 6164 6469 6e67 3a36 7078 2031 7265 6d3b  adding:6px 1rem;
+00031330: 6d61 7267 696e 3a31 7265 6d20 303b 626f  margin:1rem 0;bo
+00031340: 7264 6572 2d6c 6566 743a 3470 7820 736f  rder-left:4px so
+00031350: 6c69 6420 7661 7228 2d2d 636f 6c6f 722d  lid var(--color-
+00031360: 3229 3b62 6163 6b67 726f 756e 642d 636f  2);background-co
+00031370: 6c6f 723a 7661 7228 2d2d 636f 6c6f 722d  lor:var(--color-
+00031380: 3129 3b6c 696e 652d 6865 6967 6874 3a31  1);line-height:1
+00031390: 2e37 327d 6469 762e 6465 7072 6563 6174  .72}div.deprecat
+000313a0: 6564 3a62 6566 6f72 652c 6469 762e 7665  ed:before,div.ve
+000313b0: 7273 696f 6e61 6464 6564 3a62 6566 6f72  rsionadded:befor
+000313c0: 652c 6469 762e 7665 7273 696f 6e63 6861  e,div.versioncha
+000313d0: 6e67 6564 3a62 6566 6f72 657b 706f 7369  nged:before{posi
+000313e0: 7469 6f6e 3a61 6273 6f6c 7574 653b 636f  tion:absolute;co
+000313f0: 6e74 656e 743a 7661 7228 2d2d 7665 7273  ntent:var(--vers
+00031400: 696f 6e2d 6963 6f6e 293b 746f 703a 3130  ion-icon);top:10
+00031410: 7078 3b6c 6566 743a 2d31 3270 783b 636f  px;left:-12px;co
+00031420: 6c6f 723a 2366 6666 3b77 6964 7468 3a32  lor:#fff;width:2
+00031430: 3070 783b 6865 6967 6874 3a32 3070 783b  0px;height:20px;
+00031440: 626f 7264 6572 2d72 6164 6975 733a 3130  border-radius:10
+00031450: 3025 3b62 6163 6b67 726f 756e 642d 636f  0%;background-co
+00031460: 6c6f 723a 7661 7228 2d2d 636f 6c6f 722d  lor:var(--color-
+00031470: 3229 3b74 6578 742d 616c 6967 6e3a 6365  2);text-align:ce
+00031480: 6e74 6572 3b66 6f6e 743a 6e6f 726d 616c  nter;font:normal
+00031490: 2037 3030 2031 3470 782f 3230 7078 2076   700 14px/20px v
+000314a0: 6172 282d 2d73 792d 662d 6d6f 6e6f 297d  ar(--sy-f-mono)}
+000314b0: 6469 762e 7665 7273 696f 6e61 6464 6564  div.versionadded
+000314c0: 7b2d 2d63 6f6c 6f72 2d31 3a76 6172 282d  {--color-1:var(-
+000314d0: 2d76 6572 7369 6f6e 6164 6465 642d 3129  -versionadded-1)
+000314e0: 3b2d 2d63 6f6c 6f72 2d32 3a76 6172 282d  ;--color-2:var(-
+000314f0: 2d76 6572 7369 6f6e 6164 6465 642d 3229  -versionadded-2)
+00031500: 3b2d 2d76 6572 7369 6f6e 2d69 636f 6e3a  ;--version-icon:
+00031510: 2223 227d 6469 762e 7665 7273 696f 6e63  "#"}div.versionc
+00031520: 6861 6e67 6564 7b2d 2d63 6f6c 6f72 2d31  hanged{--color-1
+00031530: 3a76 6172 282d 2d76 6572 7369 6f6e 6368  :var(--versionch
+00031540: 616e 6765 642d 3129 3b2d 2d63 6f6c 6f72  anged-1);--color
+00031550: 2d32 3a76 6172 282d 2d76 6572 7369 6f6e  -2:var(--version
+00031560: 6368 616e 6765 642d 3229 3b2d 2d76 6572  changed-2);--ver
+00031570: 7369 6f6e 2d69 636f 6e3a 2225 227d 6469  sion-icon:"%"}di
+00031580: 762e 6465 7072 6563 6174 6564 7b2d 2d63  v.deprecated{--c
+00031590: 6f6c 6f72 2d31 3a76 6172 282d 2d64 6570  olor-1:var(--dep
+000315a0: 7265 6361 7465 642d 3129 3b2d 2d63 6f6c  recated-1);--col
+000315b0: 6f72 2d32 3a76 6172 282d 2d64 6570 7265  or-2:var(--depre
+000315c0: 6361 7465 642d 3229 3b2d 2d76 6572 7369  cated-2);--versi
+000315d0: 6f6e 2d69 636f 6e3a 2221 227d 6469 762e  on-icon:"!"}div.
+000315e0: 6465 7072 6563 6174 6564 3e70 2c64 6976  deprecated>p,div
+000315f0: 2e76 6572 7369 6f6e 6164 6465 643e 702c  .versionadded>p,
+00031600: 6469 762e 7665 7273 696f 6e63 6861 6e67  div.versionchang
+00031610: 6564 3e70 7b6d 6172 6769 6e3a 307d 2e79  ed>p{margin:0}.y
+00031620: 7565 2062 6c6f 636b 7175 6f74 652e 6570  ue blockquote.ep
+00031630: 6967 7261 7068 7b70 6164 6469 6e67 3a31  igraph{padding:1
+00031640: 7265 6d20 322e 3472 656d 3b62 6f72 6465  rem 2.4rem;borde
+00031650: 722d 6c65 6674 3a30 3b74 6578 742d 616c  r-left:0;text-al
+00031660: 6967 6e3a 6365 6e74 6572 7d2e 7975 6520  ign:center}.yue 
+00031670: 626c 6f63 6b71 756f 7465 2e68 6967 686c  blockquote.highl
+00031680: 6967 6874 737b 626f 7264 6572 2d6c 6566  ights{border-lef
+00031690: 742d 7769 6474 683a 3470 783b 7061 6464  t-width:4px;padd
+000316a0: 696e 672d 746f 703a 2e32 7265 6d3b 7061  ing-top:.2rem;pa
+000316b0: 6464 696e 672d 626f 7474 6f6d 3a2e 3272  dding-bottom:.2r
+000316c0: 656d 3b62 6163 6b67 726f 756e 642d 636f  em;background-co
+000316d0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d73  lor:var(--sy-c-s
+000316e0: 7572 6661 6365 297d 2e79 7565 2062 6c6f  urface)}.yue blo
+000316f0: 636b 7175 6f74 652e 7075 6c6c 2d71 756f  ckquote.pull-quo
+00031700: 7465 7b70 6f73 6974 696f 6e3a 7265 6c61  te{position:rela
+00031710: 7469 7665 3b66 6f6e 742d 7369 7a65 3a31  tive;font-size:1
+00031720: 2e32 3472 656d 3b70 6164 6469 6e67 3a32  .24rem;padding:2
+00031730: 2e34 7265 6d20 332e 3672 656d 2031 2e32  .4rem 3.6rem 1.2
+00031740: 7265 6d3b 626f 7264 6572 2d6c 6566 743a  rem;border-left:
+00031750: 307d 2e79 7565 2062 6c6f 636b 7175 6f74  0}.yue blockquot
+00031760: 652e 7075 6c6c 2d71 756f 7465 3a62 6566  e.pull-quote:bef
+00031770: 6f72 657b 636f 6e74 656e 743a 225c 3230  ore{content:"\20
+00031780: 3163 223b 706f 7369 7469 6f6e 3a61 6273  1c";position:abs
+00031790: 6f6c 7574 653b 746f 703a 303b 6c65 6674  olute;top:0;left
+000317a0: 3a2e 3572 656d 3b63 6f6c 6f72 3a76 6172  :.5rem;color:var
+000317b0: 282d 2d79 7565 2d63 2d71 756f 7465 2d73  (--yue-c-quote-s
+000317c0: 796d 626f 6c29 3b66 6f6e 743a 3730 3020  ymbol);font:700 
+000317d0: 3472 656d 2f31 2054 696d 6573 204e 6577  4rem/1 Times New
+000317e0: 2052 6f6d 616e 2c47 656f 7267 6961 2c50   Roman,Georgia,P
+000317f0: 616c 6174 696e 6f2c 5469 6d65 732c 7365  alatino,Times,se
+00031800: 7269 667d 2e79 7565 2062 6c6f 636b 7175  rif}.yue blockqu
+00031810: 6f74 652e 7075 6c6c 2d71 756f 7465 202e  ote.pull-quote .
+00031820: 6174 7472 6962 7574 696f 6e7b 7465 7874  attribution{text
+00031830: 2d61 6c69 676e 3a72 6967 6874 7d70 7265  -align:right}pre
+00031840: 2e6c 6974 6572 616c 2d62 6c6f 636b 7b6c  .literal-block{l
+00031850: 696e 652d 6865 6967 6874 3a31 2e34 383b  ine-height:1.48;
+00031860: 7061 6464 696e 673a 3172 656d 3b66 6f6e  padding:1rem;fon
+00031870: 742d 7369 7a65 3a2e 3936 7265 6d3b 6261  t-size:.96rem;ba
+00031880: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+00031890: 6172 282d 2d73 796e 7461 782d 7072 652d  ar(--syntax-pre-
+000318a0: 6267 293b 626f 7264 6572 2d72 6164 6975  bg);border-radiu
+000318b0: 733a 3670 783b 6f76 6572 666c 6f77 3a61  s:6px;overflow:a
+000318c0: 7574 6f7d 2e68 6967 686c 6967 6874 2c2e  uto}.highlight,.
+000318d0: 6c69 7465 7261 6c2d 626c 6f63 6b2d 7772  literal-block-wr
+000318e0: 6170 7065 727b 2d2d 6d61 7267 696e 3a31  apper{--margin:1
+000318f0: 7265 6d3b 2d2d 7261 6469 7573 3a36 7078  rem;--radius:6px
+00031900: 7d2e 6c69 7465 7261 6c2d 626c 6f63 6b2d  }.literal-block-
+00031910: 7772 6170 7065 7220 6469 765b 636c 6173  wrapper div[clas
+00031920: 735e 3d68 6967 686c 6967 6874 2d5d 7b64  s^=highlight-]{d
+00031930: 6973 706c 6179 3a66 6c65 787d 2e6c 6974  isplay:flex}.lit
+00031940: 6572 616c 2d62 6c6f 636b 2d77 7261 7070  eral-block-wrapp
+00031950: 6572 202e 6869 6768 6c69 6768 747b 7769  er .highlight{wi
+00031960: 6474 683a 3130 3025 7d2e 6869 6768 6c69  dth:100%}.highli
+00031970: 6768 743e 7072 657b 6c69 6e65 2d68 6569  ght>pre{line-hei
+00031980: 6768 743a 312e 3438 3b70 6164 6469 6e67  ght:1.48;padding
+00031990: 3a76 6172 282d 2d6d 6172 6769 6e29 3b66  :var(--margin);f
+000319a0: 6f6e 742d 7369 7a65 3a2e 3936 7265 6d3b  ont-size:.96rem;
+000319b0: 666f 6e74 2d66 616d 696c 793a 7661 7228  font-family:var(
+000319c0: 2d2d 7379 2d66 2d6d 6f6e 6f29 3b62 6163  --sy-f-mono);bac
+000319d0: 6b67 726f 756e 642d 636f 6c6f 723a 7661  kground-color:va
+000319e0: 7228 2d2d 7379 6e74 6178 2d70 7265 2d62  r(--syntax-pre-b
+000319f0: 6729 3b62 6f72 6465 722d 7261 6469 7573  g);border-radius
+00031a00: 3a76 6172 282d 2d72 6164 6975 7329 3b6f  :var(--radius);o
+00031a10: 7665 7266 6c6f 773a 6175 746f 7d2e 7769  verflow:auto}.wi
+00031a20: 6e20 2e68 6967 686c 6967 6874 3e70 7265  n .highlight>pre
+00031a30: 7b66 6f6e 742d 6661 6d69 6c79 3a22 5477  {font-family:"Tw
+00031a40: 656d 6f6a 6920 436f 756e 7472 7920 466c  emoji Country Fl
+00031a50: 6167 7322 2c76 6172 282d 2d73 792d 662d  ags",var(--sy-f-
+00031a60: 6d6f 6e6f 297d 2e68 6967 686c 6967 6874  mono)}.highlight
+00031a70: 202e 6c69 6e65 6e6f 737b 6469 7370 6c61   .linenos{displa
+00031a80: 793a 696e 6c69 6e65 2d62 6c6f 636b 3b62  y:inline-block;b
+00031a90: 6f78 2d73 6861 646f 773a 2d2e 3035 7265  ox-shadow:-.05re
+00031aa0: 6d20 3020 7661 7228 2d2d 7379 6e74 6178  m 0 var(--syntax
+00031ab0: 2d6c 696e 656e 6f73 2d64 6976 6964 6572  -linenos-divider
+00031ac0: 2920 696e 7365 743b 2d77 6562 6b69 742d  ) inset;-webkit-
+00031ad0: 7573 6572 2d73 656c 6563 743a 6e6f 6e65  user-select:none
+00031ae0: 3b2d 6d6f 7a2d 7573 6572 2d73 656c 6563  ;-moz-user-selec
+00031af0: 743a 6e6f 6e65 3b75 7365 722d 7365 6c65  t:none;user-sele
+00031b00: 6374 3a6e 6f6e 653b 6d61 7267 696e 2d72  ct:none;margin-r
+00031b10: 6967 6874 3a2e 3872 656d 3b70 6164 6469  ight:.8rem;paddi
+00031b20: 6e67 2d72 6967 6874 3a2e 3872 656d 3b6f  ng-right:.8rem;o
+00031b30: 7061 6369 7479 3a2e 367d 2e68 6967 686c  pacity:.6}.highl
+00031b40: 6967 6874 202e 686c 6c7b 6d61 7267 696e  ight .hll{margin
+00031b50: 2d6c 6566 743a 6361 6c63 2830 7265 6d20  -left:calc(0rem 
+00031b60: 2d20 7661 7228 2d2d 6d61 7267 696e 2929  - var(--margin))
+00031b70: 3b6d 6172 6769 6e2d 7269 6768 743a 6361  ;margin-right:ca
+00031b80: 6c63 2830 7265 6d20 2d20 7661 7228 2d2d  lc(0rem - var(--
+00031b90: 6d61 7267 696e 2929 3b70 6164 6469 6e67  margin));padding
+00031ba0: 3a30 2076 6172 282d 2d6d 6172 6769 6e29  :0 var(--margin)
+00031bb0: 7d2e 636f 6465 2d62 6c6f 636b 2d63 6170  }.code-block-cap
+00031bc0: 7469 6f6e 7b64 6973 706c 6179 3a66 6c65  tion{display:fle
+00031bd0: 783b 666f 6e74 2d73 697a 653a 2e38 3472  x;font-size:.84r
+00031be0: 656d 3b66 6f6e 742d 7765 6967 6874 3a36  em;font-weight:6
+00031bf0: 3030 3b63 6f6c 6f72 3a76 6172 282d 2d73  00;color:var(--s
+00031c00: 796e 7461 782d 7465 7874 293b 6261 636b  yntax-text);back
+00031c10: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+00031c20: 282d 2d73 796e 7461 782d 6361 702d 6267  (--syntax-cap-bg
+00031c30: 293b 7061 6464 696e 673a 2e34 7265 6d20  );padding:.4rem 
+00031c40: 7661 7228 2d2d 6d61 7267 696e 293b 626f  var(--margin);bo
+00031c50: 7264 6572 2d72 6164 6975 733a 7661 7228  rder-radius:var(
+00031c60: 2d2d 7261 6469 7573 2920 7661 7228 2d2d  --radius) var(--
+00031c70: 7261 6469 7573 2920 3020 307d 2e63 6f64  radius) 0 0}.cod
+00031c80: 652d 626c 6f63 6b2d 6361 7074 696f 6e2b  e-block-caption+
+00031c90: 6469 763e 2e68 6967 686c 6967 6874 3e70  div>.highlight>p
+00031ca0: 7265 7b62 6f72 6465 722d 746f 702d 6c65  re{border-top-le
+00031cb0: 6674 2d72 6164 6975 733a 303b 626f 7264  ft-radius:0;bord
+00031cc0: 6572 2d74 6f70 2d72 6967 6874 2d72 6164  er-top-right-rad
+00031cd0: 6975 733a 307d 6469 765b 636c 6173 735e  ius:0}div[class^
+00031ce0: 3d68 6967 686c 6967 6874 5d3e 2e68 6967  =highlight]>.hig
+00031cf0: 686c 6967 6874 3e70 7265 7b64 6973 706c  hlight>pre{displ
+00031d00: 6179 3a67 7269 647d 2e79 7565 202e 7461  ay:grid}.yue .ta
+00031d10: 626c 652d 7772 6170 7065 727b 7769 6474  ble-wrapper{widt
+00031d20: 683a 3130 3025 3b6f 7665 7266 6c6f 772d  h:100%;overflow-
+00031d30: 783a 6175 746f 3b6d 6172 6769 6e2d 746f  x:auto;margin-to
+00031d40: 703a 3272 656d 3b6d 6172 6769 6e2d 626f  p:2rem;margin-bo
+00031d50: 7474 6f6d 3a32 7265 6d3b 626f 7264 6572  ttom:2rem;border
+00031d60: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
+00031d70: 2d79 7565 2d63 2d74 6162 6c65 2d62 6f72  -yue-c-table-bor
+00031d80: 6465 7229 3b62 6f72 6465 722d 7261 6469  der);border-radi
+00031d90: 7573 3a36 7078 7d2e 7975 6520 2e74 6162  us:6px}.yue .tab
+00031da0: 6c65 2d77 7261 7070 6572 3e74 6162 6c65  le-wrapper>table
+00031db0: 7b6d 6172 6769 6e3a 307d 2e79 7565 202e  {margin:0}.yue .
+00031dc0: 7461 626c 652d 7772 6170 7065 7220 7468  table-wrapper th
+00031dd0: 6561 6420 7472 7b62 6f72 6465 722d 746f  ead tr{border-to
+00031de0: 703a 3170 7820 736f 6c69 6420 7661 7228  p:1px solid var(
+00031df0: 2d2d 7975 652d 632d 7464 2d62 6f72 6465  --yue-c-td-borde
+00031e00: 7229 7d2e 7975 6520 2e74 6162 6c65 2d77  r)}.yue .table-w
+00031e10: 7261 7070 6572 2074 6865 6164 2074 723a  rapper thead tr:
+00031e20: 6669 7273 742d 6368 696c 647b 626f 7264  first-child{bord
+00031e30: 6572 2d74 6f70 3a30 7d2e 7975 6520 2e74  er-top:0}.yue .t
+00031e40: 6162 6c65 2d77 7261 7070 6572 2074 687b  able-wrapper th{
+00031e50: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+00031e60: 3a76 6172 282d 2d79 7565 2d63 2d74 682d  :var(--yue-c-th-
+00031e70: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
+00031e80: 6572 2d6c 6566 743a 3170 7820 736f 6c69  er-left:1px soli
+00031e90: 6420 7661 7228 2d2d 7975 652d 632d 7464  d var(--yue-c-td
+00031ea0: 2d62 6f72 6465 7229 3b70 6164 6469 6e67  -border);padding
+00031eb0: 3a2e 3732 3572 656d 2031 7265 6d7d 2e79  :.725rem 1rem}.y
+00031ec0: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
+00031ed0: 7220 7464 7b62 6f72 6465 722d 6c65 6674  r td{border-left
+00031ee0: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
+00031ef0: 2d79 7565 2d63 2d74 642d 626f 7264 6572  -yue-c-td-border
+00031f00: 293b 7061 6464 696e 673a 2e35 7265 6d20  );padding:.5rem 
+00031f10: 3172 656d 7d2e 7975 6520 2e74 6162 6c65  1rem}.yue .table
+00031f20: 2d77 7261 7070 6572 2074 723e 7464 3a66  -wrapper tr>td:f
+00031f30: 6972 7374 2d63 6869 6c64 2c2e 7975 6520  irst-child,.yue 
+00031f40: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
+00031f50: 723e 7468 3a66 6972 7374 2d63 6869 6c64  r>th:first-child
+00031f60: 7b62 6f72 6465 722d 6c65 6674 3a30 7d2e  {border-left:0}.
+00031f70: 7975 6520 2e74 6162 6c65 2d77 7261 7070  yue .table-wrapp
+00031f80: 6572 2063 6170 7469 6f6e 7b70 6164 6469  er caption{paddi
+00031f90: 6e67 3a2e 3572 656d 3b6d 6172 6769 6e3a  ng:.5rem;margin:
+00031fa0: 303b 626f 7264 6572 2d62 6f74 746f 6d3a  0;border-bottom:
+00031fb0: 3170 7820 736f 6c69 6420 7661 7228 2d2d  1px solid var(--
+00031fc0: 7975 652d 632d 7468 2d62 6f72 6465 7229  yue-c-th-border)
+00031fd0: 7d2e 7975 6520 2e74 6162 6c65 2d77 7261  }.yue .table-wra
+00031fe0: 7070 6572 2074 626f 6479 2074 722e 726f  pper tbody tr.ro
+00031ff0: 772d 6f64 647b 6261 636b 6772 6f75 6e64  w-odd{background
+00032000: 2d63 6f6c 6f72 3a76 6172 282d 2d79 7565  -color:var(--yue
+00032010: 2d63 2d72 6f77 2d62 6163 6b67 726f 756e  -c-row-backgroun
+00032020: 6429 7d2e 7975 6520 7461 626c 652e 686c  d)}.yue table.hl
+00032030: 6973 7420 7464 7b76 6572 7469 6361 6c2d  ist td{vertical-
+00032040: 616c 6967 6e3a 746f 707d 2e74 6162 6c65  align:top}.table
+00032050: 2d77 7261 7070 6572 7b6f 7665 7266 6c6f  -wrapper{overflo
+00032060: 772d 783a 6175 746f 3b73 6372 6f6c 6c62  w-x:auto;scrollb
+00032070: 6172 2d67 7574 7465 723a 6175 746f 7d2e  ar-gutter:auto}.
+00032080: 7461 626c 652d 7772 6170 7065 723a 3a2d  table-wrapper::-
+00032090: 7765 626b 6974 2d73 6372 6f6c 6c62 6172  webkit-scrollbar
+000320a0: 7b68 6569 6768 743a 2e37 3572 656d 3b77  {height:.75rem;w
+000320b0: 6964 7468 3a2e 3735 7265 6d7d 2e74 6162  idth:.75rem}.tab
+000320c0: 6c65 2d77 7261 7070 6572 3a3a 2d77 6562  le-wrapper::-web
+000320d0: 6b69 742d 7363 726f 6c6c 6261 722d 7468  kit-scrollbar-th
+000320e0: 756d 627b 626f 7264 6572 2d72 6164 6975  umb{border-radiu
+000320f0: 733a 3130 7078 7d2e 7461 626c 652d 7772  s:10px}.table-wr
+00032100: 6170 7065 723a 3a2d 7765 626b 6974 2d73  apper::-webkit-s
+00032110: 6372 6f6c 6c62 6172 2d74 7261 636b 7b62  crollbar-track{b
+00032120: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00032130: 696e 6974 6961 6c7d 2e74 6162 6c65 2d77  initial}.table-w
+00032140: 7261 7070 6572 3a68 6f76 6572 3a3a 2d77  rapper:hover::-w
+00032150: 6562 6b69 742d 7363 726f 6c6c 6261 722d  ebkit-scrollbar-
+00032160: 7468 756d 627b 6261 636b 6772 6f75 6e64  thumb{background
+00032170: 2d63 6f6c 6f72 3a23 3962 3962 3962 3333  -color:#9b9b9b33
+00032180: 3b62 6163 6b67 726f 756e 642d 636c 6970  ;background-clip
+00032190: 3a63 6f6e 7465 6e74 2d62 6f78 3b62 6f72  :content-box;bor
+000321a0: 6465 723a 3370 7820 736f 6c69 6420 2330  der:3px solid #0
+000321b0: 3030 307d 2e79 7565 2074 6162 6c65 2e67  000}.yue table.g
+000321c0: 686f 7374 2074 642c 2e79 7565 2074 6162  host td,.yue tab
+000321d0: 6c65 2e67 686f 7374 2074 687b 626f 7264  le.ghost th{bord
+000321e0: 6572 2d6c 6566 743a 303b 626f 7264 6572  er-left:0;border
+000321f0: 2d72 6967 6874 3a30 3b62 6163 6b67 726f  -right:0;backgro
+00032200: 756e 642d 636f 6c6f 723a 696e 6974 6961  und-color:initia
+00032210: 6c7d 2e79 7565 2074 6162 6c65 2e67 686f  l}.yue table.gho
+00032220: 7374 2063 6170 7469 6f6e 7b6d 6172 6769  st caption{margi
+00032230: 6e2d 626f 7474 6f6d 3a30 3b70 6164 6469  n-bottom:0;paddi
+00032240: 6e67 2d62 6f74 746f 6d3a 2e35 7265 6d3b  ng-bottom:.5rem;
+00032250: 626f 7264 6572 2d62 6f74 746f 6d3a 3370  border-bottom:3p
+00032260: 7820 736f 6c69 6420 7661 7228 2d2d 7975  x solid var(--yu
+00032270: 652d 632d 7464 2d62 6f72 6465 7229 7d2e  e-c-td-border)}.
+00032280: 7975 6520 7461 626c 652e 6768 6f73 7420  yue table.ghost 
+00032290: 7468 6561 6420 7472 3a66 6972 7374 2d63  thead tr:first-c
+000322a0: 6869 6c64 7b62 6f72 6465 722d 746f 703a  hild{border-top:
+000322b0: 303b 626f 7264 6572 2d62 6f74 746f 6d2d  0;border-bottom-
+000322c0: 7769 6474 683a 3370 787d 2e79 7565 202e  width:3px}.yue .
+000322d0: 7461 626c 652d 7772 6170 7065 722e 6768  table-wrapper.gh
+000322e0: 6f73 747b 626f 7264 6572 3a30 7d3a 726f  ost{border:0}:ro
+000322f0: 6f74 7b2d 2d73 6967 2d70 726f 7065 7274  ot{--sig-propert
+00032300: 793a 7661 7228 2d2d 7379 6e74 6178 2d6b  y:var(--syntax-k
+00032310: 6579 776f 7264 293b 2d2d 7369 672d 6e61  eyword);--sig-na
+00032320: 6d65 3a76 6172 282d 2d73 796e 7461 782d  me:var(--syntax-
+00032330: 7072 6f70 6572 7479 293b 2d2d 7369 672d  property);--sig-
+00032340: 7479 7065 6869 6e74 3a76 6172 282d 2d73  typehint:var(--s
+00032350: 796e 7461 782d 636f 6e73 7461 6e74 293b  yntax-constant);
+00032360: 2d2d 7369 672d 7061 7261 6d3a 7661 7228  --sig-param:var(
+00032370: 2d2d 7379 6e74 6178 2d6d 6574 6129 7d64  --syntax-meta)}d
+00032380: 742e 7369 677b 706f 7369 7469 6f6e 3a72  t.sig{position:r
+00032390: 656c 6174 6976 653b 666f 6e74 2d73 697a  elative;font-siz
+000323a0: 653a 2e39 3272 656d 3b70 6164 6469 6e67  e:.92rem;padding
+000323b0: 3a2e 3235 7265 6d20 2e35 7265 6d20 2e32  :.25rem .5rem .2
+000323c0: 3572 656d 2033 7265 6d3b 7465 7874 2d69  5rem 3rem;text-i
+000323d0: 6e64 656e 743a 2d32 2e34 7265 6d3b 626f  ndent:-2.4rem;bo
+000323e0: 7264 6572 2d72 6164 6975 733a 3670 787d  rder-radius:6px}
+000323f0: 6474 2e73 6967 3a61 6674 6572 7b63 6f6e  dt.sig:after{con
+00032400: 7465 6e74 3a22 223b 6469 7370 6c61 793a  tent:"";display:
+00032410: 7461 626c 653b 636c 6561 723a 626f 7468  table;clear:both
+00032420: 7d64 742e 7369 673a 686f 7665 727b 6261  }dt.sig:hover{ba
+00032430: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
+00032440: 792d 632d 7375 7266 6163 6529 7d64 742e  y-c-surface)}dt.
+00032450: 7369 672b 6464 7b66 6f6e 742d 7369 7a65  sig+dd{font-size
+00032460: 3a2e 3932 7265 6d3b 6d61 7267 696e 2d6c  :.92rem;margin-l
+00032470: 6566 743a 3272 656d 7d64 742e 7369 673e  eft:2rem}dt.sig>
+00032480: 656d 2e70 726f 7065 7274 793a 6669 7273  em.property:firs
+00032490: 742d 6368 696c 647b 636f 6c6f 723a 7661  t-child{color:va
+000324a0: 7228 2d2d 7369 672d 7072 6f70 6572 7479  r(--sig-property
+000324b0: 297d 646c 2e66 6965 6c64 2d6c 6973 7420  )}dl.field-list 
+000324c0: 617b 666f 6e74 2d77 6569 6768 743a 3430  a{font-weight:40
+000324d0: 307d 6474 2e73 6967 2b64 643e 6469 767b  0}dt.sig+dd>div{
+000324e0: 6d61 7267 696e 2d62 6f74 746f 6d3a 3172  margin-bottom:1r
+000324f0: 656d 7d64 742e 7369 672b 6464 3e64 6c2e  em}dt.sig+dd>dl.
+00032500: 6669 656c 642d 6c69 7374 3e64 747b 7465  field-list>dt{te
+00032510: 7874 2d74 7261 6e73 666f 726d 3a75 7070  xt-transform:upp
+00032520: 6572 6361 7365 3b66 6f6e 742d 7369 7a65  ercase;font-size
+00032530: 3a2e 3736 7265 6d7d 656d 2e70 726f 7065  :.76rem}em.prope
+00032540: 7274 792c 656d 2e73 6967 2d70 6172 616d  rty,em.sig-param
+00032550: 7b66 6f6e 742d 7374 796c 653a 6e6f 726d  {font-style:norm
+00032560: 616c 7d65 6d2e 7369 672d 7061 7261 6d7b  al}em.sig-param{
+00032570: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
+00032580: 2d6c 6967 6874 297d 7370 616e 2e73 6967  -light)}span.sig
+00032590: 2d6e 616d 652c 7370 616e 2e73 6967 2d70  -name,span.sig-p
+000325a0: 7265 6e61 6d65 7b63 6f6c 6f72 3a76 6172  rename{color:var
+000325b0: 282d 2d73 6967 2d6e 616d 6529 7d73 7061  (--sig-name)}spa
+000325c0: 6e2e 7369 672d 6e61 6d65 7b66 6f6e 742d  n.sig-name{font-
+000325d0: 7765 6967 6874 3a36 3030 7d73 7061 6e2e  weight:600}span.
+000325e0: 7369 672d 7265 7475 726e 2d69 636f 6e7b  sig-return-icon{
+000325f0: 636f 6c6f 723a 7661 7228 2d2d 7379 2d63  color:var(--sy-c
+00032600: 2d6c 6967 6874 297d 7370 616e 2e73 6967  -light)}span.sig
+00032610: 2d72 6574 7572 6e2d 7479 7065 6869 6e74  -return-typehint
+00032620: 2c73 7061 6e2e 7369 672d 7265 7475 726e  ,span.sig-return
+00032630: 2d74 7970 6568 696e 743e 617b 636f 6c6f  -typehint>a{colo
+00032640: 723a 7661 7228 2d2d 7369 672d 7479 7065  r:var(--sig-type
+00032650: 6869 6e74 297d 7370 616e 2e70 7265 2c73  hint)}span.pre,s
+00032660: 7061 6e2e 7369 672d 7061 7265 6e7b 666f  pan.sig-paren{fo
+00032670: 6e74 2d66 616d 696c 793a 7661 7228 2d2d  nt-family:var(--
+00032680: 7379 2d66 2d6d 6f6e 6f29 7d64 742e 7369  sy-f-mono)}dt.si
+00032690: 673e 612e 696e 7465 726e 616c 7b66 6f6e  g>a.internal{fon
+000326a0: 742d 7369 7a65 3a2e 3832 7265 6d3b 626f  t-size:.82rem;bo
+000326b0: 7264 6572 3a30 3b63 6f6c 6f72 3a76 6172  rder:0;color:var
+000326c0: 282d 2d73 792d 632d 6c69 6768 7429 7d64  (--sy-c-light)}d
+000326d0: 742e 7369 673e 612e 696e 7465 726e 616c  t.sig>a.internal
+000326e0: 3a62 6566 6f72 657b 636f 6e74 656e 743a  :before{content:
+000326f0: 225c 6122 3b77 6869 7465 2d73 7061 6365  "\a";white-space
+00032700: 3a70 7265 7d2e 7669 6577 636f 6465 2d62  :pre}.viewcode-b
+00032710: 6c6f 636b 7b70 6f73 6974 696f 6e3a 7265  lock{position:re
+00032720: 6c61 7469 7665 7d2e 7669 6577 636f 6465  lative}.viewcode
+00032730: 2d62 6163 6b7b 706f 7369 7469 6f6e 3a61  -back{position:a
+00032740: 6273 6f6c 7574 653b 746f 703a 2d31 2e35  bsolute;top:-1.5
+00032750: 7265 6d3b 666f 6e74 2d73 697a 653a 2e38  rem;font-size:.8
+00032760: 7265 6d7d 2e63 6c61 7373 6966 6965 727b  rem}.classifier{
+00032770: 666f 6e74 2d73 7479 6c65 3a6f 626c 6971  font-style:obliq
+00032780: 7565 3b66 6f6e 742d 7765 6967 6874 3a34  ue;font-weight:4
+00032790: 3030 7d2e 636c 6173 7369 6669 6572 3a62  00}.classifier:b
+000327a0: 6566 6f72 657b 666f 6e74 2d73 7479 6c65  efore{font-style
+000327b0: 3a6e 6f72 6d61 6c3b 6d61 7267 696e 2d6c  :normal;margin-l
+000327c0: 6566 743a 2e31 7265 6d3b 6d61 7267 696e  eft:.1rem;margin
+000327d0: 2d72 6967 6874 3a2e 3572 656d 3b63 6f6e  -right:.5rem;con
+000327e0: 7465 6e74 3a22 3a22 3b64 6973 706c 6179  tent:":";display
+000327f0: 3a69 6e6c 696e 652d 626c 6f63 6b7d 2e79  :inline-block}.y
+00032800: 7565 202e 7461 626c 652d 7772 6170 7065  ue .table-wrappe
+00032810: 722e 6175 746f 7375 6d6d 6172 797b 626f  r.autosummary{bo
+00032820: 7264 6572 2d6c 6566 743a 303b 626f 7264  rder-left:0;bord
+00032830: 6572 2d72 6967 6874 3a30 3b62 6f72 6465  er-right:0;borde
+00032840: 722d 7261 6469 7573 3a30 7d2e 7975 6520  r-radius:0}.yue 
+00032850: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
+00032860: 6162 6c65 2e61 7574 6f73 756d 6d61 7279  able.autosummary
+00032870: 2074 647b 626f 7264 6572 3a6e 6f6e 653b   td{border:none;
+00032880: 7061 6464 696e 672d 746f 703a 2e32 3572  padding-top:.25r
+00032890: 656d 3b70 6164 6469 6e67 2d62 6f74 746f  em;padding-botto
+000328a0: 6d3a 2e32 3572 656d 7d2e 7975 6520 702e  m:.25rem}.yue p.
+000328b0: 7275 6272 6963 2b64 6976 2e61 7574 6f73  rubric+div.autos
+000328c0: 756d 6d61 7279 7b6d 6172 6769 6e2d 746f  ummary{margin-to
+000328d0: 703a 307d 3a72 6f6f 747b 2d2d 7379 6e74  p:0}:root{--synt
+000328e0: 6178 2d70 7265 2d62 673a 7661 7228 2d2d  ax-pre-bg:var(--
+000328f0: 6163 6365 6e74 2d61 3229 3b2d 2d73 796e  accent-a2);--syn
+00032900: 7461 782d 6361 702d 6267 3a76 6172 282d  tax-cap-bg:var(-
+00032910: 2d61 6363 656e 742d 6133 293b 2d2d 7379  -accent-a3);--sy
+00032920: 6e74 6178 2d68 6967 686c 6967 6874 2d62  ntax-highlight-b
+00032930: 673a 7661 7228 2d2d 6163 6365 6e74 2d61  g:var(--accent-a
+00032940: 3329 3b2d 2d73 796e 7461 782d 6c69 6e65  3);--syntax-line
+00032950: 6e6f 732d 6469 7669 6465 723a 7661 7228  nos-divider:var(
+00032960: 2d2d 6772 6179 2d61 3629 3b2d 2d73 796e  --gray-a6);--syn
+00032970: 7461 782d 6c69 6768 742d 7465 7874 3a23  tax-light-text:#
+00032980: 3234 3239 3266 3b2d 2d73 796e 7461 782d  24292f;--syntax-
+00032990: 6c69 6768 742d 6d65 7461 3a23 3830 3763  light-meta:#807c
+000329a0: 3837 3b2d 2d73 796e 7461 782d 6c69 6768  87;--syntax-ligh
+000329b0: 742d 636f 6d6d 656e 743a 2336 6537 3738  t-comment:#6e778
+000329c0: 313b 2d2d 7379 6e74 6178 2d6c 6967 6874  1;--syntax-light
+000329d0: 2d63 6f6e 7374 616e 743a 2330 3535 3061  -constant:#0550a
+000329e0: 653b 2d2d 7379 6e74 6178 2d6c 6967 6874  e;--syntax-light
+000329f0: 2d65 6e74 6974 793a 2332 3638 6264 323b  -entity:#268bd2;
+00032a00: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d70  --syntax-light-p
+00032a10: 726f 7065 7274 793a 2338 3235 3064 663b  roperty:#8250df;
+00032a20: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d64  --syntax-light-d
+00032a30: 6566 696e 6974 696f 6e3a 2332 3432 3932  efinition:#24292
+00032a40: 663b 2d2d 7379 6e74 6178 2d6c 6967 6874  f;--syntax-light
+00032a50: 2d74 6167 3a23 3038 353b 2d2d 7379 6e74  -tag:#085;--synt
+00032a60: 6178 2d6c 6967 6874 2d62 7569 6c74 696e  ax-light-builtin
+00032a70: 3a23 6235 3839 3030 3b2d 2d73 796e 7461  :#b58900;--synta
+00032a80: 782d 6c69 6768 742d 6b65 7977 6f72 643a  x-light-keyword:
+00032a90: 2363 6632 3232 653b 2d2d 7379 6e74 6178  #cf222e;--syntax
+00032aa0: 2d6c 6967 6874 2d65 7863 6570 7469 6f6e  -light-exception
+00032ab0: 3a23 6536 3231 3265 3b2d 2d73 796e 7461  :#e6212e;--synta
+00032ac0: 782d 6c69 6768 742d 7374 7269 6e67 3a23  x-light-string:#
+00032ad0: 3061 3330 3639 3b2d 2d73 796e 7461 782d  0a3069;--syntax-
+00032ae0: 6c69 6768 742d 7265 6765 7870 3a23 6534  light-regexp:#e4
+00032af0: 303b 2d2d 7379 6e74 6178 2d6c 6967 6874  0;--syntax-light
+00032b00: 2d76 6172 6961 626c 653a 2361 3434 3830  -variable:#a4480
+00032b10: 663b 2d2d 7379 6e74 6178 2d6c 6967 6874  f;--syntax-light
+00032b20: 2d69 6e76 616c 6964 2d69 6c6c 6567 616c  -invalid-illegal
+00032b30: 2d74 6578 743a 2366 3666 3866 613b 2d2d  -text:#f6f8fa;--
+00032b40: 7379 6e74 6178 2d6c 6967 6874 2d69 6e76  syntax-light-inv
+00032b50: 616c 6964 2d69 6c6c 6567 616c 2d62 673a  alid-illegal-bg:
+00032b60: 2338 3230 3731 653b 2d2d 7379 6e74 6178  #82071e;--syntax
+00032b70: 2d6c 6967 6874 2d6d 6172 6b75 702d 6865  -light-markup-he
+00032b80: 6164 696e 673a 2330 3535 3061 653b 2d2d  ading:#0550ae;--
+00032b90: 7379 6e74 6178 2d6c 6967 6874 2d6d 6172  syntax-light-mar
+00032ba0: 6b75 702d 6974 616c 6963 3a23 3234 3239  kup-italic:#2429
+00032bb0: 3266 3b2d 2d73 796e 7461 782d 6c69 6768  2f;--syntax-ligh
+00032bc0: 742d 6d61 726b 7570 2d62 6f6c 643a 2332  t-markup-bold:#2
+00032bd0: 3432 3932 663b 2d2d 7379 6e74 6178 2d6c  4292f;--syntax-l
+00032be0: 6967 6874 2d6d 6172 6b75 702d 6465 6c65  ight-markup-dele
+00032bf0: 7465 642d 7465 7874 3a23 3832 3037 3165  ted-text:#82071e
+00032c00: 3b2d 2d73 796e 7461 782d 6c69 6768 742d  ;--syntax-light-
+00032c10: 6d61 726b 7570 2d64 656c 6574 6564 2d62  markup-deleted-b
+00032c20: 673a 2366 6665 6265 393b 2d2d 7379 6e74  g:#ffebe9;--synt
+00032c30: 6178 2d6c 6967 6874 2d6d 6172 6b75 702d  ax-light-markup-
+00032c40: 696e 7365 7274 6564 2d74 6578 743a 2331  inserted-text:#1
+00032c50: 3136 3332 393b 2d2d 7379 6e74 6178 2d6c  16329;--syntax-l
+00032c60: 6967 6874 2d6d 6172 6b75 702d 696e 7365  ight-markup-inse
+00032c70: 7274 6564 2d62 673a 2364 6166 6265 313b  rted-bg:#dafbe1;
+00032c80: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+00032c90: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
+00032ca0: 7874 3a23 3935 3338 3030 3b2d 2d73 796e  xt:#953800;--syn
+00032cb0: 7461 782d 6c69 6768 742d 6d61 726b 7570  tax-light-markup
+00032cc0: 2d63 6861 6e67 6564 2d62 673a 2366 6664  -changed-bg:#ffd
+00032cd0: 3862 353b 2d2d 7379 6e74 6178 2d6c 6967  8b5;--syntax-lig
+00032ce0: 6874 2d6d 6172 6b75 702d 6967 6e6f 7265  ht-markup-ignore
+00032cf0: 642d 7465 7874 3a23 6561 6565 6632 3b2d  d-text:#eaeef2;-
+00032d00: 2d73 796e 7461 782d 6c69 6768 742d 6d61  -syntax-light-ma
+00032d10: 726b 7570 2d69 676e 6f72 6564 2d62 673a  rkup-ignored-bg:
+00032d20: 2330 3535 3061 653b 2d2d 7379 6e74 6178  #0550ae;--syntax
+00032d30: 2d6c 6967 6874 2d6d 6574 612d 6469 6666  -light-meta-diff
+00032d40: 2d72 616e 6765 3a23 3832 3530 6466 3b2d  -range:#8250df;-
+00032d50: 2d73 796e 7461 782d 6c69 6768 742d 7370  -syntax-light-sp
+00032d60: 6563 6961 6c2d 6267 3a23 6463 6361 6661  ecial-bg:#dccafa
+00032d70: 3b2d 2d73 796e 7461 782d 6461 726b 2d74  ;--syntax-dark-t
+00032d80: 6578 743a 2363 3964 3164 393b 2d2d 7379  ext:#c9d1d9;--sy
+00032d90: 6e74 6178 2d64 6172 6b2d 6d65 7461 3a23  ntax-dark-meta:#
+00032da0: 3665 3737 3831 3b2d 2d73 796e 7461 782d  6e7781;--syntax-
+00032db0: 6461 726b 2d63 6f6d 6d65 6e74 3a23 3862  dark-comment:#8b
+00032dc0: 3934 3965 3b2d 2d73 796e 7461 782d 6461  949e;--syntax-da
+00032dd0: 726b 2d63 6f6e 7374 616e 743a 2337 3963  rk-constant:#79c
+00032de0: 3066 663b 2d2d 7379 6e74 6178 2d64 6172  0ff;--syntax-dar
+00032df0: 6b2d 656e 7469 7479 3a23 3437 6230 6661  k-entity:#47b0fa
+00032e00: 3b2d 2d73 796e 7461 782d 6461 726b 2d70  ;--syntax-dark-p
+00032e10: 726f 7065 7274 793a 2364 3261 3866 663b  roperty:#d2a8ff;
+00032e20: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6465  --syntax-dark-de
+00032e30: 6669 6e69 7469 6f6e 3a23 6339 6431 6439  finition:#c9d1d9
+00032e40: 3b2d 2d73 796e 7461 782d 6461 726b 2d74  ;--syntax-dark-t
+00032e50: 6167 3a23 3765 6537 3837 3b2d 2d73 796e  ag:#7ee787;--syn
+00032e60: 7461 782d 6461 726b 2d62 7569 6c74 696e  tax-dark-builtin
+00032e70: 3a23 6666 6433 3463 3b2d 2d73 796e 7461  :#ffd34c;--synta
+00032e80: 782d 6461 726b 2d6b 6579 776f 7264 3a23  x-dark-keyword:#
+00032e90: 6666 3762 3732 3b2d 2d73 796e 7461 782d  ff7b72;--syntax-
+00032ea0: 6461 726b 2d65 7863 6570 7469 6f6e 3a23  dark-exception:#
+00032eb0: 6461 3437 3363 3b2d 2d73 796e 7461 782d  da473c;--syntax-
+00032ec0: 6461 726b 2d73 7472 696e 673a 2361 3564  dark-string:#a5d
+00032ed0: 3666 663b 2d2d 7379 6e74 6178 2d64 6172  6ff;--syntax-dar
+00032ee0: 6b2d 7265 6765 7870 3a23 6566 3935 3465  k-regexp:#ef954e
+00032ef0: 3b2d 2d73 796e 7461 782d 6461 726b 2d76  ;--syntax-dark-v
+00032f00: 6172 6961 626c 653a 2366 6661 3635 373b  ariable:#ffa657;
+00032f10: 2d2d 7379 6e74 6178 2d64 6172 6b2d 696e  --syntax-dark-in
+00032f20: 7661 6c69 642d 696c 6c65 6761 6c2d 7465  valid-illegal-te
+00032f30: 7874 3a23 6630 6636 6663 3b2d 2d73 796e  xt:#f0f6fc;--syn
+00032f40: 7461 782d 6461 726b 2d69 6e76 616c 6964  tax-dark-invalid
+00032f50: 2d69 6c6c 6567 616c 2d62 673a 2338 6531  -illegal-bg:#8e1
+00032f60: 3531 393b 2d2d 7379 6e74 6178 2d64 6172  519;--syntax-dar
+00032f70: 6b2d 6d61 726b 7570 2d68 6561 6469 6e67  k-markup-heading
+00032f80: 3a23 3166 3666 6562 3b2d 2d73 796e 7461  :#1f6feb;--synta
+00032f90: 782d 6461 726b 2d6d 6172 6b75 702d 6974  x-dark-markup-it
+00032fa0: 616c 6963 3a23 6339 6431 6439 3b2d 2d73  alic:#c9d1d9;--s
+00032fb0: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
+00032fc0: 702d 626f 6c64 3a23 6339 6431 6439 3b2d  p-bold:#c9d1d9;-
+00032fd0: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
+00032fe0: 6b75 702d 6465 6c65 7465 642d 7465 7874  kup-deleted-text
+00032ff0: 3a23 6666 6463 6437 3b2d 2d73 796e 7461  :#ffdcd7;--synta
+00033000: 782d 6461 726b 2d6d 6172 6b75 702d 6465  x-dark-markup-de
+00033010: 6c65 7465 642d 6267 3a23 3637 3036 3063  leted-bg:#67060c
+00033020: 3b2d 2d73 796e 7461 782d 6461 726b 2d6d  ;--syntax-dark-m
+00033030: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
+00033040: 6578 743a 2361 6666 3562 343b 2d2d 7379  ext:#aff5b4;--sy
+00033050: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
+00033060: 2d69 6e73 6572 7465 642d 6267 3a23 3033  -inserted-bg:#03
+00033070: 3361 3136 3b2d 2d73 796e 7461 782d 6461  3a16;--syntax-da
+00033080: 726b 2d6d 6172 6b75 702d 6368 616e 6765  rk-markup-change
+00033090: 642d 7465 7874 3a23 6666 6466 6236 3b2d  d-text:#ffdfb6;-
+000330a0: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
+000330b0: 6b75 702d 6368 616e 6765 642d 6267 3a23  kup-changed-bg:#
+000330c0: 3561 3165 3032 3b2d 2d73 796e 7461 782d  5a1e02;--syntax-
+000330d0: 6461 726b 2d6d 6172 6b75 702d 6967 6e6f  dark-markup-igno
+000330e0: 7265 642d 7465 7874 3a23 6339 6431 6439  red-text:#c9d1d9
+000330f0: 3b2d 2d73 796e 7461 782d 6461 726b 2d6d  ;--syntax-dark-m
+00033100: 6172 6b75 702d 6967 6e6f 7265 642d 6267  arkup-ignored-bg
+00033110: 3a23 3131 3538 6337 3b2d 2d73 796e 7461  :#1158c7;--synta
+00033120: 782d 6461 726b 2d6d 6574 612d 6469 6666  x-dark-meta-diff
+00033130: 2d72 616e 6765 3a23 6432 6138 6666 3b2d  -range:#d2a8ff;-
+00033140: 2d73 796e 7461 782d 6461 726b 2d73 7065  -syntax-dark-spe
+00033150: 6369 616c 2d62 673a 2334 6634 3235 647d  cial-bg:#4f425d}
+00033160: 3a72 6f6f 742c 6874 6d6c 2e6c 6967 6874  :root,html.light
+00033170: 7b2d 2d73 796e 7461 782d 7465 7874 3a76  {--syntax-text:v
+00033180: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00033190: 742d 7465 7874 293b 2d2d 7379 6e74 6178  t-text);--syntax
+000331a0: 2d6d 6574 613a 7661 7228 2d2d 7379 6e74  -meta:var(--synt
+000331b0: 6178 2d6c 6967 6874 2d6d 6574 6129 3b2d  ax-light-meta);-
+000331c0: 2d73 796e 7461 782d 636f 6d6d 656e 743a  -syntax-comment:
+000331d0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+000331e0: 6874 2d63 6f6d 6d65 6e74 293b 2d2d 7379  ht-comment);--sy
+000331f0: 6e74 6178 2d63 6f6e 7374 616e 743a 7661  ntax-constant:va
+00033200: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+00033210: 2d63 6f6e 7374 616e 7429 3b2d 2d73 796e  -constant);--syn
+00033220: 7461 782d 656e 7469 7479 3a76 6172 282d  tax-entity:var(-
+00033230: 2d73 796e 7461 782d 6c69 6768 742d 656e  -syntax-light-en
+00033240: 7469 7479 293b 2d2d 7379 6e74 6178 2d70  tity);--syntax-p
+00033250: 726f 7065 7274 793a 7661 7228 2d2d 7379  roperty:var(--sy
+00033260: 6e74 6178 2d6c 6967 6874 2d70 726f 7065  ntax-light-prope
+00033270: 7274 7929 3b2d 2d73 796e 7461 782d 6465  rty);--syntax-de
+00033280: 6669 6e69 7469 6f6e 3a76 6172 282d 2d73  finition:var(--s
+00033290: 796e 7461 782d 6c69 6768 742d 6465 6669  yntax-light-defi
+000332a0: 6e69 7469 6f6e 293b 2d2d 7379 6e74 6178  nition);--syntax
+000332b0: 2d74 6167 3a76 6172 282d 2d73 796e 7461  -tag:var(--synta
+000332c0: 782d 6c69 6768 742d 7461 6729 3b2d 2d73  x-light-tag);--s
+000332d0: 796e 7461 782d 6275 696c 7469 6e3a 7661  yntax-builtin:va
+000332e0: 7228 2d2d 7379 6e74 6178 2d6c 6967 6874  r(--syntax-light
+000332f0: 2d62 7569 6c74 696e 293b 2d2d 7379 6e74  -builtin);--synt
+00033300: 6178 2d6b 6579 776f 7264 3a76 6172 282d  ax-keyword:var(-
+00033310: 2d73 796e 7461 782d 6c69 6768 742d 6b65  -syntax-light-ke
+00033320: 7977 6f72 6429 3b2d 2d73 796e 7461 782d  yword);--syntax-
+00033330: 6578 6365 7074 696f 6e3a 7661 7228 2d2d  exception:var(--
+00033340: 7379 6e74 6178 2d6c 6967 6874 2d65 7863  syntax-light-exc
+00033350: 6570 7469 6f6e 293b 2d2d 7379 6e74 6178  eption);--syntax
+00033360: 2d73 7472 696e 673a 7661 7228 2d2d 7379  -string:var(--sy
+00033370: 6e74 6178 2d6c 6967 6874 2d73 7472 696e  ntax-light-strin
+00033380: 6729 3b2d 2d73 796e 7461 782d 7265 6765  g);--syntax-rege
+00033390: 7870 3a76 6172 282d 2d73 796e 7461 782d  xp:var(--syntax-
+000333a0: 6c69 6768 742d 7265 6765 7870 293b 2d2d  light-regexp);--
+000333b0: 7379 6e74 6178 2d76 6172 6961 626c 653a  syntax-variable:
+000333c0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+000333d0: 6874 2d76 6172 6961 626c 6529 3b2d 2d73  ht-variable);--s
+000333e0: 796e 7461 782d 696e 7661 6c69 642d 696c  yntax-invalid-il
+000333f0: 6c65 6761 6c2d 7465 7874 3a76 6172 282d  legal-text:var(-
+00033400: 2d73 796e 7461 782d 6c69 6768 742d 696e  -syntax-light-in
+00033410: 7661 6c69 642d 696c 6c65 6761 6c2d 7465  valid-illegal-te
+00033420: 7874 293b 2d2d 7379 6e74 6178 2d69 6e76  xt);--syntax-inv
+00033430: 616c 6964 2d69 6c6c 6567 616c 2d62 673a  alid-illegal-bg:
+00033440: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+00033450: 6874 2d69 6e76 616c 6964 2d69 6c6c 6567  ht-invalid-illeg
+00033460: 616c 2d62 6729 3b2d 2d73 796e 7461 782d  al-bg);--syntax-
+00033470: 6d61 726b 7570 2d68 6561 6469 6e67 3a76  markup-heading:v
+00033480: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00033490: 742d 6d61 726b 7570 2d68 6561 6469 6e67  t-markup-heading
+000334a0: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
+000334b0: 702d 6974 616c 6963 3a76 6172 282d 2d73  p-italic:var(--s
+000334c0: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
+000334d0: 7570 2d69 7461 6c69 6329 3b2d 2d73 796e  up-italic);--syn
+000334e0: 7461 782d 6d61 726b 7570 2d62 6f6c 643a  tax-markup-bold:
+000334f0: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+00033500: 6874 2d6d 6172 6b75 702d 626f 6c64 293b  ht-markup-bold);
+00033510: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
+00033520: 6465 6c65 7465 642d 7465 7874 3a76 6172  deleted-text:var
+00033530: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
+00033540: 6d61 726b 7570 2d64 656c 6574 6564 2d74  markup-deleted-t
+00033550: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
+00033560: 726b 7570 2d64 656c 6574 6564 2d62 673a  rkup-deleted-bg:
+00033570: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+00033580: 6874 2d6d 6172 6b75 702d 6465 6c65 7465  ht-markup-delete
+00033590: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
+000335a0: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
+000335b0: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
+000335c0: 2d6c 6967 6874 2d6d 6172 6b75 702d 696e  -light-markup-in
+000335d0: 7365 7274 6564 2d74 6578 7429 3b2d 2d73  serted-text);--s
+000335e0: 796e 7461 782d 6d61 726b 7570 2d69 6e73  yntax-markup-ins
+000335f0: 6572 7465 642d 6267 3a76 6172 282d 2d73  erted-bg:var(--s
+00033600: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
+00033610: 7570 2d69 6e73 6572 7465 642d 6267 293b  up-inserted-bg);
+00033620: 2d2d 7379 6e74 6178 2d6d 6172 6b75 702d  --syntax-markup-
+00033630: 6368 616e 6765 642d 7465 7874 3a76 6172  changed-text:var
+00033640: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
+00033650: 6d61 726b 7570 2d63 6861 6e67 6564 2d74  markup-changed-t
+00033660: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
+00033670: 726b 7570 2d63 6861 6e67 6564 2d62 673a  rkup-changed-bg:
+00033680: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+00033690: 6874 2d6d 6172 6b75 702d 6368 616e 6765  ht-markup-change
+000336a0: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
+000336b0: 6172 6b75 702d 6967 6e6f 7265 642d 7465  arkup-ignored-te
+000336c0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
+000336d0: 6c69 6768 742d 6d61 726b 7570 2d69 676e  light-markup-ign
+000336e0: 6f72 6564 2d74 6578 7429 3b2d 2d73 796e  ored-text);--syn
+000336f0: 7461 782d 6d61 726b 7570 2d69 676e 6f72  tax-markup-ignor
+00033700: 6564 2d62 673a 7661 7228 2d2d 7379 6e74  ed-bg:var(--synt
+00033710: 6178 2d6c 6967 6874 2d6d 6172 6b75 702d  ax-light-markup-
+00033720: 6967 6e6f 7265 642d 6267 293b 2d2d 7379  ignored-bg);--sy
+00033730: 6e74 6178 2d6d 6574 612d 6469 6666 2d72  ntax-meta-diff-r
+00033740: 616e 6765 3a76 6172 282d 2d73 796e 7461  ange:var(--synta
+00033750: 782d 6c69 6768 742d 6d65 7461 2d64 6966  x-light-meta-dif
+00033760: 662d 7261 6e67 6529 3b2d 2d73 796e 7461  f-range);--synta
+00033770: 782d 7370 6563 6961 6c2d 6267 3a76 6172  x-special-bg:var
+00033780: 282d 2d73 796e 7461 782d 6c69 6768 742d  (--syntax-light-
+00033790: 7370 6563 6961 6c2d 6267 297d 406d 6564  special-bg)}@med
+000337a0: 6961 2028 7072 6566 6572 732d 636f 6c6f  ia (prefers-colo
+000337b0: 722d 7363 6865 6d65 3a64 6172 6b29 7b3a  r-scheme:dark){:
+000337c0: 726f 6f74 7b2d 2d73 796e 7461 782d 7465  root{--syntax-te
+000337d0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
+000337e0: 6461 726b 2d74 6578 7429 3b2d 2d73 796e  dark-text);--syn
+000337f0: 7461 782d 6d65 7461 3a76 6172 282d 2d73  tax-meta:var(--s
+00033800: 796e 7461 782d 6461 726b 2d6d 6574 6129  yntax-dark-meta)
+00033810: 3b2d 2d73 796e 7461 782d 636f 6d6d 656e  ;--syntax-commen
+00033820: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
+00033830: 6172 6b2d 636f 6d6d 656e 7429 3b2d 2d73  ark-comment);--s
+00033840: 796e 7461 782d 636f 6e73 7461 6e74 3a76  yntax-constant:v
+00033850: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00033860: 2d63 6f6e 7374 616e 7429 3b2d 2d73 796e  -constant);--syn
+00033870: 7461 782d 656e 7469 7479 3a76 6172 282d  tax-entity:var(-
+00033880: 2d73 796e 7461 782d 6461 726b 2d65 6e74  -syntax-dark-ent
+00033890: 6974 7929 3b2d 2d73 796e 7461 782d 7072  ity);--syntax-pr
+000338a0: 6f70 6572 7479 3a76 6172 282d 2d73 796e  operty:var(--syn
+000338b0: 7461 782d 6461 726b 2d70 726f 7065 7274  tax-dark-propert
+000338c0: 7929 3b2d 2d73 796e 7461 782d 6465 6669  y);--syntax-defi
+000338d0: 6e69 7469 6f6e 3a76 6172 282d 2d73 796e  nition:var(--syn
+000338e0: 7461 782d 6461 726b 2d64 6566 696e 6974  tax-dark-definit
+000338f0: 696f 6e29 3b2d 2d73 796e 7461 782d 7461  ion);--syntax-ta
+00033900: 673a 7661 7228 2d2d 7379 6e74 6178 2d64  g:var(--syntax-d
+00033910: 6172 6b2d 7461 6729 3b2d 2d73 796e 7461  ark-tag);--synta
+00033920: 782d 6275 696c 7469 6e3a 7661 7228 2d2d  x-builtin:var(--
+00033930: 7379 6e74 6178 2d64 6172 6b2d 6275 696c  syntax-dark-buil
+00033940: 7469 6e29 3b2d 2d73 796e 7461 782d 6b65  tin);--syntax-ke
+00033950: 7977 6f72 643a 7661 7228 2d2d 7379 6e74  yword:var(--synt
+00033960: 6178 2d64 6172 6b2d 6b65 7977 6f72 6429  ax-dark-keyword)
+00033970: 3b2d 2d73 796e 7461 782d 6578 6365 7074  ;--syntax-except
+00033980: 696f 6e3a 7661 7228 2d2d 7379 6e74 6178  ion:var(--syntax
+00033990: 2d64 6172 6b2d 6578 6365 7074 696f 6e29  -dark-exception)
+000339a0: 3b2d 2d73 796e 7461 782d 7374 7269 6e67  ;--syntax-string
+000339b0: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+000339c0: 726b 2d73 7472 696e 6729 3b2d 2d73 796e  rk-string);--syn
+000339d0: 7461 782d 7265 6765 7870 3a76 6172 282d  tax-regexp:var(-
+000339e0: 2d73 796e 7461 782d 6461 726b 2d72 6567  -syntax-dark-reg
+000339f0: 6578 7029 3b2d 2d73 796e 7461 782d 7661  exp);--syntax-va
+00033a00: 7269 6162 6c65 3a76 6172 282d 2d73 796e  riable:var(--syn
+00033a10: 7461 782d 6461 726b 2d76 6172 6961 626c  tax-dark-variabl
+00033a20: 6529 3b2d 2d73 796e 7461 782d 696e 7661  e);--syntax-inva
+00033a30: 6c69 642d 696c 6c65 6761 6c2d 7465 7874  lid-illegal-text
+00033a40: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+00033a50: 726b 2d69 6e76 616c 6964 2d69 6c6c 6567  rk-invalid-illeg
+00033a60: 616c 2d74 6578 7429 3b2d 2d73 796e 7461  al-text);--synta
+00033a70: 782d 696e 7661 6c69 642d 696c 6c65 6761  x-invalid-illega
+00033a80: 6c2d 6267 3a76 6172 282d 2d73 796e 7461  l-bg:var(--synta
+00033a90: 782d 6461 726b 2d69 6e76 616c 6964 2d69  x-dark-invalid-i
+00033aa0: 6c6c 6567 616c 2d62 6729 3b2d 2d73 796e  llegal-bg);--syn
+00033ab0: 7461 782d 6d61 726b 7570 2d68 6561 6469  tax-markup-headi
+00033ac0: 6e67 3a76 6172 282d 2d73 796e 7461 782d  ng:var(--syntax-
+00033ad0: 6461 726b 2d6d 6172 6b75 702d 6865 6164  dark-markup-head
+00033ae0: 696e 6729 3b2d 2d73 796e 7461 782d 6d61  ing);--syntax-ma
+00033af0: 726b 7570 2d69 7461 6c69 633a 7661 7228  rkup-italic:var(
+00033b00: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
+00033b10: 726b 7570 2d69 7461 6c69 6329 3b2d 2d73  rkup-italic);--s
+00033b20: 796e 7461 782d 6d61 726b 7570 2d62 6f6c  yntax-markup-bol
+00033b30: 643a 7661 7228 2d2d 7379 6e74 6178 2d64  d:var(--syntax-d
+00033b40: 6172 6b2d 6d61 726b 7570 2d62 6f6c 6429  ark-markup-bold)
+00033b50: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00033b60: 2d64 656c 6574 6564 2d74 6578 743a 7661  -deleted-text:va
+00033b70: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00033b80: 6d61 726b 7570 2d64 656c 6574 6564 2d74  markup-deleted-t
+00033b90: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
+00033ba0: 726b 7570 2d64 656c 6574 6564 2d62 673a  rkup-deleted-bg:
 00033bb0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033bc0: 6b2d 7072 6f70 6572 7479 293b 2d2d 7379  k-property);--sy
-00033bd0: 6e74 6178 2d64 6566 696e 6974 696f 6e3a  ntax-definition:
-00033be0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033bf0: 6b2d 6465 6669 6e69 7469 6f6e 293b 2d2d  k-definition);--
-00033c00: 7379 6e74 6178 2d74 6167 3a76 6172 282d  syntax-tag:var(-
-00033c10: 2d73 796e 7461 782d 6461 726b 2d74 6167  -syntax-dark-tag
-00033c20: 293b 2d2d 7379 6e74 6178 2d62 7569 6c74  );--syntax-built
-00033c30: 696e 3a76 6172 282d 2d73 796e 7461 782d  in:var(--syntax-
-00033c40: 6461 726b 2d62 7569 6c74 696e 293b 2d2d  dark-builtin);--
-00033c50: 7379 6e74 6178 2d6b 6579 776f 7264 3a76  syntax-keyword:v
-00033c60: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00033c70: 2d6b 6579 776f 7264 293b 2d2d 7379 6e74  -keyword);--synt
-00033c80: 6178 2d65 7863 6570 7469 6f6e 3a76 6172  ax-exception:var
-00033c90: 282d 2d73 796e 7461 782d 6461 726b 2d65  (--syntax-dark-e
-00033ca0: 7863 6570 7469 6f6e 293b 2d2d 7379 6e74  xception);--synt
-00033cb0: 6178 2d73 7472 696e 673a 7661 7228 2d2d  ax-string:var(--
-00033cc0: 7379 6e74 6178 2d64 6172 6b2d 7374 7269  syntax-dark-stri
-00033cd0: 6e67 293b 2d2d 7379 6e74 6178 2d72 6567  ng);--syntax-reg
-00033ce0: 6578 703a 7661 7228 2d2d 7379 6e74 6178  exp:var(--syntax
-00033cf0: 2d64 6172 6b2d 7265 6765 7870 293b 2d2d  -dark-regexp);--
-00033d00: 7379 6e74 6178 2d76 6172 6961 626c 653a  syntax-variable:
-00033d10: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033d20: 6b2d 7661 7269 6162 6c65 293b 2d2d 7379  k-variable);--sy
-00033d30: 6e74 6178 2d69 6e76 616c 6964 2d69 6c6c  ntax-invalid-ill
-00033d40: 6567 616c 2d74 6578 743a 7661 7228 2d2d  egal-text:var(--
-00033d50: 7379 6e74 6178 2d64 6172 6b2d 696e 7661  syntax-dark-inva
-00033d60: 6c69 642d 696c 6c65 6761 6c2d 7465 7874  lid-illegal-text
-00033d70: 293b 2d2d 7379 6e74 6178 2d69 6e76 616c  );--syntax-inval
-00033d80: 6964 2d69 6c6c 6567 616c 2d62 673a 7661  id-illegal-bg:va
-00033d90: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-00033da0: 696e 7661 6c69 642d 696c 6c65 6761 6c2d  invalid-illegal-
-00033db0: 6267 293b 2d2d 7379 6e74 6178 2d6d 6172  bg);--syntax-mar
-00033dc0: 6b75 702d 6865 6164 696e 673a 7661 7228  kup-heading:var(
-00033dd0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-00033de0: 726b 7570 2d68 6561 6469 6e67 293b 2d2d  rkup-heading);--
-00033df0: 7379 6e74 6178 2d6d 6172 6b75 702d 6974  syntax-markup-it
-00033e00: 616c 6963 3a76 6172 282d 2d73 796e 7461  alic:var(--synta
-00033e10: 782d 6461 726b 2d6d 6172 6b75 702d 6974  x-dark-markup-it
-00033e20: 616c 6963 293b 2d2d 7379 6e74 6178 2d6d  alic);--syntax-m
-00033e30: 6172 6b75 702d 626f 6c64 3a76 6172 282d  arkup-bold:var(-
-00033e40: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-00033e50: 6b75 702d 626f 6c64 293b 2d2d 7379 6e74  kup-bold);--synt
-00033e60: 6178 2d6d 6172 6b75 702d 6465 6c65 7465  ax-markup-delete
-00033e70: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
-00033e80: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
-00033e90: 6465 6c65 7465 642d 7465 7874 293b 2d2d  deleted-text);--
-00033ea0: 7379 6e74 6178 2d6d 6172 6b75 702d 6465  syntax-markup-de
-00033eb0: 6c65 7465 642d 6267 3a76 6172 282d 2d73  leted-bg:var(--s
-00033ec0: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
-00033ed0: 702d 6465 6c65 7465 642d 6267 293b 2d2d  p-deleted-bg);--
-00033ee0: 7379 6e74 6178 2d6d 6172 6b75 702d 696e  syntax-markup-in
-00033ef0: 7365 7274 6564 2d74 6578 743a 7661 7228  serted-text:var(
-00033f00: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
-00033f10: 726b 7570 2d69 6e73 6572 7465 642d 7465  rkup-inserted-te
-00033f20: 7874 293b 2d2d 7379 6e74 6178 2d6d 6172  xt);--syntax-mar
-00033f30: 6b75 702d 696e 7365 7274 6564 2d62 673a  kup-inserted-bg:
-00033f40: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00033f50: 6b2d 6d61 726b 7570 2d69 6e73 6572 7465  k-markup-inserte
-00033f60: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-00033f70: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
-00033f80: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
-00033f90: 6461 726b 2d6d 6172 6b75 702d 6368 616e  dark-markup-chan
-00033fa0: 6765 642d 7465 7874 293b 2d2d 7379 6e74  ged-text);--synt
-00033fb0: 6178 2d6d 6172 6b75 702d 6368 616e 6765  ax-markup-change
-00033fc0: 642d 6267 3a76 6172 282d 2d73 796e 7461  d-bg:var(--synta
-00033fd0: 782d 6461 726b 2d6d 6172 6b75 702d 6368  x-dark-markup-ch
-00033fe0: 616e 6765 642d 6267 293b 2d2d 7379 6e74  anged-bg);--synt
-00033ff0: 6178 2d6d 6172 6b75 702d 6967 6e6f 7265  ax-markup-ignore
-00034000: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
-00034010: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
-00034020: 6967 6e6f 7265 642d 7465 7874 293b 2d2d  ignored-text);--
-00034030: 7379 6e74 6178 2d6d 6172 6b75 702d 6967  syntax-markup-ig
-00034040: 6e6f 7265 642d 6267 3a76 6172 282d 2d73  nored-bg:var(--s
-00034050: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
-00034060: 702d 6967 6e6f 7265 642d 6267 293b 2d2d  p-ignored-bg);--
-00034070: 7379 6e74 6178 2d6d 6574 612d 6469 6666  syntax-meta-diff
-00034080: 2d72 616e 6765 3a76 6172 282d 2d73 796e  -range:var(--syn
-00034090: 7461 782d 6461 726b 2d6d 6574 612d 6469  tax-dark-meta-di
-000340a0: 6666 2d72 616e 6765 293b 2d2d 7379 6e74  ff-range);--synt
-000340b0: 6178 2d73 7065 6369 616c 2d62 673a 7661  ax-special-bg:va
-000340c0: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
-000340d0: 7370 6563 6961 6c2d 6267 297d 2e6c 6967  special-bg)}.lig
-000340e0: 6874 202e 6461 726b 2d63 6f64 657b 2d2d  ht .dark-code{--
-000340f0: 7379 6e74 6178 2d70 7265 2d62 673a 7661  syntax-pre-bg:va
-00034100: 7228 2d2d 626c 6163 6b2d 6131 3229 3b2d  r(--black-a12);-
-00034110: 2d73 796e 7461 782d 6361 702d 6267 3a23  -syntax-cap-bg:#
-00034120: 3163 3230 3234 3b2d 2d73 796e 7461 782d  1c2024;--syntax-
-00034130: 6869 6768 6c69 6768 742d 6267 3a76 6172  highlight-bg:var
-00034140: 282d 2d77 6869 7465 2d61 3229 3b2d 2d73  (--white-a2);--s
-00034150: 796e 7461 782d 6c69 6e65 6e6f 732d 6469  yntax-linenos-di
-00034160: 7669 6465 723a 7661 7228 2d2d 7768 6974  vider:var(--whit
-00034170: 652d 6134 293b 2d2d 7379 6e74 6178 2d74  e-a4);--syntax-t
-00034180: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
-00034190: 2d64 6172 6b2d 7465 7874 293b 2d2d 7379  -dark-text);--sy
-000341a0: 6e74 6178 2d6d 6574 613a 7661 7228 2d2d  ntax-meta:var(--
-000341b0: 7379 6e74 6178 2d64 6172 6b2d 6d65 7461  syntax-dark-meta
-000341c0: 293b 2d2d 7379 6e74 6178 2d63 6f6d 6d65  );--syntax-comme
-000341d0: 6e74 3a76 6172 282d 2d73 796e 7461 782d  nt:var(--syntax-
-000341e0: 6461 726b 2d63 6f6d 6d65 6e74 293b 2d2d  dark-comment);--
-000341f0: 7379 6e74 6178 2d63 6f6e 7374 616e 743a  syntax-constant:
-00034200: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
-00034210: 6b2d 636f 6e73 7461 6e74 293b 2d2d 7379  k-constant);--sy
-00034220: 6e74 6178 2d65 6e74 6974 793a 7661 7228  ntax-entity:var(
-00034230: 2d2d 7379 6e74 6178 2d64 6172 6b2d 656e  --syntax-dark-en
-00034240: 7469 7479 293b 2d2d 7379 6e74 6178 2d70  tity);--syntax-p
-00034250: 726f 7065 7274 793a 7661 7228 2d2d 7379  roperty:var(--sy
-00034260: 6e74 6178 2d64 6172 6b2d 7072 6f70 6572  ntax-dark-proper
-00034270: 7479 293b 2d2d 7379 6e74 6178 2d64 6566  ty);--syntax-def
-00034280: 696e 6974 696f 6e3a 7661 7228 2d2d 7379  inition:var(--sy
-00034290: 6e74 6178 2d64 6172 6b2d 6465 6669 6e69  ntax-dark-defini
-000342a0: 7469 6f6e 293b 2d2d 7379 6e74 6178 2d74  tion);--syntax-t
-000342b0: 6167 3a76 6172 282d 2d73 796e 7461 782d  ag:var(--syntax-
-000342c0: 6461 726b 2d74 6167 293b 2d2d 7379 6e74  dark-tag);--synt
-000342d0: 6178 2d62 7569 6c74 696e 3a76 6172 282d  ax-builtin:var(-
-000342e0: 2d73 796e 7461 782d 6461 726b 2d62 7569  -syntax-dark-bui
-000342f0: 6c74 696e 293b 2d2d 7379 6e74 6178 2d6b  ltin);--syntax-k
-00034300: 6579 776f 7264 3a76 6172 282d 2d73 796e  eyword:var(--syn
-00034310: 7461 782d 6461 726b 2d6b 6579 776f 7264  tax-dark-keyword
-00034320: 293b 2d2d 7379 6e74 6178 2d65 7863 6570  );--syntax-excep
-00034330: 7469 6f6e 3a76 6172 282d 2d73 796e 7461  tion:var(--synta
-00034340: 782d 6461 726b 2d65 7863 6570 7469 6f6e  x-dark-exception
-00034350: 293b 2d2d 7379 6e74 6178 2d73 7472 696e  );--syntax-strin
-00034360: 673a 7661 7228 2d2d 7379 6e74 6178 2d64  g:var(--syntax-d
-00034370: 6172 6b2d 7374 7269 6e67 293b 2d2d 7379  ark-string);--sy
-00034380: 6e74 6178 2d72 6567 6578 703a 7661 7228  ntax-regexp:var(
-00034390: 2d2d 7379 6e74 6178 2d64 6172 6b2d 7265  --syntax-dark-re
-000343a0: 6765 7870 293b 2d2d 7379 6e74 6178 2d76  gexp);--syntax-v
-000343b0: 6172 6961 626c 653a 7661 7228 2d2d 7379  ariable:var(--sy
-000343c0: 6e74 6178 2d64 6172 6b2d 7661 7269 6162  ntax-dark-variab
-000343d0: 6c65 293b 2d2d 7379 6e74 6178 2d69 6e76  le);--syntax-inv
-000343e0: 616c 6964 2d69 6c6c 6567 616c 2d74 6578  alid-illegal-tex
-000343f0: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
-00034400: 6172 6b2d 696e 7661 6c69 642d 696c 6c65  ark-invalid-ille
-00034410: 6761 6c2d 7465 7874 293b 2d2d 7379 6e74  gal-text);--synt
-00034420: 6178 2d69 6e76 616c 6964 2d69 6c6c 6567  ax-invalid-illeg
-00034430: 616c 2d62 673a 7661 7228 2d2d 7379 6e74  al-bg:var(--synt
-00034440: 6178 2d64 6172 6b2d 696e 7661 6c69 642d  ax-dark-invalid-
-00034450: 696c 6c65 6761 6c2d 6267 293b 2d2d 7379  illegal-bg);--sy
-00034460: 6e74 6178 2d6d 6172 6b75 702d 6865 6164  ntax-markup-head
-00034470: 696e 673a 7661 7228 2d2d 7379 6e74 6178  ing:var(--syntax
-00034480: 2d64 6172 6b2d 6d61 726b 7570 2d68 6561  -dark-markup-hea
-00034490: 6469 6e67 293b 2d2d 7379 6e74 6178 2d6d  ding);--syntax-m
-000344a0: 6172 6b75 702d 6974 616c 6963 3a76 6172  arkup-italic:var
-000344b0: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
-000344c0: 6172 6b75 702d 6974 616c 6963 293b 2d2d  arkup-italic);--
-000344d0: 7379 6e74 6178 2d6d 6172 6b75 702d 626f  syntax-markup-bo
-000344e0: 6c64 3a76 6172 282d 2d73 796e 7461 782d  ld:var(--syntax-
-000344f0: 6461 726b 2d6d 6172 6b75 702d 626f 6c64  dark-markup-bold
-00034500: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00034510: 702d 6465 6c65 7465 642d 7465 7874 3a76  p-deleted-text:v
-00034520: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00034530: 2d6d 6172 6b75 702d 6465 6c65 7465 642d  -markup-deleted-
-00034540: 7465 7874 293b 2d2d 7379 6e74 6178 2d6d  text);--syntax-m
-00034550: 6172 6b75 702d 6465 6c65 7465 642d 6267  arkup-deleted-bg
-00034560: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-00034570: 726b 2d6d 6172 6b75 702d 6465 6c65 7465  rk-markup-delete
-00034580: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-00034590: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
-000345a0: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
-000345b0: 2d64 6172 6b2d 6d61 726b 7570 2d69 6e73  -dark-markup-ins
-000345c0: 6572 7465 642d 7465 7874 293b 2d2d 7379  erted-text);--sy
-000345d0: 6e74 6178 2d6d 6172 6b75 702d 696e 7365  ntax-markup-inse
-000345e0: 7274 6564 2d62 673a 7661 7228 2d2d 7379  rted-bg:var(--sy
-000345f0: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
-00034600: 2d69 6e73 6572 7465 642d 6267 293b 2d2d  -inserted-bg);--
-00034610: 7379 6e74 6178 2d6d 6172 6b75 702d 6368  syntax-markup-ch
-00034620: 616e 6765 642d 7465 7874 3a76 6172 282d  anged-text:var(-
-00034630: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
-00034640: 6b75 702d 6368 616e 6765 642d 7465 7874  kup-changed-text
-00034650: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00034660: 702d 6368 616e 6765 642d 6267 3a76 6172  p-changed-bg:var
-00034670: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
-00034680: 6172 6b75 702d 6368 616e 6765 642d 6267  arkup-changed-bg
-00034690: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-000346a0: 702d 6967 6e6f 7265 642d 7465 7874 3a76  p-ignored-text:v
-000346b0: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-000346c0: 2d6d 6172 6b75 702d 6967 6e6f 7265 642d  -markup-ignored-
-000346d0: 7465 7874 293b 2d2d 7379 6e74 6178 2d6d  text);--syntax-m
-000346e0: 6172 6b75 702d 6967 6e6f 7265 642d 6267  arkup-ignored-bg
-000346f0: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
-00034700: 726b 2d6d 6172 6b75 702d 6967 6e6f 7265  rk-markup-ignore
-00034710: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
-00034720: 6574 612d 6469 6666 2d72 616e 6765 3a76  eta-diff-range:v
-00034730: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
-00034740: 2d6d 6574 612d 6469 6666 2d72 616e 6765  -meta-diff-range
-00034750: 293b 2d2d 7379 6e74 6178 2d73 7065 6369  );--syntax-speci
-00034760: 616c 2d62 673a 7661 7228 2d2d 7379 6e74  al-bg:var(--synt
-00034770: 6178 2d64 6172 6b2d 7370 6563 6961 6c2d  ax-dark-special-
-00034780: 6267 297d 6874 6d6c 2e6c 6967 6874 202e  bg)}html.light .
-00034790: 6a75 7079 7465 725f 636f 6e74 6169 6e65  jupyter_containe
-000347a0: 7220 2e63 656c 6c5f 6f75 7470 7574 2c68  r .cell_output,h
-000347b0: 746d 6c2e 6c69 6768 7420 2e73 642d 7461  tml.light .sd-ta
-000347c0: 622d 636f 6e74 656e 747b 2d2d 7379 6e74  b-content{--synt
-000347d0: 6178 2d70 7265 2d62 673a 7661 7228 2d2d  ax-pre-bg:var(--
-000347e0: 636f 6c6f 722d 7375 7266 6163 652d 6163  color-surface-ac
-000347f0: 6365 6e74 293b 2d2d 7379 6e74 6178 2d63  cent);--syntax-c
-00034800: 6170 2d62 673a 7661 7228 2d2d 6163 6365  ap-bg:var(--acce
-00034810: 6e74 2d33 293b 2d2d 7379 6e74 6178 2d68  nt-3);--syntax-h
-00034820: 6967 686c 6967 6874 2d62 673a 7661 7228  ighlight-bg:var(
-00034830: 2d2d 6163 6365 6e74 2d61 3329 3b2d 2d73  --accent-a3);--s
-00034840: 796e 7461 782d 7465 7874 3a76 6172 282d  yntax-text:var(-
-00034850: 2d73 796e 7461 782d 6c69 6768 742d 7465  -syntax-light-te
-00034860: 7874 293b 2d2d 7379 6e74 6178 2d6d 6574  xt);--syntax-met
-00034870: 613a 7661 7228 2d2d 7379 6e74 6178 2d6c  a:var(--syntax-l
-00034880: 6967 6874 2d6d 6574 6129 3b2d 2d73 796e  ight-meta);--syn
-00034890: 7461 782d 636f 6d6d 656e 743a 7661 7228  tax-comment:var(
-000348a0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d63  --syntax-light-c
-000348b0: 6f6d 6d65 6e74 293b 2d2d 7379 6e74 6178  omment);--syntax
-000348c0: 2d63 6f6e 7374 616e 743a 7661 7228 2d2d  -constant:var(--
-000348d0: 7379 6e74 6178 2d6c 6967 6874 2d63 6f6e  syntax-light-con
-000348e0: 7374 616e 7429 3b2d 2d73 796e 7461 782d  stant);--syntax-
-000348f0: 656e 7469 7479 3a76 6172 282d 2d73 796e  entity:var(--syn
-00034900: 7461 782d 6c69 6768 742d 656e 7469 7479  tax-light-entity
-00034910: 293b 2d2d 7379 6e74 6178 2d70 726f 7065  );--syntax-prope
-00034920: 7274 793a 7661 7228 2d2d 7379 6e74 6178  rty:var(--syntax
-00034930: 2d6c 6967 6874 2d70 726f 7065 7274 7929  -light-property)
-00034940: 3b2d 2d73 796e 7461 782d 6465 6669 6e69  ;--syntax-defini
-00034950: 7469 6f6e 3a76 6172 282d 2d73 796e 7461  tion:var(--synta
-00034960: 782d 6c69 6768 742d 6465 6669 6e69 7469  x-light-definiti
-00034970: 6f6e 293b 2d2d 7379 6e74 6178 2d74 6167  on);--syntax-tag
-00034980: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
-00034990: 6768 742d 7461 6729 3b2d 2d73 796e 7461  ght-tag);--synta
-000349a0: 782d 6275 696c 7469 6e3a 7661 7228 2d2d  x-builtin:var(--
-000349b0: 7379 6e74 6178 2d6c 6967 6874 2d62 7569  syntax-light-bui
-000349c0: 6c74 696e 293b 2d2d 7379 6e74 6178 2d6b  ltin);--syntax-k
-000349d0: 6579 776f 7264 3a76 6172 282d 2d73 796e  eyword:var(--syn
-000349e0: 7461 782d 6c69 6768 742d 6b65 7977 6f72  tax-light-keywor
-000349f0: 6429 3b2d 2d73 796e 7461 782d 6578 6365  d);--syntax-exce
-00034a00: 7074 696f 6e3a 7661 7228 2d2d 7379 6e74  ption:var(--synt
-00034a10: 6178 2d6c 6967 6874 2d65 7863 6570 7469  ax-light-excepti
-00034a20: 6f6e 293b 2d2d 7379 6e74 6178 2d73 7472  on);--syntax-str
-00034a30: 696e 673a 7661 7228 2d2d 7379 6e74 6178  ing:var(--syntax
-00034a40: 2d6c 6967 6874 2d73 7472 696e 6729 3b2d  -light-string);-
-00034a50: 2d73 796e 7461 782d 7265 6765 7870 3a76  -syntax-regexp:v
-00034a60: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-00034a70: 742d 7265 6765 7870 293b 2d2d 7379 6e74  t-regexp);--synt
-00034a80: 6178 2d76 6172 6961 626c 653a 7661 7228  ax-variable:var(
-00034a90: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d76  --syntax-light-v
-00034aa0: 6172 6961 626c 6529 3b2d 2d73 796e 7461  ariable);--synta
-00034ab0: 782d 696e 7661 6c69 642d 696c 6c65 6761  x-invalid-illega
-00034ac0: 6c2d 7465 7874 3a76 6172 282d 2d73 796e  l-text:var(--syn
-00034ad0: 7461 782d 6c69 6768 742d 696e 7661 6c69  tax-light-invali
-00034ae0: 642d 696c 6c65 6761 6c2d 7465 7874 293b  d-illegal-text);
-00034af0: 2d2d 7379 6e74 6178 2d69 6e76 616c 6964  --syntax-invalid
-00034b00: 2d69 6c6c 6567 616c 2d62 673a 7661 7228  -illegal-bg:var(
-00034b10: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d69  --syntax-light-i
-00034b20: 6e76 616c 6964 2d69 6c6c 6567 616c 2d62  nvalid-illegal-b
-00034b30: 6729 3b2d 2d73 796e 7461 782d 6d61 726b  g);--syntax-mark
-00034b40: 7570 2d68 6561 6469 6e67 3a76 6172 282d  up-heading:var(-
-00034b50: 2d73 796e 7461 782d 6c69 6768 742d 6d61  -syntax-light-ma
-00034b60: 726b 7570 2d68 6561 6469 6e67 293b 2d2d  rkup-heading);--
-00034b70: 7379 6e74 6178 2d6d 6172 6b75 702d 6974  syntax-markup-it
-00034b80: 616c 6963 3a76 6172 282d 2d73 796e 7461  alic:var(--synta
-00034b90: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
-00034ba0: 7461 6c69 6329 3b2d 2d73 796e 7461 782d  talic);--syntax-
-00034bb0: 6d61 726b 7570 2d62 6f6c 643a 7661 7228  markup-bold:var(
-00034bc0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00034bd0: 6172 6b75 702d 626f 6c64 293b 2d2d 7379  arkup-bold);--sy
-00034be0: 6e74 6178 2d6d 6172 6b75 702d 6465 6c65  ntax-markup-dele
-00034bf0: 7465 642d 7465 7874 3a76 6172 282d 2d73  ted-text:var(--s
-00034c00: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-00034c10: 7570 2d64 656c 6574 6564 2d74 6578 7429  up-deleted-text)
-00034c20: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00034c30: 2d64 656c 6574 6564 2d62 673a 7661 7228  -deleted-bg:var(
-00034c40: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00034c50: 6172 6b75 702d 6465 6c65 7465 642d 6267  arkup-deleted-bg
-00034c60: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00034c70: 702d 696e 7365 7274 6564 2d74 6578 743a  p-inserted-text:
-00034c80: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00034c90: 6874 2d6d 6172 6b75 702d 696e 7365 7274  ht-markup-insert
-00034ca0: 6564 2d74 6578 7429 3b2d 2d73 796e 7461  ed-text);--synta
-00034cb0: 782d 6d61 726b 7570 2d69 6e73 6572 7465  x-markup-inserte
-00034cc0: 642d 6267 3a76 6172 282d 2d73 796e 7461  d-bg:var(--synta
-00034cd0: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
-00034ce0: 6e73 6572 7465 642d 6267 293b 2d2d 7379  nserted-bg);--sy
-00034cf0: 6e74 6178 2d6d 6172 6b75 702d 6368 616e  ntax-markup-chan
-00034d00: 6765 642d 7465 7874 3a76 6172 282d 2d73  ged-text:var(--s
-00034d10: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
-00034d20: 7570 2d63 6861 6e67 6564 2d74 6578 7429  up-changed-text)
-00034d30: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
-00034d40: 2d63 6861 6e67 6564 2d62 673a 7661 7228  -changed-bg:var(
-00034d50: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
-00034d60: 6172 6b75 702d 6368 616e 6765 642d 6267  arkup-changed-bg
-00034d70: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
-00034d80: 702d 6967 6e6f 7265 642d 7465 7874 3a76  p-ignored-text:v
-00034d90: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
-00034da0: 742d 6d61 726b 7570 2d69 676e 6f72 6564  t-markup-ignored
-00034db0: 2d74 6578 7429 3b2d 2d73 796e 7461 782d  -text);--syntax-
-00034dc0: 6d61 726b 7570 2d69 676e 6f72 6564 2d62  markup-ignored-b
-00034dd0: 673a 7661 7228 2d2d 7379 6e74 6178 2d6c  g:var(--syntax-l
-00034de0: 6967 6874 2d6d 6172 6b75 702d 6967 6e6f  ight-markup-igno
-00034df0: 7265 642d 6267 293b 2d2d 7379 6e74 6178  red-bg);--syntax
-00034e00: 2d6d 6574 612d 6469 6666 2d72 616e 6765  -meta-diff-range
-00034e10: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
-00034e20: 6768 742d 6d65 7461 2d64 6966 662d 7261  ght-meta-diff-ra
-00034e30: 6e67 6529 3b2d 2d73 796e 7461 782d 6869  nge);--syntax-hi
-00034e40: 6768 6c69 6768 742d 6267 3a76 6172 282d  ghlight-bg:var(-
-00034e50: 2d73 796e 7461 782d 6c69 6768 742d 6869  -syntax-light-hi
-00034e60: 6768 6c69 6768 742d 6267 293b 2d2d 7379  ghlight-bg);--sy
-00034e70: 6e74 6178 2d73 7065 6369 616c 2d62 673a  ntax-special-bg:
-00034e80: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
-00034e90: 6874 2d73 7065 6369 616c 2d62 6729 7d2e  ht-special-bg)}.
-00034ea0: 7379 2d6c 7369 6465 7b2d 2d68 6569 6768  sy-lside{--heigh
-00034eb0: 743a 3432 7078 7d2e 7379 2d6c 7369 6465  t:42px}.sy-lside
-00034ec0: 2d62 6f74 746f 6d7b 706f 7369 7469 6f6e  -bottom{position
-00034ed0: 3a73 7469 636b 793b 626f 7474 6f6d 3a30  :sticky;bottom:0
-00034ee0: 3b70 6164 6469 6e67 3a30 3b62 6f72 6465  ;padding:0;borde
-00034ef0: 722d 746f 703a 3170 7820 736f 6c69 6420  r-top:1px solid 
-00034f00: 7661 7228 2d2d 7379 2d63 2d64 6976 6964  var(--sy-c-divid
-00034f10: 6572 293b 6261 636b 6772 6f75 6e64 2d63  er);background-c
-00034f20: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-00034f30: 6261 636b 6772 6f75 6e64 293b 2d2d 7477  background);--tw
-00034f40: 2d73 6861 646f 773a 3020 2d31 3270 7820  -shadow:0 -12px 
-00034f50: 3136 7078 2076 6172 282d 2d73 792d 632d  16px var(--sy-c-
-00034f60: 6261 636b 6772 6f75 6e64 293b 626f 782d  background);box-
-00034f70: 7368 6164 6f77 3a76 6172 282d 2d74 772d  shadow:var(--tw-
-00034f80: 7269 6e67 2d6f 6666 7365 742d 7368 6164  ring-offset-shad
-00034f90: 6f77 2c30 2030 2023 3030 3030 292c 7661  ow,0 0 #0000),va
-00034fa0: 7228 2d2d 7477 2d72 696e 672d 7368 6164  r(--tw-ring-shad
-00034fb0: 6f77 2c30 2030 2023 3030 3030 292c 7661  ow,0 0 #0000),va
-00034fc0: 7228 2d2d 7477 2d73 6861 646f 7729 7d2e  r(--tw-shadow)}.
-00034fd0: 7379 2d6c 7369 6465 202e 7273 742d 7665  sy-lside .rst-ve
-00034fe0: 7273 696f 6e73 7b70 6f73 6974 696f 6e3a  rsions{position:
-00034ff0: 7374 6174 6963 3b77 6964 7468 3a31 3030  static;width:100
-00035000: 253b 6261 636b 6772 6f75 6e64 2d63 6f6c  %;background-col
-00035010: 6f72 3a76 6172 282d 2d73 792d 632d 7375  or:var(--sy-c-su
-00035020: 7266 6163 6529 3b66 6f6e 742d 6661 6d69  rface);font-fami
-00035030: 6c79 3a76 6172 282d 2d73 792d 662d 7465  ly:var(--sy-f-te
-00035040: 7874 297d 2e73 792d 6c73 6964 6520 2e72  xt)}.sy-lside .r
-00035050: 7374 2d76 6572 7369 6f6e 7320 617b 636f  st-versions a{co
-00035060: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d6c  lor:var(--sy-c-l
-00035070: 696e 6b29 7d2e 7379 2d6c 7369 6465 202e  ink)}.sy-lside .
-00035080: 7273 742d 7665 7273 696f 6e73 2061 3a68  rst-versions a:h
-00035090: 6f76 6572 7b63 6f6c 6f72 3a76 6172 282d  over{color:var(-
-000350a0: 2d73 792d 632d 6c69 6e6b 2d68 6f76 6572  -sy-c-link-hover
-000350b0: 297d 2e73 792d 6c73 6964 6520 2e72 7374  )}.sy-lside .rst
-000350c0: 2d76 6572 7369 6f6e 7320 2e72 7374 2d63  -versions .rst-c
-000350d0: 7572 7265 6e74 2d76 6572 7369 6f6e 7b62  urrent-version{b
-000350e0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-000350f0: 7661 7228 2d2d 7379 2d63 2d62 6163 6b67  var(--sy-c-backg
-00035100: 726f 756e 6429 3b63 6f6c 6f72 3a76 6172  round);color:var
-00035110: 282d 2d73 792d 632d 7465 7874 293b 7061  (--sy-c-text);pa
-00035120: 6464 696e 673a 3020 3172 656d 3b68 6569  dding:0 1rem;hei
-00035130: 6768 743a 7661 7228 2d2d 6865 6967 6874  ght:var(--height
-00035140: 293b 6c69 6e65 2d68 6569 6768 743a 7661  );line-height:va
-00035150: 7228 2d2d 6865 6967 6874 297d 2e73 792d  r(--height)}.sy-
-00035160: 6c73 6964 6520 2e72 7374 2d76 6572 7369  lside .rst-versi
-00035170: 6f6e 732e 7273 742d 6261 6467 6520 2e72  ons.rst-badge .r
-00035180: 7374 2d63 7572 7265 6e74 2d76 6572 7369  st-current-versi
-00035190: 6f6e 7b74 6578 742d 616c 6967 6e3a 6c65  on{text-align:le
-000351a0: 6674 3b66 6f6e 742d 7369 7a65 3a2e 3934  ft;font-size:.94
-000351b0: 7265 6d3b 7061 6464 696e 673a 3020 3172  rem;padding:0 1r
-000351c0: 656d 3b68 6569 6768 743a 7661 7228 2d2d  em;height:var(--
-000351d0: 6865 6967 6874 293b 6c69 6e65 2d68 6569  height);line-hei
-000351e0: 6768 743a 7661 7228 2d2d 6865 6967 6874  ght:var(--height
-000351f0: 297d 2e73 792d 6c73 6964 6520 2e72 7374  )}.sy-lside .rst
-00035200: 2d76 6572 7369 6f6e 7320 2e72 7374 2d63  -versions .rst-c
-00035210: 7572 7265 6e74 2d76 6572 7369 6f6e 202e  urrent-version .
-00035220: 6661 7b63 6f6c 6f72 3a76 6172 282d 2d73  fa{color:var(--s
-00035230: 792d 632d 7465 7874 297d 2e73 792d 6c73  y-c-text)}.sy-ls
-00035240: 6964 6520 2e72 7374 2d76 6572 7369 6f6e  ide .rst-version
-00035250: 732e 7273 742d 6261 6467 652e 7368 6966  s.rst-badge.shif
-00035260: 742d 7570 202e 7273 742d 6375 7272 656e  t-up .rst-curren
-00035270: 742d 7665 7273 696f 6e7b 7465 7874 2d61  t-version{text-a
-00035280: 6c69 676e 3a6c 6566 747d 2e73 792d 6c73  lign:left}.sy-ls
-00035290: 6964 6520 2e72 7374 2d76 6572 7369 6f6e  ide .rst-version
-000352a0: 732e 7273 742d 6261 6467 652e 7368 6966  s.rst-badge.shif
-000352b0: 742d 7570 202e 7273 742d 6375 7272 656e  t-up .rst-curren
-000352c0: 742d 7665 7273 696f 6e20 2e66 612d 626f  t-version .fa-bo
-000352d0: 6f6b 7b66 6c6f 6174 3a6e 6f6e 657d 2e73  ok{float:none}.s
-000352e0: 792d 6c73 6964 6520 2e72 7374 2d6f 7468  y-lside .rst-oth
-000352f0: 6572 2d76 6572 7369 6f6e 737b 666f 6e74  er-versions{font
-00035300: 2d73 697a 653a 2e38 3672 656d 3b62 6f72  -size:.86rem;bor
-00035310: 6465 722d 746f 703a 3170 7820 736f 6c69  der-top:1px soli
-00035320: 6420 7661 7228 2d2d 7379 2d63 2d64 6976  d var(--sy-c-div
-00035330: 6964 6572 297d 2e73 792d 6c73 6964 6520  ider)}.sy-lside 
-00035340: 2e72 7374 2d6f 7468 6572 2d76 6572 7369  .rst-other-versi
-00035350: 6f6e 7320 6474 7b66 6f6e 742d 7369 7a65  ons dt{font-size
-00035360: 3a2e 3638 7265 6d3b 666f 6e74 2d77 6569  :.68rem;font-wei
-00035370: 6768 743a 3530 303b 7061 6464 696e 673a  ght:500;padding:
-00035380: 3470 7820 3670 783b 636f 6c6f 723a 7661  4px 6px;color:va
-00035390: 7228 2d2d 7379 2d63 2d6c 6967 6874 297d  r(--sy-c-light)}
-000353a0: 2e73 792d 6c73 6964 6520 2e72 7374 2d76  .sy-lside .rst-v
-000353b0: 6572 7369 6f6e 7320 2e72 7374 2d6f 7468  ersions .rst-oth
-000353c0: 6572 2d76 6572 7369 6f6e 7320 6464 2061  er-versions dd a
-000353d0: 7b63 6f6c 6f72 3a76 6172 282d 2d73 792d  {color:var(--sy-
-000353e0: 632d 7465 7874 297d 2e73 792d 6c73 6964  c-text)}.sy-lsid
-000353f0: 6520 2e72 7374 2d76 6572 7369 6f6e 7320  e .rst-versions 
-00035400: 2e72 7374 2d6f 7468 6572 2d76 6572 7369  .rst-other-versi
-00035410: 6f6e 7320 6464 2061 3a68 6f76 6572 7b74  ons dd a:hover{t
-00035420: 6578 742d 6465 636f 7261 7469 6f6e 3a75  ext-decoration:u
-00035430: 6e64 6572 6c69 6e65 3b63 6f6c 6f72 3a76  nderline;color:v
-00035440: 6172 282d 2d73 792d 632d 6c69 6e6b 2d68  ar(--sy-c-link-h
-00035450: 6f76 6572 297d 2e73 792d 6c73 6964 6520  over)}.sy-lside 
-00035460: 2e72 7374 2d76 6572 7369 6f6e 7320 696e  .rst-versions in
-00035470: 7075 747b 7769 6474 683a 3130 3025 3b70  put{width:100%;p
-00035480: 6164 6469 6e67 3a36 7078 2031 3270 783b  adding:6px 12px;
-00035490: 666f 6e74 2d73 697a 653a 2e39 3272 656d  font-size:.92rem
-000354a0: 3b66 6f6e 742d 6661 6d69 6c79 3a76 6172  ;font-family:var
-000354b0: 282d 2d73 792d 662d 7465 7874 293b 626f  (--sy-f-text);bo
-000354c0: 7264 6572 2d72 6164 6975 733a 3670 783b  rder-radius:6px;
-000354d0: 6f75 746c 696e 653a 303b 6261 636b 6772  outline:0;backgr
-000354e0: 6f75 6e64 3a76 6172 282d 2d73 792d 632d  ound:var(--sy-c-
-000354f0: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
-00035500: 6572 3a31 7078 2073 6f6c 6964 2076 6172  er:1px solid var
-00035510: 282d 2d73 792d 632d 626f 7264 6572 297d  (--sy-c-border)}
-00035520: 2e73 792d 6c73 6964 6520 2e72 7374 2d76  .sy-lside .rst-v
-00035530: 6572 7369 6f6e 7320 2e72 7374 2d6f 7468  ersions .rst-oth
-00035540: 6572 2d76 6572 7369 6f6e 7320 6872 7b62  er-versions hr{b
-00035550: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
-00035560: 2d2d 7379 2d63 2d64 6976 6964 6572 297d  --sy-c-divider)}
-00035570: 406d 6564 6961 2028 6d69 6e2d 7769 6474  @media (min-widt
-00035580: 683a 3930 7265 6d29 7b2e 7379 2d6c 7369  h:90rem){.sy-lsi
-00035590: 6465 202e 7273 742d 7665 7273 696f 6e73  de .rst-versions
-000355a0: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
-000355b0: 2d2d 7379 2d63 2d62 6163 6b67 726f 756e  --sy-c-backgroun
-000355c0: 6429 7d7d 2e79 7565 2062 7574 746f 6e2e  d)}}.yue button.
-000355d0: 636f 7079 6274 6e7b 616c 6967 6e2d 6974  copybtn{align-it
-000355e0: 656d 733a 6365 6e74 6572 3b6a 7573 7469  ems:center;justi
-000355f0: 6679 2d63 6f6e 7465 6e74 3a63 656e 7465  fy-content:cente
-00035600: 723b 6261 636b 6772 6f75 6e64 2d63 6f6c  r;background-col
-00035610: 6f72 3a69 6e69 7469 616c 3b62 6f72 6465  or:initial;borde
-00035620: 723a 6e6f 6e65 3b63 6f6c 6f72 3a76 6172  r:none;color:var
-00035630: 282d 2d73 796e 7461 782d 7465 7874 297d  (--syntax-text)}
-00035640: 2e79 7565 2062 7574 746f 6e2e 636f 7079  .yue button.copy
-00035650: 6274 6e3e 7376 677b 7769 6474 683a 312e  btn>svg{width:1.
-00035660: 3472 656d 3b68 6569 6768 743a 312e 3472  4rem;height:1.4r
-00035670: 656d 7d2e 7975 6520 6275 7474 6f6e 2e63  em}.yue button.c
-00035680: 6f70 7962 746e 3a68 6f76 6572 7b63 6f6c  opybtn:hover{col
-00035690: 6f72 3a76 6172 282d 2d73 796e 7461 782d  or:var(--syntax-
-000356a0: 6d65 7461 297d 2e79 7565 202e 6869 6768  meta)}.yue .high
-000356b0: 6c69 6768 7420 6275 7474 6f6e 2e63 6f70  light button.cop
-000356c0: 7962 746e 3a68 6f76 6572 7b62 6163 6b67  ybtn:hover{backg
-000356d0: 726f 756e 642d 636f 6c6f 723a 696e 6974  round-color:init
-000356e0: 6961 6c7d 2e79 7565 2062 7574 746f 6e2e  ial}.yue button.
-000356f0: 636f 7079 6274 6e3a 6166 7465 727b 6261  copybtn:after{ba
-00035700: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a69  ckground-color:i
-00035710: 6e69 7469 616c 3b63 6f6c 6f72 3a76 6172  nitial;color:var
-00035720: 282d 2d73 796e 7461 782d 7465 7874 297d  (--syntax-text)}
-00035730: 2e79 7565 2062 7574 746f 6e2e 636f 7079  .yue button.copy
-00035740: 6274 6e2e 7375 6363 6573 737b 626f 7264  btn.success{bord
-00035750: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d67  er-color:var(--g
-00035760: 7265 656e 2d61 3130 293b 636f 6c6f 723a  reen-a10);color:
-00035770: 7661 7228 2d2d 6772 6565 6e2d 6131 3029  var(--green-a10)
-00035780: 7d2e 7975 6520 6275 7474 6f6e 2e63 6f70  }.yue button.cop
-00035790: 7962 746e 2e73 7563 6365 7373 3a61 6674  ybtn.success:aft
-000357a0: 6572 7b63 6f6c 6f72 3a76 6172 282d 2d67  er{color:var(--g
-000357b0: 7265 656e 2d61 3130 297d 2e79 7565 7b2d  reen-a10)}.yue{-
-000357c0: 2d73 642d 636f 6c6f 722d 7072 696d 6172  -sd-color-primar
-000357d0: 793a 7661 7228 2d2d 6163 6365 6e74 2d61  y:var(--accent-a
-000357e0: 3131 293b 2d2d 7364 2d63 6f6c 6f72 2d73  11);--sd-color-s
-000357f0: 6563 6f6e 6461 7279 3a76 6172 282d 2d67  econdary:var(--g
-00035800: 6f6c 642d 6131 3129 3b2d 2d73 642d 636f  old-a11);--sd-co
-00035810: 6c6f 722d 7375 6363 6573 733a 7661 7228  lor-success:var(
-00035820: 2d2d 6772 6565 6e2d 6131 3129 3b2d 2d73  --green-a11);--s
-00035830: 642d 636f 6c6f 722d 696e 666f 3a76 6172  d-color-info:var
-00035840: 282d 2d62 6c75 652d 6131 3129 3b2d 2d73  (--blue-a11);--s
-00035850: 642d 636f 6c6f 722d 7761 726e 696e 673a  d-color-warning:
-00035860: 7661 7228 2d2d 6f72 616e 6765 2d61 3131  var(--orange-a11
-00035870: 293b 2d2d 7364 2d63 6f6c 6f72 2d64 616e  );--sd-color-dan
-00035880: 6765 723a 7661 7228 2d2d 7265 642d 6131  ger:var(--red-a1
-00035890: 3129 3b2d 2d73 642d 636f 6c6f 722d 6c69  1);--sd-color-li
-000358a0: 6768 743a 7661 7228 2d2d 7361 6e64 2d61  ght:var(--sand-a
-000358b0: 3229 3b2d 2d73 642d 636f 6c6f 722d 6d75  2);--sd-color-mu
-000358c0: 7465 643a 7661 7228 2d2d 6772 6179 2d38  ted:var(--gray-8
-000358d0: 293b 2d2d 7364 2d63 6f6c 6f72 2d64 6172  );--sd-color-dar
-000358e0: 6b3a 2332 3132 3132 323b 2d2d 7364 2d63  k:#212122;--sd-c
-000358f0: 6f6c 6f72 2d62 6c61 636b 3a23 3030 303b  olor-black:#000;
-00035900: 2d2d 7364 2d63 6f6c 6f72 2d77 6869 7465  --sd-color-white
-00035910: 3a23 6666 663b 2d2d 7364 2d63 6f6c 6f72  :#fff;--sd-color
-00035920: 2d70 7269 6d61 7279 2d68 6967 686c 6967  -primary-highlig
-00035930: 6874 3a76 6172 282d 2d61 6363 656e 742d  ht:var(--accent-
-00035940: 6138 293b 2d2d 7364 2d63 6f6c 6f72 2d73  a8);--sd-color-s
-00035950: 6563 6f6e 6461 7279 2d68 6967 686c 6967  econdary-highlig
-00035960: 6874 3a76 6172 282d 2d67 6f6c 642d 6138  ht:var(--gold-a8
-00035970: 293b 2d2d 7364 2d63 6f6c 6f72 2d73 7563  );--sd-color-suc
-00035980: 6365 7373 2d68 6967 686c 6967 6874 3a76  cess-highlight:v
-00035990: 6172 282d 2d67 7265 656e 2d61 3829 3b2d  ar(--green-a8);-
-000359a0: 2d73 642d 636f 6c6f 722d 696e 666f 2d68  -sd-color-info-h
-000359b0: 6967 686c 6967 6874 3a76 6172 282d 2d62  ighlight:var(--b
-000359c0: 6c75 652d 6138 293b 2d2d 7364 2d63 6f6c  lue-a8);--sd-col
-000359d0: 6f72 2d77 6172 6e69 6e67 2d68 6967 686c  or-warning-highl
-000359e0: 6967 6874 3a76 6172 282d 2d6f 7261 6e67  ight:var(--orang
-000359f0: 652d 6138 293b 2d2d 7364 2d63 6f6c 6f72  e-a8);--sd-color
-00035a00: 2d64 616e 6765 722d 6869 6768 6c69 6768  -danger-highligh
-00035a10: 743a 7661 7228 2d2d 7265 642d 6138 293b  t:var(--red-a8);
-00035a20: 2d2d 7364 2d63 6f6c 6f72 2d6c 6967 6874  --sd-color-light
-00035a30: 2d68 6967 686c 6967 6874 3a76 6172 282d  -highlight:var(-
-00035a40: 2d67 7261 792d 3429 3b2d 2d73 642d 636f  -gray-4);--sd-co
-00035a50: 6c6f 722d 6d75 7465 642d 6869 6768 6c69  lor-muted-highli
-00035a60: 6768 743a 7661 7228 2d2d 6772 6179 2d31  ght:var(--gray-1
-00035a70: 3129 3b2d 2d73 642d 636f 6c6f 722d 6461  1);--sd-color-da
-00035a80: 726b 2d68 6967 686c 6967 6874 3a23 3132  rk-highlight:#12
-00035a90: 3132 3131 3b2d 2d73 642d 636f 6c6f 722d  1211;--sd-color-
-00035aa0: 626c 6163 6b2d 6869 6768 6c69 6768 743a  black-highlight:
-00035ab0: 2330 3030 3b2d 2d73 642d 636f 6c6f 722d  #000;--sd-color-
-00035ac0: 7768 6974 652d 6869 6768 6c69 6768 743a  white-highlight:
-00035ad0: 2364 3964 3964 393b 2d2d 7364 2d63 6f6c  #d9d9d9;--sd-col
-00035ae0: 6f72 2d70 7269 6d61 7279 2d74 6578 743a  or-primary-text:
-00035af0: 7661 7228 2d2d 6163 6365 6e74 2d39 2d63  var(--accent-9-c
-00035b00: 6f6e 7472 6173 7429 3b2d 2d73 642d 636f  ontrast);--sd-co
-00035b10: 6c6f 722d 7365 636f 6e64 6172 792d 7465  lor-secondary-te
-00035b20: 7874 3a76 6172 282d 2d67 6f6c 642d 392d  xt:var(--gold-9-
-00035b30: 636f 6e74 7261 7374 293b 2d2d 7364 2d63  contrast);--sd-c
-00035b40: 6f6c 6f72 2d73 7563 6365 7373 2d74 6578  olor-success-tex
-00035b50: 743a 7661 7228 2d2d 6772 6565 6e2d 392d  t:var(--green-9-
-00035b60: 636f 6e74 7261 7374 293b 2d2d 7364 2d63  contrast);--sd-c
-00035b70: 6f6c 6f72 2d69 6e66 6f2d 7465 7874 3a76  olor-info-text:v
-00035b80: 6172 282d 2d62 6c75 652d 392d 636f 6e74  ar(--blue-9-cont
-00035b90: 7261 7374 293b 2d2d 7364 2d63 6f6c 6f72  rast);--sd-color
-00035ba0: 2d77 6172 6e69 6e67 2d74 6578 743a 7661  -warning-text:va
-00035bb0: 7228 2d2d 6f72 616e 6765 2d39 2d63 6f6e  r(--orange-9-con
-00035bc0: 7472 6173 7429 3b2d 2d73 642d 636f 6c6f  trast);--sd-colo
-00035bd0: 722d 6461 6e67 6572 2d74 6578 743a 7661  r-danger-text:va
-00035be0: 7228 2d2d 7265 642d 392d 636f 6e74 7261  r(--red-9-contra
-00035bf0: 7374 293b 2d2d 7364 2d63 6f6c 6f72 2d6c  st);--sd-color-l
-00035c00: 6967 6874 2d74 6578 743a 7661 7228 2d2d  ight-text:var(--
-00035c10: 7379 2d63 2d74 6578 7429 3b2d 2d73 642d  sy-c-text);--sd-
-00035c20: 636f 6c6f 722d 6d75 7465 642d 7465 7874  color-muted-text
-00035c30: 3a23 6666 663b 2d2d 7364 2d63 6f6c 6f72  :#fff;--sd-color
-00035c40: 2d64 6172 6b2d 7465 7874 3a23 6666 663b  -dark-text:#fff;
-00035c50: 2d2d 7364 2d63 6f6c 6f72 2d62 6c61 636b  --sd-color-black
-00035c60: 2d74 6578 743a 2366 6666 3b2d 2d73 642d  -text:#fff;--sd-
-00035c70: 636f 6c6f 722d 7768 6974 652d 7465 7874  color-white-text
-00035c80: 3a23 3231 3235 3239 3b2d 2d73 642d 636f  :#212529;--sd-co
-00035c90: 6c6f 722d 7368 6164 6f77 3a76 6172 282d  lor-shadow:var(-
-00035ca0: 2d67 7261 792d 3129 3b2d 2d73 642d 636f  -gray-1);--sd-co
-00035cb0: 6c6f 722d 6361 7264 2d62 6f72 6465 723a  lor-card-border:
-00035cc0: 7661 7228 2d2d 7379 2d63 2d62 6f72 6465  var(--sy-c-borde
-00035cd0: 7229 3b2d 2d73 642d 636f 6c6f 722d 6361  r);--sd-color-ca
-00035ce0: 7264 2d62 6f72 6465 722d 686f 7665 723a  rd-border-hover:
-00035cf0: 7661 7228 2d2d 6163 6365 6e74 2d61 3929  var(--accent-a9)
-00035d00: 3b2d 2d73 642d 636f 6c6f 722d 7461 6273  ;--sd-color-tabs
-00035d10: 2d6c 6162 656c 2d69 6e61 6374 6976 653a  -label-inactive:
-00035d20: 7661 7228 2d2d 7379 2d63 2d62 6f6c 6429  var(--sy-c-bold)
-00035d30: 3b2d 2d73 642d 636f 6c6f 722d 7461 6273  ;--sd-color-tabs
-00035d40: 2d6c 6162 656c 2d61 6374 6976 653a 7661  -label-active:va
-00035d50: 7228 2d2d 7364 2d63 6f6c 6f72 2d70 7269  r(--sd-color-pri
-00035d60: 6d61 7279 293b 2d2d 7364 2d63 6f6c 6f72  mary);--sd-color
-00035d70: 2d74 6162 732d 756e 6465 726c 696e 652d  -tabs-underline-
-00035d80: 6163 7469 7665 3a76 6172 282d 2d73 642d  active:var(--sd-
-00035d90: 636f 6c6f 722d 7072 696d 6172 7929 3b2d  color-primary);-
-00035da0: 2d73 642d 636f 6c6f 722d 7461 6273 2d6c  -sd-color-tabs-l
-00035db0: 6162 656c 2d68 6f76 6572 3a76 6172 282d  abel-hover:var(-
-00035dc0: 2d61 6363 656e 742d 3929 3b2d 2d73 642d  -accent-9);--sd-
-00035dd0: 636f 6c6f 722d 7461 6273 2d75 6e64 6572  color-tabs-under
-00035de0: 6c69 6e65 2d68 6f76 6572 3a76 6172 282d  line-hover:var(-
-00035df0: 2d61 6363 656e 742d 3929 7d2e 7975 6520  -accent-9)}.yue 
-00035e00: 2e73 7572 6661 6365 7b2d 2d73 642d 636f  .surface{--sd-co
-00035e10: 6c6f 722d 6361 7264 2d74 6578 743a 7661  lor-card-text:va
-00035e20: 7228 2d2d 7379 2d63 2d6c 6967 6874 293b  r(--sy-c-light);
-00035e30: 2d2d 7364 2d63 6f6c 6f72 2d63 6172 642d  --sd-color-card-
-00035e40: 626f 7264 6572 3a23 3030 3030 3b2d 2d73  border:#0000;--s
-00035e50: 642d 636f 6c6f 722d 6361 7264 2d62 6163  d-color-card-bac
-00035e60: 6b67 726f 756e 643a 7661 7228 2d2d 7379  kground:var(--sy
-00035e70: 2d63 2d73 7572 6661 6365 297d 2e79 7565  -c-surface)}.yue
-00035e80: 2061 2e73 642d 6261 6467 652c 2e79 7565   a.sd-badge,.yue
-00035e90: 2061 2e73 642d 6261 6467 653a 686f 7665   a.sd-badge:hove
-00035ea0: 727b 626f 7264 6572 2d62 6f74 746f 6d3a  r{border-bottom:
-00035eb0: 307d 2e79 7565 202e 7364 2d62 6164 6765  0}.yue .sd-badge
-00035ec0: 7b66 6f6e 742d 7765 6967 6874 3a36 3030  {font-weight:600
-00035ed0: 3b62 6f72 6465 722d 7261 6469 7573 3a33  ;border-radius:3
-00035ee0: 7078 7d2e 7975 6520 2e73 642d 6274 6e7b  px}.yue .sd-btn{
-00035ef0: 626f 7264 6572 2d63 6f6c 6f72 3a76 6172  border-color:var
-00035f00: 282d 2d73 792d 632d 626f 7264 6572 297d  (--sy-c-border)}
-00035f10: 2e79 7565 202e 7364 2d74 6162 2d73 6574  .yue .sd-tab-set
-00035f20: 3e6c 6162 656c 7b70 6164 6469 6e67 3a31  >label{padding:1
-00035f30: 7265 6d20 2e32 3572 656d 202e 3572 656d  rem .25rem .5rem
-00035f40: 3b66 6f6e 742d 7369 7a65 3a2e 3834 7265  ;font-size:.84re
-00035f50: 6d3b 666f 6e74 2d77 6569 6768 743a 3530  m;font-weight:50
-00035f60: 307d 2e79 7565 202e 7364 2d74 6162 2d73  0}.yue .sd-tab-s
-00035f70: 6574 3e6c 6162 656c 7e6c 6162 656c 7b6d  et>label~label{m
-00035f80: 6172 6769 6e2d 6c65 6674 3a31 7265 6d7d  argin-left:1rem}
-00035f90: 2e79 7565 202e 7364 2d74 6162 2d63 6f6e  .yue .sd-tab-con
-00035fa0: 7465 6e74 7b70 6164 6469 6e67 3a30 3b62  tent{padding:0;b
-00035fb0: 6f78 2d73 6861 646f 773a 3020 2d2e 3036  ox-shadow:0 -.06
-00035fc0: 3235 7265 6d20 7661 7228 2d2d 7379 2d63  25rem var(--sy-c
-00035fd0: 2d64 6976 6964 6572 297d 2e79 7565 202e  -divider)}.yue .
-00035fe0: 7364 2d74 6162 2d63 6f6e 7465 6e74 202e  sd-tab-content .
-00035ff0: 636f 6465 2d62 6c6f 636b 2d63 6170 7469  code-block-capti
-00036000: 6f6e 2c2e 7975 6520 2e73 642d 7461 622d  on,.yue .sd-tab-
-00036010: 636f 6e74 656e 7420 2e68 6967 686c 6967  content .highlig
-00036020: 6874 2070 7265 7b62 6f72 6465 722d 7261  ht pre{border-ra
-00036030: 6469 7573 3a30 7d2e 7975 6520 2e73 642d  dius:0}.yue .sd-
-00036040: 6361 7264 2d74 6974 6c65 7b63 6f6c 6f72  card-title{color
-00036050: 3a76 6172 282d 2d73 792d 632d 7465 7874  :var(--sy-c-text
-00036060: 297d 2e79 7565 202e 7364 2d63 6172 642d  )}.yue .sd-card-
-00036070: 7469 746c 653e 7376 677b 706f 7369 7469  title>svg{positi
-00036080: 6f6e 3a72 656c 6174 6976 653b 746f 703a  on:relative;top:
-00036090: 2d31 7078 3b6d 6172 6769 6e2d 7269 6768  -1px;margin-righ
-000360a0: 743a 2e32 3572 656d 7d2e 7975 6520 2e73  t:.25rem}.yue .s
-000360b0: 642d 6361 7264 2d68 6f76 6572 3a68 6f76  d-card-hover:hov
-000360c0: 6572 7b74 7261 6e73 666f 726d 3a73 6361  er{transform:sca
-000360d0: 6c65 2831 297d 2e79 7565 202e 7364 2d63  le(1)}.yue .sd-c
-000360e0: 6172 642d 686f 7665 723a 686f 7665 7220  ard-hover:hover 
-000360f0: 2e73 642d 6361 7264 2d74 6974 6c65 7b63  .sd-card-title{c
-00036100: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-00036110: 6c69 6e6b 2d68 6f76 6572 297d 2e79 7565  link-hover)}.yue
-00036120: 202e 7364 2d63 6172 6420 612c 2e79 7565   .sd-card a,.yue
-00036130: 202e 7364 2d63 6172 6420 613a 686f 7665   .sd-card a:hove
-00036140: 727b 626f 7264 6572 2d62 6f74 746f 6d3a  r{border-bottom:
-00036150: 307d 2e79 7565 202e 7375 7266 6163 6520  0}.yue .surface 
-00036160: 2e73 642d 6361 7264 2d62 6f64 792c 2e79  .sd-card-body,.y
-00036170: 7565 202e 7375 7266 6163 6520 2e73 642d  ue .surface .sd-
-00036180: 6361 7264 2d66 6f6f 7465 722c 2e79 7565  card-footer,.yue
-00036190: 202e 7375 7266 6163 6520 2e73 642d 6361   .surface .sd-ca
-000361a0: 7264 2d68 6561 6465 727b 7061 6464 696e  rd-header{paddin
-000361b0: 672d 6c65 6674 3a31 2e35 7265 6d3b 7061  g-left:1.5rem;pa
-000361c0: 6464 696e 672d 7269 6768 743a 312e 3572  dding-right:1.5r
-000361d0: 656d 7d2e 7975 6520 2e73 7572 6661 6365  em}.yue .surface
-000361e0: 202e 7364 2d63 6172 642d 666f 6f74 6572   .sd-card-footer
-000361f0: 2c2e 7975 6520 2e73 7572 6661 6365 202e  ,.yue .surface .
-00036200: 7364 2d63 6172 642d 6865 6164 6572 7b62  sd-card-header{b
-00036210: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
-00036220: 2d2d 7379 2d63 2d62 6f72 6465 7229 7d40  --sy-c-border)}@
-00036230: 6d65 6469 6120 2870 7269 6e74 297b 2e79  media (print){.y
-00036240: 7565 202e 7364 2d63 6172 647b 7061 6765  ue .sd-card{page
-00036250: 2d62 7265 616b 2d69 6e73 6964 653a 6176  -break-inside:av
-00036260: 6f69 647d 7d2e 7975 6520 612e 7364 2d74  oid}}.yue a.sd-t
-00036270: 6578 742d 7772 6170 3a68 6f76 6572 7b62  ext-wrap:hover{b
-00036280: 6f72 6465 722d 626f 7474 6f6d 2d77 6964  order-bottom-wid
-00036290: 7468 3a31 7078 7d2e 7370 6869 6e78 2d74  th:1px}.sphinx-t
-000362a0: 6162 7320 5b72 6f6c 653d 7461 626c 6973  abs [role=tablis
-000362b0: 745d 7b62 6f72 6465 722d 636f 6c6f 723a  t]{border-color:
-000362c0: 7661 7228 2d2d 7379 2d63 2d64 6976 6964  var(--sy-c-divid
-000362d0: 6572 297d 2e79 7565 202e 7370 6869 6e78  er)}.yue .sphinx
-000362e0: 2d74 6162 732d 7461 627b 636f 6c6f 723a  -tabs-tab{color:
-000362f0: 7661 7228 2d2d 7379 2d63 2d74 6578 7429  var(--sy-c-text)
-00036300: 3b6c 696e 652d 6865 6967 6874 3a69 6e68  ;line-height:inh
-00036310: 6572 6974 3b70 6164 6469 6e67 3a31 7265  erit;padding:1re
-00036320: 6d20 2e32 3572 656d 202e 3572 656d 3b66  m .25rem .5rem;f
-00036330: 6f6e 742d 7369 7a65 3a2e 3834 7265 6d3b  ont-size:.84rem;
-00036340: 666f 6e74 2d77 6569 6768 743a 3530 303b  font-weight:500;
-00036350: 626f 7264 6572 3a6e 6f6e 653b 626f 7264  border:none;bord
-00036360: 6572 2d62 6f74 746f 6d3a 2e31 3235 7265  er-bottom:.125re
-00036370: 6d20 736f 6c69 6420 2330 3030 307d 2e79  m solid #0000}.y
-00036380: 7565 202e 7370 6869 6e78 2d74 6162 732d  ue .sphinx-tabs-
-00036390: 7461 623a 686f 7665 727b 636f 6c6f 723a  tab:hover{color:
-000363a0: 7661 7228 2d2d 7364 2d63 6f6c 6f72 2d74  var(--sd-color-t
-000363b0: 6162 732d 6c61 6265 6c2d 686f 7665 7229  abs-label-hover)
-000363c0: 3b62 6f72 6465 722d 636f 6c6f 723a 7661  ;border-color:va
-000363d0: 7228 2d2d 7364 2d63 6f6c 6f72 2d74 6162  r(--sd-color-tab
-000363e0: 732d 756e 6465 726c 696e 652d 686f 7665  s-underline-hove
-000363f0: 7229 7d2e 7975 6520 2e73 7068 696e 782d  r)}.yue .sphinx-
-00036400: 7461 6273 2d74 6162 5b61 7269 612d 7365  tabs-tab[aria-se
-00036410: 6c65 6374 6564 3d74 7275 655d 7b62 6f72  lected=true]{bor
-00036420: 6465 723a 6e6f 6e65 3b62 6f72 6465 722d  der:none;border-
-00036430: 626f 7474 6f6d 3a2e 3132 3572 656d 2073  bottom:.125rem s
-00036440: 6f6c 6964 2076 6172 282d 2d73 642d 636f  olid var(--sd-co
-00036450: 6c6f 722d 7461 6273 2d75 6e64 6572 6c69  lor-tabs-underli
-00036460: 6e65 2d61 6374 6976 6529 3b63 6f6c 6f72  ne-active);color
-00036470: 3a76 6172 282d 2d73 642d 636f 6c6f 722d  :var(--sd-color-
-00036480: 7461 6273 2d6c 6162 656c 2d61 6374 6976  tabs-label-activ
-00036490: 6529 3b62 6163 6b67 726f 756e 642d 636f  e);background-co
-000364a0: 6c6f 723a 696e 6974 6961 6c7d 2e79 7565  lor:initial}.yue
-000364b0: 202e 7370 6869 6e78 2d74 6162 732d 7461   .sphinx-tabs-ta
-000364c0: 622b 2e73 7068 696e 782d 7461 6273 2d74  b+.sphinx-tabs-t
-000364d0: 6162 7b6d 6172 6769 6e2d 6c65 6674 3a31  ab{margin-left:1
-000364e0: 7265 6d7d 2e79 7565 202e 7370 6869 6e78  rem}.yue .sphinx
-000364f0: 2d74 6162 732d 7061 6e65 6c7b 626f 7264  -tabs-panel{bord
-00036500: 6572 3a6e 6f6e 653b 7061 6464 696e 673a  er:none;padding:
-00036510: 303b 6d61 7267 696e 3a30 3b62 6f72 6465  0;margin:0;borde
-00036520: 722d 7261 6469 7573 3a30 3b62 6163 6b67  r-radius:0;backg
-00036530: 726f 756e 642d 636f 6c6f 723a 696e 6974  round-color:init
-00036540: 6961 6c7d 2e79 7565 202e 7370 6869 6e78  ial}.yue .sphinx
-00036550: 2d74 6162 732d 7061 6e65 6c2e 636f 6465  -tabs-panel.code
-00036560: 2d74 6162 7b70 6164 6469 6e67 3a30 7d2e  -tab{padding:0}.
-00036570: 7975 6520 2e73 7068 696e 782d 7461 6273  yue .sphinx-tabs
-00036580: 2d70 616e 656c 2e63 6f64 652d 7461 6220  -panel.code-tab 
-00036590: 2e63 6f64 652d 626c 6f63 6b2d 6361 7074  .code-block-capt
-000365a0: 696f 6e2c 2e79 7565 202e 7370 6869 6e78  ion,.yue .sphinx
-000365b0: 2d74 6162 732d 7061 6e65 6c2e 636f 6465  -tabs-panel.code
-000365c0: 2d74 6162 202e 6869 6768 6c69 6768 7420  -tab .highlight 
-000365d0: 7072 657b 626f 7264 6572 2d72 6164 6975  pre{border-radiu
-000365e0: 733a 307d 2e79 7565 7b2d 2d6a 702d 7769  s:0}.yue{--jp-wi
-000365f0: 6467 6574 732d 696e 7075 742d 626f 7264  dgets-input-bord
-00036600: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d67  er-color:var(--g
-00036610: 7261 792d 3529 3b2d 2d6a 702d 7769 6467  ray-5);--jp-widg
-00036620: 6574 732d 696e 7075 742d 666f 6375 732d  ets-input-focus-
-00036630: 626f 7264 6572 2d63 6f6c 6f72 3a76 6172  border-color:var
-00036640: 282d 2d67 7261 792d 3829 3b2d 2d6a 702d  (--gray-8);--jp-
-00036650: 7769 6467 6574 732d 736c 6964 6572 2d61  widgets-slider-a
-00036660: 6374 6976 652d 6861 6e64 6c65 2d63 6f6c  ctive-handle-col
-00036670: 6f72 3a76 6172 282d 2d67 7261 792d 3429  or:var(--gray-4)
-00036680: 3b2d 2d6a 702d 7769 6467 6574 732d 736c  ;--jp-widgets-sl
-00036690: 6964 6572 2d68 616e 646c 652d 626f 7264  ider-handle-bord
-000366a0: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d73  er-color:var(--s
-000366b0: 792d 632d 626f 7264 6572 297d 2e79 7565  y-c-border)}.yue
-000366c0: 202e 6a75 7079 7465 725f 636f 6e74 6169   .jupyter_contai
-000366d0: 6e65 727b 6261 636b 6772 6f75 6e64 2d63  ner{background-c
-000366e0: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-000366f0: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
-00036700: 6572 3a33 7078 2073 6f6c 6964 2076 6172  er:3px solid var
-00036710: 282d 2d73 792d 632d 626f 7264 6572 293b  (--sy-c-border);
-00036720: 626f 7264 6572 2d72 6164 6975 733a 3670  border-radius:6p
-00036730: 783b 6f76 6572 666c 6f77 3a68 6964 6465  x;overflow:hidde
-00036740: 6e3b 626f 782d 7368 6164 6f77 3a6e 6f6e  n;box-shadow:non
-00036750: 657d 2e64 6f63 756d 656e 7420 2e79 7565  e}.document .yue
-00036760: 202e 6a75 7079 7465 725f 636f 6e74 6169   .jupyter_contai
-00036770: 6e65 7220 6469 765b 636c 6173 735e 3d68  ner div[class^=h
-00036780: 6967 686c 6967 6874 5d7b 7061 6464 696e  ighlight]{paddin
-00036790: 673a 307d 2e79 7565 202e 6a75 7079 7465  g:0}.yue .jupyte
-000367a0: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
-000367b0: 6365 6c6c 5f69 6e70 7574 7b62 6163 6b67  cell_input{backg
-000367c0: 726f 756e 642d 636f 6c6f 723a 7661 7228  round-color:var(
-000367d0: 2d2d 7379 6e74 6178 2d70 7265 2d62 6729  --syntax-pre-bg)
-000367e0: 3b62 6f72 6465 723a 303b 626f 7264 6572  ;border:0;border
-000367f0: 2d72 6164 6975 733a 307d 2e79 7565 202e  -radius:0}.yue .
-00036800: 6a75 7079 7465 725f 636f 6e74 6169 6e65  jupyter_containe
-00036810: 7220 6469 762e 636f 6465 5f63 656c 6c20  r div.code_cell 
-00036820: 7072 657b 7061 6464 696e 673a 307d 2e6a  pre{padding:0}.j
-00036830: 7570 7974 6572 5f63 6f6e 7461 696e 6572  upyter_container
-00036840: 2064 6976 2e63 656c 6c5f 6f75 7470 7574   div.cell_output
-00036850: 202e 6f75 7470 7574 2c2e 6a75 7079 7465   .output,.jupyte
-00036860: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
-00036870: 6365 6c6c 5f6f 7574 7075 7420 2e73 7464  cell_output .std
-00036880: 6572 722c 2e6a 7570 7974 6572 5f63 6f6e  err,.jupyter_con
-00036890: 7461 696e 6572 2064 6976 2e63 656c 6c5f  tainer div.cell_
-000368a0: 6f75 7470 7574 202e 7769 6467 6574 2d73  output .widget-s
-000368b0: 7562 6172 6561 7b70 6164 6469 6e67 3a2e  ubarea{padding:.
-000368c0: 3572 656d 7d2e 6a75 7079 7465 725f 636f  5rem}.jupyter_co
-000368d0: 6e74 6169 6e65 7220 6469 762e 6365 6c6c  ntainer div.cell
-000368e0: 5f6f 7574 7075 7420 2e73 7464 6572 7220  _output .stderr 
-000368f0: 2e73 7464 6572 727b 7061 6464 696e 673a  .stderr{padding:
-00036900: 307d 2e6a 7570 7974 6572 2d77 6964 6765  0}.jupyter-widge
-00036910: 742d 6873 6c69 6465 7220 2e73 6c69 6465  t-hslider .slide
-00036920: 722d 636f 6e74 6169 6e65 722c 2e77 6964  r-container,.wid
-00036930: 6765 742d 6873 6c69 6465 7220 2e73 6c69  get-hslider .sli
-00036940: 6465 722d 636f 6e74 6169 6e65 727b 6469  der-container{di
-00036950: 7370 6c61 793a 666c 6578 3b61 6c69 676e  splay:flex;align
-00036960: 2d69 7465 6d73 3a63 656e 7465 727d 2e6a  -items:center}.j
-00036970: 7570 7974 6572 2d77 6964 6765 742d 736c  upyter-widget-sl
-00036980: 6964 6572 202e 6e6f 5569 2d74 6172 6765  ider .noUi-targe
-00036990: 742c 2e77 6964 6765 742d 736c 6964 6572  t,.widget-slider
-000369a0: 202e 6e6f 5569 2d74 6172 6765 747b 7769   .noUi-target{wi
-000369b0: 6474 683a 3130 3025 7d2e 6a75 7079 7465  dth:100%}.jupyte
-000369c0: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
-000369d0: 636f 6465 5f63 656c 6c20 2e68 6967 686c  code_cell .highl
-000369e0: 6967 6874 3e70 7265 7b70 6164 6469 6e67  ight>pre{padding
-000369f0: 3a31 7265 6d7d 2e6a 7570 7974 6572 5f63  :1rem}.jupyter_c
-00036a00: 6f6e 7461 696e 6572 2064 6976 2e63 6f64  ontainer div.cod
-00036a10: 655f 6365 6c6c 202e 6869 6768 6c69 6768  e_cell .highligh
-00036a20: 7420 2e68 6c6c 7b6d 6172 6769 6e2d 6c65  t .hll{margin-le
-00036a30: 6674 3a2d 3172 656d 3b6d 6172 6769 6e2d  ft:-1rem;margin-
-00036a40: 7269 6768 743a 2d31 7265 6d3b 7061 6464  right:-1rem;padd
-00036a50: 696e 673a 3020 3172 656d 7d2e 6a75 7079  ing:0 1rem}.jupy
-00036a60: 7465 725f 636f 6e74 6169 6e65 7220 6469  ter_container di
-00036a70: 762e 636f 6465 5f63 656c 6c20 2e68 6967  v.code_cell .hig
-00036a80: 686c 6967 6874 202e 6c69 6e65 6e6f 737b  hlight .linenos{
-00036a90: 6d61 7267 696e 2d72 6967 6874 3a2e 3872  margin-right:.8r
-00036aa0: 656d 7d2e 7975 6520 2e6a 7570 7974 6572  em}.yue .jupyter
-00036ab0: 5f63 6f6e 7461 696e 6572 202e 7374 6465  _container .stde
-00036ac0: 7272 7b63 6f6c 6f72 3a76 6172 282d 2d72  rr{color:var(--r
-00036ad0: 6564 2d61 3131 293b 6261 636b 6772 6f75  ed-a11);backgrou
-00036ae0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
-00036af0: 6564 2d61 3329 7d2e 7975 6520 2e6a 7570  ed-a3)}.yue .jup
-00036b00: 7974 6572 5f63 6f6e 7461 696e 6572 202e  yter_container .
-00036b10: 7374 6465 7272 202e 7374 6465 7272 7b62  stderr .stderr{b
-00036b20: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00036b30: 696e 6974 6961 6c7d 2e6e 6269 6e70 7574  initial}.nbinput
-00036b40: 202e 6869 6768 6c69 6768 747b 2d2d 7261   .highlight{--ra
-00036b50: 6469 7573 3a31 7078 7d2e 7975 6520 6469  dius:1px}.yue di
-00036b60: 762e 6e62 6c61 7374 2e63 6f6e 7461 696e  v.nblast.contain
-00036b70: 6572 7b70 6164 6469 6e67 2d74 6f70 3a35  er{padding-top:5
-00036b80: 7078 7d2e 7975 6520 6469 762e 6e62 696e  px}.yue div.nbin
-00036b90: 7075 742e 636f 6e74 6169 6e65 7220 6469  put.container di
-00036ba0: 762e 696e 7075 745f 6172 6561 7b62 6f72  v.input_area{bor
-00036bb0: 6465 722d 636f 6c6f 723a 7661 7228 2d2d  der-color:var(--
-00036bc0: 7379 2d63 2d62 6f72 6465 7229 7d2e 7975  sy-c-border)}.yu
-00036bd0: 6520 6469 762e 6e62 6f75 7470 7574 2e63  e div.nboutput.c
-00036be0: 6f6e 7461 696e 6572 2064 6976 2e6f 7574  ontainer div.out
-00036bf0: 7075 745f 6172 6561 2e73 7464 6572 727b  put_area.stderr{
-00036c00: 636f 6c6f 723a 7661 7228 2d2d 7265 642d  color:var(--red-
-00036c10: 6131 3129 3b62 6163 6b67 726f 756e 642d  a11);background-
-00036c20: 636f 6c6f 723a 7661 7228 2d2d 7265 642d  color:var(--red-
-00036c30: 6133 297d 2e79 7565 2064 6976 2e6e 626f  a3)}.yue div.nbo
-00036c40: 7574 7075 742e 636f 6e74 6169 6e65 7220  utput.container 
-00036c50: 6469 762e 6f75 7470 7574 5f61 7265 613e  div.output_area>
-00036c60: 2e6d 6174 682d 7772 6170 7065 723e 6469  .math-wrapper>di
-00036c70: 762e 6d61 7468 7b70 6164 6469 6e67 2d74  v.math{padding-t
-00036c80: 6f70 3a30 7d2e 7975 6520 2e6a 702d 5265  op:0}.yue .jp-Re
-00036c90: 6e64 6572 6564 4854 4d4c 436f 6d6d 6f6e  nderedHTMLCommon
-00036ca0: 2074 6865 6164 2c2e 7975 6520 6469 762e   thead,.yue div.
-00036cb0: 7265 6e64 6572 6564 5f68 746d 6c20 7468  rendered_html th
-00036cc0: 6561 647b 626f 7264 6572 2d63 6f6c 6f72  ead{border-color
-00036cd0: 3a76 6172 282d 2d73 792d 632d 626f 7264  :var(--sy-c-bord
-00036ce0: 6572 297d 2e79 7565 202e 6a70 2d52 656e  er)}.yue .jp-Ren
-00036cf0: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
-00036d00: 7462 6f64 7920 7472 2c2e 7975 6520 6469  tbody tr,.yue di
-00036d10: 762e 7265 6e64 6572 6564 5f68 746d 6c20  v.rendered_html 
-00036d20: 7462 6f64 7920 7472 7b63 6f6c 6f72 3a76  tbody tr{color:v
-00036d30: 6172 282d 2d73 792d 632d 7465 7874 297d  ar(--sy-c-text)}
-00036d40: 2e79 7565 202e 6a70 2d52 656e 6465 7265  .yue .jp-Rendere
-00036d50: 6448 544d 4c43 6f6d 6d6f 6e20 7462 6f64  dHTMLCommon tbod
-00036d60: 7920 7472 3a6e 7468 2d63 6869 6c64 286f  y tr:nth-child(o
-00036d70: 6464 292c 2e79 7565 2064 6976 2e72 656e  dd),.yue div.ren
-00036d80: 6465 7265 645f 6874 6d6c 2074 626f 6479  dered_html tbody
-00036d90: 2074 723a 6e74 682d 6368 696c 6428 6f64   tr:nth-child(od
-00036da0: 6429 7b62 6163 6b67 726f 756e 642d 636f  d){background-co
-00036db0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d73  lor:var(--sy-c-s
-00036dc0: 7572 6661 6365 297d 2e79 7565 202e 6a70  urface)}.yue .jp
-00036dd0: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
-00036de0: 6d6f 6e20 7462 6f64 7920 7472 3a68 6f76  mon tbody tr:hov
-00036df0: 6572 2c2e 7975 6520 6469 762e 7265 6e64  er,.yue div.rend
-00036e00: 6572 6564 5f68 746d 6c20 7462 6f64 7920  ered_html tbody 
-00036e10: 7472 3a68 6f76 6572 7b62 6163 6b67 726f  tr:hover{backgro
-00036e20: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-00036e30: 636f 6c6f 722d 7375 7266 6163 652d 6163  color-surface-ac
-00036e40: 6365 6e74 297d 2e79 7565 7b2d 2d73 672d  cent)}.yue{--sg-
-00036e50: 7465 7874 2d63 6f6c 6f72 3a76 6172 282d  text-color:var(-
-00036e60: 2d73 792d 632d 7465 7874 293b 2d2d 7367  -sy-c-text);--sg
-00036e70: 2d62 6163 6b67 726f 756e 642d 636f 6c6f  -background-colo
-00036e80: 723a 7661 7228 2d2d 7379 2d63 2d62 6163  r:var(--sy-c-bac
-00036e90: 6b67 726f 756e 6429 3b2d 2d73 672d 636f  kground);--sg-co
-00036ea0: 6465 2d62 6163 6b67 726f 756e 642d 636f  de-background-co
-00036eb0: 6c6f 723a 7661 7228 2d2d 7379 6e74 6178  lor:var(--syntax
-00036ec0: 2d70 7265 2d62 6729 3b2d 2d73 672d 7472  -pre-bg);--sg-tr
-00036ed0: 2d68 6f76 6572 2d63 6f6c 6f72 3a76 6172  -hover-color:var
-00036ee0: 282d 2d61 6363 656e 742d 6133 293b 2d2d  (--accent-a3);--
-00036ef0: 7367 2d74 722d 6f64 642d 636f 6c6f 723a  sg-tr-odd-color:
-00036f00: 7661 7228 2d2d 7379 2d63 2d73 7572 6661  var(--sy-c-surfa
-00036f10: 6365 293b 2d2d 7367 2d74 6f6f 6c74 6970  ce);--sg-tooltip
-00036f20: 2d66 6f72 6567 726f 756e 643a 7661 7228  -foreground:var(
-00036f30: 2d2d 7379 2d63 2d62 6163 6b67 726f 756e  --sy-c-backgroun
-00036f40: 642d 636f 6e74 7261 7374 293b 2d2d 7367  d-contrast);--sg
-00036f50: 2d74 6f6f 6c74 6970 2d62 6163 6b67 726f  -tooltip-backgro
-00036f60: 756e 643a 7661 7228 2d2d 7379 2d63 2d62  und:var(--sy-c-b
-00036f70: 6163 6b67 726f 756e 6429 3b2d 2d73 672d  ackground);--sg-
-00036f80: 746f 6f6c 7469 702d 626f 7264 6572 3a76  tooltip-border:v
-00036f90: 6172 282d 2d67 7261 792d 3729 2023 3030  ar(--gray-7) #00
-00036fa0: 3030 3b2d 2d73 672d 7468 756d 622d 626f  00;--sg-thumb-bo
-00036fb0: 782d 7368 6164 6f77 2d63 6f6c 6f72 3a76  x-shadow-color:v
-00036fc0: 6172 282d 2d67 7261 792d 6134 293b 2d2d  ar(--gray-a4);--
-00036fd0: 7367 2d74 6875 6d62 2d68 6f76 6572 2d62  sg-thumb-hover-b
-00036fe0: 6f72 6465 723a 7661 7228 2d2d 6163 6365  order:var(--acce
-00036ff0: 6e74 2d61 3929 3b2d 2d73 672d 7363 7269  nt-a9);--sg-scri
-00037000: 7074 2d6f 7574 3a76 6172 282d 2d73 792d  pt-out:var(--sy-
-00037010: 632d 6c69 6768 7429 3b2d 2d73 672d 7363  c-light);--sg-sc
-00037020: 7269 7074 2d70 7265 3a76 6172 282d 2d73  ript-pre:var(--s
-00037030: 796e 7461 782d 7072 652d 6267 293b 2d2d  yntax-pre-bg);--
-00037040: 7367 2d70 7974 622d 666f 7265 6772 6f75  sg-pytb-foregrou
-00037050: 6e64 3a76 6172 282d 2d73 796e 7461 782d  nd:var(--syntax-
-00037060: 7465 7874 293b 2d2d 7367 2d70 7974 622d  text);--sg-pytb-
-00037070: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
-00037080: 2d72 6564 2d61 3229 3b2d 2d73 672d 7079  -red-a2);--sg-py
-00037090: 7462 2d62 6f72 6465 722d 636f 6c6f 723a  tb-border-color:
-000370a0: 7661 7228 2d2d 7265 642d 6138 293b 2d2d  var(--red-a8);--
-000370b0: 7367 2d64 6f77 6e6c 6f61 642d 612d 6261  sg-download-a-ba
-000370c0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-000370d0: 6172 282d 2d61 6363 656e 742d 6133 293b  ar(--accent-a3);
-000370e0: 2d2d 7367 2d64 6f77 6e6c 6f61 642d 612d  --sg-download-a-
-000370f0: 6261 636b 6772 6f75 6e64 2d69 6d61 6765  background-image
-00037100: 3a6e 6f6e 653b 2d2d 7367 2d64 6f77 6e6c  :none;--sg-downl
-00037110: 6f61 642d 612d 626f 7264 6572 2d63 6f6c  oad-a-border-col
-00037120: 6f72 3a31 7078 2073 6f6c 6964 2076 6172  or:1px solid var
-00037130: 282d 2d61 6363 656e 742d 6133 293b 2d2d  (--accent-a3);--
-00037140: 7367 2d64 6f77 6e6c 6f61 642d 612d 636f  sg-download-a-co
-00037150: 6c6f 723a 7661 7228 2d2d 6163 6365 6e74  lor:var(--accent
-00037160: 2d61 3131 293b 2d2d 7367 2d64 6f77 6e6c  -a11);--sg-downl
-00037170: 6f61 642d 612d 686f 7665 722d 6261 636b  oad-a-hover-back
-00037180: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
-00037190: 282d 2d61 6363 656e 742d 6134 293b 2d2d  (--accent-a4);--
-000371a0: 7367 2d64 6f77 6e6c 6f61 642d 612d 686f  sg-download-a-ho
-000371b0: 7665 722d 626f 782d 7368 6164 6f77 2d31  ver-box-shadow-1
-000371c0: 3a23 3030 3030 3b2d 2d73 672d 646f 776e  :#0000;--sg-down
-000371d0: 6c6f 6164 2d61 2d68 6f76 6572 2d62 6f78  load-a-hover-box
-000371e0: 2d73 6861 646f 772d 323a 2330 3030 307d  -shadow-2:#0000}
-000371f0: 2e79 7565 202e 7370 6878 2d67 6c72 2d64  .yue .sphx-glr-d
-00037200: 6f77 6e6c 6f61 6420 612c 2e79 7565 202e  ownload a,.yue .
-00037210: 7370 6878 2d67 6c72 2d64 6f77 6e6c 6f61  sphx-glr-downloa
-00037220: 6420 613a 686f 7665 722c 2e79 7565 202e  d a:hover,.yue .
-00037230: 7370 6878 2d67 6c72 2d74 6875 6d62 6e61  sphx-glr-thumbna
-00037240: 696c 7320 617b 626f 7264 6572 2d62 6f74  ils a{border-bot
-00037250: 746f 6d3a 307d 2e79 7565 2070 2e73 7068  tom:0}.yue p.sph
-00037260: 782d 676c 722d 7369 676e 6174 7572 6520  x-glr-signature 
-00037270: 617b 626f 7264 6572 2d72 6164 6975 733a  a{border-radius:
-00037280: 303b 626f 7264 6572 2d62 6f74 746f 6d3a  0;border-bottom:
-00037290: 303b 7465 7874 2d64 6563 6f72 6174 696f  0;text-decoratio
-000372a0: 6e3a 756e 6465 726c 696e 657d 2e79 7565  n:underline}.yue
-000372b0: 2070 2e73 7068 782d 676c 722d 7369 676e   p.sphx-glr-sign
-000372c0: 6174 7572 6520 613a 686f 7665 727b 636f  ature a:hover{co
-000372d0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d6c  lor:var(--sy-c-l
-000372e0: 696e 6b2d 686f 7665 7229 7d2e 7975 6520  ink-hover)}.yue 
-000372f0: 2e73 7068 782d 676c 722d 666f 6f74 6572  .sphx-glr-footer
-00037300: 2069 6d67 7b64 6973 706c 6179 3a69 6e6c   img{display:inl
-00037310: 696e 653b 6d61 7267 696e 3a30 7d68 746d  ine;margin:0}htm
-00037320: 6c2e 6461 726b 2c68 746d 6c2e 6c69 6768  l.dark,html.ligh
-00037330: 747b 2d2d 646f 6373 6561 7263 682d 7072  t{--docsearch-pr
-00037340: 696d 6172 792d 636f 6c6f 723a 7661 7228  imary-color:var(
-00037350: 2d2d 6163 6365 6e74 2d39 293b 2d2d 646f  --accent-9);--do
-00037360: 6373 6561 7263 682d 7465 7874 2d63 6f6c  csearch-text-col
-00037370: 6f72 3a76 6172 282d 2d73 792d 632d 7465  or:var(--sy-c-te
-00037380: 7874 293b 2d2d 646f 6373 6561 7263 682d  xt);--docsearch-
-00037390: 6d6f 6461 6c2d 6261 636b 6772 6f75 6e64  modal-background
-000373a0: 3a76 6172 282d 2d73 792d 632d 6261 636b  :var(--sy-c-back
-000373b0: 6772 6f75 6e64 293b 2d2d 646f 6373 6561  ground);--docsea
-000373c0: 7263 682d 666f 6f74 6572 2d62 6163 6b67  rch-footer-backg
-000373d0: 726f 756e 643a 7661 7228 2d2d 7379 2d63  round:var(--sy-c
-000373e0: 2d73 7572 6661 6365 293b 2d2d 646f 6373  -surface);--docs
-000373f0: 6561 7263 682d 7365 6172 6368 626f 782d  earch-searchbox-
-00037400: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
-00037410: 2d73 792d 632d 7375 7266 6163 6529 3b2d  -sy-c-surface);-
-00037420: 2d64 6f63 7365 6172 6368 2d73 6561 7263  -docsearch-searc
-00037430: 6862 6f78 2d66 6f63 7573 2d62 6163 6b67  hbox-focus-backg
-00037440: 726f 756e 643a 7661 7228 2d2d 7379 2d63  round:var(--sy-c
-00037450: 2d62 6163 6b67 726f 756e 6429 3b2d 2d64  -background);--d
-00037460: 6f63 7365 6172 6368 2d6d 7574 6564 2d63  ocsearch-muted-c
-00037470: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
-00037480: 6c69 6768 7429 3b2d 2d64 6f63 7365 6172  light);--docsear
-00037490: 6368 2d68 6974 2d63 6f6c 6f72 3a76 6172  ch-hit-color:var
-000374a0: 282d 2d73 792d 632d 7465 7874 293b 2d2d  (--sy-c-text);--
-000374b0: 646f 6373 6561 7263 682d 6869 742d 6261  docsearch-hit-ba
-000374c0: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
-000374d0: 792d 632d 7375 7266 6163 6529 3b2d 2d64  y-c-surface);--d
-000374e0: 6f63 7365 6172 6368 2d68 6974 2d61 6374  ocsearch-hit-act
-000374f0: 6976 652d 636f 6c6f 723a 7661 7228 2d2d  ive-color:var(--
-00037500: 6163 6365 6e74 2d39 2d63 6f6e 7472 6173  accent-9-contras
-00037510: 7429 3b2d 2d64 6f63 7365 6172 6368 2d68  t);--docsearch-h
-00037520: 6974 2d73 6861 646f 773a 696e 7365 7420  it-shadow:inset 
-00037530: 3020 3020 3170 7820 3020 7661 7228 2d2d  0 0 1px 0 var(--
-00037540: 6772 6179 2d61 3131 293b 2d2d 646f 6373  gray-a11);--docs
-00037550: 6561 7263 682d 636f 6e74 6169 6e65 722d  earch-container-
-00037560: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
-00037570: 2d73 792d 632d 6f76 6572 6c61 7929 7d68  -sy-c-overlay)}h
-00037580: 746d 6c2e 6c69 6768 747b 2d2d 646f 6373  tml.light{--docs
-00037590: 6561 7263 682d 6b65 792d 6772 6164 6965  earch-key-gradie
-000375a0: 6e74 3a6c 696e 6561 722d 6772 6164 6965  nt:linear-gradie
-000375b0: 6e74 282d 3232 3564 6567 2c23 6536 6536  nt(-225deg,#e6e6
-000375c0: 6536 2c23 6638 6638 6638 293b 2d2d 646f  e6,#f8f8f8);--do
-000375d0: 6373 6561 7263 682d 6b65 792d 7368 6164  csearch-key-shad
-000375e0: 6f77 3a69 6e73 6574 2030 202d 3270 7820  ow:inset 0 -2px 
-000375f0: 2364 6264 6264 622c 696e 7365 7420 3020  #dbdbdb,inset 0 
-00037600: 3020 3170 7820 3170 7820 2366 6666 2c30  0 1px 1px #fff,0
-00037610: 2031 7078 2032 7078 2031 7078 2023 3530   1px 2px 1px #50
-00037620: 3530 3530 3636 7d68 746d 6c2e 6461 726b  505066}html.dark
-00037630: 7b2d 2d64 6f63 7365 6172 6368 2d6b 6579  {--docsearch-key
-00037640: 2d67 7261 6469 656e 743a 6c69 6e65 6172  -gradient:linear
-00037650: 2d67 7261 6469 656e 7428 2d32 3235 6465  -gradient(-225de
-00037660: 672c 2333 3533 3433 342c 2331 3431 3431  g,#353434,#14141
-00037670: 3429 3b2d 2d64 6f63 7365 6172 6368 2d6b  4);--docsearch-k
-00037680: 6579 2d73 6861 646f 773a 696e 7365 7420  ey-shadow:inset 
-00037690: 3020 2d32 7078 2023 3337 3337 3337 2c69  0 -2px #373737,i
-000376a0: 6e73 6574 2030 2030 2031 7078 2031 7078  nset 0 0 1px 1px
-000376b0: 2023 3232 322c 3020 3170 7820 3270 7820   #222,0 1px 2px 
-000376c0: 3170 7820 2330 3030 3b2d 2d64 6f63 7365  1px #000;--docse
-000376d0: 6172 6368 2d66 6f6f 7465 722d 7368 6164  arch-footer-shad
-000376e0: 6f77 3a30 202d 3170 7820 3020 3020 2333  ow:0 -1px 0 0 #3
-000376f0: 3733 3733 372c 3020 2d33 7078 2036 7078  73737,0 -3px 6px
-00037700: 2030 2023 3134 3134 3134 3b2d 2d64 6f63   0 #141414;--doc
-00037710: 7365 6172 6368 2d6d 6f64 616c 2d73 6861  search-modal-sha
-00037720: 646f 773a 696e 7365 7420 3170 7820 3170  dow:inset 1px 1p
-00037730: 7820 3020 3020 2333 3733 3733 372c 3020  x 0 0 #373737,0 
-00037740: 3370 7820 3870 7820 3020 2331 3431 3431  3px 8px 0 #14141
-00037750: 347d 2364 6f63 7365 6172 6368 202e 446f  4}#docsearch .Do
-00037760: 6353 6561 7263 682d 4275 7474 6f6e 7b62  cSearch-Button{b
-00037770: 6f72 6465 722d 7261 6469 7573 3a36 7078  order-radius:6px
-00037780: 7d23 646f 6373 6561 7263 6820 2e44 6f63  }#docsearch .Doc
-00037790: 5365 6172 6368 2d42 7574 746f 6e2d 4b65  Search-Button-Ke
-000377a0: 792c 2364 6f63 7365 6172 6368 202e 446f  y,#docsearch .Do
-000377b0: 6353 6561 7263 682d 4275 7474 6f6e 2d50  cSearch-Button-P
-000377c0: 6c61 6365 686f 6c64 6572 7b66 6f6e 742d  laceholder{font-
-000377d0: 7369 7a65 3a2e 3832 3572 656d 7d23 646f  size:.825rem}#do
-000377e0: 6373 6561 7263 6820 2e44 6f63 5365 6172  csearch .DocSear
-000377f0: 6368 2d42 7574 746f 6e2d 4b65 7973 2c23  ch-Button-Keys,#
-00037800: 646f 6373 6561 7263 6820 2e44 6f63 5365  docsearch .DocSe
-00037810: 6172 6368 2d42 7574 746f 6e2d 506c 6163  arch-Button-Plac
-00037820: 6568 6f6c 6465 727b 6469 7370 6c61 793a  eholder{display:
-00037830: 666c 6578 2169 6d70 6f72 7461 6e74 7d23  flex!important}#
-00037840: 646f 6373 6561 7263 6820 2e44 6f63 5365  docsearch .DocSe
-00037850: 6172 6368 2d53 6561 7263 682d 4963 6f6e  arch-Search-Icon
-00037860: 7b77 6964 7468 3a2e 3837 3572 656d 2169  {width:.875rem!i
-00037870: 6d70 6f72 7461 6e74 3b68 6569 6768 743a  mportant;height:
-00037880: 2e38 3735 7265 6d21 696d 706f 7274 616e  .875rem!importan
-00037890: 747d 406d 6564 6961 2028 6d61 782d 7769  t}@media (max-wi
-000378a0: 6474 683a 3736 3770 7829 7b23 646f 6373  dth:767px){#docs
-000378b0: 6561 7263 687b 706f 7369 7469 6f6e 3a61  earch{position:a
-000378c0: 6273 6f6c 7574 653b 746f 703a 3172 656d  bsolute;top:1rem
-000378d0: 3b6c 6566 743a 312e 3872 656d 3b72 6967  ;left:1.8rem;rig
-000378e0: 6874 3a31 2e38 7265 6d7d 2364 6f63 7365  ht:1.8rem}#docse
-000378f0: 6172 6368 202e 446f 6353 6561 7263 682d  arch .DocSearch-
-00037900: 4275 7474 6f6e 7b6d 6172 6769 6e2d 6c65  Button{margin-le
-00037910: 6674 3a30 3b77 6964 7468 3a31 3030 257d  ft:0;width:100%}
-00037920: 7d64 6c2e 7371 6c61 2064 747b 636f 6c6f  }dl.sqla dt{colo
-00037930: 723a 7661 7228 2d2d 7369 672d 6e61 6d65  r:var(--sig-name
-00037940: 293b 6d61 7267 696e 2d62 6f74 746f 6d3a  );margin-bottom:
-00037950: 2e35 7265 6d7d 646c 2e73 716c 6120 6474  .5rem}dl.sqla dt
-00037960: 3e65 6d7b 666f 6e74 2d77 6569 6768 743a  >em{font-weight:
-00037970: 3430 303b 666f 6e74 2d73 7479 6c65 3a6e  400;font-style:n
-00037980: 6f72 6d61 6c3b 636f 6c6f 723a 7661 7228  ormal;color:var(
-00037990: 2d2d 7369 672d 7061 7261 6d29 7d64 6c2e  --sig-param)}dl.
-000379a0: 7371 6c61 2064 643e 702e 7275 6272 6963  sqla dd>p.rubric
-000379b0: 7b6d 6172 6769 6e2d 746f 703a 312e 3572  {margin-top:1.5r
-000379c0: 656d 3b74 6578 742d 7472 616e 7366 6f72  em;text-transfor
-000379d0: 6d3a 7570 7065 7263 6173 653b 666f 6e74  m:uppercase;font
-000379e0: 2d73 697a 653a 2e37 3672 656d 7d64 6c2e  -size:.76rem}dl.
-000379f0: 7371 6c61 2064 643e 702e 7275 6272 6963  sqla dd>p.rubric
-00037a00: 2b2e 7461 626c 652d 7772 6170 7065 727b  +.table-wrapper{
-00037a10: 6d61 7267 696e 2d74 6f70 3a2e 3735 7265  margin-top:.75re
-00037a20: 6d3b 626f 7264 6572 2d6c 6566 743a 303b  m;border-left:0;
-00037a30: 626f 7264 6572 2d72 6967 6874 3a30 3b62  border-right:0;b
-00037a40: 6f72 6465 722d 7261 6469 7573 3a30 7d64  order-radius:0}d
-00037a50: 6c2e 7371 6c61 2070 2e72 7562 7269 632b  l.sqla p.rubric+
-00037a60: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
-00037a70: 642c 646c 2e73 716c 6120 702e 7275 6272  d,dl.sqla p.rubr
-00037a80: 6963 2b2e 7461 626c 652d 7772 6170 7065  ic+.table-wrappe
-00037a90: 7220 7468 7b62 6f72 6465 722d 6c65 6674  r th{border-left
-00037aa0: 3a30 3b62 6f72 6465 722d 7269 6768 743a  :0;border-right:
-00037ab0: 303b 6261 636b 6772 6f75 6e64 2d63 6f6c  0;background-col
-00037ac0: 6f72 3a69 6e69 7469 616c 7d64 6c2e 7371  or:initial}dl.sq
-00037ad0: 6c61 2070 2e72 7562 7269 632b 2e74 6162  la p.rubric+.tab
-00037ae0: 6c65 2d77 7261 7070 6572 2074 643e 707b  le-wrapper td>p{
-00037af0: 6d61 7267 696e 3a30 7d64 6c2e 7371 6c61  margin:0}dl.sqla
-00037b00: 2070 2e72 7562 7269 632b 2e74 6162 6c65   p.rubric+.table
-00037b10: 2d77 7261 7070 6572 2074 722e 726f 772d  -wrapper tr.row-
-00037b20: 6f64 647b 6261 636b 6772 6f75 6e64 2d63  odd{background-c
-00037b30: 6f6c 6f72 3a69 6e69 7469 616c 7d64 6c2e  olor:initial}dl.
-00037b40: 7371 6c61 2070 2e72 7562 7269 632b 2e74  sqla p.rubric+.t
-00037b50: 6162 6c65 2d77 7261 7070 6572 2074 722e  able-wrapper tr.
-00037b60: 726f 772d 6576 656e 7b62 6163 6b67 726f  row-even{backgro
-00037b70: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
-00037b80: 7975 652d 632d 726f 772d 6261 636b 6772  yue-c-row-backgr
-00037b90: 6f75 6e64 297d 2e79 7565 7b2d 2d78 722d  ound)}.yue{--xr-
-00037ba0: 666f 6e74 2d63 6f6c 6f72 303a 7661 7228  font-color0:var(
-00037bb0: 2d2d 7379 2d63 2d68 6561 6469 6e67 293b  --sy-c-heading);
-00037bc0: 2d2d 7872 2d66 6f6e 742d 636f 6c6f 7232  --xr-font-color2
-00037bd0: 3a76 6172 282d 2d73 792d 632d 7465 7874  :var(--sy-c-text
-00037be0: 293b 2d2d 7872 2d66 6f6e 742d 636f 6c6f  );--xr-font-colo
-00037bf0: 7233 3a76 6172 282d 2d73 792d 632d 6c69  r3:var(--sy-c-li
-00037c00: 6768 7429 3b2d 2d78 722d 626f 7264 6572  ght);--xr-border
-00037c10: 2d63 6f6c 6f72 3a76 6172 282d 2d73 792d  -color:var(--sy-
-00037c20: 632d 626f 7264 6572 293b 2d2d 7872 2d64  c-border);--xr-d
-00037c30: 6973 6162 6c65 642d 636f 6c6f 723a 7661  isabled-color:va
-00037c40: 7228 2d2d 6772 6179 2d61 3629 3b2d 2d78  r(--gray-a6);--x
-00037c50: 722d 6261 636b 6772 6f75 6e64 2d63 6f6c  r-background-col
-00037c60: 6f72 3a76 6172 282d 2d73 792d 632d 6261  or:var(--sy-c-ba
-00037c70: 636b 6772 6f75 6e64 293b 2d2d 7872 2d62  ckground);--xr-b
-00037c80: 6163 6b67 726f 756e 642d 636f 6c6f 722d  ackground-color-
-00037c90: 726f 772d 6576 656e 3a76 6172 282d 2d73  row-even:var(--s
-00037ca0: 792d 632d 6261 636b 6772 6f75 6e64 293b  y-c-background);
-00037cb0: 2d2d 7872 2d62 6163 6b67 726f 756e 642d  --xr-background-
-00037cc0: 636f 6c6f 722d 726f 772d 6f64 643a 7661  color-row-odd:va
-00037cd0: 7228 2d2d 6772 6179 2d32 297d 2e79 7565  r(--gray-2)}.yue
-00037ce0: 202e 7872 2d61 7272 6179 2d64 6174 6120   .xr-array-data 
-00037cf0: 7072 657b 6d61 7267 696e 3a30 7d2e 7975  pre{margin:0}.yu
-00037d00: 6520 6465 7461 696c 732e 746f 6767 6c65  e details.toggle
-00037d10: 2d64 6574 6169 6c73 2073 756d 6d61 7279  -details summary
-00037d20: 7b62 6f72 6465 722d 6c65 6674 2d63 6f6c  {border-left-col
-00037d30: 6f72 3a76 6172 282d 2d61 6363 656e 742d  or:var(--accent-
-00037d40: 6139 297d 406d 6564 6961 206e 6f74 2061  a9)}@media not a
-00037d50: 6c6c 2061 6e64 2028 6d69 6e2d 7769 6474  ll and (min-widt
-00037d60: 683a 3634 3070 7829 7b2e 6d61 782d 736d  h:640px){.max-sm
-00037d70: 5c3a 6d61 782d 772d 6675 6c6c 7b6d 6178  \:max-w-full{max
-00037d80: 2d77 6964 7468 3a31 3030 257d 7d40 6d65  -width:100%}}@me
-00037d90: 6469 6120 286d 696e 2d77 6964 7468 3a37  dia (min-width:7
-00037da0: 3638 7078 297b 2e6d 645c 3a73 7469 636b  68px){.md\:stick
-00037db0: 797b 706f 7369 7469 6f6e 3a73 7469 636b  y{position:stick
-00037dc0: 797d 2e6d 645c 3a69 6e6c 696e 657b 6469  y}.md\:inline{di
-00037dd0: 7370 6c61 793a 696e 6c69 6e65 7d2e 6d64  splay:inline}.md
-00037de0: 5c3a 666c 6578 7b64 6973 706c 6179 3a66  \:flex{display:f
-00037df0: 6c65 787d 2e6d 645c 3a68 6964 6465 6e7b  lex}.md\:hidden{
-00037e00: 6469 7370 6c61 793a 6e6f 6e65 7d2e 6d64  display:none}.md
-00037e10: 5c3a 772d 3732 7b77 6964 7468 3a31 3872  \:w-72{width:18r
-00037e20: 656d 7d2e 6d64 5c3a 7368 7269 6e6b 2d30  em}.md\:shrink-0
-00037e30: 7b66 6c65 782d 7368 7269 6e6b 3a30 7d7d  {flex-shrink:0}}
-00037e40: 406d 6564 6961 2028 6d69 6e2d 7769 6474  @media (min-widt
-00037e50: 683a 3132 3830 7078 297b 2e78 6c5c 3a73  h:1280px){.xl\:s
-00037e60: 7469 636b 797b 706f 7369 7469 6f6e 3a73  ticky{position:s
-00037e70: 7469 636b 797d 2e78 6c5c 3a74 6f70 2d31  ticky}.xl\:top-1
-00037e80: 367b 746f 703a 3472 656d 7d2e 786c 5c3a  6{top:4rem}.xl\:
-00037e90: 6869 6464 656e 7b64 6973 706c 6179 3a6e  hidden{display:n
-00037ea0: 6f6e 657d 2e78 6c5c 3a70 782d 3132 7b70  one}.xl\:px-12{p
-00037eb0: 6164 6469 6e67 2d6c 6566 743a 3372 656d  adding-left:3rem
-00037ec0: 3b70 6164 6469 6e67 2d72 6967 6874 3a33  ;padding-right:3
-00037ed0: 7265 6d7d 2e78 6c5c 3a70 6c2d 307b 7061  rem}.xl\:pl-0{pa
-00037ee0: 6464 696e 672d 6c65 6674 3a30 7d7d 406d  dding-left:0}}@m
-00037ef0: 6564 6961 2070 7269 6e74 7b2e 7072 696e  edia print{.prin
-00037f00: 745c 3a68 6964 6465 6e7b 6469 7370 6c61  t\:hidden{displa
-00037f10: 793a 6e6f 6e65 7d2e 7072 696e 745c 3a70  y:none}.print\:p
-00037f20: 742d 367b 7061 6464 696e 672d 746f 703a  t-6{padding-top:
-00037f30: 312e 3572 656d 7d7d                      1.5rem}}
+00033bc0: 6b2d 6d61 726b 7570 2d64 656c 6574 6564  k-markup-deleted
+00033bd0: 2d62 6729 3b2d 2d73 796e 7461 782d 6d61  -bg);--syntax-ma
+00033be0: 726b 7570 2d69 6e73 6572 7465 642d 7465  rkup-inserted-te
+00033bf0: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
+00033c00: 6461 726b 2d6d 6172 6b75 702d 696e 7365  dark-markup-inse
+00033c10: 7274 6564 2d74 6578 7429 3b2d 2d73 796e  rted-text);--syn
+00033c20: 7461 782d 6d61 726b 7570 2d69 6e73 6572  tax-markup-inser
+00033c30: 7465 642d 6267 3a76 6172 282d 2d73 796e  ted-bg:var(--syn
+00033c40: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
+00033c50: 696e 7365 7274 6564 2d62 6729 3b2d 2d73  inserted-bg);--s
+00033c60: 796e 7461 782d 6d61 726b 7570 2d63 6861  yntax-markup-cha
+00033c70: 6e67 6564 2d74 6578 743a 7661 7228 2d2d  nged-text:var(--
+00033c80: 7379 6e74 6178 2d64 6172 6b2d 6d61 726b  syntax-dark-mark
+00033c90: 7570 2d63 6861 6e67 6564 2d74 6578 7429  up-changed-text)
+00033ca0: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00033cb0: 2d63 6861 6e67 6564 2d62 673a 7661 7228  -changed-bg:var(
+00033cc0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
+00033cd0: 726b 7570 2d63 6861 6e67 6564 2d62 6729  rkup-changed-bg)
+00033ce0: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00033cf0: 2d69 676e 6f72 6564 2d74 6578 743a 7661  -ignored-text:va
+00033d00: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00033d10: 6d61 726b 7570 2d69 676e 6f72 6564 2d74  markup-ignored-t
+00033d20: 6578 7429 3b2d 2d73 796e 7461 782d 6d61  ext);--syntax-ma
+00033d30: 726b 7570 2d69 676e 6f72 6564 2d62 673a  rkup-ignored-bg:
+00033d40: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+00033d50: 6b2d 6d61 726b 7570 2d69 676e 6f72 6564  k-markup-ignored
+00033d60: 2d62 6729 3b2d 2d73 796e 7461 782d 6d65  -bg);--syntax-me
+00033d70: 7461 2d64 6966 662d 7261 6e67 653a 7661  ta-diff-range:va
+00033d80: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+00033d90: 6d65 7461 2d64 6966 662d 7261 6e67 6529  meta-diff-range)
+00033da0: 3b2d 2d73 796e 7461 782d 7370 6563 6961  ;--syntax-specia
+00033db0: 6c2d 6267 3a76 6172 282d 2d73 796e 7461  l-bg:var(--synta
+00033dc0: 782d 6461 726b 2d73 7065 6369 616c 2d62  x-dark-special-b
+00033dd0: 6729 7d7d 6874 6d6c 2e64 6172 6b7b 2d2d  g)}}html.dark{--
+00033de0: 7379 6e74 6178 2d74 6578 743a 7661 7228  syntax-text:var(
+00033df0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 7465  --syntax-dark-te
+00033e00: 7874 293b 2d2d 7379 6e74 6178 2d6d 6574  xt);--syntax-met
+00033e10: 613a 7661 7228 2d2d 7379 6e74 6178 2d64  a:var(--syntax-d
+00033e20: 6172 6b2d 6d65 7461 293b 2d2d 7379 6e74  ark-meta);--synt
+00033e30: 6178 2d63 6f6d 6d65 6e74 3a76 6172 282d  ax-comment:var(-
+00033e40: 2d73 796e 7461 782d 6461 726b 2d63 6f6d  -syntax-dark-com
+00033e50: 6d65 6e74 293b 2d2d 7379 6e74 6178 2d63  ment);--syntax-c
+00033e60: 6f6e 7374 616e 743a 7661 7228 2d2d 7379  onstant:var(--sy
+00033e70: 6e74 6178 2d64 6172 6b2d 636f 6e73 7461  ntax-dark-consta
+00033e80: 6e74 293b 2d2d 7379 6e74 6178 2d65 6e74  nt);--syntax-ent
+00033e90: 6974 793a 7661 7228 2d2d 7379 6e74 6178  ity:var(--syntax
+00033ea0: 2d64 6172 6b2d 656e 7469 7479 293b 2d2d  -dark-entity);--
+00033eb0: 7379 6e74 6178 2d70 726f 7065 7274 793a  syntax-property:
+00033ec0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+00033ed0: 6b2d 7072 6f70 6572 7479 293b 2d2d 7379  k-property);--sy
+00033ee0: 6e74 6178 2d64 6566 696e 6974 696f 6e3a  ntax-definition:
+00033ef0: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+00033f00: 6b2d 6465 6669 6e69 7469 6f6e 293b 2d2d  k-definition);--
+00033f10: 7379 6e74 6178 2d74 6167 3a76 6172 282d  syntax-tag:var(-
+00033f20: 2d73 796e 7461 782d 6461 726b 2d74 6167  -syntax-dark-tag
+00033f30: 293b 2d2d 7379 6e74 6178 2d62 7569 6c74  );--syntax-built
+00033f40: 696e 3a76 6172 282d 2d73 796e 7461 782d  in:var(--syntax-
+00033f50: 6461 726b 2d62 7569 6c74 696e 293b 2d2d  dark-builtin);--
+00033f60: 7379 6e74 6178 2d6b 6579 776f 7264 3a76  syntax-keyword:v
+00033f70: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00033f80: 2d6b 6579 776f 7264 293b 2d2d 7379 6e74  -keyword);--synt
+00033f90: 6178 2d65 7863 6570 7469 6f6e 3a76 6172  ax-exception:var
+00033fa0: 282d 2d73 796e 7461 782d 6461 726b 2d65  (--syntax-dark-e
+00033fb0: 7863 6570 7469 6f6e 293b 2d2d 7379 6e74  xception);--synt
+00033fc0: 6178 2d73 7472 696e 673a 7661 7228 2d2d  ax-string:var(--
+00033fd0: 7379 6e74 6178 2d64 6172 6b2d 7374 7269  syntax-dark-stri
+00033fe0: 6e67 293b 2d2d 7379 6e74 6178 2d72 6567  ng);--syntax-reg
+00033ff0: 6578 703a 7661 7228 2d2d 7379 6e74 6178  exp:var(--syntax
+00034000: 2d64 6172 6b2d 7265 6765 7870 293b 2d2d  -dark-regexp);--
+00034010: 7379 6e74 6178 2d76 6172 6961 626c 653a  syntax-variable:
+00034020: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+00034030: 6b2d 7661 7269 6162 6c65 293b 2d2d 7379  k-variable);--sy
+00034040: 6e74 6178 2d69 6e76 616c 6964 2d69 6c6c  ntax-invalid-ill
+00034050: 6567 616c 2d74 6578 743a 7661 7228 2d2d  egal-text:var(--
+00034060: 7379 6e74 6178 2d64 6172 6b2d 696e 7661  syntax-dark-inva
+00034070: 6c69 642d 696c 6c65 6761 6c2d 7465 7874  lid-illegal-text
+00034080: 293b 2d2d 7379 6e74 6178 2d69 6e76 616c  );--syntax-inval
+00034090: 6964 2d69 6c6c 6567 616c 2d62 673a 7661  id-illegal-bg:va
+000340a0: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+000340b0: 696e 7661 6c69 642d 696c 6c65 6761 6c2d  invalid-illegal-
+000340c0: 6267 293b 2d2d 7379 6e74 6178 2d6d 6172  bg);--syntax-mar
+000340d0: 6b75 702d 6865 6164 696e 673a 7661 7228  kup-heading:var(
+000340e0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
+000340f0: 726b 7570 2d68 6561 6469 6e67 293b 2d2d  rkup-heading);--
+00034100: 7379 6e74 6178 2d6d 6172 6b75 702d 6974  syntax-markup-it
+00034110: 616c 6963 3a76 6172 282d 2d73 796e 7461  alic:var(--synta
+00034120: 782d 6461 726b 2d6d 6172 6b75 702d 6974  x-dark-markup-it
+00034130: 616c 6963 293b 2d2d 7379 6e74 6178 2d6d  alic);--syntax-m
+00034140: 6172 6b75 702d 626f 6c64 3a76 6172 282d  arkup-bold:var(-
+00034150: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
+00034160: 6b75 702d 626f 6c64 293b 2d2d 7379 6e74  kup-bold);--synt
+00034170: 6178 2d6d 6172 6b75 702d 6465 6c65 7465  ax-markup-delete
+00034180: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
+00034190: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
+000341a0: 6465 6c65 7465 642d 7465 7874 293b 2d2d  deleted-text);--
+000341b0: 7379 6e74 6178 2d6d 6172 6b75 702d 6465  syntax-markup-de
+000341c0: 6c65 7465 642d 6267 3a76 6172 282d 2d73  leted-bg:var(--s
+000341d0: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
+000341e0: 702d 6465 6c65 7465 642d 6267 293b 2d2d  p-deleted-bg);--
+000341f0: 7379 6e74 6178 2d6d 6172 6b75 702d 696e  syntax-markup-in
+00034200: 7365 7274 6564 2d74 6578 743a 7661 7228  serted-text:var(
+00034210: 2d2d 7379 6e74 6178 2d64 6172 6b2d 6d61  --syntax-dark-ma
+00034220: 726b 7570 2d69 6e73 6572 7465 642d 7465  rkup-inserted-te
+00034230: 7874 293b 2d2d 7379 6e74 6178 2d6d 6172  xt);--syntax-mar
+00034240: 6b75 702d 696e 7365 7274 6564 2d62 673a  kup-inserted-bg:
+00034250: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+00034260: 6b2d 6d61 726b 7570 2d69 6e73 6572 7465  k-markup-inserte
+00034270: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
+00034280: 6172 6b75 702d 6368 616e 6765 642d 7465  arkup-changed-te
+00034290: 7874 3a76 6172 282d 2d73 796e 7461 782d  xt:var(--syntax-
+000342a0: 6461 726b 2d6d 6172 6b75 702d 6368 616e  dark-markup-chan
+000342b0: 6765 642d 7465 7874 293b 2d2d 7379 6e74  ged-text);--synt
+000342c0: 6178 2d6d 6172 6b75 702d 6368 616e 6765  ax-markup-change
+000342d0: 642d 6267 3a76 6172 282d 2d73 796e 7461  d-bg:var(--synta
+000342e0: 782d 6461 726b 2d6d 6172 6b75 702d 6368  x-dark-markup-ch
+000342f0: 616e 6765 642d 6267 293b 2d2d 7379 6e74  anged-bg);--synt
+00034300: 6178 2d6d 6172 6b75 702d 6967 6e6f 7265  ax-markup-ignore
+00034310: 642d 7465 7874 3a76 6172 282d 2d73 796e  d-text:var(--syn
+00034320: 7461 782d 6461 726b 2d6d 6172 6b75 702d  tax-dark-markup-
+00034330: 6967 6e6f 7265 642d 7465 7874 293b 2d2d  ignored-text);--
+00034340: 7379 6e74 6178 2d6d 6172 6b75 702d 6967  syntax-markup-ig
+00034350: 6e6f 7265 642d 6267 3a76 6172 282d 2d73  nored-bg:var(--s
+00034360: 796e 7461 782d 6461 726b 2d6d 6172 6b75  yntax-dark-marku
+00034370: 702d 6967 6e6f 7265 642d 6267 293b 2d2d  p-ignored-bg);--
+00034380: 7379 6e74 6178 2d6d 6574 612d 6469 6666  syntax-meta-diff
+00034390: 2d72 616e 6765 3a76 6172 282d 2d73 796e  -range:var(--syn
+000343a0: 7461 782d 6461 726b 2d6d 6574 612d 6469  tax-dark-meta-di
+000343b0: 6666 2d72 616e 6765 293b 2d2d 7379 6e74  ff-range);--synt
+000343c0: 6178 2d73 7065 6369 616c 2d62 673a 7661  ax-special-bg:va
+000343d0: 7228 2d2d 7379 6e74 6178 2d64 6172 6b2d  r(--syntax-dark-
+000343e0: 7370 6563 6961 6c2d 6267 297d 2e6c 6967  special-bg)}.lig
+000343f0: 6874 202e 6461 726b 2d63 6f64 657b 2d2d  ht .dark-code{--
+00034400: 7379 6e74 6178 2d70 7265 2d62 673a 7661  syntax-pre-bg:va
+00034410: 7228 2d2d 626c 6163 6b2d 6131 3229 3b2d  r(--black-a12);-
+00034420: 2d73 796e 7461 782d 6361 702d 6267 3a23  -syntax-cap-bg:#
+00034430: 3163 3230 3234 3b2d 2d73 796e 7461 782d  1c2024;--syntax-
+00034440: 6869 6768 6c69 6768 742d 6267 3a76 6172  highlight-bg:var
+00034450: 282d 2d77 6869 7465 2d61 3229 3b2d 2d73  (--white-a2);--s
+00034460: 796e 7461 782d 6c69 6e65 6e6f 732d 6469  yntax-linenos-di
+00034470: 7669 6465 723a 7661 7228 2d2d 7768 6974  vider:var(--whit
+00034480: 652d 6134 293b 2d2d 7379 6e74 6178 2d74  e-a4);--syntax-t
+00034490: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
+000344a0: 2d64 6172 6b2d 7465 7874 293b 2d2d 7379  -dark-text);--sy
+000344b0: 6e74 6178 2d6d 6574 613a 7661 7228 2d2d  ntax-meta:var(--
+000344c0: 7379 6e74 6178 2d64 6172 6b2d 6d65 7461  syntax-dark-meta
+000344d0: 293b 2d2d 7379 6e74 6178 2d63 6f6d 6d65  );--syntax-comme
+000344e0: 6e74 3a76 6172 282d 2d73 796e 7461 782d  nt:var(--syntax-
+000344f0: 6461 726b 2d63 6f6d 6d65 6e74 293b 2d2d  dark-comment);--
+00034500: 7379 6e74 6178 2d63 6f6e 7374 616e 743a  syntax-constant:
+00034510: 7661 7228 2d2d 7379 6e74 6178 2d64 6172  var(--syntax-dar
+00034520: 6b2d 636f 6e73 7461 6e74 293b 2d2d 7379  k-constant);--sy
+00034530: 6e74 6178 2d65 6e74 6974 793a 7661 7228  ntax-entity:var(
+00034540: 2d2d 7379 6e74 6178 2d64 6172 6b2d 656e  --syntax-dark-en
+00034550: 7469 7479 293b 2d2d 7379 6e74 6178 2d70  tity);--syntax-p
+00034560: 726f 7065 7274 793a 7661 7228 2d2d 7379  roperty:var(--sy
+00034570: 6e74 6178 2d64 6172 6b2d 7072 6f70 6572  ntax-dark-proper
+00034580: 7479 293b 2d2d 7379 6e74 6178 2d64 6566  ty);--syntax-def
+00034590: 696e 6974 696f 6e3a 7661 7228 2d2d 7379  inition:var(--sy
+000345a0: 6e74 6178 2d64 6172 6b2d 6465 6669 6e69  ntax-dark-defini
+000345b0: 7469 6f6e 293b 2d2d 7379 6e74 6178 2d74  tion);--syntax-t
+000345c0: 6167 3a76 6172 282d 2d73 796e 7461 782d  ag:var(--syntax-
+000345d0: 6461 726b 2d74 6167 293b 2d2d 7379 6e74  dark-tag);--synt
+000345e0: 6178 2d62 7569 6c74 696e 3a76 6172 282d  ax-builtin:var(-
+000345f0: 2d73 796e 7461 782d 6461 726b 2d62 7569  -syntax-dark-bui
+00034600: 6c74 696e 293b 2d2d 7379 6e74 6178 2d6b  ltin);--syntax-k
+00034610: 6579 776f 7264 3a76 6172 282d 2d73 796e  eyword:var(--syn
+00034620: 7461 782d 6461 726b 2d6b 6579 776f 7264  tax-dark-keyword
+00034630: 293b 2d2d 7379 6e74 6178 2d65 7863 6570  );--syntax-excep
+00034640: 7469 6f6e 3a76 6172 282d 2d73 796e 7461  tion:var(--synta
+00034650: 782d 6461 726b 2d65 7863 6570 7469 6f6e  x-dark-exception
+00034660: 293b 2d2d 7379 6e74 6178 2d73 7472 696e  );--syntax-strin
+00034670: 673a 7661 7228 2d2d 7379 6e74 6178 2d64  g:var(--syntax-d
+00034680: 6172 6b2d 7374 7269 6e67 293b 2d2d 7379  ark-string);--sy
+00034690: 6e74 6178 2d72 6567 6578 703a 7661 7228  ntax-regexp:var(
+000346a0: 2d2d 7379 6e74 6178 2d64 6172 6b2d 7265  --syntax-dark-re
+000346b0: 6765 7870 293b 2d2d 7379 6e74 6178 2d76  gexp);--syntax-v
+000346c0: 6172 6961 626c 653a 7661 7228 2d2d 7379  ariable:var(--sy
+000346d0: 6e74 6178 2d64 6172 6b2d 7661 7269 6162  ntax-dark-variab
+000346e0: 6c65 293b 2d2d 7379 6e74 6178 2d69 6e76  le);--syntax-inv
+000346f0: 616c 6964 2d69 6c6c 6567 616c 2d74 6578  alid-illegal-tex
+00034700: 743a 7661 7228 2d2d 7379 6e74 6178 2d64  t:var(--syntax-d
+00034710: 6172 6b2d 696e 7661 6c69 642d 696c 6c65  ark-invalid-ille
+00034720: 6761 6c2d 7465 7874 293b 2d2d 7379 6e74  gal-text);--synt
+00034730: 6178 2d69 6e76 616c 6964 2d69 6c6c 6567  ax-invalid-illeg
+00034740: 616c 2d62 673a 7661 7228 2d2d 7379 6e74  al-bg:var(--synt
+00034750: 6178 2d64 6172 6b2d 696e 7661 6c69 642d  ax-dark-invalid-
+00034760: 696c 6c65 6761 6c2d 6267 293b 2d2d 7379  illegal-bg);--sy
+00034770: 6e74 6178 2d6d 6172 6b75 702d 6865 6164  ntax-markup-head
+00034780: 696e 673a 7661 7228 2d2d 7379 6e74 6178  ing:var(--syntax
+00034790: 2d64 6172 6b2d 6d61 726b 7570 2d68 6561  -dark-markup-hea
+000347a0: 6469 6e67 293b 2d2d 7379 6e74 6178 2d6d  ding);--syntax-m
+000347b0: 6172 6b75 702d 6974 616c 6963 3a76 6172  arkup-italic:var
+000347c0: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
+000347d0: 6172 6b75 702d 6974 616c 6963 293b 2d2d  arkup-italic);--
+000347e0: 7379 6e74 6178 2d6d 6172 6b75 702d 626f  syntax-markup-bo
+000347f0: 6c64 3a76 6172 282d 2d73 796e 7461 782d  ld:var(--syntax-
+00034800: 6461 726b 2d6d 6172 6b75 702d 626f 6c64  dark-markup-bold
+00034810: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
+00034820: 702d 6465 6c65 7465 642d 7465 7874 3a76  p-deleted-text:v
+00034830: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00034840: 2d6d 6172 6b75 702d 6465 6c65 7465 642d  -markup-deleted-
+00034850: 7465 7874 293b 2d2d 7379 6e74 6178 2d6d  text);--syntax-m
+00034860: 6172 6b75 702d 6465 6c65 7465 642d 6267  arkup-deleted-bg
+00034870: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+00034880: 726b 2d6d 6172 6b75 702d 6465 6c65 7465  rk-markup-delete
+00034890: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
+000348a0: 6172 6b75 702d 696e 7365 7274 6564 2d74  arkup-inserted-t
+000348b0: 6578 743a 7661 7228 2d2d 7379 6e74 6178  ext:var(--syntax
+000348c0: 2d64 6172 6b2d 6d61 726b 7570 2d69 6e73  -dark-markup-ins
+000348d0: 6572 7465 642d 7465 7874 293b 2d2d 7379  erted-text);--sy
+000348e0: 6e74 6178 2d6d 6172 6b75 702d 696e 7365  ntax-markup-inse
+000348f0: 7274 6564 2d62 673a 7661 7228 2d2d 7379  rted-bg:var(--sy
+00034900: 6e74 6178 2d64 6172 6b2d 6d61 726b 7570  ntax-dark-markup
+00034910: 2d69 6e73 6572 7465 642d 6267 293b 2d2d  -inserted-bg);--
+00034920: 7379 6e74 6178 2d6d 6172 6b75 702d 6368  syntax-markup-ch
+00034930: 616e 6765 642d 7465 7874 3a76 6172 282d  anged-text:var(-
+00034940: 2d73 796e 7461 782d 6461 726b 2d6d 6172  -syntax-dark-mar
+00034950: 6b75 702d 6368 616e 6765 642d 7465 7874  kup-changed-text
+00034960: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
+00034970: 702d 6368 616e 6765 642d 6267 3a76 6172  p-changed-bg:var
+00034980: 282d 2d73 796e 7461 782d 6461 726b 2d6d  (--syntax-dark-m
+00034990: 6172 6b75 702d 6368 616e 6765 642d 6267  arkup-changed-bg
+000349a0: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
+000349b0: 702d 6967 6e6f 7265 642d 7465 7874 3a76  p-ignored-text:v
+000349c0: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+000349d0: 2d6d 6172 6b75 702d 6967 6e6f 7265 642d  -markup-ignored-
+000349e0: 7465 7874 293b 2d2d 7379 6e74 6178 2d6d  text);--syntax-m
+000349f0: 6172 6b75 702d 6967 6e6f 7265 642d 6267  arkup-ignored-bg
+00034a00: 3a76 6172 282d 2d73 796e 7461 782d 6461  :var(--syntax-da
+00034a10: 726b 2d6d 6172 6b75 702d 6967 6e6f 7265  rk-markup-ignore
+00034a20: 642d 6267 293b 2d2d 7379 6e74 6178 2d6d  d-bg);--syntax-m
+00034a30: 6574 612d 6469 6666 2d72 616e 6765 3a76  eta-diff-range:v
+00034a40: 6172 282d 2d73 796e 7461 782d 6461 726b  ar(--syntax-dark
+00034a50: 2d6d 6574 612d 6469 6666 2d72 616e 6765  -meta-diff-range
+00034a60: 293b 2d2d 7379 6e74 6178 2d73 7065 6369  );--syntax-speci
+00034a70: 616c 2d62 673a 7661 7228 2d2d 7379 6e74  al-bg:var(--synt
+00034a80: 6178 2d64 6172 6b2d 7370 6563 6961 6c2d  ax-dark-special-
+00034a90: 6267 297d 6874 6d6c 2e6c 6967 6874 202e  bg)}html.light .
+00034aa0: 6a75 7079 7465 725f 636f 6e74 6169 6e65  jupyter_containe
+00034ab0: 7220 2e63 656c 6c5f 6f75 7470 7574 2c68  r .cell_output,h
+00034ac0: 746d 6c2e 6c69 6768 7420 2e73 642d 7461  tml.light .sd-ta
+00034ad0: 622d 636f 6e74 656e 747b 2d2d 7379 6e74  b-content{--synt
+00034ae0: 6178 2d70 7265 2d62 673a 7661 7228 2d2d  ax-pre-bg:var(--
+00034af0: 636f 6c6f 722d 7375 7266 6163 652d 6163  color-surface-ac
+00034b00: 6365 6e74 293b 2d2d 7379 6e74 6178 2d63  cent);--syntax-c
+00034b10: 6170 2d62 673a 7661 7228 2d2d 6163 6365  ap-bg:var(--acce
+00034b20: 6e74 2d33 293b 2d2d 7379 6e74 6178 2d68  nt-3);--syntax-h
+00034b30: 6967 686c 6967 6874 2d62 673a 7661 7228  ighlight-bg:var(
+00034b40: 2d2d 6163 6365 6e74 2d61 3329 3b2d 2d73  --accent-a3);--s
+00034b50: 796e 7461 782d 7465 7874 3a76 6172 282d  yntax-text:var(-
+00034b60: 2d73 796e 7461 782d 6c69 6768 742d 7465  -syntax-light-te
+00034b70: 7874 293b 2d2d 7379 6e74 6178 2d6d 6574  xt);--syntax-met
+00034b80: 613a 7661 7228 2d2d 7379 6e74 6178 2d6c  a:var(--syntax-l
+00034b90: 6967 6874 2d6d 6574 6129 3b2d 2d73 796e  ight-meta);--syn
+00034ba0: 7461 782d 636f 6d6d 656e 743a 7661 7228  tax-comment:var(
+00034bb0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d63  --syntax-light-c
+00034bc0: 6f6d 6d65 6e74 293b 2d2d 7379 6e74 6178  omment);--syntax
+00034bd0: 2d63 6f6e 7374 616e 743a 7661 7228 2d2d  -constant:var(--
+00034be0: 7379 6e74 6178 2d6c 6967 6874 2d63 6f6e  syntax-light-con
+00034bf0: 7374 616e 7429 3b2d 2d73 796e 7461 782d  stant);--syntax-
+00034c00: 656e 7469 7479 3a76 6172 282d 2d73 796e  entity:var(--syn
+00034c10: 7461 782d 6c69 6768 742d 656e 7469 7479  tax-light-entity
+00034c20: 293b 2d2d 7379 6e74 6178 2d70 726f 7065  );--syntax-prope
+00034c30: 7274 793a 7661 7228 2d2d 7379 6e74 6178  rty:var(--syntax
+00034c40: 2d6c 6967 6874 2d70 726f 7065 7274 7929  -light-property)
+00034c50: 3b2d 2d73 796e 7461 782d 6465 6669 6e69  ;--syntax-defini
+00034c60: 7469 6f6e 3a76 6172 282d 2d73 796e 7461  tion:var(--synta
+00034c70: 782d 6c69 6768 742d 6465 6669 6e69 7469  x-light-definiti
+00034c80: 6f6e 293b 2d2d 7379 6e74 6178 2d74 6167  on);--syntax-tag
+00034c90: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
+00034ca0: 6768 742d 7461 6729 3b2d 2d73 796e 7461  ght-tag);--synta
+00034cb0: 782d 6275 696c 7469 6e3a 7661 7228 2d2d  x-builtin:var(--
+00034cc0: 7379 6e74 6178 2d6c 6967 6874 2d62 7569  syntax-light-bui
+00034cd0: 6c74 696e 293b 2d2d 7379 6e74 6178 2d6b  ltin);--syntax-k
+00034ce0: 6579 776f 7264 3a76 6172 282d 2d73 796e  eyword:var(--syn
+00034cf0: 7461 782d 6c69 6768 742d 6b65 7977 6f72  tax-light-keywor
+00034d00: 6429 3b2d 2d73 796e 7461 782d 6578 6365  d);--syntax-exce
+00034d10: 7074 696f 6e3a 7661 7228 2d2d 7379 6e74  ption:var(--synt
+00034d20: 6178 2d6c 6967 6874 2d65 7863 6570 7469  ax-light-excepti
+00034d30: 6f6e 293b 2d2d 7379 6e74 6178 2d73 7472  on);--syntax-str
+00034d40: 696e 673a 7661 7228 2d2d 7379 6e74 6178  ing:var(--syntax
+00034d50: 2d6c 6967 6874 2d73 7472 696e 6729 3b2d  -light-string);-
+00034d60: 2d73 796e 7461 782d 7265 6765 7870 3a76  -syntax-regexp:v
+00034d70: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+00034d80: 742d 7265 6765 7870 293b 2d2d 7379 6e74  t-regexp);--synt
+00034d90: 6178 2d76 6172 6961 626c 653a 7661 7228  ax-variable:var(
+00034da0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d76  --syntax-light-v
+00034db0: 6172 6961 626c 6529 3b2d 2d73 796e 7461  ariable);--synta
+00034dc0: 782d 696e 7661 6c69 642d 696c 6c65 6761  x-invalid-illega
+00034dd0: 6c2d 7465 7874 3a76 6172 282d 2d73 796e  l-text:var(--syn
+00034de0: 7461 782d 6c69 6768 742d 696e 7661 6c69  tax-light-invali
+00034df0: 642d 696c 6c65 6761 6c2d 7465 7874 293b  d-illegal-text);
+00034e00: 2d2d 7379 6e74 6178 2d69 6e76 616c 6964  --syntax-invalid
+00034e10: 2d69 6c6c 6567 616c 2d62 673a 7661 7228  -illegal-bg:var(
+00034e20: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d69  --syntax-light-i
+00034e30: 6e76 616c 6964 2d69 6c6c 6567 616c 2d62  nvalid-illegal-b
+00034e40: 6729 3b2d 2d73 796e 7461 782d 6d61 726b  g);--syntax-mark
+00034e50: 7570 2d68 6561 6469 6e67 3a76 6172 282d  up-heading:var(-
+00034e60: 2d73 796e 7461 782d 6c69 6768 742d 6d61  -syntax-light-ma
+00034e70: 726b 7570 2d68 6561 6469 6e67 293b 2d2d  rkup-heading);--
+00034e80: 7379 6e74 6178 2d6d 6172 6b75 702d 6974  syntax-markup-it
+00034e90: 616c 6963 3a76 6172 282d 2d73 796e 7461  alic:var(--synta
+00034ea0: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
+00034eb0: 7461 6c69 6329 3b2d 2d73 796e 7461 782d  talic);--syntax-
+00034ec0: 6d61 726b 7570 2d62 6f6c 643a 7661 7228  markup-bold:var(
+00034ed0: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+00034ee0: 6172 6b75 702d 626f 6c64 293b 2d2d 7379  arkup-bold);--sy
+00034ef0: 6e74 6178 2d6d 6172 6b75 702d 6465 6c65  ntax-markup-dele
+00034f00: 7465 642d 7465 7874 3a76 6172 282d 2d73  ted-text:var(--s
+00034f10: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
+00034f20: 7570 2d64 656c 6574 6564 2d74 6578 7429  up-deleted-text)
+00034f30: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00034f40: 2d64 656c 6574 6564 2d62 673a 7661 7228  -deleted-bg:var(
+00034f50: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+00034f60: 6172 6b75 702d 6465 6c65 7465 642d 6267  arkup-deleted-bg
+00034f70: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
+00034f80: 702d 696e 7365 7274 6564 2d74 6578 743a  p-inserted-text:
+00034f90: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+00034fa0: 6874 2d6d 6172 6b75 702d 696e 7365 7274  ht-markup-insert
+00034fb0: 6564 2d74 6578 7429 3b2d 2d73 796e 7461  ed-text);--synta
+00034fc0: 782d 6d61 726b 7570 2d69 6e73 6572 7465  x-markup-inserte
+00034fd0: 642d 6267 3a76 6172 282d 2d73 796e 7461  d-bg:var(--synta
+00034fe0: 782d 6c69 6768 742d 6d61 726b 7570 2d69  x-light-markup-i
+00034ff0: 6e73 6572 7465 642d 6267 293b 2d2d 7379  nserted-bg);--sy
+00035000: 6e74 6178 2d6d 6172 6b75 702d 6368 616e  ntax-markup-chan
+00035010: 6765 642d 7465 7874 3a76 6172 282d 2d73  ged-text:var(--s
+00035020: 796e 7461 782d 6c69 6768 742d 6d61 726b  yntax-light-mark
+00035030: 7570 2d63 6861 6e67 6564 2d74 6578 7429  up-changed-text)
+00035040: 3b2d 2d73 796e 7461 782d 6d61 726b 7570  ;--syntax-markup
+00035050: 2d63 6861 6e67 6564 2d62 673a 7661 7228  -changed-bg:var(
+00035060: 2d2d 7379 6e74 6178 2d6c 6967 6874 2d6d  --syntax-light-m
+00035070: 6172 6b75 702d 6368 616e 6765 642d 6267  arkup-changed-bg
+00035080: 293b 2d2d 7379 6e74 6178 2d6d 6172 6b75  );--syntax-marku
+00035090: 702d 6967 6e6f 7265 642d 7465 7874 3a76  p-ignored-text:v
+000350a0: 6172 282d 2d73 796e 7461 782d 6c69 6768  ar(--syntax-ligh
+000350b0: 742d 6d61 726b 7570 2d69 676e 6f72 6564  t-markup-ignored
+000350c0: 2d74 6578 7429 3b2d 2d73 796e 7461 782d  -text);--syntax-
+000350d0: 6d61 726b 7570 2d69 676e 6f72 6564 2d62  markup-ignored-b
+000350e0: 673a 7661 7228 2d2d 7379 6e74 6178 2d6c  g:var(--syntax-l
+000350f0: 6967 6874 2d6d 6172 6b75 702d 6967 6e6f  ight-markup-igno
+00035100: 7265 642d 6267 293b 2d2d 7379 6e74 6178  red-bg);--syntax
+00035110: 2d6d 6574 612d 6469 6666 2d72 616e 6765  -meta-diff-range
+00035120: 3a76 6172 282d 2d73 796e 7461 782d 6c69  :var(--syntax-li
+00035130: 6768 742d 6d65 7461 2d64 6966 662d 7261  ght-meta-diff-ra
+00035140: 6e67 6529 3b2d 2d73 796e 7461 782d 6869  nge);--syntax-hi
+00035150: 6768 6c69 6768 742d 6267 3a76 6172 282d  ghlight-bg:var(-
+00035160: 2d73 796e 7461 782d 6c69 6768 742d 6869  -syntax-light-hi
+00035170: 6768 6c69 6768 742d 6267 293b 2d2d 7379  ghlight-bg);--sy
+00035180: 6e74 6178 2d73 7065 6369 616c 2d62 673a  ntax-special-bg:
+00035190: 7661 7228 2d2d 7379 6e74 6178 2d6c 6967  var(--syntax-lig
+000351a0: 6874 2d73 7065 6369 616c 2d62 6729 7d2e  ht-special-bg)}.
+000351b0: 7379 2d6c 7369 6465 7b2d 2d68 6569 6768  sy-lside{--heigh
+000351c0: 743a 3432 7078 7d2e 7379 2d6c 7369 6465  t:42px}.sy-lside
+000351d0: 2d62 6f74 746f 6d7b 706f 7369 7469 6f6e  -bottom{position
+000351e0: 3a73 7469 636b 793b 626f 7474 6f6d 3a30  :sticky;bottom:0
+000351f0: 3b70 6164 6469 6e67 3a30 3b62 6f72 6465  ;padding:0;borde
+00035200: 722d 746f 703a 3170 7820 736f 6c69 6420  r-top:1px solid 
+00035210: 7661 7228 2d2d 7379 2d63 2d64 6976 6964  var(--sy-c-divid
+00035220: 6572 293b 6261 636b 6772 6f75 6e64 2d63  er);background-c
+00035230: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
+00035240: 6261 636b 6772 6f75 6e64 293b 2d2d 7477  background);--tw
+00035250: 2d73 6861 646f 773a 3020 2d31 3270 7820  -shadow:0 -12px 
+00035260: 3136 7078 2076 6172 282d 2d73 792d 632d  16px var(--sy-c-
+00035270: 6261 636b 6772 6f75 6e64 293b 626f 782d  background);box-
+00035280: 7368 6164 6f77 3a76 6172 282d 2d74 772d  shadow:var(--tw-
+00035290: 7269 6e67 2d6f 6666 7365 742d 7368 6164  ring-offset-shad
+000352a0: 6f77 2c30 2030 2023 3030 3030 292c 7661  ow,0 0 #0000),va
+000352b0: 7228 2d2d 7477 2d72 696e 672d 7368 6164  r(--tw-ring-shad
+000352c0: 6f77 2c30 2030 2023 3030 3030 292c 7661  ow,0 0 #0000),va
+000352d0: 7228 2d2d 7477 2d73 6861 646f 7729 7d2e  r(--tw-shadow)}.
+000352e0: 7379 2d6c 7369 6465 202e 7273 742d 7665  sy-lside .rst-ve
+000352f0: 7273 696f 6e73 7b70 6f73 6974 696f 6e3a  rsions{position:
+00035300: 7374 6174 6963 3b77 6964 7468 3a31 3030  static;width:100
+00035310: 253b 6261 636b 6772 6f75 6e64 2d63 6f6c  %;background-col
+00035320: 6f72 3a76 6172 282d 2d73 792d 632d 7375  or:var(--sy-c-su
+00035330: 7266 6163 6529 3b66 6f6e 742d 6661 6d69  rface);font-fami
+00035340: 6c79 3a76 6172 282d 2d73 792d 662d 7465  ly:var(--sy-f-te
+00035350: 7874 297d 2e73 792d 6c73 6964 6520 2e72  xt)}.sy-lside .r
+00035360: 7374 2d76 6572 7369 6f6e 7320 617b 636f  st-versions a{co
+00035370: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d6c  lor:var(--sy-c-l
+00035380: 696e 6b29 7d2e 7379 2d6c 7369 6465 202e  ink)}.sy-lside .
+00035390: 7273 742d 7665 7273 696f 6e73 2061 3a68  rst-versions a:h
+000353a0: 6f76 6572 7b63 6f6c 6f72 3a76 6172 282d  over{color:var(-
+000353b0: 2d73 792d 632d 6c69 6e6b 2d68 6f76 6572  -sy-c-link-hover
+000353c0: 297d 2e73 792d 6c73 6964 6520 2e72 7374  )}.sy-lside .rst
+000353d0: 2d76 6572 7369 6f6e 7320 2e72 7374 2d63  -versions .rst-c
+000353e0: 7572 7265 6e74 2d76 6572 7369 6f6e 7b62  urrent-version{b
+000353f0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00035400: 7661 7228 2d2d 7379 2d63 2d62 6163 6b67  var(--sy-c-backg
+00035410: 726f 756e 6429 3b63 6f6c 6f72 3a76 6172  round);color:var
+00035420: 282d 2d73 792d 632d 7465 7874 293b 7061  (--sy-c-text);pa
+00035430: 6464 696e 673a 3020 3172 656d 3b68 6569  dding:0 1rem;hei
+00035440: 6768 743a 7661 7228 2d2d 6865 6967 6874  ght:var(--height
+00035450: 293b 6c69 6e65 2d68 6569 6768 743a 7661  );line-height:va
+00035460: 7228 2d2d 6865 6967 6874 297d 2e73 792d  r(--height)}.sy-
+00035470: 6c73 6964 6520 2e72 7374 2d76 6572 7369  lside .rst-versi
+00035480: 6f6e 732e 7273 742d 6261 6467 6520 2e72  ons.rst-badge .r
+00035490: 7374 2d63 7572 7265 6e74 2d76 6572 7369  st-current-versi
+000354a0: 6f6e 7b74 6578 742d 616c 6967 6e3a 6c65  on{text-align:le
+000354b0: 6674 3b66 6f6e 742d 7369 7a65 3a2e 3934  ft;font-size:.94
+000354c0: 7265 6d3b 7061 6464 696e 673a 3020 3172  rem;padding:0 1r
+000354d0: 656d 3b68 6569 6768 743a 7661 7228 2d2d  em;height:var(--
+000354e0: 6865 6967 6874 293b 6c69 6e65 2d68 6569  height);line-hei
+000354f0: 6768 743a 7661 7228 2d2d 6865 6967 6874  ght:var(--height
+00035500: 297d 2e73 792d 6c73 6964 6520 2e72 7374  )}.sy-lside .rst
+00035510: 2d76 6572 7369 6f6e 7320 2e72 7374 2d63  -versions .rst-c
+00035520: 7572 7265 6e74 2d76 6572 7369 6f6e 202e  urrent-version .
+00035530: 6661 7b63 6f6c 6f72 3a76 6172 282d 2d73  fa{color:var(--s
+00035540: 792d 632d 7465 7874 297d 2e73 792d 6c73  y-c-text)}.sy-ls
+00035550: 6964 6520 2e72 7374 2d76 6572 7369 6f6e  ide .rst-version
+00035560: 732e 7273 742d 6261 6467 652e 7368 6966  s.rst-badge.shif
+00035570: 742d 7570 202e 7273 742d 6375 7272 656e  t-up .rst-curren
+00035580: 742d 7665 7273 696f 6e7b 7465 7874 2d61  t-version{text-a
+00035590: 6c69 676e 3a6c 6566 747d 2e73 792d 6c73  lign:left}.sy-ls
+000355a0: 6964 6520 2e72 7374 2d76 6572 7369 6f6e  ide .rst-version
+000355b0: 732e 7273 742d 6261 6467 652e 7368 6966  s.rst-badge.shif
+000355c0: 742d 7570 202e 7273 742d 6375 7272 656e  t-up .rst-curren
+000355d0: 742d 7665 7273 696f 6e20 2e66 612d 626f  t-version .fa-bo
+000355e0: 6f6b 7b66 6c6f 6174 3a6e 6f6e 657d 2e73  ok{float:none}.s
+000355f0: 792d 6c73 6964 6520 2e72 7374 2d6f 7468  y-lside .rst-oth
+00035600: 6572 2d76 6572 7369 6f6e 737b 666f 6e74  er-versions{font
+00035610: 2d73 697a 653a 2e38 3672 656d 3b62 6f72  -size:.86rem;bor
+00035620: 6465 722d 746f 703a 3170 7820 736f 6c69  der-top:1px soli
+00035630: 6420 7661 7228 2d2d 7379 2d63 2d64 6976  d var(--sy-c-div
+00035640: 6964 6572 297d 2e73 792d 6c73 6964 6520  ider)}.sy-lside 
+00035650: 2e72 7374 2d6f 7468 6572 2d76 6572 7369  .rst-other-versi
+00035660: 6f6e 7320 6474 7b66 6f6e 742d 7369 7a65  ons dt{font-size
+00035670: 3a2e 3638 7265 6d3b 666f 6e74 2d77 6569  :.68rem;font-wei
+00035680: 6768 743a 3530 303b 7061 6464 696e 673a  ght:500;padding:
+00035690: 3470 7820 3670 783b 636f 6c6f 723a 7661  4px 6px;color:va
+000356a0: 7228 2d2d 7379 2d63 2d6c 6967 6874 297d  r(--sy-c-light)}
+000356b0: 2e73 792d 6c73 6964 6520 2e72 7374 2d76  .sy-lside .rst-v
+000356c0: 6572 7369 6f6e 7320 2e72 7374 2d6f 7468  ersions .rst-oth
+000356d0: 6572 2d76 6572 7369 6f6e 7320 6464 2061  er-versions dd a
+000356e0: 7b63 6f6c 6f72 3a76 6172 282d 2d73 792d  {color:var(--sy-
+000356f0: 632d 7465 7874 297d 2e73 792d 6c73 6964  c-text)}.sy-lsid
+00035700: 6520 2e72 7374 2d76 6572 7369 6f6e 7320  e .rst-versions 
+00035710: 2e72 7374 2d6f 7468 6572 2d76 6572 7369  .rst-other-versi
+00035720: 6f6e 7320 6464 2061 3a68 6f76 6572 7b74  ons dd a:hover{t
+00035730: 6578 742d 6465 636f 7261 7469 6f6e 3a75  ext-decoration:u
+00035740: 6e64 6572 6c69 6e65 3b63 6f6c 6f72 3a76  nderline;color:v
+00035750: 6172 282d 2d73 792d 632d 6c69 6e6b 2d68  ar(--sy-c-link-h
+00035760: 6f76 6572 297d 2e73 792d 6c73 6964 6520  over)}.sy-lside 
+00035770: 2e72 7374 2d76 6572 7369 6f6e 7320 696e  .rst-versions in
+00035780: 7075 747b 7769 6474 683a 3130 3025 3b70  put{width:100%;p
+00035790: 6164 6469 6e67 3a36 7078 2031 3270 783b  adding:6px 12px;
+000357a0: 666f 6e74 2d73 697a 653a 2e39 3272 656d  font-size:.92rem
+000357b0: 3b66 6f6e 742d 6661 6d69 6c79 3a76 6172  ;font-family:var
+000357c0: 282d 2d73 792d 662d 7465 7874 293b 626f  (--sy-f-text);bo
+000357d0: 7264 6572 2d72 6164 6975 733a 3670 783b  rder-radius:6px;
+000357e0: 6f75 746c 696e 653a 303b 6261 636b 6772  outline:0;backgr
+000357f0: 6f75 6e64 3a76 6172 282d 2d73 792d 632d  ound:var(--sy-c-
+00035800: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
+00035810: 6572 3a31 7078 2073 6f6c 6964 2076 6172  er:1px solid var
+00035820: 282d 2d73 792d 632d 626f 7264 6572 297d  (--sy-c-border)}
+00035830: 2e73 792d 6c73 6964 6520 2e72 7374 2d76  .sy-lside .rst-v
+00035840: 6572 7369 6f6e 7320 2e72 7374 2d6f 7468  ersions .rst-oth
+00035850: 6572 2d76 6572 7369 6f6e 7320 6872 7b62  er-versions hr{b
+00035860: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
+00035870: 2d2d 7379 2d63 2d64 6976 6964 6572 297d  --sy-c-divider)}
+00035880: 406d 6564 6961 2028 6d69 6e2d 7769 6474  @media (min-widt
+00035890: 683a 3930 7265 6d29 7b2e 7379 2d6c 7369  h:90rem){.sy-lsi
+000358a0: 6465 202e 7273 742d 7665 7273 696f 6e73  de .rst-versions
+000358b0: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
+000358c0: 2d2d 7379 2d63 2d62 6163 6b67 726f 756e  --sy-c-backgroun
+000358d0: 6429 7d7d 2e79 7565 2062 7574 746f 6e2e  d)}}.yue button.
+000358e0: 636f 7079 6274 6e7b 616c 6967 6e2d 6974  copybtn{align-it
+000358f0: 656d 733a 6365 6e74 6572 3b6a 7573 7469  ems:center;justi
+00035900: 6679 2d63 6f6e 7465 6e74 3a63 656e 7465  fy-content:cente
+00035910: 723b 6261 636b 6772 6f75 6e64 2d63 6f6c  r;background-col
+00035920: 6f72 3a69 6e69 7469 616c 3b62 6f72 6465  or:initial;borde
+00035930: 723a 6e6f 6e65 3b63 6f6c 6f72 3a76 6172  r:none;color:var
+00035940: 282d 2d73 796e 7461 782d 7465 7874 297d  (--syntax-text)}
+00035950: 2e79 7565 2062 7574 746f 6e2e 636f 7079  .yue button.copy
+00035960: 6274 6e3e 7376 677b 7769 6474 683a 312e  btn>svg{width:1.
+00035970: 3472 656d 3b68 6569 6768 743a 312e 3472  4rem;height:1.4r
+00035980: 656d 7d2e 7975 6520 6275 7474 6f6e 2e63  em}.yue button.c
+00035990: 6f70 7962 746e 3a68 6f76 6572 7b63 6f6c  opybtn:hover{col
+000359a0: 6f72 3a76 6172 282d 2d73 796e 7461 782d  or:var(--syntax-
+000359b0: 6d65 7461 297d 2e79 7565 202e 6869 6768  meta)}.yue .high
+000359c0: 6c69 6768 7420 6275 7474 6f6e 2e63 6f70  light button.cop
+000359d0: 7962 746e 3a68 6f76 6572 7b62 6163 6b67  ybtn:hover{backg
+000359e0: 726f 756e 642d 636f 6c6f 723a 696e 6974  round-color:init
+000359f0: 6961 6c7d 2e79 7565 2062 7574 746f 6e2e  ial}.yue button.
+00035a00: 636f 7079 6274 6e3a 6166 7465 727b 6261  copybtn:after{ba
+00035a10: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a69  ckground-color:i
+00035a20: 6e69 7469 616c 3b63 6f6c 6f72 3a76 6172  nitial;color:var
+00035a30: 282d 2d73 796e 7461 782d 7465 7874 297d  (--syntax-text)}
+00035a40: 2e79 7565 2062 7574 746f 6e2e 636f 7079  .yue button.copy
+00035a50: 6274 6e2e 7375 6363 6573 737b 626f 7264  btn.success{bord
+00035a60: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d67  er-color:var(--g
+00035a70: 7265 656e 2d61 3130 293b 636f 6c6f 723a  reen-a10);color:
+00035a80: 7661 7228 2d2d 6772 6565 6e2d 6131 3029  var(--green-a10)
+00035a90: 7d2e 7975 6520 6275 7474 6f6e 2e63 6f70  }.yue button.cop
+00035aa0: 7962 746e 2e73 7563 6365 7373 3a61 6674  ybtn.success:aft
+00035ab0: 6572 7b63 6f6c 6f72 3a76 6172 282d 2d67  er{color:var(--g
+00035ac0: 7265 656e 2d61 3130 297d 2e79 7565 7b2d  reen-a10)}.yue{-
+00035ad0: 2d73 642d 636f 6c6f 722d 7072 696d 6172  -sd-color-primar
+00035ae0: 793a 7661 7228 2d2d 6163 6365 6e74 2d61  y:var(--accent-a
+00035af0: 3131 293b 2d2d 7364 2d63 6f6c 6f72 2d73  11);--sd-color-s
+00035b00: 6563 6f6e 6461 7279 3a76 6172 282d 2d67  econdary:var(--g
+00035b10: 6f6c 642d 6131 3129 3b2d 2d73 642d 636f  old-a11);--sd-co
+00035b20: 6c6f 722d 7375 6363 6573 733a 7661 7228  lor-success:var(
+00035b30: 2d2d 6772 6565 6e2d 6131 3129 3b2d 2d73  --green-a11);--s
+00035b40: 642d 636f 6c6f 722d 696e 666f 3a76 6172  d-color-info:var
+00035b50: 282d 2d62 6c75 652d 6131 3129 3b2d 2d73  (--blue-a11);--s
+00035b60: 642d 636f 6c6f 722d 7761 726e 696e 673a  d-color-warning:
+00035b70: 7661 7228 2d2d 6f72 616e 6765 2d61 3131  var(--orange-a11
+00035b80: 293b 2d2d 7364 2d63 6f6c 6f72 2d64 616e  );--sd-color-dan
+00035b90: 6765 723a 7661 7228 2d2d 7265 642d 6131  ger:var(--red-a1
+00035ba0: 3129 3b2d 2d73 642d 636f 6c6f 722d 6c69  1);--sd-color-li
+00035bb0: 6768 743a 7661 7228 2d2d 7361 6e64 2d61  ght:var(--sand-a
+00035bc0: 3229 3b2d 2d73 642d 636f 6c6f 722d 6d75  2);--sd-color-mu
+00035bd0: 7465 643a 7661 7228 2d2d 6772 6179 2d38  ted:var(--gray-8
+00035be0: 293b 2d2d 7364 2d63 6f6c 6f72 2d64 6172  );--sd-color-dar
+00035bf0: 6b3a 2332 3132 3132 323b 2d2d 7364 2d63  k:#212122;--sd-c
+00035c00: 6f6c 6f72 2d62 6c61 636b 3a23 3030 303b  olor-black:#000;
+00035c10: 2d2d 7364 2d63 6f6c 6f72 2d77 6869 7465  --sd-color-white
+00035c20: 3a23 6666 663b 2d2d 7364 2d63 6f6c 6f72  :#fff;--sd-color
+00035c30: 2d70 7269 6d61 7279 2d68 6967 686c 6967  -primary-highlig
+00035c40: 6874 3a76 6172 282d 2d61 6363 656e 742d  ht:var(--accent-
+00035c50: 6138 293b 2d2d 7364 2d63 6f6c 6f72 2d73  a8);--sd-color-s
+00035c60: 6563 6f6e 6461 7279 2d68 6967 686c 6967  econdary-highlig
+00035c70: 6874 3a76 6172 282d 2d67 6f6c 642d 6138  ht:var(--gold-a8
+00035c80: 293b 2d2d 7364 2d63 6f6c 6f72 2d73 7563  );--sd-color-suc
+00035c90: 6365 7373 2d68 6967 686c 6967 6874 3a76  cess-highlight:v
+00035ca0: 6172 282d 2d67 7265 656e 2d61 3829 3b2d  ar(--green-a8);-
+00035cb0: 2d73 642d 636f 6c6f 722d 696e 666f 2d68  -sd-color-info-h
+00035cc0: 6967 686c 6967 6874 3a76 6172 282d 2d62  ighlight:var(--b
+00035cd0: 6c75 652d 6138 293b 2d2d 7364 2d63 6f6c  lue-a8);--sd-col
+00035ce0: 6f72 2d77 6172 6e69 6e67 2d68 6967 686c  or-warning-highl
+00035cf0: 6967 6874 3a76 6172 282d 2d6f 7261 6e67  ight:var(--orang
+00035d00: 652d 6138 293b 2d2d 7364 2d63 6f6c 6f72  e-a8);--sd-color
+00035d10: 2d64 616e 6765 722d 6869 6768 6c69 6768  -danger-highligh
+00035d20: 743a 7661 7228 2d2d 7265 642d 6138 293b  t:var(--red-a8);
+00035d30: 2d2d 7364 2d63 6f6c 6f72 2d6c 6967 6874  --sd-color-light
+00035d40: 2d68 6967 686c 6967 6874 3a76 6172 282d  -highlight:var(-
+00035d50: 2d67 7261 792d 3429 3b2d 2d73 642d 636f  -gray-4);--sd-co
+00035d60: 6c6f 722d 6d75 7465 642d 6869 6768 6c69  lor-muted-highli
+00035d70: 6768 743a 7661 7228 2d2d 6772 6179 2d31  ght:var(--gray-1
+00035d80: 3129 3b2d 2d73 642d 636f 6c6f 722d 6461  1);--sd-color-da
+00035d90: 726b 2d68 6967 686c 6967 6874 3a23 3132  rk-highlight:#12
+00035da0: 3132 3131 3b2d 2d73 642d 636f 6c6f 722d  1211;--sd-color-
+00035db0: 626c 6163 6b2d 6869 6768 6c69 6768 743a  black-highlight:
+00035dc0: 2330 3030 3b2d 2d73 642d 636f 6c6f 722d  #000;--sd-color-
+00035dd0: 7768 6974 652d 6869 6768 6c69 6768 743a  white-highlight:
+00035de0: 2364 3964 3964 393b 2d2d 7364 2d63 6f6c  #d9d9d9;--sd-col
+00035df0: 6f72 2d70 7269 6d61 7279 2d74 6578 743a  or-primary-text:
+00035e00: 7661 7228 2d2d 6163 6365 6e74 2d39 2d63  var(--accent-9-c
+00035e10: 6f6e 7472 6173 7429 3b2d 2d73 642d 636f  ontrast);--sd-co
+00035e20: 6c6f 722d 7365 636f 6e64 6172 792d 7465  lor-secondary-te
+00035e30: 7874 3a76 6172 282d 2d67 6f6c 642d 392d  xt:var(--gold-9-
+00035e40: 636f 6e74 7261 7374 293b 2d2d 7364 2d63  contrast);--sd-c
+00035e50: 6f6c 6f72 2d73 7563 6365 7373 2d74 6578  olor-success-tex
+00035e60: 743a 7661 7228 2d2d 6772 6565 6e2d 392d  t:var(--green-9-
+00035e70: 636f 6e74 7261 7374 293b 2d2d 7364 2d63  contrast);--sd-c
+00035e80: 6f6c 6f72 2d69 6e66 6f2d 7465 7874 3a76  olor-info-text:v
+00035e90: 6172 282d 2d62 6c75 652d 392d 636f 6e74  ar(--blue-9-cont
+00035ea0: 7261 7374 293b 2d2d 7364 2d63 6f6c 6f72  rast);--sd-color
+00035eb0: 2d77 6172 6e69 6e67 2d74 6578 743a 7661  -warning-text:va
+00035ec0: 7228 2d2d 6f72 616e 6765 2d39 2d63 6f6e  r(--orange-9-con
+00035ed0: 7472 6173 7429 3b2d 2d73 642d 636f 6c6f  trast);--sd-colo
+00035ee0: 722d 6461 6e67 6572 2d74 6578 743a 7661  r-danger-text:va
+00035ef0: 7228 2d2d 7265 642d 392d 636f 6e74 7261  r(--red-9-contra
+00035f00: 7374 293b 2d2d 7364 2d63 6f6c 6f72 2d6c  st);--sd-color-l
+00035f10: 6967 6874 2d74 6578 743a 7661 7228 2d2d  ight-text:var(--
+00035f20: 7379 2d63 2d74 6578 7429 3b2d 2d73 642d  sy-c-text);--sd-
+00035f30: 636f 6c6f 722d 6d75 7465 642d 7465 7874  color-muted-text
+00035f40: 3a23 6666 663b 2d2d 7364 2d63 6f6c 6f72  :#fff;--sd-color
+00035f50: 2d64 6172 6b2d 7465 7874 3a23 6666 663b  -dark-text:#fff;
+00035f60: 2d2d 7364 2d63 6f6c 6f72 2d62 6c61 636b  --sd-color-black
+00035f70: 2d74 6578 743a 2366 6666 3b2d 2d73 642d  -text:#fff;--sd-
+00035f80: 636f 6c6f 722d 7768 6974 652d 7465 7874  color-white-text
+00035f90: 3a23 3231 3235 3239 3b2d 2d73 642d 636f  :#212529;--sd-co
+00035fa0: 6c6f 722d 7368 6164 6f77 3a76 6172 282d  lor-shadow:var(-
+00035fb0: 2d67 7261 792d 3129 3b2d 2d73 642d 636f  -gray-1);--sd-co
+00035fc0: 6c6f 722d 6361 7264 2d62 6f72 6465 723a  lor-card-border:
+00035fd0: 7661 7228 2d2d 7379 2d63 2d62 6f72 6465  var(--sy-c-borde
+00035fe0: 7229 3b2d 2d73 642d 636f 6c6f 722d 6361  r);--sd-color-ca
+00035ff0: 7264 2d62 6f72 6465 722d 686f 7665 723a  rd-border-hover:
+00036000: 7661 7228 2d2d 6163 6365 6e74 2d61 3929  var(--accent-a9)
+00036010: 3b2d 2d73 642d 636f 6c6f 722d 7461 6273  ;--sd-color-tabs
+00036020: 2d6c 6162 656c 2d69 6e61 6374 6976 653a  -label-inactive:
+00036030: 7661 7228 2d2d 7379 2d63 2d62 6f6c 6429  var(--sy-c-bold)
+00036040: 3b2d 2d73 642d 636f 6c6f 722d 7461 6273  ;--sd-color-tabs
+00036050: 2d6c 6162 656c 2d61 6374 6976 653a 7661  -label-active:va
+00036060: 7228 2d2d 7364 2d63 6f6c 6f72 2d70 7269  r(--sd-color-pri
+00036070: 6d61 7279 293b 2d2d 7364 2d63 6f6c 6f72  mary);--sd-color
+00036080: 2d74 6162 732d 756e 6465 726c 696e 652d  -tabs-underline-
+00036090: 6163 7469 7665 3a76 6172 282d 2d73 642d  active:var(--sd-
+000360a0: 636f 6c6f 722d 7072 696d 6172 7929 3b2d  color-primary);-
+000360b0: 2d73 642d 636f 6c6f 722d 7461 6273 2d6c  -sd-color-tabs-l
+000360c0: 6162 656c 2d68 6f76 6572 3a76 6172 282d  abel-hover:var(-
+000360d0: 2d61 6363 656e 742d 3929 3b2d 2d73 642d  -accent-9);--sd-
+000360e0: 636f 6c6f 722d 7461 6273 2d75 6e64 6572  color-tabs-under
+000360f0: 6c69 6e65 2d68 6f76 6572 3a76 6172 282d  line-hover:var(-
+00036100: 2d61 6363 656e 742d 3929 7d2e 7975 6520  -accent-9)}.yue 
+00036110: 2e73 7572 6661 6365 7b2d 2d73 642d 636f  .surface{--sd-co
+00036120: 6c6f 722d 6361 7264 2d74 6578 743a 7661  lor-card-text:va
+00036130: 7228 2d2d 7379 2d63 2d6c 6967 6874 293b  r(--sy-c-light);
+00036140: 2d2d 7364 2d63 6f6c 6f72 2d63 6172 642d  --sd-color-card-
+00036150: 626f 7264 6572 3a23 3030 3030 3b2d 2d73  border:#0000;--s
+00036160: 642d 636f 6c6f 722d 6361 7264 2d62 6163  d-color-card-bac
+00036170: 6b67 726f 756e 643a 7661 7228 2d2d 7379  kground:var(--sy
+00036180: 2d63 2d73 7572 6661 6365 297d 2e79 7565  -c-surface)}.yue
+00036190: 2061 2e73 642d 6261 6467 652c 2e79 7565   a.sd-badge,.yue
+000361a0: 2061 2e73 642d 6261 6467 653a 686f 7665   a.sd-badge:hove
+000361b0: 727b 626f 7264 6572 2d62 6f74 746f 6d3a  r{border-bottom:
+000361c0: 307d 2e79 7565 202e 7364 2d62 6164 6765  0}.yue .sd-badge
+000361d0: 7b66 6f6e 742d 7765 6967 6874 3a36 3030  {font-weight:600
+000361e0: 3b62 6f72 6465 722d 7261 6469 7573 3a33  ;border-radius:3
+000361f0: 7078 7d2e 7975 6520 2e73 642d 6274 6e7b  px}.yue .sd-btn{
+00036200: 626f 7264 6572 2d63 6f6c 6f72 3a76 6172  border-color:var
+00036210: 282d 2d73 792d 632d 626f 7264 6572 297d  (--sy-c-border)}
+00036220: 2e79 7565 202e 7364 2d74 6162 2d73 6574  .yue .sd-tab-set
+00036230: 3e6c 6162 656c 7b70 6164 6469 6e67 3a31  >label{padding:1
+00036240: 7265 6d20 2e32 3572 656d 202e 3572 656d  rem .25rem .5rem
+00036250: 3b66 6f6e 742d 7369 7a65 3a2e 3834 7265  ;font-size:.84re
+00036260: 6d3b 666f 6e74 2d77 6569 6768 743a 3530  m;font-weight:50
+00036270: 307d 2e79 7565 202e 7364 2d74 6162 2d73  0}.yue .sd-tab-s
+00036280: 6574 3e6c 6162 656c 7e6c 6162 656c 7b6d  et>label~label{m
+00036290: 6172 6769 6e2d 6c65 6674 3a31 7265 6d7d  argin-left:1rem}
+000362a0: 2e79 7565 202e 7364 2d74 6162 2d63 6f6e  .yue .sd-tab-con
+000362b0: 7465 6e74 7b70 6164 6469 6e67 3a30 3b62  tent{padding:0;b
+000362c0: 6f78 2d73 6861 646f 773a 3020 2d2e 3036  ox-shadow:0 -.06
+000362d0: 3235 7265 6d20 7661 7228 2d2d 7379 2d63  25rem var(--sy-c
+000362e0: 2d64 6976 6964 6572 297d 2e79 7565 202e  -divider)}.yue .
+000362f0: 7364 2d74 6162 2d63 6f6e 7465 6e74 202e  sd-tab-content .
+00036300: 636f 6465 2d62 6c6f 636b 2d63 6170 7469  code-block-capti
+00036310: 6f6e 2c2e 7975 6520 2e73 642d 7461 622d  on,.yue .sd-tab-
+00036320: 636f 6e74 656e 7420 2e68 6967 686c 6967  content .highlig
+00036330: 6874 2070 7265 7b62 6f72 6465 722d 7261  ht pre{border-ra
+00036340: 6469 7573 3a30 7d2e 7975 6520 2e73 642d  dius:0}.yue .sd-
+00036350: 6361 7264 2d74 6974 6c65 7b63 6f6c 6f72  card-title{color
+00036360: 3a76 6172 282d 2d73 792d 632d 7465 7874  :var(--sy-c-text
+00036370: 297d 2e79 7565 202e 7364 2d63 6172 642d  )}.yue .sd-card-
+00036380: 7469 746c 653e 7376 677b 706f 7369 7469  title>svg{positi
+00036390: 6f6e 3a72 656c 6174 6976 653b 746f 703a  on:relative;top:
+000363a0: 2d31 7078 3b6d 6172 6769 6e2d 7269 6768  -1px;margin-righ
+000363b0: 743a 2e32 3572 656d 7d2e 7975 6520 2e73  t:.25rem}.yue .s
+000363c0: 642d 6361 7264 2d68 6f76 6572 3a68 6f76  d-card-hover:hov
+000363d0: 6572 7b74 7261 6e73 666f 726d 3a73 6361  er{transform:sca
+000363e0: 6c65 2831 297d 2e79 7565 202e 7364 2d63  le(1)}.yue .sd-c
+000363f0: 6172 642d 686f 7665 723a 686f 7665 7220  ard-hover:hover 
+00036400: 2e73 642d 6361 7264 2d74 6974 6c65 7b63  .sd-card-title{c
+00036410: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
+00036420: 6c69 6e6b 2d68 6f76 6572 297d 2e79 7565  link-hover)}.yue
+00036430: 202e 7364 2d63 6172 6420 612c 2e79 7565   .sd-card a,.yue
+00036440: 202e 7364 2d63 6172 6420 613a 686f 7665   .sd-card a:hove
+00036450: 727b 626f 7264 6572 2d62 6f74 746f 6d3a  r{border-bottom:
+00036460: 307d 2e79 7565 202e 7375 7266 6163 6520  0}.yue .surface 
+00036470: 2e73 642d 6361 7264 2d62 6f64 792c 2e79  .sd-card-body,.y
+00036480: 7565 202e 7375 7266 6163 6520 2e73 642d  ue .surface .sd-
+00036490: 6361 7264 2d66 6f6f 7465 722c 2e79 7565  card-footer,.yue
+000364a0: 202e 7375 7266 6163 6520 2e73 642d 6361   .surface .sd-ca
+000364b0: 7264 2d68 6561 6465 727b 7061 6464 696e  rd-header{paddin
+000364c0: 672d 6c65 6674 3a31 2e35 7265 6d3b 7061  g-left:1.5rem;pa
+000364d0: 6464 696e 672d 7269 6768 743a 312e 3572  dding-right:1.5r
+000364e0: 656d 7d2e 7975 6520 2e73 7572 6661 6365  em}.yue .surface
+000364f0: 202e 7364 2d63 6172 642d 666f 6f74 6572   .sd-card-footer
+00036500: 2c2e 7975 6520 2e73 7572 6661 6365 202e  ,.yue .surface .
+00036510: 7364 2d63 6172 642d 6865 6164 6572 7b62  sd-card-header{b
+00036520: 6f72 6465 722d 636f 6c6f 723a 7661 7228  order-color:var(
+00036530: 2d2d 7379 2d63 2d62 6f72 6465 7229 7d40  --sy-c-border)}@
+00036540: 6d65 6469 6120 2870 7269 6e74 297b 2e79  media (print){.y
+00036550: 7565 202e 7364 2d63 6172 647b 7061 6765  ue .sd-card{page
+00036560: 2d62 7265 616b 2d69 6e73 6964 653a 6176  -break-inside:av
+00036570: 6f69 647d 7d2e 7975 6520 612e 7364 2d74  oid}}.yue a.sd-t
+00036580: 6578 742d 7772 6170 3a68 6f76 6572 7b62  ext-wrap:hover{b
+00036590: 6f72 6465 722d 626f 7474 6f6d 2d77 6964  order-bottom-wid
+000365a0: 7468 3a31 7078 7d2e 7370 6869 6e78 2d74  th:1px}.sphinx-t
+000365b0: 6162 7320 5b72 6f6c 653d 7461 626c 6973  abs [role=tablis
+000365c0: 745d 7b62 6f72 6465 722d 636f 6c6f 723a  t]{border-color:
+000365d0: 7661 7228 2d2d 7379 2d63 2d64 6976 6964  var(--sy-c-divid
+000365e0: 6572 297d 2e79 7565 202e 7370 6869 6e78  er)}.yue .sphinx
+000365f0: 2d74 6162 732d 7461 627b 636f 6c6f 723a  -tabs-tab{color:
+00036600: 7661 7228 2d2d 7379 2d63 2d74 6578 7429  var(--sy-c-text)
+00036610: 3b6c 696e 652d 6865 6967 6874 3a69 6e68  ;line-height:inh
+00036620: 6572 6974 3b70 6164 6469 6e67 3a31 7265  erit;padding:1re
+00036630: 6d20 2e32 3572 656d 202e 3572 656d 3b66  m .25rem .5rem;f
+00036640: 6f6e 742d 7369 7a65 3a2e 3834 7265 6d3b  ont-size:.84rem;
+00036650: 666f 6e74 2d77 6569 6768 743a 3530 303b  font-weight:500;
+00036660: 626f 7264 6572 3a6e 6f6e 653b 626f 7264  border:none;bord
+00036670: 6572 2d62 6f74 746f 6d3a 2e31 3235 7265  er-bottom:.125re
+00036680: 6d20 736f 6c69 6420 2330 3030 307d 2e79  m solid #0000}.y
+00036690: 7565 202e 7370 6869 6e78 2d74 6162 732d  ue .sphinx-tabs-
+000366a0: 7461 623a 686f 7665 727b 636f 6c6f 723a  tab:hover{color:
+000366b0: 7661 7228 2d2d 7364 2d63 6f6c 6f72 2d74  var(--sd-color-t
+000366c0: 6162 732d 6c61 6265 6c2d 686f 7665 7229  abs-label-hover)
+000366d0: 3b62 6f72 6465 722d 636f 6c6f 723a 7661  ;border-color:va
+000366e0: 7228 2d2d 7364 2d63 6f6c 6f72 2d74 6162  r(--sd-color-tab
+000366f0: 732d 756e 6465 726c 696e 652d 686f 7665  s-underline-hove
+00036700: 7229 7d2e 7975 6520 2e73 7068 696e 782d  r)}.yue .sphinx-
+00036710: 7461 6273 2d74 6162 5b61 7269 612d 7365  tabs-tab[aria-se
+00036720: 6c65 6374 6564 3d74 7275 655d 7b62 6f72  lected=true]{bor
+00036730: 6465 723a 6e6f 6e65 3b62 6f72 6465 722d  der:none;border-
+00036740: 626f 7474 6f6d 3a2e 3132 3572 656d 2073  bottom:.125rem s
+00036750: 6f6c 6964 2076 6172 282d 2d73 642d 636f  olid var(--sd-co
+00036760: 6c6f 722d 7461 6273 2d75 6e64 6572 6c69  lor-tabs-underli
+00036770: 6e65 2d61 6374 6976 6529 3b63 6f6c 6f72  ne-active);color
+00036780: 3a76 6172 282d 2d73 642d 636f 6c6f 722d  :var(--sd-color-
+00036790: 7461 6273 2d6c 6162 656c 2d61 6374 6976  tabs-label-activ
+000367a0: 6529 3b62 6163 6b67 726f 756e 642d 636f  e);background-co
+000367b0: 6c6f 723a 696e 6974 6961 6c7d 2e79 7565  lor:initial}.yue
+000367c0: 202e 7370 6869 6e78 2d74 6162 732d 7461   .sphinx-tabs-ta
+000367d0: 622b 2e73 7068 696e 782d 7461 6273 2d74  b+.sphinx-tabs-t
+000367e0: 6162 7b6d 6172 6769 6e2d 6c65 6674 3a31  ab{margin-left:1
+000367f0: 7265 6d7d 2e79 7565 202e 7370 6869 6e78  rem}.yue .sphinx
+00036800: 2d74 6162 732d 7061 6e65 6c7b 626f 7264  -tabs-panel{bord
+00036810: 6572 3a6e 6f6e 653b 7061 6464 696e 673a  er:none;padding:
+00036820: 303b 6d61 7267 696e 3a30 3b62 6f72 6465  0;margin:0;borde
+00036830: 722d 7261 6469 7573 3a30 3b62 6163 6b67  r-radius:0;backg
+00036840: 726f 756e 642d 636f 6c6f 723a 696e 6974  round-color:init
+00036850: 6961 6c7d 2e79 7565 202e 7370 6869 6e78  ial}.yue .sphinx
+00036860: 2d74 6162 732d 7061 6e65 6c2e 636f 6465  -tabs-panel.code
+00036870: 2d74 6162 7b70 6164 6469 6e67 3a30 7d2e  -tab{padding:0}.
+00036880: 7975 6520 2e73 7068 696e 782d 7461 6273  yue .sphinx-tabs
+00036890: 2d70 616e 656c 2e63 6f64 652d 7461 6220  -panel.code-tab 
+000368a0: 2e63 6f64 652d 626c 6f63 6b2d 6361 7074  .code-block-capt
+000368b0: 696f 6e2c 2e79 7565 202e 7370 6869 6e78  ion,.yue .sphinx
+000368c0: 2d74 6162 732d 7061 6e65 6c2e 636f 6465  -tabs-panel.code
+000368d0: 2d74 6162 202e 6869 6768 6c69 6768 7420  -tab .highlight 
+000368e0: 7072 657b 626f 7264 6572 2d72 6164 6975  pre{border-radiu
+000368f0: 733a 307d 2e79 7565 7b2d 2d6a 702d 7769  s:0}.yue{--jp-wi
+00036900: 6467 6574 732d 696e 7075 742d 626f 7264  dgets-input-bord
+00036910: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d67  er-color:var(--g
+00036920: 7261 792d 3529 3b2d 2d6a 702d 7769 6467  ray-5);--jp-widg
+00036930: 6574 732d 696e 7075 742d 666f 6375 732d  ets-input-focus-
+00036940: 626f 7264 6572 2d63 6f6c 6f72 3a76 6172  border-color:var
+00036950: 282d 2d67 7261 792d 3829 3b2d 2d6a 702d  (--gray-8);--jp-
+00036960: 7769 6467 6574 732d 736c 6964 6572 2d61  widgets-slider-a
+00036970: 6374 6976 652d 6861 6e64 6c65 2d63 6f6c  ctive-handle-col
+00036980: 6f72 3a76 6172 282d 2d67 7261 792d 3429  or:var(--gray-4)
+00036990: 3b2d 2d6a 702d 7769 6467 6574 732d 736c  ;--jp-widgets-sl
+000369a0: 6964 6572 2d68 616e 646c 652d 626f 7264  ider-handle-bord
+000369b0: 6572 2d63 6f6c 6f72 3a76 6172 282d 2d73  er-color:var(--s
+000369c0: 792d 632d 626f 7264 6572 297d 2e79 7565  y-c-border)}.yue
+000369d0: 202e 6a75 7079 7465 725f 636f 6e74 6169   .jupyter_contai
+000369e0: 6e65 727b 6261 636b 6772 6f75 6e64 2d63  ner{background-c
+000369f0: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
+00036a00: 6261 636b 6772 6f75 6e64 293b 626f 7264  background);bord
+00036a10: 6572 3a33 7078 2073 6f6c 6964 2076 6172  er:3px solid var
+00036a20: 282d 2d73 792d 632d 626f 7264 6572 293b  (--sy-c-border);
+00036a30: 626f 7264 6572 2d72 6164 6975 733a 3670  border-radius:6p
+00036a40: 783b 6f76 6572 666c 6f77 3a68 6964 6465  x;overflow:hidde
+00036a50: 6e3b 626f 782d 7368 6164 6f77 3a6e 6f6e  n;box-shadow:non
+00036a60: 657d 2e64 6f63 756d 656e 7420 2e79 7565  e}.document .yue
+00036a70: 202e 6a75 7079 7465 725f 636f 6e74 6169   .jupyter_contai
+00036a80: 6e65 7220 6469 765b 636c 6173 735e 3d68  ner div[class^=h
+00036a90: 6967 686c 6967 6874 5d7b 7061 6464 696e  ighlight]{paddin
+00036aa0: 673a 307d 2e79 7565 202e 6a75 7079 7465  g:0}.yue .jupyte
+00036ab0: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
+00036ac0: 6365 6c6c 5f69 6e70 7574 7b62 6163 6b67  cell_input{backg
+00036ad0: 726f 756e 642d 636f 6c6f 723a 7661 7228  round-color:var(
+00036ae0: 2d2d 7379 6e74 6178 2d70 7265 2d62 6729  --syntax-pre-bg)
+00036af0: 3b62 6f72 6465 723a 303b 626f 7264 6572  ;border:0;border
+00036b00: 2d72 6164 6975 733a 307d 2e79 7565 202e  -radius:0}.yue .
+00036b10: 6a75 7079 7465 725f 636f 6e74 6169 6e65  jupyter_containe
+00036b20: 7220 6469 762e 636f 6465 5f63 656c 6c20  r div.code_cell 
+00036b30: 7072 657b 7061 6464 696e 673a 307d 2e6a  pre{padding:0}.j
+00036b40: 7570 7974 6572 5f63 6f6e 7461 696e 6572  upyter_container
+00036b50: 2064 6976 2e63 656c 6c5f 6f75 7470 7574   div.cell_output
+00036b60: 202e 6f75 7470 7574 2c2e 6a75 7079 7465   .output,.jupyte
+00036b70: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
+00036b80: 6365 6c6c 5f6f 7574 7075 7420 2e73 7464  cell_output .std
+00036b90: 6572 722c 2e6a 7570 7974 6572 5f63 6f6e  err,.jupyter_con
+00036ba0: 7461 696e 6572 2064 6976 2e63 656c 6c5f  tainer div.cell_
+00036bb0: 6f75 7470 7574 202e 7769 6467 6574 2d73  output .widget-s
+00036bc0: 7562 6172 6561 7b70 6164 6469 6e67 3a2e  ubarea{padding:.
+00036bd0: 3572 656d 7d2e 6a75 7079 7465 725f 636f  5rem}.jupyter_co
+00036be0: 6e74 6169 6e65 7220 6469 762e 6365 6c6c  ntainer div.cell
+00036bf0: 5f6f 7574 7075 7420 2e73 7464 6572 7220  _output .stderr 
+00036c00: 2e73 7464 6572 727b 7061 6464 696e 673a  .stderr{padding:
+00036c10: 307d 2e6a 7570 7974 6572 2d77 6964 6765  0}.jupyter-widge
+00036c20: 742d 6873 6c69 6465 7220 2e73 6c69 6465  t-hslider .slide
+00036c30: 722d 636f 6e74 6169 6e65 722c 2e77 6964  r-container,.wid
+00036c40: 6765 742d 6873 6c69 6465 7220 2e73 6c69  get-hslider .sli
+00036c50: 6465 722d 636f 6e74 6169 6e65 727b 6469  der-container{di
+00036c60: 7370 6c61 793a 666c 6578 3b61 6c69 676e  splay:flex;align
+00036c70: 2d69 7465 6d73 3a63 656e 7465 727d 2e6a  -items:center}.j
+00036c80: 7570 7974 6572 2d77 6964 6765 742d 736c  upyter-widget-sl
+00036c90: 6964 6572 202e 6e6f 5569 2d74 6172 6765  ider .noUi-targe
+00036ca0: 742c 2e77 6964 6765 742d 736c 6964 6572  t,.widget-slider
+00036cb0: 202e 6e6f 5569 2d74 6172 6765 747b 7769   .noUi-target{wi
+00036cc0: 6474 683a 3130 3025 7d2e 6a75 7079 7465  dth:100%}.jupyte
+00036cd0: 725f 636f 6e74 6169 6e65 7220 6469 762e  r_container div.
+00036ce0: 636f 6465 5f63 656c 6c20 2e68 6967 686c  code_cell .highl
+00036cf0: 6967 6874 3e70 7265 7b70 6164 6469 6e67  ight>pre{padding
+00036d00: 3a31 7265 6d7d 2e6a 7570 7974 6572 5f63  :1rem}.jupyter_c
+00036d10: 6f6e 7461 696e 6572 2064 6976 2e63 6f64  ontainer div.cod
+00036d20: 655f 6365 6c6c 202e 6869 6768 6c69 6768  e_cell .highligh
+00036d30: 7420 2e68 6c6c 7b6d 6172 6769 6e2d 6c65  t .hll{margin-le
+00036d40: 6674 3a2d 3172 656d 3b6d 6172 6769 6e2d  ft:-1rem;margin-
+00036d50: 7269 6768 743a 2d31 7265 6d3b 7061 6464  right:-1rem;padd
+00036d60: 696e 673a 3020 3172 656d 7d2e 6a75 7079  ing:0 1rem}.jupy
+00036d70: 7465 725f 636f 6e74 6169 6e65 7220 6469  ter_container di
+00036d80: 762e 636f 6465 5f63 656c 6c20 2e68 6967  v.code_cell .hig
+00036d90: 686c 6967 6874 202e 6c69 6e65 6e6f 737b  hlight .linenos{
+00036da0: 6d61 7267 696e 2d72 6967 6874 3a2e 3872  margin-right:.8r
+00036db0: 656d 7d2e 7975 6520 2e6a 7570 7974 6572  em}.yue .jupyter
+00036dc0: 5f63 6f6e 7461 696e 6572 202e 7374 6465  _container .stde
+00036dd0: 7272 7b63 6f6c 6f72 3a76 6172 282d 2d72  rr{color:var(--r
+00036de0: 6564 2d61 3131 293b 6261 636b 6772 6f75  ed-a11);backgrou
+00036df0: 6e64 2d63 6f6c 6f72 3a76 6172 282d 2d72  nd-color:var(--r
+00036e00: 6564 2d61 3329 7d2e 7975 6520 2e6a 7570  ed-a3)}.yue .jup
+00036e10: 7974 6572 5f63 6f6e 7461 696e 6572 202e  yter_container .
+00036e20: 7374 6465 7272 202e 7374 6465 7272 7b62  stderr .stderr{b
+00036e30: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+00036e40: 696e 6974 6961 6c7d 2e6e 6269 6e70 7574  initial}.nbinput
+00036e50: 202e 6869 6768 6c69 6768 747b 2d2d 7261   .highlight{--ra
+00036e60: 6469 7573 3a31 7078 7d2e 7975 6520 6469  dius:1px}.yue di
+00036e70: 762e 6e62 6c61 7374 2e63 6f6e 7461 696e  v.nblast.contain
+00036e80: 6572 7b70 6164 6469 6e67 2d74 6f70 3a35  er{padding-top:5
+00036e90: 7078 7d2e 7975 6520 6469 762e 6e62 696e  px}.yue div.nbin
+00036ea0: 7075 742e 636f 6e74 6169 6e65 7220 6469  put.container di
+00036eb0: 762e 696e 7075 745f 6172 6561 7b62 6f72  v.input_area{bor
+00036ec0: 6465 722d 636f 6c6f 723a 7661 7228 2d2d  der-color:var(--
+00036ed0: 7379 2d63 2d62 6f72 6465 7229 7d2e 7975  sy-c-border)}.yu
+00036ee0: 6520 6469 762e 6e62 6f75 7470 7574 2e63  e div.nboutput.c
+00036ef0: 6f6e 7461 696e 6572 2064 6976 2e6f 7574  ontainer div.out
+00036f00: 7075 745f 6172 6561 2e73 7464 6572 727b  put_area.stderr{
+00036f10: 636f 6c6f 723a 7661 7228 2d2d 7265 642d  color:var(--red-
+00036f20: 6131 3129 3b62 6163 6b67 726f 756e 642d  a11);background-
+00036f30: 636f 6c6f 723a 7661 7228 2d2d 7265 642d  color:var(--red-
+00036f40: 6133 297d 2e79 7565 2064 6976 2e6e 626f  a3)}.yue div.nbo
+00036f50: 7574 7075 742e 636f 6e74 6169 6e65 7220  utput.container 
+00036f60: 6469 762e 6f75 7470 7574 5f61 7265 613e  div.output_area>
+00036f70: 2e6d 6174 682d 7772 6170 7065 723e 6469  .math-wrapper>di
+00036f80: 762e 6d61 7468 7b70 6164 6469 6e67 2d74  v.math{padding-t
+00036f90: 6f70 3a30 7d2e 7975 6520 2e6a 702d 5265  op:0}.yue .jp-Re
+00036fa0: 6e64 6572 6564 4854 4d4c 436f 6d6d 6f6e  nderedHTMLCommon
+00036fb0: 2074 6865 6164 2c2e 7975 6520 6469 762e   thead,.yue div.
+00036fc0: 7265 6e64 6572 6564 5f68 746d 6c20 7468  rendered_html th
+00036fd0: 6561 647b 626f 7264 6572 2d63 6f6c 6f72  ead{border-color
+00036fe0: 3a76 6172 282d 2d73 792d 632d 626f 7264  :var(--sy-c-bord
+00036ff0: 6572 297d 2e79 7565 202e 6a70 2d52 656e  er)}.yue .jp-Ren
+00037000: 6465 7265 6448 544d 4c43 6f6d 6d6f 6e20  deredHTMLCommon 
+00037010: 7462 6f64 7920 7472 2c2e 7975 6520 6469  tbody tr,.yue di
+00037020: 762e 7265 6e64 6572 6564 5f68 746d 6c20  v.rendered_html 
+00037030: 7462 6f64 7920 7472 7b63 6f6c 6f72 3a76  tbody tr{color:v
+00037040: 6172 282d 2d73 792d 632d 7465 7874 297d  ar(--sy-c-text)}
+00037050: 2e79 7565 202e 6a70 2d52 656e 6465 7265  .yue .jp-Rendere
+00037060: 6448 544d 4c43 6f6d 6d6f 6e20 7462 6f64  dHTMLCommon tbod
+00037070: 7920 7472 3a6e 7468 2d63 6869 6c64 286f  y tr:nth-child(o
+00037080: 6464 292c 2e79 7565 2064 6976 2e72 656e  dd),.yue div.ren
+00037090: 6465 7265 645f 6874 6d6c 2074 626f 6479  dered_html tbody
+000370a0: 2074 723a 6e74 682d 6368 696c 6428 6f64   tr:nth-child(od
+000370b0: 6429 7b62 6163 6b67 726f 756e 642d 636f  d){background-co
+000370c0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d73  lor:var(--sy-c-s
+000370d0: 7572 6661 6365 297d 2e79 7565 202e 6a70  urface)}.yue .jp
+000370e0: 2d52 656e 6465 7265 6448 544d 4c43 6f6d  -RenderedHTMLCom
+000370f0: 6d6f 6e20 7462 6f64 7920 7472 3a68 6f76  mon tbody tr:hov
+00037100: 6572 2c2e 7975 6520 6469 762e 7265 6e64  er,.yue div.rend
+00037110: 6572 6564 5f68 746d 6c20 7462 6f64 7920  ered_html tbody 
+00037120: 7472 3a68 6f76 6572 7b62 6163 6b67 726f  tr:hover{backgro
+00037130: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
+00037140: 636f 6c6f 722d 7375 7266 6163 652d 6163  color-surface-ac
+00037150: 6365 6e74 297d 2e79 7565 7b2d 2d73 672d  cent)}.yue{--sg-
+00037160: 7465 7874 2d63 6f6c 6f72 3a76 6172 282d  text-color:var(-
+00037170: 2d73 792d 632d 7465 7874 293b 2d2d 7367  -sy-c-text);--sg
+00037180: 2d62 6163 6b67 726f 756e 642d 636f 6c6f  -background-colo
+00037190: 723a 7661 7228 2d2d 7379 2d63 2d62 6163  r:var(--sy-c-bac
+000371a0: 6b67 726f 756e 6429 3b2d 2d73 672d 636f  kground);--sg-co
+000371b0: 6465 2d62 6163 6b67 726f 756e 642d 636f  de-background-co
+000371c0: 6c6f 723a 7661 7228 2d2d 7379 6e74 6178  lor:var(--syntax
+000371d0: 2d70 7265 2d62 6729 3b2d 2d73 672d 7472  -pre-bg);--sg-tr
+000371e0: 2d68 6f76 6572 2d63 6f6c 6f72 3a76 6172  -hover-color:var
+000371f0: 282d 2d61 6363 656e 742d 6133 293b 2d2d  (--accent-a3);--
+00037200: 7367 2d74 722d 6f64 642d 636f 6c6f 723a  sg-tr-odd-color:
+00037210: 7661 7228 2d2d 7379 2d63 2d73 7572 6661  var(--sy-c-surfa
+00037220: 6365 293b 2d2d 7367 2d74 6f6f 6c74 6970  ce);--sg-tooltip
+00037230: 2d66 6f72 6567 726f 756e 643a 7661 7228  -foreground:var(
+00037240: 2d2d 7379 2d63 2d62 6163 6b67 726f 756e  --sy-c-backgroun
+00037250: 642d 636f 6e74 7261 7374 293b 2d2d 7367  d-contrast);--sg
+00037260: 2d74 6f6f 6c74 6970 2d62 6163 6b67 726f  -tooltip-backgro
+00037270: 756e 643a 7661 7228 2d2d 7379 2d63 2d62  und:var(--sy-c-b
+00037280: 6163 6b67 726f 756e 6429 3b2d 2d73 672d  ackground);--sg-
+00037290: 746f 6f6c 7469 702d 626f 7264 6572 3a76  tooltip-border:v
+000372a0: 6172 282d 2d67 7261 792d 3729 2023 3030  ar(--gray-7) #00
+000372b0: 3030 3b2d 2d73 672d 7468 756d 622d 626f  00;--sg-thumb-bo
+000372c0: 782d 7368 6164 6f77 2d63 6f6c 6f72 3a76  x-shadow-color:v
+000372d0: 6172 282d 2d67 7261 792d 6134 293b 2d2d  ar(--gray-a4);--
+000372e0: 7367 2d74 6875 6d62 2d68 6f76 6572 2d62  sg-thumb-hover-b
+000372f0: 6f72 6465 723a 7661 7228 2d2d 6163 6365  order:var(--acce
+00037300: 6e74 2d61 3929 3b2d 2d73 672d 7363 7269  nt-a9);--sg-scri
+00037310: 7074 2d6f 7574 3a76 6172 282d 2d73 792d  pt-out:var(--sy-
+00037320: 632d 6c69 6768 7429 3b2d 2d73 672d 7363  c-light);--sg-sc
+00037330: 7269 7074 2d70 7265 3a76 6172 282d 2d73  ript-pre:var(--s
+00037340: 796e 7461 782d 7072 652d 6267 293b 2d2d  yntax-pre-bg);--
+00037350: 7367 2d70 7974 622d 666f 7265 6772 6f75  sg-pytb-foregrou
+00037360: 6e64 3a76 6172 282d 2d73 796e 7461 782d  nd:var(--syntax-
+00037370: 7465 7874 293b 2d2d 7367 2d70 7974 622d  text);--sg-pytb-
+00037380: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
+00037390: 2d72 6564 2d61 3229 3b2d 2d73 672d 7079  -red-a2);--sg-py
+000373a0: 7462 2d62 6f72 6465 722d 636f 6c6f 723a  tb-border-color:
+000373b0: 7661 7228 2d2d 7265 642d 6138 293b 2d2d  var(--red-a8);--
+000373c0: 7367 2d64 6f77 6e6c 6f61 642d 612d 6261  sg-download-a-ba
+000373d0: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
+000373e0: 6172 282d 2d61 6363 656e 742d 6133 293b  ar(--accent-a3);
+000373f0: 2d2d 7367 2d64 6f77 6e6c 6f61 642d 612d  --sg-download-a-
+00037400: 6261 636b 6772 6f75 6e64 2d69 6d61 6765  background-image
+00037410: 3a6e 6f6e 653b 2d2d 7367 2d64 6f77 6e6c  :none;--sg-downl
+00037420: 6f61 642d 612d 626f 7264 6572 2d63 6f6c  oad-a-border-col
+00037430: 6f72 3a31 7078 2073 6f6c 6964 2076 6172  or:1px solid var
+00037440: 282d 2d61 6363 656e 742d 6133 293b 2d2d  (--accent-a3);--
+00037450: 7367 2d64 6f77 6e6c 6f61 642d 612d 636f  sg-download-a-co
+00037460: 6c6f 723a 7661 7228 2d2d 6163 6365 6e74  lor:var(--accent
+00037470: 2d61 3131 293b 2d2d 7367 2d64 6f77 6e6c  -a11);--sg-downl
+00037480: 6f61 642d 612d 686f 7665 722d 6261 636b  oad-a-hover-back
+00037490: 6772 6f75 6e64 2d63 6f6c 6f72 3a76 6172  ground-color:var
+000374a0: 282d 2d61 6363 656e 742d 6134 293b 2d2d  (--accent-a4);--
+000374b0: 7367 2d64 6f77 6e6c 6f61 642d 612d 686f  sg-download-a-ho
+000374c0: 7665 722d 626f 782d 7368 6164 6f77 2d31  ver-box-shadow-1
+000374d0: 3a23 3030 3030 3b2d 2d73 672d 646f 776e  :#0000;--sg-down
+000374e0: 6c6f 6164 2d61 2d68 6f76 6572 2d62 6f78  load-a-hover-box
+000374f0: 2d73 6861 646f 772d 323a 2330 3030 307d  -shadow-2:#0000}
+00037500: 2e79 7565 202e 7370 6878 2d67 6c72 2d64  .yue .sphx-glr-d
+00037510: 6f77 6e6c 6f61 6420 612c 2e79 7565 202e  ownload a,.yue .
+00037520: 7370 6878 2d67 6c72 2d64 6f77 6e6c 6f61  sphx-glr-downloa
+00037530: 6420 613a 686f 7665 722c 2e79 7565 202e  d a:hover,.yue .
+00037540: 7370 6878 2d67 6c72 2d74 6875 6d62 6e61  sphx-glr-thumbna
+00037550: 696c 7320 617b 626f 7264 6572 2d62 6f74  ils a{border-bot
+00037560: 746f 6d3a 307d 2e79 7565 2070 2e73 7068  tom:0}.yue p.sph
+00037570: 782d 676c 722d 7369 676e 6174 7572 6520  x-glr-signature 
+00037580: 617b 626f 7264 6572 2d72 6164 6975 733a  a{border-radius:
+00037590: 303b 626f 7264 6572 2d62 6f74 746f 6d3a  0;border-bottom:
+000375a0: 303b 7465 7874 2d64 6563 6f72 6174 696f  0;text-decoratio
+000375b0: 6e3a 756e 6465 726c 696e 657d 2e79 7565  n:underline}.yue
+000375c0: 2070 2e73 7068 782d 676c 722d 7369 676e   p.sphx-glr-sign
+000375d0: 6174 7572 6520 613a 686f 7665 727b 636f  ature a:hover{co
+000375e0: 6c6f 723a 7661 7228 2d2d 7379 2d63 2d6c  lor:var(--sy-c-l
+000375f0: 696e 6b2d 686f 7665 7229 7d2e 7975 6520  ink-hover)}.yue 
+00037600: 2e73 7068 782d 676c 722d 666f 6f74 6572  .sphx-glr-footer
+00037610: 2069 6d67 7b64 6973 706c 6179 3a69 6e6c   img{display:inl
+00037620: 696e 653b 6d61 7267 696e 3a30 7d68 746d  ine;margin:0}htm
+00037630: 6c2e 6461 726b 2c68 746d 6c2e 6c69 6768  l.dark,html.ligh
+00037640: 747b 2d2d 646f 6373 6561 7263 682d 7072  t{--docsearch-pr
+00037650: 696d 6172 792d 636f 6c6f 723a 7661 7228  imary-color:var(
+00037660: 2d2d 6163 6365 6e74 2d39 293b 2d2d 646f  --accent-9);--do
+00037670: 6373 6561 7263 682d 7465 7874 2d63 6f6c  csearch-text-col
+00037680: 6f72 3a76 6172 282d 2d73 792d 632d 7465  or:var(--sy-c-te
+00037690: 7874 293b 2d2d 646f 6373 6561 7263 682d  xt);--docsearch-
+000376a0: 6d6f 6461 6c2d 6261 636b 6772 6f75 6e64  modal-background
+000376b0: 3a76 6172 282d 2d73 792d 632d 6261 636b  :var(--sy-c-back
+000376c0: 6772 6f75 6e64 293b 2d2d 646f 6373 6561  ground);--docsea
+000376d0: 7263 682d 666f 6f74 6572 2d62 6163 6b67  rch-footer-backg
+000376e0: 726f 756e 643a 7661 7228 2d2d 7379 2d63  round:var(--sy-c
+000376f0: 2d73 7572 6661 6365 293b 2d2d 646f 6373  -surface);--docs
+00037700: 6561 7263 682d 7365 6172 6368 626f 782d  earch-searchbox-
+00037710: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
+00037720: 2d73 792d 632d 7375 7266 6163 6529 3b2d  -sy-c-surface);-
+00037730: 2d64 6f63 7365 6172 6368 2d73 6561 7263  -docsearch-searc
+00037740: 6862 6f78 2d66 6f63 7573 2d62 6163 6b67  hbox-focus-backg
+00037750: 726f 756e 643a 7661 7228 2d2d 7379 2d63  round:var(--sy-c
+00037760: 2d62 6163 6b67 726f 756e 6429 3b2d 2d64  -background);--d
+00037770: 6f63 7365 6172 6368 2d6d 7574 6564 2d63  ocsearch-muted-c
+00037780: 6f6c 6f72 3a76 6172 282d 2d73 792d 632d  olor:var(--sy-c-
+00037790: 6c69 6768 7429 3b2d 2d64 6f63 7365 6172  light);--docsear
+000377a0: 6368 2d68 6974 2d63 6f6c 6f72 3a76 6172  ch-hit-color:var
+000377b0: 282d 2d73 792d 632d 7465 7874 293b 2d2d  (--sy-c-text);--
+000377c0: 646f 6373 6561 7263 682d 6869 742d 6261  docsearch-hit-ba
+000377d0: 636b 6772 6f75 6e64 3a76 6172 282d 2d73  ckground:var(--s
+000377e0: 792d 632d 7375 7266 6163 6529 3b2d 2d64  y-c-surface);--d
+000377f0: 6f63 7365 6172 6368 2d68 6974 2d61 6374  ocsearch-hit-act
+00037800: 6976 652d 636f 6c6f 723a 7661 7228 2d2d  ive-color:var(--
+00037810: 6163 6365 6e74 2d39 2d63 6f6e 7472 6173  accent-9-contras
+00037820: 7429 3b2d 2d64 6f63 7365 6172 6368 2d68  t);--docsearch-h
+00037830: 6974 2d73 6861 646f 773a 696e 7365 7420  it-shadow:inset 
+00037840: 3020 3020 3170 7820 3020 7661 7228 2d2d  0 0 1px 0 var(--
+00037850: 6772 6179 2d61 3131 293b 2d2d 646f 6373  gray-a11);--docs
+00037860: 6561 7263 682d 636f 6e74 6169 6e65 722d  earch-container-
+00037870: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
+00037880: 2d73 792d 632d 6f76 6572 6c61 7929 7d68  -sy-c-overlay)}h
+00037890: 746d 6c2e 6c69 6768 747b 2d2d 646f 6373  tml.light{--docs
+000378a0: 6561 7263 682d 6b65 792d 6772 6164 6965  earch-key-gradie
+000378b0: 6e74 3a6c 696e 6561 722d 6772 6164 6965  nt:linear-gradie
+000378c0: 6e74 282d 3232 3564 6567 2c23 6536 6536  nt(-225deg,#e6e6
+000378d0: 6536 2c23 6638 6638 6638 293b 2d2d 646f  e6,#f8f8f8);--do
+000378e0: 6373 6561 7263 682d 6b65 792d 7368 6164  csearch-key-shad
+000378f0: 6f77 3a69 6e73 6574 2030 202d 3270 7820  ow:inset 0 -2px 
+00037900: 2364 6264 6264 622c 696e 7365 7420 3020  #dbdbdb,inset 0 
+00037910: 3020 3170 7820 3170 7820 2366 6666 2c30  0 1px 1px #fff,0
+00037920: 2031 7078 2032 7078 2031 7078 2023 3530   1px 2px 1px #50
+00037930: 3530 3530 3636 7d68 746d 6c2e 6461 726b  505066}html.dark
+00037940: 7b2d 2d64 6f63 7365 6172 6368 2d6b 6579  {--docsearch-key
+00037950: 2d67 7261 6469 656e 743a 6c69 6e65 6172  -gradient:linear
+00037960: 2d67 7261 6469 656e 7428 2d32 3235 6465  -gradient(-225de
+00037970: 672c 2333 3533 3433 342c 2331 3431 3431  g,#353434,#14141
+00037980: 3429 3b2d 2d64 6f63 7365 6172 6368 2d6b  4);--docsearch-k
+00037990: 6579 2d73 6861 646f 773a 696e 7365 7420  ey-shadow:inset 
+000379a0: 3020 2d32 7078 2023 3337 3337 3337 2c69  0 -2px #373737,i
+000379b0: 6e73 6574 2030 2030 2031 7078 2031 7078  nset 0 0 1px 1px
+000379c0: 2023 3232 322c 3020 3170 7820 3270 7820   #222,0 1px 2px 
+000379d0: 3170 7820 2330 3030 3b2d 2d64 6f63 7365  1px #000;--docse
+000379e0: 6172 6368 2d66 6f6f 7465 722d 7368 6164  arch-footer-shad
+000379f0: 6f77 3a30 202d 3170 7820 3020 3020 2333  ow:0 -1px 0 0 #3
+00037a00: 3733 3733 372c 3020 2d33 7078 2036 7078  73737,0 -3px 6px
+00037a10: 2030 2023 3134 3134 3134 3b2d 2d64 6f63   0 #141414;--doc
+00037a20: 7365 6172 6368 2d6d 6f64 616c 2d73 6861  search-modal-sha
+00037a30: 646f 773a 696e 7365 7420 3170 7820 3170  dow:inset 1px 1p
+00037a40: 7820 3020 3020 2333 3733 3733 372c 3020  x 0 0 #373737,0 
+00037a50: 3370 7820 3870 7820 3020 2331 3431 3431  3px 8px 0 #14141
+00037a60: 347d 2364 6f63 7365 6172 6368 202e 446f  4}#docsearch .Do
+00037a70: 6353 6561 7263 682d 4275 7474 6f6e 7b62  cSearch-Button{b
+00037a80: 6f72 6465 722d 7261 6469 7573 3a36 7078  order-radius:6px
+00037a90: 7d23 646f 6373 6561 7263 6820 2e44 6f63  }#docsearch .Doc
+00037aa0: 5365 6172 6368 2d42 7574 746f 6e2d 4b65  Search-Button-Ke
+00037ab0: 792c 2364 6f63 7365 6172 6368 202e 446f  y,#docsearch .Do
+00037ac0: 6353 6561 7263 682d 4275 7474 6f6e 2d50  cSearch-Button-P
+00037ad0: 6c61 6365 686f 6c64 6572 7b66 6f6e 742d  laceholder{font-
+00037ae0: 7369 7a65 3a2e 3832 3572 656d 7d23 646f  size:.825rem}#do
+00037af0: 6373 6561 7263 6820 2e44 6f63 5365 6172  csearch .DocSear
+00037b00: 6368 2d42 7574 746f 6e2d 4b65 7973 2c23  ch-Button-Keys,#
+00037b10: 646f 6373 6561 7263 6820 2e44 6f63 5365  docsearch .DocSe
+00037b20: 6172 6368 2d42 7574 746f 6e2d 506c 6163  arch-Button-Plac
+00037b30: 6568 6f6c 6465 727b 6469 7370 6c61 793a  eholder{display:
+00037b40: 666c 6578 2169 6d70 6f72 7461 6e74 7d23  flex!important}#
+00037b50: 646f 6373 6561 7263 6820 2e44 6f63 5365  docsearch .DocSe
+00037b60: 6172 6368 2d53 6561 7263 682d 4963 6f6e  arch-Search-Icon
+00037b70: 7b77 6964 7468 3a2e 3837 3572 656d 2169  {width:.875rem!i
+00037b80: 6d70 6f72 7461 6e74 3b68 6569 6768 743a  mportant;height:
+00037b90: 2e38 3735 7265 6d21 696d 706f 7274 616e  .875rem!importan
+00037ba0: 747d 406d 6564 6961 2028 6d61 782d 7769  t}@media (max-wi
+00037bb0: 6474 683a 3736 3770 7829 7b23 646f 6373  dth:767px){#docs
+00037bc0: 6561 7263 687b 706f 7369 7469 6f6e 3a61  earch{position:a
+00037bd0: 6273 6f6c 7574 653b 746f 703a 3172 656d  bsolute;top:1rem
+00037be0: 3b6c 6566 743a 312e 3872 656d 3b72 6967  ;left:1.8rem;rig
+00037bf0: 6874 3a31 2e38 7265 6d7d 2364 6f63 7365  ht:1.8rem}#docse
+00037c00: 6172 6368 202e 446f 6353 6561 7263 682d  arch .DocSearch-
+00037c10: 4275 7474 6f6e 7b6d 6172 6769 6e2d 6c65  Button{margin-le
+00037c20: 6674 3a30 3b77 6964 7468 3a31 3030 257d  ft:0;width:100%}
+00037c30: 7d64 6c2e 7371 6c61 2064 747b 636f 6c6f  }dl.sqla dt{colo
+00037c40: 723a 7661 7228 2d2d 7369 672d 6e61 6d65  r:var(--sig-name
+00037c50: 293b 6d61 7267 696e 2d62 6f74 746f 6d3a  );margin-bottom:
+00037c60: 2e35 7265 6d7d 646c 2e73 716c 6120 6474  .5rem}dl.sqla dt
+00037c70: 3e65 6d7b 666f 6e74 2d77 6569 6768 743a  >em{font-weight:
+00037c80: 3430 303b 666f 6e74 2d73 7479 6c65 3a6e  400;font-style:n
+00037c90: 6f72 6d61 6c3b 636f 6c6f 723a 7661 7228  ormal;color:var(
+00037ca0: 2d2d 7369 672d 7061 7261 6d29 7d64 6c2e  --sig-param)}dl.
+00037cb0: 7371 6c61 2064 643e 702e 7275 6272 6963  sqla dd>p.rubric
+00037cc0: 7b6d 6172 6769 6e2d 746f 703a 312e 3572  {margin-top:1.5r
+00037cd0: 656d 3b74 6578 742d 7472 616e 7366 6f72  em;text-transfor
+00037ce0: 6d3a 7570 7065 7263 6173 653b 666f 6e74  m:uppercase;font
+00037cf0: 2d73 697a 653a 2e37 3672 656d 7d64 6c2e  -size:.76rem}dl.
+00037d00: 7371 6c61 2064 643e 702e 7275 6272 6963  sqla dd>p.rubric
+00037d10: 2b2e 7461 626c 652d 7772 6170 7065 727b  +.table-wrapper{
+00037d20: 6d61 7267 696e 2d74 6f70 3a2e 3735 7265  margin-top:.75re
+00037d30: 6d3b 626f 7264 6572 2d6c 6566 743a 303b  m;border-left:0;
+00037d40: 626f 7264 6572 2d72 6967 6874 3a30 3b62  border-right:0;b
+00037d50: 6f72 6465 722d 7261 6469 7573 3a30 7d64  order-radius:0}d
+00037d60: 6c2e 7371 6c61 2070 2e72 7562 7269 632b  l.sqla p.rubric+
+00037d70: 2e74 6162 6c65 2d77 7261 7070 6572 2074  .table-wrapper t
+00037d80: 642c 646c 2e73 716c 6120 702e 7275 6272  d,dl.sqla p.rubr
+00037d90: 6963 2b2e 7461 626c 652d 7772 6170 7065  ic+.table-wrappe
+00037da0: 7220 7468 7b62 6f72 6465 722d 6c65 6674  r th{border-left
+00037db0: 3a30 3b62 6f72 6465 722d 7269 6768 743a  :0;border-right:
+00037dc0: 303b 6261 636b 6772 6f75 6e64 2d63 6f6c  0;background-col
+00037dd0: 6f72 3a69 6e69 7469 616c 7d64 6c2e 7371  or:initial}dl.sq
+00037de0: 6c61 2070 2e72 7562 7269 632b 2e74 6162  la p.rubric+.tab
+00037df0: 6c65 2d77 7261 7070 6572 2074 643e 707b  le-wrapper td>p{
+00037e00: 6d61 7267 696e 3a30 7d64 6c2e 7371 6c61  margin:0}dl.sqla
+00037e10: 2070 2e72 7562 7269 632b 2e74 6162 6c65   p.rubric+.table
+00037e20: 2d77 7261 7070 6572 2074 722e 726f 772d  -wrapper tr.row-
+00037e30: 6f64 647b 6261 636b 6772 6f75 6e64 2d63  odd{background-c
+00037e40: 6f6c 6f72 3a69 6e69 7469 616c 7d64 6c2e  olor:initial}dl.
+00037e50: 7371 6c61 2070 2e72 7562 7269 632b 2e74  sqla p.rubric+.t
+00037e60: 6162 6c65 2d77 7261 7070 6572 2074 722e  able-wrapper tr.
+00037e70: 726f 772d 6576 656e 7b62 6163 6b67 726f  row-even{backgro
+00037e80: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
+00037e90: 7975 652d 632d 726f 772d 6261 636b 6772  yue-c-row-backgr
+00037ea0: 6f75 6e64 297d 2e79 7565 7b2d 2d78 722d  ound)}.yue{--xr-
+00037eb0: 666f 6e74 2d63 6f6c 6f72 303a 7661 7228  font-color0:var(
+00037ec0: 2d2d 7379 2d63 2d68 6561 6469 6e67 293b  --sy-c-heading);
+00037ed0: 2d2d 7872 2d66 6f6e 742d 636f 6c6f 7232  --xr-font-color2
+00037ee0: 3a76 6172 282d 2d73 792d 632d 7465 7874  :var(--sy-c-text
+00037ef0: 293b 2d2d 7872 2d66 6f6e 742d 636f 6c6f  );--xr-font-colo
+00037f00: 7233 3a76 6172 282d 2d73 792d 632d 6c69  r3:var(--sy-c-li
+00037f10: 6768 7429 3b2d 2d78 722d 626f 7264 6572  ght);--xr-border
+00037f20: 2d63 6f6c 6f72 3a76 6172 282d 2d73 792d  -color:var(--sy-
+00037f30: 632d 626f 7264 6572 293b 2d2d 7872 2d64  c-border);--xr-d
+00037f40: 6973 6162 6c65 642d 636f 6c6f 723a 7661  isabled-color:va
+00037f50: 7228 2d2d 6772 6179 2d61 3629 3b2d 2d78  r(--gray-a6);--x
+00037f60: 722d 6261 636b 6772 6f75 6e64 2d63 6f6c  r-background-col
+00037f70: 6f72 3a76 6172 282d 2d73 792d 632d 6261  or:var(--sy-c-ba
+00037f80: 636b 6772 6f75 6e64 293b 2d2d 7872 2d62  ckground);--xr-b
+00037f90: 6163 6b67 726f 756e 642d 636f 6c6f 722d  ackground-color-
+00037fa0: 726f 772d 6576 656e 3a76 6172 282d 2d73  row-even:var(--s
+00037fb0: 792d 632d 6261 636b 6772 6f75 6e64 293b  y-c-background);
+00037fc0: 2d2d 7872 2d62 6163 6b67 726f 756e 642d  --xr-background-
+00037fd0: 636f 6c6f 722d 726f 772d 6f64 643a 7661  color-row-odd:va
+00037fe0: 7228 2d2d 6772 6179 2d32 297d 2e79 7565  r(--gray-2)}.yue
+00037ff0: 202e 7872 2d61 7272 6179 2d64 6174 6120   .xr-array-data 
+00038000: 7072 657b 6d61 7267 696e 3a30 7d2e 7975  pre{margin:0}.yu
+00038010: 6520 6465 7461 696c 732e 746f 6767 6c65  e details.toggle
+00038020: 2d64 6574 6169 6c73 2073 756d 6d61 7279  -details summary
+00038030: 7b62 6f72 6465 722d 6c65 6674 2d63 6f6c  {border-left-col
+00038040: 6f72 3a76 6172 282d 2d61 6363 656e 742d  or:var(--accent-
+00038050: 6139 297d 406d 6564 6961 206e 6f74 2061  a9)}@media not a
+00038060: 6c6c 2061 6e64 2028 6d69 6e2d 7769 6474  ll and (min-widt
+00038070: 683a 3634 3070 7829 7b2e 6d61 782d 736d  h:640px){.max-sm
+00038080: 5c3a 6d61 782d 772d 6675 6c6c 7b6d 6178  \:max-w-full{max
+00038090: 2d77 6964 7468 3a31 3030 257d 7d40 6d65  -width:100%}}@me
+000380a0: 6469 6120 286d 696e 2d77 6964 7468 3a37  dia (min-width:7
+000380b0: 3638 7078 297b 2e6d 645c 3a73 7469 636b  68px){.md\:stick
+000380c0: 797b 706f 7369 7469 6f6e 3a73 7469 636b  y{position:stick
+000380d0: 797d 2e6d 645c 3a69 6e6c 696e 657b 6469  y}.md\:inline{di
+000380e0: 7370 6c61 793a 696e 6c69 6e65 7d2e 6d64  splay:inline}.md
+000380f0: 5c3a 666c 6578 7b64 6973 706c 6179 3a66  \:flex{display:f
+00038100: 6c65 787d 2e6d 645c 3a68 6964 6465 6e7b  lex}.md\:hidden{
+00038110: 6469 7370 6c61 793a 6e6f 6e65 7d2e 6d64  display:none}.md
+00038120: 5c3a 772d 3732 7b77 6964 7468 3a31 3872  \:w-72{width:18r
+00038130: 656d 7d2e 6d64 5c3a 7368 7269 6e6b 2d30  em}.md\:shrink-0
+00038140: 7b66 6c65 782d 7368 7269 6e6b 3a30 7d7d  {flex-shrink:0}}
+00038150: 406d 6564 6961 2028 6d69 6e2d 7769 6474  @media (min-widt
+00038160: 683a 3132 3830 7078 297b 2e78 6c5c 3a73  h:1280px){.xl\:s
+00038170: 7469 636b 797b 706f 7369 7469 6f6e 3a73  ticky{position:s
+00038180: 7469 636b 797d 2e78 6c5c 3a74 6f70 2d31  ticky}.xl\:top-1
+00038190: 367b 746f 703a 3472 656d 7d2e 786c 5c3a  6{top:4rem}.xl\:
+000381a0: 6869 6464 656e 7b64 6973 706c 6179 3a6e  hidden{display:n
+000381b0: 6f6e 657d 2e78 6c5c 3a70 782d 3132 7b70  one}.xl\:px-12{p
+000381c0: 6164 6469 6e67 2d6c 6566 743a 3372 656d  adding-left:3rem
+000381d0: 3b70 6164 6469 6e67 2d72 6967 6874 3a33  ;padding-right:3
+000381e0: 7265 6d7d 2e78 6c5c 3a70 6c2d 307b 7061  rem}.xl\:pl-0{pa
+000381f0: 6464 696e 672d 6c65 6674 3a30 7d7d 406d  dding-left:0}}@m
+00038200: 6564 6961 2070 7269 6e74 7b2e 7072 696e  edia print{.prin
+00038210: 745c 3a68 6964 6465 6e7b 6469 7370 6c61  t\:hidden{displa
+00038220: 793a 6e6f 6e65 7d2e 7072 696e 745c 3a70  y:none}.print\:p
+00038230: 742d 367b 7061 6464 696e 672d 746f 703a  t-6{padding-top:
+00038240: 312e 3572 656d 7d7d                      1.5rem}}
```

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/static/shibuya.js` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/static/shibuya.js`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya/theme/shibuya/theme.conf` & `shibuya-2024.5.14/src/shibuya/theme/shibuya/theme.conf`

 * *Files identical despite different names*

### Comparing `shibuya-2024.5.10/src/shibuya.egg-info/PKG-INFO` & `shibuya-2024.5.14/src/shibuya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shibuya
-Version: 2024.5.10
+Version: 2024.5.14
 Summary: A clean, responsive, and customizable Sphinx documentation theme with light/dark mode.
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/lepture/shibuya
 Project-URL: Documentation, https://shibuya.lepture.com/
 Project-URL: Sponsors, https://github.com/sponsors/lepture
 Classifier: Framework :: Sphinx
```

### Comparing `shibuya-2024.5.10/src/shibuya.egg-info/SOURCES.txt` & `shibuya-2024.5.14/src/shibuya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

