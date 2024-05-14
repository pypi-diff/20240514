# Comparing `tmp/django-cid-2.3.tar.gz` & `tmp/django-cid-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cid-2.3.tar", last modified: Mon Jun 13 04:23:51 2022, max compression
+gzip compressed data, was "django-cid-2.4.tar", last modified: Tue May 14 15:16:09 2024, max compression
```

## Comparing `django-cid-2.3.tar` & `django-cid-2.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/
--rw-r--r--   0 damien    (1000) damien    (1000)      278 2022-06-13 04:23:51.000000 django-cid-2.3/AUTHORS.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     2818 2022-06-13 04:23:51.000000 django-cid-2.3/CONTRIBUTING.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     3270 2022-06-13 04:23:51.000000 django-cid-2.3/HISTORY.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     1463 2022-06-13 04:23:51.000000 django-cid-2.3/LICENSE
--rw-r--r--   0 damien    (1000) damien    (1000)      288 2022-06-13 04:23:51.000000 django-cid-2.3/MANIFEST.in
--rw-r--r--   0 damien    (1000) damien    (1000)     3074 2022-06-13 04:23:51.486252 django-cid-2.3/PKG-INFO
--rw-r--r--   0 damien    (1000) damien    (1000)     2157 2022-06-13 04:23:51.000000 django-cid-2.3/README.rst
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/
--rw-r--r--   0 damien    (1000) damien    (1000)       90 2022-06-13 04:23:51.000000 django-cid-2.3/cid/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)      127 2022-06-13 04:23:51.000000 django-cid-2.3/cid/apps.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/backends/
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/__init__.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/backends/mysql/
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/mysql/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)      302 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/mysql/base.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/backends/oracle/
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/oracle/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)      303 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/oracle/base.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/backends/postgis/
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/postgis/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)      325 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/postgis/base.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/backends/postgresql/
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/postgresql/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)      307 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/postgresql/base.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/backends/sqlite3/
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/sqlite3/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)      305 2022-06-13 04:23:51.000000 django-cid-2.3/cid/backends/sqlite3/base.py
--rw-r--r--   0 damien    (1000) damien    (1000)      244 2022-06-13 04:23:51.000000 django-cid-2.3/cid/context_processors.py
--rw-r--r--   0 damien    (1000) damien    (1000)     1515 2022-06-13 04:23:51.000000 django-cid-2.3/cid/cursor.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/cid/locals/
--rw-r--r--   0 damien    (1000) damien    (1000)      374 2022-06-13 04:23:51.000000 django-cid-2.3/cid/locals/__init__.py
--rw-r--r--   0 damien    (1000) damien    (1000)      588 2022-06-13 04:23:51.000000 django-cid-2.3/cid/locals/base.py
--rw-r--r--   0 damien    (1000) damien    (1000)      497 2022-06-13 04:23:51.000000 django-cid-2.3/cid/locals/context.py
--rw-r--r--   0 damien    (1000) damien    (1000)      626 2022-06-13 04:23:51.000000 django-cid-2.3/cid/locals/thread_local.py
--rw-r--r--   0 damien    (1000) damien    (1000)      171 2022-06-13 04:23:51.000000 django-cid-2.3/cid/log.py
--rw-r--r--   0 damien    (1000) damien    (1000)     1202 2022-06-13 04:23:51.000000 django-cid-2.3/cid/middleware.py
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/cid/models.py
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/django_cid.egg-info/
--rw-r--r--   0 damien    (1000) damien    (1000)     3074 2022-06-13 04:23:51.000000 django-cid-2.3/django_cid.egg-info/PKG-INFO
--rw-r--r--   0 damien    (1000) damien    (1000)     1046 2022-06-13 04:23:51.000000 django-cid-2.3/django_cid.egg-info/SOURCES.txt
--rw-r--r--   0 damien    (1000) damien    (1000)        1 2022-06-13 04:23:51.000000 django-cid-2.3/django_cid.egg-info/dependency_links.txt
--rw-r--r--   0 damien    (1000) damien    (1000)        1 2022-06-13 04:23:51.000000 django-cid-2.3/django_cid.egg-info/not-zip-safe
--rw-r--r--   0 damien    (1000) damien    (1000)       12 2022-06-13 04:23:51.000000 django-cid-2.3/django_cid.egg-info/requires.txt
--rw-r--r--   0 damien    (1000) damien    (1000)        4 2022-06-13 04:23:51.000000 django-cid-2.3/django_cid.egg-info/top_level.txt
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/docs/
--rw-r--r--   0 damien    (1000) damien    (1000)      626 2022-06-13 04:23:51.000000 django-cid-2.3/docs/Makefile
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/docs/_static/
--rw-r--r--   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.000000 django-cid-2.3/docs/_static/__empty__
-drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2022-06-13 04:23:51.486252 django-cid-2.3/docs/_static/css/
--rw-r--r--   0 damien    (1000) damien    (1000)       47 2022-06-13 04:23:51.000000 django-cid-2.3/docs/_static/css/custom.css
--rw-r--r--   0 damien    (1000) damien    (1000)       93 2022-06-13 04:23:51.000000 django-cid-2.3/docs/api.rst
--rw-r--r--   0 damien    (1000) damien    (1000)       27 2022-06-13 04:23:51.000000 django-cid-2.3/docs/authors.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     5348 2022-06-13 04:23:51.000000 django-cid-2.3/docs/conf.py
--rw-r--r--   0 damien    (1000) damien    (1000)       32 2022-06-13 04:23:51.000000 django-cid-2.3/docs/contributing.rst
--rw-r--r--   0 damien    (1000) damien    (1000)       27 2022-06-13 04:23:51.000000 django-cid-2.3/docs/history.rst
--rw-r--r--   0 damien    (1000) damien    (1000)      223 2022-06-13 04:23:51.000000 django-cid-2.3/docs/index.rst
--rw-r--r--   0 damien    (1000) damien    (1000)     7733 2022-06-13 04:23:51.000000 django-cid-2.3/docs/installation.rst
--rw-r--r--   0 damien    (1000) damien    (1000)      832 2022-06-13 04:23:51.000000 django-cid-2.3/docs/make.bat
--rw-r--r--   0 damien    (1000) damien    (1000)      782 2022-06-13 04:23:51.000000 django-cid-2.3/docs/releasing.rst
--rw-r--r--   0 damien    (1000) damien    (1000)      103 2022-06-13 04:23:51.489585 django-cid-2.3/setup.cfg
--rwxr-xr-x   0 damien    (1000) damien    (1000)     1224 2022-06-13 04:23:51.000000 django-cid-2.3/setup.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.278527 django-cid-2.4/
+-rw-r--r--   0 damien    (1000) damien    (1000)      278 2024-05-14 15:16:08.000000 django-cid-2.4/AUTHORS.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)     2818 2024-05-14 15:16:08.000000 django-cid-2.4/CONTRIBUTING.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)     3487 2024-05-14 15:16:08.000000 django-cid-2.4/HISTORY.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)     1463 2024-05-14 15:16:08.000000 django-cid-2.4/LICENSE
+-rw-r--r--   0 damien    (1000) damien    (1000)      288 2024-05-14 15:16:08.000000 django-cid-2.4/MANIFEST.in
+-rw-r--r--   0 damien    (1000) damien    (1000)     3054 2024-05-14 15:16:09.278527 django-cid-2.4/PKG-INFO
+-rw-r--r--   0 damien    (1000) damien    (1000)     2157 2024-05-14 15:16:08.000000 django-cid-2.4/README.rst
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.276527 django-cid-2.4/cid/
+-rw-r--r--   0 damien    (1000) damien    (1000)      163 2024-05-14 15:16:08.000000 django-cid-2.4/cid/__init__.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      127 2024-05-14 15:16:08.000000 django-cid-2.4/cid/apps.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.276527 django-cid-2.4/cid/backends/
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/__init__.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.276527 django-cid-2.4/cid/backends/mysql/
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/mysql/__init__.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      302 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/mysql/base.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.276527 django-cid-2.4/cid/backends/oracle/
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/oracle/__init__.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      303 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/oracle/base.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.276527 django-cid-2.4/cid/backends/postgis/
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/postgis/__init__.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      325 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/postgis/base.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.276527 django-cid-2.4/cid/backends/postgresql/
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/postgresql/__init__.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      307 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/postgresql/base.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.276527 django-cid-2.4/cid/backends/sqlite3/
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/sqlite3/__init__.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      305 2024-05-14 15:16:08.000000 django-cid-2.4/cid/backends/sqlite3/base.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      244 2024-05-14 15:16:08.000000 django-cid-2.4/cid/context_processors.py
+-rw-r--r--   0 damien    (1000) damien    (1000)     1760 2024-05-14 15:16:08.000000 django-cid-2.4/cid/cursor.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.277527 django-cid-2.4/cid/locals/
+-rw-r--r--   0 damien    (1000) damien    (1000)      374 2024-05-14 15:16:08.000000 django-cid-2.4/cid/locals/__init__.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      588 2024-05-14 15:16:08.000000 django-cid-2.4/cid/locals/base.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      497 2024-05-14 15:16:08.000000 django-cid-2.4/cid/locals/context.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      626 2024-05-14 15:16:08.000000 django-cid-2.4/cid/locals/thread_local.py
+-rw-r--r--   0 damien    (1000) damien    (1000)      171 2024-05-14 15:16:08.000000 django-cid-2.4/cid/log.py
+-rw-r--r--   0 damien    (1000) damien    (1000)     1202 2024-05-14 15:16:08.000000 django-cid-2.4/cid/middleware.py
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/cid/models.py
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.277527 django-cid-2.4/django_cid.egg-info/
+-rw-r--r--   0 damien    (1000) damien    (1000)     3054 2024-05-14 15:16:09.000000 django-cid-2.4/django_cid.egg-info/PKG-INFO
+-rw-r--r--   0 damien    (1000) damien    (1000)     1046 2024-05-14 15:16:09.000000 django-cid-2.4/django_cid.egg-info/SOURCES.txt
+-rw-r--r--   0 damien    (1000) damien    (1000)        1 2024-05-14 15:16:09.000000 django-cid-2.4/django_cid.egg-info/dependency_links.txt
+-rw-r--r--   0 damien    (1000) damien    (1000)        1 2024-05-14 15:16:09.000000 django-cid-2.4/django_cid.egg-info/not-zip-safe
+-rw-r--r--   0 damien    (1000) damien    (1000)       58 2024-05-14 15:16:09.000000 django-cid-2.4/django_cid.egg-info/requires.txt
+-rw-r--r--   0 damien    (1000) damien    (1000)        4 2024-05-14 15:16:09.000000 django-cid-2.4/django_cid.egg-info/top_level.txt
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.278527 django-cid-2.4/docs/
+-rw-r--r--   0 damien    (1000) damien    (1000)      626 2024-05-14 15:16:08.000000 django-cid-2.4/docs/Makefile
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.278527 django-cid-2.4/docs/_static/
+-rw-r--r--   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:08.000000 django-cid-2.4/docs/_static/__empty__
+drwxr-xr-x   0 damien    (1000) damien    (1000)        0 2024-05-14 15:16:09.278527 django-cid-2.4/docs/_static/css/
+-rw-r--r--   0 damien    (1000) damien    (1000)       47 2024-05-14 15:16:08.000000 django-cid-2.4/docs/_static/css/custom.css
+-rw-r--r--   0 damien    (1000) damien    (1000)       93 2024-05-14 15:16:08.000000 django-cid-2.4/docs/api.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)       27 2024-05-14 15:16:08.000000 django-cid-2.4/docs/authors.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)     5348 2024-05-14 15:16:08.000000 django-cid-2.4/docs/conf.py
+-rw-r--r--   0 damien    (1000) damien    (1000)       32 2024-05-14 15:16:08.000000 django-cid-2.4/docs/contributing.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)       27 2024-05-14 15:16:08.000000 django-cid-2.4/docs/history.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)      223 2024-05-14 15:16:08.000000 django-cid-2.4/docs/index.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)     8005 2024-05-14 15:16:08.000000 django-cid-2.4/docs/installation.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)      832 2024-05-14 15:16:08.000000 django-cid-2.4/docs/make.bat
+-rw-r--r--   0 damien    (1000) damien    (1000)      782 2024-05-14 15:16:08.000000 django-cid-2.4/docs/releasing.rst
+-rw-r--r--   0 damien    (1000) damien    (1000)      103 2024-05-14 15:16:09.278527 django-cid-2.4/setup.cfg
+-rwxr-xr-x   0 damien    (1000) damien    (1000)     1335 2024-05-14 15:16:08.000000 django-cid-2.4/setup.py
```

### Comparing `django-cid-2.3/CONTRIBUTING.rst` & `django-cid-2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/HISTORY.rst` & `django-cid-2.4/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 -------
 
 .. role:: strike
     :class: strike
 
 
 
+2.4 (2024-05-14)
+++++++++++++++++
+
+- Add `CID_SQL_STATEMENT_TEMPLATE` setting to customize the position
+  of the correlation relative to the original SQL statement.
+  Contributed by Cauê Garcia Polimanti (@CaueP).
+
+
 2.3 (2022-06-13)
 ++++++++++++++++
 
 - Under Python 3.7 and later, use context variables (with the contextvars module)
   instead of a thread-local variable to avoid state bleeding in concurrent code.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-cid-2.3/LICENSE` & `django-cid-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/PKG-INFO` & `django-cid-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: django-cid
-Version: 2.3
+Version: 2.4
 Summary: Correlation IDs in Django for debugging requests
 Home-page: https://github.com/Polyconseil/django-cid
 Author: Snowball One
 Author-email: opensource+django-cid@polyconseil.fr
 Maintainer: Polyconseil
 Maintainer-email: opensource+django-cid@polyconseil.fr
 License: BSD
 Keywords: django logging correlation id debugging
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -71,9 +70,7 @@
 
 Supported versions
 ------------------
 
 We currently support Python >= 3.6 and Django >= 2.2.
 
 Other versions may work but are not supported.
-
-
```

### Comparing `django-cid-2.3/README.rst` & `django-cid-2.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/cid/cursor.py` & `django-cid-2.4/cid/cursor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.conf import settings
 
 from .locals import get_cid
 
 
 DEFAULT_CID_SQL_COMMENT_TEMPLATE = 'cid: {cid}'
+DEFAULT_SQL_STATEMENT_TEMPLATE = '/* {cid} */\n{sql}'
 
 
 class CidCursorWrapper:
     """
     A cursor wrapper that attempts to add a cid comment to each query
     """
     def __init__(self, cursor):
@@ -27,20 +28,24 @@
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def add_comment(self, sql):
         cid_sql_template = getattr(
             settings, 'CID_SQL_COMMENT_TEMPLATE', DEFAULT_CID_SQL_COMMENT_TEMPLATE
         )
+        sql_statement_template = getattr(
+            settings, 'CID_SQL_STATEMENT_TEMPLATE', DEFAULT_SQL_STATEMENT_TEMPLATE
+        )
         cid = get_cid()
         if not cid:
             return sql
         cid = cid.replace('/*', r'\/\*').replace('*/', r'\*\/')
         cid = cid_sql_template.format(cid=cid)
-        return f"/* {cid} */\n{sql}"
+        statement = sql_statement_template.format(cid=cid, sql=sql)
+        return statement
 
     # The following methods cannot be implemented in __getattr__, because the
     # code must run when the method is invoked, not just when it is accessed.
 
     def callproc(self, procname, params=None):
         return self.cursor.callproc(procname, params)
```

### Comparing `django-cid-2.3/cid/locals/base.py` & `django-cid-2.4/cid/locals/base.py`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/cid/locals/thread_local.py` & `django-cid-2.4/cid/locals/thread_local.py`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/cid/middleware.py` & `django-cid-2.4/cid/middleware.py`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/django_cid.egg-info/PKG-INFO` & `django-cid-2.4/django_cid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: django-cid
-Version: 2.3
+Version: 2.4
 Summary: Correlation IDs in Django for debugging requests
 Home-page: https://github.com/Polyconseil/django-cid
 Author: Snowball One
 Author-email: opensource+django-cid@polyconseil.fr
 Maintainer: Polyconseil
 Maintainer-email: opensource+django-cid@polyconseil.fr
 License: BSD
 Keywords: django logging correlation id debugging
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -71,9 +70,7 @@
 
 Supported versions
 ------------------
 
 We currently support Python >= 3.6 and Django >= 2.2.
 
 Other versions may work but are not supported.
-
-
```

### Comparing `django-cid-2.3/django_cid.egg-info/SOURCES.txt` & `django-cid-2.4/django_cid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/docs/Makefile` & `django-cid-2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/docs/conf.py` & `django-cid-2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/docs/installation.rst` & `django-cid-2.4/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,23 @@
 a string with a ``cid`` format parameter:
 
 .. code-block:: python
 
     CID_SQL_COMMENT_TEMPLATE = 'correlation={cid}'
 
 
+Also, you may change the position of the correlation id injected in
+the statement by defining a ``CID_SQL_STATEMENT_TEMPLATE`` that is
+a string with a ``cid`` and a ``sql`` format parameter:
+
+.. code-block:: python
+
+    CID_SQL_STATEMENT_TEMPLATE = '/* {cid} */\n{sql}'
+
+
 Inclusion of the correlation id in templates
 --------------------------------------------
 
 ``django-cid`` provides a template context processor that adds the
 correlation id to the template context if it is available. To enable
 it, you need to add it in the list of ``TEMPLATE_CONTEXT_PROCESSORS``
 in the settings:
```

### Comparing `django-cid-2.3/docs/make.bat` & `django-cid-2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/docs/releasing.rst` & `django-cid-2.4/docs/releasing.rst`

 * *Files identical despite different names*

### Comparing `django-cid-2.3/setup.py` & `django-cid-2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 
 
 with open('README.rst', encoding="utf-8") as fp:
     readme = fp.read()
 
 setup(
     name='django-cid',
-    version='2.3',
+    version='2.4',
     description="""Correlation IDs in Django for debugging requests""",
     long_description=readme,
     author='Snowball One',
     author_email='opensource+django-cid@polyconseil.fr',
     maintainer="Polyconseil",
     maintainer_email="opensource+django-cid@polyconseil.fr",
     url='https://github.com/Polyconseil/django-cid',
     packages=find_packages(exclude=('sandbox*', 'tests*')),
     include_package_data=True,
     install_requires=[
         'django>=2.2',
     ],
+    extras_require={
+        ":python_version < '3.8'": [
+            'importlib_metadata',
+        ],
+    },
+
     license="BSD",
     zip_safe=False,
     keywords='django logging correlation id debugging',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Framework :: Django',
         'Intended Audience :: Developers',
```

