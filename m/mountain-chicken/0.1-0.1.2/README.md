# Comparing `tmp/mountain_chicken-0.1.tar.gz` & `tmp/mountain_chicken-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountain_chicken-0.1.tar", last modified: Mon May 13 14:30:02 2024, max compression
+gzip compressed data, was "mountain_chicken-0.1.2.tar", last modified: Tue May 14 11:48:58 2024, max compression
```

## Comparing `mountain_chicken-0.1.tar` & `mountain_chicken-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:30:02.610613 mountain_chicken-0.1/
--rw-rw-rw-   0        0        0       61 2024-05-13 14:30:02.609614 mountain_chicken-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-13 14:29:40.000000 mountain_chicken-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:30:02.605613 mountain_chicken-0.1/mountain_chicken/
--rw-rw-rw-   0        0        0       23 2024-05-13 14:21:55.000000 mountain_chicken-0.1/mountain_chicken/__init__.py
--rw-rw-rw-   0        0        0       32 2024-05-13 14:22:01.000000 mountain_chicken-0.1/mountain_chicken/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:30:02.609115 mountain_chicken-0.1/mountain_chicken.egg-info/
--rw-rw-rw-   0        0        0       61 2024-05-13 14:30:02.000000 mountain_chicken-0.1/mountain_chicken.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-13 14:30:02.000000 mountain_chicken-0.1/mountain_chicken.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:30:02.000000 mountain_chicken-0.1/mountain_chicken.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-13 14:30:02.000000 mountain_chicken-0.1/mountain_chicken.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:30:02.610613 mountain_chicken-0.1/setup.cfg
--rw-rw-rw-   0        0        0      200 2024-05-13 14:29:39.000000 mountain_chicken-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:48:58.587035 mountain_chicken-0.1.2/
+-rw-rw-rw-   0        0        0       63 2024-05-14 11:48:58.586535 mountain_chicken-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2024-05-13 15:05:37.000000 mountain_chicken-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 11:48:58.582535 mountain_chicken-0.1.2/mountain_chicken/
+-rw-rw-rw-   0        0        0       23 2024-05-13 14:21:55.000000 mountain_chicken-0.1.2/mountain_chicken/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-05-13 19:08:16.000000 mountain_chicken-0.1.2/mountain_chicken/double_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:48:58.586035 mountain_chicken-0.1.2/mountain_chicken.egg-info/
+-rw-rw-rw-   0        0        0       63 2024-05-14 11:48:58.000000 mountain_chicken-0.1.2/mountain_chicken.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-14 11:48:58.000000 mountain_chicken-0.1.2/mountain_chicken.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 11:48:58.000000 mountain_chicken-0.1.2/mountain_chicken.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-14 11:48:58.000000 mountain_chicken-0.1.2/mountain_chicken.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 11:48:58.587035 mountain_chicken-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      202 2024-05-14 11:37:59.000000 mountain_chicken-0.1.2/setup.py
```

