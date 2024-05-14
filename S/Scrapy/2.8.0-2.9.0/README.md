# Comparing `tmp/Scrapy-2.8.0.tar.gz` & `tmp/Scrapy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapy-2.8.0.tar", last modified: Thu Feb  2 04:54:56 2023, max compression
+gzip compressed data, was "Scrapy-2.9.0.tar", last modified: Mon May  8 10:55:27 2023, max compression
```

## Comparing `Scrapy-2.8.0.tar` & `Scrapy-2.9.0.tar`

### file list

```diff
@@ -1,543 +1,542 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.330201 Scrapy-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-02 04:54:40.000000 Scrapy-2.8.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-02 04:54:40.000000 Scrapy-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-02 04:54:40.000000 Scrapy-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-02 04:54:40.000000 Scrapy-2.8.0/NEWS
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-02-02 04:54:56.330201 Scrapy-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-02-02 04:54:40.000000 Scrapy-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.250197 Scrapy-2.8.0/Scrapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-02-02 04:54:56.000000 Scrapy-2.8.0/Scrapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-02-02 04:54:56.000000 Scrapy-2.8.0/Scrapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 04:54:56.000000 Scrapy-2.8.0/Scrapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-02 04:54:56.000000 Scrapy-2.8.0/Scrapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 04:54:56.000000 Scrapy-2.8.0/Scrapy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-02 04:54:56.000000 Scrapy-2.8.0/Scrapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-02 04:54:56.000000 Scrapy-2.8.0/Scrapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-02 04:54:40.000000 Scrapy-2.8.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-02-02 04:54:40.000000 Scrapy-2.8.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.254197 Scrapy-2.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.254197 Scrapy-2.8.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/_ext/scrapydocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.254197 Scrapy-2.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/_static/selectors-sample1.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.254197 Scrapy-2.8.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.254197 Scrapy-2.8.0/docs/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/_tests/quotes.html
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/_tests/quotes1.html
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.258197 Scrapy-2.8.0/docs/intro/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/intro/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/intro/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/intro/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29876 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/intro/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)   243245 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/news.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.270198 Scrapy-2.8.0/docs/topics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.270198 Scrapy-2.8.0/docs/topics/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    53922 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/_images/inspector_01.png
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/_images/network_01.png
--rw-r--r--   0 runner    (1001) docker     (123)    82702 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/_images/network_02.png
--rw-r--r--   0 runner    (1001) docker     (123)    45506 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/_images/network_03.png
--rw-r--r--   0 runner    (1001) docker     (123)    19653 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/_images/scrapy_architecture.odg
--rw-r--r--   0 runner    (1001) docker     (123)    92558 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/_images/scrapy_architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)    53978 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/_images/scrapy_architecture_02.png
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/autothrottle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/benchmarking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/broad-crawls.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/coroutines.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/debug.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/developer-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/djangoitem.rst
--rw-r--r--   0 runner    (1001) docker     (123)    39774 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/downloader-middleware.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/dynamic-content.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/email.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15472 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/exporters.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/feed-exports.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/item-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/items.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/leaks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/link-extractors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16589 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/loaders.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25932 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/media-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/practices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    48009 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/request-response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/scheduler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/scrapyd.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34983 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/selectors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    49593 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/shell.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/signals.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/spider-middleware.rst
--rw-r--r--   0 runner    (1001) docker     (123)    32291 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/spiders.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/topics/telnetconsole.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.274198 Scrapy-2.8.0/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/utils/linkfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-02 04:54:40.000000 Scrapy-2.8.0/docs/versioning.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.274198 Scrapy-2.8.0/extras/
--rwxr-xr-x   0 runner    (1001) docker     (123)      259 2023-02-02 04:54:40.000000 Scrapy-2.8.0/extras/coverage-report.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-02-02 04:54:40.000000 Scrapy-2.8.0/extras/qps-bench-server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-02 04:54:40.000000 Scrapy-2.8.0/extras/qpsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-02 04:54:40.000000 Scrapy-2.8.0/extras/scrapy.1
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-02 04:54:40.000000 Scrapy-2.8.0/extras/scrapy_bash_completion
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-02-02 04:54:40.000000 Scrapy-2.8.0/extras/scrapy_zsh_completion
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-02 04:54:40.000000 Scrapy-2.8.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.282198 Scrapy-2.8.0/scrapy/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/cmdline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.282198 Scrapy-2.8.0/scrapy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/genspider.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/runspider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/startproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/commands/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.282198 Scrapy-2.8.0/scrapy/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/contracts/default.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.282198 Scrapy-2.8.0/scrapy/core/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.282198 Scrapy-2.8.0/scrapy/core/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/contextfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.286198 Scrapy-2.8.0/scrapy/core/downloader/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/datauri.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/http10.py
--rw-r--r--   0 runner    (1001) docker     (123)    24231 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/http11.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/http2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/handlers/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/downloader/webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.286198 Scrapy-2.8.0/scrapy/core/http2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/http2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/http2/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    16717 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/http2/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    19140 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/http2/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/core/spidermw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.286198 Scrapy-2.8.0/scrapy/downloadermiddlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/ajaxcrawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/defaultheaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/downloadtimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/httpauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/httpcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/httpcompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/httpproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/robotstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/downloadermiddlewares/useragent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/dupefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/closespider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/corestats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    22072 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/feedexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/httpcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/logstats.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/memdebug.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/memusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/spiderstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/statsmailer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/telnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/extensions/throttle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/http/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/http/request/
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/request/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/request/json_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/request/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/http/response/
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/response/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/response/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/http/response/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/linkextractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/linkextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/linkextractors/lxmlhtml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/loader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/loader/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/logformatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/mime.types
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/pipelines/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/pipelines/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/pipelines/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/pqueues.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/responsetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/robotstxt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/selector/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/selector/unified.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/settings/
--rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/settings/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/signalmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spiderloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.290199 Scrapy-2.8.0/scrapy/spidermiddlewares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spidermiddlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spidermiddlewares/depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spidermiddlewares/httperror.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spidermiddlewares/offsite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13893 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spidermiddlewares/referer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spidermiddlewares/urllength.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.294199 Scrapy-2.8.0/scrapy/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spiders/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spiders/feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spiders/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/spiders/sitemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/squeues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/statscollectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.238196 Scrapy-2.8.0/scrapy/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.294199 Scrapy-2.8.0/scrapy/templates/project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.294199 Scrapy-2.8.0/scrapy/templates/project/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/project/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/project/module/items.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/project/module/settings.py.tmpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.294199 Scrapy-2.8.0/scrapy/templates/project/module/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/project/module/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/project/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.294199 Scrapy-2.8.0/scrapy/templates/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/spiders/basic.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/spiders/crawl.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/spiders/csvfeed.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/templates/spiders/xmlfeed.tmpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.298199 Scrapy-2.8.0/scrapy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/asyncgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/benchserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/boto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/curl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/gz.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/httpobj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/ossignal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/reqser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/sitemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/testproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/testsite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/trackref.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-02 04:54:40.000000 Scrapy-2.8.0/scrapy/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-02 04:54:56.330201 Scrapy-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-02-02 04:54:40.000000 Scrapy-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.310200 Scrapy-2.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.314200 Scrapy-2.8.0/tests/CrawlerProcess/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/asyncio_custom_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/asyncio_deferred_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/asyncio_enabled_no_reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/asyncio_enabled_reactor.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/caching_hostname_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/default_name_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/reactor_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/reactor_default_twisted_reactor_select.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/reactor_select.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/reactor_select_twisted_reactor_select.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_custom_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.314200 Scrapy-2.8.0/tests/CrawlerRunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/CrawlerRunner/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/ftpserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/ignores.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.314200 Scrapy-2.8.0/tests/keys/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/example-com.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/example-com.conf
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/example-com.gen.README
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/example-com.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/localhost-ip.gen.README
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/localhost.gen.README
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/localhost.ip.crt
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/localhost.ip.key
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/keys/mitmproxy-ca.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.314200 Scrapy-2.8.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/mocks/dummydbm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/mockserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.242196 Scrapy-2.8.0/tests/sample_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.318200 Scrapy-2.8.0/tests/sample_data/compressed/
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.tar
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.xml.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.xml.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.zip
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/html-br.bin
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/html-gzip.bin
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/html-rawdeflate.bin
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/html-zlibdeflate.bin
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/html-zstd-static-content-size.bin
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/html-zstd-static-no-content-size.bin
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/truncated-crc-error-short.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/truncated-crc-error.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/unexpected-eof-output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/compressed/unexpected-eof.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.322200 Scrapy-2.8.0/tests/sample_data/feeds/
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/feeds/feed-sample1.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/feeds/feed-sample2.xml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/feeds/feed-sample3.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/feeds/feed-sample4.csv
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/feeds/feed-sample5.csv
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/feeds/feed-sample6.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.322200 Scrapy-2.8.0/tests/sample_data/link_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/link_extractor/linkextractor.html
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/link_extractor/linkextractor_latin1.html
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/link_extractor/linkextractor_no_href.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/link_extractor/linkextractor_noenc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.322200 Scrapy-2.8.0/tests/sample_data/test_site/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.242196 Scrapy-2.8.0/tests/sample_data/test_site/files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.322200 Scrapy-2.8.0/tests/sample_data/test_site/files/images/
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/test_site/files/images/python-powered-h-50x65.png
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/test_site/files/images/scrapy.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/test_site/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/test_site/item1.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/sample_data/test_site/item2.html
--rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/spiders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_closespider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.322200 Scrapy-2.8.0/tests/test_cmdline/
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.322200 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.322200 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.326200 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_command_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_command_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_command_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_command_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_command_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    36027 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_core_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27521 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21639 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    48356 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloader_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloader_handlers_http2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_ajaxcrawlable.py
--rw-r--r--   0 runner    (1001) docker     (123)    28200 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_defaultheaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_downloadtimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_httpauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25835 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_httpcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_httpcompression.py
--rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_httpproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_robotstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_downloadermiddleware_useragent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_dupefilters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_engine_stop_download_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_engine_stop_download_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21912 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_extension_telnet.py
--rw-r--r--   0 runner    (1001) docker     (123)   102299 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_feedexport.py
--rw-r--r--   0 runner    (1001) docker     (123)    24027 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_http2_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_http_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_http_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    65265 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    39197 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_http_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    32026 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_linkextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21141 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    26618 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_loader_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_logformatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_pipeline_crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_pipeline_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    25450 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_pipeline_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_pipeline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_pqueues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_proxy_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_request_attribute_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_request_cb_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_request_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_request_left.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_responsetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_robotstxt_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_scheduler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.326200 Scrapy-2.8.0/tests/test_settings/
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_settings/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.326200 Scrapy-2.8.0/tests/test_spiderloader/
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.326200 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.326200 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/nested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/nested/spider4.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/spider0.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/spider1.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/spider2.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderloader/test_spiders/spider3.py
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spidermiddleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spidermiddleware_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spidermiddleware_httperror.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spidermiddleware_offsite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spidermiddleware_output_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    43427 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spidermiddleware_referer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spidermiddleware_urllength.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_spiderstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_squeues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_squeues_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_toplevel.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_urlparse_monkeypatches.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_asyncgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_curl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_gz.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_httpobj.py
--rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.326200 Scrapy-2.8.0/tests/test_utils_misc/
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_misc/test.egg
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_misc/test_return_with_argument_inside_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.326200 Scrapy-2.8.0/tests/test_utils_misc/test_walk_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_misc/test_walk_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:56.330201 Scrapy-2.8.0/tests/test_utils_misc/test_walk_modules/mod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_misc/test_walk_modules/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_misc/test_walk_modules/mod/mod0.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_misc/test_walk_modules/mod1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_python.py
--rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_sitemap.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_trackref.py
--rw-r--r--   0 runner    (1001) docker     (123)    22553 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_utils_url.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/test_webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tests/upper-constraints.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-02-02 04:54:40.000000 Scrapy-2.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.388879 Scrapy-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-08 10:55:10.000000 Scrapy-2.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-08 10:55:10.000000 Scrapy-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 10:55:10.000000 Scrapy-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 10:55:10.000000 Scrapy-2.9.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-08 10:55:27.388879 Scrapy-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-08 10:55:10.000000 Scrapy-2.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.312875 Scrapy-2.9.0/Scrapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-08 10:55:27.000000 Scrapy-2.9.0/Scrapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-05-08 10:55:27.000000 Scrapy-2.9.0/Scrapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:55:27.000000 Scrapy-2.9.0/Scrapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 10:55:27.000000 Scrapy-2.9.0/Scrapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 10:55:27.000000 Scrapy-2.9.0/Scrapy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 10:55:27.000000 Scrapy-2.9.0/Scrapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 10:55:27.000000 Scrapy-2.9.0/Scrapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 10:55:10.000000 Scrapy-2.9.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-08 10:55:10.000000 Scrapy-2.9.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.316875 Scrapy-2.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.316875 Scrapy-2.9.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/_ext/scrapydocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.316875 Scrapy-2.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/_static/selectors-sample1.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.316875 Scrapy-2.9.0/docs/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/_tests/quotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/_tests/quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.316875 Scrapy-2.9.0/docs/intro/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/intro/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/intro/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/intro/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30722 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/intro/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   247533 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/news.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.320875 Scrapy-2.9.0/docs/topics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.324876 Scrapy-2.9.0/docs/topics/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    53922 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/_images/inspector_01.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/_images/network_01.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82702 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/_images/network_02.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45506 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/_images/network_03.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19653 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/_images/scrapy_architecture.odg
+-rw-r--r--   0 runner    (1001) docker     (123)    92558 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/_images/scrapy_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53978 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/_images/scrapy_architecture_02.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/autothrottle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/benchmarking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/broad-crawls.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/coroutines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/debug.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13859 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/developer-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/djangoitem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    39941 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/downloader-middleware.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/dynamic-content.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/email.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15581 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/exporters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23099 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/feed-exports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/item-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/items.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/leaks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/link-extractors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26684 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/media-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/practices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    48655 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/request-response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/scheduler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/scrapyd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    37989 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/selectors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    50704 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/shell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16976 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/spider-middleware.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/spiders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/topics/telnetconsole.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.324876 Scrapy-2.9.0/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/utils/linkfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-08 10:55:10.000000 Scrapy-2.9.0/docs/versioning.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.324876 Scrapy-2.9.0/extras/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      259 2023-05-08 10:55:10.000000 Scrapy-2.9.0/extras/coverage-report.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1618 2023-05-08 10:55:10.000000 Scrapy-2.9.0/extras/qps-bench-server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-08 10:55:10.000000 Scrapy-2.9.0/extras/qpsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-08 10:55:10.000000 Scrapy-2.9.0/extras/scrapy.1
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-08 10:55:10.000000 Scrapy-2.9.0/extras/scrapy_bash_completion
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-08 10:55:10.000000 Scrapy-2.9.0/extras/scrapy_zsh_completion
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-08 10:55:10.000000 Scrapy-2.9.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.328876 Scrapy-2.9.0/scrapy/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.332876 Scrapy-2.9.0/scrapy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/genspider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11977 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/runspider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/startproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/commands/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.332876 Scrapy-2.9.0/scrapy/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/contracts/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.332876 Scrapy-2.9.0/scrapy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.332876 Scrapy-2.9.0/scrapy/core/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/contextfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.336876 Scrapy-2.9.0/scrapy/core/downloader/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/datauri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/http10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24230 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/http11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/http2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/handlers/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/downloader/webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.336876 Scrapy-2.9.0/scrapy/core/http2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/http2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/http2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17089 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/http2/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/http2/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/core/spidermw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15026 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.336876 Scrapy-2.9.0/scrapy/downloadermiddlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/ajaxcrawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/defaultheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/downloadtimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/httpauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/httpcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/httpcompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/httpproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/robotstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/downloadermiddlewares/useragent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/dupefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.340876 Scrapy-2.9.0/scrapy/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/closespider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/corestats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23049 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/feedexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14726 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/httpcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/logstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/memdebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/spiderstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/statsmailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/extensions/throttle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.340876 Scrapy-2.9.0/scrapy/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.340876 Scrapy-2.9.0/scrapy/http/request/
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/request/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/request/json_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/request/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/http/response/
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/response/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/response/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/http/response/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/linkextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/linkextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/linkextractors/lxmlhtml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/loader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/loader/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/logformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/mime.types
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20897 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/pipelines/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/pipelines/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/pipelines/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/pqueues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/responsetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/robotstxt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/selector/unified.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/settings/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/signalmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spiderloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/spidermiddlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spidermiddlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spidermiddlewares/depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spidermiddlewares/httperror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spidermiddlewares/offsite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spidermiddlewares/referer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spidermiddlewares/urllength.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.344877 Scrapy-2.9.0/scrapy/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spiders/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spiders/feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spiders/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/spiders/sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/squeues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/statscollectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.308875 Scrapy-2.9.0/scrapy/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.348877 Scrapy-2.9.0/scrapy/templates/project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.348877 Scrapy-2.9.0/scrapy/templates/project/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/project/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/project/module/items.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/project/module/settings.py.tmpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.348877 Scrapy-2.9.0/scrapy/templates/project/module/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/project/module/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/project/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.348877 Scrapy-2.9.0/scrapy/templates/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/spiders/basic.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/spiders/crawl.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/templates/spiders/xmlfeed.tmpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.356877 Scrapy-2.9.0/scrapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/asyncgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/benchserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/gz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/httpobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/ossignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/reqser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/testproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/testsite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/trackref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-08 10:55:10.000000 Scrapy-2.9.0/scrapy/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-08 10:55:27.388879 Scrapy-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-08 10:55:10.000000 Scrapy-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.372878 Scrapy-2.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.376879 Scrapy-2.9.0/tests/CrawlerProcess/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/asyncio_custom_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/asyncio_deferred_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/asyncio_enabled_no_reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/asyncio_enabled_reactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/caching_hostname_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/default_name_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/reactor_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/reactor_default_twisted_reactor_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/reactor_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/reactor_select_twisted_reactor_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_custom_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.376879 Scrapy-2.9.0/tests/CrawlerRunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/CrawlerRunner/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/ftpserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/ignores.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.380879 Scrapy-2.9.0/tests/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/example-com.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/example-com.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/example-com.gen.README
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/example-com.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/localhost-ip.gen.README
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/localhost.gen.README
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/localhost.ip.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/localhost.ip.key
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/keys/mitmproxy-ca.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.380879 Scrapy-2.9.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/mocks/dummydbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/mockserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.308875 Scrapy-2.9.0/tests/sample_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.380879 Scrapy-2.9.0/tests/sample_data/compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.tar
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.xml.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.xml.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/html-br.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/html-gzip.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/html-rawdeflate.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/html-zlibdeflate.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/html-zstd-static-content-size.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/html-zstd-static-no-content-size.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/truncated-crc-error-short.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/truncated-crc-error.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/unexpected-eof-output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/compressed/unexpected-eof.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/sample_data/feeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/feeds/feed-sample1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/feeds/feed-sample2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/feeds/feed-sample3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/feeds/feed-sample4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/feeds/feed-sample5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/feeds/feed-sample6.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/sample_data/link_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/link_extractor/linkextractor.html
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/link_extractor/linkextractor_latin1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/link_extractor/linkextractor_no_href.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/link_extractor/linkextractor_noenc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/sample_data/test_site/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.308875 Scrapy-2.9.0/tests/sample_data/test_site/files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/sample_data/test_site/files/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/test_site/files/images/python-powered-h-50x65.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/test_site/files/images/scrapy.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/test_site/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/test_site/item1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/sample_data/test_site/item2.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/spiders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_closespider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/test_cmdline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/test_spider/spiders/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_command_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_command_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_command_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_command_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_command_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38178 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_core_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27521 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21639 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48356 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloader_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloader_handlers_http2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_ajaxcrawlable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28200 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_defaultheaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_downloadtimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_httpauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25829 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_httpcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_httpcompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_httpproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_robotstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloadermiddleware_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_downloaderslotssettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_dupefilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19528 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_engine_stop_download_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_engine_stop_download_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21904 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_extension_telnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106764 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_feedexport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24150 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_http2_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_http_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_http_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65262 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39832 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_http_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33209 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_linkextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21140 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_loader_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_logformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_pipeline_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24959 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_pipeline_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25447 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_pipeline_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22766 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_pipeline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_pqueues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_proxy_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_request_attribute_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_request_cb_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_request_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_request_left.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_responsetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_robotstxt_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_scheduler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/test_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_settings/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25192 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.384879 Scrapy-2.9.0/tests/test_spiderloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.388879 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.388879 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/nested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/nested/spider4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/spider0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/spider1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/spider2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderloader/test_spiders/spider3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spidermiddleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spidermiddleware_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spidermiddleware_httperror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spidermiddleware_offsite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spidermiddleware_output_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43421 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spidermiddleware_referer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spidermiddleware_urllength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_spiderstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_squeues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_squeues_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_urlparse_monkeypatches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_asyncgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_gz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_httpobj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20608 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.388879 Scrapy-2.9.0/tests/test_utils_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_misc/test.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_misc/test_return_with_argument_inside_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.388879 Scrapy-2.9.0/tests/test_utils_misc/test_walk_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_misc/test_walk_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:27.388879 Scrapy-2.9.0/tests/test_utils_misc/test_walk_modules/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_misc/test_walk_modules/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_misc/test_walk_modules/mod/mod0.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_misc/test_walk_modules/mod1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_sitemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_trackref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22553 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_utils_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/test_webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tests/upper-constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-08 10:55:10.000000 Scrapy-2.9.0/tox.ini
```

### Comparing `Scrapy-2.8.0/AUTHORS` & `Scrapy-2.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/LICENSE` & `Scrapy-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/PKG-INFO` & `Scrapy-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapy
-Version: 2.8.0
+Version: 2.9.0
 Summary: A high-level Web Crawling and Web Scraping framework
 Home-page: https://scrapy.org
 Author: Scrapy developers
 Author-email: pablo@pablohoffman.com
 Maintainer: Pablo Hoffman
 Maintainer-email: pablo@pablohoffman.com
 License: BSD
```

### Comparing `Scrapy-2.8.0/README.rst` & `Scrapy-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/Scrapy.egg-info/PKG-INFO` & `Scrapy-2.9.0/Scrapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapy
-Version: 2.8.0
+Version: 2.9.0
 Summary: A high-level Web Crawling and Web Scraping framework
 Home-page: https://scrapy.org
 Author: Scrapy developers
 Author-email: pablo@pablohoffman.com
 Maintainer: Pablo Hoffman
 Maintainer-email: pablo@pablohoffman.com
 License: BSD
```

### Comparing `Scrapy-2.8.0/Scrapy.egg-info/SOURCES.txt` & `Scrapy-2.9.0/Scrapy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 docs/index.rst
 docs/news.rst
 docs/requirements.txt
 docs/versioning.rst
 docs/_ext/scrapydocs.py
 docs/_static/custom.css
 docs/_static/selectors-sample1.html
-docs/_templates/layout.html
 docs/_tests/quotes.html
 docs/_tests/quotes1.html
 docs/intro/examples.rst
 docs/intro/install.rst
 docs/intro/overview.rst
 docs/intro/tutorial.rst
 docs/topics/api.rst
@@ -304,14 +303,15 @@
 tests/test_downloadermiddleware_httpcompression.py
 tests/test_downloadermiddleware_httpproxy.py
 tests/test_downloadermiddleware_redirect.py
 tests/test_downloadermiddleware_retry.py
 tests/test_downloadermiddleware_robotstxt.py
 tests/test_downloadermiddleware_stats.py
 tests/test_downloadermiddleware_useragent.py
+tests/test_downloaderslotssettings.py
 tests/test_dupefilters.py
 tests/test_engine.py
 tests/test_engine_stop_download_bytes.py
 tests/test_engine_stop_download_headers.py
 tests/test_exporters.py
 tests/test_extension_telnet.py
 tests/test_feedexport.py
```

### Comparing `Scrapy-2.8.0/conftest.py` & `Scrapy-2.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/Makefile` & `Scrapy-2.9.0/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,14 @@
 	      "into the Lib/ directory"
 
 coverage: BUILDER = coverage
 coverage: build
 
 htmlview: html
 	 $(PYTHON) -c "import webbrowser; from pathlib import Path; \
-	 webbrowser.open('file://' + Path('build/html/index.html').resolve())"
+	 webbrowser.open(Path('build/html/index.html').resolve().as_uri())"
 
 clean:
 	-rm -rf build/*
 
 watch: htmlview
 	watchmedo shell-command -p '*.rst' -c 'make html' -R -D
```

### Comparing `Scrapy-2.8.0/docs/README.rst` & `Scrapy-2.9.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/_ext/scrapydocs.py` & `Scrapy-2.9.0/docs/_ext/scrapydocs.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/_static/selectors-sample1.html` & `Scrapy-2.9.0/docs/_static/selectors-sample1.html`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/_tests/quotes.html` & `Scrapy-2.9.0/docs/_tests/quotes.html`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/_tests/quotes1.html` & `Scrapy-2.9.0/docs/_tests/quotes1.html`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/conf.py` & `Scrapy-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/conftest.py` & `Scrapy-2.9.0/docs/conftest.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/contributing.rst` & `Scrapy-2.9.0/docs/contributing.rst`

 * *Files 5% similar despite different names*

```diff
@@ -7,32 +7,31 @@
 .. important::
 
     Double check that you are reading the most recent version of this document at
     https://docs.scrapy.org/en/master/contributing.html
 
 There are many ways to contribute to Scrapy. Here are some of them:
 
-* Blog about Scrapy. Tell the world how you're using Scrapy. This will help
-  newcomers with more examples and will help the Scrapy project to increase its
-  visibility.
-
 * Report bugs and request features in the `issue tracker`_, trying to follow
   the guidelines detailed in `Reporting bugs`_ below.
 
 * Submit patches for new functionalities and/or bug fixes. Please read
   :ref:`writing-patches` and `Submitting patches`_ below for details on how to
   write and submit a patch.
 
+* Blog about Scrapy. Tell the world how you're using Scrapy. This will help
+  newcomers with more examples and will help the Scrapy project to increase its
+  visibility.
+
 * Join the `Scrapy subreddit`_ and share your ideas on how to
   improve Scrapy. We're always open to suggestions.
 
 * Answer Scrapy questions at
   `Stack Overflow <https://stackoverflow.com/questions/tagged/scrapy>`__.
 
-
 Reporting bugs
 ==============
 
 .. note::
 
     Please report security issues **only** to
     scrapy-security@googlegroups.com. This is a private list only open to
@@ -76,14 +75,21 @@
 .. _Minimal, Complete, and Verifiable example: https://stackoverflow.com/help/mcve
 
 .. _writing-patches:
 
 Writing patches
 ===============
 
+Scrapy has a list of `good first issues`_ and `help wanted issues`_ that you
+can work on. These issues are a great way to get started with contributing to
+Scrapy. If you're new to the codebase, you may want to focus on documentation
+or testing-related issues, as they are always useful and can help you get
+more familiar with the project. You can also check Scrapy's `test coverage`_
+to see which areas may benefit from more tests.
+
 The better a patch is written, the higher the chances that it'll get accepted and the sooner it will be merged.
 
 Well-written patches should:
 
 * contain the minimum amount of code required for the specific change. Small
   patches are easier to review and merge. So, if you're doing more than one
   change (or bug fix), please consider submitting one patch per change. Do not
@@ -310,7 +316,10 @@
 .. _Scrapy subreddit: https://reddit.com/r/scrapy
 .. _AUTHORS: https://github.com/scrapy/scrapy/blob/master/AUTHORS
 .. _tests/: https://github.com/scrapy/scrapy/tree/master/tests
 .. _open issues: https://github.com/scrapy/scrapy/issues
 .. _PEP 257: https://www.python.org/dev/peps/pep-0257/
 .. _pull request: https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request
 .. _pytest-xdist: https://github.com/pytest-dev/pytest-xdist
+.. _good first issues: https://github.com/scrapy/scrapy/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22
+.. _help wanted issues: https://github.com/scrapy/scrapy/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22
+.. _test coverage: https://app.codecov.io/gh/scrapy/scrapy
```

### Comparing `Scrapy-2.8.0/docs/faq.rst` & `Scrapy-2.9.0/docs/faq.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,35 +31,32 @@
 
 Yes, you can.
 As mentioned :ref:`above <faq-scrapy-bs-cmp>`, `BeautifulSoup`_ can be used
 for parsing HTML responses in Scrapy callbacks.
 You just have to feed the response's body into a ``BeautifulSoup`` object
 and extract whatever data you need from it.
 
-Here's an example spider using BeautifulSoup API, with ``lxml`` as the HTML parser::
+Here's an example spider using BeautifulSoup API, with ``lxml`` as the HTML parser:
 
+.. skip: next
+.. code-block:: python
 
     from bs4 import BeautifulSoup
     import scrapy
 
 
     class ExampleSpider(scrapy.Spider):
         name = "example"
         allowed_domains = ["example.com"]
-        start_urls = (
-            'http://www.example.com/',
-        )
+        start_urls = ("http://www.example.com/",)
 
         def parse(self, response):
             # use lxml to get decent HTML parsing speed
-            soup = BeautifulSoup(response.text, 'lxml')
-            yield {
-                "url": response.url,
-                "title": soup.h1.string
-            }
+            soup = BeautifulSoup(response.text, "lxml")
+            yield {"url": response.url, "title": soup.h1.string}
 
 .. note::
 
     ``BeautifulSoup`` supports several HTML/XML parsers.
     See `BeautifulSoup's official documentation`_ on which ones are available.
 
 .. _BeautifulSoup's official documentation: https://www.crummy.com/software/BeautifulSoup/bs4/doc/#specifying-the-parser-to-use
@@ -105,19 +102,21 @@
 --------------------------------------------------------
 
 By default, Scrapy uses a `LIFO`_ queue for storing pending requests, which
 basically means that it crawls in `DFO order`_. This order is more convenient
 in most cases.
 
 If you do want to crawl in true `BFO order`_, you can do it by
-setting the following settings::
+setting the following settings:
+
+.. code-block:: python
 
     DEPTH_PRIORITY = 1
-    SCHEDULER_DISK_QUEUE = 'scrapy.squeues.PickleFifoDiskQueue'
-    SCHEDULER_MEMORY_QUEUE = 'scrapy.squeues.FifoMemoryQueue'
+    SCHEDULER_DISK_QUEUE = "scrapy.squeues.PickleFifoDiskQueue"
+    SCHEDULER_MEMORY_QUEUE = "scrapy.squeues.FifoMemoryQueue"
 
 While pending requests are below the configured values of
 :setting:`CONCURRENT_REQUESTS`, :setting:`CONCURRENT_REQUESTS_PER_DOMAIN` or
 :setting:`CONCURRENT_REQUESTS_PER_IP`, those requests are sent
 concurrently. As a result, the first few requests of a crawl rarely follow the
 desired order. Lowering those settings to ``1`` enforces the desired order, but
 it significantly slows down the crawl as a whole.
@@ -155,19 +154,21 @@
     Python’s re_ to compile your URL-filtering regular expression. See
     :issue:`1908`.
 
 See also other suggestions at `StackOverflow`_.
 
 .. note:: Remember to disable
    :class:`scrapy.spidermiddlewares.offsite.OffsiteMiddleware` when you enable
-   your custom implementation::
+   your custom implementation:
+
+   .. code-block:: python
 
        SPIDER_MIDDLEWARES = {
-           'scrapy.spidermiddlewares.offsite.OffsiteMiddleware': None,
-           'myproject.middlewares.CustomOffsiteMiddleware': 500,
+           "scrapy.spidermiddlewares.offsite.OffsiteMiddleware": None,
+           "myproject.middlewares.CustomOffsiteMiddleware": 500,
        }
 
 .. _meet the installation requirements: https://github.com/andreasvc/pyre2#installation
 .. _pyre2: https://github.com/andreasvc/pyre2
 .. _re: https://docs.python.org/library/re.html
 .. _StackOverflow: https://stackoverflow.com/q/36440681/939364
 
@@ -226,24 +227,28 @@
 
 Can I return (Twisted) deferreds from signal handlers?
 ------------------------------------------------------
 
 Some signals support returning deferreds from their handlers, others don't. See
 the :ref:`topics-signals-ref` to know which ones.
 
-What does the response status code 999 means?
----------------------------------------------
+What does the response status code 999 mean?
+--------------------------------------------
 
 999 is a custom response status code used by Yahoo sites to throttle requests.
 Try slowing down the crawling speed by using a download delay of ``2`` (or
-higher) in your spider::
+higher) in your spider:
 
-    class MySpider(CrawlSpider):
+.. code-block:: python
+
+    from scrapy.spiders import CrawlSpider
 
-        name = 'myspider'
+
+    class MySpider(CrawlSpider):
+        name = "myspider"
 
         download_delay = 2
 
         # [ ... rest of the spider code ... ]
 
 Or by setting a global download delay in your project with the
 :setting:`DOWNLOAD_DELAY` setting.
@@ -347,27 +352,29 @@
 How to split an item into multiple items in an item pipeline?
 -------------------------------------------------------------
 
 :ref:`Item pipelines <topics-item-pipeline>` cannot yield multiple items per
 input item. :ref:`Create a spider middleware <custom-spider-middleware>`
 instead, and use its
 :meth:`~scrapy.spidermiddlewares.SpiderMiddleware.process_spider_output`
-method for this purpose. For example::
+method for this purpose. For example:
+
+.. code-block:: python
 
     from copy import deepcopy
 
     from itemadapter import is_item, ItemAdapter
 
-    class MultiplyItemsMiddleware:
 
+    class MultiplyItemsMiddleware:
         def process_spider_output(self, response, result, spider):
             for item in result:
                 if is_item(item):
                     adapter = ItemAdapter(item)
-                    for _ in range(adapter['multiply_by']):
+                    for _ in range(adapter["multiply_by"]):
                         yield deepcopy(item)
 
 Does Scrapy support IPv6 addresses?
 -----------------------------------
 
 Yes, by setting :setting:`DNS_RESOLVER` to ``scrapy.resolver.CachingHostnameResolver``.
 Note that by doing so, you lose the ability to set a specific timeout for DNS requests
@@ -409,8 +416,8 @@
 
 .. _has been reported: https://github.com/scrapy/scrapy/issues/2905
 .. _Python standard library modules: https://docs.python.org/py-modindex.html
 .. _Python package: https://pypi.org/
 .. _user agents: https://en.wikipedia.org/wiki/User_agent
 .. _LIFO: https://en.wikipedia.org/wiki/Stack_(abstract_data_type)
 .. _DFO order: https://en.wikipedia.org/wiki/Depth-first_search
-.. _BFO order: https://en.wikipedia.org/wiki/Breadth-first_search
+.. _BFO order: https://en.wikipedia.org/wiki/Breadth-first_search
```

### Comparing `Scrapy-2.8.0/docs/index.rst` & `Scrapy-2.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/intro/examples.rst` & `Scrapy-2.9.0/docs/intro/examples.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/intro/install.rst` & `Scrapy-2.9.0/docs/intro/install.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/intro/overview.rst` & `Scrapy-2.9.0/docs/intro/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,32 @@
 Walk-through of an example spider
 =================================
 
 In order to show you what Scrapy brings to the table, we'll walk you through an
 example of a Scrapy Spider using the simplest way to run a spider.
 
 Here's the code for a spider that scrapes famous quotes from website
-https://quotes.toscrape.com, following the pagination::
+https://quotes.toscrape.com, following the pagination:
+
+.. code-block:: python
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
-        name = 'quotes'
+        name = "quotes"
         start_urls = [
-            'https://quotes.toscrape.com/tag/humor/',
+            "https://quotes.toscrape.com/tag/humor/",
         ]
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
+            for quote in response.css("div.quote"):
                 yield {
-                    'author': quote.xpath('span/small/text()').get(),
-                    'text': quote.css('span.text::text').get(),
+                    "author": quote.xpath("span/small/text()").get(),
+                    "text": quote.css("span.text::text").get(),
                 }
 
             next_page = response.css('li.next a::attr("href")').get()
             if next_page is not None:
                 yield response.follow(next_page, self.parse)
 
 Put this in a text file, name it to something like ``quotes_spider.py``
```

### Comparing `Scrapy-2.8.0/docs/intro/tutorial.rst` & `Scrapy-2.9.0/docs/intro/tutorial.rst`

 * *Files 8% similar despite different names*

```diff
@@ -79,37 +79,39 @@
 Spiders are classes that you define and that Scrapy uses to scrape information
 from a website (or a group of websites). They must subclass
 :class:`~scrapy.Spider` and define the initial requests to make,
 optionally how to follow links in the pages, and how to parse the downloaded
 page content to extract data.
 
 This is the code for our first Spider. Save it in a file named
-``quotes_spider.py`` under the ``tutorial/spiders`` directory in your project::
+``quotes_spider.py`` under the ``tutorial/spiders`` directory in your project:
+
+.. code-block:: python
 
     from pathlib import Path
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
         name = "quotes"
 
         def start_requests(self):
             urls = [
-                'https://quotes.toscrape.com/page/1/',
-                'https://quotes.toscrape.com/page/2/',
+                "https://quotes.toscrape.com/page/1/",
+                "https://quotes.toscrape.com/page/2/",
             ]
             for url in urls:
                 yield scrapy.Request(url=url, callback=self.parse)
 
         def parse(self, response):
             page = response.url.split("/")[-2]
-            filename = f'quotes-{page}.html'
+            filename = f"quotes-{page}.html"
             Path(filename).write_bytes(response.body)
-            self.log(f'Saved file {filename}')
+            self.log(f"Saved file {filename}")
 
 
 As you can see, our Spider subclasses :class:`scrapy.Spider <scrapy.Spider>`
 and defines some attributes and methods:
 
 * :attr:`~scrapy.Spider.name`: identifies the Spider. It must be
   unique within a project, that is, you can't set the same name for different
@@ -173,31 +175,33 @@
 A shortcut to the start_requests method
 ---------------------------------------
 Instead of implementing a :meth:`~scrapy.Spider.start_requests` method
 that generates :class:`scrapy.Request <scrapy.Request>` objects from URLs,
 you can just define a :attr:`~scrapy.Spider.start_urls` class attribute
 with a list of URLs. This list will then be used by the default implementation
 of :meth:`~scrapy.Spider.start_requests` to create the initial requests
-for your spider::
+for your spider.
+
+.. code-block:: python
 
     from pathlib import Path
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
         name = "quotes"
         start_urls = [
-            'https://quotes.toscrape.com/page/1/',
-            'https://quotes.toscrape.com/page/2/',
+            "https://quotes.toscrape.com/page/1/",
+            "https://quotes.toscrape.com/page/2/",
         ]
 
         def parse(self, response):
             page = response.url.split("/")[-2]
-            filename = f'quotes-{page}.html'
+            filename = f"quotes-{page}.html"
             Path(filename).write_bytes(response.body)
 
 The :meth:`~scrapy.Spider.parse` method will be called to handle each
 of the requests for those URLs, even though we haven't explicitly told Scrapy
 to do so. This happens because :meth:`~scrapy.Spider.parse` is Scrapy's
 default callback method, which is called for requests without an explicitly
 assigned callback.
@@ -241,79 +245,95 @@
 Using the shell, you can try selecting elements using `CSS`_ with the response
 object:
 
 .. invisible-code-block: python
 
     response = load_response('https://quotes.toscrape.com/page/1/', 'quotes1.html')
 
->>> response.css('title')
-[<Selector xpath='descendant-or-self::title' data='<title>Quotes to Scrape</title>'>]
+.. code-block:: pycon
+
+    >>> response.css("title")
+    [<Selector query='descendant-or-self::title' data='<title>Quotes to Scrape</title>'>]
 
 The result of running ``response.css('title')`` is a list-like object called
 :class:`~scrapy.selector.SelectorList`, which represents a list of
 :class:`~scrapy.Selector` objects that wrap around XML/HTML elements
 and allow you to run further queries to fine-grain the selection or extract the
 data.
 
 To extract the text from the title above, you can do:
 
->>> response.css('title::text').getall()
-['Quotes to Scrape']
+.. code-block:: pycon
+
+    >>> response.css("title::text").getall()
+    ['Quotes to Scrape']
 
 There are two things to note here: one is that we've added ``::text`` to the
 CSS query, to mean we want to select only the text elements directly inside
 ``<title>`` element.  If we don't specify ``::text``, we'd get the full title
 element, including its tags:
 
->>> response.css('title').getall()
-['<title>Quotes to Scrape</title>']
+.. code-block:: pycon
+
+    >>> response.css("title").getall()
+    ['<title>Quotes to Scrape</title>']
 
 The other thing is that the result of calling ``.getall()`` is a list: it is
 possible that a selector returns more than one result, so we extract them all.
 When you know you just want the first result, as in this case, you can do:
 
->>> response.css('title::text').get()
-'Quotes to Scrape'
+.. code-block:: pycon
+
+    >>> response.css("title::text").get()
+    'Quotes to Scrape'
 
 As an alternative, you could've written:
 
->>> response.css('title::text')[0].get()
-'Quotes to Scrape'
+.. code-block:: pycon
+
+    >>> response.css("title::text")[0].get()
+    'Quotes to Scrape'
 
 Accessing an index on a :class:`~scrapy.selector.SelectorList` instance will 
-raise an :exc:`IndexError` exception if there are no results::
+raise an :exc:`IndexError` exception if there are no results:
+
+.. code-block:: pycon
 
-    >>> response.css('noelement')[0].get()
+    >>> response.css("noelement")[0].get()
     Traceback (most recent call last):
     ...
     IndexError: list index out of range
 
 You might want to use ``.get()`` directly on the 
 :class:`~scrapy.selector.SelectorList` instance instead, which returns ``None`` 
-if there are no results::
+if there are no results:
 
->>> response.css("noelement").get()
+.. code-block:: pycon
+
+    >>> response.css("noelement").get()
 
 There's a lesson here: for most scraping code, you want it to be resilient to
 errors due to things not being found on a page, so that even if some parts fail
 to be scraped, you can at least get **some** data.
 
 Besides the :meth:`~scrapy.selector.SelectorList.getall` and
 :meth:`~scrapy.selector.SelectorList.get` methods, you can also use
 the :meth:`~scrapy.selector.SelectorList.re` method to extract using
 :doc:`regular expressions <library/re>`:
 
->>> response.css('title::text').re(r'Quotes.*')
-['Quotes to Scrape']
->>> response.css('title::text').re(r'Q\w+')
-['Quotes']
->>> response.css('title::text').re(r'(\w+) to (\w+)')
-['Quotes', 'Scrape']
+.. code-block:: pycon
+
+    >>> response.css("title::text").re(r"Quotes.*")
+    ['Quotes to Scrape']
+    >>> response.css("title::text").re(r"Q\w+")
+    ['Quotes']
+    >>> response.css("title::text").re(r"(\w+) to (\w+)")
+    ['Quotes', 'Scrape']
 
-In order to find the proper CSS selectors to use, you might find useful opening
+In order to find the proper CSS selectors to use, you might find it useful to open
 the response page from the shell in your web browser using ``view(response)``.
 You can use your browser's developer tools to inspect the HTML and come up
 with a selector (see :ref:`topics-developer-tools`).
 
 `Selector Gadget`_ is also a nice tool to quickly find CSS selector for
 visually selected elements, which works in many browsers.
 
@@ -321,18 +341,20 @@
 
 
 XPath: a brief intro
 ^^^^^^^^^^^^^^^^^^^^
 
 Besides `CSS`_, Scrapy selectors also support using `XPath`_ expressions:
 
->>> response.xpath('//title')
-[<Selector xpath='//title' data='<title>Quotes to Scrape</title>'>]
->>> response.xpath('//title/text()').get()
-'Quotes to Scrape'
+.. code-block:: pycon
+
+    >>> response.xpath("//title")
+    [<Selector query='//title' data='<title>Quotes to Scrape</title>'>]
+    >>> response.xpath("//title/text()").get()
+    'Quotes to Scrape'
 
 XPath expressions are very powerful, and are the foundation of Scrapy
 Selectors. In fact, CSS selectors are converted to XPath under-the-hood. You
 can see that if you read closely the text representation of the selector
 objects in the shell.
 
 While perhaps not as popular as CSS selectors, XPath expressions offer more
@@ -381,85 +403,98 @@
 Let's open up scrapy shell and play a bit to find out how to extract the data
 we want::
 
     scrapy shell 'https://quotes.toscrape.com'
 
 We get a list of selectors for the quote HTML elements with:
 
->>> response.css("div.quote")
-[<Selector xpath="descendant-or-self::div[@class and contains(concat(' ', normalize-space(@class), ' '), ' quote ')]" data='<div class="quote" itemscope itemtype...'>,
- <Selector xpath="descendant-or-self::div[@class and contains(concat(' ', normalize-space(@class), ' '), ' quote ')]" data='<div class="quote" itemscope itemtype...'>,
- ...]
+.. code-block:: pycon
+
+    >>> response.css("div.quote")
+    [<Selector query="descendant-or-self::div[@class and contains(concat(' ', normalize-space(@class), ' '), ' quote ')]" data='<div class="quote" itemscope itemtype...'>,
+    <Selector query="descendant-or-self::div[@class and contains(concat(' ', normalize-space(@class), ' '), ' quote ')]" data='<div class="quote" itemscope itemtype...'>,
+    ...]
 
 Each of the selectors returned by the query above allows us to run further
 queries over their sub-elements. Let's assign the first selector to a
 variable, so that we can run our CSS selectors directly on a particular quote:
 
->>> quote = response.css("div.quote")[0]
+.. code-block:: pycon
+
+    >>> quote = response.css("div.quote")[0]
 
 Now, let's extract ``text``, ``author`` and the ``tags`` from that quote
 using the ``quote`` object we just created:
 
->>> text = quote.css("span.text::text").get()
->>> text
-'“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”'
->>> author = quote.css("small.author::text").get()
->>> author
-'Albert Einstein'
+.. code-block:: pycon
+
+    >>> text = quote.css("span.text::text").get()
+    >>> text
+    '“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”'
+    >>> author = quote.css("small.author::text").get()
+    >>> author
+    'Albert Einstein'
 
 Given that the tags are a list of strings, we can use the ``.getall()`` method
 to get all of them:
 
->>> tags = quote.css("div.tags a.tag::text").getall()
->>> tags
-['change', 'deep-thoughts', 'thinking', 'world']
+.. code-block:: pycon
+
+    >>> tags = quote.css("div.tags a.tag::text").getall()
+    >>> tags
+    ['change', 'deep-thoughts', 'thinking', 'world']
 
 .. invisible-code-block: python
 
   from sys import version_info
 
 Having figured out how to extract each bit, we can now iterate over all the
 quotes elements and put them together into a Python dictionary:
 
->>> for quote in response.css("div.quote"):
-...     text = quote.css("span.text::text").get()
-...     author = quote.css("small.author::text").get()
-...     tags = quote.css("div.tags a.tag::text").getall()
-...     print(dict(text=text, author=author, tags=tags))
-{'text': '“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”', 'author': 'Albert Einstein', 'tags': ['change', 'deep-thoughts', 'thinking', 'world']}
-{'text': '“It is our choices, Harry, that show what we truly are, far more than our abilities.”', 'author': 'J.K. Rowling', 'tags': ['abilities', 'choices']}
-...
+.. code-block:: pycon
+
+    >>> for quote in response.css("div.quote"):
+    ...     text = quote.css("span.text::text").get()
+    ...     author = quote.css("small.author::text").get()
+    ...     tags = quote.css("div.tags a.tag::text").getall()
+    ...     print(dict(text=text, author=author, tags=tags))
+    ...
+    {'text': '“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”', 'author': 'Albert Einstein', 'tags': ['change', 'deep-thoughts', 'thinking', 'world']}
+    {'text': '“It is our choices, Harry, that show what we truly are, far more than our abilities.”', 'author': 'J.K. Rowling', 'tags': ['abilities', 'choices']}
+    ...
 
 Extracting data in our spider
 -----------------------------
 
 Let's get back to our spider. Until now, it doesn't extract any data in
 particular, just saves the whole HTML page to a local file. Let's integrate the
 extraction logic above into our spider.
 
 A Scrapy spider typically generates many dictionaries containing the data
 extracted from the page. To do that, we use the ``yield`` Python keyword
-in the callback, as you can see below::
+in the callback, as you can see below:
+
+.. code-block:: python
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
         name = "quotes"
         start_urls = [
-            'https://quotes.toscrape.com/page/1/',
-            'https://quotes.toscrape.com/page/2/',
+            "https://quotes.toscrape.com/page/1/",
+            "https://quotes.toscrape.com/page/2/",
         ]
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
+            for quote in response.css("div.quote"):
                 yield {
-                    'text': quote.css('span.text::text').get(),
-                    'author': quote.css('small.author::text').get(),
-                    'tags': quote.css('div.tags a.tag::text').getall(),
+                    "text": quote.css("span.text::text").get(),
+                    "author": quote.css("small.author::text").get(),
+                    "tags": quote.css("div.tags a.tag::text").getall(),
                 }
 
 If you run this spider, it will output the extracted data with the log::
 
     2016-09-19 18:57:19 [scrapy.core.scraper] DEBUG: Scraped from <200 https://quotes.toscrape.com/page/1/>
     {'tags': ['life', 'love'], 'author': 'André Gide', 'text': '“It is better to be hated for what you are than to be loved for what you are not.”'}
     2016-09-19 18:57:19 [scrapy.core.scraper] DEBUG: Scraped from <200 https://quotes.toscrape.com/page/1/>
@@ -529,44 +564,50 @@
 >>> response.css('li.next a').get()
 '<a href="/page/2/">Next <span aria-hidden="true">→</span></a>'
 
 This gets the anchor element, but we want the attribute ``href``. For that,
 Scrapy supports a CSS extension that lets you select the attribute contents,
 like this:
 
->>> response.css('li.next a::attr(href)').get()
-'/page/2/'
+.. code-block:: pycon
+
+    >>> response.css("li.next a::attr(href)").get()
+    '/page/2/'
 
 There is also an ``attrib`` property available
 (see :ref:`selecting-attributes` for more):
 
->>> response.css('li.next a').attrib['href']
-'/page/2/'
+.. code-block:: pycon
+
+    >>> response.css("li.next a").attrib["href"]
+    '/page/2/'
 
 Let's see now our spider modified to recursively follow the link to the next
-page, extracting data from it::
+page, extracting data from it:
+
+.. code-block:: python
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
         name = "quotes"
         start_urls = [
-            'https://quotes.toscrape.com/page/1/',
+            "https://quotes.toscrape.com/page/1/",
         ]
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
+            for quote in response.css("div.quote"):
                 yield {
-                    'text': quote.css('span.text::text').get(),
-                    'author': quote.css('small.author::text').get(),
-                    'tags': quote.css('div.tags a.tag::text').getall(),
+                    "text": quote.css("span.text::text").get(),
+                    "author": quote.css("small.author::text").get(),
+                    "tags": quote.css("div.tags a.tag::text").getall(),
                 }
 
-            next_page = response.css('li.next a::attr(href)').get()
+            next_page = response.css("li.next a::attr(href)").get()
             if next_page is not None:
                 next_page = response.urljoin(next_page)
                 yield scrapy.Request(next_page, callback=self.parse)
 
 
 Now, after extracting the data, the ``parse()`` method looks for the link to
 the next page, builds a full absolute URL using the
@@ -590,93 +631,109 @@
 
 .. _response-follow-example:
 
 A shortcut for creating Requests
 --------------------------------
 
 As a shortcut for creating Request objects you can use
-:meth:`response.follow <scrapy.http.TextResponse.follow>`::
+:meth:`response.follow <scrapy.http.TextResponse.follow>`:
+
+.. code-block:: python
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
         name = "quotes"
         start_urls = [
-            'https://quotes.toscrape.com/page/1/',
+            "https://quotes.toscrape.com/page/1/",
         ]
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
+            for quote in response.css("div.quote"):
                 yield {
-                    'text': quote.css('span.text::text').get(),
-                    'author': quote.css('span small::text').get(),
-                    'tags': quote.css('div.tags a.tag::text').getall(),
+                    "text": quote.css("span.text::text").get(),
+                    "author": quote.css("span small::text").get(),
+                    "tags": quote.css("div.tags a.tag::text").getall(),
                 }
 
-            next_page = response.css('li.next a::attr(href)').get()
+            next_page = response.css("li.next a::attr(href)").get()
             if next_page is not None:
                 yield response.follow(next_page, callback=self.parse)
 
 Unlike scrapy.Request, ``response.follow`` supports relative URLs directly - no
 need to call urljoin. Note that ``response.follow`` just returns a Request
 instance; you still have to yield this Request.
 
+.. skip: start
+
 You can also pass a selector to ``response.follow`` instead of a string;
-this selector should extract necessary attributes::
+this selector should extract necessary attributes:
 
-    for href in response.css('ul.pager a::attr(href)'):
+.. code-block:: python
+
+    for href in response.css("ul.pager a::attr(href)"):
         yield response.follow(href, callback=self.parse)
 
 For ``<a>`` elements there is a shortcut: ``response.follow`` uses their href
-attribute automatically. So the code can be shortened further::
+attribute automatically. So the code can be shortened further:
+
+.. code-block:: python
 
-    for a in response.css('ul.pager a'):
+    for a in response.css("ul.pager a"):
         yield response.follow(a, callback=self.parse)
 
 To create multiple requests from an iterable, you can use
-:meth:`response.follow_all <scrapy.http.TextResponse.follow_all>` instead::
+:meth:`response.follow_all <scrapy.http.TextResponse.follow_all>` instead:
 
-    anchors = response.css('ul.pager a')
+.. code-block:: python
+
+    anchors = response.css("ul.pager a")
     yield from response.follow_all(anchors, callback=self.parse)
 
-or, shortening it further::
+or, shortening it further:
+
+.. code-block:: python
 
-    yield from response.follow_all(css='ul.pager a', callback=self.parse)
+    yield from response.follow_all(css="ul.pager a", callback=self.parse)
+
+.. skip: end
 
 
 More examples and patterns
 --------------------------
 
 Here is another spider that illustrates callbacks and following links,
-this time for scraping author information::
+this time for scraping author information:
+
+.. code-block:: python
 
     import scrapy
 
 
     class AuthorSpider(scrapy.Spider):
-        name = 'author'
+        name = "author"
 
-        start_urls = ['https://quotes.toscrape.com/']
+        start_urls = ["https://quotes.toscrape.com/"]
 
         def parse(self, response):
-            author_page_links = response.css('.author + a')
+            author_page_links = response.css(".author + a")
             yield from response.follow_all(author_page_links, self.parse_author)
 
-            pagination_links = response.css('li.next a')
+            pagination_links = response.css("li.next a")
             yield from response.follow_all(pagination_links, self.parse)
 
         def parse_author(self, response):
             def extract_with_css(query):
-                return response.css(query).get(default='').strip()
+                return response.css(query).get(default="").strip()
 
             yield {
-                'name': extract_with_css('h3.author-title::text'),
-                'birthdate': extract_with_css('.author-born-date::text'),
-                'bio': extract_with_css('.author-description::text'),
+                "name": extract_with_css("h3.author-title::text"),
+                "birthdate": extract_with_css(".author-born-date::text"),
+                "bio": extract_with_css(".author-description::text"),
             }
 
 This spider will start from the main page, it will follow all the links to the
 authors pages calling the ``parse_author`` callback for each of them, and also
 the pagination links with the ``parse`` callback as we saw before.
 
 Here we're passing callbacks to
@@ -716,37 +773,39 @@
     scrapy crawl quotes -O quotes-humor.json -a tag=humor
 
 These arguments are passed to the Spider's ``__init__`` method and become
 spider attributes by default.
 
 In this example, the value provided for the ``tag`` argument will be available
 via ``self.tag``. You can use this to make your spider fetch only quotes
-with a specific tag, building the URL based on the argument::
+with a specific tag, building the URL based on the argument:
+
+.. code-block:: python
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
         name = "quotes"
 
         def start_requests(self):
-            url = 'https://quotes.toscrape.com/'
-            tag = getattr(self, 'tag', None)
+            url = "https://quotes.toscrape.com/"
+            tag = getattr(self, "tag", None)
             if tag is not None:
-                url = url + 'tag/' + tag
+                url = url + "tag/" + tag
             yield scrapy.Request(url, self.parse)
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
+            for quote in response.css("div.quote"):
                 yield {
-                    'text': quote.css('span.text::text').get(),
-                    'author': quote.css('small.author::text').get(),
+                    "text": quote.css("span.text::text").get(),
+                    "author": quote.css("small.author::text").get(),
                 }
 
-            next_page = response.css('li.next a::attr(href)').get()
+            next_page = response.css("li.next a::attr(href)").get()
             if next_page is not None:
                 yield response.follow(next_page, self.parse)
 
 
 If you pass the ``tag=humor`` argument to this spider, you'll notice that it
 will only visit URLs from the ``humor`` tag, such as
 ``https://quotes.toscrape.com/tag/humor``.
```

### Comparing `Scrapy-2.8.0/docs/news.rst` & `Scrapy-2.9.0/docs/news.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,134 @@
 .. _news:
 
 Release notes
 =============
 
+.. _release-2.9.0:
+
+Scrapy 2.9.0 (2023-05-08)
+-------------------------
+
+Highlights:
+
+-   Per-domain download settings.
+-   Compatibility with new cryptography_ and new parsel_.
+-   JMESPath selectors from the new parsel_.
+-   Bug fixes.
+
+Deprecations
+~~~~~~~~~~~~
+
+-   :class:`scrapy.extensions.feedexport._FeedSlot` is renamed to
+    :class:`scrapy.extensions.feedexport.FeedSlot` and the old name is
+    deprecated. (:issue:`5876`)
+
+New features
+~~~~~~~~~~~~
+
+-   Settings correponding to :setting:`DOWNLOAD_DELAY`,
+    :setting:`CONCURRENT_REQUESTS_PER_DOMAIN` and
+    :setting:`RANDOMIZE_DOWNLOAD_DELAY` can now be set on a per-domain basis
+    via the new :setting:`DOWNLOAD_SLOTS` setting. (:issue:`5328`)
+
+-   Added :meth:`TextResponse.jmespath`, a shortcut for JMESPath selectors
+    available since parsel_ 1.8.1. (:issue:`5894`, :issue:`5915`)
+
+-   Added :signal:`feed_slot_closed` and :signal:`feed_exporter_closed`
+    signals. (:issue:`5876`)
+
+-   Added :func:`scrapy.utils.request.request_to_curl`, a function to produce a
+    curl command from a :class:`~scrapy.Request` object. (:issue:`5892`)
+
+-   Values of :setting:`FILES_STORE` and :setting:`IMAGES_STORE` can now be
+    :class:`pathlib.Path` instances. (:issue:`5801`)
+
+Bug fixes
+~~~~~~~~~
+
+-   Fixed a warning with Parsel 1.8.1+. (:issue:`5903`, :issue:`5918`)
+
+-   Fixed an error when using feed postprocessing with S3 storage.
+    (:issue:`5500`, :issue:`5581`)
+
+-   Added the missing :meth:`scrapy.settings.BaseSettings.setdefault` method.
+    (:issue:`5811`, :issue:`5821`)
+
+-   Fixed an error when using cryptography_ 40.0.0+ and
+    :setting:`DOWNLOADER_CLIENT_TLS_VERBOSE_LOGGING` is enabled.
+    (:issue:`5857`, :issue:`5858`)
+
+-   The checksums returned by :class:`~scrapy.pipelines.files.FilesPipeline`
+    for files on Google Cloud Storage are no longer Base64-encoded.
+    (:issue:`5874`, :issue:`5891`)
+
+-   :func:`scrapy.utils.request.request_from_curl` now supports $-prefixed
+    string values for the curl ``--data-raw`` argument, which are produced by
+    browsers for data that includes certain symbols. (:issue:`5899`,
+    :issue:`5901`)
+
+-   The :command:`parse` command now also works with async generator callbacks.
+    (:issue:`5819`, :issue:`5824`)
+
+-   The :command:`genspider` command now properly works with HTTPS URLs.
+    (:issue:`3553`, :issue:`5808`)
+
+-   Improved handling of asyncio loops. (:issue:`5831`, :issue:`5832`)
+
+-   :class:`LinkExtractor <scrapy.linkextractors.lxmlhtml.LxmlLinkExtractor>`
+    now skips certain malformed URLs instead of raising an exception.
+    (:issue:`5881`)
+
+-   :func:`scrapy.utils.python.get_func_args` now supports more types of
+    callables. (:issue:`5872`, :issue:`5885`)
+
+-   Fixed an error when processing non-UTF8 values of ``Content-Type`` headers.
+    (:issue:`5914`, :issue:`5917`)
+
+-   Fixed an error breaking user handling of send failures in
+    :meth:`scrapy.mail.MailSender.send()`. (:issue:`1611`, :issue:`5880`)
+
+Documentation
+~~~~~~~~~~~~~
+
+-   Expanded contributing docs. (:issue:`5109`, :issue:`5851`)
+
+-   Added blacken-docs_ to pre-commit and reformatted the docs with it.
+    (:issue:`5813`, :issue:`5816`)
+
+-   Fixed a JS issue. (:issue:`5875`, :issue:`5877`)
+
+-   Fixed ``make htmlview``. (:issue:`5878`, :issue:`5879`)
+
+-   Fixed typos and other small errors. (:issue:`5827`, :issue:`5839`,
+    :issue:`5883`, :issue:`5890`, :issue:`5895`, :issue:`5904`)
+
+Quality assurance
+~~~~~~~~~~~~~~~~~
+
+-   Extended typing hints. (:issue:`5805`, :issue:`5889`, :issue:`5896`)
+
+-   Tests for most of the examples in the docs are now run as a part of CI,
+    found problems were fixed. (:issue:`5816`, :issue:`5826`, :issue:`5919`)
+
+-   Removed usage of deprecated Python classes. (:issue:`5849`)
+
+-   Silenced ``include-ignored`` warnings from coverage. (:issue:`5820`)
+
+-   Fixed a random failure of the ``test_feedexport.test_batch_path_differ``
+    test. (:issue:`5855`, :issue:`5898`)
+
+-   Updated docstrings to match output produced by parsel_ 1.8.1 so that they
+    don't cause test failures. (:issue:`5902`, :issue:`5919`)
+
+-   Other CI and pre-commit improvements. (:issue:`5802`, :issue:`5823`,
+    :issue:`5908`)
+
+.. _blacken-docs: https://github.com/adamchainz/blacken-docs
+
 .. _release-2.8.0:
 
 Scrapy 2.8.0 (2023-02-02)
 -------------------------
 
 This is a maintenance release, with minor features, bug fixes, and cleanups.
 
@@ -2619,19 +2741,21 @@
     (:setting:`DOWNLOADER_CLIENTCONTEXTFACTORY`), its ``__init__`` method must
     accept two new parameters: ``tls_verbose_logging`` and ``tls_ciphers``
     (:issue:`2111`, :issue:`3392`, :issue:`3442`, :issue:`3450`)
 
 *   :class:`~scrapy.loader.ItemLoader` now turns the values of its input item
     into lists:
 
-    >>> item = MyItem()
-    >>> item['field'] = 'value1'
-    >>> loader = ItemLoader(item=item)
-    >>> item['field']
-    ['value1']
+    .. code-block:: pycon
+
+        >>> item = MyItem()
+        >>> item["field"] = "value1"
+        >>> loader = ItemLoader(item=item)
+        >>> item["field"]
+        ['value1']
 
     This is needed to allow adding values to existing fields
     (``loader.add_value('field', 'value2')``).
 
     (:issue:`3804`, :issue:`3819`, :issue:`3897`, :issue:`3976`, :issue:`3998`,
     :issue:`4036`)
 
@@ -4201,16 +4325,14 @@
 ~~~~~~~~~~~
 
 - ``telnetconsole`` was relocated to ``extensions/`` (:issue:`1524`).
 
   + Note: telnet is not enabled on Python 3
     (https://github.com/scrapy/scrapy/pull/1524#issuecomment-146985595)
 
-.. _parsel: https://github.com/scrapy/parsel
-
 
 Bugfixes
 ~~~~~~~~
 
 - Scrapy does not retry requests that got a ``HTTP 400 Bad Request``
   response anymore (:issue:`1289`). **Warning: backward incompatible!**
 - Support empty password for http_proxy config (:issue:`1274`).
@@ -5632,14 +5754,15 @@
 .. _Creating a pull request: https://help.github.com/en/articles/creating-a-pull-request
 .. _cryptography: https://cryptography.io/en/latest/
 .. _docstrings: https://docs.python.org/3/glossary.html#term-docstring
 .. _KeyboardInterrupt: https://docs.python.org/3/library/exceptions.html#KeyboardInterrupt
 .. _LevelDB: https://github.com/google/leveldb
 .. _lxml: https://lxml.de/
 .. _marshal: https://docs.python.org/2/library/marshal.html
+.. _parsel: https://github.com/scrapy/parsel
 .. _parsel.csstranslator.GenericTranslator: https://parsel.readthedocs.io/en/latest/parsel.html#parsel.csstranslator.GenericTranslator
 .. _parsel.csstranslator.HTMLTranslator: https://parsel.readthedocs.io/en/latest/parsel.html#parsel.csstranslator.HTMLTranslator
 .. _parsel.csstranslator.XPathExpr: https://parsel.readthedocs.io/en/latest/parsel.html#parsel.csstranslator.XPathExpr
 .. _PEP 257: https://www.python.org/dev/peps/pep-0257/
 .. _Pillow: https://python-pillow.org/
 .. _pyOpenSSL: https://www.pyopenssl.org/en/stable/
 .. _queuelib: https://github.com/scrapy/queuelib
```

### Comparing `Scrapy-2.8.0/docs/topics/_images/inspector_01.png` & `Scrapy-2.9.0/docs/topics/_images/inspector_01.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/_images/network_01.png` & `Scrapy-2.9.0/docs/topics/_images/network_01.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/_images/network_02.png` & `Scrapy-2.9.0/docs/topics/_images/network_02.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/_images/network_03.png` & `Scrapy-2.9.0/docs/topics/_images/network_03.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/_images/scrapy_architecture.odg` & `Scrapy-2.9.0/docs/topics/_images/scrapy_architecture.odg`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/_images/scrapy_architecture.png` & `Scrapy-2.9.0/docs/topics/_images/scrapy_architecture.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/_images/scrapy_architecture_02.png` & `Scrapy-2.9.0/docs/topics/_images/scrapy_architecture_02.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/api.rst` & `Scrapy-2.9.0/docs/topics/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -128,24 +128,22 @@
     settings priorities used in Scrapy.
 
     Each item defines a settings entry point, giving it a code name for
     identification and an integer priority. Greater priorities take more
     precedence over lesser ones when setting and retrieving values in the
     :class:`~scrapy.settings.Settings` class.
 
-    .. highlight:: python
-
-    ::
+    .. code-block:: python
 
         SETTINGS_PRIORITIES = {
-            'default': 0,
-            'command': 10,
-            'project': 20,
-            'spider': 30,
-            'cmdline': 40,
+            "default": 0,
+            "command": 10,
+            "project": 20,
+            "spider": 30,
+            "cmdline": 40,
         }
 
     For a detailed explanation on each settings sources, see:
     :ref:`topics-settings`.
 
 .. autofunction:: get_settings_priority
```

### Comparing `Scrapy-2.8.0/docs/topics/architecture.rst` & `Scrapy-2.9.0/docs/topics/architecture.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/asyncio.rst` & `Scrapy-2.9.0/docs/topics/asyncio.rst`

 * *Files 1% similar despite different names*

```diff
@@ -102,20 +102,22 @@
 
 Enforcing asyncio as a requirement
 ==================================
 
 If you are writing a :ref:`component <topics-components>` that requires asyncio
 to work, use :func:`scrapy.utils.reactor.is_asyncio_reactor_installed` to
 :ref:`enforce it as a requirement <enforce-component-requirements>`. For
-example::
+example:
+
+.. code-block:: python
 
     from scrapy.utils.reactor import is_asyncio_reactor_installed
 
-    class MyComponent:
 
+    class MyComponent:
         def __init__(self):
             if not is_asyncio_reactor_installed():
                 raise ValueError(
                     f"{MyComponent.__qualname__} requires the asyncio Twisted "
                     f"reactor. Make sure you have it configured in the "
                     f"TWISTED_REACTOR setting. See the asyncio documentation "
                     f"of Scrapy for more information."
```

### Comparing `Scrapy-2.8.0/docs/topics/autothrottle.rst` & `Scrapy-2.9.0/docs/topics/autothrottle.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/benchmarking.rst` & `Scrapy-2.9.0/docs/topics/benchmarking.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/broad-crawls.rst` & `Scrapy-2.9.0/docs/topics/broad-crawls.rst`

 * *Files 8% similar despite different names*

```diff
@@ -44,17 +44,19 @@
 Use the right :setting:`SCHEDULER_PRIORITY_QUEUE`
 =================================================
 
 Scrapy’s default scheduler priority queue is ``'scrapy.pqueues.ScrapyPriorityQueue'``.
 It works best during single-domain crawl. It does not work well with crawling
 many different domains in parallel
 
-To apply the recommended priority queue use::
+To apply the recommended priority queue use:
 
-    SCHEDULER_PRIORITY_QUEUE = 'scrapy.pqueues.DownloaderAwarePriorityQueue'
+.. code-block:: python
+
+    SCHEDULER_PRIORITY_QUEUE = "scrapy.pqueues.DownloaderAwarePriorityQueue"
 
 .. _broad-crawls-concurrency:
 
 Increase concurrency
 ====================
 
 Concurrency is the number of requests that are processed in parallel. There is
@@ -67,15 +69,17 @@
           :setting:`CONCURRENT_REQUESTS_PER_IP`.
 
 The default global concurrency limit in Scrapy is not suitable for crawling
 many different domains in parallel, so you will want to increase it. How much
 to increase it will depend on how much CPU and memory your crawler will have
 available.
 
-A good starting point is ``100``::
+A good starting point is ``100``:
+
+.. code-block:: python
 
     CONCURRENT_REQUESTS = 100
 
 But the best way to find out is by doing some trials and identifying at what
 concurrency your Scrapy process gets CPU bounded. For optimum performance, you
 should pick a concurrency where CPU usage is at 80-90%.
 
@@ -88,15 +92,17 @@
 
 Currently Scrapy does DNS resolution in a blocking way with usage of thread
 pool. With higher concurrency levels the crawling could be slow or even fail
 hitting DNS resolver timeouts. Possible solution to increase the number of
 threads handling DNS queries. The DNS queue will be processed faster speeding
 up establishing of connection and crawling overall.
 
-To increase maximum thread pool size use::
+To increase maximum thread pool size use:
+
+.. code-block:: python
 
     REACTOR_THREADPOOL_MAXSIZE = 20
 
 Setup your own DNS
 ==================
 
 If you have multiple crawling processes and single central DNS, it can act
@@ -110,63 +116,73 @@
 When doing broad crawls you are often only interested in the crawl rates you
 get and any errors found. These stats are reported by Scrapy when using the
 ``INFO`` log level. In order to save CPU (and log storage requirements) you
 should not use ``DEBUG`` log level when preforming large broad crawls in
 production. Using ``DEBUG`` level when developing your (broad) crawler may be
 fine though.
 
-To set the log level use::
+To set the log level use:
 
-    LOG_LEVEL = 'INFO'
+.. code-block:: python
+
+    LOG_LEVEL = "INFO"
 
 Disable cookies
 ===============
 
 Disable cookies unless you *really* need. Cookies are often not needed when
 doing broad crawls (search engine crawlers ignore them), and they improve
 performance by saving some CPU cycles and reducing the memory footprint of your
 Scrapy crawler.
 
-To disable cookies use::
+To disable cookies use:
+
+.. code-block:: python
 
     COOKIES_ENABLED = False
 
 Disable retries
 ===============
 
 Retrying failed HTTP requests can slow down the crawls substantially, specially
 when sites causes are very slow (or fail) to respond, thus causing a timeout
 error which gets retried many times, unnecessarily, preventing crawler capacity
 to be reused for other domains.
 
-To disable retries use::
+To disable retries use:
+
+.. code-block:: python
 
     RETRY_ENABLED = False
 
 Reduce download timeout
 =======================
 
 Unless you are crawling from a very slow connection (which shouldn't be the
 case for broad crawls) reduce the download timeout so that stuck requests are
 discarded quickly and free up capacity to process the next ones.
 
-To reduce the download timeout use::
+To reduce the download timeout use:
+
+.. code-block:: python
 
     DOWNLOAD_TIMEOUT = 15
 
 Disable redirects
 =================
 
 Consider disabling redirects, unless you are interested in following them. When
 doing broad crawls it's common to save redirects and resolve them when
 revisiting the site at a later crawl. This also help to keep the number of
 request constant per crawl batch, otherwise redirect loops may cause the
 crawler to dedicate too many resources on any specific domain.
 
-To disable redirects use::
+To disable redirects use:
+
+.. code-block:: python
 
     REDIRECT_ENABLED = False
 
 Enable crawling of "Ajax Crawlable Pages"
 =========================================
 
 Some pages (up to 1%, based on empirical data from year 2013) declare
@@ -175,15 +191,17 @@
 Pages can indicate it in two ways:
 
 1) by using ``#!`` in URL - this is the default way;
 2) by using a special meta tag - this way is used on
    "main", "index" website pages.
 
 Scrapy handles (1) automatically; to handle (2) enable
-:ref:`AjaxCrawlMiddleware <ajaxcrawl-middleware>`::
+:ref:`AjaxCrawlMiddleware <ajaxcrawl-middleware>`:
+
+.. code-block:: python
 
     AJAXCRAWL_ENABLED = True
 
 When doing broad crawls it's common to crawl a lot of "index" web pages;
 AjaxCrawlMiddleware helps to crawl them correctly.
 It is turned OFF by default because it has some performance overhead,
 and enabling it for focused crawls doesn't make much sense.
```

### Comparing `Scrapy-2.8.0/docs/topics/commands.rst` & `Scrapy-2.9.0/docs/topics/commands.rst`

 * *Files 5% similar despite different names*

```diff
@@ -234,17 +234,14 @@
 * Requires project: *no*
 
 .. versionadded:: 2.6.0
    The ability to pass a URL instead of a domain.
 
 Create a new spider in the current folder or in the current project's ``spiders`` folder, if called from inside a project. The ``<name>`` parameter is set as the spider's ``name``, while ``<domain or URL>`` is used to generate the ``allowed_domains`` and ``start_urls`` spider's attributes.
 
-.. note:: Even if an HTTPS URL is specified, the protocol used in
-          ``start_urls`` is always HTTP. This is a known issue: :issue:`3553`.
-
 Usage example::
 
     $ scrapy genspider -l
     Available templates:
       basic
       crawl
       csvfeed
@@ -284,21 +281,21 @@
 * ``--output-format FORMAT`` or ``-t FORMAT``: deprecated way to define format to use for dumping items, does not work in combination with ``-O``
 
 Usage examples::
 
     $ scrapy crawl myspider
     [ ... myspider starts crawling ... ]
 
-    $ scrapy -o myfile:csv myspider
+    $ scrapy crawl -o myfile:csv myspider
     [ ... myspider starts crawling and appends the result to the file myfile in csv format ... ]
 
-    $ scrapy -O myfile:json myspider
+    $ scrapy crawl -O myfile:json myspider
     [ ... myspider starts crawling and saves the result in myfile in json format overwriting the original content... ]
 
-    $ scrapy -o myfile -t csv myspider
+    $ scrapy crawl -o myfile -t csv myspider
     [ ... myspider starts crawling and appends the result to the file myfile in csv format ... ]
 
 .. command:: check
 
 check
 -----
 
@@ -613,15 +610,15 @@
 A module to use for looking up custom Scrapy commands. This is used to add custom
 commands for your Scrapy project.
 
 Example:
 
 .. code-block:: python
 
-    COMMANDS_MODULE = 'mybot.commands'
+    COMMANDS_MODULE = "mybot.commands"
 
 .. _Deploying your project: https://scrapyd.readthedocs.io/en/latest/deploy.html
 
 Register commands via setup.py entry points
 -------------------------------------------
 
 You can also add Scrapy commands from an external library by adding a
@@ -632,14 +629,15 @@
 
 .. skip: next
 
 .. code-block:: python
 
   from setuptools import setup, find_packages
 
-  setup(name='scrapy-mymodule',
-    entry_points={
-      'scrapy.commands': [
-        'my_command=my_scrapy_module.commands:MyCommand',
-      ],
-    },
-   )
+  setup(
+      name="scrapy-mymodule",
+      entry_points={
+          "scrapy.commands": [
+              "my_command=my_scrapy_module.commands:MyCommand",
+          ],
+      },
+  )
```

### Comparing `Scrapy-2.8.0/docs/topics/components.rst` & `Scrapy-2.9.0/docs/topics/components.rst`

 * *Files 4% similar despite different names*

```diff
@@ -62,23 +62,25 @@
 parameter to the exception so that it is printed in the logs, for the user to
 see. For other components, feel free to raise whatever other exception feels
 right to you; for example, :exc:`RuntimeError` would make sense for a Scrapy
 version mismatch, while :exc:`ValueError` may be better if the issue is the
 value of a setting.
 
 If your requirement is a minimum Scrapy version, you may use
-:attr:`scrapy.__version__` to enforce your requirement. For example::
+:attr:`scrapy.__version__` to enforce your requirement. For example:
+
+.. code-block:: python
 
     from pkg_resources import parse_version
 
     import scrapy
 
-    class MyComponent:
 
+    class MyComponent:
         def __init__(self):
-            if parse_version(scrapy.__version__) < parse_version('2.7'):
+            if parse_version(scrapy.__version__) < parse_version("2.7"):
                 raise RuntimeError(
                     f"{MyComponent.__qualname__} requires Scrapy 2.7 or "
                     f"later, which allow defining the process_spider_output "
                     f"method of spider middlewares as an asynchronous "
                     f"generator."
                 )
```

### Comparing `Scrapy-2.8.0/docs/topics/contracts.rst` & `Scrapy-2.9.0/docs/topics/contracts.rst`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 Testing spiders can get particularly annoying and while nothing prevents you
 from writing unit tests the task gets cumbersome quickly. Scrapy offers an
 integrated way of testing your spiders by the means of contracts.
 
 This allows you to test each callback of your spider by hardcoding a sample url
 and check various constraints for how the callback processes the response. Each
 contract is prefixed with an ``@`` and included in the docstring. See the
-following example::
+following example:
+
+.. code-block:: python
 
     def parse(self, response):
-        """ This function parses a sample response. Some contracts are mingled
+        """
+        This function parses a sample response. Some contracts are mingled
         with this docstring.
 
         @url http://www.amazon.com/s?field-keywords=selfish+gene
         @returns items 1 16
         @returns requests 0 0
         @scrapes Title Author Year Price
         """
@@ -60,19 +63,21 @@
 Use the :command:`check` command to run the contract checks.
 
 Custom Contracts
 ================
 
 If you find you need more power than the built-in Scrapy contracts you can
 create and load your own contracts in the project by using the
-:setting:`SPIDER_CONTRACTS` setting::
+:setting:`SPIDER_CONTRACTS` setting:
+
+.. code-block:: python
 
     SPIDER_CONTRACTS = {
-        'myproject.contracts.ResponseCheck': 10,
-        'myproject.contracts.ItemValidate': 10,
+        "myproject.contracts.ResponseCheck": 10,
+        "myproject.contracts.ItemValidate": 10,
     }
 
 Each contract must inherit from :class:`~scrapy.contracts.Contract` and can
 override three methods:
 
 .. module:: scrapy.contracts
 
@@ -107,42 +112,50 @@
 Raise :class:`~scrapy.exceptions.ContractFail` from
 :class:`~scrapy.contracts.Contract.pre_process` or
 :class:`~scrapy.contracts.Contract.post_process` if expectations are not met:
 
 .. autoclass:: scrapy.exceptions.ContractFail
 
 Here is a demo contract which checks the presence of a custom header in the
-response received::
+response received:
+
+.. skip: next
+.. code-block:: python
 
     from scrapy.contracts import Contract
     from scrapy.exceptions import ContractFail
 
+
     class HasHeaderContract(Contract):
-        """ Demo contract which checks the presence of a custom header
-            @has_header X-CustomHeader
+        """
+        Demo contract which checks the presence of a custom header
+        @has_header X-CustomHeader
         """
 
-        name = 'has_header'
+        name = "has_header"
 
         def pre_process(self, response):
             for header in self.args:
                 if header not in response.headers:
-                    raise ContractFail('X-CustomHeader not present')
+                    raise ContractFail("X-CustomHeader not present")
 
 .. _detecting-contract-check-runs:
 
 Detecting check runs
 ====================
 
 When ``scrapy check`` is running, the ``SCRAPY_CHECK`` environment variable is
 set to the ``true`` string. You can use :data:`os.environ` to perform any change to
-your spiders or your settings when ``scrapy check`` is used::
+your spiders or your settings when ``scrapy check`` is used:
+
+.. code-block:: python
 
     import os
     import scrapy
 
+
     class ExampleSpider(scrapy.Spider):
-        name = 'example'
+        name = "example"
 
         def __init__(self):
-            if os.environ.get('SCRAPY_CHECK'):
+            if os.environ.get("SCRAPY_CHECK"):
                 pass  # Do some scraper adjustments when a check is running
```

### Comparing `Scrapy-2.8.0/docs/topics/coroutines.rst` & `Scrapy-2.9.0/docs/topics/coroutines.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,57 +54,67 @@
 General usage
 =============
 
 There are several use cases for coroutines in Scrapy.
 
 Code that would return Deferreds when written for previous Scrapy versions,
 such as downloader middlewares and signal handlers, can be rewritten to be
-shorter and cleaner::
+shorter and cleaner:
+
+.. code-block:: python
 
     from itemadapter import ItemAdapter
 
+
     class DbPipeline:
         def _update_item(self, data, item):
             adapter = ItemAdapter(item)
-            adapter['field'] = data
+            adapter["field"] = data
             return item
 
         def process_item(self, item, spider):
             adapter = ItemAdapter(item)
-            dfd = db.get_some_data(adapter['id'])
+            dfd = db.get_some_data(adapter["id"])
             dfd.addCallback(self._update_item, item)
             return dfd
 
-becomes::
+becomes:
+
+.. code-block:: python
 
     from itemadapter import ItemAdapter
 
+
     class DbPipeline:
         async def process_item(self, item, spider):
             adapter = ItemAdapter(item)
-            adapter['field'] = await db.get_some_data(adapter['id'])
+            adapter["field"] = await db.get_some_data(adapter["id"])
             return item
 
 Coroutines may be used to call asynchronous code. This includes other
 coroutines, functions that return Deferreds and functions that return
 :term:`awaitable objects <awaitable>` such as :class:`~asyncio.Future`.
-This means you can use many useful Python libraries providing such code::
+This means you can use many useful Python libraries providing such code:
+
+.. skip: next
+.. code-block:: python
 
     class MySpiderDeferred(Spider):
         # ...
         async def parse(self, response):
-            additional_response = await treq.get('https://additional.url')
+            additional_response = await treq.get("https://additional.url")
             additional_data = await treq.content(additional_response)
             # ... use response and additional_data to yield items and requests
 
+
     class MySpiderAsyncio(Spider):
         # ...
         async def parse(self, response):
             async with aiohttp.ClientSession() as session:
-                async with session.get('https://additional.url') as additional_response:
+                async with session.get("https://additional.url") as additional_response:
                     additional_data = await additional_response.text()
             # ... use response and additional_data to yield items and requests
 
 .. note:: Many libraries that use coroutines, such as `aio-libs`_, require the
           :mod:`asyncio` loop and to use them you need to
           :doc:`enable asyncio support in Scrapy<asyncio>`.
 
@@ -188,15 +198,17 @@
 its ``process_spider_output`` method in Scrapy 2.7 and later (avoiding
 :ref:`asynchronous-to-synchronous conversions <sync-async-spider-middleware>`)
 while maintaining support for older Scrapy versions, you may define
 ``process_spider_output`` as a synchronous method and define an
 :term:`asynchronous generator` version of that method with an alternative name:
 ``process_spider_output_async``.
 
-For example::
+For example:
+
+.. code-block:: python
 
     class UniversalSpiderMiddleware:
         def process_spider_output(self, response, result, spider):
             for r in result:
                 # ... do something with r
                 yield r
```

### Comparing `Scrapy-2.8.0/docs/topics/debug.rst` & `Scrapy-2.9.0/docs/topics/debug.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 .. _topics-debug:
 
 =================
 Debugging Spiders
 =================
 
 This document explains the most common techniques for debugging spiders.
-Consider the following Scrapy spider below::
+Consider the following Scrapy spider below:
+
+.. skip: next
+.. code-block:: python
 
     import scrapy
     from myproject.items import MyItem
 
+
     class MySpider(scrapy.Spider):
-        name = 'myspider'
+        name = "myspider"
         start_urls = (
-            'http://example.com/page1',
-            'http://example.com/page2',
-            )
+            "http://example.com/page1",
+            "http://example.com/page2",
+        )
 
         def parse(self, response):
             # <processing code not shown>
             # collect `item_urls`
             for item_url in item_urls:
                 yield scrapy.Request(item_url, self.parse_item)
 
         def parse_item(self, response):
             # <processing code not shown>
             item = MyItem()
             # populate `item` fields
             # and extract item_details_url
-            yield scrapy.Request(item_details_url, self.parse_details, cb_kwargs={'item': item})
+            yield scrapy.Request(
+                item_details_url, self.parse_details, cb_kwargs={"item": item}
+            )
 
         def parse_details(self, response, item):
             # populate more `item` fields
             return item
 
 Basically this is a simple spider which parses two pages of items (the
 start_urls). Items also have a details page with additional information, so we
@@ -99,57 +105,65 @@
 spider, it is of little help to check what happens inside a callback, besides
 showing the response received and the output. How to debug the situation when
 ``parse_details`` sometimes receives no item?
 
 .. highlight:: python
 
 Fortunately, the :command:`shell` is your bread and butter in this case (see
-:ref:`topics-shell-inspect-response`)::
+:ref:`topics-shell-inspect-response`):
+
+.. code-block:: python
 
     from scrapy.shell import inspect_response
 
+
     def parse_details(self, response, item=None):
         if item:
             # populate more `item` fields
             return item
         else:
             inspect_response(response, self)
 
 See also: :ref:`topics-shell-inspect-response`.
 
 Open in browser
 ===============
 
 Sometimes you just want to see how a certain response looks in a browser, you
 can use the ``open_in_browser`` function for that. Here is an example of how
-you would use it::
+you would use it:
+
+.. code-block:: python
 
     from scrapy.utils.response import open_in_browser
 
+
     def parse_details(self, response):
         if "item name" not in response.body:
             open_in_browser(response)
 
 ``open_in_browser`` will open a browser with the response received by Scrapy at
 that point, adjusting the `base tag`_ so that images and styles are displayed
 properly.
 
 Logging
 =======
 
 Logging is another useful option for getting information about your spider run.
 Although not as convenient, it comes with the advantage that the logs will be
-available in all future runs should they be necessary again::
+available in all future runs should they be necessary again:
+
+.. code-block:: python
 
     def parse_details(self, response, item=None):
         if item:
             # populate more `item` fields
             return item
         else:
-            self.logger.warning('No item received for %s', response.url)
+            self.logger.warning("No item received for %s", response.url)
 
 For more information, check the :ref:`topics-logging` section.
 
 .. _base tag: https://www.w3schools.com/tags/tag_base.asp
 
 .. _debug-vscode:
```

### Comparing `Scrapy-2.8.0/docs/topics/deploy.rst` & `Scrapy-2.9.0/docs/topics/deploy.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/developer-tools.rst` & `Scrapy-2.9.0/docs/topics/developer-tools.rst`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,18 @@
 Then, back to your web browser, right-click on the ``span`` tag, select
 ``Copy > XPath`` and paste it in the Scrapy shell like so:
 
 .. invisible-code-block: python
 
     response = load_response('https://quotes.toscrape.com/', 'quotes.html')
 
->>> response.xpath('/html/body/div/div[2]/div[1]/div[1]/span[1]/text()').getall()
-['“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”']
+.. code-block:: pycon
+
+  >>> response.xpath("/html/body/div/div[2]/div[1]/div[1]/span[1]/text()").getall()
+  ['“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”']
 
 Adding ``text()`` at the end we are able to extract the first quote with this
 basic selector. But this XPath is not really that clever. All it does is
 go down a desired path in the source code starting from ``html``. So let's
 see if we can refine our XPath a bit:
 
 If we check the `Inspector` again we'll see that directly beneath our
@@ -120,19 +122,21 @@
     </div>
 
 
 With this knowledge we can refine our XPath: Instead of a path to follow,
 we'll simply select all ``span`` tags with the ``class="text"`` by using
 the `has-class-extension`_:
 
->>> response.xpath('//span[has-class("text")]/text()').getall()
-['“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”',
-'“It is our choices, Harry, that show what we truly are, far more than our abilities.”',
-'“There are only two ways to live your life. One is as though nothing is a miracle. The other is as though everything is a miracle.”',
-...]
+.. code-block:: pycon
+
+    >>> response.xpath('//span[has-class("text")]/text()').getall()
+    ['“The world as we have created it is a process of our thinking. It cannot be changed without changing our thinking.”',
+    '“It is our choices, Harry, that show what we truly are, far more than our abilities.”',
+    '“There are only two ways to live your life. One is as though nothing is a miracle. The other is as though everything is a miracle.”',
+    ...]
 
 And with one simple, cleverer XPath we are able to extract all quotes from
 the page. We could have constructed a loop over our first XPath to increase
 the number of the last ``div``, but this would have been unnecessarily
 complex and by simply constructing an XPath with ``has-class("text")``
 we were able to extract all quotes in one line.
 
@@ -233,25 +237,27 @@
 
 .. image:: _images/network_03.png
    :width: 777
    :height: 375
    :alt: JSON-object returned from the quotes.toscrape API
 
 With this response we can now easily parse the JSON-object and
-also request each page to get every quote on the site::
+also request each page to get every quote on the site:
+
+.. code-block:: python
 
     import scrapy
     import json
 
 
     class QuoteSpider(scrapy.Spider):
-        name = 'quote'
-        allowed_domains = ['quotes.toscrape.com']
+        name = "quote"
+        allowed_domains = ["quotes.toscrape.com"]
         page = 1
-        start_urls = ['https://quotes.toscrape.com/api/quotes?page=1']
+        start_urls = ["https://quotes.toscrape.com/api/quotes?page=1"]
 
         def parse(self, response):
             data = json.loads(response.text)
             for quote in data["quotes"]:
                 yield {"quote": quote["text"]}
             if data["has_next"]:
                 self.page += 1
@@ -271,26 +277,29 @@
 .. _requests-from-curl:
 
 In more complex websites, it could be difficult to easily reproduce the
 requests, as we could need to add ``headers`` or ``cookies`` to make it work.
 In those cases you can export the requests in `cURL <https://curl.haxx.se/>`_
 format, by right-clicking on each of them in the network tool and using the
 :meth:`~scrapy.Request.from_curl()` method to generate an equivalent
-request::
+request:
+
+.. code-block:: python
 
     from scrapy import Request
 
     request = Request.from_curl(
         "curl 'https://quotes.toscrape.com/api/quotes?page=1' -H 'User-Agent: Mozil"
         "la/5.0 (X11; Linux x86_64; rv:67.0) Gecko/20100101 Firefox/67.0' -H 'Acce"
         "pt: */*' -H 'Accept-Language: ca,en-US;q=0.7,en;q=0.3' --compressed -H 'X"
         "-Requested-With: XMLHttpRequest' -H 'Proxy-Authorization: Basic QFRLLTAzM"
         "zEwZTAxLTk5MWUtNDFiNC1iZWRmLTJjNGI4M2ZiNDBmNDpAVEstMDMzMTBlMDEtOTkxZS00MW"
         "I0LWJlZGYtMmM0YjgzZmI0MGY0' -H 'Connection: keep-alive' -H 'Referer: http"
-        "://quotes.toscrape.com/scroll' -H 'Cache-Control: max-age=0'")
+        "://quotes.toscrape.com/scroll' -H 'Cache-Control: max-age=0'"
+    )
 
 Alternatively, if you want to know the arguments needed to recreate that
 request you can use the :func:`~scrapy.utils.curl.curl_to_request_kwargs`
 function to get a dictionary with the equivalent arguments:
 
 .. autofunction:: scrapy.utils.curl.curl_to_request_kwargs
```

### Comparing `Scrapy-2.8.0/docs/topics/downloader-middleware.rst` & `Scrapy-2.9.0/docs/topics/downloader-middleware.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 Activating a downloader middleware
 ==================================
 
 To activate a downloader middleware component, add it to the
 :setting:`DOWNLOADER_MIDDLEWARES` setting, which is a dict whose keys are the
 middleware class paths and their values are the middleware orders.
 
-Here's an example::
+Here's an example:
+
+.. code-block:: python
 
     DOWNLOADER_MIDDLEWARES = {
-        'myproject.middlewares.CustomDownloaderMiddleware': 543,
+        "myproject.middlewares.CustomDownloaderMiddleware": 543,
     }
 
 The :setting:`DOWNLOADER_MIDDLEWARES` setting is merged with the
 :setting:`DOWNLOADER_MIDDLEWARES_BASE` setting defined in Scrapy (and not meant
 to be overridden) and then sorted by order to get the final sorted list of
 enabled middlewares: the first middleware is the one closer to the engine and
 the last is the one closer to the downloader. In other words,
@@ -38,19 +40,21 @@
 where you want to insert the middleware. The order does matter because each
 middleware performs a different action and your middleware could depend on some
 previous (or subsequent) middleware being applied.
 
 If you want to disable a built-in middleware (the ones defined in
 :setting:`DOWNLOADER_MIDDLEWARES_BASE` and enabled by default) you must define it
 in your project's :setting:`DOWNLOADER_MIDDLEWARES` setting and assign ``None``
-as its value.  For example, if you want to disable the user-agent middleware::
+as its value.  For example, if you want to disable the user-agent middleware:
+
+.. code-block:: python
 
     DOWNLOADER_MIDDLEWARES = {
-        'myproject.middlewares.CustomDownloaderMiddleware': 543,
-        'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': None,
+        "myproject.middlewares.CustomDownloaderMiddleware": 543,
+        "scrapy.downloadermiddlewares.useragent.UserAgentMiddleware": None,
     }
 
 Finally, keep in mind that some middlewares may need to be enabled through a
 particular setting. See each middleware documentation for more info.
 
 .. _topics-downloader-middleware-custom:
 
@@ -222,28 +226,34 @@
 Multiple cookie sessions per spider
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 There is support for keeping multiple cookie sessions per spider by using the
 :reqmeta:`cookiejar` Request meta key. By default it uses a single cookie jar
 (session), but you can pass an identifier to use different ones.
 
-For example::
+For example:
+
+.. skip: next
+.. code-block:: python
 
     for i, url in enumerate(urls):
-        yield scrapy.Request(url, meta={'cookiejar': i},
-            callback=self.parse_page)
+        yield scrapy.Request(url, meta={"cookiejar": i}, callback=self.parse_page)
 
 Keep in mind that the :reqmeta:`cookiejar` meta key is not "sticky". You need to keep
-passing it along on subsequent requests. For example::
+passing it along on subsequent requests. For example:
+
+.. code-block:: python
 
     def parse_page(self, response):
         # do some processing
-        return scrapy.Request("http://www.example.com/otherpage",
-            meta={'cookiejar': response.meta['cookiejar']},
-            callback=self.parse_other_page)
+        return scrapy.Request(
+            "http://www.example.com/otherpage",
+            meta={"cookiejar": response.meta["cookiejar"]},
+            callback=self.parse_other_page,
+        )
 
 .. setting:: COOKIES_ENABLED
 
 COOKIES_ENABLED
 ~~~~~~~~~~~~~~~
 
 Default: ``True``
@@ -335,24 +345,26 @@
         In previous Scrapy versions HttpAuthMiddleware sent the authentication
         data with all requests, which is a security problem if the spider
         makes requests to several different domains. Currently if the
         ``http_auth_domain`` attribute is not set, the middleware will use the
         domain of the first request, which will work for some spiders but not
         for others. In the future the middleware will produce an error instead.
 
-    Example::
+    Example:
+
+    .. code-block:: python
 
         from scrapy.spiders import CrawlSpider
 
-        class SomeIntranetSiteSpider(CrawlSpider):
 
-            http_user = 'someuser'
-            http_pass = 'somepass'
-            http_auth_domain = 'intranet.example.com'
-            name = 'intranet.example.com'
+        class SomeIntranetSiteSpider(CrawlSpider):
+            http_user = "someuser"
+            http_pass = "somepass"
+            http_auth_domain = "intranet.example.com"
+            name = "intranet.example.com"
 
             # .. rest of the spider code omitted ...
 
 .. _Basic access authentication: https://en.wikipedia.org/wiki/Basic_access_authentication
 
 
 HttpCacheMiddleware
@@ -788,15 +800,17 @@
 If :attr:`Request.meta <scrapy.Request.meta>` has ``dont_redirect``
 key set to True, the request will be ignored by this middleware.
 
 If you want to handle some redirect status codes in your spider, you can
 specify these in the ``handle_httpstatus_list`` spider attribute.
 
 For example, if you want the redirect middleware to ignore 301 and 302
-responses (and pass them through to your spider) you can do this::
+responses (and pass them through to your spider) you can do this:
+
+.. code-block:: python
 
     class MySpider(CrawlSpider):
         handle_httpstatus_list = [301, 302]
 
 The ``handle_httpstatus_list`` key of :attr:`Request.meta
 <scrapy.Request.meta>` can also be used to specify which response codes to
 allow on a per-request basis. You can also set the meta key
```

### Comparing `Scrapy-2.8.0/docs/topics/dynamic-content.rst` & `Scrapy-2.9.0/docs/topics/dynamic-content.rst`

 * *Files 2% similar despite different names*

```diff
@@ -115,24 +115,28 @@
 Once you have a response with the desired data, how you extract the desired
 data from it depends on the type of response:
 
 -   If the response is HTML or XML, use :ref:`selectors
     <topics-selectors>` as usual.
 
 -   If the response is JSON, use :func:`json.loads` to load the desired data from
-    :attr:`response.text <scrapy.http.TextResponse.text>`::
+    :attr:`response.text <scrapy.http.TextResponse.text>`:
+
+    .. code-block:: python
 
         data = json.loads(response.text)
 
     If the desired data is inside HTML or XML code embedded within JSON data,
     you can load that HTML or XML code into a
     :class:`~scrapy.Selector` and then
-    :ref:`use it <topics-selectors>` as usual::
+    :ref:`use it <topics-selectors>` as usual:
+
+    .. code-block:: python
 
-        selector = Selector(data['html'])
+        selector = Selector(data["html"])
 
 -   If the response is JavaScript, or HTML with a ``<script/>`` element
     containing the desired data, see :ref:`topics-parsing-javascript`.
 
 -   If the response is CSS, use a :doc:`regular expression <library/re>` to
     extract the desired data from
     :attr:`response.text <scrapy.http.TextResponse.text>`.
@@ -175,45 +179,51 @@
 -   You might be able to use a :doc:`regular expression <library/re>` to
     extract the desired data in JSON format, which you can then parse with
     :func:`json.loads`.
 
     For example, if the JavaScript code contains a separate line like
     ``var data = {"field": "value"};`` you can extract that data as follows:
 
-    >>> pattern = r'\bvar\s+data\s*=\s*(\{.*?\})\s*;\s*\n'
-    >>> json_data = response.css('script::text').re_first(pattern)
-    >>> json.loads(json_data)
-    {'field': 'value'}
+    .. code-block:: pycon
+
+        >>> pattern = r"\bvar\s+data\s*=\s*(\{.*?\})\s*;\s*\n"
+        >>> json_data = response.css("script::text").re_first(pattern)
+        >>> json.loads(json_data)
+        {'field': 'value'}
 
 -   chompjs_ provides an API to parse JavaScript objects into a :class:`dict`.
 
     For example, if the JavaScript code contains
     ``var data = {field: "value", secondField: "second value"};``
     you can extract that data as follows:
 
-    >>> import chompjs
-    >>> javascript = response.css('script::text').get()
-    >>> data = chompjs.parse_js_object(javascript)
-    >>> data
-    {'field': 'value', 'secondField': 'second value'}
+    .. code-block:: pycon
+
+        >>> import chompjs
+        >>> javascript = response.css("script::text").get()
+        >>> data = chompjs.parse_js_object(javascript)
+        >>> data
+        {'field': 'value', 'secondField': 'second value'}
 
 -   Otherwise, use js2xml_ to convert the JavaScript code into an XML document
     that you can parse using :ref:`selectors <topics-selectors>`.
 
     For example, if the JavaScript code contains
     ``var data = {field: "value"};`` you can extract that data as follows:
 
-    >>> import js2xml
-    >>> import lxml.etree
-    >>> from parsel import Selector
-    >>> javascript = response.css('script::text').get()
-    >>> xml = lxml.etree.tostring(js2xml.parse(javascript), encoding='unicode')
-    >>> selector = Selector(text=xml)
-    >>> selector.css('var[name="data"]').get()
-    '<var name="data"><object><property name="field"><string>value</string></property></object></var>'
+    .. code-block:: pycon
+
+        >>> import js2xml
+        >>> import lxml.etree
+        >>> from parsel import Selector
+        >>> javascript = response.css("script::text").get()
+        >>> xml = lxml.etree.tostring(js2xml.parse(javascript), encoding="unicode")
+        >>> selector = Selector(text=xml)
+        >>> selector.css('var[name="data"]').get()
+        '<var name="data"><object><property name="field"><string>value</string></property></object></var>'
 
 .. _topics-javascript-rendering:
 
 Pre-rendering JavaScript
 ========================
 
 On webpages that fetch data from additional requests, reproducing those
@@ -246,28 +256,31 @@
 ========================
 
 A `headless browser`_ is a special web browser that provides an API for
 automation. By installing the :ref:`asyncio reactor <install-asyncio>`,
 it is possible to integrate ``asyncio``-based libraries which handle headless browsers.
 
 One such library is `playwright-python`_ (an official Python port of `playwright`_).
-The following is a simple snippet to illustrate its usage within a Scrapy spider::
+The following is a simple snippet to illustrate its usage within a Scrapy spider:
+
+.. code-block:: python
 
     import scrapy
     from playwright.async_api import async_playwright
 
+
     class PlaywrightSpider(scrapy.Spider):
         name = "playwright"
         start_urls = ["data:,"]  # avoid using the default Scrapy downloader
 
         async def parse(self, response):
             async with async_playwright() as pw:
                 browser = await pw.chromium.launch()
                 page = await browser.new_page()
-                await page.goto("https:/example.org")
+                await page.goto("https://example.org")
                 title = await page.title()
                 return {"title": title}
 
 
 However, using `playwright-python`_ directly as in the above example
 circumvents most of the Scrapy components (middlewares, dupefilter, etc).
 We recommend using `scrapy-playwright`_ for a better integration.
```

### Comparing `Scrapy-2.8.0/docs/topics/email.rst` & `Scrapy-2.9.0/docs/topics/email.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,41 @@
 it's very easy to configure, with a few :ref:`settings
 <topics-email-settings>`.
 
 Quick example
 =============
 
 There are two ways to instantiate the mail sender. You can instantiate it using
-the standard ``__init__`` method::
+the standard ``__init__`` method:
+
+.. code-block:: python
 
     from scrapy.mail import MailSender
+
     mailer = MailSender()
 
 Or you can instantiate it passing a Scrapy settings object, which will respect
-the :ref:`settings <topics-email-settings>`::
+the :ref:`settings <topics-email-settings>`:
+
+.. skip: start
+.. code-block:: python
 
     mailer = MailSender.from_settings(settings)
 
-And here is how to use it to send an e-mail (without attachments)::
+And here is how to use it to send an e-mail (without attachments):
+
+.. code-block:: python
 
-    mailer.send(to=["someone@example.com"], subject="Some subject", body="Some body", cc=["another@example.com"])
+    mailer.send(
+        to=["someone@example.com"],
+        subject="Some subject",
+        body="Some body",
+        cc=["another@example.com"],
+    )
+.. skip: end
 
 MailSender class reference
 ==========================
 
 MailSender is the preferred class to use for sending emails from Scrapy, as it
 uses :doc:`Twisted non-blocking IO <twisted:core/howto/defer-intro>`, like the
 rest of the framework.
```

### Comparing `Scrapy-2.8.0/docs/topics/exceptions.rst` & `Scrapy-2.9.0/docs/topics/exceptions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 
     This exception can be raised from a spider callback to request the spider to be
     closed/stopped. Supported arguments:
 
     :param reason: the reason for closing
     :type reason: str
 
-For example::
+For example:
+
+.. code-block:: python
 
     def parse_page(self, response):
-        if 'Bandwidth exceeded' in response.body:
-            raise CloseSpider('bandwidth_exceeded')
+        if "Bandwidth exceeded" in response.body:
+            raise CloseSpider("bandwidth_exceeded")
 
 DontCloseSpider
 ---------------
 
 .. exception:: DontCloseSpider
 
 This exception can be raised in a :signal:`spider_idle` signal handler to
```

### Comparing `Scrapy-2.8.0/docs/topics/exporters.rst` & `Scrapy-2.9.0/docs/topics/exporters.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,35 +34,38 @@
 to export
 
 3. and finally call the :meth:`~BaseItemExporter.finish_exporting` to signal
 the end of the exporting process
 
 Here you can see an :doc:`Item Pipeline <item-pipeline>` which uses multiple
 Item Exporters to group scraped items to different files according to the
-value of one of their fields::
+value of one of their fields:
+
+.. code-block:: python
 
     from itemadapter import ItemAdapter
     from scrapy.exporters import XmlItemExporter
 
+
     class PerYearXmlExportPipeline:
         """Distribute items across multiple XML files according to their 'year' field"""
 
         def open_spider(self, spider):
             self.year_to_exporter = {}
 
         def close_spider(self, spider):
             for exporter, xml_file in self.year_to_exporter.values():
                 exporter.finish_exporting()
                 xml_file.close()
 
         def _exporter_for_item(self, item):
             adapter = ItemAdapter(item)
-            year = adapter['year']
+            year = adapter["year"]
             if year not in self.year_to_exporter:
-                xml_file = open(f'{year}.xml', 'wb')
+                xml_file = open(f"{year}.xml", "wb")
                 exporter = XmlItemExporter(xml_file)
                 exporter.start_exporting()
                 self.year_to_exporter[year] = (exporter, xml_file)
             return self.year_to_exporter[year][0]
 
         def process_item(self, item, spider):
             exporter = self._exporter_for_item(item)
@@ -90,20 +93,24 @@
 1. Declaring a serializer in the field
 --------------------------------------
 
 If you use :class:`~scrapy.Item` you can declare a serializer in the
 :ref:`field metadata <topics-items-fields>`. The serializer must be
 a callable which receives a value and returns its serialized form.
 
-Example::
+Example:
+
+.. code-block:: python
 
     import scrapy
 
+
     def serialize_price(value):
-        return f'$ {str(value)}'
+        return f"$ {str(value)}"
+
 
     class Product(scrapy.Item):
         name = scrapy.Field()
         price = scrapy.Field(serializer=serialize_price)
 
 
 2. Overriding the serialize_field() method
@@ -111,35 +118,40 @@
 
 You can also override the :meth:`~BaseItemExporter.serialize_field()` method to
 customize how your field value will be exported.
 
 Make sure you call the base class :meth:`~BaseItemExporter.serialize_field()` method
 after your custom code.
 
-Example::
+Example:
+
+.. code-block:: python
 
       from scrapy.exporters import XmlItemExporter
 
-      class ProductXmlExporter(XmlItemExporter):
 
+      class ProductXmlExporter(XmlItemExporter):
           def serialize_field(self, field, name, value):
-              if name == 'price':
-                  return f'$ {str(value)}'
+              if name == "price":
+                  return f"$ {str(value)}"
               return super().serialize_field(field, name, value)
 
 .. _topics-exporters-reference:
 
 Built-in Item Exporters reference
 =================================
 
 Here is a list of the Item Exporters bundled with Scrapy. Some of them contain
-output examples, which assume you're exporting these two items::
+output examples, which assume you're exporting these two items:
+
+.. skip: next
+.. code-block:: python
 
-    Item(name='Color TV', price='1200')
-    Item(name='DVD player', price='200')
+    Item(name="Color TV", price="1200")
+    Item(name="DVD player", price="200")
 
 BaseItemExporter
 ----------------
 
 .. class:: BaseItemExporter(fields_to_export=None, export_empty_fields=False, encoding='utf-8', indent=0, dont_fail=False)
 
    This is the (abstract) base class for all Item Exporters. It provides
```

### Comparing `Scrapy-2.8.0/docs/topics/extensions.rst` & `Scrapy-2.9.0/docs/topics/extensions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 
 Extensions are loaded and activated at startup by instantiating a single
 instance of the extension class per spider being run. All the extension
 initialization code must be performed in the class ``__init__`` method.
 
 To make an extension available, add it to the :setting:`EXTENSIONS` setting in
 your Scrapy settings. In :setting:`EXTENSIONS`, each extension is represented
-by a string: the full Python path to the extension's class name. For example::
+by a string: the full Python path to the extension's class name. For example:
+
+.. code-block:: python
 
     EXTENSIONS = {
-        'scrapy.extensions.corestats.CoreStats': 500,
-        'scrapy.extensions.telnet.TelnetConsole': 500,
+        "scrapy.extensions.corestats.CoreStats": 500,
+        "scrapy.extensions.telnet.TelnetConsole": 500,
     }
 
 
 As you can see, the :setting:`EXTENSIONS` setting is a dict where the keys are
 the extension paths, and their values are the orders, which define the
 extension *loading* order. The :setting:`EXTENSIONS` setting is merged with the
 :setting:`EXTENSIONS_BASE` setting defined in Scrapy (and not meant to be
@@ -60,18 +62,20 @@
 but disabled unless the :setting:`HTTPCACHE_ENABLED` setting is set.
 
 Disabling an extension
 ======================
 
 In order to disable an extension that comes enabled by default (i.e. those
 included in the :setting:`EXTENSIONS_BASE` setting) you must set its order to
-``None``. For example::
+``None``. For example:
+
+.. code-block:: python
 
     EXTENSIONS = {
-        'scrapy.extensions.corestats.CoreStats': None,
+        "scrapy.extensions.corestats.CoreStats": None,
     }
 
 Writing your own extension
 ==========================
 
 Each extension is a Python class. The main entry point for a Scrapy extension
 (this also includes middlewares and pipelines) is the ``from_crawler``
@@ -94,37 +98,39 @@
 * a spider is opened
 * a spider is closed
 * a specific number of items are scraped
 
 The extension will be enabled through the ``MYEXT_ENABLED`` setting and the
 number of items will be specified through the ``MYEXT_ITEMCOUNT`` setting.
 
-Here is the code of such extension::
+Here is the code of such extension:
+
+.. code-block:: python
 
     import logging
     from scrapy import signals
     from scrapy.exceptions import NotConfigured
 
     logger = logging.getLogger(__name__)
 
-    class SpiderOpenCloseLogging:
 
+    class SpiderOpenCloseLogging:
         def __init__(self, item_count):
             self.item_count = item_count
             self.items_scraped = 0
 
         @classmethod
         def from_crawler(cls, crawler):
             # first check if the extension should be enabled and raise
             # NotConfigured otherwise
-            if not crawler.settings.getbool('MYEXT_ENABLED'):
+            if not crawler.settings.getbool("MYEXT_ENABLED"):
                 raise NotConfigured
 
             # get the number of items from settings
-            item_count = crawler.settings.getint('MYEXT_ITEMCOUNT', 1000)
+            item_count = crawler.settings.getint("MYEXT_ITEMCOUNT", 1000)
 
             # instantiate the extension object
             ext = cls(item_count)
 
             # connect the extension object to signals
             crawler.signals.connect(ext.spider_opened, signal=signals.spider_opened)
             crawler.signals.connect(ext.spider_closed, signal=signals.spider_closed)
```

### Comparing `Scrapy-2.8.0/docs/topics/feed-exports.rst` & `Scrapy-2.9.0/docs/topics/feed-exports.rst`

 * *Files 2% similar despite different names*

```diff
@@ -286,18 +286,19 @@
 
 The ``item_classes`` option is implemented by the :class:`~scrapy.extensions.feedexport.ItemFilter`
 class, which is the default value of the ``item_filter`` :ref:`feed option <feed-options>`.
 
 You can create your own custom filtering class by implementing :class:`~scrapy.extensions.feedexport.ItemFilter`'s
 method ``accepts`` and taking ``feed_options`` as an argument.
 
-For instance::
+For instance:
 
-    class MyCustomFilter:
+.. code-block:: python
 
+    class MyCustomFilter:
         def __init__(self, feed_options):
             self.feed_options = feed_options
 
         def accepts(self, item):
             if "field1" in item and item["field1"] == "expected_data":
                 return True
             return False
@@ -590,31 +591,35 @@
 For a complete list of available values, access the `Canned ACL`_ section on Amazon S3 docs.
 
 .. setting:: FEED_STORAGES_BASE
 
 FEED_STORAGES_BASE
 ------------------
 
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        '': 'scrapy.extensions.feedexport.FileFeedStorage',
-        'file': 'scrapy.extensions.feedexport.FileFeedStorage',
-        'stdout': 'scrapy.extensions.feedexport.StdoutFeedStorage',
-        's3': 'scrapy.extensions.feedexport.S3FeedStorage',
-        'ftp': 'scrapy.extensions.feedexport.FTPFeedStorage',
+        "": "scrapy.extensions.feedexport.FileFeedStorage",
+        "file": "scrapy.extensions.feedexport.FileFeedStorage",
+        "stdout": "scrapy.extensions.feedexport.StdoutFeedStorage",
+        "s3": "scrapy.extensions.feedexport.S3FeedStorage",
+        "ftp": "scrapy.extensions.feedexport.FTPFeedStorage",
     }
 
 A dict containing the built-in feed storage backends supported by Scrapy. You
 can disable any of these backends by assigning ``None`` to their URI scheme in
 :setting:`FEED_STORAGES`. E.g., to disable the built-in FTP storage backend
-(without replacement), place this in your ``settings.py``::
+(without replacement), place this in your ``settings.py``:
+
+.. code-block:: python
 
     FEED_STORAGES = {
-        'ftp': None,
+        "ftp": None,
     }
 
 .. setting:: FEED_EXPORTERS
 
 FEED_EXPORTERS
 --------------
 
@@ -624,34 +629,38 @@
 serialization formats and the values are paths to :ref:`Item exporter
 <topics-exporters>` classes.
 
 .. setting:: FEED_EXPORTERS_BASE
 
 FEED_EXPORTERS_BASE
 -------------------
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        'json': 'scrapy.exporters.JsonItemExporter',
-        'jsonlines': 'scrapy.exporters.JsonLinesItemExporter',
-        'jsonl': 'scrapy.exporters.JsonLinesItemExporter',
-        'jl': 'scrapy.exporters.JsonLinesItemExporter',
-        'csv': 'scrapy.exporters.CsvItemExporter',
-        'xml': 'scrapy.exporters.XmlItemExporter',
-        'marshal': 'scrapy.exporters.MarshalItemExporter',
-        'pickle': 'scrapy.exporters.PickleItemExporter',
+        "json": "scrapy.exporters.JsonItemExporter",
+        "jsonlines": "scrapy.exporters.JsonLinesItemExporter",
+        "jsonl": "scrapy.exporters.JsonLinesItemExporter",
+        "jl": "scrapy.exporters.JsonLinesItemExporter",
+        "csv": "scrapy.exporters.CsvItemExporter",
+        "xml": "scrapy.exporters.XmlItemExporter",
+        "marshal": "scrapy.exporters.MarshalItemExporter",
+        "pickle": "scrapy.exporters.PickleItemExporter",
     }
 
 A dict containing the built-in feed exporters supported by Scrapy. You can
 disable any of these exporters by assigning ``None`` to their serialization
 format in :setting:`FEED_EXPORTERS`. E.g., to disable the built-in CSV exporter
-(without replacement), place this in your ``settings.py``::
+(without replacement), place this in your ``settings.py``:
+
+.. code-block:: python
 
     FEED_EXPORTERS = {
-        'csv': None,
+        "csv": None,
     }
 
 
 .. setting:: FEED_EXPORT_BATCH_ITEM_COUNT
 
 FEED_EXPORT_BATCH_ITEM_COUNT
 ----------------------------
@@ -673,15 +682,17 @@
 * ``%(batch_id)d`` - gets replaced by the 1-based sequence number of the batch.
 
   Use :ref:`printf-style string formatting <python:old-string-formatting>` to
   alter the number format. For example, to make the batch ID a 5-digit
   number by introducing leading zeroes as needed, use ``%(batch_id)05d``
   (e.g. ``3`` becomes ``00003``, ``123`` becomes ``00123``).
 
-For instance, if your settings include::
+For instance, if your settings include:
+
+.. code-block:: python
 
     FEED_EXPORT_BATCH_ITEM_COUNT = 100
 
 And your :command:`crawl` command line is::
 
     scrapy crawl spidername -o "dirname/%(batch_id)d-filename%(batch_time)s.json"
 
@@ -742,24 +753,28 @@
 
    .. caution:: The function should return a new dictionary, modifying
                 the received ``params`` in-place is deprecated.
 
 For example, to include the :attr:`name <scrapy.Spider.name>` of the
 source spider in the feed URI:
 
-#.  Define the following function somewhere in your project::
+#.  Define the following function somewhere in your project:
+
+    .. code-block:: python
 
         # myproject/utils.py
         def uri_params(params, spider):
-            return {**params, 'spider_name': spider.name}
+            return {**params, "spider_name": spider.name}
+
+#.  Point :setting:`FEED_URI_PARAMS` to that function in your settings:
 
-#.  Point :setting:`FEED_URI_PARAMS` to that function in your settings::
+    .. code-block:: python
 
         # myproject/settings.py
-        FEED_URI_PARAMS = 'myproject.utils.uri_params'
+        FEED_URI_PARAMS = "myproject.utils.uri_params"
 
 #.  Use ``%(spider_name)s`` in your feed URI::
 
         scrapy crawl <spider_name> -o "%(spider_name)s.jsonl"
 
 
 .. _URIs: https://en.wikipedia.org/wiki/Uniform_Resource_Identifier
```

### Comparing `Scrapy-2.8.0/docs/topics/item-pipeline.rst` & `Scrapy-2.9.0/docs/topics/item-pipeline.rst`

 * *Files 6% similar despite different names*

```diff
@@ -77,47 +77,52 @@
 
 Price validation and dropping items with no prices
 --------------------------------------------------
 
 Let's take a look at the following hypothetical pipeline that adjusts the
 ``price`` attribute for those items that do not include VAT
 (``price_excludes_vat`` attribute), and drops those items which don't
-contain a price::
+contain a price:
+
+.. code-block:: python
 
     from itemadapter import ItemAdapter
     from scrapy.exceptions import DropItem
-    class PricePipeline:
 
+
+    class PricePipeline:
         vat_factor = 1.15
 
         def process_item(self, item, spider):
             adapter = ItemAdapter(item)
-            if adapter.get('price'):
-                if adapter.get('price_excludes_vat'):
-                    adapter['price'] = adapter['price'] * self.vat_factor
+            if adapter.get("price"):
+                if adapter.get("price_excludes_vat"):
+                    adapter["price"] = adapter["price"] * self.vat_factor
                 return item
             else:
                 raise DropItem(f"Missing price in {item}")
 
 
 Write items to a JSON lines file
 --------------------------------
 
 The following pipeline stores all scraped items (from all spiders) into a
 single ``items.jsonl`` file, containing one item per line serialized in JSON
-format::
+format:
+
+.. code-block:: python
 
    import json
 
    from itemadapter import ItemAdapter
 
-   class JsonWriterPipeline:
 
+   class JsonWriterPipeline:
        def open_spider(self, spider):
-           self.file = open('items.jsonl', 'w')
+           self.file = open("items.jsonl", "w")
 
        def close_spider(self, spider):
            self.file.close()
 
        def process_item(self, item, spider):
            line = json.dumps(ItemAdapter(item).asdict()) + "\n"
            self.file.write(line)
@@ -131,32 +136,35 @@
 ----------------------
 
 In this example we'll write items to MongoDB_ using pymongo_.
 MongoDB address and database name are specified in Scrapy settings;
 MongoDB collection is named after item class.
 
 The main point of this example is to show how to use :meth:`from_crawler`
-method and how to clean up the resources properly.::
+method and how to clean up the resources properly.
+
+.. skip: next
+.. code-block:: python
 
     import pymongo
     from itemadapter import ItemAdapter
 
-    class MongoPipeline:
 
-        collection_name = 'scrapy_items'
+    class MongoPipeline:
+        collection_name = "scrapy_items"
 
         def __init__(self, mongo_uri, mongo_db):
             self.mongo_uri = mongo_uri
             self.mongo_db = mongo_db
 
         @classmethod
         def from_crawler(cls, crawler):
             return cls(
-                mongo_uri=crawler.settings.get('MONGO_URI'),
-                mongo_db=crawler.settings.get('MONGO_DATABASE', 'items')
+                mongo_uri=crawler.settings.get("MONGO_URI"),
+                mongo_db=crawler.settings.get("MONGO_DATABASE", "items"),
             )
 
         def open_spider(self, spider):
             self.client = pymongo.MongoClient(self.mongo_uri)
             self.db = self.client[self.mongo_db]
 
         def close_spider(self, spider):
@@ -179,15 +187,15 @@
 the :meth:`process_item` method.
 
 This item pipeline makes a request to a locally-running instance of Splash_ to
 render a screenshot of the item URL. After the request response is downloaded,
 the item pipeline saves the screenshot to a file and adds the filename to the
 item.
 
-::
+.. code-block:: python
 
     import hashlib
     from pathlib import Path
     from urllib.parse import quote
 
     import scrapy
     from itemadapter import ItemAdapter
@@ -227,41 +235,44 @@
 .. _Splash: https://splash.readthedocs.io/en/stable/
 
 Duplicates filter
 -----------------
 
 A filter that looks for duplicate items, and drops those items that were
 already processed. Let's say that our items have a unique id, but our spider
-returns multiples items with the same id::
+returns multiples items with the same id:
 
+.. code-block:: python
 
     from itemadapter import ItemAdapter
     from scrapy.exceptions import DropItem
 
-    class DuplicatesPipeline:
 
+    class DuplicatesPipeline:
         def __init__(self):
             self.ids_seen = set()
 
         def process_item(self, item, spider):
             adapter = ItemAdapter(item)
-            if adapter['id'] in self.ids_seen:
+            if adapter["id"] in self.ids_seen:
                 raise DropItem(f"Duplicate item found: {item!r}")
             else:
-                self.ids_seen.add(adapter['id'])
+                self.ids_seen.add(adapter["id"])
                 return item
 
 
 Activating an Item Pipeline component
 =====================================
 
 To activate an Item Pipeline component you must add its class to the
-:setting:`ITEM_PIPELINES` setting, like in the following example::
+:setting:`ITEM_PIPELINES` setting, like in the following example:
+
+.. code-block:: python
 
    ITEM_PIPELINES = {
-       'myproject.pipelines.PricePipeline': 300,
-       'myproject.pipelines.JsonWriterPipeline': 800,
+       "myproject.pipelines.PricePipeline": 300,
+       "myproject.pipelines.JsonWriterPipeline": 800,
    }
 
 The integer values you assign to classes in this setting determine the
 order in which they run: items go through from lower valued to higher
 valued classes. It's customary to define these numbers in the 0-1000 range.
```

### Comparing `Scrapy-2.8.0/docs/topics/items.rst` & `Scrapy-2.9.0/docs/topics/items.rst`

 * *Files 16% similar despite different names*

```diff
@@ -72,18 +72,21 @@
     .. attribute:: fields
 
         A dictionary containing *all declared fields* for this Item, not only
         those populated. The keys are the field names and the values are the
         :class:`Field` objects used in the :ref:`Item declaration
         <topics-items-declaring>`.
 
-Example::
+Example:
+
+.. code-block:: python
 
     from scrapy.item import Item, Field
 
+
     class CustomItem(Item):
         one_field = Field()
         another_field = Field()
 
 .. _dataclass-items:
 
 Dataclass objects
@@ -98,18 +101,21 @@
 Additionally, ``dataclass`` items also allow to:
 
 * define the type and default value of each defined field.
 
 * define custom field metadata through :func:`dataclasses.field`, which can be used to
   :ref:`customize serialization <topics-exporters-field-serialization>`.
 
-Example::
+Example:
+
+.. code-block:: python
 
     from dataclasses import dataclass
 
+
     @dataclass
     class CustomItem:
         one_field: str
         another_field: int
 
 .. note:: Field types are not enforced at run time.
 
@@ -129,18 +135,21 @@
 * define the type and default value of each defined field.
 
 * define custom field :ref:`metadata <attrs:metadata>`, which can be used to
   :ref:`customize serialization <topics-exporters-field-serialization>`.
 
 In order to use this type, the :doc:`attrs package <attrs:index>` needs to be installed.
 
-Example::
+Example:
+
+.. code-block:: python
 
     import attr
 
+
     @attr.s
     class CustomItem:
         one_field = attr.ib()
         another_field = attr.ib()
 
 
 Working with Item objects
@@ -148,18 +157,21 @@
 
 .. _topics-items-declaring:
 
 Declaring Item subclasses
 -------------------------
 
 Item subclasses are declared using a simple class definition syntax and
-:class:`Field` objects. Here is an example::
+:class:`Field` objects. Here is an example:
+
+.. code-block:: python
 
     import scrapy
 
+
     class Product(scrapy.Item):
         name = scrapy.Field()
         price = scrapy.Field()
         stock = scrapy.Field()
         tags = scrapy.Field()
         last_updated = scrapy.Field(serializer=str)
 
@@ -218,82 +230,90 @@
 Here are some examples of common tasks performed with items, using the
 ``Product`` item :ref:`declared above  <topics-items-declaring>`. You will
 notice the API is very similar to the :class:`dict` API.
 
 Creating items
 ''''''''''''''
 
->>> product = Product(name='Desktop PC', price=1000)
->>> print(product)
-Product(name='Desktop PC', price=1000)
+.. code-block:: pycon
+
+    >>> product = Product(name="Desktop PC", price=1000)
+    >>> print(product)
+    Product(name='Desktop PC', price=1000)
 
 
 Getting field values
 ''''''''''''''''''''
 
->>> product['name']
-Desktop PC
->>> product.get('name')
-Desktop PC
+.. code-block:: pycon
+
+    >>> product["name"]
+    Desktop PC
+    >>> product.get("name")
+    Desktop PC
 
->>> product['price']
-1000
+    >>> product["price"]
+    1000
 
->>> product['last_updated']
-Traceback (most recent call last):
-    ...
-KeyError: 'last_updated'
+    >>> product["last_updated"]
+    Traceback (most recent call last):
+        ...
+    KeyError: 'last_updated'
 
->>> product.get('last_updated', 'not set')
-not set
+    >>> product.get("last_updated", "not set")
+    not set
 
->>> product['lala'] # getting unknown field
-Traceback (most recent call last):
-    ...
-KeyError: 'lala'
+    >>> product["lala"]  # getting unknown field
+    Traceback (most recent call last):
+        ...
+    KeyError: 'lala'
 
->>> product.get('lala', 'unknown field')
-'unknown field'
+    >>> product.get("lala", "unknown field")
+    'unknown field'
 
->>> 'name' in product  # is name field populated?
-True
+    >>> "name" in product  # is name field populated?
+    True
 
->>> 'last_updated' in product  # is last_updated populated?
-False
+    >>> "last_updated" in product  # is last_updated populated?
+    False
 
->>> 'last_updated' in product.fields  # is last_updated a declared field?
-True
+    >>> "last_updated" in product.fields  # is last_updated a declared field?
+    True
 
->>> 'lala' in product.fields  # is lala a declared field?
-False
+    >>> "lala" in product.fields  # is lala a declared field?
+    False
 
 
 Setting field values
 ''''''''''''''''''''
 
->>> product['last_updated'] = 'today'
->>> product['last_updated']
-today
-
->>> product['lala'] = 'test' # setting unknown field
-Traceback (most recent call last):
-    ...
-KeyError: 'Product does not support field: lala'
+.. code-block:: pycon
+
+    >>> product["last_updated"] = "today"
+    >>> product["last_updated"]
+    today
+
+    >>> product["lala"] = "test"  # setting unknown field
+    Traceback (most recent call last):
+        ...
+    KeyError: 'Product does not support field: lala'
 
 
 Accessing all populated values
 ''''''''''''''''''''''''''''''
 
 To access all populated values, just use the typical :class:`dict` API:
 
->>> product.keys()
-['price', 'name']
+.. code-block:: pycon
+
+    >>> product.keys()
+    ['price', 'name']
 
->>> product.items()
-[('price', 1000), ('name', 'Desktop PC')]
+    >>> product.items()
+    [('price', 1000), ('name', 'Desktop PC')]
 
 
 .. _copying-items:
 
 Copying items
 '''''''''''''
 
@@ -323,45 +343,51 @@
 
 
 Other common tasks
 ''''''''''''''''''
 
 Creating dicts from items:
 
->>> dict(product) # create a dict from all populated values
-{'price': 1000, 'name': 'Desktop PC'}
+.. code-block:: pycon
 
-Creating items from dicts:
+    >>> dict(product)  # create a dict from all populated values
+    {'price': 1000, 'name': 'Desktop PC'}
 
->>> Product({'name': 'Laptop PC', 'price': 1500})
-Product(price=1500, name='Laptop PC')
+    Creating items from dicts:
 
->>> Product({'name': 'Laptop PC', 'lala': 1500}) # warning: unknown field in dict
-Traceback (most recent call last):
-    ...
-KeyError: 'Product does not support field: lala'
+    >>> Product({"name": "Laptop PC", "price": 1500})
+    Product(price=1500, name='Laptop PC')
+
+    >>> Product({"name": "Laptop PC", "lala": 1500})  # warning: unknown field in dict
+    Traceback (most recent call last):
+        ...
+    KeyError: 'Product does not support field: lala'
 
 
 Extending Item subclasses
 -------------------------
 
 You can extend Items (to add more fields or to change some metadata for some
 fields) by declaring a subclass of your original Item.
 
-For example::
+For example:
+
+.. code-block:: python
 
     class DiscountedProduct(Product):
         discount_percent = scrapy.Field(serializer=str)
         discount_expiration_date = scrapy.Field()
 
 You can also extend field metadata by using the previous field metadata and
-appending more values, or changing existing values, like this::
+appending more values, or changing existing values, like this:
+
+.. code-block:: python
 
     class SpecificProduct(Product):
-        name = scrapy.Field(Product.fields['name'], serializer=my_serializer)
+        name = scrapy.Field(Product.fields["name"], serializer=my_serializer)
 
 That adds (or replaces) the ``serializer`` metadata key for the ``name`` field,
 keeping all the previously existing metadata values.
 
 
 .. _supporting-item-types:
```

### Comparing `Scrapy-2.8.0/docs/topics/jobs.rst` & `Scrapy-2.9.0/docs/topics/jobs.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,21 @@
 Sometimes you'll want to keep some persistent spider state between pause/resume
 batches. You can use the ``spider.state`` attribute for that, which should be a
 dict. There's a built-in extension that takes care of serializing, storing and
 loading that attribute from the job directory, when the spider starts and
 stops.
 
 Here's an example of a callback that uses the spider state (other spider code
-is omitted for brevity)::
+is omitted for brevity):
+
+.. code-block:: python
 
     def parse_item(self, response):
         # parse item here
-        self.state['items_count'] = self.state.get('items_count', 0) + 1
+        self.state["items_count"] = self.state.get("items_count", 0) + 1
 
 Persistence gotchas
 ===================
 
 There are a few things to keep in mind if you want to be able to use the Scrapy
 persistence support:
```

### Comparing `Scrapy-2.8.0/docs/topics/leaks.rst` & `Scrapy-2.9.0/docs/topics/leaks.rst`

 * *Files 4% similar despite different names*

```diff
@@ -66,21 +66,23 @@
 
 You can enter the telnet console and inspect how many objects (of the classes
 mentioned above) are currently alive using the ``prefs()`` function which is an
 alias to the :func:`~scrapy.utils.trackref.print_live_refs` function::
 
     telnet localhost 6023
 
-    >>> prefs()
-    Live References
+    .. code-block:: pycon
 
-    ExampleSpider                       1   oldest: 15s ago
-    HtmlResponse                       10   oldest: 1s ago
-    Selector                            2   oldest: 0s ago
-    FormRequest                       878   oldest: 7s ago
+        >>> prefs()
+        Live References
+
+        ExampleSpider                       1   oldest: 15s ago
+        HtmlResponse                       10   oldest: 1s ago
+        Selector                            2   oldest: 0s ago
+        FormRequest                       878   oldest: 7s ago
 
 As you can see, that report also shows the "age" of the oldest object in each
 class. If you're running multiple spiders per process chances are you can
 figure out which spider is leaking by looking at the oldest request or response.
 You can get the oldest object of each class using the
 :func:`~scrapy.utils.trackref.get_oldest` function (from the telnet console).
 
@@ -110,15 +112,17 @@
 cause memory leaks.
 
 Let's see how we can discover the cause (without knowing it
 a priori, of course) by using the ``trackref`` tool.
 
 After the crawler is running for a few minutes and we notice its memory usage
 has grown a lot, we can enter its telnet console and check the live
-references::
+references:
+
+.. code-block:: pycon
 
     >>> prefs()
     Live References
 
     SomenastySpider                     1   oldest: 15s ago
     HtmlResponse                     3890   oldest: 265s ago
     Selector                            2   oldest: 0s ago
@@ -130,39 +134,45 @@
 of requests, so it looks like they are tied in a some way. We can now go
 and check the code of the spider to discover the nasty line that is
 generating the leaks (passing response references inside requests).
 
 Sometimes extra information about live objects can be helpful.
 Let's check the oldest response:
 
->>> from scrapy.utils.trackref import get_oldest
->>> r = get_oldest('HtmlResponse')
->>> r.url
-'http://www.somenastyspider.com/product.php?pid=123'
+.. code-block:: pycon
+
+    >>> from scrapy.utils.trackref import get_oldest
+    >>> r = get_oldest("HtmlResponse")
+    >>> r.url
+    'http://www.somenastyspider.com/product.php?pid=123'
 
 If you want to iterate over all objects, instead of getting the oldest one, you
 can use the :func:`scrapy.utils.trackref.iter_all` function:
 
->>> from scrapy.utils.trackref import iter_all
->>> [r.url for r in iter_all('HtmlResponse')]
-['http://www.somenastyspider.com/product.php?pid=123',
- 'http://www.somenastyspider.com/product.php?pid=584',
-...]
+.. code-block:: pycon
+
+    >>> from scrapy.utils.trackref import iter_all
+    >>> [r.url for r in iter_all("HtmlResponse")]
+    ['http://www.somenastyspider.com/product.php?pid=123',
+    'http://www.somenastyspider.com/product.php?pid=584',
+    ...]
 
 Too many spiders?
 -----------------
 
 If your project has too many spiders executed in parallel,
 the output of :func:`prefs()` can be difficult to read.
 For this reason, that function has a ``ignore`` argument which can be used to
 ignore a particular class (and all its subclasses). For
 example, this won't show any live references to spiders:
 
->>> from scrapy.spiders import Spider
->>> prefs(ignore=Spider)
+.. code-block:: pycon
+
+    >>> from scrapy.spiders import Spider
+    >>> prefs(ignore=Spider)
 
 .. module:: scrapy.utils.trackref
    :synopsis: Track references of live objects
 
 scrapy.utils.trackref module
 ----------------------------
 
@@ -212,38 +222,40 @@
 If you use ``pip``, you can install muppy with the following command::
 
     pip install Pympler
 
 Here's an example to view all Python objects available in
 the heap using muppy:
 
->>> from pympler import muppy
->>> all_objects = muppy.get_objects()
->>> len(all_objects)
-28667
->>> from pympler import summary
->>> suml = summary.summarize(all_objects)
->>> summary.print_(suml)
-                               types |   # objects |   total size
-==================================== | =========== | ============
-                         <class 'str |        9822 |      1.10 MB
-                        <class 'dict |        1658 |    856.62 KB
-                        <class 'type |         436 |    443.60 KB
-                        <class 'code |        2974 |    419.56 KB
-          <class '_io.BufferedWriter |           2 |    256.34 KB
-                         <class 'set |         420 |    159.88 KB
-          <class '_io.BufferedReader |           1 |    128.17 KB
-          <class 'wrapper_descriptor |        1130 |     88.28 KB
-                       <class 'tuple |        1304 |     86.57 KB
-                     <class 'weakref |        1013 |     79.14 KB
-  <class 'builtin_function_or_method |         958 |     67.36 KB
-           <class 'method_descriptor |         865 |     60.82 KB
-                 <class 'abc.ABCMeta |          62 |     59.96 KB
-                        <class 'list |         446 |     58.52 KB
-                         <class 'int |        1425 |     43.20 KB
+.. code-block:: pycon
+
+    >>> from pympler import muppy
+    >>> all_objects = muppy.get_objects()
+    >>> len(all_objects)
+    28667
+    >>> from pympler import summary
+    >>> suml = summary.summarize(all_objects)
+    >>> summary.print_(suml)
+                                   types |   # objects |   total size
+    ==================================== | =========== | ============
+                             <class 'str |        9822 |      1.10 MB
+                            <class 'dict |        1658 |    856.62 KB
+                            <class 'type |         436 |    443.60 KB
+                            <class 'code |        2974 |    419.56 KB
+              <class '_io.BufferedWriter |           2 |    256.34 KB
+                             <class 'set |         420 |    159.88 KB
+              <class '_io.BufferedReader |           1 |    128.17 KB
+              <class 'wrapper_descriptor |        1130 |     88.28 KB
+                           <class 'tuple |        1304 |     86.57 KB
+                         <class 'weakref |        1013 |     79.14 KB
+      <class 'builtin_function_or_method |         958 |     67.36 KB
+               <class 'method_descriptor |         865 |     60.82 KB
+                     <class 'abc.ABCMeta |          62 |     59.96 KB
+                            <class 'list |         446 |     58.52 KB
+                             <class 'int |        1425 |     43.20 KB
 
 For more info about muppy, refer to the `muppy documentation`_.
 
 .. _muppy documentation: https://pythonhosted.org/Pympler/muppy.html
 
 .. _topics-leaks-without-leaks:
```

### Comparing `Scrapy-2.8.0/docs/topics/link-extractors.rst` & `Scrapy-2.9.0/docs/topics/link-extractors.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 :class:`~scrapy.http.Response` object.
 
 Link extractors are used in :class:`~scrapy.spiders.CrawlSpider` spiders
 through a set of :class:`~scrapy.spiders.Rule` objects.
 
 You can also use link extractors in regular spiders. For example, you can instantiate
 :class:`LinkExtractor <scrapy.linkextractors.lxmlhtml.LxmlLinkExtractor>` into a class
-variable in your spider, and use it from your spider callbacks::
+variable in your spider, and use it from your spider callbacks:
+
+.. code-block:: python
 
     def parse(self, response):
         for link in self.link_extractor.extract_links(response):
             yield Request(link.url, callback=self.parse)
 
 .. _topics-link-extractors-ref:
 
@@ -128,18 +130,20 @@
 
         For example, to extract links from this code::
 
             <a href="javascript:goToPage('../other/page.html'); return false">Link text</a>
 
         .. highlight:: python
 
-        You can use the following function in ``process_value``::
+        You can use the following function in ``process_value``:
+
+        .. code-block:: python
 
             def process_value(value):
-                m = re.search("javascript:goToPage\('(.*?)'", value)
+                m = re.search(r"javascript:goToPage\('(.*?)'", value)
                 if m:
                     return m.group(1)
 
     :type process_value: collections.abc.Callable
 
     :param strip: whether to strip whitespaces from extracted attributes.
         According to HTML5 standard, leading and trailing whitespaces
```

### Comparing `Scrapy-2.8.0/docs/topics/loaders.rst` & `Scrapy-2.9.0/docs/topics/loaders.rst`

 * *Files 4% similar despite different names*

```diff
@@ -42,26 +42,29 @@
    allowing to add several values to the same field.
    If an ``item`` argument is passed when creating a loader,
    each of the item's values will be stored as-is if it's already
    an iterable, or wrapped with a list if it's a single value.
 
 Here is a typical Item Loader usage in a :ref:`Spider <topics-spiders>`, using
 the :ref:`Product item <topics-items-declaring>` declared in the :ref:`Items
-chapter <topics-items>`::
+chapter <topics-items>`:
+
+.. code-block:: python
 
     from scrapy.loader import ItemLoader
     from myproject.items import Product
 
+
     def parse(self, response):
         l = ItemLoader(item=Product(), response=response)
-        l.add_xpath('name', '//div[@class="product_name"]')
-        l.add_xpath('name', '//div[@class="product_title"]')
-        l.add_xpath('price', '//p[@id="price"]')
-        l.add_css('stock', 'p#stock')
-        l.add_value('last_updated', 'today') # you can also use literal values
+        l.add_xpath("name", '//div[@class="product_name"]')
+        l.add_xpath("name", '//div[@class="product_title"]')
+        l.add_xpath("price", '//p[@id="price"]')
+        l.add_css("stock", "p#stock")
+        l.add_value("last_updated", "today")  # you can also use literal values
         return l.load_item()
 
 By quickly looking at that code, we can see the ``name`` field is being
 extracted from two different XPath locations in the page:
 
 1. ``//div[@class="product_name"]``
 2. ``//div[@class="product_title"]``
@@ -89,19 +92,22 @@
 By default, :ref:`dataclass items <dataclass-items>` require all fields to be
 passed when created. This could be an issue when using dataclass items with
 item loaders: unless a pre-populated item is passed to the loader, fields
 will be populated incrementally using the loader's :meth:`~ItemLoader.add_xpath`,
 :meth:`~ItemLoader.add_css` and :meth:`~ItemLoader.add_value` methods.
 
 One approach to overcome this is to define items using the
-:func:`~dataclasses.field` function, with a ``default`` argument::
+:func:`~dataclasses.field` function, with a ``default`` argument:
+
+.. code-block:: python
 
     from dataclasses import dataclass, field
     from typing import Optional
 
+
     @dataclass
     class InventoryItem:
         name: Optional[str] = field(default=None)
         price: Optional[float] = field(default=None)
         stock: Optional[int] = field(default=None)
 
 
@@ -118,22 +124,24 @@
 :meth:`ItemLoader.load_item` method is called to populate and get the populated
 :ref:`item object <topics-items>`.  That's when the output processor is
 called with the data previously collected (and processed using the input
 processor). The result of the output processor is the final value that gets
 assigned to the item.
 
 Let's see an example to illustrate how the input and output processors are
-called for a particular field (the same applies for any other field)::
+called for a particular field (the same applies for any other field):
+
+.. code-block:: python
 
     l = ItemLoader(Product(), some_selector)
-    l.add_xpath('name', xpath1) # (1)
-    l.add_xpath('name', xpath2) # (2)
-    l.add_css('name', css) # (3)
-    l.add_value('name', 'test') # (4)
-    return l.load_item() # (5)
+    l.add_xpath("name", xpath1)  # (1)
+    l.add_xpath("name", xpath2)  # (2)
+    l.add_css("name", css)  # (3)
+    l.add_value("name", "test")  # (4)
+    return l.load_item()  # (5)
 
 So what happens is:
 
 1. Data from ``xpath1`` is extracted, and passed through the *input processor* of
    the ``name`` field. The result of the input processor is collected and kept in
    the Item Loader (but not yet assigned to the item).
 
@@ -180,21 +188,23 @@
 Last, but not least, itemloaders_ comes with some :ref:`commonly used
 processors <itemloaders:built-in-processors>` built-in for convenience.
 
 
 Declaring Item Loaders
 ======================
 
-Item Loaders are declared using a class definition syntax. Here is an example::
+Item Loaders are declared using a class definition syntax. Here is an example:
+
+.. code-block:: python
 
     from itemloaders.processors import TakeFirst, MapCompose, Join
     from scrapy.loader import ItemLoader
 
-    class ProductLoader(ItemLoader):
 
+    class ProductLoader(ItemLoader):
         default_output_processor = TakeFirst()
 
         name_in = MapCompose(str.title)
         name_out = Join()
 
         price_in = MapCompose(str.strip)
 
@@ -211,40 +221,47 @@
 Declaring Input and Output Processors
 =====================================
 
 As seen in the previous section, input and output processors can be declared in
 the Item Loader definition, and it's very common to declare input processors
 this way. However, there is one more place where you can specify the input and
 output processors to use: in the :ref:`Item Field <topics-items-fields>`
-metadata. Here is an example::
+metadata. Here is an example:
+
+.. code-block:: python
 
     import scrapy
     from itemloaders.processors import Join, MapCompose, TakeFirst
     from w3lib.html import remove_tags
 
+
     def filter_price(value):
         if value.isdigit():
             return value
 
+
     class Product(scrapy.Item):
         name = scrapy.Field(
             input_processor=MapCompose(remove_tags),
             output_processor=Join(),
         )
         price = scrapy.Field(
             input_processor=MapCompose(remove_tags, filter_price),
             output_processor=TakeFirst(),
         )
 
->>> from scrapy.loader import ItemLoader
->>> il = ItemLoader(item=Product())
->>> il.add_value('name', ['Welcome to my', '<strong>website</strong>'])
->>> il.add_value('price', ['&euro;', '<span>1000</span>'])
->>> il.load_item()
-{'name': 'Welcome to my website', 'price': '1000'}
+
+.. code-block:: pycon
+
+    >>> from scrapy.loader import ItemLoader
+    >>> il = ItemLoader(item=Product())
+    >>> il.add_value("name", ["Welcome to my", "<strong>website</strong>"])
+    >>> il.add_value("price", ["&euro;", "<span>1000</span>"])
+    >>> il.load_item()
+    {'name': 'Welcome to my website', 'price': '1000'}
 
 The precedence order, for both input and output processors, is as follows:
 
 1. Item Loader field-specific attributes: ``field_in`` and ``field_out`` (most
    precedence)
 2. Field metadata (``input_processor`` and ``output_processor`` key)
 3. Item Loader defaults: :meth:`ItemLoader.default_input_processor` and
@@ -259,45 +276,53 @@
 
 The Item Loader Context is a dict of arbitrary key/values which is shared among
 all input and output processors in the Item Loader. It can be passed when
 declaring, instantiating or using Item Loader. They are used to modify the
 behaviour of the input/output processors.
 
 For example, suppose you have a function ``parse_length`` which receives a text
-value and extracts a length from it::
+value and extracts a length from it:
+
+.. code-block:: python
 
     def parse_length(text, loader_context):
-        unit = loader_context.get('unit', 'm')
+        unit = loader_context.get("unit", "m")
         # ... length parsing code goes here ...
         return parsed_length
 
 By accepting a ``loader_context`` argument the function is explicitly telling
 the Item Loader that it's able to receive an Item Loader context, so the Item
 Loader passes the currently active context when calling it, and the processor
 function (``parse_length`` in this case) can thus use them.
 
 There are several ways to modify Item Loader context values:
 
 1. By modifying the currently active Item Loader context
-   (:attr:`~ItemLoader.context` attribute)::
+   (:attr:`~ItemLoader.context` attribute):
+
+   .. code-block:: python
 
       loader = ItemLoader(product)
-      loader.context['unit'] = 'cm'
+      loader.context["unit"] = "cm"
 
 2. On Item Loader instantiation (the keyword arguments of Item Loader
-   ``__init__`` method are stored in the Item Loader context)::
+   ``__init__`` method are stored in the Item Loader context):
 
-      loader = ItemLoader(product, unit='cm')
+   .. code-block:: python
+
+      loader = ItemLoader(product, unit="cm")
 
 3. On Item Loader declaration, for those input/output processors that support
    instantiating them with an Item Loader context. :class:`~processor.MapCompose` is one of
-   them::
+   them:
+
+   .. code-block:: python
 
        class ProductLoader(ItemLoader):
-           length_out = MapCompose(parse_length, unit='cm')
+           length_out = MapCompose(parse_length, unit="cm")
 
 
 ItemLoader objects
 ==================
 
 .. autoclass:: scrapy.loader.ItemLoader
     :members:
@@ -319,33 +344,37 @@
         <a class="social" href="https://twitter.com/whatever">Follow Us</a>
         <a class="email" href="mailto:whatever@example.com">Email Us</a>
     </footer>
 
 Without nested loaders, you need to specify the full xpath (or css) for each value
 that you wish to extract.
 
-Example::
+Example:
+
+.. code-block:: python
 
     loader = ItemLoader(item=Item())
     # load stuff not in the footer
-    loader.add_xpath('social', '//footer/a[@class = "social"]/@href')
-    loader.add_xpath('email', '//footer/a[@class = "email"]/@href')
+    loader.add_xpath("social", '//footer/a[@class = "social"]/@href')
+    loader.add_xpath("email", '//footer/a[@class = "email"]/@href')
     loader.load_item()
 
 Instead, you can create a nested loader with the footer selector and add values
 relative to the footer.  The functionality is the same but you avoid repeating
 the footer selector.
 
-Example::
+Example:
+
+.. code-block:: python
 
     loader = ItemLoader(item=Item())
     # load stuff not in the footer
-    footer_loader = loader.nested_xpath('//footer')
-    footer_loader.add_xpath('social', 'a[@class = "social"]/@href')
-    footer_loader.add_xpath('email', 'a[@class = "email"]/@href')
+    footer_loader = loader.nested_xpath("//footer")
+    footer_loader.add_xpath("social", 'a[@class = "social"]/@href')
+    footer_loader.add_xpath("email", 'a[@class = "email"]/@href')
     # no need to call footer_loader.load_item()
     loader.load_item()
 
 You can nest loaders arbitrarily and they work with either xpath or css selectors.
 As a general guideline, use nested loaders when they make your code simpler but do
 not go overboard with nesting or your parser can become difficult to read.
 
@@ -366,33 +395,40 @@
 specific spiders (or groups of spiders).
 
 Suppose, for example, that some particular site encloses their product names in
 three dashes (e.g. ``---Plasma TV---``) and you don't want to end up scraping
 those dashes in the final product names.
 
 Here's how you can remove those dashes by reusing and extending the default
-Product Item Loader (``ProductLoader``)::
+Product Item Loader (``ProductLoader``):
+
+.. code-block:: python
 
     from itemloaders.processors import MapCompose
     from myproject.ItemLoaders import ProductLoader
 
+
     def strip_dashes(x):
-        return x.strip('-')
+        return x.strip("-")
+
 
     class SiteSpecificLoader(ProductLoader):
         name_in = MapCompose(strip_dashes, ProductLoader.name_in)
 
 Another case where extending Item Loaders can be very helpful is when you have
 multiple source formats, for example XML and HTML. In the XML version you may
-want to remove ``CDATA`` occurrences. Here's an example of how to do it::
+want to remove ``CDATA`` occurrences. Here's an example of how to do it:
+
+.. code-block:: python
 
     from itemloaders.processors import MapCompose
     from myproject.ItemLoaders import ProductLoader
     from myproject.utils.xml import remove_cdata
 
+
     class XmlProductLoader(ProductLoader):
         name_in = MapCompose(remove_cdata, ProductLoader.name_in)
 
 And that's how you typically extend input processors.
 
 As for output processors, it is more common to declare them in the field metadata,
 as they usually depend only on the field and not on each specific site parsing
```

### Comparing `Scrapy-2.8.0/docs/topics/logging.rst` & `Scrapy-2.9.0/docs/topics/logging.rst`

 * *Files 6% similar despite different names*

```diff
@@ -35,52 +35,67 @@
 4. ``logging.INFO`` - for informational messages
 5. ``logging.DEBUG`` - for debugging messages (lowest severity)
 
 How to log messages
 ===================
 
 Here's a quick example of how to log a message using the ``logging.WARNING``
-level::
+level:
+
+.. code-block:: python
 
     import logging
+
     logging.warning("This is a warning")
 
 There are shortcuts for issuing log messages on any of the standard 5 levels,
 and there's also a general ``logging.log`` method which takes a given level as
-argument.  If needed, the last example could be rewritten as::
+argument.  If needed, the last example could be rewritten as:
+
+.. code-block:: python
 
     import logging
+
     logging.log(logging.WARNING, "This is a warning")
 
 On top of that, you can create different "loggers" to encapsulate messages. (For
 example, a common practice is to create different loggers for every module).
 These loggers can be configured independently, and they allow hierarchical
 constructions.
 
 The previous examples use the root logger behind the scenes, which is a top level
 logger where all messages are propagated to (unless otherwise specified). Using
 ``logging`` helpers is merely a shortcut for getting the root logger
-explicitly, so this is also an equivalent of the last snippets::
+explicitly, so this is also an equivalent of the last snippets:
+
+.. code-block:: python
 
     import logging
+
     logger = logging.getLogger()
     logger.warning("This is a warning")
 
 You can use a different logger just by getting its name with the
-``logging.getLogger`` function::
+``logging.getLogger`` function:
+
+.. code-block:: python
 
     import logging
-    logger = logging.getLogger('mycustomlogger')
+
+    logger = logging.getLogger("mycustomlogger")
     logger.warning("This is a warning")
 
 Finally, you can ensure having a custom logger for any module you're working on
 by using the ``__name__`` variable, which is populated with current module's
-path::
+path:
+
+.. code-block:: python
 
     import logging
+
     logger = logging.getLogger(__name__)
     logger.warning("This is a warning")
 
 .. seealso::
 
     Module logging, :doc:`HowTo <howto/logging>`
         Basic Logging Tutorial
@@ -90,41 +105,45 @@
 
 .. _topics-logging-from-spiders:
 
 Logging from Spiders
 ====================
 
 Scrapy provides a :data:`~scrapy.Spider.logger` within each Spider
-instance, which can be accessed and used like this::
+instance, which can be accessed and used like this:
+
+.. code-block:: python
 
     import scrapy
 
-    class MySpider(scrapy.Spider):
 
-        name = 'myspider'
-        start_urls = ['https://scrapy.org']
+    class MySpider(scrapy.Spider):
+        name = "myspider"
+        start_urls = ["https://scrapy.org"]
 
         def parse(self, response):
-            self.logger.info('Parse function called on %s', response.url)
+            self.logger.info("Parse function called on %s", response.url)
 
 That logger is created using the Spider's name, but you can use any custom
-Python logger you want. For example::
+Python logger you want. For example:
+
+.. code-block:: python
 
     import logging
     import scrapy
 
-    logger = logging.getLogger('mycustomlogger')
+    logger = logging.getLogger("mycustomlogger")
 
-    class MySpider(scrapy.Spider):
 
-        name = 'myspider'
-        start_urls = ['https://scrapy.org']
+    class MySpider(scrapy.Spider):
+        name = "myspider"
+        start_urls = ["https://scrapy.org"]
 
         def parse(self, response):
-            logger.info('Parse function called on %s', response.url)
+            logger.info("Parse function called on %s", response.url)
 
 .. _topics-logging-configuration:
 
 Logging configuration
 =====================
 
 Loggers on their own don't manage how messages sent through them are displayed.
@@ -225,71 +244,83 @@
 ``[scrapy.spidermiddlewares.httperror]``. If you get just ``[scrapy]`` then
 :setting:`LOG_SHORT_NAMES` is likely set to True; set it to False and re-run
 the crawl.
 
 Next, we can see that the message has INFO level. To hide it
 we should set logging level for ``scrapy.spidermiddlewares.httperror``
 higher than INFO; next level after INFO is WARNING. It could be done
-e.g. in the spider's ``__init__`` method::
+e.g. in the spider's ``__init__`` method:
+
+.. code-block:: python
 
     import logging
     import scrapy
 
 
     class MySpider(scrapy.Spider):
         # ...
         def __init__(self, *args, **kwargs):
-            logger = logging.getLogger('scrapy.spidermiddlewares.httperror')
+            logger = logging.getLogger("scrapy.spidermiddlewares.httperror")
             logger.setLevel(logging.WARNING)
             super().__init__(*args, **kwargs)
 
 If you run this spider again then INFO messages from
 ``scrapy.spidermiddlewares.httperror`` logger will be gone.
 
 You can also filter log records by :class:`~logging.LogRecord` data. For 
 example, you can filter log records by message content using a substring or
 a regular expression. Create a :class:`logging.Filter` subclass 
 and equip it with a regular expression pattern to
-filter out unwanted messages::
+filter out unwanted messages:
+
+.. code-block:: python
 
     import logging
     import re
-    
+
+
     class ContentFilter(logging.Filter):
         def filter(self, record):
-            match = re.search(r'\d{3} [Ee]rror, retrying', record.message)
+            match = re.search(r"\d{3} [Ee]rror, retrying", record.message)
             if match:
                 return False
-                
+
 A project-level filter may be attached to the root 
 handler created by Scrapy, this is a wieldy way to 
 filter all loggers in different parts of the project
-(middlewares, spider, etc.)::
+(middlewares, spider, etc.):
 
-    import logging
-    import scrapy
+.. code-block:: python
+
+ import logging
+ import scrapy
+
+
+ class MySpider(scrapy.Spider):
+     # ...
+     def __init__(self, *args, **kwargs):
+         for handler in logging.root.handlers:
+             handler.addFilter(ContentFilter())
 
-    class MySpider(scrapy.Spider):
-        # ...
-        def __init__(self, *args, **kwargs):
-            for handler in logging.root.handlers:
-                handler.addFilter(ContentFilter())
- 
 Alternatively, you may choose a specific logger 
-and hide it without affecting other loggers::
+and hide it without affecting other loggers:
+
+.. code-block:: python
 
     import logging
     import scrapy
-    
+
+
     class MySpider(scrapy.Spider):
         # ...
         def __init__(self, *args, **kwargs):
-            logger = logging.getLogger('my_logger')
+            logger = logging.getLogger("my_logger")
             logger.addFilter(ContentFilter())
-            
+
+
 scrapy.utils.log module
 =======================
 
 .. module:: scrapy.utils.log
    :synopsis: Logging utils
 
 .. autofunction:: configure_logging
@@ -302,19 +333,19 @@
     Another option when running custom scripts is to manually configure the logging.
     To do this you can use :func:`logging.basicConfig` to set a basic root handler.
 
     Note that :class:`~scrapy.crawler.CrawlerProcess` automatically calls ``configure_logging``,
     so it is recommended to only use :func:`logging.basicConfig` together with
     :class:`~scrapy.crawler.CrawlerRunner`.
 
-    This is an example on how to redirect ``INFO`` or higher messages to a file::
+    This is an example on how to redirect ``INFO`` or higher messages to a file:
+
+    .. code-block:: python
 
         import logging
 
         logging.basicConfig(
-            filename='log.txt',
-            format='%(levelname)s: %(message)s',
-            level=logging.INFO
+            filename="log.txt", format="%(levelname)s: %(message)s", level=logging.INFO
         )
 
     Refer to :ref:`run-from-script` for more details about using Scrapy this
     way.
```

### Comparing `Scrapy-2.8.0/docs/topics/media-pipeline.rst` & `Scrapy-2.9.0/docs/topics/media-pipeline.rst`

 * *Files 11% similar despite different names*

```diff
@@ -83,37 +83,45 @@
 
 .. setting:: IMAGES_STORE
 .. setting:: FILES_STORE
 
 To enable your media pipeline you must first add it to your project
 :setting:`ITEM_PIPELINES` setting.
 
-For Images Pipeline, use::
+For Images Pipeline, use:
 
-    ITEM_PIPELINES = {'scrapy.pipelines.images.ImagesPipeline': 1}
+.. code-block:: python
+
+    ITEM_PIPELINES = {"scrapy.pipelines.images.ImagesPipeline": 1}
 
-For Files Pipeline, use::
+For Files Pipeline, use:
+
+.. code-block:: python
 
-    ITEM_PIPELINES = {'scrapy.pipelines.files.FilesPipeline': 1}
+    ITEM_PIPELINES = {"scrapy.pipelines.files.FilesPipeline": 1}
 
 .. note::
     You can also use both the Files and Images Pipeline at the same time.
 
 
 Then, configure the target storage setting to a valid value that will be used
 for storing the downloaded images. Otherwise the pipeline will remain disabled,
 even if you include it in the :setting:`ITEM_PIPELINES` setting.
 
-For the Files Pipeline, set the :setting:`FILES_STORE` setting::
+For the Files Pipeline, set the :setting:`FILES_STORE` setting:
+
+.. code-block:: python
+
+   FILES_STORE = "/path/to/valid/dir"
 
-   FILES_STORE = '/path/to/valid/dir'
+For the Images Pipeline, set the :setting:`IMAGES_STORE` setting:
 
-For the Images Pipeline, set the :setting:`IMAGES_STORE` setting::
+.. code-block:: python
 
-   IMAGES_STORE = '/path/to/valid/dir'
+   IMAGES_STORE = "/path/to/valid/dir"
 
 .. _topics-file-naming:
 
 File Naming
 ===========
 
 Default File Naming
@@ -153,18 +161,19 @@
 
 By overriding ``file_path`` like this:
 
 .. code-block:: python
 
   import hashlib
 
+
   def file_path(self, request, response=None, info=None, *, item=None):
       image_url_hash = hashlib.shake_256(request.url.encode()).hexdigest(5)
-      image_perspective = request.url.split('/')[-2]
-      image_filename = f'{image_url_hash}_{image_perspective}.jpg'
+      image_perspective = request.url.split("/")[-2]
+      image_filename = f"{image_url_hash}_{image_perspective}.jpg"
 
       return image_filename
 
 .. warning::
   If your custom file name scheme relies on meta data that can vary between
   scrapes it may lead to unexpected re-downloading of existing media using
   new file names.
@@ -229,38 +238,46 @@
 .. setting:: FILES_STORE_S3_ACL
 .. setting:: IMAGES_STORE_S3_ACL
 
 If botocore_ >= 1.4.87 is installed, :setting:`FILES_STORE` and
 :setting:`IMAGES_STORE` can represent an Amazon S3 bucket. Scrapy will
 automatically upload the files to the bucket.
 
-For example, this is a valid :setting:`IMAGES_STORE` value::
+For example, this is a valid :setting:`IMAGES_STORE` value:
+
+.. code-block:: python
 
-    IMAGES_STORE = 's3://bucket/images'
+    IMAGES_STORE = "s3://bucket/images"
 
 You can modify the Access Control List (ACL) policy used for the stored files,
 which is defined by the :setting:`FILES_STORE_S3_ACL` and
 :setting:`IMAGES_STORE_S3_ACL` settings. By default, the ACL is set to
 ``private``. To make the files publicly available use the ``public-read``
-policy::
+policy:
 
-    IMAGES_STORE_S3_ACL = 'public-read'
+.. code-block:: python
+
+    IMAGES_STORE_S3_ACL = "public-read"
 
 For more information, see `canned ACLs`_ in the Amazon S3 Developer Guide.
 
 You can also use other S3-like storages. Storages like self-hosted `Minio`_ or
 `s3.scality`_. All you need to do is set endpoint option in you Scrapy
-settings::
+settings:
 
-    AWS_ENDPOINT_URL = 'http://minio.example.com:9000'
+.. code-block:: python
 
-For self-hosting you also might feel the need not to use SSL and not to verify SSL connection::
+    AWS_ENDPOINT_URL = "http://minio.example.com:9000"
 
-    AWS_USE_SSL = False # or True (None by default)
-    AWS_VERIFY = False # or True (None by default)
+For self-hosting you also might feel the need not to use SSL and not to verify SSL connection:
+
+.. code-block:: python
+
+    AWS_USE_SSL = False  # or True (None by default)
+    AWS_VERIFY = False  # or True (None by default)
 
 .. _botocore: https://github.com/boto/botocore
 .. _canned ACLs: https://docs.aws.amazon.com/AmazonS3/latest/dev/acl-overview.html#canned-acl
 .. _Minio: https://github.com/minio/minio
 .. _s3.scality: https://s3.scality.com/
 
 
@@ -273,31 +290,35 @@
 .. setting:: IMAGES_STORE_GCS_ACL
 
 :setting:`FILES_STORE` and :setting:`IMAGES_STORE` can represent a Google Cloud Storage
 bucket. Scrapy will automatically upload the files to the bucket. (requires `google-cloud-storage`_ )
 
 .. _google-cloud-storage: https://cloud.google.com/storage/docs/reference/libraries#client-libraries-install-python
 
-For example, these are valid :setting:`IMAGES_STORE` and :setting:`GCS_PROJECT_ID` settings::
+For example, these are valid :setting:`IMAGES_STORE` and :setting:`GCS_PROJECT_ID` settings:
 
-    IMAGES_STORE = 'gs://bucket/images/'
-    GCS_PROJECT_ID = 'project_id'
+.. code-block:: python
+
+    IMAGES_STORE = "gs://bucket/images/"
+    GCS_PROJECT_ID = "project_id"
 
 For information about authentication, see this `documentation`_.
 
 .. _documentation: https://cloud.google.com/docs/authentication/production
 
 You can modify the Access Control List (ACL) policy used for the stored files,
 which is defined by the :setting:`FILES_STORE_GCS_ACL` and
 :setting:`IMAGES_STORE_GCS_ACL` settings. By default, the ACL is set to
 ``''`` (empty string) which means that Cloud Storage applies the bucket's default object ACL to the object.
 To make the files publicly available use the ``publicRead``
-policy::
+policy:
+
+.. code-block:: python
 
-    IMAGES_STORE_GCS_ACL = 'publicRead'
+    IMAGES_STORE_GCS_ACL = "publicRead"
 
 For more information, see `Predefined ACLs`_ in the Google Cloud Platform Developer Guide.
 
 .. _Predefined ACLs: https://cloud.google.com/storage/docs/access-control/lists#predefined-acl
 
 Usage example
 =============
@@ -314,37 +335,44 @@
 field (``file_urls`` or ``image_urls``, for the Files or Images Pipeline
 respectively), the pipeline will put the results under the respective field
 (``files`` or ``images``).
 
 When using :ref:`item types <item-types>` for which fields are defined beforehand,
 you must define both the URLs field and the results field. For example, when
 using the images pipeline, items must define both the ``image_urls`` and the
-``images`` field. For instance, using the :class:`~scrapy.Item` class::
+``images`` field. For instance, using the :class:`~scrapy.Item` class:
+
+.. code-block:: python
 
     import scrapy
 
+
     class MyItem(scrapy.Item):
         # ... other item fields ...
         image_urls = scrapy.Field()
         images = scrapy.Field()
 
 If you want to use another field name for the URLs key or for the results key,
 it is also possible to override it.
 
 For the Files Pipeline, set :setting:`FILES_URLS_FIELD` and/or
-:setting:`FILES_RESULT_FIELD` settings::
+:setting:`FILES_RESULT_FIELD` settings:
 
-    FILES_URLS_FIELD = 'field_name_for_your_files_urls'
-    FILES_RESULT_FIELD = 'field_name_for_your_processed_files'
+.. code-block:: python
+
+    FILES_URLS_FIELD = "field_name_for_your_files_urls"
+    FILES_RESULT_FIELD = "field_name_for_your_processed_files"
 
 For the Images Pipeline, set :setting:`IMAGES_URLS_FIELD` and/or
-:setting:`IMAGES_RESULT_FIELD` settings::
+:setting:`IMAGES_RESULT_FIELD` settings:
 
-    IMAGES_URLS_FIELD = 'field_name_for_your_images_urls'
-    IMAGES_RESULT_FIELD = 'field_name_for_your_processed_images'
+.. code-block:: python
+
+    IMAGES_URLS_FIELD = "field_name_for_your_images_urls"
+    IMAGES_RESULT_FIELD = "field_name_for_your_processed_images"
 
 If you need something more complex and want to override the custom pipeline
 behaviour, see :ref:`topics-media-pipeline-override`.
 
 If you have multiple image pipelines inheriting from ImagePipeline and you want
 to have different settings in different pipelines you can set setting keys
 preceded with uppercase name of your pipeline class. E.g. if your pipeline is
@@ -362,15 +390,17 @@
 
 .. setting:: IMAGES_EXPIRES
 .. setting:: FILES_EXPIRES
 
 The Image Pipeline avoids downloading files that were downloaded recently. To
 adjust this retention delay use the :setting:`FILES_EXPIRES` setting (or
 :setting:`IMAGES_EXPIRES`, in case of Images Pipeline), which
-specifies the delay in number of days::
+specifies the delay in number of days:
+
+.. code-block:: python
 
     # 120 days of delay for files expiration
     FILES_EXPIRES = 120
 
     # 30 days of delay for images expiration
     IMAGES_EXPIRES = 30
 
@@ -396,19 +426,21 @@
 images.
 
 .. setting:: IMAGES_THUMBS
 
 In order to use this feature, you must set :setting:`IMAGES_THUMBS` to a dictionary
 where the keys are the thumbnail names and the values are their dimensions.
 
-For example::
+For example:
+
+.. code-block:: python
 
    IMAGES_THUMBS = {
-       'small': (50, 50),
-       'big': (270, 270),
+       "small": (50, 50),
+       "big": (270, 270),
    }
 
 When you use this feature, the Images Pipeline will create thumbnails of the
 each specified size with this format::
 
     <IMAGES_STORE>/thumbs/<size_name>/<image_id>.jpg
 
@@ -491,25 +523,27 @@
       :class:`item <scrapy.Item>`
 
       You can override this method to customize the download path of each file.
 
       For example, if file URLs end like regular paths (e.g.
       ``https://example.com/a/b/c/foo.png``), you can use the following
       approach to download all files into the ``files`` folder with their
-      original filenames (e.g. ``files/foo.png``)::
+      original filenames (e.g. ``files/foo.png``):
+
+      .. code-block:: python
 
         from pathlib import PurePosixPath
         from urllib.parse import urlparse
 
         from scrapy.pipelines.files import FilesPipeline
 
-        class MyFilesPipeline(FilesPipeline):
 
+        class MyFilesPipeline(FilesPipeline):
             def file_path(self, request, response=None, info=None, *, item=None):
-                return 'files/' + PurePosixPath(urlparse(request.url).path).name
+                return "files/" + PurePosixPath(urlparse(request.url).path).name
 
       Similarly, you can use the ``item`` to determine the file path based on some item 
       property.
       
       By default the :meth:`file_path` method returns
       ``full/<request URL hash>.<extension>``.
 
@@ -517,21 +551,24 @@
          The *item* parameter.
 
    .. method:: FilesPipeline.get_media_requests(item, info)
 
       As seen on the workflow, the pipeline will get the URLs of the images to
       download from the item. In order to do this, you can override the
       :meth:`~get_media_requests` method and return a Request for each
-      file URL::
+      file URL:
+
+      .. code-block:: python
 
          from itemadapter import ItemAdapter
 
+
          def get_media_requests(self, item, info):
              adapter = ItemAdapter(item)
-             for file_url in adapter['file_urls']:
+             for file_url in adapter["file_urls"]:
                  yield scrapy.Request(file_url)
 
       Those requests will be processed by the pipeline and, when they have finished
       downloading, the results will be sent to the
       :meth:`~item_completed` method, as a list of 2-element tuples.
       Each tuple will contain ``(success, file_info_or_error)`` where:
 
@@ -563,23 +600,34 @@
           * ``cached`` - file was already scheduled for download, by another item
             sharing the same file.
 
       The list of tuples received by :meth:`~item_completed` is
       guaranteed to retain the same order of the requests returned from the
       :meth:`~get_media_requests` method.
 
-      Here's a typical value of the ``results`` argument::
+      Here's a typical value of the ``results`` argument:
+
+      .. invisible-code-block: python
+
+          from twisted.python.failure import Failure
 
-          [(True,
-            {'checksum': '2b00042f7481c7b056c4b410d28f33cf',
-             'path': 'full/0a79c461a4062ac383dc4fade7bc09f1384a3910.jpg',
-             'url': 'http://www.example.com/files/product1.pdf',
-             'status': 'downloaded'}),
-           (False,
-            Failure(...))]
+      .. code-block:: python
+
+          [
+              (
+                  True,
+                  {
+                      "checksum": "2b00042f7481c7b056c4b410d28f33cf",
+                      "path": "full/0a79c461a4062ac383dc4fade7bc09f1384a3910.jpg",
+                      "url": "http://www.example.com/files/product1.pdf",
+                      "status": "downloaded",
+                  },
+              ),
+              (False, Failure(...)),
+          ]
 
       By default the :meth:`get_media_requests` method returns ``None`` which
       means there are no files to download for the item.
 
    .. method:: FilesPipeline.item_completed(results, item, info)
 
       The :meth:`FilesPipeline.item_completed` method called when all file
@@ -588,25 +636,28 @@
 
       The :meth:`~item_completed` method must return the
       output that will be sent to subsequent item pipeline stages, so you must
       return (or drop) the item, as you would in any pipeline.
 
       Here is an example of the :meth:`~item_completed` method where we
       store the downloaded file paths (passed in results) in the ``file_paths``
-      item field, and we drop the item if it doesn't contain any files::
+      item field, and we drop the item if it doesn't contain any files:
+
+      .. code-block:: python
 
           from itemadapter import ItemAdapter
           from scrapy.exceptions import DropItem
 
+
           def item_completed(self, results, item, info):
-              file_paths = [x['path'] for ok, x in results if ok]
+              file_paths = [x["path"] for ok, x in results if ok]
               if not file_paths:
                   raise DropItem("Item contains no files")
               adapter = ItemAdapter(item)
-              adapter['file_paths'] = file_paths
+              adapter["file_paths"] = file_paths
               return item
 
       By default, the :meth:`item_completed` method returns the item.
 
 
 .. module:: scrapy.pipelines.images
    :synopsis: Images Pipeline
@@ -630,25 +681,27 @@
       :class:`item <scrapy.Item>`
 
       You can override this method to customize the download path of each file.
 
       For example, if file URLs end like regular paths (e.g.
       ``https://example.com/a/b/c/foo.png``), you can use the following
       approach to download all files into the ``files`` folder with their
-      original filenames (e.g. ``files/foo.png``)::
+      original filenames (e.g. ``files/foo.png``):
+
+      .. code-block:: python
 
         from pathlib import PurePosixPath
         from urllib.parse import urlparse
 
         from scrapy.pipelines.images import ImagesPipeline
 
-        class MyImagesPipeline(ImagesPipeline):
 
+        class MyImagesPipeline(ImagesPipeline):
             def file_path(self, request, response=None, info=None, *, item=None):
-                return 'files/' + PurePosixPath(urlparse(request.url).path).name
+                return "files/" + PurePosixPath(urlparse(request.url).path).name
 
       Similarly, you can use the ``item`` to determine the file path based on some item 
       property.
       
       By default the :meth:`file_path` method returns
       ``full/<request URL hash>.<extension>``.
 
@@ -696,37 +749,39 @@
 
 .. _media-pipeline-example:
 
 Custom Images pipeline example
 ==============================
 
 Here is a full example of the Images Pipeline whose methods are exemplified
-above::
+above:
+
+.. code-block:: python
 
     import scrapy
     from itemadapter import ItemAdapter
     from scrapy.exceptions import DropItem
     from scrapy.pipelines.images import ImagesPipeline
 
-    class MyImagesPipeline(ImagesPipeline):
 
+    class MyImagesPipeline(ImagesPipeline):
         def get_media_requests(self, item, info):
-            for image_url in item['image_urls']:
+            for image_url in item["image_urls"]:
                 yield scrapy.Request(image_url)
 
         def item_completed(self, results, item, info):
-            image_paths = [x['path'] for ok, x in results if ok]
+            image_paths = [x["path"] for ok, x in results if ok]
             if not image_paths:
                 raise DropItem("Item contains no images")
             adapter = ItemAdapter(item)
-            adapter['image_paths'] = image_paths
+            adapter["image_paths"] = image_paths
             return item
 
 
 To enable your custom media pipeline component you must add its class import path to the
-:setting:`ITEM_PIPELINES` setting, like in the following example::
+:setting:`ITEM_PIPELINES` setting, like in the following example:
 
-   ITEM_PIPELINES = {
-       'myproject.pipelines.MyImagesPipeline': 300
-   }
+.. code-block:: python
+
+   ITEM_PIPELINES = {"myproject.pipelines.MyImagesPipeline": 300}
 
 .. _MD5 hash: https://en.wikipedia.org/wiki/MD5
```

### Comparing `Scrapy-2.8.0/docs/topics/practices.rst` & `Scrapy-2.9.0/docs/topics/practices.rst`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 ================
 Common Practices
 ================
 
 This section documents common practices when using Scrapy. These are things
 that cover many topics and don't often fall into any other specific section.
 
+.. skip: start
+
 .. _run-from-script:
 
 Run Scrapy from a script
 ========================
 
 You can use the :ref:`API <topics-api>` to run Scrapy from a script, instead of
 the typical way of running Scrapy via ``scrapy crawl``.
@@ -21,54 +23,58 @@
 The first utility you can use to run your spiders is
 :class:`scrapy.crawler.CrawlerProcess`. This class will start a Twisted reactor
 for you, configuring the logging and setting shutdown handlers. This class is
 the one used by all Scrapy commands.
 
 Here's an example showing how to run a single spider with it.
 
-::
+.. code-block:: python
 
     import scrapy
     from scrapy.crawler import CrawlerProcess
 
+
     class MySpider(scrapy.Spider):
         # Your spider definition
         ...
 
-    process = CrawlerProcess(settings={
-        "FEEDS": {
-            "items.json": {"format": "json"},
-        },
-    })
+
+    process = CrawlerProcess(
+        settings={
+            "FEEDS": {
+                "items.json": {"format": "json"},
+            },
+        }
+    )
 
     process.crawl(MySpider)
-    process.start() # the script will block here until the crawling is finished
+    process.start()  # the script will block here until the crawling is finished
 
 Define settings within dictionary in CrawlerProcess. Make sure to check :class:`~scrapy.crawler.CrawlerProcess`
 documentation to get acquainted with its usage details.
 
 If you are inside a Scrapy project there are some additional helpers you can
 use to import those components within the project. You can automatically import
 your spiders passing their name to :class:`~scrapy.crawler.CrawlerProcess`, and
 use ``get_project_settings`` to get a :class:`~scrapy.settings.Settings`
 instance with your project settings.
 
 What follows is a working example of how to do that, using the `testspiders`_
 project as example.
 
-::
+.. code-block:: python
 
     from scrapy.crawler import CrawlerProcess
     from scrapy.utils.project import get_project_settings
 
     process = CrawlerProcess(get_project_settings())
 
     # 'followall' is the name of one of the spiders of the project.
-    process.crawl('followall', domain='scrapy.org')
-    process.start() # the script will block here until the crawling is finished
+    process.crawl("followall", domain="scrapy.org")
+    process.start()  # the script will block here until the crawling is finished
 
 There's another Scrapy utility that provides more control over the crawling
 process: :class:`scrapy.crawler.CrawlerRunner`. This class is a thin wrapper
 that encapsulates some simple helpers to run multiple crawlers, but it won't
 start or interfere with existing reactors in any way.
 
 Using this class the reactor should be explicitly run after scheduling your
@@ -80,122 +86,135 @@
 spider is finished. This can be achieved by adding callbacks to the deferred
 returned by the :meth:`CrawlerRunner.crawl
 <scrapy.crawler.CrawlerRunner.crawl>` method.
 
 Here's an example of its usage, along with a callback to manually stop the
 reactor after ``MySpider`` has finished running.
 
-::
+.. code-block:: python
 
     from twisted.internet import reactor
     import scrapy
     from scrapy.crawler import CrawlerRunner
     from scrapy.utils.log import configure_logging
 
+
     class MySpider(scrapy.Spider):
         # Your spider definition
         ...
 
-    configure_logging({'LOG_FORMAT': '%(levelname)s: %(message)s'})
+
+    configure_logging({"LOG_FORMAT": "%(levelname)s: %(message)s"})
     runner = CrawlerRunner()
 
     d = runner.crawl(MySpider)
     d.addBoth(lambda _: reactor.stop())
-    reactor.run() # the script will block here until the crawling is finished
+    reactor.run()  # the script will block here until the crawling is finished
 
 .. seealso:: :doc:`twisted:core/howto/reactor-basics`
 
 .. _run-multiple-spiders:
 
 Running multiple spiders in the same process
 ============================================
 
 By default, Scrapy runs a single spider per process when you run ``scrapy
 crawl``. However, Scrapy supports running multiple spiders per process using
 the :ref:`internal API <topics-api>`.
 
 Here is an example that runs multiple spiders simultaneously:
 
-::
+.. code-block:: python
 
     import scrapy
     from scrapy.crawler import CrawlerProcess
     from scrapy.utils.project import get_project_settings
 
+
     class MySpider1(scrapy.Spider):
         # Your first spider definition
         ...
 
+
     class MySpider2(scrapy.Spider):
         # Your second spider definition
         ...
 
+
     settings = get_project_settings()
     process = CrawlerProcess(settings)
     process.crawl(MySpider1)
     process.crawl(MySpider2)
-    process.start() # the script will block here until all crawling jobs are finished
+    process.start()  # the script will block here until all crawling jobs are finished
 
 Same example using :class:`~scrapy.crawler.CrawlerRunner`:
 
-::
+.. code-block:: python
 
     import scrapy
     from twisted.internet import reactor
     from scrapy.crawler import CrawlerRunner
     from scrapy.utils.log import configure_logging
     from scrapy.utils.project import get_project_settings
 
+
     class MySpider1(scrapy.Spider):
         # Your first spider definition
         ...
 
+
     class MySpider2(scrapy.Spider):
         # Your second spider definition
         ...
 
+
     configure_logging()
     settings = get_project_settings()
     runner = CrawlerRunner(settings)
     runner.crawl(MySpider1)
     runner.crawl(MySpider2)
     d = runner.join()
     d.addBoth(lambda _: reactor.stop())
 
-    reactor.run() # the script will block here until all crawling jobs are finished
+    reactor.run()  # the script will block here until all crawling jobs are finished
 
 Same example but running the spiders sequentially by chaining the deferreds:
 
-::
+.. code-block:: python
 
     from twisted.internet import reactor, defer
     from scrapy.crawler import CrawlerRunner
     from scrapy.utils.log import configure_logging
     from scrapy.utils.project import get_project_settings
 
+
     class MySpider1(scrapy.Spider):
         # Your first spider definition
         ...
 
+
     class MySpider2(scrapy.Spider):
         # Your second spider definition
         ...
 
+
     settings = get_project_settings()
     configure_logging(settings)
     runner = CrawlerRunner(settings)
 
+
     @defer.inlineCallbacks
     def crawl():
         yield runner.crawl(MySpider1)
         yield runner.crawl(MySpider2)
         reactor.stop()
 
+
     crawl()
-    reactor.run() # the script will block here until the last crawl call is finished
+    reactor.run()  # the script will block here until the last crawl call is finished
 
 Different spiders can set different values for the same setting, but when they
 run in the same process it may be impossible, by design or because of some
 limitations, to use these different values. What happens in practice is
 different for different settings:
 
 * :setting:`SPIDER_LOADER_CLASS` and the ones used by its value
@@ -210,14 +229,16 @@
   ones used by the resolver (:setting:`DNSCACHE_ENABLED`,
   :setting:`DNSCACHE_SIZE`, :setting:`DNS_TIMEOUT` for ones included in Scrapy)
   the first available value is used. These are applied when the reactor is
   started.
 
 .. seealso:: :ref:`run-from-script`.
 
+.. skip: end
+
 .. _distributed-crawls:
 
 Distributed crawls
 ==================
 
 Scrapy doesn't provide any built-in facility for running crawls in a distribute
 (multi-server) manner. However, there are some ways to distribute crawls, which
```

### Comparing `Scrapy-2.8.0/docs/topics/request-response.rst` & `Scrapy-2.9.0/docs/topics/request-response.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,31 +72,39 @@
             :class:`Request.cookies <scrapy.Request>` parameter. This is a known
             current limitation that is being worked on.
 
     :type headers: dict
 
     :param cookies: the request cookies. These can be sent in two forms.
 
-        1. Using a dict::
+        .. invisible-code-block: python
+
+            from scrapy.http import Request
+
+        1. Using a dict:
+
+        .. code-block:: python
 
             request_with_cookies = Request(
                 url="http://www.example.com",
-                cookies={'currency': 'USD', 'country': 'UY'},
+                cookies={"currency": "USD", "country": "UY"},
             )
 
-        2. Using a list of dicts::
+        2. Using a list of dicts:
+
+        .. code-block:: python
 
             request_with_cookies = Request(
                 url="http://www.example.com",
                 cookies=[
                     {
-                        'name': 'currency',
-                        'value': 'USD',
-                        'domain': 'example.com',
-                        'path': '/currency',
+                        "name": "currency",
+                        "value": "USD",
+                        "domain": "example.com",
+                        "path": "/currency",
                     },
                 ],
             )
 
         The latter form allows for customizing the ``domain`` and ``path``
         attributes of the cookie. This is only useful if the cookies are saved
         for later requests.
@@ -108,20 +116,22 @@
         That's the typical behaviour of any regular web browser.
 
         To create a request that does not send stored cookies and does not
         store received cookies, set the ``dont_merge_cookies`` key to ``True``
         in :attr:`request.meta <scrapy.Request.meta>`.
 
         Example of a request that sends manually-defined cookies and ignores
-        cookie storage::
+        cookie storage:
+
+        .. code-block:: python
 
             Request(
                 url="http://www.example.com",
-                cookies={'currency': 'USD', 'country': 'UY'},
-                meta={'dont_merge_cookies': True},
+                cookies={"currency": "USD", "country": "UY"},
+                meta={"dont_merge_cookies": True},
             )
 
         For more info see :ref:`cookies-mw`.
 
         .. caution:: Cookies set via the ``Cookie`` header are not considered by the
             :ref:`cookies-mw`. If you need to set cookies for a request, use the
             :class:`Request.cookies <scrapy.Request>` parameter. This is a known
@@ -255,38 +265,45 @@
 Passing additional data to callback functions
 ---------------------------------------------
 
 The callback of a request is a function that will be called when the response
 of that request is downloaded. The callback function will be called with the
 downloaded :class:`Response` object as its first argument.
 
-Example::
+Example:
+
+.. code-block:: python
 
     def parse_page1(self, response):
-        return scrapy.Request("http://www.example.com/some_page.html",
-                              callback=self.parse_page2)
+        return scrapy.Request(
+            "http://www.example.com/some_page.html", callback=self.parse_page2
+        )
+
 
     def parse_page2(self, response):
         # this would log http://www.example.com/some_page.html
         self.logger.info("Visited %s", response.url)
 
 In some cases you may be interested in passing arguments to those callback
 functions so you can receive the arguments later, in the second callback.
 The following example shows how to achieve this by using the
 :attr:`Request.cb_kwargs` attribute:
 
-::
+.. code-block:: python
 
     def parse(self, response):
-        request = scrapy.Request('http://www.example.com/index.html',
-                                 callback=self.parse_page2,
-                                 cb_kwargs=dict(main_url=response.url))
-        request.cb_kwargs['foo'] = 'bar'  # add more arguments for the callback
+        request = scrapy.Request(
+            "http://www.example.com/index.html",
+            callback=self.parse_page2,
+            cb_kwargs=dict(main_url=response.url),
+        )
+        request.cb_kwargs["foo"] = "bar"  # add more arguments for the callback
         yield request
 
+
     def parse_page2(self, response, main_url, foo):
         yield dict(
             main_url=main_url,
             other_url=response.url,
             foo=foo,
         )
 
@@ -304,88 +321,100 @@
 The errback of a request is a function that will be called when an exception
 is raise while processing it.
 
 It receives a :exc:`~twisted.python.failure.Failure` as first parameter and can
 be used to track connection establishment timeouts, DNS errors etc.
 
 Here's an example spider logging all errors and catching some specific
-errors if needed::
+errors if needed:
+
+.. code-block:: python
 
     import scrapy
 
     from scrapy.spidermiddlewares.httperror import HttpError
     from twisted.internet.error import DNSLookupError
     from twisted.internet.error import TimeoutError, TCPTimedOutError
 
+
     class ErrbackSpider(scrapy.Spider):
         name = "errback_example"
         start_urls = [
-            "http://www.httpbin.org/",              # HTTP 200 expected
-            "http://www.httpbin.org/status/404",    # Not found error
-            "http://www.httpbin.org/status/500",    # server issue
-            "http://www.httpbin.org:12345/",        # non-responding host, timeout expected
-            "https://example.invalid/",             # DNS error expected
+            "http://www.httpbin.org/",  # HTTP 200 expected
+            "http://www.httpbin.org/status/404",  # Not found error
+            "http://www.httpbin.org/status/500",  # server issue
+            "http://www.httpbin.org:12345/",  # non-responding host, timeout expected
+            "https://example.invalid/",  # DNS error expected
         ]
 
         def start_requests(self):
             for u in self.start_urls:
-                yield scrapy.Request(u, callback=self.parse_httpbin,
-                                        errback=self.errback_httpbin,
-                                        dont_filter=True)
+                yield scrapy.Request(
+                    u,
+                    callback=self.parse_httpbin,
+                    errback=self.errback_httpbin,
+                    dont_filter=True,
+                )
 
         def parse_httpbin(self, response):
-            self.logger.info('Got successful response from {}'.format(response.url))
+            self.logger.info("Got successful response from {}".format(response.url))
             # do something useful here...
 
         def errback_httpbin(self, failure):
             # log all failures
             self.logger.error(repr(failure))
 
             # in case you want to do something special for some errors,
             # you may need the failure's type:
 
             if failure.check(HttpError):
                 # these exceptions come from HttpError spider middleware
                 # you can get the non-200 response
                 response = failure.value.response
-                self.logger.error('HttpError on %s', response.url)
+                self.logger.error("HttpError on %s", response.url)
 
             elif failure.check(DNSLookupError):
                 # this is the original request
                 request = failure.request
-                self.logger.error('DNSLookupError on %s', request.url)
+                self.logger.error("DNSLookupError on %s", request.url)
 
             elif failure.check(TimeoutError, TCPTimedOutError):
                 request = failure.request
-                self.logger.error('TimeoutError on %s', request.url)
+                self.logger.error("TimeoutError on %s", request.url)
 
 
 .. _errback-cb_kwargs:
 
 Accessing additional data in errback functions
 ----------------------------------------------
 
 In case of a failure to process the request, you may be interested in
 accessing arguments to the callback functions so you can process further
 based on the arguments in the errback. The following example shows how to
-achieve this by using ``Failure.request.cb_kwargs``::
+achieve this by using ``Failure.request.cb_kwargs``:
+
+.. code-block:: python
 
     def parse(self, response):
-        request = scrapy.Request('http://www.example.com/index.html',
-                                 callback=self.parse_page2,
-                                 errback=self.errback_page2,
-                                 cb_kwargs=dict(main_url=response.url))
+        request = scrapy.Request(
+            "http://www.example.com/index.html",
+            callback=self.parse_page2,
+            errback=self.errback_page2,
+            cb_kwargs=dict(main_url=response.url),
+        )
         yield request
 
+
     def parse_page2(self, response, main_url):
         pass
 
+
     def errback_page2(self, failure):
         yield dict(
-            main_url=failure.request.cb_kwargs['main_url'],
+            main_url=failure.request.cb_kwargs["main_url"],
         )
 
 
 .. _request-fingerprints:
 
 Request fingerprints
 --------------------
@@ -524,26 +553,28 @@
 :func:`scrapy.utils.request.fingerprint` with its default parameters. For some
 common use cases you can use :func:`scrapy.utils.request.fingerprint` as well
 in your :meth:`fingerprint` method implementation:
 
 .. autofunction:: scrapy.utils.request.fingerprint
 
 For example, to take the value of a request header named ``X-ID`` into
-account::
+account:
+
+.. code-block:: python
 
     # my_project/settings.py
-    REQUEST_FINGERPRINTER_CLASS = 'my_project.utils.RequestFingerprinter'
+    REQUEST_FINGERPRINTER_CLASS = "my_project.utils.RequestFingerprinter"
 
     # my_project/utils.py
     from scrapy.utils.request import fingerprint
 
-    class RequestFingerprinter:
 
+    class RequestFingerprinter:
         def fingerprint(self, request):
-            return fingerprint(request, include_headers=['X-ID'])
+            return fingerprint(request, include_headers=["X-ID"])
 
 You can also write your own fingerprinting logic from scratch.
 
 However, if you do not use :func:`scrapy.utils.request.fingerprint`, make sure
 you use :class:`~weakref.WeakKeyDictionary` to cache request fingerprints:
 
 -   Caching saves CPU by ensuring that fingerprints are calculated only once
@@ -551,68 +582,74 @@
     of a request.
 
 -   Using :class:`~weakref.WeakKeyDictionary` saves memory by ensuring that
     request objects do not stay in memory forever just because you have
     references to them in your cache dictionary.
 
 For example, to take into account only the URL of a request, without any prior
-URL canonicalization or taking the request method or body into account::
+URL canonicalization or taking the request method or body into account:
+
+.. code-block:: python
 
     from hashlib import sha1
     from weakref import WeakKeyDictionary
 
     from scrapy.utils.python import to_bytes
 
-    class RequestFingerprinter:
 
+    class RequestFingerprinter:
         cache = WeakKeyDictionary()
 
         def fingerprint(self, request):
             if request not in self.cache:
                 fp = sha1()
                 fp.update(to_bytes(request.url))
                 self.cache[request] = fp.digest()
             return self.cache[request]
 
 If you need to be able to override the request fingerprinting for arbitrary
 requests from your spider callbacks, you may implement a request fingerprinter
 that reads fingerprints from :attr:`request.meta <scrapy.http.Request.meta>`
 when available, and then falls back to
-:func:`scrapy.utils.request.fingerprint`. For example::
+:func:`scrapy.utils.request.fingerprint`. For example:
+
+.. code-block:: python
 
     from scrapy.utils.request import fingerprint
 
-    class RequestFingerprinter:
 
+    class RequestFingerprinter:
         def fingerprint(self, request):
-            if 'fingerprint' in request.meta:
-                return request.meta['fingerprint']
+            if "fingerprint" in request.meta:
+                return request.meta["fingerprint"]
             return fingerprint(request)
 
 If you need to reproduce the same fingerprinting algorithm as Scrapy 2.6
 without using the deprecated ``'2.6'`` value of the
 :setting:`REQUEST_FINGERPRINTER_IMPLEMENTATION` setting, use the following
-request fingerprinter::
+request fingerprinter:
+
+.. code-block:: python
 
     from hashlib import sha1
     from weakref import WeakKeyDictionary
 
     from scrapy.utils.python import to_bytes
     from w3lib.url import canonicalize_url
 
-    class RequestFingerprinter:
 
+    class RequestFingerprinter:
         cache = WeakKeyDictionary()
 
         def fingerprint(self, request):
             if request not in self.cache:
                 fp = sha1()
                 fp.update(to_bytes(request.method))
                 fp.update(to_bytes(canonicalize_url(request.url)))
-                fp.update(request.body or b'')
+                fp.update(request.body or b"")
                 self.cache[request] = fp.digest()
             return self.cache[request]
 
 
 .. _request-fingerprint-restrictions:
 
 Request fingerprint restrictions
@@ -733,27 +770,31 @@
 .. _topics-stop-response-download:
 
 Stopping the download of a Response
 ===================================
 
 Raising a :exc:`~scrapy.exceptions.StopDownload` exception from a handler for the
 :class:`~scrapy.signals.bytes_received` or :class:`~scrapy.signals.headers_received`
-signals will stop the download of a given response. See the following example::
+signals will stop the download of a given response. See the following example:
+
+.. code-block:: python
 
     import scrapy
 
 
     class StopSpider(scrapy.Spider):
         name = "stop"
         start_urls = ["https://docs.scrapy.org/en/latest/"]
 
         @classmethod
         def from_crawler(cls, crawler):
             spider = super().from_crawler(crawler)
-            crawler.signals.connect(spider.on_bytes_received, signal=scrapy.signals.bytes_received)
+            crawler.signals.connect(
+                spider.on_bytes_received, signal=scrapy.signals.bytes_received
+            )
             return spider
 
         def parse(self, response):
             # 'last_chars' show that the full response was not downloaded
             yield {"len": len(response.text), "last_chars": response.text[-40:]}
 
         def on_bytes_received(self, data, request, spider):
@@ -874,49 +915,59 @@
 ----------------------
 
 Using FormRequest to send data via HTTP POST
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 If you want to simulate a HTML Form POST in your spider and send a couple of
 key-value fields, you can return a :class:`FormRequest` object (from your
-spider) like this::
+spider) like this:
+
+.. skip: next
+.. code-block:: python
 
-   return [FormRequest(url="http://www.example.com/post/action",
-                       formdata={'name': 'John Doe', 'age': '27'},
-                       callback=self.after_post)]
+   return [
+       FormRequest(
+           url="http://www.example.com/post/action",
+           formdata={"name": "John Doe", "age": "27"},
+           callback=self.after_post,
+       )
+   ]
 
 .. _topics-request-response-ref-request-userlogin:
 
 Using FormRequest.from_response() to simulate a user login
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 It is usual for web sites to provide pre-populated form fields through ``<input
 type="hidden">`` elements, such as session related data or authentication
 tokens (for login pages). When scraping, you'll want these fields to be
 automatically pre-populated and only override a couple of them, such as the
 user name and password. You can use the :meth:`FormRequest.from_response`
-method for this job. Here's an example spider which uses it::
+method for this job. Here's an example spider which uses it:
 
+.. code-block:: python
 
     import scrapy
 
+
     def authentication_failed(response):
         # TODO: Check the contents of the response and return True if it failed
         # or False if it succeeded.
         pass
 
+
     class LoginSpider(scrapy.Spider):
-        name = 'example.com'
-        start_urls = ['http://www.example.com/users/login.php']
+        name = "example.com"
+        start_urls = ["http://www.example.com/users/login.php"]
 
         def parse(self, response):
             return scrapy.FormRequest.from_response(
                 response,
-                formdata={'username': 'john', 'password': 'secret'},
-                callback=self.after_login
+                formdata={"username": "john", "password": "secret"},
+                callback=self.after_login,
             )
 
         def after_login(self, response):
             if authentication_failed(response):
                 self.logger.error("Login failed")
                 return
 
@@ -948,21 +999,24 @@
    :type dumps_kwargs: dict
 
    .. autoattribute:: JsonRequest.attributes
 
 JsonRequest usage example
 -------------------------
 
-Sending a JSON POST request with a JSON payload::
+Sending a JSON POST request with a JSON payload:
+
+.. skip: next
+.. code-block:: python
 
    data = {
-       'name1': 'value1',
-       'name2': 'value2',
+       "name1": "value1",
+       "name2": "value2",
    }
-   yield JsonRequest(url='http://www.example.com/post/action', data=data)
+   yield JsonRequest(url="http://www.example.com/post/action", data=data)
 
 
 Response objects
 ================
 
 .. autoclass:: Response
 
@@ -1189,16 +1243,18 @@
        ``response.text`` multiple times without extra overhead.
 
        .. note::
 
             ``str(response.body)`` is not a correct way to convert the response
             body into a string:
 
-            >>> str(b'body')
-            "b'body'"
+            .. code-block:: pycon
+
+                >>> str(b"body")
+                "b'body'"
 
 
     .. attribute:: TextResponse.encoding
 
        A string with the encoding of this response. The encoding is resolved by
        trying the following mechanisms, in order:
 
@@ -1221,14 +1277,20 @@
         target. The selector is lazily instantiated on first access.
 
     .. autoattribute:: TextResponse.attributes
 
     :class:`TextResponse` objects support the following methods in addition to
     the standard :class:`Response` ones:
 
+    .. method:: TextResponse.jmespath(query)
+
+        A shortcut to ``TextResponse.selector.jmespath(query)``::
+
+            response.jmespath('object.[*]')
+
     .. method:: TextResponse.xpath(query)
 
         A shortcut to ``TextResponse.selector.xpath(query)``::
 
             response.xpath('//p')
 
     .. method:: TextResponse.css(query)
```

### Comparing `Scrapy-2.8.0/docs/topics/scheduler.rst` & `Scrapy-2.9.0/docs/topics/scheduler.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/topics/selectors.rst` & `Scrapy-2.9.0/docs/topics/spiders.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,2187 +1,2060 @@
-00000000: 2e2e 205f 746f 7069 6373 2d73 656c 6563  .. _topics-selec
-00000010: 746f 7273 3a0a 0a3d 3d3d 3d3d 3d3d 3d3d  tors:..=========
-00000020: 0a53 656c 6563 746f 7273 0a3d 3d3d 3d3d  .Selectors.=====
-00000030: 3d3d 3d3d 0a0a 5768 656e 2079 6f75 2772  ====..When you'r
-00000040: 6520 7363 7261 7069 6e67 2077 6562 2070  e scraping web p
-00000050: 6167 6573 2c20 7468 6520 6d6f 7374 2063  ages, the most c
-00000060: 6f6d 6d6f 6e20 7461 736b 2079 6f75 206e  ommon task you n
-00000070: 6565 6420 746f 2070 6572 666f 726d 2069  eed to perform i
-00000080: 730a 746f 2065 7874 7261 6374 2064 6174  s.to extract dat
-00000090: 6120 6672 6f6d 2074 6865 2048 544d 4c20  a from the HTML 
-000000a0: 736f 7572 6365 2e20 5468 6572 6520 6172  source. There ar
-000000b0: 6520 7365 7665 7261 6c20 6c69 6272 6172  e several librar
-000000c0: 6965 7320 6176 6169 6c61 626c 6520 746f  ies available to
-000000d0: 0a61 6368 6965 7665 2074 6869 732c 2073  .achieve this, s
-000000e0: 7563 6820 6173 3a0a 0a2d 2020 2060 4265  uch as:..-   `Be
-000000f0: 6175 7469 6675 6c53 6f75 7060 5f20 6973  autifulSoup`_ is
-00000100: 2061 2076 6572 7920 706f 7075 6c61 7220   a very popular 
-00000110: 7765 6220 7363 7261 7069 6e67 206c 6962  web scraping lib
-00000120: 7261 7279 2061 6d6f 6e67 2050 7974 686f  rary among Pytho
-00000130: 6e0a 2020 2020 7072 6f67 7261 6d6d 6572  n.    programmer
-00000140: 7320 7768 6963 6820 636f 6e73 7472 7563  s which construc
-00000150: 7473 2061 2050 7974 686f 6e20 6f62 6a65  ts a Python obje
-00000160: 6374 2062 6173 6564 206f 6e20 7468 6520  ct based on the 
-00000170: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
-00000180: 0a20 2020 2048 544d 4c20 636f 6465 2061  .    HTML code a
-00000190: 6e64 2061 6c73 6f20 6465 616c 7320 7769  nd also deals wi
-000001a0: 7468 2062 6164 206d 6172 6b75 7020 7265  th bad markup re
-000001b0: 6173 6f6e 6162 6c79 2077 656c 6c2c 2062  asonably well, b
-000001c0: 7574 2069 7420 6861 7320 6f6e 650a 2020  ut it has one.  
-000001d0: 2020 6472 6177 6261 636b 3a20 6974 2773    drawback: it's
-000001e0: 2073 6c6f 772e 0a0a 2d20 2020 606c 786d   slow...-   `lxm
-000001f0: 6c60 5f20 6973 2061 6e20 584d 4c20 7061  l`_ is an XML pa
-00000200: 7273 696e 6720 6c69 6272 6172 7920 2877  rsing library (w
-00000210: 6869 6368 2061 6c73 6f20 7061 7273 6573  hich also parses
-00000220: 2048 544d 4c29 2077 6974 6820 6120 7079   HTML) with a py
-00000230: 7468 6f6e 6963 0a20 2020 2041 5049 2062  thonic.    API b
-00000240: 6173 6564 206f 6e20 3a6d 6f64 3a60 7e78  ased on :mod:`~x
-00000250: 6d6c 2e65 7472 6565 2e45 6c65 6d65 6e74  ml.etree.Element
-00000260: 5472 6565 602e 2028 6c78 6d6c 2069 7320  Tree`. (lxml is 
-00000270: 6e6f 7420 7061 7274 206f 6620 7468 6520  not part of the 
-00000280: 5079 7468 6f6e 0a20 2020 2073 7461 6e64  Python.    stand
-00000290: 6172 6420 6c69 6272 6172 792e 290a 0a53  ard library.)..S
-000002a0: 6372 6170 7920 636f 6d65 7320 7769 7468  crapy comes with
-000002b0: 2069 7473 206f 776e 206d 6563 6861 6e69   its own mechani
-000002c0: 736d 2066 6f72 2065 7874 7261 6374 696e  sm for extractin
-000002d0: 6720 6461 7461 2e20 5468 6579 2772 6520  g data. They're 
-000002e0: 6361 6c6c 6564 0a73 656c 6563 746f 7273  called.selectors
-000002f0: 2062 6563 6175 7365 2074 6865 7920 2273   because they "s
-00000300: 656c 6563 7422 2063 6572 7461 696e 2070  elect" certain p
-00000310: 6172 7473 206f 6620 7468 6520 4854 4d4c  arts of the HTML
-00000320: 2064 6f63 756d 656e 7420 7370 6563 6966   document specif
-00000330: 6965 640a 6569 7468 6572 2062 7920 6058  ied.either by `X
-00000340: 5061 7468 605f 206f 7220 6043 5353 605f  Path`_ or `CSS`_
-00000350: 2065 7870 7265 7373 696f 6e73 2e0a 0a60   expressions...`
-00000360: 5850 6174 6860 5f20 6973 2061 206c 616e  XPath`_ is a lan
-00000370: 6775 6167 6520 666f 7220 7365 6c65 6374  guage for select
-00000380: 696e 6720 6e6f 6465 7320 696e 2058 4d4c  ing nodes in XML
-00000390: 2064 6f63 756d 656e 7473 2c20 7768 6963   documents, whic
-000003a0: 6820 6361 6e20 616c 736f 2062 650a 7573  h can also be.us
-000003b0: 6564 2077 6974 6820 4854 4d4c 2e20 6043  ed with HTML. `C
-000003c0: 5353 605f 2069 7320 6120 6c61 6e67 7561  SS`_ is a langua
-000003d0: 6765 2066 6f72 2061 7070 6c79 696e 6720  ge for applying 
-000003e0: 7374 796c 6573 2074 6f20 4854 4d4c 2064  styles to HTML d
-000003f0: 6f63 756d 656e 7473 2e20 4974 0a64 6566  ocuments. It.def
-00000400: 696e 6573 2073 656c 6563 746f 7273 2074  ines selectors t
-00000410: 6f20 6173 736f 6369 6174 6520 7468 6f73  o associate thos
-00000420: 6520 7374 796c 6573 2077 6974 6820 7370  e styles with sp
-00000430: 6563 6966 6963 2048 544d 4c20 656c 656d  ecific HTML elem
-00000440: 656e 7473 2e0a 0a2e 2e20 6e6f 7465 3a3a  ents..... note::
-00000450: 0a20 2020 2053 6372 6170 7920 5365 6c65  .    Scrapy Sele
-00000460: 6374 6f72 7320 6973 2061 2074 6869 6e20  ctors is a thin 
-00000470: 7772 6170 7065 7220 6172 6f75 6e64 2060  wrapper around `
-00000480: 7061 7273 656c 605f 206c 6962 7261 7279  parsel`_ library
-00000490: 3b20 7468 6520 7075 7270 6f73 6520 6f66  ; the purpose of
-000004a0: 0a20 2020 2074 6869 7320 7772 6170 7065  .    this wrappe
-000004b0: 7220 6973 2074 6f20 7072 6f76 6964 6520  r is to provide 
-000004c0: 6265 7474 6572 2069 6e74 6567 7261 7469  better integrati
-000004d0: 6f6e 2077 6974 6820 5363 7261 7079 2052  on with Scrapy R
-000004e0: 6573 706f 6e73 6520 6f62 6a65 6374 732e  esponse objects.
-000004f0: 0a0a 2020 2020 6070 6172 7365 6c60 5f20  ..    `parsel`_ 
-00000500: 6973 2061 2073 7461 6e64 2d61 6c6f 6e65  is a stand-alone
-00000510: 2077 6562 2073 6372 6170 696e 6720 6c69   web scraping li
-00000520: 6272 6172 7920 7768 6963 6820 6361 6e20  brary which can 
-00000530: 6265 2075 7365 6420 7769 7468 6f75 740a  be used without.
-00000540: 2020 2020 5363 7261 7079 2e20 4974 2075      Scrapy. It u
-00000550: 7365 7320 606c 786d 6c60 5f20 6c69 6272  ses `lxml`_ libr
-00000560: 6172 7920 756e 6465 7220 7468 6520 686f  ary under the ho
-00000570: 6f64 2c20 616e 6420 696d 706c 656d 656e  od, and implemen
-00000580: 7473 2061 6e0a 2020 2020 6561 7379 2041  ts an.    easy A
-00000590: 5049 206f 6e20 746f 7020 6f66 206c 786d  PI on top of lxm
-000005a0: 6c20 4150 492e 2049 7420 6d65 616e 7320  l API. It means 
-000005b0: 5363 7261 7079 2073 656c 6563 746f 7273  Scrapy selectors
-000005c0: 2061 7265 2076 6572 7920 7369 6d69 6c61   are very simila
-000005d0: 720a 2020 2020 696e 2073 7065 6564 2061  r.    in speed a
-000005e0: 6e64 2070 6172 7369 6e67 2061 6363 7572  nd parsing accur
-000005f0: 6163 7920 746f 206c 786d 6c2e 0a0a 2e2e  acy to lxml.....
-00000600: 205f 4265 6175 7469 6675 6c53 6f75 703a   _BeautifulSoup:
-00000610: 2068 7474 7073 3a2f 2f77 7777 2e63 7275   https://www.cru
-00000620: 6d6d 792e 636f 6d2f 736f 6674 7761 7265  mmy.com/software
-00000630: 2f42 6561 7574 6966 756c 536f 7570 2f0a  /BeautifulSoup/.
-00000640: 2e2e 205f 6c78 6d6c 3a20 6874 7470 733a  .. _lxml: https:
-00000650: 2f2f 6c78 6d6c 2e64 652f 0a2e 2e20 5f58  //lxml.de/... _X
-00000660: 5061 7468 3a20 6874 7470 733a 2f2f 7777  Path: https://ww
-00000670: 772e 7733 2e6f 7267 2f54 522f 7870 6174  w.w3.org/TR/xpat
-00000680: 682f 616c 6c2f 0a2e 2e20 5f43 5353 3a20  h/all/... _CSS: 
-00000690: 6874 7470 733a 2f2f 7777 772e 7733 2e6f  https://www.w3.o
-000006a0: 7267 2f54 522f 7365 6c65 6374 6f72 730a  rg/TR/selectors.
-000006b0: 2e2e 205f 7061 7273 656c 3a20 6874 7470  .. _parsel: http
-000006c0: 733a 2f2f 7061 7273 656c 2e72 6561 6474  s://parsel.readt
-000006d0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-000006e0: 6573 742f 0a0a 5573 696e 6720 7365 6c65  est/..Using sele
-000006f0: 6374 6f72 730a 3d3d 3d3d 3d3d 3d3d 3d3d  ctors.==========
-00000700: 3d3d 3d3d 3d0a 0a43 6f6e 7374 7275 6374  =====..Construct
-00000710: 696e 6720 7365 6c65 6374 6f72 730a 2d2d  ing selectors.--
-00000720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000730: 2d2d 2d2d 0a0a 2e2e 2068 6967 686c 6967  ----.... highlig
-00000740: 6874 3a3a 2070 7974 686f 6e0a 0a52 6573  ht:: python..Res
-00000750: 706f 6e73 6520 6f62 6a65 6374 7320 6578  ponse objects ex
-00000760: 706f 7365 2061 203a 636c 6173 733a 607e  pose a :class:`~
-00000770: 7363 7261 7079 2e53 656c 6563 746f 7260  scrapy.Selector`
-00000780: 2069 6e73 7461 6e63 650a 6f6e 2060 602e   instance.on ``.
-00000790: 7365 6c65 6374 6f72 6060 2061 7474 7269  selector`` attri
-000007a0: 6275 7465 3a0a 0a3e 3e3e 2072 6573 706f  bute:..>>> respo
-000007b0: 6e73 652e 7365 6c65 6374 6f72 2e78 7061  nse.selector.xpa
-000007c0: 7468 2827 2f2f 7370 616e 2f74 6578 7428  th('//span/text(
-000007d0: 2927 292e 6765 7428 290a 2767 6f6f 6427  )').get().'good'
-000007e0: 0a0a 5175 6572 7969 6e67 2072 6573 706f  ..Querying respo
-000007f0: 6e73 6573 2075 7369 6e67 2058 5061 7468  nses using XPath
-00000800: 2061 6e64 2043 5353 2069 7320 736f 2063   and CSS is so c
-00000810: 6f6d 6d6f 6e20 7468 6174 2072 6573 706f  ommon that respo
-00000820: 6e73 6573 2069 6e63 6c75 6465 2074 776f  nses include two
-00000830: 0a6d 6f72 6520 7368 6f72 7463 7574 733a  .more shortcuts:
-00000840: 2060 6072 6573 706f 6e73 652e 7870 6174   ``response.xpat
-00000850: 6828 2960 6020 616e 6420 6060 7265 7370  h()`` and ``resp
-00000860: 6f6e 7365 2e63 7373 2829 6060 3a0a 0a3e  onse.css()``:..>
-00000870: 3e3e 2072 6573 706f 6e73 652e 7870 6174  >> response.xpat
-00000880: 6828 272f 2f73 7061 6e2f 7465 7874 2829  h('//span/text()
-00000890: 2729 2e67 6574 2829 0a27 676f 6f64 270a  ').get().'good'.
-000008a0: 3e3e 3e20 7265 7370 6f6e 7365 2e63 7373  >>> response.css
-000008b0: 2827 7370 616e 3a3a 7465 7874 2729 2e67  ('span::text').g
-000008c0: 6574 2829 0a27 676f 6f64 270a 0a53 6372  et().'good'..Scr
-000008d0: 6170 7920 7365 6c65 6374 6f72 7320 6172  apy selectors ar
-000008e0: 6520 696e 7374 616e 6365 7320 6f66 203a  e instances of :
-000008f0: 636c 6173 733a 607e 7363 7261 7079 2e53  class:`~scrapy.S
-00000900: 656c 6563 746f 7260 2063 6c61 7373 0a63  elector` class.c
-00000910: 6f6e 7374 7275 6374 6564 2062 7920 7061  onstructed by pa
-00000920: 7373 696e 6720 6569 7468 6572 203a 636c  ssing either :cl
-00000930: 6173 733a 607e 7363 7261 7079 2e68 7474  ass:`~scrapy.htt
-00000940: 702e 5465 7874 5265 7370 6f6e 7365 6020  p.TextResponse` 
-00000950: 6f62 6a65 6374 206f 720a 6d61 726b 7570  object or.markup
-00000960: 2061 7320 6120 7374 7269 6e67 2028 696e   as a string (in
-00000970: 2060 6074 6578 7460 6020 6172 6775 6d65   ``text`` argume
-00000980: 6e74 292e 0a0a 5573 7561 6c6c 7920 7468  nt)...Usually th
-00000990: 6572 6520 6973 206e 6f20 6e65 6564 2074  ere is no need t
-000009a0: 6f20 636f 6e73 7472 7563 7420 5363 7261  o construct Scra
-000009b0: 7079 2073 656c 6563 746f 7273 206d 616e  py selectors man
-000009c0: 7561 6c6c 793a 0a60 6072 6573 706f 6e73  ually:.``respons
-000009d0: 6560 6020 6f62 6a65 6374 2069 7320 6176  e`` object is av
-000009e0: 6169 6c61 626c 6520 696e 2053 7069 6465  ailable in Spide
-000009f0: 7220 6361 6c6c 6261 636b 732c 2073 6f20  r callbacks, so 
-00000a00: 696e 206d 6f73 7420 6361 7365 730a 6974  in most cases.it
-00000a10: 2069 7320 6d6f 7265 2063 6f6e 7665 6e69   is more conveni
-00000a20: 656e 7420 746f 2075 7365 2060 6072 6573  ent to use ``res
-00000a30: 706f 6e73 652e 6373 7328 2960 6020 616e  ponse.css()`` an
-00000a40: 6420 6060 7265 7370 6f6e 7365 2e78 7061  d ``response.xpa
-00000a50: 7468 2829 6060 0a73 686f 7274 6375 7473  th()``.shortcuts
-00000a60: 2e20 4279 2075 7369 6e67 2060 6072 6573  . By using ``res
-00000a70: 706f 6e73 652e 7365 6c65 6374 6f72 6060  ponse.selector``
-00000a80: 206f 7220 6f6e 6520 6f66 2074 6865 7365   or one of these
-00000a90: 2073 686f 7274 6375 7473 0a79 6f75 2063   shortcuts.you c
-00000aa0: 616e 2061 6c73 6f20 656e 7375 7265 2074  an also ensure t
-00000ab0: 6865 2072 6573 706f 6e73 6520 626f 6479  he response body
-00000ac0: 2069 7320 7061 7273 6564 206f 6e6c 7920   is parsed only 
-00000ad0: 6f6e 6365 2e0a 0a42 7574 2069 6620 7265  once...But if re
-00000ae0: 7175 6972 6564 2c20 6974 2069 7320 706f  quired, it is po
-00000af0: 7373 6962 6c65 2074 6f20 7573 6520 6060  ssible to use ``
-00000b00: 5365 6c65 6374 6f72 6060 2064 6972 6563  Selector`` direc
-00000b10: 746c 792e 0a43 6f6e 7374 7275 6374 696e  tly..Constructin
-00000b20: 6720 6672 6f6d 2074 6578 743a 0a0a 3e3e  g from text:..>>
-00000b30: 3e20 6672 6f6d 2073 6372 6170 792e 7365  > from scrapy.se
-00000b40: 6c65 6374 6f72 2069 6d70 6f72 7420 5365  lector import Se
-00000b50: 6c65 6374 6f72 0a3e 3e3e 2062 6f64 7920  lector.>>> body 
-00000b60: 3d20 273c 6874 6d6c 3e3c 626f 6479 3e3c  = '<html><body><
-00000b70: 7370 616e 3e67 6f6f 643c 2f73 7061 6e3e  span>good</span>
-00000b80: 3c2f 626f 6479 3e3c 2f68 746d 6c3e 270a  </body></html>'.
-00000b90: 3e3e 3e20 5365 6c65 6374 6f72 2874 6578  >>> Selector(tex
-00000ba0: 743d 626f 6479 292e 7870 6174 6828 272f  t=body).xpath('/
-00000bb0: 2f73 7061 6e2f 7465 7874 2829 2729 2e67  /span/text()').g
-00000bc0: 6574 2829 0a27 676f 6f64 270a 0a43 6f6e  et().'good'..Con
-00000bd0: 7374 7275 6374 696e 6720 6672 6f6d 2072  structing from r
-00000be0: 6573 706f 6e73 6520 2d20 3a63 6c61 7373  esponse - :class
-00000bf0: 3a60 7e73 6372 6170 792e 6874 7470 2e48  :`~scrapy.http.H
-00000c00: 746d 6c52 6573 706f 6e73 6560 2069 7320  tmlResponse` is 
-00000c10: 6f6e 6520 6f66 0a3a 636c 6173 733a 607e  one of.:class:`~
-00000c20: 7363 7261 7079 2e68 7474 702e 5465 7874  scrapy.http.Text
-00000c30: 5265 7370 6f6e 7365 6020 7375 6263 6c61  Response` subcla
-00000c40: 7373 6573 3a0a 0a3e 3e3e 2066 726f 6d20  sses:..>>> from 
-00000c50: 7363 7261 7079 2e73 656c 6563 746f 7220  scrapy.selector 
-00000c60: 696d 706f 7274 2053 656c 6563 746f 720a  import Selector.
-00000c70: 3e3e 3e20 6672 6f6d 2073 6372 6170 792e  >>> from scrapy.
-00000c80: 6874 7470 2069 6d70 6f72 7420 4874 6d6c  http import Html
-00000c90: 5265 7370 6f6e 7365 0a3e 3e3e 2072 6573  Response.>>> res
-00000ca0: 706f 6e73 6520 3d20 4874 6d6c 5265 7370  ponse = HtmlResp
-00000cb0: 6f6e 7365 2875 726c 3d27 6874 7470 3a2f  onse(url='http:/
-00000cc0: 2f65 7861 6d70 6c65 2e63 6f6d 272c 2062  /example.com', b
-00000cd0: 6f64 793d 626f 6479 290a 3e3e 3e20 5365  ody=body).>>> Se
-00000ce0: 6c65 6374 6f72 2872 6573 706f 6e73 653d  lector(response=
-00000cf0: 7265 7370 6f6e 7365 292e 7870 6174 6828  response).xpath(
-00000d00: 272f 2f73 7061 6e2f 7465 7874 2829 2729  '//span/text()')
-00000d10: 2e67 6574 2829 0a27 676f 6f64 270a 0a60  .get().'good'..`
-00000d20: 6053 656c 6563 746f 7260 6020 6175 746f  `Selector`` auto
-00000d30: 6d61 7469 6361 6c6c 7920 6368 6f6f 7365  matically choose
-00000d40: 7320 7468 6520 6265 7374 2070 6172 7369  s the best parsi
-00000d50: 6e67 2072 756c 6573 0a28 584d 4c20 7673  ng rules.(XML vs
-00000d60: 2048 544d 4c29 2062 6173 6564 206f 6e20   HTML) based on 
-00000d70: 696e 7075 7420 7479 7065 2e0a 0a55 7369  input type...Usi
-00000d80: 6e67 2073 656c 6563 746f 7273 0a2d 2d2d  ng selectors.---
-00000d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 546f  ------------..To
-00000da0: 2065 7870 6c61 696e 2068 6f77 2074 6f20   explain how to 
-00000db0: 7573 6520 7468 6520 7365 6c65 6374 6f72  use the selector
-00000dc0: 7320 7765 276c 6c20 7573 6520 7468 6520  s we'll use the 
-00000dd0: 6060 5363 7261 7079 2073 6865 6c6c 6060  ``Scrapy shell``
-00000de0: 2028 7768 6963 680a 7072 6f76 6964 6573   (which.provides
-00000df0: 2069 6e74 6572 6163 7469 7665 2074 6573   interactive tes
-00000e00: 7469 6e67 2920 616e 6420 616e 2065 7861  ting) and an exa
-00000e10: 6d70 6c65 2070 6167 6520 6c6f 6361 7465  mple page locate
-00000e20: 6420 696e 2074 6865 2053 6372 6170 790a  d in the Scrapy.
-00000e30: 646f 6375 6d65 6e74 6174 696f 6e20 7365  documentation se
-00000e40: 7276 6572 3a0a 0a20 2020 2068 7474 7073  rver:..    https
-00000e50: 3a2f 2f64 6f63 732e 7363 7261 7079 2e6f  ://docs.scrapy.o
-00000e60: 7267 2f65 6e2f 6c61 7465 7374 2f5f 7374  rg/en/latest/_st
-00000e70: 6174 6963 2f73 656c 6563 746f 7273 2d73  atic/selectors-s
-00000e80: 616d 706c 6531 2e68 746d 6c0a 0a2e 2e20  ample1.html.... 
-00000e90: 5f74 6f70 6963 732d 7365 6c65 6374 6f72  _topics-selector
-00000ea0: 732d 6874 6d6c 636f 6465 3a0a 0a46 6f72  s-htmlcode:..For
-00000eb0: 2074 6865 2073 616b 6520 6f66 2063 6f6d   the sake of com
-00000ec0: 706c 6574 656e 6573 732c 2068 6572 6527  pleteness, here'
-00000ed0: 7320 6974 7320 6675 6c6c 2048 544d 4c20  s its full HTML 
-00000ee0: 636f 6465 3a0a 0a2e 2e20 6c69 7465 7261  code:.... litera
-00000ef0: 6c69 6e63 6c75 6465 3a3a 202e 2e2f 5f73  linclude:: ../_s
-00000f00: 7461 7469 632f 7365 6c65 6374 6f72 732d  tatic/selectors-
-00000f10: 7361 6d70 6c65 312e 6874 6d6c 0a20 2020  sample1.html.   
-00000f20: 3a6c 616e 6775 6167 653a 2068 746d 6c0a  :language: html.
-00000f30: 0a2e 2e20 6869 6768 6c69 6768 743a 3a20  ... highlight:: 
-00000f40: 7368 0a0a 4669 7273 742c 206c 6574 2773  sh..First, let's
-00000f50: 206f 7065 6e20 7468 6520 7368 656c 6c3a   open the shell:
-00000f60: 3a0a 0a20 2020 2073 6372 6170 7920 7368  :..    scrapy sh
-00000f70: 656c 6c20 6874 7470 733a 2f2f 646f 6373  ell https://docs
-00000f80: 2e73 6372 6170 792e 6f72 672f 656e 2f6c  .scrapy.org/en/l
-00000f90: 6174 6573 742f 5f73 7461 7469 632f 7365  atest/_static/se
-00000fa0: 6c65 6374 6f72 732d 7361 6d70 6c65 312e  lectors-sample1.
-00000fb0: 6874 6d6c 0a0a 5468 656e 2c20 6166 7465  html..Then, afte
-00000fc0: 7220 7468 6520 7368 656c 6c20 6c6f 6164  r the shell load
-00000fd0: 732c 2079 6f75 276c 6c20 6861 7665 2074  s, you'll have t
-00000fe0: 6865 2072 6573 706f 6e73 6520 6176 6169  he response avai
-00000ff0: 6c61 626c 6520 6173 2060 6072 6573 706f  lable as ``respo
-00001000: 6e73 6560 600a 7368 656c 6c20 7661 7269  nse``.shell vari
-00001010: 6162 6c65 2c20 616e 6420 6974 7320 6174  able, and its at
-00001020: 7461 6368 6564 2073 656c 6563 746f 7220  tached selector 
-00001030: 696e 2060 6072 6573 706f 6e73 652e 7365  in ``response.se
-00001040: 6c65 6374 6f72 6060 2061 7474 7269 6275  lector`` attribu
-00001050: 7465 2e0a 0a53 696e 6365 2077 6527 7265  te...Since we're
-00001060: 2064 6561 6c69 6e67 2077 6974 6820 4854   dealing with HT
-00001070: 4d4c 2c20 7468 6520 7365 6c65 6374 6f72  ML, the selector
-00001080: 2077 696c 6c20 6175 746f 6d61 7469 6361   will automatica
-00001090: 6c6c 7920 7573 6520 616e 2048 544d 4c20  lly use an HTML 
-000010a0: 7061 7273 6572 2e0a 0a2e 2e20 6869 6768  parser..... high
-000010b0: 6c69 6768 743a 3a20 7079 7468 6f6e 0a0a  light:: python..
-000010c0: 536f 2c20 6279 206c 6f6f 6b69 6e67 2061  So, by looking a
-000010d0: 7420 7468 6520 3a72 6566 3a60 4854 4d4c  t the :ref:`HTML
-000010e0: 2063 6f64 6520 3c74 6f70 6963 732d 7365   code <topics-se
-000010f0: 6c65 6374 6f72 732d 6874 6d6c 636f 6465  lectors-htmlcode
-00001100: 3e60 206f 6620 7468 6174 0a70 6167 652c  >` of that.page,
-00001110: 206c 6574 2773 2063 6f6e 7374 7275 6374   let's construct
-00001120: 2061 6e20 5850 6174 6820 666f 7220 7365   an XPath for se
-00001130: 6c65 6374 696e 6720 7468 6520 7465 7874  lecting the text
-00001140: 2069 6e73 6964 6520 7468 6520 7469 746c   inside the titl
-00001150: 6520 7461 673a 0a0a 3e3e 3e20 7265 7370  e tag:..>>> resp
-00001160: 6f6e 7365 2e78 7061 7468 2827 2f2f 7469  onse.xpath('//ti
-00001170: 746c 652f 7465 7874 2829 2729 0a5b 3c53  tle/text()').[<S
-00001180: 656c 6563 746f 7220 7870 6174 683d 272f  elector xpath='/
-00001190: 2f74 6974 6c65 2f74 6578 7428 2927 2064  /title/text()' d
-000011a0: 6174 613d 2745 7861 6d70 6c65 2077 6562  ata='Example web
-000011b0: 7369 7465 273e 5d0a 0a54 6f20 6163 7475  site'>]..To actu
-000011c0: 616c 6c79 2065 7874 7261 6374 2074 6865  ally extract the
-000011d0: 2074 6578 7475 616c 2064 6174 612c 2079   textual data, y
-000011e0: 6f75 206d 7573 7420 6361 6c6c 2074 6865  ou must call the
-000011f0: 2073 656c 6563 746f 7220 6060 2e67 6574   selector ``.get
-00001200: 2829 6060 0a6f 7220 6060 2e67 6574 616c  ()``.or ``.getal
-00001210: 6c28 2960 6020 6d65 7468 6f64 732c 2061  l()`` methods, a
-00001220: 7320 666f 6c6c 6f77 733a 0a0a 3e3e 3e20  s follows:..>>> 
-00001230: 7265 7370 6f6e 7365 2e78 7061 7468 2827  response.xpath('
-00001240: 2f2f 7469 746c 652f 7465 7874 2829 2729  //title/text()')
-00001250: 2e67 6574 616c 6c28 290a 5b27 4578 616d  .getall().['Exam
-00001260: 706c 6520 7765 6273 6974 6527 5d0a 3e3e  ple website'].>>
-00001270: 3e20 7265 7370 6f6e 7365 2e78 7061 7468  > response.xpath
-00001280: 2827 2f2f 7469 746c 652f 7465 7874 2829  ('//title/text()
-00001290: 2729 2e67 6574 2829 0a27 4578 616d 706c  ').get().'Exampl
-000012a0: 6520 7765 6273 6974 6527 0a0a 6060 2e67  e website'..``.g
-000012b0: 6574 2829 6060 2061 6c77 6179 7320 7265  et()`` always re
-000012c0: 7475 726e 7320 6120 7369 6e67 6c65 2072  turns a single r
-000012d0: 6573 756c 743b 2069 6620 7468 6572 6520  esult; if there 
-000012e0: 6172 6520 7365 7665 7261 6c20 6d61 7463  are several matc
-000012f0: 6865 732c 0a63 6f6e 7465 6e74 206f 6620  hes,.content of 
-00001300: 6120 6669 7273 7420 6d61 7463 6820 6973  a first match is
-00001310: 2072 6574 7572 6e65 643b 2069 6620 7468   returned; if th
-00001320: 6572 6520 6172 6520 6e6f 206d 6174 6368  ere are no match
-00001330: 6573 2c20 4e6f 6e65 0a69 7320 7265 7475  es, None.is retu
-00001340: 726e 6564 2e20 6060 2e67 6574 616c 6c28  rned. ``.getall(
-00001350: 2960 6020 7265 7475 726e 7320 6120 6c69  )`` returns a li
-00001360: 7374 2077 6974 6820 616c 6c20 7265 7375  st with all resu
-00001370: 6c74 732e 0a0a 4e6f 7469 6365 2074 6861  lts...Notice tha
-00001380: 7420 4353 5320 7365 6c65 6374 6f72 7320  t CSS selectors 
-00001390: 6361 6e20 7365 6c65 6374 2074 6578 7420  can select text 
-000013a0: 6f72 2061 7474 7269 6275 7465 206e 6f64  or attribute nod
-000013b0: 6573 2075 7369 6e67 2043 5353 330a 7073  es using CSS3.ps
-000013c0: 6575 646f 2d65 6c65 6d65 6e74 733a 0a0a  eudo-elements:..
-000013d0: 3e3e 3e20 7265 7370 6f6e 7365 2e63 7373  >>> response.css
-000013e0: 2827 7469 746c 653a 3a74 6578 7427 292e  ('title::text').
-000013f0: 6765 7428 290a 2745 7861 6d70 6c65 2077  get().'Example w
-00001400: 6562 7369 7465 270a 0a41 7320 796f 7520  ebsite'..As you 
-00001410: 6361 6e20 7365 652c 2060 602e 7870 6174  can see, ``.xpat
-00001420: 6828 2960 6020 616e 6420 6060 2e63 7373  h()`` and ``.css
-00001430: 2829 6060 206d 6574 686f 6473 2072 6574  ()`` methods ret
-00001440: 7572 6e20 610a 3a63 6c61 7373 3a60 7e73  urn a.:class:`~s
-00001450: 6372 6170 792e 7365 6c65 6374 6f72 2e53  crapy.selector.S
-00001460: 656c 6563 746f 724c 6973 7460 2069 6e73  electorList` ins
-00001470: 7461 6e63 652c 2077 6869 6368 2069 7320  tance, which is 
-00001480: 6120 6c69 7374 206f 6620 6e65 770a 7365  a list of new.se
-00001490: 6c65 6374 6f72 732e 2054 6869 7320 4150  lectors. This AP
-000014a0: 4920 6361 6e20 6265 2075 7365 6420 666f  I can be used fo
-000014b0: 7220 7175 6963 6b6c 7920 7365 6c65 6374  r quickly select
-000014c0: 696e 6720 6e65 7374 6564 2064 6174 613a  ing nested data:
-000014d0: 0a0a 3e3e 3e20 7265 7370 6f6e 7365 2e63  ..>>> response.c
-000014e0: 7373 2827 696d 6727 292e 7870 6174 6828  ss('img').xpath(
-000014f0: 2740 7372 6327 292e 6765 7461 6c6c 2829  '@src').getall()
-00001500: 0a5b 2769 6d61 6765 315f 7468 756d 622e  .['image1_thumb.
-00001510: 6a70 6727 2c0a 2027 696d 6167 6532 5f74  jpg',. 'image2_t
-00001520: 6875 6d62 2e6a 7067 272c 0a20 2769 6d61  humb.jpg',. 'ima
-00001530: 6765 335f 7468 756d 622e 6a70 6727 2c0a  ge3_thumb.jpg',.
-00001540: 2027 696d 6167 6534 5f74 6875 6d62 2e6a   'image4_thumb.j
-00001550: 7067 272c 0a20 2769 6d61 6765 355f 7468  pg',. 'image5_th
-00001560: 756d 622e 6a70 6727 5d0a 0a49 6620 796f  umb.jpg']..If yo
-00001570: 7520 7761 6e74 2074 6f20 6578 7472 6163  u want to extrac
-00001580: 7420 6f6e 6c79 2074 6865 2066 6972 7374  t only the first
-00001590: 206d 6174 6368 6564 2065 6c65 6d65 6e74   matched element
-000015a0: 2c20 796f 7520 6361 6e20 6361 6c6c 2074  , you can call t
-000015b0: 6865 0a73 656c 6563 746f 7220 6060 2e67  he.selector ``.g
-000015c0: 6574 2829 6060 2028 6f72 2069 7473 2061  et()`` (or its a
-000015d0: 6c69 6173 2060 602e 6578 7472 6163 745f  lias ``.extract_
-000015e0: 6669 7273 7428 2960 6020 636f 6d6d 6f6e  first()`` common
-000015f0: 6c79 2075 7365 6420 696e 0a70 7265 7669  ly used in.previ
-00001600: 6f75 7320 5363 7261 7079 2076 6572 7369  ous Scrapy versi
-00001610: 6f6e 7329 3a0a 0a3e 3e3e 2072 6573 706f  ons):..>>> respo
-00001620: 6e73 652e 7870 6174 6828 272f 2f64 6976  nse.xpath('//div
-00001630: 5b40 6964 3d22 696d 6167 6573 225d 2f61  [@id="images"]/a
-00001640: 2f74 6578 7428 2927 292e 6765 7428 290a  /text()').get().
-00001650: 274e 616d 653a 204d 7920 696d 6167 6520  'Name: My image 
-00001660: 3120 270a 0a49 7420 7265 7475 726e 7320  1 '..It returns 
-00001670: 6060 4e6f 6e65 6060 2069 6620 6e6f 2065  ``None`` if no e
-00001680: 6c65 6d65 6e74 2077 6173 2066 6f75 6e64  lement was found
-00001690: 3a0a 0a3e 3e3e 2072 6573 706f 6e73 652e  :..>>> response.
-000016a0: 7870 6174 6828 272f 2f64 6976 5b40 6964  xpath('//div[@id
-000016b0: 3d22 6e6f 742d 6578 6973 7473 225d 2f74  ="not-exists"]/t
-000016c0: 6578 7428 2927 292e 6765 7428 2920 6973  ext()').get() is
-000016d0: 204e 6f6e 650a 5472 7565 0a0a 4120 6465   None.True..A de
-000016e0: 6661 756c 7420 7265 7475 726e 2076 616c  fault return val
-000016f0: 7565 2063 616e 2062 6520 7072 6f76 6964  ue can be provid
-00001700: 6564 2061 7320 616e 2061 7267 756d 656e  ed as an argumen
-00001710: 742c 2074 6f20 6265 2075 7365 6420 696e  t, to be used in
-00001720: 7374 6561 640a 6f66 2060 604e 6f6e 6560  stead.of ``None`
-00001730: 603a 0a0a 3e3e 3e20 7265 7370 6f6e 7365  `:..>>> response
-00001740: 2e78 7061 7468 2827 2f2f 6469 765b 4069  .xpath('//div[@i
-00001750: 643d 226e 6f74 2d65 7869 7374 7322 5d2f  d="not-exists"]/
-00001760: 7465 7874 2829 2729 2e67 6574 2864 6566  text()').get(def
-00001770: 6175 6c74 3d27 6e6f 742d 666f 756e 6427  ault='not-found'
-00001780: 290a 276e 6f74 2d66 6f75 6e64 270a 0a49  ).'not-found'..I
-00001790: 6e73 7465 6164 206f 6620 7573 696e 6720  nstead of using 
-000017a0: 652e 672e 2060 6027 4073 7263 2760 6020  e.g. ``'@src'`` 
-000017b0: 5850 6174 6820 6974 2069 7320 706f 7373  XPath it is poss
-000017c0: 6962 6c65 2074 6f20 7175 6572 7920 666f  ible to query fo
-000017d0: 7220 6174 7472 6962 7574 6573 0a75 7369  r attributes.usi
-000017e0: 6e67 2060 602e 6174 7472 6962 6060 2070  ng ``.attrib`` p
-000017f0: 726f 7065 7274 7920 6f66 2061 203a 636c  roperty of a :cl
-00001800: 6173 733a 607e 7363 7261 7079 2e53 656c  ass:`~scrapy.Sel
-00001810: 6563 746f 7260 3a0a 0a3e 3e3e 205b 696d  ector`:..>>> [im
-00001820: 672e 6174 7472 6962 5b27 7372 6327 5d20  g.attrib['src'] 
-00001830: 666f 7220 696d 6720 696e 2072 6573 706f  for img in respo
-00001840: 6e73 652e 6373 7328 2769 6d67 2729 5d0a  nse.css('img')].
-00001850: 5b27 696d 6167 6531 5f74 6875 6d62 2e6a  ['image1_thumb.j
-00001860: 7067 272c 0a20 2769 6d61 6765 325f 7468  pg',. 'image2_th
-00001870: 756d 622e 6a70 6727 2c0a 2027 696d 6167  umb.jpg',. 'imag
-00001880: 6533 5f74 6875 6d62 2e6a 7067 272c 0a20  e3_thumb.jpg',. 
-00001890: 2769 6d61 6765 345f 7468 756d 622e 6a70  'image4_thumb.jp
-000018a0: 6727 2c0a 2027 696d 6167 6535 5f74 6875  g',. 'image5_thu
-000018b0: 6d62 2e6a 7067 275d 0a0a 4173 2061 2073  mb.jpg']..As a s
-000018c0: 686f 7274 6375 742c 2060 602e 6174 7472  hortcut, ``.attr
-000018d0: 6962 6060 2069 7320 616c 736f 2061 7661  ib`` is also ava
-000018e0: 696c 6162 6c65 206f 6e20 5365 6c65 6374  ilable on Select
-000018f0: 6f72 4c69 7374 2064 6972 6563 746c 793b  orList directly;
-00001900: 0a69 7420 7265 7475 726e 7320 6174 7472  .it returns attr
-00001910: 6962 7574 6573 2066 6f72 2074 6865 2066  ibutes for the f
-00001920: 6972 7374 206d 6174 6368 696e 6720 656c  irst matching el
-00001930: 656d 656e 743a 0a0a 3e3e 3e20 7265 7370  ement:..>>> resp
-00001940: 6f6e 7365 2e63 7373 2827 696d 6727 292e  onse.css('img').
-00001950: 6174 7472 6962 5b27 7372 6327 5d0a 2769  attrib['src'].'i
-00001960: 6d61 6765 315f 7468 756d 622e 6a70 6727  mage1_thumb.jpg'
-00001970: 0a0a 5468 6973 2069 7320 6d6f 7374 2075  ..This is most u
-00001980: 7365 6675 6c20 7768 656e 206f 6e6c 7920  seful when only 
-00001990: 6120 7369 6e67 6c65 2072 6573 756c 7420  a single result 
-000019a0: 6973 2065 7870 6563 7465 642c 2065 2e67  is expected, e.g
-000019b0: 2e20 7768 656e 2073 656c 6563 7469 6e67  . when selecting
-000019c0: 0a62 7920 6964 2c20 6f72 2073 656c 6563  .by id, or selec
-000019d0: 7469 6e67 2075 6e69 7175 6520 656c 656d  ting unique elem
-000019e0: 656e 7473 206f 6e20 6120 7765 6220 7061  ents on a web pa
-000019f0: 6765 3a0a 0a3e 3e3e 2072 6573 706f 6e73  ge:..>>> respons
-00001a00: 652e 6373 7328 2762 6173 6527 292e 6174  e.css('base').at
-00001a10: 7472 6962 5b27 6872 6566 275d 0a27 6874  trib['href'].'ht
-00001a20: 7470 3a2f 2f65 7861 6d70 6c65 2e63 6f6d  tp://example.com
-00001a30: 2f27 0a0a 4e6f 7720 7765 2772 6520 676f  /'..Now we're go
-00001a40: 696e 6720 746f 2067 6574 2074 6865 2062  ing to get the b
-00001a50: 6173 6520 5552 4c20 616e 6420 736f 6d65  ase URL and some
-00001a60: 2069 6d61 6765 206c 696e 6b73 3a0a 0a3e   image links:..>
-00001a70: 3e3e 2072 6573 706f 6e73 652e 7870 6174  >> response.xpat
-00001a80: 6828 272f 2f62 6173 652f 4068 7265 6627  h('//base/@href'
-00001a90: 292e 6765 7428 290a 2768 7474 703a 2f2f  ).get().'http://
-00001aa0: 6578 616d 706c 652e 636f 6d2f 270a 0a3e  example.com/'..>
-00001ab0: 3e3e 2072 6573 706f 6e73 652e 6373 7328  >> response.css(
-00001ac0: 2762 6173 653a 3a61 7474 7228 6872 6566  'base::attr(href
-00001ad0: 2927 292e 6765 7428 290a 2768 7474 703a  )').get().'http:
-00001ae0: 2f2f 6578 616d 706c 652e 636f 6d2f 270a  //example.com/'.
-00001af0: 0a3e 3e3e 2072 6573 706f 6e73 652e 6373  .>>> response.cs
-00001b00: 7328 2762 6173 6527 292e 6174 7472 6962  s('base').attrib
-00001b10: 5b27 6872 6566 275d 0a27 6874 7470 3a2f  ['href'].'http:/
-00001b20: 2f65 7861 6d70 6c65 2e63 6f6d 2f27 0a0a  /example.com/'..
-00001b30: 3e3e 3e20 7265 7370 6f6e 7365 2e78 7061  >>> response.xpa
-00001b40: 7468 2827 2f2f 615b 636f 6e74 6169 6e73  th('//a[contains
-00001b50: 2840 6872 6566 2c20 2269 6d61 6765 2229  (@href, "image")
-00001b60: 5d2f 4068 7265 6627 292e 6765 7461 6c6c  ]/@href').getall
-00001b70: 2829 0a5b 2769 6d61 6765 312e 6874 6d6c  ().['image1.html
-00001b80: 272c 0a20 2769 6d61 6765 322e 6874 6d6c  ',. 'image2.html
-00001b90: 272c 0a20 2769 6d61 6765 332e 6874 6d6c  ',. 'image3.html
-00001ba0: 272c 0a20 2769 6d61 6765 342e 6874 6d6c  ',. 'image4.html
-00001bb0: 272c 0a20 2769 6d61 6765 352e 6874 6d6c  ',. 'image5.html
-00001bc0: 275d 0a0a 3e3e 3e20 7265 7370 6f6e 7365  ']..>>> response
-00001bd0: 2e63 7373 2827 615b 6872 6566 2a3d 696d  .css('a[href*=im
-00001be0: 6167 655d 3a3a 6174 7472 2868 7265 6629  age]::attr(href)
-00001bf0: 2729 2e67 6574 616c 6c28 290a 5b27 696d  ').getall().['im
-00001c00: 6167 6531 2e68 746d 6c27 2c0a 2027 696d  age1.html',. 'im
-00001c10: 6167 6532 2e68 746d 6c27 2c0a 2027 696d  age2.html',. 'im
-00001c20: 6167 6533 2e68 746d 6c27 2c0a 2027 696d  age3.html',. 'im
-00001c30: 6167 6534 2e68 746d 6c27 2c0a 2027 696d  age4.html',. 'im
-00001c40: 6167 6535 2e68 746d 6c27 5d0a 0a3e 3e3e  age5.html']..>>>
-00001c50: 2072 6573 706f 6e73 652e 7870 6174 6828   response.xpath(
-00001c60: 272f 2f61 5b63 6f6e 7461 696e 7328 4068  '//a[contains(@h
-00001c70: 7265 662c 2022 696d 6167 6522 295d 2f69  ref, "image")]/i
-00001c80: 6d67 2f40 7372 6327 292e 6765 7461 6c6c  mg/@src').getall
-00001c90: 2829 0a5b 2769 6d61 6765 315f 7468 756d  ().['image1_thum
-00001ca0: 622e 6a70 6727 2c0a 2027 696d 6167 6532  b.jpg',. 'image2
-00001cb0: 5f74 6875 6d62 2e6a 7067 272c 0a20 2769  _thumb.jpg',. 'i
-00001cc0: 6d61 6765 335f 7468 756d 622e 6a70 6727  mage3_thumb.jpg'
-00001cd0: 2c0a 2027 696d 6167 6534 5f74 6875 6d62  ,. 'image4_thumb
-00001ce0: 2e6a 7067 272c 0a20 2769 6d61 6765 355f  .jpg',. 'image5_
-00001cf0: 7468 756d 622e 6a70 6727 5d0a 0a3e 3e3e  thumb.jpg']..>>>
-00001d00: 2072 6573 706f 6e73 652e 6373 7328 2761   response.css('a
-00001d10: 5b68 7265 662a 3d69 6d61 6765 5d20 696d  [href*=image] im
-00001d20: 673a 3a61 7474 7228 7372 6329 2729 2e67  g::attr(src)').g
-00001d30: 6574 616c 6c28 290a 5b27 696d 6167 6531  etall().['image1
-00001d40: 5f74 6875 6d62 2e6a 7067 272c 0a20 2769  _thumb.jpg',. 'i
-00001d50: 6d61 6765 325f 7468 756d 622e 6a70 6727  mage2_thumb.jpg'
-00001d60: 2c0a 2027 696d 6167 6533 5f74 6875 6d62  ,. 'image3_thumb
-00001d70: 2e6a 7067 272c 0a20 2769 6d61 6765 345f  .jpg',. 'image4_
-00001d80: 7468 756d 622e 6a70 6727 2c0a 2027 696d  thumb.jpg',. 'im
-00001d90: 6167 6535 5f74 6875 6d62 2e6a 7067 275d  age5_thumb.jpg']
-00001da0: 0a0a 2e2e 205f 746f 7069 6373 2d73 656c  .... _topics-sel
-00001db0: 6563 746f 7273 2d63 7373 2d65 7874 656e  ectors-css-exten
-00001dc0: 7369 6f6e 733a 0a0a 4578 7465 6e73 696f  sions:..Extensio
-00001dd0: 6e73 2074 6f20 4353 5320 5365 6c65 6374  ns to CSS Select
-00001de0: 6f72 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ors.------------
-00001df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00001e00: 0a50 6572 2057 3343 2073 7461 6e64 6172  .Per W3C standar
-00001e10: 6473 2c20 6043 5353 2073 656c 6563 746f  ds, `CSS selecto
-00001e20: 7273 605f 2064 6f20 6e6f 7420 7375 7070  rs`_ do not supp
-00001e30: 6f72 7420 7365 6c65 6374 696e 6720 7465  ort selecting te
-00001e40: 7874 206e 6f64 6573 0a6f 7220 6174 7472  xt nodes.or attr
-00001e50: 6962 7574 6520 7661 6c75 6573 2e0a 4275  ibute values..Bu
-00001e60: 7420 7365 6c65 6374 696e 6720 7468 6573  t selecting thes
-00001e70: 6520 6973 2073 6f20 6573 7365 6e74 6961  e is so essentia
-00001e80: 6c20 696e 2061 2077 6562 2073 6372 6170  l in a web scrap
-00001e90: 696e 6720 636f 6e74 6578 740a 7468 6174  ing context.that
-00001ea0: 2053 6372 6170 7920 2870 6172 7365 6c29   Scrapy (parsel)
-00001eb0: 2069 6d70 6c65 6d65 6e74 7320 6120 636f   implements a co
-00001ec0: 7570 6c65 206f 6620 2a2a 6e6f 6e2d 7374  uple of **non-st
-00001ed0: 616e 6461 7264 2070 7365 7564 6f2d 656c  andard pseudo-el
-00001ee0: 656d 656e 7473 2a2a 3a0a 0a2a 2074 6f20  ements**:..* to 
-00001ef0: 7365 6c65 6374 2074 6578 7420 6e6f 6465  select text node
-00001f00: 732c 2075 7365 2060 603a 3a74 6578 7460  s, use ``::text`
-00001f10: 600a 2a20 746f 2073 656c 6563 7420 6174  `.* to select at
-00001f20: 7472 6962 7574 6520 7661 6c75 6573 2c20  tribute values, 
-00001f30: 7573 6520 6060 3a3a 6174 7472 286e 616d  use ``::attr(nam
-00001f40: 6529 6060 2077 6865 7265 202a 6e61 6d65  e)`` where *name
-00001f50: 2a20 6973 2074 6865 0a20 206e 616d 6520  * is the.  name 
-00001f60: 6f66 2074 6865 2061 7474 7269 6275 7465  of the attribute
-00001f70: 2074 6861 7420 796f 7520 7761 6e74 2074   that you want t
-00001f80: 6865 2076 616c 7565 206f 660a 0a2e 2e20  he value of.... 
-00001f90: 7761 726e 696e 673a 3a0a 2020 2020 5468  warning::.    Th
-00001fa0: 6573 6520 7073 6575 646f 2d65 6c65 6d65  ese pseudo-eleme
-00001fb0: 6e74 7320 6172 6520 5363 7261 7079 2d2f  nts are Scrapy-/
-00001fc0: 5061 7273 656c 2d73 7065 6369 6669 632e  Parsel-specific.
-00001fd0: 0a20 2020 2054 6865 7920 7769 6c6c 206d  .    They will m
-00001fe0: 6f73 7420 7072 6f62 6162 6c79 206e 6f74  ost probably not
-00001ff0: 2077 6f72 6b20 7769 7468 206f 7468 6572   work with other
-00002000: 206c 6962 7261 7269 6573 206c 696b 650a   libraries like.
-00002010: 2020 2020 606c 786d 6c60 5f20 6f72 2060      `lxml`_ or `
-00002020: 5079 5175 6572 7960 5f2e 0a0a 2e2e 205f  PyQuery`_..... _
-00002030: 5079 5175 6572 793a 2068 7474 7073 3a2f  PyQuery: https:/
-00002040: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00002050: 742f 7079 7175 6572 792f 0a0a 4578 616d  t/pyquery/..Exam
-00002060: 706c 6573 3a0a 0a2a 2060 6074 6974 6c65  ples:..* ``title
-00002070: 3a3a 7465 7874 6060 2073 656c 6563 7473  ::text`` selects
-00002080: 2063 6869 6c64 7265 6e20 7465 7874 206e   children text n
-00002090: 6f64 6573 206f 6620 6120 6465 7363 656e  odes of a descen
-000020a0: 6461 6e74 2060 603c 7469 746c 653e 6060  dant ``<title>``
-000020b0: 2065 6c65 6d65 6e74 3a0a 0a3e 3e3e 2072   element:..>>> r
-000020c0: 6573 706f 6e73 652e 6373 7328 2774 6974  esponse.css('tit
-000020d0: 6c65 3a3a 7465 7874 2729 2e67 6574 2829  le::text').get()
-000020e0: 0a27 4578 616d 706c 6520 7765 6273 6974  .'Example websit
-000020f0: 6527 0a0a 2a20 6060 2a3a 3a74 6578 7460  e'..* ``*::text`
-00002100: 6020 7365 6c65 6374 7320 616c 6c20 6465  ` selects all de
-00002110: 7363 656e 6461 6e74 2074 6578 7420 6e6f  scendant text no
-00002120: 6465 7320 6f66 2074 6865 2063 7572 7265  des of the curre
-00002130: 6e74 2073 656c 6563 746f 7220 636f 6e74  nt selector cont
-00002140: 6578 743a 0a0a 3e3e 3e20 7265 7370 6f6e  ext:..>>> respon
-00002150: 7365 2e63 7373 2827 2369 6d61 6765 7320  se.css('#images 
-00002160: 2a3a 3a74 6578 7427 292e 6765 7461 6c6c  *::text').getall
-00002170: 2829 0a5b 275c 6e20 2020 272c 0a20 274e  ().['\n   ',. 'N
-00002180: 616d 653a 204d 7920 696d 6167 6520 3120  ame: My image 1 
-00002190: 272c 0a20 275c 6e20 2020 272c 0a20 274e  ',. '\n   ',. 'N
-000021a0: 616d 653a 204d 7920 696d 6167 6520 3220  ame: My image 2 
-000021b0: 272c 0a20 275c 6e20 2020 272c 0a20 274e  ',. '\n   ',. 'N
-000021c0: 616d 653a 204d 7920 696d 6167 6520 3320  ame: My image 3 
-000021d0: 272c 0a20 275c 6e20 2020 272c 0a20 274e  ',. '\n   ',. 'N
-000021e0: 616d 653a 204d 7920 696d 6167 6520 3420  ame: My image 4 
-000021f0: 272c 0a20 275c 6e20 2020 272c 0a20 274e  ',. '\n   ',. 'N
-00002200: 616d 653a 204d 7920 696d 6167 6520 3520  ame: My image 5 
-00002210: 272c 0a20 275c 6e20 2027 5d0a 0a2a 2060  ',. '\n  ']..* `
-00002220: 6066 6f6f 3a3a 7465 7874 6060 2072 6574  `foo::text`` ret
-00002230: 7572 6e73 206e 6f20 7265 7375 6c74 7320  urns no results 
-00002240: 6966 2060 6066 6f6f 6060 2065 6c65 6d65  if ``foo`` eleme
-00002250: 6e74 2065 7869 7374 732c 2062 7574 2063  nt exists, but c
-00002260: 6f6e 7461 696e 730a 2020 6e6f 2074 6578  ontains.  no tex
-00002270: 7420 2869 2e65 2e20 7465 7874 2069 7320  t (i.e. text is 
-00002280: 656d 7074 7929 3a0a 0a3e 3e3e 2072 6573  empty):..>>> res
-00002290: 706f 6e73 652e 6373 7328 2769 6d67 3a3a  ponse.css('img::
-000022a0: 7465 7874 2729 2e67 6574 616c 6c28 290a  text').getall().
-000022b0: 5b5d 0a0a 2020 5468 6973 206d 6561 6e73  []..  This means
-000022c0: 2060 602e 6373 7328 2766 6f6f 3a3a 7465   ``.css('foo::te
-000022d0: 7874 2729 2e67 6574 2829 6060 2063 6f75  xt').get()`` cou
-000022e0: 6c64 2072 6574 7572 6e20 4e6f 6e65 2065  ld return None e
-000022f0: 7665 6e20 6966 2061 6e20 656c 656d 656e  ven if an elemen
-00002300: 740a 2020 6578 6973 7473 2e20 5573 6520  t.  exists. Use 
-00002310: 6060 6465 6661 756c 743d 2727 6060 2069  ``default=''`` i
-00002320: 6620 796f 7520 616c 7761 7973 2077 616e  f you always wan
-00002330: 7420 6120 7374 7269 6e67 3a0a 0a3e 3e3e  t a string:..>>>
-00002340: 2072 6573 706f 6e73 652e 6373 7328 2769   response.css('i
-00002350: 6d67 3a3a 7465 7874 2729 2e67 6574 2829  mg::text').get()
-00002360: 0a3e 3e3e 2072 6573 706f 6e73 652e 6373  .>>> response.cs
-00002370: 7328 2769 6d67 3a3a 7465 7874 2729 2e67  s('img::text').g
-00002380: 6574 2864 6566 6175 6c74 3d27 2729 0a27  et(default='').'
-00002390: 270a 0a2a 2060 6061 3a3a 6174 7472 2868  '..* ``a::attr(h
-000023a0: 7265 6629 6060 2073 656c 6563 7473 2074  ref)`` selects t
-000023b0: 6865 202a 6872 6566 2a20 6174 7472 6962  he *href* attrib
-000023c0: 7574 6520 7661 6c75 6520 6f66 2064 6573  ute value of des
-000023d0: 6365 6e64 616e 7420 6c69 6e6b 733a 0a0a  cendant links:..
-000023e0: 3e3e 3e20 7265 7370 6f6e 7365 2e63 7373  >>> response.css
-000023f0: 2827 613a 3a61 7474 7228 6872 6566 2927  ('a::attr(href)'
-00002400: 292e 6765 7461 6c6c 2829 0a5b 2769 6d61  ).getall().['ima
-00002410: 6765 312e 6874 6d6c 272c 0a20 2769 6d61  ge1.html',. 'ima
-00002420: 6765 322e 6874 6d6c 272c 0a20 2769 6d61  ge2.html',. 'ima
-00002430: 6765 332e 6874 6d6c 272c 0a20 2769 6d61  ge3.html',. 'ima
-00002440: 6765 342e 6874 6d6c 272c 0a20 2769 6d61  ge4.html',. 'ima
-00002450: 6765 352e 6874 6d6c 275d 0a0a 2e2e 206e  ge5.html'].... n
-00002460: 6f74 653a 3a0a 2020 2020 5365 6520 616c  ote::.    See al
-00002470: 736f 3a20 3a72 6566 3a60 7365 6c65 6374  so: :ref:`select
-00002480: 696e 672d 6174 7472 6962 7574 6573 602e  ing-attributes`.
-00002490: 0a0a 2e2e 206e 6f74 653a 3a0a 2020 2020  .... note::.    
-000024a0: 596f 7520 6361 6e6e 6f74 2063 6861 696e  You cannot chain
-000024b0: 2074 6865 7365 2070 7365 7564 6f2d 656c   these pseudo-el
-000024c0: 656d 656e 7473 2e20 4275 7420 696e 2070  ements. But in p
-000024d0: 7261 6374 6963 6520 6974 2077 6f75 6c64  ractice it would
-000024e0: 206e 6f74 0a20 2020 206d 616b 6520 6d75   not.    make mu
-000024f0: 6368 2073 656e 7365 3a20 7465 7874 206e  ch sense: text n
-00002500: 6f64 6573 2064 6f20 6e6f 7420 6861 7665  odes do not have
-00002510: 2061 7474 7269 6275 7465 732c 2061 6e64   attributes, and
-00002520: 2061 7474 7269 6275 7465 2076 616c 7565   attribute value
-00002530: 730a 2020 2020 6172 6520 7374 7269 6e67  s.    are string
-00002540: 2076 616c 7565 7320 616c 7265 6164 7920   values already 
-00002550: 616e 6420 646f 206e 6f74 2068 6176 6520  and do not have 
-00002560: 6368 696c 6472 656e 206e 6f64 6573 2e0a  children nodes..
-00002570: 0a2e 2e20 5f43 5353 2053 656c 6563 746f  ... _CSS Selecto
-00002580: 7273 3a20 6874 7470 733a 2f2f 7777 772e  rs: https://www.
-00002590: 7733 2e6f 7267 2f54 522f 7365 6c65 6374  w3.org/TR/select
-000025a0: 6f72 732d 332f 2373 656c 6563 746f 7273  ors-3/#selectors
-000025b0: 0a0a 2e2e 205f 746f 7069 6373 2d73 656c  .... _topics-sel
-000025c0: 6563 746f 7273 2d6e 6573 7469 6e67 2d73  ectors-nesting-s
-000025d0: 656c 6563 746f 7273 3a0a 0a4e 6573 7469  electors:..Nesti
-000025e0: 6e67 2073 656c 6563 746f 7273 0a2d 2d2d  ng selectors.---
-000025f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00002600: 5468 6520 7365 6c65 6374 696f 6e20 6d65  The selection me
-00002610: 7468 6f64 7320 2860 602e 7870 6174 6828  thods (``.xpath(
-00002620: 2960 6020 6f72 2060 602e 6373 7328 2960  )`` or ``.css()`
-00002630: 6029 2072 6574 7572 6e20 6120 6c69 7374  `) return a list
-00002640: 206f 6620 7365 6c65 6374 6f72 730a 6f66   of selectors.of
-00002650: 2074 6865 2073 616d 6520 7479 7065 2c20   the same type, 
-00002660: 736f 2079 6f75 2063 616e 2063 616c 6c20  so you can call 
-00002670: 7468 6520 7365 6c65 6374 696f 6e20 6d65  the selection me
-00002680: 7468 6f64 7320 666f 7220 7468 6f73 6520  thods for those 
-00002690: 7365 6c65 6374 6f72 730a 746f 6f2e 2048  selectors.too. H
-000026a0: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
-000026b0: 3a0a 0a3e 3e3e 206c 696e 6b73 203d 2072  :..>>> links = r
-000026c0: 6573 706f 6e73 652e 7870 6174 6828 272f  esponse.xpath('/
-000026d0: 2f61 5b63 6f6e 7461 696e 7328 4068 7265  /a[contains(@hre
-000026e0: 662c 2022 696d 6167 6522 295d 2729 0a3e  f, "image")]').>
-000026f0: 3e3e 206c 696e 6b73 2e67 6574 616c 6c28  >> links.getall(
-00002700: 290a 5b27 3c61 2068 7265 663d 2269 6d61  ).['<a href="ima
-00002710: 6765 312e 6874 6d6c 223e 4e61 6d65 3a20  ge1.html">Name: 
-00002720: 4d79 2069 6d61 6765 2031 203c 6272 3e3c  My image 1 <br><
-00002730: 696d 6720 7372 633d 2269 6d61 6765 315f  img src="image1_
-00002740: 7468 756d 622e 6a70 6722 3e3c 2f61 3e27  thumb.jpg"></a>'
-00002750: 2c0a 2027 3c61 2068 7265 663d 2269 6d61  ,. '<a href="ima
-00002760: 6765 322e 6874 6d6c 223e 4e61 6d65 3a20  ge2.html">Name: 
-00002770: 4d79 2069 6d61 6765 2032 203c 6272 3e3c  My image 2 <br><
-00002780: 696d 6720 7372 633d 2269 6d61 6765 325f  img src="image2_
-00002790: 7468 756d 622e 6a70 6722 3e3c 2f61 3e27  thumb.jpg"></a>'
-000027a0: 2c0a 2027 3c61 2068 7265 663d 2269 6d61  ,. '<a href="ima
-000027b0: 6765 332e 6874 6d6c 223e 4e61 6d65 3a20  ge3.html">Name: 
-000027c0: 4d79 2069 6d61 6765 2033 203c 6272 3e3c  My image 3 <br><
-000027d0: 696d 6720 7372 633d 2269 6d61 6765 335f  img src="image3_
-000027e0: 7468 756d 622e 6a70 6722 3e3c 2f61 3e27  thumb.jpg"></a>'
-000027f0: 2c0a 2027 3c61 2068 7265 663d 2269 6d61  ,. '<a href="ima
-00002800: 6765 342e 6874 6d6c 223e 4e61 6d65 3a20  ge4.html">Name: 
-00002810: 4d79 2069 6d61 6765 2034 203c 6272 3e3c  My image 4 <br><
-00002820: 696d 6720 7372 633d 2269 6d61 6765 345f  img src="image4_
-00002830: 7468 756d 622e 6a70 6722 3e3c 2f61 3e27  thumb.jpg"></a>'
-00002840: 2c0a 2027 3c61 2068 7265 663d 2269 6d61  ,. '<a href="ima
-00002850: 6765 352e 6874 6d6c 223e 4e61 6d65 3a20  ge5.html">Name: 
-00002860: 4d79 2069 6d61 6765 2035 203c 6272 3e3c  My image 5 <br><
-00002870: 696d 6720 7372 633d 2269 6d61 6765 355f  img src="image5_
-00002880: 7468 756d 622e 6a70 6722 3e3c 2f61 3e27  thumb.jpg"></a>'
-00002890: 5d0a 0a3e 3e3e 2066 6f72 2069 6e64 6578  ]..>>> for index
-000028a0: 2c20 6c69 6e6b 2069 6e20 656e 756d 6572  , link in enumer
-000028b0: 6174 6528 6c69 6e6b 7329 3a0a 2e2e 2e20  ate(links):.... 
-000028c0: 2020 2020 6872 6566 5f78 7061 7468 203d      href_xpath =
-000028d0: 206c 696e 6b2e 7870 6174 6828 2740 6872   link.xpath('@hr
-000028e0: 6566 2729 2e67 6574 2829 0a2e 2e2e 2020  ef').get()....  
-000028f0: 2020 2069 6d67 5f78 7061 7468 203d 206c     img_xpath = l
-00002900: 696e 6b2e 7870 6174 6828 2769 6d67 2f40  ink.xpath('img/@
-00002910: 7372 6327 292e 6765 7428 290a 2e2e 2e20  src').get().... 
-00002920: 2020 2020 7072 696e 7428 6627 4c69 6e6b      print(f'Link
-00002930: 206e 756d 6265 7220 7b69 6e64 6578 7d20   number {index} 
-00002940: 706f 696e 7473 2074 6f20 7572 6c20 7b68  points to url {h
-00002950: 7265 665f 7870 6174 6821 727d 2061 6e64  ref_xpath!r} and
-00002960: 2069 6d61 6765 207b 696d 675f 7870 6174   image {img_xpat
-00002970: 6821 727d 2729 0a4c 696e 6b20 6e75 6d62  h!r}').Link numb
-00002980: 6572 2030 2070 6f69 6e74 7320 746f 2075  er 0 points to u
-00002990: 726c 2027 696d 6167 6531 2e68 746d 6c27  rl 'image1.html'
-000029a0: 2061 6e64 2069 6d61 6765 2027 696d 6167   and image 'imag
-000029b0: 6531 5f74 6875 6d62 2e6a 7067 270a 4c69  e1_thumb.jpg'.Li
-000029c0: 6e6b 206e 756d 6265 7220 3120 706f 696e  nk number 1 poin
-000029d0: 7473 2074 6f20 7572 6c20 2769 6d61 6765  ts to url 'image
-000029e0: 322e 6874 6d6c 2720 616e 6420 696d 6167  2.html' and imag
-000029f0: 6520 2769 6d61 6765 325f 7468 756d 622e  e 'image2_thumb.
-00002a00: 6a70 6727 0a4c 696e 6b20 6e75 6d62 6572  jpg'.Link number
-00002a10: 2032 2070 6f69 6e74 7320 746f 2075 726c   2 points to url
-00002a20: 2027 696d 6167 6533 2e68 746d 6c27 2061   'image3.html' a
-00002a30: 6e64 2069 6d61 6765 2027 696d 6167 6533  nd image 'image3
-00002a40: 5f74 6875 6d62 2e6a 7067 270a 4c69 6e6b  _thumb.jpg'.Link
-00002a50: 206e 756d 6265 7220 3320 706f 696e 7473   number 3 points
-00002a60: 2074 6f20 7572 6c20 2769 6d61 6765 342e   to url 'image4.
-00002a70: 6874 6d6c 2720 616e 6420 696d 6167 6520  html' and image 
-00002a80: 2769 6d61 6765 345f 7468 756d 622e 6a70  'image4_thumb.jp
-00002a90: 6727 0a4c 696e 6b20 6e75 6d62 6572 2034  g'.Link number 4
-00002aa0: 2070 6f69 6e74 7320 746f 2075 726c 2027   points to url '
-00002ab0: 696d 6167 6535 2e68 746d 6c27 2061 6e64  image5.html' and
-00002ac0: 2069 6d61 6765 2027 696d 6167 6535 5f74   image 'image5_t
-00002ad0: 6875 6d62 2e6a 7067 270a 0a2e 2e20 5f73  humb.jpg'.... _s
-00002ae0: 656c 6563 7469 6e67 2d61 7474 7269 6275  electing-attribu
-00002af0: 7465 733a 0a0a 5365 6c65 6374 696e 6720  tes:..Selecting 
-00002b00: 656c 656d 656e 7420 6174 7472 6962 7574  element attribut
-00002b10: 6573 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  es.-------------
-00002b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00002b30: 0a54 6865 7265 2061 7265 2073 6576 6572  .There are sever
-00002b40: 616c 2077 6179 7320 746f 2067 6574 2061  al ways to get a
-00002b50: 2076 616c 7565 206f 6620 616e 2061 7474   value of an att
-00002b60: 7269 6275 7465 2e20 4669 7273 742c 206f  ribute. First, o
-00002b70: 6e65 2063 616e 2075 7365 0a58 5061 7468  ne can use.XPath
-00002b80: 2073 796e 7461 783a 0a0a 3e3e 3e20 7265   syntax:..>>> re
-00002b90: 7370 6f6e 7365 2e78 7061 7468 2822 2f2f  sponse.xpath("//
-00002ba0: 612f 4068 7265 6622 292e 6765 7461 6c6c  a/@href").getall
-00002bb0: 2829 0a5b 2769 6d61 6765 312e 6874 6d6c  ().['image1.html
-00002bc0: 272c 2027 696d 6167 6532 2e68 746d 6c27  ', 'image2.html'
-00002bd0: 2c20 2769 6d61 6765 332e 6874 6d6c 272c  , 'image3.html',
-00002be0: 2027 696d 6167 6534 2e68 746d 6c27 2c20   'image4.html', 
-00002bf0: 2769 6d61 6765 352e 6874 6d6c 275d 0a0a  'image5.html']..
-00002c00: 5850 6174 6820 7379 6e74 6178 2068 6173  XPath syntax has
-00002c10: 2061 2066 6577 2061 6476 616e 7461 6765   a few advantage
-00002c20: 733a 2069 7420 6973 2061 2073 7461 6e64  s: it is a stand
-00002c30: 6172 6420 5850 6174 6820 6665 6174 7572  ard XPath featur
-00002c40: 652c 2061 6e64 0a60 6040 6174 7472 6962  e, and.``@attrib
-00002c50: 7574 6573 6060 2063 616e 2062 6520 7573  utes`` can be us
-00002c60: 6564 2069 6e20 6f74 6865 7220 7061 7274  ed in other part
-00002c70: 7320 6f66 2061 6e20 5850 6174 6820 6578  s of an XPath ex
-00002c80: 7072 6573 7369 6f6e 202d 2065 2e67 2e0a  pression - e.g..
-00002c90: 6974 2069 7320 706f 7373 6962 6c65 2074  it is possible t
-00002ca0: 6f20 6669 6c74 6572 2062 7920 6174 7472  o filter by attr
-00002cb0: 6962 7574 6520 7661 6c75 652e 0a0a 5363  ibute value...Sc
-00002cc0: 7261 7079 2061 6c73 6f20 7072 6f76 6964  rapy also provid
-00002cd0: 6573 2061 6e20 6578 7465 6e73 696f 6e20  es an extension 
-00002ce0: 746f 2043 5353 2073 656c 6563 746f 7273  to CSS selectors
-00002cf0: 2028 6060 3a3a 6174 7472 282e 2e2e 2960   (``::attr(...)`
-00002d00: 6029 0a77 6869 6368 2061 6c6c 6f77 7320  `).which allows 
-00002d10: 746f 2067 6574 2061 7474 7269 6275 7465  to get attribute
-00002d20: 2076 616c 7565 733a 0a0a 3e3e 3e20 7265   values:..>>> re
-00002d30: 7370 6f6e 7365 2e63 7373 2827 613a 3a61  sponse.css('a::a
-00002d40: 7474 7228 6872 6566 2927 292e 6765 7461  ttr(href)').geta
-00002d50: 6c6c 2829 0a5b 2769 6d61 6765 312e 6874  ll().['image1.ht
-00002d60: 6d6c 272c 2027 696d 6167 6532 2e68 746d  ml', 'image2.htm
-00002d70: 6c27 2c20 2769 6d61 6765 332e 6874 6d6c  l', 'image3.html
-00002d80: 272c 2027 696d 6167 6534 2e68 746d 6c27  ', 'image4.html'
-00002d90: 2c20 2769 6d61 6765 352e 6874 6d6c 275d  , 'image5.html']
-00002da0: 0a0a 496e 2061 6464 6974 696f 6e20 746f  ..In addition to
-00002db0: 2074 6861 742c 2074 6865 7265 2069 7320   that, there is 
-00002dc0: 6120 6060 2e61 7474 7269 6260 6020 7072  a ``.attrib`` pr
-00002dd0: 6f70 6572 7479 206f 6620 5365 6c65 6374  operty of Select
-00002de0: 6f72 2e0a 596f 7520 6361 6e20 7573 6520  or..You can use 
-00002df0: 6974 2069 6620 796f 7520 7072 6566 6572  it if you prefer
-00002e00: 2074 6f20 6c6f 6f6b 7570 2061 7474 7269   to lookup attri
-00002e10: 6275 7465 7320 696e 2050 7974 686f 6e0a  butes in Python.
-00002e20: 636f 6465 2c20 7769 7468 6f75 7420 7573  code, without us
-00002e30: 696e 6720 5850 6174 6873 206f 7220 4353  ing XPaths or CS
-00002e40: 5320 6578 7465 6e73 696f 6e73 3a0a 0a3e  S extensions:..>
-00002e50: 3e3e 205b 612e 6174 7472 6962 5b27 6872  >> [a.attrib['hr
-00002e60: 6566 275d 2066 6f72 2061 2069 6e20 7265  ef'] for a in re
-00002e70: 7370 6f6e 7365 2e63 7373 2827 6127 295d  sponse.css('a')]
-00002e80: 0a5b 2769 6d61 6765 312e 6874 6d6c 272c  .['image1.html',
-00002e90: 2027 696d 6167 6532 2e68 746d 6c27 2c20   'image2.html', 
-00002ea0: 2769 6d61 6765 332e 6874 6d6c 272c 2027  'image3.html', '
-00002eb0: 696d 6167 6534 2e68 746d 6c27 2c20 2769  image4.html', 'i
-00002ec0: 6d61 6765 352e 6874 6d6c 275d 0a0a 5468  mage5.html']..Th
-00002ed0: 6973 2070 726f 7065 7274 7920 6973 2061  is property is a
-00002ee0: 6c73 6f20 6176 6169 6c61 626c 6520 6f6e  lso available on
-00002ef0: 2053 656c 6563 746f 724c 6973 743b 2069   SelectorList; i
-00002f00: 7420 7265 7475 726e 7320 6120 6469 6374  t returns a dict
-00002f10: 696f 6e61 7279 0a77 6974 6820 6174 7472  ionary.with attr
-00002f20: 6962 7574 6573 206f 6620 6120 6669 7273  ibutes of a firs
-00002f30: 7420 6d61 7463 6869 6e67 2065 6c65 6d65  t matching eleme
-00002f40: 6e74 2e20 4974 2069 7320 636f 6e76 656e  nt. It is conven
-00002f50: 6965 6e74 2074 6f20 7573 6520 7768 656e  ient to use when
-00002f60: 0a61 2073 656c 6563 746f 7220 6973 2065  .a selector is e
-00002f70: 7870 6563 7465 6420 746f 2067 6976 6520  xpected to give 
-00002f80: 6120 7369 6e67 6c65 2072 6573 756c 7420  a single result 
-00002f90: 2865 2e67 2e20 7768 656e 2073 656c 6563  (e.g. when selec
-00002fa0: 7469 6e67 2062 7920 656c 656d 656e 740a  ting by element.
-00002fb0: 4944 2c20 6f72 2077 6865 6e20 7365 6c65  ID, or when sele
-00002fc0: 6374 696e 6720 616e 2075 6e69 7175 6520  cting an unique 
-00002fd0: 656c 656d 656e 7420 6f6e 2061 2070 6167  element on a pag
-00002fe0: 6529 3a0a 0a3e 3e3e 2072 6573 706f 6e73  e):..>>> respons
-00002ff0: 652e 6373 7328 2762 6173 6527 292e 6174  e.css('base').at
-00003000: 7472 6962 0a7b 2768 7265 6627 3a20 2768  trib.{'href': 'h
-00003010: 7474 703a 2f2f 6578 616d 706c 652e 636f  ttp://example.co
-00003020: 6d2f 277d 0a3e 3e3e 2072 6573 706f 6e73  m/'}.>>> respons
-00003030: 652e 6373 7328 2762 6173 6527 292e 6174  e.css('base').at
-00003040: 7472 6962 5b27 6872 6566 275d 0a27 6874  trib['href'].'ht
-00003050: 7470 3a2f 2f65 7861 6d70 6c65 2e63 6f6d  tp://example.com
-00003060: 2f27 0a0a 6060 2e61 7474 7269 6260 6020  /'..``.attrib`` 
-00003070: 7072 6f70 6572 7479 206f 6620 616e 2065  property of an e
-00003080: 6d70 7479 2053 656c 6563 746f 724c 6973  mpty SelectorLis
-00003090: 7420 6973 2065 6d70 7479 3a0a 0a3e 3e3e  t is empty:..>>>
-000030a0: 2072 6573 706f 6e73 652e 6373 7328 2766   response.css('f
-000030b0: 6f6f 2729 2e61 7474 7269 620a 7b7d 0a0a  oo').attrib.{}..
-000030c0: 5573 696e 6720 7365 6c65 6374 6f72 7320  Using selectors 
-000030d0: 7769 7468 2072 6567 756c 6172 2065 7870  with regular exp
-000030e0: 7265 7373 696f 6e73 0a2d 2d2d 2d2d 2d2d  ressions.-------
-000030f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003110: 2d0a 0a3a 636c 6173 733a 607e 7363 7261  -..:class:`~scra
-00003120: 7079 2e53 656c 6563 746f 7260 2061 6c73  py.Selector` als
-00003130: 6f20 6861 7320 6120 6060 2e72 6528 2960  o has a ``.re()`
-00003140: 6020 6d65 7468 6f64 2066 6f72 2065 7874  ` method for ext
-00003150: 7261 6374 696e 670a 6461 7461 2075 7369  racting.data usi
-00003160: 6e67 2072 6567 756c 6172 2065 7870 7265  ng regular expre
-00003170: 7373 696f 6e73 2e20 486f 7765 7665 722c  ssions. However,
-00003180: 2075 6e6c 696b 6520 7573 696e 6720 6060   unlike using ``
-00003190: 2e78 7061 7468 2829 6060 206f 720a 6060  .xpath()`` or.``
-000031a0: 2e63 7373 2829 6060 206d 6574 686f 6473  .css()`` methods
-000031b0: 2c20 6060 2e72 6528 2960 6020 7265 7475  , ``.re()`` retu
-000031c0: 726e 7320 6120 6c69 7374 206f 6620 7374  rns a list of st
-000031d0: 7269 6e67 732e 2053 6f20 796f 750a 6361  rings. So you.ca
-000031e0: 6e27 7420 636f 6e73 7472 7563 7420 6e65  n't construct ne
-000031f0: 7374 6564 2060 602e 7265 2829 6060 2063  sted ``.re()`` c
-00003200: 616c 6c73 2e0a 0a48 6572 6527 7320 616e  alls...Here's an
-00003210: 2065 7861 6d70 6c65 2075 7365 6420 746f   example used to
-00003220: 2065 7874 7261 6374 2069 6d61 6765 206e   extract image n
-00003230: 616d 6573 2066 726f 6d20 7468 6520 3a72  ames from the :r
-00003240: 6566 3a60 4854 4d4c 2063 6f64 650a 3c74  ef:`HTML code.<t
-00003250: 6f70 6963 732d 7365 6c65 6374 6f72 732d  opics-selectors-
-00003260: 6874 6d6c 636f 6465 3e60 2061 626f 7665  htmlcode>` above
-00003270: 3a0a 0a3e 3e3e 2072 6573 706f 6e73 652e  :..>>> response.
-00003280: 7870 6174 6828 272f 2f61 5b63 6f6e 7461  xpath('//a[conta
-00003290: 696e 7328 4068 7265 662c 2022 696d 6167  ins(@href, "imag
-000032a0: 6522 295d 2f74 6578 7428 2927 292e 7265  e")]/text()').re
-000032b0: 2872 274e 616d 653a 5c73 2a28 2e2a 2927  (r'Name:\s*(.*)'
-000032c0: 290a 5b27 4d79 2069 6d61 6765 2031 272c  ).['My image 1',
-000032d0: 0a20 274d 7920 696d 6167 6520 3227 2c0a  . 'My image 2',.
-000032e0: 2027 4d79 2069 6d61 6765 2033 272c 0a20   'My image 3',. 
-000032f0: 274d 7920 696d 6167 6520 3427 2c0a 2027  'My image 4',. '
-00003300: 4d79 2069 6d61 6765 2035 275d 0a0a 5468  My image 5']..Th
-00003310: 6572 6527 7320 616e 2061 6464 6974 696f  ere's an additio
-00003320: 6e61 6c20 6865 6c70 6572 2072 6563 6970  nal helper recip
-00003330: 726f 6361 7469 6e67 2060 602e 6765 7428  rocating ``.get(
-00003340: 2960 6020 2861 6e64 2069 7473 0a61 6c69  )`` (and its.ali
-00003350: 6173 2060 602e 6578 7472 6163 745f 6669  as ``.extract_fi
-00003360: 7273 7428 2960 6029 2066 6f72 2060 602e  rst()``) for ``.
-00003370: 7265 2829 6060 2c20 6e61 6d65 6420 6060  re()``, named ``
-00003380: 2e72 655f 6669 7273 7428 2960 602e 0a55  .re_first()``..U
-00003390: 7365 2069 7420 746f 2065 7874 7261 6374  se it to extract
-000033a0: 206a 7573 7420 7468 6520 6669 7273 7420   just the first 
-000033b0: 6d61 7463 6869 6e67 2073 7472 696e 673a  matching string:
-000033c0: 0a0a 3e3e 3e20 7265 7370 6f6e 7365 2e78  ..>>> response.x
-000033d0: 7061 7468 2827 2f2f 615b 636f 6e74 6169  path('//a[contai
-000033e0: 6e73 2840 6872 6566 2c20 2269 6d61 6765  ns(@href, "image
-000033f0: 2229 5d2f 7465 7874 2829 2729 2e72 655f  ")]/text()').re_
-00003400: 6669 7273 7428 7227 4e61 6d65 3a5c 732a  first(r'Name:\s*
-00003410: 282e 2a29 2729 0a27 4d79 2069 6d61 6765  (.*)').'My image
-00003420: 2031 270a 0a2e 2e20 5f6f 6c64 2d65 7874   1'.... _old-ext
-00003430: 7261 6374 696f 6e2d 6170 693a 0a0a 6578  raction-api:..ex
-00003440: 7472 6163 7428 2920 616e 6420 6578 7472  tract() and extr
-00003450: 6163 745f 6669 7273 7428 290a 2d2d 2d2d  act_first().----
-00003460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003470: 2d2d 2d2d 2d2d 2d2d 2d0a 0a49 6620 796f  ---------..If yo
-00003480: 7527 7265 2061 206c 6f6e 672d 7469 6d65  u're a long-time
-00003490: 2053 6372 6170 7920 7573 6572 2c20 796f   Scrapy user, yo
-000034a0: 7527 7265 2070 726f 6261 626c 7920 6661  u're probably fa
-000034b0: 6d69 6c69 6172 0a77 6974 6820 6060 2e65  miliar.with ``.e
-000034c0: 7874 7261 6374 2829 6060 2061 6e64 2060  xtract()`` and `
-000034d0: 602e 6578 7472 6163 745f 6669 7273 7428  `.extract_first(
-000034e0: 2960 6020 7365 6c65 6374 6f72 206d 6574  )`` selector met
-000034f0: 686f 6473 2e20 4d61 6e79 2062 6c6f 6720  hods. Many blog 
-00003500: 706f 7374 730a 616e 6420 7475 746f 7269  posts.and tutori
-00003510: 616c 7320 6172 6520 7573 696e 6720 7468  als are using th
-00003520: 656d 2061 7320 7765 6c6c 2e20 5468 6573  em as well. Thes
-00003530: 6520 6d65 7468 6f64 7320 6172 6520 7374  e methods are st
-00003540: 696c 6c20 7375 7070 6f72 7465 640a 6279  ill supported.by
-00003550: 2053 6372 6170 792c 2074 6865 7265 2061   Scrapy, there a
-00003560: 7265 202a 2a6e 6f20 706c 616e 732a 2a20  re **no plans** 
-00003570: 746f 2064 6570 7265 6361 7465 2074 6865  to deprecate the
-00003580: 6d2e 0a0a 486f 7765 7665 722c 2053 6372  m...However, Scr
-00003590: 6170 7920 7573 6167 6520 646f 6373 2061  apy usage docs a
-000035a0: 7265 206e 6f77 2077 7269 7474 656e 2075  re now written u
-000035b0: 7369 6e67 2060 602e 6765 7428 2960 6020  sing ``.get()`` 
-000035c0: 616e 640a 6060 2e67 6574 616c 6c28 2960  and.``.getall()`
-000035d0: 6020 6d65 7468 6f64 732e 2057 6520 6665  ` methods. We fe
-000035e0: 656c 2074 6861 7420 7468 6573 6520 6e65  el that these ne
-000035f0: 7720 6d65 7468 6f64 7320 7265 7375 6c74  w methods result
-00003600: 2069 6e20 6120 6d6f 7265 2063 6f6e 6369   in a more conci
-00003610: 7365 0a61 6e64 2072 6561 6461 626c 6520  se.and readable 
-00003620: 636f 6465 2e0a 0a54 6865 2066 6f6c 6c6f  code...The follo
-00003630: 7769 6e67 2065 7861 6d70 6c65 7320 7368  wing examples sh
-00003640: 6f77 2068 6f77 2074 6865 7365 206d 6574  ow how these met
-00003650: 686f 6473 206d 6170 2074 6f20 6561 6368  hods map to each
-00003660: 206f 7468 6572 2e0a 0a31 2e20 2060 6053   other...1.  ``S
-00003670: 656c 6563 746f 724c 6973 742e 6765 7428  electorList.get(
-00003680: 2960 6020 6973 2074 6865 2073 616d 6520  )`` is the same 
-00003690: 6173 2060 6053 656c 6563 746f 724c 6973  as ``SelectorLis
-000036a0: 742e 6578 7472 6163 745f 6669 7273 7428  t.extract_first(
-000036b0: 2960 603a 0a0a 2020 2020 3e3e 3e20 7265  )``:..    >>> re
-000036c0: 7370 6f6e 7365 2e63 7373 2827 613a 3a61  sponse.css('a::a
-000036d0: 7474 7228 6872 6566 2927 292e 6765 7428  ttr(href)').get(
-000036e0: 290a 2020 2020 2769 6d61 6765 312e 6874  ).    'image1.ht
-000036f0: 6d6c 270a 2020 2020 3e3e 3e20 7265 7370  ml'.    >>> resp
-00003700: 6f6e 7365 2e63 7373 2827 613a 3a61 7474  onse.css('a::att
-00003710: 7228 6872 6566 2927 292e 6578 7472 6163  r(href)').extrac
-00003720: 745f 6669 7273 7428 290a 2020 2020 2769  t_first().    'i
-00003730: 6d61 6765 312e 6874 6d6c 270a 0a32 2e20  mage1.html'..2. 
-00003740: 2060 6053 656c 6563 746f 724c 6973 742e   ``SelectorList.
-00003750: 6765 7461 6c6c 2829 6060 2069 7320 7468  getall()`` is th
-00003760: 6520 7361 6d65 2061 7320 6060 5365 6c65  e same as ``Sele
-00003770: 6374 6f72 4c69 7374 2e65 7874 7261 6374  ctorList.extract
-00003780: 2829 6060 3a0a 0a20 2020 203e 3e3e 2072  ()``:..    >>> r
-00003790: 6573 706f 6e73 652e 6373 7328 2761 3a3a  esponse.css('a::
-000037a0: 6174 7472 2868 7265 6629 2729 2e67 6574  attr(href)').get
-000037b0: 616c 6c28 290a 2020 2020 5b27 696d 6167  all().    ['imag
-000037c0: 6531 2e68 746d 6c27 2c20 2769 6d61 6765  e1.html', 'image
-000037d0: 322e 6874 6d6c 272c 2027 696d 6167 6533  2.html', 'image3
-000037e0: 2e68 746d 6c27 2c20 2769 6d61 6765 342e  .html', 'image4.
-000037f0: 6874 6d6c 272c 2027 696d 6167 6535 2e68  html', 'image5.h
-00003800: 746d 6c27 5d0a 2020 2020 3e3e 3e20 7265  tml'].    >>> re
-00003810: 7370 6f6e 7365 2e63 7373 2827 613a 3a61  sponse.css('a::a
-00003820: 7474 7228 6872 6566 2927 292e 6578 7472  ttr(href)').extr
-00003830: 6163 7428 290a 2020 2020 5b27 696d 6167  act().    ['imag
-00003840: 6531 2e68 746d 6c27 2c20 2769 6d61 6765  e1.html', 'image
-00003850: 322e 6874 6d6c 272c 2027 696d 6167 6533  2.html', 'image3
-00003860: 2e68 746d 6c27 2c20 2769 6d61 6765 342e  .html', 'image4.
-00003870: 6874 6d6c 272c 2027 696d 6167 6535 2e68  html', 'image5.h
-00003880: 746d 6c27 5d0a 0a33 2e20 2060 6053 656c  tml']..3.  ``Sel
-00003890: 6563 746f 722e 6765 7428 2960 6020 6973  ector.get()`` is
-000038a0: 2074 6865 2073 616d 6520 6173 2060 6053   the same as ``S
-000038b0: 656c 6563 746f 722e 6578 7472 6163 7428  elector.extract(
-000038c0: 2960 603a 0a0a 2020 2020 3e3e 3e20 7265  )``:..    >>> re
-000038d0: 7370 6f6e 7365 2e63 7373 2827 613a 3a61  sponse.css('a::a
-000038e0: 7474 7228 6872 6566 2927 295b 305d 2e67  ttr(href)')[0].g
-000038f0: 6574 2829 0a20 2020 2027 696d 6167 6531  et().    'image1
-00003900: 2e68 746d 6c27 0a20 2020 203e 3e3e 2072  .html'.    >>> r
-00003910: 6573 706f 6e73 652e 6373 7328 2761 3a3a  esponse.css('a::
-00003920: 6174 7472 2868 7265 6629 2729 5b30 5d2e  attr(href)')[0].
-00003930: 6578 7472 6163 7428 290a 2020 2020 2769  extract().    'i
-00003940: 6d61 6765 312e 6874 6d6c 270a 0a34 2e20  mage1.html'..4. 
-00003950: 2046 6f72 2063 6f6e 7369 7374 656e 6379   For consistency
-00003960: 2c20 7468 6572 6520 6973 2061 6c73 6f20  , there is also 
-00003970: 6060 5365 6c65 6374 6f72 2e67 6574 616c  ``Selector.getal
-00003980: 6c28 2960 602c 2077 6869 6368 2072 6574  l()``, which ret
-00003990: 7572 6e73 2061 206c 6973 743a 0a0a 2020  urns a list:..  
-000039a0: 2020 3e3e 3e20 7265 7370 6f6e 7365 2e63    >>> response.c
-000039b0: 7373 2827 613a 3a61 7474 7228 6872 6566  ss('a::attr(href
-000039c0: 2927 295b 305d 2e67 6574 616c 6c28 290a  )')[0].getall().
-000039d0: 2020 2020 5b27 696d 6167 6531 2e68 746d      ['image1.htm
-000039e0: 6c27 5d0a 0a53 6f2c 2074 6865 206d 6169  l']..So, the mai
-000039f0: 6e20 6469 6666 6572 656e 6365 2069 7320  n difference is 
-00003a00: 7468 6174 206f 7574 7075 7420 6f66 2060  that output of `
-00003a10: 602e 6765 7428 2960 6020 616e 6420 6060  `.get()`` and ``
-00003a20: 2e67 6574 616c 6c28 2960 6020 6d65 7468  .getall()`` meth
-00003a30: 6f64 730a 6973 206d 6f72 6520 7072 6564  ods.is more pred
-00003a40: 6963 7461 626c 653a 2060 602e 6765 7428  ictable: ``.get(
-00003a50: 2960 6020 616c 7761 7973 2072 6574 7572  )`` always retur
-00003a60: 6e73 2061 2073 696e 676c 6520 7265 7375  ns a single resu
-00003a70: 6c74 2c20 6060 2e67 6574 616c 6c28 2960  lt, ``.getall()`
-00003a80: 600a 616c 7761 7973 2072 6574 7572 6e73  `.always returns
-00003a90: 2061 206c 6973 7420 6f66 2061 6c6c 2065   a list of all e
-00003aa0: 7874 7261 6374 6564 2072 6573 756c 7473  xtracted results
-00003ab0: 2e20 5769 7468 2060 602e 6578 7472 6163  . With ``.extrac
-00003ac0: 7428 2960 6020 6d65 7468 6f64 0a69 7420  t()`` method.it 
-00003ad0: 7761 7320 6e6f 7420 616c 7761 7973 206f  was not always o
-00003ae0: 6276 696f 7573 2069 6620 6120 7265 7375  bvious if a resu
-00003af0: 6c74 2069 7320 6120 6c69 7374 206f 7220  lt is a list or 
-00003b00: 6e6f 743b 2074 6f20 6765 7420 6120 7369  not; to get a si
-00003b10: 6e67 6c65 0a72 6573 756c 7420 6569 7468  ngle.result eith
-00003b20: 6572 2060 602e 6578 7472 6163 7428 2960  er ``.extract()`
-00003b30: 6020 6f72 2060 602e 6578 7472 6163 745f  ` or ``.extract_
-00003b40: 6669 7273 7428 2960 6020 7368 6f75 6c64  first()`` should
-00003b50: 2062 6520 6361 6c6c 6564 2e0a 0a0a 2e2e   be called......
-00003b60: 205f 746f 7069 6373 2d73 656c 6563 746f   _topics-selecto
-00003b70: 7273 2d78 7061 7468 733a 0a0a 576f 726b  rs-xpaths:..Work
-00003b80: 696e 6720 7769 7468 2058 5061 7468 730a  ing with XPaths.
-00003b90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003ba0: 3d3d 3d0a 0a48 6572 6520 6172 6520 736f  ===..Here are so
-00003bb0: 6d65 2074 6970 7320 7768 6963 6820 6d61  me tips which ma
-00003bc0: 7920 6865 6c70 2079 6f75 2074 6f20 7573  y help you to us
-00003bd0: 6520 5850 6174 6820 7769 7468 2053 6372  e XPath with Scr
-00003be0: 6170 7920 7365 6c65 6374 6f72 730a 6566  apy selectors.ef
-00003bf0: 6665 6374 6976 656c 792e 2049 6620 796f  fectively. If yo
-00003c00: 7520 6172 6520 6e6f 7420 6d75 6368 2066  u are not much f
-00003c10: 616d 696c 6961 7220 7769 7468 2058 5061  amiliar with XPa
-00003c20: 7468 2079 6574 2c0a 796f 7520 6d61 7920  th yet,.you may 
-00003c30: 7761 6e74 2074 6f20 7461 6b65 2061 206c  want to take a l
-00003c40: 6f6f 6b20 6669 7273 7420 6174 2074 6869  ook first at thi
-00003c50: 7320 6058 5061 7468 2074 7574 6f72 6961  s `XPath tutoria
-00003c60: 6c60 5f2e 0a0a 2e2e 206e 6f74 653a 3a0a  l`_..... note::.
-00003c70: 2020 2020 536f 6d65 206f 6620 7468 6520      Some of the 
-00003c80: 7469 7073 2061 7265 2062 6173 6564 206f  tips are based o
-00003c90: 6e20 6074 6869 7320 706f 7374 2066 726f  n `this post fro
-00003ca0: 6d20 5a79 7465 2773 2062 6c6f 6760 5f2e  m Zyte's blog`_.
-00003cb0: 0a0a 2e2e 205f 6058 5061 7468 2074 7574  .... _`XPath tut
-00003cc0: 6f72 6961 6c60 3a20 6874 7470 3a2f 2f77  orial`: http://w
-00003cd0: 7777 2e7a 766f 6e2e 6f72 672f 636f 6d70  ww.zvon.org/comp
-00003ce0: 2f72 2f74 7574 2d58 5061 7468 5f31 2e68  /r/tut-XPath_1.h
-00003cf0: 746d 6c0a 2e2e 205f 7468 6973 2070 6f73  tml... _this pos
-00003d00: 7420 6672 6f6d 205a 7974 6527 7320 626c  t from Zyte's bl
-00003d10: 6f67 3a20 6874 7470 733a 2f2f 7777 772e  og: https://www.
-00003d20: 7a79 7465 2e63 6f6d 2f62 6c6f 672f 7870  zyte.com/blog/xp
-00003d30: 6174 682d 7469 7073 2d66 726f 6d2d 7468  ath-tips-from-th
-00003d40: 652d 7765 622d 7363 7261 7069 6e67 2d74  e-web-scraping-t
-00003d50: 7265 6e63 6865 732f 0a0a 0a2e 2e20 5f74  renches/..... _t
-00003d60: 6f70 6963 732d 7365 6c65 6374 6f72 732d  opics-selectors-
-00003d70: 7265 6c61 7469 7665 2d78 7061 7468 733a  relative-xpaths:
-00003d80: 0a0a 576f 726b 696e 6720 7769 7468 2072  ..Working with r
-00003d90: 656c 6174 6976 6520 5850 6174 6873 0a2d  elative XPaths.-
-00003da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a4b 6565  -----------..Kee
-00003dc0: 7020 696e 206d 696e 6420 7468 6174 2069  p in mind that i
-00003dd0: 6620 796f 7520 6172 6520 6e65 7374 696e  f you are nestin
-00003de0: 6720 7365 6c65 6374 6f72 7320 616e 6420  g selectors and 
-00003df0: 7573 6520 616e 2058 5061 7468 2074 6861  use an XPath tha
-00003e00: 7420 7374 6172 7473 0a77 6974 6820 6060  t starts.with ``
-00003e10: 2f60 602c 2074 6861 7420 5850 6174 6820  /``, that XPath 
-00003e20: 7769 6c6c 2062 6520 6162 736f 6c75 7465  will be absolute
-00003e30: 2074 6f20 7468 6520 646f 6375 6d65 6e74   to the document
-00003e40: 2061 6e64 206e 6f74 2072 656c 6174 6976   and not relativ
-00003e50: 6520 746f 2074 6865 0a60 6053 656c 6563  e to the.``Selec
-00003e60: 746f 7260 6020 796f 7527 7265 2063 616c  tor`` you're cal
-00003e70: 6c69 6e67 2069 7420 6672 6f6d 2e0a 0a46  ling it from...F
-00003e80: 6f72 2065 7861 6d70 6c65 2c20 7375 7070  or example, supp
-00003e90: 6f73 6520 796f 7520 7761 6e74 2074 6f20  ose you want to 
-00003ea0: 6578 7472 6163 7420 616c 6c20 6060 3c70  extract all ``<p
-00003eb0: 3e60 6020 656c 656d 656e 7473 2069 6e73  >`` elements ins
-00003ec0: 6964 6520 6060 3c64 6976 3e60 600a 656c  ide ``<div>``.el
-00003ed0: 656d 656e 7473 2e20 4669 7273 742c 2079  ements. First, y
-00003ee0: 6f75 2077 6f75 6c64 2067 6574 2061 6c6c  ou would get all
-00003ef0: 2060 603c 6469 763e 6060 2065 6c65 6d65   ``<div>`` eleme
-00003f00: 6e74 733a 0a0a 3e3e 3e20 6469 7673 203d  nts:..>>> divs =
-00003f10: 2072 6573 706f 6e73 652e 7870 6174 6828   response.xpath(
-00003f20: 272f 2f64 6976 2729 0a0a 4174 2066 6972  '//div')..At fir
-00003f30: 7374 2c20 796f 7520 6d61 7920 6265 2074  st, you may be t
-00003f40: 656d 7074 6564 2074 6f20 7573 6520 7468  empted to use th
-00003f50: 6520 666f 6c6c 6f77 696e 6720 6170 7072  e following appr
-00003f60: 6f61 6368 2c20 7768 6963 6820 6973 2077  oach, which is w
-00003f70: 726f 6e67 2c20 6173 0a69 7420 6163 7475  rong, as.it actu
-00003f80: 616c 6c79 2065 7874 7261 6374 7320 616c  ally extracts al
-00003f90: 6c20 6060 3c70 3e60 6020 656c 656d 656e  l ``<p>`` elemen
-00003fa0: 7473 2066 726f 6d20 7468 6520 646f 6375  ts from the docu
-00003fb0: 6d65 6e74 2c20 6e6f 7420 6f6e 6c79 2074  ment, not only t
-00003fc0: 686f 7365 0a69 6e73 6964 6520 6060 3c64  hose.inside ``<d
-00003fd0: 6976 3e60 6020 656c 656d 656e 7473 3a0a  iv>`` elements:.
-00003fe0: 0a3e 3e3e 2066 6f72 2070 2069 6e20 6469  .>>> for p in di
-00003ff0: 7673 2e78 7061 7468 2827 2f2f 7027 293a  vs.xpath('//p'):
-00004000: 2020 2320 7468 6973 2069 7320 7772 6f6e    # this is wron
-00004010: 6720 2d20 6765 7473 2061 6c6c 203c 703e  g - gets all <p>
-00004020: 2066 726f 6d20 7468 6520 7768 6f6c 6520   from the whole 
-00004030: 646f 6375 6d65 6e74 0a2e 2e2e 2020 2020  document....    
-00004040: 2070 7269 6e74 2870 2e67 6574 2829 290a   print(p.get()).
-00004050: 0a54 6869 7320 6973 2074 6865 2070 726f  .This is the pro
-00004060: 7065 7220 7761 7920 746f 2064 6f20 6974  per way to do it
-00004070: 2028 6e6f 7465 2074 6865 2064 6f74 2070   (note the dot p
-00004080: 7265 6669 7869 6e67 2074 6865 2060 602e  refixing the ``.
-00004090: 2f2f 7060 6020 5850 6174 6829 3a0a 0a3e  //p`` XPath):..>
-000040a0: 3e3e 2066 6f72 2070 2069 6e20 6469 7673  >> for p in divs
-000040b0: 2e78 7061 7468 2827 2e2f 2f70 2729 3a20  .xpath('.//p'): 
-000040c0: 2023 2065 7874 7261 6374 7320 616c 6c20   # extracts all 
-000040d0: 3c70 3e20 696e 7369 6465 0a2e 2e2e 2020  <p> inside....  
-000040e0: 2020 2070 7269 6e74 2870 2e67 6574 2829     print(p.get()
-000040f0: 290a 0a41 6e6f 7468 6572 2063 6f6d 6d6f  )..Another commo
-00004100: 6e20 6361 7365 2077 6f75 6c64 2062 6520  n case would be 
-00004110: 746f 2065 7874 7261 6374 2061 6c6c 2064  to extract all d
-00004120: 6972 6563 7420 6060 3c70 3e60 6020 6368  irect ``<p>`` ch
-00004130: 696c 6472 656e 3a0a 0a3e 3e3e 2066 6f72  ildren:..>>> for
-00004140: 2070 2069 6e20 6469 7673 2e78 7061 7468   p in divs.xpath
-00004150: 2827 7027 293a 0a2e 2e2e 2020 2020 2070  ('p'):....     p
-00004160: 7269 6e74 2870 2e67 6574 2829 290a 0a46  rint(p.get())..F
-00004170: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
-00004180: 6162 6f75 7420 7265 6c61 7469 7665 2058  about relative X
-00004190: 5061 7468 7320 7365 6520 7468 6520 604c  Paths see the `L
-000041a0: 6f63 6174 696f 6e20 5061 7468 7360 5f20  ocation Paths`_ 
-000041b0: 7365 6374 696f 6e20 696e 2074 6865 0a58  section in the.X
-000041c0: 5061 7468 2073 7065 6369 6669 6361 7469  Path specificati
-000041d0: 6f6e 2e0a 0a2e 2e20 5f4c 6f63 6174 696f  on..... _Locatio
-000041e0: 6e20 5061 7468 733a 2068 7474 7073 3a2f  n Paths: https:/
-000041f0: 2f77 7777 2e77 332e 6f72 672f 5452 2f78  /www.w3.org/TR/x
-00004200: 7061 7468 2f61 6c6c 2f23 6c6f 6361 7469  path/all/#locati
-00004210: 6f6e 2d70 6174 6873 0a0a 5768 656e 2071  on-paths..When q
-00004220: 7565 7279 696e 6720 6279 2063 6c61 7373  uerying by class
-00004230: 2c20 636f 6e73 6964 6572 2075 7369 6e67  , consider using
-00004240: 2043 5353 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d   CSS.-----------
-00004250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00004270: 0a42 6563 6175 7365 2061 6e20 656c 656d  .Because an elem
-00004280: 656e 7420 6361 6e20 636f 6e74 6169 6e20  ent can contain 
-00004290: 6d75 6c74 6970 6c65 2043 5353 2063 6c61  multiple CSS cla
-000042a0: 7373 6573 2c20 7468 6520 5850 6174 6820  sses, the XPath 
-000042b0: 7761 7920 746f 2073 656c 6563 7420 656c  way to select el
-000042c0: 656d 656e 7473 0a62 7920 636c 6173 7320  ements.by class 
-000042d0: 6973 2074 6865 2072 6174 6865 7220 7665  is the rather ve
-000042e0: 7262 6f73 653a 3a0a 0a20 2020 202a 5b63  rbose::..    *[c
-000042f0: 6f6e 7461 696e 7328 636f 6e63 6174 2827  ontains(concat('
-00004300: 2027 2c20 6e6f 726d 616c 697a 652d 7370   ', normalize-sp
-00004310: 6163 6528 4063 6c61 7373 292c 2027 2027  ace(@class), ' '
-00004320: 292c 2027 2073 6f6d 6563 6c61 7373 2027  ), ' someclass '
-00004330: 295d 0a0a 4966 2079 6f75 2075 7365 2060  )]..If you use `
-00004340: 6040 636c 6173 733d 2773 6f6d 6563 6c61  `@class='somecla
-00004350: 7373 2760 6020 796f 7520 6d61 7920 656e  ss'`` you may en
-00004360: 6420 7570 206d 6973 7369 6e67 2065 6c65  d up missing ele
-00004370: 6d65 6e74 7320 7468 6174 2068 6176 650a  ments that have.
-00004380: 6f74 6865 7220 636c 6173 7365 732c 2061  other classes, a
-00004390: 6e64 2069 6620 796f 7520 6a75 7374 2075  nd if you just u
-000043a0: 7365 2060 6063 6f6e 7461 696e 7328 4063  se ``contains(@c
-000043b0: 6c61 7373 2c20 2773 6f6d 6563 6c61 7373  lass, 'someclass
-000043c0: 2729 6060 2074 6f20 6d61 6b65 2075 700a  ')`` to make up.
-000043d0: 666f 7220 7468 6174 2079 6f75 206d 6179  for that you may
-000043e0: 2065 6e64 2075 7020 7769 7468 206d 6f72   end up with mor
-000043f0: 6520 656c 656d 656e 7473 2074 6861 7420  e elements that 
-00004400: 796f 7520 7761 6e74 2c20 6966 2074 6865  you want, if the
-00004410: 7920 6861 7665 2061 2064 6966 6665 7265  y have a differe
-00004420: 6e74 0a63 6c61 7373 206e 616d 6520 7468  nt.class name th
-00004430: 6174 2073 6861 7265 7320 7468 6520 7374  at shares the st
-00004440: 7269 6e67 2060 6073 6f6d 6563 6c61 7373  ring ``someclass
-00004450: 6060 2e0a 0a41 7320 6974 2074 7572 6e73  ``...As it turns
-00004460: 206f 7574 2c20 5363 7261 7079 2073 656c   out, Scrapy sel
-00004470: 6563 746f 7273 2061 6c6c 6f77 2079 6f75  ectors allow you
-00004480: 2074 6f20 6368 6169 6e20 7365 6c65 6374   to chain select
-00004490: 6f72 732c 2073 6f20 6d6f 7374 206f 6620  ors, so most of 
-000044a0: 7468 6520 7469 6d65 0a79 6f75 2063 616e  the time.you can
-000044b0: 206a 7573 7420 7365 6c65 6374 2062 7920   just select by 
-000044c0: 636c 6173 7320 7573 696e 6720 4353 5320  class using CSS 
-000044d0: 616e 6420 7468 656e 2073 7769 7463 6820  and then switch 
-000044e0: 746f 2058 5061 7468 2077 6865 6e20 6e65  to XPath when ne
-000044f0: 6564 6564 3a0a 0a3e 3e3e 2066 726f 6d20  eded:..>>> from 
-00004500: 7363 7261 7079 2069 6d70 6f72 7420 5365  scrapy import Se
-00004510: 6c65 6374 6f72 0a3e 3e3e 2073 656c 203d  lector.>>> sel =
-00004520: 2053 656c 6563 746f 7228 7465 7874 3d27   Selector(text='
-00004530: 3c64 6976 2063 6c61 7373 3d22 6865 726f  <div class="hero
-00004540: 2073 686f 7574 223e 3c74 696d 6520 6461   shout"><time da
-00004550: 7465 7469 6d65 3d22 3230 3134 2d30 372d  tetime="2014-07-
-00004560: 3233 2031 393a 3030 223e 5370 6563 6961  23 19:00">Specia
-00004570: 6c20 6461 7465 3c2f 7469 6d65 3e3c 2f64  l date</time></d
-00004580: 6976 3e27 290a 3e3e 3e20 7365 6c2e 6373  iv>').>>> sel.cs
-00004590: 7328 272e 7368 6f75 7427 292e 7870 6174  s('.shout').xpat
-000045a0: 6828 272e 2f74 696d 652f 4064 6174 6574  h('./time/@datet
-000045b0: 696d 6527 292e 6765 7461 6c6c 2829 0a5b  ime').getall().[
-000045c0: 2732 3031 342d 3037 2d32 3320 3139 3a30  '2014-07-23 19:0
-000045d0: 3027 5d0a 0a54 6869 7320 6973 2063 6c65  0']..This is cle
-000045e0: 616e 6572 2074 6861 6e20 7573 696e 6720  aner than using 
-000045f0: 7468 6520 7665 7262 6f73 6520 5850 6174  the verbose XPat
-00004600: 6820 7472 6963 6b20 7368 6f77 6e20 6162  h trick shown ab
-00004610: 6f76 652e 204a 7573 7420 7265 6d65 6d62  ove. Just rememb
-00004620: 6572 0a74 6f20 7573 6520 7468 6520 6060  er.to use the ``
-00004630: 2e60 6020 696e 2074 6865 2058 5061 7468  .`` in the XPath
-00004640: 2065 7870 7265 7373 696f 6e73 2074 6861   expressions tha
-00004650: 7420 7769 6c6c 2066 6f6c 6c6f 772e 0a0a  t will follow...
-00004660: 4265 7761 7265 206f 6620 7468 6520 6469  Beware of the di
-00004670: 6666 6572 656e 6365 2062 6574 7765 656e  fference between
-00004680: 202f 2f6e 6f64 655b 315d 2061 6e64 2028   //node[1] and (
-00004690: 2f2f 6e6f 6465 295b 315d 0a2d 2d2d 2d2d  //node)[1].-----
-000046a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000046b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000046c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000046d0: 2d2d 2d2d 2d0a 0a60 602f 2f6e 6f64 655b  -----..``//node[
-000046e0: 315d 6060 2073 656c 6563 7473 2061 6c6c  1]`` selects all
-000046f0: 2074 6865 206e 6f64 6573 206f 6363 7572   the nodes occur
-00004700: 7269 6e67 2066 6972 7374 2075 6e64 6572  ring first under
-00004710: 2074 6865 6972 2072 6573 7065 6374 6976   their respectiv
-00004720: 6520 7061 7265 6e74 732e 0a0a 6060 282f  e parents...``(/
-00004730: 2f6e 6f64 6529 5b31 5d60 6020 7365 6c65  /node)[1]`` sele
-00004740: 6374 7320 616c 6c20 7468 6520 6e6f 6465  cts all the node
-00004750: 7320 696e 2074 6865 2064 6f63 756d 656e  s in the documen
-00004760: 742c 2061 6e64 2074 6865 6e20 6765 7473  t, and then gets
-00004770: 206f 6e6c 7920 7468 6520 6669 7273 7420   only the first 
-00004780: 6f66 2074 6865 6d2e 0a0a 4578 616d 706c  of them...Exampl
-00004790: 653a 0a0a 3e3e 3e20 6672 6f6d 2073 6372  e:..>>> from scr
-000047a0: 6170 7920 696d 706f 7274 2053 656c 6563  apy import Selec
-000047b0: 746f 720a 3e3e 3e20 7365 6c20 3d20 5365  tor.>>> sel = Se
-000047c0: 6c65 6374 6f72 2874 6578 743d 2222 220a  lector(text=""".
-000047d0: 2e2e 2e2e 3a20 2020 2020 3c75 6c20 636c  ....:     <ul cl
-000047e0: 6173 733d 226c 6973 7422 3e0a 2e2e 2e2e  ass="list">.....
-000047f0: 3a20 2020 2020 2020 2020 3c6c 693e 313c  :         <li>1<
-00004800: 2f6c 693e 0a2e 2e2e 2e3a 2020 2020 2020  /li>.....:      
-00004810: 2020 203c 6c69 3e32 3c2f 6c69 3e0a 2e2e     <li>2</li>...
-00004820: 2e2e 3a20 2020 2020 2020 2020 3c6c 693e  ..:         <li>
-00004830: 333c 2f6c 693e 0a2e 2e2e 2e3a 2020 2020  3</li>.....:    
-00004840: 203c 2f75 6c3e 0a2e 2e2e 2e3a 2020 2020   </ul>.....:    
-00004850: 203c 756c 2063 6c61 7373 3d22 6c69 7374   <ul class="list
-00004860: 223e 0a2e 2e2e 2e3a 2020 2020 2020 2020  ">.....:        
-00004870: 203c 6c69 3e34 3c2f 6c69 3e0a 2e2e 2e2e   <li>4</li>.....
-00004880: 3a20 2020 2020 2020 2020 3c6c 693e 353c  :         <li>5<
-00004890: 2f6c 693e 0a2e 2e2e 2e3a 2020 2020 2020  /li>.....:      
-000048a0: 2020 203c 6c69 3e36 3c2f 6c69 3e0a 2e2e     <li>6</li>...
-000048b0: 2e2e 3a20 2020 2020 3c2f 756c 3e22 2222  ..:     </ul>"""
-000048c0: 290a 3e3e 3e20 7870 203d 206c 616d 6264  ).>>> xp = lambd
-000048d0: 6120 783a 2073 656c 2e78 7061 7468 2878  a x: sel.xpath(x
-000048e0: 292e 6765 7461 6c6c 2829 0a0a 5468 6973  ).getall()..This
-000048f0: 2067 6574 7320 616c 6c20 6669 7273 7420   gets all first 
-00004900: 6060 3c6c 693e 6060 2020 656c 656d 656e  ``<li>``  elemen
-00004910: 7473 2075 6e64 6572 2077 6861 7465 7665  ts under whateve
-00004920: 7220 6974 2069 7320 6974 7320 7061 7265  r it is its pare
-00004930: 6e74 3a0a 0a3e 3e3e 2078 7028 222f 2f6c  nt:..>>> xp("//l
-00004940: 695b 315d 2229 0a5b 273c 6c69 3e31 3c2f  i[1]").['<li>1</
-00004950: 6c69 3e27 2c20 273c 6c69 3e34 3c2f 6c69  li>', '<li>4</li
-00004960: 3e27 5d0a 0a41 6e64 2074 6869 7320 6765  >']..And this ge
-00004970: 7473 2074 6865 2066 6972 7374 2060 603c  ts the first ``<
-00004980: 6c69 3e60 6020 2065 6c65 6d65 6e74 2069  li>``  element i
-00004990: 6e20 7468 6520 7768 6f6c 6520 646f 6375  n the whole docu
-000049a0: 6d65 6e74 3a0a 0a3e 3e3e 2078 7028 2228  ment:..>>> xp("(
-000049b0: 2f2f 6c69 295b 315d 2229 0a5b 273c 6c69  //li)[1]").['<li
-000049c0: 3e31 3c2f 6c69 3e27 5d0a 0a54 6869 7320  >1</li>']..This 
-000049d0: 6765 7473 2061 6c6c 2066 6972 7374 2060  gets all first `
-000049e0: 603c 6c69 3e60 6020 2065 6c65 6d65 6e74  `<li>``  element
-000049f0: 7320 756e 6465 7220 616e 2060 603c 756c  s under an ``<ul
-00004a00: 3e60 6020 2070 6172 656e 743a 0a0a 3e3e  >``  parent:..>>
-00004a10: 3e20 7870 2822 2f2f 756c 2f6c 695b 315d  > xp("//ul/li[1]
-00004a20: 2229 0a5b 273c 6c69 3e31 3c2f 6c69 3e27  ").['<li>1</li>'
-00004a30: 2c20 273c 6c69 3e34 3c2f 6c69 3e27 5d0a  , '<li>4</li>'].
-00004a40: 0a41 6e64 2074 6869 7320 6765 7473 2074  .And this gets t
-00004a50: 6865 2066 6972 7374 2060 603c 6c69 3e60  he first ``<li>`
-00004a60: 6020 2065 6c65 6d65 6e74 2075 6e64 6572  `  element under
-00004a70: 2061 6e20 6060 3c75 6c3e 6060 2020 7061   an ``<ul>``  pa
-00004a80: 7265 6e74 2069 6e20 7468 6520 7768 6f6c  rent in the whol
-00004a90: 6520 646f 6375 6d65 6e74 3a0a 0a3e 3e3e  e document:..>>>
-00004aa0: 2078 7028 2228 2f2f 756c 2f6c 6929 5b31   xp("(//ul/li)[1
-00004ab0: 5d22 290a 5b27 3c6c 693e 313c 2f6c 693e  ]").['<li>1</li>
-00004ac0: 275d 0a0a 5573 696e 6720 7465 7874 206e  ']..Using text n
-00004ad0: 6f64 6573 2069 6e20 6120 636f 6e64 6974  odes in a condit
-00004ae0: 696f 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ion.------------
-00004af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004b00: 2d2d 2d0a 0a57 6865 6e20 796f 7520 6e65  ---..When you ne
-00004b10: 6564 2074 6f20 7573 6520 7468 6520 7465  ed to use the te
-00004b20: 7874 2063 6f6e 7465 6e74 2061 7320 6172  xt content as ar
-00004b30: 6775 6d65 6e74 2074 6f20 616e 2060 5850  gument to an `XP
-00004b40: 6174 6820 7374 7269 6e67 2066 756e 6374  ath string funct
-00004b50: 696f 6e60 5f2c 0a61 766f 6964 2075 7369  ion`_,.avoid usi
-00004b60: 6e67 2060 602e 2f2f 7465 7874 2829 6060  ng ``.//text()``
-00004b70: 2061 6e64 2075 7365 206a 7573 7420 6060   and use just ``
-00004b80: 2e60 6020 696e 7374 6561 642e 0a0a 5468  .`` instead...Th
-00004b90: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
-00004ba0: 6520 6578 7072 6573 7369 6f6e 2060 602e  e expression ``.
-00004bb0: 2f2f 7465 7874 2829 6060 2079 6965 6c64  //text()`` yield
-00004bc0: 7320 6120 636f 6c6c 6563 7469 6f6e 206f  s a collection o
-00004bd0: 6620 7465 7874 2065 6c65 6d65 6e74 7320  f text elements 
-00004be0: 2d2d 2061 202a 6e6f 6465 2d73 6574 2a2e  -- a *node-set*.
-00004bf0: 0a41 6e64 2077 6865 6e20 6120 6e6f 6465  .And when a node
-00004c00: 2d73 6574 2069 7320 636f 6e76 6572 7465  -set is converte
-00004c10: 6420 746f 2061 2073 7472 696e 672c 2077  d to a string, w
-00004c20: 6869 6368 2068 6170 7065 6e73 2077 6865  hich happens whe
-00004c30: 6e20 6974 2069 7320 7061 7373 6564 2061  n it is passed a
-00004c40: 7320 6172 6775 6d65 6e74 2074 6f0a 6120  s argument to.a 
-00004c50: 7374 7269 6e67 2066 756e 6374 696f 6e20  string function 
-00004c60: 6c69 6b65 2060 6063 6f6e 7461 696e 7328  like ``contains(
-00004c70: 2960 6020 6f72 2060 6073 7461 7274 732d  )`` or ``starts-
-00004c80: 7769 7468 2829 6060 2c20 6974 2072 6573  with()``, it res
-00004c90: 756c 7473 2069 6e20 7468 6520 7465 7874  ults in the text
-00004ca0: 2066 6f72 2074 6865 2066 6972 7374 2065   for the first e
-00004cb0: 6c65 6d65 6e74 206f 6e6c 792e 0a0a 4578  lement only...Ex
-00004cc0: 616d 706c 653a 0a0a 3e3e 3e20 6672 6f6d  ample:..>>> from
-00004cd0: 2073 6372 6170 7920 696d 706f 7274 2053   scrapy import S
-00004ce0: 656c 6563 746f 720a 3e3e 3e20 7365 6c20  elector.>>> sel 
-00004cf0: 3d20 5365 6c65 6374 6f72 2874 6578 743d  = Selector(text=
-00004d00: 273c 6120 6872 6566 3d22 2322 3e43 6c69  '<a href="#">Cli
-00004d10: 636b 2068 6572 6520 746f 2067 6f20 746f  ck here to go to
-00004d20: 2074 6865 203c 7374 726f 6e67 3e4e 6578   the <strong>Nex
-00004d30: 7420 5061 6765 3c2f 7374 726f 6e67 3e3c  t Page</strong><
-00004d40: 2f61 3e27 290a 0a43 6f6e 7665 7274 696e  /a>')..Convertin
-00004d50: 6720 6120 2a6e 6f64 652d 7365 742a 2074  g a *node-set* t
-00004d60: 6f20 7374 7269 6e67 3a0a 0a3e 3e3e 2073  o string:..>>> s
-00004d70: 656c 2e78 7061 7468 2827 2f2f 612f 2f74  el.xpath('//a//t
-00004d80: 6578 7428 2927 292e 6765 7461 6c6c 2829  ext()').getall()
-00004d90: 2023 2074 616b 6520 6120 7065 656b 2061   # take a peek a
-00004da0: 7420 7468 6520 6e6f 6465 2d73 6574 0a5b  t the node-set.[
-00004db0: 2743 6c69 636b 2068 6572 6520 746f 2067  'Click here to g
-00004dc0: 6f20 746f 2074 6865 2027 2c20 274e 6578  o to the ', 'Nex
-00004dd0: 7420 5061 6765 275d 0a3e 3e3e 2073 656c  t Page'].>>> sel
-00004de0: 2e78 7061 7468 2822 7374 7269 6e67 282f  .xpath("string(/
-00004df0: 2f61 5b31 5d2f 2f74 6578 7428 2929 2229  /a[1]//text())")
-00004e00: 2e67 6574 616c 6c28 2920 2320 636f 6e76  .getall() # conv
-00004e10: 6572 7420 6974 2074 6f20 7374 7269 6e67  ert it to string
-00004e20: 0a5b 2743 6c69 636b 2068 6572 6520 746f  .['Click here to
-00004e30: 2067 6f20 746f 2074 6865 2027 5d0a 0a41   go to the ']..A
-00004e40: 202a 6e6f 6465 2a20 636f 6e76 6572 7465   *node* converte
-00004e50: 6420 746f 2061 2073 7472 696e 672c 2068  d to a string, h
-00004e60: 6f77 6576 6572 2c20 7075 7473 2074 6f67  owever, puts tog
-00004e70: 6574 6865 7220 7468 6520 7465 7874 206f  ether the text o
-00004e80: 6620 6974 7365 6c66 2070 6c75 7320 6f66  f itself plus of
-00004e90: 2061 6c6c 2069 7473 2064 6573 6365 6e64   all its descend
-00004ea0: 616e 7473 3a0a 0a3e 3e3e 2073 656c 2e78  ants:..>>> sel.x
-00004eb0: 7061 7468 2822 2f2f 615b 315d 2229 2e67  path("//a[1]").g
-00004ec0: 6574 616c 6c28 2920 2320 7365 6c65 6374  etall() # select
-00004ed0: 2074 6865 2066 6972 7374 206e 6f64 650a   the first node.
-00004ee0: 5b27 3c61 2068 7265 663d 2223 223e 436c  ['<a href="#">Cl
-00004ef0: 6963 6b20 6865 7265 2074 6f20 676f 2074  ick here to go t
-00004f00: 6f20 7468 6520 3c73 7472 6f6e 673e 4e65  o the <strong>Ne
-00004f10: 7874 2050 6167 653c 2f73 7472 6f6e 673e  xt Page</strong>
-00004f20: 3c2f 613e 275d 0a3e 3e3e 2073 656c 2e78  </a>'].>>> sel.x
-00004f30: 7061 7468 2822 7374 7269 6e67 282f 2f61  path("string(//a
-00004f40: 5b31 5d29 2229 2e67 6574 616c 6c28 2920  [1])").getall() 
-00004f50: 2320 636f 6e76 6572 7420 6974 2074 6f20  # convert it to 
-00004f60: 7374 7269 6e67 0a5b 2743 6c69 636b 2068  string.['Click h
-00004f70: 6572 6520 746f 2067 6f20 746f 2074 6865  ere to go to the
-00004f80: 204e 6578 7420 5061 6765 275d 0a0a 536f   Next Page']..So
-00004f90: 2c20 7573 696e 6720 7468 6520 6060 2e2f  , using the ``./
-00004fa0: 2f74 6578 7428 2960 6020 6e6f 6465 2d73  /text()`` node-s
-00004fb0: 6574 2077 6f6e 2774 2073 656c 6563 7420  et won't select 
-00004fc0: 616e 7974 6869 6e67 2069 6e20 7468 6973  anything in this
-00004fd0: 2063 6173 653a 0a0a 3e3e 3e20 7365 6c2e   case:..>>> sel.
-00004fe0: 7870 6174 6828 222f 2f61 5b63 6f6e 7461  xpath("//a[conta
-00004ff0: 696e 7328 2e2f 2f74 6578 7428 292c 2027  ins(.//text(), '
-00005000: 4e65 7874 2050 6167 6527 295d 2229 2e67  Next Page')]").g
-00005010: 6574 616c 6c28 290a 5b5d 0a0a 4275 7420  etall().[]..But 
-00005020: 7573 696e 6720 7468 6520 6060 2e60 6020  using the ``.`` 
-00005030: 746f 206d 6561 6e20 7468 6520 6e6f 6465  to mean the node
-00005040: 2c20 776f 726b 733a 0a0a 3e3e 3e20 7365  , works:..>>> se
-00005050: 6c2e 7870 6174 6828 222f 2f61 5b63 6f6e  l.xpath("//a[con
-00005060: 7461 696e 7328 2e2c 2027 4e65 7874 2050  tains(., 'Next P
-00005070: 6167 6527 295d 2229 2e67 6574 616c 6c28  age')]").getall(
-00005080: 290a 5b27 3c61 2068 7265 663d 2223 223e  ).['<a href="#">
-00005090: 436c 6963 6b20 6865 7265 2074 6f20 676f  Click here to go
-000050a0: 2074 6f20 7468 6520 3c73 7472 6f6e 673e   to the <strong>
-000050b0: 4e65 7874 2050 6167 653c 2f73 7472 6f6e  Next Page</stron
-000050c0: 673e 3c2f 613e 275d 0a0a 2e2e 205f 6058  g></a>'].... _`X
-000050d0: 5061 7468 2073 7472 696e 6720 6675 6e63  Path string func
-000050e0: 7469 6f6e 603a 2068 7474 7073 3a2f 2f77  tion`: https://w
-000050f0: 7777 2e77 332e 6f72 672f 5452 2f78 7061  ww.w3.org/TR/xpa
-00005100: 7468 2f61 6c6c 2f23 7365 6374 696f 6e2d  th/all/#section-
-00005110: 5374 7269 6e67 2d46 756e 6374 696f 6e73  String-Functions
-00005120: 0a0a 2e2e 205f 746f 7069 6373 2d73 656c  .... _topics-sel
-00005130: 6563 746f 7273 2d78 7061 7468 2d76 6172  ectors-xpath-var
-00005140: 6961 626c 6573 3a0a 0a56 6172 6961 626c  iables:..Variabl
-00005150: 6573 2069 6e20 5850 6174 6820 6578 7072  es in XPath expr
-00005160: 6573 7369 6f6e 730a 2d2d 2d2d 2d2d 2d2d  essions.--------
-00005170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005180: 2d2d 2d2d 2d2d 0a0a 5850 6174 6820 616c  ------..XPath al
-00005190: 6c6f 7773 2079 6f75 2074 6f20 7265 6665  lows you to refe
-000051a0: 7265 6e63 6520 7661 7269 6162 6c65 7320  rence variables 
-000051b0: 696e 2079 6f75 7220 5850 6174 6820 6578  in your XPath ex
-000051c0: 7072 6573 7369 6f6e 732c 2075 7369 6e67  pressions, using
-000051d0: 0a74 6865 2060 6024 736f 6d65 7661 7269  .the ``$somevari
-000051e0: 6162 6c65 6060 2073 796e 7461 782e 2054  able`` syntax. T
-000051f0: 6869 7320 6973 2073 6f6d 6577 6861 7420  his is somewhat 
-00005200: 7369 6d69 6c61 7220 746f 2070 6172 616d  similar to param
-00005210: 6574 6572 697a 6564 0a71 7565 7269 6573  eterized.queries
-00005220: 206f 7220 7072 6570 6172 6564 2073 7461   or prepared sta
-00005230: 7465 6d65 6e74 7320 696e 2074 6865 2053  tements in the S
-00005240: 514c 2077 6f72 6c64 2077 6865 7265 2079  QL world where y
-00005250: 6f75 2072 6570 6c61 6365 0a73 6f6d 6520  ou replace.some 
-00005260: 6172 6775 6d65 6e74 7320 696e 2079 6f75  arguments in you
-00005270: 7220 7175 6572 6965 7320 7769 7468 2070  r queries with p
-00005280: 6c61 6365 686f 6c64 6572 7320 6c69 6b65  laceholders like
-00005290: 2060 603f 6060 2c0a 7768 6963 6820 6172   ``?``,.which ar
-000052a0: 6520 7468 656e 2073 7562 7374 6974 7574  e then substitut
-000052b0: 6564 2077 6974 6820 7661 6c75 6573 2070  ed with values p
-000052c0: 6173 7365 6420 7769 7468 2074 6865 2071  assed with the q
-000052d0: 7565 7279 2e0a 0a48 6572 6527 7320 616e  uery...Here's an
-000052e0: 2065 7861 6d70 6c65 2074 6f20 6d61 7463   example to matc
-000052f0: 6820 616e 2065 6c65 6d65 6e74 2062 6173  h an element bas
-00005300: 6564 206f 6e20 6974 7320 2269 6422 2061  ed on its "id" a
-00005310: 7474 7269 6275 7465 2076 616c 7565 2c0a  ttribute value,.
-00005320: 7769 7468 6f75 7420 6861 7264 2d63 6f64  without hard-cod
-00005330: 696e 6720 6974 2028 7468 6174 2077 6173  ing it (that was
-00005340: 2073 686f 776e 2070 7265 7669 6f75 736c   shown previousl
-00005350: 7929 3a0a 0a3e 3e3e 2023 2060 2476 616c  y):..>>> # `$val
-00005360: 6020 7573 6564 2069 6e20 7468 6520 6578  ` used in the ex
-00005370: 7072 6573 7369 6f6e 2c20 6120 6076 616c  pression, a `val
-00005380: 6020 6172 6775 6d65 6e74 206e 6565 6473  ` argument needs
-00005390: 2074 6f20 6265 2070 6173 7365 640a 3e3e   to be passed.>>
-000053a0: 3e20 7265 7370 6f6e 7365 2e78 7061 7468  > response.xpath
-000053b0: 2827 2f2f 6469 765b 4069 643d 2476 616c  ('//div[@id=$val
-000053c0: 5d2f 612f 7465 7874 2829 272c 2076 616c  ]/a/text()', val
-000053d0: 3d27 696d 6167 6573 2729 2e67 6574 2829  ='images').get()
-000053e0: 0a27 4e61 6d65 3a20 4d79 2069 6d61 6765  .'Name: My image
-000053f0: 2031 2027 0a0a 4865 7265 2773 2061 6e6f   1 '..Here's ano
-00005400: 7468 6572 2065 7861 6d70 6c65 2c20 746f  ther example, to
-00005410: 2066 696e 6420 7468 6520 2269 6422 2061   find the "id" a
-00005420: 7474 7269 6275 7465 206f 6620 6120 6060  ttribute of a ``
-00005430: 3c64 6976 3e60 6020 7461 6720 636f 6e74  <div>`` tag cont
-00005440: 6169 6e69 6e67 0a66 6976 6520 6060 3c61  aining.five ``<a
-00005450: 3e60 6020 6368 696c 6472 656e 2028 6865  >`` children (he
-00005460: 7265 2077 6520 7061 7373 2074 6865 2076  re we pass the v
-00005470: 616c 7565 2060 6035 6060 2061 7320 616e  alue ``5`` as an
-00005480: 2069 6e74 6567 6572 293a 0a0a 3e3e 3e20   integer):..>>> 
-00005490: 7265 7370 6f6e 7365 2e78 7061 7468 2827  response.xpath('
-000054a0: 2f2f 6469 765b 636f 756e 7428 6129 3d24  //div[count(a)=$
-000054b0: 636e 745d 2f40 6964 272c 2063 6e74 3d35  cnt]/@id', cnt=5
-000054c0: 292e 6765 7428 290a 2769 6d61 6765 7327  ).get().'images'
-000054d0: 0a0a 416c 6c20 7661 7269 6162 6c65 2072  ..All variable r
-000054e0: 6566 6572 656e 6365 7320 6d75 7374 2068  eferences must h
-000054f0: 6176 6520 6120 6269 6e64 696e 6720 7661  ave a binding va
-00005500: 6c75 6520 7768 656e 2063 616c 6c69 6e67  lue when calling
-00005510: 2060 602e 7870 6174 6828 2960 600a 286f   ``.xpath()``.(o
-00005520: 7468 6572 7769 7365 2079 6f75 276c 6c20  therwise you'll 
-00005530: 6765 7420 6120 6060 5661 6c75 6545 7272  get a ``ValueErr
-00005540: 6f72 3a20 5850 6174 6820 6572 726f 723a  or: XPath error:
-00005550: 6060 2065 7863 6570 7469 6f6e 292e 0a54  `` exception)..T
-00005560: 6869 7320 6973 2064 6f6e 6520 6279 2070  his is done by p
-00005570: 6173 7369 6e67 2061 7320 6d61 6e79 206e  assing as many n
-00005580: 616d 6564 2061 7267 756d 656e 7473 2061  amed arguments a
-00005590: 7320 6e65 6365 7373 6172 792e 0a0a 6070  s necessary...`p
-000055a0: 6172 7365 6c60 5f2c 2074 6865 206c 6962  arsel`_, the lib
-000055b0: 7261 7279 2070 6f77 6572 696e 6720 5363  rary powering Sc
-000055c0: 7261 7079 2073 656c 6563 746f 7273 2c20  rapy selectors, 
-000055d0: 6861 7320 6d6f 7265 2064 6574 6169 6c73  has more details
-000055e0: 2061 6e64 2065 7861 6d70 6c65 730a 6f6e   and examples.on
-000055f0: 2060 5850 6174 6820 7661 7269 6162 6c65   `XPath variable
-00005600: 7360 5f2e 0a0a 2e2e 205f 5850 6174 6820  s`_..... _XPath 
-00005610: 7661 7269 6162 6c65 733a 2068 7474 7073  variables: https
-00005620: 3a2f 2f70 6172 7365 6c2e 7265 6164 7468  ://parsel.readth
-00005630: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00005640: 7374 2f75 7361 6765 2e68 746d 6c23 7661  st/usage.html#va
-00005650: 7269 6162 6c65 732d 696e 2d78 7061 7468  riables-in-xpath
-00005660: 2d65 7870 7265 7373 696f 6e73 0a0a 0a2e  -expressions....
-00005670: 2e20 5f72 656d 6f76 696e 672d 6e61 6d65  . _removing-name
-00005680: 7370 6163 6573 3a0a 0a52 656d 6f76 696e  spaces:..Removin
-00005690: 6720 6e61 6d65 7370 6163 6573 0a2d 2d2d  g namespaces.---
-000056a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000056b0: 0a0a 5768 656e 2064 6561 6c69 6e67 2077  ..When dealing w
-000056c0: 6974 6820 7363 7261 7069 6e67 2070 726f  ith scraping pro
-000056d0: 6a65 6374 732c 2069 7420 6973 206f 6674  jects, it is oft
-000056e0: 656e 2071 7569 7465 2063 6f6e 7665 6e69  en quite conveni
-000056f0: 656e 7420 746f 2067 6574 2072 6964 206f  ent to get rid o
-00005700: 660a 6e61 6d65 7370 6163 6573 2061 6c74  f.namespaces alt
-00005710: 6f67 6574 6865 7220 616e 6420 6a75 7374  ogether and just
-00005720: 2077 6f72 6b20 7769 7468 2065 6c65 6d65   work with eleme
-00005730: 6e74 206e 616d 6573 2c20 746f 2077 7269  nt names, to wri
-00005740: 7465 206d 6f72 650a 7369 6d70 6c65 2f63  te more.simple/c
-00005750: 6f6e 7665 6e69 656e 7420 5850 6174 6873  onvenient XPaths
-00005760: 2e20 596f 7520 6361 6e20 7573 6520 7468  . You can use th
-00005770: 650a 3a6d 6574 683a 6053 656c 6563 746f  e.:meth:`Selecto
-00005780: 722e 7265 6d6f 7665 5f6e 616d 6573 7061  r.remove_namespa
-00005790: 6365 7360 206d 6574 686f 6420 666f 7220  ces` method for 
-000057a0: 7468 6174 2e0a 0a4c 6574 2773 2073 686f  that...Let's sho
-000057b0: 7720 616e 2065 7861 6d70 6c65 2074 6861  w an example tha
-000057c0: 7420 696c 6c75 7374 7261 7465 7320 7468  t illustrates th
-000057d0: 6973 2077 6974 6820 7468 6520 5079 7468  is with the Pyth
-000057e0: 6f6e 2049 6e73 6964 6572 2062 6c6f 6720  on Insider blog 
-000057f0: 6174 6f6d 2066 6565 642e 0a0a 2e2e 2068  atom feed..... h
-00005800: 6967 686c 6967 6874 3a3a 2073 680a 0a46  ighlight:: sh..F
-00005810: 6972 7374 2c20 7765 206f 7065 6e20 7468  irst, we open th
-00005820: 6520 7368 656c 6c20 7769 7468 2074 6865  e shell with the
-00005830: 2075 726c 2077 6520 7761 6e74 2074 6f20   url we want to 
-00005840: 7363 7261 7065 3a3a 0a0a 2020 2020 2420  scrape::..    $ 
-00005850: 7363 7261 7079 2073 6865 6c6c 2068 7474  scrapy shell htt
-00005860: 7073 3a2f 2f66 6565 6473 2e66 6565 6462  ps://feeds.feedb
-00005870: 7572 6e65 722e 636f 6d2f 5079 7468 6f6e  urner.com/Python
-00005880: 496e 7369 6465 720a 0a54 6869 7320 6973  Insider..This is
-00005890: 2068 6f77 2074 6865 2066 696c 6520 7374   how the file st
-000058a0: 6172 7473 3a3a 0a0a 2020 2020 3c3f 786d  arts::..    <?xm
-000058b0: 6c20 7665 7273 696f 6e3d 2231 2e30 2220  l version="1.0" 
-000058c0: 656e 636f 6469 6e67 3d22 5554 462d 3822  encoding="UTF-8"
-000058d0: 3f3e 0a20 2020 203c 3f78 6d6c 2d73 7479  ?>.    <?xml-sty
-000058e0: 6c65 7368 6565 7420 2e2e 2e0a 2020 2020  lesheet ....    
-000058f0: 3c66 6565 6420 786d 6c6e 733d 2268 7474  <feed xmlns="htt
-00005900: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
-00005910: 3030 352f 4174 6f6d 220a 2020 2020 2020  005/Atom".      
-00005920: 2020 2020 786d 6c6e 733a 6f70 656e 5365      xmlns:openSe
-00005930: 6172 6368 3d22 6874 7470 3a2f 2f61 392e  arch="http://a9.
-00005940: 636f 6d2f 2d2f 7370 6563 2f6f 7065 6e73  com/-/spec/opens
-00005950: 6561 7263 6872 7373 2f31 2e30 2f22 0a20  earchrss/1.0/". 
-00005960: 2020 2020 2020 2020 2078 6d6c 6e73 3a62           xmlns:b
-00005970: 6c6f 6767 6572 3d22 6874 7470 3a2f 2f73  logger="http://s
-00005980: 6368 656d 6173 2e67 6f6f 676c 652e 636f  chemas.google.co
-00005990: 6d2f 626c 6f67 6765 722f 3230 3038 220a  m/blogger/2008".
-000059a0: 2020 2020 2020 2020 2020 786d 6c6e 733a            xmlns:
-000059b0: 6765 6f72 7373 3d22 6874 7470 3a2f 2f77  georss="http://w
-000059c0: 7777 2e67 656f 7273 732e 6f72 672f 6765  ww.georss.org/ge
-000059d0: 6f72 7373 220a 2020 2020 2020 2020 2020  orss".          
-000059e0: 786d 6c6e 733a 6764 3d22 6874 7470 3a2f  xmlns:gd="http:/
-000059f0: 2f73 6368 656d 6173 2e67 6f6f 676c 652e  /schemas.google.
-00005a00: 636f 6d2f 672f 3230 3035 220a 2020 2020  com/g/2005".    
-00005a10: 2020 2020 2020 786d 6c6e 733a 7468 723d        xmlns:thr=
-00005a20: 2268 7474 703a 2f2f 7075 726c 2e6f 7267  "http://purl.org
-00005a30: 2f73 796e 6469 6361 7469 6f6e 2f74 6872  /syndication/thr
-00005a40: 6561 642f 312e 3022 0a20 2020 2020 2020  ead/1.0".       
-00005a50: 2020 2078 6d6c 6e73 3a66 6565 6462 7572     xmlns:feedbur
-00005a60: 6e65 723d 2268 7474 703a 2f2f 7273 736e  ner="http://rssn
-00005a70: 616d 6573 7061 6365 2e6f 7267 2f66 6565  amespace.org/fee
-00005a80: 6462 7572 6e65 722f 6578 742f 312e 3022  dburner/ext/1.0"
-00005a90: 3e0a 2020 2020 2020 2e2e 2e0a 0a59 6f75  >.      .....You
-00005aa0: 2063 616e 2073 6565 2073 6576 6572 616c   can see several
-00005ab0: 206e 616d 6573 7061 6365 2064 6563 6c61   namespace decla
-00005ac0: 7261 7469 6f6e 7320 696e 636c 7564 696e  rations includin
-00005ad0: 6720 6120 6465 6661 756c 740a 2268 7474  g a default."htt
-00005ae0: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
-00005af0: 3030 352f 4174 6f6d 2220 616e 6420 616e  005/Atom" and an
-00005b00: 6f74 6865 7220 6f6e 6520 7573 696e 6720  other one using 
-00005b10: 7468 6520 2267 643a 2220 7072 6566 6978  the "gd:" prefix
-00005b20: 2066 6f72 0a22 6874 7470 3a2f 2f73 6368   for."http://sch
-00005b30: 656d 6173 2e67 6f6f 676c 652e 636f 6d2f  emas.google.com/
-00005b40: 672f 3230 3035 222e 0a0a 2e2e 2068 6967  g/2005"..... hig
-00005b50: 686c 6967 6874 3a3a 2070 7974 686f 6e0a  hlight:: python.
-00005b60: 0a4f 6e63 6520 696e 2074 6865 2073 6865  .Once in the she
-00005b70: 6c6c 2077 6520 6361 6e20 7472 7920 7365  ll we can try se
-00005b80: 6c65 6374 696e 6720 616c 6c20 6060 3c6c  lecting all ``<l
-00005b90: 696e 6b3e 6060 206f 626a 6563 7473 2061  ink>`` objects a
-00005ba0: 6e64 2073 6565 2074 6861 7420 6974 0a64  nd see that it.d
-00005bb0: 6f65 736e 2774 2077 6f72 6b20 2862 6563  oesn't work (bec
-00005bc0: 6175 7365 2074 6865 2041 746f 6d20 584d  ause the Atom XM
-00005bd0: 4c20 6e61 6d65 7370 6163 6520 6973 206f  L namespace is o
-00005be0: 6266 7573 6361 7469 6e67 2074 686f 7365  bfuscating those
-00005bf0: 206e 6f64 6573 293a 0a0a 3e3e 3e20 7265   nodes):..>>> re
-00005c00: 7370 6f6e 7365 2e78 7061 7468 2822 2f2f  sponse.xpath("//
-00005c10: 6c69 6e6b 2229 0a5b 5d0a 0a42 7574 206f  link").[]..But o
-00005c20: 6e63 6520 7765 2063 616c 6c20 7468 6520  nce we call the 
-00005c30: 3a6d 6574 683a 6053 656c 6563 746f 722e  :meth:`Selector.
-00005c40: 7265 6d6f 7665 5f6e 616d 6573 7061 6365  remove_namespace
-00005c50: 7360 206d 6574 686f 642c 2061 6c6c 0a6e  s` method, all.n
-00005c60: 6f64 6573 2063 616e 2062 6520 6163 6365  odes can be acce
-00005c70: 7373 6564 2064 6972 6563 746c 7920 6279  ssed directly by
-00005c80: 2074 6865 6972 206e 616d 6573 3a0a 0a3e   their names:..>
-00005c90: 3e3e 2072 6573 706f 6e73 652e 7365 6c65  >> response.sele
-00005ca0: 6374 6f72 2e72 656d 6f76 655f 6e61 6d65  ctor.remove_name
-00005cb0: 7370 6163 6573 2829 0a3e 3e3e 2072 6573  spaces().>>> res
-00005cc0: 706f 6e73 652e 7870 6174 6828 222f 2f6c  ponse.xpath("//l
-00005cd0: 696e 6b22 290a 5b3c 5365 6c65 6374 6f72  ink").[<Selector
-00005ce0: 2078 7061 7468 3d27 2f2f 6c69 6e6b 2720   xpath='//link' 
-00005cf0: 6461 7461 3d27 3c6c 696e 6b20 7265 6c3d  data='<link rel=
-00005d00: 2261 6c74 6572 6e61 7465 2220 7479 7065  "alternate" type
-00005d10: 3d22 7465 7874 2f68 746d 6c22 2068 273e  ="text/html" h'>
-00005d20: 2c0a 2020 2020 3c53 656c 6563 746f 7220  ,.    <Selector 
-00005d30: 7870 6174 683d 272f 2f6c 696e 6b27 2064  xpath='//link' d
-00005d40: 6174 613d 273c 6c69 6e6b 2072 656c 3d22  ata='<link rel="
-00005d50: 6e65 7874 2220 7479 7065 3d22 6170 706c  next" type="appl
-00005d60: 6963 6174 696f 6e2f 6174 6f6d 2b27 3e2c  ication/atom+'>,
-00005d70: 0a20 2020 202e 2e2e 0a0a 4966 2079 6f75  .    .....If you
-00005d80: 2077 6f6e 6465 7220 7768 7920 7468 6520   wonder why the 
-00005d90: 6e61 6d65 7370 6163 6520 7265 6d6f 7661  namespace remova
-00005da0: 6c20 7072 6f63 6564 7572 6520 6973 6e27  l procedure isn'
-00005db0: 7420 616c 7761 7973 2063 616c 6c65 6420  t always called 
-00005dc0: 6279 2064 6566 6175 6c74 0a69 6e73 7465  by default.inste
-00005dd0: 6164 206f 6620 6861 7669 6e67 2074 6f20  ad of having to 
-00005de0: 6361 6c6c 2069 7420 6d61 6e75 616c 6c79  call it manually
-00005df0: 2c20 7468 6973 2069 7320 6265 6361 7573  , this is becaus
-00005e00: 6520 6f66 2074 776f 2072 6561 736f 6e73  e of two reasons
-00005e10: 2c20 7768 6963 682c 2069 6e20 6f72 6465  , which, in orde
-00005e20: 720a 6f66 2072 656c 6576 616e 6365 2c20  r.of relevance, 
-00005e30: 6172 653a 0a0a 312e 2052 656d 6f76 696e  are:..1. Removin
-00005e40: 6720 6e61 6d65 7370 6163 6573 2072 6571  g namespaces req
-00005e50: 7569 7265 7320 746f 2069 7465 7261 7465  uires to iterate
-00005e60: 2061 6e64 206d 6f64 6966 7920 616c 6c20   and modify all 
-00005e70: 6e6f 6465 7320 696e 2074 6865 0a20 2020  nodes in the.   
-00005e80: 646f 6375 6d65 6e74 2c20 7768 6963 6820  document, which 
-00005e90: 6973 2061 2072 6561 736f 6e61 626c 7920  is a reasonably 
-00005ea0: 6578 7065 6e73 6976 6520 6f70 6572 6174  expensive operat
-00005eb0: 696f 6e20 746f 2070 6572 666f 726d 2062  ion to perform b
-00005ec0: 7920 6465 6661 756c 740a 2020 2066 6f72  y default.   for
-00005ed0: 2061 6c6c 2064 6f63 756d 656e 7473 2063   all documents c
-00005ee0: 7261 776c 6564 2062 7920 5363 7261 7079  rawled by Scrapy
-00005ef0: 0a0a 322e 2054 6865 7265 2063 6f75 6c64  ..2. There could
-00005f00: 2062 6520 736f 6d65 2063 6173 6573 2077   be some cases w
-00005f10: 6865 7265 2075 7369 6e67 206e 616d 6573  here using names
-00005f20: 7061 6365 7320 6973 2061 6374 7561 6c6c  paces is actuall
-00005f30: 7920 7265 7175 6972 6564 2c20 696e 0a20  y required, in. 
-00005f40: 2020 6361 7365 2073 6f6d 6520 656c 656d    case some elem
-00005f50: 656e 7420 6e61 6d65 7320 636c 6173 6820  ent names clash 
-00005f60: 6265 7477 6565 6e20 6e61 6d65 7370 6163  between namespac
-00005f70: 6573 2e20 5468 6573 6520 6361 7365 7320  es. These cases 
-00005f80: 6172 6520 7665 7279 2072 6172 650a 2020  are very rare.  
-00005f90: 2074 686f 7567 682e 0a0a 0a55 7369 6e67   though....Using
-00005fa0: 2045 5853 4c54 2065 7874 656e 7369 6f6e   EXSLT extension
-00005fb0: 730a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s.--------------
-00005fc0: 2d2d 2d2d 2d2d 2d2d 0a0a 4265 696e 6720  --------..Being 
-00005fd0: 6275 696c 7420 6174 6f70 2060 6c78 6d6c  built atop `lxml
-00005fe0: 605f 2c20 5363 7261 7079 2073 656c 6563  `_, Scrapy selec
-00005ff0: 746f 7273 2073 7570 706f 7274 2073 6f6d  tors support som
-00006000: 6520 6045 5853 4c54 605f 2065 7874 656e  e `EXSLT`_ exten
-00006010: 7369 6f6e 730a 616e 6420 636f 6d65 2077  sions.and come w
-00006020: 6974 6820 7468 6573 6520 7072 652d 7265  ith these pre-re
-00006030: 6769 7374 6572 6564 206e 616d 6573 7061  gistered namespa
-00006040: 6365 7320 746f 2075 7365 2069 6e20 5850  ces to use in XP
-00006050: 6174 6820 6578 7072 6573 7369 6f6e 733a  ath expressions:
-00006060: 0a0a 0a3d 3d3d 3d3d 3d20 203d 3d3d 3d3d  ...======  =====
-00006070: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006090: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d      ============
-000060a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 7072 6566  ===========.pref
-000060b0: 6978 2020 6e61 6d65 7370 6163 6520 2020  ix  namespace   
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 2020 2020 2020 2020 2020 2020 2075 7361               usa
-000060e0: 6765 0a3d 3d3d 3d3d 3d20 203d 3d3d 3d3d  ge.======  =====
-000060f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006110: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d      ============
-00006120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 7265 2020  ===========.re  
-00006130: 2020 2020 5c68 7474 703a 2f2f 6578 736c      \http://exsl
-00006140: 742e 6f72 672f 7265 6775 6c61 722d 6578  t.org/regular-ex
-00006150: 7072 6573 7369 6f6e 7320 2020 2060 7265  pressions    `re
-00006160: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
-00006170: 7360 5f0a 7365 7420 2020 2020 5c68 7474  s`_.set     \htt
-00006180: 703a 2f2f 6578 736c 742e 6f72 672f 7365  p://exslt.org/se
-00006190: 7473 2020 2020 2020 2020 2020 2020 2020  ts              
-000061a0: 2020 2020 2060 7365 7420 6d61 6e69 7075       `set manipu
-000061b0: 6c61 7469 6f6e 605f 0a3d 3d3d 3d3d 3d20  lation`_.====== 
-000061c0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-000061d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000061e0: 3d3d 3d3d 3d3d 2020 2020 3d3d 3d3d 3d3d  ======    ======
-000061f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00006200: 3d0a 0a52 6567 756c 6172 2065 7870 7265  =..Regular expre
-00006210: 7373 696f 6e73 0a7e 7e7e 7e7e 7e7e 7e7e  ssions.~~~~~~~~~
-00006220: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 5468 6520  ~~~~~~~~~~..The 
-00006230: 6060 7465 7374 2829 6060 2066 756e 6374  ``test()`` funct
-00006240: 696f 6e2c 2066 6f72 2065 7861 6d70 6c65  ion, for example
-00006250: 2c20 6361 6e20 7072 6f76 6520 7175 6974  , can prove quit
-00006260: 6520 7573 6566 756c 2077 6865 6e20 5850  e useful when XP
-00006270: 6174 6827 730a 6060 7374 6172 7473 2d77  ath's.``starts-w
-00006280: 6974 6828 2960 6020 6f72 2060 6063 6f6e  ith()`` or ``con
-00006290: 7461 696e 7328 2960 6020 6172 6520 6e6f  tains()`` are no
-000062a0: 7420 7375 6666 6963 6965 6e74 2e0a 0a45  t sufficient...E
-000062b0: 7861 6d70 6c65 2073 656c 6563 7469 6e67  xample selecting
-000062c0: 206c 696e 6b73 2069 6e20 6c69 7374 2069   links in list i
-000062d0: 7465 6d20 7769 7468 2061 2022 636c 6173  tem with a "clas
-000062e0: 7322 2061 7474 7269 6275 7465 2065 6e64  s" attribute end
-000062f0: 696e 6720 7769 7468 2061 2064 6967 6974  ing with a digit
-00006300: 3a0a 0a3e 3e3e 2066 726f 6d20 7363 7261  :..>>> from scra
-00006310: 7079 2069 6d70 6f72 7420 5365 6c65 6374  py import Select
-00006320: 6f72 0a3e 3e3e 2064 6f63 203d 2022 2222  or.>>> doc = """
-00006330: 0a2e 2e2e 203c 6469 763e 0a2e 2e2e 2020  .... <div>....  
-00006340: 2020 203c 756c 3e0a 2e2e 2e20 2020 2020     <ul>....     
-00006350: 2020 2020 3c6c 6920 636c 6173 733d 2269      <li class="i
-00006360: 7465 6d2d 3022 3e3c 6120 6872 6566 3d22  tem-0"><a href="
-00006370: 6c69 6e6b 312e 6874 6d6c 223e 6669 7273  link1.html">firs
-00006380: 7420 6974 656d 3c2f 613e 3c2f 6c69 3e0a  t item</a></li>.
-00006390: 2e2e 2e20 2020 2020 2020 2020 3c6c 6920  ...         <li 
-000063a0: 636c 6173 733d 2269 7465 6d2d 3122 3e3c  class="item-1"><
-000063b0: 6120 6872 6566 3d22 6c69 6e6b 322e 6874  a href="link2.ht
-000063c0: 6d6c 223e 7365 636f 6e64 2069 7465 6d3c  ml">second item<
-000063d0: 2f61 3e3c 2f6c 693e 0a2e 2e2e 2020 2020  /a></li>....    
-000063e0: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
-000063f0: 6974 656d 2d69 6e61 6374 6976 6522 3e3c  item-inactive"><
-00006400: 6120 6872 6566 3d22 6c69 6e6b 332e 6874  a href="link3.ht
-00006410: 6d6c 223e 7468 6972 6420 6974 656d 3c2f  ml">third item</
-00006420: 613e 3c2f 6c69 3e0a 2e2e 2e20 2020 2020  a></li>....     
-00006430: 2020 2020 3c6c 6920 636c 6173 733d 2269      <li class="i
-00006440: 7465 6d2d 3122 3e3c 6120 6872 6566 3d22  tem-1"><a href="
-00006450: 6c69 6e6b 342e 6874 6d6c 223e 666f 7572  link4.html">four
-00006460: 7468 2069 7465 6d3c 2f61 3e3c 2f6c 693e  th item</a></li>
-00006470: 0a2e 2e2e 2020 2020 2020 2020 203c 6c69  ....         <li
-00006480: 2063 6c61 7373 3d22 6974 656d 2d30 223e   class="item-0">
-00006490: 3c61 2068 7265 663d 226c 696e 6b35 2e68  <a href="link5.h
-000064a0: 746d 6c22 3e66 6966 7468 2069 7465 6d3c  tml">fifth item<
-000064b0: 2f61 3e3c 2f6c 693e 0a2e 2e2e 2020 2020  /a></li>....    
-000064c0: 203c 2f75 6c3e 0a2e 2e2e 203c 2f64 6976   </ul>.... </div
-000064d0: 3e0a 2e2e 2e20 2222 220a 3e3e 3e20 7365  >.... """.>>> se
-000064e0: 6c20 3d20 5365 6c65 6374 6f72 2874 6578  l = Selector(tex
-000064f0: 743d 646f 632c 2074 7970 653d 2268 746d  t=doc, type="htm
-00006500: 6c22 290a 3e3e 3e20 7365 6c2e 7870 6174  l").>>> sel.xpat
-00006510: 6828 272f 2f6c 692f 2f40 6872 6566 2729  h('//li//@href')
-00006520: 2e67 6574 616c 6c28 290a 5b27 6c69 6e6b  .getall().['link
-00006530: 312e 6874 6d6c 272c 2027 6c69 6e6b 322e  1.html', 'link2.
-00006540: 6874 6d6c 272c 2027 6c69 6e6b 332e 6874  html', 'link3.ht
-00006550: 6d6c 272c 2027 6c69 6e6b 342e 6874 6d6c  ml', 'link4.html
-00006560: 272c 2027 6c69 6e6b 352e 6874 6d6c 275d  ', 'link5.html']
-00006570: 0a3e 3e3e 2073 656c 2e78 7061 7468 2827  .>>> sel.xpath('
-00006580: 2f2f 6c69 5b72 653a 7465 7374 2840 636c  //li[re:test(@cl
-00006590: 6173 732c 2022 6974 656d 2d5c 6424 2229  ass, "item-\d$")
-000065a0: 5d2f 2f40 6872 6566 2729 2e67 6574 616c  ]//@href').getal
-000065b0: 6c28 290a 5b27 6c69 6e6b 312e 6874 6d6c  l().['link1.html
-000065c0: 272c 2027 6c69 6e6b 322e 6874 6d6c 272c  ', 'link2.html',
-000065d0: 2027 6c69 6e6b 342e 6874 6d6c 272c 2027   'link4.html', '
-000065e0: 6c69 6e6b 352e 6874 6d6c 275d 0a0a 2e2e  link5.html']....
-000065f0: 2077 6172 6e69 6e67 3a3a 2043 206c 6962   warning:: C lib
-00006600: 7261 7279 2060 606c 6962 7873 6c74 6060  rary ``libxslt``
-00006610: 2064 6f65 736e 2774 206e 6174 6976 656c   doesn't nativel
-00006620: 7920 7375 7070 6f72 7420 4558 534c 5420  y support EXSLT 
-00006630: 7265 6775 6c61 720a 2020 2020 6578 7072  regular.    expr
-00006640: 6573 7369 6f6e 7320 736f 2060 6c78 6d6c  essions so `lxml
-00006650: 605f 2773 2069 6d70 6c65 6d65 6e74 6174  `_'s implementat
-00006660: 696f 6e20 7573 6573 2068 6f6f 6b73 2074  ion uses hooks t
-00006670: 6f20 5079 7468 6f6e 2773 2060 6072 6560  o Python's ``re`
-00006680: 6020 6d6f 6475 6c65 2e0a 2020 2020 5468  ` module..    Th
-00006690: 7573 2c20 7573 696e 6720 7265 6765 7870  us, using regexp
-000066a0: 2066 756e 6374 696f 6e73 2069 6e20 796f   functions in yo
-000066b0: 7572 2058 5061 7468 2065 7870 7265 7373  ur XPath express
-000066c0: 696f 6e73 206d 6179 2061 6464 2061 2073  ions may add a s
-000066d0: 6d61 6c6c 0a20 2020 2070 6572 666f 726d  mall.    perform
-000066e0: 616e 6365 2070 656e 616c 7479 2e0a 0a53  ance penalty...S
-000066f0: 6574 206f 7065 7261 7469 6f6e 730a 7e7e  et operations.~~
-00006700: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 5468  ~~~~~~~~~~~~..Th
-00006710: 6573 6520 6361 6e20 6265 2068 616e 6479  ese can be handy
-00006720: 2066 6f72 2065 7863 6c75 6469 6e67 2070   for excluding p
-00006730: 6172 7473 206f 6620 6120 646f 6375 6d65  arts of a docume
-00006740: 6e74 2074 7265 6520 6265 666f 7265 0a65  nt tree before.e
-00006750: 7874 7261 6374 696e 6720 7465 7874 2065  xtracting text e
-00006760: 6c65 6d65 6e74 7320 666f 7220 6578 616d  lements for exam
-00006770: 706c 652e 0a0a 4578 616d 706c 6520 6578  ple...Example ex
-00006780: 7472 6163 7469 6e67 206d 6963 726f 6461  tracting microda
-00006790: 7461 2028 7361 6d70 6c65 2063 6f6e 7465  ta (sample conte
-000067a0: 6e74 2074 616b 656e 2066 726f 6d20 6874  nt taken from ht
-000067b0: 7470 733a 2f2f 7363 6865 6d61 2e6f 7267  tps://schema.org
-000067c0: 2f50 726f 6475 6374 290a 7769 7468 2067  /Product).with g
-000067d0: 726f 7570 7320 6f66 2069 7465 6d73 636f  roups of itemsco
-000067e0: 7065 7320 616e 6420 636f 7272 6573 706f  pes and correspo
-000067f0: 6e64 696e 6720 6974 656d 7072 6f70 733a  nding itemprops:
-00006800: 3a0a 0a20 2020 203e 3e3e 2064 6f63 203d  :..    >>> doc =
-00006810: 2022 2222 0a20 2020 202e 2e2e 203c 6469   """.    ... <di
-00006820: 7620 6974 656d 7363 6f70 6520 6974 656d  v itemscope item
-00006830: 7479 7065 3d22 6874 7470 3a2f 2f73 6368  type="http://sch
-00006840: 656d 612e 6f72 672f 5072 6f64 7563 7422  ema.org/Product"
-00006850: 3e0a 2020 2020 2e2e 2e20 2020 3c73 7061  >.    ...   <spa
-00006860: 6e20 6974 656d 7072 6f70 3d22 6e61 6d65  n itemprop="name
-00006870: 223e 4b65 6e6d 6f72 6520 5768 6974 6520  ">Kenmore White 
-00006880: 3137 2220 4d69 6372 6f77 6176 653c 2f73  17" Microwave</s
-00006890: 7061 6e3e 0a20 2020 202e 2e2e 2020 203c  pan>.    ...   <
-000068a0: 696d 6720 7372 633d 226b 656e 6d6f 7265  img src="kenmore
-000068b0: 2d6d 6963 726f 7761 7665 2d31 3769 6e2e  -microwave-17in.
-000068c0: 6a70 6722 2061 6c74 3d27 4b65 6e6d 6f72  jpg" alt='Kenmor
-000068d0: 6520 3137 2220 4d69 6372 6f77 6176 6527  e 17" Microwave'
-000068e0: 202f 3e0a 2020 2020 2e2e 2e20 2020 3c64   />.    ...   <d
-000068f0: 6976 2069 7465 6d70 726f 703d 2261 6767  iv itemprop="agg
-00006900: 7265 6761 7465 5261 7469 6e67 220a 2020  regateRating".  
-00006910: 2020 2e2e 2e20 2020 2020 6974 656d 7363    ...     itemsc
-00006920: 6f70 6520 6974 656d 7479 7065 3d22 6874  ope itemtype="ht
-00006930: 7470 3a2f 2f73 6368 656d 612e 6f72 672f  tp://schema.org/
-00006940: 4167 6772 6567 6174 6552 6174 696e 6722  AggregateRating"
-00006950: 3e0a 2020 2020 2e2e 2e20 2020 2052 6174  >.    ...    Rat
-00006960: 6564 203c 7370 616e 2069 7465 6d70 726f  ed <span itempro
-00006970: 703d 2272 6174 696e 6756 616c 7565 223e  p="ratingValue">
-00006980: 332e 353c 2f73 7061 6e3e 2f35 0a20 2020  3.5</span>/5.   
-00006990: 202e 2e2e 2020 2020 6261 7365 6420 6f6e   ...    based on
-000069a0: 203c 7370 616e 2069 7465 6d70 726f 703d   <span itemprop=
-000069b0: 2272 6576 6965 7743 6f75 6e74 223e 3131  "reviewCount">11
-000069c0: 3c2f 7370 616e 3e20 6375 7374 6f6d 6572  </span> customer
-000069d0: 2072 6576 6965 7773 0a20 2020 202e 2e2e   reviews.    ...
-000069e0: 2020 203c 2f64 6976 3e0a 2020 2020 2e2e     </div>.    ..
-000069f0: 2e0a 2020 2020 2e2e 2e20 2020 3c64 6976  ..    ...   <div
-00006a00: 2069 7465 6d70 726f 703d 226f 6666 6572   itemprop="offer
-00006a10: 7322 2069 7465 6d73 636f 7065 2069 7465  s" itemscope ite
-00006a20: 6d74 7970 653d 2268 7474 703a 2f2f 7363  mtype="http://sc
-00006a30: 6865 6d61 2e6f 7267 2f4f 6666 6572 223e  hema.org/Offer">
-00006a40: 0a20 2020 202e 2e2e 2020 2020 203c 7370  .    ...     <sp
-00006a50: 616e 2069 7465 6d70 726f 703d 2270 7269  an itemprop="pri
-00006a60: 6365 223e 2435 352e 3030 3c2f 7370 616e  ce">$55.00</span
-00006a70: 3e0a 2020 2020 2e2e 2e20 2020 2020 3c6c  >.    ...     <l
-00006a80: 696e 6b20 6974 656d 7072 6f70 3d22 6176  ink itemprop="av
-00006a90: 6169 6c61 6269 6c69 7479 2220 6872 6566  ailability" href
-00006aa0: 3d22 6874 7470 3a2f 2f73 6368 656d 612e  ="http://schema.
-00006ab0: 6f72 672f 496e 5374 6f63 6b22 202f 3e49  org/InStock" />I
-00006ac0: 6e20 7374 6f63 6b0a 2020 2020 2e2e 2e20  n stock.    ... 
-00006ad0: 2020 3c2f 6469 763e 0a20 2020 202e 2e2e    </div>.    ...
-00006ae0: 0a20 2020 202e 2e2e 2020 2050 726f 6475  .    ...   Produ
-00006af0: 6374 2064 6573 6372 6970 7469 6f6e 3a0a  ct description:.
-00006b00: 2020 2020 2e2e 2e20 2020 3c73 7061 6e20      ...   <span 
-00006b10: 6974 656d 7072 6f70 3d22 6465 7363 7269  itemprop="descri
-00006b20: 7074 696f 6e22 3e30 2e37 2063 7562 6963  ption">0.7 cubic
-00006b30: 2066 6565 7420 636f 756e 7465 7274 6f70   feet countertop
-00006b40: 206d 6963 726f 7761 7665 2e0a 2020 2020   microwave..    
-00006b50: 2e2e 2e20 2020 4861 7320 7369 7820 7072  ...   Has six pr
-00006b60: 6573 6574 2063 6f6f 6b69 6e67 2063 6174  eset cooking cat
-00006b70: 6567 6f72 6965 7320 616e 6420 636f 6e76  egories and conv
-00006b80: 656e 6965 6e63 6520 6665 6174 7572 6573  enience features
-00006b90: 206c 696b 650a 2020 2020 2e2e 2e20 2020   like.    ...   
-00006ba0: 4164 642d 412d 4d69 6e75 7465 2061 6e64  Add-A-Minute and
-00006bb0: 2043 6869 6c64 204c 6f63 6b2e 3c2f 7370   Child Lock.</sp
-00006bc0: 616e 3e0a 2020 2020 2e2e 2e0a 2020 2020  an>.    ....    
-00006bd0: 2e2e 2e20 2020 4375 7374 6f6d 6572 2072  ...   Customer r
-00006be0: 6576 6965 7773 3a0a 2020 2020 2e2e 2e0a  eviews:.    ....
-00006bf0: 2020 2020 2e2e 2e20 2020 3c64 6976 2069      ...   <div i
-00006c00: 7465 6d70 726f 703d 2272 6576 6965 7722  temprop="review"
-00006c10: 2069 7465 6d73 636f 7065 2069 7465 6d74   itemscope itemt
-00006c20: 7970 653d 2268 7474 703a 2f2f 7363 6865  ype="http://sche
-00006c30: 6d61 2e6f 7267 2f52 6576 6965 7722 3e0a  ma.org/Review">.
-00006c40: 2020 2020 2e2e 2e20 2020 2020 3c73 7061      ...     <spa
-00006c50: 6e20 6974 656d 7072 6f70 3d22 6e61 6d65  n itemprop="name
-00006c60: 223e 4e6f 7420 6120 6861 7070 7920 6361  ">Not a happy ca
-00006c70: 6d70 6572 3c2f 7370 616e 3e20 2d0a 2020  mper</span> -.  
-00006c80: 2020 2e2e 2e20 2020 2020 6279 203c 7370    ...     by <sp
-00006c90: 616e 2069 7465 6d70 726f 703d 2261 7574  an itemprop="aut
-00006ca0: 686f 7222 3e45 6c6c 6965 3c2f 7370 616e  hor">Ellie</span
-00006cb0: 3e2c 0a20 2020 202e 2e2e 2020 2020 203c  >,.    ...     <
-00006cc0: 6d65 7461 2069 7465 6d70 726f 703d 2264  meta itemprop="d
-00006cd0: 6174 6550 7562 6c69 7368 6564 2220 636f  atePublished" co
-00006ce0: 6e74 656e 743d 2232 3031 312d 3034 2d30  ntent="2011-04-0
-00006cf0: 3122 3e41 7072 696c 2031 2c20 3230 3131  1">April 1, 2011
-00006d00: 0a20 2020 202e 2e2e 2020 2020 203c 6469  .    ...     <di
-00006d10: 7620 6974 656d 7072 6f70 3d22 7265 7669  v itemprop="revi
-00006d20: 6577 5261 7469 6e67 2220 6974 656d 7363  ewRating" itemsc
-00006d30: 6f70 6520 6974 656d 7479 7065 3d22 6874  ope itemtype="ht
-00006d40: 7470 3a2f 2f73 6368 656d 612e 6f72 672f  tp://schema.org/
-00006d50: 5261 7469 6e67 223e 0a20 2020 202e 2e2e  Rating">.    ...
-00006d60: 2020 2020 2020 203c 6d65 7461 2069 7465         <meta ite
-00006d70: 6d70 726f 703d 2277 6f72 7374 5261 7469  mprop="worstRati
-00006d80: 6e67 2220 636f 6e74 656e 7420 3d20 2231  ng" content = "1
-00006d90: 223e 0a20 2020 202e 2e2e 2020 2020 2020  ">.    ...      
-00006da0: 203c 7370 616e 2069 7465 6d70 726f 703d   <span itemprop=
-00006db0: 2272 6174 696e 6756 616c 7565 223e 313c  "ratingValue">1<
-00006dc0: 2f73 7061 6e3e 2f0a 2020 2020 2e2e 2e20  /span>/.    ... 
-00006dd0: 2020 2020 2020 3c73 7061 6e20 6974 656d        <span item
-00006de0: 7072 6f70 3d22 6265 7374 5261 7469 6e67  prop="bestRating
-00006df0: 223e 353c 2f73 7061 6e3e 7374 6172 730a  ">5</span>stars.
-00006e00: 2020 2020 2e2e 2e20 2020 2020 3c2f 6469      ...     </di
-00006e10: 763e 0a20 2020 202e 2e2e 2020 2020 203c  v>.    ...     <
-00006e20: 7370 616e 2069 7465 6d70 726f 703d 2264  span itemprop="d
-00006e30: 6573 6372 6970 7469 6f6e 223e 5468 6520  escription">The 
-00006e40: 6c61 6d70 2062 7572 6e65 6420 6f75 7420  lamp burned out 
-00006e50: 616e 6420 6e6f 7720 4920 6861 7665 2074  and now I have t
-00006e60: 6f20 7265 706c 6163 650a 2020 2020 2e2e  o replace.    ..
-00006e70: 2e20 2020 2020 6974 2e20 3c2f 7370 616e  .     it. </span
-00006e80: 3e0a 2020 2020 2e2e 2e20 2020 3c2f 6469  >.    ...   </di
-00006e90: 763e 0a20 2020 202e 2e2e 0a20 2020 202e  v>.    ....    .
-00006ea0: 2e2e 2020 203c 6469 7620 6974 656d 7072  ..   <div itempr
-00006eb0: 6f70 3d22 7265 7669 6577 2220 6974 656d  op="review" item
-00006ec0: 7363 6f70 6520 6974 656d 7479 7065 3d22  scope itemtype="
-00006ed0: 6874 7470 3a2f 2f73 6368 656d 612e 6f72  http://schema.or
-00006ee0: 672f 5265 7669 6577 223e 0a20 2020 202e  g/Review">.    .
-00006ef0: 2e2e 2020 2020 203c 7370 616e 2069 7465  ..     <span ite
-00006f00: 6d70 726f 703d 226e 616d 6522 3e56 616c  mprop="name">Val
-00006f10: 7565 2070 7572 6368 6173 653c 2f73 7061  ue purchase</spa
-00006f20: 6e3e 202d 0a20 2020 202e 2e2e 2020 2020  n> -.    ...    
-00006f30: 2062 7920 3c73 7061 6e20 6974 656d 7072   by <span itempr
-00006f40: 6f70 3d22 6175 7468 6f72 223e 4c75 6361  op="author">Luca
-00006f50: 733c 2f73 7061 6e3e 2c0a 2020 2020 2e2e  s</span>,.    ..
-00006f60: 2e20 2020 2020 3c6d 6574 6120 6974 656d  .     <meta item
-00006f70: 7072 6f70 3d22 6461 7465 5075 626c 6973  prop="datePublis
-00006f80: 6865 6422 2063 6f6e 7465 6e74 3d22 3230  hed" content="20
-00006f90: 3131 2d30 332d 3235 223e 4d61 7263 6820  11-03-25">March 
-00006fa0: 3235 2c20 3230 3131 0a20 2020 202e 2e2e  25, 2011.    ...
-00006fb0: 2020 2020 203c 6469 7620 6974 656d 7072       <div itempr
-00006fc0: 6f70 3d22 7265 7669 6577 5261 7469 6e67  op="reviewRating
-00006fd0: 2220 6974 656d 7363 6f70 6520 6974 656d  " itemscope item
-00006fe0: 7479 7065 3d22 6874 7470 3a2f 2f73 6368  type="http://sch
-00006ff0: 656d 612e 6f72 672f 5261 7469 6e67 223e  ema.org/Rating">
-00007000: 0a20 2020 202e 2e2e 2020 2020 2020 203c  .    ...       <
-00007010: 6d65 7461 2069 7465 6d70 726f 703d 2277  meta itemprop="w
-00007020: 6f72 7374 5261 7469 6e67 2220 636f 6e74  orstRating" cont
-00007030: 656e 7420 3d20 2231 222f 3e0a 2020 2020  ent = "1"/>.    
-00007040: 2e2e 2e20 2020 2020 2020 3c73 7061 6e20  ...       <span 
-00007050: 6974 656d 7072 6f70 3d22 7261 7469 6e67  itemprop="rating
-00007060: 5661 6c75 6522 3e34 3c2f 7370 616e 3e2f  Value">4</span>/
-00007070: 0a20 2020 202e 2e2e 2020 2020 2020 203c  .    ...       <
-00007080: 7370 616e 2069 7465 6d70 726f 703d 2262  span itemprop="b
-00007090: 6573 7452 6174 696e 6722 3e35 3c2f 7370  estRating">5</sp
-000070a0: 616e 3e73 7461 7273 0a20 2020 202e 2e2e  an>stars.    ...
-000070b0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000070c0: 2e2e 2e20 2020 2020 3c73 7061 6e20 6974  ...     <span it
-000070d0: 656d 7072 6f70 3d22 6465 7363 7269 7074  emprop="descript
-000070e0: 696f 6e22 3e47 7265 6174 206d 6963 726f  ion">Great micro
-000070f0: 7761 7665 2066 6f72 2074 6865 2070 7269  wave for the pri
-00007100: 6365 2e20 4974 2069 7320 736d 616c 6c20  ce. It is small 
-00007110: 616e 640a 2020 2020 2e2e 2e20 2020 2020  and.    ...     
-00007120: 6669 7473 2069 6e20 6d79 2061 7061 7274  fits in my apart
-00007130: 6d65 6e74 2e3c 2f73 7061 6e3e 0a20 2020  ment.</span>.   
-00007140: 202e 2e2e 2020 203c 2f64 6976 3e0a 2020   ...   </div>.  
-00007150: 2020 2e2e 2e20 2020 2e2e 2e0a 2020 2020    ...   ....    
-00007160: 2e2e 2e20 3c2f 6469 763e 0a20 2020 202e  ... </div>.    .
-00007170: 2e2e 2022 2222 0a20 2020 203e 3e3e 2073  .. """.    >>> s
-00007180: 656c 203d 2053 656c 6563 746f 7228 7465  el = Selector(te
-00007190: 7874 3d64 6f63 2c20 7479 7065 3d22 6874  xt=doc, type="ht
-000071a0: 6d6c 2229 0a20 2020 203e 3e3e 2066 6f72  ml").    >>> for
-000071b0: 2073 636f 7065 2069 6e20 7365 6c2e 7870   scope in sel.xp
-000071c0: 6174 6828 272f 2f64 6976 5b40 6974 656d  ath('//div[@item
-000071d0: 7363 6f70 655d 2729 3a0a 2020 2020 2e2e  scope]'):.    ..
-000071e0: 2e20 2020 2020 7072 696e 7428 2263 7572  .     print("cur
-000071f0: 7265 6e74 2073 636f 7065 3a22 2c20 7363  rent scope:", sc
-00007200: 6f70 652e 7870 6174 6828 2740 6974 656d  ope.xpath('@item
-00007210: 7479 7065 2729 2e67 6574 616c 6c28 2929  type').getall())
-00007220: 0a20 2020 202e 2e2e 2020 2020 2070 726f  .    ...     pro
-00007230: 7073 203d 2073 636f 7065 2e78 7061 7468  ps = scope.xpath
-00007240: 2827 2727 0a20 2020 202e 2e2e 2020 2020  ('''.    ...    
-00007250: 2020 2020 2020 2020 2020 2020 2073 6574               set
-00007260: 3a64 6966 6665 7265 6e63 6528 2e2f 6465  :difference(./de
-00007270: 7363 656e 6461 6e74 3a3a 2a2f 4069 7465  scendant::*/@ite
-00007280: 6d70 726f 702c 0a20 2020 202e 2e2e 2020  mprop,.    ...  
-00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072a0: 2020 2020 2020 2020 2020 2020 2020 2e2f                ./
-000072b0: 2f2a 5b40 6974 656d 7363 6f70 655d 2f2a  /*[@itemscope]/*
-000072c0: 2f40 6974 656d 7072 6f70 2927 2727 290a  /@itemprop)''').
-000072d0: 2020 2020 2e2e 2e20 2020 2020 7072 696e      ...     prin
-000072e0: 7428 6622 2020 2020 7072 6f70 6572 7469  t(f"    properti
-000072f0: 6573 3a20 7b70 726f 7073 2e67 6574 616c  es: {props.getal
-00007300: 6c28 297d 2229 0a20 2020 202e 2e2e 2020  l()}").    ...  
-00007310: 2020 2070 7269 6e74 2822 2229 0a0a 2020     print("")..  
-00007320: 2020 6375 7272 656e 7420 7363 6f70 653a    current scope:
-00007330: 205b 2768 7474 703a 2f2f 7363 6865 6d61   ['http://schema
-00007340: 2e6f 7267 2f50 726f 6475 6374 275d 0a20  .org/Product']. 
-00007350: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
-00007360: 733a 205b 276e 616d 6527 2c20 2761 6767  s: ['name', 'agg
-00007370: 7265 6761 7465 5261 7469 6e67 272c 2027  regateRating', '
-00007380: 6f66 6665 7273 272c 2027 6465 7363 7269  offers', 'descri
-00007390: 7074 696f 6e27 2c20 2772 6576 6965 7727  ption', 'review'
-000073a0: 2c20 2772 6576 6965 7727 5d0a 0a20 2020  , 'review']..   
-000073b0: 2063 7572 7265 6e74 2073 636f 7065 3a20   current scope: 
-000073c0: 5b27 6874 7470 3a2f 2f73 6368 656d 612e  ['http://schema.
-000073d0: 6f72 672f 4167 6772 6567 6174 6552 6174  org/AggregateRat
-000073e0: 696e 6727 5d0a 2020 2020 2020 2020 7072  ing'].        pr
-000073f0: 6f70 6572 7469 6573 3a20 5b27 7261 7469  operties: ['rati
-00007400: 6e67 5661 6c75 6527 2c20 2772 6576 6965  ngValue', 'revie
-00007410: 7743 6f75 6e74 275d 0a0a 2020 2020 6375  wCount']..    cu
-00007420: 7272 656e 7420 7363 6f70 653a 205b 2768  rrent scope: ['h
-00007430: 7474 703a 2f2f 7363 6865 6d61 2e6f 7267  ttp://schema.org
-00007440: 2f4f 6666 6572 275d 0a20 2020 2020 2020  /Offer'].       
-00007450: 2070 726f 7065 7274 6965 733a 205b 2770   properties: ['p
-00007460: 7269 6365 272c 2027 6176 6169 6c61 6269  rice', 'availabi
-00007470: 6c69 7479 275d 0a0a 2020 2020 6375 7272  lity']..    curr
-00007480: 656e 7420 7363 6f70 653a 205b 2768 7474  ent scope: ['htt
-00007490: 703a 2f2f 7363 6865 6d61 2e6f 7267 2f52  p://schema.org/R
-000074a0: 6576 6965 7727 5d0a 2020 2020 2020 2020  eview'].        
-000074b0: 7072 6f70 6572 7469 6573 3a20 5b27 6e61  properties: ['na
-000074c0: 6d65 272c 2027 6175 7468 6f72 272c 2027  me', 'author', '
-000074d0: 6461 7465 5075 626c 6973 6865 6427 2c20  datePublished', 
-000074e0: 2772 6576 6965 7752 6174 696e 6727 2c20  'reviewRating', 
-000074f0: 2764 6573 6372 6970 7469 6f6e 275d 0a0a  'description']..
-00007500: 2020 2020 6375 7272 656e 7420 7363 6f70      current scop
-00007510: 653a 205b 2768 7474 703a 2f2f 7363 6865  e: ['http://sche
-00007520: 6d61 2e6f 7267 2f52 6174 696e 6727 5d0a  ma.org/Rating'].
-00007530: 2020 2020 2020 2020 7072 6f70 6572 7469          properti
-00007540: 6573 3a20 5b27 776f 7273 7452 6174 696e  es: ['worstRatin
-00007550: 6727 2c20 2772 6174 696e 6756 616c 7565  g', 'ratingValue
-00007560: 272c 2027 6265 7374 5261 7469 6e67 275d  ', 'bestRating']
-00007570: 0a0a 2020 2020 6375 7272 656e 7420 7363  ..    current sc
-00007580: 6f70 653a 205b 2768 7474 703a 2f2f 7363  ope: ['http://sc
-00007590: 6865 6d61 2e6f 7267 2f52 6576 6965 7727  hema.org/Review'
-000075a0: 5d0a 2020 2020 2020 2020 7072 6f70 6572  ].        proper
-000075b0: 7469 6573 3a20 5b27 6e61 6d65 272c 2027  ties: ['name', '
-000075c0: 6175 7468 6f72 272c 2027 6461 7465 5075  author', 'datePu
-000075d0: 626c 6973 6865 6427 2c20 2772 6576 6965  blished', 'revie
-000075e0: 7752 6174 696e 6727 2c20 2764 6573 6372  wRating', 'descr
-000075f0: 6970 7469 6f6e 275d 0a0a 2020 2020 6375  iption']..    cu
-00007600: 7272 656e 7420 7363 6f70 653a 205b 2768  rrent scope: ['h
-00007610: 7474 703a 2f2f 7363 6865 6d61 2e6f 7267  ttp://schema.org
-00007620: 2f52 6174 696e 6727 5d0a 2020 2020 2020  /Rating'].      
-00007630: 2020 7072 6f70 6572 7469 6573 3a20 5b27    properties: ['
-00007640: 776f 7273 7452 6174 696e 6727 2c20 2772  worstRating', 'r
-00007650: 6174 696e 6756 616c 7565 272c 2027 6265  atingValue', 'be
-00007660: 7374 5261 7469 6e67 275d 0a0a 0a48 6572  stRating']...Her
-00007670: 6520 7765 2066 6972 7374 2069 7465 7261  e we first itera
-00007680: 7465 206f 7665 7220 6060 6974 656d 7363  te over ``itemsc
-00007690: 6f70 6560 6020 656c 656d 656e 7473 2c20  ope`` elements, 
-000076a0: 616e 6420 666f 7220 6561 6368 206f 6e65  and for each one
-000076b0: 2c0a 7765 206c 6f6f 6b20 666f 7220 616c  ,.we look for al
-000076c0: 6c20 6060 6974 656d 7072 6f70 7360 6020  l ``itemprops`` 
-000076d0: 656c 656d 656e 7473 2061 6e64 2065 7863  elements and exc
-000076e0: 6c75 6465 2074 686f 7365 2074 6861 7420  lude those that 
-000076f0: 6172 6520 7468 656d 7365 6c76 6573 0a69  are themselves.i
-00007700: 6e73 6964 6520 616e 6f74 6865 7220 6060  nside another ``
-00007710: 6974 656d 7363 6f70 6560 602e 0a0a 2e2e  itemscope``.....
-00007720: 205f 4558 534c 543a 2068 7474 703a 2f2f   _EXSLT: http://
-00007730: 6578 736c 742e 6f72 672f 0a2e 2e20 5f72  exslt.org/... _r
-00007740: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
-00007750: 6e73 3a20 6874 7470 3a2f 2f65 7873 6c74  ns: http://exslt
-00007760: 2e6f 7267 2f72 6567 6578 702f 696e 6465  .org/regexp/inde
-00007770: 782e 6874 6d6c 0a2e 2e20 5f73 6574 206d  x.html... _set m
-00007780: 616e 6970 756c 6174 696f 6e3a 2068 7474  anipulation: htt
-00007790: 703a 2f2f 6578 736c 742e 6f72 672f 7365  p://exslt.org/se
-000077a0: 742f 696e 6465 782e 6874 6d6c 0a0a 4f74  t/index.html..Ot
-000077b0: 6865 7220 5850 6174 6820 6578 7465 6e73  her XPath extens
-000077c0: 696f 6e73 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ions.-----------
-000077d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a53 6372  -----------..Scr
-000077e0: 6170 7920 7365 6c65 6374 6f72 7320 616c  apy selectors al
-000077f0: 736f 2070 726f 7669 6465 2061 2073 6f72  so provide a sor
-00007800: 656c 7920 6d69 7373 6564 2058 5061 7468  ely missed XPath
-00007810: 2065 7874 656e 7369 6f6e 2066 756e 6374   extension funct
-00007820: 696f 6e0a 6060 6861 732d 636c 6173 7360  ion.``has-class`
-00007830: 6020 7468 6174 2072 6574 7572 6e73 2060  ` that returns `
-00007840: 6054 7275 6560 6020 666f 7220 6e6f 6465  `True`` for node
-00007850: 7320 7468 6174 2068 6176 6520 616c 6c20  s that have all 
-00007860: 6f66 2074 6865 2073 7065 6369 6669 6564  of the specified
-00007870: 0a48 544d 4c20 636c 6173 7365 732e 0a0a  .HTML classes...
-00007880: 2e2e 2068 6967 686c 6967 6874 3a3a 2068  .. highlight:: h
-00007890: 746d 6c0a 0a46 6f72 2074 6865 2066 6f6c  tml..For the fol
-000078a0: 6c6f 7769 6e67 2048 544d 4c3a 3a0a 0a20  lowing HTML::.. 
-000078b0: 2020 203c 7020 636c 6173 733d 2266 6f6f     <p class="foo
-000078c0: 2062 6172 2d62 617a 223e 4669 7273 743c   bar-baz">First<
-000078d0: 2f70 3e0a 2020 2020 3c70 2063 6c61 7373  /p>.    <p class
-000078e0: 3d22 666f 6f22 3e53 6563 6f6e 643c 2f70  ="foo">Second</p
-000078f0: 3e0a 2020 2020 3c70 2063 6c61 7373 3d22  >.    <p class="
-00007900: 6261 7222 3e54 6869 7264 3c2f 703e 0a20  bar">Third</p>. 
-00007910: 2020 203c 703e 466f 7572 7468 3c2f 703e     <p>Fourth</p>
-00007920: 0a0a 2e2e 2068 6967 686c 6967 6874 3a3a  .... highlight::
-00007930: 2070 7974 686f 6e0a 0a59 6f75 2063 616e   python..You can
-00007940: 2075 7365 2069 7420 6c69 6b65 2074 6869   use it like thi
-00007950: 733a 0a0a 3e3e 3e20 7265 7370 6f6e 7365  s:..>>> response
-00007960: 2e78 7061 7468 2827 2f2f 705b 6861 732d  .xpath('//p[has-
-00007970: 636c 6173 7328 2266 6f6f 2229 5d27 290a  class("foo")]').
-00007980: 5b3c 5365 6c65 6374 6f72 2078 7061 7468  [<Selector xpath
-00007990: 3d27 2f2f 705b 6861 732d 636c 6173 7328  ='//p[has-class(
-000079a0: 2266 6f6f 2229 5d27 2064 6174 613d 273c  "foo")]' data='<
-000079b0: 7020 636c 6173 733d 2266 6f6f 2062 6172  p class="foo bar
-000079c0: 2d62 617a 223e 4669 7273 743c 2f70 3e27  -baz">First</p>'
-000079d0: 3e2c 0a20 3c53 656c 6563 746f 7220 7870  >,. <Selector xp
-000079e0: 6174 683d 272f 2f70 5b68 6173 2d63 6c61  ath='//p[has-cla
-000079f0: 7373 2822 666f 6f22 295d 2720 6461 7461  ss("foo")]' data
-00007a00: 3d27 3c70 2063 6c61 7373 3d22 666f 6f22  ='<p class="foo"
-00007a10: 3e53 6563 6f6e 643c 2f70 3e27 3e5d 0a3e  >Second</p>'>].>
-00007a20: 3e3e 2072 6573 706f 6e73 652e 7870 6174  >> response.xpat
-00007a30: 6828 272f 2f70 5b68 6173 2d63 6c61 7373  h('//p[has-class
-00007a40: 2822 666f 6f22 2c20 2262 6172 2d62 617a  ("foo", "bar-baz
-00007a50: 2229 5d27 290a 5b3c 5365 6c65 6374 6f72  ")]').[<Selector
-00007a60: 2078 7061 7468 3d27 2f2f 705b 6861 732d   xpath='//p[has-
-00007a70: 636c 6173 7328 2266 6f6f 222c 2022 6261  class("foo", "ba
-00007a80: 722d 6261 7a22 295d 2720 6461 7461 3d27  r-baz")]' data='
-00007a90: 3c70 2063 6c61 7373 3d22 666f 6f20 6261  <p class="foo ba
-00007aa0: 722d 6261 7a22 3e46 6972 7374 3c2f 703e  r-baz">First</p>
-00007ab0: 273e 5d0a 3e3e 3e20 7265 7370 6f6e 7365  '>].>>> response
-00007ac0: 2e78 7061 7468 2827 2f2f 705b 6861 732d  .xpath('//p[has-
-00007ad0: 636c 6173 7328 2266 6f6f 222c 2022 6261  class("foo", "ba
-00007ae0: 7222 295d 2729 0a5b 5d0a 0a53 6f20 5850  r")]').[]..So XP
-00007af0: 6174 6820 6060 2f2f 705b 6861 732d 636c  ath ``//p[has-cl
-00007b00: 6173 7328 2266 6f6f 222c 2022 6261 722d  ass("foo", "bar-
-00007b10: 6261 7a22 295d 6060 2069 7320 726f 7567  baz")]`` is roug
-00007b20: 686c 7920 6571 7569 7661 6c65 6e74 2074  hly equivalent t
-00007b30: 6f20 4353 530a 6060 702e 666f 6f2e 6261  o CSS.``p.foo.ba
-00007b40: 722d 6261 7a60 602e 2020 506c 6561 7365  r-baz``.  Please
-00007b50: 206e 6f74 652c 2074 6861 7420 6974 2069   note, that it i
-00007b60: 7320 736c 6f77 6572 2069 6e20 6d6f 7374  s slower in most
-00007b70: 206f 6620 7468 6520 6361 7365 732c 0a62   of the cases,.b
-00007b80: 6563 6175 7365 2069 7427 7320 6120 7075  ecause it's a pu
-00007b90: 7265 2d50 7974 686f 6e20 6675 6e63 7469  re-Python functi
-00007ba0: 6f6e 2074 6861 7427 7320 696e 766f 6b65  on that's invoke
-00007bb0: 6420 666f 7220 6576 6572 7920 6e6f 6465  d for every node
-00007bc0: 2069 6e20 7175 6573 7469 6f6e 0a77 6865   in question.whe
-00007bd0: 7265 6173 2074 6865 2043 5353 206c 6f6f  reas the CSS loo
-00007be0: 6b75 7020 6973 2074 7261 6e73 6c61 7465  kup is translate
-00007bf0: 6420 696e 746f 2058 5061 7468 2061 6e64  d into XPath and
-00007c00: 2074 6875 7320 7275 6e73 206d 6f72 6520   thus runs more 
-00007c10: 6566 6669 6369 656e 746c 792c 0a73 6f20  efficiently,.so 
-00007c20: 7065 7266 6f72 6d61 6e63 652d 7769 7365  performance-wise
-00007c30: 2069 7473 2075 7365 7320 6172 6520 6c69   its uses are li
-00007c40: 6d69 7465 6420 746f 2073 6974 7561 7469  mited to situati
-00007c50: 6f6e 7320 7468 6174 2061 7265 206e 6f74  ons that are not
-00007c60: 2065 6173 696c 790a 6465 7363 7269 6265   easily.describe
-00007c70: 6420 7769 7468 2043 5353 2073 656c 6563  d with CSS selec
-00007c80: 746f 7273 2e0a 0a50 6172 7365 6c20 616c  tors...Parsel al
-00007c90: 736f 2073 696d 706c 6966 6965 7320 6164  so simplifies ad
-00007ca0: 6469 6e67 2079 6f75 7220 6f77 6e20 5850  ding your own XP
-00007cb0: 6174 6820 6578 7465 6e73 696f 6e73 2e0a  ath extensions..
-00007cc0: 0a2e 2e20 6175 746f 6675 6e63 7469 6f6e  ... autofunction
-00007cd0: 3a3a 2070 6172 7365 6c2e 7870 6174 6866  :: parsel.xpathf
-00007ce0: 756e 6373 2e73 6574 5f78 7061 7468 6675  uncs.set_xpathfu
-00007cf0: 6e63 0a0a 0a2e 2e20 5f74 6f70 6963 732d  nc..... _topics-
-00007d00: 7365 6c65 6374 6f72 732d 7265 663a 0a0a  selectors-ref:..
-00007d10: 4275 696c 742d 696e 2053 656c 6563 746f  Built-in Selecto
-00007d20: 7273 2072 6566 6572 656e 6365 0a3d 3d3d  rs reference.===
-00007d30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007d40: 3d3d 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 6d6f  =========.... mo
-00007d50: 6475 6c65 3a3a 2073 6372 6170 792e 7365  dule:: scrapy.se
-00007d60: 6c65 6374 6f72 0a20 2020 3a73 796e 6f70  lector.   :synop
-00007d70: 7369 733a 2053 656c 6563 746f 7220 636c  sis: Selector cl
-00007d80: 6173 730a 0a53 656c 6563 746f 7220 6f62  ass..Selector ob
-00007d90: 6a65 6374 730a 2d2d 2d2d 2d2d 2d2d 2d2d  jects.----------
-00007da0: 2d2d 2d2d 2d2d 0a0a 2e2e 2061 7574 6f63  ------.... autoc
-00007db0: 6c61 7373 3a3a 2053 656c 6563 746f 720a  lass:: Selector.
-00007dc0: 0a20 202e 2e20 6175 746f 6d65 7468 6f64  .  .. automethod
-00007dd0: 3a3a 2078 7061 7468 0a0a 2020 2020 2020  :: xpath..      
-00007de0: 2e2e 206e 6f74 653a 3a0a 0a20 2020 2020  .. note::..     
-00007df0: 2020 2020 2046 6f72 2063 6f6e 7665 6e69       For conveni
-00007e00: 656e 6365 2c20 7468 6973 206d 6574 686f  ence, this metho
-00007e10: 6420 6361 6e20 6265 2063 616c 6c65 6420  d can be called 
-00007e20: 6173 2060 6072 6573 706f 6e73 652e 7870  as ``response.xp
-00007e30: 6174 6828 2960 600a 0a20 202e 2e20 6175  ath()``..  .. au
-00007e40: 746f 6d65 7468 6f64 3a3a 2063 7373 0a0a  tomethod:: css..
-00007e50: 2020 2020 2020 2e2e 206e 6f74 653a 3a0a        .. note::.
-00007e60: 0a20 2020 2020 2020 2020 2046 6f72 2063  .          For c
-00007e70: 6f6e 7665 6e69 656e 6365 2c20 7468 6973  onvenience, this
-00007e80: 206d 6574 686f 6420 6361 6e20 6265 2063   method can be c
-00007e90: 616c 6c65 6420 6173 2060 6072 6573 706f  alled as ``respo
-00007ea0: 6e73 652e 6373 7328 2960 600a 0a20 202e  nse.css()``..  .
-00007eb0: 2e20 6175 746f 6d65 7468 6f64 3a3a 2067  . automethod:: g
-00007ec0: 6574 0a0a 2020 2020 2053 6565 2061 6c73  et..     See als
-00007ed0: 6f3a 203a 7265 663a 606f 6c64 2d65 7874  o: :ref:`old-ext
-00007ee0: 7261 6374 696f 6e2d 6170 6960 0a0a 2020  raction-api`..  
-00007ef0: 2e2e 2061 7574 6f61 7474 7269 6275 7465  .. autoattribute
-00007f00: 3a3a 2061 7474 7269 620a 0a20 2020 2020  :: attrib..     
-00007f10: 5365 6520 616c 736f 3a20 3a72 6566 3a60  See also: :ref:`
-00007f20: 7365 6c65 6374 696e 672d 6174 7472 6962  selecting-attrib
-00007f30: 7574 6573 602e 0a0a 2020 2e2e 2061 7574  utes`...  .. aut
-00007f40: 6f6d 6574 686f 643a 3a20 7265 0a0a 2020  omethod:: re..  
-00007f50: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
-00007f60: 7265 5f66 6972 7374 0a0a 2020 2e2e 2061  re_first..  .. a
-00007f70: 7574 6f6d 6574 686f 643a 3a20 7265 6769  utomethod:: regi
-00007f80: 7374 6572 5f6e 616d 6573 7061 6365 0a0a  ster_namespace..
-00007f90: 2020 2e2e 2061 7574 6f6d 6574 686f 643a    .. automethod:
-00007fa0: 3a20 7265 6d6f 7665 5f6e 616d 6573 7061  : remove_namespa
-00007fb0: 6365 730a 0a20 202e 2e20 6175 746f 6d65  ces..  .. autome
-00007fc0: 7468 6f64 3a3a 205f 5f62 6f6f 6c5f 5f0a  thod:: __bool__.
-00007fd0: 0a20 202e 2e20 6175 746f 6d65 7468 6f64  .  .. automethod
-00007fe0: 3a3a 2067 6574 616c 6c0a 0a20 2020 2020  :: getall..     
-00007ff0: 5468 6973 206d 6574 686f 6420 6973 2061  This method is a
-00008000: 6464 6564 2074 6f20 5365 6c65 6374 6f72  dded to Selector
-00008010: 2066 6f72 2063 6f6e 7369 7374 656e 6379   for consistency
-00008020: 3b20 6974 2069 7320 6d6f 7265 2075 7365  ; it is more use
-00008030: 6675 6c0a 2020 2020 2077 6974 6820 5365  ful.     with Se
-00008040: 6c65 6374 6f72 4c69 7374 2e20 5365 6520  lectorList. See 
-00008050: 616c 736f 3a20 3a72 6566 3a60 6f6c 642d  also: :ref:`old-
-00008060: 6578 7472 6163 7469 6f6e 2d61 7069 600a  extraction-api`.
-00008070: 0a53 656c 6563 746f 724c 6973 7420 6f62  .SelectorList ob
-00008080: 6a65 6374 730a 2d2d 2d2d 2d2d 2d2d 2d2d  jects.----------
-00008090: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2061  ----------.... a
-000080a0: 7574 6f63 6c61 7373 3a3a 2053 656c 6563  utoclass:: Selec
-000080b0: 746f 724c 6973 740a 0a20 2020 2e2e 2061  torList..   .. a
-000080c0: 7574 6f6d 6574 686f 643a 3a20 7870 6174  utomethod:: xpat
-000080d0: 680a 0a20 2020 2e2e 2061 7574 6f6d 6574  h..   .. automet
-000080e0: 686f 643a 3a20 6373 730a 0a20 2020 2e2e  hod:: css..   ..
-000080f0: 2061 7574 6f6d 6574 686f 643a 3a20 6765   automethod:: ge
-00008100: 7461 6c6c 0a0a 2020 2020 2020 5365 6520  tall..      See 
-00008110: 616c 736f 3a20 3a72 6566 3a60 6f6c 642d  also: :ref:`old-
-00008120: 6578 7472 6163 7469 6f6e 2d61 7069 600a  extraction-api`.
-00008130: 0a20 2020 2e2e 2061 7574 6f6d 6574 686f  .   .. autometho
-00008140: 643a 3a20 6765 740a 0a20 2020 2020 2053  d:: get..      S
-00008150: 6565 2061 6c73 6f3a 203a 7265 663a 606f  ee also: :ref:`o
-00008160: 6c64 2d65 7874 7261 6374 696f 6e2d 6170  ld-extraction-ap
-00008170: 6960 0a0a 2020 202e 2e20 6175 746f 6d65  i`..   .. autome
-00008180: 7468 6f64 3a3a 2072 650a 0a20 2020 2e2e  thod:: re..   ..
-00008190: 2061 7574 6f6d 6574 686f 643a 3a20 7265   automethod:: re
-000081a0: 5f66 6972 7374 0a0a 2020 202e 2e20 6175  _first..   .. au
-000081b0: 746f 6174 7472 6962 7574 653a 3a20 6174  toattribute:: at
-000081c0: 7472 6962 0a0a 2020 2020 2020 5365 6520  trib..      See 
-000081d0: 616c 736f 3a20 3a72 6566 3a60 7365 6c65  also: :ref:`sele
-000081e0: 6374 696e 672d 6174 7472 6962 7574 6573  cting-attributes
-000081f0: 602e 0a0a 2e2e 205f 7365 6c65 6374 6f72  `..... _selector
-00008200: 2d65 7861 6d70 6c65 733a 0a0a 4578 616d  -examples:..Exam
-00008210: 706c 6573 0a3d 3d3d 3d3d 3d3d 3d0a 0a2e  ples.========...
-00008220: 2e20 5f73 656c 6563 746f 722d 6578 616d  . _selector-exam
-00008230: 706c 6573 2d68 746d 6c3a 0a0a 5365 6c65  ples-html:..Sele
-00008240: 6374 6f72 2065 7861 6d70 6c65 7320 6f6e  ctor examples on
-00008250: 2048 544d 4c20 7265 7370 6f6e 7365 0a2d   HTML response.-
-00008260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008280: 2d0a 0a48 6572 6520 6172 6520 736f 6d65  -..Here are some
-00008290: 203a 636c 6173 733a 6053 656c 6563 746f   :class:`Selecto
-000082a0: 7260 2065 7861 6d70 6c65 7320 746f 2069  r` examples to i
-000082b0: 6c6c 7573 7472 6174 6520 7365 7665 7261  llustrate severa
-000082c0: 6c20 636f 6e63 6570 7473 2e0a 496e 2061  l concepts..In a
-000082d0: 6c6c 2063 6173 6573 2c20 7765 2061 7373  ll cases, we ass
-000082e0: 756d 6520 7468 6572 6520 6973 2061 6c72  ume there is alr
-000082f0: 6561 6479 2061 203a 636c 6173 733a 6053  eady a :class:`S
-00008300: 656c 6563 746f 7260 2069 6e73 7461 6e74  elector` instant
-00008310: 6961 7465 6420 7769 7468 0a61 203a 636c  iated with.a :cl
-00008320: 6173 733a 607e 7363 7261 7079 2e68 7474  ass:`~scrapy.htt
-00008330: 702e 4874 6d6c 5265 7370 6f6e 7365 6020  p.HtmlResponse` 
-00008340: 6f62 6a65 6374 206c 696b 6520 7468 6973  object like this
-00008350: 3a3a 0a0a 2020 2020 2020 7365 6c20 3d20  ::..      sel = 
-00008360: 5365 6c65 6374 6f72 2868 746d 6c5f 7265  Selector(html_re
-00008370: 7370 6f6e 7365 290a 0a31 2e20 5365 6c65  sponse)..1. Sele
-00008380: 6374 2061 6c6c 2060 603c 6831 3e60 6020  ct all ``<h1>`` 
-00008390: 656c 656d 656e 7473 2066 726f 6d20 616e  elements from an
-000083a0: 2048 544d 4c20 7265 7370 6f6e 7365 2062   HTML response b
-000083b0: 6f64 792c 2072 6574 7572 6e69 6e67 2061  ody, returning a
-000083c0: 206c 6973 7420 6f66 0a20 2020 3a63 6c61   list of.   :cla
-000083d0: 7373 3a60 5365 6c65 6374 6f72 6020 6f62  ss:`Selector` ob
-000083e0: 6a65 6374 7320 2869 2e65 2e20 6120 3a63  jects (i.e. a :c
-000083f0: 6c61 7373 3a60 5365 6c65 6374 6f72 4c69  lass:`SelectorLi
-00008400: 7374 6020 6f62 6a65 6374 293a 3a0a 0a20  st` object)::.. 
-00008410: 2020 2020 2073 656c 2e78 7061 7468 2822       sel.xpath("
-00008420: 2f2f 6831 2229 0a0a 322e 2045 7874 7261  //h1")..2. Extra
-00008430: 6374 2074 6865 2074 6578 7420 6f66 2061  ct the text of a
-00008440: 6c6c 2060 603c 6831 3e60 6020 656c 656d  ll ``<h1>`` elem
-00008450: 656e 7473 2066 726f 6d20 616e 2048 544d  ents from an HTM
-00008460: 4c20 7265 7370 6f6e 7365 2062 6f64 792c  L response body,
-00008470: 0a20 2020 7265 7475 726e 696e 6720 6120  .   returning a 
-00008480: 6c69 7374 206f 6620 7374 7269 6e67 733a  list of strings:
-00008490: 3a0a 0a20 2020 2020 2073 656c 2e78 7061  :..      sel.xpa
-000084a0: 7468 2822 2f2f 6831 2229 2e67 6574 616c  th("//h1").getal
-000084b0: 6c28 2920 2020 2020 2020 2020 2320 7468  l()         # th
-000084c0: 6973 2069 6e63 6c75 6465 7320 7468 6520  is includes the 
-000084d0: 6831 2074 6167 0a20 2020 2020 2073 656c  h1 tag.      sel
-000084e0: 2e78 7061 7468 2822 2f2f 6831 2f74 6578  .xpath("//h1/tex
-000084f0: 7428 2922 292e 6765 7461 6c6c 2829 2020  t()").getall()  
-00008500: 2320 7468 6973 2065 7863 6c75 6465 7320  # this excludes 
-00008510: 7468 6520 6831 2074 6167 0a0a 332e 2049  the h1 tag..3. I
-00008520: 7465 7261 7465 206f 7665 7220 616c 6c20  terate over all 
-00008530: 6060 3c70 3e60 6020 7461 6773 2061 6e64  ``<p>`` tags and
-00008540: 2070 7269 6e74 2074 6865 6972 2063 6c61   print their cla
-00008550: 7373 2061 7474 7269 6275 7465 3a3a 0a0a  ss attribute::..
-00008560: 2020 2020 2020 666f 7220 6e6f 6465 2069        for node i
-00008570: 6e20 7365 6c2e 7870 6174 6828 222f 2f70  n sel.xpath("//p
-00008580: 2229 3a0a 2020 2020 2020 2020 2020 7072  "):.          pr
-00008590: 696e 7428 6e6f 6465 2e61 7474 7269 625b  int(node.attrib[
-000085a0: 2763 6c61 7373 275d 290a 0a0a 2e2e 205f  'class'])..... _
-000085b0: 7365 6c65 6374 6f72 2d65 7861 6d70 6c65  selector-example
-000085c0: 732d 786d 6c3a 0a0a 5365 6c65 6374 6f72  s-xml:..Selector
-000085d0: 2065 7861 6d70 6c65 7320 6f6e 2058 4d4c   examples on XML
-000085e0: 2072 6573 706f 6e73 650a 2d2d 2d2d 2d2d   response.------
-000085f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a48 6572  -----------..Her
-00008610: 6520 6172 6520 736f 6d65 2065 7861 6d70  e are some examp
-00008620: 6c65 7320 746f 2069 6c6c 7573 7472 6174  les to illustrat
-00008630: 6520 636f 6e63 6570 7473 2066 6f72 203a  e concepts for :
-00008640: 636c 6173 733a 6053 656c 6563 746f 7260  class:`Selector`
-00008650: 206f 626a 6563 7473 0a69 6e73 7461 6e74   objects.instant
-00008660: 6961 7465 6420 7769 7468 2061 6e20 3a63  iated with an :c
-00008670: 6c61 7373 3a60 7e73 6372 6170 792e 6874  lass:`~scrapy.ht
-00008680: 7470 2e58 6d6c 5265 7370 6f6e 7365 6020  tp.XmlResponse` 
-00008690: 6f62 6a65 6374 3a3a 0a0a 2020 2020 2020  object::..      
-000086a0: 7365 6c20 3d20 5365 6c65 6374 6f72 2878  sel = Selector(x
-000086b0: 6d6c 5f72 6573 706f 6e73 6529 0a0a 312e  ml_response)..1.
-000086c0: 2053 656c 6563 7420 616c 6c20 6060 3c70   Select all ``<p
-000086d0: 726f 6475 6374 3e60 6020 656c 656d 656e  roduct>`` elemen
-000086e0: 7473 2066 726f 6d20 616e 2058 4d4c 2072  ts from an XML r
-000086f0: 6573 706f 6e73 6520 626f 6479 2c20 7265  esponse body, re
-00008700: 7475 726e 696e 6720 6120 6c69 7374 0a20  turning a list. 
-00008710: 2020 6f66 203a 636c 6173 733a 6053 656c    of :class:`Sel
-00008720: 6563 746f 7260 206f 626a 6563 7473 2028  ector` objects (
-00008730: 692e 652e 2061 203a 636c 6173 733a 6053  i.e. a :class:`S
-00008740: 656c 6563 746f 724c 6973 7460 206f 626a  electorList` obj
-00008750: 6563 7429 3a3a 0a0a 2020 2020 2020 7365  ect)::..      se
-00008760: 6c2e 7870 6174 6828 222f 2f70 726f 6475  l.xpath("//produ
-00008770: 6374 2229 0a0a 322e 2045 7874 7261 6374  ct")..2. Extract
-00008780: 2061 6c6c 2070 7269 6365 7320 6672 6f6d   all prices from
-00008790: 2061 2060 476f 6f67 6c65 2042 6173 6520   a `Google Base 
-000087a0: 584d 4c20 6665 6564 605f 2077 6869 6368  XML feed`_ which
-000087b0: 2072 6571 7569 7265 7320 7265 6769 7374   requires regist
-000087c0: 6572 696e 670a 2020 2061 206e 616d 6573  ering.   a names
-000087d0: 7061 6365 3a3a 0a0a 2020 2020 2020 7365  pace::..      se
-000087e0: 6c2e 7265 6769 7374 6572 5f6e 616d 6573  l.register_names
-000087f0: 7061 6365 2822 6722 2c20 2268 7474 703a  pace("g", "http:
-00008800: 2f2f 6261 7365 2e67 6f6f 676c 652e 636f  //base.google.co
-00008810: 6d2f 6e73 2f31 2e30 2229 0a20 2020 2020  m/ns/1.0").     
-00008820: 2073 656c 2e78 7061 7468 2822 2f2f 673a   sel.xpath("//g:
-00008830: 7072 6963 6522 292e 6765 7461 6c6c 2829  price").getall()
-00008840: 0a0a 2e2e 205f 476f 6f67 6c65 2042 6173  .... _Google Bas
-00008850: 6520 584d 4c20 6665 6564 3a20 6874 7470  e XML feed: http
-00008860: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
-00008870: 6c65 2e63 6f6d 2f6d 6572 6368 616e 7473  le.com/merchants
-00008880: 2f61 6e73 7765 722f 3136 3035 3839 3f68  /answer/160589?h
-00008890: 6c3d 656e 2672 6566 5f74 6f70 6963 3d32  l=en&ref_topic=2
-000088a0: 3437 3337 3939 0a                        473799.
+00000000: 2e2e 205f 746f 7069 6373 2d73 7069 6465  .. _topics-spide
+00000010: 7273 3a0a 0a3d 3d3d 3d3d 3d3d 0a53 7069  rs:..=======.Spi
+00000020: 6465 7273 0a3d 3d3d 3d3d 3d3d 0a0a 5370  ders.=======..Sp
+00000030: 6964 6572 7320 6172 6520 636c 6173 7365  iders are classe
+00000040: 7320 7768 6963 6820 6465 6669 6e65 2068  s which define h
+00000050: 6f77 2061 2063 6572 7461 696e 2073 6974  ow a certain sit
+00000060: 6520 286f 7220 6120 6772 6f75 7020 6f66  e (or a group of
+00000070: 2073 6974 6573 2920 7769 6c6c 2062 650a   sites) will be.
+00000080: 7363 7261 7065 642c 2069 6e63 6c75 6469  scraped, includi
+00000090: 6e67 2068 6f77 2074 6f20 7065 7266 6f72  ng how to perfor
+000000a0: 6d20 7468 6520 6372 6177 6c20 2869 2e65  m the crawl (i.e
+000000b0: 2e20 666f 6c6c 6f77 206c 696e 6b73 2920  . follow links) 
+000000c0: 616e 6420 686f 7720 746f 0a65 7874 7261  and how to.extra
+000000d0: 6374 2073 7472 7563 7475 7265 6420 6461  ct structured da
+000000e0: 7461 2066 726f 6d20 7468 6569 7220 7061  ta from their pa
+000000f0: 6765 7320 2869 2e65 2e20 7363 7261 7069  ges (i.e. scrapi
+00000100: 6e67 2069 7465 6d73 292e 2049 6e20 6f74  ng items). In ot
+00000110: 6865 7220 776f 7264 732c 0a53 7069 6465  her words,.Spide
+00000120: 7273 2061 7265 2074 6865 2070 6c61 6365  rs are the place
+00000130: 2077 6865 7265 2079 6f75 2064 6566 696e   where you defin
+00000140: 6520 7468 6520 6375 7374 6f6d 2062 6568  e the custom beh
+00000150: 6176 696f 7572 2066 6f72 2063 7261 776c  aviour for crawl
+00000160: 696e 6720 616e 640a 7061 7273 696e 6720  ing and.parsing 
+00000170: 7061 6765 7320 666f 7220 6120 7061 7274  pages for a part
+00000180: 6963 756c 6172 2073 6974 6520 286f 722c  icular site (or,
+00000190: 2069 6e20 736f 6d65 2063 6173 6573 2c20   in some cases, 
+000001a0: 6120 6772 6f75 7020 6f66 2073 6974 6573  a group of sites
+000001b0: 292e 0a0a 466f 7220 7370 6964 6572 732c  )...For spiders,
+000001c0: 2074 6865 2073 6372 6170 696e 6720 6379   the scraping cy
+000001d0: 636c 6520 676f 6573 2074 6872 6f75 6768  cle goes through
+000001e0: 2073 6f6d 6574 6869 6e67 206c 696b 6520   something like 
+000001f0: 7468 6973 3a0a 0a31 2e20 596f 7520 7374  this:..1. You st
+00000200: 6172 7420 6279 2067 656e 6572 6174 696e  art by generatin
+00000210: 6720 7468 6520 696e 6974 6961 6c20 5265  g the initial Re
+00000220: 7175 6573 7473 2074 6f20 6372 6177 6c20  quests to crawl 
+00000230: 7468 6520 6669 7273 7420 5552 4c73 2c20  the first URLs, 
+00000240: 616e 640a 2020 2073 7065 6369 6679 2061  and.   specify a
+00000250: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
+00000260: 6f6e 2074 6f20 6265 2063 616c 6c65 6420  on to be called 
+00000270: 7769 7468 2074 6865 2072 6573 706f 6e73  with the respons
+00000280: 6520 646f 776e 6c6f 6164 6564 2066 726f  e downloaded fro
+00000290: 6d0a 2020 2074 686f 7365 2072 6571 7565  m.   those reque
+000002a0: 7374 732e 0a0a 2020 2054 6865 2066 6972  sts...   The fir
+000002b0: 7374 2072 6571 7565 7374 7320 746f 2070  st requests to p
+000002c0: 6572 666f 726d 2061 7265 206f 6274 6169  erform are obtai
+000002d0: 6e65 6420 6279 2063 616c 6c69 6e67 2074  ned by calling t
+000002e0: 6865 0a20 2020 3a6d 6574 683a 607e 7363  he.   :meth:`~sc
+000002f0: 7261 7079 2e53 7069 6465 722e 7374 6172  rapy.Spider.star
+00000300: 745f 7265 7175 6573 7473 6020 6d65 7468  t_requests` meth
+00000310: 6f64 2077 6869 6368 2028 6279 2064 6566  od which (by def
+00000320: 6175 6c74 290a 2020 2067 656e 6572 6174  ault).   generat
+00000330: 6573 203a 636c 6173 733a 607e 7363 7261  es :class:`~scra
+00000340: 7079 2e52 6571 7565 7374 6020 666f 7220  py.Request` for 
+00000350: 7468 6520 5552 4c73 2073 7065 6369 6669  the URLs specifi
+00000360: 6564 2069 6e20 7468 650a 2020 203a 6174  ed in the.   :at
+00000370: 7472 3a60 7e73 6372 6170 792e 5370 6964  tr:`~scrapy.Spid
+00000380: 6572 2e73 7461 7274 5f75 726c 7360 2061  er.start_urls` a
+00000390: 6e64 2074 6865 0a20 2020 3a61 7474 723a  nd the.   :attr:
+000003a0: 607e 7363 7261 7079 2e53 7069 6465 722e  `~scrapy.Spider.
+000003b0: 7061 7273 6560 206d 6574 686f 6420 6173  parse` method as
+000003c0: 2063 616c 6c62 6163 6b20 6675 6e63 7469   callback functi
+000003d0: 6f6e 2066 6f72 2074 6865 0a20 2020 5265  on for the.   Re
+000003e0: 7175 6573 7473 2e0a 0a32 2e20 496e 2074  quests...2. In t
+000003f0: 6865 2063 616c 6c62 6163 6b20 6675 6e63  he callback func
+00000400: 7469 6f6e 2c20 796f 7520 7061 7273 6520  tion, you parse 
+00000410: 7468 6520 7265 7370 6f6e 7365 2028 7765  the response (we
+00000420: 6220 7061 6765 2920 616e 6420 7265 7475  b page) and retu
+00000430: 726e 0a20 2020 3a72 6566 3a60 6974 656d  rn.   :ref:`item
+00000440: 206f 626a 6563 7473 203c 746f 7069 6373   objects <topics
+00000450: 2d69 7465 6d73 3e60 2c0a 2020 203a 636c  -items>`,.   :cl
+00000460: 6173 733a 607e 7363 7261 7079 2e52 6571  ass:`~scrapy.Req
+00000470: 7565 7374 6020 6f62 6a65 6374 732c 206f  uest` objects, o
+00000480: 7220 616e 2069 7465 7261 626c 6520 6f66  r an iterable of
+00000490: 2074 6865 7365 206f 626a 6563 7473 2e0a   these objects..
+000004a0: 2020 2054 686f 7365 2052 6571 7565 7374     Those Request
+000004b0: 7320 7769 6c6c 2061 6c73 6f20 636f 6e74  s will also cont
+000004c0: 6169 6e20 6120 6361 6c6c 6261 636b 2028  ain a callback (
+000004d0: 6d61 7962 650a 2020 2074 6865 2073 616d  maybe.   the sam
+000004e0: 6529 2061 6e64 2077 696c 6c20 7468 656e  e) and will then
+000004f0: 2062 6520 646f 776e 6c6f 6164 6564 2062   be downloaded b
+00000500: 7920 5363 7261 7079 2061 6e64 2074 6865  y Scrapy and the
+00000510: 6e20 7468 6569 720a 2020 2072 6573 706f  n their.   respo
+00000520: 6e73 6520 6861 6e64 6c65 6420 6279 2074  nse handled by t
+00000530: 6865 2073 7065 6369 6669 6564 2063 616c  he specified cal
+00000540: 6c62 6163 6b2e 0a0a 332e 2049 6e20 6361  lback...3. In ca
+00000550: 6c6c 6261 636b 2066 756e 6374 696f 6e73  llback functions
+00000560: 2c20 796f 7520 7061 7273 6520 7468 6520  , you parse the 
+00000570: 7061 6765 2063 6f6e 7465 6e74 732c 2074  page contents, t
+00000580: 7970 6963 616c 6c79 2075 7369 6e67 0a20  ypically using. 
+00000590: 2020 3a72 6566 3a60 746f 7069 6373 2d73    :ref:`topics-s
+000005a0: 656c 6563 746f 7273 6020 2862 7574 2079  electors` (but y
+000005b0: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
+000005c0: 4265 6175 7469 6675 6c53 6f75 702c 206c  BeautifulSoup, l
+000005d0: 786d 6c20 6f72 2077 6861 7465 7665 720a  xml or whatever.
+000005e0: 2020 206d 6563 6861 6e69 736d 2079 6f75     mechanism you
+000005f0: 2070 7265 6665 7229 2061 6e64 2067 656e   prefer) and gen
+00000600: 6572 6174 6520 6974 656d 7320 7769 7468  erate items with
+00000610: 2074 6865 2070 6172 7365 6420 6461 7461   the parsed data
+00000620: 2e0a 0a34 2e20 4669 6e61 6c6c 792c 2074  ...4. Finally, t
+00000630: 6865 2069 7465 6d73 2072 6574 7572 6e65  he items returne
+00000640: 6420 6672 6f6d 2074 6865 2073 7069 6465  d from the spide
+00000650: 7220 7769 6c6c 2062 6520 7479 7069 6361  r will be typica
+00000660: 6c6c 7920 7065 7273 6973 7465 6420 746f  lly persisted to
+00000670: 2061 0a20 2020 6461 7461 6261 7365 2028   a.   database (
+00000680: 696e 2073 6f6d 6520 3a72 6566 3a60 4974  in some :ref:`It
+00000690: 656d 2050 6970 656c 696e 6520 3c74 6f70  em Pipeline <top
+000006a0: 6963 732d 6974 656d 2d70 6970 656c 696e  ics-item-pipelin
+000006b0: 653e 6029 206f 7220 7772 6974 7465 6e20  e>`) or written 
+000006c0: 746f 0a20 2020 6120 6669 6c65 2075 7369  to.   a file usi
+000006d0: 6e67 203a 7265 663a 6074 6f70 6963 732d  ng :ref:`topics-
+000006e0: 6665 6564 2d65 7870 6f72 7473 602e 0a0a  feed-exports`...
+000006f0: 4576 656e 2074 686f 7567 6820 7468 6973  Even though this
+00000700: 2063 7963 6c65 2061 7070 6c69 6573 2028   cycle applies (
+00000710: 6d6f 7265 206f 7220 6c65 7373 2920 746f  more or less) to
+00000720: 2061 6e79 206b 696e 6420 6f66 2073 7069   any kind of spi
+00000730: 6465 722c 2074 6865 7265 2061 7265 0a64  der, there are.d
+00000740: 6966 6665 7265 6e74 206b 696e 6473 206f  ifferent kinds o
+00000750: 6620 6465 6661 756c 7420 7370 6964 6572  f default spider
+00000760: 7320 6275 6e64 6c65 6420 696e 746f 2053  s bundled into S
+00000770: 6372 6170 7920 666f 7220 6469 6666 6572  crapy for differ
+00000780: 656e 7420 7075 7270 6f73 6573 2e0a 5765  ent purposes..We
+00000790: 2077 696c 6c20 7461 6c6b 2061 626f 7574   will talk about
+000007a0: 2074 686f 7365 2074 7970 6573 2068 6572   those types her
+000007b0: 652e 0a0a 2e2e 205f 746f 7069 6373 2d73  e..... _topics-s
+000007c0: 7069 6465 7273 2d72 6566 3a0a 0a73 6372  piders-ref:..scr
+000007d0: 6170 792e 5370 6964 6572 0a3d 3d3d 3d3d  apy.Spider.=====
+000007e0: 3d3d 3d3d 3d3d 3d3d 0a0a 2e2e 2063 6c61  ========.... cla
+000007f0: 7373 3a3a 2073 6372 6170 792e 7370 6964  ss:: scrapy.spid
+00000800: 6572 732e 5370 6964 6572 0a2e 2e20 636c  ers.Spider... cl
+00000810: 6173 733a 3a20 7363 7261 7079 2e53 7069  ass:: scrapy.Spi
+00000820: 6465 7228 290a 0a20 2020 5468 6973 2069  der()..   This i
+00000830: 7320 7468 6520 7369 6d70 6c65 7374 2073  s the simplest s
+00000840: 7069 6465 722c 2061 6e64 2074 6865 206f  pider, and the o
+00000850: 6e65 2066 726f 6d20 7768 6963 6820 6576  ne from which ev
+00000860: 6572 7920 6f74 6865 7220 7370 6964 6572  ery other spider
+00000870: 0a20 2020 6d75 7374 2069 6e68 6572 6974  .   must inherit
+00000880: 2028 696e 636c 7564 696e 6720 7370 6964   (including spid
+00000890: 6572 7320 7468 6174 2063 6f6d 6520 6275  ers that come bu
+000008a0: 6e64 6c65 6420 7769 7468 2053 6372 6170  ndled with Scrap
+000008b0: 792c 2061 7320 7765 6c6c 2061 7320 7370  y, as well as sp
+000008c0: 6964 6572 730a 2020 2074 6861 7420 796f  iders.   that yo
+000008d0: 7520 7772 6974 6520 796f 7572 7365 6c66  u write yourself
+000008e0: 292e 2049 7420 646f 6573 6e27 7420 7072  ). It doesn't pr
+000008f0: 6f76 6964 6520 616e 7920 7370 6563 6961  ovide any specia
+00000900: 6c20 6675 6e63 7469 6f6e 616c 6974 792e  l functionality.
+00000910: 2049 7420 6a75 7374 0a20 2020 7072 6f76   It just.   prov
+00000920: 6964 6573 2061 2064 6566 6175 6c74 203a  ides a default :
+00000930: 6d65 7468 3a60 7374 6172 745f 7265 7175  meth:`start_requ
+00000940: 6573 7473 6020 696d 706c 656d 656e 7461  ests` implementa
+00000950: 7469 6f6e 2077 6869 6368 2073 656e 6473  tion which sends
+00000960: 2072 6571 7565 7374 7320 6672 6f6d 0a20   requests from. 
+00000970: 2020 7468 6520 3a61 7474 723a 6073 7461    the :attr:`sta
+00000980: 7274 5f75 726c 7360 2073 7069 6465 7220  rt_urls` spider 
+00000990: 6174 7472 6962 7574 6520 616e 6420 6361  attribute and ca
+000009a0: 6c6c 7320 7468 6520 7370 6964 6572 2773  lls the spider's
+000009b0: 206d 6574 686f 6420 6060 7061 7273 6560   method ``parse`
+000009c0: 600a 2020 2066 6f72 2065 6163 6820 6f66  `.   for each of
+000009d0: 2074 6865 2072 6573 756c 7469 6e67 2072   the resulting r
+000009e0: 6573 706f 6e73 6573 2e0a 0a20 2020 2e2e  esponses...   ..
+000009f0: 2061 7474 7269 6275 7465 3a3a 206e 616d   attribute:: nam
+00000a00: 650a 0a20 2020 2020 2020 4120 7374 7269  e..       A stri
+00000a10: 6e67 2077 6869 6368 2064 6566 696e 6573  ng which defines
+00000a20: 2074 6865 206e 616d 6520 666f 7220 7468   the name for th
+00000a30: 6973 2073 7069 6465 722e 2054 6865 2073  is spider. The s
+00000a40: 7069 6465 7220 6e61 6d65 2069 7320 686f  pider name is ho
+00000a50: 770a 2020 2020 2020 2074 6865 2073 7069  w.       the spi
+00000a60: 6465 7220 6973 206c 6f63 6174 6564 2028  der is located (
+00000a70: 616e 6420 696e 7374 616e 7469 6174 6564  and instantiated
+00000a80: 2920 6279 2053 6372 6170 792c 2073 6f20  ) by Scrapy, so 
+00000a90: 6974 206d 7573 7420 6265 0a20 2020 2020  it must be.     
+00000aa0: 2020 756e 6971 7565 2e20 486f 7765 7665    unique. Howeve
+00000ab0: 722c 206e 6f74 6869 6e67 2070 7265 7665  r, nothing preve
+00000ac0: 6e74 7320 796f 7520 6672 6f6d 2069 6e73  nts you from ins
+00000ad0: 7461 6e74 6961 7469 6e67 206d 6f72 6520  tantiating more 
+00000ae0: 7468 616e 206f 6e65 0a20 2020 2020 2020  than one.       
+00000af0: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
+00000b00: 7361 6d65 2073 7069 6465 722e 2054 6869  same spider. Thi
+00000b10: 7320 6973 2074 6865 206d 6f73 7420 696d  s is the most im
+00000b20: 706f 7274 616e 7420 7370 6964 6572 2061  portant spider a
+00000b30: 7474 7269 6275 7465 0a20 2020 2020 2020  ttribute.       
+00000b40: 616e 6420 6974 2773 2072 6571 7569 7265  and it's require
+00000b50: 642e 0a0a 2020 2020 2020 2049 6620 7468  d...       If th
+00000b60: 6520 7370 6964 6572 2073 6372 6170 6573  e spider scrapes
+00000b70: 2061 2073 696e 676c 6520 646f 6d61 696e   a single domain
+00000b80: 2c20 6120 636f 6d6d 6f6e 2070 7261 6374  , a common pract
+00000b90: 6963 6520 6973 2074 6f20 6e61 6d65 2074  ice is to name t
+00000ba0: 6865 0a20 2020 2020 2020 7370 6964 6572  he.       spider
+00000bb0: 2061 6674 6572 2074 6865 2064 6f6d 6169   after the domai
+00000bc0: 6e2c 2077 6974 6820 6f72 2077 6974 686f  n, with or witho
+00000bd0: 7574 2074 6865 2060 544c 4460 5f2e 2053  ut the `TLD`_. S
+00000be0: 6f2c 2066 6f72 2065 7861 6d70 6c65 2c20  o, for example, 
+00000bf0: 610a 2020 2020 2020 2073 7069 6465 7220  a.       spider 
+00000c00: 7468 6174 2063 7261 776c 7320 6060 6d79  that crawls ``my
+00000c10: 7765 6273 6974 652e 636f 6d60 6020 776f  website.com`` wo
+00000c20: 756c 6420 6f66 7465 6e20 6265 2063 616c  uld often be cal
+00000c30: 6c65 640a 2020 2020 2020 2060 606d 7977  led.       ``myw
+00000c40: 6562 7369 7465 6060 2e0a 0a20 2020 2e2e  ebsite``...   ..
+00000c50: 2061 7474 7269 6275 7465 3a3a 2061 6c6c   attribute:: all
+00000c60: 6f77 6564 5f64 6f6d 6169 6e73 0a0a 2020  owed_domains..  
+00000c70: 2020 2020 2041 6e20 6f70 7469 6f6e 616c       An optional
+00000c80: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
+00000c90: 2063 6f6e 7461 696e 696e 6720 646f 6d61   containing doma
+00000ca0: 696e 7320 7468 6174 2074 6869 7320 7370  ins that this sp
+00000cb0: 6964 6572 2069 730a 2020 2020 2020 2061  ider is.       a
+00000cc0: 6c6c 6f77 6564 2074 6f20 6372 6177 6c2e  llowed to crawl.
+00000cd0: 2052 6571 7565 7374 7320 666f 7220 5552   Requests for UR
+00000ce0: 4c73 206e 6f74 2062 656c 6f6e 6769 6e67  Ls not belonging
+00000cf0: 2074 6f20 7468 6520 646f 6d61 696e 206e   to the domain n
+00000d00: 616d 6573 0a20 2020 2020 2020 7370 6563  ames.       spec
+00000d10: 6966 6965 6420 696e 2074 6869 7320 6c69  ified in this li
+00000d20: 7374 2028 6f72 2074 6865 6972 2073 7562  st (or their sub
+00000d30: 646f 6d61 696e 7329 2077 6f6e 2774 2062  domains) won't b
+00000d40: 6520 666f 6c6c 6f77 6564 2069 660a 2020  e followed if.  
+00000d50: 2020 2020 203a 636c 6173 733a 607e 7363       :class:`~sc
+00000d60: 7261 7079 2e73 7069 6465 726d 6964 646c  rapy.spidermiddl
+00000d70: 6577 6172 6573 2e6f 6666 7369 7465 2e4f  ewares.offsite.O
+00000d80: 6666 7369 7465 4d69 6464 6c65 7761 7265  ffsiteMiddleware
+00000d90: 6020 6973 2065 6e61 626c 6564 2e0a 0a20  ` is enabled... 
+00000da0: 2020 2020 2020 4c65 7427 7320 7361 7920        Let's say 
+00000db0: 796f 7572 2074 6172 6765 7420 7572 6c20  your target url 
+00000dc0: 6973 2060 6068 7474 7073 3a2f 2f77 7777  is ``https://www
+00000dd0: 2e65 7861 6d70 6c65 2e63 6f6d 2f31 2e68  .example.com/1.h
+00000de0: 746d 6c60 602c 0a20 2020 2020 2020 7468  tml``,.       th
+00000df0: 656e 2061 6464 2060 6027 6578 616d 706c  en add ``'exampl
+00000e00: 652e 636f 6d27 6060 2074 6f20 7468 6520  e.com'`` to the 
+00000e10: 6c69 7374 2e0a 0a20 2020 2e2e 2061 7474  list...   .. att
+00000e20: 7269 6275 7465 3a3a 2073 7461 7274 5f75  ribute:: start_u
+00000e30: 726c 730a 0a20 2020 2020 2020 4120 6c69  rls..       A li
+00000e40: 7374 206f 6620 5552 4c73 2077 6865 7265  st of URLs where
+00000e50: 2074 6865 2073 7069 6465 7220 7769 6c6c   the spider will
+00000e60: 2062 6567 696e 2074 6f20 6372 6177 6c20   begin to crawl 
+00000e70: 6672 6f6d 2c20 7768 656e 206e 6f0a 2020  from, when no.  
+00000e80: 2020 2020 2070 6172 7469 6375 6c61 7220       particular 
+00000e90: 5552 4c73 2061 7265 2073 7065 6369 6669  URLs are specifi
+00000ea0: 6564 2e20 536f 2c20 7468 6520 6669 7273  ed. So, the firs
+00000eb0: 7420 7061 6765 7320 646f 776e 6c6f 6164  t pages download
+00000ec0: 6564 2077 696c 6c20 6265 2074 686f 7365  ed will be those
+00000ed0: 0a20 2020 2020 2020 6c69 7374 6564 2068  .       listed h
+00000ee0: 6572 652e 2054 6865 2073 7562 7365 7175  ere. The subsequ
+00000ef0: 656e 7420 3a63 6c61 7373 3a60 7e73 6372  ent :class:`~scr
+00000f00: 6170 792e 5265 7175 6573 7460 2077 696c  apy.Request` wil
+00000f10: 6c20 6265 2067 656e 6572 6174 6564 2073  l be generated s
+00000f20: 7563 6365 7373 6976 656c 7920 6672 6f6d  uccessively from
+00000f30: 2064 6174 610a 2020 2020 2020 2063 6f6e   data.       con
+00000f40: 7461 696e 6564 2069 6e20 7468 6520 7374  tained in the st
+00000f50: 6172 7420 5552 4c73 2e0a 0a20 2020 2e2e  art URLs...   ..
+00000f60: 2061 7474 7269 6275 7465 3a3a 2063 7573   attribute:: cus
+00000f70: 746f 6d5f 7365 7474 696e 6773 0a0a 2020  tom_settings..  
+00000f80: 2020 2020 4120 6469 6374 696f 6e61 7279      A dictionary
+00000f90: 206f 6620 7365 7474 696e 6773 2074 6861   of settings tha
+00000fa0: 7420 7769 6c6c 2062 6520 6f76 6572 7269  t will be overri
+00000fb0: 6464 656e 2066 726f 6d20 7468 6520 7072  dden from the pr
+00000fc0: 6f6a 6563 7420 7769 6465 0a20 2020 2020  oject wide.     
+00000fd0: 2063 6f6e 6669 6775 7261 7469 6f6e 2077   configuration w
+00000fe0: 6865 6e20 7275 6e6e 696e 6720 7468 6973  hen running this
+00000ff0: 2073 7069 6465 722e 2049 7420 6d75 7374   spider. It must
+00001000: 2062 6520 6465 6669 6e65 6420 6173 2061   be defined as a
+00001010: 2063 6c61 7373 0a20 2020 2020 2061 7474   class.      att
+00001020: 7269 6275 7465 2073 696e 6365 2074 6865  ribute since the
+00001030: 2073 6574 7469 6e67 7320 6172 6520 7570   settings are up
+00001040: 6461 7465 6420 6265 666f 7265 2069 6e73  dated before ins
+00001050: 7461 6e74 6961 7469 6f6e 2e0a 0a20 2020  tantiation...   
+00001060: 2020 2046 6f72 2061 206c 6973 7420 6f66     For a list of
+00001070: 2061 7661 696c 6162 6c65 2062 7569 6c74   available built
+00001080: 2d69 6e20 7365 7474 696e 6773 2073 6565  -in settings see
+00001090: 3a0a 2020 2020 2020 3a72 6566 3a60 746f  :.      :ref:`to
+000010a0: 7069 6373 2d73 6574 7469 6e67 732d 7265  pics-settings-re
+000010b0: 6660 2e0a 0a20 2020 2e2e 2061 7474 7269  f`...   .. attri
+000010c0: 6275 7465 3a3a 2063 7261 776c 6572 0a0a  bute:: crawler..
+000010d0: 2020 2020 2020 5468 6973 2061 7474 7269        This attri
+000010e0: 6275 7465 2069 7320 7365 7420 6279 2074  bute is set by t
+000010f0: 6865 203a 6d65 7468 3a60 6672 6f6d 5f63  he :meth:`from_c
+00001100: 7261 776c 6572 6020 636c 6173 7320 6d65  rawler` class me
+00001110: 7468 6f64 2061 6674 6572 0a20 2020 2020  thod after.     
+00001120: 2069 6e69 7469 616c 697a 696e 6720 7468   initializing th
+00001130: 6520 636c 6173 732c 2061 6e64 206c 696e  e class, and lin
+00001140: 6b73 2074 6f20 7468 650a 2020 2020 2020  ks to the.      
+00001150: 3a63 6c61 7373 3a60 7e73 6372 6170 792e  :class:`~scrapy.
+00001160: 6372 6177 6c65 722e 4372 6177 6c65 7260  crawler.Crawler`
+00001170: 206f 626a 6563 7420 746f 2077 6869 6368   object to which
+00001180: 2074 6869 7320 7370 6964 6572 2069 6e73   this spider ins
+00001190: 7461 6e63 6520 6973 0a20 2020 2020 2062  tance is.      b
+000011a0: 6f75 6e64 2e0a 0a20 2020 2020 2043 7261  ound...      Cra
+000011b0: 776c 6572 7320 656e 6361 7073 756c 6174  wlers encapsulat
+000011c0: 6520 6120 6c6f 7420 6f66 2063 6f6d 706f  e a lot of compo
+000011d0: 6e65 6e74 7320 696e 2074 6865 2070 726f  nents in the pro
+000011e0: 6a65 6374 2066 6f72 2074 6865 6972 2073  ject for their s
+000011f0: 696e 676c 650a 2020 2020 2020 656e 7472  ingle.      entr
+00001200: 7920 6163 6365 7373 2028 7375 6368 2061  y access (such a
+00001210: 7320 6578 7465 6e73 696f 6e73 2c20 6d69  s extensions, mi
+00001220: 6464 6c65 7761 7265 732c 2073 6967 6e61  ddlewares, signa
+00001230: 6c73 206d 616e 6167 6572 732c 2065 7463  ls managers, etc
+00001240: 292e 0a20 2020 2020 2053 6565 203a 7265  )..      See :re
+00001250: 663a 6074 6f70 6963 732d 6170 692d 6372  f:`topics-api-cr
+00001260: 6177 6c65 7260 2074 6f20 6b6e 6f77 206d  awler` to know m
+00001270: 6f72 6520 6162 6f75 7420 7468 656d 2e0a  ore about them..
+00001280: 0a20 2020 2e2e 2061 7474 7269 6275 7465  .   .. attribute
+00001290: 3a3a 2073 6574 7469 6e67 730a 0a20 2020  :: settings..   
+000012a0: 2020 2043 6f6e 6669 6775 7261 7469 6f6e     Configuration
+000012b0: 2066 6f72 2072 756e 6e69 6e67 2074 6869   for running thi
+000012c0: 7320 7370 6964 6572 2e20 5468 6973 2069  s spider. This i
+000012d0: 7320 610a 2020 2020 2020 3a63 6c61 7373  s a.      :class
+000012e0: 3a60 7e73 6372 6170 792e 7365 7474 696e  :`~scrapy.settin
+000012f0: 6773 2e53 6574 7469 6e67 7360 2069 6e73  gs.Settings` ins
+00001300: 7461 6e63 652c 2073 6565 2074 6865 0a20  tance, see the. 
+00001310: 2020 2020 203a 7265 663a 6074 6f70 6963       :ref:`topic
+00001320: 732d 7365 7474 696e 6773 6020 746f 7069  s-settings` topi
+00001330: 6320 666f 7220 6120 6465 7461 696c 6564  c for a detailed
+00001340: 2069 6e74 726f 6475 6374 696f 6e20 6f6e   introduction on
+00001350: 2074 6869 7320 7375 626a 6563 742e 0a0a   this subject...
+00001360: 2020 202e 2e20 6174 7472 6962 7574 653a     .. attribute:
+00001370: 3a20 6c6f 6767 6572 0a0a 2020 2020 2020  : logger..      
+00001380: 5079 7468 6f6e 206c 6f67 6765 7220 6372  Python logger cr
+00001390: 6561 7465 6420 7769 7468 2074 6865 2053  eated with the S
+000013a0: 7069 6465 7227 7320 3a61 7474 723a 606e  pider's :attr:`n
+000013b0: 616d 6560 2e20 596f 7520 6361 6e20 7573  ame`. You can us
+000013c0: 6520 6974 2074 6f0a 2020 2020 2020 7365  e it to.      se
+000013d0: 6e64 206c 6f67 206d 6573 7361 6765 7320  nd log messages 
+000013e0: 7468 726f 7567 6820 6974 2061 7320 6465  through it as de
+000013f0: 7363 7269 6265 6420 6f6e 0a20 2020 2020  scribed on.     
+00001400: 203a 7265 663a 6074 6f70 6963 732d 6c6f   :ref:`topics-lo
+00001410: 6767 696e 672d 6672 6f6d 2d73 7069 6465  gging-from-spide
+00001420: 7273 602e 0a0a 2020 202e 2e20 6174 7472  rs`...   .. attr
+00001430: 6962 7574 653a 3a20 7374 6174 650a 0a20  ibute:: state.. 
+00001440: 2020 2020 2041 2064 6963 7420 796f 7520       A dict you 
+00001450: 6361 6e20 7573 6520 746f 2070 6572 7369  can use to persi
+00001460: 7374 2073 6f6d 6520 7370 6964 6572 2073  st some spider s
+00001470: 7461 7465 2062 6574 7765 656e 2062 6174  tate between bat
+00001480: 6368 6573 2e0a 2020 2020 2020 5365 6520  ches..      See 
+00001490: 3a72 6566 3a60 746f 7069 6373 2d6b 6565  :ref:`topics-kee
+000014a0: 7069 6e67 2d70 6572 7369 7374 656e 742d  ping-persistent-
+000014b0: 7374 6174 652d 6265 7477 6565 6e2d 6261  state-between-ba
+000014c0: 7463 6865 7360 2074 6f20 6b6e 6f77 206d  tches` to know m
+000014d0: 6f72 6520 6162 6f75 7420 6974 2e0a 0a20  ore about it... 
+000014e0: 2020 2e2e 206d 6574 686f 643a 3a20 6672    .. method:: fr
+000014f0: 6f6d 5f63 7261 776c 6572 2863 7261 776c  om_crawler(crawl
+00001500: 6572 2c20 2a61 7267 732c 202a 2a6b 7761  er, *args, **kwa
+00001510: 7267 7329 0a0a 2020 2020 2020 2054 6869  rgs)..       Thi
+00001520: 7320 6973 2074 6865 2063 6c61 7373 206d  s is the class m
+00001530: 6574 686f 6420 7573 6564 2062 7920 5363  ethod used by Sc
+00001540: 7261 7079 2074 6f20 6372 6561 7465 2079  rapy to create y
+00001550: 6f75 7220 7370 6964 6572 732e 0a0a 2020  our spiders...  
+00001560: 2020 2020 2059 6f75 2070 726f 6261 626c       You probabl
+00001570: 7920 776f 6e27 7420 6e65 6564 2074 6f20  y won't need to 
+00001580: 6f76 6572 7269 6465 2074 6869 7320 6469  override this di
+00001590: 7265 6374 6c79 2062 6563 6175 7365 2074  rectly because t
+000015a0: 6865 2064 6566 6175 6c74 0a20 2020 2020  he default.     
+000015b0: 2020 696d 706c 656d 656e 7461 7469 6f6e    implementation
+000015c0: 2061 6374 7320 6173 2061 2070 726f 7879   acts as a proxy
+000015d0: 2074 6f20 7468 6520 3a6d 6574 683a 605f   to the :meth:`_
+000015e0: 5f69 6e69 745f 5f60 206d 6574 686f 642c  _init__` method,
+000015f0: 2063 616c 6c69 6e67 0a20 2020 2020 2020   calling.       
+00001600: 6974 2077 6974 6820 7468 6520 6769 7665  it with the give
+00001610: 6e20 6172 6775 6d65 6e74 7320 6060 6172  n arguments ``ar
+00001620: 6773 6060 2061 6e64 206e 616d 6564 2061  gs`` and named a
+00001630: 7267 756d 656e 7473 2060 606b 7761 7267  rguments ``kwarg
+00001640: 7360 602e 0a0a 2020 2020 2020 204e 6f6e  s``...       Non
+00001650: 6574 6865 6c65 7373 2c20 7468 6973 206d  etheless, this m
+00001660: 6574 686f 6420 7365 7473 2074 6865 203a  ethod sets the :
+00001670: 6174 7472 3a60 6372 6177 6c65 7260 2061  attr:`crawler` a
+00001680: 6e64 203a 6174 7472 3a60 7365 7474 696e  nd :attr:`settin
+00001690: 6773 600a 2020 2020 2020 2061 7474 7269  gs`.       attri
+000016a0: 6275 7465 7320 696e 2074 6865 206e 6577  butes in the new
+000016b0: 2069 6e73 7461 6e63 6520 736f 2074 6865   instance so the
+000016c0: 7920 6361 6e20 6265 2061 6363 6573 7365  y can be accesse
+000016d0: 6420 6c61 7465 7220 696e 7369 6465 2074  d later inside t
+000016e0: 6865 0a20 2020 2020 2020 7370 6964 6572  he.       spider
+000016f0: 2773 2063 6f64 652e 0a0a 2020 2020 2020  's code...      
+00001700: 203a 7061 7261 6d20 6372 6177 6c65 723a   :param crawler:
+00001710: 2063 7261 776c 6572 2074 6f20 7768 6963   crawler to whic
+00001720: 6820 7468 6520 7370 6964 6572 2077 696c  h the spider wil
+00001730: 6c20 6265 2062 6f75 6e64 0a20 2020 2020  l be bound.     
+00001740: 2020 3a74 7970 6520 6372 6177 6c65 723a    :type crawler:
+00001750: 203a 636c 6173 733a 607e 7363 7261 7079   :class:`~scrapy
+00001760: 2e63 7261 776c 6572 2e43 7261 776c 6572  .crawler.Crawler
+00001770: 6020 696e 7374 616e 6365 0a0a 2020 2020  ` instance..    
+00001780: 2020 203a 7061 7261 6d20 6172 6773 3a20     :param args: 
+00001790: 6172 6775 6d65 6e74 7320 7061 7373 6564  arguments passed
+000017a0: 2074 6f20 7468 6520 3a6d 6574 683a 605f   to the :meth:`_
+000017b0: 5f69 6e69 745f 5f60 206d 6574 686f 640a  _init__` method.
+000017c0: 2020 2020 2020 203a 7479 7065 2061 7267         :type arg
+000017d0: 733a 206c 6973 740a 0a20 2020 2020 2020  s: list..       
+000017e0: 3a70 6172 616d 206b 7761 7267 733a 206b  :param kwargs: k
+000017f0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+00001800: 2070 6173 7365 6420 746f 2074 6865 203a   passed to the :
+00001810: 6d65 7468 3a60 5f5f 696e 6974 5f5f 6020  meth:`__init__` 
+00001820: 6d65 7468 6f64 0a20 2020 2020 2020 3a74  method.       :t
+00001830: 7970 6520 6b77 6172 6773 3a20 6469 6374  ype kwargs: dict
+00001840: 0a0a 2020 202e 2e20 6d65 7468 6f64 3a3a  ..   .. method::
+00001850: 2073 7461 7274 5f72 6571 7565 7374 7328   start_requests(
+00001860: 290a 0a20 2020 2020 2020 5468 6973 206d  )..       This m
+00001870: 6574 686f 6420 6d75 7374 2072 6574 7572  ethod must retur
+00001880: 6e20 616e 2069 7465 7261 626c 6520 7769  n an iterable wi
+00001890: 7468 2074 6865 2066 6972 7374 2052 6571  th the first Req
+000018a0: 7565 7374 7320 746f 2063 7261 776c 2066  uests to crawl f
+000018b0: 6f72 0a20 2020 2020 2020 7468 6973 2073  or.       this s
+000018c0: 7069 6465 722e 2049 7420 6973 2063 616c  pider. It is cal
+000018d0: 6c65 6420 6279 2053 6372 6170 7920 7768  led by Scrapy wh
+000018e0: 656e 2074 6865 2073 7069 6465 7220 6973  en the spider is
+000018f0: 206f 7065 6e65 6420 666f 720a 2020 2020   opened for.    
+00001900: 2020 2073 6372 6170 696e 672e 2053 6372     scraping. Scr
+00001910: 6170 7920 6361 6c6c 7320 6974 206f 6e6c  apy calls it onl
+00001920: 7920 6f6e 6365 2c20 736f 2069 7420 6973  y once, so it is
+00001930: 2073 6166 6520 746f 2069 6d70 6c65 6d65   safe to impleme
+00001940: 6e74 0a20 2020 2020 2020 3a6d 6574 683a  nt.       :meth:
+00001950: 6073 7461 7274 5f72 6571 7565 7374 7360  `start_requests`
+00001960: 2061 7320 6120 6765 6e65 7261 746f 722e   as a generator.
+00001970: 0a0a 2020 2020 2020 2054 6865 2064 6566  ..       The def
+00001980: 6175 6c74 2069 6d70 6c65 6d65 6e74 6174  ault implementat
+00001990: 696f 6e20 6765 6e65 7261 7465 7320 6060  ion generates ``
+000019a0: 5265 7175 6573 7428 7572 6c2c 2064 6f6e  Request(url, don
+000019b0: 745f 6669 6c74 6572 3d54 7275 6529 6060  t_filter=True)``
+000019c0: 0a20 2020 2020 2020 666f 7220 6561 6368  .       for each
+000019d0: 2075 726c 2069 6e20 3a61 7474 723a 6073   url in :attr:`s
+000019e0: 7461 7274 5f75 726c 7360 2e0a 0a20 2020  tart_urls`...   
+000019f0: 2020 2020 4966 2079 6f75 2077 616e 7420      If you want 
+00001a00: 746f 2063 6861 6e67 6520 7468 6520 5265  to change the Re
+00001a10: 7175 6573 7473 2075 7365 6420 746f 2073  quests used to s
+00001a20: 7461 7274 2073 6372 6170 696e 6720 6120  tart scraping a 
+00001a30: 646f 6d61 696e 2c20 7468 6973 2069 730a  domain, this is.
+00001a40: 2020 2020 2020 2074 6865 206d 6574 686f         the metho
+00001a50: 6420 746f 206f 7665 7272 6964 652e 2046  d to override. F
+00001a60: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
+00001a70: 6f75 206e 6565 6420 746f 2073 7461 7274  ou need to start
+00001a80: 2062 7920 6c6f 6767 696e 6720 696e 2075   by logging in u
+00001a90: 7369 6e67 0a20 2020 2020 2020 6120 504f  sing.       a PO
+00001aa0: 5354 2072 6571 7565 7374 2c20 796f 7520  ST request, you 
+00001ab0: 636f 756c 6420 646f 3a0a 0a20 2020 2020  could do:..     
+00001ac0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00001ad0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00001ae0: 2020 2020 2069 6d70 6f72 7420 7363 7261       import scra
+00001af0: 7079 0a0a 0a20 2020 2020 2020 2020 2020  py...           
+00001b00: 636c 6173 7320 4d79 5370 6964 6572 2873  class MySpider(s
+00001b10: 6372 6170 792e 5370 6964 6572 293a 0a20  crapy.Spider):. 
+00001b20: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+00001b30: 6d65 203d 2022 6d79 7370 6964 6572 220a  me = "myspider".
+00001b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b50: 6465 6620 7374 6172 745f 7265 7175 6573  def start_reques
+00001b60: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+00001b70: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00001b80: 7572 6e20 5b0a 2020 2020 2020 2020 2020  urn [.          
+00001b90: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00001ba0: 6170 792e 466f 726d 5265 7175 6573 7428  apy.FormRequest(
+00001bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001bc0: 2020 2020 2020 2020 2020 2020 2268 7474              "htt
+00001bd0: 703a 2f2f 7777 772e 6578 616d 706c 652e  p://www.example.
+00001be0: 636f 6d2f 6c6f 6769 6e22 2c0a 2020 2020  com/login",.    
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c00: 2020 2020 2020 2066 6f72 6d64 6174 613d         formdata=
+00001c10: 7b22 7573 6572 223a 2022 6a6f 686e 222c  {"user": "john",
+00001c20: 2022 7061 7373 223a 2022 7365 6372 6574   "pass": "secret
+00001c30: 227d 2c0a 2020 2020 2020 2020 2020 2020  "},.            
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001c50: 616c 6c62 6163 6b3d 7365 6c66 2e6c 6f67  allback=self.log
+00001c60: 6765 645f 696e 2c0a 2020 2020 2020 2020  ged_in,.        
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00001c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c90: 2020 2020 5d0a 0a20 2020 2020 2020 2020      ]..         
+00001ca0: 2020 2020 2020 6465 6620 6c6f 6767 6564        def logged
+00001cb0: 5f69 6e28 7365 6c66 2c20 7265 7370 6f6e  _in(self, respon
+00001cc0: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+00001cd0: 2020 2020 2020 2020 2320 6865 7265 2079          # here y
+00001ce0: 6f75 2077 6f75 6c64 2065 7874 7261 6374  ou would extract
+00001cf0: 206c 696e 6b73 2074 6f20 666f 6c6c 6f77   links to follow
+00001d00: 2061 6e64 2072 6574 7572 6e20 5265 7175   and return Requ
+00001d10: 6573 7473 2066 6f72 0a20 2020 2020 2020  ests for.       
+00001d20: 2020 2020 2020 2020 2020 2020 2320 6561              # ea
+00001d30: 6368 206f 6620 7468 656d 2c20 7769 7468  ch of them, with
+00001d40: 2061 6e6f 7468 6572 2063 616c 6c62 6163   another callbac
+00001d50: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+00001d60: 2020 2020 2070 6173 730a 0a20 2020 2e2e       pass..   ..
+00001d70: 206d 6574 686f 643a 3a20 7061 7273 6528   method:: parse(
+00001d80: 7265 7370 6f6e 7365 290a 0a20 2020 2020  response)..     
+00001d90: 2020 5468 6973 2069 7320 7468 6520 6465    This is the de
+00001da0: 6661 756c 7420 6361 6c6c 6261 636b 2075  fault callback u
+00001db0: 7365 6420 6279 2053 6372 6170 7920 746f  sed by Scrapy to
+00001dc0: 2070 726f 6365 7373 2064 6f77 6e6c 6f61   process downloa
+00001dd0: 6465 640a 2020 2020 2020 2072 6573 706f  ded.       respo
+00001de0: 6e73 6573 2c20 7768 656e 2074 6865 6972  nses, when their
+00001df0: 2072 6571 7565 7374 7320 646f 6e27 7420   requests don't 
+00001e00: 7370 6563 6966 7920 6120 6361 6c6c 6261  specify a callba
+00001e10: 636b 2e0a 0a20 2020 2020 2020 5468 6520  ck...       The 
+00001e20: 6060 7061 7273 6560 6020 6d65 7468 6f64  ``parse`` method
+00001e30: 2069 7320 696e 2063 6861 7267 6520 6f66   is in charge of
+00001e40: 2070 726f 6365 7373 696e 6720 7468 6520   processing the 
+00001e50: 7265 7370 6f6e 7365 2061 6e64 2072 6574  response and ret
+00001e60: 7572 6e69 6e67 0a20 2020 2020 2020 7363  urning.       sc
+00001e70: 7261 7065 6420 6461 7461 2061 6e64 2f6f  raped data and/o
+00001e80: 7220 6d6f 7265 2055 524c 7320 746f 2066  r more URLs to f
+00001e90: 6f6c 6c6f 772e 204f 7468 6572 2052 6571  ollow. Other Req
+00001ea0: 7565 7374 7320 6361 6c6c 6261 636b 7320  uests callbacks 
+00001eb0: 6861 7665 0a20 2020 2020 2020 7468 6520  have.       the 
+00001ec0: 7361 6d65 2072 6571 7569 7265 6d65 6e74  same requirement
+00001ed0: 7320 6173 2074 6865 203a 636c 6173 733a  s as the :class:
+00001ee0: 6053 7069 6465 7260 2063 6c61 7373 2e0a  `Spider` class..
+00001ef0: 0a20 2020 2020 2020 5468 6973 206d 6574  .       This met
+00001f00: 686f 642c 2061 7320 7765 6c6c 2061 7320  hod, as well as 
+00001f10: 616e 7920 6f74 6865 7220 5265 7175 6573  any other Reques
+00001f20: 7420 6361 6c6c 6261 636b 2c20 6d75 7374  t callback, must
+00001f30: 2072 6574 7572 6e20 610a 2020 2020 2020   return a.      
+00001f40: 203a 636c 6173 733a 607e 7363 7261 7079   :class:`~scrapy
+00001f50: 2e52 6571 7565 7374 6020 6f62 6a65 6374  .Request` object
+00001f60: 2c20 616e 203a 7265 663a 6069 7465 6d20  , an :ref:`item 
+00001f70: 6f62 6a65 6374 203c 746f 7069 6373 2d69  object <topics-i
+00001f80: 7465 6d73 3e60 2c20 616e 0a20 2020 2020  tems>`, an.     
+00001f90: 2020 6974 6572 6162 6c65 206f 6620 3a63    iterable of :c
+00001fa0: 6c61 7373 3a60 7e73 6372 6170 792e 5265  lass:`~scrapy.Re
+00001fb0: 7175 6573 7460 206f 626a 6563 7473 2061  quest` objects a
+00001fc0: 6e64 2f6f 7220 3a72 6566 3a60 6974 656d  nd/or :ref:`item
+00001fd0: 206f 626a 6563 7473 0a20 2020 2020 2020   objects.       
+00001fe0: 3c74 6f70 6963 732d 6974 656d 733e 602c  <topics-items>`,
+00001ff0: 206f 7220 6060 4e6f 6e65 6060 2e0a 0a20   or ``None``... 
+00002000: 2020 2020 2020 3a70 6172 616d 2072 6573        :param res
+00002010: 706f 6e73 653a 2074 6865 2072 6573 706f  ponse: the respo
+00002020: 6e73 6520 746f 2070 6172 7365 0a20 2020  nse to parse.   
+00002030: 2020 2020 3a74 7970 6520 7265 7370 6f6e      :type respon
+00002040: 7365 3a20 3a63 6c61 7373 3a60 7e73 6372  se: :class:`~scr
+00002050: 6170 792e 6874 7470 2e52 6573 706f 6e73  apy.http.Respons
+00002060: 6560 0a0a 2020 202e 2e20 6d65 7468 6f64  e`..   .. method
+00002070: 3a3a 206c 6f67 286d 6573 7361 6765 2c20  :: log(message, 
+00002080: 5b6c 6576 656c 2c20 636f 6d70 6f6e 656e  [level, componen
+00002090: 745d 290a 0a20 2020 2020 2020 5772 6170  t])..       Wrap
+000020a0: 7065 7220 7468 6174 2073 656e 6473 2061  per that sends a
+000020b0: 206c 6f67 206d 6573 7361 6765 2074 6872   log message thr
+000020c0: 6f75 6768 2074 6865 2053 7069 6465 7227  ough the Spider'
+000020d0: 7320 3a61 7474 723a 606c 6f67 6765 7260  s :attr:`logger`
+000020e0: 2c0a 2020 2020 2020 206b 6570 7420 666f  ,.       kept fo
+000020f0: 7220 6261 636b 7761 7264 2063 6f6d 7061  r backward compa
+00002100: 7469 6269 6c69 7479 2e20 466f 7220 6d6f  tibility. For mo
+00002110: 7265 2069 6e66 6f72 6d61 7469 6f6e 2073  re information s
+00002120: 6565 0a20 2020 2020 2020 3a72 6566 3a60  ee.       :ref:`
+00002130: 746f 7069 6373 2d6c 6f67 6769 6e67 2d66  topics-logging-f
+00002140: 726f 6d2d 7370 6964 6572 7360 2e0a 0a20  rom-spiders`... 
+00002150: 2020 2e2e 206d 6574 686f 643a 3a20 636c    .. method:: cl
+00002160: 6f73 6564 2872 6561 736f 6e29 0a0a 2020  osed(reason)..  
+00002170: 2020 2020 2043 616c 6c65 6420 7768 656e       Called when
+00002180: 2074 6865 2073 7069 6465 7220 636c 6f73   the spider clos
+00002190: 6573 2e20 5468 6973 206d 6574 686f 6420  es. This method 
+000021a0: 7072 6f76 6964 6573 2061 2073 686f 7274  provides a short
+000021b0: 6375 7420 746f 0a20 2020 2020 2020 7369  cut to.       si
+000021c0: 676e 616c 732e 636f 6e6e 6563 7428 2920  gnals.connect() 
+000021d0: 666f 7220 7468 6520 3a73 6967 6e61 6c3a  for the :signal:
+000021e0: 6073 7069 6465 725f 636c 6f73 6564 6020  `spider_closed` 
+000021f0: 7369 676e 616c 2e0a 0a4c 6574 2773 2073  signal...Let's s
+00002200: 6565 2061 6e20 6578 616d 706c 653a 0a0a  ee an example:..
+00002210: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00002220: 7079 7468 6f6e 0a0a 2020 2020 696d 706f  python..    impo
+00002230: 7274 2073 6372 6170 790a 0a0a 2020 2020  rt scrapy...    
+00002240: 636c 6173 7320 4d79 5370 6964 6572 2873  class MySpider(s
+00002250: 6372 6170 792e 5370 6964 6572 293a 0a20  crapy.Spider):. 
+00002260: 2020 2020 2020 206e 616d 6520 3d20 2265         name = "e
+00002270: 7861 6d70 6c65 2e63 6f6d 220a 2020 2020  xample.com".    
+00002280: 2020 2020 616c 6c6f 7765 645f 646f 6d61      allowed_doma
+00002290: 696e 7320 3d20 5b22 6578 616d 706c 652e  ins = ["example.
+000022a0: 636f 6d22 5d0a 2020 2020 2020 2020 7374  com"].        st
+000022b0: 6172 745f 7572 6c73 203d 205b 0a20 2020  art_urls = [.   
+000022c0: 2020 2020 2020 2020 2022 6874 7470 3a2f           "http:/
+000022d0: 2f77 7777 2e65 7861 6d70 6c65 2e63 6f6d  /www.example.com
+000022e0: 2f31 2e68 746d 6c22 2c0a 2020 2020 2020  /1.html",.      
+000022f0: 2020 2020 2020 2268 7474 703a 2f2f 7777        "http://ww
+00002300: 772e 6578 616d 706c 652e 636f 6d2f 322e  w.example.com/2.
+00002310: 6874 6d6c 222c 0a20 2020 2020 2020 2020  html",.         
+00002320: 2020 2022 6874 7470 3a2f 2f77 7777 2e65     "http://www.e
+00002330: 7861 6d70 6c65 2e63 6f6d 2f33 2e68 746d  xample.com/3.htm
+00002340: 6c22 2c0a 2020 2020 2020 2020 5d0a 0a20  l",.        ].. 
+00002350: 2020 2020 2020 2064 6566 2070 6172 7365         def parse
+00002360: 2873 656c 662c 2072 6573 706f 6e73 6529  (self, response)
+00002370: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00002380: 6c66 2e6c 6f67 6765 722e 696e 666f 2822  lf.logger.info("
+00002390: 4120 7265 7370 6f6e 7365 2066 726f 6d20  A response from 
+000023a0: 2573 206a 7573 7420 6172 7269 7665 6421  %s just arrived!
+000023b0: 222c 2072 6573 706f 6e73 652e 7572 6c29  ", response.url)
+000023c0: 0a0a 5265 7475 726e 206d 756c 7469 706c  ..Return multipl
+000023d0: 6520 5265 7175 6573 7473 2061 6e64 2069  e Requests and i
+000023e0: 7465 6d73 2066 726f 6d20 6120 7369 6e67  tems from a sing
+000023f0: 6c65 2063 616c 6c62 6163 6b3a 0a0a 2e2e  le callback:....
+00002400: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00002410: 7468 6f6e 0a0a 2020 2020 696d 706f 7274  thon..    import
+00002420: 2073 6372 6170 790a 0a0a 2020 2020 636c   scrapy...    cl
+00002430: 6173 7320 4d79 5370 6964 6572 2873 6372  ass MySpider(scr
+00002440: 6170 792e 5370 6964 6572 293a 0a20 2020  apy.Spider):.   
+00002450: 2020 2020 206e 616d 6520 3d20 2265 7861       name = "exa
+00002460: 6d70 6c65 2e63 6f6d 220a 2020 2020 2020  mple.com".      
+00002470: 2020 616c 6c6f 7765 645f 646f 6d61 696e    allowed_domain
+00002480: 7320 3d20 5b22 6578 616d 706c 652e 636f  s = ["example.co
+00002490: 6d22 5d0a 2020 2020 2020 2020 7374 6172  m"].        star
+000024a0: 745f 7572 6c73 203d 205b 0a20 2020 2020  t_urls = [.     
+000024b0: 2020 2020 2020 2022 6874 7470 3a2f 2f77         "http://w
+000024c0: 7777 2e65 7861 6d70 6c65 2e63 6f6d 2f31  ww.example.com/1
+000024d0: 2e68 746d 6c22 2c0a 2020 2020 2020 2020  .html",.        
+000024e0: 2020 2020 2268 7474 703a 2f2f 7777 772e      "http://www.
+000024f0: 6578 616d 706c 652e 636f 6d2f 322e 6874  example.com/2.ht
+00002500: 6d6c 222c 0a20 2020 2020 2020 2020 2020  ml",.           
+00002510: 2022 6874 7470 3a2f 2f77 7777 2e65 7861   "http://www.exa
+00002520: 6d70 6c65 2e63 6f6d 2f33 2e68 746d 6c22  mple.com/3.html"
+00002530: 2c0a 2020 2020 2020 2020 5d0a 0a20 2020  ,.        ]..   
+00002540: 2020 2020 2064 6566 2070 6172 7365 2873       def parse(s
+00002550: 656c 662c 2072 6573 706f 6e73 6529 3a0a  elf, response):.
+00002560: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002570: 6833 2069 6e20 7265 7370 6f6e 7365 2e78  h3 in response.x
+00002580: 7061 7468 2822 2f2f 6833 2229 2e67 6574  path("//h3").get
+00002590: 616c 6c28 293a 0a20 2020 2020 2020 2020  all():.         
+000025a0: 2020 2020 2020 2079 6965 6c64 207b 2274         yield {"t
+000025b0: 6974 6c65 223a 2068 337d 0a0a 2020 2020  itle": h3}..    
+000025c0: 2020 2020 2020 2020 666f 7220 6872 6566          for href
+000025d0: 2069 6e20 7265 7370 6f6e 7365 2e78 7061   in response.xpa
+000025e0: 7468 2822 2f2f 612f 4068 7265 6622 292e  th("//a/@href").
+000025f0: 6765 7461 6c6c 2829 3a0a 2020 2020 2020  getall():.      
+00002600: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+00002610: 7363 7261 7079 2e52 6571 7565 7374 2872  scrapy.Request(r
+00002620: 6573 706f 6e73 652e 7572 6c6a 6f69 6e28  esponse.urljoin(
+00002630: 6872 6566 292c 2073 656c 662e 7061 7273  href), self.pars
+00002640: 6529 0a0a 496e 7374 6561 6420 6f66 203a  e)..Instead of :
+00002650: 6174 7472 3a60 7e2e 7374 6172 745f 7572  attr:`~.start_ur
+00002660: 6c73 6020 796f 7520 6361 6e20 7573 6520  ls` you can use 
+00002670: 3a6d 6574 683a 607e 2e73 7461 7274 5f72  :meth:`~.start_r
+00002680: 6571 7565 7374 7360 2064 6972 6563 746c  equests` directl
+00002690: 793b 0a74 6f20 6769 7665 2064 6174 6120  y;.to give data 
+000026a0: 6d6f 7265 2073 7472 7563 7475 7265 2079  more structure y
+000026b0: 6f75 2063 616e 2075 7365 203a 636c 6173  ou can use :clas
+000026c0: 733a 607e 7363 7261 7079 2e49 7465 6d60  s:`~scrapy.Item`
+000026d0: 206f 626a 6563 7473 3a0a 0a2e 2e20 736b   objects:.... sk
+000026e0: 6970 3a20 6e65 7874 0a2e 2e20 636f 6465  ip: next... code
+000026f0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00002700: 0a20 2020 2069 6d70 6f72 7420 7363 7261  .    import scra
+00002710: 7079 0a20 2020 2066 726f 6d20 6d79 7072  py.    from mypr
+00002720: 6f6a 6563 742e 6974 656d 7320 696d 706f  oject.items impo
+00002730: 7274 204d 7949 7465 6d0a 0a0a 2020 2020  rt MyItem...    
+00002740: 636c 6173 7320 4d79 5370 6964 6572 2873  class MySpider(s
+00002750: 6372 6170 792e 5370 6964 6572 293a 0a20  crapy.Spider):. 
+00002760: 2020 2020 2020 206e 616d 6520 3d20 2265         name = "e
+00002770: 7861 6d70 6c65 2e63 6f6d 220a 2020 2020  xample.com".    
+00002780: 2020 2020 616c 6c6f 7765 645f 646f 6d61      allowed_doma
+00002790: 696e 7320 3d20 5b22 6578 616d 706c 652e  ins = ["example.
+000027a0: 636f 6d22 5d0a 0a20 2020 2020 2020 2064  com"]..        d
+000027b0: 6566 2073 7461 7274 5f72 6571 7565 7374  ef start_request
+000027c0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+000027d0: 2020 2020 2079 6965 6c64 2073 6372 6170       yield scrap
+000027e0: 792e 5265 7175 6573 7428 2268 7474 703a  y.Request("http:
+000027f0: 2f2f 7777 772e 6578 616d 706c 652e 636f  //www.example.co
+00002800: 6d2f 312e 6874 6d6c 222c 2073 656c 662e  m/1.html", self.
+00002810: 7061 7273 6529 0a20 2020 2020 2020 2020  parse).         
+00002820: 2020 2079 6965 6c64 2073 6372 6170 792e     yield scrapy.
+00002830: 5265 7175 6573 7428 2268 7474 703a 2f2f  Request("http://
+00002840: 7777 772e 6578 616d 706c 652e 636f 6d2f  www.example.com/
+00002850: 322e 6874 6d6c 222c 2073 656c 662e 7061  2.html", self.pa
+00002860: 7273 6529 0a20 2020 2020 2020 2020 2020  rse).           
+00002870: 2079 6965 6c64 2073 6372 6170 792e 5265   yield scrapy.Re
+00002880: 7175 6573 7428 2268 7474 703a 2f2f 7777  quest("http://ww
+00002890: 772e 6578 616d 706c 652e 636f 6d2f 332e  w.example.com/3.
+000028a0: 6874 6d6c 222c 2073 656c 662e 7061 7273  html", self.pars
+000028b0: 6529 0a0a 2020 2020 2020 2020 6465 6620  e)..        def 
+000028c0: 7061 7273 6528 7365 6c66 2c20 7265 7370  parse(self, resp
+000028d0: 6f6e 7365 293a 0a20 2020 2020 2020 2020  onse):.         
+000028e0: 2020 2066 6f72 2068 3320 696e 2072 6573     for h3 in res
+000028f0: 706f 6e73 652e 7870 6174 6828 222f 2f68  ponse.xpath("//h
+00002900: 3322 292e 6765 7461 6c6c 2829 3a0a 2020  3").getall():.  
+00002910: 2020 2020 2020 2020 2020 2020 2020 7969                yi
+00002920: 656c 6420 4d79 4974 656d 2874 6974 6c65  eld MyItem(title
+00002930: 3d68 3329 0a0a 2020 2020 2020 2020 2020  =h3)..          
+00002940: 2020 666f 7220 6872 6566 2069 6e20 7265    for href in re
+00002950: 7370 6f6e 7365 2e78 7061 7468 2822 2f2f  sponse.xpath("//
+00002960: 612f 4068 7265 6622 292e 6765 7461 6c6c  a/@href").getall
+00002970: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00002980: 2020 2020 7969 656c 6420 7363 7261 7079      yield scrapy
+00002990: 2e52 6571 7565 7374 2872 6573 706f 6e73  .Request(respons
+000029a0: 652e 7572 6c6a 6f69 6e28 6872 6566 292c  e.urljoin(href),
+000029b0: 2073 656c 662e 7061 7273 6529 0a0a 2e2e   self.parse)....
+000029c0: 205f 7370 6964 6572 6172 6773 3a0a 0a53   _spiderargs:..S
+000029d0: 7069 6465 7220 6172 6775 6d65 6e74 730a  pider arguments.
+000029e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000029f0: 0a0a 5370 6964 6572 7320 6361 6e20 7265  ..Spiders can re
+00002a00: 6365 6976 6520 6172 6775 6d65 6e74 7320  ceive arguments 
+00002a10: 7468 6174 206d 6f64 6966 7920 7468 6569  that modify thei
+00002a20: 7220 6265 6861 7669 6f75 722e 2053 6f6d  r behaviour. Som
+00002a30: 6520 636f 6d6d 6f6e 2075 7365 7320 666f  e common uses fo
+00002a40: 720a 7370 6964 6572 2061 7267 756d 656e  r.spider argumen
+00002a50: 7473 2061 7265 2074 6f20 6465 6669 6e65  ts are to define
+00002a60: 2074 6865 2073 7461 7274 2055 524c 7320   the start URLs 
+00002a70: 6f72 2074 6f20 7265 7374 7269 6374 2074  or to restrict t
+00002a80: 6865 2063 7261 776c 2074 6f0a 6365 7274  he crawl to.cert
+00002a90: 6169 6e20 7365 6374 696f 6e73 206f 6620  ain sections of 
+00002aa0: 7468 6520 7369 7465 2c20 6275 7420 7468  the site, but th
+00002ab0: 6579 2063 616e 2062 6520 7573 6564 2074  ey can be used t
+00002ac0: 6f20 636f 6e66 6967 7572 6520 616e 790a  o configure any.
+00002ad0: 6675 6e63 7469 6f6e 616c 6974 7920 6f66  functionality of
+00002ae0: 2074 6865 2073 7069 6465 722e 0a0a 5370   the spider...Sp
+00002af0: 6964 6572 2061 7267 756d 656e 7473 2061  ider arguments a
+00002b00: 7265 2070 6173 7365 6420 7468 726f 7567  re passed throug
+00002b10: 6820 7468 6520 3a63 6f6d 6d61 6e64 3a60  h the :command:`
+00002b20: 6372 6177 6c60 2063 6f6d 6d61 6e64 2075  crawl` command u
+00002b30: 7369 6e67 2074 6865 0a60 602d 6160 6020  sing the.``-a`` 
+00002b40: 6f70 7469 6f6e 2e20 466f 7220 6578 616d  option. For exam
+00002b50: 706c 653a 3a0a 0a20 2020 2073 6372 6170  ple::..    scrap
+00002b60: 7920 6372 6177 6c20 6d79 7370 6964 6572  y crawl myspider
+00002b70: 202d 6120 6361 7465 676f 7279 3d65 6c65   -a category=ele
+00002b80: 6374 726f 6e69 6373 0a0a 5370 6964 6572  ctronics..Spider
+00002b90: 7320 6361 6e20 6163 6365 7373 2061 7267  s can access arg
+00002ba0: 756d 656e 7473 2069 6e20 7468 6569 7220  uments in their 
+00002bb0: 605f 5f69 6e69 745f 5f60 206d 6574 686f  `__init__` metho
+00002bc0: 6473 3a0a 0a2e 2e20 636f 6465 2d62 6c6f  ds:.... code-blo
+00002bd0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
+00002be0: 2069 6d70 6f72 7420 7363 7261 7079 0a0a   import scrapy..
+00002bf0: 0a20 2020 2063 6c61 7373 204d 7953 7069  .    class MySpi
+00002c00: 6465 7228 7363 7261 7079 2e53 7069 6465  der(scrapy.Spide
+00002c10: 7229 3a0a 2020 2020 2020 2020 6e61 6d65  r):.        name
+00002c20: 203d 2022 6d79 7370 6964 6572 220a 0a20   = "myspider".. 
+00002c30: 2020 2020 2020 2064 6566 205f 5f69 6e69         def __ini
+00002c40: 745f 5f28 7365 6c66 2c20 6361 7465 676f  t__(self, catego
+00002c50: 7279 3d4e 6f6e 652c 202a 6172 6773 2c20  ry=None, *args, 
+00002c60: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00002c70: 2020 2020 2020 2073 7570 6572 284d 7953         super(MyS
+00002c80: 7069 6465 722c 2073 656c 6629 2e5f 5f69  pider, self).__i
+00002c90: 6e69 745f 5f28 2a61 7267 732c 202a 2a6b  nit__(*args, **k
+00002ca0: 7761 7267 7329 0a20 2020 2020 2020 2020  wargs).         
+00002cb0: 2020 2073 656c 662e 7374 6172 745f 7572     self.start_ur
+00002cc0: 6c73 203d 205b 6622 6874 7470 3a2f 2f77  ls = [f"http://w
+00002cd0: 7777 2e65 7861 6d70 6c65 2e63 6f6d 2f63  ww.example.com/c
+00002ce0: 6174 6567 6f72 6965 732f 7b63 6174 6567  ategories/{categ
+00002cf0: 6f72 797d 225d 0a20 2020 2020 2020 2020  ory}"].         
+00002d00: 2020 2023 202e 2e2e 0a0a 5468 6520 6465     # .....The de
+00002d10: 6661 756c 7420 605f 5f69 6e69 745f 5f60  fault `__init__`
+00002d20: 206d 6574 686f 6420 7769 6c6c 2074 616b   method will tak
+00002d30: 6520 616e 7920 7370 6964 6572 2061 7267  e any spider arg
+00002d40: 756d 656e 7473 0a61 6e64 2063 6f70 7920  uments.and copy 
+00002d50: 7468 656d 2074 6f20 7468 6520 7370 6964  them to the spid
+00002d60: 6572 2061 7320 6174 7472 6962 7574 6573  er as attributes
+00002d70: 2e0a 5468 6520 6162 6f76 6520 6578 616d  ..The above exam
+00002d80: 706c 6520 6361 6e20 616c 736f 2062 6520  ple can also be 
+00002d90: 7772 6974 7465 6e20 6173 2066 6f6c 6c6f  written as follo
+00002da0: 7773 3a0a 0a2e 2e20 636f 6465 2d62 6c6f  ws:.... code-blo
+00002db0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
+00002dc0: 2069 6d70 6f72 7420 7363 7261 7079 0a0a   import scrapy..
+00002dd0: 0a20 2020 2063 6c61 7373 204d 7953 7069  .    class MySpi
+00002de0: 6465 7228 7363 7261 7079 2e53 7069 6465  der(scrapy.Spide
+00002df0: 7229 3a0a 2020 2020 2020 2020 6e61 6d65  r):.        name
+00002e00: 203d 2022 6d79 7370 6964 6572 220a 0a20   = "myspider".. 
+00002e10: 2020 2020 2020 2064 6566 2073 7461 7274         def start
+00002e20: 5f72 6571 7565 7374 7328 7365 6c66 293a  _requests(self):
+00002e30: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+00002e40: 6c64 2073 6372 6170 792e 5265 7175 6573  ld scrapy.Reques
+00002e50: 7428 6622 6874 7470 3a2f 2f77 7777 2e65  t(f"http://www.e
+00002e60: 7861 6d70 6c65 2e63 6f6d 2f63 6174 6567  xample.com/categ
+00002e70: 6f72 6965 732f 7b73 656c 662e 6361 7465  ories/{self.cate
+00002e80: 676f 7279 7d22 290a 0a49 6620 796f 7520  gory}")..If you 
+00002e90: 6172 6520 3a72 6566 3a60 7275 6e6e 696e  are :ref:`runnin
+00002ea0: 6720 5363 7261 7079 2066 726f 6d20 6120  g Scrapy from a 
+00002eb0: 7363 7269 7074 203c 7275 6e2d 6672 6f6d  script <run-from
+00002ec0: 2d73 6372 6970 743e 602c 2079 6f75 2063  -script>`, you c
+00002ed0: 616e 200a 7370 6563 6966 7920 7370 6964  an .specify spid
+00002ee0: 6572 2061 7267 756d 656e 7473 2077 6865  er arguments whe
+00002ef0: 6e20 6361 6c6c 696e 6720 0a3a 636c 6173  n calling .:clas
+00002f00: 733a 6043 7261 776c 6572 5072 6f63 6573  s:`CrawlerProces
+00002f10: 732e 6372 6177 6c20 3c73 6372 6170 792e  s.crawl <scrapy.
+00002f20: 6372 6177 6c65 722e 4372 6177 6c65 7250  crawler.CrawlerP
+00002f30: 726f 6365 7373 2e63 7261 776c 3e60 206f  rocess.crawl>` o
+00002f40: 720a 3a63 6c61 7373 3a60 4372 6177 6c65  r.:class:`Crawle
+00002f50: 7252 756e 6e65 722e 6372 6177 6c20 3c73  rRunner.crawl <s
+00002f60: 6372 6170 792e 6372 6177 6c65 722e 4372  crapy.crawler.Cr
+00002f70: 6177 6c65 7252 756e 6e65 722e 6372 6177  awlerRunner.craw
+00002f80: 6c3e 603a 0a0a 2e2e 2073 6b69 703a 206e  l>`:.... skip: n
+00002f90: 6578 740a 2e2e 2063 6f64 652d 626c 6f63  ext... code-bloc
+00002fa0: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
+00002fb0: 7072 6f63 6573 7320 3d20 4372 6177 6c65  process = Crawle
+00002fc0: 7250 726f 6365 7373 2829 0a20 2020 2070  rProcess().    p
+00002fd0: 726f 6365 7373 2e63 7261 776c 284d 7953  rocess.crawl(MyS
+00002fe0: 7069 6465 722c 2063 6174 6567 6f72 793d  pider, category=
+00002ff0: 2265 6c65 6374 726f 6e69 6373 2229 0a0a  "electronics")..
+00003000: 4b65 6570 2069 6e20 6d69 6e64 2074 6861  Keep in mind tha
+00003010: 7420 7370 6964 6572 2061 7267 756d 656e  t spider argumen
+00003020: 7473 2061 7265 206f 6e6c 7920 7374 7269  ts are only stri
+00003030: 6e67 732e 0a54 6865 2073 7069 6465 7220  ngs..The spider 
+00003040: 7769 6c6c 206e 6f74 2064 6f20 616e 7920  will not do any 
+00003050: 7061 7273 696e 6720 6f6e 2069 7473 206f  parsing on its o
+00003060: 776e 2e0a 4966 2079 6f75 2077 6572 6520  wn..If you were 
+00003070: 746f 2073 6574 2074 6865 2060 6073 7461  to set the ``sta
+00003080: 7274 5f75 726c 7360 6020 6174 7472 6962  rt_urls`` attrib
+00003090: 7574 6520 6672 6f6d 2074 6865 2063 6f6d  ute from the com
+000030a0: 6d61 6e64 206c 696e 652c 0a79 6f75 2077  mand line,.you w
+000030b0: 6f75 6c64 2068 6176 6520 746f 2070 6172  ould have to par
+000030c0: 7365 2069 7420 6f6e 2079 6f75 7220 6f77  se it on your ow
+000030d0: 6e20 696e 746f 2061 206c 6973 740a 7573  n into a list.us
+000030e0: 696e 6720 736f 6d65 7468 696e 6720 6c69  ing something li
+000030f0: 6b65 203a 6675 6e63 3a60 6173 742e 6c69  ke :func:`ast.li
+00003100: 7465 7261 6c5f 6576 616c 6020 6f72 203a  teral_eval` or :
+00003110: 6675 6e63 3a60 6a73 6f6e 2e6c 6f61 6473  func:`json.loads
+00003120: 600a 616e 6420 7468 656e 2073 6574 2069  `.and then set i
+00003130: 7420 6173 2061 6e20 6174 7472 6962 7574  t as an attribut
+00003140: 652e 0a4f 7468 6572 7769 7365 2c20 796f  e..Otherwise, yo
+00003150: 7520 776f 756c 6420 6361 7573 6520 6974  u would cause it
+00003160: 6572 6174 696f 6e20 6f76 6572 2061 2060  eration over a `
+00003170: 6073 7461 7274 5f75 726c 7360 6020 7374  `start_urls`` st
+00003180: 7269 6e67 0a28 6120 7665 7279 2063 6f6d  ring.(a very com
+00003190: 6d6f 6e20 7079 7468 6f6e 2070 6974 6661  mon python pitfa
+000031a0: 6c6c 290a 7265 7375 6c74 696e 6720 696e  ll).resulting in
+000031b0: 2065 6163 6820 6368 6172 6163 7465 7220   each character 
+000031c0: 6265 696e 6720 7365 656e 2061 7320 6120  being seen as a 
+000031d0: 7365 7061 7261 7465 2075 726c 2e0a 0a41  separate url...A
+000031e0: 2076 616c 6964 2075 7365 2063 6173 6520   valid use case 
+000031f0: 6973 2074 6f20 7365 7420 7468 6520 6874  is to set the ht
+00003200: 7470 2061 7574 6820 6372 6564 656e 7469  tp auth credenti
+00003210: 616c 730a 7573 6564 2062 7920 3a63 6c61  als.used by :cla
+00003220: 7373 3a60 7e73 6372 6170 792e 646f 776e  ss:`~scrapy.down
+00003230: 6c6f 6164 6572 6d69 6464 6c65 7761 7265  loadermiddleware
+00003240: 732e 6874 7470 6175 7468 2e48 7474 7041  s.httpauth.HttpA
+00003250: 7574 684d 6964 646c 6577 6172 6560 0a6f  uthMiddleware`.o
+00003260: 7220 7468 6520 7573 6572 2061 6765 6e74  r the user agent
+00003270: 0a75 7365 6420 6279 203a 636c 6173 733a  .used by :class:
+00003280: 607e 7363 7261 7079 2e64 6f77 6e6c 6f61  `~scrapy.downloa
+00003290: 6465 726d 6964 646c 6577 6172 6573 2e75  dermiddlewares.u
+000032a0: 7365 7261 6765 6e74 2e55 7365 7241 6765  seragent.UserAge
+000032b0: 6e74 4d69 6464 6c65 7761 7265 603a 3a0a  ntMiddleware`::.
+000032c0: 0a20 2020 2073 6372 6170 7920 6372 6177  .    scrapy craw
+000032d0: 6c20 6d79 7370 6964 6572 202d 6120 6874  l myspider -a ht
+000032e0: 7470 5f75 7365 723d 6d79 7573 6572 202d  tp_user=myuser -
+000032f0: 6120 6874 7470 5f70 6173 733d 6d79 7061  a http_pass=mypa
+00003300: 7373 776f 7264 202d 6120 7573 6572 5f61  ssword -a user_a
+00003310: 6765 6e74 3d6d 7962 6f74 0a0a 5370 6964  gent=mybot..Spid
+00003320: 6572 2061 7267 756d 656e 7473 2063 616e  er arguments can
+00003330: 2061 6c73 6f20 6265 2070 6173 7365 6420   also be passed 
+00003340: 7468 726f 7567 6820 7468 6520 5363 7261  through the Scra
+00003350: 7079 6420 6060 7363 6865 6475 6c65 2e6a  pyd ``schedule.j
+00003360: 736f 6e60 6020 4150 492e 0a53 6565 2060  son`` API..See `
+00003370: 5363 7261 7079 6420 646f 6375 6d65 6e74  Scrapyd document
+00003380: 6174 696f 6e60 5f2e 0a0a 2e2e 205f 6275  ation`_..... _bu
+00003390: 696c 7469 6e2d 7370 6964 6572 733a 0a0a  iltin-spiders:..
+000033a0: 4765 6e65 7269 6320 5370 6964 6572 730a  Generic Spiders.
+000033b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+000033c0: 0a53 6372 6170 7920 636f 6d65 7320 7769  .Scrapy comes wi
+000033d0: 7468 2073 6f6d 6520 7573 6566 756c 2067  th some useful g
+000033e0: 656e 6572 6963 2073 7069 6465 7273 2074  eneric spiders t
+000033f0: 6861 7420 796f 7520 6361 6e20 7573 6520  hat you can use 
+00003400: 746f 2073 7562 636c 6173 730a 796f 7572  to subclass.your
+00003410: 2073 7069 6465 7273 2066 726f 6d2e 2054   spiders from. T
+00003420: 6865 6972 2061 696d 2069 7320 746f 2070  heir aim is to p
+00003430: 726f 7669 6465 2063 6f6e 7665 6e69 656e  rovide convenien
+00003440: 7420 6675 6e63 7469 6f6e 616c 6974 7920  t functionality 
+00003450: 666f 7220 6120 6665 770a 636f 6d6d 6f6e  for a few.common
+00003460: 2073 6372 6170 696e 6720 6361 7365 732c   scraping cases,
+00003470: 206c 696b 6520 666f 6c6c 6f77 696e 6720   like following 
+00003480: 616c 6c20 6c69 6e6b 7320 6f6e 2061 2073  all links on a s
+00003490: 6974 6520 6261 7365 6420 6f6e 2063 6572  ite based on cer
+000034a0: 7461 696e 0a72 756c 6573 2c20 6372 6177  tain.rules, craw
+000034b0: 6c69 6e67 2066 726f 6d20 6053 6974 656d  ling from `Sitem
+000034c0: 6170 7360 5f2c 206f 7220 7061 7273 696e  aps`_, or parsin
+000034d0: 6720 616e 2058 4d4c 2f43 5356 2066 6565  g an XML/CSV fee
+000034e0: 642e 0a0a 466f 7220 7468 6520 6578 616d  d...For the exam
+000034f0: 706c 6573 2075 7365 6420 696e 2074 6865  ples used in the
+00003500: 2066 6f6c 6c6f 7769 6e67 2073 7069 6465   following spide
+00003510: 7273 2c20 7765 276c 6c20 6173 7375 6d65  rs, we'll assume
+00003520: 2079 6f75 2068 6176 6520 6120 7072 6f6a   you have a proj
+00003530: 6563 740a 7769 7468 2061 2060 6054 6573  ect.with a ``Tes
+00003540: 7449 7465 6d60 6020 6465 636c 6172 6564  tItem`` declared
+00003550: 2069 6e20 6120 6060 6d79 7072 6f6a 6563   in a ``myprojec
+00003560: 742e 6974 656d 7360 6020 6d6f 6475 6c65  t.items`` module
+00003570: 3a0a 0a2e 2e20 636f 6465 2d62 6c6f 636b  :.... code-block
+00003580: 3a3a 2070 7974 686f 6e0a 0a20 2020 2069  :: python..    i
+00003590: 6d70 6f72 7420 7363 7261 7079 0a0a 0a20  mport scrapy... 
+000035a0: 2020 2063 6c61 7373 2054 6573 7449 7465     class TestIte
+000035b0: 6d28 7363 7261 7079 2e49 7465 6d29 3a0a  m(scrapy.Item):.
+000035c0: 2020 2020 2020 2020 6964 203d 2073 6372          id = scr
+000035d0: 6170 792e 4669 656c 6428 290a 2020 2020  apy.Field().    
+000035e0: 2020 2020 6e61 6d65 203d 2073 6372 6170      name = scrap
+000035f0: 792e 4669 656c 6428 290a 2020 2020 2020  y.Field().      
+00003600: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
+00003610: 7363 7261 7079 2e46 6965 6c64 2829 0a0a  scrapy.Field()..
+00003620: 0a2e 2e20 6375 7272 656e 746d 6f64 756c  ... currentmodul
+00003630: 653a 3a20 7363 7261 7079 2e73 7069 6465  e:: scrapy.spide
+00003640: 7273 0a0a 4372 6177 6c53 7069 6465 720a  rs..CrawlSpider.
+00003650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e 2e20  -----------.... 
+00003660: 636c 6173 733a 3a20 4372 6177 6c53 7069  class:: CrawlSpi
+00003670: 6465 720a 0a20 2020 5468 6973 2069 7320  der..   This is 
+00003680: 7468 6520 6d6f 7374 2063 6f6d 6d6f 6e6c  the most commonl
+00003690: 7920 7573 6564 2073 7069 6465 7220 666f  y used spider fo
+000036a0: 7220 6372 6177 6c69 6e67 2072 6567 756c  r crawling regul
+000036b0: 6172 2077 6562 7369 7465 732c 2061 7320  ar websites, as 
+000036c0: 6974 0a20 2020 7072 6f76 6964 6573 2061  it.   provides a
+000036d0: 2063 6f6e 7665 6e69 656e 7420 6d65 6368   convenient mech
+000036e0: 616e 6973 6d20 666f 7220 666f 6c6c 6f77  anism for follow
+000036f0: 696e 6720 6c69 6e6b 7320 6279 2064 6566  ing links by def
+00003700: 696e 696e 6720 6120 7365 7420 6f66 2072  ining a set of r
+00003710: 756c 6573 2e0a 2020 2049 7420 6d61 7920  ules..   It may 
+00003720: 6e6f 7420 6265 2074 6865 2062 6573 7420  not be the best 
+00003730: 7375 6974 6564 2066 6f72 2079 6f75 7220  suited for your 
+00003740: 7061 7274 6963 756c 6172 2077 6562 2073  particular web s
+00003750: 6974 6573 206f 7220 7072 6f6a 6563 742c  ites or project,
+00003760: 2062 7574 0a20 2020 6974 2773 2067 656e   but.   it's gen
+00003770: 6572 6963 2065 6e6f 7567 6820 666f 7220  eric enough for 
+00003780: 7365 7665 7261 6c20 6361 7365 732c 2073  several cases, s
+00003790: 6f20 796f 7520 6361 6e20 7374 6172 7420  o you can start 
+000037a0: 6672 6f6d 2069 7420 616e 6420 6f76 6572  from it and over
+000037b0: 7269 6465 2069 740a 2020 2061 7320 6e65  ride it.   as ne
+000037c0: 6564 6564 2066 6f72 206d 6f72 6520 6375  eded for more cu
+000037d0: 7374 6f6d 2066 756e 6374 696f 6e61 6c69  stom functionali
+000037e0: 7479 2c20 6f72 206a 7573 7420 696d 706c  ty, or just impl
+000037f0: 656d 656e 7420 796f 7572 206f 776e 2073  ement your own s
+00003800: 7069 6465 722e 0a0a 2020 2041 7061 7274  pider...   Apart
+00003810: 2066 726f 6d20 7468 6520 6174 7472 6962   from the attrib
+00003820: 7574 6573 2069 6e68 6572 6974 6564 2066  utes inherited f
+00003830: 726f 6d20 5370 6964 6572 2028 7468 6174  rom Spider (that
+00003840: 2079 6f75 206d 7573 740a 2020 2073 7065   you must.   spe
+00003850: 6369 6679 292c 2074 6869 7320 636c 6173  cify), this clas
+00003860: 7320 7375 7070 6f72 7473 2061 206e 6577  s supports a new
+00003870: 2061 7474 7269 6275 7465 3a0a 0a20 2020   attribute:..   
+00003880: 2e2e 2061 7474 7269 6275 7465 3a3a 2072  .. attribute:: r
+00003890: 756c 6573 0a0a 2020 2020 2020 2057 6869  ules..       Whi
+000038a0: 6368 2069 7320 6120 6c69 7374 206f 6620  ch is a list of 
+000038b0: 6f6e 6520 286f 7220 6d6f 7265 2920 3a63  one (or more) :c
+000038c0: 6c61 7373 3a60 5275 6c65 6020 6f62 6a65  lass:`Rule` obje
+000038d0: 6374 732e 2020 4561 6368 203a 636c 6173  cts.  Each :clas
+000038e0: 733a 6052 756c 6560 0a20 2020 2020 2020  s:`Rule`.       
+000038f0: 6465 6669 6e65 7320 6120 6365 7274 6169  defines a certai
+00003900: 6e20 6265 6861 7669 6f75 7220 666f 7220  n behaviour for 
+00003910: 6372 6177 6c69 6e67 2074 6865 2073 6974  crawling the sit
+00003920: 652e 2052 756c 6573 206f 626a 6563 7473  e. Rules objects
+00003930: 2061 7265 0a20 2020 2020 2020 6465 7363   are.       desc
+00003940: 7269 6265 6420 6265 6c6f 772e 2049 6620  ribed below. If 
+00003950: 6d75 6c74 6970 6c65 2072 756c 6573 206d  multiple rules m
+00003960: 6174 6368 2074 6865 2073 616d 6520 6c69  atch the same li
+00003970: 6e6b 2c20 7468 6520 6669 7273 7420 6f6e  nk, the first on
+00003980: 650a 2020 2020 2020 2077 696c 6c20 6265  e.       will be
+00003990: 2075 7365 642c 2061 6363 6f72 6469 6e67   used, according
+000039a0: 2074 6f20 7468 6520 6f72 6465 7220 7468   to the order th
+000039b0: 6579 2772 6520 6465 6669 6e65 6420 696e  ey're defined in
+000039c0: 2074 6869 7320 6174 7472 6962 7574 652e   this attribute.
+000039d0: 0a0a 2020 2054 6869 7320 7370 6964 6572  ..   This spider
+000039e0: 2061 6c73 6f20 6578 706f 7365 7320 616e   also exposes an
+000039f0: 206f 7665 7272 6964 6162 6c65 206d 6574   overridable met
+00003a00: 686f 643a 0a0a 2020 202e 2e20 6d65 7468  hod:..   .. meth
+00003a10: 6f64 3a3a 2070 6172 7365 5f73 7461 7274  od:: parse_start
+00003a20: 5f75 726c 2872 6573 706f 6e73 652c 202a  _url(response, *
+00003a30: 2a6b 7761 7267 7329 0a0a 2020 2020 2020  *kwargs)..      
+00003a40: 5468 6973 206d 6574 686f 6420 6973 2063  This method is c
+00003a50: 616c 6c65 6420 666f 7220 6561 6368 2072  alled for each r
+00003a60: 6573 706f 6e73 6520 7072 6f64 7563 6564  esponse produced
+00003a70: 2066 6f72 2074 6865 2055 524c 7320 696e   for the URLs in
+00003a80: 0a20 2020 2020 2074 6865 2073 7069 6465  .      the spide
+00003a90: 7227 7320 6060 7374 6172 745f 7572 6c73  r's ``start_urls
+00003aa0: 6060 2061 7474 7269 6275 7465 2e20 4974  `` attribute. It
+00003ab0: 2061 6c6c 6f77 7320 746f 2070 6172 7365   allows to parse
+00003ac0: 0a20 2020 2020 2074 6865 2069 6e69 7469  .      the initi
+00003ad0: 616c 2072 6573 706f 6e73 6573 2061 6e64  al responses and
+00003ae0: 206d 7573 7420 7265 7475 726e 2065 6974   must return eit
+00003af0: 6865 7220 616e 0a20 2020 2020 203a 7265  her an.      :re
+00003b00: 663a 6069 7465 6d20 6f62 6a65 6374 203c  f:`item object <
+00003b10: 746f 7069 6373 2d69 7465 6d73 3e60 2c20  topics-items>`, 
+00003b20: 6120 3a63 6c61 7373 3a60 7e73 6372 6170  a :class:`~scrap
+00003b30: 792e 5265 7175 6573 7460 0a20 2020 2020  y.Request`.     
+00003b40: 206f 626a 6563 742c 206f 7220 616e 2069   object, or an i
+00003b50: 7465 7261 626c 6520 636f 6e74 6169 6e69  terable containi
+00003b60: 6e67 2061 6e79 206f 6620 7468 656d 2e0a  ng any of them..
+00003b70: 0a43 7261 776c 696e 6720 7275 6c65 730a  .Crawling rules.
+00003b80: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a  ~~~~~~~~~~~~~~..
+00003b90: 2e2e 2061 7574 6f63 6c61 7373 3a3a 2052  .. autoclass:: R
+00003ba0: 756c 650a 0a20 2020 6060 6c69 6e6b 5f65  ule..   ``link_e
+00003bb0: 7874 7261 6374 6f72 6060 2069 7320 6120  xtractor`` is a 
+00003bc0: 3a72 6566 3a60 4c69 6e6b 2045 7874 7261  :ref:`Link Extra
+00003bd0: 6374 6f72 203c 746f 7069 6373 2d6c 696e  ctor <topics-lin
+00003be0: 6b2d 6578 7472 6163 746f 7273 3e60 206f  k-extractors>` o
+00003bf0: 626a 6563 7420 7768 6963 680a 2020 2064  bject which.   d
+00003c00: 6566 696e 6573 2068 6f77 206c 696e 6b73  efines how links
+00003c10: 2077 696c 6c20 6265 2065 7874 7261 6374   will be extract
+00003c20: 6564 2066 726f 6d20 6561 6368 2063 7261  ed from each cra
+00003c30: 776c 6564 2070 6167 652e 2045 6163 6820  wled page. Each 
+00003c40: 7072 6f64 7563 6564 206c 696e 6b20 7769  produced link wi
+00003c50: 6c6c 0a20 2020 6265 2075 7365 6420 746f  ll.   be used to
+00003c60: 2067 656e 6572 6174 6520 6120 3a63 6c61   generate a :cla
+00003c70: 7373 3a60 7e73 6372 6170 792e 5265 7175  ss:`~scrapy.Requ
+00003c80: 6573 7460 206f 626a 6563 742c 2077 6869  est` object, whi
+00003c90: 6368 2077 696c 6c20 636f 6e74 6169 6e20  ch will contain 
+00003ca0: 7468 650a 2020 206c 696e 6b27 7320 7465  the.   link's te
+00003cb0: 7874 2069 6e20 6974 7320 6060 6d65 7461  xt in its ``meta
+00003cc0: 6060 2064 6963 7469 6f6e 6172 7920 2875  `` dictionary (u
+00003cd0: 6e64 6572 2074 6865 2060 606c 696e 6b5f  nder the ``link_
+00003ce0: 7465 7874 6060 206b 6579 292e 0a20 2020  text`` key)..   
+00003cf0: 4966 206f 6d69 7474 6564 2c20 6120 6465  If omitted, a de
+00003d00: 6661 756c 7420 6c69 6e6b 2065 7874 7261  fault link extra
+00003d10: 6374 6f72 2063 7265 6174 6564 2077 6974  ctor created wit
+00003d20: 6820 6e6f 2061 7267 756d 656e 7473 2077  h no arguments w
+00003d30: 696c 6c20 6265 2075 7365 642c 0a20 2020  ill be used,.   
+00003d40: 7265 7375 6c74 696e 6720 696e 2061 6c6c  resulting in all
+00003d50: 206c 696e 6b73 2062 6569 6e67 2065 7874   links being ext
+00003d60: 7261 6374 6564 2e0a 0a20 2020 6060 6361  racted...   ``ca
+00003d70: 6c6c 6261 636b 6060 2069 7320 6120 6361  llback`` is a ca
+00003d80: 6c6c 6162 6c65 206f 7220 6120 7374 7269  llable or a stri
+00003d90: 6e67 2028 696e 2077 6869 6368 2063 6173  ng (in which cas
+00003da0: 6520 6120 6d65 7468 6f64 2066 726f 6d20  e a method from 
+00003db0: 7468 6520 7370 6964 6572 0a20 2020 6f62  the spider.   ob
+00003dc0: 6a65 6374 2077 6974 6820 7468 6174 206e  ject with that n
+00003dd0: 616d 6520 7769 6c6c 2062 6520 7573 6564  ame will be used
+00003de0: 2920 746f 2062 6520 6361 6c6c 6564 2066  ) to be called f
+00003df0: 6f72 2065 6163 6820 6c69 6e6b 2065 7874  or each link ext
+00003e00: 7261 6374 6564 2077 6974 680a 2020 2074  racted with.   t
+00003e10: 6865 2073 7065 6369 6669 6564 206c 696e  he specified lin
+00003e20: 6b20 6578 7472 6163 746f 722e 2054 6869  k extractor. Thi
+00003e30: 7320 6361 6c6c 6261 636b 2072 6563 6569  s callback recei
+00003e40: 7665 7320 6120 3a63 6c61 7373 3a60 7e73  ves a :class:`~s
+00003e50: 6372 6170 792e 6874 7470 2e52 6573 706f  crapy.http.Respo
+00003e60: 6e73 6560 0a20 2020 6173 2069 7473 2066  nse`.   as its f
+00003e70: 6972 7374 2061 7267 756d 656e 7420 616e  irst argument an
+00003e80: 6420 6d75 7374 2072 6574 7572 6e20 6569  d must return ei
+00003e90: 7468 6572 2061 2073 696e 676c 6520 696e  ther a single in
+00003ea0: 7374 616e 6365 206f 7220 616e 2069 7465  stance or an ite
+00003eb0: 7261 626c 6520 6f66 0a20 2020 3a72 6566  rable of.   :ref
+00003ec0: 3a60 6974 656d 206f 626a 6563 7473 203c  :`item objects <
+00003ed0: 746f 7069 6373 2d69 7465 6d73 3e60 2061  topics-items>` a
+00003ee0: 6e64 2f6f 7220 3a63 6c61 7373 3a60 7e73  nd/or :class:`~s
+00003ef0: 6372 6170 792e 5265 7175 6573 7460 206f  crapy.Request` o
+00003f00: 626a 6563 7473 0a20 2020 286f 7220 616e  bjects.   (or an
+00003f10: 7920 7375 6263 6c61 7373 206f 6620 7468  y subclass of th
+00003f20: 656d 292e 2041 7320 6d65 6e74 696f 6e65  em). As mentione
+00003f30: 6420 6162 6f76 652c 2074 6865 2072 6563  d above, the rec
+00003f40: 6569 7665 6420 3a63 6c61 7373 3a60 7e73  eived :class:`~s
+00003f50: 6372 6170 792e 6874 7470 2e52 6573 706f  crapy.http.Respo
+00003f60: 6e73 6560 0a20 2020 6f62 6a65 6374 2077  nse`.   object w
+00003f70: 696c 6c20 636f 6e74 6169 6e20 7468 6520  ill contain the 
+00003f80: 7465 7874 206f 6620 7468 6520 6c69 6e6b  text of the link
+00003f90: 2074 6861 7420 7072 6f64 7563 6564 2074   that produced t
+00003fa0: 6865 203a 636c 6173 733a 607e 7363 7261  he :class:`~scra
+00003fb0: 7079 2e52 6571 7565 7374 600a 2020 2069  py.Request`.   i
+00003fc0: 6e20 6974 7320 6060 6d65 7461 6060 2064  n its ``meta`` d
+00003fd0: 6963 7469 6f6e 6172 7920 2875 6e64 6572  ictionary (under
+00003fe0: 2074 6865 2060 606c 696e 6b5f 7465 7874   the ``link_text
+00003ff0: 6060 206b 6579 290a 0a20 2020 6060 6362  `` key)..   ``cb
+00004000: 5f6b 7761 7267 7360 6020 6973 2061 2064  _kwargs`` is a d
+00004010: 6963 7420 636f 6e74 6169 6e69 6e67 2074  ict containing t
+00004020: 6865 206b 6579 776f 7264 2061 7267 756d  he keyword argum
+00004030: 656e 7473 2074 6f20 6265 2070 6173 7365  ents to be passe
+00004040: 6420 746f 2074 6865 0a20 2020 6361 6c6c  d to the.   call
+00004050: 6261 636b 2066 756e 6374 696f 6e2e 0a0a  back function...
+00004060: 2020 2060 6066 6f6c 6c6f 7760 6020 6973     ``follow`` is
+00004070: 2061 2062 6f6f 6c65 616e 2077 6869 6368   a boolean which
+00004080: 2073 7065 6369 6669 6573 2069 6620 6c69   specifies if li
+00004090: 6e6b 7320 7368 6f75 6c64 2062 6520 666f  nks should be fo
+000040a0: 6c6c 6f77 6564 2066 726f 6d20 6561 6368  llowed from each
+000040b0: 0a20 2020 7265 7370 6f6e 7365 2065 7874  .   response ext
+000040c0: 7261 6374 6564 2077 6974 6820 7468 6973  racted with this
+000040d0: 2072 756c 652e 2049 6620 6060 6361 6c6c   rule. If ``call
+000040e0: 6261 636b 6060 2069 7320 4e6f 6e65 2060  back`` is None `
+000040f0: 6066 6f6c 6c6f 7760 6020 6465 6661 756c  `follow`` defaul
+00004100: 7473 0a20 2020 746f 2060 6054 7275 6560  ts.   to ``True`
+00004110: 602c 206f 7468 6572 7769 7365 2069 7420  `, otherwise it 
+00004120: 6465 6661 756c 7473 2074 6f20 6060 4661  defaults to ``Fa
+00004130: 6c73 6560 602e 0a0a 2020 2060 6070 726f  lse``...   ``pro
+00004140: 6365 7373 5f6c 696e 6b73 6060 2069 7320  cess_links`` is 
+00004150: 6120 6361 6c6c 6162 6c65 2c20 6f72 2061  a callable, or a
+00004160: 2073 7472 696e 6720 2869 6e20 7768 6963   string (in whic
+00004170: 6820 6361 7365 2061 206d 6574 686f 6420  h case a method 
+00004180: 6672 6f6d 2074 6865 0a20 2020 7370 6964  from the.   spid
+00004190: 6572 206f 626a 6563 7420 7769 7468 2074  er object with t
+000041a0: 6861 7420 6e61 6d65 2077 696c 6c20 6265  hat name will be
+000041b0: 2075 7365 6429 2077 6869 6368 2077 696c   used) which wil
+000041c0: 6c20 6265 2063 616c 6c65 6420 666f 7220  l be called for 
+000041d0: 6561 6368 206c 6973 740a 2020 206f 6620  each list.   of 
+000041e0: 6c69 6e6b 7320 6578 7472 6163 7465 6420  links extracted 
+000041f0: 6672 6f6d 2065 6163 6820 7265 7370 6f6e  from each respon
+00004200: 7365 2075 7369 6e67 2074 6865 2073 7065  se using the spe
+00004210: 6369 6669 6564 2060 606c 696e 6b5f 6578  cified ``link_ex
+00004220: 7472 6163 746f 7260 602e 0a20 2020 5468  tractor``..   Th
+00004230: 6973 2069 7320 6d61 696e 6c79 2075 7365  is is mainly use
+00004240: 6420 666f 7220 6669 6c74 6572 696e 6720  d for filtering 
+00004250: 7075 7270 6f73 6573 2e0a 0a20 2020 6060  purposes...   ``
+00004260: 7072 6f63 6573 735f 7265 7175 6573 7460  process_request`
+00004270: 6020 6973 2061 2063 616c 6c61 626c 6520  ` is a callable 
+00004280: 286f 7220 6120 7374 7269 6e67 2c20 696e  (or a string, in
+00004290: 2077 6869 6368 2063 6173 6520 6120 6d65   which case a me
+000042a0: 7468 6f64 2066 726f 6d0a 2020 2074 6865  thod from.   the
+000042b0: 2073 7069 6465 7220 6f62 6a65 6374 2077   spider object w
+000042c0: 6974 6820 7468 6174 206e 616d 6520 7769  ith that name wi
+000042d0: 6c6c 2062 6520 7573 6564 2920 7768 6963  ll be used) whic
+000042e0: 6820 7769 6c6c 2062 6520 6361 6c6c 6564  h will be called
+000042f0: 2066 6f72 2065 7665 7279 0a20 2020 3a63   for every.   :c
+00004300: 6c61 7373 3a60 7e73 6372 6170 792e 5265  lass:`~scrapy.Re
+00004310: 7175 6573 7460 2065 7874 7261 6374 6564  quest` extracted
+00004320: 2062 7920 7468 6973 2072 756c 652e 2054   by this rule. T
+00004330: 6869 7320 6361 6c6c 6162 6c65 2073 686f  his callable sho
+00004340: 756c 640a 2020 2074 616b 6520 7361 6964  uld.   take said
+00004350: 2072 6571 7565 7374 2061 7320 6669 7273   request as firs
+00004360: 7420 6172 6775 6d65 6e74 2061 6e64 2074  t argument and t
+00004370: 6865 203a 636c 6173 733a 607e 7363 7261  he :class:`~scra
+00004380: 7079 2e68 7474 702e 5265 7370 6f6e 7365  py.http.Response
+00004390: 600a 2020 2066 726f 6d20 7768 6963 6820  `.   from which 
+000043a0: 7468 6520 7265 7175 6573 7420 6f72 6967  the request orig
+000043b0: 696e 6174 6564 2061 7320 7365 636f 6e64  inated as second
+000043c0: 2061 7267 756d 656e 742e 2049 7420 6d75   argument. It mu
+000043d0: 7374 2072 6574 7572 6e20 610a 2020 2060  st return a.   `
+000043e0: 6052 6571 7565 7374 6060 206f 626a 6563  `Request`` objec
+000043f0: 7420 6f72 2060 604e 6f6e 6560 6020 2874  t or ``None`` (t
+00004400: 6f20 6669 6c74 6572 206f 7574 2074 6865  o filter out the
+00004410: 2072 6571 7565 7374 292e 0a0a 2020 2060   request)...   `
+00004420: 6065 7272 6261 636b 6060 2069 7320 6120  `errback`` is a 
+00004430: 6361 6c6c 6162 6c65 206f 7220 6120 7374  callable or a st
+00004440: 7269 6e67 2028 696e 2077 6869 6368 2063  ring (in which c
+00004450: 6173 6520 6120 6d65 7468 6f64 2066 726f  ase a method fro
+00004460: 6d20 7468 6520 7370 6964 6572 0a20 2020  m the spider.   
+00004470: 6f62 6a65 6374 2077 6974 6820 7468 6174  object with that
+00004480: 206e 616d 6520 7769 6c6c 2062 6520 7573   name will be us
+00004490: 6564 2920 746f 2062 6520 6361 6c6c 6564  ed) to be called
+000044a0: 2069 6620 616e 7920 6578 6365 7074 696f   if any exceptio
+000044b0: 6e20 6973 0a20 2020 7261 6973 6564 2077  n is.   raised w
+000044c0: 6869 6c65 2070 726f 6365 7373 696e 6720  hile processing 
+000044d0: 6120 7265 7175 6573 7420 6765 6e65 7261  a request genera
+000044e0: 7465 6420 6279 2074 6865 2072 756c 652e  ted by the rule.
+000044f0: 0a20 2020 4974 2072 6563 6569 7665 7320  .   It receives 
+00004500: 6120 3a63 6c61 7373 3a60 5477 6973 7465  a :class:`Twiste
+00004510: 6420 4661 696c 7572 6520 3c74 7769 7374  d Failure <twist
+00004520: 6564 2e70 7974 686f 6e2e 6661 696c 7572  ed.python.failur
+00004530: 652e 4661 696c 7572 653e 600a 2020 2069  e.Failure>`.   i
+00004540: 6e73 7461 6e63 6520 6173 2066 6972 7374  nstance as first
+00004550: 2070 6172 616d 6574 6572 2e0a 0a20 2020   parameter...   
+00004560: 2e2e 2077 6172 6e69 6e67 3a3a 2042 6563  .. warning:: Bec
+00004570: 6175 7365 206f 6620 6974 7320 696e 7465  ause of its inte
+00004580: 726e 616c 2069 6d70 6c65 6d65 6e74 6174  rnal implementat
+00004590: 696f 6e2c 2079 6f75 206d 7573 7420 6578  ion, you must ex
+000045a0: 706c 6963 6974 6c79 2073 6574 0a20 2020  plicitly set.   
+000045b0: 2020 2063 616c 6c62 6163 6b73 2066 6f72     callbacks for
+000045c0: 206e 6577 2072 6571 7565 7374 7320 7768   new requests wh
+000045d0: 656e 2077 7269 7469 6e67 203a 636c 6173  en writing :clas
+000045e0: 733a 6043 7261 776c 5370 6964 6572 602d  s:`CrawlSpider`-
+000045f0: 6261 7365 6420 7370 6964 6572 733b 0a20  based spiders;. 
+00004600: 2020 2020 2075 6e65 7870 6563 7465 6420       unexpected 
+00004610: 6265 6861 7669 6f75 7220 6361 6e20 6f63  behaviour can oc
+00004620: 6375 7220 6f74 6865 7277 6973 652e 0a0a  cur otherwise...
+00004630: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
+00004640: 6564 3a3a 2032 2e30 0a20 2020 2020 2054  ed:: 2.0.      T
+00004650: 6865 202a 6572 7262 6163 6b2a 2070 6172  he *errback* par
+00004660: 616d 6574 6572 2e0a 0a43 7261 776c 5370  ameter...CrawlSp
+00004670: 6964 6572 2065 7861 6d70 6c65 0a7e 7e7e  ider example.~~~
+00004680: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00004690: 0a0a 4c65 7427 7320 6e6f 7720 7461 6b65  ..Let's now take
+000046a0: 2061 206c 6f6f 6b20 6174 2061 6e20 6578   a look at an ex
+000046b0: 616d 706c 6520 4372 6177 6c53 7069 6465  ample CrawlSpide
+000046c0: 7220 7769 7468 2072 756c 6573 3a0a 0a2e  r with rules:...
+000046d0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+000046e0: 7974 686f 6e0a 0a20 2020 2069 6d70 6f72  ython..    impor
+000046f0: 7420 7363 7261 7079 0a20 2020 2066 726f  t scrapy.    fro
+00004700: 6d20 7363 7261 7079 2e73 7069 6465 7273  m scrapy.spiders
+00004710: 2069 6d70 6f72 7420 4372 6177 6c53 7069   import CrawlSpi
+00004720: 6465 722c 2052 756c 650a 2020 2020 6672  der, Rule.    fr
+00004730: 6f6d 2073 6372 6170 792e 6c69 6e6b 6578  om scrapy.linkex
+00004740: 7472 6163 746f 7273 2069 6d70 6f72 7420  tractors import 
+00004750: 4c69 6e6b 4578 7472 6163 746f 720a 0a0a  LinkExtractor...
+00004760: 2020 2020 636c 6173 7320 4d79 5370 6964      class MySpid
+00004770: 6572 2843 7261 776c 5370 6964 6572 293a  er(CrawlSpider):
+00004780: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
+00004790: 2265 7861 6d70 6c65 2e63 6f6d 220a 2020  "example.com".  
+000047a0: 2020 2020 2020 616c 6c6f 7765 645f 646f        allowed_do
+000047b0: 6d61 696e 7320 3d20 5b22 6578 616d 706c  mains = ["exampl
+000047c0: 652e 636f 6d22 5d0a 2020 2020 2020 2020  e.com"].        
+000047d0: 7374 6172 745f 7572 6c73 203d 205b 2268  start_urls = ["h
+000047e0: 7474 703a 2f2f 7777 772e 6578 616d 706c  ttp://www.exampl
+000047f0: 652e 636f 6d22 5d0a 0a20 2020 2020 2020  e.com"]..       
+00004800: 2072 756c 6573 203d 2028 0a20 2020 2020   rules = (.     
+00004810: 2020 2020 2020 2023 2045 7874 7261 6374         # Extract
+00004820: 206c 696e 6b73 206d 6174 6368 696e 6720   links matching 
+00004830: 2763 6174 6567 6f72 792e 7068 7027 2028  'category.php' (
+00004840: 6275 7420 6e6f 7420 6d61 7463 6869 6e67  but not matching
+00004850: 2027 7375 6273 6563 7469 6f6e 2e70 6870   'subsection.php
+00004860: 2729 0a20 2020 2020 2020 2020 2020 2023  ').            #
+00004870: 2061 6e64 2066 6f6c 6c6f 7720 6c69 6e6b   and follow link
+00004880: 7320 6672 6f6d 2074 6865 6d20 2873 696e  s from them (sin
+00004890: 6365 206e 6f20 6361 6c6c 6261 636b 206d  ce no callback m
+000048a0: 6561 6e73 2066 6f6c 6c6f 773d 5472 7565  eans follow=True
+000048b0: 2062 7920 6465 6661 756c 7429 2e0a 2020   by default)..  
+000048c0: 2020 2020 2020 2020 2020 5275 6c65 284c            Rule(L
+000048d0: 696e 6b45 7874 7261 6374 6f72 2861 6c6c  inkExtractor(all
+000048e0: 6f77 3d28 7222 6361 7465 676f 7279 5c2e  ow=(r"category\.
+000048f0: 7068 7022 2c29 2c20 6465 6e79 3d28 7222  php",), deny=(r"
+00004900: 7375 6273 6563 7469 6f6e 5c2e 7068 7022  subsection\.php"
+00004910: 2c29 2929 2c0a 2020 2020 2020 2020 2020  ,))),.          
+00004920: 2020 2320 4578 7472 6163 7420 6c69 6e6b    # Extract link
+00004930: 7320 6d61 7463 6869 6e67 2027 6974 656d  s matching 'item
+00004940: 2e70 6870 2720 616e 6420 7061 7273 6520  .php' and parse 
+00004950: 7468 656d 2077 6974 6820 7468 6520 7370  them with the sp
+00004960: 6964 6572 2773 206d 6574 686f 6420 7061  ider's method pa
+00004970: 7273 655f 6974 656d 0a20 2020 2020 2020  rse_item.       
+00004980: 2020 2020 2052 756c 6528 4c69 6e6b 4578       Rule(LinkEx
+00004990: 7472 6163 746f 7228 616c 6c6f 773d 2872  tractor(allow=(r
+000049a0: 2269 7465 6d5c 2e70 6870 222c 2929 2c20  "item\.php",)), 
+000049b0: 6361 6c6c 6261 636b 3d22 7061 7273 655f  callback="parse_
+000049c0: 6974 656d 2229 2c0a 2020 2020 2020 2020  item"),.        
+000049d0: 290a 0a20 2020 2020 2020 2064 6566 2070  )..        def p
+000049e0: 6172 7365 5f69 7465 6d28 7365 6c66 2c20  arse_item(self, 
+000049f0: 7265 7370 6f6e 7365 293a 0a20 2020 2020  response):.     
+00004a00: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+00004a10: 6572 2e69 6e66 6f28 2248 692c 2074 6869  er.info("Hi, thi
+00004a20: 7320 6973 2061 6e20 6974 656d 2070 6167  s is an item pag
+00004a30: 6521 2025 7322 2c20 7265 7370 6f6e 7365  e! %s", response
+00004a40: 2e75 726c 290a 2020 2020 2020 2020 2020  .url).          
+00004a50: 2020 6974 656d 203d 2073 6372 6170 792e    item = scrapy.
+00004a60: 4974 656d 2829 0a20 2020 2020 2020 2020  Item().         
+00004a70: 2020 2069 7465 6d5b 2269 6422 5d20 3d20     item["id"] = 
+00004a80: 7265 7370 6f6e 7365 2e78 7061 7468 2827  response.xpath('
+00004a90: 2f2f 7464 5b40 6964 3d22 6974 656d 5f69  //td[@id="item_i
+00004aa0: 6422 5d2f 7465 7874 2829 2729 2e72 6528  d"]/text()').re(
+00004ab0: 7222 4944 3a20 285c 642b 2922 290a 2020  r"ID: (\d+)").  
+00004ac0: 2020 2020 2020 2020 2020 6974 656d 5b22            item["
+00004ad0: 6e61 6d65 225d 203d 2072 6573 706f 6e73  name"] = respons
+00004ae0: 652e 7870 6174 6828 272f 2f74 645b 4069  e.xpath('//td[@i
+00004af0: 643d 2269 7465 6d5f 6e61 6d65 225d 2f74  d="item_name"]/t
+00004b00: 6578 7428 2927 292e 6765 7428 290a 2020  ext()').get().  
+00004b10: 2020 2020 2020 2020 2020 6974 656d 5b22            item["
+00004b20: 6465 7363 7269 7074 696f 6e22 5d20 3d20  description"] = 
+00004b30: 7265 7370 6f6e 7365 2e78 7061 7468 280a  response.xpath(.
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 272f 2f74 645b 4069 643d 2269 7465 6d5f  '//td[@id="item_
+00004b60: 6465 7363 7269 7074 696f 6e22 5d2f 7465  description"]/te
+00004b70: 7874 2829 270a 2020 2020 2020 2020 2020  xt()'.          
+00004b80: 2020 292e 6765 7428 290a 2020 2020 2020    ).get().      
+00004b90: 2020 2020 2020 6974 656d 5b22 6c69 6e6b        item["link
+00004ba0: 5f74 6578 7422 5d20 3d20 7265 7370 6f6e  _text"] = respon
+00004bb0: 7365 2e6d 6574 615b 226c 696e 6b5f 7465  se.meta["link_te
+00004bc0: 7874 225d 0a20 2020 2020 2020 2020 2020  xt"].           
+00004bd0: 2075 726c 203d 2072 6573 706f 6e73 652e   url = response.
+00004be0: 7870 6174 6828 272f 2f74 645b 4069 643d  xpath('//td[@id=
+00004bf0: 2261 6464 6974 696f 6e61 6c5f 6461 7461  "additional_data
+00004c00: 225d 2f40 6872 6566 2729 2e67 6574 2829  "]/@href').get()
+00004c10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004c20: 7572 6e20 7265 7370 6f6e 7365 2e66 6f6c  urn response.fol
+00004c30: 6c6f 7728 0a20 2020 2020 2020 2020 2020  low(.           
+00004c40: 2020 2020 2075 726c 2c20 7365 6c66 2e70       url, self.p
+00004c50: 6172 7365 5f61 6464 6974 696f 6e61 6c5f  arse_additional_
+00004c60: 7061 6765 2c20 6362 5f6b 7761 7267 733d  page, cb_kwargs=
+00004c70: 6469 6374 2869 7465 6d3d 6974 656d 290a  dict(item=item).
+00004c80: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00004c90: 2020 2020 2020 2064 6566 2070 6172 7365         def parse
+00004ca0: 5f61 6464 6974 696f 6e61 6c5f 7061 6765  _additional_page
+00004cb0: 2873 656c 662c 2072 6573 706f 6e73 652c  (self, response,
+00004cc0: 2069 7465 6d29 3a0a 2020 2020 2020 2020   item):.        
+00004cd0: 2020 2020 6974 656d 5b22 6164 6469 7469      item["additi
+00004ce0: 6f6e 616c 5f64 6174 6122 5d20 3d20 7265  onal_data"] = re
+00004cf0: 7370 6f6e 7365 2e78 7061 7468 280a 2020  sponse.xpath(.  
+00004d00: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+00004d10: 2f70 5b40 6964 3d22 6164 6469 7469 6f6e  /p[@id="addition
+00004d20: 616c 5f64 6174 6122 5d2f 7465 7874 2829  al_data"]/text()
+00004d30: 270a 2020 2020 2020 2020 2020 2020 292e  '.            ).
+00004d40: 6765 7428 290a 2020 2020 2020 2020 2020  get().          
+00004d50: 2020 7265 7475 726e 2069 7465 6d0a 0a0a    return item...
+00004d60: 5468 6973 2073 7069 6465 7220 776f 756c  This spider woul
+00004d70: 6420 7374 6172 7420 6372 6177 6c69 6e67  d start crawling
+00004d80: 2065 7861 6d70 6c65 2e63 6f6d 2773 2068   example.com's h
+00004d90: 6f6d 6520 7061 6765 2c20 636f 6c6c 6563  ome page, collec
+00004da0: 7469 6e67 2063 6174 6567 6f72 790a 6c69  ting category.li
+00004db0: 6e6b 732c 2061 6e64 2069 7465 6d20 6c69  nks, and item li
+00004dc0: 6e6b 732c 2070 6172 7369 6e67 2074 6865  nks, parsing the
+00004dd0: 206c 6174 7465 7220 7769 7468 2074 6865   latter with the
+00004de0: 2060 6070 6172 7365 5f69 7465 6d60 6020   ``parse_item`` 
+00004df0: 6d65 7468 6f64 2e20 466f 720a 6561 6368  method. For.each
+00004e00: 2069 7465 6d20 7265 7370 6f6e 7365 2c20   item response, 
+00004e10: 736f 6d65 2064 6174 6120 7769 6c6c 2062  some data will b
+00004e20: 6520 6578 7472 6163 7465 6420 6672 6f6d  e extracted from
+00004e30: 2074 6865 2048 544d 4c20 7573 696e 6720   the HTML using 
+00004e40: 5850 6174 682c 2061 6e64 0a61 6e20 3a63  XPath, and.an :c
+00004e50: 6c61 7373 3a60 7e73 6372 6170 792e 4974  lass:`~scrapy.It
+00004e60: 656d 6020 7769 6c6c 2062 6520 6669 6c6c  em` will be fill
+00004e70: 6564 2077 6974 6820 6974 2e0a 0a58 4d4c  ed with it...XML
+00004e80: 4665 6564 5370 6964 6572 0a2d 2d2d 2d2d  FeedSpider.-----
+00004e90: 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2063 6c61  --------.... cla
+00004ea0: 7373 3a3a 2058 4d4c 4665 6564 5370 6964  ss:: XMLFeedSpid
+00004eb0: 6572 0a0a 2020 2020 584d 4c46 6565 6453  er..    XMLFeedS
+00004ec0: 7069 6465 7220 6973 2064 6573 6967 6e65  pider is designe
+00004ed0: 6420 666f 7220 7061 7273 696e 6720 584d  d for parsing XM
+00004ee0: 4c20 6665 6564 7320 6279 2069 7465 7261  L feeds by itera
+00004ef0: 7469 6e67 2074 6872 6f75 6768 2074 6865  ting through the
+00004f00: 6d20 6279 2061 0a20 2020 2063 6572 7461  m by a.    certa
+00004f10: 696e 206e 6f64 6520 6e61 6d65 2e20 2054  in node name.  T
+00004f20: 6865 2069 7465 7261 746f 7220 6361 6e20  he iterator can 
+00004f30: 6265 2063 686f 7365 6e20 6672 6f6d 3a20  be chosen from: 
+00004f40: 6060 6974 6572 6e6f 6465 7360 602c 2060  ``iternodes``, `
+00004f50: 6078 6d6c 6060 2c0a 2020 2020 616e 6420  `xml``,.    and 
+00004f60: 6060 6874 6d6c 6060 2e20 2049 7427 7320  ``html``.  It's 
+00004f70: 7265 636f 6d6d 656e 6465 6420 746f 2075  recommended to u
+00004f80: 7365 2074 6865 2060 6069 7465 726e 6f64  se the ``iternod
+00004f90: 6573 6060 2069 7465 7261 746f 7220 666f  es`` iterator fo
+00004fa0: 720a 2020 2020 7065 7266 6f72 6d61 6e63  r.    performanc
+00004fb0: 6520 7265 6173 6f6e 732c 2073 696e 6365  e reasons, since
+00004fc0: 2074 6865 2060 6078 6d6c 6060 2061 6e64   the ``xml`` and
+00004fd0: 2060 6068 746d 6c60 6020 6974 6572 6174   ``html`` iterat
+00004fe0: 6f72 7320 6765 6e65 7261 7465 2074 6865  ors generate the
+00004ff0: 0a20 2020 2077 686f 6c65 2044 4f4d 2061  .    whole DOM a
+00005000: 7420 6f6e 6365 2069 6e20 6f72 6465 7220  t once in order 
+00005010: 746f 2070 6172 7365 2069 742e 2020 486f  to parse it.  Ho
+00005020: 7765 7665 722c 2075 7369 6e67 2060 6068  wever, using ``h
+00005030: 746d 6c60 6020 6173 2074 6865 0a20 2020  tml`` as the.   
+00005040: 2069 7465 7261 746f 7220 6d61 7920 6265   iterator may be
+00005050: 2075 7365 6675 6c20 7768 656e 2070 6172   useful when par
+00005060: 7369 6e67 2058 4d4c 2077 6974 6820 6261  sing XML with ba
+00005070: 6420 6d61 726b 7570 2e0a 0a20 2020 2054  d markup...    T
+00005080: 6f20 7365 7420 7468 6520 6974 6572 6174  o set the iterat
+00005090: 6f72 2061 6e64 2074 6865 2074 6167 206e  or and the tag n
+000050a0: 616d 652c 2079 6f75 206d 7573 7420 6465  ame, you must de
+000050b0: 6669 6e65 2074 6865 2066 6f6c 6c6f 7769  fine the followi
+000050c0: 6e67 2063 6c61 7373 0a20 2020 2061 7474  ng class.    att
+000050d0: 7269 6275 7465 733a 0a0a 2020 2020 2e2e  ributes:..    ..
+000050e0: 2061 7474 7269 6275 7465 3a3a 2069 7465   attribute:: ite
+000050f0: 7261 746f 720a 0a20 2020 2020 2020 2041  rator..        A
+00005100: 2073 7472 696e 6720 7768 6963 6820 6465   string which de
+00005110: 6669 6e65 7320 7468 6520 6974 6572 6174  fines the iterat
+00005120: 6f72 2074 6f20 7573 652e 2049 7420 6361  or to use. It ca
+00005130: 6e20 6265 2065 6974 6865 723a 0a0a 2020  n be either:..  
+00005140: 2020 2020 2020 2020 202d 2060 6027 6974           - ``'it
+00005150: 6572 6e6f 6465 7327 6060 202d 2061 2066  ernodes'`` - a f
+00005160: 6173 7420 6974 6572 6174 6f72 2062 6173  ast iterator bas
+00005170: 6564 206f 6e20 7265 6775 6c61 7220 6578  ed on regular ex
+00005180: 7072 6573 7369 6f6e 730a 0a20 2020 2020  pressions..     
+00005190: 2020 2020 2020 2d20 6060 2768 746d 6c27        - ``'html'
+000051a0: 6060 202d 2061 6e20 6974 6572 6174 6f72  `` - an iterator
+000051b0: 2077 6869 6368 2075 7365 7320 3a63 6c61   which uses :cla
+000051c0: 7373 3a60 7e73 6372 6170 792e 5365 6c65  ss:`~scrapy.Sele
+000051d0: 6374 6f72 602e 0a20 2020 2020 2020 2020  ctor`..         
+000051e0: 2020 2020 4b65 6570 2069 6e20 6d69 6e64      Keep in mind
+000051f0: 2074 6869 7320 7573 6573 2044 4f4d 2070   this uses DOM p
+00005200: 6172 7369 6e67 2061 6e64 206d 7573 7420  arsing and must 
+00005210: 6c6f 6164 2061 6c6c 2044 4f4d 2069 6e20  load all DOM in 
+00005220: 6d65 6d6f 7279 0a20 2020 2020 2020 2020  memory.         
+00005230: 2020 2020 7768 6963 6820 636f 756c 6420      which could 
+00005240: 6265 2061 2070 726f 626c 656d 2066 6f72  be a problem for
+00005250: 2062 6967 2066 6565 6473 0a0a 2020 2020   big feeds..    
+00005260: 2020 2020 2020 202d 2060 6027 786d 6c27         - ``'xml'
+00005270: 6060 202d 2061 6e20 6974 6572 6174 6f72  `` - an iterator
+00005280: 2077 6869 6368 2075 7365 7320 3a63 6c61   which uses :cla
+00005290: 7373 3a60 7e73 6372 6170 792e 5365 6c65  ss:`~scrapy.Sele
+000052a0: 6374 6f72 602e 0a20 2020 2020 2020 2020  ctor`..         
+000052b0: 2020 2020 4b65 6570 2069 6e20 6d69 6e64      Keep in mind
+000052c0: 2074 6869 7320 7573 6573 2044 4f4d 2070   this uses DOM p
+000052d0: 6172 7369 6e67 2061 6e64 206d 7573 7420  arsing and must 
+000052e0: 6c6f 6164 2061 6c6c 2044 4f4d 2069 6e20  load all DOM in 
+000052f0: 6d65 6d6f 7279 0a20 2020 2020 2020 2020  memory.         
+00005300: 2020 2020 7768 6963 6820 636f 756c 6420      which could 
+00005310: 6265 2061 2070 726f 626c 656d 2066 6f72  be a problem for
+00005320: 2062 6967 2066 6565 6473 0a0a 2020 2020   big feeds..    
+00005330: 2020 2020 4974 2064 6566 6175 6c74 7320      It defaults 
+00005340: 746f 3a20 6060 2769 7465 726e 6f64 6573  to: ``'iternodes
+00005350: 2760 602e 0a0a 2020 2020 2e2e 2061 7474  '``...    .. att
+00005360: 7269 6275 7465 3a3a 2069 7465 7274 6167  ribute:: itertag
+00005370: 0a0a 2020 2020 2020 2020 4120 7374 7269  ..        A stri
+00005380: 6e67 2077 6974 6820 7468 6520 6e61 6d65  ng with the name
+00005390: 206f 6620 7468 6520 6e6f 6465 2028 6f72   of the node (or
+000053a0: 2065 6c65 6d65 6e74 2920 746f 2069 7465   element) to ite
+000053b0: 7261 7465 2069 6e2e 2045 7861 6d70 6c65  rate in. Example
+000053c0: 3a3a 0a0a 2020 2020 2020 2020 2020 2020  ::..            
+000053d0: 6974 6572 7461 6720 3d20 2770 726f 6475  itertag = 'produ
+000053e0: 6374 270a 0a20 2020 202e 2e20 6174 7472  ct'..    .. attr
+000053f0: 6962 7574 653a 3a20 6e61 6d65 7370 6163  ibute:: namespac
+00005400: 6573 0a0a 2020 2020 2020 2020 4120 6c69  es..        A li
+00005410: 7374 206f 6620 6060 2870 7265 6669 782c  st of ``(prefix,
+00005420: 2075 7269 2960 6020 7475 706c 6573 2077   uri)`` tuples w
+00005430: 6869 6368 2064 6566 696e 6520 7468 6520  hich define the 
+00005440: 6e61 6d65 7370 6163 6573 0a20 2020 2020  namespaces.     
+00005450: 2020 2061 7661 696c 6162 6c65 2069 6e20     available in 
+00005460: 7468 6174 2064 6f63 756d 656e 7420 7468  that document th
+00005470: 6174 2077 696c 6c20 6265 2070 726f 6365  at will be proce
+00005480: 7373 6564 2077 6974 6820 7468 6973 2073  ssed with this s
+00005490: 7069 6465 722e 2054 6865 0a20 2020 2020  pider. The.     
+000054a0: 2020 2060 6070 7265 6669 7860 6020 616e     ``prefix`` an
+000054b0: 6420 6060 7572 6960 6020 7769 6c6c 2062  d ``uri`` will b
+000054c0: 6520 7573 6564 2074 6f20 6175 746f 6d61  e used to automa
+000054d0: 7469 6361 6c6c 7920 7265 6769 7374 6572  tically register
+000054e0: 0a20 2020 2020 2020 206e 616d 6573 7061  .        namespa
+000054f0: 6365 7320 7573 696e 6720 7468 650a 2020  ces using the.  
+00005500: 2020 2020 2020 3a6d 6574 683a 607e 7363        :meth:`~sc
+00005510: 7261 7079 2e53 656c 6563 746f 722e 7265  rapy.Selector.re
+00005520: 6769 7374 6572 5f6e 616d 6573 7061 6365  gister_namespace
+00005530: 6020 6d65 7468 6f64 2e0a 0a20 2020 2020  ` method...     
+00005540: 2020 2059 6f75 2063 616e 2074 6865 6e20     You can then 
+00005550: 7370 6563 6966 7920 6e6f 6465 7320 7769  specify nodes wi
+00005560: 7468 206e 616d 6573 7061 6365 7320 696e  th namespaces in
+00005570: 2074 6865 203a 6174 7472 3a60 6974 6572   the :attr:`iter
+00005580: 7461 6760 0a20 2020 2020 2020 2061 7474  tag`.        att
+00005590: 7269 6275 7465 2e0a 0a20 2020 2020 2020  ribute...       
+000055a0: 2045 7861 6d70 6c65 3a3a 0a0a 2020 2020   Example::..    
+000055b0: 2020 2020 2020 2020 636c 6173 7320 596f          class Yo
+000055c0: 7572 5370 6964 6572 2858 4d4c 4665 6564  urSpider(XMLFeed
+000055d0: 5370 6964 6572 293a 0a0a 2020 2020 2020  Spider):..      
+000055e0: 2020 2020 2020 2020 2020 6e61 6d65 7370            namesp
+000055f0: 6163 6573 203d 205b 2827 6e27 2c20 2768  aces = [('n', 'h
+00005600: 7474 703a 2f2f 7777 772e 7369 7465 6d61  ttp://www.sitema
+00005610: 7073 2e6f 7267 2f73 6368 656d 6173 2f73  ps.org/schemas/s
+00005620: 6974 656d 6170 2f30 2e39 2729 5d0a 2020  itemap/0.9')].  
+00005630: 2020 2020 2020 2020 2020 2020 2020 6974                it
+00005640: 6572 7461 6720 3d20 276e 3a75 726c 270a  ertag = 'n:url'.
+00005650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005660: 2320 2e2e 2e0a 0a20 2020 2041 7061 7274  # .....    Apart
+00005670: 2066 726f 6d20 7468 6573 6520 6e65 7720   from these new 
+00005680: 6174 7472 6962 7574 6573 2c20 7468 6973  attributes, this
+00005690: 2073 7069 6465 7220 6861 7320 7468 6520   spider has the 
+000056a0: 666f 6c6c 6f77 696e 6720 6f76 6572 7269  following overri
+000056b0: 6461 626c 650a 2020 2020 6d65 7468 6f64  dable.    method
+000056c0: 7320 746f 6f3a 0a0a 2020 2020 2e2e 206d  s too:..    .. m
+000056d0: 6574 686f 643a 3a20 6164 6170 745f 7265  ethod:: adapt_re
+000056e0: 7370 6f6e 7365 2872 6573 706f 6e73 6529  sponse(response)
+000056f0: 0a0a 2020 2020 2020 2020 4120 6d65 7468  ..        A meth
+00005700: 6f64 2074 6861 7420 7265 6365 6976 6573  od that receives
+00005710: 2074 6865 2072 6573 706f 6e73 6520 6173   the response as
+00005720: 2073 6f6f 6e20 6173 2069 7420 6172 7269   soon as it arri
+00005730: 7665 7320 6672 6f6d 2074 6865 2073 7069  ves from the spi
+00005740: 6465 720a 2020 2020 2020 2020 6d69 6464  der.        midd
+00005750: 6c65 7761 7265 2c20 6265 666f 7265 2074  leware, before t
+00005760: 6865 2073 7069 6465 7220 7374 6172 7473  he spider starts
+00005770: 2070 6172 7369 6e67 2069 742e 2049 7420   parsing it. It 
+00005780: 6361 6e20 6265 2075 7365 6420 746f 206d  can be used to m
+00005790: 6f64 6966 790a 2020 2020 2020 2020 7468  odify.        th
+000057a0: 6520 7265 7370 6f6e 7365 2062 6f64 7920  e response body 
+000057b0: 6265 666f 7265 2070 6172 7369 6e67 2069  before parsing i
+000057c0: 742e 2054 6869 7320 6d65 7468 6f64 2072  t. This method r
+000057d0: 6563 6569 7665 7320 6120 7265 7370 6f6e  eceives a respon
+000057e0: 7365 2061 6e64 0a20 2020 2020 2020 2061  se and.        a
+000057f0: 6c73 6f20 7265 7475 726e 7320 6120 7265  lso returns a re
+00005800: 7370 6f6e 7365 2028 6974 2063 6f75 6c64  sponse (it could
+00005810: 2062 6520 7468 6520 7361 6d65 206f 7220   be the same or 
+00005820: 616e 6f74 6865 7220 6f6e 6529 2e0a 0a20  another one)... 
+00005830: 2020 202e 2e20 6d65 7468 6f64 3a3a 2070     .. method:: p
+00005840: 6172 7365 5f6e 6f64 6528 7265 7370 6f6e  arse_node(respon
+00005850: 7365 2c20 7365 6c65 6374 6f72 290a 0a20  se, selector).. 
+00005860: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+00005870: 6f64 2069 7320 6361 6c6c 6564 2066 6f72  od is called for
+00005880: 2074 6865 206e 6f64 6573 206d 6174 6368   the nodes match
+00005890: 696e 6720 7468 6520 7072 6f76 6964 6564  ing the provided
+000058a0: 2074 6167 206e 616d 650a 2020 2020 2020   tag name.      
+000058b0: 2020 2860 6069 7465 7274 6167 6060 292e    (``itertag``).
+000058c0: 2020 5265 6365 6976 6573 2074 6865 2072    Receives the r
+000058d0: 6573 706f 6e73 6520 616e 6420 616e 0a20  esponse and an. 
+000058e0: 2020 2020 2020 203a 636c 6173 733a 607e         :class:`~
+000058f0: 7363 7261 7079 2e53 656c 6563 746f 7260  scrapy.Selector`
+00005900: 2066 6f72 2065 6163 6820 6e6f 6465 2e20   for each node. 
+00005910: 204f 7665 7272 6964 696e 6720 7468 6973   Overriding this
+00005920: 0a20 2020 2020 2020 206d 6574 686f 6420  .        method 
+00005930: 6973 206d 616e 6461 746f 7279 2e20 4f74  is mandatory. Ot
+00005940: 6865 7277 6973 652c 2079 6f75 2073 7069  herwise, you spi
+00005950: 6465 7220 776f 6e27 7420 776f 726b 2e20  der won't work. 
+00005960: 2054 6869 7320 6d65 7468 6f64 0a20 2020   This method.   
+00005970: 2020 2020 206d 7573 7420 7265 7475 726e       must return
+00005980: 2061 6e20 3a72 6566 3a60 6974 656d 206f   an :ref:`item o
+00005990: 626a 6563 7420 3c74 6f70 6963 732d 6974  bject <topics-it
+000059a0: 656d 733e 602c 2061 0a20 2020 2020 2020  ems>`, a.       
+000059b0: 203a 636c 6173 733a 607e 7363 7261 7079   :class:`~scrapy
+000059c0: 2e52 6571 7565 7374 6020 6f62 6a65 6374  .Request` object
+000059d0: 2c20 6f72 2061 6e20 6974 6572 6162 6c65  , or an iterable
+000059e0: 2063 6f6e 7461 696e 696e 6720 616e 7920   containing any 
+000059f0: 6f66 0a20 2020 2020 2020 2074 6865 6d2e  of.        them.
+00005a00: 0a0a 2020 2020 2e2e 206d 6574 686f 643a  ..    .. method:
+00005a10: 3a20 7072 6f63 6573 735f 7265 7375 6c74  : process_result
+00005a20: 7328 7265 7370 6f6e 7365 2c20 7265 7375  s(response, resu
+00005a30: 6c74 7329 0a0a 2020 2020 2020 2020 5468  lts)..        Th
+00005a40: 6973 206d 6574 686f 6420 6973 2063 616c  is method is cal
+00005a50: 6c65 6420 666f 7220 6561 6368 2072 6573  led for each res
+00005a60: 756c 7420 2869 7465 6d20 6f72 2072 6571  ult (item or req
+00005a70: 7565 7374 2920 7265 7475 726e 6564 2062  uest) returned b
+00005a80: 7920 7468 650a 2020 2020 2020 2020 7370  y the.        sp
+00005a90: 6964 6572 2c20 616e 6420 6974 2773 2069  ider, and it's i
+00005aa0: 6e74 656e 6465 6420 746f 2070 6572 666f  ntended to perfo
+00005ab0: 726d 2061 6e79 206c 6173 7420 7469 6d65  rm any last time
+00005ac0: 2070 726f 6365 7373 696e 6720 7265 7175   processing requ
+00005ad0: 6972 6564 0a20 2020 2020 2020 2062 6566  ired.        bef
+00005ae0: 6f72 6520 7265 7475 726e 696e 6720 7468  ore returning th
+00005af0: 6520 7265 7375 6c74 7320 746f 2074 6865  e results to the
+00005b00: 2066 7261 6d65 776f 726b 2063 6f72 652c   framework core,
+00005b10: 2066 6f72 2065 7861 6d70 6c65 2073 6574   for example set
+00005b20: 7469 6e67 2074 6865 0a20 2020 2020 2020  ting the.       
+00005b30: 2069 7465 6d20 4944 732e 2049 7420 7265   item IDs. It re
+00005b40: 6365 6976 6573 2061 206c 6973 7420 6f66  ceives a list of
+00005b50: 2072 6573 756c 7473 2061 6e64 2074 6865   results and the
+00005b60: 2072 6573 706f 6e73 6520 7768 6963 6820   response which 
+00005b70: 6f72 6967 696e 6174 6564 0a20 2020 2020  originated.     
+00005b80: 2020 2074 686f 7365 2072 6573 756c 7473     those results
+00005b90: 2e20 4974 206d 7573 7420 7265 7475 726e  . It must return
+00005ba0: 2061 206c 6973 7420 6f66 2072 6573 756c   a list of resul
+00005bb0: 7473 2028 6974 656d 7320 6f72 2072 6571  ts (items or req
+00005bc0: 7565 7374 7329 2e0a 0a20 2020 202e 2e20  uests)...    .. 
+00005bd0: 7761 726e 696e 673a 3a20 4265 6361 7573  warning:: Becaus
+00005be0: 6520 6f66 2069 7473 2069 6e74 6572 6e61  e of its interna
+00005bf0: 6c20 696d 706c 656d 656e 7461 7469 6f6e  l implementation
+00005c00: 2c20 796f 7520 6d75 7374 2065 7870 6c69  , you must expli
+00005c10: 6369 746c 7920 7365 740a 2020 2020 2020  citly set.      
+00005c20: 2063 616c 6c62 6163 6b73 2066 6f72 206e   callbacks for n
+00005c30: 6577 2072 6571 7565 7374 7320 7768 656e  ew requests when
+00005c40: 2077 7269 7469 6e67 203a 636c 6173 733a   writing :class:
+00005c50: 6058 4d4c 4665 6564 5370 6964 6572 602d  `XMLFeedSpider`-
+00005c60: 6261 7365 6420 7370 6964 6572 733b 0a20  based spiders;. 
+00005c70: 2020 2020 2020 756e 6578 7065 6374 6564        unexpected
+00005c80: 2062 6568 6176 696f 7572 2063 616e 206f   behaviour can o
+00005c90: 6363 7572 206f 7468 6572 7769 7365 2e0a  ccur otherwise..
+00005ca0: 0a0a 584d 4c46 6565 6453 7069 6465 7220  ..XMLFeedSpider 
+00005cb0: 6578 616d 706c 650a 7e7e 7e7e 7e7e 7e7e  example.~~~~~~~~
+00005cc0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a54  ~~~~~~~~~~~~~..T
+00005cd0: 6865 7365 2073 7069 6465 7273 2061 7265  hese spiders are
+00005ce0: 2070 7265 7474 7920 6561 7379 2074 6f20   pretty easy to 
+00005cf0: 7573 652c 206c 6574 2773 2068 6176 6520  use, let's have 
+00005d00: 6120 6c6f 6f6b 2061 7420 6f6e 6520 6578  a look at one ex
+00005d10: 616d 706c 653a 0a0a 2e2e 2073 6b69 703a  ample:.... skip:
+00005d20: 206e 6578 740a 2e2e 2063 6f64 652d 626c   next... code-bl
+00005d30: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+00005d40: 2020 6672 6f6d 2073 6372 6170 792e 7370    from scrapy.sp
+00005d50: 6964 6572 7320 696d 706f 7274 2058 4d4c  iders import XML
+00005d60: 4665 6564 5370 6964 6572 0a20 2020 2066  FeedSpider.    f
+00005d70: 726f 6d20 6d79 7072 6f6a 6563 742e 6974  rom myproject.it
+00005d80: 656d 7320 696d 706f 7274 2054 6573 7449  ems import TestI
+00005d90: 7465 6d0a 0a0a 2020 2020 636c 6173 7320  tem...    class 
+00005da0: 4d79 5370 6964 6572 2858 4d4c 4665 6564  MySpider(XMLFeed
+00005db0: 5370 6964 6572 293a 0a20 2020 2020 2020  Spider):.       
+00005dc0: 206e 616d 6520 3d20 2265 7861 6d70 6c65   name = "example
+00005dd0: 2e63 6f6d 220a 2020 2020 2020 2020 616c  .com".        al
+00005de0: 6c6f 7765 645f 646f 6d61 696e 7320 3d20  lowed_domains = 
+00005df0: 5b22 6578 616d 706c 652e 636f 6d22 5d0a  ["example.com"].
+00005e00: 2020 2020 2020 2020 7374 6172 745f 7572          start_ur
+00005e10: 6c73 203d 205b 2268 7474 703a 2f2f 7777  ls = ["http://ww
+00005e20: 772e 6578 616d 706c 652e 636f 6d2f 6665  w.example.com/fe
+00005e30: 6564 2e78 6d6c 225d 0a20 2020 2020 2020  ed.xml"].       
+00005e40: 2069 7465 7261 746f 7220 3d20 2269 7465   iterator = "ite
+00005e50: 726e 6f64 6573 2220 2023 2054 6869 7320  rnodes"  # This 
+00005e60: 6973 2061 6374 7561 6c6c 7920 756e 6e65  is actually unne
+00005e70: 6365 7373 6172 792c 2073 696e 6365 2069  cessary, since i
+00005e80: 7427 7320 7468 6520 6465 6661 756c 7420  t's the default 
+00005e90: 7661 6c75 650a 2020 2020 2020 2020 6974  value.        it
+00005ea0: 6572 7461 6720 3d20 2269 7465 6d22 0a0a  ertag = "item"..
+00005eb0: 2020 2020 2020 2020 6465 6620 7061 7273          def pars
+00005ec0: 655f 6e6f 6465 2873 656c 662c 2072 6573  e_node(self, res
+00005ed0: 706f 6e73 652c 206e 6f64 6529 3a0a 2020  ponse, node):.  
+00005ee0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00005ef0: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
+00005f00: 2020 2020 2020 2020 2020 2020 2248 692c              "Hi,
+00005f10: 2074 6869 7320 6973 2061 203c 2573 3e20   this is a <%s> 
+00005f20: 6e6f 6465 213a 2025 7322 2c20 7365 6c66  node!: %s", self
+00005f30: 2e69 7465 7274 6167 2c20 2222 2e6a 6f69  .itertag, "".joi
+00005f40: 6e28 6e6f 6465 2e67 6574 616c 6c28 2929  n(node.getall())
+00005f50: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00005f60: 2020 2020 2020 2020 2020 2020 6974 656d              item
+00005f70: 203d 2054 6573 7449 7465 6d28 290a 2020   = TestItem().  
+00005f80: 2020 2020 2020 2020 2020 6974 656d 5b22            item["
+00005f90: 6964 225d 203d 206e 6f64 652e 7870 6174  id"] = node.xpat
+00005fa0: 6828 2240 6964 2229 2e67 6574 2829 0a20  h("@id").get(). 
+00005fb0: 2020 2020 2020 2020 2020 2069 7465 6d5b             item[
+00005fc0: 226e 616d 6522 5d20 3d20 6e6f 6465 2e78  "name"] = node.x
+00005fd0: 7061 7468 2822 6e61 6d65 2229 2e67 6574  path("name").get
+00005fe0: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+00005ff0: 7465 6d5b 2264 6573 6372 6970 7469 6f6e  tem["description
+00006000: 225d 203d 206e 6f64 652e 7870 6174 6828  "] = node.xpath(
+00006010: 2264 6573 6372 6970 7469 6f6e 2229 2e67  "description").g
+00006020: 6574 2829 0a20 2020 2020 2020 2020 2020  et().           
+00006030: 2072 6574 7572 6e20 6974 656d 0a0a 4261   return item..Ba
+00006040: 7369 6361 6c6c 7920 7768 6174 2077 6520  sically what we 
+00006050: 6469 6420 7570 2074 6865 7265 2077 6173  did up there was
+00006060: 2074 6f20 6372 6561 7465 2061 2073 7069   to create a spi
+00006070: 6465 7220 7468 6174 2064 6f77 6e6c 6f61  der that downloa
+00006080: 6473 2061 2066 6565 6420 6672 6f6d 0a74  ds a feed from.t
+00006090: 6865 2067 6976 656e 2060 6073 7461 7274  he given ``start
+000060a0: 5f75 726c 7360 602c 2061 6e64 2074 6865  _urls``, and the
+000060b0: 6e20 6974 6572 6174 6573 2074 6872 6f75  n iterates throu
+000060c0: 6768 2065 6163 6820 6f66 2069 7473 2060  gh each of its `
+000060d0: 6069 7465 6d60 6020 7461 6773 2c0a 7072  `item`` tags,.pr
+000060e0: 696e 7473 2074 6865 6d20 6f75 742c 2061  ints them out, a
+000060f0: 6e64 2073 746f 7265 7320 736f 6d65 2072  nd stores some r
+00006100: 616e 646f 6d20 6461 7461 2069 6e20 616e  andom data in an
+00006110: 203a 636c 6173 733a 607e 7363 7261 7079   :class:`~scrapy
+00006120: 2e49 7465 6d60 2e0a 0a43 5356 4665 6564  .Item`...CSVFeed
+00006130: 5370 6964 6572 0a2d 2d2d 2d2d 2d2d 2d2d  Spider.---------
+00006140: 2d2d 2d2d 0a0a 2e2e 2063 6c61 7373 3a3a  ----.... class::
+00006150: 2043 5356 4665 6564 5370 6964 6572 0a0a   CSVFeedSpider..
+00006160: 2020 2054 6869 7320 7370 6964 6572 2069     This spider i
+00006170: 7320 7665 7279 2073 696d 696c 6172 2074  s very similar t
+00006180: 6f20 7468 6520 584d 4c46 6565 6453 7069  o the XMLFeedSpi
+00006190: 6465 722c 2065 7863 6570 7420 7468 6174  der, except that
+000061a0: 2069 7420 6974 6572 6174 6573 0a20 2020   it iterates.   
+000061b0: 6f76 6572 2072 6f77 732c 2069 6e73 7465  over rows, inste
+000061c0: 6164 206f 6620 6e6f 6465 732e 2054 6865  ad of nodes. The
+000061d0: 206d 6574 686f 6420 7468 6174 2067 6574   method that get
+000061e0: 7320 6361 6c6c 6564 2069 6e20 6561 6368  s called in each
+000061f0: 2069 7465 7261 7469 6f6e 0a20 2020 6973   iteration.   is
+00006200: 203a 6d65 7468 3a60 7061 7273 655f 726f   :meth:`parse_ro
+00006210: 7760 2e0a 0a20 2020 2e2e 2061 7474 7269  w`...   .. attri
+00006220: 6275 7465 3a3a 2064 656c 696d 6974 6572  bute:: delimiter
+00006230: 0a0a 2020 2020 2020 2041 2073 7472 696e  ..       A strin
+00006240: 6720 7769 7468 2074 6865 2073 6570 6172  g with the separ
+00006250: 6174 6f72 2063 6861 7261 6374 6572 2066  ator character f
+00006260: 6f72 2065 6163 6820 6669 656c 6420 696e  or each field in
+00006270: 2074 6865 2043 5356 2066 696c 650a 2020   the CSV file.  
+00006280: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00006290: 2060 6027 2c27 6060 2028 636f 6d6d 6129   ``','`` (comma)
+000062a0: 2e0a 0a20 2020 2e2e 2061 7474 7269 6275  ...   .. attribu
+000062b0: 7465 3a3a 2071 756f 7465 6368 6172 0a0a  te:: quotechar..
+000062c0: 2020 2020 2020 2041 2073 7472 696e 6720         A string 
+000062d0: 7769 7468 2074 6865 2065 6e63 6c6f 7375  with the enclosu
+000062e0: 7265 2063 6861 7261 6374 6572 2066 6f72  re character for
+000062f0: 2065 6163 6820 6669 656c 6420 696e 2074   each field in t
+00006300: 6865 2043 5356 2066 696c 650a 2020 2020  he CSV file.    
+00006310: 2020 2044 6566 6175 6c74 7320 746f 2060     Defaults to `
+00006320: 6027 2227 6060 2028 7175 6f74 6174 696f  `'"'`` (quotatio
+00006330: 6e20 6d61 726b 292e 0a0a 2020 202e 2e20  n mark)...   .. 
+00006340: 6174 7472 6962 7574 653a 3a20 6865 6164  attribute:: head
+00006350: 6572 730a 0a20 2020 2020 2020 4120 6c69  ers..       A li
+00006360: 7374 206f 6620 7468 6520 636f 6c75 6d6e  st of the column
+00006370: 206e 616d 6573 2069 6e20 7468 6520 4353   names in the CS
+00006380: 5620 6669 6c65 2e0a 0a20 2020 2e2e 206d  V file...   .. m
+00006390: 6574 686f 643a 3a20 7061 7273 655f 726f  ethod:: parse_ro
+000063a0: 7728 7265 7370 6f6e 7365 2c20 726f 7729  w(response, row)
+000063b0: 0a0a 2020 2020 2020 2052 6563 6569 7665  ..       Receive
+000063c0: 7320 6120 7265 7370 6f6e 7365 2061 6e64  s a response and
+000063d0: 2061 2064 6963 7420 2872 6570 7265 7365   a dict (represe
+000063e0: 6e74 696e 6720 6561 6368 2072 6f77 2920  nting each row) 
+000063f0: 7769 7468 2061 206b 6579 2066 6f72 2065  with a key for e
+00006400: 6163 680a 2020 2020 2020 2070 726f 7669  ach.       provi
+00006410: 6465 6420 286f 7220 6465 7465 6374 6564  ded (or detected
+00006420: 2920 6865 6164 6572 206f 6620 7468 6520  ) header of the 
+00006430: 4353 5620 6669 6c65 2e20 2054 6869 7320  CSV file.  This 
+00006440: 7370 6964 6572 2061 6c73 6f20 6769 7665  spider also give
+00006450: 7320 7468 650a 2020 2020 2020 206f 7070  s the.       opp
+00006460: 6f72 7475 6e69 7479 2074 6f20 6f76 6572  ortunity to over
+00006470: 7269 6465 2060 6061 6461 7074 5f72 6573  ride ``adapt_res
+00006480: 706f 6e73 6560 6020 616e 6420 6060 7072  ponse`` and ``pr
+00006490: 6f63 6573 735f 7265 7375 6c74 7360 6020  ocess_results`` 
+000064a0: 6d65 7468 6f64 730a 2020 2020 2020 2066  methods.       f
+000064b0: 6f72 2070 7265 2d20 616e 6420 706f 7374  or pre- and post
+000064c0: 2d70 726f 6365 7373 696e 6720 7075 7270  -processing purp
+000064d0: 6f73 6573 2e0a 0a43 5356 4665 6564 5370  oses...CSVFeedSp
+000064e0: 6964 6572 2065 7861 6d70 6c65 0a7e 7e7e  ider example.~~~
+000064f0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00006500: 7e7e 0a0a 4c65 7427 7320 7365 6520 616e  ~~..Let's see an
+00006510: 2065 7861 6d70 6c65 2073 696d 696c 6172   example similar
+00006520: 2074 6f20 7468 6520 7072 6576 696f 7573   to the previous
+00006530: 206f 6e65 2c20 6275 7420 7573 696e 6720   one, but using 
+00006540: 610a 3a63 6c61 7373 3a60 4353 5646 6565  a.:class:`CSVFee
+00006550: 6453 7069 6465 7260 3a0a 0a2e 2e20 736b  dSpider`:.... sk
+00006560: 6970 3a20 6e65 7874 0a2e 2e20 636f 6465  ip: next... code
+00006570: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00006580: 0a20 2020 2066 726f 6d20 7363 7261 7079  .    from scrapy
+00006590: 2e73 7069 6465 7273 2069 6d70 6f72 7420  .spiders import 
+000065a0: 4353 5646 6565 6453 7069 6465 720a 2020  CSVFeedSpider.  
+000065b0: 2020 6672 6f6d 206d 7970 726f 6a65 6374    from myproject
+000065c0: 2e69 7465 6d73 2069 6d70 6f72 7420 5465  .items import Te
+000065d0: 7374 4974 656d 0a0a 0a20 2020 2063 6c61  stItem...    cla
+000065e0: 7373 204d 7953 7069 6465 7228 4353 5646  ss MySpider(CSVF
+000065f0: 6565 6453 7069 6465 7229 3a0a 2020 2020  eedSpider):.    
+00006600: 2020 2020 6e61 6d65 203d 2022 6578 616d      name = "exam
+00006610: 706c 652e 636f 6d22 0a20 2020 2020 2020  ple.com".       
+00006620: 2061 6c6c 6f77 6564 5f64 6f6d 6169 6e73   allowed_domains
+00006630: 203d 205b 2265 7861 6d70 6c65 2e63 6f6d   = ["example.com
+00006640: 225d 0a20 2020 2020 2020 2073 7461 7274  "].        start
+00006650: 5f75 726c 7320 3d20 5b22 6874 7470 3a2f  _urls = ["http:/
+00006660: 2f77 7777 2e65 7861 6d70 6c65 2e63 6f6d  /www.example.com
+00006670: 2f66 6565 642e 6373 7622 5d0a 2020 2020  /feed.csv"].    
+00006680: 2020 2020 6465 6c69 6d69 7465 7220 3d20      delimiter = 
+00006690: 223b 220a 2020 2020 2020 2020 7175 6f74  ";".        quot
+000066a0: 6563 6861 7220 3d20 2227 220a 2020 2020  echar = "'".    
+000066b0: 2020 2020 6865 6164 6572 7320 3d20 5b22      headers = ["
+000066c0: 6964 222c 2022 6e61 6d65 222c 2022 6465  id", "name", "de
+000066d0: 7363 7269 7074 696f 6e22 5d0a 0a20 2020  scription"]..   
+000066e0: 2020 2020 2064 6566 2070 6172 7365 5f72       def parse_r
+000066f0: 6f77 2873 656c 662c 2072 6573 706f 6e73  ow(self, respons
+00006700: 652c 2072 6f77 293a 0a20 2020 2020 2020  e, row):.       
+00006710: 2020 2020 2073 656c 662e 6c6f 6767 6572       self.logger
+00006720: 2e69 6e66 6f28 2248 692c 2074 6869 7320  .info("Hi, this 
+00006730: 6973 2061 2072 6f77 213a 2025 7222 2c20  is a row!: %r", 
+00006740: 726f 7729 0a0a 2020 2020 2020 2020 2020  row)..          
+00006750: 2020 6974 656d 203d 2054 6573 7449 7465    item = TestIte
+00006760: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
+00006770: 6974 656d 5b22 6964 225d 203d 2072 6f77  item["id"] = row
+00006780: 5b22 6964 225d 0a20 2020 2020 2020 2020  ["id"].         
+00006790: 2020 2069 7465 6d5b 226e 616d 6522 5d20     item["name"] 
+000067a0: 3d20 726f 775b 226e 616d 6522 5d0a 2020  = row["name"].  
+000067b0: 2020 2020 2020 2020 2020 6974 656d 5b22            item["
+000067c0: 6465 7363 7269 7074 696f 6e22 5d20 3d20  description"] = 
+000067d0: 726f 775b 2264 6573 6372 6970 7469 6f6e  row["description
+000067e0: 225d 0a20 2020 2020 2020 2020 2020 2072  "].            r
+000067f0: 6574 7572 6e20 6974 656d 0a0a 0a53 6974  eturn item...Sit
+00006800: 656d 6170 5370 6964 6572 0a2d 2d2d 2d2d  emapSpider.-----
+00006810: 2d2d 2d2d 2d2d 2d2d 0a0a 2e2e 2063 6c61  --------.... cla
+00006820: 7373 3a3a 2053 6974 656d 6170 5370 6964  ss:: SitemapSpid
+00006830: 6572 0a0a 2020 2020 5369 7465 6d61 7053  er..    SitemapS
+00006840: 7069 6465 7220 616c 6c6f 7773 2079 6f75  pider allows you
+00006850: 2074 6f20 6372 6177 6c20 6120 7369 7465   to crawl a site
+00006860: 2062 7920 6469 7363 6f76 6572 696e 6720   by discovering 
+00006870: 7468 6520 5552 4c73 2075 7369 6e67 0a20  the URLs using. 
+00006880: 2020 2060 5369 7465 6d61 7073 605f 2e0a     `Sitemaps`_..
+00006890: 0a20 2020 2049 7420 7375 7070 6f72 7473  .    It supports
+000068a0: 206e 6573 7465 6420 7369 7465 6d61 7073   nested sitemaps
+000068b0: 2061 6e64 2064 6973 636f 7665 7269 6e67   and discovering
+000068c0: 2073 6974 656d 6170 2075 726c 7320 6672   sitemap urls fr
+000068d0: 6f6d 0a20 2020 2060 726f 626f 7473 2e74  om.    `robots.t
+000068e0: 7874 605f 2e0a 0a20 2020 202e 2e20 6174  xt`_...    .. at
+000068f0: 7472 6962 7574 653a 3a20 7369 7465 6d61  tribute:: sitema
+00006900: 705f 7572 6c73 0a0a 2020 2020 2020 2020  p_urls..        
+00006910: 4120 6c69 7374 206f 6620 7572 6c73 2070  A list of urls p
+00006920: 6f69 6e74 696e 6720 746f 2074 6865 2073  ointing to the s
+00006930: 6974 656d 6170 7320 7768 6f73 6520 7572  itemaps whose ur
+00006940: 6c73 2079 6f75 2077 616e 7420 746f 2063  ls you want to c
+00006950: 7261 776c 2e0a 0a20 2020 2020 2020 2059  rawl...        Y
+00006960: 6f75 2063 616e 2061 6c73 6f20 706f 696e  ou can also poin
+00006970: 7420 746f 2061 2060 726f 626f 7473 2e74  t to a `robots.t
+00006980: 7874 605f 2061 6e64 2069 7420 7769 6c6c  xt`_ and it will
+00006990: 2062 6520 7061 7273 6564 2074 6f20 6578   be parsed to ex
+000069a0: 7472 6163 740a 2020 2020 2020 2020 7369  tract.        si
+000069b0: 7465 6d61 7020 7572 6c73 2066 726f 6d20  temap urls from 
+000069c0: 6974 2e0a 0a20 2020 202e 2e20 6174 7472  it...    .. attr
+000069d0: 6962 7574 653a 3a20 7369 7465 6d61 705f  ibute:: sitemap_
+000069e0: 7275 6c65 730a 0a20 2020 2020 2020 2041  rules..        A
+000069f0: 206c 6973 7420 6f66 2074 7570 6c65 7320   list of tuples 
+00006a00: 6060 2872 6567 6578 2c20 6361 6c6c 6261  ``(regex, callba
+00006a10: 636b 2960 6020 7768 6572 653a 0a0a 2020  ck)`` where:..  
+00006a20: 2020 2020 2020 2a20 6060 7265 6765 7860        * ``regex`
+00006a30: 6020 6973 2061 2072 6567 756c 6172 2065  ` is a regular e
+00006a40: 7870 7265 7373 696f 6e20 746f 206d 6174  xpression to mat
+00006a50: 6368 2075 726c 7320 6578 7472 6163 7465  ch urls extracte
+00006a60: 6420 6672 6f6d 2073 6974 656d 6170 732e  d from sitemaps.
+00006a70: 0a20 2020 2020 2020 2020 2060 6072 6567  .          ``reg
+00006a80: 6578 6060 2063 616e 2062 6520 6569 7468  ex`` can be eith
+00006a90: 6572 2061 2073 7472 206f 7220 6120 636f  er a str or a co
+00006aa0: 6d70 696c 6564 2072 6567 6578 206f 626a  mpiled regex obj
+00006ab0: 6563 742e 0a0a 2020 2020 2020 2020 2a20  ect...        * 
+00006ac0: 6361 6c6c 6261 636b 2069 7320 7468 6520  callback is the 
+00006ad0: 6361 6c6c 6261 636b 2074 6f20 7573 6520  callback to use 
+00006ae0: 666f 7220 7072 6f63 6573 7369 6e67 2074  for processing t
+00006af0: 6865 2075 726c 7320 7468 6174 206d 6174  he urls that mat
+00006b00: 6368 0a20 2020 2020 2020 2020 2074 6865  ch.          the
+00006b10: 2072 6567 756c 6172 2065 7870 7265 7373   regular express
+00006b20: 696f 6e2e 2060 6063 616c 6c62 6163 6b60  ion. ``callback`
+00006b30: 6020 6361 6e20 6265 2061 2073 7472 696e  ` can be a strin
+00006b40: 6720 2869 6e64 6963 6174 696e 6720 7468  g (indicating th
+00006b50: 650a 2020 2020 2020 2020 2020 6e61 6d65  e.          name
+00006b60: 206f 6620 6120 7370 6964 6572 206d 6574   of a spider met
+00006b70: 686f 6429 206f 7220 6120 6361 6c6c 6162  hod) or a callab
+00006b80: 6c65 2e0a 0a20 2020 2020 2020 2046 6f72  le...        For
+00006b90: 2065 7861 6d70 6c65 3a3a 0a0a 2020 2020   example::..    
+00006ba0: 2020 2020 2020 2020 7369 7465 6d61 705f          sitemap_
+00006bb0: 7275 6c65 7320 3d20 5b28 272f 7072 6f64  rules = [('/prod
+00006bc0: 7563 742f 272c 2027 7061 7273 655f 7072  uct/', 'parse_pr
+00006bd0: 6f64 7563 7427 295d 0a0a 2020 2020 2020  oduct')]..      
+00006be0: 2020 5275 6c65 7320 6172 6520 6170 706c    Rules are appl
+00006bf0: 6965 6420 696e 206f 7264 6572 2c20 616e  ied in order, an
+00006c00: 6420 6f6e 6c79 2074 6865 2066 6972 7374  d only the first
+00006c10: 206f 6e65 2074 6861 7420 6d61 7463 6865   one that matche
+00006c20: 7320 7769 6c6c 2062 650a 2020 2020 2020  s will be.      
+00006c30: 2020 7573 6564 2e0a 0a20 2020 2020 2020    used...       
+00006c40: 2049 6620 796f 7520 6f6d 6974 2074 6869   If you omit thi
+00006c50: 7320 6174 7472 6962 7574 652c 2061 6c6c  s attribute, all
+00006c60: 2075 726c 7320 666f 756e 6420 696e 2073   urls found in s
+00006c70: 6974 656d 6170 7320 7769 6c6c 2062 650a  itemaps will be.
+00006c80: 2020 2020 2020 2020 7072 6f63 6573 7365          processe
+00006c90: 6420 7769 7468 2074 6865 2060 6070 6172  d with the ``par
+00006ca0: 7365 6060 2063 616c 6c62 6163 6b2e 0a0a  se`` callback...
+00006cb0: 2020 2020 2e2e 2061 7474 7269 6275 7465      .. attribute
+00006cc0: 3a3a 2073 6974 656d 6170 5f66 6f6c 6c6f  :: sitemap_follo
+00006cd0: 770a 0a20 2020 2020 2020 2041 206c 6973  w..        A lis
+00006ce0: 7420 6f66 2072 6567 6578 6573 206f 6620  t of regexes of 
+00006cf0: 7369 7465 6d61 7020 7468 6174 2073 686f  sitemap that sho
+00006d00: 756c 6420 6265 2066 6f6c 6c6f 7765 642e  uld be followed.
+00006d10: 2054 6869 7320 6973 206f 6e6c 790a 2020   This is only.  
+00006d20: 2020 2020 2020 666f 7220 7369 7465 7320        for sites 
+00006d30: 7468 6174 2075 7365 2060 5369 7465 6d61  that use `Sitema
+00006d40: 7020 696e 6465 7820 6669 6c65 7360 5f20  p index files`_ 
+00006d50: 7468 6174 2070 6f69 6e74 2074 6f20 6f74  that point to ot
+00006d60: 6865 7220 7369 7465 6d61 700a 2020 2020  her sitemap.    
+00006d70: 2020 2020 6669 6c65 732e 0a0a 2020 2020      files...    
+00006d80: 2020 2020 4279 2064 6566 6175 6c74 2c20      By default, 
+00006d90: 616c 6c20 7369 7465 6d61 7073 2061 7265  all sitemaps are
+00006da0: 2066 6f6c 6c6f 7765 642e 0a0a 2020 2020   followed...    
+00006db0: 2e2e 2061 7474 7269 6275 7465 3a3a 2073  .. attribute:: s
+00006dc0: 6974 656d 6170 5f61 6c74 6572 6e61 7465  itemap_alternate
+00006dd0: 5f6c 696e 6b73 0a0a 2020 2020 2020 2020  _links..        
+00006de0: 5370 6563 6966 6965 7320 6966 2061 6c74  Specifies if alt
+00006df0: 6572 6e61 7465 206c 696e 6b73 2066 6f72  ernate links for
+00006e00: 206f 6e65 2060 6075 726c 6060 2073 686f   one ``url`` sho
+00006e10: 756c 6420 6265 2066 6f6c 6c6f 7765 642e  uld be followed.
+00006e20: 2054 6865 7365 0a20 2020 2020 2020 2061   These.        a
+00006e30: 7265 206c 696e 6b73 2066 6f72 2074 6865  re links for the
+00006e40: 2073 616d 6520 7765 6273 6974 6520 696e   same website in
+00006e50: 2061 6e6f 7468 6572 206c 616e 6775 6167   another languag
+00006e60: 6520 7061 7373 6564 2077 6974 6869 6e0a  e passed within.
+00006e70: 2020 2020 2020 2020 7468 6520 7361 6d65          the same
+00006e80: 2060 6075 726c 6060 2062 6c6f 636b 2e0a   ``url`` block..
+00006e90: 0a20 2020 2020 2020 2046 6f72 2065 7861  .        For exa
+00006ea0: 6d70 6c65 3a3a 0a0a 2020 2020 2020 2020  mple::..        
+00006eb0: 2020 2020 3c75 726c 3e0a 2020 2020 2020      <url>.      
+00006ec0: 2020 2020 2020 2020 2020 3c6c 6f63 3e68            <loc>h
+00006ed0: 7474 703a 2f2f 6578 616d 706c 652e 636f  ttp://example.co
+00006ee0: 6d2f 3c2f 6c6f 633e 0a20 2020 2020 2020  m/</loc>.       
+00006ef0: 2020 2020 2020 2020 203c 7868 746d 6c3a           <xhtml:
+00006f00: 6c69 6e6b 2072 656c 3d22 616c 7465 726e  link rel="altern
+00006f10: 6174 6522 2068 7265 666c 616e 673d 2264  ate" hreflang="d
+00006f20: 6522 2068 7265 663d 2268 7474 703a 2f2f  e" href="http://
+00006f30: 6578 616d 706c 652e 636f 6d2f 6465 222f  example.com/de"/
+00006f40: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00006f50: 7572 6c3e 0a0a 2020 2020 2020 2020 5769  url>..        Wi
+00006f60: 7468 2060 6073 6974 656d 6170 5f61 6c74  th ``sitemap_alt
+00006f70: 6572 6e61 7465 5f6c 696e 6b73 6060 2073  ernate_links`` s
+00006f80: 6574 2c20 7468 6973 2077 6f75 6c64 2072  et, this would r
+00006f90: 6574 7269 6576 6520 626f 7468 2055 524c  etrieve both URL
+00006fa0: 732e 2057 6974 680a 2020 2020 2020 2020  s. With.        
+00006fb0: 6060 7369 7465 6d61 705f 616c 7465 726e  ``sitemap_altern
+00006fc0: 6174 655f 6c69 6e6b 7360 6020 6469 7361  ate_links`` disa
+00006fd0: 626c 6564 2c20 6f6e 6c79 2060 6068 7474  bled, only ``htt
+00006fe0: 703a 2f2f 6578 616d 706c 652e 636f 6d2f  p://example.com/
+00006ff0: 6060 2077 6f75 6c64 2062 650a 2020 2020  `` would be.    
+00007000: 2020 2020 7265 7472 6965 7665 642e 0a0a      retrieved...
+00007010: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
+00007020: 6973 2060 6073 6974 656d 6170 5f61 6c74  is ``sitemap_alt
+00007030: 6572 6e61 7465 5f6c 696e 6b73 6060 2064  ernate_links`` d
+00007040: 6973 6162 6c65 642e 0a0a 2020 2020 2e2e  isabled...    ..
+00007050: 206d 6574 686f 643a 3a20 7369 7465 6d61   method:: sitema
+00007060: 705f 6669 6c74 6572 2865 6e74 7269 6573  p_filter(entries
+00007070: 290a 0a20 2020 2020 2020 2054 6869 7320  )..        This 
+00007080: 6973 2061 2066 696c 7465 7220 6675 6e63  is a filter func
+00007090: 7469 6f6e 2074 6861 7420 636f 756c 6420  tion that could 
+000070a0: 6265 206f 7665 7272 6964 6465 6e20 746f  be overridden to
+000070b0: 2073 656c 6563 7420 7369 7465 6d61 7020   select sitemap 
+000070c0: 656e 7472 6965 730a 2020 2020 2020 2020  entries.        
+000070d0: 6261 7365 6420 6f6e 2074 6865 6972 2061  based on their a
+000070e0: 7474 7269 6275 7465 732e 0a0a 2020 2020  ttributes...    
+000070f0: 2020 2020 466f 7220 6578 616d 706c 653a      For example:
+00007100: 3a0a 0a20 2020 2020 2020 2020 2020 203c  :..            <
+00007110: 7572 6c3e 0a20 2020 2020 2020 2020 2020  url>.           
+00007120: 2020 2020 203c 6c6f 633e 6874 7470 3a2f       <loc>http:/
+00007130: 2f65 7861 6d70 6c65 2e63 6f6d 2f3c 2f6c  /example.com/</l
+00007140: 6f63 3e0a 2020 2020 2020 2020 2020 2020  oc>.            
+00007150: 2020 2020 3c6c 6173 746d 6f64 3e32 3030      <lastmod>200
+00007160: 352d 3031 2d30 313c 2f6c 6173 746d 6f64  5-01-01</lastmod
+00007170: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00007180: 7572 6c3e 0a0a 2020 2020 2020 2020 5765  url>..        We
+00007190: 2063 616e 2064 6566 696e 6520 6120 6060   can define a ``
+000071a0: 7369 7465 6d61 705f 6669 6c74 6572 6060  sitemap_filter``
+000071b0: 2066 756e 6374 696f 6e20 746f 2066 696c   function to fil
+000071c0: 7465 7220 6060 656e 7472 6965 7360 6020  ter ``entries`` 
+000071d0: 6279 2064 6174 653a 0a0a 2020 2020 2020  by date:..      
+000071e0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+000071f0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00007200: 2020 2020 2020 6672 6f6d 2064 6174 6574        from datet
+00007210: 696d 6520 696d 706f 7274 2064 6174 6574  ime import datet
+00007220: 696d 650a 2020 2020 2020 2020 2020 2020  ime.            
+00007230: 6672 6f6d 2073 6372 6170 792e 7370 6964  from scrapy.spid
+00007240: 6572 7320 696d 706f 7274 2053 6974 656d  ers import Sitem
+00007250: 6170 5370 6964 6572 0a0a 0a20 2020 2020  apSpider...     
+00007260: 2020 2020 2020 2063 6c61 7373 2046 696c         class Fil
+00007270: 7465 7265 6453 6974 656d 6170 5370 6964  teredSitemapSpid
+00007280: 6572 2853 6974 656d 6170 5370 6964 6572  er(SitemapSpider
+00007290: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000072a0: 2020 206e 616d 6520 3d20 2266 696c 7465     name = "filte
+000072b0: 7265 645f 7369 7465 6d61 705f 7370 6964  red_sitemap_spid
+000072c0: 6572 220a 2020 2020 2020 2020 2020 2020  er".            
+000072d0: 2020 2020 616c 6c6f 7765 645f 646f 6d61      allowed_doma
+000072e0: 696e 7320 3d20 5b22 6578 616d 706c 652e  ins = ["example.
+000072f0: 636f 6d22 5d0a 2020 2020 2020 2020 2020  com"].          
+00007300: 2020 2020 2020 7369 7465 6d61 705f 7572        sitemap_ur
+00007310: 6c73 203d 205b 2268 7474 703a 2f2f 6578  ls = ["http://ex
+00007320: 616d 706c 652e 636f 6d2f 7369 7465 6d61  ample.com/sitema
+00007330: 702e 786d 6c22 5d0a 0a20 2020 2020 2020  p.xml"]..       
+00007340: 2020 2020 2020 2020 2064 6566 2073 6974           def sit
+00007350: 656d 6170 5f66 696c 7465 7228 7365 6c66  emap_filter(self
+00007360: 2c20 656e 7472 6965 7329 3a0a 2020 2020  , entries):.    
+00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007380: 666f 7220 656e 7472 7920 696e 2065 6e74  for entry in ent
+00007390: 7269 6573 3a0a 2020 2020 2020 2020 2020  ries:.          
+000073a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000073b0: 7465 5f74 696d 6520 3d20 6461 7465 7469  te_time = dateti
+000073c0: 6d65 2e73 7472 7074 696d 6528 656e 7472  me.strptime(entr
+000073d0: 795b 226c 6173 746d 6f64 225d 2c20 2225  y["lastmod"], "%
+000073e0: 592d 256d 2d25 6422 290a 2020 2020 2020  Y-%m-%d").      
+000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007400: 2020 6966 2064 6174 655f 7469 6d65 2e79    if date_time.y
+00007410: 6561 7220 3e3d 2032 3030 353a 0a20 2020  ear >= 2005:.   
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 2020 2079 6965 6c64 2065           yield e
+00007440: 6e74 7279 0a0a 2020 2020 2020 2020 5468  ntry..        Th
+00007450: 6973 2077 6f75 6c64 2072 6574 7269 6576  is would retriev
+00007460: 6520 6f6e 6c79 2060 6065 6e74 7269 6573  e only ``entries
+00007470: 6060 206d 6f64 6966 6965 6420 6f6e 2032  `` modified on 2
+00007480: 3030 3520 616e 6420 7468 6520 666f 6c6c  005 and the foll
+00007490: 6f77 696e 670a 2020 2020 2020 2020 7965  owing.        ye
+000074a0: 6172 732e 0a0a 2020 2020 2020 2020 456e  ars...        En
+000074b0: 7472 6965 7320 6172 6520 6469 6374 206f  tries are dict o
+000074c0: 626a 6563 7473 2065 7874 7261 6374 6564  bjects extracted
+000074d0: 2066 726f 6d20 7468 6520 7369 7465 6d61   from the sitema
+000074e0: 7020 646f 6375 6d65 6e74 2e0a 2020 2020  p document..    
+000074f0: 2020 2020 5573 7561 6c6c 792c 2074 6865      Usually, the
+00007500: 206b 6579 2069 7320 7468 6520 7461 6720   key is the tag 
+00007510: 6e61 6d65 2061 6e64 2074 6865 2076 616c  name and the val
+00007520: 7565 2069 7320 7468 6520 7465 7874 2069  ue is the text i
+00007530: 6e73 6964 6520 6974 2e0a 0a20 2020 2020  nside it...     
+00007540: 2020 2049 7427 7320 696d 706f 7274 616e     It's importan
+00007550: 7420 746f 206e 6f74 6963 6520 7468 6174  t to notice that
+00007560: 3a0a 0a20 2020 2020 2020 202d 2061 7320  :..        - as 
+00007570: 7468 6520 6c6f 6320 6174 7472 6962 7574  the loc attribut
+00007580: 6520 6973 2072 6571 7569 7265 642c 2065  e is required, e
+00007590: 6e74 7269 6573 2077 6974 686f 7574 2074  ntries without t
+000075a0: 6869 7320 7461 6720 6172 6520 6469 7363  his tag are disc
+000075b0: 6172 6465 640a 2020 2020 2020 2020 2d20  arded.        - 
+000075c0: 616c 7465 726e 6174 6520 6c69 6e6b 7320  alternate links 
+000075d0: 6172 6520 7374 6f72 6564 2069 6e20 6120  are stored in a 
+000075e0: 6c69 7374 2077 6974 6820 7468 6520 6b65  list with the ke
+000075f0: 7920 6060 616c 7465 726e 6174 6560 600a  y ``alternate``.
+00007600: 2020 2020 2020 2020 2020 2873 6565 2060            (see `
+00007610: 6073 6974 656d 6170 5f61 6c74 6572 6e61  `sitemap_alterna
+00007620: 7465 5f6c 696e 6b73 6060 290a 2020 2020  te_links``).    
+00007630: 2020 2020 2d20 6e61 6d65 7370 6163 6573      - namespaces
+00007640: 2061 7265 2072 656d 6f76 6564 2c20 736f   are removed, so
+00007650: 206c 786d 6c20 7461 6773 206e 616d 6564   lxml tags named
+00007660: 2061 7320 6060 7b6e 616d 6573 7061 6365   as ``{namespace
+00007670: 7d74 6167 6e61 6d65 6060 2062 6563 6f6d  }tagname`` becom
+00007680: 6520 6f6e 6c79 2060 6074 6167 6e61 6d65  e only ``tagname
+00007690: 6060 0a0a 2020 2020 2020 2020 4966 2079  ``..        If y
+000076a0: 6f75 206f 6d69 7420 7468 6973 206d 6574  ou omit this met
+000076b0: 686f 642c 2061 6c6c 2065 6e74 7269 6573  hod, all entries
+000076c0: 2066 6f75 6e64 2069 6e20 7369 7465 6d61   found in sitema
+000076d0: 7073 2077 696c 6c20 6265 0a20 2020 2020  ps will be.     
+000076e0: 2020 2070 726f 6365 7373 6564 2c20 6f62     processed, ob
+000076f0: 7365 7276 696e 6720 6f74 6865 7220 6174  serving other at
+00007700: 7472 6962 7574 6573 2061 6e64 2074 6865  tributes and the
+00007710: 6972 2073 6574 7469 6e67 732e 0a0a 0a53  ir settings....S
+00007720: 6974 656d 6170 5370 6964 6572 2065 7861  itemapSpider exa
+00007730: 6d70 6c65 730a 7e7e 7e7e 7e7e 7e7e 7e7e  mples.~~~~~~~~~~
+00007740: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 5369  ~~~~~~~~~~~~..Si
+00007750: 6d70 6c65 7374 2065 7861 6d70 6c65 3a20  mplest example: 
+00007760: 7072 6f63 6573 7320 616c 6c20 7572 6c73  process all urls
+00007770: 2064 6973 636f 7665 7265 6420 7468 726f   discovered thro
+00007780: 7567 6820 7369 7465 6d61 7073 2075 7369  ugh sitemaps usi
+00007790: 6e67 2074 6865 0a60 6070 6172 7365 6060  ng the.``parse``
+000077a0: 2063 616c 6c62 6163 6b3a 0a0a 2e2e 2063   callback:.... c
+000077b0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
+000077c0: 6f6e 0a0a 2020 2020 6672 6f6d 2073 6372  on..    from scr
+000077d0: 6170 792e 7370 6964 6572 7320 696d 706f  apy.spiders impo
+000077e0: 7274 2053 6974 656d 6170 5370 6964 6572  rt SitemapSpider
+000077f0: 0a0a 0a20 2020 2063 6c61 7373 204d 7953  ...    class MyS
+00007800: 7069 6465 7228 5369 7465 6d61 7053 7069  pider(SitemapSpi
+00007810: 6465 7229 3a0a 2020 2020 2020 2020 7369  der):.        si
+00007820: 7465 6d61 705f 7572 6c73 203d 205b 2268  temap_urls = ["h
+00007830: 7474 703a 2f2f 7777 772e 6578 616d 706c  ttp://www.exampl
+00007840: 652e 636f 6d2f 7369 7465 6d61 702e 786d  e.com/sitemap.xm
+00007850: 6c22 5d0a 0a20 2020 2020 2020 2064 6566  l"]..        def
+00007860: 2070 6172 7365 2873 656c 662c 2072 6573   parse(self, res
+00007870: 706f 6e73 6529 3a0a 2020 2020 2020 2020  ponse):.        
+00007880: 2020 2020 7061 7373 2020 2320 2e2e 2e20      pass  # ... 
+00007890: 7363 7261 7065 2069 7465 6d20 6865 7265  scrape item here
+000078a0: 202e 2e2e 0a0a 5072 6f63 6573 7320 736f   .....Process so
+000078b0: 6d65 2075 726c 7320 7769 7468 2063 6572  me urls with cer
+000078c0: 7461 696e 2063 616c 6c62 6163 6b20 616e  tain callback an
+000078d0: 6420 6f74 6865 7220 7572 6c73 2077 6974  d other urls wit
+000078e0: 6820 6120 6469 6666 6572 656e 740a 6361  h a different.ca
+000078f0: 6c6c 6261 636b 3a0a 0a2e 2e20 636f 6465  llback:.... code
+00007900: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00007910: 0a20 2020 2066 726f 6d20 7363 7261 7079  .    from scrapy
+00007920: 2e73 7069 6465 7273 2069 6d70 6f72 7420  .spiders import 
+00007930: 5369 7465 6d61 7053 7069 6465 720a 0a0a  SitemapSpider...
+00007940: 2020 2020 636c 6173 7320 4d79 5370 6964      class MySpid
+00007950: 6572 2853 6974 656d 6170 5370 6964 6572  er(SitemapSpider
+00007960: 293a 0a20 2020 2020 2020 2073 6974 656d  ):.        sitem
+00007970: 6170 5f75 726c 7320 3d20 5b22 6874 7470  ap_urls = ["http
+00007980: 3a2f 2f77 7777 2e65 7861 6d70 6c65 2e63  ://www.example.c
+00007990: 6f6d 2f73 6974 656d 6170 2e78 6d6c 225d  om/sitemap.xml"]
+000079a0: 0a20 2020 2020 2020 2073 6974 656d 6170  .        sitemap
+000079b0: 5f72 756c 6573 203d 205b 0a20 2020 2020  _rules = [.     
+000079c0: 2020 2020 2020 2028 222f 7072 6f64 7563         ("/produc
+000079d0: 742f 222c 2022 7061 7273 655f 7072 6f64  t/", "parse_prod
+000079e0: 7563 7422 292c 0a20 2020 2020 2020 2020  uct"),.         
+000079f0: 2020 2028 222f 6361 7465 676f 7279 2f22     ("/category/"
+00007a00: 2c20 2270 6172 7365 5f63 6174 6567 6f72  , "parse_categor
+00007a10: 7922 292c 0a20 2020 2020 2020 205d 0a0a  y"),.        ]..
+00007a20: 2020 2020 2020 2020 6465 6620 7061 7273          def pars
+00007a30: 655f 7072 6f64 7563 7428 7365 6c66 2c20  e_product(self, 
+00007a40: 7265 7370 6f6e 7365 293a 0a20 2020 2020  response):.     
+00007a50: 2020 2020 2020 2070 6173 7320 2023 202e         pass  # .
+00007a60: 2e2e 2073 6372 6170 6520 7072 6f64 7563  .. scrape produc
+00007a70: 7420 2e2e 2e0a 0a20 2020 2020 2020 2064  t .....        d
+00007a80: 6566 2070 6172 7365 5f63 6174 6567 6f72  ef parse_categor
+00007a90: 7928 7365 6c66 2c20 7265 7370 6f6e 7365  y(self, response
+00007aa0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
+00007ab0: 6173 7320 2023 202e 2e2e 2073 6372 6170  ass  # ... scrap
+00007ac0: 6520 6361 7465 676f 7279 202e 2e2e 0a0a  e category .....
+00007ad0: 466f 6c6c 6f77 2073 6974 656d 6170 7320  Follow sitemaps 
+00007ae0: 6465 6669 6e65 6420 696e 2074 6865 2060  defined in the `
+00007af0: 726f 626f 7473 2e74 7874 605f 2066 696c  robots.txt`_ fil
+00007b00: 6520 616e 6420 6f6e 6c79 2066 6f6c 6c6f  e and only follo
+00007b10: 7720 7369 7465 6d61 7073 0a77 686f 7365  w sitemaps.whose
+00007b20: 2075 726c 2063 6f6e 7461 696e 7320 6060   url contains ``
+00007b30: 2f73 6974 656d 6170 5f73 686f 7060 603a  /sitemap_shop``:
+00007b40: 0a0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+00007b50: 3a20 7079 7468 6f6e 0a0a 2020 2020 6672  : python..    fr
+00007b60: 6f6d 2073 6372 6170 792e 7370 6964 6572  om scrapy.spider
+00007b70: 7320 696d 706f 7274 2053 6974 656d 6170  s import Sitemap
+00007b80: 5370 6964 6572 0a0a 0a20 2020 2063 6c61  Spider...    cla
+00007b90: 7373 204d 7953 7069 6465 7228 5369 7465  ss MySpider(Site
+00007ba0: 6d61 7053 7069 6465 7229 3a0a 2020 2020  mapSpider):.    
+00007bb0: 2020 2020 7369 7465 6d61 705f 7572 6c73      sitemap_urls
+00007bc0: 203d 205b 2268 7474 703a 2f2f 7777 772e   = ["http://www.
+00007bd0: 6578 616d 706c 652e 636f 6d2f 726f 626f  example.com/robo
+00007be0: 7473 2e74 7874 225d 0a20 2020 2020 2020  ts.txt"].       
+00007bf0: 2073 6974 656d 6170 5f72 756c 6573 203d   sitemap_rules =
+00007c00: 205b 0a20 2020 2020 2020 2020 2020 2028   [.            (
+00007c10: 222f 7368 6f70 2f22 2c20 2270 6172 7365  "/shop/", "parse
+00007c20: 5f73 686f 7022 292c 0a20 2020 2020 2020  _shop"),.       
+00007c30: 205d 0a20 2020 2020 2020 2073 6974 656d   ].        sitem
+00007c40: 6170 5f66 6f6c 6c6f 7720 3d20 5b22 2f73  ap_follow = ["/s
+00007c50: 6974 656d 6170 5f73 686f 7073 225d 0a0a  itemap_shops"]..
+00007c60: 2020 2020 2020 2020 6465 6620 7061 7273          def pars
+00007c70: 655f 7368 6f70 2873 656c 662c 2072 6573  e_shop(self, res
+00007c80: 706f 6e73 6529 3a0a 2020 2020 2020 2020  ponse):.        
+00007c90: 2020 2020 7061 7373 2020 2320 2e2e 2e20      pass  # ... 
+00007ca0: 7363 7261 7065 2073 686f 7020 6865 7265  scrape shop here
+00007cb0: 202e 2e2e 0a0a 436f 6d62 696e 6520 5369   .....Combine Si
+00007cc0: 7465 6d61 7053 7069 6465 7220 7769 7468  temapSpider with
+00007cd0: 206f 7468 6572 2073 6f75 7263 6573 206f   other sources o
+00007ce0: 6620 7572 6c73 3a0a 0a2e 2e20 636f 6465  f urls:.... code
+00007cf0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00007d00: 0a20 2020 2066 726f 6d20 7363 7261 7079  .    from scrapy
+00007d10: 2e73 7069 6465 7273 2069 6d70 6f72 7420  .spiders import 
+00007d20: 5369 7465 6d61 7053 7069 6465 720a 0a0a  SitemapSpider...
+00007d30: 2020 2020 636c 6173 7320 4d79 5370 6964      class MySpid
+00007d40: 6572 2853 6974 656d 6170 5370 6964 6572  er(SitemapSpider
+00007d50: 293a 0a20 2020 2020 2020 2073 6974 656d  ):.        sitem
+00007d60: 6170 5f75 726c 7320 3d20 5b22 6874 7470  ap_urls = ["http
+00007d70: 3a2f 2f77 7777 2e65 7861 6d70 6c65 2e63  ://www.example.c
+00007d80: 6f6d 2f72 6f62 6f74 732e 7478 7422 5d0a  om/robots.txt"].
+00007d90: 2020 2020 2020 2020 7369 7465 6d61 705f          sitemap_
+00007da0: 7275 6c65 7320 3d20 5b0a 2020 2020 2020  rules = [.      
+00007db0: 2020 2020 2020 2822 2f73 686f 702f 222c        ("/shop/",
+00007dc0: 2022 7061 7273 655f 7368 6f70 2229 2c0a   "parse_shop"),.
+00007dd0: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
+00007de0: 2020 206f 7468 6572 5f75 726c 7320 3d20     other_urls = 
+00007df0: 5b22 6874 7470 3a2f 2f77 7777 2e65 7861  ["http://www.exa
+00007e00: 6d70 6c65 2e63 6f6d 2f61 626f 7574 225d  mple.com/about"]
+00007e10: 0a0a 2020 2020 2020 2020 6465 6620 7374  ..        def st
+00007e20: 6172 745f 7265 7175 6573 7473 2873 656c  art_requests(sel
+00007e30: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+00007e40: 7265 7175 6573 7473 203d 206c 6973 7428  requests = list(
+00007e50: 7375 7065 7228 4d79 5370 6964 6572 2c20  super(MySpider, 
+00007e60: 7365 6c66 292e 7374 6172 745f 7265 7175  self).start_requ
+00007e70: 6573 7473 2829 290a 2020 2020 2020 2020  ests()).        
+00007e80: 2020 2020 7265 7175 6573 7473 202b 3d20      requests += 
+00007e90: 5b73 6372 6170 792e 5265 7175 6573 7428  [scrapy.Request(
+00007ea0: 782c 2073 656c 662e 7061 7273 655f 6f74  x, self.parse_ot
+00007eb0: 6865 7229 2066 6f72 2078 2069 6e20 7365  her) for x in se
+00007ec0: 6c66 2e6f 7468 6572 5f75 726c 735d 0a20  lf.other_urls]. 
+00007ed0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007ee0: 6e20 7265 7175 6573 7473 0a0a 2020 2020  n requests..    
+00007ef0: 2020 2020 6465 6620 7061 7273 655f 7368      def parse_sh
+00007f00: 6f70 2873 656c 662c 2072 6573 706f 6e73  op(self, respons
+00007f10: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00007f20: 7061 7373 2020 2320 2e2e 2e20 7363 7261  pass  # ... scra
+00007f30: 7065 2073 686f 7020 6865 7265 202e 2e2e  pe shop here ...
+00007f40: 0a0a 2020 2020 2020 2020 6465 6620 7061  ..        def pa
+00007f50: 7273 655f 6f74 6865 7228 7365 6c66 2c20  rse_other(self, 
+00007f60: 7265 7370 6f6e 7365 293a 0a20 2020 2020  response):.     
+00007f70: 2020 2020 2020 2070 6173 7320 2023 202e         pass  # .
+00007f80: 2e2e 2073 6372 6170 6520 6f74 6865 7220  .. scrape other 
+00007f90: 6865 7265 202e 2e2e 0a0a 2e2e 205f 5369  here ....... _Si
+00007fa0: 7465 6d61 7073 3a20 6874 7470 733a 2f2f  temaps: https://
+00007fb0: 7777 772e 7369 7465 6d61 7073 2e6f 7267  www.sitemaps.org
+00007fc0: 2f69 6e64 6578 2e68 746d 6c0a 2e2e 205f  /index.html... _
+00007fd0: 5369 7465 6d61 7020 696e 6465 7820 6669  Sitemap index fi
+00007fe0: 6c65 733a 2068 7474 7073 3a2f 2f77 7777  les: https://www
+00007ff0: 2e73 6974 656d 6170 732e 6f72 672f 7072  .sitemaps.org/pr
+00008000: 6f74 6f63 6f6c 2e68 746d 6c23 696e 6465  otocol.html#inde
+00008010: 780a 2e2e 205f 726f 626f 7473 2e74 7874  x... _robots.txt
+00008020: 3a20 6874 7470 733a 2f2f 7777 772e 726f  : https://www.ro
+00008030: 626f 7473 7478 742e 6f72 672f 0a2e 2e20  botstxt.org/... 
+00008040: 5f54 4c44 3a20 6874 7470 733a 2f2f 656e  _TLD: https://en
+00008050: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00008060: 696b 692f 546f 702d 6c65 7665 6c5f 646f  iki/Top-level_do
+00008070: 6d61 696e 0a2e 2e20 5f53 6372 6170 7964  main... _Scrapyd
+00008080: 2064 6f63 756d 656e 7461 7469 6f6e 3a20   documentation: 
+00008090: 6874 7470 733a 2f2f 7363 7261 7079 642e  https://scrapyd.
+000080a0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000080b0: 6e2f 6c61 7465 7374 2f0a                 n/latest/.
```

### Comparing `Scrapy-2.8.0/docs/topics/settings.rst` & `Scrapy-2.9.0/docs/topics/settings.rst`

 * *Files 6% similar despite different names*

```diff
@@ -63,21 +63,26 @@
     scrapy crawl myspider -s LOG_FILE=scrapy.log
 
 2. Settings per-spider
 ----------------------
 
 Spiders (See the :ref:`topics-spiders` chapter for reference) can define their
 own settings that will take precedence and override the project ones. They can
-do so by setting their :attr:`~scrapy.Spider.custom_settings` attribute::
+do so by setting their :attr:`~scrapy.Spider.custom_settings` attribute:
+
+.. code-block:: python
+
+    import scrapy
+
 
     class MySpider(scrapy.Spider):
-        name = 'myspider'
+        name = "myspider"
 
         custom_settings = {
-            'SOME_SETTING': 'some value',
+            "SOME_SETTING": "some value",
         }
 
 3. Project settings module
 --------------------------
 
 The project settings module is the standard configuration file for your Scrapy
 project, it's where most of your custom settings will be populated. For a
@@ -111,60 +116,68 @@
 When a setting references a callable object to be imported by Scrapy, such as a
 class or a function, there are two different ways you can specify that object:
 
 -   As a string containing the import path of that object
 
 -   As the object itself
 
-For example::
+For example:
+
+.. skip: next
+.. code-block:: python
 
    from mybot.pipelines.validate import ValidateMyItem
+
    ITEM_PIPELINES = {
        # passing the classname...
        ValidateMyItem: 300,
        # ...equals passing the class path
-       'mybot.pipelines.validate.ValidateMyItem': 300,
+       "mybot.pipelines.validate.ValidateMyItem": 300,
    }
 
 .. note:: Passing non-callable objects is not supported.
 
 
 How to access settings
 ======================
 
 .. highlight:: python
 
-In a spider, the settings are available through ``self.settings``::
+In a spider, the settings are available through ``self.settings``:
+
+.. code-block:: python
 
     class MySpider(scrapy.Spider):
-        name = 'myspider'
-        start_urls = ['http://example.com']
+        name = "myspider"
+        start_urls = ["http://example.com"]
 
         def parse(self, response):
             print(f"Existing settings: {self.settings.attributes.keys()}")
 
 .. note::
     The ``settings`` attribute is set in the base Spider class after the spider
     is initialized.  If you want to use the settings before the initialization
     (e.g., in your spider's ``__init__()`` method), you'll need to override the
     :meth:`~scrapy.Spider.from_crawler` method.
 
 Settings can be accessed through the :attr:`scrapy.crawler.Crawler.settings`
 attribute of the Crawler that is passed to ``from_crawler`` method in
-extensions, middlewares and item pipelines::
+extensions, middlewares and item pipelines:
+
+.. code-block:: python
 
     class MyExtension:
         def __init__(self, log_is_enabled=False):
             if log_is_enabled:
                 print("log is enabled!")
 
         @classmethod
         def from_crawler(cls, crawler):
             settings = crawler.settings
-            return cls(settings.getbool('LOG_ENABLED'))
+            return cls(settings.getbool("LOG_ENABLED"))
 
 The settings object can be used like a dict (e.g.,
 ``settings['LOG_ENABLED']``), but it's usually preferred to extract the setting
 in the format you need it to avoid type errors, using one of the methods
 provided by the :class:`~scrapy.settings.Settings` API.
 
 Rationale for setting names
@@ -361,19 +374,21 @@
 Scrapy shell <topics-shell>`.
 
 .. setting:: DEFAULT_REQUEST_HEADERS
 
 DEFAULT_REQUEST_HEADERS
 -----------------------
 
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
-        'Accept-Language': 'en',
+        "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
+        "Accept-Language": "en",
     }
 
 The default headers used for Scrapy HTTP Requests. They're populated in the
 :class:`~scrapy.downloadermiddlewares.defaultheaders.DefaultHeadersMiddleware`.
 
 .. caution:: Cookies set via the ``Cookie`` header are not considered by the
     :ref:`cookies-mw`. If you need to set cookies for a request, use the
@@ -400,17 +415,20 @@
 Default: ``0``
 
 Scope: ``scrapy.spidermiddlewares.depth.DepthMiddleware``
 
 An integer that is used to adjust the :attr:`~scrapy.Request.priority` of
 a :class:`~scrapy.Request` based on its depth.
 
-The priority of a request is adjusted as follows::
+The priority of a request is adjusted as follows:
+
+.. skip: next
+.. code-block:: python
 
-    request.priority = request.priority - ( depth * DEPTH_PRIORITY )
+    request.priority = request.priority - (depth * DEPTH_PRIORITY)
 
 As depth increases, positive values of ``DEPTH_PRIORITY`` decrease request
 priority (BFO), while negative values increase request priority (DFO). See
 also :ref:`faq-bfo-dfo`.
 
 .. note::
 
@@ -591,31 +609,33 @@
 orders. For more info see :ref:`topics-downloader-middleware-setting`.
 
 .. setting:: DOWNLOADER_MIDDLEWARES_BASE
 
 DOWNLOADER_MIDDLEWARES_BASE
 ---------------------------
 
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        'scrapy.downloadermiddlewares.robotstxt.RobotsTxtMiddleware': 100,
-        'scrapy.downloadermiddlewares.httpauth.HttpAuthMiddleware': 300,
-        'scrapy.downloadermiddlewares.downloadtimeout.DownloadTimeoutMiddleware': 350,
-        'scrapy.downloadermiddlewares.defaultheaders.DefaultHeadersMiddleware': 400,
-        'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware': 500,
-        'scrapy.downloadermiddlewares.retry.RetryMiddleware': 550,
-        'scrapy.downloadermiddlewares.ajaxcrawl.AjaxCrawlMiddleware': 560,
-        'scrapy.downloadermiddlewares.redirect.MetaRefreshMiddleware': 580,
-        'scrapy.downloadermiddlewares.httpcompression.HttpCompressionMiddleware': 590,
-        'scrapy.downloadermiddlewares.redirect.RedirectMiddleware': 600,
-        'scrapy.downloadermiddlewares.cookies.CookiesMiddleware': 700,
-        'scrapy.downloadermiddlewares.httpproxy.HttpProxyMiddleware': 750,
-        'scrapy.downloadermiddlewares.stats.DownloaderStats': 850,
-        'scrapy.downloadermiddlewares.httpcache.HttpCacheMiddleware': 900,
+        "scrapy.downloadermiddlewares.robotstxt.RobotsTxtMiddleware": 100,
+        "scrapy.downloadermiddlewares.httpauth.HttpAuthMiddleware": 300,
+        "scrapy.downloadermiddlewares.downloadtimeout.DownloadTimeoutMiddleware": 350,
+        "scrapy.downloadermiddlewares.defaultheaders.DefaultHeadersMiddleware": 400,
+        "scrapy.downloadermiddlewares.useragent.UserAgentMiddleware": 500,
+        "scrapy.downloadermiddlewares.retry.RetryMiddleware": 550,
+        "scrapy.downloadermiddlewares.ajaxcrawl.AjaxCrawlMiddleware": 560,
+        "scrapy.downloadermiddlewares.redirect.MetaRefreshMiddleware": 580,
+        "scrapy.downloadermiddlewares.httpcompression.HttpCompressionMiddleware": 590,
+        "scrapy.downloadermiddlewares.redirect.RedirectMiddleware": 600,
+        "scrapy.downloadermiddlewares.cookies.CookiesMiddleware": 700,
+        "scrapy.downloadermiddlewares.httpproxy.HttpProxyMiddleware": 750,
+        "scrapy.downloadermiddlewares.stats.DownloaderStats": 850,
+        "scrapy.downloadermiddlewares.httpcache.HttpCacheMiddleware": 900,
     }
 
 A dict containing the downloader middlewares enabled by default in Scrapy. Low
 orders are closer to the engine, high orders are closer to the downloader. You
 should never modify this setting in your project, modify
 :setting:`DOWNLOADER_MIDDLEWARES` instead.  For more info see
 :ref:`topics-downloader-middleware-setting`.
@@ -683,49 +703,55 @@
 See :setting:`DOWNLOAD_HANDLERS_BASE` for example format.
 
 .. setting:: DOWNLOAD_HANDLERS_BASE
 
 DOWNLOAD_HANDLERS_BASE
 ----------------------
 
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        'data': 'scrapy.core.downloader.handlers.datauri.DataURIDownloadHandler',
-        'file': 'scrapy.core.downloader.handlers.file.FileDownloadHandler',
-        'http': 'scrapy.core.downloader.handlers.http.HTTPDownloadHandler',
-        'https': 'scrapy.core.downloader.handlers.http.HTTPDownloadHandler',
-        's3': 'scrapy.core.downloader.handlers.s3.S3DownloadHandler',
-        'ftp': 'scrapy.core.downloader.handlers.ftp.FTPDownloadHandler',
+        "data": "scrapy.core.downloader.handlers.datauri.DataURIDownloadHandler",
+        "file": "scrapy.core.downloader.handlers.file.FileDownloadHandler",
+        "http": "scrapy.core.downloader.handlers.http.HTTPDownloadHandler",
+        "https": "scrapy.core.downloader.handlers.http.HTTPDownloadHandler",
+        "s3": "scrapy.core.downloader.handlers.s3.S3DownloadHandler",
+        "ftp": "scrapy.core.downloader.handlers.ftp.FTPDownloadHandler",
     }
 
 
 A dict containing the request download handlers enabled by default in Scrapy.
 You should never modify this setting in your project, modify
 :setting:`DOWNLOAD_HANDLERS` instead.
 
 You can disable any of these download handlers by assigning ``None`` to their
 URI scheme in :setting:`DOWNLOAD_HANDLERS`. E.g., to disable the built-in FTP
-handler (without replacement), place this in your ``settings.py``::
+handler (without replacement), place this in your ``settings.py``:
+
+.. code-block:: python
 
     DOWNLOAD_HANDLERS = {
-        'ftp': None,
+        "ftp": None,
     }
 
 .. _http2:
 
 The default HTTPS handler uses HTTP/1.1. To use HTTP/2:
 
 #.  Install ``Twisted[http2]>=17.9.0`` to install the packages required to
     enable HTTP/2 support in Twisted.
 
-#.  Update :setting:`DOWNLOAD_HANDLERS` as follows::
+#.  Update :setting:`DOWNLOAD_HANDLERS` as follows:
+
+    .. code-block:: python
 
         DOWNLOAD_HANDLERS = {
-            'https': 'scrapy.core.downloader.handlers.http2.H2DownloadHandler',
+            "https": "scrapy.core.downloader.handlers.http2.H2DownloadHandler",
         }
 
 .. warning::
 
     HTTP/2 support in Scrapy is experimental, and not yet recommended for
     production environments. Future Scrapy versions may introduce related
     changes without a deprecation period or warning.
@@ -746,14 +772,39 @@
     -   No support for the :signal:`bytes_received` and
         :signal:`headers_received` signals.
 
 .. _frame size: https://tools.ietf.org/html/rfc7540#section-4.2
 .. _http2 faq: https://http2.github.io/faq/#does-http2-require-encryption
 .. _server pushes: https://tools.ietf.org/html/rfc7540#section-8.2
 
+.. setting:: DOWNLOAD_SLOTS
+
+DOWNLOAD_SLOTS
+----------------
+
+Default: ``{}``
+
+Allows to define concurrency/delay parameters on per slot (domain) basis:
+
+    .. code-block:: python
+
+        DOWNLOAD_SLOTS = {
+            "quotes.toscrape.com": {"concurrency": 1, "delay": 2, "randomize_delay": False},
+            "books.toscrape.com": {"delay": 3, "randomize_delay": False},
+        }
+
+.. note::
+
+    For other downloader slots default settings values will be used:
+
+    -   :setting:`DOWNLOAD_DELAY`: ``delay``
+    -   :setting:`CONCURRENT_REQUESTS_PER_DOMAIN`: ``concurrency``
+    -   :setting:`RANDOMIZE_DOWNLOAD_DELAY`: ``randomize_delay``
+
+
 .. setting:: DOWNLOAD_TIMEOUT
 
 DOWNLOAD_TIMEOUT
 ----------------
 
 Default: ``180``
 
@@ -886,26 +937,28 @@
 A dict containing the extensions enabled in your project, and their orders.
 
 .. setting:: EXTENSIONS_BASE
 
 EXTENSIONS_BASE
 ---------------
 
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        'scrapy.extensions.corestats.CoreStats': 0,
-        'scrapy.extensions.telnet.TelnetConsole': 0,
-        'scrapy.extensions.memusage.MemoryUsage': 0,
-        'scrapy.extensions.memdebug.MemoryDebugger': 0,
-        'scrapy.extensions.closespider.CloseSpider': 0,
-        'scrapy.extensions.feedexport.FeedExporter': 0,
-        'scrapy.extensions.logstats.LogStats': 0,
-        'scrapy.extensions.spiderstate.SpiderState': 0,
-        'scrapy.extensions.throttle.AutoThrottle': 0,
+        "scrapy.extensions.corestats.CoreStats": 0,
+        "scrapy.extensions.telnet.TelnetConsole": 0,
+        "scrapy.extensions.memusage.MemoryUsage": 0,
+        "scrapy.extensions.memdebug.MemoryDebugger": 0,
+        "scrapy.extensions.closespider.CloseSpider": 0,
+        "scrapy.extensions.feedexport.FeedExporter": 0,
+        "scrapy.extensions.logstats.LogStats": 0,
+        "scrapy.extensions.spiderstate.SpiderState": 0,
+        "scrapy.extensions.throttle.AutoThrottle": 0,
     }
 
 A dict containing the extensions available by default in Scrapy, and their
 orders. This setting contains all stable built-in extensions. Keep in mind that
 some of them need to be enabled through a setting.
 
 For more information See the :ref:`extensions user guide  <topics-extensions>`
@@ -984,19 +1037,21 @@
 
 Default: ``{}``
 
 A dict containing the item pipelines to use, and their orders. Order values are
 arbitrary, but it is customary to define them in the 0-1000 range. Lower orders
 process before higher orders.
 
-Example::
+Example:
+
+.. code-block:: python
 
    ITEM_PIPELINES = {
-       'mybot.pipelines.validate.ValidateMyItem': 300,
-       'mybot.pipelines.validate.StoreMyItem': 800,
+       "mybot.pipelines.validate.ValidateMyItem": 300,
+       "mybot.pipelines.validate.StoreMyItem": 800,
    }
 
 .. setting:: ITEM_PIPELINES_BASE
 
 ITEM_PIPELINES_BASE
 -------------------
 
@@ -1056,15 +1111,15 @@
 
 LOG_FORMAT
 ----------
 
 Default: ``'%(asctime)s [%(name)s] %(levelname)s: %(message)s'``
 
 String for formatting log messages. Refer to the
-:ref:`Python logging documentation <logrecord-attributes>` for the qwhole
+:ref:`Python logging documentation <logrecord-attributes>` for the whole
 list of available placeholders.
 
 .. setting:: LOG_DATEFORMAT
 
 LOG_DATEFORMAT
 --------------
 
@@ -1413,32 +1468,36 @@
 testing spiders. For more info see :ref:`topics-contracts`.
 
 .. setting:: SPIDER_CONTRACTS_BASE
 
 SPIDER_CONTRACTS_BASE
 ---------------------
 
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        'scrapy.contracts.default.UrlContract' : 1,
-        'scrapy.contracts.default.ReturnsContract': 2,
-        'scrapy.contracts.default.ScrapesContract': 3,
+        "scrapy.contracts.default.UrlContract": 1,
+        "scrapy.contracts.default.ReturnsContract": 2,
+        "scrapy.contracts.default.ScrapesContract": 3,
     }
 
 A dict containing the Scrapy contracts enabled by default in Scrapy. You should
 never modify this setting in your project, modify :setting:`SPIDER_CONTRACTS`
 instead. For more info see :ref:`topics-contracts`.
 
 You can disable any of these contracts by assigning ``None`` to their class
 path in :setting:`SPIDER_CONTRACTS`. E.g., to disable the built-in
-``ScrapesContract``, place this in your ``settings.py``::
+``ScrapesContract``, place this in your ``settings.py``:
+
+.. code-block:: python
 
     SPIDER_CONTRACTS = {
-        'scrapy.contracts.default.ScrapesContract': None,
+        "scrapy.contracts.default.ScrapesContract": None,
     }
 
 .. setting:: SPIDER_LOADER_CLASS
 
 SPIDER_LOADER_CLASS
 -------------------
 
@@ -1479,22 +1538,24 @@
 orders. For more info see :ref:`topics-spider-middleware-setting`.
 
 .. setting:: SPIDER_MIDDLEWARES_BASE
 
 SPIDER_MIDDLEWARES_BASE
 -----------------------
 
-Default::
+Default:
+
+.. code-block:: python
 
     {
-        'scrapy.spidermiddlewares.httperror.HttpErrorMiddleware': 50,
-        'scrapy.spidermiddlewares.offsite.OffsiteMiddleware': 500,
-        'scrapy.spidermiddlewares.referer.RefererMiddleware': 700,
-        'scrapy.spidermiddlewares.urllength.UrlLengthMiddleware': 800,
-        'scrapy.spidermiddlewares.depth.DepthMiddleware': 900,
+        "scrapy.spidermiddlewares.httperror.HttpErrorMiddleware": 50,
+        "scrapy.spidermiddlewares.offsite.OffsiteMiddleware": 500,
+        "scrapy.spidermiddlewares.referer.RefererMiddleware": 700,
+        "scrapy.spidermiddlewares.urllength.UrlLengthMiddleware": 800,
+        "scrapy.spidermiddlewares.depth.DepthMiddleware": 900,
     }
 
 A dict containing the spider middlewares enabled by default in Scrapy, and
 their orders. Low orders are closer to the engine, high orders are closer to
 the spider. For more info see :ref:`topics-spider-middleware-setting`.
 
 .. setting:: SPIDER_MODULES
@@ -1502,17 +1563,19 @@
 SPIDER_MODULES
 --------------
 
 Default: ``[]``
 
 A list of modules where Scrapy will look for spiders.
 
-Example::
+Example:
 
-    SPIDER_MODULES = ['mybot.spiders_prod', 'mybot.spiders_dev']
+.. code-block:: python
+
+    SPIDER_MODULES = ["mybot.spiders_prod", "mybot.spiders_dev"]
 
 .. setting:: STATS_CLASS
 
 STATS_CLASS
 -----------
 
 Default: ``'scrapy.statscollectors.MemoryStatsCollector'``
@@ -1593,68 +1656,73 @@
 :meth:`CrawlerRunner.__init__ <scrapy.crawler.CrawlerRunner.__init__>` raises
 :exc:`Exception` if the installed reactor does not match the
 :setting:`TWISTED_REACTOR` setting; therefore, having top-level
 :mod:`~twisted.internet.reactor` imports in project files and imported
 third-party libraries will make Scrapy raise :exc:`Exception` when
 it checks which reactor is installed.
 
-In order to use the reactor installed by Scrapy::
+In order to use the reactor installed by Scrapy:
+
+.. code-block:: python
 
     import scrapy
     from twisted.internet import reactor
 
 
     class QuotesSpider(scrapy.Spider):
-        name = 'quotes'
+        name = "quotes"
 
         def __init__(self, *args, **kwargs):
-            self.timeout = int(kwargs.pop('timeout', '60'))
+            self.timeout = int(kwargs.pop("timeout", "60"))
             super(QuotesSpider, self).__init__(*args, **kwargs)
 
         def start_requests(self):
             reactor.callLater(self.timeout, self.stop)
 
-            urls = ['https://quotes.toscrape.com/page/1']
+            urls = ["https://quotes.toscrape.com/page/1"]
             for url in urls:
                 yield scrapy.Request(url=url, callback=self.parse)
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
-                yield {'text': quote.css('span.text::text').get()}
+            for quote in response.css("div.quote"):
+                yield {"text": quote.css("span.text::text").get()}
 
         def stop(self):
-            self.crawler.engine.close_spider(self, 'timeout')
+            self.crawler.engine.close_spider(self, "timeout")
 
 
-which raises :exc:`Exception`, becomes::
+which raises :exc:`Exception`, becomes:
+
+.. code-block:: python
 
     import scrapy
 
 
     class QuotesSpider(scrapy.Spider):
-        name = 'quotes'
+        name = "quotes"
 
         def __init__(self, *args, **kwargs):
-            self.timeout = int(kwargs.pop('timeout', '60'))
+            self.timeout = int(kwargs.pop("timeout", "60"))
             super(QuotesSpider, self).__init__(*args, **kwargs)
 
         def start_requests(self):
             from twisted.internet import reactor
+
             reactor.callLater(self.timeout, self.stop)
 
-            urls = ['https://quotes.toscrape.com/page/1']
+            urls = ["https://quotes.toscrape.com/page/1"]
             for url in urls:
                 yield scrapy.Request(url=url, callback=self.parse)
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
-                yield {'text': quote.css('span.text::text').get()}
+            for quote in response.css("div.quote"):
+                yield {"text": quote.css("span.text::text").get()}
 
         def stop(self):
-            self.crawler.engine.close_spider(self, 'timeout')
+            self.crawler.engine.close_spider(self, "timeout")
 
 
 The default value of the :setting:`TWISTED_REACTOR` setting is ``None``, which
 means that Scrapy will use the existing reactor if one is already installed, or
 install the default reactor defined by Twisted for the current platform. This
 is to maintain backward compatibility and avoid possible problems caused by
 using a non-default reactor.
```

### Comparing `Scrapy-2.8.0/docs/topics/shell.rst` & `Scrapy-2.9.0/docs/topics/shell.rst`

 * *Files 10% similar despite different names*

```diff
@@ -187,66 +187,70 @@
     [s]   view(response)    View response in a browser
 
     >>>
 
 
 After that, we can start playing with the objects:
 
->>> response.xpath('//title/text()').get()
-'Scrapy | A Fast and Powerful Scraping and Web Crawling Framework'
+.. code-block:: pycon
 
->>> fetch("https://old.reddit.com/")
+    >>> response.xpath("//title/text()").get()
+    'Scrapy | A Fast and Powerful Scraping and Web Crawling Framework'
 
->>> response.xpath('//title/text()').get()
-'reddit: the front page of the internet'
+    >>> fetch("https://old.reddit.com/")
 
->>> request = request.replace(method="POST")
-
->>> fetch(request)
-
->>> response.status
-404
-
->>> from pprint import pprint
-
->>> pprint(response.headers)
-{'Accept-Ranges': ['bytes'],
- 'Cache-Control': ['max-age=0, must-revalidate'],
- 'Content-Type': ['text/html; charset=UTF-8'],
- 'Date': ['Thu, 08 Dec 2016 16:21:19 GMT'],
- 'Server': ['snooserv'],
- 'Set-Cookie': ['loid=KqNLou0V9SKMX4qb4n; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure',
-                'loidcreated=2016-12-08T16%3A21%3A19.445Z; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure',
-                'loid=vi0ZVe4NkxNWdlH7r7; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure',
-                'loidcreated=2016-12-08T16%3A21%3A19.459Z; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure'],
- 'Vary': ['accept-encoding'],
- 'Via': ['1.1 varnish'],
- 'X-Cache': ['MISS'],
- 'X-Cache-Hits': ['0'],
- 'X-Content-Type-Options': ['nosniff'],
- 'X-Frame-Options': ['SAMEORIGIN'],
- 'X-Moose': ['majestic'],
- 'X-Served-By': ['cache-cdg8730-CDG'],
- 'X-Timer': ['S1481214079.394283,VS0,VE159'],
- 'X-Ua-Compatible': ['IE=edge'],
- 'X-Xss-Protection': ['1; mode=block']}
+    >>> response.xpath("//title/text()").get()
+    'reddit: the front page of the internet'
+
+    >>> request = request.replace(method="POST")
+
+    >>> fetch(request)
+
+    >>> response.status
+    404
+
+    >>> from pprint import pprint
+
+    >>> pprint(response.headers)
+    {'Accept-Ranges': ['bytes'],
+    'Cache-Control': ['max-age=0, must-revalidate'],
+    'Content-Type': ['text/html; charset=UTF-8'],
+    'Date': ['Thu, 08 Dec 2016 16:21:19 GMT'],
+    'Server': ['snooserv'],
+    'Set-Cookie': ['loid=KqNLou0V9SKMX4qb4n; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure',
+                    'loidcreated=2016-12-08T16%3A21%3A19.445Z; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure',
+                    'loid=vi0ZVe4NkxNWdlH7r7; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure',
+                    'loidcreated=2016-12-08T16%3A21%3A19.459Z; Domain=reddit.com; Max-Age=63071999; Path=/; expires=Sat, 08-Dec-2018 16:21:19 GMT; secure'],
+    'Vary': ['accept-encoding'],
+    'Via': ['1.1 varnish'],
+    'X-Cache': ['MISS'],
+    'X-Cache-Hits': ['0'],
+    'X-Content-Type-Options': ['nosniff'],
+    'X-Frame-Options': ['SAMEORIGIN'],
+    'X-Moose': ['majestic'],
+    'X-Served-By': ['cache-cdg8730-CDG'],
+    'X-Timer': ['S1481214079.394283,VS0,VE159'],
+    'X-Ua-Compatible': ['IE=edge'],
+    'X-Xss-Protection': ['1; mode=block']}
 
 
 .. _topics-shell-inspect-response:
 
 Invoking the shell from spiders to inspect responses
 ====================================================
 
 Sometimes you want to inspect the responses that are being processed in a
 certain point of your spider, if only to check that response you expect is
 getting there.
 
 This can be achieved by using the ``scrapy.shell.inspect_response`` function.
 
-Here's an example of how you would call it from your spider::
+Here's an example of how you would call it from your spider:
+
+.. code-block:: python
 
     import scrapy
 
 
     class MySpider(scrapy.Spider):
         name = "myspider"
         start_urls = [
@@ -255,14 +259,15 @@
             "http://example.net",
         ]
 
         def parse(self, response):
             # We want to inspect one specific response.
             if ".org" in response.url:
                 from scrapy.shell import inspect_response
+
                 inspect_response(response, self)
 
             # Rest of parsing code.
 
 When you run the spider, you will get something similar to this::
 
     2014-01-23 17:48:31-0400 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://example.com> (referer: None)
@@ -272,22 +277,26 @@
     ...
 
     >>> response.url
     'http://example.org'
 
 Then, you can check if the extraction code is working:
 
->>> response.xpath('//h1[@class="fn"]')
-[]
+.. code-block:: pycon
+
+    >>> response.xpath('//h1[@class="fn"]')
+    []
 
 Nope, it doesn't. So you can open the response in your web browser and see if
 it's the response you were expecting:
 
->>> view(response)
-True
+.. code-block:: pycon
+
+    >>> view(response)
+    True
 
 Finally you hit Ctrl-D (or Ctrl-Z in Windows) to exit the shell and resume the
 crawling::
 
     >>> ^D
     2014-01-23 17:50:03-0400 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://example.net> (referer: None)
     ...
```

### Comparing `Scrapy-2.8.0/docs/topics/signals.rst` & `Scrapy-2.9.0/docs/topics/signals.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,38 @@
 Even though signals provide several arguments, the handlers that catch them
 don't need to accept all of them - the signal dispatching mechanism will only
 deliver the arguments that the handler receives.
 
 You can connect to signals (or send your own) through the
 :ref:`topics-api-signals`.
 
-Here is a simple example showing how you can catch signals and perform some action::
+Here is a simple example showing how you can catch signals and perform some action:
+
+.. code-block:: python
 
     from scrapy import signals
     from scrapy import Spider
 
 
     class DmozSpider(Spider):
         name = "dmoz"
         allowed_domains = ["dmoz.org"]
         start_urls = [
             "http://www.dmoz.org/Computers/Programming/Languages/Python/Books/",
             "http://www.dmoz.org/Computers/Programming/Languages/Python/Resources/",
         ]
 
-
         @classmethod
         def from_crawler(cls, crawler, *args, **kwargs):
             spider = super(DmozSpider, cls).from_crawler(crawler, *args, **kwargs)
             crawler.signals.connect(spider.spider_closed, signal=signals.spider_closed)
             return spider
 
-
         def spider_closed(self, spider):
-            spider.logger.info('Spider closed: %s', spider.name)
-
+            spider.logger.info("Spider closed: %s", spider.name)
 
         def parse(self, response):
             pass
 
 .. _signal-deferred:
 
 Deferred signal handlers
@@ -52,42 +51,47 @@
 
 Some signals support returning :class:`~twisted.internet.defer.Deferred`
 or :term:`awaitable objects <awaitable>` from their handlers, allowing
 you to run asynchronous code that does not block Scrapy. If a signal
 handler returns one of these objects, Scrapy waits for that asynchronous
 operation to finish.
 
-Let's take an example using :ref:`coroutines <topics-coroutines>`::
+Let's take an example using :ref:`coroutines <topics-coroutines>`:
+
+.. code-block:: python
+
+    import scrapy
+
 
     class SignalSpider(scrapy.Spider):
-        name = 'signals'
-        start_urls = ['https://quotes.toscrape.com/page/1/']
+        name = "signals"
+        start_urls = ["https://quotes.toscrape.com/page/1/"]
 
         @classmethod
         def from_crawler(cls, crawler, *args, **kwargs):
             spider = super(SignalSpider, cls).from_crawler(crawler, *args, **kwargs)
             crawler.signals.connect(spider.item_scraped, signal=signals.item_scraped)
             return spider
 
         async def item_scraped(self, item):
             # Send the scraped item to the server
             response = await treq.post(
-                'http://example.com/post',
-                json.dumps(item).encode('ascii'),
-                headers={b'Content-Type': [b'application/json']}
+                "http://example.com/post",
+                json.dumps(item).encode("ascii"),
+                headers={b"Content-Type": [b"application/json"]},
             )
 
             return response
 
         def parse(self, response):
-            for quote in response.css('div.quote'):
+            for quote in response.css("div.quote"):
                 yield {
-                    'text': quote.css('span.text::text').get(),
-                    'author': quote.css('small.author::text').get(),
-                    'tags': quote.css('div.tags a.tag::text').getall(),
+                    "text": quote.css("span.text::text").get(),
+                    "author": quote.css("small.author::text").get(),
+                    "tags": quote.css("div.tags a.tag::text").getall(),
                 }
 
 See the :ref:`topics-signals-ref` below to know which signals support
 :class:`~twisted.internet.defer.Deferred` and :term:`awaitable objects <awaitable>`.
 
 .. _topics-signals-ref:
 
@@ -299,14 +303,41 @@
 
     :param response: the response being processed when the exception was raised
     :type response: :class:`~scrapy.http.Response` object
 
     :param spider: the spider which raised the exception
     :type spider: :class:`~scrapy.Spider` object
 
+feed_slot_closed
+~~~~~~~~~~~~~~~~
+
+.. signal:: feed_slot_closed
+.. function:: feed_slot_closed(slot)
+
+    Sent when a :ref:`feed exports <topics-feed-exports>` slot is closed.
+
+    This signal supports returning deferreds from its handlers.
+
+    :param slot: the slot closed
+    :type slot: scrapy.extensions.feedexport.FeedSlot
+
+
+feed_exporter_closed
+~~~~~~~~~~~~~~~~~~~~
+
+.. signal:: feed_exporter_closed
+.. function:: feed_exporter_closed()
+
+    Sent when the :ref:`feed exports <topics-feed-exports>` extension is closed,
+    during the handling of the :signal:`spider_closed` signal by the extension,
+    after all feed exporting has been handled.
+
+    This signal supports returning deferreds from its handlers.
+
+
 Request signals
 ---------------
 
 request_scheduled
 ~~~~~~~~~~~~~~~~~
 
 .. signal:: request_scheduled
```

### Comparing `Scrapy-2.8.0/docs/topics/spider-middleware.rst` & `Scrapy-2.9.0/docs/topics/spider-middleware.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 Activating a spider middleware
 ==============================
 
 To activate a spider middleware component, add it to the
 :setting:`SPIDER_MIDDLEWARES` setting, which is a dict whose keys are the
 middleware class path and their values are the middleware orders.
 
-Here's an example::
+Here's an example:
+
+.. code-block:: python
 
     SPIDER_MIDDLEWARES = {
-        'myproject.middlewares.CustomSpiderMiddleware': 543,
+        "myproject.middlewares.CustomSpiderMiddleware": 543,
     }
 
 The :setting:`SPIDER_MIDDLEWARES` setting is merged with the
 :setting:`SPIDER_MIDDLEWARES_BASE` setting defined in Scrapy (and not meant to
 be overridden) and then sorted by order to get the final sorted list of enabled
 middlewares: the first middleware is the one closer to the engine and the last
 is the one closer to the spider. In other words,
@@ -40,19 +42,21 @@
 you want to insert the middleware. The order does matter because each
 middleware performs a different action and your middleware could depend on some
 previous (or subsequent) middleware being applied.
 
 If you want to disable a builtin middleware (the ones defined in
 :setting:`SPIDER_MIDDLEWARES_BASE`, and enabled by default) you must define it
 in your project :setting:`SPIDER_MIDDLEWARES` setting and assign ``None`` as its
-value.  For example, if you want to disable the off-site middleware::
+value.  For example, if you want to disable the off-site middleware:
+
+.. code-block:: python
 
     SPIDER_MIDDLEWARES = {
-        'myproject.middlewares.CustomSpiderMiddleware': 543,
-        'scrapy.spidermiddlewares.offsite.OffsiteMiddleware': None,
+        "myproject.middlewares.CustomSpiderMiddleware": 543,
+        "scrapy.spidermiddlewares.offsite.OffsiteMiddleware": None,
     }
 
 Finally, keep in mind that some middlewares may need to be enabled through a
 particular setting. See each middleware documentation for more info.
 
 .. _custom-spider-middleware:
 
@@ -257,15 +261,20 @@
 
 If you still want to process response codes outside that range, you can
 specify which response codes the spider is able to handle using the
 ``handle_httpstatus_list`` spider attribute or
 :setting:`HTTPERROR_ALLOWED_CODES` setting.
 
 For example, if you want your spider to handle 404 responses you can do
-this::
+this:
+
+.. code-block:: python
+
+    from scrapy.spiders import CrawlSpider
+
 
     class MySpider(CrawlSpider):
         handle_httpstatus_list = [404]
 
 .. reqmeta:: handle_httpstatus_list
 
 .. reqmeta:: handle_httpstatus_all
```

### Comparing `Scrapy-2.8.0/docs/topics/stats.rst` & `Scrapy-2.9.0/docs/topics/stats.rst`

 * *Files 6% similar despite different names*

```diff
@@ -26,50 +26,63 @@
 
 .. _topics-stats-usecases:
 
 Common Stats Collector uses
 ===========================
 
 Access the stats collector through the :attr:`~scrapy.crawler.Crawler.stats`
-attribute. Here is an example of an extension that access stats::
+attribute. Here is an example of an extension that access stats:
 
-    class ExtensionThatAccessStats:
+.. code-block:: python
 
+    class ExtensionThatAccessStats:
         def __init__(self, stats):
             self.stats = stats
 
         @classmethod
         def from_crawler(cls, crawler):
             return cls(crawler.stats)
 
-Set stat value::
+Set stat value:
+
+.. code-block:: python
+
+    stats.set_value("hostname", socket.gethostname())
 
-    stats.set_value('hostname', socket.gethostname())
+Increment stat value:
 
-Increment stat value::
+.. code-block:: python
 
-    stats.inc_value('custom_count')
+    stats.inc_value("custom_count")
 
-Set stat value only if greater than previous::
+Set stat value only if greater than previous:
 
-    stats.max_value('max_items_scraped', value)
+.. code-block:: python
 
-Set stat value only if lower than previous::
+    stats.max_value("max_items_scraped", value)
 
-    stats.min_value('min_free_memory_percent', value)
+Set stat value only if lower than previous:
+
+.. code-block:: python
+
+    stats.min_value("min_free_memory_percent", value)
 
 Get stat value:
 
->>> stats.get_value('custom_count')
-1
+.. code-block:: pycon
+
+    >>> stats.get_value("custom_count")
+    1
 
 Get all stats:
 
->>> stats.get_stats()
-{'custom_count': 1, 'start_time': datetime.datetime(2009, 7, 14, 21, 47, 28, 977139)}
+.. code-block:: pycon
+
+    >>> stats.get_stats()
+    {'custom_count': 1, 'start_time': datetime.datetime(2009, 7, 14, 21, 47, 28, 977139)}
 
 Available Stats Collectors
 ==========================
 
 Besides the basic :class:`StatsCollector` there are other Stats Collectors
 available in Scrapy which extend the basic Stats Collector. You can select
 which Stats Collector to use through the :setting:`STATS_CLASS` setting. The
```

### Comparing `Scrapy-2.8.0/docs/topics/telnetconsole.rst` & `Scrapy-2.9.0/docs/topics/telnetconsole.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/docs/utils/linkfix.py` & `Scrapy-2.9.0/docs/utils/linkfix.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import re
 import sys
 from pathlib import Path
 
 
 def main():
-
     # Used for remembering the file (and its contents)
     # so we don't have to open the same file again.
     _filename = None
     _contents = None
 
     # A regex that matches standard linkcheck output lines
     line_re = re.compile(r"(.*)\:\d+\:\s\[(.*)\]\s(?:(.*)\sto\s(.*)|(.*))")
@@ -46,15 +45,14 @@
             # Broken links can't be fixed and
             # I am not sure what do with the local ones.
             if errortype.lower() in ["broken", "local"]:
                 print("Not Fixed: " + line)
             else:
                 # If this is a new file
                 if newfilename != _filename:
-
                     # Update the previous file
                     if _filename:
                         Path(_filename).write_text(_contents, encoding="utf-8")
 
                     _filename = newfilename
 
                     # Read the new file to memory
```

### Comparing `Scrapy-2.8.0/docs/versioning.rst` & `Scrapy-2.9.0/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/extras/qps-bench-server.py` & `Scrapy-2.9.0/extras/qps-bench-server.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/extras/qpsclient.py` & `Scrapy-2.9.0/extras/qpsclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from scrapy.http import Request
 from scrapy.spiders import Spider
 
 
 class QPSSpider(Spider):
-
     name = "qps"
     benchurl = "http://localhost:8880/"
 
     # Max concurrency is limited by global CONCURRENT_REQUESTS setting
     max_concurrent_requests = 8
     # Requests per second goal
     qps = None  # same as: 1 / download_delay
```

### Comparing `Scrapy-2.8.0/extras/scrapy.1` & `Scrapy-2.9.0/extras/scrapy.1`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/extras/scrapy_bash_completion` & `Scrapy-2.9.0/extras/scrapy_bash_completion`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/extras/scrapy_zsh_completion` & `Scrapy-2.9.0/extras/scrapy_zsh_completion`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/pytest.ini` & `Scrapy-2.9.0/pytest.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [pytest]
 xfail_strict = true
 usefixtures = chdir
 python_files=test_*.py __init__.py
 python_classes=
 addopts =
     --assert=plain
-    --doctest-modules
     --ignore=docs/_ext
     --ignore=docs/conf.py
     --ignore=docs/news.rst
     --ignore=docs/topics/dynamic-content.rst
     --ignore=docs/topics/items.rst
     --ignore=docs/topics/leaks.rst
     --ignore=docs/topics/loaders.rst
```

### Comparing `Scrapy-2.8.0/scrapy/__init__.py` & `Scrapy-2.9.0/scrapy/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/cmdline.py` & `Scrapy-2.9.0/scrapy/cmdline.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/commands/__init__.py` & `Scrapy-2.9.0/scrapy/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from scrapy.crawler import CrawlerProcess
 from scrapy.exceptions import UsageError
 from scrapy.utils.conf import arglist_to_dict, feed_process_params_from_cli
 
 
 class ScrapyCommand:
-
     requires_project = False
     crawler_process: Optional[CrawlerProcess] = None
 
     # default settings to be used for this command instead of global defaults
     default_settings: Dict[str, Any] = {}
 
     exitcode = 0
```

### Comparing `Scrapy-2.8.0/scrapy/commands/bench.py` & `Scrapy-2.9.0/scrapy/commands/bench.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import scrapy
 from scrapy.commands import ScrapyCommand
 from scrapy.linkextractors import LinkExtractor
 
 
 class Command(ScrapyCommand):
-
     default_settings = {
         "LOG_LEVEL": "INFO",
         "LOGSTATS_INTERVAL": 1,
         "CLOSESPIDER_TIMEOUT": 10,
     }
 
     def short_desc(self):
```

### Comparing `Scrapy-2.8.0/scrapy/commands/check.py` & `Scrapy-2.9.0/scrapy/commands/check.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/commands/crawl.py` & `Scrapy-2.9.0/scrapy/commands/crawl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from scrapy.commands import BaseRunSpiderCommand
 from scrapy.exceptions import UsageError
 
 
 class Command(BaseRunSpiderCommand):
-
     requires_project = True
 
     def syntax(self):
         return "[options] <spider>"
 
     def short_desc(self):
         return "Run a spider"
```

### Comparing `Scrapy-2.8.0/scrapy/commands/edit.py` & `Scrapy-2.9.0/scrapy/commands/edit.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import sys
 
 from scrapy.commands import ScrapyCommand
 from scrapy.exceptions import UsageError
 
 
 class Command(ScrapyCommand):
-
     requires_project = True
     default_settings = {"LOG_ENABLED": False}
 
     def syntax(self):
         return "<spider>"
 
     def short_desc(self):
```

### Comparing `Scrapy-2.8.0/scrapy/commands/fetch.py` & `Scrapy-2.9.0/scrapy/commands/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from scrapy.exceptions import UsageError
 from scrapy.http import Request
 from scrapy.utils.datatypes import SequenceExclude
 from scrapy.utils.spider import DefaultSpider, spidercls_for_request
 
 
 class Command(ScrapyCommand):
-
     requires_project = False
 
     def syntax(self):
         return "[options] <url>"
 
     def short_desc(self):
         return "Fetch a URL using the Scrapy downloader"
```

### Comparing `Scrapy-2.8.0/scrapy/commands/genspider.py` & `Scrapy-2.9.0/scrapy/commands/genspider.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,23 @@
     """Extract domain name from URL string"""
     o = urlparse(url)
     if o.scheme == "" and o.netloc == "":
         o = urlparse("//" + url.lstrip("/"))
     return o.netloc
 
 
-class Command(ScrapyCommand):
+def verify_url_scheme(url):
+    """Check url for scheme and insert https if none found."""
+    parsed = urlparse(url)
+    if parsed.scheme == "" and parsed.netloc == "":
+        parsed = urlparse("//" + url)._replace(scheme="https")
+    return parsed.geturl()
+
 
+class Command(ScrapyCommand):
     requires_project = False
     default_settings = {"LOG_ENABLED": False}
 
     def syntax(self):
         return "[options] <name> <domain>"
 
     def short_desc(self):
@@ -88,38 +95,40 @@
             if template_file:
                 print(template_file.read_text(encoding="utf-8"))
             return
         if len(args) != 2:
             raise UsageError()
 
         name, url = args[0:2]
-        domain = extract_domain(url)
+        url = verify_url_scheme(url)
         module = sanitize_module_name(name)
 
         if self.settings.get("BOT_NAME") == module:
             print("Cannot create a spider with the same name as your project")
             return
 
         if not opts.force and self._spider_exists(name):
             return
 
         template_file = self._find_template(opts.template)
         if template_file:
-            self._genspider(module, name, domain, opts.template, template_file)
+            self._genspider(module, name, url, opts.template, template_file)
             if opts.edit:
                 self.exitcode = os.system(f'scrapy edit "{name}"')
 
-    def _genspider(self, module, name, domain, template_name, template_file):
+    def _genspider(self, module, name, url, template_name, template_file):
         """Generate the spider module, based on the given template"""
         capitalized_module = "".join(s.capitalize() for s in module.split("_"))
+        domain = extract_domain(url)
         tvars = {
             "project_name": self.settings.get("BOT_NAME"),
             "ProjectName": string_camelcase(self.settings.get("BOT_NAME")),
             "module": module,
             "name": name,
+            "url": url,
             "domain": domain,
             "classname": f"{capitalized_module}Spider",
         }
         if self.settings.get("NEWSPIDER_MODULE"):
             spiders_module = import_module(self.settings["NEWSPIDER_MODULE"])
             spiders_dir = Path(spiders_module.__file__).parent.resolve()
         else:
```

### Comparing `Scrapy-2.8.0/scrapy/commands/parse.py` & `Scrapy-2.9.0/scrapy/commands/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import inspect
 import json
 import logging
 from typing import Dict
 
 from itemadapter import ItemAdapter, is_item
 from twisted.internet.defer import maybeDeferred
 from w3lib.url import is_url
 
 from scrapy.commands import BaseRunSpiderCommand
 from scrapy.exceptions import UsageError
 from scrapy.http import Request
 from scrapy.utils import display
-from scrapy.utils.spider import iterate_spider_output, spidercls_for_request
+from scrapy.utils.asyncgen import collect_asyncgen
+from scrapy.utils.defer import aiter_errback, deferred_from_coro
+from scrapy.utils.log import failure_to_exc_info
+from scrapy.utils.misc import arg_to_iter
+from scrapy.utils.spider import spidercls_for_request
 
 logger = logging.getLogger(__name__)
 
 
 class Command(BaseRunSpiderCommand):
     requires_project = True
 
@@ -104,14 +109,33 @@
         max_items, max_requests = 0, 0
         if self.items:
             max_items = max(self.items)
         if self.requests:
             max_requests = max(self.requests)
         return max(max_items, max_requests)
 
+    def handle_exception(self, _failure):
+        logger.error(
+            "An error is caught while iterating the async iterable",
+            exc_info=failure_to_exc_info(_failure),
+        )
+
+    def iterate_spider_output(self, result):
+        if inspect.isasyncgen(result):
+            d = deferred_from_coro(
+                collect_asyncgen(aiter_errback(result, self.handle_exception))
+            )
+            d.addCallback(self.iterate_spider_output)
+            return d
+        if inspect.iscoroutine(result):
+            d = deferred_from_coro(result)
+            d.addCallback(self.iterate_spider_output)
+            return d
+        return arg_to_iter(deferred_from_coro(result))
+
     def add_items(self, lvl, new_items):
         old_items = self.items.get(lvl, [])
         self.items[lvl] = old_items + new_items
 
     def add_requests(self, lvl, new_reqs):
         old_reqs = self.requests.get(lvl, [])
         self.requests[lvl] = old_reqs + new_reqs
@@ -161,15 +185,15 @@
                 items.append(x)
             elif isinstance(x, Request):
                 requests.append(x)
         return items, requests, opts, depth, spider, callback
 
     def run_callback(self, response, callback, cb_kwargs=None):
         cb_kwargs = cb_kwargs or {}
-        d = maybeDeferred(iterate_spider_output, callback(response, **cb_kwargs))
+        d = maybeDeferred(self.iterate_spider_output, callback(response, **cb_kwargs))
         return d
 
     def get_callback_from_rules(self, spider, response):
         if getattr(spider, "rules", None):
             for rule in spider.rules:
                 if rule.link_extractor.matches(response.url):
                     return rule.callback or "parse"
```

### Comparing `Scrapy-2.8.0/scrapy/commands/runspider.py` & `Scrapy-2.9.0/scrapy/commands/runspider.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         module = import_module(abspath.stem)
     finally:
         sys.path.pop(0)
     return module
 
 
 class Command(BaseRunSpiderCommand):
-
     requires_project = False
     default_settings = {"SPIDER_LOADER_WARN_ONLY": True}
 
     def syntax(self):
         return "[options] <spider_file>"
 
     def short_desc(self):
```

### Comparing `Scrapy-2.8.0/scrapy/commands/settings.py` & `Scrapy-2.9.0/scrapy/commands/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 
 from scrapy.commands import ScrapyCommand
 from scrapy.settings import BaseSettings
 
 
 class Command(ScrapyCommand):
-
     requires_project = False
     default_settings = {"LOG_ENABLED": False, "SPIDER_LOADER_WARN_ONLY": True}
 
     def syntax(self):
         return "[options]"
 
     def short_desc(self):
```

### Comparing `Scrapy-2.8.0/scrapy/commands/shell.py` & `Scrapy-2.9.0/scrapy/commands/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from scrapy.http import Request
 from scrapy.shell import Shell
 from scrapy.utils.spider import DefaultSpider, spidercls_for_request
 from scrapy.utils.url import guess_scheme
 
 
 class Command(ScrapyCommand):
-
     requires_project = False
     default_settings = {
         "KEEP_ALIVE": True,
         "LOGSTATS_INTERVAL": 0,
         "DUPEFILTER_CLASS": "scrapy.dupefilters.BaseDupeFilter",
     }
```

### Comparing `Scrapy-2.8.0/scrapy/commands/startproject.py` & `Scrapy-2.9.0/scrapy/commands/startproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 def _make_writable(path):
     current_permissions = os.stat(path).st_mode
     os.chmod(path, current_permissions | OWNER_WRITE_PERMISSION)
 
 
 class Command(ScrapyCommand):
-
     requires_project = False
     default_settings = {"LOG_ENABLED": False, "SPIDER_LOADER_WARN_ONLY": True}
 
     def syntax(self):
         return "<project_name> [project_dir]"
 
     def short_desc(self):
```

### Comparing `Scrapy-2.8.0/scrapy/commands/version.py` & `Scrapy-2.9.0/scrapy/commands/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import scrapy
 from scrapy.commands import ScrapyCommand
 from scrapy.utils.versions import scrapy_components_versions
 
 
 class Command(ScrapyCommand):
-
     default_settings = {"LOG_ENABLED": False, "SPIDER_LOADER_WARN_ONLY": True}
 
     def syntax(self):
         return "[-v]"
 
     def short_desc(self):
         return "Print Scrapy version"
```

### Comparing `Scrapy-2.8.0/scrapy/commands/view.py` & `Scrapy-2.9.0/scrapy/commands/view.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/contracts/__init__.py` & `Scrapy-2.9.0/scrapy/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/contracts/default.py` & `Scrapy-2.9.0/scrapy/contracts/default.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/__init__.py` & `Scrapy-2.9.0/scrapy/core/downloader/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,146 +1,169 @@
 import random
 from collections import deque
 from datetime import datetime
 from time import time
+from typing import TYPE_CHECKING, Any, Deque, Dict, Set, Tuple, cast
 
-from twisted.internet import defer, task
+from twisted.internet import task
+from twisted.internet.defer import Deferred
 
-from scrapy import signals
+from scrapy import Request, Spider, signals
 from scrapy.core.downloader.handlers import DownloadHandlers
 from scrapy.core.downloader.middleware import DownloaderMiddlewareManager
+from scrapy.http import Response
 from scrapy.resolver import dnscache
+from scrapy.settings import BaseSettings
+from scrapy.signalmanager import SignalManager
 from scrapy.utils.defer import mustbe_deferred
 from scrapy.utils.httpobj import urlparse_cached
 
+if TYPE_CHECKING:
+    from scrapy.crawler import Crawler
+
 
 class Slot:
     """Downloader slot"""
 
-    def __init__(self, concurrency, delay, randomize_delay):
-        self.concurrency = concurrency
-        self.delay = delay
-        self.randomize_delay = randomize_delay
-
-        self.active = set()
-        self.queue = deque()
-        self.transferring = set()
-        self.lastseen = 0
+    def __init__(self, concurrency: int, delay: float, randomize_delay: bool):
+        self.concurrency: int = concurrency
+        self.delay: float = delay
+        self.randomize_delay: bool = randomize_delay
+
+        self.active: Set[Request] = set()
+        self.queue: Deque[Tuple[Request, Deferred]] = deque()
+        self.transferring: Set[Request] = set()
+        self.lastseen: float = 0
         self.latercall = None
 
-    def free_transfer_slots(self):
+    def free_transfer_slots(self) -> int:
         return self.concurrency - len(self.transferring)
 
-    def download_delay(self):
+    def download_delay(self) -> float:
         if self.randomize_delay:
             return random.uniform(0.5 * self.delay, 1.5 * self.delay)
         return self.delay
 
-    def close(self):
+    def close(self) -> None:
         if self.latercall and self.latercall.active():
             self.latercall.cancel()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         cls_name = self.__class__.__name__
         return (
             f"{cls_name}(concurrency={self.concurrency!r}, "
             f"delay={self.delay:.2f}, "
             f"randomize_delay={self.randomize_delay!r})"
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
             f"<downloader.Slot concurrency={self.concurrency!r} "
             f"delay={self.delay:.2f} randomize_delay={self.randomize_delay!r} "
             f"len(active)={len(self.active)} len(queue)={len(self.queue)} "
             f"len(transferring)={len(self.transferring)} "
             f"lastseen={datetime.fromtimestamp(self.lastseen).isoformat()}>"
         )
 
 
-def _get_concurrency_delay(concurrency, spider, settings):
-    delay = settings.getfloat("DOWNLOAD_DELAY")
+def _get_concurrency_delay(
+    concurrency: int, spider: Spider, settings: BaseSettings
+) -> Tuple[int, float]:
+    delay: float = settings.getfloat("DOWNLOAD_DELAY")
     if hasattr(spider, "download_delay"):
         delay = spider.download_delay
 
     if hasattr(spider, "max_concurrent_requests"):
         concurrency = spider.max_concurrent_requests
 
     return concurrency, delay
 
 
 class Downloader:
-
     DOWNLOAD_SLOT = "download_slot"
 
-    def __init__(self, crawler):
-        self.settings = crawler.settings
-        self.signals = crawler.signals
-        self.slots = {}
-        self.active = set()
-        self.handlers = DownloadHandlers(crawler)
-        self.total_concurrency = self.settings.getint("CONCURRENT_REQUESTS")
-        self.domain_concurrency = self.settings.getint("CONCURRENT_REQUESTS_PER_DOMAIN")
-        self.ip_concurrency = self.settings.getint("CONCURRENT_REQUESTS_PER_IP")
-        self.randomize_delay = self.settings.getbool("RANDOMIZE_DOWNLOAD_DELAY")
-        self.middleware = DownloaderMiddlewareManager.from_crawler(crawler)
-        self._slot_gc_loop = task.LoopingCall(self._slot_gc)
+    def __init__(self, crawler: "Crawler"):
+        self.settings: BaseSettings = crawler.settings
+        self.signals: SignalManager = crawler.signals
+        self.slots: Dict[str, Slot] = {}
+        self.active: Set[Request] = set()
+        self.handlers: DownloadHandlers = DownloadHandlers(crawler)
+        self.total_concurrency: int = self.settings.getint("CONCURRENT_REQUESTS")
+        self.domain_concurrency: int = self.settings.getint(
+            "CONCURRENT_REQUESTS_PER_DOMAIN"
+        )
+        self.ip_concurrency: int = self.settings.getint("CONCURRENT_REQUESTS_PER_IP")
+        self.randomize_delay: bool = self.settings.getbool("RANDOMIZE_DOWNLOAD_DELAY")
+        self.middleware: DownloaderMiddlewareManager = (
+            DownloaderMiddlewareManager.from_crawler(crawler)
+        )
+        self._slot_gc_loop: task.LoopingCall = task.LoopingCall(self._slot_gc)
         self._slot_gc_loop.start(60)
+        self.per_slot_settings: Dict[str, Dict[str, Any]] = self.settings.getdict(
+            "DOWNLOAD_SLOTS", {}
+        )
 
-    def fetch(self, request, spider):
-        def _deactivate(response):
+    def fetch(self, request: Request, spider: Spider) -> Deferred:
+        def _deactivate(response: Response) -> Response:
             self.active.remove(request)
             return response
 
         self.active.add(request)
         dfd = self.middleware.download(self._enqueue_request, request, spider)
         return dfd.addBoth(_deactivate)
 
-    def needs_backout(self):
+    def needs_backout(self) -> bool:
         return len(self.active) >= self.total_concurrency
 
-    def _get_slot(self, request, spider):
+    def _get_slot(self, request: Request, spider: Spider) -> Tuple[str, Slot]:
         key = self._get_slot_key(request, spider)
         if key not in self.slots:
+            slot_settings = self.per_slot_settings.get(key, {})
             conc = (
                 self.ip_concurrency if self.ip_concurrency else self.domain_concurrency
             )
             conc, delay = _get_concurrency_delay(conc, spider, self.settings)
-            self.slots[key] = Slot(conc, delay, self.randomize_delay)
+            conc, delay = (
+                slot_settings.get("concurrency", conc),
+                slot_settings.get("delay", delay),
+            )
+            randomize_delay = slot_settings.get("randomize_delay", self.randomize_delay)
+            new_slot = Slot(conc, delay, randomize_delay)
+            self.slots[key] = new_slot
 
         return key, self.slots[key]
 
-    def _get_slot_key(self, request, spider):
+    def _get_slot_key(self, request: Request, spider: Spider) -> str:
         if self.DOWNLOAD_SLOT in request.meta:
-            return request.meta[self.DOWNLOAD_SLOT]
+            return cast(str, request.meta[self.DOWNLOAD_SLOT])
 
         key = urlparse_cached(request).hostname or ""
         if self.ip_concurrency:
             key = dnscache.get(key, key)
 
         return key
 
-    def _enqueue_request(self, request, spider):
+    def _enqueue_request(self, request: Request, spider: Spider) -> Deferred:
         key, slot = self._get_slot(request, spider)
         request.meta[self.DOWNLOAD_SLOT] = key
 
-        def _deactivate(response):
+        def _deactivate(response: Response) -> Response:
             slot.active.remove(request)
             return response
 
         slot.active.add(request)
         self.signals.send_catch_log(
             signal=signals.request_reached_downloader, request=request, spider=spider
         )
-        deferred = defer.Deferred().addBoth(_deactivate)
+        deferred = Deferred().addBoth(_deactivate)
         slot.queue.append((request, deferred))
         self._process_queue(spider, slot)
         return deferred
 
-    def _process_queue(self, spider, slot):
+    def _process_queue(self, spider: Spider, slot: Slot) -> None:
         from twisted.internet import reactor
 
         if slot.latercall and slot.latercall.active():
             return
 
         # Delay queue processing if a download_delay is configured
         now = time()
@@ -160,23 +183,23 @@
             dfd = self._download(slot, request, spider)
             dfd.chainDeferred(deferred)
             # prevent burst if inter-request delays were configured
             if delay:
                 self._process_queue(spider, slot)
                 break
 
-    def _download(self, slot, request, spider):
+    def _download(self, slot: Slot, request: Request, spider: Spider) -> Deferred:
         # The order is very important for the following deferreds. Do not change!
 
         # 1. Create the download deferred
         dfd = mustbe_deferred(self.handlers.download_request, request, spider)
 
         # 2. Notify response_downloaded listeners about the recent download
         # before querying queue for next request
-        def _downloaded(response):
+        def _downloaded(response: Response) -> Response:
             self.signals.send_catch_log(
                 signal=signals.response_downloaded,
                 response=response,
                 request=request,
                 spider=spider,
             )
             return response
@@ -185,27 +208,27 @@
 
         # 3. After response arrives, remove the request from transferring
         # state to free up the transferring slot so it can be used by the
         # following requests (perhaps those which came from the downloader
         # middleware itself)
         slot.transferring.add(request)
 
-        def finish_transferring(_):
+        def finish_transferring(_: Any) -> Any:
             slot.transferring.remove(request)
             self._process_queue(spider, slot)
             self.signals.send_catch_log(
                 signal=signals.request_left_downloader, request=request, spider=spider
             )
             return _
 
         return dfd.addBoth(finish_transferring)
 
-    def close(self):
+    def close(self) -> None:
         self._slot_gc_loop.stop()
         for slot in self.slots.values():
             slot.close()
 
-    def _slot_gc(self, age=60):
+    def _slot_gc(self, age: float = 60) -> None:
         mintime = time() - age
         for key, slot in list(self.slots.items()):
             if not slot.active and slot.lastseen + slot.delay < mintime:
                 self.slots.pop(key).close()
```

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/contextfactory.py` & `Scrapy-2.9.0/scrapy/core/downloader/contextfactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from typing import TYPE_CHECKING, Any, List, Optional
 
 from OpenSSL import SSL
 from twisted.internet._sslverify import _setAcceptableProtocols
 from twisted.internet.ssl import (
     AcceptableCiphers,
     CertificateOptions,
     optionsForClientTLS,
@@ -14,16 +15,20 @@
 from zope.interface.verify import verifyObject
 
 from scrapy.core.downloader.tls import (
     DEFAULT_CIPHERS,
     ScrapyClientTLSOptions,
     openssl_methods,
 )
+from scrapy.settings import BaseSettings
 from scrapy.utils.misc import create_instance, load_object
 
+if TYPE_CHECKING:
+    from twisted.internet._sslverify import ClientTLSOptions
+
 
 @implementer(IPolicyForHTTPS)
 class ScrapyClientContextFactory(BrowserLikePolicyForHTTPS):
     """
     Non-peer-certificate verifying HTTPS context factory
 
     Default OpenSSL method is TLS_METHOD (also called SSLv23_METHOD)
@@ -31,41 +36,50 @@
 
     'A TLS/SSL connection established with [this method] may
      understand the TLSv1, TLSv1.1 and TLSv1.2 protocols.'
     """
 
     def __init__(
         self,
-        method=SSL.SSLv23_METHOD,
-        tls_verbose_logging=False,
-        tls_ciphers=None,
-        *args,
-        **kwargs,
+        method: int = SSL.SSLv23_METHOD,
+        tls_verbose_logging: bool = False,
+        tls_ciphers: Optional[str] = None,
+        *args: Any,
+        **kwargs: Any,
     ):
         super().__init__(*args, **kwargs)
-        self._ssl_method = method
-        self.tls_verbose_logging = tls_verbose_logging
+        self._ssl_method: int = method
+        self.tls_verbose_logging: bool = tls_verbose_logging
+        self.tls_ciphers: AcceptableCiphers
         if tls_ciphers:
             self.tls_ciphers = AcceptableCiphers.fromOpenSSLCipherString(tls_ciphers)
         else:
             self.tls_ciphers = DEFAULT_CIPHERS
 
     @classmethod
-    def from_settings(cls, settings, method=SSL.SSLv23_METHOD, *args, **kwargs):
-        tls_verbose_logging = settings.getbool("DOWNLOADER_CLIENT_TLS_VERBOSE_LOGGING")
-        tls_ciphers = settings["DOWNLOADER_CLIENT_TLS_CIPHERS"]
-        return cls(
+    def from_settings(
+        cls,
+        settings: BaseSettings,
+        method: int = SSL.SSLv23_METHOD,
+        *args: Any,
+        **kwargs: Any,
+    ):
+        tls_verbose_logging: bool = settings.getbool(
+            "DOWNLOADER_CLIENT_TLS_VERBOSE_LOGGING"
+        )
+        tls_ciphers: Optional[str] = settings["DOWNLOADER_CLIENT_TLS_CIPHERS"]
+        return cls(  # type: ignore[misc]
             method=method,
             tls_verbose_logging=tls_verbose_logging,
             tls_ciphers=tls_ciphers,
             *args,
             **kwargs,
         )
 
-    def getCertificateOptions(self):
+    def getCertificateOptions(self) -> CertificateOptions:
         # setting verify=True will require you to provide CAs
         # to verify against; in other words: it's not that simple
 
         # backward-compatible SSL/TLS method:
         #
         # * this will respect `method` attribute in often recommended
         #   `ScrapyClientContextFactory` subclass
@@ -78,20 +92,20 @@
             method=getattr(self, "method", getattr(self, "_ssl_method", None)),
             fixBrokenPeers=True,
             acceptableCiphers=self.tls_ciphers,
         )
 
     # kept for old-style HTTP/1.0 downloader context twisted calls,
     # e.g. connectSSL()
-    def getContext(self, hostname=None, port=None):
+    def getContext(self, hostname: Any = None, port: Any = None) -> SSL.Context:
         ctx = self.getCertificateOptions().getContext()
         ctx.set_options(0x4)  # OP_LEGACY_SERVER_CONNECT
         return ctx
 
-    def creatorForNetloc(self, hostname, port):
+    def creatorForNetloc(self, hostname: bytes, port: int) -> "ClientTLSOptions":
         return ScrapyClientTLSOptions(
             hostname.decode("ascii"),
             self.getContext(),
             verbose_logging=self.tls_verbose_logging,
         )
 
 
@@ -110,15 +124,15 @@
     :class:`~twisted.web.client.BrowserLikePolicyForHTTPS` except this context
     factory allows setting the TLS/SSL method to use.
 
     The default OpenSSL method is ``TLS_METHOD`` (also called
     ``SSLv23_METHOD``) which allows TLS protocol negotiation.
     """
 
-    def creatorForNetloc(self, hostname, port):
+    def creatorForNetloc(self, hostname: bytes, port: int) -> "ClientTLSOptions":
         # trustRoot set to platformTrust() will use the platform's root CAs.
         #
         # This means that a website like https://www.cacert.org will be rejected
         # by default, since CAcert.org CA certificate is seldom shipped.
         return optionsForClientTLS(
             hostname=hostname.decode("ascii"),
             trustRoot=platformTrust(),
@@ -129,21 +143,23 @@
 @implementer(IPolicyForHTTPS)
 class AcceptableProtocolsContextFactory:
     """Context factory to used to override the acceptable protocols
     to set up the [OpenSSL.SSL.Context] for doing NPN and/or ALPN
     negotiation.
     """
 
-    def __init__(self, context_factory, acceptable_protocols):
+    def __init__(self, context_factory: Any, acceptable_protocols: List[bytes]):
         verifyObject(IPolicyForHTTPS, context_factory)
-        self._wrapped_context_factory = context_factory
-        self._acceptable_protocols = acceptable_protocols
+        self._wrapped_context_factory: Any = context_factory
+        self._acceptable_protocols: List[bytes] = acceptable_protocols
 
-    def creatorForNetloc(self, hostname, port):
-        options = self._wrapped_context_factory.creatorForNetloc(hostname, port)
+    def creatorForNetloc(self, hostname: bytes, port: int) -> "ClientTLSOptions":
+        options: "ClientTLSOptions" = self._wrapped_context_factory.creatorForNetloc(
+            hostname, port
+        )
         _setAcceptableProtocols(options._ctx, self._acceptable_protocols)
         return options
 
 
 def load_context_factory_from_settings(settings, crawler):
     ssl_method = openssl_methods[settings.get("DOWNLOADER_CLIENT_TLS_METHOD")]
     context_factory_cls = load_object(settings["DOWNLOADER_CLIENTCONTEXTFACTORY"])
```

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/handlers/__init__.py` & `Scrapy-2.9.0/scrapy/http/headers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,102 @@
-"""Download handlers for different schemes"""
+from collections.abc import Mapping
 
-import logging
+from w3lib.http import headers_dict_to_raw
 
-from twisted.internet import defer
+from scrapy.utils.datatypes import CaselessDict
+from scrapy.utils.python import to_unicode
 
-from scrapy import signals
-from scrapy.exceptions import NotConfigured, NotSupported
-from scrapy.utils.httpobj import urlparse_cached
-from scrapy.utils.misc import create_instance, load_object
-from scrapy.utils.python import without_none_values
 
-logger = logging.getLogger(__name__)
+class Headers(CaselessDict):
+    """Case insensitive http headers dictionary"""
+
+    def __init__(self, seq=None, encoding="utf-8"):
+        self.encoding = encoding
+        super().__init__(seq)
+
+    def update(self, seq):
+        seq = seq.items() if isinstance(seq, Mapping) else seq
+        iseq = {}
+        for k, v in seq:
+            iseq.setdefault(self.normkey(k), []).extend(self.normvalue(v))
+        super().update(iseq)
+
+    def normkey(self, key):
+        """Normalize key to bytes"""
+        return self._tobytes(key.title())
+
+    def normvalue(self, value):
+        """Normalize values to bytes"""
+        if value is None:
+            value = []
+        elif isinstance(value, (str, bytes)):
+            value = [value]
+        elif not hasattr(value, "__iter__"):
+            value = [value]
+
+        return [self._tobytes(x) for x in value]
+
+    def _tobytes(self, x):
+        if isinstance(x, bytes):
+            return x
+        if isinstance(x, str):
+            return x.encode(self.encoding)
+        if isinstance(x, int):
+            return str(x).encode(self.encoding)
+        raise TypeError(f"Unsupported value type: {type(x)}")
 
-
-class DownloadHandlers:
-    def __init__(self, crawler):
-        self._crawler = crawler
-        self._schemes = {}  # stores acceptable schemes on instancing
-        self._handlers = {}  # stores instanced handlers for schemes
-        self._notconfigured = {}  # remembers failed handlers
-        handlers = without_none_values(
-            crawler.settings.getwithbase("DOWNLOAD_HANDLERS")
-        )
-        for scheme, clspath in handlers.items():
-            self._schemes[scheme] = clspath
-            self._load_handler(scheme, skip_lazy=True)
-
-        crawler.signals.connect(self._close, signals.engine_stopped)
-
-    def _get_handler(self, scheme):
-        """Lazy-load the downloadhandler for a scheme
-        only on the first request for that scheme.
-        """
-        if scheme in self._handlers:
-            return self._handlers[scheme]
-        if scheme in self._notconfigured:
-            return None
-        if scheme not in self._schemes:
-            self._notconfigured[scheme] = "no handler available for that scheme"
+    def __getitem__(self, key):
+        try:
+            return super().__getitem__(key)[-1]
+        except IndexError:
             return None
 
-        return self._load_handler(scheme)
-
-    def _load_handler(self, scheme, skip_lazy=False):
-        path = self._schemes[scheme]
+    def get(self, key, def_val=None):
         try:
-            dhcls = load_object(path)
-            if skip_lazy and getattr(dhcls, "lazy", True):
-                return None
-            dh = create_instance(
-                objcls=dhcls,
-                settings=self._crawler.settings,
-                crawler=self._crawler,
-            )
-        except NotConfigured as ex:
-            self._notconfigured[scheme] = str(ex)
+            return super().get(key, def_val)[-1]
+        except IndexError:
             return None
-        except Exception as ex:
-            logger.error(
-                'Loading "%(clspath)s" for scheme "%(scheme)s"',
-                {"clspath": path, "scheme": scheme},
-                exc_info=True,
-                extra={"crawler": self._crawler},
-            )
-            self._notconfigured[scheme] = str(ex)
-            return None
-        else:
-            self._handlers[scheme] = dh
-            return dh
-
-    def download_request(self, request, spider):
-        scheme = urlparse_cached(request).scheme
-        handler = self._get_handler(scheme)
-        if not handler:
-            raise NotSupported(
-                f"Unsupported URL scheme '{scheme}': {self._notconfigured[scheme]}"
+
+    def getlist(self, key, def_val=None):
+        try:
+            return super().__getitem__(key)
+        except KeyError:
+            if def_val is not None:
+                return self.normvalue(def_val)
+            return []
+
+    def setlist(self, key, list_):
+        self[key] = list_
+
+    def setlistdefault(self, key, default_list=()):
+        return self.setdefault(key, default_list)
+
+    def appendlist(self, key, value):
+        lst = self.getlist(key)
+        lst.extend(self.normvalue(value))
+        self[key] = lst
+
+    def items(self):
+        return ((k, self.getlist(k)) for k in self.keys())
+
+    def values(self):
+        return [self[k] for k in self.keys()]
+
+    def to_string(self):
+        return headers_dict_to_raw(self)
+
+    def to_unicode_dict(self):
+        """Return headers as a CaselessDict with unicode keys
+        and unicode values. Multiple values are joined with ','.
+        """
+        return CaselessDict(
+            (
+                to_unicode(key, encoding=self.encoding),
+                to_unicode(b",".join(value), encoding=self.encoding),
             )
-        return handler.download_request(request, spider)
+            for key, value in self.items()
+        )
+
+    def __copy__(self):
+        return self.__class__(self)
 
-    @defer.inlineCallbacks
-    def _close(self, *_a, **_kw):
-        for dh in self._handlers.values():
-            if hasattr(dh, "close"):
-                yield dh.close()
+    copy = __copy__
```

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/handlers/datauri.py` & `Scrapy-2.9.0/scrapy/core/downloader/handlers/datauri.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/handlers/ftp.py` & `Scrapy-2.9.0/scrapy/core/downloader/handlers/ftp.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/handlers/http10.py` & `Scrapy-2.9.0/scrapy/core/downloader/handlers/http10.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/handlers/http11.py` & `Scrapy-2.9.0/scrapy/core/downloader/handlers/http11.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,14 @@
             headers=headers,
             bodyProducer=bodyProducer,
             requestPath=uri,
         )
 
 
 class ScrapyAgent:
-
     _Agent = Agent
     _ProxyAgent = ScrapyProxyAgent
     _TunnelingAgent = TunnelingAgent
 
     def __init__(
         self,
         contextFactory=None,
```

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/handlers/http2.py` & `Scrapy-2.9.0/scrapy/core/downloader/handlers/http2.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/handlers/s3.py` & `Scrapy-2.9.0/scrapy/core/downloader/handlers/s3.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/middleware.py` & `Scrapy-2.9.0/scrapy/core/downloader/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
 Downloader Middleware manager
 
 See documentation in docs/topics/downloader-middleware.rst
 """
-from typing import Callable, Union, cast
+from typing import Any, Callable, Generator, List, Union, cast
 
-from twisted.internet import defer
+from twisted.internet.defer import Deferred, inlineCallbacks
 from twisted.python.failure import Failure
 
 from scrapy import Spider
 from scrapy.exceptions import _InvalidOutput
 from scrapy.http import Request, Response
 from scrapy.middleware import MiddlewareManager
+from scrapy.settings import BaseSettings
 from scrapy.utils.conf import build_component_list
 from scrapy.utils.defer import deferred_from_coro, mustbe_deferred
 
 
 class DownloaderMiddlewareManager(MiddlewareManager):
-
     component_name = "downloader middleware"
 
     @classmethod
-    def _get_mwlist_from_settings(cls, settings):
+    def _get_mwlist_from_settings(cls, settings: BaseSettings) -> List[Any]:
         return build_component_list(settings.getwithbase("DOWNLOADER_MIDDLEWARES"))
 
-    def _add_middleware(self, mw):
+    def _add_middleware(self, mw: Any) -> None:
         if hasattr(mw, "process_request"):
             self.methods["process_request"].append(mw.process_request)
         if hasattr(mw, "process_response"):
             self.methods["process_response"].appendleft(mw.process_response)
         if hasattr(mw, "process_exception"):
             self.methods["process_exception"].appendleft(mw.process_exception)
 
-    def download(self, download_func: Callable, request: Request, spider: Spider):
-        @defer.inlineCallbacks
-        def process_request(request: Request):
+    def download(
+        self, download_func: Callable, request: Request, spider: Spider
+    ) -> Deferred:
+        @inlineCallbacks
+        def process_request(request: Request) -> Generator[Deferred, Any, Any]:
             for method in self.methods["process_request"]:
                 method = cast(Callable, method)
                 response = yield deferred_from_coro(
                     method(request=request, spider=spider)
                 )
                 if response is not None and not isinstance(
                     response, (Response, Request)
@@ -47,16 +49,18 @@
                         f"Middleware {method.__qualname__} must return None, Response or "
                         f"Request, got {response.__class__.__name__}"
                     )
                 if response:
                     return response
             return (yield download_func(request=request, spider=spider))
 
-        @defer.inlineCallbacks
-        def process_response(response: Union[Response, Request]):
+        @inlineCallbacks
+        def process_response(
+            response: Union[Response, Request]
+        ) -> Generator[Deferred, Any, Union[Response, Request]]:
             if response is None:
                 raise TypeError("Received None in process_response")
             elif isinstance(response, Request):
                 return response
 
             for method in self.methods["process_response"]:
                 method = cast(Callable, method)
@@ -68,16 +72,18 @@
                         f"Middleware {method.__qualname__} must return Response or Request, "
                         f"got {type(response)}"
                     )
                 if isinstance(response, Request):
                     return response
             return response
 
-        @defer.inlineCallbacks
-        def process_exception(failure: Failure):
+        @inlineCallbacks
+        def process_exception(
+            failure: Failure,
+        ) -> Generator[Deferred, Any, Union[Failure, Response, Request]]:
             exception = failure.value
             for method in self.methods["process_exception"]:
                 method = cast(Callable, method)
                 response = yield deferred_from_coro(
                     method(request=request, exception=exception, spider=spider)
                 )
                 if response is not None and not isinstance(
```

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/tls.py` & `Scrapy-2.9.0/scrapy/core/downloader/tls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import Any, Dict
 
 from OpenSSL import SSL
 from service_identity.exceptions import CertificateError
 from twisted.internet._sslverify import (
     ClientTLSOptions,
     VerificationError,
     verifyHostname,
@@ -16,15 +17,15 @@
 
 METHOD_TLS = "TLS"
 METHOD_TLSv10 = "TLSv1.0"
 METHOD_TLSv11 = "TLSv1.1"
 METHOD_TLSv12 = "TLSv1.2"
 
 
-openssl_methods = {
+openssl_methods: Dict[str, int] = {
     METHOD_TLS: SSL.SSLv23_METHOD,  # protocol negotiation (recommended)
     METHOD_TLSv10: SSL.TLSv1_METHOD,  # TLS 1.0 only
     METHOD_TLSv11: SSL.TLSv1_1_METHOD,  # TLS 1.1 only
     METHOD_TLSv12: SSL.TLSv1_2_METHOD,  # TLS 1.2 only
 }
 
 
@@ -35,35 +36,38 @@
 
     Same as Twisted's private _sslverify.ClientTLSOptions,
     except that VerificationError, CertificateError and ValueError
     exceptions are caught, so that the connection is not closed, only
     logging warnings. Also, HTTPS connection parameters logging is added.
     """
 
-    def __init__(self, hostname, ctx, verbose_logging=False):
+    def __init__(self, hostname: str, ctx: SSL.Context, verbose_logging: bool = False):
         super().__init__(hostname, ctx)
-        self.verbose_logging = verbose_logging
+        self.verbose_logging: bool = verbose_logging
 
-    def _identityVerifyingInfoCallback(self, connection, where, ret):
+    def _identityVerifyingInfoCallback(
+        self, connection: SSL.Connection, where: int, ret: Any
+    ) -> None:
         if where & SSL.SSL_CB_HANDSHAKE_START:
             connection.set_tlsext_host_name(self._hostnameBytes)
         elif where & SSL.SSL_CB_HANDSHAKE_DONE:
             if self.verbose_logging:
                 logger.debug(
                     "SSL connection to %s using protocol %s, cipher %s",
                     self._hostnameASCII,
                     connection.get_protocol_version_name(),
                     connection.get_cipher_name(),
                 )
                 server_cert = connection.get_peer_certificate()
-                logger.debug(
-                    'SSL connection certificate: issuer "%s", subject "%s"',
-                    x509name_to_string(server_cert.get_issuer()),
-                    x509name_to_string(server_cert.get_subject()),
-                )
+                if server_cert:
+                    logger.debug(
+                        'SSL connection certificate: issuer "%s", subject "%s"',
+                        x509name_to_string(server_cert.get_issuer()),
+                        x509name_to_string(server_cert.get_subject()),
+                    )
                 key_info = get_temp_key_info(connection._ssl)
                 if key_info:
                     logger.debug("SSL temp key: %s", key_info)
 
             try:
                 verifyHostname(connection, self._hostnameASCII)
             except (CertificateError, VerificationError) as e:
@@ -78,8 +82,10 @@
                     "Ignoring error while verifying certificate "
                     'from host "%s" (exception: %r)',
                     self._hostnameASCII,
                     e,
                 )
 
 
-DEFAULT_CIPHERS = AcceptableCiphers.fromOpenSSLCipherString("DEFAULT")
+DEFAULT_CIPHERS: AcceptableCiphers = AcceptableCiphers.fromOpenSSLCipherString(
+    "DEFAULT"
+)
```

### Comparing `Scrapy-2.8.0/scrapy/core/downloader/webclient.py` & `Scrapy-2.9.0/scrapy/core/downloader/webclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import re
 from time import time
-from urllib.parse import urldefrag, urlparse, urlunparse
+from typing import Optional, Tuple
+from urllib.parse import ParseResult, urldefrag, urlparse, urlunparse
 
 from twisted.internet import defer
 from twisted.internet.protocol import ClientFactory
 from twisted.web.http import HTTPClient
 
+from scrapy import Request
 from scrapy.http import Headers
 from scrapy.responsetypes import responsetypes
 from scrapy.utils.httpobj import urlparse_cached
 from scrapy.utils.python import to_bytes, to_unicode
 
 
-def _parsed_url_args(parsed):
+def _parsed_url_args(parsed: ParseResult) -> Tuple[bytes, bytes, bytes, int, bytes]:
     # Assume parsed is urlparse-d from Request.url,
     # which was passed via safe_url_string and is ascii-only.
-    path = urlunparse(("", "", parsed.path or "/", parsed.params, parsed.query, ""))
-    path = to_bytes(path, encoding="ascii")
+    path_str = urlunparse(("", "", parsed.path or "/", parsed.params, parsed.query, ""))
+    path = to_bytes(path_str, encoding="ascii")
+    assert parsed.hostname is not None
     host = to_bytes(parsed.hostname, encoding="ascii")
     port = parsed.port
     scheme = to_bytes(parsed.scheme, encoding="ascii")
     netloc = to_bytes(parsed.netloc, encoding="ascii")
     if port is None:
         port = 443 if scheme == b"https" else 80
     return scheme, netloc, host, port, path
 
 
-def _parse(url):
+def _parse(url: str) -> Tuple[bytes, bytes, bytes, int, bytes]:
     """Return tuple of (scheme, netloc, host, port, path),
     all in bytes except for port which is int.
     Assume url is from Request.url, which was passed via safe_url_string
     and is ascii-only.
     """
     url = url.strip()
     if not re.match(r"^\w+://", url):
         url = "//" + url
     parsed = urlparse(url)
     return _parsed_url_args(parsed)
 
 
 class ScrapyHTTPPageGetter(HTTPClient):
-
     delimiter = b"\n"
 
     def connectionMade(self):
         self.headers = Headers()  # bucket for response headers
 
         # Method command
         self.sendCommand(self.factory.method, self.factory.path)
@@ -99,15 +101,14 @@
 
 
 # This class used to inherit from Twisted’s
 # twisted.web.client.HTTPClientFactory. When that class was deprecated in
 # Twisted (https://github.com/twisted/twisted/pull/643), we merged its
 # non-overridden code into this class.
 class ScrapyHTTPClientFactory(ClientFactory):
-
     protocol = ScrapyHTTPPageGetter
 
     waiting = 1
     noisy = False
     followRedirect = False
     afterFoundGet = False
 
@@ -130,33 +131,35 @@
             parsed
         )
         proxy = request.meta.get("proxy")
         if proxy:
             self.scheme, _, self.host, self.port, _ = _parse(proxy)
             self.path = self.url
 
-    def __init__(self, request, timeout=180):
-        self._url = urldefrag(request.url)[0]
+    def __init__(self, request: Request, timeout: float = 180):
+        self._url: str = urldefrag(request.url)[0]
         # converting to bytes to comply to Twisted interface
-        self.url = to_bytes(self._url, encoding="ascii")
-        self.method = to_bytes(request.method, encoding="ascii")
-        self.body = request.body or None
-        self.headers = Headers(request.headers)
-        self.response_headers = None
-        self.timeout = request.meta.get("download_timeout") or timeout
-        self.start_time = time()
-        self.deferred = defer.Deferred().addCallback(self._build_response, request)
+        self.url: bytes = to_bytes(self._url, encoding="ascii")
+        self.method: bytes = to_bytes(request.method, encoding="ascii")
+        self.body: Optional[bytes] = request.body or None
+        self.headers: Headers = Headers(request.headers)
+        self.response_headers: Optional[Headers] = None
+        self.timeout: float = request.meta.get("download_timeout") or timeout
+        self.start_time: float = time()
+        self.deferred: defer.Deferred = defer.Deferred().addCallback(
+            self._build_response, request
+        )
 
         # Fixes Twisted 11.1.0+ support as HTTPClientFactory is expected
         # to have _disconnectedDeferred. See Twisted r32329.
         # As Scrapy implements it's own logic to handle redirects is not
         # needed to add the callback _waitForDisconnect.
         # Specifically this avoids the AttributeError exception when
         # clientConnectionFailed method is called.
-        self._disconnectedDeferred = defer.Deferred()
+        self._disconnectedDeferred: defer.Deferred = defer.Deferred()
 
         self._set_connection_attributes(request)
 
         # set Host header based on url
         self.headers.setdefault("Host", self.netloc)
 
         # set Content-Length based len of body
@@ -164,16 +167,16 @@
             self.headers["Content-Length"] = len(self.body)
             # just in case a broken http/1.1 decides to keep connection alive
             self.headers.setdefault("Connection", "close")
         # Content-Length must be specified in POST method even with no body
         elif self.method == b"POST":
             self.headers["Content-Length"] = 0
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__}: {self.url}>"
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}: {self._url}>"
 
     def _cancelTimeout(self, result, timeoutCall):
         if timeoutCall.active():
             timeoutCall.cancel()
         return result
 
     def buildProtocol(self, addr):
```

### Comparing `Scrapy-2.8.0/scrapy/core/engine.py` & `Scrapy-2.9.0/scrapy/core/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,48 +3,68 @@
 
 For more information see docs/topics/architecture.rst
 
 """
 import logging
 import warnings
 from time import time
-from typing import Callable, Iterable, Iterator, Optional, Set, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generator,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Set,
+    Type,
+    Union,
+    cast,
+)
 
 from twisted.internet.defer import Deferred, inlineCallbacks, succeed
 from twisted.internet.task import LoopingCall
 from twisted.python.failure import Failure
 
 from scrapy import signals
+from scrapy.core.downloader import Downloader
 from scrapy.core.scraper import Scraper
 from scrapy.exceptions import CloseSpider, DontCloseSpider, ScrapyDeprecationWarning
 from scrapy.http import Request, Response
-from scrapy.settings import BaseSettings
+from scrapy.logformatter import LogFormatter
+from scrapy.settings import BaseSettings, Settings
+from scrapy.signalmanager import SignalManager
 from scrapy.spiders import Spider
 from scrapy.utils.log import failure_to_exc_info, logformatter_adapter
 from scrapy.utils.misc import create_instance, load_object
 from scrapy.utils.reactor import CallLaterOnce
 
+if TYPE_CHECKING:
+    from scrapy.core.scheduler import BaseScheduler
+    from scrapy.crawler import Crawler
+
 logger = logging.getLogger(__name__)
 
 
 class Slot:
     def __init__(
         self,
-        start_requests: Iterable,
+        start_requests: Iterable[Request],
         close_if_idle: bool,
         nextcall: CallLaterOnce,
-        scheduler,
+        scheduler: "BaseScheduler",
     ) -> None:
         self.closing: Optional[Deferred] = None
         self.inprogress: Set[Request] = set()
-        self.start_requests: Optional[Iterator] = iter(start_requests)
-        self.close_if_idle = close_if_idle
-        self.nextcall = nextcall
-        self.scheduler = scheduler
-        self.heartbeat = LoopingCall(nextcall.schedule)
+        self.start_requests: Optional[Iterator[Request]] = iter(start_requests)
+        self.close_if_idle: bool = close_if_idle
+        self.nextcall: CallLaterOnce = nextcall
+        self.scheduler: "BaseScheduler" = scheduler
+        self.heartbeat: LoopingCall = LoopingCall(nextcall.schedule)
 
     def add_request(self, request: Request) -> None:
         self.inprogress.add(request)
 
     def remove_request(self, request: Request) -> None:
         self.inprogress.remove(request)
         self._maybe_fire_closing()
@@ -60,55 +80,58 @@
                 self.nextcall.cancel()
                 if self.heartbeat.running:
                     self.heartbeat.stop()
             self.closing.callback(None)
 
 
 class ExecutionEngine:
-    def __init__(self, crawler, spider_closed_callback: Callable) -> None:
-        self.crawler = crawler
-        self.settings = crawler.settings
-        self.signals = crawler.signals
-        self.logformatter = crawler.logformatter
+    def __init__(self, crawler: "Crawler", spider_closed_callback: Callable) -> None:
+        self.crawler: "Crawler" = crawler
+        self.settings: Settings = crawler.settings
+        self.signals: SignalManager = crawler.signals
+        self.logformatter: LogFormatter = crawler.logformatter
         self.slot: Optional[Slot] = None
         self.spider: Optional[Spider] = None
-        self.running = False
-        self.paused = False
-        self.scheduler_cls = self._get_scheduler_class(crawler.settings)
-        downloader_cls = load_object(self.settings["DOWNLOADER"])
-        self.downloader = downloader_cls(crawler)
+        self.running: bool = False
+        self.paused: bool = False
+        self.scheduler_cls: Type["BaseScheduler"] = self._get_scheduler_class(
+            crawler.settings
+        )
+        downloader_cls: Type[Downloader] = load_object(self.settings["DOWNLOADER"])
+        self.downloader: Downloader = downloader_cls(crawler)
         self.scraper = Scraper(crawler)
-        self._spider_closed_callback = spider_closed_callback
+        self._spider_closed_callback: Callable = spider_closed_callback
+        self.start_time: Optional[float] = None
 
-    def _get_scheduler_class(self, settings: BaseSettings) -> type:
+    def _get_scheduler_class(self, settings: BaseSettings) -> Type["BaseScheduler"]:
         from scrapy.core.scheduler import BaseScheduler
 
-        scheduler_cls = load_object(settings["SCHEDULER"])
+        scheduler_cls: Type = load_object(settings["SCHEDULER"])
         if not issubclass(scheduler_cls, BaseScheduler):
             raise TypeError(
                 f"The provided scheduler class ({settings['SCHEDULER']})"
                 " does not fully implement the scheduler interface"
             )
         return scheduler_cls
 
     @inlineCallbacks
-    def start(self) -> Deferred:
+    def start(self) -> Generator[Deferred, Any, None]:
         if self.running:
             raise RuntimeError("Engine already running")
         self.start_time = time()
         yield self.signals.send_catch_log_deferred(signal=signals.engine_started)
         self.running = True
-        self._closewait = Deferred()
+        self._closewait: Deferred = Deferred()
         yield self._closewait
 
     def stop(self) -> Deferred:
         """Gracefully stop the execution engine"""
 
         @inlineCallbacks
-        def _finish_stopping_engine(_) -> Deferred:
+        def _finish_stopping_engine(_: Any) -> Generator[Deferred, Any, None]:
             yield self.signals.send_catch_log_deferred(signal=signals.engine_stopped)
             self._closewait.callback(None)
 
         if not self.running:
             raise RuntimeError("Engine not running")
 
         self.running = False
@@ -126,15 +149,16 @@
         """
         if self.running:
             return self.stop()  # will also close spider and downloader
         if self.spider is not None:
             return self.close_spider(
                 self.spider, reason="shutdown"
             )  # will also close downloader
-        return succeed(self.downloader.close())
+        self.downloader.close()
+        return succeed(None)
 
     def pause(self) -> None:
         self.paused = True
 
     def unpause(self) -> None:
         self.paused = False
 
@@ -168,19 +192,21 @@
             else:
                 self.crawl(request)
 
         if self.spider_is_idle() and self.slot.close_if_idle:
             self._spider_idle()
 
     def _needs_backout(self) -> bool:
+        assert self.slot is not None  # typing
+        assert self.scraper.slot is not None  # typing
         return (
             not self.running
-            or self.slot.closing  # type: ignore[union-attr]
+            or bool(self.slot.closing)
             or self.downloader.needs_backout()
-            or self.scraper.slot.needs_backout()  # type: ignore[union-attr]
+            or self.scraper.slot.needs_backout()
         )
 
     def _next_request_from_scheduler(self) -> Optional[Deferred]:
         assert self.slot is not None  # typing
         assert self.spider is not None  # typing
 
         request = self.slot.scheduler.next_request()
@@ -192,15 +218,15 @@
         d.addErrback(
             lambda f: logger.info(
                 "Error while handling downloader output",
                 exc_info=failure_to_exc_info(f),
                 extra={"spider": self.spider},
             )
         )
-        d.addBoth(lambda _: self.slot.remove_request(request))
+        d.addBoth(lambda _: cast(Slot, self.slot).remove_request(request))  # type: ignore[arg-type]
         d.addErrback(
             lambda f: logger.info(
                 "Error while removing request from slot",
                 exc_info=failure_to_exc_info(f),
                 extra={"spider": self.spider},
             )
         )
@@ -322,38 +348,41 @@
             if not isinstance(result, (Response, Request)):
                 raise TypeError(
                     f"Incorrect type: expected Response or Request, got {type(result)}: {result!r}"
                 )
             if isinstance(result, Response):
                 if result.request is None:
                     result.request = request
+                assert spider is not None
                 logkws = self.logformatter.crawled(result.request, result, spider)
                 if logkws is not None:
                     logger.log(*logformatter_adapter(logkws), extra={"spider": spider})
                 self.signals.send_catch_log(
                     signal=signals.response_received,
                     response=result,
                     request=result.request,
                     spider=spider,
                 )
             return result
 
-        def _on_complete(_):
+        def _on_complete(_: Any) -> Any:
+            assert self.slot is not None
             self.slot.nextcall.schedule()
             return _
 
+        assert spider is not None
         dwld = self.downloader.fetch(request, spider)
         dwld.addCallbacks(_on_success)
         dwld.addBoth(_on_complete)
         return dwld
 
     @inlineCallbacks
     def open_spider(
         self, spider: Spider, start_requests: Iterable = (), close_if_idle: bool = True
-    ):
+    ) -> Generator[Deferred, Any, None]:
         if self.slot is not None:
             raise RuntimeError(f"No free spider slot when opening {spider.name!r}")
         logger.info("Spider opened", extra={"spider": spider})
         nextcall = CallLaterOnce(self._next_request)
         scheduler = create_instance(
             self.scheduler_cls, settings=None, crawler=self.crawler
         )
@@ -420,15 +449,15 @@
         dfd.addBoth(lambda _: self.downloader.close())
         dfd.addErrback(log_failure("Downloader close failure"))
 
         dfd.addBoth(lambda _: self.scraper.close_spider(spider))
         dfd.addErrback(log_failure("Scraper close failure"))
 
         if hasattr(self.slot.scheduler, "close"):
-            dfd.addBoth(lambda _: self.slot.scheduler.close(reason))
+            dfd.addBoth(lambda _: cast(Slot, self.slot).scheduler.close(reason))
             dfd.addErrback(log_failure("Scheduler close failure"))
 
         dfd.addBoth(
             lambda _: self.signals.send_catch_log_deferred(
                 signal=signals.spider_closed,
                 spider=spider,
                 reason=reason,
@@ -454,15 +483,15 @@
         dfd.addErrback(log_failure("Error while unassigning spider"))
 
         dfd.addBoth(lambda _: self._spider_closed_callback(spider))
 
         return dfd
 
     @property
-    def open_spiders(self) -> list:
+    def open_spiders(self) -> List[Spider]:
         warnings.warn(
             "ExecutionEngine.open_spiders is deprecated, please use ExecutionEngine.spider instead",
             category=ScrapyDeprecationWarning,
             stacklevel=2,
         )
         return [self.spider] if self.spider is not None else []
```

### Comparing `Scrapy-2.8.0/scrapy/core/http2/agent.py` & `Scrapy-2.9.0/scrapy/core/http2/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 from typing import Deque, Dict, List, Optional, Tuple
 
 from twisted.internet import defer
 from twisted.internet.base import ReactorBase
 from twisted.internet.defer import Deferred
 from twisted.internet.endpoints import HostnameEndpoint
 from twisted.python.failure import Failure
-from twisted.web.client import URI, BrowserLikePolicyForHTTPS, _StandardEndpointFactory
+from twisted.web.client import (
+    URI,
+    BrowserLikePolicyForHTTPS,
+    ResponseFailed,
+    _StandardEndpointFactory,
+)
 from twisted.web.error import SchemeNotSupported
 
 from scrapy.core.downloader.contextfactory import AcceptableProtocolsContextFactory
 from scrapy.core.http2.protocol import H2ClientFactory, H2ClientProtocol
 from scrapy.http.request import Request
 from scrapy.settings import Settings
 from scrapy.spiders import Spider
@@ -31,15 +36,15 @@
     def get_connection(
         self, key: Tuple, uri: URI, endpoint: HostnameEndpoint
     ) -> Deferred:
         if key in self._pending_requests:
             # Received a request while connecting to remote
             # Create a deferred which will fire with the H2ClientProtocol
             # instance
-            d = Deferred()
+            d: Deferred = Deferred()
             self._pending_requests[key].append(d)
             return d
 
         # Check if we already have a connection to the remote
         conn = self._connections.get(key, None)
         if conn:
             # Return this connection instance wrapped inside a deferred
@@ -49,22 +54,22 @@
         return self._new_connection(key, uri, endpoint)
 
     def _new_connection(
         self, key: Tuple, uri: URI, endpoint: HostnameEndpoint
     ) -> Deferred:
         self._pending_requests[key] = deque()
 
-        conn_lost_deferred = Deferred()
+        conn_lost_deferred: Deferred = Deferred()
         conn_lost_deferred.addCallback(self._remove_connection, key)
 
         factory = H2ClientFactory(uri, self.settings, conn_lost_deferred)
         conn_d = endpoint.connect(factory)
         conn_d.addCallback(self.put_connection, key)
 
-        d = Deferred()
+        d: Deferred = Deferred()
         self._pending_requests[key].append(d)
         return d
 
     def put_connection(self, conn: H2ClientProtocol, key: Tuple) -> H2ClientProtocol:
         self._connections[key] = conn
 
         # Now as we have established a proper HTTP/2 connection
@@ -79,23 +84,24 @@
     def _remove_connection(self, errors: List[BaseException], key: Tuple) -> None:
         self._connections.pop(key)
 
         # Call the errback of all the pending requests for this connection
         pending_requests = self._pending_requests.pop(key, None)
         while pending_requests:
             d = pending_requests.popleft()
-            d.errback(errors)
+            d.errback(ResponseFailed(errors))
 
     def close_connections(self) -> None:
         """Close all the HTTP/2 connections and remove them from pool
 
         Returns:
             Deferred that fires when all connections have been closed
         """
         for conn in self._connections.values():
+            assert conn.transport is not None  # typing
             conn.transport.abortConnection()
 
 
 class H2Agent:
     def __init__(
         self,
         reactor: ReactorBase,
```

### Comparing `Scrapy-2.8.0/scrapy/core/http2/protocol.py` & `Scrapy-2.9.0/scrapy/core/http2/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 
     @property
     def h2_connected(self) -> bool:
         """Boolean to keep track of the connection status.
         This is used while initiating pending streams to make sure
         that we initiate stream only during active HTTP/2 Connection
         """
+        assert self.transport is not None  # typing
         return bool(self.transport.connected) and self.metadata["settings_acknowledged"]
 
     @property
     def allowed_max_concurrent_streams(self) -> int:
         """We keep total two streams for client (sending data) and
         server side (receiving data) for a single request. To be safe
         we choose the minimum. Since this value can change in event
@@ -192,14 +193,15 @@
         self.streams[stream.stream_id] = stream
         return stream
 
     def _write_to_transport(self) -> None:
         """Write data to the underlying transport connection
         from the HTTP2 connection instance if any
         """
+        assert self.transport is not None  # typing
         # Reset the idle timeout as connection is still actively sending data
         self.resetTimeout()
 
         data = self.conn.data_to_send()
         self.transport.write(data)
 
     def request(self, request: Request, spider: Spider) -> Deferred:
@@ -222,31 +224,34 @@
     def connectionMade(self) -> None:
         """Called by Twisted when the connection is established. We can start
         sending some data now: we should open with the connection preamble.
         """
         # Initialize the timeout
         self.setTimeout(self.IDLE_TIMEOUT)
 
+        assert self.transport is not None  # typing
         destination = self.transport.getPeer()
         self.metadata["ip_address"] = ipaddress.ip_address(destination.host)
 
         # Initiate H2 Connection
         self.conn.initiate_connection()
         self._write_to_transport()
 
     def _lose_connection_with_error(self, errors: List[BaseException]) -> None:
         """Helper function to lose the connection with the error sent as a
         reason"""
         self._conn_lost_errors += errors
+        assert self.transport is not None  # typing
         self.transport.loseConnection()
 
     def handshakeCompleted(self) -> None:
         """
         Close the connection if it's not made via the expected protocol
         """
+        assert self.transport is not None  # typing
         if (
             self.transport.negotiatedProtocol is not None
             and self.transport.negotiatedProtocol != PROTOCOL_NAME
         ):
             # we have not initiated the connection yet, no need to send a GOAWAY frame to the remote peer
             self._lose_connection_with_error(
                 [InvalidNegotiatedProtocol(self.transport.negotiatedProtocol)]
@@ -271,14 +276,15 @@
             events = self.conn.receive_data(data)
             self._handle_events(events)
         except H2Error as e:
             if isinstance(e, FrameTooLargeError):
                 # hyper-h2 does not drop the connection in this scenario, we
                 # need to abort the connection manually.
                 self._conn_lost_errors += [e]
+                assert self.transport is not None  # typing
                 self.transport.abortConnection()
                 return
 
             # Save this error as ultimately the connection will be dropped
             # internally by hyper-h2. Saved error will be passed to all the streams
             # closed with the connection.
             self._lose_connection_with_error([e])
@@ -384,14 +390,15 @@
         self.metadata["settings_acknowledged"] = True
 
         # Send off all the pending requests as now we have
         # established a proper HTTP/2 connection
         self._send_pending_requests()
 
         # Update certificate when our HTTP/2 connection is established
+        assert self.transport is not None  # typing
         self.metadata["certificate"] = Certificate(self.transport.getPeerCertificate())
 
     def stream_ended(self, event: StreamEnded) -> None:
         try:
             stream = self.pop_stream(event.stream_id)
         except KeyError:
             pass  # We ignore server-initiated events
```

### Comparing `Scrapy-2.8.0/scrapy/core/http2/stream.py` & `Scrapy-2.9.0/scrapy/core/http2/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             # If the associated request is initiated we reset this stream
             # else we directly call close() method
             if self.metadata["request_sent"]:
                 self.reset_stream(StreamCloseReason.CANCELLED)
             else:
                 self.close(StreamCloseReason.CANCELLED)
 
-        self._deferred_response = Deferred(_cancel)
+        self._deferred_response: Deferred = Deferred(_cancel)
 
     def __repr__(self) -> str:
         return f"Stream(id={self.stream_id!r})"
 
     @property
     def _log_warnsize(self) -> bool:
         """Checks if we have received data which exceeds the download warnsize
```

### Comparing `Scrapy-2.8.0/scrapy/core/scheduler.py` & `Scrapy-2.9.0/scrapy/core/scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import json
 import logging
 from abc import abstractmethod
 from pathlib import Path
-from typing import Optional, Type, TypeVar
+from typing import Any, Optional, Type, TypeVar, cast
 
 from twisted.internet.defer import Deferred
 
 from scrapy.crawler import Crawler
+from scrapy.dupefilters import BaseDupeFilter
 from scrapy.http.request import Request
 from scrapy.spiders import Spider
+from scrapy.statscollectors import StatsCollector
 from scrapy.utils.job import job_dir
 from scrapy.utils.misc import create_instance, load_object
 
 logger = logging.getLogger(__name__)
 
 
 class BaseSchedulerMeta(type):
     """
     Metaclass to check scheduler classes against the necessary interface
     """
 
-    def __instancecheck__(cls, instance):
+    def __instancecheck__(cls, instance: Any) -> bool:
         return cls.__subclasscheck__(type(instance))
 
-    def __subclasscheck__(cls, subclass):
+    def __subclasscheck__(cls, subclass: type) -> bool:
         return (
             hasattr(subclass, "has_pending_requests")
             and callable(subclass.has_pending_requests)
             and hasattr(subclass, "enqueue_request")
             and callable(subclass.enqueue_request)
             and hasattr(subclass, "next_request")
             and callable(subclass.next_request)
@@ -164,34 +166,34 @@
 
     :param crawler: The crawler object corresponding to the current crawl.
     :type crawler: :class:`scrapy.crawler.Crawler`
     """
 
     def __init__(
         self,
-        dupefilter,
+        dupefilter: BaseDupeFilter,
         jobdir: Optional[str] = None,
         dqclass=None,
         mqclass=None,
         logunser: bool = False,
-        stats=None,
+        stats: Optional[StatsCollector] = None,
         pqclass=None,
         crawler: Optional[Crawler] = None,
     ):
-        self.df = dupefilter
-        self.dqdir = self._dqdir(jobdir)
+        self.df: BaseDupeFilter = dupefilter
+        self.dqdir: Optional[str] = self._dqdir(jobdir)
         self.pqclass = pqclass
         self.dqclass = dqclass
         self.mqclass = mqclass
-        self.logunser = logunser
-        self.stats = stats
-        self.crawler = crawler
+        self.logunser: bool = logunser
+        self.stats: Optional[StatsCollector] = stats
+        self.crawler: Optional[Crawler] = crawler
 
     @classmethod
-    def from_crawler(cls: Type[SchedulerTV], crawler) -> SchedulerTV:
+    def from_crawler(cls: Type[SchedulerTV], crawler: Crawler) -> SchedulerTV:
         """
         Factory method, initializes the scheduler with arguments taken from the crawl settings
         """
         dupefilter_cls = load_object(crawler.settings["DUPEFILTER_CLASS"])
         return cls(
             dupefilter=create_instance(dupefilter_cls, crawler.settings, crawler),
             jobdir=job_dir(crawler.settings),
@@ -238,14 +240,15 @@
 
         Return ``True`` if the request was stored successfully, ``False`` otherwise.
         """
         if not request.dont_filter and self.df.request_seen(request):
             self.df.log(request, self.spider)
             return False
         dqok = self._dqpush(request)
+        assert self.stats is not None
         if dqok:
             self.stats.inc_value("scheduler/enqueued/disk", spider=self.spider)
         else:
             self._mqpush(request)
             self.stats.inc_value("scheduler/enqueued/memory", spider=self.spider)
         self.stats.inc_value("scheduler/enqueued", spider=self.spider)
         return True
@@ -255,15 +258,16 @@
         Return a :class:`~scrapy.http.Request` object from the memory queue,
         falling back to the disk queue if the memory queue is empty.
         Return ``None`` if there are no more enqueued requests.
 
         Increment the appropriate stats, such as: ``scheduler/dequeued``,
         ``scheduler/dequeued/disk``, ``scheduler/dequeued/memory``.
         """
-        request = self.mqs.pop()
+        request: Optional[Request] = self.mqs.pop()
+        assert self.stats is not None
         if request is not None:
             self.stats.inc_value("scheduler/dequeued/memory", spider=self.spider)
         else:
             request = self._dqpop()
             if request is not None:
                 self.stats.inc_value("scheduler/dequeued/disk", spider=self.spider)
         if request is not None:
@@ -291,14 +295,15 @@
                 logger.warning(
                     msg,
                     {"request": request, "reason": e},
                     exc_info=True,
                     extra={"spider": self.spider},
                 )
                 self.logunser = False
+            assert self.stats is not None
             self.stats.inc_value("scheduler/unserializable", spider=self.spider)
             return False
         else:
             return True
 
     def _mqpush(self, request: Request) -> None:
         self.mqs.push(request)
@@ -347,12 +352,12 @@
         return None
 
     def _read_dqs_state(self, dqdir: str) -> list:
         path = Path(dqdir, "active.json")
         if not path.exists():
             return []
         with path.open(encoding="utf-8") as f:
-            return json.load(f)
+            return cast(list, json.load(f))
 
     def _write_dqs_state(self, dqdir: str, state: list) -> None:
         with Path(dqdir, "active.json").open("w", encoding="utf-8") as f:
             json.dump(state, f)
```

### Comparing `Scrapy-2.8.0/scrapy/core/scraper.py` & `Scrapy-2.9.0/scrapy/core/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,29 @@
     AsyncIterable,
     Deque,
     Generator,
     Iterable,
     Optional,
     Set,
     Tuple,
+    Type,
     Union,
 )
 
 from itemadapter import is_item
 from twisted.internet.defer import Deferred, inlineCallbacks
 from twisted.python.failure import Failure
 
 from scrapy import Spider, signals
 from scrapy.core.spidermw import SpiderMiddlewareManager
 from scrapy.exceptions import CloseSpider, DropItem, IgnoreRequest
 from scrapy.http import Request, Response
+from scrapy.logformatter import LogFormatter
+from scrapy.pipelines import ItemPipelineManager
+from scrapy.signalmanager import SignalManager
 from scrapy.utils.defer import (
     aiter_errback,
     defer_fail,
     defer_succeed,
     iter_errback,
     parallel,
     parallel_async,
@@ -60,15 +64,15 @@
         self.active_size: int = 0
         self.itemproc_size: int = 0
         self.closing: Optional[Deferred] = None
 
     def add_response_request(
         self, result: Union[Response, Failure], request: Request
     ) -> Deferred:
-        deferred = Deferred()
+        deferred: Deferred = Deferred()
         self.queue.append((result, request, deferred))
         if isinstance(result, Response):
             self.active_size += max(len(result.body), self.MIN_RESPONSE_SIZE)
         else:
             self.active_size += self.MIN_RESPONSE_SIZE
         return deferred
 
@@ -92,24 +96,28 @@
     def needs_backout(self) -> bool:
         return self.active_size > self.max_active_size
 
 
 class Scraper:
     def __init__(self, crawler: Crawler) -> None:
         self.slot: Optional[Slot] = None
-        self.spidermw = SpiderMiddlewareManager.from_crawler(crawler)
-        itemproc_cls = load_object(crawler.settings["ITEM_PROCESSOR"])
-        self.itemproc = itemproc_cls.from_crawler(crawler)
-        self.concurrent_items = crawler.settings.getint("CONCURRENT_ITEMS")
-        self.crawler = crawler
-        self.signals = crawler.signals
-        self.logformatter = crawler.logformatter
+        self.spidermw: SpiderMiddlewareManager = SpiderMiddlewareManager.from_crawler(
+            crawler
+        )
+        itemproc_cls: Type[ItemPipelineManager] = load_object(
+            crawler.settings["ITEM_PROCESSOR"]
+        )
+        self.itemproc: ItemPipelineManager = itemproc_cls.from_crawler(crawler)
+        self.concurrent_items: int = crawler.settings.getint("CONCURRENT_ITEMS")
+        self.crawler: Crawler = crawler
+        self.signals: SignalManager = crawler.signals
+        self.logformatter: LogFormatter = crawler.logformatter
 
     @inlineCallbacks
-    def open_spider(self, spider: Spider):
+    def open_spider(self, spider: Spider) -> Generator[Deferred, Any, None]:
         """Open the given spider for scraping and allocate resources for it"""
         self.slot = Slot(self.crawler.settings.getint("SCRAPER_SLOT_MAX_ACTIVE_SIZE"))
         yield self.itemproc.open_spider(spider)
 
     def close_spider(self, spider: Spider) -> Deferred:
         """Close a spider being scraped and release its resources"""
         if self.slot is None:
@@ -131,15 +139,16 @@
     def enqueue_scrape(
         self, result: Union[Response, Failure], request: Request, spider: Spider
     ) -> Deferred:
         if self.slot is None:
             raise RuntimeError("Scraper slot not assigned")
         dfd = self.slot.add_response_request(result, request)
 
-        def finish_scraping(_):
+        def finish_scraping(_: Any) -> Any:
+            assert self.slot is not None
             self.slot.finish_response(result, request)
             self._check_if_closing(spider)
             self._scrape_next(spider)
             return _
 
         dfd.addBoth(finish_scraping)
         dfd.addErrback(
@@ -199,18 +208,20 @@
             callback = result.request.callback or spider._parse
             warn_on_generator_with_return_value(spider, callback)
             dfd = defer_succeed(result)
             dfd.addCallbacks(
                 callback=callback, callbackKeywords=result.request.cb_kwargs
             )
         else:  # result is a Failure
-            result.request = request
-            warn_on_generator_with_return_value(spider, request.errback)
+            # TODO: properly type adding this attribute to a Failure
+            result.request = request  # type: ignore[attr-defined]
             dfd = defer_fail(result)
-            dfd.addErrback(request.errback)
+            if request.errback:
+                warn_on_generator_with_return_value(spider, request.errback)
+                dfd.addErrback(request.errback)
         return dfd.addCallback(iterate_spider_output)
 
     def handle_spider_error(
         self, _failure: Failure, request: Request, response: Response, spider: Spider
     ) -> None:
         exc = _failure.value
         if isinstance(exc, CloseSpider):
@@ -332,15 +343,15 @@
 
         if spider_failure is not download_failure:
             return spider_failure
         return None
 
     def _itemproc_finished(
         self, output: Any, item: Any, response: Response, spider: Spider
-    ) -> None:
+    ) -> Deferred:
         """ItemProcessor finished for the given ``item`` and returned ``output``"""
         assert self.slot is not None  # typing
         self.slot.itemproc_size -= 1
         if isinstance(output, Failure):
             ex = output.value
             if isinstance(ex, DropItem):
                 logkws = self.logformatter.dropped(item, ex, response, spider)
```

### Comparing `Scrapy-2.8.0/scrapy/core/spidermw.py` & `Scrapy-2.9.0/scrapy/core/spidermw.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 from typing import (
     Any,
     AsyncGenerator,
     AsyncIterable,
     Callable,
     Generator,
     Iterable,
+    List,
+    Optional,
     Tuple,
     Union,
     cast,
 )
 
 from twisted.internet.defer import Deferred, inlineCallbacks
 from twisted.python.failure import Failure
 
 from scrapy import Request, Spider
 from scrapy.exceptions import _InvalidOutput
 from scrapy.http import Response
 from scrapy.middleware import MiddlewareManager
+from scrapy.settings import BaseSettings
 from scrapy.utils.asyncgen import as_async_generator, collect_asyncgen
 from scrapy.utils.conf import build_component_list
 from scrapy.utils.defer import (
     deferred_f_from_coro_f,
     deferred_from_coro,
     maybe_deferred_to_future,
     mustbe_deferred,
@@ -37,31 +40,30 @@
 
 logger = logging.getLogger(__name__)
 
 
 ScrapeFunc = Callable[[Union[Response, Failure], Request, Spider], Any]
 
 
-def _isiterable(o) -> bool:
+def _isiterable(o: Any) -> bool:
     return isinstance(o, (Iterable, AsyncIterable))
 
 
 class SpiderMiddlewareManager(MiddlewareManager):
-
     component_name = "spider middleware"
 
-    def __init__(self, *middlewares):
+    def __init__(self, *middlewares: Any):
         super().__init__(*middlewares)
         self.downgrade_warning_done = False
 
     @classmethod
-    def _get_mwlist_from_settings(cls, settings):
+    def _get_mwlist_from_settings(cls, settings: BaseSettings) -> List[Any]:
         return build_component_list(settings.getwithbase("SPIDER_MIDDLEWARES"))
 
-    def _add_middleware(self, mw):
+    def _add_middleware(self, mw: Any) -> None:
         super()._add_middleware(mw)
         if hasattr(mw, "process_spider_input"):
             self.methods["process_spider_input"].append(mw.process_spider_input)
         if hasattr(mw, "process_start_requests"):
             self.methods["process_start_requests"].appendleft(mw.process_start_requests)
         process_spider_output = self._get_async_method_pair(mw, "process_spider_output")
         self.methods["process_spider_output"].appendleft(process_spider_output)
@@ -95,27 +97,27 @@
         self,
         response: Response,
         spider: Spider,
         iterable: Union[Iterable, AsyncIterable],
         exception_processor_index: int,
         recover_to: Union[MutableChain, MutableAsyncChain],
     ) -> Union[Generator, AsyncGenerator]:
-        def process_sync(iterable: Iterable):
+        def process_sync(iterable: Iterable) -> Generator:
             try:
                 for r in iterable:
                     yield r
             except Exception as ex:
                 exception_result = self._process_spider_exception(
                     response, spider, Failure(ex), exception_processor_index
                 )
                 if isinstance(exception_result, Failure):
                     raise
                 recover_to.extend(exception_result)
 
-        async def process_async(iterable: AsyncIterable):
+        async def process_async(iterable: AsyncIterable) -> AsyncGenerator:
             try:
                 async for r in iterable:
                     yield r
             except Exception as ex:
                 exception_result = self._process_spider_exception(
                     response, spider, Failure(ex), exception_processor_index
                 )
@@ -152,15 +154,15 @@
                 dfd: Deferred = self._process_spider_output(
                     response, spider, result, method_index + 1
                 )
                 # _process_spider_output() returns a Deferred only because of downgrading so this can be
                 # simplified when downgrading is removed.
                 if dfd.called:
                     # the result is available immediately if _process_spider_output didn't do downgrading
-                    return dfd.result
+                    return cast(MutableChain, dfd.result)
                 # we forbid waiting here because otherwise we would need to return a deferred from
                 # _process_spider_exception too, which complicates the architecture
                 msg = f"Async iterable returned from {method.__qualname__} cannot be downgraded"
                 raise _InvalidOutput(msg)
             elif result is None:
                 continue
             else:
@@ -177,15 +179,15 @@
     @inlineCallbacks
     def _process_spider_output(
         self,
         response: Response,
         spider: Spider,
         result: Union[Iterable, AsyncIterable],
         start_index: int = 0,
-    ) -> Deferred:
+    ) -> Generator[Deferred, Any, Union[MutableChain, MutableAsyncChain]]:
         # items in this iterable do not need to go through the process_spider_output
         # chain, they went through it already from the process_spider_exception method
         recovered: Union[MutableChain, MutableAsyncChain]
         last_result_is_async = isinstance(result, AsyncIterable)
         if last_result_is_async:
             recovered = MutableAsyncChain()
         else:
@@ -277,15 +279,15 @@
             self._process_spider_output(response, spider, result)
         )
         if isinstance(result, AsyncIterable):
             return MutableAsyncChain(result, recovered)
         if isinstance(recovered, AsyncIterable):
             recovered_collected = await collect_asyncgen(recovered)
             recovered = MutableChain(recovered_collected)
-        return MutableChain(result, recovered)  # type: ignore[arg-type]
+        return MutableChain(result, recovered)
 
     def scrape_response(
         self,
         scrape_func: ScrapeFunc,
         response: Response,
         request: Request,
         spider: Spider,
@@ -303,25 +305,27 @@
         )
         dfd.addCallbacks(
             callback=deferred_f_from_coro_f(process_callback_output),
             errback=process_spider_exception,
         )
         return dfd
 
-    def process_start_requests(self, start_requests, spider: Spider) -> Deferred:
+    def process_start_requests(
+        self, start_requests: Iterable[Request], spider: Spider
+    ) -> Deferred:
         return self._process_chain("process_start_requests", start_requests, spider)
 
     # This method is only needed until _async compatibility methods are removed.
     @staticmethod
     def _get_async_method_pair(
         mw: Any, methodname: str
     ) -> Union[None, Callable, Tuple[Callable, Callable]]:
-        normal_method = getattr(mw, methodname, None)
+        normal_method: Optional[Callable] = getattr(mw, methodname, None)
         methodname_async = methodname + "_async"
-        async_method = getattr(mw, methodname_async, None)
+        async_method: Optional[Callable] = getattr(mw, methodname_async, None)
         if not async_method:
             return normal_method
         if not normal_method:
             logger.error(
                 f"Middleware {mw.__qualname__} has {methodname_async} "
                 f"without {methodname}, skipping this method."
             )
```

### Comparing `Scrapy-2.8.0/scrapy/crawler.py` & `Scrapy-2.9.0/scrapy/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 import pprint
 import signal
 import warnings
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Type, Union
 
 from twisted.internet import defer
 from zope.interface.exceptions import DoesNotImplement
 
 try:
     # zope >= 5.0 only supports MultipleInvalid
     from zope.interface.exceptions import MultipleInvalid
@@ -18,16 +18,18 @@
 from zope.interface.verify import verifyClass
 
 from scrapy import Spider, signals
 from scrapy.core.engine import ExecutionEngine
 from scrapy.exceptions import ScrapyDeprecationWarning
 from scrapy.extension import ExtensionManager
 from scrapy.interfaces import ISpiderLoader
+from scrapy.logformatter import LogFormatter
 from scrapy.settings import Settings, overridden_settings
 from scrapy.signalmanager import SignalManager
+from scrapy.statscollectors import StatsCollector
 from scrapy.utils.log import (
     LogCounterHandler,
     configure_logging,
     get_scrapy_root_handler,
     install_scrapy_root_handler,
     log_reactor_info,
     log_scrapy_info,
@@ -45,28 +47,33 @@
     from scrapy.utils.request import RequestFingerprinter
 
 
 logger = logging.getLogger(__name__)
 
 
 class Crawler:
-    def __init__(self, spidercls, settings=None, init_reactor: bool = False):
+    def __init__(
+        self,
+        spidercls: Type[Spider],
+        settings: Union[None, dict, Settings] = None,
+        init_reactor: bool = False,
+    ):
         if isinstance(spidercls, Spider):
             raise ValueError("The spidercls argument must be a class, not an object")
 
         if isinstance(settings, dict) or settings is None:
             settings = Settings(settings)
 
-        self.spidercls = spidercls
-        self.settings = settings.copy()
+        self.spidercls: Type[Spider] = spidercls
+        self.settings: Settings = settings.copy()
         self.spidercls.update_settings(self.settings)
 
-        self.signals = SignalManager(self)
+        self.signals: SignalManager = SignalManager(self)
 
-        self.stats = load_object(self.settings["STATS_CLASS"])(self)
+        self.stats: StatsCollector = load_object(self.settings["STATS_CLASS"])(self)
 
         handler = LogCounterHandler(self, level=self.settings.get("LOG_LEVEL"))
         logging.root.addHandler(handler)
 
         d = dict(overridden_settings(self.settings))
         logger.info(
             "Overridden settings:\n%(settings)s", {"settings": pprint.pformat(d)}
@@ -76,43 +83,43 @@
             # scrapy root handler already installed: update it with new settings
             install_scrapy_root_handler(self.settings)
         # lambda is assigned to Crawler attribute because this way it is not
         # garbage collected after leaving __init__ scope
         self.__remove_handler = lambda: logging.root.removeHandler(handler)
         self.signals.connect(self.__remove_handler, signals.engine_stopped)
 
-        lf_cls = load_object(self.settings["LOG_FORMATTER"])
-        self.logformatter = lf_cls.from_crawler(self)
+        lf_cls: Type[LogFormatter] = load_object(self.settings["LOG_FORMATTER"])
+        self.logformatter: LogFormatter = lf_cls.from_crawler(self)
 
         self.request_fingerprinter: RequestFingerprinter = create_instance(
             load_object(self.settings["REQUEST_FINGERPRINTER_CLASS"]),
             settings=self.settings,
             crawler=self,
         )
 
-        reactor_class = self.settings["TWISTED_REACTOR"]
-        event_loop = self.settings["ASYNCIO_EVENT_LOOP"]
+        reactor_class: str = self.settings["TWISTED_REACTOR"]
+        event_loop: str = self.settings["ASYNCIO_EVENT_LOOP"]
         if init_reactor:
             # this needs to be done after the spider settings are merged,
             # but before something imports twisted.internet.reactor
             if reactor_class:
                 install_reactor(reactor_class, event_loop)
             else:
                 from twisted.internet import reactor  # noqa: F401
             log_reactor_info()
         if reactor_class:
             verify_installed_reactor(reactor_class)
             if is_asyncio_reactor_installed() and event_loop:
                 verify_installed_asyncio_event_loop(event_loop)
 
-        self.extensions = ExtensionManager.from_crawler(self)
+        self.extensions: ExtensionManager = ExtensionManager.from_crawler(self)
 
         self.settings.freeze()
-        self.crawling = False
-        self.spider = None
+        self.crawling: bool = False
+        self.spider: Optional[Spider] = None
         self.engine: Optional[ExecutionEngine] = None
 
     @defer.inlineCallbacks
     def crawl(self, *args, **kwargs):
         if self.crawling:
             raise RuntimeError("Crawling already taking place")
         self.crawling = True
```

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/ajaxcrawl.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/ajaxcrawl.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         self.lookup_bytes = settings.getint("AJAXCRAWL_MAXSIZE", 32768)
 
     @classmethod
     def from_crawler(cls, crawler):
         return cls(crawler.settings)
 
     def process_response(self, request, response, spider):
-
         if not isinstance(response, HtmlResponse) or response.status != 200:
             return response
 
         if request.method != "GET":
             # other HTTP methods are either not safe or don't have a body
             return response
```

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/cookies.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/cookies.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/decompression.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/decompression.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         respcls = responsetypes.from_args(filename=tar_file.members[0].name, body=body)
         return response.replace(body=body, cls=respcls)
 
     def _is_zip(self, response):
         archive = BytesIO(response.body)
         try:
             zip_file = zipfile.ZipFile(archive)
-        except zipfile.BadZipfile:
+        except zipfile.BadZipFile:
             return
 
         namelist = zip_file.namelist()
         body = zip_file.read(namelist[0])
         respcls = responsetypes.from_args(filename=namelist[0], body=body)
         return response.replace(body=body, cls=respcls)
```

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/defaultheaders.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/downloadtimeout.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/downloadtimeout.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/httpauth.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/httpauth.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/httpcache.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/httpcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from scrapy.statscollectors import StatsCollector
 from scrapy.utils.misc import load_object
 
 HttpCacheMiddlewareTV = TypeVar("HttpCacheMiddlewareTV", bound="HttpCacheMiddleware")
 
 
 class HttpCacheMiddleware:
-
     DOWNLOAD_EXCEPTIONS = (
         defer.TimeoutError,
         TimeoutError,
         DNSLookupError,
         ConnectionRefusedError,
         ConnectionDone,
         ConnectError,
```

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/httpcompression.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/httpcompression.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
             result.stats = crawler.stats
             return result
 
     def process_request(self, request, spider):
         request.headers.setdefault("Accept-Encoding", b", ".join(ACCEPTED_ENCODINGS))
 
     def process_response(self, request, response, spider):
-
         if request.method == "HEAD":
             return response
         if isinstance(response, Response):
             content_encoding = response.headers.getlist("Content-Encoding")
             if content_encoding:
                 encoding = content_encoding.pop()
                 decoded_body = self._decode(response.body, encoding.lower())
```

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/httpproxy.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/httpproxy.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/redirect.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/redirect.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         redirect_request_netloc = urlparse_cached(redirect_request).netloc
         if source_request_netloc != redirect_request_netloc:
             del redirect_request.headers["Cookie"]
     return redirect_request
 
 
 class BaseRedirectMiddleware:
-
     enabled_setting = "REDIRECT_ENABLED"
 
     def __init__(self, settings):
         if not settings.getbool(self.enabled_setting):
             raise NotConfigured
 
         self.max_redirect_times = settings.getint("REDIRECT_MAX_TIMES")
@@ -111,15 +110,14 @@
             return self._redirect(redirected, request, spider, response.status)
 
         redirected = self._redirect_request_using_get(request, redirected_url)
         return self._redirect(redirected, request, spider, response.status)
 
 
 class MetaRefreshMiddleware(BaseRedirectMiddleware):
-
     enabled_setting = "METAREFRESH_ENABLED"
 
     def __init__(self, settings):
         super().__init__(settings)
         self._ignore_tags = settings.getlist("METAREFRESH_IGNORE_TAGS")
         self._maxdelay = settings.getint("METAREFRESH_MAXDELAY")
```

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/retry.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         {"request": request, "retry_times": retry_times, "reason": reason},
         extra={"spider": spider},
     )
     return None
 
 
 class RetryMiddleware:
-
     # IOError is raised by the HttpCompression middleware when trying to
     # decompress an empty response
     EXCEPTIONS_TO_RETRY = (
         defer.TimeoutError,
         TimeoutError,
         DNSLookupError,
         ConnectionRefusedError,
```

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/robotstxt.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/robotstxt.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/stats.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/stats.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/downloadermiddlewares/useragent.py` & `Scrapy-2.9.0/scrapy/downloadermiddlewares/useragent.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/dupefilters.py` & `Scrapy-2.9.0/scrapy/dupefilters.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/exceptions.py` & `Scrapy-2.9.0/scrapy/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     pass
 
 
 class CloseSpider(Exception):
     """Raise this from callbacks to request the spider to be closed"""
 
-    def __init__(self, reason="cancelled"):
+    def __init__(self, reason: str = "cancelled"):
         super().__init__()
         self.reason = reason
 
 
 class StopDownload(Exception):
     """
     Stop the download of the body for a given response.
```

### Comparing `Scrapy-2.8.0/scrapy/exporters.py` & `Scrapy-2.9.0/scrapy/exporters.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/closespider.py` & `Scrapy-2.9.0/scrapy/extensions/closespider.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/corestats.py` & `Scrapy-2.9.0/scrapy/extensions/corestats.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/debug.py` & `Scrapy-2.9.0/scrapy/extensions/debug.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/feedexport.py` & `Scrapy-2.9.0/scrapy/extensions/feedexport.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 import logging
 import re
 import sys
 import warnings
 from datetime import datetime
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import IO, Any, Callable, Optional, Tuple, Union
+from typing import IO, Any, Callable, List, Optional, Tuple, Union
 from urllib.parse import unquote, urlparse
 
 from twisted.internet import defer, threads
+from twisted.internet.defer import DeferredList
 from w3lib.url import file_uri_to_path
 from zope.interface import Interface, implementer
 
 from scrapy import Spider, signals
 from scrapy.exceptions import NotConfigured, ScrapyDeprecationWarning
 from scrapy.extensions.postprocessing import PostProcessingManager
 from scrapy.utils.boto import is_botocore_available
 from scrapy.utils.conf import feed_complete_default_values_from_settings
+from scrapy.utils.defer import maybe_deferred_to_future
+from scrapy.utils.deprecate import create_deprecated_class
 from scrapy.utils.ftp import ftp_store_file
 from scrapy.utils.log import failure_to_exc_info
 from scrapy.utils.misc import create_instance, load_object
 from scrapy.utils.python import get_func_args, without_none_values
 
 logger = logging.getLogger(__name__)
 
@@ -267,15 +270,15 @@
             username=self.username,
             password=self.password,
             use_active_mode=self.use_active_mode,
             overwrite=self.overwrite,
         )
 
 
-class _FeedSlot:
+class FeedSlot:
     def __init__(
         self,
         file,
         exporter,
         storage,
         uri,
         format,
@@ -305,15 +308,23 @@
 
     def finish_exporting(self):
         if self._exporting:
             self.exporter.finish_exporting()
             self._exporting = False
 
 
+_FeedSlot = create_deprecated_class(
+    name="_FeedSlot",
+    new_class=FeedSlot,
+)
+
+
 class FeedExporter:
+    _pending_deferreds: List[defer.Deferred] = []
+
     @classmethod
     def from_crawler(cls, crawler):
         exporter = cls(crawler)
         crawler.signals.connect(exporter.open_spider, signals.spider_opened)
         crawler.signals.connect(exporter.close_spider, signals.spider_closed)
         crawler.signals.connect(exporter.item_scraped, signals.item_scraped)
         return exporter
@@ -371,36 +382,57 @@
                     uri=uri % uri_params,
                     feed_options=feed_options,
                     spider=spider,
                     uri_template=uri,
                 )
             )
 
-    def close_spider(self, spider):
-        deferred_list = []
+    async def close_spider(self, spider):
         for slot in self.slots:
-            d = self._close_slot(slot, spider)
-            deferred_list.append(d)
-        return defer.DeferredList(deferred_list) if deferred_list else None
+            self._close_slot(slot, spider)
+
+        # Await all deferreds
+        if self._pending_deferreds:
+            await maybe_deferred_to_future(DeferredList(self._pending_deferreds))
+
+        # Send FEED_EXPORTER_CLOSED signal
+        await maybe_deferred_to_future(
+            self.crawler.signals.send_catch_log_deferred(signals.feed_exporter_closed)
+        )
 
     def _close_slot(self, slot, spider):
+        def get_file(slot_):
+            if isinstance(slot_.file, PostProcessingManager):
+                slot_.file.close()
+                return slot_.file.file
+            return slot_.file
+
         slot.finish_exporting()
         if not slot.itemcount and not slot.store_empty:
             # We need to call slot.storage.store nonetheless to get the file
             # properly closed.
-            return defer.maybeDeferred(slot.storage.store, slot.file)
+            return defer.maybeDeferred(slot.storage.store, get_file(slot))
+
         logmsg = f"{slot.format} feed ({slot.itemcount} items) in: {slot.uri}"
-        d = defer.maybeDeferred(slot.storage.store, slot.file)
+        d = defer.maybeDeferred(slot.storage.store, get_file(slot))
 
         d.addCallback(
             self._handle_store_success, logmsg, spider, type(slot.storage).__name__
         )
         d.addErrback(
             self._handle_store_error, logmsg, spider, type(slot.storage).__name__
         )
+        self._pending_deferreds.append(d)
+        d.addCallback(
+            lambda _: self.crawler.signals.send_catch_log_deferred(
+                signals.feed_slot_closed, slot=slot
+            )
+        )
+        d.addBoth(lambda _: self._pending_deferreds.remove(d))
+
         return d
 
     def _handle_store_error(self, f, logmsg, spider, slot_type):
         logger.error(
             "Error storing %s",
             logmsg,
             exc_info=failure_to_exc_info(f),
@@ -433,15 +465,15 @@
             file=file,
             format=feed_options["format"],
             fields_to_export=feed_options["fields"],
             encoding=feed_options["encoding"],
             indent=feed_options["indent"],
             **feed_options["item_export_kwargs"],
         )
-        slot = _FeedSlot(
+        slot = FeedSlot(
             file=file,
             exporter=exporter,
             storage=storage,
             uri=uri,
             format=feed_options["format"],
             store_empty=feed_options["store_empty"],
             batch_id=batch_id,
@@ -568,15 +600,15 @@
             raise TypeError(f"{feedcls.__qualname__}.{method_name} returned None")
         return instance
 
     def _get_uri_params(
         self,
         spider: Spider,
         uri_params_function: Optional[Union[str, Callable[[dict, Spider], dict]]],
-        slot: Optional[_FeedSlot] = None,
+        slot: Optional[FeedSlot] = None,
     ) -> dict:
         params = {}
         for k in dir(spider):
             params[k] = getattr(spider, k)
         utc_now = datetime.utcnow()
         params["time"] = utc_now.replace(microsecond=0).isoformat().replace(":", "-")
         params["batch_time"] = utc_now.isoformat().replace(":", "-")
```

### Comparing `Scrapy-2.8.0/scrapy/extensions/httpcache.py` & `Scrapy-2.9.0/scrapy/extensions/httpcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         return True
 
     def is_cached_response_valid(self, cachedresponse, response, request):
         return True
 
 
 class RFC2616Policy:
-
     MAXAGE = 3600 * 24 * 365  # one year
 
     def __init__(self, settings):
         self.always_store = settings.getbool("HTTPCACHE_ALWAYS_STORE")
         self.ignore_schemes = settings.getlist("HTTPCACHE_IGNORE_SCHEMES")
         self._cc_parsed = WeakKeyDictionary()
         self.ignore_response_cache_controls = [
```

### Comparing `Scrapy-2.8.0/scrapy/extensions/logstats.py` & `Scrapy-2.9.0/scrapy/extensions/logstats.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/memdebug.py` & `Scrapy-2.9.0/scrapy/extensions/memdebug.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/memusage.py` & `Scrapy-2.9.0/scrapy/extensions/memusage.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/postprocessing.py` & `Scrapy-2.9.0/scrapy/extensions/postprocessing.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/spiderstate.py` & `Scrapy-2.9.0/scrapy/extensions/spiderstate.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/statsmailer.py` & `Scrapy-2.9.0/scrapy/extensions/statsmailer.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/telnet.py` & `Scrapy-2.9.0/scrapy/extensions/telnet.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/extensions/throttle.py` & `Scrapy-2.9.0/scrapy/extensions/throttle.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/http/__init__.py` & `Scrapy-2.9.0/scrapy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/http/cookies.py` & `Scrapy-2.9.0/scrapy/http/cookies.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/http/headers.py` & `Scrapy-2.9.0/tests/test_command_check.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,96 @@
-from collections.abc import Mapping
+from tests.test_commands import CommandTest
 
-from w3lib.http import headers_dict_to_raw
 
-from scrapy.utils.datatypes import CaselessDict
-from scrapy.utils.python import to_unicode
+class CheckCommandTest(CommandTest):
+    command = "check"
 
-
-class Headers(CaselessDict):
-    """Case insensitive http headers dictionary"""
-
-    def __init__(self, seq=None, encoding="utf-8"):
-        self.encoding = encoding
-        super().__init__(seq)
-
-    def update(self, seq):
-        seq = seq.items() if isinstance(seq, Mapping) else seq
-        iseq = {}
-        for k, v in seq:
-            iseq.setdefault(self.normkey(k), []).extend(self.normvalue(v))
-        super().update(iseq)
-
-    def normkey(self, key):
-        """Normalize key to bytes"""
-        return self._tobytes(key.title())
-
-    def normvalue(self, value):
-        """Normalize values to bytes"""
-        if value is None:
-            value = []
-        elif isinstance(value, (str, bytes)):
-            value = [value]
-        elif not hasattr(value, "__iter__"):
-            value = [value]
-
-        return [self._tobytes(x) for x in value]
-
-    def _tobytes(self, x):
-        if isinstance(x, bytes):
-            return x
-        if isinstance(x, str):
-            return x.encode(self.encoding)
-        if isinstance(x, int):
-            return str(x).encode(self.encoding)
-        raise TypeError(f"Unsupported value type: {type(x)}")
-
-    def __getitem__(self, key):
-        try:
-            return super().__getitem__(key)[-1]
-        except IndexError:
-            return None
-
-    def get(self, key, def_val=None):
-        try:
-            return super().get(key, def_val)[-1]
-        except IndexError:
-            return None
-
-    def getlist(self, key, def_val=None):
-        try:
-            return super().__getitem__(key)
-        except KeyError:
-            if def_val is not None:
-                return self.normvalue(def_val)
-            return []
-
-    def setlist(self, key, list_):
-        self[key] = list_
-
-    def setlistdefault(self, key, default_list=()):
-        return self.setdefault(key, default_list)
-
-    def appendlist(self, key, value):
-        lst = self.getlist(key)
-        lst.extend(self.normvalue(value))
-        self[key] = lst
-
-    def items(self):
-        return ((k, self.getlist(k)) for k in self.keys())
-
-    def values(self):
-        return [self[k] for k in self.keys()]
-
-    def to_string(self):
-        return headers_dict_to_raw(self)
-
-    def to_unicode_dict(self):
-        """Return headers as a CaselessDict with unicode keys
-        and unicode values. Multiple values are joined with ','.
-        """
-        return CaselessDict(
-            (
-                to_unicode(key, encoding=self.encoding),
-                to_unicode(b",".join(value), encoding=self.encoding),
-            )
-            for key, value in self.items()
+    def setUp(self):
+        super().setUp()
+        self.spider_name = "check_spider"
+        self.spider = (self.proj_mod_path / "spiders" / "checkspider.py").resolve()
+
+    def _write_contract(self, contracts, parse_def):
+        self.spider.write_text(
+            f"""
+import scrapy
+
+class CheckSpider(scrapy.Spider):
+    name = '{self.spider_name}'
+    start_urls = ['http://toscrape.com']
+
+    def parse(self, response, **cb_kwargs):
+        \"\"\"
+        @url http://toscrape.com
+        {contracts}
+        \"\"\"
+        {parse_def}
+        """,
+            encoding="utf-8",
         )
 
-    def __copy__(self):
-        return self.__class__(self)
+    def _test_contract(self, contracts="", parse_def="pass"):
+        self._write_contract(contracts, parse_def)
+        p, out, err = self.proc("check")
+        self.assertNotIn("F", out)
+        self.assertIn("OK", err)
+        self.assertEqual(p.returncode, 0)
+
+    def test_check_returns_requests_contract(self):
+        contracts = """
+        @returns requests 1
+        """
+        parse_def = """
+        yield scrapy.Request(url='http://next-url.com')
+        """
+        self._test_contract(contracts, parse_def)
+
+    def test_check_returns_items_contract(self):
+        contracts = """
+        @returns items 1
+        """
+        parse_def = """
+        yield {'key1': 'val1', 'key2': 'val2'}
+        """
+        self._test_contract(contracts, parse_def)
+
+    def test_check_cb_kwargs_contract(self):
+        contracts = """
+        @cb_kwargs {"arg1": "val1", "arg2": "val2"}
+        """
+        parse_def = """
+        if len(cb_kwargs.items()) == 0:
+            raise Exception("Callback args not set")
+        """
+        self._test_contract(contracts, parse_def)
+
+    def test_check_scrapes_contract(self):
+        contracts = """
+        @scrapes key1 key2
+        """
+        parse_def = """
+        yield {'key1': 'val1', 'key2': 'val2'}
+        """
+        self._test_contract(contracts, parse_def)
+
+    def test_check_all_default_contracts(self):
+        contracts = """
+        @returns items 1
+        @returns requests 1
+        @scrapes key1 key2
+        @cb_kwargs {"arg1": "val1", "arg2": "val2"}
+        """
+        parse_def = """
+        yield {'key1': 'val1', 'key2': 'val2'}
+        yield scrapy.Request(url='http://next-url.com')
+        if len(cb_kwargs.items()) == 0:
+            raise Exception("Callback args not set")
+        """
+        self._test_contract(contracts, parse_def)
 
-    copy = __copy__
+    def test_SCRAPY_CHECK_set(self):
+        parse_def = """
+        import os
+        if not os.environ.get('SCRAPY_CHECK'):
+            raise Exception('SCRAPY_CHECK not set')
+        """
+        self._test_contract(parse_def=parse_def)
```

### Comparing `Scrapy-2.8.0/scrapy/http/request/__init__.py` & `Scrapy-2.9.0/scrapy/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/http/request/form.py` & `Scrapy-2.9.0/scrapy/http/request/form.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """
 This module implements the FormRequest class which is a more convenient class
 (than Request) to generate Requests based on form data.
 
 See documentation in docs/topics/request-response.rst
 """
 
-from typing import Iterable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Iterable, List, Optional, Tuple, Type, TypeVar, Union, cast
 from urllib.parse import urlencode, urljoin, urlsplit, urlunsplit
 
-from lxml.html import FormElement, HtmlElement, HTMLParser, SelectElement
+from lxml.html import (
+    FormElement,
+    HTMLParser,
+    InputElement,
+    MultipleSelectOptions,
+    SelectElement,
+    TextareaElement,
+)
 from parsel.selector import create_root_node
 from w3lib.html import strip_html5_whitespace
 
 from scrapy.http.request import Request
 from scrapy.http.response.text import TextResponse
 from scrapy.utils.python import is_listlike, to_bytes
 from scrapy.utils.response import get_base_url
 
 FormRequestTypeVar = TypeVar("FormRequestTypeVar", bound="FormRequest")
 
-FormdataType = Optional[Union[dict, List[Tuple[str, str]]]]
+FormdataKVType = Tuple[str, Union[str, Iterable[str]]]
+FormdataType = Optional[Union[dict, List[FormdataKVType]]]
 
 
 class FormRequest(Request):
     valid_form_methods = ["GET", "POST"]
 
     def __init__(self, *args, formdata: FormdataType = None, **kwargs) -> None:
         if formdata and kwargs.get("method") is None:
@@ -46,15 +54,15 @@
 
     @classmethod
     def from_response(
         cls: Type[FormRequestTypeVar],
         response: TextResponse,
         formname: Optional[str] = None,
         formid: Optional[str] = None,
-        formnumber: Optional[int] = 0,
+        formnumber: int = 0,
         formdata: FormdataType = None,
         clickdata: Optional[dict] = None,
         dont_click: bool = False,
         formxpath: Optional[str] = None,
         formcss: Optional[str] = None,
         **kwargs,
     ) -> FormRequestTypeVar:
@@ -75,36 +83,37 @@
             if method not in cls.valid_form_methods:
                 method = "GET"
 
         return cls(url=url, method=method, formdata=formdata, **kwargs)
 
 
 def _get_form_url(form: FormElement, url: Optional[str]) -> str:
+    assert form.base_url is not None  # typing
     if url is None:
         action = form.get("action")
         if action is None:
             return form.base_url
         return urljoin(form.base_url, strip_html5_whitespace(action))
     return urljoin(form.base_url, url)
 
 
-def _urlencode(seq: Iterable, enc: str) -> str:
+def _urlencode(seq: Iterable[FormdataKVType], enc: str) -> str:
     values = [
         (to_bytes(k, enc), to_bytes(v, enc))
         for k, vs in seq
-        for v in (vs if is_listlike(vs) else [vs])
+        for v in (cast(Iterable[str], vs) if is_listlike(vs) else [cast(str, vs)])
     ]
     return urlencode(values, doseq=True)
 
 
 def _get_form(
     response: TextResponse,
     formname: Optional[str],
     formid: Optional[str],
-    formnumber: Optional[int],
+    formnumber: int,
     formxpath: Optional[str],
 ) -> FormElement:
     """Find the wanted form element within the given response."""
     root = create_root_node(response.text, HTMLParser, base_url=get_base_url(response))
     forms = root.xpath("//form")
     if not forms:
         raise ValueError(f"No <form> element found in {response}")
@@ -129,29 +138,28 @@
                     return el
                 el = el.getparent()
                 if el is None:
                     break
         raise ValueError(f"No <form> element found with {formxpath}")
 
     # If we get here, it means that either formname was None or invalid
-    if formnumber is not None:
-        try:
-            form = forms[formnumber]
-        except IndexError:
-            raise IndexError(f"Form number {formnumber} not found in {response}")
-        else:
-            return form
+    try:
+        form = forms[formnumber]
+    except IndexError:
+        raise IndexError(f"Form number {formnumber} not found in {response}")
+    else:
+        return form
 
 
 def _get_inputs(
     form: FormElement,
     formdata: FormdataType,
     dont_click: bool,
     clickdata: Optional[dict],
-) -> List[Tuple[str, str]]:
+) -> List[FormdataKVType]:
     """Return a list of key-value pairs for the inputs found in the given form."""
     try:
         formdata_keys = dict(formdata or ()).keys()
     except (ValueError, TypeError):
         raise ValueError("formdata should be a dict or iterable of tuples")
 
     if not formdata:
@@ -161,15 +169,15 @@
         "|descendant::select"
         "|descendant::input[not(@type) or @type["
         ' not(re:test(., "^(?:submit|image|reset)$", "i"))'
         " and (../@checked or"
         '  not(re:test(., "^(?:checkbox|radio)$", "i")))]]',
         namespaces={"re": "http://exslt.org/regular-expressions"},
     )
-    values = [
+    values: List[FormdataKVType] = [
         (k, "" if v is None else v)
         for k, v in (_value(e) for e in inputs)
         if k and k not in formdata_keys
     ]
 
     if not dont_click:
         clickable = _get_clickable(clickdata, form)
@@ -179,35 +187,33 @@
     if isinstance(formdata, dict):
         formdata = formdata.items()  # type: ignore[assignment]
 
     values.extend((k, v) for k, v in formdata if v is not None)
     return values
 
 
-def _value(ele: HtmlElement):
+def _value(
+    ele: Union[InputElement, SelectElement, TextareaElement]
+) -> Tuple[Optional[str], Union[None, str, MultipleSelectOptions]]:
     n = ele.name
     v = ele.value
     if ele.tag == "select":
-        return _select_value(ele, n, v)
+        return _select_value(cast(SelectElement, ele), n, v)
     return n, v
 
 
-def _select_value(ele: SelectElement, n: str, v: str):
+def _select_value(
+    ele: SelectElement, n: Optional[str], v: Union[None, str, MultipleSelectOptions]
+) -> Tuple[Optional[str], Union[None, str, MultipleSelectOptions]]:
     multiple = ele.multiple
     if v is None and not multiple:
         # Match browser behaviour on simple select tag without options selected
         # And for select tags without options
         o = ele.value_options
         return (n, o[0]) if o else (None, None)
-    if v is not None and multiple:
-        # This is a workaround to bug in lxml fixed 2.3.1
-        # fix https://github.com/lxml/lxml/commit/57f49eed82068a20da3db8f1b18ae00c1bab8b12#L1L1139
-        selected_options = ele.xpath(".//option[@selected]")
-        values = [(o.get("value") or o.text or "").strip() for o in selected_options]
-        return n, values
     return n, v
 
 
 def _get_clickable(
     clickdata: Optional[dict], form: FormElement
 ) -> Optional[Tuple[str, str]]:
     """
```

### Comparing `Scrapy-2.8.0/scrapy/http/request/json_request.py` & `Scrapy-2.9.0/scrapy/http/request/json_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from typing import Optional, Tuple
 
 from scrapy.http.request import Request
 from scrapy.utils.deprecate import create_deprecated_class
 
 
 class JsonRequest(Request):
-
     attributes: Tuple[str, ...] = Request.attributes + ("dumps_kwargs",)
 
     def __init__(self, *args, dumps_kwargs: Optional[dict] = None, **kwargs) -> None:
         dumps_kwargs = copy.deepcopy(dumps_kwargs) if dumps_kwargs is not None else {}
         dumps_kwargs.setdefault("sort_keys", True)
         self._dumps_kwargs = dumps_kwargs
```

### Comparing `Scrapy-2.8.0/scrapy/http/request/rpc.py` & `Scrapy-2.9.0/scrapy/http/request/rpc.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/http/response/__init__.py` & `Scrapy-2.9.0/scrapy/http/response/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,14 +138,20 @@
 
     def css(self, *a, **kw):
         """Shortcut method implemented only by responses whose content
         is text (subclasses of TextResponse).
         """
         raise NotSupported("Response content isn't text")
 
+    def jmespath(self, *a, **kw):
+        """Shortcut method implemented only by responses whose content
+        is text (subclasses of TextResponse).
+        """
+        raise NotSupported("Response content isn't text")
+
     def xpath(self, *a, **kw):
         """Shortcut method implemented only by responses whose content
         is text (subclasses of TextResponse).
         """
         raise NotSupported("Response content isn't text")
 
     def follow(
```

### Comparing `Scrapy-2.8.0/scrapy/http/response/text.py` & `Scrapy-2.9.0/scrapy/http/response/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from scrapy.utils.python import memoizemethod_noargs, to_unicode
 from scrapy.utils.response import get_base_url
 
 _NONE = object()
 
 
 class TextResponse(Response):
-
     _DEFAULT_ENCODING = "ascii"
     _cached_decoded_json = _NONE
 
     attributes: Tuple[str, ...] = Response.attributes + ("encoding",)
 
     def __init__(self, *args, **kwargs):
         self._encoding = kwargs.pop("encoding", None)
@@ -97,19 +96,21 @@
         """Join this Response's url with a possible relative url to form an
         absolute interpretation of the latter."""
         return urljoin(get_base_url(self), url)
 
     @memoizemethod_noargs
     def _headers_encoding(self):
         content_type = self.headers.get(b"Content-Type", b"")
-        return http_content_type_encoding(to_unicode(content_type))
+        return http_content_type_encoding(to_unicode(content_type, encoding="latin-1"))
 
     def _body_inferred_encoding(self):
         if self._cached_benc is None:
-            content_type = to_unicode(self.headers.get(b"Content-Type", b""))
+            content_type = to_unicode(
+                self.headers.get(b"Content-Type", b""), encoding="latin-1"
+            )
             benc, ubody = html_to_unicode(
                 content_type,
                 self.body,
                 auto_detect_fun=self._auto_detect_fun,
                 default_encoding=self._DEFAULT_ENCODING,
             )
             self._cached_benc = benc
@@ -136,14 +137,22 @@
     def selector(self):
         from scrapy.selector import Selector
 
         if self._cached_selector is None:
             self._cached_selector = Selector(self)
         return self._cached_selector
 
+    def jmespath(self, query, **kwargs):
+        if not hasattr(self.selector, "jmespath"):  # type: ignore[attr-defined]
+            raise AttributeError(
+                "Please install parsel >= 1.8.1 to get jmespath support"
+            )
+
+        return self.selector.jmespath(query, **kwargs)  # type: ignore[attr-defined]
+
     def xpath(self, query, **kwargs):
         return self.selector.xpath(query, **kwargs)
 
     def css(self, query):
         return self.selector.css(query)
 
     def follow(
```

### Comparing `Scrapy-2.8.0/scrapy/interfaces.py` & `Scrapy-2.9.0/scrapy/interfaces.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/item.py` & `Scrapy-2.9.0/scrapy/item.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/link.py` & `Scrapy-2.9.0/scrapy/link.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/linkextractors/__init__.py` & `Scrapy-2.9.0/scrapy/linkextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/linkextractors/lxmlhtml.py` & `Scrapy-2.9.0/scrapy/linkextractors/lxmlhtml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Link extractor based on lxml.html
 """
+import logging
 import operator
 from functools import partial
 from urllib.parse import urljoin, urlparse
 
 from lxml import etree
 from parsel.csstranslator import HTMLTranslator
 from w3lib.html import strip_html5_whitespace
@@ -19,14 +20,16 @@
     re,
 )
 from scrapy.utils.misc import arg_to_iter, rel_has_nofollow
 from scrapy.utils.python import unique as unique_list
 from scrapy.utils.response import get_base_url
 from scrapy.utils.url import url_has_any_extension, url_is_from_any_domain
 
+logger = logging.getLogger(__name__)
+
 # from lxml/src/lxml/html/__init__.py
 XHTML_NAMESPACE = "http://www.w3.org/1999/xhtml"
 
 _collect_string_content = etree.XPath("string()")
 
 
 def _nons(tag):
@@ -84,15 +87,20 @@
                 attr_val = urljoin(base_url, attr_val)
             except ValueError:
                 continue  # skipping bogus links
             else:
                 url = self.process_attr(attr_val)
                 if url is None:
                     continue
-            url = safe_url_string(url, encoding=response_encoding)
+            try:
+                url = safe_url_string(url, encoding=response_encoding)
+            except ValueError:
+                logger.debug(f"Skipping extraction of link with bad URL {url!r}")
+                continue
+
             # to fix relative links after process_value
             url = urljoin(response_url, url)
             link = Link(
                 url,
                 _collect_string_content(el) or "",
                 nofollow=rel_has_nofollow(el.get("rel")),
             )
@@ -190,15 +198,14 @@
         ):
             return False
         if self.restrict_text and not _matches(link.text, self.restrict_text):
             return False
         return True
 
     def matches(self, url):
-
         if self.allow_domains and not url_is_from_any_domain(url, self.allow_domains):
             return False
         if self.deny_domains and url_is_from_any_domain(url, self.deny_domains):
             return False
 
         allowed = (
             (regex.search(url) for regex in self.allow_res)
```

### Comparing `Scrapy-2.8.0/scrapy/loader/__init__.py` & `Scrapy-2.9.0/scrapy/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/loader/common.py` & `Scrapy-2.9.0/scrapy/loader/common.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/loader/processors.py` & `Scrapy-2.9.0/scrapy/loader/processors.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/logformatter.py` & `Scrapy-2.9.0/scrapy/logformatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import logging
 import os
+from typing import Any, Dict, Optional, Union
 
 from twisted.python.failure import Failure
 
+from scrapy import Request, Spider
+from scrapy.http import Response
 from scrapy.utils.request import referer_str
 
 SCRAPEDMSG = "Scraped from %(src)s" + os.linesep + "%(item)s"
 DROPPEDMSG = "Dropped: %(exception)s" + os.linesep + "%(item)s"
 CRAWLEDMSG = "Crawled (%(status)s) %(request)s%(request_flags)s (referer: %(referer)s)%(response_flags)s"
 ITEMERRORMSG = "Error processing %(item)s"
 SPIDERERRORMSG = "Spider error processing %(request)s (referer: %(referer)s)"
@@ -48,15 +51,15 @@
                         'args': {
                             'exception': exception,
                             'item': item,
                         }
                     }
     """
 
-    def crawled(self, request, response, spider):
+    def crawled(self, request: Request, response: Response, spider: Spider) -> dict:
         """Logs a message when the crawler finds a webpage."""
         request_flags = f" {str(request.flags)}" if request.flags else ""
         response_flags = f" {str(response.flags)}" if response.flags else ""
         return {
             "level": logging.DEBUG,
             "msg": CRAWLEDMSG,
             "args": {
@@ -66,75 +69,90 @@
                 "referer": referer_str(request),
                 "response_flags": response_flags,
                 # backward compatibility with Scrapy logformatter below 1.4 version
                 "flags": response_flags,
             },
         }
 
-    def scraped(self, item, response, spider):
+    def scraped(
+        self, item: Any, response: Union[Response, Failure], spider: Spider
+    ) -> dict:
         """Logs a message when an item is scraped by a spider."""
+        src: Any
         if isinstance(response, Failure):
             src = response.getErrorMessage()
         else:
             src = response
         return {
             "level": logging.DEBUG,
             "msg": SCRAPEDMSG,
             "args": {
                 "src": src,
                 "item": item,
             },
         }
 
-    def dropped(self, item, exception, response, spider):
+    def dropped(
+        self, item: Any, exception: BaseException, response: Response, spider: Spider
+    ) -> dict:
         """Logs a message when an item is dropped while it is passing through the item pipeline."""
         return {
             "level": logging.WARNING,
             "msg": DROPPEDMSG,
             "args": {
                 "exception": exception,
                 "item": item,
             },
         }
 
-    def item_error(self, item, exception, response, spider):
+    def item_error(
+        self, item: Any, exception, response: Response, spider: Spider
+    ) -> dict:
         """Logs a message when an item causes an error while it is passing
         through the item pipeline.
 
         .. versionadded:: 2.0
         """
         return {
             "level": logging.ERROR,
             "msg": ITEMERRORMSG,
             "args": {
                 "item": item,
             },
         }
 
-    def spider_error(self, failure, request, response, spider):
+    def spider_error(
+        self, failure: Failure, request: Request, response: Response, spider: Spider
+    ) -> dict:
         """Logs an error message from a spider.
 
         .. versionadded:: 2.0
         """
         return {
             "level": logging.ERROR,
             "msg": SPIDERERRORMSG,
             "args": {
                 "request": request,
                 "referer": referer_str(request),
             },
         }
 
-    def download_error(self, failure, request, spider, errmsg=None):
+    def download_error(
+        self,
+        failure: Failure,
+        request: Request,
+        spider: Spider,
+        errmsg: Optional[str] = None,
+    ) -> dict:
         """Logs a download error message from a spider (typically coming from
         the engine).
 
         .. versionadded:: 2.0
         """
-        args = {"request": request}
+        args: Dict[str, Any] = {"request": request}
         if errmsg:
             msg = DOWNLOADERRORMSG_LONG
             args["errmsg"] = errmsg
         else:
             msg = DOWNLOADERRORMSG_SHORT
         return {
             "level": logging.ERROR,
```

### Comparing `Scrapy-2.8.0/scrapy/mail.py` & `Scrapy-2.9.0/scrapy/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
                 "mailto": to,
                 "mailcc": cc,
                 "mailsubject": subject,
                 "mailattachs": nattachs,
                 "mailerr": errstr,
             },
         )
+        return failure
 
     def _sendmail(self, to_addrs, msg):
         from twisted.internet import reactor
 
         msg = BytesIO(msg)
         d = defer.Deferred()
```

### Comparing `Scrapy-2.8.0/scrapy/middleware.py` & `Scrapy-2.9.0/scrapy/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import pprint
 from collections import defaultdict, deque
-from typing import Any, Callable, Deque, Dict, Iterable, Tuple, Union, cast
+from typing import Any, Callable, Deque, Dict, Iterable, List, Tuple, Union, cast
 
 from twisted.internet.defer import Deferred
 
 from scrapy import Spider
 from scrapy.exceptions import NotConfigured
 from scrapy.settings import Settings
 from scrapy.utils.defer import process_chain, process_parallel
@@ -26,15 +26,15 @@
         self.methods: Dict[
             str, Deque[Union[None, Callable, Tuple[Callable, Callable]]]
         ] = defaultdict(deque)
         for mw in middlewares:
             self._add_middleware(mw)
 
     @classmethod
-    def _get_mwlist_from_settings(cls, settings: Settings) -> list:
+    def _get_mwlist_from_settings(cls, settings: Settings) -> List[Any]:
         raise NotImplementedError
 
     @classmethod
     def from_settings(cls, settings: Settings, crawler=None):
         mwlist = cls._get_mwlist_from_settings(settings)
         middlewares = []
         enabled = []
@@ -63,25 +63,25 @@
         )
         return cls(*middlewares)
 
     @classmethod
     def from_crawler(cls, crawler):
         return cls.from_settings(crawler.settings, crawler)
 
-    def _add_middleware(self, mw) -> None:
+    def _add_middleware(self, mw: Any) -> None:
         if hasattr(mw, "open_spider"):
             self.methods["open_spider"].append(mw.open_spider)
         if hasattr(mw, "close_spider"):
             self.methods["close_spider"].appendleft(mw.close_spider)
 
-    def _process_parallel(self, methodname: str, obj, *args) -> Deferred:
+    def _process_parallel(self, methodname: str, obj: Any, *args: Any) -> Deferred:
         methods = cast(Iterable[Callable], self.methods[methodname])
         return process_parallel(methods, obj, *args)
 
-    def _process_chain(self, methodname: str, obj, *args) -> Deferred:
+    def _process_chain(self, methodname: str, obj: Any, *args: Any) -> Deferred:
         methods = cast(Iterable[Callable], self.methods[methodname])
         return process_chain(methods, obj, *args)
 
     def open_spider(self, spider: Spider) -> Deferred:
         return self._process_parallel("open_spider", spider)
 
     def close_spider(self, spider: Spider) -> Deferred:
```

### Comparing `Scrapy-2.8.0/scrapy/mime.types` & `Scrapy-2.9.0/scrapy/mime.types`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/pipelines/files.py` & `Scrapy-2.9.0/scrapy/pipelines/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Files Pipeline
 
 See documentation in topics/media-pipeline.rst
 """
+import base64
 import functools
 import hashlib
 import logging
 import mimetypes
 import os
 import time
 from collections import defaultdict
 from contextlib import suppress
 from ftplib import FTP
 from io import BytesIO
+from os import PathLike
 from pathlib import Path
-from typing import DefaultDict, Optional, Set
+from typing import DefaultDict, Optional, Set, Union
 from urllib.parse import urlparse
 
 from itemadapter import ItemAdapter
 from twisted.internet import defer, threads
 
 from scrapy.exceptions import IgnoreRequest, NotConfigured
 from scrapy.http import Request
@@ -32,45 +34,52 @@
 from scrapy.utils.misc import md5sum
 from scrapy.utils.python import to_bytes
 from scrapy.utils.request import referer_str
 
 logger = logging.getLogger(__name__)
 
 
+def _to_string(path: Union[str, PathLike]) -> str:
+    return str(path)  # convert a Path object to string
+
+
 class FileException(Exception):
     """General media error exception"""
 
 
 class FSFilesStore:
-    def __init__(self, basedir: str):
+    def __init__(self, basedir: Union[str, PathLike]):
+        basedir = _to_string(basedir)
         if "://" in basedir:
             basedir = basedir.split("://", 1)[1]
         self.basedir = basedir
         self._mkdir(Path(self.basedir))
         self.created_directories: DefaultDict[str, Set[str]] = defaultdict(set)
 
-    def persist_file(self, path: str, buf, info, meta=None, headers=None):
+    def persist_file(
+        self, path: Union[str, PathLike], buf, info, meta=None, headers=None
+    ):
         absolute_path = self._get_filesystem_path(path)
         self._mkdir(absolute_path.parent, info)
         absolute_path.write_bytes(buf.getvalue())
 
-    def stat_file(self, path: str, info):
+    def stat_file(self, path: Union[str, PathLike], info):
         absolute_path = self._get_filesystem_path(path)
         try:
             last_modified = absolute_path.stat().st_mtime
         except os.error:
             return {}
 
         with absolute_path.open("rb") as f:
             checksum = md5sum(f)
 
         return {"last_modified": last_modified, "checksum": checksum}
 
-    def _get_filesystem_path(self, path: str) -> Path:
-        path_comps = path.split("/")
+    def _get_filesystem_path(self, path: Union[str, PathLike]) -> Path:
+        path_comps = _to_string(path).split("/")
         return Path(self.basedir, *path_comps)
 
     def _mkdir(self, dirname: Path, domain: Optional[str] = None):
         seen = self.created_directories[domain] if domain else set()
         if str(dirname) not in seen:
             if not dirname.exists():
                 dirname.mkdir(parents=True)
@@ -183,15 +192,14 @@
                 raise TypeError(f'Header "{key}" is not supported by botocore')
             else:
                 extra[kwarg] = value
         return extra
 
 
 class GCSFilesStore:
-
     GCS_PROJECT_ID = None
 
     CACHE_CONTROL = "max-age=172800"
 
     # The bucket's default object ACL will be applied to the object.
     # Overridden from settings.FILES_STORE_GCS_ACL in FilesPipeline.from_settings.
     POLICY = None
@@ -217,15 +225,15 @@
                 "No 'storage.objects.create' permission for GSC bucket %(bucket)s. Saving files will be impossible!",
                 {"bucket": bucket},
             )
 
     def stat_file(self, path, info):
         def _onsuccess(blob):
             if blob:
-                checksum = blob.md5_hash
+                checksum = base64.b64decode(blob.md5_hash).hex()
                 last_modified = time.mktime(blob.updated.timetuple())
                 return {"checksum": checksum, "last_modified": last_modified}
             return {}
 
         blob_path = self._get_blob_path(path)
         return threads.deferToThread(self.bucket.get_blob, blob_path).addCallback(
             _onsuccess
@@ -249,15 +257,14 @@
             data=buf.getvalue(),
             content_type=self._get_content_type(headers),
             predefined_acl=self.POLICY,
         )
 
 
 class FTPFilesStore:
-
     FTP_USERNAME = None
     FTP_PASSWORD = None
     USE_ACTIVE_MODE = None
 
     def __init__(self, uri):
         if not uri.startswith("ftp://"):
             raise ValueError(f"Incorrect URI scheme in {uri}, expected 'ftp'")
@@ -330,20 +337,20 @@
         "gs": GCSFilesStore,
         "ftp": FTPFilesStore,
     }
     DEFAULT_FILES_URLS_FIELD = "file_urls"
     DEFAULT_FILES_RESULT_FIELD = "files"
 
     def __init__(self, store_uri, download_func=None, settings=None):
+        store_uri = _to_string(store_uri)
         if not store_uri:
             raise NotConfigured
 
         if isinstance(settings, dict) or settings is None:
             settings = Settings(settings)
-
         cls_name = "FilesPipeline"
         self.store = self._get_store(store_uri)
         resolve = functools.partial(
             self._key_for_pipe, base_class_name=cls_name, settings=settings
         )
         self.expires = settings.getint(resolve("FILES_EXPIRES"), self.EXPIRES)
         if not hasattr(self, "FILES_URLS_FIELD"):
```

### Comparing `Scrapy-2.8.0/scrapy/pipelines/images.py` & `Scrapy-2.9.0/scrapy/pipelines/images.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/pipelines/media.py` & `Scrapy-2.9.0/scrapy/pipelines/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 
 def _DUMMY_CALLBACK(response):
     return response
 
 
 class MediaPipeline:
-
     LOG_FAILED_RESULTS = True
 
     class SpiderInfo:
         def __init__(self, spider):
             self.spider = spider
             self.downloading = set()
             self.downloaded = {}
```

### Comparing `Scrapy-2.8.0/scrapy/pqueues.py` & `Scrapy-2.9.0/scrapy/pqueues.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/resolver.py` & `Scrapy-2.9.0/scrapy/resolver.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/responsetypes.py` & `Scrapy-2.9.0/scrapy/responsetypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 from scrapy.http import Response
 from scrapy.utils.misc import load_object
 from scrapy.utils.python import binary_is_text, to_bytes, to_unicode
 
 
 class ResponseTypes:
-
     CLASSES = {
         "text/html": "scrapy.http.HtmlResponse",
         "application/atom+xml": "scrapy.http.XmlResponse",
         "application/rdf+xml": "scrapy.http.XmlResponse",
         "application/rss+xml": "scrapy.http.XmlResponse",
         "application/xhtml+xml": "scrapy.http.HtmlResponse",
         "application/vnd.wap.xhtml+xml": "scrapy.http.HtmlResponse",
@@ -48,15 +47,17 @@
         return self.classes.get(basetype, Response)
 
     def from_content_type(self, content_type, content_encoding=None):
         """Return the most appropriate Response class from an HTTP Content-Type
         header"""
         if content_encoding:
             return Response
-        mimetype = to_unicode(content_type).split(";")[0].strip().lower()
+        mimetype = (
+            to_unicode(content_type, encoding="latin-1").split(";")[0].strip().lower()
+        )
         return self.from_mimetype(mimetype)
 
     def from_content_disposition(self, content_disposition):
         try:
             filename = (
                 to_unicode(content_disposition, encoding="latin-1", errors="replace")
                 .split(";")[1]
```

### Comparing `Scrapy-2.8.0/scrapy/robotstxt.py` & `Scrapy-2.9.0/scrapy/robotstxt.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/selector/unified.py` & `Scrapy-2.9.0/scrapy/selector/unified.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from scrapy.http import HtmlResponse, XmlResponse
 from scrapy.utils.python import to_bytes
 from scrapy.utils.trackref import object_ref
 
 __all__ = ["Selector", "SelectorList"]
 
+_NOT_SET = object()
+
 
 def _st(response, st):
     if st is None:
         return "xml" if isinstance(response, XmlResponse) else "html"
     return st
 
 
@@ -59,15 +61,15 @@
     Otherwise, if ``type`` is set, the selector type will be forced and no
     detection will occur.
     """
 
     __slots__ = ["response"]
     selectorlist_cls = SelectorList
 
-    def __init__(self, response=None, text=None, type=None, root=None, **kwargs):
+    def __init__(self, response=None, text=None, type=None, root=_NOT_SET, **kwargs):
         if response is not None and text is not None:
             raise ValueError(
                 f"{self.__class__.__name__}.__init__() received "
                 "both response and text"
             )
 
         st = _st(response, type)
@@ -76,8 +78,12 @@
             response = _response_from_text(text, st)
 
         if response is not None:
             text = response.text
             kwargs.setdefault("base_url", response.url)
 
         self.response = response
-        super().__init__(text=text, type=st, root=root, **kwargs)
+
+        if root is not _NOT_SET:
+            kwargs["root"] = root
+
+        super().__init__(text=text, type=st, **kwargs)
```

### Comparing `Scrapy-2.8.0/scrapy/settings/__init__.py` & `Scrapy-2.9.0/scrapy/settings/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,21 @@
             if isinstance(value, SettingsAttribute):
                 self.attributes[name] = value
             else:
                 self.attributes[name] = SettingsAttribute(value, priority)
         else:
             self.attributes[name].set(value, priority)
 
+    def setdefault(self, name, default=None, priority="project"):
+        if name not in self:
+            self.set(name, default, priority)
+            return default
+
+        return self.attributes[name].value
+
     def setdict(self, values, priority="project"):
         self.update(values, priority)
 
     def setmodule(self, module, priority="project"):
         """
         Store settings from a module with a given priority.
```

### Comparing `Scrapy-2.8.0/scrapy/settings/default_settings.py` & `Scrapy-2.9.0/scrapy/settings/default_settings.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/shell.py` & `Scrapy-2.9.0/scrapy/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from scrapy.utils.datatypes import SequenceExclude
 from scrapy.utils.misc import load_object
 from scrapy.utils.reactor import is_asyncio_reactor_installed, set_asyncio_event_loop
 from scrapy.utils.response import open_in_browser
 
 
 class Shell:
-
     relevant_classes = (Crawler, Spider, Request, Response, Settings)
 
     def __init__(self, crawler, update_vars=None, code=None):
         self.crawler = crawler
         self.update_vars = update_vars or (lambda x: None)
         self.item_class = load_object(crawler.settings["DEFAULT_ITEM_CLASS"])
         self.spider = None
```

### Comparing `Scrapy-2.8.0/scrapy/signalmanager.py` & `Scrapy-2.9.0/scrapy/signalmanager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,71 @@
+from typing import Any, List, Tuple
+
 from pydispatch import dispatcher
+from twisted.internet.defer import Deferred
 
 from scrapy.utils import signal as _signal
 
 
 class SignalManager:
-    def __init__(self, sender=dispatcher.Anonymous):
-        self.sender = sender
+    def __init__(self, sender: Any = dispatcher.Anonymous):
+        self.sender: Any = sender
 
-    def connect(self, receiver, signal, **kwargs):
+    def connect(self, receiver: Any, signal: Any, **kwargs: Any) -> None:
         """
         Connect a receiver function to a signal.
 
         The signal can be any object, although Scrapy comes with some
         predefined signals that are documented in the :ref:`topics-signals`
         section.
 
         :param receiver: the function to be connected
         :type receiver: collections.abc.Callable
 
         :param signal: the signal to connect to
         :type signal: object
         """
         kwargs.setdefault("sender", self.sender)
-        return dispatcher.connect(receiver, signal, **kwargs)
+        dispatcher.connect(receiver, signal, **kwargs)
 
-    def disconnect(self, receiver, signal, **kwargs):
+    def disconnect(self, receiver: Any, signal: Any, **kwargs: Any) -> None:
         """
         Disconnect a receiver function from a signal. This has the
         opposite effect of the :meth:`connect` method, and the arguments
         are the same.
         """
         kwargs.setdefault("sender", self.sender)
-        return dispatcher.disconnect(receiver, signal, **kwargs)
+        dispatcher.disconnect(receiver, signal, **kwargs)
 
-    def send_catch_log(self, signal, **kwargs):
+    def send_catch_log(self, signal: Any, **kwargs: Any) -> List[Tuple[Any, Any]]:
         """
         Send a signal, catch exceptions and log them.
 
         The keyword arguments are passed to the signal handlers (connected
         through the :meth:`connect` method).
         """
         kwargs.setdefault("sender", self.sender)
         return _signal.send_catch_log(signal, **kwargs)
 
-    def send_catch_log_deferred(self, signal, **kwargs):
+    def send_catch_log_deferred(self, signal: Any, **kwargs: Any) -> Deferred:
         """
         Like :meth:`send_catch_log` but supports returning
         :class:`~twisted.internet.defer.Deferred` objects from signal handlers.
 
         Returns a Deferred that gets fired once all signal handlers
         deferreds were fired. Send a signal, catch exceptions and log them.
 
         The keyword arguments are passed to the signal handlers (connected
         through the :meth:`connect` method).
         """
         kwargs.setdefault("sender", self.sender)
         return _signal.send_catch_log_deferred(signal, **kwargs)
 
-    def disconnect_all(self, signal, **kwargs):
+    def disconnect_all(self, signal: Any, **kwargs: Any) -> None:
         """
         Disconnect all receivers from the given signal.
 
         :param signal: the signal to disconnect from
         :type signal: object
         """
         kwargs.setdefault("sender", self.sender)
-        return _signal.disconnect_all(signal, **kwargs)
+        _signal.disconnect_all(signal, **kwargs)
```

### Comparing `Scrapy-2.8.0/scrapy/signals.py` & `Scrapy-2.9.0/scrapy/signals.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 response_received = object()
 response_downloaded = object()
 headers_received = object()
 bytes_received = object()
 item_scraped = object()
 item_dropped = object()
 item_error = object()
+feed_slot_closed = object()
+feed_exporter_closed = object()
 
 # for backward compatibility
 stats_spider_opened = spider_opened
 stats_spider_closing = spider_closed
 stats_spider_closed = spider_closed
 
 item_passed = item_scraped
```

### Comparing `Scrapy-2.8.0/scrapy/spiderloader.py` & `Scrapy-2.9.0/scrapy/spiderloader.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/spidermiddlewares/depth.py` & `Scrapy-2.9.0/scrapy/spidermiddlewares/depth.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/spidermiddlewares/httperror.py` & `Scrapy-2.9.0/scrapy/spidermiddlewares/httperror.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/spidermiddlewares/offsite.py` & `Scrapy-2.9.0/scrapy/spidermiddlewares/offsite.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/spidermiddlewares/referer.py` & `Scrapy-2.9.0/scrapy/spidermiddlewares/referer.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 POLICY_ORIGIN_WHEN_CROSS_ORIGIN = "origin-when-cross-origin"
 POLICY_STRICT_ORIGIN_WHEN_CROSS_ORIGIN = "strict-origin-when-cross-origin"
 POLICY_UNSAFE_URL = "unsafe-url"
 POLICY_SCRAPY_DEFAULT = "scrapy-default"
 
 
 class ReferrerPolicy:
-
     NOREFERRER_SCHEMES: Tuple[str, ...] = LOCAL_SCHEMES
     name: str
 
     def referrer(self, response_url, request_url):
         raise NotImplementedError()
 
     def stripped_referrer(self, url):
```

### Comparing `Scrapy-2.8.0/scrapy/spidermiddlewares/urllength.py` & `Scrapy-2.9.0/scrapy/spidermiddlewares/urllength.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/spiders/__init__.py` & `Scrapy-2.9.0/scrapy/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/spiders/crawl.py` & `Scrapy-2.9.0/scrapy/spiders/crawl.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         self.callback = _get_method(self.callback, spider)
         self.errback = _get_method(self.errback, spider)
         self.process_links = _get_method(self.process_links, spider)
         self.process_request = _get_method(self.process_request, spider)
 
 
 class CrawlSpider(Spider):
-
     rules: Sequence[Rule] = ()
 
     def __init__(self, *a, **kw):
         super().__init__(*a, **kw)
         self._compile_rules()
 
     def _parse(self, response, **kwargs):
```

### Comparing `Scrapy-2.8.0/scrapy/spiders/feed.py` & `Scrapy-2.9.0/scrapy/spiders/feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def _iternodes(self, response):
         for node in xmliter(response, self.itertag):
             self._register_namespaces(node)
             yield node
 
     def _register_namespaces(self, selector):
-        for (prefix, uri) in self.namespaces:
+        for prefix, uri in self.namespaces:
             selector.register_namespace(prefix, uri)
 
 
 class CSVFeedSpider(Spider):
     """Spider for parsing CSV feeds.
     It receives a CSV file in a response; iterates through each of its rows,
     and calls parse_row with a dict containing each field's data.
```

### Comparing `Scrapy-2.8.0/scrapy/spiders/init.py` & `Scrapy-2.9.0/scrapy/spiders/init.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/spiders/sitemap.py` & `Scrapy-2.9.0/scrapy/spiders/sitemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from scrapy.utils.gz import gunzip, gzip_magic_number
 from scrapy.utils.sitemap import Sitemap, sitemap_urls_from_robots
 
 logger = logging.getLogger(__name__)
 
 
 class SitemapSpider(Spider):
-
     sitemap_urls = ()
     sitemap_rules = [("", "parse")]
     sitemap_follow = [""]
     sitemap_alternate_links = False
 
     def __init__(self, *a, **kw):
         super().__init__(*a, **kw)
```

### Comparing `Scrapy-2.8.0/scrapy/squeues.py` & `Scrapy-2.9.0/scrapy/squeues.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/templates/project/module/middlewares.py.tmpl` & `Scrapy-2.9.0/scrapy/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/templates/project/module/settings.py.tmpl` & `Scrapy-2.9.0/scrapy/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/templates/spiders/crawl.tmpl` & `Scrapy-2.9.0/scrapy/templates/spiders/crawl.tmpl`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from scrapy.linkextractors import LinkExtractor
 from scrapy.spiders import CrawlSpider, Rule
 
 
 class $classname(CrawlSpider):
     name = "$name"
     allowed_domains = ["$domain"]
-    start_urls = ["http://$domain/"]
+    start_urls = ["$url"]
 
     rules = (Rule(LinkExtractor(allow=r"Items/"), callback="parse_item", follow=True),)
 
     def parse_item(self, response):
         item = {}
         #item["domain_id"] = response.xpath('//input[@id="sid"]/@value').get()
         #item["name"] = response.xpath('//div[@id="name"]').get()
```

### Comparing `Scrapy-2.8.0/scrapy/templates/spiders/csvfeed.tmpl` & `Scrapy-2.9.0/scrapy/templates/spiders/csvfeed.tmpl`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from scrapy.spiders import CSVFeedSpider
 
 
 class $classname(CSVFeedSpider):
     name = "$name"
     allowed_domains = ["$domain"]
-    start_urls = ["http://$domain/feed.csv"]
+    start_urls = ["$url"]
     #headers = ["id", "name", "description", "image_link"]
     #delimiter = "\t"
 
     # Do any adaptations you need here
     #def adapt_response(self, response):
     #    return response
```

### Comparing `Scrapy-2.8.0/scrapy/templates/spiders/xmlfeed.tmpl` & `Scrapy-2.9.0/scrapy/templates/spiders/xmlfeed.tmpl`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from scrapy.spiders import XMLFeedSpider
 
 
 class $classname(XMLFeedSpider):
     name = "$name"
     allowed_domains = ["$domain"]
-    start_urls = ["http://$domain/feed.xml"]
+    start_urls = ["$url"]
     iterator = "iternodes"  # you can change this; see the docs
     itertag = "item"  # change it accordingly
 
     def parse_node(self, response, selector):
         item = {}
         #item["url"] = selector.select("url").get()
         #item["name"] = selector.select("name").get()
```

### Comparing `Scrapy-2.8.0/scrapy/utils/benchserver.py` & `Scrapy-2.9.0/scrapy/utils/benchserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from urllib.parse import urlencode
 
 from twisted.web.resource import Resource
 from twisted.web.server import Site
 
 
 class Root(Resource):
-
     isLeaf = True
 
     def getChild(self, name, request):
         return self
 
     def render(self, request):
         total = _getarg(request, b"total", 100, int)
```

### Comparing `Scrapy-2.8.0/scrapy/utils/conf.py` & `Scrapy-2.9.0/scrapy/utils/conf.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/console.py` & `Scrapy-2.9.0/scrapy/utils/console.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/curl.py` & `Scrapy-2.9.0/scrapy/utils/curl.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,33 @@
 from http.cookies import SimpleCookie
 from shlex import split
 from urllib.parse import urlparse
 
 from w3lib.http import basic_auth_header
 
 
+class DataAction(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        value = str(values)
+        if value.startswith("$"):
+            value = value[1:]
+        setattr(namespace, self.dest, value)
+
+
 class CurlParser(argparse.ArgumentParser):
     def error(self, message):
         error_msg = f"There was an error parsing the curl command: {message}"
         raise ValueError(error_msg)
 
 
 curl_parser = CurlParser()
 curl_parser.add_argument("url")
 curl_parser.add_argument("-H", "--header", dest="headers", action="append")
 curl_parser.add_argument("-X", "--request", dest="method")
-curl_parser.add_argument("-d", "--data", "--data-raw", dest="data")
+curl_parser.add_argument("-d", "--data", "--data-raw", dest="data", action=DataAction)
 curl_parser.add_argument("-u", "--user", dest="auth")
 
 
 safe_to_ignore_arguments = [
     ["--compressed"],
     # `--compressed` argument is not safe to ignore, but it's included here
     # because the `HttpCompressionMiddleware` is enabled by default
```

### Comparing `Scrapy-2.8.0/scrapy/utils/datatypes.py` & `Scrapy-2.9.0/scrapy/utils/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 import collections
 import weakref
 from collections.abc import Mapping
 
 
 class CaselessDict(dict):
-
     __slots__ = ()
 
     def __init__(self, seq=None):
         super().__init__()
         if seq:
             self.update(seq)
```

### Comparing `Scrapy-2.8.0/scrapy/utils/decorators.py` & `Scrapy-2.9.0/scrapy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/defer.py` & `Scrapy-2.9.0/scrapy/utils/defer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Coroutine,
     Generator,
     Iterable,
     Iterator,
     List,
     Optional,
     Union,
+    cast,
 )
 
 from twisted.internet import defer
 from twisted.internet.defer import Deferred, DeferredList, ensureDeferred
 from twisted.internet.task import Cooperator
 from twisted.python import failure
 from twisted.python.failure import Failure
@@ -34,29 +35,29 @@
     next reactor loop
 
     It delays by 100ms so reactor has a chance to go through readers and writers
     before attending pending delayed calls, so do not set delay to zero.
     """
     from twisted.internet import reactor
 
-    d = Deferred()
+    d: Deferred = Deferred()
     reactor.callLater(0.1, d.errback, _failure)
     return d
 
 
 def defer_succeed(result) -> Deferred:
     """Same as twisted.internet.defer.succeed but delay calling callback until
     next reactor loop
 
     It delays by 100ms so reactor has a chance to go through readers and writers
     before attending pending delayed calls, so do not set delay to zero.
     """
     from twisted.internet import reactor
 
-    d = Deferred()
+    d: Deferred = Deferred()
     reactor.callLater(0.1, d.callback, result)
     return d
 
 
 def defer_result(result) -> Deferred:
     if isinstance(result, Deferred):
         return result
@@ -80,15 +81,15 @@
         return defer_fail(failure.Failure())
     else:
         return defer_result(result)
 
 
 def parallel(
     iterable: Iterable, count: int, callable: Callable, *args, **named
-) -> DeferredList:
+) -> Deferred:
     """Execute a callable over the objects in the given iterable, in parallel,
     using no more than ``count`` concurrent calls.
 
     Taken from: https://jcalderone.livejournal.com/24285.html
     """
     coop = Cooperator()
     work = (callable(elem, *args, **named) for elem in iterable)
@@ -178,53 +179,55 @@
         self.finished = True
         for d in self.waiting_deferreds:
             d.callback(None)
 
     def _call_anext(self) -> None:
         # This starts waiting for the next result from aiterator.
         # If aiterator is exhausted, _errback will be called.
-        self.anext_deferred = deferred_from_coro(self.aiterator.__anext__())
+        self.anext_deferred = cast(
+            Deferred, deferred_from_coro(self.aiterator.__anext__())
+        )
         self.anext_deferred.addCallbacks(self._callback, self._errback)
 
     def __next__(self) -> Deferred:
         # This puts a new Deferred into self.waiting_deferreds and returns it.
         # It also calls __anext__() if needed.
         if self.finished:
             raise StopIteration
-        d = Deferred()
+        d: Deferred = Deferred()
         self.waiting_deferreds.append(d)
         if not self.anext_deferred:
             self._call_anext()
         return d
 
 
 def parallel_async(
     async_iterable: AsyncIterable, count: int, callable: Callable, *args, **named
-) -> DeferredList:
+) -> Deferred:
     """Like parallel but for async iterators"""
     coop = Cooperator()
     work = _AsyncCooperatorAdapter(async_iterable, callable, *args, **named)
-    dl = DeferredList([coop.coiterate(work) for _ in range(count)])
+    dl: Deferred = DeferredList([coop.coiterate(work) for _ in range(count)])
     return dl
 
 
 def process_chain(callbacks: Iterable[Callable], input, *a, **kw) -> Deferred:
     """Return a Deferred built by chaining the given callbacks"""
-    d = Deferred()
+    d: Deferred = Deferred()
     for x in callbacks:
         d.addCallback(x, *a, **kw)
     d.callback(input)
     return d
 
 
 def process_chain_both(
     callbacks: Iterable[Callable], errbacks: Iterable[Callable], input, *a, **kw
 ) -> Deferred:
     """Return a Deferred built by chaining the given callbacks and errbacks"""
-    d = Deferred()
+    d: Deferred = Deferred()
     for cb, eb in zip(callbacks, errbacks):
         d.addCallbacks(
             callback=cb,
             errback=eb,
             callbackArgs=a,
             callbackKeywords=kw,
             errbackArgs=a,
@@ -238,15 +241,15 @@
 
 
 def process_parallel(callbacks: Iterable[Callable], input, *a, **kw) -> Deferred:
     """Return a Deferred with the output of all successful calls to the given
     callbacks
     """
     dfds = [defer.succeed(input).addCallback(x, *a, **kw) for x in callbacks]
-    d = DeferredList(dfds, fireOnOneErrback=True, consumeErrors=True)
+    d: Deferred = DeferredList(dfds, fireOnOneErrback=True, consumeErrors=True)
     d.addCallbacks(lambda r: [x[1] for x in r], lambda f: f.value.subFailure)
     return d
 
 
 def iter_errback(iterable: Iterable, errback: Callable, *a, **kw) -> Generator:
     """Wraps an iterable calling an errback if an error is caught while
     iterating it.
@@ -281,15 +284,15 @@
     """Converts a coroutine into a Deferred, or returns the object as is if it isn't a coroutine"""
     if isinstance(o, Deferred):
         return o
     if asyncio.isfuture(o) or inspect.isawaitable(o):
         if not is_asyncio_reactor_installed():
             # wrapping the coroutine directly into a Deferred, this doesn't work correctly with coroutines
             # that use asyncio, e.g. "await asyncio.sleep(1)"
-            return ensureDeferred(o)
+            return ensureDeferred(cast(Coroutine[Deferred, Any, Any], o))
         # wrapping the coroutine into a Future and then into a Deferred, this requires AsyncioSelectorReactor
         event_loop = _get_asyncio_event_loop()
         return Deferred.fromFuture(asyncio.ensure_future(o, loop=event_loop))
     return o
 
 
 def deferred_f_from_coro_f(coro_f: Callable[..., Coroutine]) -> Callable:
```

### Comparing `Scrapy-2.8.0/scrapy/utils/deprecate.py` & `Scrapy-2.9.0/scrapy/utils/deprecate.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     Then, if user class inherits from OldName, warning is issued. Also, if
     some code uses ``issubclass(sub, OldName)`` or ``isinstance(sub(), OldName)``
     checks they'll still return True if sub is a subclass of NewName instead of
     OldName.
     """
 
     class DeprecatedClass(new_class.__class__):
-
         deprecated_class = None
         warned_on_subclass = False
 
         def __new__(metacls, name, bases, clsdict_):
             cls = super().__new__(metacls, name, bases, clsdict_)
             if metacls.deprecated_class is None:
                 metacls.deprecated_class = cls
```

### Comparing `Scrapy-2.8.0/scrapy/utils/display.py` & `Scrapy-2.9.0/scrapy/utils/display.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/engine.py` & `Scrapy-2.9.0/scrapy/utils/engine.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/ftp.py` & `Scrapy-2.9.0/scrapy/utils/ftp.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/gz.py` & `Scrapy-2.9.0/scrapy/utils/gz.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/httpobj.py` & `Scrapy-2.9.0/scrapy/utils/httpobj.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/iterators.py` & `Scrapy-2.9.0/scrapy/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/log.py` & `Scrapy-2.9.0/scrapy/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 import sys
 import warnings
 from logging.config import dictConfig
+from typing import Tuple
 
 from twisted.python import log as twisted_log
 from twisted.python.failure import Failure
 
 import scrapy
 from scrapy.exceptions import ScrapyDeprecationWarning
 from scrapy.settings import Settings
 from scrapy.utils.versions import scrapy_components_versions
 
 logger = logging.getLogger(__name__)
 
 
-def failure_to_exc_info(failure):
+def failure_to_exc_info(failure: Failure):
     """Extract exc_info from Failure instances"""
     if isinstance(failure, Failure):
         return (failure.type, failure.value, failure.getTracebackObject())
 
 
 class TopLevelFormatter(logging.Filter):
     """Keep only top level loggers's name (direct children from root) from
@@ -202,15 +203,15 @@
         self.crawler = crawler
 
     def emit(self, record):
         sname = f"log_count/{record.levelname}"
         self.crawler.stats.inc_value(sname)
 
 
-def logformatter_adapter(logkws):
+def logformatter_adapter(logkws: dict) -> Tuple[int, str, dict]:
     """
     Helper that takes the dictionary output from the methods in LogFormatter
     and adapts it into a tuple of positional arguments for logger.log calls,
     handling backward compatibility as well.
     """
     if not {"level", "msg", "args"} <= set(logkws):
         warnings.warn("Missing keys in LogFormatter method", ScrapyDeprecationWarning)
```

### Comparing `Scrapy-2.8.0/scrapy/utils/misc.py` & `Scrapy-2.9.0/scrapy/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,27 @@
 import re
 import warnings
 from collections import deque
 from contextlib import contextmanager
 from functools import partial
 from importlib import import_module
 from pkgutil import iter_modules
+from typing import TYPE_CHECKING, Any, Callable, Union
 
 from w3lib.html import replace_entities
 
 from scrapy.item import Item
 from scrapy.utils.datatypes import LocalWeakReferencedCache
 from scrapy.utils.deprecate import ScrapyDeprecationWarning
 from scrapy.utils.python import flatten, to_unicode
 
+if TYPE_CHECKING:
+    from scrapy import Spider
+
+
 _ITERABLE_SINGLE_VALUES = dict, Item, str, bytes
 
 
 def arg_to_iter(arg):
     """Convert an argument to an iterable. The argument can be a None, single
     value, or an iterable.
 
@@ -30,15 +35,15 @@
     if arg is None:
         return []
     if not isinstance(arg, _ITERABLE_SINGLE_VALUES) and hasattr(arg, "__iter__"):
         return arg
     return [arg]
 
 
-def load_object(path):
+def load_object(path: Union[str, Callable]) -> Any:
     """Load an object given its absolute object path, and return it.
 
     The object can be the import path of a class, function, variable or an
     instance, e.g. 'scrapy.downloadermiddlewares.redirect.RedirectMiddleware'.
 
     If ``path`` is not a string, but is a callable object, such as a class or
     a function, then return it as is.
@@ -245,15 +250,15 @@
                 _generator_callbacks_cache[callable] = True
                 return _generator_callbacks_cache[callable]
 
     _generator_callbacks_cache[callable] = False
     return _generator_callbacks_cache[callable]
 
 
-def warn_on_generator_with_return_value(spider, callable):
+def warn_on_generator_with_return_value(spider: "Spider", callable: Callable) -> None:
     """
     Logs a warning if a callable is a generator function and includes
     a 'return' statement with a value different than None
     """
     try:
         if is_generator_with_return_value(callable):
             warnings.warn(
```

### Comparing `Scrapy-2.8.0/scrapy/utils/ossignal.py` & `Scrapy-2.9.0/scrapy/utils/ossignal.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/project.py` & `Scrapy-2.9.0/scrapy/utils/project.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/python.py` & `Scrapy-2.9.0/scrapy/utils/python.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,24 @@
 import gc
 import inspect
 import re
 import sys
 import weakref
 from functools import partial, wraps
 from itertools import chain
-from typing import AsyncGenerator, AsyncIterable, Iterable, Union
+from typing import (
+    Any,
+    AsyncGenerator,
+    AsyncIterable,
+    Iterable,
+    Mapping,
+    Optional,
+    Union,
+    overload,
+)
 
 from scrapy.utils.asyncgen import as_async_generator
 
 
 def flatten(x):
     """flatten(sequence) -> list
 
@@ -41,15 +50,15 @@
         if is_listlike(el):
             for el_ in iflatten(el):
                 yield el_
         else:
             yield el
 
 
-def is_listlike(x):
+def is_listlike(x: Any) -> bool:
     """
     >>> is_listlike("foo")
     False
     >>> is_listlike(5)
     False
     >>> is_listlike(b"foo")
     False
@@ -78,30 +87,34 @@
         if seenkey in seen:
             continue
         seen.add(seenkey)
         result.append(item)
     return result
 
 
-def to_unicode(text, encoding=None, errors="strict"):
+def to_unicode(
+    text: Union[str, bytes], encoding: Optional[str] = None, errors: str = "strict"
+) -> str:
     """Return the unicode representation of a bytes object ``text``. If
     ``text`` is already an unicode object, return it as-is."""
     if isinstance(text, str):
         return text
     if not isinstance(text, (bytes, str)):
         raise TypeError(
             "to_unicode must receive a bytes or str "
             f"object, got {type(text).__name__}"
         )
     if encoding is None:
         encoding = "utf-8"
     return text.decode(encoding, errors)
 
 
-def to_bytes(text, encoding=None, errors="strict"):
+def to_bytes(
+    text: Union[str, bytes], encoding: Optional[str] = None, errors: str = "strict"
+) -> bytes:
     """Return the binary representation of ``text``. If ``text``
     is already a bytes object, return it as-is."""
     if isinstance(text, bytes):
         return text
     if not isinstance(text, str):
         raise TypeError(
             "to_bytes must receive a str or bytes " f"object, got {type(text).__name__}"
@@ -156,55 +169,56 @@
         if self not in cache:
             cache[self] = method(self, *args, **kwargs)
         return cache[self]
 
     return new_method
 
 
-_BINARYCHARS = {to_bytes(chr(i)) for i in range(32)} - {b"\0", b"\t", b"\n", b"\r"}
-_BINARYCHARS |= {ord(ch) for ch in _BINARYCHARS}
+_BINARYCHARS = {
+    i for i in range(32) if to_bytes(chr(i)) not in {b"\0", b"\t", b"\n", b"\r"}
+}
 
 
-def binary_is_text(data):
+def binary_is_text(data: bytes) -> bool:
     """Returns ``True`` if the given ``data`` argument (a ``bytes`` object)
     does not contain unprintable control characters.
     """
     if not isinstance(data, bytes):
         raise TypeError(f"data must be bytes, got '{type(data).__name__}'")
     return all(c not in _BINARYCHARS for c in data)
 
 
 def get_func_args(func, stripself=False):
-    """Return the argument name list of a callable"""
-    if inspect.isfunction(func):
-        spec = inspect.getfullargspec(func)
-        func_args = spec.args + spec.kwonlyargs
-    elif inspect.isclass(func):
-        return get_func_args(func.__init__, True)
-    elif inspect.ismethod(func):
-        return get_func_args(func.__func__, True)
-    elif inspect.ismethoddescriptor(func):
-        return []
-    elif isinstance(func, partial):
-        return [
-            x
-            for x in get_func_args(func.func)[len(func.args) :]
-            if not (func.keywords and x in func.keywords)
-        ]
-    elif hasattr(func, "__call__"):
-        if inspect.isroutine(func):
-            return []
-        if getattr(func, "__name__", None) == "__call__":
-            return []
-        return get_func_args(func.__call__, True)
+    """Return the argument name list of a callable object"""
+    if not callable(func):
+        raise TypeError(f"func must be callable, got '{type(func).__name__}'")
+
+    args = []
+    try:
+        sig = inspect.signature(func)
+    except ValueError:
+        return args
+
+    if isinstance(func, partial):
+        partial_args = func.args
+        partial_kw = func.keywords
+
+        for name, param in sig.parameters.items():
+            if param.name in partial_args:
+                continue
+            if partial_kw and param.name in partial_kw:
+                continue
+            args.append(name)
     else:
-        raise TypeError(f"{type(func)} is not callable")
-    if stripself:
-        func_args.pop(0)
-    return func_args
+        for name in sig.parameters.keys():
+            args.append(name)
+
+    if stripself and args and args[0] == "self":
+        args = args[1:]
+    return args
 
 
 def get_spec(func):
     """Returns (args, kwargs) tuple for a function
     >>> import re
     >>> get_spec(re.match)
     (['pattern', 'string'], {'flags': 0})
@@ -254,14 +268,24 @@
                 return False
         elif getattr(obj1, attr, temp1) != getattr(obj2, attr, temp2):
             return False
     # all attributes equal
     return True
 
 
+@overload
+def without_none_values(iterable: Mapping) -> dict:
+    ...
+
+
+@overload
+def without_none_values(iterable: Iterable) -> Iterable:
+    ...
+
+
 def without_none_values(iterable):
     """Return a copy of ``iterable`` with all ``None`` entries removed.
 
     If ``iterable`` is a mapping, return a dictionary where all pairs that have
     value ``None`` have been removed.
     """
     try:
```

### Comparing `Scrapy-2.8.0/scrapy/utils/reactor.py` & `Scrapy-2.9.0/scrapy/utils/reactor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import asyncio
 import sys
 from contextlib import suppress
-from warnings import catch_warnings, filterwarnings
+from typing import Any, Callable, Dict, Optional, Sequence
+from warnings import catch_warnings, filterwarnings, warn
 
 from twisted.internet import asyncioreactor, error
+from twisted.internet.base import DelayedCall
 
+from scrapy.exceptions import ScrapyDeprecationWarning
 from scrapy.utils.misc import load_object
 
 
 def listen_tcp(portrange, host, factory):
     """Like reactor.listenTCP but tries different ports in a range."""
     from twisted.internet import reactor
 
@@ -29,54 +32,78 @@
 
 
 class CallLaterOnce:
     """Schedule a function to be called in the next reactor loop, but only if
     it hasn't been already scheduled since the last time it ran.
     """
 
-    def __init__(self, func, *a, **kw):
-        self._func = func
-        self._a = a
-        self._kw = kw
-        self._call = None
+    def __init__(self, func: Callable, *a: Any, **kw: Any):
+        self._func: Callable = func
+        self._a: Sequence[Any] = a
+        self._kw: Dict[str, Any] = kw
+        self._call: Optional[DelayedCall] = None
 
-    def schedule(self, delay=0):
+    def schedule(self, delay: float = 0) -> None:
         from twisted.internet import reactor
 
         if self._call is None:
             self._call = reactor.callLater(delay, self)
 
-    def cancel(self):
+    def cancel(self) -> None:
         if self._call:
             self._call.cancel()
 
-    def __call__(self):
+    def __call__(self) -> Any:
         self._call = None
         return self._func(*self._a, **self._kw)
 
 
+def set_asyncio_event_loop_policy():
+    """The policy functions from asyncio often behave unexpectedly,
+    so we restrict their use to the absolutely essential case.
+    This should only be used to install the reactor.
+    """
+    _get_asyncio_event_loop_policy()
+
+
 def get_asyncio_event_loop_policy():
+    warn(
+        "Call to deprecated function "
+        "scrapy.utils.reactor.get_asyncio_event_loop_policy().\n"
+        "\n"
+        "Please use get_event_loop, new_event_loop and set_event_loop"
+        " from asyncio instead, as the corresponding policy methods may lead"
+        " to unexpected behaviour.\n"
+        "This function is replaced by set_asyncio_event_loop_policy and"
+        " is meant to be used only when the reactor is being installed.",
+        category=ScrapyDeprecationWarning,
+        stacklevel=2,
+    )
+    return _get_asyncio_event_loop_policy()
+
+
+def _get_asyncio_event_loop_policy():
     policy = asyncio.get_event_loop_policy()
     if (
         sys.version_info >= (3, 8)
         and sys.platform == "win32"
         and not isinstance(policy, asyncio.WindowsSelectorEventLoopPolicy)
     ):
         policy = asyncio.WindowsSelectorEventLoopPolicy()
         asyncio.set_event_loop_policy(policy)
-
     return policy
 
 
 def install_reactor(reactor_path, event_loop_path=None):
     """Installs the :mod:`~twisted.internet.reactor` with the specified
     import path. Also installs the asyncio event loop with the specified import
     path if the asyncio reactor is enabled"""
     reactor_class = load_object(reactor_path)
     if reactor_class is asyncioreactor.AsyncioSelectorReactor:
+        set_asyncio_event_loop_policy()
         with suppress(error.ReactorAlreadyInstalledError):
             event_loop = set_asyncio_event_loop(event_loop_path)
             asyncioreactor.install(eventloop=event_loop)
     else:
         *module, _ = reactor_path.split(".")
         installer_path = module + ["install"]
         installer = load_object(".".join(installer_path))
@@ -86,15 +113,14 @@
 
 def _get_asyncio_event_loop():
     return set_asyncio_event_loop(None)
 
 
 def set_asyncio_event_loop(event_loop_path):
     """Sets and returns the event loop with specified import path."""
-    policy = get_asyncio_event_loop_policy()
     if event_loop_path is not None:
         event_loop_class = load_object(event_loop_path)
         event_loop = event_loop_class()
         asyncio.set_event_loop(event_loop)
     else:
         try:
             with catch_warnings():
@@ -105,23 +131,21 @@
                 # prepared for that future behavior, we ignore the deprecation
                 # warning.
                 filterwarnings(
                     "ignore",
                     message="There is no current event loop",
                     category=DeprecationWarning,
                 )
-                event_loop = policy.get_event_loop()
+                event_loop = asyncio.get_event_loop()
         except RuntimeError:
             # `get_event_loop` raises RuntimeError when called with no asyncio
             # event loop yet installed in the following scenarios:
-            # - From a thread other than the main thread. For example, when
-            #   using ``scrapy shell``.
             # - Previsibly on Python 3.14 and later.
             #   https://github.com/python/cpython/issues/100160#issuecomment-1345581902
-            event_loop = policy.new_event_loop()
+            event_loop = asyncio.new_event_loop()
             asyncio.set_event_loop(event_loop)
     return event_loop
 
 
 def verify_installed_reactor(reactor_path):
     """Raises :exc:`Exception` if the installed
     :mod:`~twisted.internet.reactor` does not match the specified import
```

### Comparing `Scrapy-2.8.0/scrapy/utils/reqser.py` & `Scrapy-2.9.0/scrapy/utils/reqser.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/request.py` & `Scrapy-2.9.0/scrapy/utils/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,7 +323,38 @@
 def _get_method(obj, name):
     """Helper function for request_from_dict"""
     name = str(name)
     try:
         return getattr(obj, name)
     except AttributeError:
         raise ValueError(f"Method {name!r} not found in: {obj}")
+
+
+def request_to_curl(request: Request) -> str:
+    """
+    Converts a :class:`~scrapy.Request` object to a curl command.
+
+    :param :class:`~scrapy.Request`: Request object to be converted
+    :return: string containing the curl command
+    """
+    method = request.method
+
+    data = f"--data-raw '{request.body.decode('utf-8')}'" if request.body else ""
+
+    headers = " ".join(
+        f"-H '{k.decode()}: {v[0].decode()}'" for k, v in request.headers.items()
+    )
+
+    url = request.url
+    cookies = ""
+    if request.cookies:
+        if isinstance(request.cookies, dict):
+            cookie = "; ".join(f"{k}={v}" for k, v in request.cookies.items())
+            cookies = f"--cookie '{cookie}'"
+        elif isinstance(request.cookies, list):
+            cookie = "; ".join(
+                f"{list(c.keys())[0]}={list(c.values())[0]}" for c in request.cookies
+            )
+            cookies = f"--cookie '{cookie}'"
+
+    curl_cmd = f"curl -X {method} {url} {data} {headers} {cookies}".strip()
+    return " ".join(curl_cmd.split())
```

### Comparing `Scrapy-2.8.0/scrapy/utils/response.py` & `Scrapy-2.9.0/scrapy/utils/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module provides some useful functions for working with
 scrapy.http.Response objects
 """
 import os
 import re
 import tempfile
 import webbrowser
-from typing import Any, Callable, Iterable, Optional, Tuple, Union
+from typing import Any, Callable, Iterable, Tuple, Union
 from weakref import WeakKeyDictionary
 
 from twisted.web import http
 from w3lib import html
 
 import scrapy
 from scrapy.http.response import Response
@@ -33,20 +33,21 @@
 _metaref_cache: "WeakKeyDictionary[Response, Union[Tuple[None, None], Tuple[float, str]]]" = (
     WeakKeyDictionary()
 )
 
 
 def get_meta_refresh(
     response: "scrapy.http.response.text.TextResponse",
-    ignore_tags: Optional[Iterable[str]] = ("script", "noscript"),
+    ignore_tags: Iterable[str] = ("script", "noscript"),
 ) -> Union[Tuple[None, None], Tuple[float, str]]:
     """Parse the http-equiv refresh parameter from the given response"""
     if response not in _metaref_cache:
         text = response.text[0:4096]
-        _metaref_cache[response] = html.get_meta_refresh(
+        # a w3lib typing bug here, fixed in https://github.com/scrapy/w3lib/pull/211
+        _metaref_cache[response] = html.get_meta_refresh(  # type: ignore[assignment]
             text, response.url, response.encoding, ignore_tags=ignore_tags
         )
     return _metaref_cache[response]
 
 
 def response_status_message(status: Union[bytes, float, int, str]) -> str:
     """Return status code plus status text descriptive message"""
```

### Comparing `Scrapy-2.8.0/scrapy/utils/serialize.py` & `Scrapy-2.9.0/scrapy/utils/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from itemadapter import ItemAdapter, is_item
 from twisted.internet import defer
 
 from scrapy.http import Request, Response
 
 
 class ScrapyJSONEncoder(json.JSONEncoder):
-
     DATE_FORMAT = "%Y-%m-%d"
     TIME_FORMAT = "%H:%M:%S"
 
     def default(self, o):
         if isinstance(o, set):
             return list(o)
         if isinstance(o, datetime.datetime):
```

### Comparing `Scrapy-2.8.0/scrapy/utils/signal.py` & `Scrapy-2.9.0/scrapy/utils/signal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Helper functions for working with signals"""
 import collections.abc
 import logging
+from typing import Any as TypingAny
+from typing import List, Tuple
 
 from pydispatch.dispatcher import (
     Anonymous,
     Any,
     disconnect,
     getAllReceivers,
     liveReceivers,
@@ -16,28 +18,31 @@
 from scrapy.exceptions import StopDownload
 from scrapy.utils.defer import maybeDeferred_coro
 from scrapy.utils.log import failure_to_exc_info
 
 logger = logging.getLogger(__name__)
 
 
-def send_catch_log(signal=Any, sender=Anonymous, *arguments, **named):
+def send_catch_log(
+    signal=Any, sender=Anonymous, *arguments, **named
+) -> List[Tuple[TypingAny, TypingAny]]:
     """Like pydispatcher.robust.sendRobust but it also logs errors and returns
     Failures instead of exceptions.
     """
     dont_log = named.pop("dont_log", ())
     dont_log = (
         tuple(dont_log)
         if isinstance(dont_log, collections.abc.Sequence)
         else (dont_log,)
     )
     dont_log += (StopDownload,)
     spider = named.get("spider", None)
-    responses = []
+    responses: List[Tuple[TypingAny, TypingAny]] = []
     for receiver in liveReceivers(getAllReceivers(sender, signal)):
+        result: TypingAny
         try:
             response = robustApply(
                 receiver, signal=signal, sender=sender, *arguments, **named
             )
             if isinstance(response, Deferred):
                 logger.error(
                     "Cannot return deferreds from signal handler: %(receiver)s",
```

### Comparing `Scrapy-2.8.0/scrapy/utils/sitemap.py` & `Scrapy-2.9.0/scrapy/utils/sitemap.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/spider.py` & `Scrapy-2.9.0/scrapy/utils/spider.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/ssl.py` & `Scrapy-2.9.0/scrapy/utils/ssl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+from typing import Any, Optional, cast
+
 import OpenSSL._util as pyOpenSSLutil
 import OpenSSL.SSL
+import OpenSSL.version
+from OpenSSL.crypto import X509Name
 
 from scrapy.utils.python import to_unicode
 
 
-def ffi_buf_to_string(buf):
+def ffi_buf_to_string(buf: Any) -> str:
     return to_unicode(pyOpenSSLutil.ffi.string(buf))
 
 
-def x509name_to_string(x509name):
+def x509name_to_string(x509name: X509Name) -> str:
     # from OpenSSL.crypto.X509Name.__repr__
-    result_buffer = pyOpenSSLutil.ffi.new("char[]", 512)
+    result_buffer: Any = pyOpenSSLutil.ffi.new("char[]", 512)
     pyOpenSSLutil.lib.X509_NAME_oneline(
-        x509name._name, result_buffer, len(result_buffer)
+        x509name._name, result_buffer, len(result_buffer)  # type: ignore[attr-defined]
     )
 
     return ffi_buf_to_string(result_buffer)
 
 
-def get_temp_key_info(ssl_object):
+def get_temp_key_info(ssl_object: Any) -> Optional[str]:
     # adapted from OpenSSL apps/s_cb.c::ssl_print_tmp_key()
+    if not hasattr(pyOpenSSLutil.lib, "SSL_get_server_tmp_key"):
+        # removed in cryptography 40.0.0
+        return None
     temp_key_p = pyOpenSSLutil.ffi.new("EVP_PKEY **")
     if not pyOpenSSLutil.lib.SSL_get_server_tmp_key(ssl_object, temp_key_p):
         return None
     temp_key = temp_key_p[0]
     if temp_key == pyOpenSSLutil.ffi.NULL:
         return None
     temp_key = pyOpenSSLutil.ffi.gc(temp_key, pyOpenSSLutil.lib.EVP_PKEY_free)
@@ -46,12 +53,14 @@
         key_info.append(ffi_buf_to_string(cname))
     else:
         key_info.append(ffi_buf_to_string(pyOpenSSLutil.lib.OBJ_nid2sn(key_type)))
     key_info.append(f"{pyOpenSSLutil.lib.EVP_PKEY_bits(temp_key)} bits")
     return ", ".join(key_info)
 
 
-def get_openssl_version():
-    system_openssl = OpenSSL.SSL.SSLeay_version(OpenSSL.SSL.SSLEAY_VERSION).decode(
-        "ascii", errors="replace"
+def get_openssl_version() -> str:
+    # https://github.com/python/typeshed/issues/10024
+    system_openssl_bytes = cast(
+        bytes, OpenSSL.SSL.SSLeay_version(OpenSSL.SSL.SSLEAY_VERSION)
     )
+    system_openssl = system_openssl_bytes.decode("ascii", errors="replace")
     return f"{OpenSSL.version.__version__} ({system_openssl})"
```

### Comparing `Scrapy-2.8.0/scrapy/utils/template.py` & `Scrapy-2.9.0/scrapy/utils/template.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/test.py` & `Scrapy-2.9.0/scrapy/utils/test.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/testproc.py` & `Scrapy-2.9.0/scrapy/utils/testproc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import sys
 
 from twisted.internet import defer, protocol
 
 
 class ProcessTest:
-
     command = None
     prefix = [sys.executable, "-m", "scrapy.cmdline"]
     cwd = os.getcwd()  # trial chdirs to temp dir
 
     def execute(self, args, check_code=True, settings=None):
         from twisted.internet import reactor
```

### Comparing `Scrapy-2.8.0/scrapy/utils/testsite.py` & `Scrapy-2.9.0/scrapy/utils/testsite.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/trackref.py` & `Scrapy-2.9.0/scrapy/utils/trackref.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/scrapy/utils/url.py` & `Scrapy-2.9.0/scrapy/utils/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
 def strip_url(
     url,
     strip_credentials=True,
     strip_default_port=True,
     origin_only=False,
     strip_fragment=True,
 ):
-
     """Strip URL string from some of its components:
 
     - ``strip_credentials`` removes "user:password@"
     - ``strip_default_port`` removes ":80" (resp. ":443", ":21")
       from http:// (resp. https://, ftp://) URLs
     - ``origin_only`` replaces path component with "/", also dropping
       query and fragment components ; it also strips credentials
```

### Comparing `Scrapy-2.8.0/scrapy/utils/versions.py` & `Scrapy-2.9.0/scrapy/utils/versions.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/setup.cfg` & `Scrapy-2.9.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 doc_files = docs AUTHORS INSTALL LICENSE README.rst
 
 [bdist_wheel]
 universal = 1
 
 [mypy]
 ignore_missing_imports = true
+
+[mypy-twisted.internet.interfaces]
+follow_imports = skip
+
+[mypy-twisted.internet.reactor]
 follow_imports = skip
 
 [mypy-scrapy.downloadermiddlewares.httpproxy]
 ignore_errors = True
 
 [mypy-scrapy.interfaces]
 ignore_errors = True
```

### Comparing `Scrapy-2.8.0/setup.py` & `Scrapy-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/asyncio_deferred_signal.py` & `Scrapy-2.9.0/tests/CrawlerProcess/asyncio_deferred_signal.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/asyncio_enabled_reactor.py` & `Scrapy-2.9.0/tests/CrawlerProcess/asyncio_enabled_reactor.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py` & `Scrapy-2.9.0/tests/CrawlerProcess/asyncio_enabled_reactor_different_loop.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py` & `Scrapy-2.9.0/tests/CrawlerProcess/asyncio_enabled_reactor_same_loop.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/caching_hostname_resolver.py` & `Scrapy-2.9.0/tests/CrawlerProcess/caching_hostname_resolver.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py` & `Scrapy-2.9.0/tests/CrawlerProcess/caching_hostname_resolver_ipv6.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py` & `Scrapy-2.9.0/tests/CrawlerProcess/reactor_select_subclass_twisted_reactor_select.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py` & `Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_custom_settings_conflict.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py` & `Scrapy-2.9.0/tests/CrawlerProcess/twisted_reactor_custom_settings_same.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/CrawlerRunner/ip_address.py` & `Scrapy-2.9.0/tests/CrawlerRunner/ip_address.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/__init__.py` & `Scrapy-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/ftpserver.py` & `Scrapy-2.9.0/tests/ftpserver.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/__init__.py` & `Scrapy-2.9.0/tests/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/example-com.cert.pem` & `Scrapy-2.9.0/tests/keys/example-com.cert.pem`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/example-com.conf` & `Scrapy-2.9.0/tests/keys/example-com.conf`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/example-com.gen.README` & `Scrapy-2.9.0/tests/keys/example-com.gen.README`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/example-com.key.pem` & `Scrapy-2.9.0/tests/keys/example-com.key.pem`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/localhost-ip.gen.README` & `Scrapy-2.9.0/tests/keys/localhost-ip.gen.README`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/localhost.gen.README` & `Scrapy-2.9.0/tests/keys/localhost.gen.README`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/localhost.ip.crt` & `Scrapy-2.9.0/tests/keys/localhost.ip.crt`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/localhost.ip.key` & `Scrapy-2.9.0/tests/keys/localhost.ip.key`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/keys/mitmproxy-ca.pem` & `Scrapy-2.9.0/tests/keys/mitmproxy-ca.pem`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/mockserver.py` & `Scrapy-2.9.0/tests/mockserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from shutil import rmtree
 from subprocess import PIPE, Popen
 from tempfile import mkdtemp
 from urllib.parse import urlencode
 
 from OpenSSL import SSL
 from twisted.internet import defer, reactor, ssl
+from twisted.internet.protocol import ServerFactory
 from twisted.internet.task import deferLater
 from twisted.names import dns, error
 from twisted.names.server import DNSServerFactory
 from twisted.web import resource, server
 from twisted.web.server import NOT_DONE_YET, GzipEncoderFactory, Site
 from twisted.web.static import File
 from twisted.web.util import redirectTo
@@ -91,15 +92,14 @@
         # only sends 3 bytes even though it claims to send 5
         request.setHeader(b"content-length", b"5")
         request.write(b"abc")
         return b""
 
 
 class LeafResource(resource.Resource):
-
     isLeaf = True
 
     def deferRequest(self, request, delay, f, *a, **kw):
         def _cancelrequest(_):
             # silence CancelledError
             d.addErrback(lambda _: None)
             d.cancel()
@@ -365,14 +365,16 @@
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-t", "--type", type=str, choices=("http", "dns"), default="http"
     )
     args = parser.parse_args()
 
+    factory: ServerFactory
+
     if args.type == "http":
         root = Root()
         factory = Site(root)
         httpPort = reactor.listenTCP(0, factory)
         contextFactory = ssl_context_factory()
         httpsPort = reactor.listenSSL(0, factory, contextFactory)
```

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.tar` & `Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.tar`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.xml` & `Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.xml`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.xml.bz2` & `Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.xml.bz2`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.xml.gz` & `Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.xml.gz`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/feed-sample1.zip` & `Scrapy-2.9.0/tests/sample_data/compressed/feed-sample1.zip`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/html-br.bin` & `Scrapy-2.9.0/tests/sample_data/compressed/html-br.bin`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/html-gzip.bin` & `Scrapy-2.9.0/tests/sample_data/compressed/html-gzip.bin`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/html-rawdeflate.bin` & `Scrapy-2.9.0/tests/sample_data/compressed/html-rawdeflate.bin`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/html-zlibdeflate.bin` & `Scrapy-2.9.0/tests/sample_data/compressed/html-zlibdeflate.bin`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/html-zstd-static-content-size.bin` & `Scrapy-2.9.0/tests/sample_data/compressed/html-zstd-static-content-size.bin`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/html-zstd-static-no-content-size.bin` & `Scrapy-2.9.0/tests/sample_data/compressed/html-zstd-static-no-content-size.bin`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin` & `Scrapy-2.9.0/tests/sample_data/compressed/html-zstd-streaming-no-content-size.bin`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/truncated-crc-error-short.gz` & `Scrapy-2.9.0/tests/sample_data/compressed/truncated-crc-error-short.gz`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/truncated-crc-error.gz` & `Scrapy-2.9.0/tests/sample_data/compressed/truncated-crc-error.gz`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/unexpected-eof-output.txt` & `Scrapy-2.9.0/tests/sample_data/compressed/unexpected-eof-output.txt`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/compressed/unexpected-eof.gz` & `Scrapy-2.9.0/tests/sample_data/compressed/unexpected-eof.gz`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/feeds/feed-sample1.xml` & `Scrapy-2.9.0/tests/sample_data/feeds/feed-sample1.xml`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/feeds/feed-sample2.xml` & `Scrapy-2.9.0/tests/sample_data/feeds/feed-sample2.xml`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/link_extractor/linkextractor.html` & `Scrapy-2.9.0/tests/sample_data/link_extractor/linkextractor.html`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/link_extractor/linkextractor_latin1.html` & `Scrapy-2.9.0/tests/sample_data/link_extractor/linkextractor_latin1.html`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/link_extractor/linkextractor_no_href.html` & `Scrapy-2.9.0/tests/sample_data/link_extractor/linkextractor_no_href.html`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png` & `Scrapy-2.9.0/tests/sample_data/test_site/files/images/python-logo-master-v3-TM-flattened.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/test_site/files/images/python-powered-h-50x65.png` & `Scrapy-2.9.0/tests/sample_data/test_site/files/images/python-powered-h-50x65.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/sample_data/test_site/files/images/scrapy.png` & `Scrapy-2.9.0/tests/sample_data/test_site/files/images/scrapy.png`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/spiders.py` & `Scrapy-2.9.0/tests/spiders.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,25 @@
 class MockServerSpider(Spider):
     def __init__(self, mockserver=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.mockserver = mockserver
 
 
 class MetaSpider(MockServerSpider):
-
     name = "meta"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta = {}
 
     def closed(self, reason):
         self.meta["close_reason"] = reason
 
 
 class FollowAllSpider(MetaSpider):
-
     name = "follow"
     link_extractor = LinkExtractor()
 
     def __init__(
         self, total=10, show=20, order="rand", maxlatency=0.0, *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
@@ -55,15 +53,14 @@
         self.urls_visited.append(response.url)
         self.times.append(time.time())
         for link in self.link_extractor.extract_links(response):
             yield Request(link.url, callback=self.parse)
 
 
 class DelaySpider(MetaSpider):
-
     name = "delay"
 
     def __init__(self, n=1, b=0, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.n = n
         self.b = b
         self.t1 = self.t2 = self.t2_err = 0
@@ -77,68 +74,62 @@
         self.t2 = time.time()
 
     def errback(self, failure):
         self.t2_err = time.time()
 
 
 class SimpleSpider(MetaSpider):
-
     name = "simple"
 
     def __init__(self, url="http://localhost:8998", *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.start_urls = [url]
 
     def parse(self, response):
         self.logger.info(f"Got response {response.status}")
 
 
 class AsyncDefSpider(SimpleSpider):
-
     name = "asyncdef"
 
     async def parse(self, response):
         await defer.succeed(42)
         self.logger.info(f"Got response {response.status}")
 
 
 class AsyncDefAsyncioSpider(SimpleSpider):
-
     name = "asyncdef_asyncio"
 
     async def parse(self, response):
         await asyncio.sleep(0.2)
         status = await get_from_asyncio_queue(response.status)
         self.logger.info(f"Got response {status}")
 
 
 class AsyncDefAsyncioReturnSpider(SimpleSpider):
-
     name = "asyncdef_asyncio_return"
 
     async def parse(self, response):
         await asyncio.sleep(0.2)
         status = await get_from_asyncio_queue(response.status)
         self.logger.info(f"Got response {status}")
         return [{"id": 1}, {"id": 2}]
 
 
 class AsyncDefAsyncioReturnSingleElementSpider(SimpleSpider):
-
     name = "asyncdef_asyncio_return_single_element"
 
     async def parse(self, response):
         await asyncio.sleep(0.1)
         status = await get_from_asyncio_queue(response.status)
         self.logger.info(f"Got response {status}")
         return {"foo": 42}
 
 
 class AsyncDefAsyncioReqsReturnSpider(SimpleSpider):
-
     name = "asyncdef_asyncio_reqs_return"
 
     async def parse(self, response):
         await asyncio.sleep(0.2)
         req_id = response.meta.get("req_id", 0)
         status = await get_from_asyncio_queue(response.status)
         self.logger.info(f"Got response {status}, req_id {req_id}")
@@ -187,36 +178,33 @@
         resp = await maybe_deferred_to_future(
             get_web_client_agent_req(self.mockserver.url("/status?n=200"))
         )
         yield {"code": resp.code}
 
 
 class AsyncDefAsyncioGenSpider(SimpleSpider):
-
     name = "asyncdef_asyncio_gen"
 
     async def parse(self, response):
         await asyncio.sleep(0.2)
         yield {"foo": 42}
         self.logger.info(f"Got response {response.status}")
 
 
 class AsyncDefAsyncioGenLoopSpider(SimpleSpider):
-
     name = "asyncdef_asyncio_gen_loop"
 
     async def parse(self, response):
         for i in range(10):
             await asyncio.sleep(0.1)
             yield {"foo": i}
         self.logger.info(f"Got response {response.status}")
 
 
 class AsyncDefAsyncioGenComplexSpider(SimpleSpider):
-
     name = "asyncdef_asyncio_gen_complex"
     initial_reqs = 4
     following_reqs = 3
     depth = 2
 
     def _get_req(self, index, cb=None):
         return Request(
@@ -242,44 +230,41 @@
 
     async def parse2(self, response):
         await asyncio.sleep(0.1)
         yield {"index2": response.meta["index"]}
 
 
 class ItemSpider(FollowAllSpider):
-
     name = "item"
 
     def parse(self, response):
         for request in super().parse(response):
             yield request
             yield Item()
             yield {}
 
 
 class DefaultError(Exception):
     pass
 
 
 class ErrorSpider(FollowAllSpider):
-
     name = "error"
     exception_cls = DefaultError
 
     def raise_exception(self):
         raise self.exception_cls("Expected exception")
 
     def parse(self, response):
         for request in super().parse(response):
             yield request
             self.raise_exception()
 
 
 class BrokenStartRequestsSpider(FollowAllSpider):
-
     fail_before_yield = False
     fail_yielding = False
 
     def __init__(self, *a, **kw):
         super().__init__(*a, **kw)
         self.seedsseen = []
 
@@ -301,15 +286,14 @@
     def parse(self, response):
         self.seedsseen.append(response.meta.get("seed"))
         for req in super().parse(response):
             yield req
 
 
 class SingleRequestSpider(MetaSpider):
-
     seed = None
     callback_func = None
     errback_func = None
 
     def start_requests(self):
         if isinstance(self.seed, Request):
             yield self.seed.replace(callback=self.parse, errback=self.on_error)
@@ -447,15 +431,14 @@
 
     def process_request(self, request, response):
         request.cb_kwargs["foo"] = "process_request"
         return request
 
 
 class BytesReceivedCallbackSpider(MetaSpider):
-
     full_response_length = 2**18
 
     @classmethod
     def from_crawler(cls, crawler, *args, **kwargs):
         spider = super().from_crawler(crawler, *args, **kwargs)
         crawler.signals.connect(spider.bytes_received, signals.bytes_received)
         return spider
```

### Comparing `Scrapy-2.8.0/tests/test_closespider.py` & `Scrapy-2.9.0/tests/test_closespider.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_cmdline/__init__.py` & `Scrapy-2.9.0/tests/test_cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_cmdline_crawl_with_pipeline/__init__.py` & `Scrapy-2.9.0/tests/test_cmdline_crawl_with_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_command_fetch.py` & `Scrapy-2.9.0/tests/test_command_fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from twisted.trial import unittest
 
 from scrapy.utils.testproc import ProcessTest
 from scrapy.utils.testsite import SiteTest
 
 
 class FetchTest(ProcessTest, SiteTest, unittest.TestCase):
-
     command = "fetch"
 
     @defer.inlineCallbacks
     def test_output(self):
         _, out, _ = yield self.execute([self.url("/text")])
         self.assertEqual(out.strip(), b"Works")
```

### Comparing `Scrapy-2.8.0/tests/test_command_parse.py` & `Scrapy-2.9.0/tests/test_command_parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,22 +26,61 @@
         self.spider_name = "parse_spider"
         (self.proj_mod_path / "spiders" / "myspider.py").write_text(
             f"""
 import scrapy
 from scrapy.linkextractors import LinkExtractor
 from scrapy.spiders import CrawlSpider, Rule
 from scrapy.utils.test import get_from_asyncio_queue
+import asyncio
 
-class AsyncDefAsyncioSpider(scrapy.Spider):
 
-    name = 'asyncdef{self.spider_name}'
+class AsyncDefAsyncioReturnSpider(scrapy.Spider):
+    name = "asyncdef_asyncio_return"
 
     async def parse(self, response):
+        await asyncio.sleep(0.2)
         status = await get_from_asyncio_queue(response.status)
-        return [scrapy.Item(), dict(foo='bar')]
+        self.logger.info(f"Got response {{status}}")
+        return [{{'id': 1}}, {{'id': 2}}]
+
+class AsyncDefAsyncioReturnSingleElementSpider(scrapy.Spider):
+    name = "asyncdef_asyncio_return_single_element"
+
+    async def parse(self, response):
+        await asyncio.sleep(0.1)
+        status = await get_from_asyncio_queue(response.status)
+        self.logger.info(f"Got response {{status}}")
+        return {{'foo': 42}}
+
+class AsyncDefAsyncioGenLoopSpider(scrapy.Spider):
+    name = "asyncdef_asyncio_gen_loop"
+
+    async def parse(self, response):
+        for i in range(10):
+            await asyncio.sleep(0.1)
+            yield {{'foo': i}}
+        self.logger.info(f"Got response {{response.status}}")
+
+class AsyncDefAsyncioSpider(scrapy.Spider):
+    name = "asyncdef_asyncio"
+
+    async def parse(self, response):
+        await asyncio.sleep(0.2)
+        status = await get_from_asyncio_queue(response.status)
+        self.logger.debug(f"Got response {{status}}")
+
+class AsyncDefAsyncioGenExcSpider(scrapy.Spider):
+    name = "asyncdef_asyncio_gen_exc"
+
+    async def parse(self, response):
+        for i in range(10):
+            await asyncio.sleep(0.1)
+            yield {{'foo': i}}
+            if i > 5:
+                raise ValueError("Stopping the processing")
 
 class MySpider(scrapy.Spider):
     name = '{self.spider_name}'
 
     def parse(self, response):
         if getattr(self, 'test_arg', None):
             self.logger.debug('It Works!')
@@ -209,25 +248,84 @@
                 "--verbose",
                 self.url("/html"),
             ]
         )
         self.assertIn("INFO: It Works!", _textmode(stderr))
 
     @defer.inlineCallbacks
-    def test_asyncio_parse_items(self):
+    def test_async_def_asyncio_parse_items_list(self):
         status, out, stderr = yield self.execute(
             [
                 "--spider",
-                "asyncdef" + self.spider_name,
+                "asyncdef_asyncio_return",
                 "-c",
                 "parse",
                 self.url("/html"),
             ]
         )
-        self.assertIn("""[{}, {'foo': 'bar'}]""", _textmode(out))
+        self.assertIn("INFO: Got response 200", _textmode(stderr))
+        self.assertIn("{'id': 1}", _textmode(out))
+        self.assertIn("{'id': 2}", _textmode(out))
+
+    @defer.inlineCallbacks
+    def test_async_def_asyncio_parse_items_single_element(self):
+        status, out, stderr = yield self.execute(
+            [
+                "--spider",
+                "asyncdef_asyncio_return_single_element",
+                "-c",
+                "parse",
+                self.url("/html"),
+            ]
+        )
+        self.assertIn("INFO: Got response 200", _textmode(stderr))
+        self.assertIn("{'foo': 42}", _textmode(out))
+
+    @defer.inlineCallbacks
+    def test_async_def_asyncgen_parse_loop(self):
+        status, out, stderr = yield self.execute(
+            [
+                "--spider",
+                "asyncdef_asyncio_gen_loop",
+                "-c",
+                "parse",
+                self.url("/html"),
+            ]
+        )
+        self.assertIn("INFO: Got response 200", _textmode(stderr))
+        for i in range(10):
+            self.assertIn(f"{{'foo': {i}}}", _textmode(out))
+
+    @defer.inlineCallbacks
+    def test_async_def_asyncgen_parse_exc(self):
+        status, out, stderr = yield self.execute(
+            [
+                "--spider",
+                "asyncdef_asyncio_gen_exc",
+                "-c",
+                "parse",
+                self.url("/html"),
+            ]
+        )
+        self.assertIn("ValueError", _textmode(stderr))
+        for i in range(7):
+            self.assertIn(f"{{'foo': {i}}}", _textmode(out))
+
+    @defer.inlineCallbacks
+    def test_async_def_asyncio_parse(self):
+        _, _, stderr = yield self.execute(
+            [
+                "--spider",
+                "asyncdef_asyncio",
+                "-c",
+                "parse",
+                self.url("/html"),
+            ]
+        )
+        self.assertIn("DEBUG: Got response 200", _textmode(stderr))
 
     @defer.inlineCallbacks
     def test_parse_items(self):
         status, out, stderr = yield self.execute(
             ["--spider", self.spider_name, "-c", "parse", self.url("/html")]
         )
         self.assertIn("""[{}, {'foo': 'bar'}]""", _textmode(out))
```

### Comparing `Scrapy-2.8.0/tests/test_command_shell.py` & `Scrapy-2.9.0/tests/test_command_shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from scrapy.utils.testproc import ProcessTest
 from scrapy.utils.testsite import SiteTest
 from tests import NON_EXISTING_RESOLVABLE, tests_datadir
 
 
 class ShellTest(ProcessTest, SiteTest, unittest.TestCase):
-
     command = "shell"
 
     @defer.inlineCallbacks
     def test_empty(self):
         _, out, _ = yield self.execute(["-c", "item"])
         assert b"{}" in out
```

### Comparing `Scrapy-2.8.0/tests/test_command_version.py` & `Scrapy-2.9.0/tests/test_command_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from twisted.trial import unittest
 
 import scrapy
 from scrapy.utils.testproc import ProcessTest
 
 
 class VersionTest(ProcessTest, unittest.TestCase):
-
     command = "version"
 
     @defer.inlineCallbacks
     def test_output(self):
         encoding = getattr(sys.stdout, "encoding") or "utf-8"
         _, out, _ = yield self.execute([])
         self.assertEqual(
```

### Comparing `Scrapy-2.8.0/tests/test_commands.py` & `Scrapy-2.9.0/tests/test_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,15 +219,14 @@
                 relative_path = relative_path.replace(search_string, replacement)
             permissions = get_permissions(absolute_path)
             permissions_dict[relative_path] = permissions
     return permissions_dict
 
 
 class StartprojectTemplatesTest(ProjectTest):
-
     maxDiff = None
 
     def setUp(self):
         super().setUp()
         self.tmpl = str(Path(self.temp_path, "templates"))
         self.tmpl_proj = str(Path(self.tmpl, "project"))
 
@@ -538,29 +537,80 @@
             domain,
             self.find_in_file(
                 Path(self.proj_mod_path, "spiders", "test_name.py"),
                 r"allowed_domains\s*=\s*\[['\"](.+)['\"]\]",
             ).group(1),
         )
         self.assertEqual(
-            f"http://{domain}/",
+            f"https://{domain}",
             self.find_in_file(
                 Path(self.proj_mod_path, "spiders", "test_name.py"),
                 r"start_urls\s*=\s*\[['\"](.+)['\"]\]",
             ).group(1),
         )
 
     def test_url_schema(self):
-        self.test_url("http://test.com", "test.com")
+        self.test_url("https://test.com", "test.com")
+
+    def test_template_start_urls(
+        self, url="test.com", expected="https://test.com", template="basic"
+    ):
+        self.assertEqual(
+            0, self.call("genspider", "-t", template, "--force", "test_name", url)
+        )
+        self.assertEqual(
+            expected,
+            self.find_in_file(
+                Path(self.proj_mod_path, "spiders", "test_name.py"),
+                r"start_urls\s*=\s*\[['\"](.+)['\"]\]",
+            ).group(1),
+        )
+
+    def test_genspider_basic_start_urls(self):
+        self.test_template_start_urls("https://test.com", "https://test.com", "basic")
+        self.test_template_start_urls("http://test.com", "http://test.com", "basic")
+        self.test_template_start_urls(
+            "http://test.com/other/path", "http://test.com/other/path", "basic"
+        )
+        self.test_template_start_urls(
+            "test.com/other/path", "https://test.com/other/path", "basic"
+        )
+
+    def test_genspider_crawl_start_urls(self):
+        self.test_template_start_urls("https://test.com", "https://test.com", "crawl")
+        self.test_template_start_urls("http://test.com", "http://test.com", "crawl")
+        self.test_template_start_urls(
+            "http://test.com/other/path", "http://test.com/other/path", "crawl"
+        )
+        self.test_template_start_urls(
+            "test.com/other/path", "https://test.com/other/path", "crawl"
+        )
+        self.test_template_start_urls("test.com", "https://test.com", "crawl")
 
-    def test_url_path(self):
-        self.test_url("test.com/some/other/page", "test.com")
+    def test_genspider_xmlfeed_start_urls(self):
+        self.test_template_start_urls(
+            "https://test.com/feed.xml", "https://test.com/feed.xml", "xmlfeed"
+        )
+        self.test_template_start_urls(
+            "http://test.com/feed.xml", "http://test.com/feed.xml", "xmlfeed"
+        )
+        self.test_template_start_urls(
+            "test.com/feed.xml", "https://test.com/feed.xml", "xmlfeed"
+        )
 
-    def test_url_schema_path(self):
-        self.test_url("https://test.com/some/other/page", "test.com")
+    def test_genspider_csvfeed_start_urls(self):
+        self.test_template_start_urls(
+            "https://test.com/feed.csv", "https://test.com/feed.csv", "csvfeed"
+        )
+        self.test_template_start_urls(
+            "http://test.com/feed.xml", "http://test.com/feed.xml", "csvfeed"
+        )
+        self.test_template_start_urls(
+            "test.com/feed.csv", "https://test.com/feed.csv", "csvfeed"
+        )
 
 
 class GenspiderStandaloneCommandTest(ProjectTest):
     def test_generate_standalone_spider(self):
         self.call("genspider", "example", "example.com")
         assert Path(self.temp_path, "example.py").exists()
 
@@ -600,15 +650,14 @@
 
 class MiscCommandsTest(CommandTest):
     def test_list(self):
         self.assertEqual(0, self.call("list"))
 
 
 class RunSpiderCommandTest(CommandTest):
-
     spider_filename = "myspider.py"
 
     debug_log_spider = """
 import scrapy
 
 class MySpider(scrapy.Spider):
     name = 'myspider'
@@ -869,15 +918,14 @@
         args = ["-o", "-:json"]
         log = self.get_log(spider_code, args=args)
         self.assertIn("[myspider] DEBUG: FEEDS: {'stdout:': {'format': 'json'}}", log)
 
 
 @skipIf(platform.system() != "Windows", "Windows required for .pyw files")
 class WindowsRunSpiderCommandTest(RunSpiderCommandTest):
-
     spider_filename = "myspider.pyw"
 
     def setUp(self):
         super().setUp()
 
     def test_start_requests_errors(self):
         log = self.get_log(self.badspider, name="badspider.pyw")
```

### Comparing `Scrapy-2.8.0/tests/test_contracts.py` & `Scrapy-2.9.0/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_crawl.py` & `Scrapy-2.9.0/tests/test_crawl.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_crawler.py` & `Scrapy-2.9.0/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_dependencies.py` & `Scrapy-2.9.0/tests/test_dependencies.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,11 +33,7 @@
         config_parser = ConfigParser()
         config_parser.read(tox_config_file_path)
         pattern = r"Twisted\[http2\]==([\d.]+)"
         match = re.search(pattern, config_parser["pinned"]["deps"])
         pinned_twisted_version_string = match[1]
 
         self.assertEqual(twisted_version.short(), pinned_twisted_version_string)
-
-
-if __name__ == "__main__":
-    unittest.main()
```

### Comparing `Scrapy-2.8.0/tests/test_downloader_handlers.py` & `Scrapy-2.9.0/tests/test_downloader_handlers.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloader_handlers_http2.py` & `Scrapy-2.9.0/tests/test_downloader_handlers_http2.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     Https11TestCase,
     UriResource,
 )
 
 
 @skipIf(not H2_ENABLED, "HTTP/2 support in Twisted is not enabled")
 class Https2TestCase(Https11TestCase):
-
     scheme = "https"
     HTTP2_DATALOSS_SKIP_REASON = "Content-Length mismatch raises InvalidBodyLengthError"
 
     @classmethod
     def setUpClass(cls):
         from scrapy.core.downloader.handlers.http2 import H2DownloadHandler
```

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from scrapy.http import Request, Response
 from scrapy.spiders import Spider
 from scrapy.utils.python import to_bytes
 from scrapy.utils.test import get_crawler, get_from_asyncio_queue
 
 
 class ManagerTestCase(TestCase):
-
     settings_dict = None
 
     def setUp(self):
         self.crawler = get_crawler(Spider, self.settings_dict)
         self.spider = self.crawler._create_spider("foo")
         self.mwman = DownloaderMiddlewareManager.from_crawler(self.crawler)
         # some mw depends on stats collector
```

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_ajaxcrawlable.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_ajaxcrawlable.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_cookies.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_cookies.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_decompression.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_decompression.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     for format in formats:
         body = get_testdata("compressed", "feed-sample1." + format)
         test_responses[format] = Response("http://foo.com/bar", body=body)
     return uncompressed_body, test_responses
 
 
 class DecompressionMiddlewareTest(TestCase):
-
     test_formats = ["tar", "xml.bz2", "xml.gz", "zip"]
     uncompressed_body, test_responses = _test_data(test_formats)
 
     def setUp(self):
         self.mw = DecompressionMiddleware()
         self.spider = Spider("foo")
```

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_defaultheaders.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_defaultheaders.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_downloadtimeout.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_downloadtimeout.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_httpauth.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_httpauth.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_httpcache.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_httpcache.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from scrapy.http import HtmlResponse, Request, Response
 from scrapy.settings import Settings
 from scrapy.spiders import Spider
 from scrapy.utils.test import get_crawler
 
 
 class _BaseTest(unittest.TestCase):
-
     storage_class = "scrapy.extensions.httpcache.DbmCacheStorage"
     policy_class = "scrapy.extensions.httpcache.RFC2616Policy"
 
     def setUp(self):
         self.yesterday = email.utils.formatdate(time.time() - 86400)
         self.today = email.utils.formatdate()
         self.tomorrow = email.utils.formatdate(time.time() + 86400)
@@ -142,45 +141,41 @@
             storage.store_response(self.spider, self.request, response)
             cached_response = storage.retrieve_response(self.spider, self.request)
             self.assertIsInstance(cached_response, HtmlResponse)
             self.assertEqualResponse(response, cached_response)
 
 
 class DbmStorageTest(DefaultStorageTest):
-
     storage_class = "scrapy.extensions.httpcache.DbmCacheStorage"
 
 
 class DbmStorageWithCustomDbmModuleTest(DbmStorageTest):
-
     dbm_module = "tests.mocks.dummydbm"
 
     def _get_settings(self, **new_settings):
         new_settings.setdefault("HTTPCACHE_DBM_MODULE", self.dbm_module)
         return super()._get_settings(**new_settings)
 
     def test_custom_dbm_module_loaded(self):
         # make sure our dbm module has been loaded
         with self._storage() as storage:
             self.assertEqual(storage.dbmodule.__name__, self.dbm_module)
 
 
 class FilesystemStorageTest(DefaultStorageTest):
-
     storage_class = "scrapy.extensions.httpcache.FilesystemCacheStorage"
 
 
 class FilesystemStorageGzipTest(FilesystemStorageTest):
     def _get_settings(self, **new_settings):
         new_settings.setdefault("HTTPCACHE_GZIP", True)
         return super()._get_settings(**new_settings)
 
 
 class DummyPolicyTest(_BaseTest):
-
     policy_class = "scrapy.extensions.httpcache.DummyPolicy"
 
     def test_middleware(self):
         with self._middleware() as mw:
             assert mw.process_request(self.request, self.spider) is None
             mw.process_response(self.request, self.response, self.spider)
             response = mw.process_request(self.request, self.spider)
@@ -266,15 +261,14 @@
             response = mw.process_request(self.request, self.spider)
             assert isinstance(response, HtmlResponse)
             self.assertEqualResponse(self.response, response)
             assert "cached" in response.flags
 
 
 class RFC2616PolicyTest(DefaultStorageTest):
-
     policy_class = "scrapy.extensions.httpcache.RFC2616Policy"
 
     def _process_requestresponse(self, mw, request, response):
         result = None
         try:
             result = mw.process_request(request, self.spider)
             if result:
```

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_httpcompression.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_httpcompression.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_httpproxy.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_httpproxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from scrapy.spiders import Spider
 from scrapy.utils.test import get_crawler
 
 spider = Spider("foo")
 
 
 class TestHttpProxyMiddleware(TestCase):
-
-    failureException = AssertionError
+    failureException = AssertionError  # type: ignore[assignment]
 
     def setUp(self):
         self._oldenv = os.environ.copy()
 
     def tearDown(self):
         os.environ = self._oldenv
```

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_redirect.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_redirect.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_retry.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 
         # discard it
         req = self.mw.process_exception(req, exception, self.spider)
         self.assertEqual(req, None)
 
 
 class MaxRetryTimesTest(unittest.TestCase):
-
     invalid_url = "http://www.scrapytest.org/invalid_url"
 
     def get_spider_and_middleware(self, settings=None):
         crawler = get_crawler(Spider, settings or {})
         spider = crawler._create_spider("foo")
         middleware = RetryMiddleware.from_crawler(crawler)
         return spider, middleware
```

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_robotstxt.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_robotstxt.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_stats.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_stats.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_downloadermiddleware_useragent.py` & `Scrapy-2.9.0/tests/test_downloadermiddleware_useragent.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_dupefilters.py` & `Scrapy-2.9.0/tests/test_dupefilters.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_engine.py` & `Scrapy-2.9.0/tests/test_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,14 @@
         signalargs.pop("sender", None)
         self.signals_caught[sig] = signalargs
 
 
 class EngineTest(unittest.TestCase):
     @defer.inlineCallbacks
     def test_crawler(self):
-
         for spider in (
             TestSpider,
             DictItemsSpider,
             AttrsItemsSpider,
             DataClassItemsSpider,
         ):
             run = CrawlerRun(spider)
```

### Comparing `Scrapy-2.8.0/tests/test_engine_stop_download_bytes.py` & `Scrapy-2.9.0/tests/test_engine_stop_download_bytes.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_engine_stop_download_headers.py` & `Scrapy-2.9.0/tests/test_engine_stop_download_headers.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_exporters.py` & `Scrapy-2.9.0/tests/test_exporters.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 @dataclasses.dataclass
 class CustomFieldDataclass:
     name: str
     age: int = dataclasses.field(metadata={"serializer": custom_serializer})
 
 
 class BaseItemExporterTest(unittest.TestCase):
-
     item_class = TestItem
     custom_field_item_class = CustomFieldItem
 
     def setUp(self):
         self.i = self.item_class(name="John\xa3", age="22")
         self.output = BytesIO()
         self.ie = self._get_exporter()
@@ -509,21 +508,19 @@
                    </item>
                 </items>
             """,
         )
 
 
 class XmlItemExporterDataclassTest(XmlItemExporterTest):
-
     item_class = TestDataClass
     custom_field_item_class = CustomFieldDataclass
 
 
 class JsonLinesItemExporterTest(BaseItemExporterTest):
-
     _expected_nested = {
         "name": "Jesus",
         "age": {"name": "Maria", "age": {"name": "Joseph", "age": "22"}},
     }
 
     def _get_exporter(self, **kwargs):
         return JsonLinesItemExporter(self.output, **kwargs)
@@ -555,21 +552,19 @@
         self.ie.finish_exporting()
         exported = json.loads(to_unicode(self.output.getvalue()))
         item["time"] = str(item["time"])
         self.assertEqual(exported, item)
 
 
 class JsonLinesItemExporterDataclassTest(JsonLinesItemExporterTest):
-
     item_class = TestDataClass
     custom_field_item_class = CustomFieldDataclass
 
 
 class JsonItemExporterTest(JsonLinesItemExporterTest):
-
     _expected_nested = [JsonLinesItemExporterTest._expected_nested]
 
     def _get_exporter(self, **kwargs):
         return JsonItemExporter(self.output, **kwargs)
 
     def _check_output(self):
         exported = json.loads(to_unicode(self.output.getvalue().strip()))
@@ -623,21 +618,19 @@
         self.ie.finish_exporting()
         exported = json.loads(to_unicode(self.output.getvalue()))
         item["time"] = str(item["time"])
         self.assertEqual(exported, [item])
 
 
 class JsonItemExporterDataclassTest(JsonItemExporterTest):
-
     item_class = TestDataClass
     custom_field_item_class = CustomFieldDataclass
 
 
 class CustomExporterItemTest(unittest.TestCase):
-
     item_class = TestItem
 
     def setUp(self):
         if self.item_class is None:
             raise unittest.SkipTest("item class is None")
 
     def test_exporter_custom_serializer(self):
@@ -660,13 +653,12 @@
 
         i2 = {"name": "John", "age": "22"}
         self.assertEqual(ie.serialize_field({}, "name", i2["name"]), "John")
         self.assertEqual(ie.serialize_field({}, "age", i2["age"]), "23")
 
 
 class CustomExporterDataclassTest(CustomExporterItemTest):
-
     item_class = TestDataClass
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `Scrapy-2.8.0/tests/test_extension_telnet.py` & `Scrapy-2.9.0/tests/test_extension_telnet.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_feedexport.py` & `Scrapy-2.9.0/tests/test_feedexport.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,27 @@
 from twisted.internet import defer
 from twisted.trial import unittest
 from w3lib.url import file_uri_to_path, path_to_file_uri
 from zope.interface import implementer
 from zope.interface.verify import verifyObject
 
 import scrapy
+from scrapy import signals
 from scrapy.exceptions import NotConfigured, ScrapyDeprecationWarning
 from scrapy.exporters import CsvItemExporter, JsonItemExporter
 from scrapy.extensions.feedexport import (
     BlockingFeedStorage,
     FeedExporter,
+    FeedSlot,
     FileFeedStorage,
     FTPFeedStorage,
     GCSFeedStorage,
     IFeedStorage,
     S3FeedStorage,
     StdoutFeedStorage,
-    _FeedSlot,
 )
 from scrapy.settings import Settings
 from scrapy.utils.python import to_unicode
 from scrapy.utils.test import get_crawler, mock_google_cloud_storage, skip_if_no_boto
 from tests.mockserver import MockFTPServer, MockServer
 from tests.spiders import ItemSpider
 
@@ -656,16 +657,16 @@
                 try:
                     result.append(load_func(temp))
                 except EOFError:
                     break
         return result
 
 
-class InstrumentedFeedSlot(_FeedSlot):
-    """Instrumented _FeedSlot subclass for keeping track of calls to
+class InstrumentedFeedSlot(FeedSlot):
+    """Instrumented FeedSlot subclass for keeping track of calls to
     start_exporting and finish_exporting."""
 
     def start_exporting(self):
         self.update_listener("start")
         super().start_exporting()
 
     def finish_exporting(self):
@@ -960,15 +961,15 @@
             },
             "FEED_EXPORT_INDENT": None,
         }
 
         listener = IsExportingListener()
         InstrumentedFeedSlot.subscribe__listener(listener)
 
-        with mock.patch("scrapy.extensions.feedexport._FeedSlot", InstrumentedFeedSlot):
+        with mock.patch("scrapy.extensions.feedexport.FeedSlot", InstrumentedFeedSlot):
             _ = yield self.exported_data(items, settings)
             self.assertFalse(listener.start_without_finish)
             self.assertFalse(listener.finish_without_start)
 
     @defer.inlineCallbacks
     def test_start_finish_exporting_no_items(self):
         items = []
@@ -978,15 +979,15 @@
             },
             "FEED_EXPORT_INDENT": None,
         }
 
         listener = IsExportingListener()
         InstrumentedFeedSlot.subscribe__listener(listener)
 
-        with mock.patch("scrapy.extensions.feedexport._FeedSlot", InstrumentedFeedSlot):
+        with mock.patch("scrapy.extensions.feedexport.FeedSlot", InstrumentedFeedSlot):
             _ = yield self.exported_data(items, settings)
             self.assertFalse(listener.start_without_finish)
             self.assertFalse(listener.finish_without_start)
 
     @defer.inlineCallbacks
     def test_start_finish_exporting_items_exception(self):
         items = [
@@ -999,15 +1000,15 @@
             "FEED_EXPORTERS": {"json": ExceptionJsonItemExporter},
             "FEED_EXPORT_INDENT": None,
         }
 
         listener = IsExportingListener()
         InstrumentedFeedSlot.subscribe__listener(listener)
 
-        with mock.patch("scrapy.extensions.feedexport._FeedSlot", InstrumentedFeedSlot):
+        with mock.patch("scrapy.extensions.feedexport.FeedSlot", InstrumentedFeedSlot):
             _ = yield self.exported_data(items, settings)
             self.assertFalse(listener.start_without_finish)
             self.assertFalse(listener.finish_without_start)
 
     @defer.inlineCallbacks
     def test_start_finish_exporting_no_items_exception(self):
         items = []
@@ -1018,15 +1019,15 @@
             "FEED_EXPORTERS": {"json": ExceptionJsonItemExporter},
             "FEED_EXPORT_INDENT": None,
         }
 
         listener = IsExportingListener()
         InstrumentedFeedSlot.subscribe__listener(listener)
 
-        with mock.patch("scrapy.extensions.feedexport._FeedSlot", InstrumentedFeedSlot):
+        with mock.patch("scrapy.extensions.feedexport.FeedSlot", InstrumentedFeedSlot):
             _ = yield self.exported_data(items, settings)
             self.assertFalse(listener.start_without_finish)
             self.assertFalse(listener.finish_without_start)
 
     @defer.inlineCallbacks
     def test_export_no_items_store_empty(self):
         formats = (
@@ -1064,15 +1065,14 @@
             yield self.exported_no_data(settings)
 
         print(log)
         self.assertEqual(str(log).count("Storage.store is called"), 3)
 
     @defer.inlineCallbacks
     def test_export_multiple_item_classes(self):
-
         items = [
             self.MyItem({"foo": "bar1", "egg": "spam1"}),
             self.MyItem2({"hello": "world2", "foo": "bar2"}),
             self.MyItem({"foo": "bar3", "egg": "spam3", "baz": "quux3"}),
             {"hello": "world4", "egg": "spam4"},
         ]
 
@@ -1635,14 +1635,65 @@
                 },
                 "FEED_EXPORT_INDENT": None,
             }
 
             data = yield self.exported_data(items, settings)
             self.assertEqual(row["expected"], data[feed_options["format"]])
 
+    @defer.inlineCallbacks
+    def test_storage_file_no_postprocessing(self):
+        @implementer(IFeedStorage)
+        class Storage:
+            def __init__(self, uri, *, feed_options=None):
+                pass
+
+            def open(self, spider):
+                Storage.open_file = tempfile.NamedTemporaryFile(prefix="feed-")
+                return Storage.open_file
+
+            def store(self, file):
+                Storage.store_file = file
+                file.close()
+
+        settings = {
+            "FEEDS": {self._random_temp_filename(): {"format": "jsonlines"}},
+            "FEED_STORAGES": {"file": Storage},
+        }
+        yield self.exported_no_data(settings)
+        self.assertIs(Storage.open_file, Storage.store_file)
+
+    @defer.inlineCallbacks
+    def test_storage_file_postprocessing(self):
+        @implementer(IFeedStorage)
+        class Storage:
+            def __init__(self, uri, *, feed_options=None):
+                pass
+
+            def open(self, spider):
+                Storage.open_file = tempfile.NamedTemporaryFile(prefix="feed-")
+                return Storage.open_file
+
+            def store(self, file):
+                Storage.store_file = file
+                file.close()
+
+        settings = {
+            "FEEDS": {
+                self._random_temp_filename(): {
+                    "format": "jsonlines",
+                    "postprocessing": [
+                        "scrapy.extensions.postprocessing.GzipPlugin",
+                    ],
+                },
+            },
+            "FEED_STORAGES": {"file": Storage},
+        }
+        yield self.exported_no_data(settings)
+        self.assertIs(Storage.open_file, Storage.store_file)
+
 
 class FeedPostProcessedExportsTest(FeedExportTestBase):
     __test__ = True
 
     items = [{"foo": "bar"}]
     expected = b"foo\r\nbar\r\n"
 
@@ -1707,15 +1758,14 @@
         gzipf.write(data)
         gzipf.close()
         data_stream.seek(0)
         return data_stream.read()
 
     @defer.inlineCallbacks
     def test_gzip_plugin(self):
-
         filename = self._named_tempfile("gzip_file")
 
         settings = {
             "FEEDS": {
                 filename: {
                     "format": "csv",
                     "postprocessing": ["scrapy.extensions.postprocessing.GzipPlugin"],
@@ -1727,15 +1777,14 @@
         try:
             gzip.decompress(data[filename])
         except OSError:
             self.fail("Received invalid gzip data.")
 
     @defer.inlineCallbacks
     def test_gzip_plugin_compresslevel(self):
-
         filename_to_compressed = {
             self._named_tempfile("compresslevel_0"): self.get_gzip_compressed(
                 self.expected, compresslevel=0
             ),
             self._named_tempfile("compresslevel_9"): self.get_gzip_compressed(
                 self.expected, compresslevel=9
             ),
@@ -1835,15 +1884,14 @@
         for filename, compressed in filename_to_compressed.items():
             result = gzip.decompress(data[filename])
             self.assertEqual(compressed, data[filename])
             self.assertEqual(self.expected, result)
 
     @defer.inlineCallbacks
     def test_lzma_plugin(self):
-
         filename = self._named_tempfile("lzma_file")
 
         settings = {
             "FEEDS": {
                 filename: {
                     "format": "csv",
                     "postprocessing": ["scrapy.extensions.postprocessing.LZMAPlugin"],
@@ -1855,15 +1903,14 @@
         try:
             lzma.decompress(data[filename])
         except lzma.LZMAError:
             self.fail("Received invalid lzma data.")
 
     @defer.inlineCallbacks
     def test_lzma_plugin_format(self):
-
         filename_to_compressed = {
             self._named_tempfile("format_FORMAT_XZ"): lzma.compress(
                 self.expected, format=lzma.FORMAT_XZ
             ),
             self._named_tempfile("format_FORMAT_ALONE"): lzma.compress(
                 self.expected, format=lzma.FORMAT_ALONE
             ),
@@ -1889,15 +1936,14 @@
         for filename, compressed in filename_to_compressed.items():
             result = lzma.decompress(data[filename])
             self.assertEqual(compressed, data[filename])
             self.assertEqual(self.expected, result)
 
     @defer.inlineCallbacks
     def test_lzma_plugin_check(self):
-
         filename_to_compressed = {
             self._named_tempfile("check_CHECK_NONE"): lzma.compress(
                 self.expected, check=lzma.CHECK_NONE
             ),
             self._named_tempfile("check_CHECK_CRC256"): lzma.compress(
                 self.expected, check=lzma.CHECK_SHA256
             ),
@@ -1923,15 +1969,14 @@
         for filename, compressed in filename_to_compressed.items():
             result = lzma.decompress(data[filename])
             self.assertEqual(compressed, data[filename])
             self.assertEqual(self.expected, result)
 
     @defer.inlineCallbacks
     def test_lzma_plugin_preset(self):
-
         filename_to_compressed = {
             self._named_tempfile("preset_PRESET_0"): lzma.compress(
                 self.expected, preset=0
             ),
             self._named_tempfile("preset_PRESET_9"): lzma.compress(
                 self.expected, preset=9
             ),
@@ -1982,15 +2027,14 @@
         data = yield self.exported_data(self.items, settings)
         self.assertEqual(compressed, data[filename])
         result = lzma.decompress(data[filename])
         self.assertEqual(self.expected, result)
 
     @defer.inlineCallbacks
     def test_bz2_plugin(self):
-
         filename = self._named_tempfile("bz2_file")
 
         settings = {
             "FEEDS": {
                 filename: {
                     "format": "csv",
                     "postprocessing": ["scrapy.extensions.postprocessing.Bz2Plugin"],
@@ -2002,15 +2046,14 @@
         try:
             bz2.decompress(data[filename])
         except OSError:
             self.fail("Received invalid bz2 data.")
 
     @defer.inlineCallbacks
     def test_bz2_plugin_compresslevel(self):
-
         filename_to_compressed = {
             self._named_tempfile("compresslevel_1"): bz2.compress(
                 self.expected, compresslevel=1
             ),
             self._named_tempfile("compresslevel_9"): bz2.compress(
                 self.expected, compresslevel=9
             ),
@@ -2052,15 +2095,14 @@
         }
 
         data = yield self.exported_data(self.items, settings)
         self.assertEqual(self.expected, data[filename])
 
     @defer.inlineCallbacks
     def test_custom_plugin_with_parameter(self):
-
         expected = b"foo\r\n\nbar\r\n\n"
         filename = self._named_tempfile("newline")
 
         settings = {
             "FEEDS": {
                 filename: {
                     "format": "csv",
@@ -2071,15 +2113,14 @@
         }
 
         data = yield self.exported_data(self.items, settings)
         self.assertEqual(expected, data[filename])
 
     @defer.inlineCallbacks
     def test_custom_plugin_with_compression(self):
-
         expected = b"foo\r\n\nbar\r\n\n"
 
         filename_to_decompressor = {
             self._named_tempfile("bz2"): bz2.decompress,
             self._named_tempfile("lzma"): lzma.decompress,
             self._named_tempfile("gzip"): gzip.decompress,
         }
@@ -2498,25 +2539,25 @@
     @pytest.mark.skipif(
         sys.platform == "win32", reason="Odd behaviour on file creation/output"
     )
     @defer.inlineCallbacks
     def test_batch_path_differ(self):
         """
         Test that the name of all batch files differ from each other.
-        So %(batch_time)s replaced with the current date.
+        So %(batch_id)d replaced with the current id.
         """
         items = [
             self.MyItem({"foo": "bar1", "egg": "spam1"}),
             self.MyItem({"foo": "bar2", "egg": "spam2", "baz": "quux2"}),
             self.MyItem({"foo": "bar3", "baz": "quux3"}),
         ]
         settings = {
             "FEEDS": {
                 self._random_temp_filename()
-                / "%(batch_time)s": {
+                / "%(batch_id)d": {
                     "format": "json",
                 },
             },
             "FEED_EXPORT_BATCH_ITEM_COUNT": 1,
         }
         data = yield self.exported_data(items, settings)
         self.assertEqual(len(items), len([_ for _ in data["json"] if _]))
@@ -2551,15 +2592,14 @@
         items = [
             self.MyItem({"foo": "bar1", "egg": "spam1"}),
             self.MyItem({"foo": "bar2", "egg": "spam2", "baz": "quux2"}),
             self.MyItem({"foo": "bar3", "baz": "quux3"}),
         ]
 
         class CustomS3FeedStorage(S3FeedStorage):
-
             stubs = []
 
             def open(self, *args, **kwargs):
                 from botocore.stub import ANY, Stubber
 
                 stub = Stubber(self.s3_client)
                 stub.activate()
@@ -2572,15 +2612,15 @@
                         "Key": ANY,
                     },
                     service_response={},
                 )
                 return super().open(*args, **kwargs)
 
         key = "export.csv"
-        uri = f"s3://{bucket}/{key}/%(batch_time)s.json"
+        uri = f"s3://{bucket}/{key}/%(batch_id)d.json"
         batch_item_count = 1
         settings = {
             "AWS_ACCESS_KEY_ID": "access_key",
             "AWS_SECRET_ACCESS_KEY": "secret_key",
             "FEED_EXPORT_BATCH_ITEM_COUNT": batch_item_count,
             "FEED_STORAGES": {
                 "s3": CustomS3FeedStorage,
@@ -2608,14 +2648,91 @@
             yield crawler.crawl()
 
         self.assertEqual(len(CustomS3FeedStorage.stubs), len(items) + 1)
         for stub in CustomS3FeedStorage.stubs[:-1]:
             stub.assert_no_pending_responses()
 
 
+# Test that the FeedExporer sends the feed_exporter_closed and feed_slot_closed signals
+class FeedExporterSignalsTest(unittest.TestCase):
+    items = [
+        {"foo": "bar1", "egg": "spam1"},
+        {"foo": "bar2", "egg": "spam2", "baz": "quux2"},
+        {"foo": "bar3", "baz": "quux3"},
+    ]
+
+    with tempfile.NamedTemporaryFile(suffix="json") as tmp:
+        settings = {
+            "FEEDS": {
+                f"file:///{tmp.name}": {
+                    "format": "json",
+                },
+            },
+        }
+
+    def feed_exporter_closed_signal_handler(self):
+        self.feed_exporter_closed_received = True
+
+    def feed_slot_closed_signal_handler(self, slot):
+        self.feed_slot_closed_received = True
+
+    def feed_exporter_closed_signal_handler_deferred(self):
+        d = defer.Deferred()
+        d.addCallback(lambda _: setattr(self, "feed_exporter_closed_received", True))
+        d.callback(None)
+        return d
+
+    def feed_slot_closed_signal_handler_deferred(self, slot):
+        d = defer.Deferred()
+        d.addCallback(lambda _: setattr(self, "feed_slot_closed_received", True))
+        d.callback(None)
+        return d
+
+    def run_signaled_feed_exporter(
+        self, feed_exporter_signal_handler, feed_slot_signal_handler
+    ):
+        crawler = get_crawler(settings_dict=self.settings)
+        feed_exporter = FeedExporter.from_crawler(crawler)
+        spider = scrapy.Spider("default")
+        spider.crawler = crawler
+        crawler.signals.connect(
+            feed_exporter_signal_handler,
+            signal=signals.feed_exporter_closed,
+        )
+        crawler.signals.connect(
+            feed_slot_signal_handler, signal=signals.feed_slot_closed
+        )
+        feed_exporter.open_spider(spider)
+        for item in self.items:
+            feed_exporter.item_scraped(item, spider)
+        defer.ensureDeferred(feed_exporter.close_spider(spider))
+
+    def test_feed_exporter_signals_sent(self):
+        self.feed_exporter_closed_received = False
+        self.feed_slot_closed_received = False
+
+        self.run_signaled_feed_exporter(
+            self.feed_exporter_closed_signal_handler,
+            self.feed_slot_closed_signal_handler,
+        )
+        self.assertTrue(self.feed_slot_closed_received)
+        self.assertTrue(self.feed_exporter_closed_received)
+
+    def test_feed_exporter_signals_sent_deferred(self):
+        self.feed_exporter_closed_received = False
+        self.feed_slot_closed_received = False
+
+        self.run_signaled_feed_exporter(
+            self.feed_exporter_closed_signal_handler_deferred,
+            self.feed_slot_closed_signal_handler_deferred,
+        )
+        self.assertTrue(self.feed_slot_closed_received)
+        self.assertTrue(self.feed_exporter_closed_received)
+
+
 class FeedExportInitTest(unittest.TestCase):
     def test_unsupported_storage(self):
         settings = {
             "FEEDS": {
                 "unsupported://uri": {},
             },
         }
@@ -2824,15 +2941,14 @@
             match="FTPFeedStorageWithoutFeedOptionsWithFromCrawler.from_crawler does not support "
             "the 'feed_options' keyword argument.",
         ):
             feed_exporter.open_spider(spider)
 
 
 class URIParamsTest:
-
     spider_name = "uri_params_spider"
     deprecated_options = False
 
     def build_settings(self, uri="file:///tmp/foobar", uri_params=None):
         raise NotImplementedError
 
     def _crawler_feed_exporter(self, settings):
```

### Comparing `Scrapy-2.8.0/tests/test_http2_client_protocol.py` & `Scrapy-2.9.0/tests/test_http2_client_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import random
 import re
 import shutil
 import string
 from ipaddress import IPv4Address
 from pathlib import Path
+from typing import Dict
 from unittest import mock, skipIf
 from urllib.parse import urlencode
 
 from twisted.internet import reactor
 from twisted.internet.defer import (
     CancelledError,
     Deferred,
@@ -83,14 +84,15 @@
         request.setHeader("Content-Type", "text/html; charset=UTF-8")
         return Data.HTML_LARGE
 
 
 class PostDataJsonMixin:
     @staticmethod
     def make_response(request: TxRequest, extra_data: str):
+        assert request.content is not None
         response = {
             "request-headers": {},
             "request-body": json.loads(request.content.read()),
             "extra-data": extra_data,
         }
         for k, v in request.requestHeaders.getAllRawHeaders():
             response["request-headers"][str(k, "utf-8")] = str(v[0], "utf-8")
@@ -141,15 +143,16 @@
 
 
 class QueryParams(LeafResource):
     def render_GET(self, request: TxRequest):
         request.setHeader("Content-Type", "application/json; charset=UTF-8")
         request.setHeader("Content-Encoding", "UTF-8")
 
-        query_params = {}
+        query_params: Dict[str, str] = {}
+        assert request.args is not None
         for k, v in request.args.items():
             query_params[str(k, "utf-8")] = str(v[0], "utf-8")
 
         return bytes(json.dumps(query_params), "utf-8")
 
 
 class RequestHeaders(LeafResource):
```

### Comparing `Scrapy-2.8.0/tests/test_http_cookies.py` & `Scrapy-2.9.0/tests/test_http_cookies.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_http_headers.py` & `Scrapy-2.9.0/tests/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_http_request.py` & `Scrapy-2.9.0/tests/test_http_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     XmlRpcRequest,
 )
 from scrapy.http.request import NO_CALLBACK
 from scrapy.utils.python import to_bytes, to_unicode
 
 
 class RequestTest(unittest.TestCase):
-
     request_class = Request
     default_method = "GET"
     default_headers = {}
     default_meta = {}
 
     def test_init(self):
         # Request requires url in the __init__ method
@@ -420,15 +419,14 @@
                 'curl -X PATCH "http://example.org" --foo -z',
                 ignore_unknown_options=False,
             ),
         )
 
 
 class FormRequestTest(RequestTest):
-
     request_class = FormRequest
 
     def assertQueryEqual(self, first, second, msg=None):
         first = to_unicode(first).split("&")
         second = to_unicode(second).split("&")
         return self.assertEqual(sorted(first), sorted(second), msg)
 
@@ -1443,15 +1441,14 @@
     uqs = unquote_to_bytes(qs)
     if to_unicode:
         uqs = uqs.decode(encoding)
     return parse_qs(uqs, True)
 
 
 class XmlRpcRequestTest(RequestTest):
-
     request_class = XmlRpcRequest
     default_method = "POST"
     default_headers = {b"Content-Type": [b"text/xml"]}
 
     def _test_request(self, **kwargs):
         r = self.request_class("http://scrapytest.org/rpc2", **kwargs)
         self.assertEqual(r.headers[b"Content-Type"], b"text/xml")
```

### Comparing `Scrapy-2.8.0/tests/test_http_response.py` & `Scrapy-2.9.0/tests/test_http_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 from scrapy.link import Link
 from scrapy.selector import Selector
 from scrapy.utils.python import to_unicode
 from tests import get_testdata
 
 
 class BaseResponseTest(unittest.TestCase):
-
     response_class = Response
 
     def test_init(self):
         # Response requires url in the constructor
         self.assertRaises(Exception, self.response_class)
         self.assertTrue(
             isinstance(self.response_class("http://example.com/"), self.response_class)
         )
         self.assertRaises(TypeError, self.response_class, b"http://example.com")
+        self.assertRaises(
+            TypeError, self.response_class, url="http://example.com", body={}
+        )
         # body can be str or None
         self.assertTrue(
             isinstance(
                 self.response_class("http://example.com/", body=b""),
                 self.response_class,
             )
         )
@@ -189,14 +191,15 @@
     def test_shortcut_attributes(self):
         r = self.response_class("http://example.com", body=b"hello")
         if self.response_class == Response:
             msg = "Response content isn't text"
             self.assertRaisesRegex(AttributeError, msg, getattr, r, "text")
             self.assertRaisesRegex(NotSupported, msg, r.css, "body")
             self.assertRaisesRegex(NotSupported, msg, r.xpath, "//body")
+            self.assertRaisesRegex(NotSupported, msg, r.jmespath, "body")
         else:
             r.text
             r.css("body")
             r.xpath("//body")
 
     # Response.follow
 
@@ -345,15 +348,14 @@
     def _links_response_no_href(self):
         body = get_testdata("link_extractor", "linkextractor_no_href.html")
         resp = self.response_class("http://example.com/index", body=body)
         return resp
 
 
 class TextResponseTest(BaseResponseTest):
-
     response_class = TextResponse
 
     def test_replace(self):
         super().test_replace()
         r1 = self.response_class(
             "http://www.example.com", body="hello", encoding="cp852"
         )
@@ -446,36 +448,47 @@
             headers={"Content-type": ["text/html; charset=gbk"]},
         )
         r8 = self.response_class(
             "http://www.example.com",
             body=codecs.BOM_UTF8 + b"\xc2\xa3",
             headers={"Content-type": ["text/html; charset=cp1251"]},
         )
+        r9 = self.response_class(
+            "http://www.example.com",
+            body=b"\x80",
+            headers={
+                "Content-type": [b"application/x-download; filename=\x80dummy.txt"]
+            },
+        )
 
         self.assertEqual(r1._headers_encoding(), "utf-8")
         self.assertEqual(r2._headers_encoding(), None)
         self.assertEqual(r2._declared_encoding(), "utf-8")
         self._assert_response_encoding(r2, "utf-8")
         self.assertEqual(r3._headers_encoding(), "cp1252")
         self.assertEqual(r3._declared_encoding(), "cp1252")
         self.assertEqual(r4._headers_encoding(), None)
         self.assertEqual(r5._headers_encoding(), None)
         self.assertEqual(r8._headers_encoding(), "cp1251")
+        self.assertEqual(r9._headers_encoding(), None)
         self.assertEqual(r8._declared_encoding(), "utf-8")
+        self.assertEqual(r9._declared_encoding(), None)
         self._assert_response_encoding(r5, "utf-8")
         self._assert_response_encoding(r8, "utf-8")
+        self._assert_response_encoding(r9, "cp1252")
         assert (
             r4._body_inferred_encoding() is not None
             and r4._body_inferred_encoding() != "ascii"
         )
         self._assert_response_values(r1, "utf-8", "\xa3")
         self._assert_response_values(r2, "utf-8", "\xa3")
         self._assert_response_values(r3, "iso-8859-1", "\xa3")
         self._assert_response_values(r6, "gb18030", "\u2015")
         self._assert_response_values(r7, "gb18030", "\u2015")
+        self._assert_response_values(r9, "cp1252", "€")
 
         # TextResponse (and subclasses) must be passed a encoding when instantiating with unicode bodies
         self.assertRaises(
             TypeError,
             self.response_class,
             "http://www.example.com",
             body="\xa3",
@@ -831,19 +844,17 @@
             with mock.patch("json.loads") as mock_json:
                 for _ in range(2):
                     json_response.json()
                 mock_json.assert_called_once_with(json_body.decode())
 
 
 class HtmlResponseTest(TextResponseTest):
-
     response_class = HtmlResponse
 
     def test_html_encoding(self):
-
         body = b"""<html><head><title>Some page</title>
         <meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1">
         </head><body>Price: \xa3100</body></html>'
         """
         r1 = self.response_class("http://www.example.com", body=body)
         self._assert_response_values(r1, "iso-8859-1", body)
 
@@ -874,15 +885,14 @@
     def test_html5_meta_charset(self):
         body = b"""<html><head><meta charset="gb2312" /><title>Some page</title><body>bla bla</body>"""
         r1 = self.response_class("http://www.example.com", body=body)
         self._assert_response_values(r1, "gb2312", body)
 
 
 class XmlResponseTest(TextResponseTest):
-
     response_class = XmlResponse
 
     def test_xml_encoding(self):
         body = b"<xml></xml>"
         r1 = self.response_class("http://www.example.com", body=body)
         self._assert_response_values(r1, self.response_class._DEFAULT_ENCODING, body)
```

### Comparing `Scrapy-2.8.0/tests/test_item.py` & `Scrapy-2.9.0/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_link.py` & `Scrapy-2.9.0/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_linkextractors.py` & `Scrapy-2.9.0/tests/test_linkextractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import pickle
 import re
 import unittest
 
+from packaging.version import Version
+from pytest import mark
+from w3lib import __version__ as w3lib_version
+
 from scrapy.http import HtmlResponse, XmlResponse
 from scrapy.link import Link
 from scrapy.linkextractors.lxmlhtml import LxmlLinkExtractor
 from tests import get_testdata
 
 
 # a hack to skip base class tests in pytest
@@ -811,7 +815,38 @@
                     nofollow=False,
                 ),
             ],
         )
 
     def test_restrict_xpaths_with_html_entities(self):
         super().test_restrict_xpaths_with_html_entities()
+
+    @mark.skipif(
+        Version(w3lib_version) < Version("2.0.0"),
+        reason=(
+            "Before w3lib 2.0.0, w3lib.url.safe_url_string would not complain "
+            "about an invalid port value."
+        ),
+    )
+    def test_skip_bad_links(self):
+        html = b"""
+        <a href="http://example.org:non-port">Why would you do this?</a>
+        <a href="http://example.org/item2.html">Good Link</a>
+        <a href="http://example.org/item3.html">Good Link 2</a>
+        """
+        response = HtmlResponse("http://example.org/index.html", body=html)
+        lx = self.extractor_cls()
+        self.assertEqual(
+            [link for link in lx.extract_links(response)],
+            [
+                Link(
+                    url="http://example.org/item2.html",
+                    text="Good Link",
+                    nofollow=False,
+                ),
+                Link(
+                    url="http://example.org/item3.html",
+                    text="Good Link 2",
+                    nofollow=False,
+                ),
+            ],
+        )
```

### Comparing `Scrapy-2.8.0/tests/test_loader.py` & `Scrapy-2.9.0/tests/test_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         il = TestItemLoader()
         il.add_value("name", "marta")
         item = il.load_item()
         self.assertEqual(item["name"], ["Marta"])
 
 
 class InitializationTestMixin:
-
     item_class = None
 
     def test_keep_single_value(self):
         """Loaded item should contain values from the initial item"""
         input_item = self.item_class(name="foo")
         il = ItemLoader(item=input_item)
         loaded_item = il.load_item()
```

### Comparing `Scrapy-2.8.0/tests/test_loader_deprecated.py` & `Scrapy-2.9.0/tests/test_loader_deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,14 @@
         il = TestItemLoader()
         self.assertRaises(
             ValueError, il.add_value, "name", ["marta", "other"], Compose(float)
         )
 
 
 class InitializationFromDictTest(unittest.TestCase):
-
     item_class = dict
 
     def test_keep_single_value(self):
         """Loaded item should contain values from the initial item"""
         input_item = self.item_class(name="foo")
         il = ItemLoader(item=input_item)
         loaded_item = il.load_item()
```

### Comparing `Scrapy-2.8.0/tests/test_logformatter.py` & `Scrapy-2.9.0/tests/test_logformatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from scrapy.spiders import Spider
 from scrapy.utils.test import get_crawler
 from tests.mockserver import MockServer
 from tests.spiders import ItemSpider
 
 
 class CustomItem(Item):
-
     name = Field()
 
     def __str__(self):
         return f"name: {self['name']}"
 
 
 class LogFormatterTestCase(unittest.TestCase):
```

### Comparing `Scrapy-2.8.0/tests/test_mail.py` & `Scrapy-2.9.0/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_middleware.py` & `Scrapy-2.9.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_pipeline_crawl.py` & `Scrapy-2.9.0/tests/test_pipeline_crawl.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 
         # check that the image files where actually written to the media store
         for item in items:
             for i in item[self.media_key]:
                 self.assertTrue((self.tmpmediastore / i["path"]).exists())
 
     def _assert_files_download_failure(self, crawler, items, code, logs):
-
         # check that the item does NOT have the "images/files" field populated
         self.assertEqual(len(items), 1)
         self.assertIn(self.media_key, items[0])
         self.assertFalse(items[0][self.media_key])
 
         # check that there was 1 successful fetch and 3 other responses with non-200 code
         self.assertEqual(
@@ -201,15 +200,14 @@
         "Missing Python Imaging Library, install https://pypi.python.org/pypi/Pillow"
     )
 else:
     skip_pillow = None
 
 
 class ImageDownloadCrawlTestCase(FileDownloadCrawlTestCase):
-
     skip = skip_pillow
 
     pipeline_class = "scrapy.pipelines.images.ImagesPipeline"
     store_setting_key = "IMAGES_STORE"
     media_key = "images"
     media_urls_key = "image_urls"
```

### Comparing `Scrapy-2.8.0/tests/test_pipeline_files.py` & `Scrapy-2.9.0/tests/test_pipeline_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,14 +476,30 @@
 
         pipeline_cls = UserPipe.from_settings(Settings(settings))
 
         for pipe_attr, settings_attr, pipe_inst_attr in self.file_cls_attr_settings_map:
             expected_value = settings.get(settings_attr)
             self.assertEqual(getattr(pipeline_cls, pipe_inst_attr), expected_value)
 
+    def test_file_pipeline_using_pathlike_objects(self):
+        class CustomFilesPipelineWithPathLikeDir(FilesPipeline):
+            def file_path(self, request, response=None, info=None, *, item=None):
+                return Path("subdir") / Path(request.url).name
+
+        pipeline = CustomFilesPipelineWithPathLikeDir.from_settings(
+            Settings({"FILES_STORE": Path("./Temp")})
+        )
+        request = Request("http://example.com/image01.jpg")
+        self.assertEqual(pipeline.file_path(request), Path("subdir/image01.jpg"))
+
+    def test_files_store_constructor_with_pathlike_object(self):
+        path = Path("./FileDir")
+        fs_store = FSFilesStore(path)
+        self.assertEqual(fs_store.basedir, str(path))
+
 
 class TestS3FilesStore(unittest.TestCase):
     @defer.inlineCallbacks
     def test_persist(self):
         skip_if_no_boto()
 
         bucket = "mybucket"
@@ -581,15 +597,15 @@
         store = GCSFilesStore(uri)
         store.POLICY = "authenticatedRead"
         expected_policy = {"role": "READER", "entity": "allAuthenticatedUsers"}
         yield store.persist_file(path, buf, info=None, meta=meta, headers=None)
         s = yield store.stat_file(path, info=None)
         self.assertIn("last_modified", s)
         self.assertIn("checksum", s)
-        self.assertEqual(s["checksum"], "zc2oVgXkbQr2EQdSdw3OPA==")
+        self.assertEqual(s["checksum"], "cdcda85605e46d0af6110752770dce3c")
         u = urlparse(uri)
         content, acl, blob = get_gcs_content_and_delete(u.hostname, u.path[1:] + path)
         self.assertEqual(content, data)
         self.assertEqual(blob.metadata, {"foo": "bar"})
         self.assertEqual(blob.cache_control, GCSFilesStore.CACHE_CONTROL)
         self.assertEqual(blob.content_type, "application/octet-stream")
         self.assertIn(expected_policy, acl)
```

### Comparing `Scrapy-2.8.0/tests/test_pipeline_images.py` & `Scrapy-2.9.0/tests/test_pipeline_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     if not encoders.issubset(set(Image.core.__dict__)):
         skip_pillow = "Missing JPEG encoders"
     else:
         skip_pillow = None
 
 
 class ImagesPipelineTestCase(unittest.TestCase):
-
     skip = skip_pillow
 
     def setUp(self):
         self.tempdir = mkdtemp()
         self.pipeline = ImagesPipeline(self.tempdir)
 
     def tearDown(self):
@@ -321,15 +320,14 @@
 
     def thumb_key(self, url, thumb_id):
         thumb_guid = hashlib.sha1(to_bytes(url)).hexdigest()
         return f"thumbsup/{thumb_id}/{thumb_guid}.jpg"
 
 
 class ImagesPipelineTestCaseFieldsMixin:
-
     skip = skip_pillow
 
     def test_item_fields_default(self):
         url = "http://www.example.com/images/1.jpg"
         item = self.item_class(name="item1", image_urls=[url])
         pipeline = ImagesPipeline.from_settings(
             Settings({"IMAGES_STORE": "s3://example/images/"})
@@ -416,15 +414,14 @@
 class ImagesPipelineTestCaseFieldsAttrsItem(
     ImagesPipelineTestCaseFieldsMixin, unittest.TestCase
 ):
     item_class = ImagesPipelineTestAttrsItem
 
 
 class ImagesPipelineTestCaseCustomSettings(unittest.TestCase):
-
     skip = skip_pillow
 
     img_cls_attribute_names = [
         # Pipeline attribute names with corresponding setting names.
         ("EXPIRES", "IMAGES_EXPIRES"),
         ("MIN_WIDTH", "IMAGES_MIN_WIDTH"),
         ("MIN_HEIGHT", "IMAGES_MIN_HEIGHT"),
```

### Comparing `Scrapy-2.8.0/tests/test_pipeline_media.py` & `Scrapy-2.9.0/tests/test_pipeline_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 def _mocked_download_func(request, info):
     assert request.callback is NO_CALLBACK
     response = request.meta.get("response")
     return response() if callable(response) else response
 
 
 class BaseMediaPipelineTestCase(unittest.TestCase):
-
     pipeline_class = MediaPipeline
     settings = None
 
     def setUp(self):
         spider_cls = Spider
         self.spider = spider_cls("media.com")
         crawler = get_crawler(spider_cls, self.settings)
@@ -209,15 +208,14 @@
         self._mockcalled.append("item_completed")
         item = super().item_completed(results, item, info)
         item["results"] = results
         return item
 
 
 class MediaPipelineTestCase(BaseMediaPipelineTestCase):
-
     pipeline_class = MockedMediaPipeline
 
     def _callback(self, result):
         self.pipe._mockcalled.append("request_callback")
         return result
 
     def _errback(self, result):
```

### Comparing `Scrapy-2.8.0/tests/test_pipelines.py` & `Scrapy-2.9.0/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_pqueues.py` & `Scrapy-2.9.0/tests/test_pqueues.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_proxy_connect.py` & `Scrapy-2.9.0/tests/test_proxy_connect.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_request_attribute_binding.py` & `Scrapy-2.9.0/tests/test_request_attribute_binding.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_request_cb_kwargs.py` & `Scrapy-2.9.0/tests/test_request_cb_kwargs.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,14 @@
 
     def parse_spider_mw_2(self, response, from_process_spider_output):
         self.checks.append(bool(from_process_spider_output))
         self.crawler.stats.inc_value("boolean_checks", 1)
 
 
 class CallbackKeywordArgumentsTestCase(TestCase):
-
     maxDiff = None
 
     def setUp(self):
         self.mockserver = MockServer()
         self.mockserver.__enter__()
 
     def tearDown(self):
```

### Comparing `Scrapy-2.8.0/tests/test_request_dict.py` & `Scrapy-2.9.0/tests/test_request_dict.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_request_left.py` & `Scrapy-2.9.0/tests/test_request_left.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_responsetypes.py` & `Scrapy-2.9.0/tests/test_responsetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
             ("text/xml; charset=UTF-8", XmlResponse),
             ("application/xhtml+xml; charset=UTF-8", HtmlResponse),
             ("application/vnd.wap.xhtml+xml; charset=utf-8", HtmlResponse),
             ("application/xml; charset=UTF-8", XmlResponse),
             ("application/octet-stream", Response),
             ("application/x-json; encoding=UTF8;charset=UTF-8", TextResponse),
             ("application/json-amazonui-streaming;charset=UTF-8", TextResponse),
+            (b"application/x-download; filename=\x80dummy.txt", Response),
         ]
         for source, cls in mappings:
             retcls = responsetypes.from_content_type(source)
             assert retcls is cls, f"{source} ==> {retcls} != {cls}"
 
     def test_from_body(self):
         mappings = [
```

### Comparing `Scrapy-2.8.0/tests/test_robotstxt_interface.py` & `Scrapy-2.9.0/tests/test_robotstxt_interface.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_scheduler.py` & `Scrapy-2.9.0/tests/test_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     def close(self):
         pass
 
 
 class MockCrawler(Crawler):
     def __init__(self, priority_queue_cls, jobdir):
-
         settings = dict(
             SCHEDULER_DEBUG=False,
             SCHEDULER_DISK_QUEUE="scrapy.squeues.PickleLifoDiskQueue",
             SCHEDULER_MEMORY_QUEUE="scrapy.squeues.LifoMemoryQueue",
             SCHEDULER_PRIORITY_QUEUE=priority_queue_cls,
             JOBDIR=jobdir,
             DUPEFILTER_CLASS="scrapy.dupefilters.BaseDupeFilter",
@@ -321,15 +320,14 @@
     @defer.inlineCallbacks
     def tearDown(self):
         yield self.crawler.stop()
 
     @defer.inlineCallbacks
     def test_integration_downloader_aware_priority_queue(self):
         with MockServer() as mockserver:
-
             url = mockserver.url("/status?n=200", is_secure=False)
             start_urls = [url] * 6
             yield self.crawler.crawl(start_urls)
             self.assertEqual(
                 self.crawler.stats.get_value("downloader/response_count"),
                 len(start_urls),
             )
```

### Comparing `Scrapy-2.8.0/tests/test_scheduler_base.py` & `Scrapy-2.9.0/tests/test_scheduler_base.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_settings/__init__.py` & `Scrapy-2.9.0/tests/test_settings/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,27 @@
         )
 
 
 class BaseSettingsTest(unittest.TestCase):
     def setUp(self):
         self.settings = BaseSettings()
 
+    def test_setdefault_not_existing_value(self):
+        settings = BaseSettings()
+        value = settings.setdefault("TEST_OPTION", "value")
+        self.assertEqual(settings["TEST_OPTION"], "value")
+        self.assertEqual(value, "value")
+        self.assertIsNotNone(value)
+
+    def test_setdefault_existing_value(self):
+        settings = BaseSettings({"TEST_OPTION": "value"})
+        value = settings.setdefault("TEST_OPTION", None)
+        self.assertEqual(settings["TEST_OPTION"], "value")
+        self.assertEqual(value, "value")
+
     def test_set_new_attribute(self):
         self.settings.set("TEST_OPTION", "value", 0)
         self.assertIn("TEST_OPTION", self.settings.attributes)
 
         attr = self.settings.attributes["TEST_OPTION"]
         self.assertIsInstance(attr, SettingsAttribute)
         self.assertEqual(attr.value, "value")
@@ -89,15 +102,14 @@
         self.assertIs(attr, self.settings.attributes["TEST_OPTION"])
 
     def test_set_calls_settings_attributes_methods_on_update(self):
         attr = SettingsAttribute("value", 10)
         with mock.patch.object(attr, "__setattr__") as mock_setattr, mock.patch.object(
             attr, "set"
         ) as mock_set:
-
             self.settings.attributes = {"TEST_OPTION": attr}
 
             for priority in (0, 10, 20):
                 self.settings.set("TEST_OPTION", "othervalue", priority)
                 mock_set.assert_called_once_with("othervalue", priority)
                 self.assertFalse(mock_setattr.called)
                 mock_set.reset_mock()
```

### Comparing `Scrapy-2.8.0/tests/test_signals.py` & `Scrapy-2.9.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_spider.py` & `Scrapy-2.9.0/tests/test_spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 )
 from scrapy.spiders.init import InitSpider
 from scrapy.utils.test import get_crawler
 from tests import get_testdata
 
 
 class SpiderTest(unittest.TestCase):
-
     spider_class = Spider
 
     def setUp(self):
         warnings.simplefilter("always")
 
     def tearDown(self):
         warnings.resetwarnings()
@@ -111,20 +110,18 @@
         spider = self.spider_class("example.com")
         with mock.patch("scrapy.spiders.Spider.logger") as mock_logger:
             spider.log("test log msg", "INFO")
         mock_logger.log.assert_called_once_with("INFO", "test log msg")
 
 
 class InitSpiderTest(SpiderTest):
-
     spider_class = InitSpider
 
 
 class XMLFeedSpiderTest(SpiderTest):
-
     spider_class = XMLFeedSpider
 
     def test_register_namespace(self):
         body = b"""<?xml version="1.0" encoding="UTF-8"?>
         <urlset xmlns:x="http://www.google.com/schemas/sitemap/0.84"
                 xmlns:y="http://www.example.com/schemas/extras/1.0">
         <url><x:loc>http://www.example.com/Special-Offers.html</loc><y:updated>2009-08-16</updated>
@@ -170,15 +167,14 @@
                     },
                 ],
                 iterator,
             )
 
 
 class CSVFeedSpiderTest(SpiderTest):
-
     spider_class = CSVFeedSpider
 
     def test_parse_rows(self):
         body = get_testdata("feeds", "feed-sample6.csv")
         response = Response("http://example.org/dummy.csv", body=body)
 
         class _CrawlSpider(self.spider_class):
@@ -192,29 +188,27 @@
         spider = _CrawlSpider()
         rows = list(spider.parse_rows(response))
         assert rows[0] == {"id": "1", "name": "alpha", "value": "foobar"}
         assert len(rows) == 4
 
 
 class CrawlSpiderTest(SpiderTest):
-
     test_body = b"""<html><head><title>Page title<title>
     <body>
     <p><a href="item/12.html">Item 12</a></p>
     <div class='links'>
     <p><a href="/about.html">About us</a></p>
     </div>
     <div>
     <p><a href="/nofollow.html">This shouldn't be followed</a></p>
     </div>
     </body></html>"""
     spider_class = CrawlSpider
 
     def test_rule_without_link_extractor(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         class _CrawlSpider(self.spider_class):
             name = "test"
             allowed_domains = ["example.org"]
@@ -230,15 +224,14 @@
                 "http://example.org/somepage/item/12.html",
                 "http://example.org/about.html",
                 "http://example.org/nofollow.html",
             ],
         )
 
     def test_process_links(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         class _CrawlSpider(self.spider_class):
             name = "test"
             allowed_domains = ["example.org"]
@@ -257,15 +250,14 @@
                 "http://example.org/somepage/item/12.html",
                 "http://example.org/about.html",
                 "http://example.org/nofollow.html",
             ],
         )
 
     def test_process_links_filter(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         class _CrawlSpider(self.spider_class):
             import re
 
@@ -286,15 +278,14 @@
             [
                 "http://example.org/somepage/item/12.html",
                 "http://example.org/about.html",
             ],
         )
 
     def test_process_links_generator(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         class _CrawlSpider(self.spider_class):
             name = "test"
             allowed_domains = ["example.org"]
@@ -314,15 +305,14 @@
                 "http://example.org/somepage/item/12.html",
                 "http://example.org/about.html",
                 "http://example.org/nofollow.html",
             ],
         )
 
     def test_process_request(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         def process_request_change_domain(request, response):
             return request.replace(url=request.url.replace(".org", ".com"))
 
@@ -343,15 +333,14 @@
                 "http://example.com/somepage/item/12.html",
                 "http://example.com/about.html",
                 "http://example.com/nofollow.html",
             ],
         )
 
     def test_process_request_with_response(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         def process_request_meta_response_class(request, response):
             request.meta["response_class"] = response.__class__.__name__
             return request
@@ -379,15 +368,14 @@
         )
         self.assertEqual(
             [r.meta["response_class"] for r in output],
             ["HtmlResponse", "HtmlResponse", "HtmlResponse"],
         )
 
     def test_process_request_instance_method(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         class _CrawlSpider(self.spider_class):
             name = "test"
             allowed_domains = ["example.org"]
@@ -406,15 +394,14 @@
                 safe_url_string("http://EXAMPLE.ORG/SOMEPAGE/ITEM/12.HTML"),
                 safe_url_string("http://EXAMPLE.ORG/ABOUT.HTML"),
                 safe_url_string("http://EXAMPLE.ORG/NOFOLLOW.HTML"),
             ],
         )
 
     def test_process_request_instance_method_with_response(self):
-
         response = HtmlResponse(
             "http://example.org/somepage/index.html", body=self.test_body
         )
 
         class _CrawlSpider(self.spider_class):
             name = "test"
             allowed_domains = ["example.org"]
@@ -463,15 +450,14 @@
         spider.start_url = "https://www.example.com"
 
         with self.assertRaisesRegex(AttributeError, r"^Crawling could not start.*$"):
             list(spider.start_requests())
 
 
 class SitemapSpiderTest(SpiderTest):
-
     spider_class = SitemapSpider
 
     BODY = b"SITEMAP"
     f = BytesIO()
     g = gzip.GzipFile(fileobj=f, mode="w+b")
     g.write(BODY)
     g.close()
@@ -685,15 +671,14 @@
 class DeprecationTest(unittest.TestCase):
     def test_crawl_spider(self):
         assert issubclass(CrawlSpider, Spider)
         assert isinstance(CrawlSpider(name="foo"), Spider)
 
 
 class NoParseMethodSpiderTest(unittest.TestCase):
-
     spider_class = Spider
 
     def test_undefined_parse_method(self):
         spider = self.spider_class("example.com")
         text = b"Random text"
         resp = TextResponse(url="http://www.example.com/random_url", body=text)
```

### Comparing `Scrapy-2.8.0/tests/test_spiderloader/__init__.py` & `Scrapy-2.9.0/tests/test_spiderloader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,21 +110,19 @@
         )
 
         crawler = runner.create_crawler("spider1")
         self.assertTrue(issubclass(crawler.spidercls, scrapy.Spider))
         self.assertEqual(crawler.spidercls.name, "spider1")
 
     def test_bad_spider_modules_exception(self):
-
         module = "tests.test_spiderloader.test_spiders.doesnotexist"
         settings = Settings({"SPIDER_MODULES": [module]})
         self.assertRaises(ImportError, SpiderLoader.from_settings, settings)
 
     def test_bad_spider_modules_warning(self):
-
         with warnings.catch_warnings(record=True) as w:
             module = "tests.test_spiderloader.test_spiders.doesnotexist"
             settings = Settings(
                 {"SPIDER_MODULES": [module], "SPIDER_LOADER_WARN_ONLY": True}
             )
             spider_loader = SpiderLoader.from_settings(settings)
             if str(w[0].message).startswith("_SixMetaPathImporter"):
```

### Comparing `Scrapy-2.8.0/tests/test_spidermiddleware.py` & `Scrapy-2.9.0/tests/test_spidermiddleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 
 class BaseAsyncSpiderMiddlewareTestCase(SpiderMiddlewareTestCase):
     """Helpers for testing sync, async and mixed middlewares.
 
     Should work for process_spider_output and, when it's supported, process_start_requests.
     """
 
+    ITEM_TYPE: type
     RESULT_COUNT = 3  # to simplify checks, let everything return 3 objects
 
     @staticmethod
     def _construct_mw_setting(*mw_classes, start_index: Optional[int] = None):
         if start_index is None:
             start_index = 10
         return {i: c for c, i in enumerate(mw_classes, start=start_index)}
```

### Comparing `Scrapy-2.8.0/tests/test_spidermiddleware_depth.py` & `Scrapy-2.9.0/tests/test_spidermiddleware_depth.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_spidermiddleware_httperror.py` & `Scrapy-2.9.0/tests/test_spidermiddleware_httperror.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_spidermiddleware_offsite.py` & `Scrapy-2.9.0/tests/test_spidermiddleware_offsite.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_spidermiddleware_output_chain.py` & `Scrapy-2.9.0/tests/test_spidermiddleware_output_chain.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_spidermiddleware_referer.py` & `Scrapy-2.9.0/tests/test_spidermiddleware_referer.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     StrictOriginWhenCrossOriginPolicy,
     UnsafeUrlPolicy,
 )
 from scrapy.spiders import Spider
 
 
 class TestRefererMiddleware(TestCase):
-
     req_meta = {}
     resp_headers = {}
     settings = {}
     scenarii = [
         ("http://scrapytest.org", "http://scrapytest.org/", b"http://scrapytest.org"),
     ]
 
@@ -47,15 +46,14 @@
     def get_request(self, target):
         return Request(target, meta=self.req_meta)
 
     def get_response(self, origin):
         return Response(origin, headers=self.resp_headers)
 
     def test(self):
-
         for origin, target, referrer in self.scenarii:
             response = self.get_response(origin)
             request = self.get_request(target)
             out = list(self.mw.process_spider_output(response, [request], self.spider))
             self.assertEqual(out[0].headers.get("Referer"), referrer)
 
 
@@ -766,15 +764,14 @@
     settings = {
         "REFERRER_POLICY": "scrapy.spidermiddlewares.referer.OriginWhenCrossOriginPolicy"
     }
     req_meta = {"referrer_policy": POLICY_UNSAFE_URL}
 
 
 class TestRequestMetaSettingFallback(TestCase):
-
     params = [
         (
             # When an unknown policy is referenced in Request.meta
             # (here, a typo error),
             # the policy defined in settings takes precedence
             {
                 "REFERRER_POLICY": "scrapy.spidermiddlewares.referer.OriginWhenCrossOriginPolicy"
@@ -820,15 +817,14 @@
             {},
             OriginWhenCrossOriginPolicy,
             True,
         ),
     ]
 
     def test(self):
-
         origin = "http://www.scrapy.org"
         target = "http://www.example.com"
 
         for (
             settings,
             response_headers,
             request_meta,
@@ -919,15 +915,14 @@
     settings = {
         "REFERRER_POLICY": "scrapy.spidermiddlewares.referer.OriginWhenCrossOriginPolicy"
     }
     resp_headers = {"Referrer-Policy": ""}
 
 
 class TestReferrerOnRedirect(TestRefererMiddleware):
-
     settings = {"REFERRER_POLICY": "scrapy.spidermiddlewares.referer.UnsafeUrlPolicy"}
     scenarii = [
         (
             "http://scrapytest.org/1",  # parent
             "http://scrapytest.org/2",  # target
             (
                 # redirections: code, URL
@@ -962,15 +957,14 @@
     def setUp(self):
         self.spider = Spider("foo")
         settings = Settings(self.settings)
         self.referrermw = RefererMiddleware(settings)
         self.redirectmw = RedirectMiddleware(settings)
 
     def test(self):
-
         for (
             parent,
             target,
             redirections,
             init_referrer,
             final_referrer,
         ) in self.scenarii:
```

### Comparing `Scrapy-2.8.0/tests/test_spidermiddleware_urllength.py` & `Scrapy-2.9.0/tests/test_spidermiddleware_urllength.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_spiderstate.py` & `Scrapy-2.9.0/tests/test_spiderstate.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_squeues.py` & `Scrapy-2.9.0/tests/test_squeues.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
 
 class ChunkSize4MarshalFifoDiskQueueTest(MarshalFifoDiskQueueTest):
     chunksize = 4
 
 
 class PickleFifoDiskQueueTest(t.FifoDiskQueueTest, FifoDiskQueueTestMixin):
-
     chunksize = 100000
 
     def queue(self):
         return _PickleFifoSerializationDiskQueue(self.qpath, chunksize=self.chunksize)
 
     def test_serialize_item(self):
         q = self.queue()
```

### Comparing `Scrapy-2.8.0/tests/test_squeues_request.py` & `Scrapy-2.9.0/tests/test_squeues_request.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_stats.py` & `Scrapy-2.9.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_toplevel.py` & `Scrapy-2.9.0/tests/test_toplevel.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_asyncgen.py` & `Scrapy-2.9.0/tests/test_utils_asyncgen.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_asyncio.py` & `Scrapy-2.9.0/tests/test_utils_asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import asyncio
 import warnings
 from unittest import TestCase
 
 from pytest import mark
 
-from scrapy.utils.reactor import install_reactor, is_asyncio_reactor_installed
+from scrapy.utils.reactor import (
+    install_reactor,
+    is_asyncio_reactor_installed,
+    set_asyncio_event_loop,
+)
 
 
 @mark.usefixtures("reactor_pytest")
 class AsyncioTest(TestCase):
     def test_is_asyncio_reactor_installed(self):
         # the result should depend only on the pytest --reactor argument
         self.assertEqual(
@@ -19,7 +24,11 @@
 
         with warnings.catch_warnings(record=True) as w:
             install_reactor("twisted.internet.asyncioreactor.AsyncioSelectorReactor")
             self.assertEqual(len(w), 0)
         from twisted.internet import reactor
 
         assert original_reactor == reactor
+
+    async def test_set_asyncio_event_loop(self):
+        install_reactor("twisted.internet.asyncioreactor.AsyncioSelectorReactor")
+        assert set_asyncio_event_loop() is asyncio.get_running_loop()
```

### Comparing `Scrapy-2.8.0/tests/test_utils_conf.py` & `Scrapy-2.9.0/tests/test_utils_conf.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_console.py` & `Scrapy-2.9.0/tests/test_utils_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,29 @@
     del IPython
 except ImportError:
     ipy = False
 
 
 class UtilsConsoleTestCase(unittest.TestCase):
     def test_get_shell_embed_func(self):
-
         shell = get_shell_embed_func(["invalid"])
         self.assertEqual(shell, None)
 
         shell = get_shell_embed_func(["invalid", "python"])
         self.assertTrue(callable(shell))
         self.assertEqual(shell.__name__, "_embed_standard_shell")
 
     @unittest.skipIf(not bpy, "bpython not available in testenv")
     def test_get_shell_embed_func2(self):
-
         shell = get_shell_embed_func(["bpython"])
         self.assertTrue(callable(shell))
         self.assertEqual(shell.__name__, "_embed_bpython_shell")
 
     @unittest.skipIf(not ipy, "IPython not available in testenv")
     def test_get_shell_embed_func3(self):
-
         # default shell should be 'ipython'
         shell = get_shell_embed_func()
         self.assertEqual(shell.__name__, "_embed_ipython_shell")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `Scrapy-2.8.0/tests/test_utils_curl.py` & `Scrapy-2.9.0/tests/test_utils_curl.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,23 @@
                 "excerptLength=200&enableDidYouMean=true&sortCriteria=ffirstz3"
                 "2xnamez32x201740686%20ascending&queryFunctions=%5B%5D&ranking"
                 "Functions=%5B%5D"
             ),
         }
         self._test_command(curl_command, expected_result)
 
+    def test_post_data_raw_with_string_prefix(self):
+        curl_command = "curl 'https://www.example.org/' --data-raw $'{\"$filters\":\"Filter\u0021\"}'"
+        expected_result = {
+            "method": "POST",
+            "url": "https://www.example.org/",
+            "body": '{"$filters":"Filter!"}',
+        }
+        self._test_command(curl_command, expected_result)
+
     def test_explicit_get_with_data(self):
         curl_command = "curl httpbin.org/anything -X GET --data asdf"
         expected_result = {
             "method": "GET",
             "url": "http://httpbin.org/anything",
             "body": "asdf",
         }
```

### Comparing `Scrapy-2.8.0/tests/test_utils_datatypes.py` & `Scrapy-2.9.0/tests/test_utils_datatypes.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_defer.py` & `Scrapy-2.9.0/tests/test_utils_defer.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_deprecate.py` & `Scrapy-2.9.0/tests/test_utils_deprecate.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_display.py` & `Scrapy-2.9.0/tests/test_utils_display.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_gz.py` & `Scrapy-2.9.0/tests/test_utils_gz.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_httpobj.py` & `Scrapy-2.9.0/tests/test_utils_httpobj.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_iterators.py` & `Scrapy-2.9.0/tests/test_utils_iterators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from scrapy.http import Response, TextResponse, XmlResponse
 from scrapy.utils.iterators import _body_or_str, csviter, xmliter, xmliter_lxml
 from tests import get_testdata
 
 
 class XmliterTestCase(unittest.TestCase):
-
     xmliter = staticmethod(xmliter)
 
     def test_xmliter(self):
         body = b"""
             <?xml version="1.0" encoding="UTF-8"?>
             <products xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                       xsi:noNamespaceSchemaLocation="someschmea.xsd">
@@ -524,11 +523,7 @@
             self.assertTrue(type(r1) is not type(r3))
 
     def _assert_type_and_value(self, a, b, obj):
         self.assertTrue(
             type(a) is type(b), f"Got {type(a)}, expected {type(b)} for { obj!r}"
         )
         self.assertEqual(a, b)
-
-
-if __name__ == "__main__":
-    unittest.main()
```

### Comparing `Scrapy-2.8.0/tests/test_utils_log.py` & `Scrapy-2.9.0/tests/test_utils_log.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_misc/__init__.py` & `Scrapy-2.9.0/tests/test_utils_misc/__init__.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_misc/test.egg` & `Scrapy-2.9.0/tests/test_utils_misc/test.egg`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_misc/test_return_with_argument_inside_generator.py` & `Scrapy-2.9.0/tests/test_utils_misc/test_return_with_argument_inside_generator.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_project.py` & `Scrapy-2.9.0/tests/test_utils_project.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_python.py` & `Scrapy-2.9.0/tests/test_utils_python.py`

 * *Files 5% similar despite different names*

```diff
@@ -231,33 +231,25 @@
         self.assertEqual(get_func_args(A), ["a", "b", "c"])
         self.assertEqual(get_func_args(a.method), ["a", "b", "c"])
         self.assertEqual(get_func_args(partial_f1), ["b", "c"])
         self.assertEqual(get_func_args(partial_f2), ["a", "c"])
         self.assertEqual(get_func_args(partial_f3), ["c"])
         self.assertEqual(get_func_args(cal), ["a", "b", "c"])
         self.assertEqual(get_func_args(object), [])
+        self.assertEqual(get_func_args(str.split, stripself=True), ["sep", "maxsplit"])
+        self.assertEqual(get_func_args(" ".join, stripself=True), ["iterable"])
 
         if platform.python_implementation() == "CPython":
-            # TODO: how do we fix this to return the actual argument names?
-            self.assertEqual(get_func_args(str.split), [])
-            self.assertEqual(get_func_args(" ".join), [])
+            # doesn't work on CPython: https://bugs.python.org/issue42785
             self.assertEqual(get_func_args(operator.itemgetter(2)), [])
         elif platform.python_implementation() == "PyPy":
             self.assertEqual(
-                get_func_args(str.split, stripself=True), ["sep", "maxsplit"]
-            )
-            self.assertEqual(
                 get_func_args(operator.itemgetter(2), stripself=True), ["obj"]
             )
-            self.assertEqual(get_func_args(" ".join, stripself=True), ["iterable"])
 
     def test_without_none_values(self):
         self.assertEqual(without_none_values([1, None, 3, 4]), [1, 3, 4])
         self.assertEqual(without_none_values((1, None, 3, 4)), (1, 3, 4))
         self.assertEqual(
             without_none_values({"one": 1, "none": None, "three": 3, "four": 4}),
             {"one": 1, "three": 3, "four": 4},
         )
-
-
-if __name__ == "__main__":
-    unittest.main()
```

### Comparing `Scrapy-2.8.0/tests/test_utils_request.py` & `Scrapy-2.9.0/tests/test_utils_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import unittest
 import warnings
 from hashlib import sha1
 from typing import Dict, Mapping, Optional, Tuple, Union
 from weakref import WeakKeyDictionary
 
 import pytest
@@ -14,14 +15,15 @@
     _deprecated_fingerprint_cache,
     _fingerprint_cache,
     _request_fingerprint_as_bytes,
     fingerprint,
     request_authenticate,
     request_fingerprint,
     request_httprepr,
+    request_to_curl,
 )
 from scrapy.utils.test import get_crawler
 
 
 class UtilsRequestTest(unittest.TestCase):
     def test_request_authenticate(self):
         r = Request("http://www.example.com")
@@ -458,15 +460,14 @@
 
     def test_custom_component_backward_compatibility(self):
         """Tests that the backward-compatible request fingerprinting class featured
         in the documentation is indeed backward compatible and does not cause a
         warning to be logged."""
 
         class RequestFingerprinter:
-
             cache = WeakKeyDictionary()
 
             def fingerprint(self, request):
                 if request not in self.cache:
                     fp = sha1()
                     fp.update(to_bytes(request.method))
                     fp.update(to_bytes(canonicalize_url(request.url)))
@@ -637,15 +638,14 @@
 
         request = Request("http://www.example.com")
         fingerprint = crawler.request_fingerprinter.fingerprint(request)
         self.assertEqual(fingerprint, settings["FINGERPRINT"])
 
     def test_from_crawler_and_settings(self):
         class RequestFingerprinter:
-
             # This method is ignored due to the presence of from_crawler
             @classmethod
             def from_settings(cls, settings):
                 return cls(settings)
 
             @classmethod
             def from_crawler(cls, crawler):
@@ -664,9 +664,71 @@
         crawler = get_crawler(settings_dict=settings)
 
         request = Request("http://www.example.com")
         fingerprint = crawler.request_fingerprinter.fingerprint(request)
         self.assertEqual(fingerprint, settings["FINGERPRINT"])
 
 
+class RequestToCurlTest(unittest.TestCase):
+    def _test_request(self, request_object, expected_curl_command):
+        curl_command = request_to_curl(request_object)
+        self.assertEqual(curl_command, expected_curl_command)
+
+    def test_get(self):
+        request_object = Request("https://www.example.com")
+        expected_curl_command = "curl -X GET https://www.example.com"
+        self._test_request(request_object, expected_curl_command)
+
+    def test_post(self):
+        request_object = Request(
+            "https://www.httpbin.org/post",
+            method="POST",
+            body=json.dumps({"foo": "bar"}),
+        )
+        expected_curl_command = (
+            'curl -X POST https://www.httpbin.org/post --data-raw \'{"foo": "bar"}\''
+        )
+        self._test_request(request_object, expected_curl_command)
+
+    def test_headers(self):
+        request_object = Request(
+            "https://www.httpbin.org/post",
+            method="POST",
+            headers={"Content-Type": "application/json", "Accept": "application/json"},
+            body=json.dumps({"foo": "bar"}),
+        )
+        expected_curl_command = (
+            "curl -X POST https://www.httpbin.org/post"
+            ' --data-raw \'{"foo": "bar"}\''
+            " -H 'Content-Type: application/json' -H 'Accept: application/json'"
+        )
+        self._test_request(request_object, expected_curl_command)
+
+    def test_cookies_dict(self):
+        request_object = Request(
+            "https://www.httpbin.org/post",
+            method="POST",
+            cookies={"foo": "bar"},
+            body=json.dumps({"foo": "bar"}),
+        )
+        expected_curl_command = (
+            "curl -X POST https://www.httpbin.org/post"
+            " --data-raw '{\"foo\": \"bar\"}' --cookie 'foo=bar'"
+        )
+        self._test_request(request_object, expected_curl_command)
+
+    def test_cookies_list(self):
+        request_object = Request(
+            "https://www.httpbin.org/post",
+            method="POST",
+            cookies=[{"foo": "bar"}],
+            body=json.dumps({"foo": "bar"}),
+        )
+        expected_curl_command = (
+            "curl -X POST https://www.httpbin.org/post"
+            " --data-raw '{\"foo\": \"bar\"}' --cookie 'foo=bar'"
+        )
+        self._test_request(request_object, expected_curl_command)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `Scrapy-2.8.0/tests/test_utils_response.py` & `Scrapy-2.9.0/tests/test_utils_response.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_serialize.py` & `Scrapy-2.9.0/tests/test_utils_serialize.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_signal.py` & `Scrapy-2.9.0/tests/test_utils_signal.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_sitemap.py` & `Scrapy-2.9.0/tests/test_utils_sitemap.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_spider.py` & `Scrapy-2.9.0/tests/test_utils_spider.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_template.py` & `Scrapy-2.9.0/tests/test_utils_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     def setUp(self):
         self.tmp_path = mkdtemp()
 
     def tearDown(self):
         rmtree(self.tmp_path)
 
     def test_simple_render(self):
-
         context = dict(project_name="proj", name="spi", classname="TheSpider")
         template = "from ${project_name}.spiders.${name} import ${classname}"
         rendered = "from proj.spiders.spi import TheSpider"
 
         template_path = Path(self.tmp_path, "templ.py.tmpl")
         render_path = Path(self.tmp_path, "templ.py")
```

### Comparing `Scrapy-2.8.0/tests/test_utils_trackref.py` & `Scrapy-2.9.0/tests/test_utils_trackref.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_utils_url.py` & `Scrapy-2.9.0/tests/test_utils_url.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tests/test_webclient.py` & `Scrapy-2.9.0/tests/test_webclient.py`

 * *Files identical despite different names*

### Comparing `Scrapy-2.8.0/tox.ini` & `Scrapy-2.9.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = security,flake8,black,typing,py
+envlist = pre-commit,pylint,typing,py
 minversion = 1.7.0
 
 [testenv]
 deps =
     -rtests/requirements.txt
     # mitmproxy does not support PyPy
     # Python 3.9+ requires mitmproxy >= 5.3.0
@@ -26,59 +26,51 @@
     AWS_SECRET_ACCESS_KEY
     AWS_SESSION_TOKEN
     GCS_TEST_FILE_URI
     GCS_PROJECT_ID
 #allow tox virtualenv to upgrade pip/wheel/setuptools
 download = true
 commands =
-    pytest --cov=scrapy --cov-report=xml --cov-report= {posargs:--durations=10 docs scrapy tests}
+    pytest --cov=scrapy --cov-report=xml --cov-report= {posargs:--durations=10 docs scrapy tests} --doctest-modules
 install_command =
     python -I -m pip install -ctests/upper-constraints.txt {opts} {packages}
 
 [testenv:typing]
 basepython = python3
 deps =
-    lxml-stubs==0.2.0
-    mypy==0.991
+    mypy==1.2.0
     types-attrs==19.1.0
-    types-pyOpenSSL==21.0.0
-    types-setuptools==57.0.0
+    types-lxml==2023.3.28
+    types-Pillow==9.4.0.19
+    types-Pygments==2.14.0.7
+    types-pyOpenSSL==23.1.0.1
+    types-setuptools==67.6.0.7
 commands =
     mypy --show-error-codes {posargs: scrapy tests}
 
-[testenv:security]
+[testenv:pre-commit]
 basepython = python3
 deps =
-    bandit==1.7.4
+    pre-commit
 commands =
-    bandit -r -c .bandit.yml {posargs:scrapy}
-
-[testenv:flake8]
-basepython = python3
-deps =
-    {[testenv]deps}
-    # Twisted[http2] is required to import some files
-    Twisted[http2]>=17.9.0
-    flake8==6.0.0
-commands =
-    flake8 {posargs:docs scrapy tests}
+    pre-commit run {posargs:--all-files}
 
 [testenv:pylint]
 basepython = python3
 deps =
     {[testenv:extra-deps]deps}
-    pylint==2.15.6
+    pylint==2.17.2
 commands =
     pylint conftest.py docs extras scrapy setup.py tests
 
 [testenv:twinecheck]
 basepython = python3
 deps =
-    twine==4.0.1
-    build==0.9.0
+    twine==4.0.2
+    build==0.10.0
 commands =
     python -m build --sdist
     twine check dist/*
 
 [pinned]
 deps =
     cryptography==3.4.6
@@ -103,31 +95,36 @@
     botocore==1.4.87
     google-cloud-storage==1.29.0
     Pillow==7.1.0
 setenv =
     _SCRAPY_PINNED=true
 install_command =
     python -I -m pip install {opts} {packages}
+commands =
+    pytest --cov=scrapy --cov-report=xml --cov-report= {posargs:--durations=10 scrapy tests}
 
 [testenv:pinned]
+basepython = python3.7
 deps =
     {[pinned]deps}
     PyDispatcher==2.0.5
 install_command = {[pinned]install_command}
 setenv =
     {[pinned]setenv}
+commands = {[pinned]commands}
 
 [testenv:windows-pinned]
 basepython = python3
 deps =
     {[pinned]deps}
     PyDispatcher==2.0.5
 install_command = {[pinned]install_command}
 setenv =
     {[pinned]setenv}
+commands = {[pinned]commands}
 
 [testenv:extra-deps]
 basepython = python3
 deps =
     {[testenv]deps}
     boto
     google-cloud-storage
@@ -140,30 +137,31 @@
 
 [testenv:asyncio]
 commands =
     {[testenv]commands} --reactor=asyncio
 
 [testenv:asyncio-pinned]
 deps = {[testenv:pinned]deps}
-commands = {[testenv:asyncio]commands}
+commands = {[pinned]commands} --reactor=asyncio
 install_command = {[pinned]install_command}
 setenv =
     {[pinned]setenv}
 
 [testenv:pypy3]
 basepython = pypy3
 commands =
     pytest {posargs:--durations=10 docs scrapy tests}
 
 [testenv:pypy3-pinned]
 basepython = {[testenv:pypy3]basepython}
 deps =
     {[pinned]deps}
     PyPyDispatcher==2.1.0
-commands = {[testenv:pypy3]commands}
+commands =
+    pytest --durations=10 scrapy tests
 install_command = {[pinned]install_command}
 setenv =
     {[pinned]setenv}
 
 [docs]
 changedir = docs
 deps =
@@ -191,13 +189,7 @@
 [testenv:docs-links]
 basepython = python3
 changedir = {[docs]changedir}
 deps = {[docs]deps}
 setenv = {[docs]setenv}
 commands =
     sphinx-build -W -b linkcheck . {envtmpdir}/linkcheck
-
-[testenv:black]
-deps =
-    black==22.12.0
-commands =
-    black {posargs:--check .}
```

