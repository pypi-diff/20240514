# Comparing `tmp/botasaurus_api-4.0.1.tar.gz` & `tmp/botasaurus_api-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_api-4.0.1.tar", last modified: Thu Mar 14 08:24:53 2024, max compression
+gzip compressed data, was "botasaurus_api-4.0.2.tar", last modified: Tue May 14 15:48:51 2024, max compression
```

## Comparing `botasaurus_api-4.0.1.tar` & `botasaurus_api-4.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 08:24:53.579259 botasaurus_api-4.0.1/
--rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus_api-4.0.1/LICENSE
--rw-rw-rw-   0        0        0     1115 2024-03-14 08:24:53.578753 botasaurus_api-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-03-14 07:59:30.000000 botasaurus_api-4.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 08:24:53.544939 botasaurus_api-4.0.1/botasaurus_api/
--rw-rw-rw-   0        0        0     1630 2024-03-14 07:57:10.000000 botasaurus_api-4.0.1/botasaurus_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 08:24:53.576721 botasaurus_api-4.0.1/botasaurus_api.egg-info/
--rw-rw-rw-   0        0        0     1115 2024-03-14 08:24:53.000000 botasaurus_api-4.0.1/botasaurus_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-03-14 08:24:53.000000 botasaurus_api-4.0.1/botasaurus_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 08:24:53.000000 botasaurus_api-4.0.1/botasaurus_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-14 08:24:53.000000 botasaurus_api-4.0.1/botasaurus_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-14 08:24:53.000000 botasaurus_api-4.0.1/botasaurus_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-14 08:24:53.582974 botasaurus_api-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1644 2024-03-14 08:24:52.000000 botasaurus_api-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:48:51.739036 botasaurus_api-4.0.2/
+-rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus_api-4.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6962 2024-05-14 15:48:51.738411 botasaurus_api-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5863 2024-04-11 11:33:13.000000 botasaurus_api-4.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:48:51.694727 botasaurus_api-4.0.2/botasaurus_api/
+-rw-rw-rw-   0        0        0    14011 2024-04-11 13:30:57.000000 botasaurus_api-4.0.2/botasaurus_api/__init__.py
+-rw-rw-rw-   0        0        0     1881 2024-04-12 12:13:48.000000 botasaurus_api-4.0.2/botasaurus_api/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:48:51.736521 botasaurus_api-4.0.2/botasaurus_api.egg-info/
+-rw-rw-rw-   0        0        0     6962 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-14 15:48:51.000000 botasaurus_api-4.0.2/botasaurus_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-14 15:48:51.742700 botasaurus_api-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1644 2024-05-14 15:48:50.000000 botasaurus_api-4.0.2/setup.py
```

### Comparing `botasaurus_api-4.0.1/LICENSE` & `botasaurus_api-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_api-4.0.1/setup.py` & `botasaurus_api-4.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return long_description
     except:
         return None
 
 
 setup(
     name="botasaurus_api",
-    version='4.0.1',
+    version='4.0.2',
     author="Chetan Jain",
     author_email="chetan@omkar.cloud",
     description="The Botasaurus API Client provides programmatic access to Botasaurus scrapers with a developer-friendly API.",
     license="MIT",
     keywords=["seleniumwire proxy authentication", "proxy authentication"],
     url="https://github.com/omkarcloud/botasaurus-proxy-authentication",
     packages=["botasaurus_api"],
```

