# Comparing `tmp/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5.tar.gz` & `tmp/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5.tar", last modified: Mon May 13 14:49:03 2024, max compression
+gzip compressed data, was "tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6.tar", last modified: Tue May 14 14:07:19 2024, max compression
```

## Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5.tar` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 14:49:03.512595 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/
--rw-r--r--   0 test      (1000) test      (1000)      155 2024-05-13 14:49:03.512595 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)      232 2024-05-13 14:48:54.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/pyproject.toml
--rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-13 14:49:03.512595 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/setup.cfg
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 14:49:03.508595 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 14:49:03.512595 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql/
--rw-rw-r--   0 test      (1000) test      (1000)     2890 2024-05-13 14:47:36.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql/main.py
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 14:49:03.512595 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/
--rw-r--r--   0 test      (1000) test      (1000)      155 2024-05-13 14:49:03.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1000) test      (1000)      404 2024-05-13 14:49:03.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1000) test      (1000)        1 2024-05-13 14:49:03.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-13 14:49:03.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/requires.txt
--rw-rw-r--   0 test      (1000) test      (1000)        7 2024-05-13 14:49:03.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/top_level.txt
-drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-13 14:49:03.512595 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/test/
--rw-rw-r--   0 test      (1000) test      (1000)     1655 2024-05-10 18:02:47.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/test/test_sql.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-14 14:07:19.155549 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/
+-rw-r--r--   0 test      (1000) test      (1000)      147 2024-05-14 14:07:19.155549 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)      224 2024-05-14 13:52:29.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/pyproject.toml
+-rw-rw-r--   0 test      (1000) test      (1000)       38 2024-05-14 14:07:19.155549 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/setup.cfg
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-14 14:07:19.151549 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-14 14:07:19.151549 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql/
+-rw-rw-r--   0 test      (1000) test      (1000)     2890 2024-05-13 14:47:36.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql/main.py
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-14 14:07:19.155549 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/
+-rw-r--r--   0 test      (1000) test      (1000)      147 2024-05-14 14:07:19.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1000) test      (1000)      404 2024-05-14 14:07:19.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        1 2024-05-14 14:07:19.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1000) test      (1000)       30 2024-05-14 14:07:19.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/requires.txt
+-rw-rw-r--   0 test      (1000) test      (1000)        7 2024-05-14 14:07:19.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064.egg-info/top_level.txt
+drwxrwxr-x   0 test      (1000) test      (1000)        0 2024-05-14 14:07:19.155549 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/test/
+-rw-rw-r--   0 test      (1000) test      (1000)     1655 2024-05-10 18:02:47.000000 tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/test/test_sql.py
```

### Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/src/tp_sql/main.py` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/src/tp_sql/main.py`

 * *Files identical despite different names*

### Comparing `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.5/test/test_sql.py` & `tp_sql_09c77c38_19e1_42d9_886a_42a530ba9064-0.0.6/test/test_sql.py`

 * *Files identical despite different names*

