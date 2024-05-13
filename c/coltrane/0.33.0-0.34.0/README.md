# Comparing `tmp/coltrane-0.33.0.tar.gz` & `tmp/coltrane-0.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coltrane-0.33.0.tar", max compression
+gzip compressed data, was "coltrane-0.34.0.tar", max compression
```

## Comparing `coltrane-0.33.0.tar` & `coltrane-0.34.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.33.0/LICENSE
--rw-r--r--   0        0        0     4810 2024-03-01 12:58:35.976688 coltrane-0.33.0/README.md
--rw-r--r--   0        0        0    14167 2024-03-01 12:30:51.464951 coltrane-0.33.0/coltrane/__init__.py
--rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.33.0/coltrane/config/__init__.py
--rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.33.0/coltrane/config/cache.py
--rw-r--r--   0        0        0     2766 2024-03-01 12:33:39.377224 coltrane-0.33.0/coltrane/config/paths.py
--rw-r--r--   0        0        0     2982 2024-03-01 12:33:39.377454 coltrane-0.33.0/coltrane/config/settings.py
--rw-r--r--   0        0        0     4474 2024-03-01 12:56:48.123352 coltrane-0.33.0/coltrane/console.py
--rw-r--r--   0        0        0     1404 2024-01-07 19:55:42.426694 coltrane-0.33.0/coltrane/default-files/Dockerfile
--rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.33.0/coltrane/default-files/README.md
--rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.33.0/coltrane/default-files/app.py
--rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.33.0/coltrane/default-files/env
--rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.33.0/coltrane/default-files/gitignore
--rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.33.0/coltrane/default-files/gunicorn.conf.py
--rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.33.0/coltrane/default-files/watchmanconfig
--rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.33.0/coltrane/feeds.py
--rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.33.0/coltrane/management/__init__.py
--rw-r--r--   0        0        0        0 2022-01-01 20:39:50.444939 coltrane-0.33.0/coltrane/management/commands/__init__.py
--rw-r--r--   0        0        0    10893 2024-02-26 04:37:14.377626 coltrane-0.33.0/coltrane/management/commands/build.py
--rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.33.0/coltrane/manifest.py
--rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.33.0/coltrane/middleware.py
--rw-r--r--   0        0        0    14028 2024-03-01 12:33:39.377952 coltrane-0.33.0/coltrane/renderer.py
--rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.33.0/coltrane/retriever.py
--rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.33.0/coltrane/sitemaps.py
--rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.33.0/coltrane/templates/coltrane/base.html
--rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.33.0/coltrane/templates/coltrane/content.html
--rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.33.0/coltrane/templatetags/__init__.py
--rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.33.0/coltrane/templatetags/coltrane_tags.py
--rw-r--r--   0        0        0     1268 2024-03-01 12:33:39.378176 coltrane-0.33.0/coltrane/urls.py
--rw-r--r--   0        0        0     1740 2023-11-21 02:29:05.209258 coltrane-0.33.0/coltrane/utils.py
--rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.33.0/coltrane/views.py
--rw-r--r--   0        0        0     5226 2024-03-01 13:01:44.678784 coltrane-0.33.0/pyproject.toml
--rw-r--r--   0        0        0     6714 1970-01-01 00:00:00.000000 coltrane-0.33.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.34.0/LICENSE
+-rw-r--r--   0        0        0     4820 2024-05-13 22:55:14.205664 coltrane-0.34.0/README.md
+-rw-r--r--   0        0        0    14047 2024-05-13 22:55:14.205913 coltrane-0.34.0/coltrane/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.34.0/coltrane/config/__init__.py
+-rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.34.0/coltrane/config/cache.py
+-rw-r--r--   0        0        0     2918 2024-05-13 22:55:14.206087 coltrane-0.34.0/coltrane/config/paths.py
+-rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.34.0/coltrane/config/redirects.py
+-rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.34.0/coltrane/config/settings.py
+-rw-r--r--   0        0        0     4474 2024-03-01 13:05:09.414741 coltrane-0.34.0/coltrane/console.py
+-rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.34.0/coltrane/context_processors.py
+-rw-r--r--   0        0        0     1404 2024-01-07 19:55:42.426694 coltrane-0.34.0/coltrane/default-files/Dockerfile
+-rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.34.0/coltrane/default-files/README.md
+-rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.34.0/coltrane/default-files/app.py
+-rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.34.0/coltrane/default-files/env
+-rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.34.0/coltrane/default-files/gitignore
+-rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.34.0/coltrane/default-files/gunicorn.conf.py
+-rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.34.0/coltrane/default-files/watchmanconfig
+-rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.34.0/coltrane/feeds.py
+-rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.34.0/coltrane/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.34.0/coltrane/management/commands/__init__.py
+-rw-r--r--   0        0        0    12040 2024-05-13 22:55:14.206800 coltrane-0.34.0/coltrane/management/commands/build.py
+-rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.34.0/coltrane/manifest.py
+-rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.34.0/coltrane/middleware.py
+-rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.34.0/coltrane/module_finder.py
+-rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.34.0/coltrane/renderer.py
+-rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.34.0/coltrane/retriever.py
+-rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.34.0/coltrane/sitemaps.py
+-rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.34.0/coltrane/templates/coltrane/base.html
+-rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.34.0/coltrane/templates/coltrane/content.html
+-rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.34.0/coltrane/templatetags/__init__.py
+-rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.34.0/coltrane/templatetags/coltrane_tags.py
+-rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.34.0/coltrane/urls.py
+-rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.34.0/coltrane/utils.py
+-rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.34.0/coltrane/views.py
+-rw-r--r--   0        0        0     5360 2024-05-13 22:55:14.210389 coltrane-0.34.0/pyproject.toml
+-rw-r--r--   0        0        0     6799 1970-01-01 00:00:00.000000 coltrane-0.34.0/PKG-INFO
```

### Comparing `coltrane-0.33.0/LICENSE` & `coltrane-0.34.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/README.md` & `coltrane-0.34.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <p align="center">
   <a href="https://coltrane.readthedocs.io"><h1 align="center">coltrane</h1></a>
 </p>
-<p align="center">A Dynamic Site Generator that harnesses the power of Django without the hassle 🎵</p>
+<p align="center">A minimal app framework for content sites 🎵</p>
 
 ![PyPI](https://img.shields.io/pypi/v/coltrane?color=blue&style=flat-square)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/coltrane?color=blue&style=flat-square)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/adamghill?color=blue&style=flat-square)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 ![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
@@ -17,14 +17,15 @@
 ## ⭐ Features
 
 - Render `markdown` files as HTML with automatic URL routing based on the filesystem
 - Use JSON files as data sources in HTML templates or `markdown`
 - Automatic generation of `sitemap.xml` and `rss.xml` files
 - Can serve non-markdown files like `robots.txt`
 - Local development server which includes [live re-rendering of markdown and data](https://twitter.com/adamghill/status/1487522925393715205) via https://github.com/adamchainz/django-browser-reload
+- Site-wide redirects
 - Deployment best practices with `whitenoise` and `gunicorn` already configured
 - Leverage the power of built-in `Django` templates, template tags, and filters inside `markdown` files
 - Any custom template tags and filters are enabled automatically for use in `markdown` or HTML templates
 - Include any third-party [`Django` app](https://djangopackages.org) for additional functionality
 - Optional command to generate static HTML files
 - Able to be integrated into a regular `Django` project as a standard third-party `Django` app
 
@@ -53,14 +54,15 @@
 │   └── index.md
 ├── data
 ├── Dockerfile
 ├── gunicorn.conf.py
 ├── templates
 ├── poetry.lock
 └── pyproject.toml
+└── redirects.json
 ```
 
 ## 📝 Content
 
 Add `markdown` files or sub-directories to the `content` directory and rendered HTML will be accessible via auto-generated routes.
 
 - `/` would render the `markdown` in `content/index.md`
```

#### html2text {}

```diff
@@ -1,57 +1,57 @@
                             _**_**_**_**_**_**_ _cc_oo_ll_tt_rr_aa_nn_ee_ _**_**_**_**_**_**
-A Dynamic Site Generator that harnesses the power of Django without the hassle
-                                     ðµ
+                A minimal app framework for content sites ðµ
 ![PyPI](https://img.shields.io/pypi/v/coltrane?color=blue&style=flat-square) !
 [PyPI - Downloads](https://img.shields.io/pypi/dm/
 coltrane?color=blue&style=flat-square) ![GitHub Sponsors](https://
 img.shields.io/github/sponsors/adamghill?color=blue&style=flat-square) ![All
 Contributors](https://img.shields.io/badge/all_contributors-1-
 orange.svg?style=flat-square) ð Complete documentation at https://
 coltrane.readthedocs.io. ð¦ Package located at https://pypi.org/project/
 coltrane/. ## â­ Features - Render `markdown` files as HTML with automatic URL
 routing based on the filesystem - Use JSON files as data sources in HTML
 templates or `markdown` - Automatic generation of `sitemap.xml` and `rss.xml`
 files - Can serve non-markdown files like `robots.txt` - Local development
 server which includes [live re-rendering of markdown and data](https://
 twitter.com/adamghill/status/1487522925393715205) via https://github.com/
-adamchainz/django-browser-reload - Deployment best practices with `whitenoise`
-and `gunicorn` already configured - Leverage the power of built-in `Django`
-templates, template tags, and filters inside `markdown` files - Any custom
-template tags and filters are enabled automatically for use in `markdown` or
-HTML templates - Include any third-party [`Django` app](https://
-djangopackages.org) for additional functionality - Optional command to generate
-static HTML files - Able to be integrated into a regular `Django` project as a
-standard third-party `Django` app ## â¡ Quick start 1. `mkdir new-site && cd
-new-site` to create a new folder 1. `poetry init --no-interaction --dependency
-'coltrane:<1' && poetry install` to create a new virtual environment and
-install the `coltrane` package 1. Optional: `brew install watchman` on MacOS
-for less resource-intensive local development server 1. `poetry run coltrane
-create` to create the folder structure for a new site 1. `poetry run coltrane
-play` to start local development server 1. Go to http://localhost:8000 to see
-the original markdown rendered into HTML 1. Update `content/index.md` 1. Go to
-http://localhost:8000 to see the updated markdown rendered into HTML 1.
-Optional: run `poetry run coltrane record` to build static HTML files ###
-Generated `coltrane` file structure ```bash . âââ .env âââ
-.gitignore âââ .watchmanconfig âââ __init__.py âââ app.py
-âââ content âÂ Â  âââ index.md âââ data âââ
-Dockerfile âââ gunicorn.conf.py âââ templates âââ poetry.lock
-âââ pyproject.toml ``` ## ð Content Add `markdown` files or sub-
-directories to the `content` directory and rendered HTML will be accessible via
-auto-generated routes. - `/` would render the `markdown` in `content/index.md`
-- `/about/` would render the `markdown` in `content/about.md` - `/articles/
-this-is-the-first-article/` would render the content from `/content/articles/
-this-is-the-first-article.md` - `/not-there/` will 404 HTML will also be served
-automatically if a `markdown` file can not be found. - `/app/` would render the
-HTML from `/templates/app.html` or `/templates/app/index.html` - `/app/some-
-user` would render the HTML from `/templates/app/*.html` ## Deployment Example
-`Dockerfile` and `gunicorn.conf.py` files are created when an app is created,
-and optional dependencies can be installed for efficient `static` serving with
-`whitenoise`. # ð Documentation Read all of the documentation at https://
-coltrane.readthedocs.io. ## Contributors â¨ Thanks goes to these wonderful
-people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+adamchainz/django-browser-reload - Site-wide redirects - Deployment best
+practices with `whitenoise` and `gunicorn` already configured - Leverage the
+power of built-in `Django` templates, template tags, and filters inside
+`markdown` files - Any custom template tags and filters are enabled
+automatically for use in `markdown` or HTML templates - Include any third-party
+[`Django` app](https://djangopackages.org) for additional functionality -
+Optional command to generate static HTML files - Able to be integrated into a
+regular `Django` project as a standard third-party `Django` app ## â¡ Quick
+start 1. `mkdir new-site && cd new-site` to create a new folder 1. `poetry init
+--no-interaction --dependency 'coltrane:<1' && poetry install` to create a new
+virtual environment and install the `coltrane` package 1. Optional: `brew
+install watchman` on MacOS for less resource-intensive local development server
+1. `poetry run coltrane create` to create the folder structure for a new site
+1. `poetry run coltrane play` to start local development server 1. Go to http:/
+/localhost:8000 to see the original markdown rendered into HTML 1. Update
+`content/index.md` 1. Go to http://localhost:8000 to see the updated markdown
+rendered into HTML 1. Optional: run `poetry run coltrane record` to build
+static HTML files ### Generated `coltrane` file structure ```bash . âââ
+.env âââ .gitignore âââ .watchmanconfig âââ __init__.py
+âââ app.py âââ content âÂ Â  âââ index.md âââ data
+âââ Dockerfile âââ gunicorn.conf.py âââ templates âââ
+poetry.lock âââ pyproject.toml âââ redirects.json ``` ## ð
+Content Add `markdown` files or sub-directories to the `content` directory and
+rendered HTML will be accessible via auto-generated routes. - `/` would render
+the `markdown` in `content/index.md` - `/about/` would render the `markdown` in
+`content/about.md` - `/articles/this-is-the-first-article/` would render the
+content from `/content/articles/this-is-the-first-article.md` - `/not-there/
+` will 404 HTML will also be served automatically if a `markdown` file can not
+be found. - `/app/` would render the HTML from `/templates/app.html` or `/
+templates/app/index.html` - `/app/some-user` would render the HTML from `/
+templates/app/*.html` ## Deployment Example `Dockerfile` and `gunicorn.conf.py`
+files are created when an app is created, and optional dependencies can be
+installed for efficient `static` serving with `whitenoise`. # ð
+Documentation Read all of the documentation at https://coltrane.readthedocs.io.
+## Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
 _[_T_o_b_i_ _D_E_G_N_O_N_]
  _TT_oo_bb_ii_ _DD_EE_GG_NN_OO_NN
  _â__ _ï_¸_ _ð___»
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `coltrane-0.33.0/coltrane/__init__.py` & `coltrane-0.34.0/coltrane/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import logging
 import sys
 from copy import deepcopy
-from importlib.util import find_spec
 from os import getenv
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from django import setup as django_setup
 from django.conf import settings
 from django.core.handlers.wsgi import WSGIHandler
 from django.template.library import InvalidTemplateLibrary, import_library
 from dotenv import load_dotenv
 
 from coltrane.config.settings import (
     DEFAULT_COLTRANE_SETTINGS,
 )
+from coltrane.module_finder import (
+    is_django_compressor_installed,
+    is_django_unicorn_installed,
+    is_unicorn_module_available,
+    is_whitenoise_installed,
+)
 from coltrane.utils import dict_merge
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "initialize",
 ]
@@ -128,14 +133,15 @@
             "DIRS": [template_dir],
             "OPTIONS": {
                 "builtins": builtins,
                 "context_processors": [
                     "django.template.context_processors.request",
                     "django.template.context_processors.debug",
                     "django.template.context_processors.static",
+                    "coltrane.context_processors.coltrane",
                 ],
             },
         }
     ]
 
 
 def _merge_installed_apps(django_settings: Dict[str, Any], installed_apps: List[str]) -> List[str]:
@@ -212,40 +218,14 @@
 
     if value_from_env := getenv(env_name):
         env_values = value_from_env.split(",")
 
     return env_values
 
 
-def _is_module_available(module_name: str) -> bool:
-    """
-    Helper function to check if a module is available.
-
-    Could be an installed package or an available module.
-    """
-
-    return find_spec(module_name) is not None
-
-
-def _is_whitenoise_installed() -> bool:
-    """
-    Helper function to check if `whitenoise` is installed.
-    """
-
-    return _is_module_available("whitenoise")
-
-
-def _is_django_unicorn_installed() -> bool:
-    """
-    Helper function to check if `django_unicorn` is installed.
-    """
-
-    return _is_module_available("django_unicorn")
-
-
 def _set_coltrane_setting(settings: Dict, initialize_settings: Dict, setting_name: str) -> Dict:
     """
     Sets a setting on the `COLTRANE` dictionary that is in the environment or passed
     in to `initialize`. Environment takes precedence.
 
     For example:
     - `COLTRANE_TITLE=Awesome Blog 1` in `.env` equals `COLTRANE['TITLE'] = 'Awesome Blog 1'` in settings
@@ -311,26 +291,27 @@
     staticfiles_dirs = [
         base_dir / "static",
     ]
 
     middleware = deepcopy(DEFAULT_MIDDLEWARE)
     installed_apps = deepcopy(DEFAULT_INSTALLED_APPS)
 
-    if _is_django_unicorn_installed():
+    if is_django_unicorn_installed():
         installed_apps.append("django_unicorn")
 
-        if _is_module_available("unicorn"):
+        if is_unicorn_module_available():
             installed_apps.append("unicorn")
 
-    is_whitenoise_installed = _is_whitenoise_installed()
-
-    if is_whitenoise_installed:
+    if is_whitenoise_installed():
         middleware.insert(1, "whitenoise.middleware.WhiteNoiseMiddleware")
         installed_apps.insert(0, "whitenoise.runserver_nostatic")
 
+    if is_django_compressor_installed():
+        installed_apps.append("compressor")
+
     if debug and not is_build_management_command:
         # Add settings required for django-browser-reload when appropriate
         middleware.append("django_browser_reload.middleware.BrowserReloadMiddleware")
         installed_apps.append("django_browser_reload")
 
         # Add content and data to "staticfiles" so django-browser-reload can monitor them
         content_directory = _get_from_env_or_settings(
@@ -377,28 +358,33 @@
         "SETTINGS_MODULE": "coltrane",
     }
 
     # Check for `COLTRANE` settings in env variables or passed into app.initialize()
     for setting_name in DEFAULT_COLTRANE_SETTINGS.keys():
         default_settings = _set_coltrane_setting(default_settings, django_settings, setting_name)
 
-    if is_whitenoise_installed:
+    if is_whitenoise_installed():
         default_settings["WHITENOISE_MANIFEST_STRICT"] = False
         default_settings["STATICFILES_STORAGE"] = "whitenoise.storage.CompressedManifestStaticFilesStorage"
 
+    if is_django_compressor_installed():
+        default_settings["COMPRESS_ENABLED"] = True
+
+        default_settings["STATICFILES_FINDERS"] = (
+            "django.contrib.staticfiles.finders.FileSystemFinder",
+            "django.contrib.staticfiles.finders.AppDirectoriesFinder",
+            "compressor.finders.CompressorFinder",
+        )
+
+        default_settings["TEMPLATES"][0]["OPTIONS"]["builtins"].append("compressor.templatetags.compress")
+
     # Make sure BASE_DIR is a `Path` if it got passed in
     if "BASE_DIR" in django_settings and isinstance(django_settings["BASE_DIR"], str):
         django_settings["BASE_DIR"] = Path(django_settings["BASE_DIR"])
 
-    # Override STATIC_ROOT if the output directory name is manually set
-    try:
-        django_settings["STATIC_ROOT"] = base_dir / django_settings["COLTRANE"]["OUTPUT"]["PATH"] / "static"
-    except KeyError:
-        pass
-
     # Override STATIC_ROOT if the output directory is manually set
     try:
         django_settings["STATIC_ROOT"] = Path(django_settings["COLTRANE"]["OUTPUT"]["DIRECTORY"]) / "static"
     except KeyError:
         pass
 
     django_settings = dict_merge(default_settings, django_settings, destination_overrides_source=True)
```

### Comparing `coltrane-0.33.0/coltrane/config/cache.py` & `coltrane-0.34.0/coltrane/config/cache.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/config/paths.py` & `coltrane-0.34.0/coltrane/config/paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,7 +113,15 @@
 
 def get_output_static_directory() -> Path:
     """
     Get the path of Django's static path.
     """
 
     return Path(settings.STATIC_ROOT)
+
+
+def get_redirects_json() -> Path:
+    """
+    Get the path of of the redirects.json file.
+    """
+
+    return get_base_directory() / "redirects.json"
```

### Comparing `coltrane-0.33.0/coltrane/config/settings.py` & `coltrane-0.34.0/coltrane/config/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from os import getenv
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional
 
 from django.conf import settings
 
 # List of available `mistune` plugins: https://mistune.lepture.com/en/latest/plugins.html
 DEFAULT_MISTUNE_PLUGINS = [
     "strikethrough",
     "footnotes",
```

### Comparing `coltrane-0.33.0/coltrane/console.py` & `coltrane-0.34.0/coltrane/console.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/default-files/Dockerfile` & `coltrane-0.34.0/coltrane/default-files/Dockerfile`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/feeds.py` & `coltrane-0.34.0/coltrane/feeds.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/management/commands/build.py` & `coltrane-0.34.0/coltrane/management/commands/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import sys
 import time
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import Future, ThreadPoolExecutor
+from contextlib import redirect_stdout
 from io import StringIO
 from multiprocessing import cpu_count
 from pathlib import Path
 from shutil import copy2
 from types import SimpleNamespace
 from typing import Dict, List, Optional
 
@@ -21,24 +22,25 @@
     get_extra_file_paths,
     get_output_directory,
     get_output_json,
     get_output_static_directory,
 )
 from coltrane.feeds import ContentFeed
 from coltrane.manifest import Manifest, ManifestItem
+from coltrane.module_finder import is_django_compressor_installed
 from coltrane.renderer import StaticRequest
 from coltrane.retriever import get_content_paths
 from coltrane.urls import sitemaps
 from coltrane.utils import threadpool
 
 logger = logging.getLogger(__name__)
 
 
 class Command(BaseCommand):
-    help = "Build all static HTML files and put them into a directory named output."  # noqa: A003
+    help = "Build all static HTML files and put them into a directory named output."
 
     is_force = False
     threads_count = 2
     manifest = None
     output_result_counts = SimpleNamespace(create_count=0, update_count=0, skip_count=0)
 
     def add_arguments(self, parser):
@@ -116,14 +118,39 @@
         collectstatic_stdout = f"Copy {collectstatic_stdout}"
 
         # TODO: Handle files in output.json that weren't
         # found in content? (--clean option?)
 
         return collectstatic_stdout
 
+    @threadpool
+    def _call_compress(self) -> str:
+        stdout = StringIO()
+        stderr = StringIO()
+
+        # Force DEBUG to always be `False` so that
+        settings.DEBUG = False
+        settings.COMPRESS_OFFLINE = True
+
+        # redirect_stdout is required
+        # https://github.com/django-compressor/django-compressor/blob/develop/compressor/management/commands/compress.py#L385
+        with redirect_stdout(stdout):
+            management.call_command(
+                "compress",
+                verbosity=1,
+                stdout=None,
+                stderr=stderr,
+            )
+
+        compress_stdout = (
+            stdout.getvalue().replace("Compressing... done\n", "").replace("Compressed ", "Compress ")[:-2]
+        )
+
+        return compress_stdout
+
     def _output_markdown_file(self, markdown_file: Path) -> None:
         if not self.manifest:
             raise AssertionError("Manifest must be loaded first")
 
         is_skipped = False
 
         item = ManifestItem.create(markdown_file)
@@ -152,15 +179,15 @@
             self.manifest.add(markdown_file)
 
     def _success(self, text: str, ending="\n") -> None:
         self.stdout.write(LogSymbols.SUCCESS.value, ending=" ")
         self.stdout.write(text, ending=ending)
 
     def _set_output_directory(self, options: Dict) -> None:
-        if "output" in options and options["output"]:
+        if options.get("output"):
             if not hasattr(settings, "COLTRANE"):
                 settings.COLTRANE = {}
 
             if "OUTPUT" not in settings.COLTRANE:
                 settings.COLTRANE["OUTPUT"] = {}
 
             settings.COLTRANE["OUTPUT"]["PATH"] = options["output"]
@@ -192,14 +219,19 @@
 
         spinner = Halo(spinner="dots")
 
         self._set_output_directory(options)
 
         collectstatic_future = self._call_collectstatic()
 
+        compress_future = None
+
+        if is_django_compressor_installed():
+            compress_future = self._call_compress()
+
         self.output_directory = get_output_directory()
         self._success("Use output directory of ", ending="")
         self.stdout.write(self.style.WARNING(str(self.output_directory)))
         self.output_directory.mkdir(exist_ok=True)
 
         spinner.start("Load manifest")
         self.manifest = self._load_manifest()
@@ -210,29 +242,34 @@
             self._success("Force update because ", ending="")
             self.stdout.write(self.style.WARNING("--force"))
 
         spinner.start("Collect static files")
         collectstatic_stdout = collectstatic_future.result()
         spinner.succeed(collectstatic_stdout)
 
+        if compress_future:
+            spinner.start("Compress files")
+            compress_stdout = compress_future.result()
+            spinner.succeed(compress_stdout)
+
         spinner.start("Copy extra files")
         extra_file_count = 0
         for extra_file_path in get_extra_file_paths():
             copy2(extra_file_path, self.output_directory)
             extra_file_count += 1
         spinner.succeed(f"Copy {extra_file_count} extra files")
 
         if not self.is_force and self.manifest.static_files_manifest_changed:
             # At least one static file has changed, so re-render all files because
             # we don't have granularity to know which static files are used in
             # particular markdown or template files
             self.is_force = True
             self._success("Force update because static file(s) updated")
 
-        if "threads" in options and options["threads"]:
+        if options.get("threads"):
             try:
                 self.threads_count = int(options["threads"])
             except ValueError:
                 pass
         else:
             try:
                 self.threads_count = (cpu_count() // 2) - 1
@@ -287,15 +324,15 @@
             spinner.succeed()
 
         elapsed_time = time.time() - start_time
 
         for error_message in self.errors:
             spinner.fail(error_message)
 
-        self.stdout.write()
+        self.stdout.write("")
 
         if self.errors:
             self.stderr.write(self.style.ERROR(f"Static site output completed with errors in {elapsed_time:.4f}s\n"))
 
             if "ignore" not in options or not options["ignore"]:
                 # Call sys.exit explicitly instead of CommandError for nicer error output
                 sys.exit(1)
```

### Comparing `coltrane-0.33.0/coltrane/manifest.py` & `coltrane-0.34.0/coltrane/manifest.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/middleware.py` & `coltrane-0.34.0/coltrane/middleware.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/renderer.py` & `coltrane-0.34.0/coltrane/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         Returns:
             Tuple of template file name (i.e. `coltrane/content.html`) and context
             dictionary.
         """
 
         (html, metadata) = self.get_html_and_markdown(slug)
-        context = {"debug": settings.DEBUG}
+        context = {"debug": settings.DEBUG, "coltrane": settings.COLTRANE}
 
         # Start with any metadata from the markdown frontmatter
         context.update(metadata)
 
         # Add JSON data to the context
         data = get_data()
         context["data"] = data
```

### Comparing `coltrane-0.33.0/coltrane/retriever.py` & `coltrane-0.34.0/coltrane/retriever.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/templatetags/coltrane_tags.py` & `coltrane-0.34.0/coltrane/templatetags/coltrane_tags.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/urls.py` & `coltrane-0.34.0/coltrane/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from django.conf import settings
 from django.contrib.sitemaps.views import sitemap
 from django.urls import include, path, re_path
+from django.views.generic.base import RedirectView
 
 from coltrane import views
+from coltrane.config.redirects import get_redirects
 from coltrane.config.settings import get_extra_file_names
 from coltrane.feeds import ContentFeed
 from coltrane.sitemaps import ContentSitemap
 
 app_name = "coltrane"
 
 sitemaps = {"content": ContentSitemap}
 
 urlpatterns = []
 
+
+for redirect in get_redirects():
+    urlpatterns += [
+        path(redirect.from_url, RedirectView.as_view(url=redirect.to_url, permanent=redirect.permanent)),
+    ]
+
 # Add browser reload URL if not prod
 if settings.DEBUG:
     urlpatterns += [
         path("__reload__/", include("django_browser_reload.urls")),
     ]
 
 # Add sitemap and RSS URLs
```

### Comparing `coltrane-0.33.0/coltrane/utils.py` & `coltrane-0.34.0/coltrane/utils.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/coltrane/views.py` & `coltrane-0.34.0/coltrane/views.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.33.0/pyproject.toml` & `coltrane-0.34.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "coltrane"
 authors = [{name = "Adam Hill", email = "adam@adamghill.com"}]
 dynamic = ["version", "description"]
 
 [tool.poetry]
 name = "coltrane"
-version = "0.33.0"
+version = "0.34.0"
 description = "A minimal app framework for content sites 🎵"
 authors = ["adamghill <adam@adamghill.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "python", "static", "markdown"]
 packages = [{ include = "coltrane" }]
 repository = "https://github.com/adamghill/coltrane/"
@@ -19,34 +19,38 @@
 [tool.poetry.urls]
 "Funding" = "https://github.com/sponsors/adamghill"
 
 [tool.poetry.scripts]
 coltrane = "coltrane.console:cli"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<4.0"
 Django = ">3.0"
 python-dotenv = ">0.17"
 click = "^8"
 dateparser = "^1"
 mistune = "^3"
 python-frontmatter = "^1"
 pygments = ">=2.7.3"
 minestrone = ">=0.6.2"
 halo = "^0"
 rich-click = "^1"
 django-fastdev = "^1"
 django-browser-reload = "^1"
 pywatchman = "*"
+msgspec = "^0"
 click-aliases = "^1"
 
 # deploy extras
 gunicorn = { version = "*", optional = true }
 whitenoise = { version = "*", optional = true }
 
+# django-compressor extras
+django-compressor = { version = "^4", optional = true }
+
 # JSON5 extras
 pyjson5 = { version = "*", optional = true }
 
 # docs extras
 Sphinx = { version = "*", optional = true }
 linkify-it-py = { version = "*", optional = true }
 myst-parser = { version = "*", optional = true }
@@ -55,14 +59,15 @@
 sphinx-autobuild = { version = "*", optional = true }
 toml = { version = "*", optional = true }
 attrs = { version = "*", optional = true }
 
 [tool.poetry.extras]
 deploy = ["gunicorn", "whitenoise"]
 json5 = ["pyjson5"]
+compressor = ["django-compressor"]
 docs = ["Sphinx", "linkify-it-py", "myst-parser", "furo", "sphinx-copybutton", "sphinx-autobuild", "toml", "attrs"]
 
 [tool.poetry.group.development.dependencies]
 poethepoet = "*"
 ruff = "*"
 coverage = {extras = ["toml"], version = "*"}
 pytest-cov = "*"
```

### Comparing `coltrane-0.33.0/PKG-INFO` & `coltrane-0.34.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: coltrane
-Version: 0.33.0
+Version: 0.34.0
 Summary: A minimal app framework for content sites 🎵
 Home-page: https://github.com/adamghill/coltrane/
 License: MIT
 Keywords: django,python,static,markdown
 Author: adamghill
 Author-email: adam@adamghill.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: compressor
 Provides-Extra: deploy
 Provides-Extra: docs
 Provides-Extra: json5
 Requires-Dist: Django (>3.0)
 Requires-Dist: Sphinx ; extra == "docs"
 Requires-Dist: attrs ; extra == "docs"
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-aliases (>=1,<2)
 Requires-Dist: dateparser (>=1,<2)
 Requires-Dist: django-browser-reload (>=1,<2)
+Requires-Dist: django-compressor (>=4,<5) ; extra == "compressor"
 Requires-Dist: django-fastdev (>=1,<2)
 Requires-Dist: furo ; extra == "docs"
 Requires-Dist: gunicorn ; extra == "deploy"
 Requires-Dist: halo (>=0,<1)
 Requires-Dist: linkify-it-py ; extra == "docs"
 Requires-Dist: minestrone (>=0.6.2)
 Requires-Dist: mistune (>=3,<4)
+Requires-Dist: msgspec (>=0,<1)
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: pygments (>=2.7.3)
 Requires-Dist: pyjson5 ; extra == "json5"
 Requires-Dist: python-dotenv (>0.17)
 Requires-Dist: python-frontmatter (>=1,<2)
 Requires-Dist: pywatchman
 Requires-Dist: rich-click (>=1,<2)
@@ -47,15 +49,15 @@
 Project-URL: Funding, https://github.com/sponsors/adamghill
 Project-URL: Repository, https://github.com/adamghill/coltrane/
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://coltrane.readthedocs.io"><h1 align="center">coltrane</h1></a>
 </p>
-<p align="center">A Dynamic Site Generator that harnesses the power of Django without the hassle 🎵</p>
+<p align="center">A minimal app framework for content sites 🎵</p>
 
 ![PyPI](https://img.shields.io/pypi/v/coltrane?color=blue&style=flat-square)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/coltrane?color=blue&style=flat-square)
 ![GitHub Sponsors](https://img.shields.io/github/sponsors/adamghill?color=blue&style=flat-square)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 ![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
@@ -67,14 +69,15 @@
 ## ⭐ Features
 
 - Render `markdown` files as HTML with automatic URL routing based on the filesystem
 - Use JSON files as data sources in HTML templates or `markdown`
 - Automatic generation of `sitemap.xml` and `rss.xml` files
 - Can serve non-markdown files like `robots.txt`
 - Local development server which includes [live re-rendering of markdown and data](https://twitter.com/adamghill/status/1487522925393715205) via https://github.com/adamchainz/django-browser-reload
+- Site-wide redirects
 - Deployment best practices with `whitenoise` and `gunicorn` already configured
 - Leverage the power of built-in `Django` templates, template tags, and filters inside `markdown` files
 - Any custom template tags and filters are enabled automatically for use in `markdown` or HTML templates
 - Include any third-party [`Django` app](https://djangopackages.org) for additional functionality
 - Optional command to generate static HTML files
 - Able to be integrated into a regular `Django` project as a standard third-party `Django` app
 
@@ -103,14 +106,15 @@
 │   └── index.md
 ├── data
 ├── Dockerfile
 ├── gunicorn.conf.py
 ├── templates
 ├── poetry.lock
 └── pyproject.toml
+└── redirects.json
 ```
 
 ## 📝 Content
 
 Add `markdown` files or sub-directories to the `content` directory and rendered HTML will be accessible via auto-generated routes.
 
 - `/` would render the `markdown` in `content/index.md`
```

#### html2text {}

```diff
@@ -1,83 +1,84 @@
-Metadata-Version: 2.1 Name: coltrane Version: 0.33.0 Summary: A minimal app
+Metadata-Version: 2.1 Name: coltrane Version: 0.34.0 Summary: A minimal app
 framework for content sites ðµ Home-page: https://github.com/adamghill/
 coltrane/ License: MIT Keywords: django,python,static,markdown Author:
-adamghill Author-email: adam@adamghill.com Requires-Python: >=3.7,<4.0
+adamghill Author-email: adam@adamghill.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Provides-Extra: deploy
-Provides-Extra: docs Provides-Extra: json5 Requires-Dist: Django (>3.0)
-Requires-Dist: Sphinx ; extra == "docs" Requires-Dist: attrs ; extra == "docs"
-Requires-Dist: click (>=8,<9) Requires-Dist: click-aliases (>=1,<2) Requires-
-Dist: dateparser (>=1,<2) Requires-Dist: django-browser-reload (>=1,<2)
-Requires-Dist: django-fastdev (>=1,<2) Requires-Dist: furo ; extra == "docs"
-Requires-Dist: gunicorn ; extra == "deploy" Requires-Dist: halo (>=0,<1)
-Requires-Dist: linkify-it-py ; extra == "docs" Requires-Dist: minestrone
-(>=0.6.2) Requires-Dist: mistune (>=3,<4) Requires-Dist: myst-parser ; extra ==
-"docs" Requires-Dist: pygments (>=2.7.3) Requires-Dist: pyjson5 ; extra ==
-"json5" Requires-Dist: python-dotenv (>0.17) Requires-Dist: python-frontmatter
-(>=1,<2) Requires-Dist: pywatchman Requires-Dist: rich-click (>=1,<2) Requires-
-Dist: sphinx-autobuild ; extra == "docs" Requires-Dist: sphinx-copybutton ;
-extra == "docs" Requires-Dist: toml ; extra == "docs" Requires-Dist: whitenoise
-; extra == "deploy" Project-URL: Documentation, https://
-coltrane.readthedocs.io/ Project-URL: Funding, https://github.com/sponsors/
-adamghill Project-URL: Repository, https://github.com/adamghill/coltrane/
-Description-Content-Type: text/markdown
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: compressor Provides-Extra: deploy Provides-Extra: docs
+Provides-Extra: json5 Requires-Dist: Django (>3.0) Requires-Dist: Sphinx ;
+extra == "docs" Requires-Dist: attrs ; extra == "docs" Requires-Dist: click
+(>=8,<9) Requires-Dist: click-aliases (>=1,<2) Requires-Dist: dateparser
+(>=1,<2) Requires-Dist: django-browser-reload (>=1,<2) Requires-Dist: django-
+compressor (>=4,<5) ; extra == "compressor" Requires-Dist: django-fastdev
+(>=1,<2) Requires-Dist: furo ; extra == "docs" Requires-Dist: gunicorn ; extra
+== "deploy" Requires-Dist: halo (>=0,<1) Requires-Dist: linkify-it-py ; extra
+== "docs" Requires-Dist: minestrone (>=0.6.2) Requires-Dist: mistune (>=3,<4)
+Requires-Dist: msgspec (>=0,<1) Requires-Dist: myst-parser ; extra == "docs"
+Requires-Dist: pygments (>=2.7.3) Requires-Dist: pyjson5 ; extra == "json5"
+Requires-Dist: python-dotenv (>0.17) Requires-Dist: python-frontmatter (>=1,<2)
+Requires-Dist: pywatchman Requires-Dist: rich-click (>=1,<2) Requires-Dist:
+sphinx-autobuild ; extra == "docs" Requires-Dist: sphinx-copybutton ; extra ==
+"docs" Requires-Dist: toml ; extra == "docs" Requires-Dist: whitenoise ; extra
+== "deploy" Project-URL: Documentation, https://coltrane.readthedocs.io/
+Project-URL: Funding, https://github.com/sponsors/adamghill Project-URL:
+Repository, https://github.com/adamghill/coltrane/ Description-Content-Type:
+text/markdown
                             _**_**_**_**_**_**_ _cc_oo_ll_tt_rr_aa_nn_ee_ _**_**_**_**_**_**
-A Dynamic Site Generator that harnesses the power of Django without the hassle
-                                     ðµ
+                A minimal app framework for content sites ðµ
 ![PyPI](https://img.shields.io/pypi/v/coltrane?color=blue&style=flat-square) !
 [PyPI - Downloads](https://img.shields.io/pypi/dm/
 coltrane?color=blue&style=flat-square) ![GitHub Sponsors](https://
 img.shields.io/github/sponsors/adamghill?color=blue&style=flat-square) ![All
 Contributors](https://img.shields.io/badge/all_contributors-1-
 orange.svg?style=flat-square) ð Complete documentation at https://
 coltrane.readthedocs.io. ð¦ Package located at https://pypi.org/project/
 coltrane/. ## â­ Features - Render `markdown` files as HTML with automatic URL
 routing based on the filesystem - Use JSON files as data sources in HTML
 templates or `markdown` - Automatic generation of `sitemap.xml` and `rss.xml`
 files - Can serve non-markdown files like `robots.txt` - Local development
 server which includes [live re-rendering of markdown and data](https://
 twitter.com/adamghill/status/1487522925393715205) via https://github.com/
-adamchainz/django-browser-reload - Deployment best practices with `whitenoise`
-and `gunicorn` already configured - Leverage the power of built-in `Django`
-templates, template tags, and filters inside `markdown` files - Any custom
-template tags and filters are enabled automatically for use in `markdown` or
-HTML templates - Include any third-party [`Django` app](https://
-djangopackages.org) for additional functionality - Optional command to generate
-static HTML files - Able to be integrated into a regular `Django` project as a
-standard third-party `Django` app ## â¡ Quick start 1. `mkdir new-site && cd
-new-site` to create a new folder 1. `poetry init --no-interaction --dependency
-'coltrane:<1' && poetry install` to create a new virtual environment and
-install the `coltrane` package 1. Optional: `brew install watchman` on MacOS
-for less resource-intensive local development server 1. `poetry run coltrane
-create` to create the folder structure for a new site 1. `poetry run coltrane
-play` to start local development server 1. Go to http://localhost:8000 to see
-the original markdown rendered into HTML 1. Update `content/index.md` 1. Go to
-http://localhost:8000 to see the updated markdown rendered into HTML 1.
-Optional: run `poetry run coltrane record` to build static HTML files ###
-Generated `coltrane` file structure ```bash . âââ .env âââ
-.gitignore âââ .watchmanconfig âââ __init__.py âââ app.py
-âââ content âÂ Â  âââ index.md âââ data âââ
-Dockerfile âââ gunicorn.conf.py âââ templates âââ poetry.lock
-âââ pyproject.toml ``` ## ð Content Add `markdown` files or sub-
-directories to the `content` directory and rendered HTML will be accessible via
-auto-generated routes. - `/` would render the `markdown` in `content/index.md`
-- `/about/` would render the `markdown` in `content/about.md` - `/articles/
-this-is-the-first-article/` would render the content from `/content/articles/
-this-is-the-first-article.md` - `/not-there/` will 404 HTML will also be served
-automatically if a `markdown` file can not be found. - `/app/` would render the
-HTML from `/templates/app.html` or `/templates/app/index.html` - `/app/some-
-user` would render the HTML from `/templates/app/*.html` ## Deployment Example
-`Dockerfile` and `gunicorn.conf.py` files are created when an app is created,
-and optional dependencies can be installed for efficient `static` serving with
-`whitenoise`. # ð Documentation Read all of the documentation at https://
-coltrane.readthedocs.io. ## Contributors â¨ Thanks goes to these wonderful
-people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+adamchainz/django-browser-reload - Site-wide redirects - Deployment best
+practices with `whitenoise` and `gunicorn` already configured - Leverage the
+power of built-in `Django` templates, template tags, and filters inside
+`markdown` files - Any custom template tags and filters are enabled
+automatically for use in `markdown` or HTML templates - Include any third-party
+[`Django` app](https://djangopackages.org) for additional functionality -
+Optional command to generate static HTML files - Able to be integrated into a
+regular `Django` project as a standard third-party `Django` app ## â¡ Quick
+start 1. `mkdir new-site && cd new-site` to create a new folder 1. `poetry init
+--no-interaction --dependency 'coltrane:<1' && poetry install` to create a new
+virtual environment and install the `coltrane` package 1. Optional: `brew
+install watchman` on MacOS for less resource-intensive local development server
+1. `poetry run coltrane create` to create the folder structure for a new site
+1. `poetry run coltrane play` to start local development server 1. Go to http:/
+/localhost:8000 to see the original markdown rendered into HTML 1. Update
+`content/index.md` 1. Go to http://localhost:8000 to see the updated markdown
+rendered into HTML 1. Optional: run `poetry run coltrane record` to build
+static HTML files ### Generated `coltrane` file structure ```bash . âââ
+.env âââ .gitignore âââ .watchmanconfig âââ __init__.py
+âââ app.py âââ content âÂ Â  âââ index.md âââ data
+âââ Dockerfile âââ gunicorn.conf.py âââ templates âââ
+poetry.lock âââ pyproject.toml âââ redirects.json ``` ## ð
+Content Add `markdown` files or sub-directories to the `content` directory and
+rendered HTML will be accessible via auto-generated routes. - `/` would render
+the `markdown` in `content/index.md` - `/about/` would render the `markdown` in
+`content/about.md` - `/articles/this-is-the-first-article/` would render the
+content from `/content/articles/this-is-the-first-article.md` - `/not-there/
+` will 404 HTML will also be served automatically if a `markdown` file can not
+be found. - `/app/` would render the HTML from `/templates/app.html` or `/
+templates/app/index.html` - `/app/some-user` would render the HTML from `/
+templates/app/*.html` ## Deployment Example `Dockerfile` and `gunicorn.conf.py`
+files are created when an app is created, and optional dependencies can be
+installed for efficient `static` serving with `whitenoise`. # ð
+Documentation Read all of the documentation at https://coltrane.readthedocs.io.
+## Contributors â¨ Thanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):
 _[_T_o_b_i_ _D_E_G_N_O_N_]
  _TT_oo_bb_ii_ _DD_EE_GG_NN_OO_NN
  _â__ _ï_¸_ _ð___»
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

