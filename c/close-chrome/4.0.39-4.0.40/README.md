# Comparing `tmp/close_chrome-4.0.39.tar.gz` & `tmp/close_chrome-4.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "close_chrome-4.0.39.tar", last modified: Sat Apr 13 06:36:30 2024, max compression
+gzip compressed data, was "close_chrome-4.0.40.tar", last modified: Tue May 14 15:48:03 2024, max compression
```

## Comparing `close_chrome-4.0.39.tar` & `close_chrome-4.0.40.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 06:36:30.708531 close_chrome-4.0.39/
--rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 close_chrome-4.0.39/LICENSE
--rw-rw-rw-   0        0        0     1365 2024-04-13 06:36:30.707517 close_chrome-4.0.39/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-13 06:36:06.000000 close_chrome-4.0.39/README.md
--rw-rw-rw-   0        0        0       86 2024-04-13 06:36:30.714331 close_chrome-4.0.39/setup.cfg
--rw-rw-rw-   0        0        0     8176 2024-04-13 06:36:29.000000 close_chrome-4.0.39/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:36:30.663038 close_chrome-4.0.39/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 06:36:30.671674 close_chrome-4.0.39/src/close_chrome/
--rw-rw-rw-   0        0        0        0 2024-03-20 08:25:56.000000 close_chrome-4.0.39/src/close_chrome/__init__.py
--rw-rw-rw-   0        0        0      970 2024-04-13 06:31:40.000000 close_chrome-4.0.39/src/close_chrome/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 06:36:30.705838 close_chrome-4.0.39/src/close_chrome.egg-info/
--rw-rw-rw-   0        0        0     1365 2024-04-13 06:36:30.000000 close_chrome-4.0.39/src/close_chrome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2024-04-13 06:36:30.000000 close_chrome-4.0.39/src/close_chrome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 06:36:30.000000 close_chrome-4.0.39/src/close_chrome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-13 06:36:30.000000 close_chrome-4.0.39/src/close_chrome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 06:36:30.000000 close_chrome-4.0.39/src/close_chrome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 15:48:03.538485 close_chrome-4.0.40/
+-rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 close_chrome-4.0.40/LICENSE
+-rw-rw-rw-   0        0        0     1365 2024-05-14 15:48:03.537872 close_chrome-4.0.40/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-04-13 06:36:06.000000 close_chrome-4.0.40/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 15:48:03.550298 close_chrome-4.0.40/setup.cfg
+-rw-rw-rw-   0        0        0     8176 2024-05-14 15:48:02.000000 close_chrome-4.0.40/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:48:03.433056 close_chrome-4.0.40/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 15:48:03.449372 close_chrome-4.0.40/src/close_chrome/
+-rw-rw-rw-   0        0        0        0 2024-03-20 08:25:56.000000 close_chrome-4.0.40/src/close_chrome/__init__.py
+-rw-rw-rw-   0        0        0      970 2024-05-14 12:31:53.000000 close_chrome-4.0.40/src/close_chrome/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:48:03.534995 close_chrome-4.0.40/src/close_chrome.egg-info/
+-rw-rw-rw-   0        0        0     1365 2024-05-14 15:48:03.000000 close_chrome-4.0.40/src/close_chrome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-05-14 15:48:03.000000 close_chrome-4.0.40/src/close_chrome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:48:03.000000 close_chrome-4.0.40/src/close_chrome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-14 15:48:03.000000 close_chrome-4.0.40/src/close_chrome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 15:48:03.000000 close_chrome-4.0.40/src/close_chrome.egg-info/top_level.txt
```

### Comparing `close_chrome-4.0.39/LICENSE` & `close_chrome-4.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `close_chrome-4.0.39/PKG-INFO` & `close_chrome-4.0.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: close_chrome
-Version: 4.0.39
+Version: 4.0.40
 Summary: CLI for botasaurus.
 Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Project-URL: Bug Reports, https://github.com/omkarcloud/botasaurus/issues
 Project-URL: Say Thanks!, https://github.com/omkarcloud/botasaurus
```

### Comparing `close_chrome-4.0.39/setup.py` & `close_chrome-4.0.40/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-optional
-    version='4.0.39',
+    version='4.0.40',
     author="Chetan Jain",
     author_email="chetan@omkar.cloud",
     description="CLI for botasaurus.",
     license="MIT",
     keywords=["seleniumwire proxy authentication", "proxy authentication"],
     url="https://github.com/omkarcloud/botasaurus-proxy-authentication",
     long_description_content_type="text/markdown",
```

### Comparing `close_chrome-4.0.39/src/close_chrome/__main__.py` & `close_chrome-4.0.40/src/close_chrome/__main__.py`

 * *Files identical despite different names*

### Comparing `close_chrome-4.0.39/src/close_chrome.egg-info/PKG-INFO` & `close_chrome-4.0.40/src/close_chrome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: close_chrome
-Version: 4.0.39
+Version: 4.0.40
 Summary: CLI for botasaurus.
 Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Project-URL: Bug Reports, https://github.com/omkarcloud/botasaurus/issues
 Project-URL: Say Thanks!, https://github.com/omkarcloud/botasaurus
```

