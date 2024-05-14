# Comparing `tmp/nautiluszim-1.1.1.tar.gz` & `tmp/nautiluszim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautiluszim-1.1.1.tar", last modified: Fri May  5 15:50:05 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nautiluszim-1.1.1.tar` & `nautiluszim-1.2.0.tar`

### file list

```diff
@@ -1,588 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/locale/messages.pot
--rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.633405 nautiluszim-1.1.1/nautiluszim/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/database.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/display_rows.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/info-circle-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/init.js
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/main-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/media_player.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/modal_empty_body.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/modal_title.handlebars
--rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/nautilus.js
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim/templates/precompiled.js
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/nautiluszim/templates/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.633405 nautiluszim-1.1.1/nautiluszim/templates/vendors/
--rw-r--r--   0 runner    (1001) docker     (123)    17430 2020-05-04 16:04:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ScrollMagic.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.637405 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    67871 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)   157964 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    50935 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   115021 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)    77346 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32546 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   197170 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   504418 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   159515 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   641867 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.637405 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   227980 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   410007 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    80698 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   318045 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   135079 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)   256099 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    60010 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   194435 2019-11-28 12:59:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.681405 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2018-08-05 19:09:20.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/3g2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/3ga.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/3gp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/7z.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aa.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aac.svg
--rw-r--r--   0 runner    (1001) docker     (123)      555 2018-08-04 18:46:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ac.svg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/accdb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/accdt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      982 2018-08-05 18:47:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/adn.svg
--rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ai.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aif.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aifc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aiff.svg
--rw-r--r--   0 runner    (1001) docker     (123)      515 2018-06-30 00:55:16.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ait.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/amr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2018-06-23 16:58:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ani.svg
--rw-r--r--   0 runner    (1001) docker     (123)      829 2018-06-23 17:59:22.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/apk.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/app.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2018-08-04 19:09:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/applescript.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asax.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ascx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ashx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asmx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      730 2018-07-28 14:27:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aspx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/asx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/au.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-08-05 04:08:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/avi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/axd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-24 12:27:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/aze.svg
--rw-r--r--   0 runner    (1001) docker     (123)      309 2018-06-24 12:59:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bak.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bash.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/blank.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bmp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2018-08-05 17:23:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bowerrc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-06-24 17:12:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/browser.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/bz2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      407 2018-06-30 00:29:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/c.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cad.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/caf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2018-06-29 23:33:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2018-08-05 20:11:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      596 2018-07-27 01:55:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cfml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 03:33:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cgi.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2018-07-28 15:17:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/class.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cmd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2018-08-04 16:34:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/codekit.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2018-08-04 23:31:11.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/coffee.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/coffeelintignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/com.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2018-06-24 16:56:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/compile.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2018-08-05 17:39:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/conf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/config.svg
--rw-r--r--   0 runner    (1001) docker     (123)      583 2018-06-30 00:30:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cpp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      675 2018-07-27 01:50:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cptx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cr2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2018-07-21 22:39:54.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crdownload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-07-16 05:46:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/crypt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      655 2018-06-30 00:30:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2018-08-04 23:32:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cson.svg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csproj.svg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2018-06-29 21:26:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/css.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/csv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2018-07-16 05:44:20.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/cue.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2018-06-24 11:19:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dat.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-08-05 04:11:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/db.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dbf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/deb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dgn.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2018-07-21 20:21:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/diz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dll.svg
--rw-r--r--   0 runner    (1001) docker     (123)      615 2018-08-04 14:05:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dmg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dng.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/doc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:50.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/docb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/docm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-08-05 04:11:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/docx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dotm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      319 2018-06-19 06:59:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dotx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      740 2018-07-22 03:47:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:35:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dpj.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2018-06-30 18:59:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ds_store.svg
--rw-r--r--   0 runner    (1001) docker     (123)      555 2018-07-18 23:08:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dtd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dwg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/dxf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2018-08-04 20:17:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/editorconfig.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:16:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/el.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/enc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-07-28 16:31:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/epub.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/eslintignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2018-06-23 17:59:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/exe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/f4v.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2018-07-18 23:43:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fax.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fb2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      343 2018-06-23 16:11:22.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/fla.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/flac.svg
--rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/flv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 2018-08-05 19:39:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2018-06-24 13:07:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gadget.svg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2018-08-04 20:28:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gdp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2018-06-30 04:29:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gem.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gif.svg
--rw-r--r--   0 runner    (1001) docker     (123)      694 2018-08-04 20:41:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gitattributes.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gitignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2018-07-16 05:26:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/go.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-08-05 19:40:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/gz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 2018-07-19 02:16:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/h.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/handlebars.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2018-07-27 03:46:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/hbs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/heic.svg
--rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/hs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      416 2018-07-27 03:50:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/hsl.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/htm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      593 2018-06-29 21:25:38.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/html.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ibooks.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/icns.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2018-06-23 16:52:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ico.svg
--rw-r--r--   0 runner    (1001) docker     (123)      591 2018-06-29 23:32:36.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ics.svg
--rw-r--r--   0 runner    (1001) docker     (123)      644 2018-07-18 23:46:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/idx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/iff.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2018-08-05 17:40:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ifo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/img.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/in.svg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2018-06-23 16:06:20.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/indd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/inf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2018-07-17 22:31:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ini.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/iso.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2018-07-21 14:30:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/j2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jar.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:36:50.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/java.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jpe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2018-06-29 21:26:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/js.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2018-06-29 21:39:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2018-08-05 19:37:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jsp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2018-06-29 21:40:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/jsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/key.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kf8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2018-08-04 17:53:19.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kmk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ksh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2018-08-04 18:52:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/kup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2018-07-28 15:17:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/less.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/licx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2018-08-05 17:15:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lisp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2018-08-05 16:10:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lnk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 2018-06-24 16:25:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/log.svg
--rw-r--r--   0 runner    (1001) docker     (123)      465 2018-07-21 17:43:54.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/lua.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2018-08-05 17:33:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m2v.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m3u.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m3u8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2018-08-05 06:23:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4a.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4r.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/m4v.svg
--rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/map.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/master.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2018-07-21 18:59:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/md.svg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2018-08-05 18:46:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mdb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      307 2018-08-05 05:48:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/me.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/midi.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mkv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      482 2018-08-05 17:27:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2018-06-24 14:49:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mobi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mod.svg
--rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mov.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp3.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mp4.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpa.svg
--rw-r--r--   0 runner    (1001) docker     (123)      913 2018-07-18 23:59:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpe.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpga.svg
--rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      916 2018-07-18 23:55:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/mpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/msi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      514 2018-06-30 14:04:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/msu.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nef.svg
--rw-r--r--   0 runner    (1001) docker     (123)      589 2018-08-05 18:13:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nes.svg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2018-07-21 20:21:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nfo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-27 02:23:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/nix.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/npmignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2018-07-19 00:19:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      671 2018-06-23 11:58:54.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ods.svg
--rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/odt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ogg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ogv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ost.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/otf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      741 2018-07-19 02:37:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ott.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ova.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ovf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/p12.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/p7b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2018-07-19 02:45:38.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pages.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2018-07-19 02:50:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/part.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pcd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pdb.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2018-06-19 08:11:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pem.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pfx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      478 2018-06-24 19:11:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pgp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ph.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2018-06-30 18:08:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/phar.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2018-06-29 22:06:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/php.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pkg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2018-06-30 11:23:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pl.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2018-08-04 20:04:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/plist.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2018-06-30 11:22:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/png.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/po.svg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2018-07-21 17:42:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pom.svg
--rw-r--r--   0 runner    (1001) docker     (123)      545 2018-07-19 02:56:21.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/potx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pps.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ppsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ppt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pptm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 2018-06-19 10:03:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pptx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 2018-06-19 09:52:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/prop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2018-07-21 21:37:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ps1.svg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2018-06-23 16:13:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/psd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/psp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2018-07-19 00:11:29.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pst.svg
--rw-r--r--   0 runner    (1001) docker     (123)      627 2018-07-19 00:02:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pub.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2018-06-24 17:07:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/py.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2018-07-16 05:23:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/pyc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      665 2018-06-30 03:56:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/qt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ra.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ram.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rar.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/raw.svg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-06-23 18:18:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/resx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2018-07-28 14:56:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/retry.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2018-08-05 16:36:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rom.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rpm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2018-06-24 16:28:18.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rsa.svg
--rw-r--r--   0 runner    (1001) docker     (123)      668 2018-08-05 04:06:37.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rss.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rtf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      926 2018-07-27 04:19:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ru.svg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2018-06-24 14:07:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/rub.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sass.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2018-06-24 19:05:14.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/scss.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2018-08-05 18:23:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sed.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      791 2018-08-05 05:46:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sitemap.svg
--rw-r--r--   0 runner    (1001) docker     (123)      905 2018-07-28 16:28:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/skin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sldm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2018-08-05 19:09:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sldx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      906 2018-07-28 15:15:35.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sln.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2018-07-21 18:47:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sol.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2018-06-23 16:42:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sql.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2018-08-05 19:02:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sqlite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/step.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2018-06-30 04:01:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/stl.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2018-08-05 17:36:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      558 2018-07-28 14:46:24.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      847 2018-06-30 12:16:27.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/swift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2018-08-05 19:41:27.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/sys.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tar.svg
--rw-r--r--   0 runner    (1001) docker     (123)      304 2018-06-30 00:57:52.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tcsh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 2018-06-23 18:15:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tfignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tga.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tgz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tif.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tiff.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2018-08-05 03:53:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tmp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      979 2018-06-30 03:47:11.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/torrent.svg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2018-08-04 17:10:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ts.svg
--rw-r--r--   0 runner    (1001) docker     (123)      429 2018-07-18 23:02:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/tsv.svg
--rw-r--r--   0 runner    (1001) docker     (123)      807 2018-08-04 16:11:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/ttf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      358 2018-07-27 01:37:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/twig.svg
--rw-r--r--   0 runner    (1001) docker     (123)      287 2018-06-19 09:38:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/txt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/udf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      555 2018-06-30 00:51:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vb.svg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2018-06-24 13:12:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vbproj.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2018-08-05 18:09:55.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vbs.svg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2018-06-23 17:49:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vcd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      453 2018-06-24 19:18:25.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vcs.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vdx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2018-07-17 22:38:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vmdk.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vob.svg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2018-07-16 04:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vscodeignore.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vsd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vss.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vst.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      845 2018-06-30 19:13:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/vtx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2018-08-05 19:36:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/war.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wav.svg
--rw-r--r--   0 runner    (1001) docker     (123)      716 2018-08-05 03:42:49.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wbk.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2018-08-05 19:41:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/webinfo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/webm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2018-06-19 09:52:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/webp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      531 2018-06-22 22:20:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wma.svg
--rw-r--r--   0 runner    (1001) docker     (123)      518 2018-06-30 04:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wmf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2018-06-22 22:03:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wmv.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/woff.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2018-06-30 04:23:07.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/woff2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      685 2018-06-30 14:11:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wps.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/wsf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2018-07-22 02:04:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xcf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xls.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlsm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlsx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xlt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xltm.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-06-19 07:21:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xltx.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-07-26 04:04:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      722 2018-07-22 03:42:57.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xpi.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xps.svg
--rw-r--r--   0 runner    (1001) docker     (123)      517 2018-06-29 23:06:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xrb.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2018-07-28 19:17:51.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xsd.svg
--rw-r--r--   0 runner    (1001) docker     (123)      400 2018-06-24 17:31:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xsl.svg
--rw-r--r--   0 runner    (1001) docker     (123)      839 2018-06-24 12:06:00.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xspf.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/xz.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2018-07-17 22:25:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/yml.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/z.svg
--rw-r--r--   0 runner    (1001) docker     (123)      703 2018-06-23 15:40:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/zip.svg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2018-06-23 18:48:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ext-icons/zsh.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20696 2021-02-15 09:49:41.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/handlebars.runtime.min-v4.7.7.js
--rw-r--r--   0 runner    (1001) docker     (123)    88145 2022-02-16 10:50:39.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.689405 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2019-03-12 21:12:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2019-03-12 21:13:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-dav1d.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2019-03-12 21:13:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-ogg.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-opus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-theora.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/COPYING-vorbis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2019-03-12 21:13:31.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/LICENSE-nestegg.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/LICENSE-vpx.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2019-03-12 21:13:32.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/PATENTS-vpx.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2019-06-18 15:00:08.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/dynamicaudio.swf
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2019-06-18 15:06:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   133919 2019-06-18 15:06:14.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   235857 2019-06-18 15:06:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-opus.js
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2019-06-18 15:05:09.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   136930 2019-06-18 15:05:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   244171 2019-06-18 15:05:03.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-audio-vorbis.js
--rw-r--r--   0 runner    (1001) docker     (123)    66341 2019-06-18 15:09:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   120118 2019-06-18 15:09:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.js.mem
--rw-r--r--   0 runner    (1001) docker     (123)   337274 2019-06-18 15:09:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:56.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-mt-wasm.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)    11462 2019-06-18 15:09:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   435089 2019-06-18 15:09:02.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   934028 2019-06-18 15:08:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-av1.js
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2019-06-18 15:07:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    62814 2019-06-18 15:07:01.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   128000 2019-06-18 15:06:59.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-theora.js
--rw-r--r--   0 runner    (1001) docker     (123)    67131 2019-06-18 15:09:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2019-06-18 15:09:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.js.mem
--rw-r--r--   0 runner    (1001) docker     (123)   143573 2019-06-18 15:09:44.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:42.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-mt-wasm.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2019-06-18 15:08:15.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   123379 2019-06-18 15:08:12.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   260845 2019-06-18 15:08:10.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp8.js
--rw-r--r--   0 runner    (1001) docker     (123)    64871 2019-06-18 15:09:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    32370 2019-06-18 15:09:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.js.mem
--rw-r--r--   0 runner    (1001) docker     (123)   223005 2019-06-18 15:09:48.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2019-06-18 15:09:46.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-mt-wasm.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2019-06-18 15:08:40.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)   238580 2019-06-18 15:08:36.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   465673 2019-06-18 15:08:34.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-decoder-video-vp9.js
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2019-06-18 15:03:36.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    59932 2019-06-18 15:03:33.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   171551 2019-06-18 15:03:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-ogg.js
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2019-06-18 15:04:17.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.js
--rw-r--r--   0 runner    (1001) docker     (123)    48118 2019-06-18 15:04:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm-wasm.wasm
--rw-r--r--   0 runner    (1001) docker     (123)   122752 2019-06-18 15:04:11.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-demuxer-webm.js
--rw-r--r--   0 runner    (1001) docker     (123)   140564 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-es2017.js
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-support.js
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2019-06-18 15:01:27.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-version.js
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2019-06-18 15:01:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-worker-audio.js
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2019-06-18 15:01:28.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv-worker-video.js
--rw-r--r--   0 runner    (1001) docker     (123)   148482 2019-06-18 15:01:30.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/ogvjs/ogv.js
--rw-r--r--   0 runner    (1001) docker     (123)    59078 2023-05-05 15:50:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/pouchdb.find.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   125540 2023-05-05 15:50:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/pouchdb.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    68850 2023-05-05 15:50:04.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/sugar.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.697405 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.697405 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/
--rwxr-xr-x   0 runner    (1001) docker     (123)    28407 2019-08-28 19:46:06.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7080 2019-08-28 19:46:06.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)     4324 2019-08-28 19:46:06.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/font/VideoJS.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ar.js
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ar.json
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ba.js
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ba.json
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/bg.js
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/bg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ca.json
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cs.js
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cs.json
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cy.js
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/cy.json
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/da.js
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/da.json
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/de.js
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/de.json
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/el.js
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/el.json
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/en.js
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/es.js
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/es.json
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fa.json
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fi.js
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fr.js
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/fr.json
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gd.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gd.json
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gl.js
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/gl.json
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/he.js
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/he.json
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hr.js
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hu.js
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/hu.json
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/it.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/it.json
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ja.js
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ja.json
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ko.js
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ko.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nb.js
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nb.json
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nl.js
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nl.json
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nn.js
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/nn.json
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/oc.js
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/oc.json
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pl.js
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pl.json
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-BR.json
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-PT.js
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/pt-PT.json
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ru.js
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/ru.json
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sk.js
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sk.json
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sr.js
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sr.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sv.js
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/sv.json
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/tr.js
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/tr.json
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/uk.js
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/uk.json
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/vi.js
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/vi.json
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-CN.js
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-CN.json
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hans.js
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hans.json
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hant.js
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-Hant.json
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-TW.js
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2019-08-28 19:45:47.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/lang/zh-TW.json
--rw-r--r--   0 runner    (1001) docker     (123)    45293 2019-08-28 19:45:45.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video-js.css
--rw-r--r--   0 runner    (1001) docker     (123)    40028 2019-08-28 19:46:05.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video-js.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1361043 2019-08-28 19:45:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.cjs.js
--rw-r--r--   0 runner    (1001) docker     (123)  1360644 2019-08-28 19:45:26.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.es.js
--rw-r--r--   0 runner    (1001) docker     (123)  1797606 2019-08-28 19:45:23.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.js
--rw-r--r--   0 runner    (1001) docker     (123)   480256 2019-08-28 19:45:58.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs/video.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2016-10-14 10:25:13.000000 nautiluszim-1.1.1/nautiluszim/templates/vendors/videojs-ogvjs.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:50:05.629405 nautiluszim-1.1.1/nautiluszim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 15:50:05.000000 nautiluszim-1.1.1/nautiluszim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:50:05.705405 nautiluszim-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-05 15:49:48.000000 nautiluszim-1.1.1/setup.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/Dockerfile
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/openzim.toml
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/tasks.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/VERSION
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/__init__.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/constants.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/entrypoint.py
+-rw-r--r--   0        0        0    20684 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/scraper.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/locale/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/database.js
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/display_rows.handlebars
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/favicon.png
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/home.html
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/info-circle-solid.svg
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/init.js
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/main-logo.png
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/media_player.handlebars
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/modal_empty_body.handlebars
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/modal_title.handlebars
+-rw-r--r--   0        0        0    19903 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/nautilus.js
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/src/nautiluszim/templates/styles.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/tests/test_stub.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/README.md
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 nautiluszim-1.2.0/PKG-INFO
```

### Comparing `nautiluszim-1.1.1/LICENSE` & `nautiluszim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.1/PKG-INFO` & `nautiluszim-1.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,19 @@
-Metadata-Version: 2.1
-Name: nautiluszim
-Version: 1.1.1
-Summary: turns a collection of documents into a browsable ZIM file
-Home-page: https://github.com/openzim/nautilus
-Author: kiwix
-Author-email: reg@kiwix.org
-License: GPLv3+
-Keywords: kiwix zim offline
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
-Nautilus
-=============
+# Nautilus
+
+`nautilus` turns a collection of documents into a browsable [ZIM file](https://openzim.org).
 
 [![CodeFactor](https://www.codefactor.io/repository/github/openzim/nautilus/badge)](https://www.codefactor.io/repository/github/openzim/nautilus)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![codecov](https://codecov.io/gh/openzim/nautilus/branch/main/graph/badge.svg)](https://codecov.io/gh/openzim/nautilus)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/nautiluszim/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nautiluszim.svg)](https://pypi.org/project/nautiluszim)
 [![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/latest_tag?label=docker)](https://ghcr.io/openzim/nautilus)
 
-`nautilus` turns a collection of documents into a browsable [ZIM file](https://openzim.org).
-
 It downloads the video (webm or mp4 format – optionally recompress it in lower-quality, smaller size), the thumbnails, the subtitles and the authors' profile pictures ; then, it creates a static HTML files folder of it before creating a ZIM off of it.
 
 # Preparing the archive
 
 To be used with nautilus, your archive should be a ZIP file.
 * it doesn't need to be structured, but it can.
 * it doesn't need to be compressed. It's usually recommended not to.
@@ -51,69 +31,79 @@
 Either inside the archive ZIP as `/collection.json` or elsewhere, 
 specified via `--collection mycollection.json`, you must supply a JSON file describing your content.
 
 The user-interface only gives access to files referenced properly in the collection.
 
 At the moment, the JSON file needs to provide the following fields for each item in an array:
 
-``` JSON
+```json
 [
     {
         "title": "...",
         "description": "...",
         "authors": "...",
         "files": ["relative/path/to/file"]
-     }
+    },
+    {
+        "title": "...",
+        "description": "...",
+        "authors": "...",
+        "files": [
+            {
+                "archive-member": "01 BOOK for printing .pdf",  // optional, member name inside archive (same as simpler format)
+                "url": "http://books.com/310398120.pdf",  // optional, has precedence over `archive-member`, url to download file from
+                "filename": "My book.pdf",  // optional, filename to use in ZIM, regardless of original one
+            }
+        ]
+    }
 ]
 ```
 
 ## About page
 
 Either inside the archive ZIP as `/about.html` or elsewhere, specified via `--about myabout.html`,
 
 - You may supply an about page in HTML format. It will be displayed in a modal popup and will be included.
 - At its bottom your *secondary-logo* if provided.
 
 * Use only content tags (no `<html />` nor `<head />` nor `<script />` etc)
 * Use inline styling if required, but no styling is recommended.
 * Include one logo inline if required.
 
-# Requirements
+## Usage
 
-* `wget` and `unzip` to install JS dependencies. See `get_js_deps.sh` if you want to do it manually.
-* `wget` is used to download archive files as well.
-* [`handlebars`](https://handlebarsjs.com) is used to compile JS templates
+```sh
+❯ nautuluszim --help
+usage: nautuluszim [-h] [-V]
 
-# Installation
-
-`nautilus` is a python program. if you are not using the docker image, you are advised to use it in a virtual-environment. See `requirements.txt` for the list of python dependencies.
-
-## docker
+# everything bundled in a ZIP
+nautiluszim --archive my-content.zip
 
-```
-docker run -v my_dir:/output ghcr.io/openzim/nautilus nautiluszim --help
+# In this mode every file entry must have a valid url.
+nautiluszim --collection https://example.com/to-your-collection-file
 ```
 
-## pip
+### Installation
 
-```
-pip install nautiluszim
-nautiluszim --help
+You'd want to install it in a dedicated virtual-environment (`python3 -m venv some-env && source ./some-env/bin/activate`)
+
+```sh
+❯ pip install nautiluszim
 ```
 
-# Usage
+### Contributing
 
-```
-nautiluszim --archive my-content.zip
+```sh
+❯ pip install -e .
 ```
 
-## Notes
+#### Notes
 
 * On macOS, the locale setting is buggy. You need to launch it with the `LANGUAGE` environment variable (as ISO-639-1) for the translations to work.
 
 ```
 LANGUAGE=fr nautiluszim --language fra
 ```
 
-## Development
+Nautilus adheres to openZIM's [Contribution Guidelines](https://github.com/openzim/overview/wiki/Contributing).
 
-See [CONTRIBUTING.md](CONTRIBUTING.md)
+Nautilus has implemented openZIM's [Python bootstrap, conventions and policies](https://github.com/openzim/_python-bootstrap/docs/Policy.md) **v1.0.0**.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_jzze1irq_/tmp4hapkhhx_TarContainer/0/4", line 120, column 0: CDATA terminal not found*

```diff
@@ -1,43 +1,40 @@
-Metadata-Version: 2.1 Name: nautiluszim Version: 1.1.1 Summary: turns a
-collection of documents into a browsable ZIM file Home-page: https://
-github.com/openzim/nautilus Author: kiwix Author-email: reg@kiwix.org License:
-GPLv3+ Keywords: kiwix zim offline Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
-Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Python:
->=3.7 Description-Content-Type: text/markdown License-File: LICENSE Nautilus
-============= [![CodeFactor](https://www.codefactor.io/repository/github/
-openzim/nautilus/badge)](https://www.codefactor.io/repository/github/openzim/
-nautilus) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-
-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![PyPI version shields.io]
-(https://img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/
-nautiluszim/) [![Docker](https://ghcr-badge.deta.dev/openzim/nautilus/
-latest_tag?label=docker)](https://ghcr.io/openzim/nautilus) `nautilus` turns a
-collection of documents into a browsable [ZIM file](https://openzim.org). It
-downloads the video (webm or mp4 format â optionally recompress it in lower-
-quality, smaller size), the thumbnails, the subtitles and the authors' profile
-pictures ; then, it creates a static HTML files folder of it before creating a
-ZIM off of it. # Preparing the archive To be used with nautilus, your archive
-should be a ZIP file. * it doesn't need to be structured, but it can. * it
-doesn't need to be compressed. It's usually recommended not to. * it should
-contain a `collection.json` file, but it can also be provided separately (see
-below). * it should only contain to-be-included files. No filtering is done. *
-Audio and video files should be in ogg format with an `.ogg`/`.ogv` extension
-to be supported on all platforms (`mp3`/`mp4` would work only on platforms with
-native support). ``` cd content/path zip -r -0 -T ../content_name.zip * ``` ##
-JSON collection file Either inside the archive ZIP as `/collection.json` or
-elsewhere, specified via `--collection mycollection.json`, you must supply a
-JSON file describing your content. The user-interface only gives access to
-files referenced properly in the collection. At the moment, the JSON file needs
-to provide the following fields for each item in an array: ``` JSON [
-{ "title": "...", "description": "...", "authors": "...", "files": ["relative/
-path/to/file"] } ] ``` ## About page Either inside the archive ZIP as `/
-about.html` or elsewhere, specified via `--about myabout.html`, - You may
-supply an about page in HTML format. It will be displayed in a modal popup and
-will be included. - At its bottom your *secondary-logo* if provided. * Use only
-content tags (no `
+# Nautilus `nautilus` turns a collection of documents into a browsable [ZIM
+file](https://openzim.org). [![CodeFactor](https://www.codefactor.io/
+repository/github/openzim/nautilus/badge)](https://www.codefactor.io/
+repository/github/openzim/nautilus) [![License: GPL v3](https://img.shields.io/
+badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [!
+[codecov](https://codecov.io/gh/openzim/nautilus/branch/main/graph/badge.svg)]
+(https://codecov.io/gh/openzim/nautilus) [![PyPI version shields.io](https://
+img.shields.io/pypi/v/nautiluszim.svg)](https://pypi.org/project/nautiluszim/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
+nautiluszim.svg)](https://pypi.org/project/nautiluszim) [![Docker](https://
+ghcr-badge.deta.dev/openzim/nautilus/latest_tag?label=docker)](https://ghcr.io/
+openzim/nautilus) It downloads the video (webm or mp4 format â optionally
+recompress it in lower-quality, smaller size), the thumbnails, the subtitles
+and the authors' profile pictures ; then, it creates a static HTML files folder
+of it before creating a ZIM off of it. # Preparing the archive To be used with
+nautilus, your archive should be a ZIP file. * it doesn't need to be
+structured, but it can. * it doesn't need to be compressed. It's usually
+recommended not to. * it should contain a `collection.json` file, but it can
+also be provided separately (see below). * it should only contain to-be-
+included files. No filtering is done. * Audio and video files should be in ogg
+format with an `.ogg`/`.ogv` extension to be supported on all platforms (`mp3`/
+`mp4` would work only on platforms with native support). ``` cd content/path
+zip -r -0 -T ../content_name.zip * ``` ## JSON collection file Either inside
+the archive ZIP as `/collection.json` or elsewhere, specified via `--collection
+mycollection.json`, you must supply a JSON file describing your content. The
+user-interface only gives access to files referenced properly in the
+collection. At the moment, the JSON file needs to provide the following fields
+for each item in an array: ```json [ { "title": "...", "description": "...",
+"authors": "...", "files": ["relative/path/to/file"] }, { "title": "...",
+"description": "...", "authors": "...", "files": [ { "archive-member": "01 BOOK
+for printing .pdf", // optional, member name inside archive (same as simpler
+format) "url": "http://books.com/310398120.pdf", // optional, has precedence
+over `archive-member`, url to download file from "filename": "My book.pdf", /
+/ optional, filename to use in ZIM, regardless of original one } ] } ] ``` ##
+About page Either inside the archive ZIP as `/about.html` or elsewhere,
+specified via `--about myabout.html`, - You may supply an about page in HTML
+format. It will be displayed in a modal popup and will be included. - At its
+bottom your *secondary-logo* if provided. * Use only content tags (no `
 ` nor `
 ` nor `
```

### Comparing `nautiluszim-1.1.1/nautiluszim/constants.py` & `nautiluszim-1.2.0/src/nautiluszim/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# vim: ai ts=4 sts=4 et sw=4 nu
-
 import logging
 import pathlib
 
 from zimscraperlib.logging import getLogger as lib_getLogger
 
 ROOT_DIR = pathlib.Path(__file__).parent
 NAME = ROOT_DIR.name
 
-with open(ROOT_DIR.joinpath("VERSION"), "r") as fh:
+with open(ROOT_DIR.joinpath("VERSION")) as fh:
     VERSION = fh.read().strip()
 
 SCRAPER = f"{NAME} {VERSION}"
 
 
 class Global:
     debug = False
 
 
-def setDebug(debug):
+def set_debug(debug):
     """toggle constants global DEBUG flag (used by getLogger)"""
     Global.debug = bool(debug)
 
 
-def getLogger():
+def get_logger():
     """configured logger respecting DEBUG flag"""
     return lib_getLogger(NAME, level=logging.DEBUG if Global.debug else logging.INFO)
```

### Comparing `nautiluszim-1.1.1/nautiluszim/entrypoint.py` & `nautiluszim-1.2.0/src/nautiluszim/entrypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# vim: ai ts=4 sts=4 et sw=4 nu
-
 import argparse
 
-from .constants import NAME, SCRAPER, getLogger, setDebug
+from nautiluszim.constants import NAME, SCRAPER, get_logger, set_debug
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog=NAME,
         description="Create a ZIM file off a collection of file documents",
     )
 
     parser.add_argument(
         "--archive",
         help="Path or URL to a ZIP archive containing all the documents",
-        required=True,
+        required=False,
     )
     parser.add_argument(
         "--collection",
         help="Different collection JSON path or URL. "
-        "Otherwise using `collection.json` from archive",
+        + "Otherwise using `collection.json` from archive",
         required=False,
     )
     parser.add_argument(
         "--name",
         help="ZIM name. Used as identifier and filename (date will be appended)",
         required=True,
     )
@@ -77,21 +73,21 @@
         action="store_true",
         dest="keep_build_dir",
     )
 
     parser.add_argument(
         "--language",
         help="ISO-639-3 (3 chars) language code of content. "
-        "comma-separated if multiple ones",
+        + "comma-separated if multiple ones",
         default="eng",
     )
     parser.add_argument(
         "--locale",
         help="Locale name to use for translations (if avail) and time representations. "
-        "Defaults to (first) --language or English.",
+        + "Defaults to (first) --language or English.",
         dest="locale_name",
     )
     parser.add_argument(
         "--tags",
         help="List of comma-separated Tags for the ZIM file.",
         default="",
     )
@@ -115,61 +111,61 @@
     )
     parser.add_argument(
         "--publisher", help="Custom publisher name (ZIM metadata)", default="Kiwix"
     )
     parser.add_argument(
         "--favicon",
         help="Custom favicon. Will be resized to 48x48px. Nautilus one otherwise. "
-        "Also used as ZIM illustration",
+        + "Also used as ZIM illustration",
     )
     parser.add_argument(
         "--main-logo",
         help="Custom logo. Will be resized to 300x65px",
         dest="main_logo",
     )
     parser.add_argument(
         "--secondary-logo",
         help="Custom footer logo. Will be resized to 300x65px. None otherwise",
         dest="secondary_logo",
     )
     parser.add_argument(
         "--main-color",
         help="Custom header color. Hex/HTML syntax (#DEDEDE). "
-        "Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
+        + "Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
     )
     parser.add_argument(
         "--secondary-color",
         help="Custom secondary color. Hex/HTML syntax (#DEDEDE). "
-        "Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
+        + "Default to main-logo's primary color solarized (or #95A5A6 if no logo).",
     )
 
     parser.add_argument(
         "--about",
         help="Custom about HTML file. "
-        "Uses file `about.html` of archive if present otherwise.",
+        + "Uses file `about.html` of archive if present otherwise.",
     )
 
     parser.add_argument(
         "--version",
         help="Display scraper version and exit",
         action="version",
         version=SCRAPER,
     )
 
     args = parser.parse_args()
 
-    setDebug(args.debug)
-    logger = getLogger()
-    from .scraper import Nautilus
+    set_debug(args.debug)
+    logger = get_logger()
+    from nautiluszim.scraper import Nautilus
 
     try:
         scraper = Nautilus(**dict(args._get_kwargs()))
         scraper.run()
     except Exception as exc:
         logger.error(f"FAILED. An error occured: {exc}")
         if args.debug:
             logger.exception(exc)
-        raise SystemExit(1)
+        raise SystemExit(1) from exc
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `nautiluszim-1.1.1/nautiluszim/locale/fr/LC_MESSAGES/messages.po` & `nautiluszim-1.2.0/src/nautiluszim/locale/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.1/nautiluszim/scraper.py` & `nautiluszim-1.2.0/src/nautiluszim/scraper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,39 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# vim: ai ts=4 sts=4 et sw=4 nu
-
 import datetime
 import json
 import locale
 import os
 import pathlib
 import shutil
+import tempfile
 import unicodedata
 import uuid
 import zipfile
 from pathlib import Path
-from typing import Optional
 
 import jinja2
-from zimscraperlib.constants import (
-    MAXIMUM_DESCRIPTION_METADATA_LENGTH,
-    MAXIMUM_LONG_DESCRIPTION_METADATA_LENGTH,
-)
-from zimscraperlib.download import save_large_file
+from zimscraperlib.download import requests, save_large_file
 from zimscraperlib.i18n import _, get_language_details, setlocale
 from zimscraperlib.image.convertion import create_favicon
 from zimscraperlib.image.probing import get_colors, is_hex_color
 from zimscraperlib.image.transformation import resize_image
-from zimscraperlib.inputs import handle_user_provided_file
+from zimscraperlib.inputs import compute_descriptions, handle_user_provided_file
 from zimscraperlib.zim.creator import Creator
 
-from .constants import ROOT_DIR, SCRAPER, getLogger
+from nautiluszim.constants import ROOT_DIR, SCRAPER, get_logger
 
-logger = getLogger()
+logger = get_logger()
 
 
 def normalized_path(path: str) -> str:
     """ASCII version of a path for use in URL"""
     return unicodedata.normalize("NFKC", path)
 
 
-class Nautilus(object):
+class Nautilus:
     def __init__(
         self,
         archive,
         collection,
         nb_items_per_page,
         no_random,
         show_description,
@@ -104,15 +96,15 @@
             or get_language_details(self.language.split(",")[0])["iso-639-1"]
         )
         try:
             self.locale = setlocale(ROOT_DIR, locale_name)
         except locale.Error:
             logger.error(
                 f"No locale for {locale_name}. Use --locale to specify it. "
-                "defaulting to en_US"
+                + "defaulting to en_US"
             )
             self.locale = setlocale(ROOT_DIR, "en")
 
     @property
     def root_dir(self):
         return ROOT_DIR
 
@@ -127,35 +119,44 @@
             if self.archive.startswith("http")
             else pathlib.Path(self.archive).expanduser().resolve()
         )
 
     def run(self):
         """execute the scrapper step by step"""
 
-        self.check_description_length()
+        self.description, self.long_description = compute_descriptions(
+            self.description or "", self.description, self.long_description
+        )
 
         logger.info(f"starting nautilus scraper for {self.archive}")
 
-        logger.info("preparing build folder at {}".format(self.build_dir.resolve()))
+        logger.info(f"preparing build folder at {self.build_dir.resolve()}")
         if not self.keep_build_dir and self.build_dir.exists():
             shutil.rmtree(self.build_dir)
         self.make_build_folder()
 
         # fail early if supplied branding files are missing
         self.check_branding_values()
 
+        # fail early if remote entries URLs are not OK
+        self.test_all_urls()
+
         # download archive
-        self.download_archive()
+        if self.archive:
+            self.download_archive()
 
         if not self.collection:
             self.collection = self.extract_to_fs("collection.json")
             if not self.about:
                 self.extract_to_fs("about.html", failsafe=True)
 
-        self.test_collection()
+        if not self.archive:
+            self.test_archiveless_collection()
+        else:
+            self.test_archive_collection()
 
         logger.info("update general metadata")
         self.update_metadata()
 
         # prepare creator
         self.zim_creator = Creator(
             filename=self.output_dir / self.fname,
@@ -168,15 +169,15 @@
                 Name=self.name,
                 Language=self.language,
                 Title=self.title,
                 Description=self.description,
                 LongDescription=self.long_description,
                 Creator=self.creator,
                 Publisher=self.publisher,
-                Date=datetime.date.today(),
+                Date=datetime.datetime.now().date(),
                 Illustration_48x48_at_1=fh.read(),
                 Tags=";".join(self.tags),
                 Scraper=SCRAPER,
             )
         self.zim_creator.start()
 
         logger.info("adding U.I")
@@ -249,37 +250,22 @@
             raise ValueError(
                 f"--main-color is not a valid hex color: {self.main_color}"
             )
 
         if self.secondary_color and not is_hex_color(self.secondary_color):
             raise ValueError(
                 "--secondary_color-color is not a valid hex color: "
-                f"{self.secondary_color}"
+                + f"{self.secondary_color}"
             )
 
         if self.about:
             handle_user_provided_file(
                 source=self.about, dest=self.build_dir / "about.html"
             )
 
-    def check_description_length(self):
-        if len(self.description) > MAXIMUM_DESCRIPTION_METADATA_LENGTH:
-            raise ValueError(
-                "--The description is greater "
-                f"than {MAXIMUM_DESCRIPTION_METADATA_LENGTH} characters: "
-                f"{len(self.description)} characters"
-            )
-        if self.long_description is not None:
-            if len(self.long_description) > MAXIMUM_LONG_DESCRIPTION_METADATA_LENGTH:
-                raise ValueError(
-                    "--The Long Description is greater "
-                    f"than {MAXIMUM_LONG_DESCRIPTION_METADATA_LENGTH} characters: "
-                    f"{len(self.long_description)} characters"
-                )
-
     def update_metadata(self):
         self.fname = Path(
             self.fname if self.fname else f"{self.name}_{self.period}.zim"
         )
         self.title = self.title or self.name
         self.creator = self.creator or "Unknown"
         self.publisher = self.publisher or "openZIM"
@@ -302,73 +288,217 @@
 
         # get about content from param, archive or defaults to desc
 
         # setting the about_content to long_description if it is provided by the user
         self.about_content = f"<p>{self.long_description or self.description}</p>"
         about_source = self.build_dir / "about.html"
         if about_source.exists():
-            with open(about_source, "r") as fh:
+            with open(about_source) as fh:
                 self.about_content = fh.read()
             about_source.unlink(missing_ok=True)
 
     def download_archive(self):
         # download if it's a URL
         if self.archive.startswith("http"):
             logger.info(f"Downloading archive at {self.archive}")
             save_large_file(self.archive, self.archive_path)
 
     def extract_to_fs(
-        self, name: str, failsafe: Optional[bool] = False
-    ) -> pathlib.Path:
+        self, name: str, *, failsafe: bool | None = False
+    ) -> pathlib.Path | None:
         """extracting single archive member `name` to filesystem at `to`"""
 
         with zipfile.ZipFile(self.archive_path, "r") as zh:
             try:
                 normalized_name = zh.extract(member=name, path=self.build_dir)
                 return self.build_dir.joinpath(normalized_name)
             except Exception as exc:
                 logger.error(f"Unable to extract {name} from archive: {exc}")
                 if failsafe:
                     return
                 raise exc
 
-    def test_collection(self):
-        with open(self.collection, "r") as fp:
+    def load_collection(self):
+        """Load the collection.json"""
+        if not self.collection:
+            self.json_collection = []
+            return
+        with open(self.collection) as fp:
             self.json_collection = [i for i in json.load(fp) if i.get("files", [])]
         nb_items = len(self.json_collection)
         nb_files = sum([len(i.get("files", [])) for i in self.json_collection])
         logger.info(f"Collection loaded. {nb_items} items, {nb_files} files")
 
+    def test_all_urls(self):
+        """Check that all URL entries in collection respond successfully"""
+        self.load_collection()
+        failed = False
+
+        for entry in self.json_collection:
+            if not entry.get("files"):
+                continue
+            for file in entry["files"]:
+                if not isinstance(file, dict) or not file.get("url"):
+                    continue
+                url = file["url"]
+
+                if not url.startswith("http"):
+                    logger.error(f"- Not a valid HTTP URL: {url}")
+                    failed = True
+                    continue
+
+                try:
+                    resp = requests.get(url, stream=True)
+                except Exception as exc:
+                    logger.error(f"- Connection Error: {url} ({exc})")
+                    failed = True
+                    continue
+
+                try:
+                    resp.raise_for_status()
+                except Exception as exc:
+                    logger.error(f"- HTTP {resp.status_code}: {url} ({exc})")
+                    failed = True
+                    continue
+
+        if failed:
+            raise ValueError("Remote entries failed access test")
+
+    def test_archiveless_collection(self):
+        """Test the collection.json without archive file"""
+        self.load_collection()
+
+        (
+            duplicate_filenames,
+            missing_filenames,
+            all_uris,
+        ) = self.test_files()
+
+        if not all_uris:
+            raise ValueError("Collection is emtpy:\n")
+
+        for uri in all_uris:
+            if not uri.startswith("http"):
+                raise ValueError(
+                    f"File referenced in collection which are not urls:\n - {uri}\n "
+                )
+
+        self._ensure_no_missing_files(missing_filenames, [])
+        self._ensure_no_duplicate_filenames(duplicate_filenames)
+
+    def test_archive_collection(self):
+        """Test the collection.json with the archive file"""
+        self.load_collection()
         with zipfile.ZipFile(self.archive_path, "r") as zh:
             all_names = zh.namelist()
+        duplicate_filenames, missing_filenames, _ = self.test_files(all_names)
+
+        self._ensure_no_missing_files(missing_filenames, all_names)
+        self._ensure_no_duplicate_filenames(duplicate_filenames)
+
+    def _ensure_no_missing_files(self, files, member_names):
+        if not files:
+            return
+        extra = ""
+        if member_names:
+            extra = (
+                "\n FYI, here is the list of all members in archive:\n -"
+                + "\n - ".join(
+                    [f"{member} -- {json.dumps(member)}" for member in member_names]
+                )
+            )
+
+        raise ValueError(
+            "File(s) referenced in collection which are missing:\n - "
+            + "\n - ".join(files)
+            + extra
+        )
+
+    def _ensure_no_duplicate_filenames(self, files):
+        if not files:
+            return
+        raise ValueError(
+            "Files in collection which are duplicate:\n - " + "\n - ".join(files)
+        )
+
+    def test_files(
+        self, available_filenames: list[str] | None = None
+    ) -> tuple[list[str], list[str], list[str]]:
+        """Tests the file entries and returns:
+        duplicate_filenames: list of target (in ZIM) filenames that are present 2+ times
+        missing_filenames: list of entry titles for which a filename is missing
+        all_uris: list of all target filenames
+        """
+
+        missing_filenames = []
+        all_uris = []
 
-        missing_files = []
         for entry in self.json_collection:
             if not entry.get("files"):
                 continue
-            for relative_path in entry["files"]:
-                if relative_path not in all_names:
-                    missing_files.append(relative_path)
+            for file in entry["files"]:
+                try:
+                    uri, _ = self.get_file_entry_from(file)
+                    all_uris.append(uri)
+                    if (
+                        not uri.startswith("http")
+                        and available_filenames
+                        and uri not in available_filenames
+                    ):
+                        missing_filenames.append(uri)
+                except ValueError:
+                    missing_filenames.append(entry["title"])
 
-        if missing_files:
-            raise ValueError(
-                "File(s) referenced in collection but missing:\n - "
-                + "\n - ".join(missing_files)
-            )
+        duplicate_filenames = [
+            filename for filename in all_uris if all_uris.count(filename) > 1
+        ]
+        return (duplicate_filenames, missing_filenames, all_uris)
+
+    def get_file_entry_from(self, file: str | dict[str, str]) -> tuple:
+        """Converting a file entity to the (uri, filename)"""
+        # It's for old-format, pathname-only entries
+        if isinstance(file, str):
+            return (file, file)
+        archive_member = file.get("archive-member", None)
+        url = file.get("url", None)
+        uri = None
+        filename = None
+        if not archive_member and not url:
+            raise ValueError("archive-member and url are both missing")
+        if url:
+            uri = url
+            filename = Path(url).name
+        else:
+            uri = archive_member
+            filename = archive_member
+        filename = file.get("filename", filename)
+        return (uri, filename)
 
     def process_collection_entries(self):
         for entry in self.json_collection:
             if not entry.get("files"):
                 continue
 
-            for relative_path in entry["files"]:
-                logger.debug(f"> {relative_path}")
+            for file in entry["files"]:
+                uri, filename = self.get_file_entry_from(file)
+                logger.debug(f"> {uri}")
+
+                if uri.startswith("http"):
+                    fpath = pathlib.Path(
+                        tempfile.NamedTemporaryFile(
+                            dir=self.build_dir, delete=False
+                        ).name
+                    )
+                    save_large_file(uri, fpath)
+                else:
+                    fpath = self.extract_to_fs(uri)
+
                 self.zim_creator.add_item_for(
-                    path="files/" + normalized_path(relative_path),
-                    fpath=self.extract_to_fs(relative_path),
+                    path="files/" + normalized_path(filename),
+                    fpath=fpath,
                     delete_fpath=True,
                     is_front=False,
                 )
 
     def add_ui(self):
         """make up HTML structure to read the content"""
 
@@ -439,15 +569,16 @@
                 str(
                     {
                         "_id": str(docid).zfill(5),
                         "ti": document.get("title") or "Unknown?",
                         "dsc": document.get("description") or "",
                         "aut": document.get("authors") or "",
                         "fp": [
-                            normalized_path(path) for path in document.get("files", [])
+                            normalized_path(self.get_file_entry_from(file)[1])
+                            for file in document.get("files", [])
                         ],
                     }
                 )
             )
         database_js += "];\n"
         self.zim_creator.add_item_for(
             path="database.js",
@@ -457,10 +588,13 @@
         )
 
         # recursively add all templates's folder
         for fpath in self.templates_dir.glob("**/*"):
             if not fpath.is_file():
                 continue
             path = str(fpath.relative_to(self.templates_dir))
+            # index is an actual template which shouldn't be in ZIM
+            if path == "index.html":
+                continue
 
             logger.debug(f"> {path}")
             self.zim_creator.add_item_for(path=path, fpath=fpath, is_front=False)
```

### Comparing `nautiluszim-1.1.1/nautiluszim/templates/favicon.png` & `nautiluszim-1.2.0/src/nautiluszim/templates/favicon.png`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.1/nautiluszim/templates/home.html` & `nautiluszim-1.2.0/src/nautiluszim/templates/home.html`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         footer { background-color: {{ secondary_color }};}
     </style>
   </head>
   <body>
     <header class="container-fluid">
         <div class="row">
             <div class="col-xs-12 col-sm-6">
-                <a href="home.html"><img class="logo" src="main-logo.png" /></a>
+                <a href="home"><img class="logo" src="main-logo.png" /></a>
                 <a href="#" class="btn about-btn" role="button" data-toggle="tooltip" title="{{ about_label }}">
                     <img src="info-circle-solid.svg" />
                 </a>
             </div>
             <form class="form-check-inline search-box col-xs-12 col-sm-6">
                 <input class="form-control" type="search" placeholder="{{ search_input_label }}" id="search_text" />
                 <button class="btn btn-dark ml-2">{{ search_label }}</button>
```

### Comparing `nautiluszim-1.1.1/nautiluszim/templates/info-circle-solid.svg` & `nautiluszim-1.2.0/src/nautiluszim/templates/info-circle-solid.svg`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.1/nautiluszim/templates/init.js` & `nautiluszim-1.2.0/src/nautiluszim/templates/init.js`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.1/nautiluszim/templates/main-logo.png` & `nautiluszim-1.2.0/src/nautiluszim/templates/main-logo.png`

 * *Files identical despite different names*

### Comparing `nautiluszim-1.1.1/nautiluszim/templates/nautilus.js` & `nautiluszim-1.2.0/src/nautiluszim/templates/nautilus.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -154,27 +154,29 @@
                     _this.console.error("Error inserting JS data from " + _this.options.database_path + " into database.", err);
                 });
         });
     };
 
     Nautilus.prototype.init_videojs = function() {
         videojs.options.controls = true;
+        videojs.options.playsinline = true;
         videojs.options.crossorigin = true;
         videojs.options.preload = "auto";
         videojs.options.techOrder = ["html5", "ogvjs"];
         videojs.options.ogvjs = {
             base: "vendors/ogvjs"
         };
         videojs.options.controlBar = {
             pictureInPictureToggle: false
         };
         // for some reason, global controls options is not working
         window.videojs_options = {
             controls: true,
             preload: 'auto',
+            playsinline: true,
             crossorigin: true,
             controlBar: {
                 pictureInPictureToggle: false
             }
         };
     };
```

### Comparing `nautiluszim-1.1.1/nautiluszim/templates/styles.css` & `nautiluszim-1.2.0/src/nautiluszim/templates/styles.css`

 * *Files identical despite different names*

