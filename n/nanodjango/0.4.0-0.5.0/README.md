# Comparing `tmp/nanodjango-0.4.0.tar.gz` & `tmp/nanodjango-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanodjango-0.4.0.tar", last modified: Sun Apr 21 09:50:36 2024, max compression
+gzip compressed data, was "nanodjango-0.5.0.tar", last modified: Tue May 14 19:19:15 2024, max compression
```

## Comparing `nanodjango-0.4.0.tar` & `nanodjango-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-21 09:50:36.661413 nanodjango-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-21 09:50:31.000000 nanodjango-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.657412 nanodjango-0.4.0/nanodjango/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/app_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/nanodjango/convert/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16626 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/convert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/nanodjango/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/django_glue/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/django_glue/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-21 09:50:31.000000 nanodjango-0.4.0/nanodjango/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/nanodjango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 09:50:36.000000 nanodjango-0.4.0/nanodjango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-21 09:50:31.000000 nanodjango-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 09:50:36.661413 nanodjango-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 09:50:36.661413 nanodjango-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-21 09:50:31.000000 nanodjango-0.4.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-21 09:50:31.000000 nanodjango-0.4.0/tests/test_run_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-21 09:50:31.000000 nanodjango-0.4.0/tests/test_run_runserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.504042 nanodjango-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-14 19:19:15.500042 nanodjango-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-14 19:19:10.000000 nanodjango-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.496042 nanodjango-0.5.0/nanodjango/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/app_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango/convert/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/contrib/django_ninja.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/convert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/django_glue/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/django_glue/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 19:19:10.000000 nanodjango-0.5.0/nanodjango/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/nanodjango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 19:19:15.000000 nanodjango-0.5.0/nanodjango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-14 19:19:10.000000 nanodjango-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:19:15.504042 nanodjango-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:19:15.500042 nanodjango-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 19:19:10.000000 nanodjango-0.5.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-14 19:19:10.000000 nanodjango-0.5.0/tests/test_run_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-14 19:19:10.000000 nanodjango-0.5.0/tests/test_run_runserver.py
```

### Comparing `nanodjango-0.4.0/PKG-INFO` & `nanodjango-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodjango
-Version: 0.4.0
+Version: 0.5.0
 Summary: Run Django models and views from a single file, and convert it to a full project.
 Author-email: Richard Terry <code@radiac.net>
 Project-URL: Homepage, https://radiac.net/projects/nanodjango/
 Project-URL: Documentation, https://nanodjango.readthedocs.io/en/latest/
 Project-URL: Changelog, https://nanodjango.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/radiac/nanodjango
 Project-URL: Issues, https://github.com/radiac/nanodjango/issues
@@ -27,15 +27,20 @@
 [![Documentation](https://readthedocs.org/projects/nanodjango/badge/?version=latest)](https://nanodjango.readthedocs.io/en/latest/)
 [![Tests](https://github.com/radiac/nanodjango/actions/workflows/ci.yml/badge.svg)](https://github.com/radiac/nanodjango/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/radiac/nanodjango/branch/main/graph/badge.svg?token=BCNM45T6GI)](https://codecov.io/gh/radiac/nanodjango)
 
 Write a Django site in a single file, using views, models and admin, then automatically
 convert it to a full Django project when you're ready for it to grow.
 
-Perfect for experiments, prototypes, tutorials, and small applications.
+An alternative to Flask (see example below) and FastAPI (see our django-ninja example) -
+similar simple syntax, but with full access to Django's features such as the ORM, auth
+and admin site.
+
+Perfect for experiments, prototypes, sharing working code samples, and deploying small
+production applications.
 
 
 ## Quickstart
 
 
 Install nanodjango:
 
@@ -48,33 +53,33 @@
 are:
 
 ```python
 
 from django.db import models
 from nanodjango import Django
 
-app = Django(ADMIN_URL="admin/")
+app = Django()
 
 @app.admin
 class CountLog(models.Model):
     timestamp = models.DateTimeField(auto_now_add=True)
 
 @app.route("/")
 def count(request):
     CountLog.objects.create()
     return f"<p>Number of page loads: {CountLog.objects.count()}</p>"
 ```
 
 Save that as ``counter.py``, then set up your database and run it locally with:
 
 ```sh
-nanodjango counter.py run makemigrations counter
-nanodjango counter.py run migrate
-nanodjango counter.py run createsuperuser
-nanodjango counter.py run
+nanodjango run counter.py makemigrations counter
+nanodjango run counter.py migrate
+nanodjango run counter.py createsuperuser
+nanodjango run counter.py
 ```
 
 It will create your database in a ``db.sqlite3`` file next to your ``counter.py``, with
 the appropriate migrations in ``migrations/``.
 
 Run it in production using WSGI:
 
@@ -102,7 +107,9 @@
 
 For more details, see
 
 * [Getting started](https://nanodjango.readthedocs.io/en/latest/get_started.html)
 * [Tutorial](https://nanodjango.readthedocs.io/en/latest/tutorial.html)
 * [Full Documentation](https://nanodjango.readthedocs.io/en/latest/index.html)
 * [Changelog](https://nanodjango.readthedocs.io/en/latest/changelog.html)
+* [Examples](https://github.com/radiac/nanodjango/tree/main/examples) including how to
+  use nanodjango with Django Ninja
```

### Comparing `nanodjango-0.4.0/README.md` & `nanodjango-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 [![Documentation](https://readthedocs.org/projects/nanodjango/badge/?version=latest)](https://nanodjango.readthedocs.io/en/latest/)
 [![Tests](https://github.com/radiac/nanodjango/actions/workflows/ci.yml/badge.svg)](https://github.com/radiac/nanodjango/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/radiac/nanodjango/branch/main/graph/badge.svg?token=BCNM45T6GI)](https://codecov.io/gh/radiac/nanodjango)
 
 Write a Django site in a single file, using views, models and admin, then automatically
 convert it to a full Django project when you're ready for it to grow.
 
-Perfect for experiments, prototypes, tutorials, and small applications.
+An alternative to Flask (see example below) and FastAPI (see our django-ninja example) -
+similar simple syntax, but with full access to Django's features such as the ORM, auth
+and admin site.
+
+Perfect for experiments, prototypes, sharing working code samples, and deploying small
+production applications.
 
 
 ## Quickstart
 
 
 Install nanodjango:
 
@@ -25,33 +30,33 @@
 are:
 
 ```python
 
 from django.db import models
 from nanodjango import Django
 
-app = Django(ADMIN_URL="admin/")
+app = Django()
 
 @app.admin
 class CountLog(models.Model):
     timestamp = models.DateTimeField(auto_now_add=True)
 
 @app.route("/")
 def count(request):
     CountLog.objects.create()
     return f"<p>Number of page loads: {CountLog.objects.count()}</p>"
 ```
 
 Save that as ``counter.py``, then set up your database and run it locally with:
 
 ```sh
-nanodjango counter.py run makemigrations counter
-nanodjango counter.py run migrate
-nanodjango counter.py run createsuperuser
-nanodjango counter.py run
+nanodjango run counter.py makemigrations counter
+nanodjango run counter.py migrate
+nanodjango run counter.py createsuperuser
+nanodjango run counter.py
 ```
 
 It will create your database in a ``db.sqlite3`` file next to your ``counter.py``, with
 the appropriate migrations in ``migrations/``.
 
 Run it in production using WSGI:
 
@@ -79,7 +84,9 @@
 
 For more details, see
 
 * [Getting started](https://nanodjango.readthedocs.io/en/latest/get_started.html)
 * [Tutorial](https://nanodjango.readthedocs.io/en/latest/tutorial.html)
 * [Full Documentation](https://nanodjango.readthedocs.io/en/latest/index.html)
 * [Changelog](https://nanodjango.readthedocs.io/en/latest/changelog.html)
+* [Examples](https://github.com/radiac/nanodjango/tree/main/examples) including how to
+  use nanodjango with Django Ninja
```

### Comparing `nanodjango-0.4.0/nanodjango/app.py` & `nanodjango-0.5.0/nanodjango/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import os
 import sys
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, Callable
 
 from django import setup
+from django import urls as django_urls
 from django.contrib import admin
-from django.urls import path as url_path
 from django.views import View
 
 from . import app_meta
 from .exceptions import ConfigurationError, UsageError
 from .urls import urlpatterns
 from .views import string_view
 
@@ -25,28 +25,45 @@
 
 
 class Django:
     """
     The main Django app
     """
 
+    # Class variable to ensure there can be only one
+    _instantiated = False
+
     #: Name of the app script
     app_name: str
 
     #: Reference to the app script's module
     app_module: ModuleType
 
     #: Path of app script
     app_path: Path
 
-    # Caches to aid ``convert``
-    _settings: dict[str, Any] = {}
-    _routes: dict[str, Callable] = {}
+    #: Whether this app has defined an @app.admin
+    has_admin: bool = False
+
+    #: Variable name for this current app
+    _instance_name: str
+
+    # Settings cache to aid ``convert``
+    _settings: dict[str, Any]
+
+    # URL cache to aid ``convert``
+    # {pattern:
+    _routes: dict[str, tuple[Callable | None, dict[str, Any]]]
 
     def __new__(cls, *args, **kwargs):
+        # Enforce only one Django() per script, otherwise everything will get confused
+        if cls._instantiated:
+            raise ConfigurationError("An app can only have one Django() instance")
+        cls._instantiated = True
+
         instance = super().__new__(cls)
 
         # Set app meta
         app_name = inspect.stack()[1].frame.f_globals["__name__"]
         app_meta._app_module = sys.modules[app_name]
         return instance
 
@@ -55,14 +72,17 @@
         Initialise a new Django app, optionally with settings
 
         Usage::
 
             app = Django()
             app = Django(SECRET_KEY="some-secret", ALLOWED_HOSTS=["my.example.com"])
         """
+        self.has_admin = False
+        self._settings = {}
+        self._routes = {}
         self._config(_settings)
 
     def _config(self, _settings):
         """
         Configure settings and patch Django ready for model definitions
         """
         self._settings = app_meta._app_conf = _settings
@@ -93,96 +113,129 @@
     def _prepare(self):
         """
         Perform any final setup for this project after it has been imported:
 
         * register the admin site
         """
         admin_url = self.settings.ADMIN_URL
-        if admin_url:
+        if admin_url or self.has_admin:
+            if admin_url is None:
+                admin_url = "admin/"
             if not isinstance(admin_url, str) or not admin_url.endswith("/"):
                 raise ConfigurationError(
                     "settings.ADMIN_URL must be a string path ending in /"
                 )
-            urlpatterns.append(url_path(admin_url.removeprefix("/"), admin.site.urls))
+            urlpatterns.append(
+                django_urls.path(admin_url.removeprefix("/"), admin.site.urls)
+            )
 
-    def route(self, pattern: str):
+    def route(self, pattern: str, *, re=False, include=None):
         """
         Decorator to add a view to the urls
 
         The pattern should use the Django path syntax - see
         https://docs.djangoproject.com/en/dev/ref/urls/#path
 
         Usage::
 
+            # No parameters
             @app.route("/")
             def view(request):
                 return "Hello"
 
+            # path() parameters
+            @app.route("/<int:pk>/")
+            def view(request, pk):
+                return f"Hello {pk}"
+
+            # re_path() parameters
+            @app.route("/(?P<slug>[a-z]/", re=True)
+            def view(request, char):
+                return f"Hello {char}"
+
+            # Include another urlconf
+            # Note this is called as a function, not a decorator
+            # If this is a list not an include()
+            app.route("/api/", include=api.urls)
+
         All paths are relative to the root URL, leading slashes will be ignored.
         """
         # We want to support Flask-like patterns which have leading / in its patterns.
         # Django does not use these, so strip them out.
-        if pattern.startswith("/"):
-            pattern = pattern[1:]
+        pattern = pattern.removeprefix("/")
+
+        # Find if it's a path() or re_path()
+        path_fn = django_urls.re_path if re else django_urls.path
+
+        if include is not None:
+            # Being called directly with an include
+            urlpatterns.append(path_fn(pattern, include))
+
+            # If we're converting, we're going to need the source
+            caller = inspect.currentframe().f_back  # type: ignore
+            source = inspect.getframeinfo(caller).code_context[0]  # type: ignore
+            self._routes[pattern] = (
+                None,
+                {"re": re, "include": True, "source": source},
+            )
+
+            # Make sure this isn't being used as a decorator, that wouldn't make sense
+            def invalid(fn):
+                raise UsageError(
+                    "app.route(path, include=urlconf) cannot be used as a decorator"
+                )
+
+            return invalid
 
         def wrapped(fn):
             # Store route for convert lookup
-            self._routes[pattern] = fn
+            self._routes[pattern] = (fn, {"re": re, "include": False})
 
             # Prepare CBVs
             if inspect.isclass(fn) and issubclass(fn, View):
                 fn = fn.as_view()
 
             # Register URL
-            urlpatterns.append(
-                url_path(pattern.removeprefix("/"), string_view(fn), name=fn.__name__)
-            )
+            urlpatterns.append(path_fn(pattern, string_view(fn), name=fn.__name__))
             return fn
 
         return wrapped
 
-    @property
-    def has_admin(self):
-        return isinstance(self.settings.ADMIN_URL, str)
-
     def admin(self, model: type[Model] | None = None, **options):
         """
         Decorator to add a model to the admin site
 
         The admin site must be added using ``settings.ADMIN_URL``.
         """
-        if not self.has_admin:
-            raise ConfigurationError(
-                "Cannot register ModelAdmin - settings.ADMIN_URL is not set"
-            )
+        self.has_admin = True
 
         def wrap(model: type[Model]):
             admin.site.register(model, **options)
             return model
 
         if model is None:
             # Called with arguments, @admin(attr=val)
             return wrap
 
         # Called without arguments, @admin - call wrapped immediately
         return wrap(model)
 
-    def run(self, args: list[str] | None = None):
+    def run(self, args: list[str] | tuple[str] | None = None):
         """
         Run a Django management command, passing all arguments
 
         Defaults to:
             runserver 0:8000
         """
         # Check if this is being called from click commands or directly
         if self.app_name not in sys.modules:
             # Hasn't been run through the ``nanodjango`` command
             if (
                 "__main__" not in sys.modules
-                or getattr(sys.modules["__main__"], "app") != self
+                or getattr(sys.modules["__main__"], self._instance_name) != self
             ):
                 # Doesn't look like it was run directly either
                 raise UsageError("App module not initialised")
 
             # Run directly, so register app module so Django won't try to load it again
             sys.modules[self.app_name] = sys.modules["__main__"]
 
@@ -203,15 +256,15 @@
         from .convert import Converter
 
         if path.exists():
             raise UsageError("Upgrade path is not empty - path cannot exist")
         path.mkdir()
 
         converter = Converter(app=self, path=path, name=name)
-        converter.write()
+        converter.build()
 
     def __call__(self, *args, **kwargs):
         from django.core.wsgi import get_wsgi_application
 
         if "DEBUG" not in self._settings:
             from django.conf import settings
```

### Comparing `nanodjango-0.4.0/nanodjango/app_meta.py` & `nanodjango-0.5.0/nanodjango/app_meta.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.4.0/nanodjango/convert/converter.py` & `nanodjango-0.5.0/nanodjango/convert/converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,63 +2,90 @@
 
 import ast
 import inspect
 import os
 import shutil
 import subprocess
 from pathlib import Path
+from types import ModuleType
 from typing import TYPE_CHECKING, cast
 
 from django.db.models import Model
 
 import isort
 from black import FileMode, format_str
 
 from ..exceptions import ConversionError
 from .objects import AppModel, AppView
-from .utils import collect_references, ensure_http_response, import_from_path
+from .plugin import plugins
+from .utils import collect_references, ensure_http_response, import_from_path, make_url
 
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from ..app import Django
 
 
 class Resolver:
+    """
+    Resolve names and references within the scope of a generated Python file
+    """
+
     imports: set[str]
     local_refs: set[str]
     global_refs: set[str]
 
     def __init__(self, converter: Converter, module_name: str):
+        """
+        Args:
+            converter (Converter): The current converter instance
+            module_name (str): The name of the module we're currently building
+        """
         self.converter = converter
         self.module_name = module_name
 
         self.imports = set()
         self.local_refs = set()
         self.global_refs = set()
 
     def add(self, name: str, references: set[str]):
-        # Log this object definition
+        """
+        Register an object definition, and the objects it references
+        """
+        self.add_object(name)
+        self.add_references(references)
+
+    def add_object(self, name: str):
+        """
+        Register an object definition
+        """
         self.converter.imports[name] = f"from {self.module_name} import {name}"
         self.local_refs.add(name)
 
-        self.add_references(references)
-
     def add_references(self, references: set[str]):
-        # Collect import and global references
+        """
+        Collect references to imports and globals
+        """
         for ref in references:
-            if ref in self.local_refs:
+            # Most of the time this will be either an object or an imported symbol,
+            # but it could be an object.child, eg admin.site.urls
+            ref_base = ref.split(".", 1)[0]
+            if ref_base in self.local_refs:
                 pass
-            elif ref in self.converter.imports:
-                self.imports.add(self.converter.imports[ref])
+            elif ref_base in self.converter.imports:
+                self.imports.add(self.converter.imports[ref_base])
             else:
-                self.global_refs.add(ref)
+                self.global_refs.add(ref_base)
 
     def gen_src(self):
+        """
+        Generate the source code required to resolve discovered references, either by
+        copying in referenced code, or importing them from another file.
+        """
         all_src = []
         global_refs = self.global_refs.copy()
         while self.global_refs:
             # Collect the source for the reference, and grab any references it may have
             global_ref = self.global_refs.pop()
             src, references = self.converter.collect_definition(global_ref)
             all_src.append(src)
@@ -79,51 +106,186 @@
 
         # Restore global refs
         self.global_refs = global_refs
         return "\n".join(list(self.imports) + all_src)
 
 
 class Converter:
+    #: Reference to the ``Django`` app instance
+    app: Django
+
+    #: Root path to build the project (``django-admin startproject ... {root_path}``)
+    root_path: Path
+
+    #: Name of the Django project (``django-admin startproject {project_name} ...``)
+    project_name: str
+
+    #: The module to convert
+    module: ModuleType
+
+    #: The source for the module to convert
+    src: str
+
+    #: The abstract syntax tree of the module to convert
+    ast: ast.Module
+
     #: AppModel instances for models that are being moved to models.py
     models: list[AppModel]
 
     #: AppView instances for views that are being moved to views.py
     views: list[AppView]
 
     #: Import paths - existing imports in the app, plus converted models and views
     imports: dict[str, str]
 
     #: Definitions in the module's top level scope which have been converted
     used: set[str]
 
     def __init__(self, app: Django, path: Path, name: str):
+        """
+        Prepare state and load plugins
+        """
         self.app = app
         self.root_path = path
         self.project_name = name
         self.module = app.app_module
         self.src = inspect.getsource(app.app_module)
         self.ast = ast.parse(self.src)
+
+        self.models = []
+        self.views = []
+        self.imports = {}
         self.used = set()
 
-        self.collect_imports()
+        plugins.load()
+        plugins.init(self)
+
+    @property
+    def project_path(self):
+        return self.root_path / self.project_name
+
+    @property
+    def app_path(self):
+        return self.project_path / self.app.app_name
 
     def write_file(self, filename: str | Path, *content):
         path = Path(filename)
         formatted = isort.code(format_str("\n".join(content), mode=FileMode()))
         path.write_text(formatted)
 
-    def write(self) -> None:
+    def collect_definition(self, obj_name) -> tuple[str, set[str]]:
+        """
+        Collect a definition of a module top-level scope object
+
+        Args:
+            obj_name (str): Name of object to collect
+
+        Returns:
+            obj_src (str): Source for object
+            references (set[str]): Set of referenced object names
+        """
+        if obj_name == "ensure_http_response":
+            # Inject its dependencies
+            self.imports.update(getattr(ensure_http_response, "_dependencies", {}))
+            obj_src = inspect.getsource(ensure_http_response)
+            obj_ast = ast.parse(obj_src)
+            references = collect_references(obj_ast.body[0])
+            return obj_src, references
+
+        if obj_name not in self.module.__dict__:
+            raise ConversionError(f"Reference to unknown symbol {obj_name}")
+        obj = self.module.__dict__[obj_name]
+
+        # Try to build src from the object
+        try:
+            obj_src = inspect.getsource(obj)
+        except TypeError:
+            # Not a class, method, function, or code object
+            pass
+        else:
+            self.used.add(obj_name)
+            obj_ast = ast.parse(obj_src)
+            references = collect_references(obj_ast.body[0])
+            return obj_src, references
+
+        # Look for an assignment
+        for node in self.ast.body:
+            if isinstance(node, ast.Assign):
+                for target in node.targets:
+                    if isinstance(target, ast.Name) and target.id == obj_name:
+                        obj_src = ast.unparse(node).strip()
+                        self.used.add(obj_name)
+                        obj_ast = ast.parse(obj_src)
+                        references = collect_references(obj_ast.body[0])
+                        return obj_src, references
+
+        # TODO: We could have more exhaustive definition collection
+        raise ConversionError(f"Reference to undetermined symbol {obj_name}")
+
+    def build(self) -> None:
+        """
+        Create the project and build the files for the project and app
+
+        Hooks:
+            build_start: Called at the start
+            build_end: Called at the end
+        """
+        plugins.build_start(self)
+
+        self.collect_imports()
+
         self.build_project()
+        plugins.build_project_done(self)
+
+        self.build_settings()
+        plugins.build_settings_done(self)
+
+        self.copy_assets()
+
         self.build_app_models()
+        plugins.build_app_models_done(self)
+
         self.build_app_views()
+        plugins.build_app_views_done(self)
+
+        self.app_has_urls = False
         self.build_app_urls()
+        plugins.build_app_urls_done(self)
+        self.build_urls()
+        plugins.build_urls_done(self)
+
         self.build_app_admin()
+        plugins.build_app_admin_done(self)
+
         self.build_app_unused()
 
+        plugins.build_end(self)
+
+    def collect_imports(self) -> dict[str, str]:
+        """
+        Collect a lookup for imported names
+
+        Values are the import strings - we'll use isort to merge modules later
+        """
+        self.imports = {}
+        for node in self.ast.body:
+            if isinstance(node, ast.Import):
+                for alias in node.names:
+                    self.imports[alias.name] = f"import {alias.name}"
+            elif isinstance(node, ast.ImportFrom):
+                for alias in node.names:
+                    self.imports[alias.name] = f"from {node.module} import {alias.name}"
+
+        plugins.collect_imports(self)
+        return self.imports
+
     def build_project(self) -> None:
+        """
+        Run ``django-admin startproject`` and create the app dir
+        """
         # Copy the env, so we're still working within any venv
         env = os.environ.copy()
         env.pop("DJANGO_SETTINGS_MODULE", None)
         try:
             result = subprocess.run(
                 ["django-admin", "startproject", self.project_name, self.root_path],
                 env=env,
@@ -133,37 +295,37 @@
         except Exception as e:
             raise ConversionError(f"Could not run django-admin: {e}")
 
         if result.returncode != 0:
             raise ConversionError(f"django-admin startproject failed: {result.stderr}")
 
         # Create app dir
-        app_dir = self.root_path / self.project_name / self.app.app_name
+        app_dir = self.app_path
         app_dir.mkdir()
         (app_dir / "__init__.py").touch()
 
-        self.build_settings()
-        self.build_urls()
-        self.copy_assets()
-
     def build_settings(self) -> None:
         """
         Collect settings from the app definition and update the project settings
+
+        Hooks:
+            build_settings: Customise ``project/settings.py`` AST
+            build_settings_done: After ``project/settings.py`` has been written
         """
         resolver = Resolver(self, f"{self.project_name}.settings")
 
         # Collect from app definition and remove nanodjango-specific settings
         app_settings = {}
         for node in self.ast.body:
             # Look for app = Django(..)
             if (
                 isinstance(node, ast.Assign)
                 and any(
                     [
-                        target.id == "app"
+                        target.id == self.app._instance_name
                         for target in node.targets
                         if isinstance(target, ast.Name)
                     ]
                 )
                 and isinstance(node.value, ast.Call)
                 and isinstance(node.value.func, ast.Name)
                 and node.value.func.id == "Django"
@@ -180,15 +342,15 @@
                         ]:
                             continue
                         else:
                             app_settings[name] = keyword.value
                             resolver.add_references(collect_references(keyword.value))
 
         # Load settings file
-        filename = self.root_path / self.project_name / "settings.py"
+        filename = self.project_path / "settings.py"
         settings = import_from_path("nanodjango.convert.tmp_settings", filename)
         settings_src = inspect.getsource(settings)
         settings_ast = ast.parse(settings_src)
 
         # Replace settings
         for node in settings_ast.body:
             if isinstance(node, ast.Assign):
@@ -215,14 +377,17 @@
                                 node.value.elts.append(ast.Constant(value=extra_app))
 
         # Add any extra vars
         for name, value in app_settings.items():
             node = ast.Assign(targets=[ast.Name(id=name, ctx=ast.Store())], value=value)
             settings_ast.body.append(node)
 
+        # Plugin hook
+        resolver, settings_ast = plugins.build_settings(self, resolver, settings_ast)
+
         # Insert any references - usually imports
         ref_src = resolver.gen_src()
         if ref_src:
             imports = set()
             others = set()
 
             for node in ast.parse(ref_src).body:
@@ -248,224 +413,284 @@
                     continue
                 break
             settings_ast.body[index:index] = others
 
         # Save settings
         self.write_file(filename, ast.unparse(settings_ast))
 
-    def build_urls(self) -> None:
-        filename = self.root_path / self.project_name / "urls.py"
-        src = filename.read_text()
-
-        # Add path to app
-        pattern = "urlpatterns = ["
-        if pattern not in src:
-            raise ConversionError("Expected to find urlpatterns in urls.py")
-        src = src.replace(
-            "from django.urls import path",
-            "from django.urls import include, path",
-        ).replace(
-            pattern,
-            f'{pattern}\n    path("", include("{self.project_name}.{self.app.app_name}.urls")),',
-        )
-
-        if "ADMIN_URL" in self.app._settings:
-            pattern = '"admin/"'
-            if pattern not in src:
-                raise ConversionError("Expected to find admin path in urls.py")
-            src = src.replace(pattern, f'"{self.app._settings["ADMIN_URL"]}"')
-
-        self.write_file(filename, src)
-
     def copy_assets(self) -> None:
         """
         Copy static, templates, and migrations into app, and db.sqlite3 if it exists
+
+        Hooks:
+            copy_assets: After the primary assets have been copied
         """
         script_dir = self.app.app_path.parent
 
         db_file = script_dir / self.app._settings.get("SQLITE_DATABASE", "db.sqlite3")
         if db_file.exists():
             shutil.copy(db_file, self.root_path / "db.sqlite3")
 
+        # List of (source, dest)
         dir_names = [
-            "static",
-            "templates",
-            self.app._settings.get("MIGRATIONS_DIR", "migrations"),
+            ("static", "static"),
+            ("templates", "templates"),
+            (self.app._settings.get("MIGRATIONS_DIR", "migrations"), "migrations"),
         ]
-        for dir_name in dir_names:
-            src_dir = script_dir / dir_name
+        for source_name, dest_name in dir_names:
+            src_dir = script_dir / source_name
             if src_dir.exists() and src_dir.is_dir():
                 shutil.copytree(
                     src_dir,
-                    self.root_path / self.project_name / self.app.app_name / dir_name,
+                    self.app_path / dest_name,
                 )
 
-    def collect_imports(self) -> dict[str, str]:
-        """
-        Collect a lookup for imported names
+        plugins.copy_assets(self)
 
-        Values are the import strings - we'll use isort to merge modules later
+    def build_app_models(self) -> None:
         """
-        self.imports = {}
-        for node in self.ast.body:
-            if isinstance(node, ast.Import):
-                for alias in node.names:
-                    self.imports[alias.name] = f"import {alias.name}"
-            elif isinstance(node, ast.ImportFrom):
-                for alias in node.names:
-                    self.imports[alias.name] = f"from {node.module} import {alias.name}"
+        Build ``app/models.py`` and collect models in ``self.models`` (a list of
+        ``AppModel instances).
 
-        return self.imports
-
-    def collect_definition(self, obj_name) -> tuple[str, set[str]]:
-        """
-        Collect a definition of a module top-level scope object
+        Hooks:
+            build_app_models: Modify ``self.models`` or add content to ``app/models.py``
+            build_app_models_done: After ``app/models.py`` has been written
         """
-        if obj_name == "ensure_http_response":
-            # Inject its dependencies
-            self.imports.update(getattr(ensure_http_response, "_dependencies", {}))
-            obj_src = inspect.getsource(ensure_http_response)
-            obj_ast = ast.parse(obj_src)
-            references = collect_references(obj_ast.body[0])
-            return obj_src, references
-
-        if obj_name not in self.module.__dict__:
-            raise ConversionError(f"Reference to unknown symbol {obj_name}")
-        obj = self.module.__dict__[obj_name]
-
-        # Try to build src from the object
-        try:
-            obj_src = inspect.getsource(obj)
-        except TypeError:
-            # Not a class, method, function, or code object
-            pass
-        else:
-            self.used.add(obj_name)
-            obj_ast = ast.parse(obj_src)
-            references = collect_references(obj_ast.body[0])
-            return obj_src, references
-
-        # Look for an assignment
-        for node in self.ast.body:
-            if isinstance(node, ast.Assign):
-                for target in node.targets:
-                    if isinstance(target, ast.Name) and target.id == obj_name:
-                        obj_src = ast.unparse(node).strip()
-                        self.used.add(obj_name)
-                        obj_ast = ast.parse(obj_src)
-                        references = collect_references(obj_ast.body[0])
-                        return obj_src, references
-
-        # TODO: We could have more exhaustive definition collection
-        raise ConversionError(f"Reference to undetermined symbol {obj_name}")
-
-    def build_app_models(self) -> None:
         self.models = []
         resolver = Resolver(self, ".models")
 
         for name, obj in self.module.__dict__.items():
             if inspect.isclass(obj) and issubclass(obj, Model):
                 app_model = AppModel(name, obj)
                 self.models.append(app_model)
                 resolver.add(name, app_model.references)
 
-        if not self.models:
+        resolver, extra_src = plugins.build_app_models(self, resolver, [])
+
+        if not self.models and not extra_src:
             return
 
         self.write_file(
-            self.root_path / self.project_name / self.app.app_name / "models.py",
+            self.app_path / "models.py",
             resolver.gen_src(),
             "\n".join([app_model.src for app_model in self.models]),
+            "\n".join(extra_src),
         )
 
     def build_app_views(self) -> None:
+        """
+        Build ``app/views.py`` and collect views in ``self.views`` (a list of
+        ``AppView`` instances).
+
+        Hooks:
+            build_app_views: Modify ``self.views`` or add content to ``app/views.py``
+            build_app_views_done: After ``app/views.py`` has been written.
+        """
         self.views = []
         resolver = Resolver(self, ".views")
 
-        for pattern, view in self.app._routes.items():
-            app_view = AppView(pattern, view)
+        for pattern, (view, url_config) in self.app._routes.items():
+            if view is None:
+                # An include
+                continue
+            app_view = AppView(view, pattern, url_config)
             self.views.append(app_view)
             resolver.add(view.__name__, app_view.references)
 
-        if not self.views:
+        resolver, extra_src = plugins.build_app_views(self, resolver, [])
+
+        if not self.views and not extra_src:
             return
 
         self.write_file(
-            self.root_path / self.project_name / self.app.app_name / "views.py",
+            self.app_path / "views.py",
             resolver.gen_src(),
             "\n".join([app_view.src for app_view in self.views]),
+            "\n".join(extra_src),
         )
 
     def build_app_urls(self) -> None:
+        """
+        Build ``app/urls.py``
+
+        Hooks:
+            build_app_views: Modify ``self.views`` or add content to ``app/views.py``
+            build_app_views_done: After ``app/views.py`` has been written.
+        """
+        imports = set()
         urls = []
-        for app_view in self.views:
-            urls.append(app_view.make_url())
+        resolver = Resolver(self, ".urls")
 
-        if not urls:
+        app_views = self.views.copy()
+        for pattern, (view, url_config) in self.app._routes.items():
+            if app_views and app_views[0].pattern == pattern:
+                # path(pattern, view)
+                app_view = app_views.pop(0)
+                urls.append(app_view.make_url())
+            else:
+                # path(pattern, include)
+                # Extract the ``include`` reference
+                route_ast = ast.parse(url_config["source"])
+                if (
+                    (body := route_ast.body[0])
+                    and isinstance(body, ast.Expr)
+                    and (call := getattr(body, "value"))
+                    and isinstance(call, ast.Call)
+                    and call.keywords
+                    and (
+                        include_ast := cast(
+                            ast.Attribute,
+                            next(kw for kw in call.keywords if kw.arg == "include"),
+                        )
+                    )
+                ):
+                    # Collect references, in case this is an include(..) call etc.
+                    include_src = ast.unparse(include_ast.value)
+                    references = collect_references(include_ast.value)
+                    urls.append(make_url(pattern, include_src, **url_config))
+                    resolver.add_references(references)
+                else:
+                    raise ConversionError(
+                        f"Could not understand route {url_config['source']}"
+                    )
+            if url_config["re"]:
+                imports.add("re_path")
+            else:
+                imports.add("path")
+
+        resolver, urls, extra_src = plugins.build_app_urls(self, resolver, urls, [])
+
+        if not urls and not extra_src:
             return
 
+        # Register that we found URLs so build_urls() will link to app.urls.urlpatterns
+        self.app_has_urls = True
+
+        views_import = "from . import views"
+        if not self.views:
+            # We've got a urls.py which doesn't have any views - eg a plugin has added
+            # extra_views or given us extra URLs
+            views_import = ""
+
         self.write_file(
-            self.root_path / self.project_name / self.app.app_name / "urls.py",
-            "from django.urls import path",
-            "from . import views",
+            self.app_path / "urls.py",
+            f"from django.urls import {', '.join(imports)}",
+            views_import,
+            resolver.gen_src(),
             "urlpatterns = [",
-            "\n".join([src for src in urls]),
+            "\n".join(urls),
             "]",
+            "\n".join(extra_src),
         )
 
+    def build_urls(self) -> None:
+        """
+        Update ``project/urls.py``
+
+        Hooks:
+            build_urls: Modify source for ``project/urls.py``
+            build_urls_done: After ``project/urls.py`` has been written.
+        """
+        filename = self.project_path / "urls.py"
+        src = filename.read_text()
+
+        # Add path to app
+        pattern = "urlpatterns = ["
+        if pattern not in src:
+            raise ConversionError("Expected to find urlpatterns in urls.py")
+
+        if self.app_has_urls:
+            src = src.replace(
+                "from django.urls import path",
+                "from django.urls import include, path",
+            ).replace(
+                pattern,
+                f'{pattern}\n    path("", include("{self.project_name}.{self.app.app_name}.urls")),',
+            )
+
+        if "ADMIN_URL" in self.app._settings:
+            pattern = '"admin/"'
+            if pattern not in src:
+                raise ConversionError("Expected to find admin path in urls.py")
+            src = src.replace(pattern, f'"{self.app._settings["ADMIN_URL"]}"')
+
+        src = plugins.build_urls(self, src)
+        self.write_file(filename, src)
+
     def build_app_admin(self) -> None:
+        """
+        Write discovered model admin registrations in ``app/admin.py``
+
+        Hooks:
+            build_app_admin: Modify or add content to ``app/admin.py``
+            build_app_admin_done: After ``app/admin.py`` has been written.
+        """
         model_names: list[str] = []
-        admin_srcs: list[str] = []
+        admins: list[str] = []
         resolver = Resolver(self, ".admin")
 
         # Collect @app.admin decorated models
         for app_model in self.models:
             if not app_model.admin_decorator:
                 continue
             model_names.append(app_model.name)
-            admin_srcs.append(app_model.make_model_admin())
+            admins.append(app_model.make_model_admin())
             resolver.add_references(set([app_model.name]))
 
         # TODO: We could collect ModelAdmin. For now lets let it fall into unused
 
+        resolver, admins, extra_src = plugins.build_app_admin(
+            self, resolver, admins, []
+        )
+
         if not model_names:
             return
 
         self.write_file(
-            self.root_path / self.project_name / self.app.app_name / "admin.py",
+            self.app_path / "admin.py",
             "from django.contrib import admin",
             resolver.gen_src(),
-            "\n".join([src for src in admin_srcs]),
+            "\n".join(admins),
+            "\n".join(extra_src),
         )
 
     def build_app_unused(self) -> None:
+        """
+        Write unused code into``app/unused.py``
+
+        Hooks:
+            build_app_unused: Modify or add content to ``app/unused.py``
+        """
         resolver = Resolver(self, ".unused")
 
         # We're not going to worry about unused imports
         self.used.update(self.imports.keys())
 
         # Also going to ignore the app
-        self.used.add("app")
+        self.used.add(self.app._instance_name)
 
         unused = set(self.module.__dict__.keys()) - self.used
         all_src = []
         for obj_name in unused:
             if obj_name.startswith("_"):
                 continue
 
             # Collect the source and objects it references
             obj_src, references = self.collect_definition(obj_name)
             all_src.append(obj_src)
             resolver.add(obj_name, references)
 
-        if not all_src:
+        resolver, extra_src = plugins.build_app_unused(self, resolver, [])
+
+        if not all_src or extra_src:
             return
 
         self.write_file(
-            self.root_path / self.project_name / self.app.app_name / "unused.py",
+            self.app_path / "unused.py",
             "# Definitions that were not used by the nanodjango converter",
             "# These will need to be merged into the rest of the app manually",
             resolver.gen_src(),
-            "\n".join([src for src in all_src]),
+            "\n".join(all_src),
+            "\n".join(extra_src),
         )
 
         print(f"Unused code detected, see {self.app.app_name}/unused.py")
```

### Comparing `nanodjango-0.4.0/nanodjango/convert/objects.py` & `nanodjango-0.5.0/nanodjango/convert/objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import ast
 import inspect
-from typing import Callable, cast
+from typing import Any, Callable, cast
 
 from django.http import HttpResponse
 
 from .utils import (
     applied_ensure_http_response,
     collect_references,
+    get_decorators,
     is_admin_decorator,
     is_view_decorator,
+    make_url,
     obj_to_ast,
     parse_admin_decorator,
 )
 
 
 class ConverterObject:
     def __init__(self, name: str, obj):
@@ -25,21 +27,21 @@
         self.references: set[str] = set()
 
     def remove_decorators(self, filter_fn: Callable) -> list[ast.AST]:
         """
         Remove certain decorators from the object, update self.src and self.ast, and
         return a list of removed decorators.
         """
-        all_decorators = getattr(self.ast, "decorator_list", [])
-        filtered_decorators = []
+        all_decorators = get_decorators(self.ast)
         if not all_decorators:
             return []
 
         self.ast = cast(ast.FunctionDef | ast.ClassDef, self.ast)
         self.ast.decorator_list = []
+        filtered_decorators = []
         for decorator in all_decorators:
             if filter_fn(decorator):
                 filtered_decorators.append(decorator)
             else:
                 self.ast.decorator_list.append(decorator)
         self.src = ast.unparse(self.ast)
 
@@ -47,18 +49,20 @@
 
     def collect_references(self):
         self.references = collect_references(self.ast)
 
 
 class AppView(ConverterObject):
     pattern: str
+    url_config: dict[str, Any]
 
-    def __init__(self, pattern, obj):
+    def __init__(self, obj: Callable, pattern: str, url_config: dict[str, Any]):
         super().__init__(obj.__name__, obj)
         self.pattern = pattern
+        self.url_config = url_config
 
         # Clear all route decorators
         self.remove_decorators(is_view_decorator)
 
         self.fix_return_value()
         self.collect_references()
 
@@ -82,20 +86,19 @@
 
         # We could be returning a string - add the decorator
         self.ast = cast(ast.FunctionDef, self.ast)
         self.ast.decorator_list.append(applied_ensure_http_response)
         self.src = ast.unparse(self.ast)
 
     def make_url(self) -> str:
-        # TODO: We should probably escape self.pattern, but it's an extreme edge case
-        # that doesn't seem worth the effort at the moment. Contributions welcome.
         view_fn = f"views.{self.name}"
         if inspect.isclass(self.obj):
             view_fn = f"{view_fn}.as_view()"
-        return f'    path("{self.pattern}", {view_fn}),'
+
+        return make_url(self.pattern, view_fn, **self.url_config)
 
 
 class AppModel(ConverterObject):
     admin_decorator: ast.AST | None
 
     def __init__(self, name, obj):
         super().__init__(name, obj)
```

### Comparing `nanodjango-0.4.0/nanodjango/convert/reference.py` & `nanodjango-0.5.0/nanodjango/convert/reference.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 class ReferenceVisitor(ast.NodeVisitor):
     """
     Visitor to traverse the AST of a class or function, looking for references to
     objects outside its scope
     """
 
-    # This is likely incomplete. Contributions welcome.
+    # This class is likely incomplete. Contributions welcome.
+
+    #: Set of global names referenced
+    globals_ref: set[str]
 
     def __init__(self):
         self.locals_stack = [set()]
         self.globals_ref = set()
 
     def push_scope(self):
         self.locals_stack.append(self.current_scope.copy())
```

### Comparing `nanodjango-0.4.0/nanodjango/convert/utils.py` & `nanodjango-0.5.0/nanodjango/convert/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,20 +40,25 @@
         raise ValueError(
             f"Object source does not seem to be a single object: {obj_src}"
         )
     obj_ast = obj_ast_module.body[0]
     return obj_ast
 
 
-def collect_references(node: ast.AST):
+def collect_references(node: ast.AST) -> set[str]:
     visitor = ReferenceVisitor()
     visitor.visit(node)
     return visitor.globals_ref
 
 
+def get_decorators(obj_ast: ast.AST) -> list[ast.AST]:
+    all_decorators = getattr(obj_ast, "decorator_list", [])
+    return all_decorators
+
+
 def parse_admin_decorator(obj_ast: ast.AST) -> dict[str, Any]:
     keywords: dict[str, Any] = {}
     if isinstance(obj_ast, ast.Call):
         keywords = {}
 
         for keyword in obj_ast.keywords:
             if not isinstance(keyword.arg, str):
@@ -132,7 +137,20 @@
 def decorated():
     pass
 
 
 applied_ensure_http_response = cast(
     ast.FunctionDef, obj_to_ast(inspect.getsource(decorated))
 ).decorator_list[0]
+
+
+# Generate a line for an url_patterns
+def make_url(pattern, view_fn, re=False, include=None, **url_config):
+    # TODO: We should probably escape self.pattern, but it's an extreme edge case
+    # that doesn't seem worth the effort at the moment. Contributions welcome.
+    if re:
+        path_fn = "re_path"
+        r = "r"
+    else:
+        path_fn = "path"
+        r = ""
+    return f'    {path_fn}({r}"{pattern}", {view_fn}),'
```

### Comparing `nanodjango-0.4.0/nanodjango/django_glue/apps.py` & `nanodjango-0.5.0/nanodjango/django_glue/apps.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.4.0/nanodjango/django_glue/db.py` & `nanodjango-0.5.0/nanodjango/django_glue/db.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.4.0/nanodjango/settings.py` & `nanodjango-0.5.0/nanodjango/settings.py`

 * *Files identical despite different names*

### Comparing `nanodjango-0.4.0/nanodjango.egg-info/PKG-INFO` & `nanodjango-0.5.0/nanodjango.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodjango
-Version: 0.4.0
+Version: 0.5.0
 Summary: Run Django models and views from a single file, and convert it to a full project.
 Author-email: Richard Terry <code@radiac.net>
 Project-URL: Homepage, https://radiac.net/projects/nanodjango/
 Project-URL: Documentation, https://nanodjango.readthedocs.io/en/latest/
 Project-URL: Changelog, https://nanodjango.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/radiac/nanodjango
 Project-URL: Issues, https://github.com/radiac/nanodjango/issues
@@ -27,15 +27,20 @@
 [![Documentation](https://readthedocs.org/projects/nanodjango/badge/?version=latest)](https://nanodjango.readthedocs.io/en/latest/)
 [![Tests](https://github.com/radiac/nanodjango/actions/workflows/ci.yml/badge.svg)](https://github.com/radiac/nanodjango/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/radiac/nanodjango/branch/main/graph/badge.svg?token=BCNM45T6GI)](https://codecov.io/gh/radiac/nanodjango)
 
 Write a Django site in a single file, using views, models and admin, then automatically
 convert it to a full Django project when you're ready for it to grow.
 
-Perfect for experiments, prototypes, tutorials, and small applications.
+An alternative to Flask (see example below) and FastAPI (see our django-ninja example) -
+similar simple syntax, but with full access to Django's features such as the ORM, auth
+and admin site.
+
+Perfect for experiments, prototypes, sharing working code samples, and deploying small
+production applications.
 
 
 ## Quickstart
 
 
 Install nanodjango:
 
@@ -48,33 +53,33 @@
 are:
 
 ```python
 
 from django.db import models
 from nanodjango import Django
 
-app = Django(ADMIN_URL="admin/")
+app = Django()
 
 @app.admin
 class CountLog(models.Model):
     timestamp = models.DateTimeField(auto_now_add=True)
 
 @app.route("/")
 def count(request):
     CountLog.objects.create()
     return f"<p>Number of page loads: {CountLog.objects.count()}</p>"
 ```
 
 Save that as ``counter.py``, then set up your database and run it locally with:
 
 ```sh
-nanodjango counter.py run makemigrations counter
-nanodjango counter.py run migrate
-nanodjango counter.py run createsuperuser
-nanodjango counter.py run
+nanodjango run counter.py makemigrations counter
+nanodjango run counter.py migrate
+nanodjango run counter.py createsuperuser
+nanodjango run counter.py
 ```
 
 It will create your database in a ``db.sqlite3`` file next to your ``counter.py``, with
 the appropriate migrations in ``migrations/``.
 
 Run it in production using WSGI:
 
@@ -102,7 +107,9 @@
 
 For more details, see
 
 * [Getting started](https://nanodjango.readthedocs.io/en/latest/get_started.html)
 * [Tutorial](https://nanodjango.readthedocs.io/en/latest/tutorial.html)
 * [Full Documentation](https://nanodjango.readthedocs.io/en/latest/index.html)
 * [Changelog](https://nanodjango.readthedocs.io/en/latest/changelog.html)
+* [Examples](https://github.com/radiac/nanodjango/tree/main/examples) including how to
+  use nanodjango with Django Ninja
```

### Comparing `nanodjango-0.4.0/nanodjango.egg-info/SOURCES.txt` & `nanodjango-0.5.0/nanodjango.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 nanodjango.egg-info/dependency_links.txt
 nanodjango.egg-info/entry_points.txt
 nanodjango.egg-info/requires.txt
 nanodjango.egg-info/top_level.txt
 nanodjango/convert/__init__.py
 nanodjango/convert/converter.py
 nanodjango/convert/objects.py
+nanodjango/convert/plugin.py
 nanodjango/convert/reference.py
 nanodjango/convert/utils.py
+nanodjango/convert/contrib/__init__.py
+nanodjango/convert/contrib/django_ninja.py
 nanodjango/django_glue/__init__.py
 nanodjango/django_glue/apps.py
 nanodjango/django_glue/db.py
 tests/test_convert.py
 tests/test_run_check.py
 tests/test_run_runserver.py
```

### Comparing `nanodjango-0.4.0/pyproject.toml` & `nanodjango-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nanodjango-0.4.0/tests/test_convert.py` & `nanodjango-0.5.0/tests/test_convert.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 TEST_SCRIPT = f"examples/{TEST_APP}.py"
 TEST_BIND = "127.0.0.1:8042"
 TEST_HTTP = f"http://{TEST_BIND}/"
 TIMEOUT = 10
 
 
 def test_runserver__fbv_with_model(tmp_path):
-    cmd(TEST_SCRIPT, "run", "makemigrations", TEST_APP)
-    cmd(TEST_SCRIPT, "run", "migrate")
-    cmd(TEST_SCRIPT, "convert", str(tmp_path), "--name=converted", "--delete")
+    cmd("run", TEST_SCRIPT, "makemigrations", TEST_APP)
+    cmd("run", TEST_SCRIPT, "migrate")
+    cmd("convert", TEST_SCRIPT, str(tmp_path), "--name=converted", "--delete")
 
     with (
         converted_process(tmp_path, "runserver", TEST_BIND) as handle,
         runserver(handle),
     ):
         response = urllib.request.urlopen(TEST_HTTP, timeout=TIMEOUT)
         assert response.getcode() == 200
```

### Comparing `nanodjango-0.4.0/tests/test_run_runserver.py` & `nanodjango-0.5.0/tests/test_run_runserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 TEST_SCRIPT = f"examples/{TEST_APP}.py"
 TEST_BIND = "127.0.0.1:8042"
 TEST_HTTP = f"http://{TEST_BIND}/"
 TIMEOUT = 10
 
 
 def test_runserver__fbv_with_model():
-    cmd(TEST_SCRIPT, "run", "makemigrations", TEST_APP)
-    cmd(TEST_SCRIPT, "run", "migrate")
+    cmd("run", TEST_SCRIPT, "makemigrations", TEST_APP)
+    cmd("run", TEST_SCRIPT, "migrate")
 
     with (
-        nanodjango_process(TEST_SCRIPT, "run", "runserver", TEST_BIND) as handle,
+        nanodjango_process("run", TEST_SCRIPT, "runserver", TEST_BIND) as handle,
         runserver(handle),
     ):
         response = urllib.request.urlopen(TEST_HTTP, timeout=TIMEOUT)
         assert response.getcode() == 200
         assert "Number of page loads" in response.read().decode("utf-8")
```

