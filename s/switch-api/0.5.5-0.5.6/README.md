# Comparing `tmp/switch_api-0.5.5.tar.gz` & `tmp/switch_api-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_api-0.5.5.tar", last modified: Thu May  9 03:27:36 2024, max compression
+gzip compressed data, was "switch_api-0.5.6.tar", last modified: Tue May 14 03:33:57 2024, max compression
```

## Comparing `switch_api-0.5.5.tar` & `switch_api-0.5.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.718298 switch_api-0.5.5/
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-09 03:27:25.000000 switch_api-0.5.5/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    36391 2024-05-09 03:27:25.000000 switch_api-0.5.5/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-05-09 03:27:25.000000 switch_api-0.5.5/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-05-09 03:27:25.000000 switch_api-0.5.5/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    37665 2024-05-09 03:27:36.718298 switch_api-0.5.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-05-09 03:27:25.000000 switch_api-0.5.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-05-09 03:27:25.000000 switch_api-0.5.5/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-09 03:27:36.718298 switch_api-0.5.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1448 2024-05-09 03:27:25.000000 switch_api-0.5.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.710297 switch_api-0.5.5/switch_api/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.710297 switch_api-0.5.5/switch_api/_authentication/
--rw-r--r--   0 vsts      (1001) docker     (127)      391 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_authentication/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8127 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_authentication/_authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/_authentication/_credentials_store/
--rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_authentication/_credentials_store/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5851 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_authentication/_credentials_store/_credentials_store.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/_authentication/_msal/
--rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_authentication/_msal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8752 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_authentication/_msal/_custom_application.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/_guide/
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_guide/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3108 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_guide/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2093 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_guide/processor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4199 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5952 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_utils/_marketplace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14920 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_utils/_platform.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23502 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/_utils/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/analytics/
--rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/analytics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14655 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/analytics/analytics.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/cache/
--rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6985 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/controls/
--rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/controls/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      803 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/controls/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11630 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/controls/_mqtt.py
--rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/controls/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13320 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/controls/controls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8458 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/controls/mqtt.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/dataset/
--rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/dataset/dataset.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.714298 switch_api-0.5.5/switch_api/email/
--rw-r--r--   0 vsts      (1001) docker     (127)      472 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/email/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/email/email_sender.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.718298 switch_api-0.5.5/switch_api/error_handlers/
--rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/error_handlers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15754 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/error_handlers/error_handlers.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.718298 switch_api-0.5.5/switch_api/extensions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7519 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/extensions/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1652 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/extensions/field_meta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2970 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/extensions/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1406 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/extensions/pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/initialize.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.718298 switch_api-0.5.5/switch_api/integration/
--rw-r--r--   0 vsts      (1001) docker     (127)     1872 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12939 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/integration/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36653 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/integration/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)   117136 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/integration/integration.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.718298 switch_api-0.5.5/switch_api/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    88340 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/pipeline/automation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35931 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/pipeline/definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29571 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/pipeline/pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.718298 switch_api-0.5.5/switch_api/platform_insights/
--rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/platform_insights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2214 2024-05-09 03:27:25.000000 switch_api-0.5.5/switch_api/platform_insights/platform_insights.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 03:27:36.710297 switch_api-0.5.5/switch_api.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    37665 2024-05-09 03:27:36.000000 switch_api-0.5.5/switch_api.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1909 2024-05-09 03:27:36.000000 switch_api-0.5.5/switch_api.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 03:27:36.000000 switch_api-0.5.5/switch_api.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-05-09 03:27:36.000000 switch_api-0.5.5/switch_api.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-09 03:27:36.000000 switch_api-0.5.5/switch_api.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/
+-rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-14 03:33:49.000000 switch_api-0.5.6/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    36804 2024-05-14 03:33:49.000000 switch_api-0.5.6/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-05-14 03:33:49.000000 switch_api-0.5.6/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-05-14 03:33:49.000000 switch_api-0.5.6/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    38078 2024-05-14 03:33:57.927328 switch_api-0.5.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-05-14 03:33:49.000000 switch_api-0.5.6/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-05-14 03:33:49.000000 switch_api-0.5.6/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-14 03:33:57.931328 switch_api-0.5.6/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1448 2024-05-14 03:33:49.000000 switch_api-0.5.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_authentication/
+-rw-r--r--   0 vsts      (1001) docker     (127)      391 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8127 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_authentication/_credentials_store/
+-rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_credentials_store/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5851 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_credentials_store/_credentials_store.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_authentication/_msal/
+-rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_msal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8752 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_authentication/_msal/_custom_application.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api/_guide/
+-rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_guide/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3108 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_guide/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2093 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_guide/processor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4205 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5952 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_marketplace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14920 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_platform.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23502 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/_utils/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/analytics/
+-rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/analytics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14655 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/analytics/analytics.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/cache/
+-rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6985 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/controls/
+-rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      803 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11630 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/_mqtt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      325 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13320 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/controls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8458 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/controls/mqtt.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/dataset/dataset.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/email/
+-rw-r--r--   0 vsts      (1001) docker     (127)      472 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/email/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/email/email_sender.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/error_handlers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/error_handlers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15754 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/error_handlers/error_handlers.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7519 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1652 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/field_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2970 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1406 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/extensions/pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/initialize.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/integration/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1872 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12939 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36653 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   117136 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/integration/integration.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    88414 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/automation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35931 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30536 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/pipeline/pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.927328 switch_api-0.5.6/switch_api/platform_insights/
+-rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/platform_insights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2214 2024-05-14 03:33:49.000000 switch_api-0.5.6/switch_api/platform_insights/platform_insights.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 03:33:57.923328 switch_api-0.5.6/switch_api.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    38078 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1909 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-14 03:33:57.000000 switch_api-0.5.6/switch_api.egg-info/top_level.txt
```

### Comparing `switch_api-0.5.5/HISTORY.md` & `switch_api-0.5.6/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # History
 
+## 0.5.5
+### Added
+In the `pipeline` module: 
+- Added a new task `IQTask`
+  - Additional abstract property `module_type` that accepts strings. This should define the type of IQ module. 
+  - Abstract method `process` must be instantiated for the task to be registered. 
+  
+### Modified
+In the `pipeline` module: 
+- Updated the `Automation.register_task()` method to accept tasks that subclass the new `IQTask`.  
+
 ## 0.5.4
 
 ### Added
 
 In the `integration` module:
 
 - Added new function `upsert_reservations()`
```

### Comparing `switch_api-0.5.5/LICENCE` & `switch_api-0.5.6/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/PKG-INFO` & `switch_api-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_api
-Version: 0.5.5
+Version: 0.5.6
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,25 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.5.5
+### Added
+In the `pipeline` module: 
+- Added a new task `IQTask`
+  - Additional abstract property `module_type` that accepts strings. This should define the type of IQ module. 
+  - Abstract method `process` must be instantiated for the task to be registered. 
+  
+### Modified
+In the `pipeline` module: 
+- Updated the `Automation.register_task()` method to accept tasks that subclass the new `IQTask`.  
+
 ## 0.5.4
 
 ### Added
 
 In the `integration` module:
 
 - Added new function `upsert_reservations()`
```

### Comparing `switch_api-0.5.5/README.md` & `switch_api-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/setup.py` & `switch_api-0.5.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author="Switch Automation Pty Ltd.",
     description="A complete package for data ingestion into the Switch Automation Platform.",
     long_description=open('README.md', 'r').read() +
     '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_api",
-    version="0.5.5",
+    version="0.5.6",
     packages=find_packages(include=["switch_api", "switch_api.*"]),
     install_requires=['pandas', 'requests', 'azure-storage-blob', 'pandera[io]==0.7.1', 'azure-servicebus',
                       'msal>=1.11.0', 'paho-mqtt==1.6.1', 'uvicorn==0.22.0', 'fastapi==0.98.0', 'pyodbc==4.0.39'],
     python_requires=">=3.8.0",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
```

### Comparing `switch_api-0.5.5/switch_api/__init__.py` & `switch_api-0.5.6/switch_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 # _ch.setLevel(logging.INFO)  # sets the handler info
 # _ch.setFormatter(logging.Formatter(INFOFORMATTER))  # sets the handler formatting
 #
 # # adds the handler to the global variable: log
 # log.addHandler(_ch)
 # https://dev.to/joaomcteixeira/setting-up-python-logging-for-a-library-app-6ml
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
```

### Comparing `switch_api-0.5.5/switch_api/_authentication/_authentication.py` & `switch_api-0.5.6/switch_api/_authentication/_authentication.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/_authentication/_credentials_store/_credentials_store.py` & `switch_api-0.5.6/switch_api/_authentication/_credentials_store/_credentials_store.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/_authentication/_msal/_custom_application.py` & `switch_api-0.5.6/switch_api/_authentication/_msal/_custom_application.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/_guide/main.py` & `switch_api-0.5.6/switch_api/_guide/main.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/_guide/processor.py` & `switch_api-0.5.6/switch_api/_guide/processor.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/_utils/_constants.py` & `switch_api-0.5.6/switch_api/_utils/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 RESPONSE_TYPE = Literal['dataframe', 'json', 'string']
 
 ERROR_TYPE = Literal['DateTime', 'MissingDevices', 'NonNumeric', 'MissingRequiredField(s)', 'MissingSite(s)',
                      'DuplicateRecords', 'MissingSensors', 'UnableToReadFile', 'InvalidFileType', 'InvalidInputSettings']
 
 PROCESS_STATUS = Literal['ActionRequired', 'Failed']
 
-MAPPING_ENTITIES = Literal['Installations', 'Devices/Sensors', 'Readings', 'Work Orders']
+MAPPING_ENTITIES = Literal['Installations', 'Devices/Sensors', 'Readings', 'Work Orders', 'IQ']
 
 WORK_ORDER_CATEGORY = Literal['Preventative Maintenance', 'Tenant Request']
 
 WORK_ORDER_PRIORITY = Literal['Low', 'Medium', 'High']
 
 WORK_ORDER_STATUS = Literal['Submitted', 'Open', 'In Progress', 'Waiting for 3rd Party', 'Resolved', 'Abandoned',
                             'Closed']
```

### Comparing `switch_api-0.5.5/switch_api/_utils/_marketplace.py` & `switch_api-0.5.6/switch_api/_utils/_marketplace.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/_utils/_platform.py` & `switch_api-0.5.6/switch_api/_utils/_platform.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/_utils/_utils.py` & `switch_api-0.5.6/switch_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/analytics/__init__.py` & `switch_api-0.5.6/switch_api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/analytics/analytics.py` & `switch_api-0.5.6/switch_api/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/cache/cache.py` & `switch_api-0.5.6/switch_api/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/controls/_constants.py` & `switch_api-0.5.6/switch_api/controls/_constants.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/controls/_mqtt.py` & `switch_api-0.5.6/switch_api/controls/_mqtt.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/controls/controls.py` & `switch_api-0.5.6/switch_api/controls/controls.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/controls/mqtt.py` & `switch_api-0.5.6/switch_api/controls/mqtt.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/dataset/__init__.py` & `switch_api-0.5.6/switch_api/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/dataset/dataset.py` & `switch_api-0.5.6/switch_api/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/email/email_sender.py` & `switch_api-0.5.6/switch_api/email/email_sender.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/error_handlers/__init__.py` & `switch_api-0.5.6/switch_api/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/error_handlers/error_handlers.py` & `switch_api-0.5.6/switch_api/error_handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/extensions/__init__.py` & `switch_api-0.5.6/switch_api/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/extensions/extensions.py` & `switch_api-0.5.6/switch_api/extensions/extensions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/extensions/field_meta.py` & `switch_api-0.5.6/switch_api/extensions/field_meta.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/extensions/helpers.py` & `switch_api-0.5.6/switch_api/extensions/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/extensions/pipeline.py` & `switch_api-0.5.6/switch_api/extensions/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/initialize.py` & `switch_api-0.5.6/switch_api/initialize.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/integration/__init__.py` & `switch_api-0.5.6/switch_api/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/integration/_utils.py` & `switch_api-0.5.6/switch_api/integration/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/integration/helpers.py` & `switch_api-0.5.6/switch_api/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/integration/integration.py` & `switch_api-0.5.6/switch_api/integration/integration.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/pipeline/__init__.py` & `switch_api-0.5.6/switch_api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/pipeline/automation.py` & `switch_api-0.5.6/switch_api/pipeline/automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,26 +156,27 @@
 
         df = pandas.read_json(response.text, typ="Series")
 
         return df
 
     @staticmethod
     def register_task(api_inputs: ApiInputs, task: Union[Task, IntegrationTask, DiscoverableIntegrationTask, QueueTask,
-                                                         AnalyticsTask, LogicModuleTask, EventWorkOrderTask, ExtensionTask]):
+                                                         AnalyticsTask, LogicModuleTask, EventWorkOrderTask, IQTask,
+                                                         ExtensionTask]):
         """Register the task.
 
         Registers the task that was defined.
 
         Parameters
         ----------
         api_inputs : ApiInputs
             Object returned by initialize() function.
         task : Union[Task, IntegrationTask, DiscoverableIntegrationTask, QueueTask, AnalyticsTask, LogicModuleTask, EventWorkOrderTask]
             An instance of the custom class created from the Abstract Base Class `Task` or its abstract sub-classes:
-            `IntegrationTask`,`DiscoverableIntegrationTask`, `AnalyticsTask`, `QueueTask`, `EventWorkOrderTask`, 
+            `IntegrationTask`,`DiscoverableIntegrationTask`, `AnalyticsTask`, `QueueTask`, `EventWorkOrderTask`, `IQTask`,
             `LogicModuleTask`, or `ExtensionTask`.
 
         Returns
         -------
         pandas.DataFrame
 
         """
```

### Comparing `switch_api-0.5.5/switch_api/pipeline/definitions.py` & `switch_api-0.5.6/switch_api/pipeline/definitions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/pipeline/pipeline.py` & `switch_api-0.5.6/switch_api/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -736,14 +736,49 @@
                 The object returned by call to initialize()
             settings (any):
                 Any settings required to be passed to the deploy of driver
         """
         pass
 
 
+class IQTask(Task):
+    """IQ Task
+
+    This class is used to create IQ modules that post data to the Switch Automation Platform.
+
+    """
+
+    @property
+    def mapping_entities(self) -> List[MAPPING_ENTITIES]:
+        """The type of entities being mapped."""
+        return 'IQ'
+
+    @property
+    @abstractmethod
+    def module_type(self) -> str:
+        """The type of IQ Module."""
+        pass
+
+    @abstractmethod
+    def process(self, api_inputs: ApiInputs, iq_settings: dict):
+        """Method to be implemented if data
+
+        The method should contain all code used to cleanse, reformat & post the data pulled via the integration.
+
+        Parameters
+        ----------
+        api_inputs: ApiInputs
+            object returned by call to initialize()
+        iq_settings : dict
+            Any settings required to be passed to the integration to run. For example, username & password, api key,
+            auth token, etc.
+
+        """
+        pass
+
 # class GuideTask(Task):
 #
 #     def __init__(self) -> None:
 #         self.logger = logging.getLogger(__name__)
 #         self.logger.setLevel(logging.DEBUG)
 #         consoleHandler = logging.StreamHandler(sys.stdout)
 #         consoleHandler.setLevel(logging.INFO)
```

### Comparing `switch_api-0.5.5/switch_api/platform_insights/__init__.py` & `switch_api-0.5.6/switch_api/platform_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api/platform_insights/platform_insights.py` & `switch_api-0.5.6/switch_api/platform_insights/platform_insights.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.5/switch_api.egg-info/PKG-INFO` & `switch_api-0.5.6/switch_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-api
-Version: 0.5.5
+Version: 0.5.6
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,25 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.5.5
+### Added
+In the `pipeline` module: 
+- Added a new task `IQTask`
+  - Additional abstract property `module_type` that accepts strings. This should define the type of IQ module. 
+  - Abstract method `process` must be instantiated for the task to be registered. 
+  
+### Modified
+In the `pipeline` module: 
+- Updated the `Automation.register_task()` method to accept tasks that subclass the new `IQTask`.  
+
 ## 0.5.4
 
 ### Added
 
 In the `integration` module:
 
 - Added new function `upsert_reservations()`
```

### Comparing `switch_api-0.5.5/switch_api.egg-info/SOURCES.txt` & `switch_api-0.5.6/switch_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

