# Comparing `tmp/cssutils-2.8.0.tar.gz` & `tmp/cssutils-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssutils-2.8.0.tar", last modified: Thu Oct 12 17:13:40 2023, max compression
+gzip compressed data, was "cssutils-2.9.0.tar", last modified: Thu Oct 12 18:44:10 2023, max compression
```

## Comparing `cssutils-2.8.0.tar` & `cssutils-2.9.0.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.321753 cssutils-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 17:13:19.000000 cssutils-2.8.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-10-12 17:13:19.000000 cssutils-2.8.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.281754 cssutils-2.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-12 17:13:19.000000 cssutils-2.8.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-12 17:13:19.000000 cssutils-2.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.281754 cssutils-2.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-10-12 17:13:19.000000 cssutils-2.8.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-12 17:13:19.000000 cssutils-2.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-12 17:13:19.000000 cssutils-2.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35821 2023-10-12 17:13:19.000000 cssutils-2.8.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2023-10-12 17:13:19.000000 cssutils-2.8.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)   122282 2023-10-12 17:13:19.000000 cssutils-2.8.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9085 2023-10-12 17:13:40.321753 cssutils-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2023-10-12 17:13:19.000000 cssutils-2.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-12 17:13:19.000000 cssutils-2.8.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-12 17:13:19.000000 cssutils-2.8.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.285754 cssutils-2.8.0/cssutils/
--rw-r--r--   0 runner    (1001) docker     (127)    13946 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/_fetchgae.py
--rw-r--r--   0 runner    (1001) docker     (127)    22279 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/codec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.289754 cssutils-2.8.0/cssutils/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5943 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/csscharsetrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/csscomment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssfontfacerule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14672 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssimportrule.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssmediarule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11314 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssnamespacerule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15491 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/csspagerule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssproperties.py
--rw-r--r--   0 runner    (1001) docker     (127)    11327 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssrulelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    27105 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssstyledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssstylerule.py
--rw-r--r--   0 runner    (1001) docker     (127)    33799 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssstylesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssunknownrule.py
--rw-r--r--   0 runner    (1001) docker     (127)    47907 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssvariablesdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/cssvariablesrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/marginrule.py
--rw-r--r--   0 runner    (1001) docker     (127)    18379 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/property.py
--rw-r--r--   0 runner    (1001) docker     (127)    32604 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/selectorlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    32614 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/css2productions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/cssproductions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/errorhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8552 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    27811 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/prodparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    34884 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    17145 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/sac.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.289754 cssutils-2.8.0/cssutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/scripts/csscapture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/scripts/csscombine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/scripts/cssparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    42013 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.289754 cssutils-2.8.0/cssutils/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/stylesheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/stylesheets/medialist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/stylesheets/mediaquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/stylesheets/stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/stylesheets/stylesheetlist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.293753 cssutils-2.8.0/cssutils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/basetest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.301753 cssutils-2.8.0/cssutils/tests/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/096.css
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/097.css
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/1.css
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/1ascii.css
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/1import.css
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/1inherit-ascii.css
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/1inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/1inherit-utf8.css
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/1utf.css
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/2inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/2resolve.css
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/acid2.css
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/all.css
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/atrule.css
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/bad.css
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)   208303 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/bundle.css
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/cases.css
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/csscombine-1.css
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/csscombine-2.css
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/csscombine-proxy.css
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/cthedot_default.css
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/default_html4.css
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/hacks.css
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/html.css
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/html20.css
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/html40.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.301753 cssutils-2.8.0/cssutils/tests/sheets/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/images/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.301753 cssutils-2.8.0/cssutils/tests/sheets/import/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.301753 cssutils-2.8.0/cssutils/tests/sheets/import/images2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/import/images2/example2.gif
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/import/import-impossible.css
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/import/import2.css
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/import.css
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/import3.css
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/ll.css
--rw-r--r--   0 runner    (1001) docker     (127)    97995 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/ll2.css
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/multiple-values.css
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/page_test.css
--rw-r--r--   0 runner    (1001) docker     (127)    17998 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/sample_5.css
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/sample_7.css
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/simple.css
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/single-color.css
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/slashcode.css
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/t-HACKS.css
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/test-unicode.css
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/test.css
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/tigris.css
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/tigris2.css
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/u_simple.css
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/v_simple.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.301753 cssutils-2.8.0/cssutils/tests/sheets/var/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/var/start.css
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/var/use.css
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/var/vars.css
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/var/vars2.css
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/vars.css
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/varsimport.css
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/xhtml2.css
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/xhtml22.css
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/sheets/yuck.css
--rw-r--r--   0 runner    (1001) docker     (127)    14385 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_csscharsetrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_csscomment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssfontfacerule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16588 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssimportrule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssmediarule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssnamespacerule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_csspagerule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssproperties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8122 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssrule.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssrulelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    22035 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssstyledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssstylerule.py
--rw-r--r--   0 runner    (1001) docker     (127)    32323 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssstylesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssunknownrule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssutilsimport.py
--rw-r--r--   0 runner    (1001) docker     (127)    33005 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssvariablesdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_cssvariablesrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_domimplementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17682 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_encutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_errorhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_marginrule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_medialist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_mediaquery.py
--rw-r--r--   0 runner    (1001) docker     (127)    19268 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    13854 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_prodparser.py
--rw-r--r--   0 runner    (1001) docker     (127)    24356 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_scripts_csscombine.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_selectorlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    25069 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    22391 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_tokenize2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20121 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    46059 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tests/test_x.py
--rw-r--r--   0 runner    (1001) docker     (127)    11762 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/tokenize2.py
--rw-r--r--   0 runner    (1001) docker     (127)    34381 2023-10-12 17:13:19.000000 cssutils-2.8.0/cssutils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.285754 cssutils-2.8.0/cssutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9085 2023-10-12 17:13:40.000000 cssutils-2.8.0/cssutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2023-10-12 17:13:40.000000 cssutils-2.8.0/cssutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 17:13:40.000000 cssutils-2.8.0/cssutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-10-12 17:13:40.000000 cssutils-2.8.0/cssutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-12 17:13:40.000000 cssutils-2.8.0/cssutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-12 17:13:40.000000 cssutils-2.8.0/cssutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.301753 cssutils-2.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/backlog.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/codec.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/css.rst
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/encutils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.305753 cssutils-2.8.0/docs/html/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/.buildinfo
--rw-r--r--   0 runner    (1001) docker     (127)   217445 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/CHANGELOG.html
--rw-r--r--   0 runner    (1001) docker     (127)    17807 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/README.html
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_2to3 py3.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.305753 cssutils-2.8.0/docs/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)   116989 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.305753 cssutils-2.8.0/docs/html/_sources/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/backlog.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/codec.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/css.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/cssstyledeclaration.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/cssutils.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/encutils.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/implementation.txt
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/logging.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/migrate.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/parse.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/profiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/scripts.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/serialize.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/settings.txt
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/stylesheets.txt
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/utilities.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/docs/variables.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_sources/index.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.309753 cssutils-2.8.0/docs/html/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8269 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)    72174 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/sidebar.js
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.309753 cssutils-2.8.0/docs/html/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/backlog.html
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/codec.html
--rw-r--r--   0 runner    (1001) docker     (127)   167032 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/css.html
--rw-r--r--   0 runner    (1001) docker     (127)    24168 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/encutils.html
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/logging.html
--rw-r--r--   0 runner    (1001) docker     (127)    27207 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/migrate.html
--rw-r--r--   0 runner    (1001) docker     (127)    28207 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/parse.html
--rw-r--r--   0 runner    (1001) docker     (127)    22715 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/profiles.html
--rw-r--r--   0 runner    (1001) docker     (127)    18744 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)    15756 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/serialize.html
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)    21169 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/stylesheets.html
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/utilities.html
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/docs/variables.html
--rw-r--r--   0 runner    (1001) docker     (127)    50793 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)    20302 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/search.html
--rw-r--r--   0 runner    (1001) docker     (127)    42048 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/known issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/migrate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/parse.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/profiles.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/serialize.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/stylesheets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-10-12 17:13:19.000000 cssutils-2.8.0/docs/variables.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.309753 cssutils-2.8.0/encutils/
--rw-r--r--   0 runner    (1001) docker     (127)    21282 2023-10-12 17:13:19.000000 cssutils-2.8.0/encutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.313753 cssutils-2.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/cssencodings.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/customlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/minify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/properties_with_same_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/selectors_tolower.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/styledeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/testutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2023-10-12 17:13:19.000000 cssutils-2.8.0/examples/website.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-12 17:13:19.000000 cssutils-2.8.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-12 17:13:19.000000 cssutils-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-10-12 17:13:19.000000 cssutils-2.8.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-10-12 17:13:19.000000 cssutils-2.8.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2023-10-12 17:13:40.325753 cssutils-2.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.317753 cssutils-2.8.0/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/096.css
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/097.css
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/1.css
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/1ascii.css
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/1import.css
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/1inherit-ascii.css
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/1inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/1inherit-utf8.css
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/1utf.css
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/2inherit-iso.css
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/2resolve.css
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/acid2.css
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/all.css
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/atrule.css
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/bad.css
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/basic.css
--rw-r--r--   0 runner    (1001) docker     (127)   208303 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/bundle.css
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/cases.css
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/csscombine-1.css
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/csscombine-2.css
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/csscombine-proxy.css
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/cthedot_default.css
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/default_html4.css
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/hacks.css
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/html.css
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/html20.css
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/html40.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.317753 cssutils-2.8.0/sheets/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/images/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.317753 cssutils-2.8.0/sheets/import/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.317753 cssutils-2.8.0/sheets/import/images2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/import/images2/example2.gif
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/import/import-impossible.css
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/import/import2.css
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/import.css
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/import3.css
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/ll.css
--rw-r--r--   0 runner    (1001) docker     (127)    97995 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/ll2.css
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/multiple-values.css
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/page_test.css
--rw-r--r--   0 runner    (1001) docker     (127)    17998 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/sample_5.css
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/sample_7.css
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/simple.css
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/single-color.css
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/slashcode.css
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/t-HACKS.css
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/test-unicode.css
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/test.css
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/tigris.css
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/tigris2.css
--rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/u_simple.css
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/v_simple.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.317753 cssutils-2.8.0/sheets/var/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/var/start.css
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/var/use.css
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/var/vars.css
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/var/vars2.css
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/vars.css
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/varsimport.css
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/xhtml2.css
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/xhtml22.css
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-12 17:13:19.000000 cssutils-2.8.0/sheets/yuck.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 17:13:40.317753 cssutils-2.8.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-10-12 17:13:19.000000 cssutils-2.8.0/tools/speed.py
--rw-r--r--   0 runner    (1001) docker     (127)    37536 2023-10-12 17:13:19.000000 cssutils-2.8.0/tools/try.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-12 17:13:19.000000 cssutils-2.8.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-12 17:13:19.000000 cssutils-2.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.314098 cssutils-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 18:43:47.000000 cssutils-2.9.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-10-12 18:43:47.000000 cssutils-2.9.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.278092 cssutils-2.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-12 18:43:47.000000 cssutils-2.9.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-12 18:43:47.000000 cssutils-2.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.278092 cssutils-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2023-10-12 18:43:47.000000 cssutils-2.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-12 18:43:47.000000 cssutils-2.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-12 18:43:47.000000 cssutils-2.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35821 2023-10-12 18:43:47.000000 cssutils-2.9.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2023-10-12 18:43:47.000000 cssutils-2.9.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)   122366 2023-10-12 18:43:47.000000 cssutils-2.9.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2023-10-12 18:44:10.314098 cssutils-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2023-10-12 18:43:47.000000 cssutils-2.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-12 18:43:47.000000 cssutils-2.9.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-12 18:43:47.000000 cssutils-2.9.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.278092 cssutils-2.9.0/cssutils/
+-rw-r--r--   0 runner    (1001) docker     (127)    13946 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/_fetchgae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22279 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/codec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.282092 cssutils-2.9.0/cssutils/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5943 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/csscharsetrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/csscomment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssfontfacerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14672 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssimportrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssmediarule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11314 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssnamespacerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/csspagerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssproperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssrulelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27105 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssstyledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssstylerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33799 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssstylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssunknownrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47907 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssvariablesdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/cssvariablesrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/marginrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18379 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32604 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/selectorlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32614 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/css2productions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/cssproductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/errorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8552 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27811 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/prodparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34884 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17145 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/sac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.282092 cssutils-2.9.0/cssutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/scripts/csscapture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/scripts/csscombine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/scripts/cssparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42013 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.282092 cssutils-2.9.0/cssutils/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/stylesheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/stylesheets/medialist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/stylesheets/mediaquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/stylesheets/stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/stylesheets/stylesheetlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.290094 cssutils-2.9.0/cssutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/basetest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.294094 cssutils-2.9.0/cssutils/tests/sheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/096.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/097.css
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/1.css
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/1ascii.css
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/1import.css
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/1inherit-ascii.css
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/1inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/1inherit-utf8.css
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/1utf.css
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/2inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/2resolve.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/acid2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/all.css
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/atrule.css
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/bad.css
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)   208303 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/cases.css
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/csscombine-1.css
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/csscombine-2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/csscombine-proxy.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/cthedot_default.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/default_html4.css
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/hacks.css
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/html.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/html20.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/html40.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.294094 cssutils-2.9.0/cssutils/tests/sheets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/images/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.294094 cssutils-2.9.0/cssutils/tests/sheets/import/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.294094 cssutils-2.9.0/cssutils/tests/sheets/import/images2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/import/images2/example2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/import/import-impossible.css
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/import/import2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/import.css
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/import3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/ll.css
+-rw-r--r--   0 runner    (1001) docker     (127)    97995 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/ll2.css
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/multiple-values.css
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/page_test.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17998 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/sample_5.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/sample_7.css
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/simple.css
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/single-color.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/slashcode.css
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/t-HACKS.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/test-unicode.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/test.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/tigris.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/tigris2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/u_simple.css
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/v_simple.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.294094 cssutils-2.9.0/cssutils/tests/sheets/var/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/var/start.css
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/var/use.css
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/var/vars.css
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/var/vars2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/vars.css
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/varsimport.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/xhtml2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/xhtml22.css
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/sheets/yuck.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14385 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_csscharsetrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_csscomment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssfontfacerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16588 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssimportrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssmediarule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssnamespacerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13395 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_csspagerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssproperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssrulelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22035 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssstyledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssstylerule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32323 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssstylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssunknownrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssutilsimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33005 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssvariablesdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_cssvariablesrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_domimplementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17682 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_encutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_errorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_marginrule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_medialist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_mediaquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19268 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13854 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_prodparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24356 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_scripts_csscombine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_selectorlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25069 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_tokenize2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20121 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46059 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tests/test_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11762 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/tokenize2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34381 2023-10-12 18:43:47.000000 cssutils-2.9.0/cssutils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.278092 cssutils-2.9.0/cssutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2023-10-12 18:44:10.000000 cssutils-2.9.0/cssutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2023-10-12 18:44:10.000000 cssutils-2.9.0/cssutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 18:44:10.000000 cssutils-2.9.0/cssutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-10-12 18:44:10.000000 cssutils-2.9.0/cssutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-12 18:44:10.000000 cssutils-2.9.0/cssutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-12 18:44:10.000000 cssutils-2.9.0/cssutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.298095 cssutils-2.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/backlog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/codec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/css.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/encutils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.298095 cssutils-2.9.0/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/.buildinfo
+-rw-r--r--   0 runner    (1001) docker     (127)   217445 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/CHANGELOG.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17807 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/README.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_2to3 py3.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.298095 cssutils-2.9.0/docs/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)   116989 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.302096 cssutils-2.9.0/docs/html/_sources/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/backlog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/codec.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/css.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/cssstyledeclaration.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/cssutils.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/encutils.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/implementation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/logging.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/migrate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/parse.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/profiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/scripts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/serialize.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/settings.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/stylesheets.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/utilities.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/docs/variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_sources/index.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.302096 cssutils-2.9.0/docs/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)    72174 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.302096 cssutils-2.9.0/docs/html/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/backlog.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/codec.html
+-rw-r--r--   0 runner    (1001) docker     (127)   167032 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/css.html
+-rw-r--r--   0 runner    (1001) docker     (127)    24168 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/encutils.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/logging.html
+-rw-r--r--   0 runner    (1001) docker     (127)    27207 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/migrate.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28207 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/parse.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22715 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/profiles.html
+-rw-r--r--   0 runner    (1001) docker     (127)    18744 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15756 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/serialize.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/settings.html
+-rw-r--r--   0 runner    (1001) docker     (127)    21169 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/stylesheets.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/utilities.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/docs/variables.html
+-rw-r--r--   0 runner    (1001) docker     (127)    50793 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20302 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)    42048 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/html/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/known issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/migrate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/parse.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/profiles.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/serialize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/stylesheets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-10-12 18:43:47.000000 cssutils-2.9.0/docs/variables.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.302096 cssutils-2.9.0/encutils/
+-rw-r--r--   0 runner    (1001) docker     (127)    21282 2023-10-12 18:43:47.000000 cssutils-2.9.0/encutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.306096 cssutils-2.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/cssencodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/customlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/minify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/properties_with_same_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/selectors_tolower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/styledeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2023-10-12 18:43:47.000000 cssutils-2.9.0/examples/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-12 18:43:47.000000 cssutils-2.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-10-12 18:43:47.000000 cssutils-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2023-10-12 18:43:47.000000 cssutils-2.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-10-12 18:43:47.000000 cssutils-2.9.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2023-10-12 18:44:10.314098 cssutils-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.310097 cssutils-2.9.0/sheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/096.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/097.css
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/1.css
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/1ascii.css
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/1import.css
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/1inherit-ascii.css
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/1inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/1inherit-utf8.css
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/1utf.css
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/2inherit-iso.css
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/2resolve.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/acid2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/all.css
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/atrule.css
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/bad.css
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/basic.css
+-rw-r--r--   0 runner    (1001) docker     (127)   208303 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/cases.css
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/csscombine-1.css
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/csscombine-2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/csscombine-proxy.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/cthedot_default.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/default_html4.css
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/hacks.css
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/html.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/html20.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/html40.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.310097 cssutils-2.9.0/sheets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/images/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.310097 cssutils-2.9.0/sheets/import/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.314098 cssutils-2.9.0/sheets/import/images2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/import/images2/example2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/import/import-impossible.css
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/import/import2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/import.css
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/import3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/ll.css
+-rw-r--r--   0 runner    (1001) docker     (127)    97995 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/ll2.css
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/multiple-values.css
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/page_test.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17998 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/sample_5.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/sample_7.css
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/simple.css
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/single-color.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18645 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/slashcode.css
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/t-HACKS.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/test-unicode.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/test.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/tigris.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/tigris2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/u_simple.css
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/v_simple.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.314098 cssutils-2.9.0/sheets/var/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/var/start.css
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/var/use.css
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/var/vars.css
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/var/vars2.css
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/vars.css
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/varsimport.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/xhtml2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/xhtml22.css
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-12 18:43:47.000000 cssutils-2.9.0/sheets/yuck.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 18:44:10.314098 cssutils-2.9.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2023-10-12 18:43:47.000000 cssutils-2.9.0/tools/speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37536 2023-10-12 18:43:47.000000 cssutils-2.9.0/tools/try.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-12 18:43:47.000000 cssutils-2.9.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-10-12 18:43:47.000000 cssutils-2.9.0/tox.ini
```

### Comparing `cssutils-2.8.0/.github/workflows/main.yml` & `cssutils-2.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/COPYING` & `cssutils-2.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/COPYING.LESSER` & `cssutils-2.9.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/NEWS.rst` & `cssutils-2.9.0/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.9.0
+======
+
+Features
+--------
+
+- Made URL fetcher lenient to missing metadata.
+
+
 v2.8.0
 ======
 
 Features
 --------
 
 - Require Python 3.8 or later.
```

### Comparing `cssutils-2.8.0/PKG-INFO` & `cssutils-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssutils
-Version: 2.8.0
+Version: 2.9.0
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/jaraco/cssutils
 Author: Christof Hoeke
 Author-email: c@cthedot.de
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
```

### Comparing `cssutils-2.8.0/README.rst` & `cssutils-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/conftest.py` & `cssutils-2.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/__init__.py` & `cssutils-2.9.0/cssutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/_fetch.py` & `cssutils-2.9.0/cssutils/_fetch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 """Default URL reading functions"""
 __all__ = ['_defaultFetcher']
 
+import functools
 import urllib.request
 import urllib.error
 
 try:
     from importlib import metadata
 except ImportError:
     import importlib_metadata as metadata
 
 import encutils
 from . import errorhandler
 
 log = errorhandler.ErrorHandler()
 
 
+@functools.lru_cache()
+def _get_version():
+    try:
+        return metadata.version('cssutils')
+    except metadata.PackageNotFoundError:
+        return 'unknown'
+
+
 def _defaultFetcher(url):
     """Retrieve data from ``url``. cssutils default implementation of fetch
     URL function.
 
     Returns ``(encoding, string)`` or ``None``
     """
     try:
         request = urllib.request.Request(url)
-        version = metadata.version('cssutils')
-        agent = f'cssutils {version} (https://pypi.org/project/cssutils)'
+        agent = f'cssutils/{_get_version()} (https://pypi.org/project/cssutils)'
         request.add_header('User-agent', agent)
         res = urllib.request.urlopen(request)
     except urllib.error.HTTPError as e:
         # http error, e.g. 404, e can be raised
         log.warn(f'HTTPError opening url={url}: {e.code} {e.msg}', error=e)
     except urllib.error.URLError as e:
         # URLError like mailto: or other IO errors, e can be raised
```

### Comparing `cssutils-2.8.0/cssutils/_fetchgae.py` & `cssutils-2.9.0/cssutils/_fetchgae.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/codec.py` & `cssutils-2.9.0/cssutils/codec.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/__init__.py` & `cssutils-2.9.0/cssutils/css/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/colors.py` & `cssutils-2.9.0/cssutils/css/colors.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/csscharsetrule.py` & `cssutils-2.9.0/cssutils/css/csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/csscomment.py` & `cssutils-2.9.0/cssutils/css/csscomment.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssfontfacerule.py` & `cssutils-2.9.0/cssutils/css/cssfontfacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssimportrule.py` & `cssutils-2.9.0/cssutils/css/cssimportrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssmediarule.py` & `cssutils-2.9.0/cssutils/css/cssmediarule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssnamespacerule.py` & `cssutils-2.9.0/cssutils/css/cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/csspagerule.py` & `cssutils-2.9.0/cssutils/css/csspagerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssproperties.py` & `cssutils-2.9.0/cssutils/css/cssproperties.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssrule.py` & `cssutils-2.9.0/cssutils/css/cssrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssrulelist.py` & `cssutils-2.9.0/cssutils/css/cssrulelist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssstyledeclaration.py` & `cssutils-2.9.0/cssutils/css/cssstyledeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssstylerule.py` & `cssutils-2.9.0/cssutils/css/cssstylerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssstylesheet.py` & `cssutils-2.9.0/cssutils/css/cssstylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssunknownrule.py` & `cssutils-2.9.0/cssutils/css/cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssvalue.py` & `cssutils-2.9.0/cssutils/css/cssvalue.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssvariablesdeclaration.py` & `cssutils-2.9.0/cssutils/css/cssvariablesdeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/cssvariablesrule.py` & `cssutils-2.9.0/cssutils/css/cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/marginrule.py` & `cssutils-2.9.0/cssutils/css/marginrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/property.py` & `cssutils-2.9.0/cssutils/css/property.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/selector.py` & `cssutils-2.9.0/cssutils/css/selector.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/selectorlist.py` & `cssutils-2.9.0/cssutils/css/selectorlist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css/value.py` & `cssutils-2.9.0/cssutils/css/value.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/css2productions.py` & `cssutils-2.9.0/cssutils/css2productions.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/cssproductions.py` & `cssutils-2.9.0/cssutils/cssproductions.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/errorhandler.py` & `cssutils-2.9.0/cssutils/errorhandler.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/helper.py` & `cssutils-2.9.0/cssutils/helper.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/parse.py` & `cssutils-2.9.0/cssutils/parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/prodparser.py` & `cssutils-2.9.0/cssutils/prodparser.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/profiles.py` & `cssutils-2.9.0/cssutils/profiles.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/sac.py` & `cssutils-2.9.0/cssutils/sac.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/script.py` & `cssutils-2.9.0/cssutils/script.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/scripts/csscapture.py` & `cssutils-2.9.0/cssutils/scripts/csscapture.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/scripts/csscombine.py` & `cssutils-2.9.0/cssutils/scripts/csscombine.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/scripts/cssparse.py` & `cssutils-2.9.0/cssutils/scripts/cssparse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/serialize.py` & `cssutils-2.9.0/cssutils/serialize.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/settings.py` & `cssutils-2.9.0/cssutils/settings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/stylesheets/medialist.py` & `cssutils-2.9.0/cssutils/stylesheets/medialist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/stylesheets/mediaquery.py` & `cssutils-2.9.0/cssutils/stylesheets/mediaquery.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/stylesheets/stylesheet.py` & `cssutils-2.9.0/cssutils/stylesheets/stylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/stylesheets/stylesheetlist.py` & `cssutils-2.9.0/cssutils/stylesheets/stylesheetlist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/basetest.py` & `cssutils-2.9.0/cssutils/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/096.css` & `cssutils-2.9.0/cssutils/tests/sheets/096.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/097.css` & `cssutils-2.9.0/cssutils/tests/sheets/097.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/acid2.css` & `cssutils-2.9.0/cssutils/tests/sheets/acid2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/bundle.css` & `cssutils-2.9.0/cssutils/tests/sheets/bundle.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/cthedot_default.css` & `cssutils-2.9.0/cssutils/tests/sheets/cthedot_default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/default_html4.css` & `cssutils-2.9.0/cssutils/tests/sheets/default_html4.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/hacks.css` & `cssutils-2.9.0/cssutils/tests/sheets/hacks.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/html20.css` & `cssutils-2.9.0/cssutils/tests/sheets/html20.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/html40.css` & `cssutils-2.9.0/cssutils/tests/sheets/html40.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/ll.css` & `cssutils-2.9.0/cssutils/tests/sheets/ll.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/ll2.css` & `cssutils-2.9.0/cssutils/tests/sheets/ll2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/sample_5.css` & `cssutils-2.9.0/cssutils/tests/sheets/sample_5.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/sample_7.css` & `cssutils-2.9.0/cssutils/tests/sheets/sample_7.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/slashcode.css` & `cssutils-2.9.0/cssutils/tests/sheets/slashcode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/t-HACKS.css` & `cssutils-2.9.0/cssutils/tests/sheets/t-HACKS.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/test-unicode.css` & `cssutils-2.9.0/cssutils/tests/sheets/test-unicode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/test.css` & `cssutils-2.9.0/cssutils/tests/sheets/test.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/tigris.css` & `cssutils-2.9.0/cssutils/tests/sheets/tigris.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/tigris2.css` & `cssutils-2.9.0/cssutils/tests/sheets/tigris2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/xhtml2.css` & `cssutils-2.9.0/cssutils/tests/sheets/xhtml2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/sheets/xhtml22.css` & `cssutils-2.9.0/cssutils/tests/sheets/xhtml22.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_codec.py` & `cssutils-2.9.0/cssutils/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_csscharsetrule.py` & `cssutils-2.9.0/cssutils/tests/test_csscharsetrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_csscomment.py` & `cssutils-2.9.0/cssutils/tests/test_csscomment.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssfontfacerule.py` & `cssutils-2.9.0/cssutils/tests/test_cssfontfacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssimportrule.py` & `cssutils-2.9.0/cssutils/tests/test_cssimportrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssmediarule.py` & `cssutils-2.9.0/cssutils/tests/test_cssmediarule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssnamespacerule.py` & `cssutils-2.9.0/cssutils/tests/test_cssnamespacerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_csspagerule.py` & `cssutils-2.9.0/cssutils/tests/test_csspagerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssproperties.py` & `cssutils-2.9.0/cssutils/tests/test_cssproperties.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssrule.py` & `cssutils-2.9.0/cssutils/tests/test_cssrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssrulelist.py` & `cssutils-2.9.0/cssutils/tests/test_cssrulelist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssstyledeclaration.py` & `cssutils-2.9.0/cssutils/tests/test_cssstyledeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssstylerule.py` & `cssutils-2.9.0/cssutils/tests/test_cssstylerule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssstylesheet.py` & `cssutils-2.9.0/cssutils/tests/test_cssstylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssunknownrule.py` & `cssutils-2.9.0/cssutils/tests/test_cssunknownrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssutils.py` & `cssutils-2.9.0/cssutils/tests/test_cssutils.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssvalue.py` & `cssutils-2.9.0/cssutils/tests/test_cssvalue.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssvariablesdeclaration.py` & `cssutils-2.9.0/cssutils/tests/test_cssvariablesdeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_cssvariablesrule.py` & `cssutils-2.9.0/cssutils/tests/test_cssvariablesrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_domimplementation.py` & `cssutils-2.9.0/cssutils/tests/test_domimplementation.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_encutils.py` & `cssutils-2.9.0/cssutils/tests/test_encutils.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_errorhandler.py` & `cssutils-2.9.0/cssutils/tests/test_errorhandler.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_helper.py` & `cssutils-2.9.0/cssutils/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_marginrule.py` & `cssutils-2.9.0/cssutils/tests/test_marginrule.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_medialist.py` & `cssutils-2.9.0/cssutils/tests/test_medialist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_mediaquery.py` & `cssutils-2.9.0/cssutils/tests/test_mediaquery.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_parse.py` & `cssutils-2.9.0/cssutils/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_prodparser.py` & `cssutils-2.9.0/cssutils/tests/test_prodparser.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_profiles.py` & `cssutils-2.9.0/cssutils/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_properties.py` & `cssutils-2.9.0/cssutils/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_property.py` & `cssutils-2.9.0/cssutils/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_scripts_csscombine.py` & `cssutils-2.9.0/cssutils/tests/test_scripts_csscombine.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_selector.py` & `cssutils-2.9.0/cssutils/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_selectorlist.py` & `cssutils-2.9.0/cssutils/tests/test_selectorlist.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_serialize.py` & `cssutils-2.9.0/cssutils/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_settings.py` & `cssutils-2.9.0/cssutils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_stylesheet.py` & `cssutils-2.9.0/cssutils/tests/test_stylesheet.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_tokenize2.py` & `cssutils-2.9.0/cssutils/tests/test_tokenize2.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_util.py` & `cssutils-2.9.0/cssutils/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_value.py` & `cssutils-2.9.0/cssutils/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tests/test_x.py` & `cssutils-2.9.0/cssutils/tests/test_x.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/tokenize2.py` & `cssutils-2.9.0/cssutils/tokenize2.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils/util.py` & `cssutils-2.9.0/cssutils/util.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/cssutils.egg-info/PKG-INFO` & `cssutils-2.9.0/cssutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cssutils
-Version: 2.8.0
+Version: 2.9.0
 Summary: A CSS Cascading Style Sheets library for Python
 Home-page: https://github.com/jaraco/cssutils
 Author: Christof Hoeke
 Author-email: c@cthedot.de
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Keywords: CSS,Cascading Style Sheets,CSSParser,DOM Level 2 Stylesheets,DOM Level 2 CSS
```

### Comparing `cssutils-2.8.0/cssutils.egg-info/SOURCES.txt` & `cssutils-2.9.0/cssutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/backlog.rst` & `cssutils-2.9.0/docs/backlog.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/conf.py` & `cssutils-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/css.rst` & `cssutils-2.9.0/docs/css.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/CHANGELOG.html` & `cssutils-2.9.0/docs/html/CHANGELOG.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/README.html` & `cssutils-2.9.0/docs/html/README.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_2to3 py3.html` & `cssutils-2.9.0/docs/html/_2to3 py3.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/CHANGELOG.txt` & `cssutils-2.9.0/docs/html/_sources/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/README.txt` & `cssutils-2.9.0/docs/html/_sources/README.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/backlog.txt` & `cssutils-2.9.0/docs/html/_sources/docs/backlog.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/css.txt` & `cssutils-2.9.0/docs/html/_sources/docs/css.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/cssstyledeclaration.txt` & `cssutils-2.9.0/docs/html/_sources/docs/cssstyledeclaration.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/implementation.txt` & `cssutils-2.9.0/docs/html/_sources/docs/implementation.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/logging.txt` & `cssutils-2.9.0/docs/html/_sources/docs/logging.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/migrate.txt` & `cssutils-2.9.0/docs/html/_sources/docs/migrate.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/parse.txt` & `cssutils-2.9.0/docs/html/_sources/docs/parse.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/profiles.txt` & `cssutils-2.9.0/docs/html/_sources/docs/profiles.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/scripts.txt` & `cssutils-2.9.0/docs/html/_sources/docs/scripts.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/serialize.txt` & `cssutils-2.9.0/docs/html/_sources/docs/serialize.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/settings.txt` & `cssutils-2.9.0/docs/html/_sources/docs/settings.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/docs/stylesheets.txt` & `cssutils-2.9.0/docs/html/_sources/docs/stylesheets.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_sources/index.txt` & `cssutils-2.9.0/docs/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/basic.css` & `cssutils-2.9.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/default.css` & `cssutils-2.9.0/docs/html/_static/default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/doctools.js` & `cssutils-2.9.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/jquery.js` & `cssutils-2.9.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/pygments.css` & `cssutils-2.9.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/searchtools.js` & `cssutils-2.9.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/sidebar.js` & `cssutils-2.9.0/docs/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/_static/underscore.js` & `cssutils-2.9.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/backlog.html` & `cssutils-2.9.0/docs/html/docs/backlog.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/codec.html` & `cssutils-2.9.0/docs/html/docs/codec.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/css.html` & `cssutils-2.9.0/docs/html/docs/css.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/encutils.html` & `cssutils-2.9.0/docs/html/docs/encutils.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/logging.html` & `cssutils-2.9.0/docs/html/docs/logging.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/migrate.html` & `cssutils-2.9.0/docs/html/docs/migrate.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/parse.html` & `cssutils-2.9.0/docs/html/docs/parse.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/profiles.html` & `cssutils-2.9.0/docs/html/docs/profiles.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/scripts.html` & `cssutils-2.9.0/docs/html/docs/scripts.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/serialize.html` & `cssutils-2.9.0/docs/html/docs/serialize.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/settings.html` & `cssutils-2.9.0/docs/html/docs/settings.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/stylesheets.html` & `cssutils-2.9.0/docs/html/docs/stylesheets.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/utilities.html` & `cssutils-2.9.0/docs/html/docs/utilities.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/docs/variables.html` & `cssutils-2.9.0/docs/html/docs/variables.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/genindex.html` & `cssutils-2.9.0/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/index.html` & `cssutils-2.9.0/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/py-modindex.html` & `cssutils-2.9.0/docs/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/search.html` & `cssutils-2.9.0/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/html/searchindex.js` & `cssutils-2.9.0/docs/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/index.rst` & `cssutils-2.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/known issues.rst` & `cssutils-2.9.0/docs/known issues.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/logging.rst` & `cssutils-2.9.0/docs/logging.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/migrate.rst` & `cssutils-2.9.0/docs/migrate.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/parse.rst` & `cssutils-2.9.0/docs/parse.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/profiles.rst` & `cssutils-2.9.0/docs/profiles.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/scripts.rst` & `cssutils-2.9.0/docs/scripts.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/serialize.rst` & `cssutils-2.9.0/docs/serialize.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/settings.rst` & `cssutils-2.9.0/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/docs/stylesheets.rst` & `cssutils-2.9.0/docs/stylesheets.rst`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/encutils/__init__.py` & `cssutils-2.9.0/encutils/__init__.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/build.py` & `cssutils-2.9.0/examples/build.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/cssencodings.py` & `cssutils-2.9.0/examples/cssencodings.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/customlog.py` & `cssutils-2.9.0/examples/customlog.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/imports.py` & `cssutils-2.9.0/examples/imports.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/minify.py` & `cssutils-2.9.0/examples/minify.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/parse.py` & `cssutils-2.9.0/examples/parse.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/properties_with_same_name.py` & `cssutils-2.9.0/examples/properties_with_same_name.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/selectors_tolower.py` & `cssutils-2.9.0/examples/selectors_tolower.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/serialize.py` & `cssutils-2.9.0/examples/serialize.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/style.py` & `cssutils-2.9.0/examples/style.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/styledeclaration.py` & `cssutils-2.9.0/examples/styledeclaration.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/testutil.py` & `cssutils-2.9.0/examples/testutil.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/examples/website.py` & `cssutils-2.9.0/examples/website.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/pytest.ini` & `cssutils-2.9.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/setup.cfg` & `cssutils-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/096.css` & `cssutils-2.9.0/sheets/096.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/097.css` & `cssutils-2.9.0/sheets/097.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/acid2.css` & `cssutils-2.9.0/sheets/acid2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/bundle.css` & `cssutils-2.9.0/sheets/bundle.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/cthedot_default.css` & `cssutils-2.9.0/sheets/cthedot_default.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/default_html4.css` & `cssutils-2.9.0/sheets/default_html4.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/hacks.css` & `cssutils-2.9.0/sheets/hacks.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/html20.css` & `cssutils-2.9.0/sheets/html20.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/html40.css` & `cssutils-2.9.0/sheets/html40.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/ll.css` & `cssutils-2.9.0/sheets/ll.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/ll2.css` & `cssutils-2.9.0/sheets/ll2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/sample_5.css` & `cssutils-2.9.0/sheets/sample_5.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/sample_7.css` & `cssutils-2.9.0/sheets/sample_7.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/slashcode.css` & `cssutils-2.9.0/sheets/slashcode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/t-HACKS.css` & `cssutils-2.9.0/sheets/t-HACKS.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/test-unicode.css` & `cssutils-2.9.0/sheets/test-unicode.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/test.css` & `cssutils-2.9.0/sheets/test.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/tigris.css` & `cssutils-2.9.0/sheets/tigris.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/tigris2.css` & `cssutils-2.9.0/sheets/tigris2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/xhtml2.css` & `cssutils-2.9.0/sheets/xhtml2.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/sheets/xhtml22.css` & `cssutils-2.9.0/sheets/xhtml22.css`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/tools/speed.py` & `cssutils-2.9.0/tools/speed.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/tools/try.py` & `cssutils-2.9.0/tools/try.py`

 * *Files identical despite different names*

### Comparing `cssutils-2.8.0/tox.ini` & `cssutils-2.9.0/tox.ini`

 * *Files identical despite different names*

