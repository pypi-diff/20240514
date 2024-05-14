# Comparing `tmp/betty-0.3.4.tar.gz` & `tmp/betty-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betty-0.3.4.tar", last modified: Sun May  5 11:20:20 2024, max compression
+gzip compressed data, was "betty-0.3.5.tar", last modified: Tue May 14 21:11:39 2024, max compression
```

## Comparing `betty-0.3.4.tar` & `betty-0.3.5.tar`

### file list

```diff
@@ -1,307 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.591119 betty-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-05 11:19:09.000000 betty-0.3.4/.browserslistrc
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-05-05 11:19:09.000000 betty-0.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 11:19:09.000000 betty-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43621 2024-05-05 11:20:20.591119 betty-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-05 11:19:09.000000 betty-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.551119 betty-0.3.4/betty/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 11:19:09.000000 betty-0.3.4/betty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_npm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.535119 betty-0.3.4/betty/_package/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/_package/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/_package/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/hooks/hook-betty.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_resizeimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-05 11:19:09.000000 betty-0.3.4/betty/about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/app/
--rw-r--r--   0 runner    (1001) docker     (127)    19649 2024-05-05 11:19:09.000000 betty-0.3.4/betty/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/app/extension/
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-05 11:19:09.000000 betty-0.3.4/betty/app/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-05 11:19:09.000000 betty-0.3.4/betty/app/extension/requirement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 11:19:20.000000 betty-0.3.4/betty/assets/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)    21029 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/betty.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.535119 betty-0.3.4/betty/assets/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/de-DE/
--rw-r--r--   0 runner    (1001) docker     (127)    36131 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/de-DE/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/fr-FR/
--rw-r--r--   0 runner    (1001) docker     (127)    25486 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/fr-FR/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/nl-NL/
--rw-r--r--   0 runner    (1001) docker     (127)    36020 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/nl-NL/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/uk/
--rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/uk/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.535119 betty-0.3.4/betty/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/localized/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/assets/public/static/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)   152126 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty.ico
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/robots.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/base.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/assets/templates/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/entity/page-list.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/entity/page.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/head.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/linked-data.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/scripts.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/sitemap-index.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/sitemap.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/stylesheets.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-05 11:19:09.000000 betty-0.3.4/betty/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-05 11:19:09.000000 betty-0.3.4/betty/classtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-05 11:19:09.000000 betty-0.3.4/betty/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-05 11:19:09.000000 betty-0.3.4/betty/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-05 11:19:09.000000 betty-0.3.4/betty/contextlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-05 11:19:09.000000 betty-0.3.4/betty/deriver.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 11:19:09.000000 betty-0.3.4/betty/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-05 11:19:09.000000 betty-0.3.4/betty/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-05 11:19:09.000000 betty-0.3.4/betty/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/extension/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/cotton_candy/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/cotton_candy/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/search-index.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/assets/public/static/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/static/betty.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/static/search-configuration.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/base.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.571119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-extended--application--pdf.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-extended--image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-extended.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-summary--application--pdf.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-summary--image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-summary.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/footer.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.571119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/macro/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/macro/citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/map.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/media.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/permalink.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/references.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.571119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/results.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/section-notes.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/show-countable.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/show.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/timeline.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/tree.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/cotton_candy/webpack/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/accessibility.scss
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/citation.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/entity.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/file.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/file.ts
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/main.scss
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/main.ts
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/meta.scss
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/overlay.scss
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/page.scss
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/permalink.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/person.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/search.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/search.ts
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/show.scss
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/show.ts
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/demo/
--rw-r--r--   0 runner    (1001) docker     (127)    17350 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/deriver/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/deriver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/gramps/
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/gramps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/gramps/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/gramps/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/http_api_doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/http_api_doc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/http_api_doc/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/http_api_doc/assets/public/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/http_api_doc/assets/public/static/api/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/assets/public/static/api/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/http_api_doc/webpack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/webpack/main.ts
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/webpack/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/maps/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/maps/webpack/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/main.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/maps.js
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/nginx/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/assets/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/assets/content_negotiation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/assets/nginx.conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/privatizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/privatizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/trees/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/trees/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/trees/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/trees/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/assets/public/localized/people.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/trees/webpack/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/main.ts
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/trees.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.543119 betty-0.3.4/betty/extension/webpack/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/assets/templates/webpack-entry-loader.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/jinja2/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/webpack/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/webpack/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/webpack/webpack.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/wikipedia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.543119 betty-0.3.4/betty/extension/wikipedia/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/wikipedia/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/wikipedia/assets/templates/wikipedia.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-05 11:19:09.000000 betty-0.3.4/betty/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-05 11:19:09.000000 betty-0.3.4/betty/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-05 11:19:09.000000 betty-0.3.4/betty/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/gramps/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gramps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gramps/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gramps/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    33182 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-05 11:19:09.000000 betty-0.3.4/betty/hashid.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-05 11:19:09.000000 betty-0.3.4/betty/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-05 11:19:09.000000 betty-0.3.4/betty/importlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-05 11:19:09.000000 betty-0.3.4/betty/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17552 2024-05-05 11:19:09.000000 betty-0.3.4/betty/jinja2/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-05 11:19:09.000000 betty-0.3.4/betty/jinja2/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 11:19:09.000000 betty-0.3.4/betty/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/json/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 11:19:09.000000 betty-0.3.4/betty/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-05 11:19:09.000000 betty-0.3.4/betty/json/linked_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-05 11:19:09.000000 betty-0.3.4/betty/json/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-05 11:19:09.000000 betty-0.3.4/betty/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-05-05 11:19:09.000000 betty-0.3.4/betty/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-05 11:19:09.000000 betty-0.3.4/betty/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-05 11:19:09.000000 betty-0.3.4/betty/media_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/model/
--rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-05-05 11:19:09.000000 betty-0.3.4/betty/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58905 2024-05-05 11:19:09.000000 betty-0.3.4/betty/model/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-05 11:19:09.000000 betty-0.3.4/betty/model/event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-05 11:19:09.000000 betty-0.3.4/betty/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-05 11:19:09.000000 betty-0.3.4/betty/os.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-05 11:19:09.000000 betty-0.3.4/betty/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-05 11:19:09.000000 betty-0.3.4/betty/privatizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-05 11:19:09.000000 betty-0.3.4/betty/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-05 11:19:09.000000 betty-0.3.4/betty/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-05 11:19:09.000000 betty-0.3.4/betty/requirement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty/serde/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 11:19:09.000000 betty-0.3.4/betty/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty/sphinx/extension/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-05 11:19:09.000000 betty-0.3.4/betty/sphinx/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-05 11:19:09.000000 betty-0.3.4/betty/sphinx/extension/replacements.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-05 11:19:09.000000 betty-0.3.4/betty/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 11:19:09.000000 betty-0.3.4/betty/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-05 11:19:09.000000 betty-0.3.4/betty/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-05 11:19:09.000000 betty-0.3.4/betty/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17927 2024-05-05 11:19:09.000000 betty-0.3.4/betty/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43621 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-05 11:19:09.000000 betty-0.3.4/documentation/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-05 11:19:09.000000 betty-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 11:20:20.591119 betty-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-05 11:19:09.000000 betty-0.3.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 11:19:09.000000 betty-0.3.4/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.633154 betty-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 21:10:24.000000 betty-0.3.5/.browserslistrc
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-05-14 21:10:24.000000 betty-0.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 21:10:24.000000 betty-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43515 2024-05-14 21:11:39.633154 betty-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-14 21:10:24.000000 betty-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-14 21:10:24.000000 betty-0.3.5/betty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_npm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/_package/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/_package/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_package/pyinstaller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/_package/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_package/pyinstaller/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_package/pyinstaller/hooks/hook-betty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_package/pyinstaller/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-14 21:10:24.000000 betty-0.3.5/betty/_resizeimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-14 21:10:24.000000 betty-0.3.5/betty/about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    19649 2024-05-14 21:10:24.000000 betty-0.3.5/betty/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/app/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-05-14 21:10:24.000000 betty-0.3.5/betty/app/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-14 21:10:24.000000 betty-0.3.5/betty/app/extension/requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 21:10:30.000000 betty-0.3.5/betty/assets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/betty.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.581154 betty-0.3.5/betty/assets/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/assets/locale/de-DE/
+-rw-r--r--   0 runner    (1001) docker     (127)    36613 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/locale/de-DE/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.597154 betty-0.3.5/betty/assets/locale/fr-FR/
+-rw-r--r--   0 runner    (1001) docker     (127)    25968 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/locale/fr-FR/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/assets/locale/nl-NL/
+-rw-r--r--   0 runner    (1001) docker     (127)    36930 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/locale/nl-NL/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/assets/locale/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/locale/uk/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.581154 betty-0.3.5/betty/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/localized/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/assets/public/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/static/betty-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/static/betty-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/static/betty-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/static/betty-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)   152126 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/static/betty.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/static/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/public/static/robots.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/base.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/assets/templates/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/entity/page-list.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/entity/page.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/head.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/linked-data.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/scripts.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/sitemap-index.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/sitemap.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-14 21:10:24.000000 betty-0.3.5/betty/assets/templates/stylesheets.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-14 21:10:24.000000 betty-0.3.5/betty/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-14 21:10:24.000000 betty-0.3.5/betty/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-14 21:10:24.000000 betty-0.3.5/betty/cache/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-14 21:10:24.000000 betty-0.3.5/betty/cache/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-14 21:10:24.000000 betty-0.3.5/betty/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-14 21:10:24.000000 betty-0.3.5/betty/classtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-14 21:10:24.000000 betty-0.3.5/betty/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-14 21:10:24.000000 betty-0.3.5/betty/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23178 2024-05-14 21:10:24.000000 betty-0.3.5/betty/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-14 21:10:24.000000 betty-0.3.5/betty/contextlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-14 21:10:24.000000 betty-0.3.5/betty/deriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-14 21:10:24.000000 betty-0.3.5/betty/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-14 21:10:24.000000 betty-0.3.5/betty/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-14 21:10:24.000000 betty-0.3.5/betty/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.601154 betty-0.3.5/betty/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.605154 betty-0.3.5/betty/extension/cotton_candy/
+-rw-r--r--   0 runner    (1001) docker     (127)    15495 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/cotton_candy/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/cotton_candy/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.605154 betty-0.3.5/betty/extension/cotton_candy/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/public/localized/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/public/localized/search-index.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.605154 betty-0.3.5/betty/extension/cotton_candy/assets/public/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/public/static/betty.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/public/static/search-configuration.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.609154 betty-0.3.5/betty/extension/cotton_candy/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/base.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.613154 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/list--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/list--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page-list--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page-list--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page-list--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page-list--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/file-extended--application--pdf.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/file-extended--image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/file-extended.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/file-summary--application--pdf.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/file-summary--image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/file-summary.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/footer.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.613154 betty-0.3.5/betty/extension/cotton_candy/assets/templates/macro/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/macro/citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/map.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/media.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/permalink.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/references.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.613154 betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/result-person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/result-place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/result.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/results.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/section-notes.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/show-countable.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/show.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/timeline.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/assets/templates/tree.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/cotton_candy/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/accessibility.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/citation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/entity.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/file.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/file.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/main.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/meta.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/overlay.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/page.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/permalink.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/person.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/search.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/search.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/show.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/show.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/cotton_candy/webpack/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)    17350 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/deriver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/deriver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/gramps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/gramps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/gramps/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/gramps/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/http_api_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/http_api_doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/http_api_doc/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/http_api_doc/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/http_api_doc/assets/public/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/http_api_doc/assets/public/static/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/http_api_doc/assets/public/static/api/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/http_api_doc/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/http_api_doc/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/http_api_doc/webpack/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.617154 betty-0.3.5/betty/extension/maps/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/maps/webpack/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/maps/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/maps/webpack/maps.js
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/maps/webpack/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/nginx/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/assets/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/assets/content_negotiation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/assets/nginx.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/nginx/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/privatizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/privatizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/trees/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/trees/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/trees/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/trees/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/trees/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/trees/assets/public/localized/people.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/trees/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/trees/webpack/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/trees/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/trees/webpack/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/trees/webpack/trees.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/webpack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.585154 betty-0.3.5/betty/extension/webpack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/webpack/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/webpack/assets/templates/webpack-entry-loader.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/webpack/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/webpack/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/webpack/jinja2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/webpack/jinja2/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/webpack/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/webpack/webpack/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/webpack/webpack/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/wikipedia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.589154 betty-0.3.5/betty/extension/wikipedia/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/extension/wikipedia/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/wikipedia/assets/templates/wikipedia.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/wikipedia/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-14 21:10:24.000000 betty-0.3.5/betty/extension/wikipedia/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-14 21:10:24.000000 betty-0.3.5/betty/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-14 21:10:24.000000 betty-0.3.5/betty/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-14 21:10:24.000000 betty-0.3.5/betty/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.621154 betty-0.3.5/betty/gramps/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gramps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gramps/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37386 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gramps/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.625154 betty-0.3.5/betty/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33182 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-14 21:10:24.000000 betty-0.3.5/betty/gui/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-14 21:10:24.000000 betty-0.3.5/betty/hashid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-14 21:10:24.000000 betty-0.3.5/betty/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-14 21:10:24.000000 betty-0.3.5/betty/importlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.625154 betty-0.3.5/betty/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-14 21:10:24.000000 betty-0.3.5/betty/jinja2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17552 2024-05-14 21:10:24.000000 betty-0.3.5/betty/jinja2/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-14 21:10:24.000000 betty-0.3.5/betty/jinja2/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-14 21:10:24.000000 betty-0.3.5/betty/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.625154 betty-0.3.5/betty/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 21:10:24.000000 betty-0.3.5/betty/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-14 21:10:24.000000 betty-0.3.5/betty/json/linked_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-14 21:10:24.000000 betty-0.3.5/betty/json/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 21:10:24.000000 betty-0.3.5/betty/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39959 2024-05-14 21:10:24.000000 betty-0.3.5/betty/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-14 21:10:24.000000 betty-0.3.5/betty/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-14 21:10:24.000000 betty-0.3.5/betty/media_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.625154 betty-0.3.5/betty/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-05-14 21:10:24.000000 betty-0.3.5/betty/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61308 2024-05-14 21:10:24.000000 betty-0.3.5/betty/model/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-14 21:10:24.000000 betty-0.3.5/betty/model/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-14 21:10:24.000000 betty-0.3.5/betty/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-14 21:10:24.000000 betty-0.3.5/betty/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-14 21:10:24.000000 betty-0.3.5/betty/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-14 21:10:24.000000 betty-0.3.5/betty/privatizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-14 21:10:24.000000 betty-0.3.5/betty/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:10:24.000000 betty-0.3.5/betty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-14 21:10:24.000000 betty-0.3.5/betty/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-14 21:10:24.000000 betty-0.3.5/betty/requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.625154 betty-0.3.5/betty/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 21:10:24.000000 betty-0.3.5/betty/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-14 21:10:24.000000 betty-0.3.5/betty/serde/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-14 21:10:24.000000 betty-0.3.5/betty/serde/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-14 21:10:24.000000 betty-0.3.5/betty/serde/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16320 2024-05-14 21:10:24.000000 betty-0.3.5/betty/serde/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-14 21:10:24.000000 betty-0.3.5/betty/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.625154 betty-0.3.5/betty/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 21:10:24.000000 betty-0.3.5/betty/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.629154 betty-0.3.5/betty/sphinx/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 21:10:24.000000 betty-0.3.5/betty/sphinx/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 21:10:24.000000 betty-0.3.5/betty/sphinx/extension/replacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-14 21:10:24.000000 betty-0.3.5/betty/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-14 21:10:24.000000 betty-0.3.5/betty/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-14 21:10:24.000000 betty-0.3.5/betty/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-14 21:10:24.000000 betty-0.3.5/betty/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19526 2024-05-14 21:10:24.000000 betty-0.3.5/betty/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.629154 betty-0.3.5/betty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43515 2024-05-14 21:11:39.000000 betty-0.3.5/betty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-05-14 21:11:39.000000 betty-0.3.5/betty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:11:39.000000 betty-0.3.5/betty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-14 21:11:39.000000 betty-0.3.5/betty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-14 21:11:39.000000 betty-0.3.5/betty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 21:11:39.000000 betty-0.3.5/betty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.629154 betty-0.3.5/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-14 21:10:24.000000 betty-0.3.5/documentation/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-14 21:10:24.000000 betty-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:11:39.633154 betty-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 21:10:24.000000 betty-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:11:39.629154 betty-0.3.5/site/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-14 21:10:24.000000 betty-0.3.5/site/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 21:10:24.000000 betty-0.3.5/tsconfig.json
```

### Comparing `betty-0.3.4/LICENSE.txt` & `betty-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/PKG-INFO` & `betty-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.3.4
+Version: 0.3.5
 Summary: Betty helps you visualize and publish your family history by building interactive genealogy websites out of your Gramps and GECOM family trees
 Author-email: Bart Feenstra <bar@bartfeenstra.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,25 +695,23 @@
 Requires-Dist: html5lib~=1.1; extra == "test"
 Requires-Dist: lxml~=5.0; sys_platform != "win32" and extra == "test"
 Requires-Dist: pip-licenses>=4.3.0,~=4.3; extra == "test"
 Requires-Dist: pydocstyle>=6.3.0,~=6.3; extra == "test"
 Requires-Dist: pytest>=7.3.1,~=7.3; extra == "test"
 Requires-Dist: pytest-aioresponses>=0.2.0,~=0.2; extra == "test"
 Requires-Dist: pytest-asyncio>=0.23.4,~=0.23; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: pytest-mock>=3.10.0,~=3.10; extra == "test"
 Requires-Dist: pytest-qt>=4.2.0,~=4.2; extra == "test"
 Requires-Dist: pytest-xvfb>=3.0.0,~=3.0; extra == "test"
 Requires-Dist: types-aiofiles>=23.2.0.20240403,~=23.2; extra == "test"
 Requires-Dist: types-babel>=2.11.0.15,~=2.11; extra == "test"
 Requires-Dist: types-click>=7.1.8,~=7.1; extra == "test"
 Requires-Dist: types-html5lib>=1.1.11.20240228,~=1.1; extra == "test"
 Requires-Dist: types-jsonschema>=4.21.0.20240331,~=4.21; extra == "test"
 Requires-Dist: types-lxml>=2024.3.27; extra == "test"
-Requires-Dist: types-mock>=5.0.0.6,~=5.0; extra == "test"
 Requires-Dist: types-polib>=1.2.0.0,~=1.2; extra == "test"
 Requires-Dist: types-pyinstaller>=6.5.0.20240311,~=6.5; extra == "test"
 Requires-Dist: types-pyyaml>=6.0.6,~=6.0; extra == "test"
 Requires-Dist: types-requests>=2.29.0.0,~=2.29; extra == "test"
 Requires-Dist: types-setuptools~=69.0; extra == "test"
 Requires-Dist: virtualenv~=20.26; extra == "test"
 Requires-Dist: betty[pyinstaller]; extra == "test"
```

### Comparing `betty-0.3.4/README.md` & `betty-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/_npm.py` & `betty-0.3.5/betty/_npm.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/_package/pyinstaller/main.py` & `betty-0.3.5/betty/_package/pyinstaller/main.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/_patch.py` & `betty-0.3.5/betty/_patch.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/_resizeimage.py` & `betty-0.3.5/betty/_resizeimage.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/about.py` & `betty-0.3.5/betty/about.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/app/__init__.py` & `betty-0.3.5/betty/app/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/app/extension/__init__.py` & `betty-0.3.5/betty/app/extension/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 from betty.locale import Str
 
 if TYPE_CHECKING:
     from betty.app import App
 
 
 class ExtensionError(BaseException):
-    pass
+    pass  # pragma: no cover
 
 
 class ExtensionTypeError(ExtensionError, ValueError):
-    pass
+    pass  # pragma: no cover
 
 
 class ExtensionTypeImportError(ExtensionTypeError, ImportError):
     """
     Raised when an alleged extension type cannot be imported.
     """
 
@@ -203,15 +203,15 @@
 
     @classmethod
     def description(cls) -> Str:
         raise NotImplementedError(repr(cls))
 
 
 class Theme(UserFacingExtension):
-    pass
+    pass  # pragma: no cover
 
 
 @functools.singledispatch
 def get_extension_type(
     extension_type_definition: str | type[Extension] | Extension,
 ) -> type[Extension]:
     """
```

### Comparing `betty-0.3.4/betty/app/extension/requirement.py` & `betty-0.3.5/betty/app/extension/requirement.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/assets/betty.pot` & `betty-0.3.5/betty/assets/betty.pot`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Betty VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-30 22:56+0100\n"
+"POT-Creation-Date: 2024-05-08 17:53+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.14.0\n"
@@ -324,14 +324,17 @@
 
 msgid "Display the HTTP API documentation in a user-friendly way using <a href=\"https://github.com/Redocly/redoc\">ReDoc</a>."
 msgstr ""
 
 msgid "Divorce"
 msgstr ""
 
+msgid "Download images from the Wikipedia links in your ancestry"
+msgstr ""
+
 #, python-format
 msgid "E.g. \"%(example)s\""
 msgstr ""
 
 msgid "Emigration"
 msgstr ""
 
@@ -577,14 +580,17 @@
 
 msgid "Place"
 msgstr ""
 
 msgid "Places"
 msgstr ""
 
+msgid "Populate images"
+msgstr ""
+
 msgid "Pre-built Webpack front-end assets are available"
 msgstr ""
 
 msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr ""
 
 msgid "Presence"
@@ -697,14 +703,20 @@
 
 msgid "Stop the site"
 msgstr ""
 
 msgid "Subject"
 msgstr ""
 
+msgid "The Gramps {gramps_entity_reference} entity has a \"betty:link-{link_name}:media_type\" attribute with value \"{media_type}\", which is not a valid IANA media type. This media type was ignored."
+msgstr ""
+
+msgid "The Gramps {gramps_entity_reference} entity requires a \"betty:link-{link_name}:url\" attribute. This link was ignored."
+msgstr ""
+
 msgid "The age at which people are presumed dead."
 msgstr ""
 
 msgid "The base URL must include a path."
 msgstr ""
 
 msgid "The base URL must start with a scheme such as https://, http://, or file://."
```

### Comparing `betty-0.3.4/betty/assets/locale/de-DE/betty.po` & `betty-0.3.5/betty/assets/locale/de-DE/betty.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Betty project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Betty VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-30 22:56+0100\n"
+"POT-Creation-Date: 2024-05-08 17:53+0100\n"
 "PO-Revision-Date: 2024-02-08 13:24+0000\n"
 "Last-Translator: Bart Feenstra <bart@bartfeenstra.com>\n"
 "Language: de\n"
 "Language-Team: rainerthi@gmail.com\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -478,14 +478,17 @@
 msgstr ""
 "Zeige die HTTP-API-Dokumentation auf benutzerfreundliche Weise mit <a "
 "href=\"https://github.com/Redocly/redoc\">ReDoc</a> an."
 
 msgid "Divorce"
 msgstr "Scheidung"
 
+msgid "Download images from the Wikipedia links in your ancestry"
+msgstr ""
+
 #, python-format
 msgid "E.g. \"%(example)s\""
 msgstr "Z.B. \"%(example)s\""
 
 msgid "Emigration"
 msgstr "Auswanderung"
 
@@ -747,14 +750,17 @@
 
 msgid "Place"
 msgstr "Ort"
 
 msgid "Places"
 msgstr "Orte"
 
+msgid "Populate images"
+msgstr ""
+
 msgid "Pre-built Webpack front-end assets are available"
 msgstr "Vorgefertigte Webpack front-end assets sind verfügbar"
 
 msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr "Vorgefertigte Webpack front-end assets sind nicht verfügbar"
 
 msgid "Presence"
@@ -886,14 +892,26 @@
 
 msgid "Stop the site"
 msgstr "Seite anhalten"
 
 msgid "Subject"
 msgstr "Betreff"
 
+msgid ""
+"The Gramps {gramps_entity_reference} entity has a "
+"\"betty:link-{link_name}:media_type\" attribute with value "
+"\"{media_type}\", which is not a valid IANA media type. This media type "
+"was ignored."
+msgstr ""
+
+msgid ""
+"The Gramps {gramps_entity_reference} entity requires a "
+"\"betty:link-{link_name}:url\" attribute. This link was ignored."
+msgstr ""
+
 msgid "The age at which people are presumed dead."
 msgstr "Das Alter, ab dem Menschen als tot angesehen werden."
 
 msgid "The base URL must include a path."
 msgstr "Die Basis-URL muss einen Pfad beinhalten."
 
 msgid ""
```

### Comparing `betty-0.3.4/betty/assets/locale/fr-FR/betty.po` & `betty-0.3.5/betty/assets/locale/fr-FR/betty.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-30 22:56+0100\n"
+"POT-Creation-Date: 2024-05-08 17:53+0100\n"
 "PO-Revision-Date: 2024-02-08 13:24+0000\n"
 "Last-Translator: Bart Feenstra <bart@bartfeenstra.com>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -398,14 +398,17 @@
 "Display the HTTP API documentation in a user-friendly way using <a "
 "href=\"https://github.com/Redocly/redoc\">ReDoc</a>."
 msgstr ""
 
 msgid "Divorce"
 msgstr "Divorce"
 
+msgid "Download images from the Wikipedia links in your ancestry"
+msgstr ""
+
 #, python-format
 msgid "E.g. \"%(example)s\""
 msgstr "Par exemple \"%(example)s\""
 
 msgid "Emigration"
 msgstr "Emigration"
 
@@ -661,14 +664,17 @@
 
 msgid "Place"
 msgstr "Lieu"
 
 msgid "Places"
 msgstr "Lieux"
 
+msgid "Populate images"
+msgstr ""
+
 msgid "Pre-built Webpack front-end assets are available"
 msgstr ""
 
 msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr ""
 
 msgid "Presence"
@@ -790,14 +796,26 @@
 
 msgid "Stop the site"
 msgstr ""
 
 msgid "Subject"
 msgstr "Sujet"
 
+msgid ""
+"The Gramps {gramps_entity_reference} entity has a "
+"\"betty:link-{link_name}:media_type\" attribute with value "
+"\"{media_type}\", which is not a valid IANA media type. This media type "
+"was ignored."
+msgstr ""
+
+msgid ""
+"The Gramps {gramps_entity_reference} entity requires a "
+"\"betty:link-{link_name}:url\" attribute. This link was ignored."
+msgstr ""
+
 msgid "The age at which people are presumed dead."
 msgstr ""
 
 msgid "The base URL must include a path."
 msgstr ""
 
 msgid ""
```

### Comparing `betty-0.3.4/betty/assets/locale/nl-NL/betty.po` & `betty-0.3.5/betty/assets/locale/nl-NL/betty.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-30 22:56+0100\n"
+"POT-Creation-Date: 2024-05-08 17:53+0100\n"
 "PO-Revision-Date: 2024-02-11 15:31+0000\n"
 "Last-Translator: Bart Feenstra <bart@bartfeenstra.com>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -471,14 +471,17 @@
 msgstr ""
 "Geef de HTTP API-documentatie op een gebruiksvriendelijke manier weer met"
 " behulp van <a href=\"https://github.com/Redocly/redoc\">ReDoc</a>."
 
 msgid "Divorce"
 msgstr "Echtscheiding"
 
+msgid "Download images from the Wikipedia links in your ancestry"
+msgstr "Download afbeeldingen gebaseerd op de Wikipedialinks in je familiegeschiedenis"
+
 #, python-format
 msgid "E.g. \"%(example)s\""
 msgstr "Bijvoorbeeld \"%(example)s\""
 
 msgid "Emigration"
 msgstr "Emigratie"
 
@@ -742,14 +745,17 @@
 
 msgid "Place"
 msgstr "Plaats"
 
 msgid "Places"
 msgstr "Plaatsen"
 
+msgid "Populate images"
+msgstr "Afbeeldingen aanvullen"
+
 msgid "Pre-built Webpack front-end assets are available"
 msgstr "Vooraf gebouwde Webpack front-end assets zijn beschikbaar."
 
 msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr "Vooraf gebouwde Webpack front-end assets zijn niet beschikbaar."
 
 msgid "Presence"
@@ -880,14 +886,30 @@
 
 msgid "Stop the site"
 msgstr "Stop de site"
 
 msgid "Subject"
 msgstr "Onderwerp"
 
+msgid ""
+"The Gramps {gramps_entity_reference} entity has a "
+"\"betty:link-{link_name}:media_type\" attribute with value "
+"\"{media_type}\", which is not a valid IANA media type. This media type "
+"was ignored."
+msgstr ""
+"De Gramps-entiteit {gramps_entity_reference} heeft een attribuut "
+"\"betty:link-{link_name}:media_type\" met waarde \"{media_type}\", wat "
+"geen geldig IANA-mediatype is. Dit mediatype is genegeerd."
+
+msgid ""
+"The Gramps {gramps_entity_reference} entity requires a "
+"\"betty:link-{link_name}:url\" attribute. This link was ignored."
+msgstr "De Gramps-entiteit {gramps_entity_reference} vereist het "
+"attribuut \"betty:link-{link_name}:url\". Deze link is genegeerd."
+
 msgid "The age at which people are presumed dead."
 msgstr "De leeftijd waarop mensen overleden verondersteld worden."
 
 msgid "The base URL must include a path."
 msgstr "De basis-URL moet een pad bevatten."
 
 msgid ""
```

### Comparing `betty-0.3.4/betty/assets/locale/uk/betty.po` & `betty-0.3.5/betty/assets/locale/uk/betty.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Betty project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Betty VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-30 22:56+0100\n"
+"POT-Creation-Date: 2024-05-08 17:53+0100\n"
 "PO-Revision-Date: 2024-02-08 13:08+0000\n"
 "Last-Translator: Rainer Thieringer <rainerthi@gmail.com>\n"
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
@@ -399,14 +399,17 @@
 "Display the HTTP API documentation in a user-friendly way using <a "
 "href=\"https://github.com/Redocly/redoc\">ReDoc</a>."
 msgstr ""
 
 msgid "Divorce"
 msgstr "Розлучення"
 
+msgid "Download images from the Wikipedia links in your ancestry"
+msgstr ""
+
 #, python-format
 msgid "E.g. \"%(example)s\""
 msgstr "Наприклад «%(example)s»"
 
 msgid "Emigration"
 msgstr "Еміграція"
 
@@ -661,14 +664,17 @@
 
 msgid "Place"
 msgstr "Місце"
 
 msgid "Places"
 msgstr "Місця"
 
+msgid "Populate images"
+msgstr ""
+
 msgid "Pre-built Webpack front-end assets are available"
 msgstr ""
 
 msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr ""
 
 msgid "Presence"
@@ -790,14 +796,26 @@
 
 msgid "Stop the site"
 msgstr ""
 
 msgid "Subject"
 msgstr "Предмет"
 
+msgid ""
+"The Gramps {gramps_entity_reference} entity has a "
+"\"betty:link-{link_name}:media_type\" attribute with value "
+"\"{media_type}\", which is not a valid IANA media type. This media type "
+"was ignored."
+msgstr ""
+
+msgid ""
+"The Gramps {gramps_entity_reference} entity requires a "
+"\"betty:link-{link_name}:url\" attribute. This link was ignored."
+msgstr ""
+
 msgid "The age at which people are presumed dead."
 msgstr ""
 
 msgid "The base URL must include a path."
 msgstr ""
 
 msgid ""
```

### Comparing `betty-0.3.4/betty/assets/public/static/betty-16x16.png` & `betty-0.3.5/betty/assets/public/static/betty-16x16.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/assets/public/static/betty-192x192.png` & `betty-0.3.5/betty/assets/public/static/betty-192x192.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/assets/public/static/betty-32x32.png` & `betty-0.3.5/betty/assets/public/static/betty-32x32.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/assets/public/static/betty-512x512.png` & `betty-0.3.5/betty/assets/public/static/betty-512x512.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/assets/public/static/betty.ico` & `betty-0.3.5/betty/assets/public/static/betty.ico`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/assets/templates/head.html.j2` & `betty-0.3.5/betty/assets/templates/head.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/asyncio.py` & `betty-0.3.5/betty/asyncio.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/cache/__init__.py` & `betty-0.3.5/betty/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/cache/_base.py` & `betty-0.3.5/betty/cache/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,26 +96,26 @@
     @overload
     def getset(self, cache_item_id: str) -> AsyncContextManager[
         tuple[
             CacheItem[CacheItemValueContraT] | None,
             CacheItemValueSetter[CacheItemValueContraT],
         ]
     ]:
-        pass
+        pass  # pragma: no cover
 
     @overload
     def getset(
         self, cache_item_id: str, *, wait: Literal[False] = False
     ) -> AsyncContextManager[
         tuple[
             CacheItem[CacheItemValueContraT] | None,
             CacheItemValueSetter[CacheItemValueContraT] | None,
         ]
     ]:
-        pass
+        pass  # pragma: no cover
 
     @asynccontextmanager  # type: ignore[misc]
     async def getset(self, cache_item_id: str, *, wait: bool = True) -> AsyncIterator[
         tuple[
             CacheItem[CacheItemValueContraT] | None,
             CacheItemValueSetter[CacheItemValueContraT] | None,
         ]
```

### Comparing `betty-0.3.4/betty/cache/file.py` & `betty-0.3.5/betty/cache/file.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/cache/memory.py` & `betty-0.3.5/betty/cache/memory.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/cli.py` & `betty-0.3.5/betty/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,33 +3,29 @@
 """
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import sys
+from asyncio import run
 from contextlib import suppress, contextmanager
 from functools import wraps
 from pathlib import Path
 from typing import Callable, TypeVar, cast, Iterator, Awaitable, ParamSpec, Concatenate
 
 import click
 from PyQt6.QtWidgets import QMainWindow
 from click import get_current_context, Context, Option, Command, Parameter
 
-from betty import about, generate, load, documentation
+from betty import about, generate, load, documentation, locale
 from betty.app import App
-from betty.asyncio import wait_to_thread
 from betty.contextlib import SynchronizedContextManager
 from betty.error import UserFacingError
-from betty.extension import demo
-from betty.gui import BettyApplication
-from betty.gui.app import WelcomeWindow
-from betty.gui.project import ProjectWindow
-from betty.locale import update_translations, init_translation, Str
+from betty.locale import Str
 from betty.logging import CliHandler
 from betty.serde.load import AssertionFailed
 from betty.serve import AppServer
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
@@ -46,66 +42,67 @@
     Catch and log all exceptions.
     """
     try:
         yield
     except KeyboardInterrupt:
         print("Quitting...")
         sys.exit(0)
-    except BaseException as e:  # noqa: B036
+    except Exception as e:
         logger = logging.getLogger(__name__)
         if isinstance(e, UserFacingError):
             logger.error(str(e))
         else:
             logger.exception(e)
         sys.exit(1)
 
 
-def _command(
-    f: Callable[P, Awaitable[None]] | Callable[Concatenate[App, P], Awaitable[None]],
-    is_app_command: bool,
-) -> Callable[P, None]:
+def global_command(f: Callable[P, Awaitable[None]]) -> Callable[P, None]:
+    """
+    Decorate a command to be global.
+    """
+
     @wraps(f)
     @catch_exceptions()
     def _command(*args: P.args, **kwargs: P.kwargs) -> None:
-        if is_app_command:
-            # We must get the current Click context from the main thread.
-            # Once that is done, we can wait for the async commands to complete, which MAY be done in a thread.
-            app = get_current_context().obj["app"]
-
-            async def _app_command():
-                async with app:
-                    await f(app, *args, **kwargs)
+        # Use a wrapper, because the decorator uses Awaitable, but asyncio.run requires Coroutine.
+        async def __command():
+            await f(*args, **kwargs)
 
-            return wait_to_thread(_app_command())
-        return wait_to_thread(f(*args, **kwargs))
+        return run(__command())
 
     return _command
 
 
-def global_command(f: Callable[P, Awaitable[None]]) -> Callable[P, None]:
+def app_command(f: Callable[Concatenate[App, P], Awaitable[None]]) -> Callable[P, None]:
     """
-    Decorate a command to be global.
+    Decorate a command to receive the currently running :py:class:`betty.app.App` as its first argument.
     """
-    return _command(f, False)
 
+    @wraps(f)
+    @catch_exceptions()
+    def _command(*args: P.args, **kwargs: P.kwargs) -> None:
+        # Use a wrapper, because the decorator uses Awaitable, but asyncio.run requires Coroutine.
+        app = get_current_context().obj["app"]
 
-def app_command(f: Callable[Concatenate[App, P], Awaitable[None]]) -> Callable[P, None]:
-    """
-    Decorate a command to receive an app.
-    """
-    return _command(f, True)
+        async def __command():
+            async with app:
+                await f(app, *args, **kwargs)
+
+        return run(__command())
+
+    return _command
 
 
 @catch_exceptions()
 def _init_ctx_app(
     ctx: Context,
     __: Option | Parameter | None = None,
     configuration_file_path: str | None = None,
 ) -> None:
-    wait_to_thread(__init_ctx_app(ctx, configuration_file_path))
+    run(__init_ctx_app(ctx, configuration_file_path))
 
 
 async def __init_ctx_app(
     ctx: Context,
     configuration_file_path: str | None = None,
 ) -> None:
     ctx.ensure_object(dict)
@@ -122,15 +119,15 @@
     )
     ctx.obj["commands"] = {
         "docs": _docs,
         "clear-caches": _clear_caches,
         "demo": _demo,
         "gui": _gui,
     }
-    if wait_to_thread(about.is_development()):
+    if await about.is_development():
         ctx.obj["commands"]["init-translation"] = _init_translation
         ctx.obj["commands"]["update-translations"] = _update_translations
     ctx.obj["app"] = app
 
     if configuration_file_path is None:
         try_configuration_file_paths = [
             Path.cwd() / f"betty{extension}" for extension in {".json", ".yaml", ".yml"}
@@ -183,14 +180,15 @@
             ):
                 logger = logging.getLogger(logger_name)
                 if (
                     logger_level is not None
                     and logger.getEffectiveLevel() > logger_level
                 ):
                     logger.setLevel(logger_level)
+                    raise RuntimeError([logger_level, logger, logger.level])
 
     return _init_ctx_verbosity
 
 
 class _BettyCommands(click.MultiCommand):
     @catch_exceptions()
     def list_commands(self, ctx: Context) -> list[str]:
@@ -244,35 +242,37 @@
     is_eager=True,
     default=False,
     is_flag=True,
     help="Show most verbose output, including all log messages.",
     callback=_build_init_ctx_verbosity(logging.NOTSET, logging.NOTSET),
 )
 @click.version_option(
-    wait_to_thread(about.version_label()),
-    message=wait_to_thread(about.report()),
+    run(about.version_label()),
+    message=run(about.report()),
     prog_name="Betty",
 )
 def main(app: App, verbose: bool, more_verbose: bool, most_verbose: bool) -> None:
     """
     Launch Betty's Command-Line Interface.
     """
-    pass
+    pass  # pragma: no cover
 
 
 @click.command(help="Clear all caches.")
 @app_command
 async def _clear_caches(app: App) -> None:
     await app.cache.clear()
 
 
 @click.command(help="Explore a demonstration site.")
 @app_command
 async def _demo(app: App) -> None:
-    async with demo.DemoServer(app=app) as server:
+    from betty.extension.demo import DemoServer
+
+    async with DemoServer(app=app) as server:
         await server.show()
         while True:
             await asyncio.sleep(999)
 
 
 @click.command(help="Open Betty's graphical user interface (GUI).")
 @click.option(
@@ -281,26 +281,29 @@
     "configuration_file_path",
     is_eager=True,
     help="The path to a Betty project configuration file. Defaults to betty.json|yaml|yml in the current working directory.",
     callback=lambda _, __, configuration_file_path: (
         Path(configuration_file_path) if configuration_file_path else None
     ),
 )
-@global_command
-async def _gui(configuration_file_path: Path | None) -> None:
-    async with App.new_from_environment() as app:
-        async with BettyApplication([sys.argv[0]]).with_app(app) as qapp:
-            window: QMainWindow
-            if configuration_file_path is None:
-                window = WelcomeWindow(app)
-            else:
-                await app.project.configuration.read(configuration_file_path)
-                window = ProjectWindow(app)
-            window.show()
-            sys.exit(qapp.exec())
+@app_command
+async def _gui(app: App, configuration_file_path: Path | None) -> None:
+    from betty.gui import BettyApplication
+    from betty.gui.app import WelcomeWindow
+    from betty.gui.project import ProjectWindow
+
+    async with BettyApplication([sys.argv[0]]).with_app(app) as qapp:
+        window: QMainWindow
+        if configuration_file_path is None:
+            window = WelcomeWindow(app)
+        else:
+            await app.project.configuration.read(configuration_file_path)
+            window = ProjectWindow(app)
+        window.show()
+        sys.exit(qapp.exec())
 
 
 @click.command(help="Generate a static site.")
 @app_command
 async def _generate(app: App) -> None:
     await load.load(app)
     await generate.generate(app)
@@ -312,39 +315,38 @@
     async with AppServer.get(app) as server:
         await server.show()
         while True:
             await asyncio.sleep(999)
 
 
 @click.command(help="View the documentation.")
+@app_command
+async def _docs(app: App):
+    server = documentation.DocumentationServer(
+        app.binary_file_cache.path,
+        localizer=app.localizer,
+    )
+    async with server:
+        await server.show()
+        while True:
+            await asyncio.sleep(999)
+
+
+@click.command(
+    short_help="Initialize a new translation",
+    help="Initialize a new translation.\n\nThis is available only when developing Betty.",
+)
+@click.argument("locale")
 @global_command
-async def _docs():
-    async with App.new_from_environment() as app:
-        async with app:
-            server = documentation.DocumentationServer(
-                app.binary_file_cache.path,
-                localizer=app.localizer,
-            )
-            async with server:
-                await server.show()
-                while True:
-                    await asyncio.sleep(999)
+async def _init_translation(locale: str) -> None:
+    from betty.locale import init_translation
 
+    await init_translation(locale)
 
-if wait_to_thread(about.is_development()):
 
-    @click.command(
-        short_help="Initialize a new translation",
-        help="Initialize a new translation.\n\nThis is available only when developing Betty.",
-    )
-    @click.argument("locale")
-    @global_command
-    async def _init_translation(locale: str) -> None:
-        await init_translation(locale)
-
-    @click.command(
-        short_help="Update all existing translations",
-        help="Update all existing translations.\n\nThis is available only when developing Betty.",
-    )
-    @global_command
-    async def _update_translations() -> None:
-        await update_translations()
+@click.command(
+    short_help="Update all existing translations",
+    help="Update all existing translations.\n\nThis is available only when developing Betty.",
+)
+@global_command
+async def _update_translations() -> None:
+    await locale.update_translations()
```

### Comparing `betty-0.3.4/betty/concurrent.py` & `betty-0.3.5/betty/concurrent.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/config.py` & `betty-0.3.5/betty/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,20 +307,14 @@
         for index in sorted(unique_indices):
             yield self.to_key(index)
 
     @classmethod
     def _item_type(cls) -> type[ConfigurationT]:
         raise NotImplementedError(repr(cls))
 
-    @classmethod
-    def _create_default_item(
-        cls, configuration_key: ConfigurationKeyT
-    ) -> ConfigurationT:
-        raise NotImplementedError(repr(cls))
-
     def keys(self) -> Iterator[ConfigurationKeyT]:
         raise NotImplementedError(repr(self))
 
     def values(self) -> Iterator[ConfigurationT]:
         raise NotImplementedError(repr(self))
 
     def prepend(self, *configurations: ConfigurationT) -> None:
@@ -359,19 +353,19 @@
         return configuration_key
 
     def to_key(self, index: int) -> int:
         return index
 
     @overload
     def __getitem__(self, configuration_key: int) -> ConfigurationT:
-        pass
+        pass  # pragma: no cover
 
     @overload
     def __getitem__(self, configuration_key: slice) -> Sequence[ConfigurationT]:
-        pass
+        pass  # pragma: no cover
 
     def __getitem__(
         self, configuration_key: int | slice
     ) -> ConfigurationT | Sequence[ConfigurationT]:
         return self._configurations[configuration_key]
 
     def __iter__(self) -> Iterator[ConfigurationT]:
@@ -380,15 +374,16 @@
     def keys(self) -> Iterator[int]:
         return iter(range(0, len(self._configurations)))
 
     def values(self) -> Iterator[ConfigurationT]:
         yield from self._configurations
 
     def update(self, other: Self) -> None:
-        raise NotImplementedError(repr(self))
+        self._clear_without_dispatch()
+        self.append(*other)
 
     @classmethod
     def load(
         cls,
         dump: Dump,
         configuration: Self | None = None,
     ) -> Self:
@@ -629,14 +624,20 @@
         key_dump: str,
     ) -> Dump:
         raise NotImplementedError(repr(cls))
 
     def _dump_key(self, item_dump: VoidableDump) -> tuple[VoidableDump, str]:
         raise NotImplementedError(repr(self))
 
+    @classmethod
+    def _create_default_item(
+        cls, configuration_key: ConfigurationKeyT
+    ) -> ConfigurationT:
+        raise NotImplementedError(repr(cls))
+
 
 class Configurable(Generic[ConfigurationT]):
     _configuration: ConfigurationT
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
```

### Comparing `betty-0.3.4/betty/contextlib.py` & `betty-0.3.5/betty/contextlib.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/deriver.py` & `betty-0.3.5/betty/deriver.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/documentation.py` & `betty-0.3.5/betty/documentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 """
 Provide the Documentation API.
 """
 
 import asyncio
-import logging
 import shutil
-from contextlib import suppress, AsyncExitStack
+from contextlib import AsyncExitStack
 from pathlib import Path
-from subprocess import CalledProcessError
 from tempfile import TemporaryDirectory
 
 from aiofiles.os import makedirs
 
-from betty import serve
+from betty import serve, fs
 from betty.fs import ROOT_DIRECTORY_PATH
 from betty.locale import Str, Localizer
 from betty.serve import Server, NoPublicUrlBecauseServerNotStartedError
 from betty.subprocess import run_process
 
 
-async def _build_cache(cache_directory_path: Path) -> Path:
-    cache_directory_path /= "docs"
+async def _prebuild_documentation() -> None:
+    await _build(fs.PREBUILT_ASSETS_DIRECTORY_PATH / "documentation")
+
+
+async def _ensure_documentation_directory(cache_directory_path: Path) -> Path:
+    if (fs.PREBUILT_ASSETS_DIRECTORY_PATH / "documentation").exists():
+        return fs.PREBUILT_ASSETS_DIRECTORY_PATH / "documentation"
+    cache_directory_path /= "documentation"
     if not cache_directory_path.exists():
         await _build(cache_directory_path)
     return cache_directory_path
 
 
 async def _build(output_directory_path: Path) -> None:
-    with suppress(FileExistsError):
-        await makedirs(output_directory_path)
+    await makedirs(output_directory_path, exist_ok=True)
     with TemporaryDirectory() as working_directory_path_str:
         working_directory_path = Path(working_directory_path_str)
         # sphinx-apidoc must output to the documentation directory, but because we do not want
         # to 'pollute' that with generated files that must not be committed, do our work in a
         # temporary directory and copy the documentation source files there.
         source_directory_path = working_directory_path / "source"
         await asyncio.to_thread(
             shutil.copytree,
             ROOT_DIRECTORY_PATH / "documentation",
             source_directory_path,
         )
-        try:
-
-            await run_process(
-                [
-                    "sphinx-apidoc",
-                    "--force",
-                    "--separate",
-                    "-d",
-                    "999",
-                    "-o",
-                    str(source_directory_path),
-                    str(ROOT_DIRECTORY_PATH / "betty"),
-                    str(ROOT_DIRECTORY_PATH / "betty" / "tests"),
-                ],
-                cwd=working_directory_path,
-            )
-            await run_process(
-                [
-                    "sphinx-build",
-                    "-j",
-                    "auto",
-                    "-b",
-                    "dirhtml",
-                    str(source_directory_path),
-                    str(output_directory_path),
-                ],
-                cwd=working_directory_path,
-            )
-        except CalledProcessError as e:
-            if e.stderr is not None:
-                logging.getLogger().error(e.stderr)
-            raise
+        await run_process(
+            [
+                "sphinx-apidoc",
+                "--force",
+                "--separate",
+                "-d",
+                "999",
+                "-o",
+                str(source_directory_path),
+                str(ROOT_DIRECTORY_PATH / "betty"),
+                str(ROOT_DIRECTORY_PATH / "betty" / "tests"),
+            ],
+            cwd=working_directory_path,
+        )
+        await run_process(
+            [
+                "sphinx-build",
+                "-b",
+                "dirhtml",
+                str(source_directory_path),
+                str(output_directory_path),
+            ],
+            cwd=working_directory_path,
+        )
 
 
 class DocumentationServer(Server):
     def __init__(
         self,
         cache_directory_path: Path,
         *,
@@ -94,15 +89,17 @@
     def public_url(self) -> str:
         if self._server is not None:
             return self._server.public_url
         raise NoPublicUrlBecauseServerNotStartedError()
 
     async def start(self) -> None:
         await super().start()
-        www_directory_path = await _build_cache(self._cache_directory_path)
+        www_directory_path = await _ensure_documentation_directory(
+            self._cache_directory_path
+        )
         self._server = serve.BuiltinServer(
             www_directory_path, localizer=self._localizer
         )
         await self._exit_stack.enter_async_context(self._server)
         await self.assert_available()
 
     async def stop(self) -> None:
```

### Comparing `betty-0.3.4/betty/error.py` & `betty-0.3.5/betty/error.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/__init__.py` & `betty-0.3.5/betty/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/__init__.py` & `betty-0.3.5/betty/extension/cotton_candy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from jinja2 import pass_context
 from jinja2.runtime import Context
 
 from betty.app.extension import ConfigurableExtension, Extension, Theme
 from betty.config import Configuration
 from betty.extension.cotton_candy.search import Index
 from betty.extension.webpack import Webpack, WebpackEntrypointProvider
-from betty.functools import walk
 from betty.gui import GuiBuilder
 from betty.html import CssProvider
 from betty.jinja2 import (
     Jinja2Provider,
     context_app,
     context_localizer,
     context_job_context,
@@ -423,17 +422,17 @@
                 end_date = reference_dates[-1]
 
     if start_date is not None and end_date is not None:
         associated_people = filter(
             is_public,
             (
                 # All ancestors.
-                *walk(person, "parents"),
+                *person.ancestors,
                 # All descendants.
-                *walk(person, "children"),
+                *person.descendants,
                 # All siblings.
                 *person.siblings,
             ),
         )
         for associated_person in associated_people:
             # For associated events, we are only interested in people's start- or end-of-life events.
             for associated_presence in associated_person.presences:
```

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/index.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/public/localized/index.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/public/static/betty.webmanifest` & `betty-0.3.5/betty/extension/cotton_candy/assets/public/static/betty.webmanifest`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/base.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/base.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                 'entity/meta.html.j2',
             ] ignore missing %}
         {% endwith %}
     </a>
 </div>
 
 <div class="featured-entity-feature">
-    {% set places = place | walk('encloses') | select('entity', 'Place') | list %}
+    {% set places = place.walk_encloses | map(attribute='encloses') | select('entity', 'Place') | list %}
     {% if place.coordinates %}
         {% set places = places + [place] %}
     {% endif %}
     {% if places | length > 0 %}
         {% with hide_list = True, featured = False %}
             {% include 'entity/list--place.html.j2' %}
         {% endwith %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% set place = place | default(entity) %}
 ********** {{%% iinncclluuddee [[ ''eennttiittyy//llaabbeell----ppllaaccee..hhttmmll..jj22'',, ''eennttiittyy//llaabbeell..hhttmmll..jj22'',, ]] %%}}
 **********
 _{_%_ _w_i_t_h_ _e_m_b_e_d_d_e_d_ _=_ _T_r_u_e_ _%_}_ _{_%_ _i_n_c_l_u_d_e_ _[_ _'_e_n_t_i_t_y_/_m_e_t_a_-_-_p_l_a_c_e_._h_t_m_l_._j_2_'_,_ _'_e_n_t_i_t_y_/
 _m_e_t_a_._h_t_m_l_._j_2_'_,_ _]_ _i_g_n_o_r_e_ _m_i_s_s_i_n_g_ _%_}_ _{_%_ _e_n_d_w_i_t_h_ _%_}
-{% set places = place | walk('encloses') | select('entity', 'Place') | list %}
-{% if place.coordinates %} {% set places = places + [place] %} {% endif %} {%
-if places | length > 0 %} {% with hide_list = True, featured = False %} {%
-include 'entity/list--place.html.j2' %} {% endwith %} {% endif %}
+{% set places = place.walk_encloses | map(attribute='encloses') | select
+('entity', 'Place') | list %} {% if place.coordinates %} {% set places = places
++ [place] %} {% endif %} {% if places | length > 0 %} {% with hide_list = True,
+featured = False %} {% include 'entity/list--place.html.j2' %} {% endwith %} {%
+endif %}
```

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                                     {%- trans sibling_count = siblings | length -%}
                                         They grew up with a sibling.
                                     {%- pluralize -%}
                                         They grew up with {{ sibling_count }} siblings.
                                     {%- endtrans -%}
                                 {% endif %}
                             </p>
-                            {% set ancestral_affiliation_names = person | walk('parents') | select('public') | map(attribute='names') | flatten | select('public') | map(attribute='affiliation') | reject('none') | unique | list | sort %}
+                            {% set ancestral_affiliation_names = person.ancestors | select('public') | map(attribute='names') | flatten | select('public') | map(attribute='affiliation') | reject('none') | unique | list | sort %}
                             {% if ancestral_affiliation_names | length > 0 %}
                                 <p>
                                     {%- trans -%}
                                         Ancestral names include
                                     {%- endtrans %}
                                     {{ ancestral_affiliation_names[:3] | join(', ') -}}
                                     {%- if ancestral_affiliation_names | length <= 3 -%}
@@ -163,15 +163,15 @@
                                                 They had {{ child_count }} children.
                                             {%- endtrans -%}
                                         {%- endif -%}
                                     {%- endif -%}
                                 </p>
                                 {% set ns = namespace(descendant_affiliation_names=[]) %}
                                 {% for per_parent_child in family_children %}
-                                    {% set ns.descendant_affiliation_names = ns.descendant_affiliation_names + (per_parent_child | walk('children') | list + [per_parent_child]) | select('public') | map(attribute='names') | flatten | select('public') | map(attribute='affiliation') | reject('none') | list %}
+                                    {% set ns.descendant_affiliation_names = ns.descendant_affiliation_names + (per_parent_child.descendants | list + [per_parent_child]) | select('public') | map(attribute='names') | flatten | select('public') | map(attribute='affiliation') | reject('none') | list %}
                                 {% endfor %}
                                 {% set ns.descendant_affiliation_names = ns.descendant_affiliation_names | unique | list | sort | list %}
                                 {% if ns.descendant_affiliation_names | length > 0 %}
                                     <p>
                                         {%- trans -%}
                                             Descendant names include
                                         {%- endtrans %} {{ ns.descendant_affiliation_names[:3] | join(', ') -}}
```

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends 'entity/page.html.j2' %}
 {% set place = place | default(entity) %}
 {% set page_title = place.names | negotiate_localizeds %}
 {% block page_content %}
     {% include 'entity/meta--place.html.j2' %}
 
-    {% set places = place | walk('encloses') | select('entity', 'Place') | list %}
+    {% set places = place.walk_encloses | map(attribute='encloses') | select('entity', 'Place') | list %}
     {% if place.coordinates %}
         {% set places = places + [place] %}
     {% endif %}
     {% if places | length > 0 %}
         <section id="places">
             <h2 class="js-visually-hidden">
                 {% trans %}Places{% endtrans %}
```

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% set page_title = source.name %}
 {% block page_content %}
     {% include 'entity/meta--source.html.j2' %}
     {% with notes = source.notes %}
         {% include 'section-notes.html.j2' %}
     {% endwith %}
 
-    {% set sources = [source] + source | walk('contains') | select('public') | list %}
+    {% set sources = [source] + source.walk_contains | select('public') | list %}
     {% set have_files = sources %}
     {% set have_files = have_files + sources | map(attribute='citations') | flatten | list %}
     {% with files = have_files | select('public') | map(attribute='files') | flatten | unique %}
         {% include 'media.html.j2' %}
     {% endwith %}
     {% set facts = sources | map(attribute='citations') | flatten | select('public') | map(attribute='facts') | flatten | select('public') | reject('has_generated_entity_id') | unique | list %}
     {% if facts | length > 0 %}
```

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/file.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/references.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/references.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2` & `betty-0.3.5/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/gui.py` & `betty-0.3.5/betty/extension/cotton_candy/gui.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/search.py` & `betty-0.3.5/betty/extension/cotton_candy/search.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/citation.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/citation.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/entity.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/entity.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/file.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/file.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/file.ts` & `betty-0.3.5/betty/extension/cotton_candy/webpack/file.ts`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/overlay.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/overlay.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/page.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/page.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/person.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/person.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/search.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/search.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/search.ts` & `betty-0.3.5/betty/extension/cotton_candy/webpack/search.ts`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/show.ts` & `betty-0.3.5/betty/extension/cotton_candy/webpack/show.ts`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/text.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/text.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/cotton_candy/webpack/variables.scss` & `betty-0.3.5/betty/extension/cotton_candy/webpack/variables.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/demo/__init__.py` & `betty-0.3.5/betty/extension/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/deriver/__init__.py` & `betty-0.3.5/betty/extension/deriver/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/gramps/__init__.py` & `betty-0.3.5/betty/extension/gramps/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/gramps/config.py` & `betty-0.3.5/betty/extension/gramps/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,28 +51,22 @@
                     | asserter.assert_setattr(configuration, "file_path"),
                 ),
             )
         )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
-        return {
-            "file": str(self.file_path),
-        }
+        return {"file": str(self.file_path) if self.file_path else None}
 
-
-class FamilyTreeConfigurationSequence(ConfigurationSequence[FamilyTreeConfiguration]):
     def update(self, other: Self) -> None:
-        self._clear_without_dispatch()
-        self.append(*other)
+        self.file_path = other.file_path
+        self._dispatch_change()
 
-    @classmethod
-    def _create_default_item(cls, configuration_key: int) -> FamilyTreeConfiguration:
-        return FamilyTreeConfiguration()
 
+class FamilyTreeConfigurationSequence(ConfigurationSequence[FamilyTreeConfiguration]):
     @classmethod
     def _item_type(cls) -> type[FamilyTreeConfiguration]:
         return FamilyTreeConfiguration
 
 
 class GrampsConfiguration(Configuration):
     def __init__(
```

### Comparing `betty-0.3.4/betty/extension/gramps/gui.py` & `betty-0.3.5/betty/extension/gramps/gui.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/http_api_doc/__init__.py` & `betty-0.3.5/betty/extension/http_api_doc/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/http_api_doc/assets/public/static/api/index.html.j2` & `betty-0.3.5/betty/extension/http_api_doc/assets/public/static/api/index.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/maps/__init__.py` & `betty-0.3.5/betty/extension/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/maps/webpack/maps.js` & `betty-0.3.5/betty/extension/maps/webpack/maps.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/nginx/artifact.py` & `betty-0.3.5/betty/extension/nginx/artifact.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/nginx/assets/content_negotiation.lua` & `betty-0.3.5/betty/extension/nginx/assets/content_negotiation.lua`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/nginx/assets/nginx.conf.j2` & `betty-0.3.5/betty/extension/nginx/assets/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/nginx/docker.py` & `betty-0.3.5/betty/extension/nginx/docker.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/nginx/serve.py` & `betty-0.3.5/betty/extension/nginx/serve.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,12 +83,12 @@
         if self._container is not None:
             return "http://%s" % self._container.ip
         raise NoPublicUrlBecauseServerNotStartedError()
 
     @classmethod
     def is_available(cls) -> bool:
         try:
-            docker.from_env().info()
+            docker.from_env()
             return True
         except DockerException as e:
             logging.getLogger(__name__).warning(e)
             return False
```

### Comparing `betty-0.3.4/betty/extension/privatizer/__init__.py` & `betty-0.3.5/betty/extension/privatizer/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/trees/__init__.py` & `betty-0.3.5/betty/extension/trees/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/trees/assets/public/localized/people.json.j2` & `betty-0.3.5/betty/extension/trees/assets/public/localized/people.json.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/trees/webpack/trees.js` & `betty-0.3.5/betty/extension/trees/webpack/trees.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/webpack/__init__.py` & `betty-0.3.5/betty/extension/webpack/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from shutil import copytree
 from typing import Any
 
 from aiofiles.tempfile import TemporaryDirectory
 
 from betty import fs
 from betty._npm import NpmRequirement, NpmUnavailable
-from betty.app.extension import Extension
+from betty.app import App
+from betty.app.extension import Extension, discover_extension_types
 from betty.extension.webpack import build
 from betty.extension.webpack.build import webpack_build_id
 from betty.extension.webpack.jinja2.filter import FILTERS
 from betty.generate import Generator, GenerationContext
 from betty.html import CssProvider
 from betty.jinja2 import Jinja2Provider
 from betty.job import Context
@@ -39,14 +40,32 @@
     return (
         fs.PREBUILT_ASSETS_DIRECTORY_PATH
         / "webpack"
         / f"build-{webpack_build_id(entrypoint_providers)}"
     )
 
 
+async def _prebuild_webpack_assets() -> None:
+    """
+    Prebuild Webpack assets for inclusion in package builds.
+    """
+    job_context = Context()
+    async with App.new_temporary() as app, app:
+        app.project.configuration.extensions.enable(Webpack)
+        webpack = app.extensions[Webpack]
+        app.project.configuration.extensions.enable(
+            *{
+                extension_type
+                for extension_type in discover_extension_types()
+                if issubclass(extension_type, WebpackEntrypointProvider)
+            }
+        )
+        await webpack.prebuild(job_context=job_context)
+
+
 class WebpackEntrypointProvider:
     @classmethod
     def webpack_entrypoint_directory_path(cls) -> Path:
         """
         Get the path to the directory with the entrypoint assets.
 
         The directory must include at least a ``package.json`` and ``main.ts``.
```

### Comparing `betty-0.3.4/betty/extension/webpack/build.py` & `betty-0.3.5/betty/extension/webpack/build.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/webpack/jinja2/filter.py` & `betty-0.3.5/betty/extension/webpack/jinja2/filter.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/webpack/webpack/package.json` & `betty-0.3.5/betty/extension/webpack/webpack/package.json`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/webpack/webpack/webpack.config.js` & `betty-0.3.5/betty/extension/webpack/webpack/webpack.config.js`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/extension/wikipedia/__init__.py` & `betty-0.3.5/betty/extension/wikipedia/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,45 +5,63 @@
 import logging
 from pathlib import Path
 from typing import Callable, Iterable, Any
 
 from jinja2 import pass_context
 from jinja2.runtime import Context
 
-from betty import wikipedia
-from betty.app.extension import UserFacingExtension
+from betty.app.extension import UserFacingExtension, ConfigurableExtension
 from betty.asyncio import gather
+from betty.extension.wikipedia.config import WikipediaConfiguration
+from betty.extension.wikipedia.gui import _WikipediaGuiWidget
+from betty.gui import GuiBuilder
 from betty.jinja2 import Jinja2Provider, context_localizer
 from betty.load import PostLoader
 from betty.locale import negotiate_locale, Str
 from betty.model.ancestry import Link
-from betty.wikipedia import Summary, _parse_url, NotAPageError, RetrievalError
-
-
-class Wikipedia(UserFacingExtension, Jinja2Provider, PostLoader):
+from betty.wikipedia import (
+    Summary,
+    _parse_url,
+    NotAPageError,
+    RetrievalError,
+    _Fetcher,
+    _Retriever,
+    _Populator,
+)
+
+
+class Wikipedia(
+    ConfigurableExtension[WikipediaConfiguration],
+    UserFacingExtension,
+    Jinja2Provider,
+    PostLoader,
+    GuiBuilder,
+):
     @classmethod
     def name(cls) -> str:
         return "betty.extension.Wikipedia"
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
-        self.__retriever: wikipedia._Retriever | None = None
-        self.__populator: wikipedia._Populator | None = None
+        self.__retriever: _Retriever | None = None
+        self.__populator: _Populator | None = None
 
     async def post_load(self) -> None:
-        populator = wikipedia._Populator(self.app, self._retriever)
+        populator = _Populator(self.app, self._retriever)
         await populator.populate()
 
     @property
-    def _retriever(self) -> wikipedia._Retriever:
+    def _retriever(self) -> _Retriever:
         if self.__retriever is None:
-            self.__retriever = wikipedia._Retriever(
-                self.app.http_client,
-                self._app.cache,
-                self._app.binary_file_cache.with_scope(self.name()),
+            self.__retriever = _Retriever(
+                _Fetcher(
+                    self.app.http_client,
+                    self._app.cache,
+                    self._app.binary_file_cache.with_scope(self.name()),
+                ),
             )
         return self.__retriever
 
     @_retriever.deleter
     def _retriever(self) -> None:
         self.__retriever = None
 
@@ -98,7 +116,14 @@
             """
 Display <a href="https://www.wikipedia.org/">Wikipedia</a> summaries for resources with external links. In your custom <a href="https://jinja2docs.readthedocs.io/en/stable/">Jinja2</a> templates, use the following: <pre><code>
 {{% with resource=resource_with_links %}}
     {{% include 'wikipedia.html.j2' %}}
 {{% endwith %}}
 </code></pre>"""
         )
+
+    @classmethod
+    def default_configuration(cls) -> WikipediaConfiguration:
+        return WikipediaConfiguration()
+
+    def gui_build(self) -> _WikipediaGuiWidget:
+        return _WikipediaGuiWidget(self._app, self._configuration)
```

### Comparing `betty-0.3.4/betty/fs.py` & `betty-0.3.5/betty/fs.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/functools.py` & `betty-0.3.5/betty/functools.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,23 @@
     Iterator,
     Generic,
     cast,
     ParamSpec,
     Awaitable,
 )
 
+from betty.warnings import deprecated
+
 T = TypeVar("T")
 U = TypeVar("U")
 
 
+@deprecated(
+    "This function is deprecated as of Betty 0.3.5, and will be removed in Betty 0.4.x. Instead, use a custom function, tailored to your data type."
+)
 def walk(item: Any, attribute_name: str) -> Iterable[Any]:
     """
     Walk over a graph of objects by following a single attribute.
     """
     child = getattr(item, attribute_name)
 
     # If the child has the requested attribute, yield it,
```

### Comparing `betty-0.3.4/betty/generate.py` & `betty-0.3.5/betty/generate.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gramps/loader.py` & `betty-0.3.5/betty/gramps/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 
 from __future__ import annotations
 
 import gzip
 import re
 import tarfile
 from collections import defaultdict
+from collections.abc import MutableMapping, Mapping
 from contextlib import suppress
+from dataclasses import dataclass
+from enum import Enum
 from logging import getLogger
 from pathlib import Path
 from typing import Iterable, Any, IO, cast
 from xml.etree import ElementTree
 
 import aiofiles
 from aiofiles.tempfile import TemporaryDirectory
 from geopy import Point
 
 from betty.gramps.error import GrampsError
 from betty.locale import DateRange, Datey, Date, Str, Localizer
-from betty.media_type import MediaType
+from betty.media_type import MediaType, InvalidMediaType
 from betty.model import Entity, EntityGraphBuilder, AliasedEntity, AliasableEntity
 from betty.model.ancestry import (
     Ancestry,
     Note,
     File,
     Source,
     Citation,
@@ -77,23 +80,40 @@
 )
 from betty.path import rootname
 from betty.project import Project
 from betty.warnings import deprecate
 
 
 class GrampsLoadFileError(GrampsError, RuntimeError):
-    pass
+    pass  # pragma: no cover
 
 
 class GrampsFileNotFoundError(GrampsError, FileNotFoundError):
-    pass
+    pass  # pragma: no cover
 
 
 class XPathError(GrampsError, RuntimeError):
-    pass
+    pass  # pragma: no cover
+
+
+class GrampsEntityType(Enum):
+    CITATION = "citation"
+    EVENT = "event"
+    OBJECT = "object"
+    PERSON = "person"
+    SOURCE = "source"
+
+
+@dataclass(frozen=True)
+class GrampsEntityReference:
+    entity_type: GrampsEntityType
+    entity_id: str
+
+    def __str__(self) -> str:
+        return f"{self.entity_type.value} ({self.entity_id})"
 
 
 class GrampsLoader:
     def __init__(
         self,
         project_or_ancestry: Project | Ancestry,
         *,
@@ -400,15 +420,20 @@
         description = file_element.get("description")
         if description:
             file.description = description
         if element.get("priv") == "1":
             file.private = True
         aliased_file = AliasedEntity(file, file_handle)
 
-        self._load_attributes(file, element, "attribute")
+        self._load_attributes_for(
+            file,
+            GrampsEntityReference(GrampsEntityType.OBJECT, file.id),
+            element,
+            "attribute",
+        )
 
         self.add_entity(
             aliased_file,  # type: ignore[arg-type]
         )
         for citation_handle in self._load_handles("citationref", element):
             self.add_association(
                 File, file_handle, "citations", Citation, citation_handle
@@ -466,15 +491,20 @@
                 Person, person_handle, "names", PersonName, person_name.id
             )
 
         self._load_eventrefs(person_handle, element)
         if element.get("priv") == "1":
             person.private = True
 
-        self._load_attributes(person, element, "attribute")
+        self._load_attributes_for(
+            person,
+            GrampsEntityReference(GrampsEntityType.PERSON, person.id),
+            element,
+            "attribute",
+        )
 
         aliased_person = AliasedEntity(person, person_handle)
         self._load_citationref(
             aliased_person,  # type: ignore[arg-type]
             element,
         )
         self._load_objref(
@@ -554,15 +584,20 @@
                 )
             )
 
         presence = Presence(None, role, None)
         if eventref.get("priv") == "1":
             presence.private = True
 
-        self._load_attributes(presence, eventref, "attribute")
+        self._load_attributes_for(
+            presence,
+            GrampsEntityReference(GrampsEntityType.PERSON, person_id),
+            eventref,
+            "attribute",
+        )
 
         self.add_entity(presence)
         self.add_association(Presence, presence.id, "person", Person, person_id)
         self.add_association(Presence, presence.id, "event", Event, event_handle)
 
     def _load_places(self, database: ElementTree.Element) -> None:
         for element in self._xpath(database, "./ns:places/ns:placeobj"):
@@ -721,15 +756,20 @@
             element,
         )
         self._load_noteref(
             aliased_event,  # type: ignore[arg-type]
             element,
         )
 
-        self._load_attributes(event, element, "attribute")
+        self._load_attributes_for(
+            event,
+            GrampsEntityReference(GrampsEntityType.EVENT, event.id),
+            element,
+            "attribute",
+        )
 
         self.add_entity(
             aliased_event,  # type: ignore[arg-type]
         )
 
     def _load_repositories(self, database: ElementTree.Element) -> None:
         for element in self._xpath(database, "./ns:repositories/ns:repository"):
@@ -782,15 +822,20 @@
         # Load the publication info.
         with suppress(XPathError):
             source.publisher = self._xpath1(element, "./ns:spubinfo").text
 
         if element.get("priv") == "1":
             source.private = True
 
-        self._load_attributes(source, element, "srcattribute")
+        self._load_attributes_for(
+            source,
+            GrampsEntityReference(GrampsEntityType.SOURCE, source.id),
+            element,
+            "srcattribute",
+        )
 
         aliased_source = AliasedEntity(source, source_handle)
         self._load_objref(
             aliased_source,  # type: ignore[arg-type]
             element,
         )
         self._load_noteref(
@@ -821,15 +866,20 @@
 
         aliased_citation = AliasedEntity(citation, citation_handle)
         self._load_objref(
             aliased_citation,  # type: ignore[arg-type]
             element,
         )
 
-        self._load_attributes(citation, element, "srcattribute")
+        self._load_attributes_for(
+            citation,
+            GrampsEntityReference(GrampsEntityType.CITATION, citation.id),
+            element,
+            "srcattribute",
+        )
 
         self.add_entity(
             aliased_citation,  # type: ignore[arg-type]
         )
 
     def _load_citationref(
         self,
@@ -890,25 +940,106 @@
                 privacy_value=privacy_value,
                 entity_type=entity.entity_type_label().localize(self._localizer),
                 entity_id=entity.id,
                 entity_label=entity.label.localize(self._localizer),
             )
         )
 
+    _LINK_ATTRIBUTE_PATTERN = re.compile(r"^link-([^:]+?):(.+?)$")
+
+    def _load_attribute_links(
+        self,
+        entity: HasLinks & Entity,
+        gramps_entity_reference: GrampsEntityReference,
+        element: ElementTree.Element,
+        tag: str,
+    ) -> None:
+        logger = getLogger(__name__)
+
+        attributes = self._load_attributes(element, tag)
+        links_attributes: MutableMapping[str, MutableMapping[str, str]] = defaultdict(
+            dict
+        )
+        for attribute_type, attribute_value in attributes.items():
+            match = self._LINK_ATTRIBUTE_PATTERN.fullmatch(attribute_type)
+            if match is None:
+                continue
+            link_name = match.group(1)
+            link_attribute_name = match.group(2)
+            links_attributes[link_name][link_attribute_name] = attribute_value
+        for link_name, link_attributes in links_attributes.items():
+            if "url" not in link_attributes:
+                logger.warning(
+                    self._localizer._(
+                        'The Gramps {gramps_entity_reference} entity requires a "betty:link-{link_name}:url" attribute. This link was ignored.',
+                    ).format(
+                        gramps_entity_reference=gramps_entity_reference,
+                        link_name=link_name,
+                    )
+                )
+                continue
+            link = Link(link_attributes["url"])
+            entity.links.append(link)
+            if "description" in link_attributes:
+                link.description = link_attributes["description"]
+            if "label" in link_attributes:
+                link.label = link_attributes["label"]
+            if "locale" in link_attributes:
+                link.locale = link_attributes["locale"]
+            if "media_type" in link_attributes:
+                try:
+                    media_type = MediaType(link_attributes["media_type"])
+                except InvalidMediaType:
+                    logger.warning(
+                        self._localizer._(
+                            'The Gramps {gramps_entity_reference} entity has a "betty:link-{link_name}:media_type" attribute with value "{media_type}", which is not a valid IANA media type. This media type was ignored.',
+                        ).format(
+                            gramps_entity_reference=gramps_entity_reference,
+                            link_name=link_name,
+                            media_type=link_attributes["media_type"],
+                        )
+                    )
+                else:
+                    link.media_type = media_type
+            if "relationship" in link_attributes:
+                link.relationship = link_attributes["relationship"]
+
     def _load_attribute(
         self, name: str, element: ElementTree.Element, tag: str
     ) -> str | None:
+        try:
+            return self._load_attributes(element, tag)[name]
+        except KeyError:
+            return None
+
+    def _load_attributes(
+        self, element: ElementTree.Element, tag: str
+    ) -> Mapping[str, str]:
         prefixes = ["betty"]
+        hash(element)
         if self._project is not None and self._project.configuration.name is not None:
-            prefixes.insert(0, f"betty-{self._project.configuration.name}")
+            prefixes.append(f"betty-{self._project.configuration.name}")
+        attributes: MutableMapping[str, str] = {}
         for prefix in prefixes:
             with suppress(XPathError):
-                return self._xpath1(
-                    element, f'./ns:{tag}[@type="{prefix}:{name}"]'
-                ).get("value")
-        return None
+                attribute_elements = self._xpath(element, f"./ns:{tag}")
+                for attribute_element in attribute_elements:
+                    attribute_type = attribute_element.attrib["type"]
+                    attribute_value = attribute_element.get("value")
+                    if (
+                        attribute_type.startswith(f"{prefix}:")
+                        and attribute_value is not None
+                    ):
+                        attributes[attribute_type[len(prefix) + 1 :]] = attribute_value
+        return attributes
 
-    def _load_attributes(
-        self, entity: Entity, element: ElementTree.Element, tag: str
+    def _load_attributes_for(
+        self,
+        entity: Entity,
+        gramps_entity_reference: GrampsEntityReference,
+        element: ElementTree.Element,
+        tag: str,
     ) -> None:
         if isinstance(entity, HasPrivacy):
             self._load_attribute_privacy(entity, element, tag)
+        if isinstance(entity, HasLinks):
+            self._load_attribute_links(entity, gramps_entity_reference, element, tag)
```

### Comparing `betty-0.3.4/betty/gui/__init__.py` & `betty-0.3.5/betty/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/app.py` & `betty-0.3.5/betty/gui/app.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/error.py` & `betty-0.3.5/betty/gui/error.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/locale.py` & `betty-0.3.5/betty/gui/locale.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/logging.py` & `betty-0.3.5/betty/gui/logging.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/model.py` & `betty-0.3.5/betty/gui/model.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/project.py` & `betty-0.3.5/betty/gui/project.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/serve.py` & `betty-0.3.5/betty/gui/serve.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/text.py` & `betty-0.3.5/betty/gui/text.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/gui/window.py` & `betty-0.3.5/betty/gui/window.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/hashid.py` & `betty-0.3.5/betty/hashid.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/importlib.py` & `betty-0.3.5/betty/importlib.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/jinja2/__init__.py` & `betty-0.3.5/betty/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/jinja2/filter.py` & `betty-0.3.5/betty/jinja2/filter.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/jinja2/test.py` & `betty-0.3.5/betty/jinja2/test.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/job.py` & `betty-0.3.5/betty/job.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/json/linked_data.py` & `betty-0.3.5/betty/json/linked_data.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/json/schema.py` & `betty-0.3.5/betty/json/schema.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/load.py` & `betty-0.3.5/betty/load.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/locale.py` & `betty-0.3.5/betty/locale.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         schema = await super().linked_data_schema(app)
         properties = dump_default(schema, "properties", dict)
         properties["locale"] = ref_locale(schema)
         return schema
 
 
 class IncompleteDateError(ValueError):
-    pass
+    pass  # pragma: no cover
 
 
 def _dump_date_iso8601(date: Date) -> str | None:
     if not date.complete:
         return None
     assert date.year
     assert date.month
```

### Comparing `betty-0.3.4/betty/logging.py` & `betty-0.3.5/betty/logging.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/media_type.py` & `betty-0.3.5/betty/media_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 from email.message import EmailMessage
 from typing import Any
 
 
 class InvalidMediaType(ValueError):
-    pass
+    pass  # pragma: no cover
 
 
 class MediaType:
     def __init__(self, media_type: str):
         self._str = media_type
         message = EmailMessage()
         message["Content-Type"] = media_type
@@ -23,14 +23,17 @@
         if not media_type.startswith(type_part):
             raise InvalidMediaType(f'"{media_type}" is not a valid media type.')
         self._parameters: dict[str, str] = dict(message["Content-Type"].params)
         self._type, self._subtype = type_part.split("/")
         if not self._subtype:
             raise InvalidMediaType("The subtype must not be empty.")
 
+    def __hash__(self) -> int:
+        return hash(self._str)
+
     @property
     def type(self) -> str:
         return self._type
 
     @property
     def subtype(self) -> str:
         return self._subtype
```

### Comparing `betty-0.3.4/betty/model/__init__.py` & `betty-0.3.5/betty/model/__init__.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/model/ancestry.py` & `betty-0.3.5/betty/model/ancestry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Provide Betty's main data model.
 """
 
 from __future__ import annotations
 
-from collections.abc import MutableSequence
+from collections.abc import MutableSequence, Iterator
 from contextlib import suppress
 from enum import Enum
 from pathlib import Path
 from reprlib import recursive_repr
 from typing import Iterable, Any, TYPE_CHECKING
 from urllib.parse import quote
 
@@ -467,19 +467,19 @@
         )
         self._text = text
         if entity is not None:
             self.entity = entity
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Note")
+        return Str._("Note")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Notes")
+        return Str._("Notes")  # pragma: no cover
 
     @property
     def text(self) -> str:
         return self._text
 
     @property
     def label(self) -> Str:
@@ -512,23 +512,23 @@
             **kwargs,
         )
         if notes is not None:
             self.notes = notes  # type: ignore[assignment]
 
     @property
     def notes(self) -> EntityCollection[Note]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @notes.setter
     def notes(self, notes: Iterable[Note]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @notes.deleter
     def notes(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         dump["notes"] = [
             app.static_url_generator.generate(f"/note/{quote(note.id)}/index.json")
             for note in self.notes
             if not isinstance(note.id, GeneratedEntityId)
@@ -561,23 +561,23 @@
             **kwargs,
         )
         if citations is not None:
             self.citations = citations  # type: ignore[assignment]
 
     @property
     def citations(self) -> EntityCollection[Citation]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @citations.setter
     def citations(self, citations: Iterable[Citation]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @citations.deleter
     def citations(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         dump["citations"] = [
             app.static_url_generator.generate(
                 f"/citation/{quote(citation.id)}/index.json"
             )
@@ -635,31 +635,31 @@
             private=private,
             links=links,
         )
         self._path = path
 
     @property
     def entities(self) -> EntityCollection[Entity]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @entities.setter
     def entities(self, entities: Iterable[Entity]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @entities.deleter
     def entities(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("File")
+        return Str._("File")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Files")
+        return Str._("Files")  # pragma: no cover
 
     @property
     def path(self) -> Path:
         return self._path
 
     @property
     def label(self) -> Str:
@@ -700,23 +700,23 @@
             **kwargs,
         )
         if files is not None:
             self.files = files  # type: ignore[assignment]
 
     @property
     def files(self) -> EntityCollection[File]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @files.setter
     def files(self, files: Iterable[File]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @files.deleter
     def files(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @property
     def associated_files(self) -> Iterable[File]:
         return self.files
 
 
 @many_to_one("contained_by", "betty.model.ancestry.Source", "contains")
@@ -766,43 +766,49 @@
         privacy = super()._get_effective_privacy()
         if self.contained_by:
             return merge_privacies(privacy, self.contained_by.privacy)
         return privacy
 
     @property
     def contains(self) -> EntityCollection[Source]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @contains.setter
     def contains(self, contains: Iterable[Source]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @contains.deleter
     def contains(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @property
     def citations(self) -> EntityCollection[Citation]:  # type: ignore[empty-body]
         pass
 
     @citations.setter
     def citations(self, citations: Iterable[Citation]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @citations.deleter
     def citations(self) -> None:
-        pass
+        pass  # pragma: no cover
+
+    @property
+    def walk_contains(self) -> Iterator[Source]:
+        for source in self.contains:
+            yield source
+            yield from source.contains
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Source")
+        return Str._("Source")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Sources")
+        return Str._("Sources")  # pragma: no cover
 
     @property
     def label(self) -> Str:
         return Str.plain(self.name) if self.name else super().label
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
@@ -901,20 +907,20 @@
     @property  # type: ignore[override]
     def name(self) -> str:
         return "private"
 
     @name.setter
     def name(self, _) -> None:
         # This is a no-op as the name is 'hardcoded'.
-        pass
+        pass  # pragma: no cover
 
     @name.deleter
     def name(self) -> None:
         # This is a no-op as the name is 'hardcoded'.
-        pass
+        pass  # pragma: no cover
 
 
 @many_to_many("facts", "betty.model.ancestry.HasCitations", "citations")
 @many_to_one("source", "betty.model.ancestry.Source", "citations")
 class Citation(Dated, HasFiles, HasPrivacy, HasLinksEntity, UserFacingEntity, Entity):
     def __init__(
         self,
@@ -946,31 +952,31 @@
         privacy = super()._get_effective_privacy()
         if self.source:
             return merge_privacies(privacy, self.source.privacy)
         return privacy
 
     @property
     def facts(self) -> EntityCollection[HasCitations & Entity]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @facts.setter
     def facts(self, facts: Iterable[HasCitations & Entity]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @facts.deleter
     def facts(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Citation")
+        return Str._("Citation")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Citations")
+        return Str._("Citations")  # pragma: no cover
 
     @property
     def label(self) -> Str:
         return self.location or Str.plain("")
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
@@ -1004,25 +1010,27 @@
 
 @deprecated(
     f"This class is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. No direct replacement is available. Instead, set the privacy for {Citation} entities accordingly."
 )
 class AnonymousCitation(Citation):
     @property  # type: ignore[override]
     def location(self) -> Str:
-        return Str._("private (in order to protect people's privacy)")
+        return Str._(
+            "private (in order to protect people's privacy)"
+        )  # pragma: no cover
 
     @location.setter
     def location(self, _) -> None:
         # This is a no-op as the location is 'hardcoded'.
-        pass
+        pass  # pragma: no cover
 
     @location.deleter
     def location(self) -> None:
         # This is a no-op as the location is 'hardcoded'.
-        pass
+        pass  # pragma: no cover
 
 
 class PlaceName(Localized, Dated, LinkedDataDumpable):
     def __init__(
         self,
         name: str,
         *,
@@ -1082,19 +1090,19 @@
     ):
         super().__init__()
         self.encloses = encloses
         self.enclosed_by = enclosed_by
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Enclosure")
+        return Str._("Enclosure")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Enclosures")
+        return Str._("Enclosures")  # pragma: no cover
 
 
 @one_to_many("events", "betty.model.ancestry.Event", "place")
 @one_to_many("enclosed_by", "betty.model.ancestry.Enclosure", "encloses")
 @one_to_many("encloses", "betty.model.ancestry.Enclosure", "enclosed_by")
 class Place(HasLinksEntity, HasFiles, HasNotes, HasPrivacy, UserFacingEntity, Entity):
     def __init__(
@@ -1127,55 +1135,62 @@
         if enclosed_by is not None:
             self.enclosed_by = enclosed_by  # type: ignore[assignment]
         if encloses is not None:
             self.encloses = encloses  # type: ignore[assignment]
 
     @property
     def enclosed_by(self) -> EntityCollection[Enclosure]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @enclosed_by.setter
     def enclosed_by(self, enclosed_by: Iterable[Enclosure]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @enclosed_by.deleter
     def enclosed_by(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @property
     def encloses(self) -> EntityCollection[Enclosure]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @encloses.setter
     def encloses(self, encloses: Iterable[Enclosure]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @encloses.deleter
     def encloses(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @property
     def events(self) -> EntityCollection[Event]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @events.setter
     def events(self, events: Iterable[Event]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @events.deleter
     def events(self) -> None:
-        pass
+        pass  # pragma: no cover
+
+    @property
+    def walk_encloses(self) -> Iterator[Enclosure]:
+        for enclosure in self.encloses:
+            yield enclosure
+            if enclosure.encloses is not None:
+                yield from enclosure.encloses.walk_encloses
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Place")
+        return Str._("Place")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Places")
+        return Str._("Places")  # pragma: no cover
 
     @property
     def names(self) -> list[PlaceName]:
         return self._names
 
     @property
     def coordinates(self) -> Point | None:
@@ -1310,75 +1325,75 @@
 class Subject(PresenceRole):
     @classmethod
     def name(cls) -> str:
         return "subject"
 
     @property
     def label(self) -> Str:
-        return Str._("Subject")
+        return Str._("Subject")  # pragma: no cover
 
 
 class Witness(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return "witness"
+        return "witness"  # pragma: no cover
 
     @property
     def label(self) -> Str:
-        return Str._("Witness")
+        return Str._("Witness")  # pragma: no cover
 
 
 class Beneficiary(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return "beneficiary"
+        return "beneficiary"  # pragma: no cover
 
     @property
     def label(self) -> Str:
-        return Str._("Beneficiary")
+        return Str._("Beneficiary")  # pragma: no cover
 
 
 class Attendee(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return "attendee"
+        return "attendee"  # pragma: no cover
 
     @property
     def label(self) -> Str:
-        return Str._("Attendee")
+        return Str._("Attendee")  # pragma: no cover
 
 
 class Speaker(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return "speaker"
+        return "speaker"  # pragma: no cover
 
     @property
     def label(self) -> Str:
-        return Str._("Speaker")
+        return Str._("Speaker")  # pragma: no cover
 
 
 class Celebrant(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return "celebrant"
+        return "celebrant"  # pragma: no cover
 
     @property
     def label(self) -> Str:
-        return Str._("Celebrant")
+        return Str._("Celebrant")  # pragma: no cover
 
 
 class Organizer(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return "organizer"
+        return "organizer"  # pragma: no cover
 
     @property
     def label(self) -> Str:
-        return Str._("Organizer")
+        return Str._("Organizer")  # pragma: no cover
 
 
 @many_to_one_to_many(
     "betty.model.ancestry.Person",
     "presences",
     "person",
     "event",
@@ -1399,19 +1414,19 @@
         super().__init__(None)
         self.person = person
         self.role = role
         self.event = event
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Presence")
+        return Str._("Presence")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Presences")
+        return Str._("Presences")  # pragma: no cover
 
     @property
     def label(self) -> Str:
         return Str._(
             "Presence of {person} at {event}",
             person=self.person.label if self.person else Str._("Unknown"),
             event=self.event.label if self.event else Str._("Unknown"),
@@ -1506,31 +1521,31 @@
 
     @recursive_repr()
     def __repr__(self) -> str:
         return repr_instance(self, id=self._id, type=self._event_type)
 
     @property
     def presences(self) -> EntityCollection[Presence]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @presences.setter
     def presences(self, presences: Iterable[Presence]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @presences.deleter
     def presences(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Event")
+        return Str._("Event")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Events")
+        return Str._("Events")  # pragma: no cover
 
     @property
     def event_type(self) -> type[EventType]:
         return self._event_type
 
     @property
     def associated_files(self) -> Iterable[File]:
@@ -1688,19 +1703,19 @@
     def __repr__(self) -> str:
         return repr_instance(
             self, id=self.id, individual=self.individual, affiliation=self.affiliation
         )
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Person name")
+        return Str._("Person name")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("Person names")
+        return Str._("Person names")  # pragma: no cover
 
     @property
     def individual(self) -> str | None:
         return self._individual
 
     @property
     def affiliation(self) -> str | None:
@@ -1793,78 +1808,90 @@
         if presences is not None:
             self.presences = presences  # type: ignore[assignment]
         if names is not None:
             self.names = names  # type: ignore[assignment]
 
     @property
     def parents(self) -> EntityCollection[Person]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @parents.setter
     def parents(self, parents: Iterable[Person]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @parents.deleter
     def parents(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @property
     def children(self) -> EntityCollection[Person]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @children.setter
     def children(self, children: Iterable[Person]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @children.deleter
     def children(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @property
     def presences(self) -> EntityCollection[Presence]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @presences.setter
     def presences(self, presences: Iterable[Presence]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @presences.deleter
     def presences(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @property
     def names(self) -> EntityCollection[PersonName]:  # type: ignore[empty-body]
-        pass
+        pass  # pragma: no cover
 
     @names.setter
     def names(self, names: Iterable[PersonName]) -> None:
-        pass
+        pass  # pragma: no cover
 
     @names.deleter
     def names(self) -> None:
-        pass
+        pass  # pragma: no cover
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._("Person")
+        return Str._("Person")  # pragma: no cover
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._("People")
+        return Str._("People")  # pragma: no cover
+
+    @property
+    def ancestors(self) -> Iterator[Person]:
+        for parent in self.parents:
+            yield parent
+            yield from parent.ancestors
 
     @property
     def siblings(self) -> list[Person]:
         siblings = []
         for parent in self.parents:
             for sibling in parent.children:
                 if sibling != self and sibling not in siblings:
                     siblings.append(sibling)
         return siblings
 
     @property
+    def descendants(self) -> Iterator[Person]:
+        for child in self.children:
+            yield child
+            yield from child.descendants
+
+    @property
     def associated_files(self) -> Iterable[File]:
         files = [
             *self.files,
             *[
                 file
                 for name in self.names
                 for citation in name.citations
```

### Comparing `betty-0.3.4/betty/openapi.py` & `betty-0.3.5/betty/openapi.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/os.py` & `betty-0.3.5/betty/os.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/privatizer.py` & `betty-0.3.5/betty/privatizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from __future__ import annotations
 
 import logging
 from contextlib import suppress
 from datetime import datetime
 from typing import Iterator, TypeAlias, Any
 
-from betty.functools import walk
 from betty.locale import DateRange, Date, Localizer
 from betty.model import Entity
 from betty.model.ancestry import (
     Person,
     Event,
     HasFiles,
     HasCitations,
@@ -195,15 +194,15 @@
 
         for ancestor, generations_ago in self._ancestors_by_generation(person):
             if self.has_expired(ancestor, generations_ago + 1):
                 person.public = True
                 return
 
         # If any descendant has any expired event, the person is considered not private.
-        for descendant in walk(person, "children"):
+        for descendant in person.descendants:
             if self.has_expired(descendant, 1):
                 person.public = True
                 return
 
         person.private = True
         logging.getLogger(__name__).debug(
             self._localizer._(
```

### Comparing `betty-0.3.4/betty/project.py` & `betty-0.3.5/betty/project.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/render.py` & `betty-0.3.5/betty/render.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/requirement.py` & `betty-0.3.5/betty/requirement.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/serde/dump.py` & `betty-0.3.5/betty/serde/dump.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TypeVar, Sequence, Mapping, overload, Literal, TypeAlias, Any
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 class Void:
-    pass
+    pass  # pragma: no cover
 
 
 DumpType: TypeAlias = bool | int | float | str | None | list["Dump"] | dict[str, "Dump"]
 DumpTypeT = TypeVar("DumpTypeT", bound=DumpType)
 
 Dump: TypeAlias = (
     bool | int | float | str | None | Sequence["Dump"] | Mapping[str, "Dump"]
@@ -40,20 +40,20 @@
 )
 
 
 @overload
 def minimize(
     dump: _MinimizableDump[VoidableDump], voidable: Literal[True] = True
 ) -> VoidableDump:
-    pass
+    pass  # pragma: no cover
 
 
 @overload
 def minimize(dump: _MinimizableDump[VoidableDump], voidable: Literal[False]) -> Dump:
-    pass
+    pass  # pragma: no cover
 
 
 def minimize(
     dump: _MinimizableDump[VoidableDump], voidable: bool = True
 ) -> VoidableDump:
     """
     Minimize a configuration dump by removing any Void configurationfrom sequences and mappings.
@@ -86,22 +86,22 @@
     return None if value is Void else value
 
 
 @overload
 def dump_default(
     dump: DictDump[Dump], key: str, default_type: type[dict[Any, Any]]
 ) -> DictDump[Dump]:
-    pass
+    pass  # pragma: no cover
 
 
 @overload
 def dump_default(
     dump: DictDump[Dump], key: str, default_type: type[list[Any]]
 ) -> ListDump[Dump]:
-    pass
+    pass  # pragma: no cover
 
 
 def dump_default(dump, key, default_type):
     """
     Add a key and value to a dump, if the key does not exist yet.
     """
     try:
```

### Comparing `betty-0.3.4/betty/serde/error.py` & `betty-0.3.5/betty/serde/error.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/serde/format.py` & `betty-0.3.5/betty/serde/format.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/serde/load.py` & `betty-0.3.5/betty/serde/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 FValueT = TypeVar("FValueT")
 MapReturnT = TypeVar("MapReturnT")
 Number: TypeAlias = int | float
 NumberT = TypeVar("NumberT", bound=Number)
 
 
 class LoadError(SerdeError):
-    pass
+    pass  # pragma: no cover
 
 
 class AssertionFailed(LoadError):
-    pass
+    pass  # pragma: no cover
 
 
 class FormatError(LoadError):
-    pass
+    pass  # pragma: no cover
 
 
 Assertion: TypeAlias = Callable[
     [
         ValueT,
     ],
     ReturnT,
@@ -112,20 +112,20 @@
 class _Field(Generic[ValueT, ReturnT]):
     name: str
     assertion: _Assertions[ValueT, ReturnT, Any] | None = None
 
 
 @dataclass(frozen=True)
 class RequiredField(Generic[ValueT, ReturnT], _Field[ValueT, ReturnT]):
-    pass
+    pass  # pragma: no cover
 
 
 @dataclass(frozen=True)
 class OptionalField(Generic[ValueT, ReturnT], _Field[ValueT, ReturnT]):
-    pass
+    pass  # pragma: no cover
 
 
 class Fields:
     def __init__(self, *fields: _Field[Any, Any]):
         self._fields = fields
 
     def __iter__(self) -> Iterator[_Field[Any, Any]]:
@@ -302,21 +302,21 @@
 
         return _assert_fields
 
     @overload
     def assert_field(
         self, field: RequiredField[ValueT, ReturnT]
     ) -> Assertion[ValueT, ReturnT]:
-        pass
+        pass  # pragma: no cover
 
     @overload
     def assert_field(
         self, field: OptionalField[ValueT, ReturnT]
     ) -> Assertion[ValueT, ReturnT | type[Void]]:
-        pass
+        pass  # pragma: no cover
 
     def assert_field(
         self, field: _Field[ValueT, ReturnT]
     ) -> Assertion[ValueT, ReturnT | type[Void]]:
         def _assert_field(value: Any) -> ReturnT | type[Void]:
             fields = self.assert_fields(Fields(field))(value)
             try:
```

### Comparing `betty-0.3.4/betty/serve.py` & `betty-0.3.5/betty/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 from betty.functools import Do
 from betty.locale import Str, Localizer
 
 DEFAULT_PORT = 8000
 
 
 class ServerNotStartedError(RuntimeError):
-    pass
+    pass  # pragma: no cover
 
 
 class NoPublicUrlBecauseServerNotStartedError(ServerNotStartedError):
     def __init__(self):
         super().__init__(
             "Cannot get the public URL for a server that has not started yet."
         )
 
 
 class OsError(UserFacingError, OSError):
-    pass
+    pass  # pragma: no cover
 
 
 class Server:
     """
     Provide a development web server.
     """
```

### Comparing `betty-0.3.4/betty/sphinx/extension/replacements.py` & `betty-0.3.5/betty/sphinx/extension/replacements.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/string.py` & `betty-0.3.5/betty/string.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/subprocess.py` & `betty-0.3.5/betty/subprocess.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/url.py` & `betty-0.3.5/betty/url.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty/warnings.py` & `betty-0.3.5/betty/warnings.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class BettyDeprecationWarning(DeprecationWarning):
     """
     Raised for deprecated Betty functionality.
     """
 
-    pass
+    pass  # pragma: no cover
 
 
 def deprecate(message: str, stacklevel: int = 1):
     """
     Raise a Betty deprecation warning.
     """
     warnings.warn(message, category=BettyDeprecationWarning, stacklevel=stacklevel + 1)
```

### Comparing `betty-0.3.4/betty/wikipedia.py` & `betty-0.3.5/betty/wikipedia.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,38 @@
 
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import re
-from collections.abc import Sequence, MutableSequence, Callable, Awaitable
+from collections import defaultdict
+from collections.abc import (
+    Sequence,
+    MutableSequence,
+    Callable,
+    Awaitable,
+    Mapping,
+    MutableMapping,
+)
 from contextlib import suppress
 from pathlib import Path
 from time import time
 from typing import cast, Any
 from urllib.parse import quote
 
 import aiohttp
 from aiohttp import ClientResponse
 from geopy import Point
 
 from betty.app import App
 from betty.asyncio import gather
 from betty.cache import Cache, CacheItemValueT
 from betty.cache.file import BinaryFileCache
-from betty.concurrent import RateLimiter
+from betty.concurrent import RateLimiter, _Lock, AsynchronizedLock
 from betty.functools import filter_suppress
 from betty.hashid import hashid
 from betty.locale import (
     Localized,
     negotiate_locale,
     to_locale,
     get_data,
@@ -35,23 +43,23 @@
     Localey,
 )
 from betty.media_type import MediaType
 from betty.model.ancestry import Link, HasLinks, Place, File, HasFiles
 
 
 class WikipediaError(BaseException):
-    pass
+    pass  # pragma: no cover
 
 
 class NotAPageError(WikipediaError, ValueError):
-    pass
+    pass  # pragma: no cover
 
 
 class RetrievalError(WikipediaError, RuntimeError):
-    pass
+    pass  # pragma: no cover
 
 
 _URL_PATTERN = re.compile(r"^https?://([a-z]+)\.wikipedia\.org/wiki/([^/?#]+).*$")
 
 
 def _parse_url(url: str) -> tuple[str, str]:
     match = _URL_PATTERN.fullmatch(url)
@@ -63,14 +71,27 @@
 class Summary(Localized):
     def __init__(self, locale: str, name: str, title: str, content: str):
         super().__init__(locale=locale)
         self._name = name
         self._title = title
         self._content = content
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Summary):
+            return False
+        if self.name != other.name:
+            return False
+        if self.url != other.url:
+            return False
+        if self.title != other.title:
+            return False
+        if self.content != other.content:
+            return False
+        return True
+
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def url(self) -> str:
         return "https://%s.wikipedia.org/wiki/%s" % (self.locale, self._name)
@@ -93,14 +114,19 @@
         wikimedia_commons_url: str,
     ):
         self._path = path
         self._media_type = media_type
         self._title = title
         self._wikimedia_commons_url = wikimedia_commons_url
 
+    def __hash__(self) -> int:
+        return hash(
+            (self.path, self.media_type, self.title, self.wikimedia_commons_url)
+        )
+
     @property
     def path(self) -> Path:
         return self._path
 
     @property
     def media_type(self) -> MediaType:
         return self._media_type
@@ -180,21 +206,17 @@
         )
         return self._binary_file_cache.cache_item_file_path(cache_item_id)
 
 
 class _Retriever:
     def __init__(
         self,
-        http_client: aiohttp.ClientSession,
-        cache: Cache[str],
-        binary_file_cache: BinaryFileCache,
-        # Default to seven days.
-        ttl: int = 86400 * 7,
+        fetcher: _Fetcher,
     ):
-        self._fetcher = _Fetcher(http_client, cache, binary_file_cache, ttl)
+        self._fetcher = fetcher
         self._images: dict[str, Image | None] = {}
 
     async def _get_query_api_data(self, url: str) -> dict[str, Any]:
         response_data = await self._fetcher.fetch(url)
         api_data = json.loads(response_data)
         try:
             return api_data["query"]["pages"][0]  # type: ignore[no-any-return]
@@ -217,69 +239,74 @@
             api_data = await self._get_page_query_api_data(page_language, page_name)
         except RetrievalError as error:
             logger = logging.getLogger(__name__)
             logger.warning(str(error))
             return {}
         try:
             translations_data = api_data["langlinks"]
-        except KeyError:
+        except LookupError:
             # There may not be any translations.
             return {}
         return {
             translation_data["lang"]: translation_data["title"]
             for translation_data in translations_data
         }
 
     async def get_summary(self, page_language: str, page_name: str) -> Summary | None:
-        logger = logging.getLogger(__name__)
         try:
             url = f"https://{page_language}.wikipedia.org/api/rest_v1/page/summary/{page_name}"
             response_data = await self._fetcher.fetch(url)
             try:
                 api_data = json.loads(response_data)
-                return Summary(
-                    page_language,
-                    page_name,
-                    api_data["titles"]["normalized"],
-                    (
-                        api_data["extract_html"]
-                        if "extract_html" in api_data
-                        else api_data["extract"]
-                    ),
-                )
-            except (json.JSONDecodeError, KeyError) as error:
+            except json.JSONDecodeError as error:
                 raise RetrievalError(
                     f"Could not successfully parse the JSON content returned by {url}: {error}"
                 )
+            else:
+                try:
+                    return Summary(
+                        page_language,
+                        page_name,
+                        api_data["titles"]["normalized"],
+                        (
+                            api_data["extract_html"]
+                            if "extract_html" in api_data
+                            else api_data["extract"]
+                        ),
+                    )
+                except LookupError as error:
+                    raise RetrievalError(
+                        f"Could not successfully parse the JSON content returned by {url}: {error}"
+                    )
         except RetrievalError as error:
+            logger = logging.getLogger(__name__)
             logger.warning(str(error))
-        return None
+            return None
 
     async def get_image(self, page_language: str, page_name: str) -> Image | None:
         try:
             api_data = await self._get_page_query_api_data(page_language, page_name)
             try:
                 page_image_name = api_data["pageimage"]
-            except KeyError:
+            except LookupError:
                 # There may not be any images.
                 return None
 
             if page_image_name in self._images:
                 return self._images[page_image_name]
 
             url = f"https://en.wikipedia.org/w/api.php?action=query&prop=imageinfo&titles=File:{quote(page_image_name)}&iiprop=url|mime|canonicaltitle&format=json&formatversion=2"
             image_info_api_data = await self._get_query_api_data(url)
 
             try:
                 image_info = image_info_api_data["imageinfo"][0]
-            except KeyError as error:
+            except LookupError as error:
                 raise RetrievalError(
                     f"Could not successfully parse the JSON content returned by {url}: {error}"
                 )
-
             image = Image(
                 await self._fetcher.fetch_file(image_info["url"]),
                 MediaType(image_info["mime"]),
                 # Strip "File:" or any translated equivalent from the beginning of the image's title.
                 image_info["canonicaltitle"][
                     image_info["canonicaltitle"].index(":") + 1 :
                 ],
@@ -291,56 +318,63 @@
             logger = logging.getLogger(__name__)
             logger.warning(str(error))
             return None
 
     async def get_place_coordinates(
         self, page_language: str, page_name: str
     ) -> Point | None:
-        api_data = await self._get_page_query_api_data(page_language, page_name)
         try:
-            coordinates = api_data["coordinates"][0]
-        except KeyError:
-            # There may not be any coordinates.
-            return None
-        try:
-            if coordinates["globe"] != "earth":
+            api_data = await self._get_page_query_api_data(page_language, page_name)
+            try:
+                coordinates = api_data["coordinates"][0]
+            except LookupError:
+                # There may not be any coordinates.
                 return None
-            return Point(coordinates["lat"], coordinates["lon"])
-        except KeyError as error:
-            raise RetrievalError(
-                f"Could not successfully parse the JSON content: {error}"
-            )
+            try:
+                if coordinates["globe"] != "earth":
+                    return None
+                return Point(coordinates["lat"], coordinates["lon"])
+            except LookupError as error:
+                raise RetrievalError(
+                    f"Could not successfully parse the JSON content: {error}"
+                )
+        except RetrievalError as error:
+            logger = logging.getLogger(__name__)
+            logger.warning(str(error))
+            return None
 
 
 class _Populator:
     def __init__(self, app: App, retriever: _Retriever):
         self._app = app
         self._retriever = retriever
-        self._image_files: dict[Image, File] = {}
+        self._image_files: MutableMapping[Image, File] = {}
+        self._image_files_locks: Mapping[Image, _Lock] = defaultdict(
+            AsynchronizedLock.threading
+        )
 
     async def populate(self) -> None:
         locales = list(
             map(lambda x: x.alias, self._app.project.configuration.locales.values())
         )
         await gather(
             *(
                 self._populate_entity(entity, locales)
                 for entity in self._app.project.ancestry
                 if isinstance(entity, HasLinks)
             )
         )
 
     async def _populate_entity(self, entity: HasLinks, locales: Sequence[str]) -> None:
-        await self._populate_has_links(entity, locales)
-
+        populations = [self._populate_has_links(entity, locales)]
         if isinstance(entity, HasFiles):
-            await self._populate_has_files(entity)
-
+            populations.append(self._populate_has_files(entity))
         if isinstance(entity, Place):
-            await self._populate_place(entity)
+            populations.append(self._populate_place(entity))
+        await gather(*populations)
 
     async def _populate_has_links(
         self, has_links: HasLinks, locales: Sequence[str]
     ) -> None:
         summary_links: MutableSequence[tuple[str, str]] = []
         for link in has_links.links:
             try:
@@ -424,68 +458,81 @@
         if summary is not None and link.label is None:
             link.label = summary.title
 
     async def _populate_place(self, place: Place) -> None:
         await self._populate_place_coordinates(place)
 
     async def _populate_place_coordinates(self, place: Place) -> None:
-        if place.coordinates:
-            return
+        await gather(
+            *(
+                self._populate_place_coordinates_link(place, link)
+                for link in place.links
+            )
+        )
 
-        for link in place.links:
-            try:
-                page_language, page_name = _parse_url(link.url)
-            except NotAPageError:
-                continue
-            else:
-                coordinates = await self._retriever.get_place_coordinates(
-                    page_language, page_name
-                )
-                if coordinates:
-                    place.coordinates = coordinates
-                    return
+    async def _populate_place_coordinates_link(self, place: Place, link: Link) -> None:
+        try:
+            page_language, page_name = _parse_url(link.url)
+        except NotAPageError:
+            return
+        else:
+            coordinates = await self._retriever.get_place_coordinates(
+                page_language, page_name
+            )
+            if coordinates:
+                place.coordinates = coordinates
 
     async def _populate_has_files(self, has_files: HasFiles & HasLinks) -> None:
-        for link in has_files.links:
-            try:
-                page_language, page_name = _parse_url(link.url)
-            except NotAPageError:
-                continue
-            else:
-                image = await self._retriever.get_image(page_language, page_name)
-                if not image:
-                    continue
+        await gather(
+            *(
+                self._populate_has_files_link(has_files, link)
+                for link in has_files.links
+            )
+        )
 
-                try:
-                    file = self._image_files[image]
-                except KeyError:
-                    links = []
-                    for (
-                        locale_configuration
-                    ) in self._app.project.configuration.locales.values():
-                        localizer = await self._app.localizers.get(
-                            locale_configuration.locale
-                        )
-                        links.append(
-                            Link(
-                                f"{image.wikimedia_commons_url}?uselang={locale_configuration.alias}",
-                                label=localizer._(
-                                    "Description, licensing, and image history"
-                                ),
-                                description=localizer._(
-                                    "Find out more about this image on Wikimedia Commons."
-                                ),
-                                locale=locale_configuration.locale,
-                                media_type=MediaType("text/html"),
-                            )
+    async def _populate_has_files_link(
+        self, has_files: HasFiles & HasLinks, link: Link
+    ) -> None:
+        try:
+            page_language, page_name = _parse_url(link.url)
+        except NotAPageError:
+            return
+        else:
+            image = await self._retriever.get_image(page_language, page_name)
+            if not image:
+                return
+            has_files.files.add(await self._image_file(image))
+
+    async def _image_file(self, image: Image) -> File:
+        async with self._image_files_locks[image]:
+            try:
+                return self._image_files[image]
+            except KeyError:
+                links = []
+                for (
+                    locale_configuration
+                ) in self._app.project.configuration.locales.values():
+                    localizer = await self._app.localizers.get(
+                        locale_configuration.locale
+                    )
+                    links.append(
+                        Link(
+                            f"{image.wikimedia_commons_url}?uselang={locale_configuration.alias}",
+                            label=localizer._(
+                                "Description, licensing, and image history"
+                            ),
+                            description=localizer._(
+                                "Find out more about this image on Wikimedia Commons."
+                            ),
+                            locale=locale_configuration.locale,
+                            media_type=MediaType("text/html"),
                         )
-                    file = File(
-                        id=f"wikipedia-{image.title}",
-                        path=image.path,
-                        media_type=image.media_type,
-                        links=links,
                     )
-                    self._image_files[image] = file
-
-                has_files.files.add(file)
+                file = File(
+                    id=f"wikipedia-{image.title}",
+                    path=image.path,
+                    media_type=image.media_type,
+                    links=links,
+                )
+                self._image_files[image] = file
                 self._app.project.ancestry.add(file)
-                return
+                return file
```

### Comparing `betty-0.3.4/betty.egg-info/PKG-INFO` & `betty-0.3.5/betty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.3.4
+Version: 0.3.5
 Summary: Betty helps you visualize and publish your family history by building interactive genealogy websites out of your Gramps and GECOM family trees
 Author-email: Bart Feenstra <bar@bartfeenstra.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,25 +695,23 @@
 Requires-Dist: html5lib~=1.1; extra == "test"
 Requires-Dist: lxml~=5.0; sys_platform != "win32" and extra == "test"
 Requires-Dist: pip-licenses>=4.3.0,~=4.3; extra == "test"
 Requires-Dist: pydocstyle>=6.3.0,~=6.3; extra == "test"
 Requires-Dist: pytest>=7.3.1,~=7.3; extra == "test"
 Requires-Dist: pytest-aioresponses>=0.2.0,~=0.2; extra == "test"
 Requires-Dist: pytest-asyncio>=0.23.4,~=0.23; extra == "test"
-Requires-Dist: pytest-cov~=5.0; extra == "test"
 Requires-Dist: pytest-mock>=3.10.0,~=3.10; extra == "test"
 Requires-Dist: pytest-qt>=4.2.0,~=4.2; extra == "test"
 Requires-Dist: pytest-xvfb>=3.0.0,~=3.0; extra == "test"
 Requires-Dist: types-aiofiles>=23.2.0.20240403,~=23.2; extra == "test"
 Requires-Dist: types-babel>=2.11.0.15,~=2.11; extra == "test"
 Requires-Dist: types-click>=7.1.8,~=7.1; extra == "test"
 Requires-Dist: types-html5lib>=1.1.11.20240228,~=1.1; extra == "test"
 Requires-Dist: types-jsonschema>=4.21.0.20240331,~=4.21; extra == "test"
 Requires-Dist: types-lxml>=2024.3.27; extra == "test"
-Requires-Dist: types-mock>=5.0.0.6,~=5.0; extra == "test"
 Requires-Dist: types-polib>=1.2.0.0,~=1.2; extra == "test"
 Requires-Dist: types-pyinstaller>=6.5.0.20240311,~=6.5; extra == "test"
 Requires-Dist: types-pyyaml>=6.0.6,~=6.0; extra == "test"
 Requires-Dist: types-requests>=2.29.0.0,~=2.29; extra == "test"
 Requires-Dist: types-setuptools~=69.0; extra == "test"
 Requires-Dist: virtualenv~=20.26; extra == "test"
 Requires-Dist: betty[pyinstaller]; extra == "test"
```

### Comparing `betty-0.3.4/betty.egg-info/SOURCES.txt` & `betty-0.3.5/betty.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 betty.egg-info/SOURCES.txt
 betty.egg-info/dependency_links.txt
 betty.egg-info/entry_points.txt
 betty.egg-info/requires.txt
 betty.egg-info/top_level.txt
 betty/../.browserslistrc
 betty/../tsconfig.json
+betty/_package/__init__.py
 betty/_package/pyinstaller/__init__.py
 betty/_package/pyinstaller/main.py
 betty/_package/pyinstaller/hooks/__init__.py
 betty/_package/pyinstaller/hooks/hook-betty.py
 betty/app/__init__.py
 betty/app/extension/__init__.py
 betty/app/extension/requirement.py
@@ -180,15 +181,18 @@
 betty/extension/maps/__init__.py
 betty/extension/maps/webpack/main.css
 betty/extension/maps/webpack/main.ts
 betty/extension/maps/webpack/maps.js
 betty/extension/maps/webpack/package.json
 betty/extension/nginx/__init__.py
 betty/extension/nginx/artifact.py
+betty/extension/nginx/cli.py
+betty/extension/nginx/config.py
 betty/extension/nginx/docker.py
+betty/extension/nginx/gui.py
 betty/extension/nginx/serve.py
 betty/extension/nginx/assets/Dockerfile
 betty/extension/nginx/assets/content_negotiation.lua
 betty/extension/nginx/assets/nginx.conf.j2
 betty/extension/privatizer/__init__.py
 betty/extension/trees/__init__.py
 betty/extension/trees/assets/public/localized/people.json.j2
@@ -200,14 +204,16 @@
 betty/extension/webpack/build.py
 betty/extension/webpack/assets/templates/webpack-entry-loader.html.j2
 betty/extension/webpack/jinja2/__init__.py
 betty/extension/webpack/jinja2/filter.py
 betty/extension/webpack/webpack/package.json
 betty/extension/webpack/webpack/webpack.config.js
 betty/extension/wikipedia/__init__.py
+betty/extension/wikipedia/config.py
+betty/extension/wikipedia/gui.py
 betty/extension/wikipedia/assets/templates/wikipedia.html.j2
 betty/gramps/__init__.py
 betty/gramps/error.py
 betty/gramps/loader.py
 betty/gui/__init__.py
 betty/gui/app.py
 betty/gui/error.py
@@ -231,8 +237,9 @@
 betty/serde/dump.py
 betty/serde/error.py
 betty/serde/format.py
 betty/serde/load.py
 betty/sphinx/__init__.py
 betty/sphinx/extension/__init__.py
 betty/sphinx/extension/replacements.py
-documentation/conf.py
+documentation/conf.py
+site/sitecustomize.py
```

### Comparing `betty-0.3.4/betty.egg-info/entry_points.txt` & `betty-0.3.5/betty.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/betty.egg-info/requires.txt` & `betty-0.3.5/betty.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -45,25 +45,23 @@
 flake8-bugbear~=24.4
 html5lib~=1.1
 pip-licenses>=4.3.0,~=4.3
 pydocstyle>=6.3.0,~=6.3
 pytest>=7.3.1,~=7.3
 pytest-aioresponses>=0.2.0,~=0.2
 pytest-asyncio>=0.23.4,~=0.23
-pytest-cov~=5.0
 pytest-mock>=3.10.0,~=3.10
 pytest-qt>=4.2.0,~=4.2
 pytest-xvfb>=3.0.0,~=3.0
 types-aiofiles>=23.2.0.20240403,~=23.2
 types-babel>=2.11.0.15,~=2.11
 types-click>=7.1.8,~=7.1
 types-html5lib>=1.1.11.20240228,~=1.1
 types-jsonschema>=4.21.0.20240331,~=4.21
 types-lxml>=2024.3.27
-types-mock>=5.0.0.6,~=5.0
 types-polib>=1.2.0.0,~=1.2
 types-pyinstaller>=6.5.0.20240311,~=6.5
 types-pyyaml>=6.0.6,~=6.0
 types-requests>=2.29.0.0,~=2.29
 types-setuptools~=69.0
 virtualenv~=20.26
 betty[pyinstaller]
```

### Comparing `betty-0.3.4/documentation/conf.py` & `betty-0.3.5/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `betty-0.3.4/pyproject.toml` & `betty-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -107,25 +107,23 @@
     'html5lib ~= 1.1',
     'lxml ~= 5.0; sys.platform != "win32"',
     'pip-licenses ~= 4.3, >= 4.3.0',
     'pydocstyle ~= 6.3, >= 6.3.0',
     'pytest ~= 7.3, >= 7.3.1',
     'pytest-aioresponses ~= 0.2, >= 0.2.0 ',
     'pytest-asyncio ~= 0.23, >= 0.23.4 ',
-    'pytest-cov ~= 5.0',
     'pytest-mock ~= 3.10, >= 3.10.0',
     'pytest-qt ~= 4.2, >= 4.2.0',
     'pytest-xvfb ~= 3.0, >= 3.0.0',
     'types-aiofiles ~= 23.2, >= 23.2.0.20240403 ',
     'types-babel ~= 2.11, >= 2.11.0.15',
     'types-click ~= 7.1, >= 7.1.8',
     'types-html5lib ~= 1.1, >= 1.1.11.20240228',
     'types-jsonschema ~= 4.21, >= 4.21.0.20240331',
     'types-lxml >= 2024.3.27 ',
-    'types-mock ~= 5.0, >= 5.0.0.6',
     'types-polib ~= 1.2, >= 1.2.0.0',
     'types-pyinstaller ~= 6.5, >= 6.5.0.20240311',
     'types-pyyaml ~= 6.0, >= 6.0.6',
     'types-requests ~= 2.29, >= 2.29.0.0',
     'types-setuptools ~= 69.0',
     'virtualenv ~= 20.26',
     'betty[pyinstaller]',
```

