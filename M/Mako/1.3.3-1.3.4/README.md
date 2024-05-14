# Comparing `tmp/Mako-1.3.3.tar.gz` & `tmp/Mako-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mako-1.3.3.tar", last modified: Wed Apr 10 15:30:54 2024, max compression
+gzip compressed data, was "Mako-1.3.4.tar", last modified: Tue May 14 01:17:19 2024, max compression
```

## Comparing `Mako-1.3.3.tar` & `Mako-1.3.4.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.210187 Mako-1.3.3/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.195187 Mako-1.3.3/.github/
--rw-r--r--   0 classic   (1000) classic   (1000)      111 2024-04-10 15:30:43.000000 Mako-1.3.3/.github/FUNDING.yml
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.196187 Mako-1.3.3/.github/workflows/
--rw-r--r--   0 classic   (1000) classic   (1000)     1121 2024-04-10 15:30:43.000000 Mako-1.3.3/.github/workflows/run-on-pr.yaml
--rw-r--r--   0 classic   (1000) classic   (1000)     1481 2024-04-10 15:30:43.000000 Mako-1.3.3/.github/workflows/run-test.yaml
--rw-r--r--   0 classic   (1000) classic   (1000)      131 2024-04-10 15:30:43.000000 Mako-1.3.3/.gitignore
--rw-r--r--   0 classic   (1000) classic   (1000)       79 2024-04-10 15:30:43.000000 Mako-1.3.3/.gitreview
--rw-r--r--   0 classic   (1000) classic   (1000)      302 2024-04-10 15:30:43.000000 Mako-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0 classic   (1000) classic   (1000)      282 2024-04-10 15:30:43.000000 Mako-1.3.3/AUTHORS
--rw-r--r--   0 classic   (1000) classic   (1000)      179 2024-04-10 15:30:43.000000 Mako-1.3.3/CHANGES
--rw-r--r--   0 classic   (1000) classic   (1000)     1098 2024-04-10 15:30:43.000000 Mako-1.3.3/LICENSE
--rw-r--r--   0 classic   (1000) classic   (1000)      266 2024-04-10 15:30:43.000000 Mako-1.3.3/MANIFEST.in
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.196187 Mako-1.3.3/Mako.egg-info/
--rw-r--r--   0 classic   (1000) classic   (1000)     2896 2024-04-10 15:30:54.000000 Mako-1.3.3/Mako.egg-info/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     4690 2024-04-10 15:30:54.000000 Mako-1.3.3/Mako.egg-info/SOURCES.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-04-10 15:30:54.000000 Mako-1.3.3/Mako.egg-info/dependency_links.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      512 2024-04-10 15:30:54.000000 Mako-1.3.3/Mako.egg-info/entry_points.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-04-10 15:30:54.000000 Mako-1.3.3/Mako.egg-info/not-zip-safe
--rw-r--r--   0 classic   (1000) classic   (1000)       68 2024-04-10 15:30:54.000000 Mako-1.3.3/Mako.egg-info/requires.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        5 2024-04-10 15:30:54.000000 Mako-1.3.3/Mako.egg-info/top_level.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     2896 2024-04-10 15:30:54.210187 Mako-1.3.3/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     1459 2024-04-10 15:30:43.000000 Mako-1.3.3/README.rst
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.198187 Mako-1.3.3/doc/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.199187 Mako-1.3.3/doc/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)     4289 2024-04-10 15:30:52.000000 Mako-1.3.3/doc/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 classic   (1000) classic   (1000)    15094 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/_static/basic.css
--rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-11-08 19:26:03.000000 Mako-1.3.3/doc/_static/changelog.css
--rw-r--r--   0 classic   (1000) classic   (1000)     7177 2024-03-04 13:24:31.000000 Mako-1.3.3/doc/_static/docs.css
--rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-11-08 19:25:57.000000 Mako-1.3.3/doc/_static/doctools.js
--rw-r--r--   0 classic   (1000) classic   (1000)      329 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/_static/documentation_options.js
--rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-11-08 19:25:57.000000 Mako-1.3.3/doc/_static/file.png
--rw-r--r--   0 classic   (1000) classic   (1000)    89501 2024-04-10 15:30:52.000000 Mako-1.3.3/doc/_static/jquery.js
--rw-r--r--   0 classic   (1000) classic   (1000)     4758 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/_static/language_data.js
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-11-08 19:25:57.000000 Mako-1.3.3/doc/_static/minus.png
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-11-08 19:25:57.000000 Mako-1.3.3/doc/_static/plus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4929 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/_static/pygments.css
--rw-r--r--   0 classic   (1000) classic   (1000)    18732 2023-11-08 19:25:57.000000 Mako-1.3.3/doc/_static/searchtools.js
--rw-r--r--   0 classic   (1000) classic   (1000)     5123 2023-11-08 19:25:57.000000 Mako-1.3.3/doc/_static/sphinx_highlight.js
--rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-11-08 19:26:03.000000 Mako-1.3.3/doc/_static/sphinx_paramlinks.css
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.200187 Mako-1.3.3/doc/build/
--rw-r--r--   0 classic   (1000) classic   (1000)     4863 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/Makefile
--rw-r--r--   0 classic   (1000) classic   (1000)    13676 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/caching.rst
--rw-------   0 classic   (1000) classic   (1000)    69705 2024-04-10 15:30:51.000000 Mako-1.3.3/doc/build/changelog.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     9571 2024-04-10 15:30:51.000000 Mako-1.3.3/doc/build/conf.py
--rw-r--r--   0 classic   (1000) classic   (1000)    17708 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/defs.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    11278 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/filtering.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      268 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/index.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    19744 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/inheritance.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    14575 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/namespaces.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      217 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/requirements.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    16137 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/runtime.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    14103 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/syntax.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     5391 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/unicode.rst
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.200187 Mako-1.3.3/doc/build/unreleased/
--rw-r--r--   0 classic   (1000) classic   (1000)      385 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/unreleased/README.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    17836 2024-04-10 15:30:43.000000 Mako-1.3.3/doc/build/usage.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    85770 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/caching.html
--rw-r--r--   0 classic   (1000) classic   (1000)   180555 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/changelog.html
--rw-r--r--   0 classic   (1000) classic   (1000)    56857 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/defs.html
--rw-r--r--   0 classic   (1000) classic   (1000)    36801 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/filtering.html
--rw-r--r--   0 classic   (1000) classic   (1000)    26164 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/genindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    12769 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)    61365 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/inheritance.html
--rw-r--r--   0 classic   (1000) classic   (1000)    86600 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/namespaces.html
--rw-r--r--   0 classic   (1000) classic   (1000)    69788 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/runtime.html
--rw-r--r--   0 classic   (1000) classic   (1000)     3812 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/search.html
--rw-r--r--   0 classic   (1000) classic   (1000)    63587 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/searchindex.js
--rw-r--r--   0 classic   (1000) classic   (1000)    44381 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/syntax.html
--rw-r--r--   0 classic   (1000) classic   (1000)    18276 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/unicode.html
--rw-r--r--   0 classic   (1000) classic   (1000)   137745 2024-04-10 15:30:53.000000 Mako-1.3.3/doc/usage.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.194187 Mako-1.3.3/examples/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.200187 Mako-1.3.3/examples/bench/
--rw-r--r--   0 classic   (1000) classic   (1000)     6593 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/basic.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.201187 Mako-1.3.3/examples/bench/cheetah/
--rw-r--r--   0 classic   (1000) classic   (1000)       25 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/cheetah/footer.tmpl
--rw-r--r--   0 classic   (1000) classic   (1000)       45 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/cheetah/header.tmpl
--rw-r--r--   0 classic   (1000) classic   (1000)      678 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/cheetah/template.tmpl
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.194187 Mako-1.3.3/examples/bench/django/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.201187 Mako-1.3.3/examples/bench/django/templates/
--rw-r--r--   0 classic   (1000) classic   (1000)      335 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/django/templates/base.html
--rw-r--r--   0 classic   (1000) classic   (1000)      410 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/django/templates/template.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.201187 Mako-1.3.3/examples/bench/django/templatetags/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/django/templatetags/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)      199 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/django/templatetags/bench.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.201187 Mako-1.3.3/examples/bench/genshi/
--rw-r--r--   0 classic   (1000) classic   (1000)      310 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/genshi/base.html
--rw-r--r--   0 classic   (1000) classic   (1000)      667 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/genshi/template.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.201187 Mako-1.3.3/examples/bench/jinja2/
--rw-r--r--   0 classic   (1000) classic   (1000)       25 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/jinja2/footer.html
--rw-r--r--   0 classic   (1000) classic   (1000)       48 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/jinja2/header.html
--rw-r--r--   0 classic   (1000) classic   (1000)      694 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/jinja2/template.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.201187 Mako-1.3.3/examples/bench/jinja2_inheritance/
--rw-r--r--   0 classic   (1000) classic   (1000)      454 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/jinja2_inheritance/base.html
--rw-r--r--   0 classic   (1000) classic   (1000)      357 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/jinja2_inheritance/template.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.202187 Mako-1.3.3/examples/bench/kid/
--rw-r--r--   0 classic   (1000) classic   (1000)      336 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/kid/base.kid
--rw-r--r--   0 classic   (1000) classic   (1000)      610 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/kid/template.kid
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.202187 Mako-1.3.3/examples/bench/mako/
--rw-r--r--   0 classic   (1000) classic   (1000)       25 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/mako/footer.html
--rw-r--r--   0 classic   (1000) classic   (1000)       47 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/mako/header.html
--rw-r--r--   0 classic   (1000) classic   (1000)      670 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/mako/template.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.202187 Mako-1.3.3/examples/bench/mako_inheritance/
--rw-r--r--   0 classic   (1000) classic   (1000)      405 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/mako_inheritance/base.html
--rw-r--r--   0 classic   (1000) classic   (1000)      285 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/mako_inheritance/template.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.202187 Mako-1.3.3/examples/bench/myghty/
--rw-r--r--   0 classic   (1000) classic   (1000)      431 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/myghty/base.myt
--rw-r--r--   0 classic   (1000) classic   (1000)      505 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/bench/myghty/template.myt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.202187 Mako-1.3.3/examples/wsgi/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.202187 Mako-1.3.3/examples/wsgi/htdocs/
--rw-r--r--   0 classic   (1000) classic   (1000)      106 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/wsgi/htdocs/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)     2472 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/wsgi/run_wsgi.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.202187 Mako-1.3.3/examples/wsgi/templates/
--rw-r--r--   0 classic   (1000) classic   (1000)       80 2024-04-10 15:30:43.000000 Mako-1.3.3/examples/wsgi/templates/root.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.204187 Mako-1.3.3/mako/
--rw-r--r--   0 classic   (1000) classic   (1000)      242 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    20247 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/_ast_util.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6642 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ast.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7680 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/cache.py
--rwxr-xr-x   0 classic   (1000) classic   (1000)     2813 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/cmd.py
--rw-r--r--   0 classic   (1000) classic   (1000)    47736 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/codegen.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1820 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/compat.py
--rw-r--r--   0 classic   (1000) classic   (1000)    12530 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/exceptions.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.204187 Mako-1.3.3/mako/ext/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1885 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/autohandler.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2091 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/babelplugin.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2578 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/beaker_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4659 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/extract.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1935 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/linguaplugin.py
--rw-r--r--   0 classic   (1000) classic   (1000)      576 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/preprocessors.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4753 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/pygmentplugin.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2141 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/ext/turbogears.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4658 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/filters.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16324 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/lexer.py
--rw-r--r--   0 classic   (1000) classic   (1000)    12428 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/lookup.py
--rw-r--r--   0 classic   (1000) classic   (1000)    19007 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/parsetree.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10416 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/pygen.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7656 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/pyparser.py
--rw-r--r--   0 classic   (1000) classic   (1000)    27804 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/runtime.py
--rw-r--r--   0 classic   (1000) classic   (1000)    23857 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/template.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.205187 Mako-1.3.3/mako/testing/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/testing/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3566 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/testing/_config.py
--rw-r--r--   0 classic   (1000) classic   (1000)     5161 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/testing/assertions.py
--rw-r--r--   0 classic   (1000) classic   (1000)      323 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/testing/config.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1553 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/testing/exclusions.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3044 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/testing/fixtures.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1623 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/testing/helpers.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10638 2024-04-10 15:30:43.000000 Mako-1.3.3/mako/util.py
--rw-r--r--   0 classic   (1000) classic   (1000)      153 2024-04-10 15:30:43.000000 Mako-1.3.3/pyproject.toml
--rw-r--r--   0 classic   (1000) classic   (1000)     2533 2024-04-10 15:30:54.210187 Mako-1.3.3/setup.cfg
--rw-r--r--   0 classic   (1000) classic   (1000)       38 2024-04-10 15:30:43.000000 Mako-1.3.3/setup.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.207187 Mako-1.3.3/test/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:43.000000 Mako-1.3.3/test/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.207187 Mako-1.3.3/test/ext/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:43.000000 Mako-1.3.3/test/ext/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3932 2024-04-10 15:30:43.000000 Mako-1.3.3/test/ext/test_babelplugin.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1802 2024-04-10 15:30:43.000000 Mako-1.3.3/test/ext/test_linguaplugin.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.207187 Mako-1.3.3/test/foo/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:43.000000 Mako-1.3.3/test/foo/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)      145 2024-04-10 15:30:43.000000 Mako-1.3.3/test/foo/mod_no_encoding.py
--rw-r--r--   0 classic   (1000) classic   (1000)      181 2024-04-10 15:30:43.000000 Mako-1.3.3/test/foo/test_ns.py
--rw-r--r--   0 classic   (1000) classic   (1000)       30 2024-04-10 15:30:43.000000 Mako-1.3.3/test/module_to_import.py
--rw-r--r--   0 classic   (1000) classic   (1000)      151 2024-04-10 15:30:43.000000 Mako-1.3.3/test/sample_module_namespace.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.209187 Mako-1.3.3/test/templates/
--rw-r--r--   0 classic   (1000) classic   (1000)      192 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/badbom.html
--rw-r--r--   0 classic   (1000) classic   (1000)      167 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/bom.html
--rw-r--r--   0 classic   (1000) classic   (1000)      192 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/bommagic.html
--rw-r--r--   0 classic   (1000) classic   (1000)      157 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/chs_unicode_py3k.html
--rw-r--r--   0 classic   (1000) classic   (1000)      290 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/chs_utf8.html
--rw-r--r--   0 classic   (1000) classic   (1000)       16 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/cmd_good.mako
--rw-r--r--   0 classic   (1000) classic   (1000)        4 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/cmd_runtime.mako
--rw-r--r--   0 classic   (1000) classic   (1000)        3 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/cmd_syntax.mako
--rw-r--r--   0 classic   (1000) classic   (1000)      252 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/crlf.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.209187 Mako-1.3.3/test/templates/foo/
--rw-r--r--   0 classic   (1000) classic   (1000)      703 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/foo/modtest.html.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2432 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/gettext.mako
--rw-r--r--   0 classic   (1000) classic   (1000)       13 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/gettext_cp1251.mako
--rw-r--r--   0 classic   (1000) classic   (1000)       14 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/gettext_utf8.mako
--rw-r--r--   0 classic   (1000) classic   (1000)       13 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)    58538 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/internationalization.html
--rw-r--r--   0 classic   (1000) classic   (1000)       14 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/modtest.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.209187 Mako-1.3.3/test/templates/othersubdir/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/othersubdir/foo.html
--rw-r--r--   0 classic   (1000) classic   (1000)      233 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/read_unicode_py3k.html
--rw-r--r--   0 classic   (1000) classic   (1000)       29 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/runtimeerr_py3k.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.209187 Mako-1.3.3/test/templates/subdir/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.209187 Mako-1.3.3/test/templates/subdir/foo/
--rw-r--r--   0 classic   (1000) classic   (1000)      724 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/subdir/foo/modtest.html.py
--rw-r--r--   0 classic   (1000) classic   (1000)       23 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/subdir/incl.html
--rw-r--r--   0 classic   (1000) classic   (1000)       56 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/subdir/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)       14 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/subdir/modtest.html
--rw-r--r--   0 classic   (1000) classic   (1000)      189 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/unicode.html
--rw-r--r--   0 classic   (1000) classic   (1000)      289 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/unicode_arguments_py3k.html
--rw-r--r--   0 classic   (1000) classic   (1000)      153 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/unicode_code_py3k.html
--rw-r--r--   0 classic   (1000) classic   (1000)      195 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/unicode_expr_py3k.html
--rw-r--r--   0 classic   (1000) classic   (1000)      212 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/unicode_runtime_error.html
--rw-r--r--   0 classic   (1000) classic   (1000)      200 2024-04-10 15:30:43.000000 Mako-1.3.3/test/templates/unicode_syntax_error.html
--rw-r--r--   0 classic   (1000) classic   (1000)    11558 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_ast.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16038 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_block.py
--rw-r--r--   0 classic   (1000) classic   (1000)    18518 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)    14039 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_call.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3392 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_cmd.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3282 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_decorators.py
--rw-r--r--   0 classic   (1000) classic   (1000)    17699 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_def.py
--rw-r--r--   0 classic   (1000) classic   (1000)    11474 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_exceptions.py
--rw-r--r--   0 classic   (1000) classic   (1000)    11088 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_filters.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10782 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_inheritance.py
--rw-r--r--   0 classic   (1000) classic   (1000)    38286 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_lexer.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4836 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_lookup.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10401 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_loop.py
--rw-r--r--   0 classic   (1000) classic   (1000)      829 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_lru.py
--rw-r--r--   0 classic   (1000) classic   (1000)    24878 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_namespace.py
--rw-r--r--   0 classic   (1000) classic   (1000)     5688 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_pygen.py
--rw-r--r--   0 classic   (1000) classic   (1000)      503 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_runtime.py
--rw-r--r--   0 classic   (1000) classic   (1000)    50653 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_template.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1561 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_tgplugin.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1936 2024-04-10 15:30:43.000000 Mako-1.3.3/test/test_util.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-04-10 15:30:54.209187 Mako-1.3.3/test/testing/
--rw-r--r--   0 classic   (1000) classic   (1000)      363 2024-04-10 15:30:43.000000 Mako-1.3.3/test/testing/dummy.cfg
--rw-r--r--   0 classic   (1000) classic   (1000)     4622 2024-04-10 15:30:43.000000 Mako-1.3.3/test/testing/test_config.py
--rw-r--r--   0 classic   (1000) classic   (1000)      661 2024-04-10 15:30:43.000000 Mako-1.3.3/tox.ini
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.515633 Mako-1.3.4/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.500634 Mako-1.3.4/.github/
+-rw-r--r--   0 classic   (1000) classic   (1000)      111 2024-05-14 01:17:05.000000 Mako-1.3.4/.github/FUNDING.yml
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.500634 Mako-1.3.4/.github/workflows/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1121 2024-05-14 01:17:05.000000 Mako-1.3.4/.github/workflows/run-on-pr.yaml
+-rw-r--r--   0 classic   (1000) classic   (1000)     1481 2024-05-14 01:17:05.000000 Mako-1.3.4/.github/workflows/run-test.yaml
+-rw-r--r--   0 classic   (1000) classic   (1000)      131 2024-05-14 01:17:05.000000 Mako-1.3.4/.gitignore
+-rw-r--r--   0 classic   (1000) classic   (1000)       79 2024-05-14 01:17:05.000000 Mako-1.3.4/.gitreview
+-rw-r--r--   0 classic   (1000) classic   (1000)      302 2024-05-14 01:17:05.000000 Mako-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 classic   (1000) classic   (1000)      282 2024-05-14 01:17:05.000000 Mako-1.3.4/AUTHORS
+-rw-r--r--   0 classic   (1000) classic   (1000)      179 2024-05-14 01:17:05.000000 Mako-1.3.4/CHANGES
+-rw-r--r--   0 classic   (1000) classic   (1000)     1098 2024-05-14 01:17:05.000000 Mako-1.3.4/LICENSE
+-rw-r--r--   0 classic   (1000) classic   (1000)      266 2024-05-14 01:17:05.000000 Mako-1.3.4/MANIFEST.in
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.501634 Mako-1.3.4/Mako.egg-info/
+-rw-r--r--   0 classic   (1000) classic   (1000)     2896 2024-05-14 01:17:19.000000 Mako-1.3.4/Mako.egg-info/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     4690 2024-05-14 01:17:19.000000 Mako-1.3.4/Mako.egg-info/SOURCES.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-05-14 01:17:19.000000 Mako-1.3.4/Mako.egg-info/dependency_links.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      512 2024-05-14 01:17:19.000000 Mako-1.3.4/Mako.egg-info/entry_points.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-05-14 01:17:19.000000 Mako-1.3.4/Mako.egg-info/not-zip-safe
+-rw-r--r--   0 classic   (1000) classic   (1000)       68 2024-05-14 01:17:19.000000 Mako-1.3.4/Mako.egg-info/requires.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        5 2024-05-14 01:17:19.000000 Mako-1.3.4/Mako.egg-info/top_level.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     2896 2024-05-14 01:17:19.515633 Mako-1.3.4/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     1459 2024-05-14 01:17:05.000000 Mako-1.3.4/README.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.502634 Mako-1.3.4/doc/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.504634 Mako-1.3.4/doc/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)     4289 2024-05-14 01:17:17.000000 Mako-1.3.4/doc/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 classic   (1000) classic   (1000)    15094 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/_static/basic.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      107 2024-05-05 17:52:31.000000 Mako-1.3.4/doc/_static/changelog.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     7177 2024-05-05 17:52:31.000000 Mako-1.3.4/doc/_static/docs.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4472 2024-05-14 01:17:16.000000 Mako-1.3.4/doc/_static/doctools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      329 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/_static/documentation_options.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      286 2024-05-14 01:17:16.000000 Mako-1.3.4/doc/_static/file.png
+-rw-r--r--   0 classic   (1000) classic   (1000)    89501 2024-05-14 01:17:17.000000 Mako-1.3.4/doc/_static/jquery.js
+-rw-r--r--   0 classic   (1000) classic   (1000)     4758 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/_static/language_data.js
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2024-05-14 01:17:16.000000 Mako-1.3.4/doc/_static/minus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2024-05-14 01:17:16.000000 Mako-1.3.4/doc/_static/plus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4929 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/_static/pygments.css
+-rw-r--r--   0 classic   (1000) classic   (1000)    18732 2024-05-14 01:17:16.000000 Mako-1.3.4/doc/_static/searchtools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)     5123 2024-05-14 01:17:16.000000 Mako-1.3.4/doc/_static/sphinx_highlight.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      204 2024-05-05 17:52:31.000000 Mako-1.3.4/doc/_static/sphinx_paramlinks.css
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.505633 Mako-1.3.4/doc/build/
+-rw-r--r--   0 classic   (1000) classic   (1000)     4863 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/Makefile
+-rw-r--r--   0 classic   (1000) classic   (1000)    13676 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/caching.rst
+-rw-------   0 classic   (1000) classic   (1000)    70465 2024-05-14 01:17:17.000000 Mako-1.3.4/doc/build/changelog.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     9571 2024-05-14 01:17:17.000000 Mako-1.3.4/doc/build/conf.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    17708 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/defs.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    11278 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/filtering.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      268 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/index.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    19744 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/inheritance.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    14575 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/namespaces.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      217 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/requirements.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    16137 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/runtime.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    14103 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/syntax.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     5391 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/unicode.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.505633 Mako-1.3.4/doc/build/unreleased/
+-rw-r--r--   0 classic   (1000) classic   (1000)      385 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/unreleased/README.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    17836 2024-05-14 01:17:05.000000 Mako-1.3.4/doc/build/usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    85770 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/caching.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   182420 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/changelog.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    56857 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/defs.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    36801 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/filtering.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    26164 2024-05-14 01:17:19.000000 Mako-1.3.4/doc/genindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    12769 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    61365 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/inheritance.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    86600 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/namespaces.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    69788 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/runtime.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     3812 2024-05-14 01:17:19.000000 Mako-1.3.4/doc/search.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    63758 2024-05-14 01:17:19.000000 Mako-1.3.4/doc/searchindex.js
+-rw-r--r--   0 classic   (1000) classic   (1000)    44381 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/syntax.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    18276 2024-05-14 01:17:18.000000 Mako-1.3.4/doc/unicode.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   137745 2024-05-14 01:17:19.000000 Mako-1.3.4/doc/usage.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.498634 Mako-1.3.4/examples/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.505633 Mako-1.3.4/examples/bench/
+-rw-r--r--   0 classic   (1000) classic   (1000)     6593 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/basic.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.506633 Mako-1.3.4/examples/bench/cheetah/
+-rw-r--r--   0 classic   (1000) classic   (1000)       25 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/cheetah/footer.tmpl
+-rw-r--r--   0 classic   (1000) classic   (1000)       45 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/cheetah/header.tmpl
+-rw-r--r--   0 classic   (1000) classic   (1000)      678 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/cheetah/template.tmpl
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.498634 Mako-1.3.4/examples/bench/django/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.506633 Mako-1.3.4/examples/bench/django/templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)      335 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/django/templates/base.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      410 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/django/templates/template.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.506633 Mako-1.3.4/examples/bench/django/templatetags/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/django/templatetags/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      199 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/django/templatetags/bench.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.506633 Mako-1.3.4/examples/bench/genshi/
+-rw-r--r--   0 classic   (1000) classic   (1000)      310 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/genshi/base.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      667 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/genshi/template.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.506633 Mako-1.3.4/examples/bench/jinja2/
+-rw-r--r--   0 classic   (1000) classic   (1000)       25 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/jinja2/footer.html
+-rw-r--r--   0 classic   (1000) classic   (1000)       48 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/jinja2/header.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      694 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/jinja2/template.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.507633 Mako-1.3.4/examples/bench/jinja2_inheritance/
+-rw-r--r--   0 classic   (1000) classic   (1000)      454 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/jinja2_inheritance/base.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      357 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/jinja2_inheritance/template.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.507633 Mako-1.3.4/examples/bench/kid/
+-rw-r--r--   0 classic   (1000) classic   (1000)      336 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/kid/base.kid
+-rw-r--r--   0 classic   (1000) classic   (1000)      610 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/kid/template.kid
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.507633 Mako-1.3.4/examples/bench/mako/
+-rw-r--r--   0 classic   (1000) classic   (1000)       25 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/mako/footer.html
+-rw-r--r--   0 classic   (1000) classic   (1000)       47 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/mako/header.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      670 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/mako/template.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.507633 Mako-1.3.4/examples/bench/mako_inheritance/
+-rw-r--r--   0 classic   (1000) classic   (1000)      405 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/mako_inheritance/base.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      285 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/mako_inheritance/template.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.507633 Mako-1.3.4/examples/bench/myghty/
+-rw-r--r--   0 classic   (1000) classic   (1000)      431 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/myghty/base.myt
+-rw-r--r--   0 classic   (1000) classic   (1000)      505 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/bench/myghty/template.myt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.507633 Mako-1.3.4/examples/wsgi/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.507633 Mako-1.3.4/examples/wsgi/htdocs/
+-rw-r--r--   0 classic   (1000) classic   (1000)      106 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/wsgi/htdocs/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     2472 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/wsgi/run_wsgi.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.508633 Mako-1.3.4/examples/wsgi/templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)       80 2024-05-14 01:17:05.000000 Mako-1.3.4/examples/wsgi/templates/root.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.509633 Mako-1.3.4/mako/
+-rw-r--r--   0 classic   (1000) classic   (1000)      242 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    20247 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/_ast_util.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6642 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ast.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7680 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/cache.py
+-rwxr-xr-x   0 classic   (1000) classic   (1000)     2813 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/cmd.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    47736 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/codegen.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1820 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/compat.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    12530 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/exceptions.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.510633 Mako-1.3.4/mako/ext/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1885 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/autohandler.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2091 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/babelplugin.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2578 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/beaker_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4659 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/extract.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1935 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/linguaplugin.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      576 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/preprocessors.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4753 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/pygmentplugin.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2141 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/ext/turbogears.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4658 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/filters.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16324 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/lexer.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    12428 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/lookup.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    19005 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/parsetree.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10416 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/pygen.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7478 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/pyparser.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    27804 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/runtime.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    23857 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/template.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.510633 Mako-1.3.4/mako/testing/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/testing/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3566 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/testing/_config.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5161 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/testing/assertions.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      323 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/testing/config.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1553 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/testing/exclusions.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3044 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/testing/fixtures.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1623 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/testing/helpers.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10638 2024-05-14 01:17:05.000000 Mako-1.3.4/mako/util.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      153 2024-05-14 01:17:05.000000 Mako-1.3.4/pyproject.toml
+-rw-r--r--   0 classic   (1000) classic   (1000)     2537 2024-05-14 01:17:19.516633 Mako-1.3.4/setup.cfg
+-rw-r--r--   0 classic   (1000) classic   (1000)       38 2024-05-14 01:17:05.000000 Mako-1.3.4/setup.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.512633 Mako-1.3.4/test/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:05.000000 Mako-1.3.4/test/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.512633 Mako-1.3.4/test/ext/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:05.000000 Mako-1.3.4/test/ext/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3932 2024-05-14 01:17:05.000000 Mako-1.3.4/test/ext/test_babelplugin.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1802 2024-05-14 01:17:05.000000 Mako-1.3.4/test/ext/test_linguaplugin.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.513633 Mako-1.3.4/test/foo/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:05.000000 Mako-1.3.4/test/foo/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      145 2024-05-14 01:17:05.000000 Mako-1.3.4/test/foo/mod_no_encoding.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      181 2024-05-14 01:17:05.000000 Mako-1.3.4/test/foo/test_ns.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       30 2024-05-14 01:17:05.000000 Mako-1.3.4/test/module_to_import.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      151 2024-05-14 01:17:05.000000 Mako-1.3.4/test/sample_module_namespace.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.514633 Mako-1.3.4/test/templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)      192 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/badbom.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      167 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/bom.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      192 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/bommagic.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      157 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/chs_unicode_py3k.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      290 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/chs_utf8.html
+-rw-r--r--   0 classic   (1000) classic   (1000)       16 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/cmd_good.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)        4 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/cmd_runtime.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)        3 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/cmd_syntax.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)      252 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/crlf.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.514633 Mako-1.3.4/test/templates/foo/
+-rw-r--r--   0 classic   (1000) classic   (1000)      703 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/foo/modtest.html.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2432 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/gettext.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)       13 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/gettext_cp1251.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)       14 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/gettext_utf8.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)       13 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    58538 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/internationalization.html
+-rw-r--r--   0 classic   (1000) classic   (1000)       14 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/modtest.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.514633 Mako-1.3.4/test/templates/othersubdir/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/othersubdir/foo.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      233 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/read_unicode_py3k.html
+-rw-r--r--   0 classic   (1000) classic   (1000)       29 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/runtimeerr_py3k.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.515633 Mako-1.3.4/test/templates/subdir/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.515633 Mako-1.3.4/test/templates/subdir/foo/
+-rw-r--r--   0 classic   (1000) classic   (1000)      724 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/subdir/foo/modtest.html.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       23 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/subdir/incl.html
+-rw-r--r--   0 classic   (1000) classic   (1000)       56 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/subdir/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)       14 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/subdir/modtest.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      189 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/unicode.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      289 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/unicode_arguments_py3k.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      153 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/unicode_code_py3k.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      195 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/unicode_expr_py3k.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      212 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/unicode_runtime_error.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      200 2024-05-14 01:17:05.000000 Mako-1.3.4/test/templates/unicode_syntax_error.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    11558 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_ast.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16038 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_block.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    18518 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    14039 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_call.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3392 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_cmd.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3282 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_decorators.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    17699 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_def.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    11474 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_exceptions.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    11088 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_filters.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10782 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_inheritance.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    44027 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_lexer.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4836 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_lookup.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10401 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_loop.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      829 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_lru.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    24878 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_namespace.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5688 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_pygen.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      503 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_runtime.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    50946 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_template.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1561 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_tgplugin.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1936 2024-05-14 01:17:05.000000 Mako-1.3.4/test/test_util.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-14 01:17:19.515633 Mako-1.3.4/test/testing/
+-rw-r--r--   0 classic   (1000) classic   (1000)      363 2024-05-14 01:17:05.000000 Mako-1.3.4/test/testing/dummy.cfg
+-rw-r--r--   0 classic   (1000) classic   (1000)     4622 2024-05-14 01:17:05.000000 Mako-1.3.4/test/testing/test_config.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      661 2024-05-14 01:17:05.000000 Mako-1.3.4/tox.ini
```

### Comparing `Mako-1.3.3/.github/workflows/run-on-pr.yaml` & `Mako-1.3.4/.github/workflows/run-on-pr.yaml`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/.github/workflows/run-test.yaml` & `Mako-1.3.4/.github/workflows/run-test.yaml`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/LICENSE` & `Mako-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/Mako.egg-info/PKG-INFO` & `Mako-1.3.4/Mako.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mako
-Version: 1.3.3
+Version: 1.3.4
 Summary: A super-fast templating language that borrows the best ideas from the existing templating languages.
 Home-page: https://www.makotemplates.org/
 Author: Mike Bayer
 Author-email: mike@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://docs.makotemplates.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/mako
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Mako Version: 1.3.3 Summary: A super-fast
+Metadata-Version: 2.1 Name: Mako Version: 1.3.4 Summary: A super-fast
 templating language that borrows the best ideas from the existing templating
 languages. Home-page: https://www.makotemplates.org/ Author: Mike Bayer Author-
 email: mike@zzzcomputing.com License: MIT Project-URL: Documentation, https://
 docs.makotemplates.org Project-URL: Issue Tracker, https://github.com/
 sqlalchemy/mako Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Environment ::
 Web Environment Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `Mako-1.3.3/Mako.egg-info/SOURCES.txt` & `Mako-1.3.4/Mako.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/Mako.egg-info/entry_points.txt` & `Mako-1.3.4/Mako.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/PKG-INFO` & `Mako-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mako
-Version: 1.3.3
+Version: 1.3.4
 Summary: A super-fast templating language that borrows the best ideas from the existing templating languages.
 Home-page: https://www.makotemplates.org/
 Author: Mike Bayer
 Author-email: mike@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://docs.makotemplates.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/mako
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Mako Version: 1.3.3 Summary: A super-fast
+Metadata-Version: 2.1 Name: Mako Version: 1.3.4 Summary: A super-fast
 templating language that borrows the best ideas from the existing templating
 languages. Home-page: https://www.makotemplates.org/ Author: Mike Bayer Author-
 email: mike@zzzcomputing.com License: MIT Project-URL: Documentation, https://
 docs.makotemplates.org Project-URL: Issue Tracker, https://github.com/
 sqlalchemy/mako Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Environment ::
 Web Environment Classifier: Intended Audience :: Developers Classifier:
```

### Comparing `Mako-1.3.3/README.rst` & `Mako-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/_sphinx_javascript_frameworks_compat.js` & `Mako-1.3.4/doc/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/basic.css` & `Mako-1.3.4/doc/_static/basic.css`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/docs.css` & `Mako-1.3.4/doc/_static/docs.css`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/doctools.js` & `Mako-1.3.4/doc/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/jquery.js` & `Mako-1.3.4/doc/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/language_data.js` & `Mako-1.3.4/doc/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/pygments.css` & `Mako-1.3.4/doc/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/searchtools.js` & `Mako-1.3.4/doc/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/_static/sphinx_highlight.js` & `Mako-1.3.4/doc/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/Makefile` & `Mako-1.3.4/doc/build/Makefile`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/caching.rst` & `Mako-1.3.4/doc/build/caching.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/changelog.rst` & `Mako-1.3.4/doc/build/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,35 @@
 Changelog
 =========
 
 1.3
 ===
 
 .. changelog::
+    :version: 1.3.4
+    :released: Mon May 13 2024
+
+    .. change::
+        :tags: bug, parser
+        :tickets: 398
+
+        Fixed regression caused by the fix for :ticket:`320` where new logic added
+        to interpret list and dictionary comprehensions would fail for expression
+        oriented keys.  As the parsing in question was not necessary for these
+        keys, it's been removed.  Pull request courtesy Sébastien Granjoux.
+
+    .. change::
+        :tags: bug, lexer
+        :tickets: 400
+
+        Fixed issue where a parsed expression which contained sub-brackets, such as
+        dictionary literals, would fail to be interpreted correctly even though the
+        initial parsing is correct. Pull request courtesy Jose Galvez.
+
+.. changelog::
     :version: 1.3.3
     :released: Wed Apr 10 2024
 
     .. change::
         :tags: bug, codegen
         :tickets: 146
```

### Comparing `Mako-1.3.3/doc/build/conf.py` & `Mako-1.3.4/doc/build/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = mako.__version__
 # The full version, including alpha/beta/rc tags.
-release = "1.3.3"
-release_date = "Wed Apr 10 2024"
+release = "1.3.4"
+release_date = "Mon May 13 2024"
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
```

### Comparing `Mako-1.3.3/doc/build/defs.rst` & `Mako-1.3.4/doc/build/defs.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/filtering.rst` & `Mako-1.3.4/doc/build/filtering.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/inheritance.rst` & `Mako-1.3.4/doc/build/inheritance.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/namespaces.rst` & `Mako-1.3.4/doc/build/namespaces.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/runtime.rst` & `Mako-1.3.4/doc/build/runtime.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/syntax.rst` & `Mako-1.3.4/doc/build/syntax.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/unicode.rst` & `Mako-1.3.4/doc/build/unicode.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/build/usage.rst` & `Mako-1.3.4/doc/build/usage.rst`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/doc/caching.html` & `Mako-1.3.4/doc/caching.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Caching
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="Changelog" href="changelog.html" />
         <link rel="prev" title="The Unicode Chapter" href="unicode.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Caching
             
 
         <h2>
             
                 Caching
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _T_h_e_ _U_n_i_c_o_d_e_ _C_h_a_p_t_e_r
     * Next: _C_h_a_n_g_e_l_o_g
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Caching
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Caching
 ********** CCaacchhiinngg **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _C_a_c_h_i_n_g
           o _C_a_c_h_e_ _A_r_g_u_m_e_n_t_s
                 # _B_a_c_k_e_n_d_-_S_p_e_c_i_f_i_c_ _C_a_c_h_e_ _A_r_g_u_m_e_n_t_s
                 # _U_s_i_n_g_ _t_h_e_ _B_e_a_k_e_r_ _C_a_c_h_e_ _B_a_c_k_e_n_d
                 # _U_s_i_n_g_ _t_h_e_ _d_o_g_p_i_l_e_._c_a_c_h_e_ _B_a_c_k_e_n_d
```

### Comparing `Mako-1.3.3/doc/changelog.html` & `Mako-1.3.4/doc/changelog.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Changelog
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="prev" title="Caching" href="caching.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
         
@@ -54,27 +54,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -87,15 +87,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Changelog
             
 
         <h2>
             
                 Changelog
@@ -113,14 +113,18 @@
         
     </div>
 
     <h3><a href="index.html">Table of Contents</a></h3>
     <div id="sidebar-toc"><ul>
 <li><a class="reference internal" href="#">Changelog</a><ul>
 <li><a class="reference internal" href="#id1">1.3</a><ul>
+<li><a class="reference internal" href="#change-1.3.4">1.3.4</a><ul>
+<li><a class="reference internal" href="#change-1.3.4-bug">bug</a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#change-1.3.3">1.3.3</a><ul>
 <li><a class="reference internal" href="#change-1.3.3-bug">bug</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#change-1.3.2">1.3.2</a><ul>
 <li><a class="reference internal" href="#change-1.3.2-bug">bug</a></li>
 </ul>
@@ -371,14 +375,35 @@
 
     <div id="docs-body" class="withsidebar" >
         
 <section id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Link to this heading">¶</a></h1>
 <section id="id1">
 <h2>1.3<a class="headerlink" href="#id1" title="Link to this heading">¶</a></h2>
+<section id="change-1.3.4">
+<h3 class="release-version">1.3.4<a class="headerlink" href="#change-1.3.4" title="Link to this heading">¶</a></h3>
+Released: Mon May 13 2024<section id="change-1.3.4-bug">
+<h4>bug<a class="headerlink" href="#change-1.3.4-bug" title="Link to this heading">¶</a></h4>
+<ul class="simple">
+<li><p class="caption" id="change-1.3.4-0"><span class="target" id="change-524b743a8f403d85e8d3c78b2ac8fcba"><strong>[bug] [parser]</strong> <a class="changelog-reference headerlink reference internal" href="#change-524b743a8f403d85e8d3c78b2ac8fcba">¶</a></span><p>Fixed regression caused by the fix for <a class="reference external" href="https://github.com/sqlalchemy/mako/issues/320">#320</a> where new logic added
+to interpret list and dictionary comprehensions would fail for expression
+oriented keys.  As the parsing in question was not necessary for these
+keys, it’s been removed.  Pull request courtesy Sébastien Granjoux.</p>
+<p>References: <a class="reference external" href="https://github.com/sqlalchemy/mako/issues/398">#398</a></p>
+</p>
+</li>
+<li><p class="caption" id="change-1.3.4-1"><span class="target" id="change-9173d5d68ed09e464c8ad2b8a6c6ac71"><strong>[bug] [lexer]</strong> <a class="changelog-reference headerlink reference internal" href="#change-9173d5d68ed09e464c8ad2b8a6c6ac71">¶</a></span><p>Fixed issue where a parsed expression which contained sub-brackets, such as
+dictionary literals, would fail to be interpreted correctly even though the
+initial parsing is correct. Pull request courtesy Jose Galvez.</p>
+<p>References: <a class="reference external" href="https://github.com/sqlalchemy/mako/issues/400">#400</a></p>
+</p>
+</li>
+</ul>
+</section>
+</section>
 <section id="change-1.3.3">
 <h3 class="release-version">1.3.3<a class="headerlink" href="#change-1.3.3" title="Link to this heading">¶</a></h3>
 Released: Wed Apr 10 2024<section id="change-1.3.3-bug">
 <h4>bug<a class="headerlink" href="#change-1.3.3-bug" title="Link to this heading">¶</a></h4>
 <ul class="simple">
 <li><p class="caption" id="change-1.3.3-0"><span class="target" id="change-cb106213ca05ea1e91076d005c7212a7"><strong>[bug] [codegen]</strong> <a class="changelog-reference headerlink reference internal" href="#change-cb106213ca05ea1e91076d005c7212a7">¶</a></span><p>Fixed unexpected error when use control lines which the
 first control block with no bodies other than comments,
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _C_a_c_h_i_n_g
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Changelog
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Changelog
 ********** CChhaannggeelloogg **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _C_h_a_n_g_e_l_o_g
           o _1_._3
+                # _1_._3_._4
+                      # _b_u_g
                 # _1_._3_._3
                       # _b_u_g
                 # _1_._3_._2
                       # _b_u_g
                 # _1_._3_._1
                       # _b_u_g
                 # _1_._3_._0
@@ -144,14 +146,28 @@
                 # _0_._1_._1
 ****** PPrreevviioouuss TTooppiicc ******
 _C_a_c_h_i_n_g
 ****** QQuuiicckk SSeeaarrcchh ******
 [q                 ][Search]
 ************ CChhaannggeelloogg_?¶ ************
 ********** 11..33_?¶ **********
+******** 11..33..44_?¶ ********
+Released: Mon May 13 2024
+****** bbuugg_?¶ ******
+    * [[bbuugg]] [[ppaarrsseerr]] _¶
+      Fixed regression caused by the fix for _#_3_2_0 where new logic added to
+      interpret list and dictionary comprehensions would fail for expression
+      oriented keys. As the parsing in question was not necessary for these
+      keys, it’s been removed. Pull request courtesy Sébastien Granjoux.
+      References: _#_3_9_8
+[[bbuugg]] [[lleexxeerr]] _¶
+Fixed issue where a parsed expression which contained sub-brackets, such as
+dictionary literals, would fail to be interpreted correctly even though the
+initial parsing is correct. Pull request courtesy Jose Galvez.
+References: _#_4_0_0
 ******** 11..33..33_?¶ ********
 Released: Wed Apr 10 2024
 ****** bbuugg_?¶ ******
     * [[bbuugg]] [[ccooddeeggeenn]] _¶
       Fixed unexpected error when use control lines which the first control
       block with no bodies other than comments, aspassis now added to the first
       empty block. Pull request courtesy Hai Zhu.
```

### Comparing `Mako-1.3.3/doc/defs.html` & `Mako-1.3.4/doc/defs.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Defs and Blocks
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="The Mako Runtime Environment" href="runtime.html" />
         <link rel="prev" title="Syntax" href="syntax.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Defs and Blocks
             
 
         <h2>
             
                 Defs and Blocks
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _S_y_n_t_a_x
     * Next: _T_h_e_ _M_a_k_o_ _R_u_n_t_i_m_e_ _E_n_v_i_r_o_n_m_e_n_t
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Defs and Blocks
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Defs and Blocks
 ********** DDeeffss aanndd BBlloocckkss **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _D_e_f_s_ _a_n_d_ _B_l_o_c_k_s
           o _U_s_i_n_g_ _D_e_f_s
                 # _C_a_l_l_i_n_g_ _D_e_f_s_ _f_r_o_m_ _O_t_h_e_r_ _F_i_l_e_s
                 # _C_a_l_l_i_n_g_ _D_e_f_s_ _P_r_o_g_r_a_m_m_a_t_i_c_a_l_l_y
                 # _D_e_f_s_ _w_i_t_h_i_n_ _D_e_f_s
```

### Comparing `Mako-1.3.3/doc/filtering.html` & `Mako-1.3.4/doc/filtering.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Filtering and Buffering
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="The Unicode Chapter" href="unicode.html" />
         <link rel="prev" title="Inheritance" href="inheritance.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Filtering and Buffering
             
 
         <h2>
             
                 Filtering and Buffering
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _I_n_h_e_r_i_t_a_n_c_e
     * Next: _T_h_e_ _U_n_i_c_o_d_e_ _C_h_a_p_t_e_r
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Filtering and Buffering
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Filtering and Buffering
 ********** FFiilltteerriinngg aanndd BBuuffffeerriinngg **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _F_i_l_t_e_r_i_n_g_ _a_n_d_ _B_u_f_f_e_r_i_n_g
           o _E_x_p_r_e_s_s_i_o_n_ _F_i_l_t_e_r_i_n_g
                 # _T_h_e_ _d_e_f_a_u_l_t___f_i_l_t_e_r_s_ _A_r_g_u_m_e_n_t
                 # _T_u_r_n_i_n_g_ _o_f_f_ _F_i_l_t_e_r_i_n_g_ _w_i_t_h_ _t_h_e_ _n_ _F_i_l_t_e_r
           o _F_i_l_t_e_r_i_n_g_ _D_e_f_s_ _a_n_d_ _B_l_o_c_k_s
```

### Comparing `Mako-1.3.3/doc/genindex.html` & `Mako-1.3.4/doc/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <html xmlns="http://www.w3.org/1999/xhtml">
     <head>
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
         
         <title>
             
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -27,15 +27,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
         
 
@@ -49,27 +49,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -79,15 +79,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="#">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
     Index
 
 
         <h2>
             
     Index
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Index
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Index
 ********** IInnddeexx **********
 ************ IInnddeexx ************
 _SS_yy_mm_bb_oo_ll_ss | _AA | _BB | _CC | _DD | _EE | _FF | _GG | _HH | _II | _KK | _LL | _MM | _NN | _OO | _PP | _RR | _SS | _TT
 | _UU | _VV | _WW
 ===============================================================================
 ********** SSyymmbboollss **********
   _*_*_k_w_ _(_m_a_k_o_._c_a_c_h_e_._C_a_c_h_e_._g_e_t_ _p_a_r_a_m_e_t_e_r_)
```

### Comparing `Mako-1.3.3/doc/index.html` & `Mako-1.3.4/doc/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <head>
         <meta name="viewport" content="width=device-width, initial-scale=1">
         <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -28,15 +28,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="#" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="#" />
         <link rel="next" title="Usage" href="usage.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
         
@@ -51,27 +51,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -84,15 +84,15 @@
             <a href="#">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="#">Mako 1.3.3 Documentation</a>
+        <a href="#">Mako 1.3.4 Documentation</a>
 
         <h2>
             
                 Table of Contents
             
         </h2>
     </div>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Next: _U_s_a_g_e
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n
 ********** TTaabbllee ooff CCoonntteennttss **********
 ************ TTaabbllee ooff CCoonntteennttss_?¶ ************
     * _U_s_a_g_e
           o _B_a_s_i_c_ _U_s_a_g_e
           o _U_s_i_n_g_ _F_i_l_e_-_B_a_s_e_d_ _T_e_m_p_l_a_t_e_s
           o _U_s_i_n_g_ _T_e_m_p_l_a_t_e_L_o_o_k_u_p
           o _U_s_i_n_g_ _U_n_i_c_o_d_e_ _a_n_d_ _E_n_c_o_d_i_n_g
```

### Comparing `Mako-1.3.3/doc/inheritance.html` & `Mako-1.3.4/doc/inheritance.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Inheritance
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="Filtering and Buffering" href="filtering.html" />
         <link rel="prev" title="Namespaces" href="namespaces.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Inheritance
             
 
         <h2>
             
                 Inheritance
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _N_a_m_e_s_p_a_c_e_s
     * Next: _F_i_l_t_e_r_i_n_g_ _a_n_d_ _B_u_f_f_e_r_i_n_g
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Inheritance
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Inheritance
 ********** IInnhheerriittaannccee **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _I_n_h_e_r_i_t_a_n_c_e
           o _N_e_s_t_i_n_g_ _B_l_o_c_k_s
           o _R_e_n_d_e_r_i_n_g_ _a_ _N_a_m_e_d_ _B_l_o_c_k_ _M_u_l_t_i_p_l_e_ _T_i_m_e_s
           o _B_u_t_ _w_h_a_t_ _a_b_o_u_t_ _D_e_f_s_?
           o _U_s_i_n_g_ _t_h_e_ _n_e_x_t_ _N_a_m_e_s_p_a_c_e_ _t_o_ _P_r_o_d_u_c_e_ _C_o_n_t_e_n_t_ _W_r_a_p_p_i_n_g
```

### Comparing `Mako-1.3.3/doc/namespaces.html` & `Mako-1.3.4/doc/namespaces.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Namespaces
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="Inheritance" href="inheritance.html" />
         <link rel="prev" title="The Mako Runtime Environment" href="runtime.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Namespaces
             
 
         <h2>
             
                 Namespaces
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _T_h_e_ _M_a_k_o_ _R_u_n_t_i_m_e_ _E_n_v_i_r_o_n_m_e_n_t
     * Next: _I_n_h_e_r_i_t_a_n_c_e
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Namespaces
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Namespaces
 ********** NNaammeessppaacceess **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _N_a_m_e_s_p_a_c_e_s
           o _W_a_y_s_ _t_o_ _C_a_l_l_ _N_a_m_e_s_p_a_c_e_s
           o _N_a_m_e_s_p_a_c_e_s_ _f_r_o_m_ _R_e_g_u_l_a_r_ _P_y_t_h_o_n_ _M_o_d_u_l_e_s
           o _D_e_c_l_a_r_i_n_g_ _D_e_f_s_ _i_n_ _N_a_m_e_s_p_a_c_e_s
           o _T_h_e_ _b_o_d_y_(_)_ _M_e_t_h_o_d
```

### Comparing `Mako-1.3.3/doc/runtime.html` & `Mako-1.3.4/doc/runtime.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 The Mako Runtime Environment
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="Namespaces" href="namespaces.html" />
         <link rel="prev" title="Defs and Blocks" href="defs.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 The Mako Runtime Environment
             
 
         <h2>
             
                 The Mako Runtime Environment
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _D_e_f_s_ _a_n_d_ _B_l_o_c_k_s
     * Next: _N_a_m_e_s_p_a_c_e_s
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » The Mako Runtime Environment
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » The Mako Runtime Environment
 ********** TThhee MMaakkoo RRuunnttiimmee EEnnvviirroonnmmeenntt **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _T_h_e_ _M_a_k_o_ _R_u_n_t_i_m_e_ _E_n_v_i_r_o_n_m_e_n_t
           o _C_o_n_t_e_x_t
                 # _T_h_e_ _B_u_f_f_e_r
                 # _C_o_n_t_e_x_t_ _V_a_r_i_a_b_l_e_s
                 # _C_o_n_t_e_x_t_ _M_e_t_h_o_d_s_ _a_n_d_ _A_c_c_e_s_s_o_r_s
```

### Comparing `Mako-1.3.3/doc/search.html` & `Mako-1.3.4/doc/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
         
         <title>
             
     
     Search
  &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -30,15 +30,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
         
 
@@ -52,27 +52,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="#" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -82,15 +82,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
     Search
 
 
         <h2>
             
     Search
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Search
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Search
 ********** SSeeaarrcchh **********
 © Copyright the Mako authors and contributors. Documentation generated using
 _S_p_h_i_n_x 7.2.6 with Mako templates.
```

### Comparing `Mako-1.3.3/doc/searchindex.js` & `Mako-1.3.4/doc/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -427,64 +427,84 @@
         "popul": 0,
         "befor": [0, 1, 3, 5, 6, 8, 10],
         "context": [0, 1, 2, 3, 4, 5, 6, 9, 10],
         "modulepath": 0,
         "objnam": 0,
         "beaker_cach": 0,
         "signatur": [0, 1, 2, 6, 10],
+        "mon": 1,
+        "2024": 1,
+        "parser": 1,
+        "regress": 1,
+        "caus": [1, 3, 6, 7, 10],
+        "320": 1,
+        "logic": [1, 3],
+        "ad": [1, 3, 5, 8],
+        "interpret": [1, 2, 10],
+        "comprehens": 1,
+        "fail": 1,
+        "express": [1, 2, 4, 5, 6, 7, 10],
+        "orient": [1, 2, 5],
+        "pars": [1, 8, 9, 10],
+        "question": 1,
+        "necessari": 1,
+        "remov": [1, 6],
+        "pull": [1, 2, 6, 7, 10],
+        "courtesi": 1,
+        "s\u00e9bastien": 1,
+        "granjoux": 1,
+        "refer": [1, 2, 3, 4, 5, 8],
+        "398": 1,
+        "lexer": [1, 8, 10],
+        "issu": [1, 2, 10],
+        "sub": [1, 2, 8],
+        "bracket": 1,
+        "liter": [1, 3, 6, 10],
+        "correctli": [1, 7],
+        "even": [1, 5, 7, 8],
+        "initi": [1, 2],
+        "correct": [1, 6],
+        "jose": 1,
+        "galvez": 1,
+        "400": 1,
         "wed": 1,
         "apr": 1,
-        "2024": 1,
         "codegen": 1,
         "unexpect": 1,
         "error": [1, 2, 7, 10],
         "us": [1, 3, 4, 8, 9],
         "control": [1, 2, 3, 4, 5, 7, 10],
         "line": [1, 5, 8, 10],
         "comment": [1, 4, 9, 10],
         "now": [1, 3, 5, 7, 8, 9],
-        "ad": [1, 3, 5, 8],
         "empti": [1, 3, 8],
-        "pull": [1, 2, 6, 7, 10],
-        "courtesi": 1,
         "hai": 1,
         "zhu": 1,
-        "refer": [1, 2, 3, 4, 5, 8],
         "146": 1,
-        "parser": 1,
         "syntax": [1, 2, 3, 4, 9, 10],
         "strict_undefin": [1, 7, 10],
         "mode": 1,
-        "comprehens": 1,
         "python": [1, 2, 3, 4, 5, 7, 9, 10],
         "code": [1, 2, 3, 6, 7, 8, 9, 10],
         "variabl": [1, 2, 5, 6, 8, 10],
         "won": [1, 5, 7, 10],
         "checklist": 1,
-        "320": 1,
         "tue": 1,
         "jan": 1,
         "30": 1,
-        "lexer": [1, 8, 10],
-        "pars": [1, 8, 9, 10],
-        "issu": [1, 2, 10],
         "percent": [1, 8],
         "sign": [1, 8],
         "escap": [1, 2, 3, 4],
-        "correctli": [1, 7],
         "were": [1, 5, 6, 7, 9],
         "charact": [1, 8, 10],
         "revis": [1, 10],
         "similar": [1, 2, 3, 5, 6, 7, 8, 10],
-        "caus": [1, 3, 6, 7, 10],
-        "regress": 1,
         "result": [1, 2, 3, 5, 7, 8, 10],
         "yank": 1,
         "323": 1,
-        "mon": 1,
         "22": 1,
         "pypi": 1,
         "revert": 1,
         "modifi": [1, 2, 5, 9, 10],
         "nov": 1,
         "2023": 1,
         "bump": 1,
@@ -499,17 +519,15 @@
         "tupl": [1, 10],
         "loop": [1, 2, 4, 10],
         "rais": [1, 2, 7, 10],
         "couldn": 1,
         "appli": [1, 2, 3, 6, 7, 8, 9, 10],
         "regex": 1,
         "match": 1,
-        "express": [1, 2, 4, 5, 6, 7, 10],
         "parenthes": 1,
-        "sub": [1, 2, 8],
         "matt": 1,
         "trescott": 1,
         "368": 1,
         "thu": [1, 10],
         "sep": 1,
         "categori": [1, 6],
         "366": 1,
@@ -517,15 +535,14 @@
         "end": [1, 3, 5, 8],
         "didn": 1,
         "organ": [1, 5, 6],
         "surround": [1, 8],
         "whitespac": [1, 2, 3, 8],
         "lead": [1, 3, 6, 7],
         "high": 1,
-        "interpret": [1, 2, 10],
         "hang": 1,
         "close": [1, 2, 6, 8, 10],
         "incorrectli": 1,
         "had": 1,
         "larg": [1, 5],
         "amount": 1,
         "untermin": 1,
@@ -568,25 +585,23 @@
         "prior": [1, 3, 7],
         "cach": [1, 2, 3, 4, 6, 7, 8, 10],
         "takuto": 1,
         "ikuta": 1,
         "361": 1,
         "mar": 1,
         "py3k": 1,
-        "correct": [1, 6],
         "univers": 1,
         "wheel": 1,
         "cfg": [1, 10],
         "build": [1, 2, 5, 6],
         "doe": [1, 2, 5, 6, 7, 8],
         "target": [1, 2, 3],
         "351": 1,
         "bytestring_passthrough": 1,
         "argument": [1, 4, 6, 7, 8, 9, 10],
-        "remov": [1, 6],
         "cstringio": 1,
         "fastencodingbuff": 1,
         "exclus": [1, 10],
         "disable_unicod": 1,
         "longer": 1,
         "refactor": 1,
         "util": [1, 10],
@@ -748,15 +763,14 @@
         "293": 1,
         "further": [1, 8],
         "previou": [1, 2, 5, 6, 7, 10],
         "287": 1,
         "reli": 1,
         "monkeypatch": 1,
         "reason": [1, 7],
-        "fail": 1,
         "hasn": 1,
         "constant": [1, 7],
         "lacsap": 1,
         "271": 1,
         "element": [1, 2, 5, 7, 8, 10],
         "unnecessari": 1,
         "hugo": 1,
@@ -791,15 +805,14 @@
         "sequenc": 1,
         "bitwis": 1,
         "oper": [1, 2, 3, 6, 7, 8, 9, 10],
         "pipe": [1, 3],
         "symbol": [1, 8],
         "distinct": [1, 10],
         "enclos": [1, 2, 7],
-        "bracket": 1,
         "daniel": 1,
         "19": 1,
         "oct": 1,
         "2015": 1,
         "translat": [1, 10],
         "non": [1, 7, 8, 9, 10],
         "roman": 1,
@@ -867,15 +880,14 @@
         "haltner": 1,
         "html_escap": 1,
         "unicod": [1, 3, 4],
         "u": [1, 2, 3, 6, 8],
         "properli": 1,
         "georg": 1,
         "xie": 1,
-        "logic": [1, 3],
         "try": [1, 3, 7, 8, 10],
         "227": 1,
         "rework": 1,
         "pathnam": 1,
         "outsid": [1, 2, 5, 6, 7],
         "some_templ": [1, 10],
         "root": [1, 10],
@@ -916,15 +928,14 @@
         "clarifi": 1,
         "deliv": [1, 3, 6],
         "219": 1,
         "some_tag": 1,
         "attr": [1, 5],
         "_": [1, 10],
         "foo": [1, 2, 3, 6, 7, 8, 9, 10],
-        "liter": [1, 3, 6, 10],
         "incompat": 1,
         "v": 1,
         "187": 1,
         "somemodul": 1,
         "skip": [1, 10],
         "over": [1, 3, 6, 7],
         "explcitli": 1,
@@ -978,15 +989,14 @@
         "becam": 1,
         "192": 1,
         "191": 1,
         "info": [1, 10],
         "index": [1, 4, 5, 6, 7, 8, 10],
         "last": [1, 7, 10],
         "odd": [1, 7],
-        "even": [1, 5, 7, 8],
         "migrat": [1, 10],
         "enable_loop": [1, 7, 10],
         "thank": 1,
         "125": 1,
         "real": [1, 8, 10],
         "reserv": 1,
         "cannot": [1, 2, 10],
@@ -1315,15 +1325,14 @@
         "moduletempl": 1,
         "alon": 1,
         "pypars": 1,
         "90": 1,
         "87": 1,
         "critic": 1,
         "refresh": 1,
-        "initi": [1, 2],
         "complet": [1, 5, 6, 10],
         "16": 1,
         "peopl": 1,
         "contribut": 1,
         "passthru": 1,
         "awar": [1, 7],
         "receiv": [1, 2, 3, 6, 8],
@@ -1472,15 +1481,14 @@
         "svn": 1,
         "cant": 1,
         "prune": 1,
         "convers": [1, 9],
         "scalar": [1, 6],
         "demarc": 2,
         "wherea": [2, 7, 8],
-        "orient": [2, 5],
         "hello": [2, 6, 8, 9, 10],
         "world": [2, 6, 7, 8, 9, 10],
         "anywher": [2, 6, 8],
         "contextu": 2,
         "exactli": [2, 5],
         "usernam": [2, 8],
         "accountdata": 2,
@@ -2308,18 +2316,18 @@
         "guidelin": 0,
         "write": 0,
         "api": [0, 6, 7, 10],
         "refer": [0, 6, 7, 10],
         "changelog": 1,
         "1": 1,
         "3": 1,
+        "4": 1,
         "bug": 1,
         "2": 1,
         "0": 1,
-        "4": 1,
         "misc": 1,
         "chang": 1,
         "6": 1,
         "5": 1,
         "featur": 1,
         "14": 1,
         "13": 1,
@@ -2485,18 +2493,19 @@
         ],
         "Changelog": [
             [1, "changelog"]
         ],
         "1.3": [
             [1, "id1"]
         ],
-        "1.3.3": [
-            [1, "change-1.3.3"]
+        "1.3.4": [
+            [1, "change-1.3.4"]
         ],
         "bug": [
+            [1, "change-1.3.4-bug"],
             [1, "change-1.3.3-bug"],
             [1, "change-1.3.2-bug"],
             [1, "change-1.3.1-bug"],
             [1, "change-1.2.4-bug"],
             [1, "change-1.2.3-bug"],
             [1, "change-1.2.2-bug"],
             [1, "change-1.2.1-bug"],
@@ -2528,14 +2537,17 @@
             [1, "change-0.7.2-bug"],
             [1, "change-0.7.1-bug"],
             [1, "change-0.7.0-bug"],
             [1, "change-0.6.2-bug"],
             [1, "change-0.6.1-bug"],
             [1, "change-0.6.0-bug"]
         ],
+        "1.3.3": [
+            [1, "change-1.3.3"]
+        ],
         "1.3.2": [
             [1, "change-1.3.2"]
         ],
         "1.3.1": [
             [1, "change-1.3.1"]
         ],
         "1.3.0": [
```

### Comparing `Mako-1.3.3/doc/syntax.html` & `Mako-1.3.4/doc/syntax.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Syntax
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="Defs and Blocks" href="defs.html" />
         <link rel="prev" title="Usage" href="usage.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Syntax
             
 
         <h2>
             
                 Syntax
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _U_s_a_g_e
     * Next: _D_e_f_s_ _a_n_d_ _B_l_o_c_k_s
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Syntax
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Syntax
 ********** SSyynnttaaxx **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _S_y_n_t_a_x
           o _E_x_p_r_e_s_s_i_o_n_ _S_u_b_s_t_i_t_u_t_i_o_n
           o _E_x_p_r_e_s_s_i_o_n_ _E_s_c_a_p_i_n_g
           o _C_o_n_t_r_o_l_ _S_t_r_u_c_t_u_r_e_s
                 # _T_h_e_ _L_o_o_p_ _C_o_n_t_e_x_t
```

### Comparing `Mako-1.3.3/doc/unicode.html` & `Mako-1.3.4/doc/unicode.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 The Unicode Chapter
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="Caching" href="caching.html" />
         <link rel="prev" title="Filtering and Buffering" href="filtering.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 The Unicode Chapter
             
 
         <h2>
             
                 The Unicode Chapter
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _F_i_l_t_e_r_i_n_g_ _a_n_d_ _B_u_f_f_e_r_i_n_g
     * Next: _C_a_c_h_i_n_g
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » The Unicode Chapter
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » The Unicode Chapter
 ********** TThhee UUnniiccooddee CChhaapptteerr **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _T_h_e_ _U_n_i_c_o_d_e_ _C_h_a_p_t_e_r
           o _S_p_e_c_i_f_y_i_n_g_ _t_h_e_ _E_n_c_o_d_i_n_g_ _o_f_ _a_ _T_e_m_p_l_a_t_e_ _F_i_l_e
           o _H_a_n_d_l_i_n_g_ _E_x_p_r_e_s_s_i_o_n_s
           o _D_e_f_i_n_i_n_g_ _O_u_t_p_u_t_ _E_n_c_o_d_i_n_g
 ****** PPrreevviioouuss TTooppiicc ******
```

### Comparing `Mako-1.3.3/doc/usage.html` & `Mako-1.3.4/doc/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         <meta name="viewport" content="width=device-width, initial-scale=1" />
 
         <title>
             
     
                 Usage
              &mdash;
-    Mako 1.3.3 Documentation
+    Mako 1.3.4 Documentation
 
         </title>
 
         
             <!-- begin iterate through site-imported + sphinx environment css_files -->
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
                 <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
@@ -31,15 +31,15 @@
         
     
 
     <!-- begin layout.mako headers -->
 
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
-    <link rel="top" title="Mako 1.3.3 Documentation" href="index.html" />
+    <link rel="top" title="Mako 1.3.4 Documentation" href="index.html" />
         <link rel="next" title="Syntax" href="syntax.html" />
         <link rel="prev" title="Table of Contents" href="index.html" />
     <!-- end layout.mako headers -->
 
 
     </head>
     <body>
@@ -55,27 +55,27 @@
 
 
 <div id="docs-container">
 
 
 
 <div id="docs-header">
-    <h1>Mako 1.3.3 Documentation</h1>
+    <h1>Mako 1.3.4 Documentation</h1>
 
     <div id="docs-search">
     Search:
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" size="18" /> <input type="submit" value="Search" />
       <input type="hidden" name="check_keywords" value="yes" />
       <input type="hidden" name="area" value="default" />
     </form>
     </div>
 
     <div id="docs-version-header">
-        Release: <span class="version-num">1.3.3</span>
+        Release: <span class="version-num">1.3.4</span>
 
     </div>
 
 </div>
 
 <div id="docs-top-navigation">
     <div id="docs-top-page-control" class="docs-navigation-links">
@@ -91,15 +91,15 @@
             <a href="index.html">Table of Contents</a> |
             <a href="genindex.html">Index</a>
         </li>
         </ul>
     </div>
 
     <div id="docs-navigation-banner">
-        <a href="index.html">Mako 1.3.3 Documentation</a>
+        <a href="index.html">Mako 1.3.4 Documentation</a>
         » 
                 Usage
             
 
         <h2>
             
                 Usage
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ MMaakkoo 11..33..33 DDooccuummeennttaattiioonn ************
+************ MMaakkoo 11..33..44 DDooccuummeennttaattiioonn ************
 Search:
 [q                 ][Search]
-Release: 1.3.3
+Release: 1.3.4
     * Prev: _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s
     * Next: _S_y_n_t_a_x
     * _T_a_b_l_e_ _o_f_ _C_o_n_t_e_n_t_s | _I_n_d_e_x
-_M_a_k_o_ _1_._3_._3_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Usage
+_M_a_k_o_ _1_._3_._4_ _D_o_c_u_m_e_n_t_a_t_i_o_n » Usage
 ********** UUssaaggee **********
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _U_s_a_g_e
           o _B_a_s_i_c_ _U_s_a_g_e
           o _U_s_i_n_g_ _F_i_l_e_-_B_a_s_e_d_ _T_e_m_p_l_a_t_e_s
           o _U_s_i_n_g_ _T_e_m_p_l_a_t_e_L_o_o_k_u_p
                 # _S_e_t_t_i_n_g_ _t_h_e_ _C_o_l_l_e_c_t_i_o_n_ _S_i_z_e
```

### Comparing `Mako-1.3.3/examples/bench/basic.py` & `Mako-1.3.4/examples/bench/basic.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/examples/bench/cheetah/template.tmpl` & `Mako-1.3.4/examples/bench/cheetah/template.tmpl`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/examples/bench/genshi/template.html` & `Mako-1.3.4/examples/bench/genshi/template.html`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/examples/bench/jinja2/template.html` & `Mako-1.3.4/examples/bench/jinja2/template.html`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/examples/bench/kid/template.kid` & `Mako-1.3.4/examples/bench/kid/template.kid`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/examples/bench/mako/template.html` & `Mako-1.3.4/examples/bench/mako/template.html`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/examples/wsgi/run_wsgi.py` & `Mako-1.3.4/examples/wsgi/run_wsgi.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/_ast_util.py` & `Mako-1.3.4/mako/_ast_util.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ast.py` & `Mako-1.3.4/mako/ast.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/cache.py` & `Mako-1.3.4/mako/cache.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/cmd.py` & `Mako-1.3.4/mako/cmd.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/codegen.py` & `Mako-1.3.4/mako/codegen.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/compat.py` & `Mako-1.3.4/mako/compat.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/exceptions.py` & `Mako-1.3.4/mako/exceptions.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/autohandler.py` & `Mako-1.3.4/mako/ext/autohandler.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/babelplugin.py` & `Mako-1.3.4/mako/ext/babelplugin.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/beaker_cache.py` & `Mako-1.3.4/mako/ext/beaker_cache.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/extract.py` & `Mako-1.3.4/mako/ext/extract.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/linguaplugin.py` & `Mako-1.3.4/mako/ext/linguaplugin.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/preprocessors.py` & `Mako-1.3.4/mako/ext/preprocessors.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/pygmentplugin.py` & `Mako-1.3.4/mako/ext/pygmentplugin.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/ext/turbogears.py` & `Mako-1.3.4/mako/ext/turbogears.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/filters.py` & `Mako-1.3.4/mako/filters.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/lexer.py` & `Mako-1.3.4/mako/lexer.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/lookup.py` & `Mako-1.3.4/mako/lookup.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/parsetree.py` & `Mako-1.3.4/mako/parsetree.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,18 +318,18 @@
 
     def _parse_attributes(self, expressions, nonexpressions):
         undeclared_identifiers = set()
         self.parsed_attributes = {}
         for key in self.attributes:
             if key in expressions:
                 expr = []
-                for x in re.compile(r"(\${.+?})", re.S).split(
+                for x in re.compile(r"(\${.+})", re.S).split(
                     self.attributes[key]
                 ):
-                    m = re.compile(r"^\${(.+?)}$", re.S).match(x)
+                    m = re.compile(r"^\${(.+)}$", re.S).match(x)
                     if m:
                         code = ast.PythonCode(
                             m.group(1).rstrip(), **self.exception_kwargs
                         )
                         # we aren't discarding "declared_identifiers" here,
                         # which we do so that list comprehension-declared
                         # variables aren't counted.   As yet can't find a
```

### Comparing `Mako-1.3.3/mako/pygen.py` & `Mako-1.3.4/mako/pygen.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/pyparser.py` & `Mako-1.3.4/mako/pyparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,27 +88,23 @@
 
     def visit_FunctionDef(self, node):
         self._add_declared(node.name)
         self._visit_function(node, False)
 
     def visit_ListComp(self, node):
         if self.in_function:
-            if not isinstance(node.elt, _ast.Name):
-                self.visit(node.elt)
             for comp in node.generators:
                 self.visit(comp.iter)
         else:
             self.generic_visit(node)
 
     visit_SetComp = visit_GeneratorExp = visit_ListComp
 
     def visit_DictComp(self, node):
         if self.in_function:
-            if not isinstance(node.key, _ast.Name):
-                self.visit(node.elt)
             for comp in node.generators:
                 self.visit(comp.iter)
         else:
             self.generic_visit(node)
 
     def _expand_tuples(self, args):
         for arg in args:
```

### Comparing `Mako-1.3.3/mako/runtime.py` & `Mako-1.3.4/mako/runtime.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/template.py` & `Mako-1.3.4/mako/template.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/testing/_config.py` & `Mako-1.3.4/mako/testing/_config.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/testing/assertions.py` & `Mako-1.3.4/mako/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/testing/exclusions.py` & `Mako-1.3.4/mako/testing/exclusions.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/testing/fixtures.py` & `Mako-1.3.4/mako/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/testing/helpers.py` & `Mako-1.3.4/mako/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/mako/util.py` & `Mako-1.3.4/mako/util.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/setup.cfg` & `Mako-1.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 sign = 1
 identity = 4BFDF51E
 
 [flake8]
 show-source = true
 enable-extensions = G
 ignore = 
-	A003,
+	A003,A005
 	D,
 	E203,E305,E711,E712,E721,E722,E741,
 	N801,N802,N806,
 	RST304,RST303,RST299,RST399,
 	W503,W504
 exclude = .venv,.git,.tox,dist,docs/*,*egg,build
 import-order-style = google
```

### Comparing `Mako-1.3.3/test/ext/test_babelplugin.py` & `Mako-1.3.4/test/ext/test_babelplugin.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/ext/test_linguaplugin.py` & `Mako-1.3.4/test/ext/test_linguaplugin.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/templates/foo/modtest.html.py` & `Mako-1.3.4/test/templates/foo/modtest.html.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/templates/gettext.mako` & `Mako-1.3.4/test/templates/gettext.mako`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/templates/internationalization.html` & `Mako-1.3.4/test/templates/internationalization.html`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/templates/subdir/foo/modtest.html.py` & `Mako-1.3.4/test/templates/subdir/foo/modtest.html.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_ast.py` & `Mako-1.3.4/test/test_ast.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_block.py` & `Mako-1.3.4/test/test_block.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_cache.py` & `Mako-1.3.4/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_call.py` & `Mako-1.3.4/test/test_call.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_cmd.py` & `Mako-1.3.4/test/test_cmd.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_decorators.py` & `Mako-1.3.4/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_def.py` & `Mako-1.3.4/test/test_def.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_exceptions.py` & `Mako-1.3.4/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_filters.py` & `Mako-1.3.4/test/test_filters.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_inheritance.py` & `Mako-1.3.4/test/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_lexer.py` & `Mako-1.3.4/test/test_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -806,14 +806,180 @@
                         r"""'Tricky string: ' + '\\\"\\\'|\\'""", [], (4, 13)
                     ),
                     Text("\n        ", (4, 49)),
                 ],
             ),
         )
 
+    def test_dict_expression(self):
+        template = """
+        <%def name="dtest(d)">
+            % for k,v in d.items():
+            ${k} = ${v}
+            % endfor
+        </%def>
+
+        <%self:dtest d="${
+                            {
+                                'id':'4',
+                                'foo':'barr'
+                            }
+                        }" />
+        """
+        nodes = Lexer(template).parse()
+        self._compare(
+            nodes,
+            TemplateNode(
+                {},
+                [
+                    Text("\n        ", (1, 1)),
+                    DefTag(
+                        "def",
+                        {"name": "dtest(d)"},
+                        (2, 9),
+                        [
+                            Text("\n", (2, 31)),
+                            ControlLine(
+                                "for", "for k,v in d.items():", False, (3, 1)
+                            ),
+                            Text("            ", (4, 1)),
+                            Expression("k", [], (4, 13)),
+                            Text(" = ", (4, 17)),
+                            Expression("v", [], (4, 20)),
+                            Text("\n", (4, 24)),
+                            ControlLine("for", "endfor", True, (5, 1)),
+                            Text("        ", (6, 1)),
+                        ],
+                    ),
+                    Text("\n\n        ", (6, 16)),
+                    CallNamespaceTag(
+                        "self:dtest",
+                        {
+                            "d": "${\n                            "
+                            "{\n                                'id':'4',\n"
+                            "                                'foo':'barr'\n"
+                            "                            }\n"
+                            "                        }"
+                        },
+                        (8, 9),
+                        [],
+                    ),
+                    Text("\n        ", (13, 30)),
+                ],
+            ),
+        )
+
+    def test_dict_expression_2(self):
+        template = """
+        <%def name="thing(thing)">
+            ${type(thing)}
+        </%def>
+
+        <%self:thing thing="foo" />
+
+        <%self:thing thing="${5}" />
+
+        <%self:thing thing="${[1,2,3]}" />
+
+        <%self:thing thing="${{'id':'4'}, {'id': 5}}" />
+
+
+        <%
+            foo="this is foo"
+            g=False
+        %>
+
+        <%def name="bar(x, y)">
+            ${x} ${y}
+        </%def>
+
+        <%self:bar x=" ${{'id':4}} " y="x${g and '1' or '2'}y"/>
+
+        <%self:dtest d="${ {
+            'x-on:click':foo,
+            'foo':'bar'
+        } }" />
+        """
+        nodes = Lexer(template).parse()
+        self._compare(
+            nodes,
+            TemplateNode(
+                {},
+                [
+                    Text("\n        ", (1, 1)),
+                    DefTag(
+                        "def",
+                        {"name": "thing(thing)"},
+                        (2, 9),
+                        [
+                            Text("\n            ", (2, 35)),
+                            Expression("type(thing)", [], (3, 13)),
+                            Text("\n        ", (3, 27)),
+                        ],
+                    ),
+                    Text("\n\n        ", (4, 16)),
+                    CallNamespaceTag(
+                        "self:thing", {"thing": "foo"}, (6, 9), []
+                    ),
+                    Text("\n\n        ", (6, 36)),
+                    CallNamespaceTag(
+                        "self:thing", {"thing": "${5}"}, (8, 9), []
+                    ),
+                    Text("\n\n        ", (8, 37)),
+                    CallNamespaceTag(
+                        "self:thing", {"thing": "${[1,2,3]}"}, (10, 9), []
+                    ),
+                    Text("\n\n        ", (10, 43)),
+                    CallNamespaceTag(
+                        "self:thing",
+                        {"thing": "${{'id':'4'}, {'id': 5}}"},
+                        (12, 9),
+                        [],
+                    ),
+                    Text("\n\n\n        ", (12, 57)),
+                    Code(
+                        '\nfoo="this is foo"\ng=False\n        \n',
+                        False,
+                        (15, 9),
+                    ),
+                    Text("\n\n        ", (18, 11)),
+                    DefTag(
+                        "def",
+                        {"name": "bar(x, y)"},
+                        (20, 9),
+                        [
+                            Text("\n            ", (20, 32)),
+                            Expression("x", [], (21, 13)),
+                            Text(" ", (21, 17)),
+                            Expression("y", [], (21, 18)),
+                            Text("\n        ", (21, 22)),
+                        ],
+                    ),
+                    Text("\n\n        ", (22, 16)),
+                    CallNamespaceTag(
+                        "self:bar",
+                        {"x": " ${{'id':4}} ", "y": "x${g and '1' or '2'}y"},
+                        (24, 9),
+                        [],
+                    ),
+                    Text("\n\n        ", (24, 65)),
+                    CallNamespaceTag(
+                        "self:dtest",
+                        {
+                            "d": "${ {\n            'x-on:click':foo,\n"
+                            "            'foo':'bar'\n        } }"
+                        },
+                        (26, 9),
+                        [],
+                    ),
+                    Text("\n        ", (29, 16)),
+                ],
+            ),
+        )
+
     def test_tricky_code(self):
         template = """<% print('hi %>') %>"""
         nodes = Lexer(template).parse()
         self._compare(
             nodes, TemplateNode({}, [Code("print('hi %>') \n", False, (1, 1))])
         )
```

### Comparing `Mako-1.3.3/test/test_lookup.py` & `Mako-1.3.4/test/test_lookup.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_loop.py` & `Mako-1.3.4/test/test_loop.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_lru.py` & `Mako-1.3.4/test/test_lru.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_namespace.py` & `Mako-1.3.4/test/test_namespace.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_pygen.py` & `Mako-1.3.4/test/test_pygen.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_template.py` & `Mako-1.3.4/test/test_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -874,14 +874,29 @@
             ${",".join([t for t in ("a", "b", "c")])}
         """,
             strict_undefined=True,
         )
 
         eq_(result_lines(t.render(t="T")), ["t is: T", "a,b,c"])
 
+    def test_dict_comprehensions_in_function_plus_undeclared_strict(self):
+        t = Template(
+            """
+<%
+    def foo():
+        return {s[0]: s for s in ('foo',)}
+%>
+
+${ foo()['f'] }
+""",
+            strict_undefined=True,
+        )
+
+        eq_(result_lines(t.render()), ["foo"])
+
 
 class StopRenderingTest(TemplateTest):
     def test_return_in_template(self):
         t = Template(
             """
            Line one
            <% return STOP_RENDERING %>
```

### Comparing `Mako-1.3.3/test/test_tgplugin.py` & `Mako-1.3.4/test/test_tgplugin.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/test_util.py` & `Mako-1.3.4/test/test_util.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/test/testing/test_config.py` & `Mako-1.3.4/test/testing/test_config.py`

 * *Files identical despite different names*

### Comparing `Mako-1.3.3/tox.ini` & `Mako-1.3.4/tox.ini`

 * *Files identical despite different names*

