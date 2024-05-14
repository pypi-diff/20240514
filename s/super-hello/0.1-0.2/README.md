# Comparing `tmp/super_hello-0.1.tar.gz` & `tmp/super_hello-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_hello-0.1.tar", last modified: Tue May 14 12:21:34 2024, max compression
+gzip compressed data, was "super_hello-0.2.tar", last modified: Tue May 14 12:25:04 2024, max compression
```

## Comparing `super_hello-0.1.tar` & `super_hello-0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:21:34.901047 super_hello-0.1/
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      134 2024-05-14 12:21:34.901047 super_hello-0.1/PKG-INFO
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:18:46.000000 super_hello-0.1/README.md
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       38 2024-05-14 12:21:34.901047 super_hello-0.1/setup.cfg
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      155 2024-05-14 12:21:17.000000 super_hello-0.1/setup.py
-drwxrwxr-x   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:21:34.901047 super_hello-0.1/super_hello/
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       23 2024-05-14 12:20:22.000000 super_hello-0.1/super_hello/__init__.py
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       38 2024-05-14 12:19:40.000000 super_hello-0.1/super_hello/main.py
-drwxrwxr-x   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:21:34.901047 super_hello-0.1/super_hello.egg-info/
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      134 2024-05-14 12:21:34.000000 super_hello-0.1/super_hello.egg-info/PKG-INFO
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      202 2024-05-14 12:21:34.000000 super_hello-0.1/super_hello.egg-info/SOURCES.txt
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)        1 2024-05-14 12:21:34.000000 super_hello-0.1/super_hello.egg-info/dependency_links.txt
--rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       12 2024-05-14 12:21:34.000000 super_hello-0.1/super_hello.egg-info/top_level.txt
+drwxrwxr-x   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:25:03.993891 super_hello-0.2/
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      134 2024-05-14 12:25:03.993891 super_hello-0.2/PKG-INFO
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:18:46.000000 super_hello-0.2/README.md
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       38 2024-05-14 12:25:03.993891 super_hello-0.2/setup.cfg
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      267 2024-05-14 12:24:31.000000 super_hello-0.2/setup.py
+drwxrwxr-x   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:25:03.993891 super_hello-0.2/super_hello/
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       23 2024-05-14 12:20:22.000000 super_hello-0.2/super_hello/__init__.py
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       38 2024-05-14 12:19:40.000000 super_hello-0.2/super_hello/main.py
+drwxrwxr-x   0 alpserin  (1000) alpserin  (1000)        0 2024-05-14 12:25:03.993891 super_hello-0.2/super_hello.egg-info/
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      134 2024-05-14 12:25:03.000000 super_hello-0.2/super_hello.egg-info/PKG-INFO
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)      240 2024-05-14 12:25:03.000000 super_hello-0.2/super_hello.egg-info/SOURCES.txt
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)        1 2024-05-14 12:25:03.000000 super_hello-0.2/super_hello.egg-info/dependency_links.txt
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       51 2024-05-14 12:25:03.000000 super_hello-0.2/super_hello.egg-info/entry_points.txt
+-rw-rw-r--   0 alpserin  (1000) alpserin  (1000)       12 2024-05-14 12:25:03.000000 super_hello-0.2/super_hello.egg-info/top_level.txt
```

