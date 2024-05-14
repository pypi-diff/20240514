# Comparing `tmp/basic_web_server-0.2.tar.gz` & `tmp/basic_web_server-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic_web_server-0.2.tar", last modified: Tue May 14 01:39:15 2024, max compression
+gzip compressed data, was "basic_web_server-0.3.tar", last modified: Tue May 14 11:58:49 2024, max compression
```

## Comparing `basic_web_server-0.2.tar` & `basic_web_server-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 01:39:15.752792 basic_web_server-0.2/
--rw-rw-rw-   0        0        0      228 2024-05-14 01:39:15.739240 basic_web_server-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      856 2024-05-13 23:51:18.000000 basic_web_server-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 01:39:15.737237 basic_web_server-0.2/basic_web_server.egg-info/
--rw-rw-rw-   0        0        0      228 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-14 01:39:15.000000 basic_web_server-0.2/basic_web_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4855 2024-05-14 01:39:10.000000 basic_web_server-0.2/basic_webserver.py
--rw-rw-rw-   0        0        0       42 2024-05-14 01:39:15.753788 basic_web_server-0.2/setup.cfg
--rw-rw-rw-   0        0        0      365 2024-05-14 01:38:52.000000 basic_web_server-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:58:49.752365 basic_web_server-0.3/
+-rw-rw-rw-   0        0        0     1127 2024-05-14 11:58:49.742793 basic_web_server-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      856 2024-05-13 23:51:18.000000 basic_web_server-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 11:58:49.741799 basic_web_server-0.3/basic_web_server.egg-info/
+-rw-rw-rw-   0        0        0     1127 2024-05-14 11:58:49.000000 basic_web_server-0.3/basic_web_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-05-14 11:58:49.000000 basic_web_server-0.3/basic_web_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 11:58:49.000000 basic_web_server-0.3/basic_web_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-14 11:58:49.000000 basic_web_server-0.3/basic_web_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8925 2024-05-14 11:54:56.000000 basic_web_server-0.3/basic_webserver.py
+-rw-rw-rw-   0        0        0       42 2024-05-14 11:58:49.752365 basic_web_server-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      527 2024-05-14 11:58:46.000000 basic_web_server-0.3/setup.py
```

### Comparing `basic_web_server-0.2/README.md` & `basic_web_server-0.3/README.md`

 * *Files identical despite different names*

