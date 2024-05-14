# Comparing `tmp/newshomepages-0.0.91.tar.gz` & `tmp/newshomepages-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newshomepages-0.0.91.tar", last modified: Tue Apr  9 19:12:12 2024, max compression
+gzip compressed data, was "newshomepages-0.0.92.tar", last modified: Tue May 14 15:36:21 2024, max compression
```

## Comparing `newshomepages-0.0.91.tar` & `newshomepages-0.0.92.tar`

### file list

```diff
@@ -1,635 +1,635 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.321858 newshomepages-0.0.91/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.devcontainer/postCreateCommand.sh
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/ISSUE_TEMPLATE/add-a-site.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/ISSUE_TEMPLATE/report-a-broken-site.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.197857 newshomepages-0.0.91/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.github/workflows/site.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-09 19:11:53.000000 newshomepages-0.0.91/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-09 19:11:53.000000 newshomepages-0.0.91/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 19:11:53.000000 newshomepages-0.0.91/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 19:11:53.000000 newshomepages-0.0.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 19:11:53.000000 newshomepages-0.0.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-09 19:11:53.000000 newshomepages-0.0.91/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-09 19:12:12.321858 newshomepages-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-09 19:11:53.000000 newshomepages-0.0.91/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)   203048 2024-04-09 19:11:53.000000 newshomepages-0.0.91/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 19:11:53.000000 newshomepages-0.0.91/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 19:11:53.000000 newshomepages-0.0.91/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 19:11:53.000000 newshomepages-0.0.91/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/adstxt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/drudge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/lighthouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/analyze/us_right_wing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/extensions/adguard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ar/
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ar/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.201857 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/be/
--rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/be/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bg/
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bg/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bn/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ca/
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ca/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/cs/
--rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/cs/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/da/
--rw-r--r--   0 runner    (1001) docker     (127)    32176 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/da/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/de/
--rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/de/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/el/
--rw-r--r--   0 runner    (1001) docker     (127)    35861 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/el/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/en/
--rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/en/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es/
--rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es_419/
--rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es_419/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/et/
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/et/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fa/
--rw-r--r--   0 runner    (1001) docker     (127)    24231 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fa/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fi/
--rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fil/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fil/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fr/
--rw-r--r--   0 runner    (1001) docker     (127)    34308 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/he/
--rw-r--r--   0 runner    (1001) docker     (127)    35288 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/he/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hi/
--rw-r--r--   0 runner    (1001) docker     (127)    21672 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hr/
--rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hu/
--rw-r--r--   0 runner    (1001) docker     (127)    34371 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hu/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.205858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hy/
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hy/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/id/
--rw-r--r--   0 runner    (1001) docker     (127)    32258 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/id/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/it/
--rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/it/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ja/
--rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ja/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/kn/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/kn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ko/
--rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ko/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lt/
--rw-r--r--   0 runner    (1001) docker     (127)    21630 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lv/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/mk-MK/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/mk-MK/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ms/
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ms/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nb/
--rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nb/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nl/
--rw-r--r--   0 runner    (1001) docker     (127)    33052 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pl/
--rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (127)    33333 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_BR/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (127)    33264 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_PT/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ro/
--rw-r--r--   0 runner    (1001) docker     (127)    33424 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ro/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ru/
--rw-r--r--   0 runner    (1001) docker     (127)    40337 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ru/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sk/
--rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sl/
--rw-r--r--   0 runner    (1001) docker     (127)    32933 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.209858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr-Latn/
--rw-r--r--   0 runner    (1001) docker     (127)    31450 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sv/
--rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ta/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ta/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/te/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/te/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/th/
--rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/th/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/tr/
--rw-r--r--   0 runner    (1001) docker     (127)    33471 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/tr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/uk/
--rw-r--r--   0 runner    (1001) docker     (127)    39572 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/uk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/vi/
--rw-r--r--   0 runner    (1001) docker     (127)    35067 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/vi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_CN/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_TW/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.213858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/alert-popup.css
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/c3.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.217857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/dark.css
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/layout.css
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/log.css
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/nanobar.css
--rw-r--r--   0 runner    (1001) docker     (127)    54145 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.217857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    66004 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    66708 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    65764 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.217857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-38.png
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-38.png
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-38.png
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-128.png
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-19.png
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-38.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/app-store.svg
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/avatar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/chrome.svg
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/cross.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/dropbox.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/filters.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/google-play.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-green.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-red.svg
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-shield.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo_adguard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico.svg
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/shield.svg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/tick.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/toggler-bg.svg
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/trash.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/js/preload-theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/scriptlets/
--rw-r--r--   0 runner    (1001) docker     (127)   141578 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.221858 newshomepages-0.0.91/newshomepages/extensions/adguard/content-script/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/content-script/subscribe.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.257858 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/
--rw-r--r--   0 runner    (1001) docker     (127)  1206317 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    73188 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_10.txt
--rw-r--r--   0 runner    (1001) docker     (127)   313462 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)    94026 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)   402899 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_13.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2213341 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_14.txt
--rw-r--r--   0 runner    (1001) docker     (127)   928335 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_15.txt
--rw-r--r--   0 runner    (1001) docker     (127)   774091 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_16.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35060 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_17.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4655227 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   735758 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_224.txt
--rw-r--r--   0 runner    (1001) docker     (127)   914459 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)   585242 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   496599 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_6.txt
--rw-r--r--   0 runner    (1001) docker     (127)   271134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_7.txt
--rw-r--r--   0 runner    (1001) docker     (127)    69106 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_8.txt
--rw-r--r--   0 runner    (1001) docker     (127)   237431 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_9.txt
--rw-r--r--   0 runner    (1001) docker     (127)   483303 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    67127 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_10.txt
--rw-r--r--   0 runner    (1001) docker     (127)   256792 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)    71645 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)   363915 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_13.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1223256 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_14.txt
--rw-r--r--   0 runner    (1001) docker     (127)   899376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_15.txt
--rw-r--r--   0 runner    (1001) docker     (127)   341390 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_16.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_17.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1640295 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)   710272 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_224.txt
--rw-r--r--   0 runner    (1001) docker     (127)   806171 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)   361755 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)   193843 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_6.txt
--rw-r--r--   0 runner    (1001) docker     (127)   249182 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_7.txt
--rw-r--r--   0 runner    (1001) docker     (127)    58256 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_8.txt
--rw-r--r--   0 runner    (1001) docker     (127)   191331 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_9.txt
--rw-r--r--   0 runner    (1001) docker     (127)    51441 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters.json
--rw-r--r--   0 runner    (1001) docker     (127)   799078 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters_i18n.json
--rw-r--r--   0 runner    (1001) docker     (127)  1545375 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/filters/local_script_rules.json
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.273858 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/ad-blocked.html
--rw-r--r--   0 runner    (1001) docker     (127)   177876 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/ad-blocked.js
--rw-r--r--   0 runner    (1001) docker     (127)   650939 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/assistant.js
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/background.html
--rw-r--r--   0 runner    (1001) docker     (127)  3189967 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/background.js
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-end.js
--rw-r--r--   0 runner    (1001) docker     (127)   288034 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-start.js
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools.html
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools.js
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.html
--rw-r--r--   0 runner    (1001) docker     (127)    62185 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.js
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filtering-log.html
--rw-r--r--   0 runner    (1001) docker     (127)  1408341 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filtering-log.js
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html
--rw-r--r--   0 runner    (1001) docker     (127)   582536 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.html
--rw-r--r--   0 runner    (1001) docker     (127)  1079105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.js
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/popup.html
--rw-r--r--   0 runner    (1001) docker     (127)  1072410 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/popup.js
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.html
--rw-r--r--   0 runner    (1001) docker     (127)   177879 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.js
--rw-r--r--   0 runner    (1001) docker     (127)    62942 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/pages/thankyou.js
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/runtime.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.273858 newshomepages-0.0.91/newshomepages/extensions/adguard/shared/
--rw-r--r--   0 runner    (1001) docker     (127)  1063347 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/shared/editor.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.273858 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)   176243 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/mobx.js
--rw-r--r--   0 runner    (1001) docker     (127)   135893 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/react.js
--rw-r--r--   0 runner    (1001) docker     (127)    50712 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/xstate.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.185857 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/1x1-transparent.gif
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/2x2-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/32x32-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/3x2-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopcss.css
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopframe.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjs.js
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjson.json
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/nooptext.js
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast02.xml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast03.xml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast04.xml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvmap01.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.193858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ar/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ar/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/be/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/be/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/bg/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/bg/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.281858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/cs/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/cs/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/da/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/da/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/de/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/en/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/en/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/es/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/es/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/et/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/et/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fa/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fa/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fi/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/he/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/he/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hr/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hu/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hu/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hy/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hy/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/id/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/id/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/it/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/it/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ja/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ko/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ko/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/lt/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/lt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/nl/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/nl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/no/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/no/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pl/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.285858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt-PT/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ro/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ro/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ru/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sl/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sl/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sv/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sv/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/tr/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/uk/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/vi/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/vi/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh-TW/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.193858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.289858 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_installed.png
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/content-script.js
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/options.js
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/popup.css
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/popup.html
--rw-r--r--   0 runner    (1001) docker     (127)   158820 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extensions/adguardextra/userscript.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.293858 newshomepages-0.0.91/newshomepages/extract/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/consolidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/hyperlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/lighthouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/robotstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/extract/wayback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/hyperlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/robotstxt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.293858 newshomepages-0.0.91/newshomepages/site/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/accessibility_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/bundle_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/bundle_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/country_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/country_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/drudge.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/language_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/language_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/latest_screenshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/performance_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/site_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/source_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/site/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.297858 newshomepages-0.0.91/newshomepages/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/bundles.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.321858 newshomepages-0.0.91/newshomepages/sources/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/20minutes.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/404mediaco.js
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/abc_es.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/adnkronos.js
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/andscape.js
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/arthasarokar.js
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/asahi.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/baltimorebanner.js
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/baltimoremag.js
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/baltimoresun.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bariweiss.js
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bbc.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/blaw.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bloombergjapan.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/bonginoreport.js
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/breitbartnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/calgaryherald.js
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/capradionews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/cbcnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/chess24com.js
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/chicagotribune.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/civilbeat.js
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/cnn.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/corriere.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/crucessunnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/daily_record.js
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dailycaller.js
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dailymirror.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dallasnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/diariope.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/dmregister.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/drudge.js
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/el_universal_mx.js
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/elcorreo_com.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/eltiempo.js
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/estadao.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/examinationnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/financialpost.js
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/fiquemsabendo.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/firstthingsmag.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/fortunemagazine.js
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/foxnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/france24.js
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/france24_en.js
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/franceinfo.js
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/frednewspost.js
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ft.js
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gazettedotcom.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gbpressgazette.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/georgiastraight.js
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gfherald.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/globalnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/globeandmail.js
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/gridnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/guardian.js
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/harpers.js
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/htrnews.js
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/humanevents.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ilmanifesto.js
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/independent.js
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/izvestia_ru.js
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/jdemontreal.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/jessicavalenti.js
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/jornaloglobo.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/journalsentinel.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kcautv.js
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kccinews.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kpbs.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/kpcc.js
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/laist.js
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lajornada.js
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lanacion.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/larazon_es.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lastampa.js
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/latimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lavozdegalicia.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/le_figaro.js
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/le_parisien.js
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ledevoir.js
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lehuffpost.js
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lemonde_en.js
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lemondefr.js
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/libe.js
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lobs.js
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/lp_lapresse.js
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/maroelamedia.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/mediapart.js
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/moreperfectus.js
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/motherjones.js
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/msnbc.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/mtlgazette.js
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/mtnstspotlight.js
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nationalpost.js
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nbcnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/news_letter.js
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/newshour.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nhk_news.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nikkei.js
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ntdaily.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nybooks.js
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/nytimes.js
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/oann.js
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/occrp.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/opensecretsdc.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/openvallejo.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/ottawacitizen.js
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/pajaropolitico.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/pioneerpress.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/platformer.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/postcrescent.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/presscitizen.js
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/propublica.js
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/publicintegrity.js
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/pulitzercenter.js
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/qctimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/realdailywire.js
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/repubblica.js
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/rfi.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sahanjournal.js
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sankei_news.js
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sdut.js
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/seikyoofficial.js
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sfchronicle.js
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sjvwater.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sowetanlive.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/spotlightpa.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/sputnikint.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/startribune.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/statnews.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/stevenspointjrl.js
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/teamtrace.js
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/telegraph.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theathletic.js
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thebabylonbee.js
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theblaze.js
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thedbk.js
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thedispatch.js
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theeconomist.js
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thehilltimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theintercept.js
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theinterceptbr.js
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theonion.js
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thephilacitizen.js
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/theriotimes.js
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thesun.js
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thetimes.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thetorontosun.js
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thetriibe.js
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/thewrap.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/timeslive.js
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/torontostar.js
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/tribunedelyon.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/usatoday.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/uvaldenews.js
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/vancouversun.js
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/vcstar.js
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/votebeatus.js
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/vryeweekblad.js
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/washingtonpost.js
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/wcfcourier.js
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/wonkette.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/javascript/zerohora.js
--rw-r--r--   0 runner    (1001) docker     (127)   115162 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/sources/sites.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/telegrammer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/toot.py
--rw-r--r--   0 runner    (1001) docker     (127)    29225 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 19:11:53.000000 newshomepages-0.0.91/newshomepages/wayback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:12:12.321858 newshomepages-0.0.91/newshomepages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26988 2024-04-09 19:12:12.000000 newshomepages-0.0.91/newshomepages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 19:12:11.000000 newshomepages-0.0.91/newshomepages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:12:12.321858 newshomepages-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-09 19:11:53.000000 newshomepages-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.572296 newshomepages-0.0.92/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.432296 newshomepages-0.0.92/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.devcontainer/postCreateCommand.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.432296 newshomepages-0.0.92/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.432296 newshomepages-0.0.92/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.github/ISSUE_TEMPLATE/add-a-site.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.github/ISSUE_TEMPLATE/report-a-broken-site.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.432296 newshomepages-0.0.92/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.github/workflows/site.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-14 15:36:01.000000 newshomepages-0.0.92/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-14 15:36:01.000000 newshomepages-0.0.92/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-14 15:36:01.000000 newshomepages-0.0.92/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 15:36:01.000000 newshomepages-0.0.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-14 15:36:01.000000 newshomepages-0.0.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-14 15:36:01.000000 newshomepages-0.0.92/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-14 15:36:21.572296 newshomepages-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-14 15:36:01.000000 newshomepages-0.0.92/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)   203156 2024-05-14 15:36:01.000000 newshomepages-0.0.92/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-14 15:36:01.000000 newshomepages-0.0.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 15:36:01.000000 newshomepages-0.0.92/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 15:36:01.000000 newshomepages-0.0.92/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.436296 newshomepages-0.0.92/newshomepages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/adstxt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/analyze/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/analyze/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/analyze/drudge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/analyze/lighthouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/analyze/us_right_wing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.424296 newshomepages-0.0.92/newshomepages/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.420296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ar/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/be/
+-rw-r--r--   0 runner    (1001) docker     (127)    39687 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/be/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/bg/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/bn/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/bn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ca/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/cs/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/da/
+-rw-r--r--   0 runner    (1001) docker     (127)    32176 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/da/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/de/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/el/
+-rw-r--r--   0 runner    (1001) docker     (127)    35861 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/el/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/en/
+-rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/en/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/es/
+-rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/es/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/es_419/
+-rw-r--r--   0 runner    (1001) docker     (127)    33470 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/es_419/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/et/
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/et/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.440296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)    24231 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fa/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)    32862 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fil/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fil/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)    34308 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/he/
+-rw-r--r--   0 runner    (1001) docker     (127)    35288 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/he/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hi/
+-rw-r--r--   0 runner    (1001) docker     (127)    21672 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)    34371 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hu/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hy/
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hy/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/id/
+-rw-r--r--   0 runner    (1001) docker     (127)    32258 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/id/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/it/
+-rw-r--r--   0 runner    (1001) docker     (127)    33384 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/it/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ja/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/kn/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/kn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ko/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)    21630 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/lt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/lv/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/lv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/mk-MK/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/mk-MK/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ms/
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ms/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.444296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/nb/
+-rw-r--r--   0 runner    (1001) docker     (127)    20450 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/nb/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)    33052 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/nl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)    33296 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (127)    33333 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pt_BR/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (127)    33264 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pt_PT/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)    33424 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ro/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)    40337 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ru/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)    32933 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sr-Latn/
+-rw-r--r--   0 runner    (1001) docker     (127)    31450 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ta/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/te/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/te/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/th/
+-rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/th/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)    33471 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/tr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)    39572 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/uk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)    35067 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/vi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.448296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (127)    31240 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/zh_CN/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.452296 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/zh_TW/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.420296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.452296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    22094 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/alert-popup.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/c3.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.452296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/layout.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/log.css
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/nanobar.css
+-rw-r--r--   0 runner    (1001) docker     (127)    54145 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.456296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    66004 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    66708 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    65764 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.456296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-off-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-off-38.png
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-on-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-on-38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/gray-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/gray-38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-128.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-38.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.460296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/app-store.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/avatar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/chrome.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/dropbox.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/filters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/google-play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/hero-green.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/hero-red.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo-shield.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo_adguard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/reload-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/shield.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/tick.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/toggler-bg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/trash.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.460296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/js/preload-theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.420296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.460296 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/libs/scriptlets/
+-rw-r--r--   0 runner    (1001) docker     (127)   141578 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.460296 newshomepages-0.0.92/newshomepages/extensions/adguard/content-script/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/content-script/subscribe.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.500296 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)  1206317 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    73188 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   313462 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    94026 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   402899 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2213341 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   928335 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   774091 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35060 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4655227 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   735758 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_224.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   914459 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   585242 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   496599 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   271134 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    69106 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   237431 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   483303 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    67127 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   256792 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    71645 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   363915 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1223256 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   899376 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   341390 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1640295 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   710272 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_224.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   806171 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   361755 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   193843 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   249182 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    58256 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   191331 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    51441 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filters.json
+-rw-r--r--   0 runner    (1001) docker     (127)   799078 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filters_i18n.json
+-rw-r--r--   0 runner    (1001) docker     (127)  1545375 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/filters/local_script_rules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.516296 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/ad-blocked.html
+-rw-r--r--   0 runner    (1001) docker     (127)   177876 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/ad-blocked.js
+-rw-r--r--   0 runner    (1001) docker     (127)   650939 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/assistant.js
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/background.html
+-rw-r--r--   0 runner    (1001) docker     (127)  3189967 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/background.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/content-script-end.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288034 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/content-script-start.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19803 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/devtools.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/devtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/filter-download.html
+-rw-r--r--   0 runner    (1001) docker     (127)    62185 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/filter-download.js
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/filtering-log.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1408341 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/filtering-log.js
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html
+-rw-r--r--   0 runner    (1001) docker     (127)   582536 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/options.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1079105 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/popup.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1072410 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/popup.js
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/safebrowsing.html
+-rw-r--r--   0 runner    (1001) docker     (127)   177879 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/safebrowsing.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62942 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/pages/thankyou.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/runtime.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.516296 newshomepages-0.0.92/newshomepages/extensions/adguard/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)  1063347 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/shared/editor.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.520296 newshomepages-0.0.92/newshomepages/extensions/adguard/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)   176243 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/vendors/mobx.js
+-rw-r--r--   0 runner    (1001) docker     (127)   135893 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/vendors/react.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50712 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/vendors/xstate.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.424296 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.524296 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/1x1-transparent.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/2x2-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/32x32-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/3x2-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopcss.css
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopframe.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopjson.json
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/nooptext.js
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast02.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast03.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvast04.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopvmap01.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.428296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ar/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/be/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/be/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/bg/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/cs/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/da/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/da/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/de/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/en/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/es/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/es/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/et/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/et/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fa/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/he/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/he/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hu/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hy/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hy/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/id/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/id/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.528296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/it/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/it/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ja/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ko/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ko/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/lt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/nl/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/nl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/no/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/no/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pt/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pt-PT/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ro/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ru/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sl/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sv/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/tr/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/uk/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/vi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/vi/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/zh/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/zh/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.532297 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/zh-TW/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.428296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.536296 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_installed.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/content-script.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/popup.css
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/popup.html
+-rw-r--r--   0 runner    (1001) docker     (127)   158820 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extensions/adguardextra/userscript.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.536296 newshomepages-0.0.92/newshomepages/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/consolidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/hyperlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/lighthouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/robotstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/extract/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/hyperlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/robotstxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.540296 newshomepages-0.0.92/newshomepages/site/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/accessibility_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/bundle_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/bundle_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/country_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/country_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/drudge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/language_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/language_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/latest_screenshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/performance_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/site_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/source_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/site/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.540296 newshomepages-0.0.92/newshomepages/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/bundles.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.572296 newshomepages-0.0.92/newshomepages/sources/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/20minutes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/404mediaco.js
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/abc_es.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/adnkronos.js
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/andscape.js
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/arthasarokar.js
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/asahi.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/baltimorebanner.js
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/baltimoremag.js
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/baltimoresun.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/bariweiss.js
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/bbc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/blaw.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/bloombergjapan.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/bonginoreport.js
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/breitbartnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/calgaryherald.js
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/capradionews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/cbcnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/chess24com.js
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/chicagotribune.js
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/civilbeat.js
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/cnn.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/corriere.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/crucessunnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/daily_record.js
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/dailycaller.js
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/dailymirror.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/dallasnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/diariope.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/dmregister.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/drudge.js
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/el_universal_mx.js
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/elcorreo_com.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/eltiempo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/estadao.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/examinationnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/financialpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/fiquemsabendo.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/firstthingsmag.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/fortunemagazine.js
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/foxnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/france24.js
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/france24_en.js
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/franceinfo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/frednewspost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/ft.js
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/gazettedotcom.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/gbpressgazette.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/georgiastraight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/gfherald.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/globalnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/globeandmail.js
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/gridnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/guardian.js
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/harpers.js
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/htrnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/humanevents.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/ilmanifesto.js
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/independent.js
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/izvestia_ru.js
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/jdemontreal.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/jessicavalenti.js
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/jornaloglobo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/journalsentinel.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/kcautv.js
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/kccinews.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/kpbs.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/kpcc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/laist.js
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lajornada.js
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lanacion.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/larazon_es.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lastampa.js
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/latimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lavozdegalicia.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/le_figaro.js
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/le_parisien.js
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/ledevoir.js
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lehuffpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lemonde_en.js
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lemondefr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/libe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lobs.js
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/lp_lapresse.js
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/maroelamedia.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/mediapart.js
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/moreperfectus.js
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/motherjones.js
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/msnbc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/mtlgazette.js
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/mtnstspotlight.js
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/nationalpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/nbcnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/news_letter.js
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/newshour.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/nhk_news.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/nikkei.js
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/ntdaily.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/nybooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/nytimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/oann.js
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/occrp.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/opensecretsdc.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/openvallejo.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/ottawacitizen.js
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/pajaropolitico.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/pioneerpress.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/platformer.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/postcrescent.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/presscitizen.js
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/propublica.js
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/publicintegrity.js
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/pulitzercenter.js
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/qctimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/realdailywire.js
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/repubblica.js
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/rfi.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/sahanjournal.js
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/sankei_news.js
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/sdut.js
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/seikyoofficial.js
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/sfchronicle.js
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/sjvwater.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/sowetanlive.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/spotlightpa.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/sputnikint.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/startribune.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/statnews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/stevenspointjrl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/teamtrace.js
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/telegraph.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/theathletic.js
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thebabylonbee.js
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/theblaze.js
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thedbk.js
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thedispatch.js
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/theeconomist.js
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thehilltimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/theintercept.js
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/theinterceptbr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/theonion.js
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thephilacitizen.js
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/theriotimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thesun.js
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thetimes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thetorontosun.js
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thetriibe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/thewrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/timeslive.js
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/torontostar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/tribunedelyon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/usatoday.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/uvaldenews.js
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/vancouversun.js
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/vcstar.js
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/votebeatus.js
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/vryeweekblad.js
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/washingtonpost.js
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/wcfcourier.js
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/wonkette.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/javascript/zerohora.js
+-rw-r--r--   0 runner    (1001) docker     (127)   115263 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/sources/sites.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/telegrammer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/toot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29225 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-14 15:36:01.000000 newshomepages-0.0.92/newshomepages/wayback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:36:21.572296 newshomepages-0.0.92/newshomepages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-14 15:36:21.000000 newshomepages-0.0.92/newshomepages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26988 2024-05-14 15:36:21.000000 newshomepages-0.0.92/newshomepages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:36:21.000000 newshomepages-0.0.92/newshomepages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-14 15:36:21.000000 newshomepages-0.0.92/newshomepages.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:36:21.000000 newshomepages-0.0.92/newshomepages.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-14 15:36:21.000000 newshomepages-0.0.92/newshomepages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 15:36:21.000000 newshomepages-0.0.92/newshomepages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:36:21.572296 newshomepages-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-14 15:36:01.000000 newshomepages-0.0.92/setup.py
```

### Comparing `newshomepages-0.0.91/.github/ISSUE_TEMPLATE/add-a-site.yaml` & `newshomepages-0.0.92/.github/ISSUE_TEMPLATE/add-a-site.yaml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/.github/workflows/continuous-deployment.yml` & `newshomepages-0.0.92/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/.github/workflows/site.yml` & `newshomepages-0.0.92/.github/workflows/site.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/.gitignore` & `newshomepages-0.0.92/.gitignore`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/.pre-commit-config.yaml` & `newshomepages-0.0.92/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/CODE_OF_CONDUCT.md` & `newshomepages-0.0.92/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/LICENSE` & `newshomepages-0.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/Makefile` & `newshomepages-0.0.92/Makefile`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/PKG-INFO` & `newshomepages-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newshomepages
-Version: 0.0.91
+Version: 0.0.92
 Summary: An open-source archive that gathers, saves, shares and analyzes news homepages
 Home-page: https://homepages.news
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: GPLv3
 Project-URL: Maintainer, https://palewi.re/who-is-ben-welsh/
 Project-URL: Source, https://github.com/palewire/news-homepages
```

### Comparing `newshomepages-0.0.91/Pipfile` & `newshomepages-0.0.92/Pipfile`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/Pipfile.lock` & `newshomepages-0.0.92/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980048500881834%*

 * *Differences: {"'default'": "{'idna': {'hashes': "*

 * *              "['sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc', "*

 * *              "'sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0'], "*

 * *              "'version': '==3.7', 'index': 'pypi'}, 'jinja2': {'hashes': "*

 * *              "['sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369', "*

 * *              "'sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d'], "*

 * *              '\'version\': […]*

```diff
@@ -422,19 +422,20 @@
                 "sha256:8915f5a3627c4d47b73e8202457cb28f1266982d1159bd5779d86a80c0eab1cd"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==0.26.0"
         },
         "idna": {
             "hashes": [
-                "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca",
-                "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
+                "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc",
+                "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"
             ],
+            "index": "pypi",
             "markers": "python_version >= '3.5'",
-            "version": "==3.6"
+            "version": "==3.7"
         },
         "internetarchive": {
             "hashes": [
                 "sha256:86c011e23751f5dff1d5cc6e3bc610b2eca3331d5e502c1cd34c2021068b6bbd"
             ],
             "index": "pypi",
             "version": "==3.6.0"
@@ -445,19 +446,20 @@
                 "sha256:fcd551b8dda66b44e9f9e6d6bbbee3a1145a22447c0a556e5d0fb1ad1e491719"
             ],
             "index": "pypi",
             "version": "==2.1.1"
         },
         "jinja2": {
             "hashes": [
-                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
-                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
+                "sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369",
+                "sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d"
             ],
             "index": "pypi",
-            "version": "==3.1.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.4"
         },
         "joblib": {
             "hashes": [
                 "sha256:92f865e621e17784e7955080b6d042489e3b8e294949cc44c6eac304f59772b1",
                 "sha256:ef4331c65f239985f3f2220ecc87db222f08fd22097a3dd5698f693875f8cbb9"
             ],
             "markers": "python_version >= '3.7'",
@@ -1381,19 +1383,20 @@
                 "sha256:b9c4510a8766d377033b6bace7e9f1f17a891383ced3c5d50c150f181e9e1cc2"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==5.1.1"
         },
         "tqdm": {
             "hashes": [
-                "sha256:1ee4f8a893eb9bef51c6e35730cebf234d5d0b6bd112b0271e10ed7c24a02bd9",
-                "sha256:6cd52cdf0fef0e0f543299cfc96fec90d7b8a7e88745f411ec33eb44d5ed3531"
+                "sha256:23097a41eba115ba99ecae40d06444c15d1c0c698d527a01c6c8bd1c5d0647e5",
+                "sha256:4f41d54107ff9a223dca80b53efe4fb654c67efaba7f47bada3ee9d50e05bd53"
             ],
+            "index": "pypi",
             "markers": "python_version >= '3.7'",
-            "version": "==4.66.2"
+            "version": "==4.66.3"
         },
         "typer": {
             "hashes": [
                 "sha256:50922fd79aea2f4751a8e0408ff10d2662bd0c8bbfa84755a699f3bada2978b2",
                 "sha256:5d96d986a21493606a358cae4461bd8cdf83cbf33a5aa950ae629ca3b51467ee"
             ],
             "markers": "python_version >= '3.6'",
@@ -1801,19 +1804,19 @@
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14",
-                "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"
+                "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad",
+                "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.2.0"
+            "version": "==1.2.1"
         },
         "execnet": {
             "hashes": [
                 "sha256:88256416ae766bc9e8895c76a87928c0012183da3cc4fc18016e6f050e025f41",
                 "sha256:cc59bc4423742fd71ad227122eb0dd44db51efb3dc4095b45ac9a08c770096af"
             ],
             "markers": "python_version >= '3.7'",
@@ -2382,19 +2385,19 @@
                 "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==4.2.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981",
-                "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
+                "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1",
+                "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==1.4.0"
+            "version": "==1.5.0"
         },
         "pockets": {
             "hashes": [
                 "sha256:68597934193c08a08eb2bf6a1d85593f627c22f9b065cc727a4f03f669d96d86",
                 "sha256:9320f1a3c6f7a9133fe3b571f283bcf3353cd70249025ae8d618e40e9f7e92b3"
             ],
             "version": "==0.9.1"
@@ -2467,20 +2470,20 @@
                 "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.17.2"
         },
         "pytest": {
             "hashes": [
-                "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7",
-                "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"
+                "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233",
+                "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==8.1.1"
+            "version": "==8.2.0"
         },
         "pytest-cov": {
             "hashes": [
                 "sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652",
                 "sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857"
             ],
             "index": "pypi",
```

### Comparing `newshomepages-0.0.91/README.md` & `newshomepages-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/accessibility.py` & `newshomepages-0.0.92/newshomepages/accessibility.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/adstxt.py` & `newshomepages-0.0.92/newshomepages/adstxt.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/analyze/drudge.py` & `newshomepages-0.0.92/newshomepages/analyze/drudge.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/analyze/lighthouse.py` & `newshomepages-0.0.92/newshomepages/analyze/lighthouse.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/analyze/us_right_wing.py` & `newshomepages-0.0.92/newshomepages/analyze/us_right_wing.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/archive.py` & `newshomepages-0.0.92/newshomepages/archive.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/batch.py` & `newshomepages-0.0.92/newshomepages/batch.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ar/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ar/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/be/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/be/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/bg/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/bg/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ca/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ca/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/cs/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/cs/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/da/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/da/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/de/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/de/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/el/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/el/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/en/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/en/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/es/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/es_419/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/es_419/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/et/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/et/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fa/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fa/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fi/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/fr/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/fr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/he/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/he/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hi/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hr/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hu/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hu/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/hy/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/hy/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/id/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/id/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/it/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/it/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ja/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ja/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ko/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ko/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/lt/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/lt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ms/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ms/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nb/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/nb/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/nl/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/nl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pl/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_BR/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pt_BR/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/pt_PT/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/pt_PT/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ro/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ro/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/ru/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/ru/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sk/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sl/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sr-Latn/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/sv/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/sv/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/th/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/th/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/tr/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/tr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/uk/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/uk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/vi/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/vi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_CN/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/zh_CN/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/_locales/zh_TW/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/_locales/zh_TW/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/alert-popup.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/alert-popup.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/c3.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/c3.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/custom.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/custom.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/dark.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/dark.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/elementsPanel.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/inspectorCommon.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/inspectorStyle.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/inspectorSyntaxHighlight.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/devtools/sidebarPane.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/layout.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/layout.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/log.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/log.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/css/style.css` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/fonts/Roboto-Bold.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/fonts/Roboto-Medium.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/fonts/Roboto-Regular.woff2`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-19.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-off-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-off-38.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-off-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-19.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-on-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/b13-on-38.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/b13-on-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-19.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/gray-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/gray-38.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/gray-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-128.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-128.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-16.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-16.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-19.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/icons/green-38.png` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/icons/green-38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/alert.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/alert.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/app-store.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/app-store.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/arrow-down-grey.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/arrow-down.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/arrow-down.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/avatar.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/avatar.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/checked.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/checked.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/chrome.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/chrome.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/cross.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/cross.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/dropbox.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/dropbox.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/favicon.ico` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/filters.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/filters.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/google-play.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/google-play.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-green.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/hero-green.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/hero-red.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/hero-red.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-dark.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo-shield.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo-shield.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/logo_adguard.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/logo_adguard.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/reload-ico-green.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/reload-ico.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/reload-ico.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/tick.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/tick.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/images/toggler-bg.svg` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/images/toggler-bg.svg`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/js/preload-theme.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/js/preload-theme.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml` & `newshomepages-0.0.92/newshomepages/extensions/adguard/assets/libs/scriptlets/redirects.yml`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/content-script/subscribe.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/content-script/subscribe.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_1.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_1.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_10.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_10.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_11.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_11.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_12.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_12.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_13.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_13.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_14.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_14.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_15.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_15.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_16.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_16.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_17.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_17.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_2.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_2.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_224.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_224.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_3.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_3.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_4.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_4.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_5.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_5.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_6.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_6.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_7.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_7.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_8.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_8.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_9.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_9.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_1.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_1.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_10.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_10.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_11.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_11.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_12.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_12.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_13.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_13.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_14.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_14.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_15.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_15.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_16.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_16.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_17.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_17.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_2.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_2.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_224.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_224.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_3.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_3.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_4.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_4.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_5.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_5.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_6.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_6.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_7.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_7.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_8.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_8.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filter_mobile_9.txt` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filter_mobile_9.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filters.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/filters_i18n.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/filters_i18n.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/filters/local_script_rules.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/filters/local_script_rules.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/manifest.json` & `newshomepages-0.0.92/newshomepages/extensions/adguard/manifest.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/ad-blocked.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/ad-blocked.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/assistant.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/assistant.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/background.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/background.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-end.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/content-script-end.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/content-script-start.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/content-script-start.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/devtools-elements-sidebar.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/devtools.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/devtools.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.html` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/filter-download.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filter-download.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/filter-download.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/filtering-log.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/filtering-log.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/fullscreen-user-rules.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/fullscreen-user-rules.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.html` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/options.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/options.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/options.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/popup.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/popup.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.html` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/safebrowsing.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/safebrowsing.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/safebrowsing.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/pages/thankyou.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/pages/thankyou.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/runtime.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/runtime.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/shared/editor.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/shared/editor.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/mobx.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/vendors/mobx.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/react.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/vendors/react.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/vendors/xstate.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/vendors/xstate.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/amazon-apstag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/ati-smarttag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/click2load.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/didomi-loader.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs2.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/fingerprintjs3.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/gemius.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics-ga.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-analytics.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/google-ima3.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/googlesyndication-adsbygoogle.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagmanager-gtm.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/googletagservices-gpt.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/matomo.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-tag.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/metrika-yandex-watch.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/naver-wcslog.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noeval.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp3.mp3`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/noopmp4.mp4`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid-ads.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prebid.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-bab2.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-fab-3.2.0.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/prevent-popads-net.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/scorecardresearch-beacon.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js` & `newshomepages-0.0.92/newshomepages/extensions/adguard/web-accessible-resources/redirects/set-popads-dummy.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/be/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/be/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/cs/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/cs/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/da/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/da/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/de/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/de/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/en/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/en/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/es/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/es/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fi/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/fr/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/fr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/he/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/he/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hr/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/hu/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/hu/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/id/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/id/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/it/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/it/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ja/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ja/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ko/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ko/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/lt/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/lt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/nl/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/nl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/no/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/no/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pl/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pt/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/pt-PT/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ro/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ro/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/ru/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/ru/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sk/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sl/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sl/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/sr/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/sr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/tr/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/tr/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/uk/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/uk/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/vi/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/vi/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/zh/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/_locales/zh-TW/messages.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_128.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_16.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_19.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_icon_38.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_installed.png` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_installed.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/assets/images/extra_logo.png` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/assets/images/extra_logo.png`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/content-script.js` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/content-script.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/manifest.json` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/manifest.json`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/options.js` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/options.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/popup.html` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/popup.html`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extensions/adguardextra/userscript.js` & `newshomepages-0.0.92/newshomepages/extensions/adguardextra/userscript.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/accessibility.py` & `newshomepages-0.0.92/newshomepages/extract/accessibility.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/cli.py` & `newshomepages-0.0.92/newshomepages/extract/cli.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/consolidate.py` & `newshomepages-0.0.92/newshomepages/extract/consolidate.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/hyperlinks.py` & `newshomepages-0.0.92/newshomepages/extract/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/items.py` & `newshomepages-0.0.92/newshomepages/extract/items.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/lighthouse.py` & `newshomepages-0.0.92/newshomepages/extract/lighthouse.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/robotstxt.py` & `newshomepages-0.0.92/newshomepages/extract/robotstxt.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/utils.py` & `newshomepages-0.0.92/newshomepages/extract/utils.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/extract/wayback.py` & `newshomepages-0.0.92/newshomepages/extract/wayback.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/hyperlinks.py` & `newshomepages-0.0.92/newshomepages/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/mosaic.py` & `newshomepages-0.0.92/newshomepages/mosaic.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/robotstxt.py` & `newshomepages-0.0.92/newshomepages/robotstxt.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/rss.py` & `newshomepages-0.0.92/newshomepages/rss.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/screenshot.py` & `newshomepages-0.0.92/newshomepages/screenshot.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/accessibility_ranking.py` & `newshomepages-0.0.92/newshomepages/site/accessibility_ranking.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/bundle_detail.py` & `newshomepages-0.0.92/newshomepages/site/bundle_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/cli.py` & `newshomepages-0.0.92/newshomepages/site/cli.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/country_detail.py` & `newshomepages-0.0.92/newshomepages/site/country_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/country_list.py` & `newshomepages-0.0.92/newshomepages/site/country_list.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/drudge.py` & `newshomepages-0.0.92/newshomepages/site/drudge.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/language_detail.py` & `newshomepages-0.0.92/newshomepages/site/language_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/language_list.py` & `newshomepages-0.0.92/newshomepages/site/language_list.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/latest_screenshots.py` & `newshomepages-0.0.92/newshomepages/site/latest_screenshots.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/openai.py` & `newshomepages-0.0.92/newshomepages/site/openai.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/performance_ranking.py` & `newshomepages-0.0.92/newshomepages/site/performance_ranking.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/site_detail.py` & `newshomepages-0.0.92/newshomepages/site/site_detail.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/status_report.py` & `newshomepages-0.0.92/newshomepages/site/status_report.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/site/utils.py` & `newshomepages-0.0.92/newshomepages/site/utils.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/slack.py` & `newshomepages-0.0.92/newshomepages/slack.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/sources/bundles.csv` & `newshomepages-0.0.92/newshomepages/sources/bundles.csv`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/sources/javascript/news_letter.js` & `newshomepages-0.0.92/newshomepages/sources/javascript/news_letter.js`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/sources/sites.csv` & `newshomepages-0.0.92/newshomepages/sources/sites.csv`

 * *Files 0% similar despite different names*

```diff
@@ -699,14 +699,15 @@
 nextcityorg,https://nextcity.org/,Next City,Philadelphia,America/New_York,US,en,pennsylvania|philadelphia,,
 nhk_news,https://www3.nhk.or.jp/news/,NHK,Tokyo,Asia/Tokyo,JP,ja,,,
 nhpr,https://www.nhpr.org/,New Hampshire Public Radio,Manchester,America/New_York,US,en,new-hampshire,,
 nhregister,https://www.nhregister.com/,New Haven Register,New Haven,America/New_York,US,en,connecticut,,
 niemanlab,https://www.niemanlab.org/,Nieman Lab,Cambridge,America/New_York,US,en,massachusetts,,
 nikkei,https://www.nikkei.com/,Nikkei,Tokyo,Asia/Tokyo,JP,ja,,,
 njherald,https://www.njherald.com/,New Jersey Herald,Newton,America/New_York,US,en,new-jersey|gannett,,
+not_the_bee,https://notthebee.com/,Not the Bee,Jupiter,America/New_York,US,en,us-right-wing|satire,,
 northjersey,https://www.northjersey.com/,northjersey.com,Hackensack,America/New_York,US,en,new-jersey|gannett,,
 norwichbulletin,https://www.norwichbulletin.com/,The Norwich Bulletin,Norwich,America/New_York,US,en,connecticut|gannett,,
 novayagazeta_eu,https://novayagazeta.eu/,Novaya Gazeta,Moscow,Europe/Moscow,RU,ru,,,
 npr,https://www.npr.org/,NPR,Washington,America/New_York,US,en,us-national,,
 nrk,https://www.nrk.no/,NRK,Oslo,Europe/Oslo,NO,no,,,
 nro,https://www.nationalreview.com/,National Review,Washington,America/New_York,US,en,us-right-wing,,
 ntdaily,https://www.ntdaily.com/,North Texas Daily,Denton,America/Chicago,US,en,texas,,
```

### Comparing `newshomepages-0.0.91/newshomepages/telegrammer.py` & `newshomepages-0.0.92/newshomepages/telegrammer.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/toot.py` & `newshomepages-0.0.92/newshomepages/toot.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/utils.py` & `newshomepages-0.0.92/newshomepages/utils.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages/wayback.py` & `newshomepages-0.0.92/newshomepages/wayback.py`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages.egg-info/PKG-INFO` & `newshomepages-0.0.92/newshomepages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newshomepages
-Version: 0.0.91
+Version: 0.0.92
 Summary: An open-source archive that gathers, saves, shares and analyzes news homepages
 Home-page: https://homepages.news
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: GPLv3
 Project-URL: Maintainer, https://palewi.re/who-is-ben-welsh/
 Project-URL: Source, https://github.com/palewire/news-homepages
```

### Comparing `newshomepages-0.0.91/newshomepages.egg-info/SOURCES.txt` & `newshomepages-0.0.92/newshomepages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/newshomepages.egg-info/entry_points.txt` & `newshomepages-0.0.92/newshomepages.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `newshomepages-0.0.91/setup.py` & `newshomepages-0.0.92/setup.py`

 * *Files identical despite different names*

