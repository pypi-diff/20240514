# Comparing `tmp/django_protoni-0.4.6.tar.gz` & `tmp/django_protoni-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_protoni-0.4.6.tar", last modified: Tue Apr 16 12:25:36 2024, max compression
+gzip compressed data, was "django_protoni-0.4.7.tar", last modified: Tue May 14 09:54:51 2024, max compression
```

## Comparing `django_protoni-0.4.6.tar` & `django_protoni-0.4.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-16 12:25:36.505323 django_protoni-0.4.6/
--rw-r--r--   0 aha        (501) staff       (20)      117 2024-04-16 12:25:36.505022 django_protoni-0.4.6/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-16 12:25:36.504608 django_protoni-0.4.6/django_protoni.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      117 2024-04-16 12:25:36.000000 django_protoni-0.4.6/django_protoni.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      816 2024-04-16 12:25:36.000000 django_protoni-0.4.6/django_protoni.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2024-04-16 12:25:36.000000 django_protoni-0.4.6/django_protoni.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      549 2024-04-16 12:25:36.000000 django_protoni-0.4.6/django_protoni.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     9236 2024-04-16 12:25:36.000000 django_protoni-0.4.6/django_protoni.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)       29 2024-04-16 12:25:36.000000 django_protoni-0.4.6/django_protoni.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)       15 2024-04-16 12:25:36.000000 django_protoni-0.4.6/django_protoni.egg-info/top_level.txt
--rwxr-xr-x   0 aha        (501) staff       (20)     1005 2023-11-03 11:42:16.000000 django_protoni-0.4.6/manage.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-16 12:25:36.501922 django_protoni-0.4.6/protoni/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django_protoni-0.4.6/protoni/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)     8176 2024-01-26 14:34:24.000000 django_protoni-0.4.6/protoni/asetukset.py
--rw-r--r--   0 aha        (501) staff       (20)      731 2023-11-03 11:42:40.000000 django_protoni-0.4.6/protoni/asgi.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-04-16 12:25:36.504279 django_protoni-0.4.6/protoni/laajennos/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django_protoni-0.4.6/protoni/laajennos/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django_protoni-0.4.6/protoni/laajennos/celery.py
--rw-r--r--   0 aha        (501) staff       (20)      441 2023-06-05 11:08:55.000000 django_protoni-0.4.6/protoni/laajennos/corsheaders.py
--rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django_protoni-0.4.6/protoni/laajennos/debug_toolbar.py
--rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django_protoni-0.4.6/protoni/laajennos/dj_database_url.py
--rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django_protoni-0.4.6/protoni/laajennos/extensions.py
--rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django_protoni-0.4.6/protoni/laajennos/heroku.py
--rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django_protoni-0.4.6/protoni/laajennos/hosts.py
--rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django_protoni-0.4.6/protoni/laajennos/pipeline.py
--rw-r--r--   0 aha        (501) staff       (20)     2001 2024-04-16 08:32:57.000000 django_protoni-0.4.6/protoni/laajennos/sentry.py
--rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django_protoni-0.4.6/protoni/laajennos/whitenoise.py
--rw-r--r--   0 aha        (501) staff       (20)     1823 2023-11-23 08:00:27.000000 django_protoni-0.4.6/protoni/nakymat.py
--rw-r--r--   0 aha        (501) staff       (20)     1397 2024-01-29 11:51:19.000000 django_protoni-0.4.6/protoni/osoitteet.py
--rw-r--r--   0 aha        (501) staff       (20)     2240 2024-01-29 11:56:30.000000 django_protoni-0.4.6/protoni/palvelimet.py
--rw-r--r--   0 aha        (501) staff       (20)     1656 2023-06-05 11:08:55.000000 django_protoni-0.4.6/protoni/palvelin.py
--rw-r--r--   0 aha        (501) staff       (20)      253 2023-06-05 11:08:55.000000 django_protoni-0.4.6/protoni/tyoasema.py
--rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django_protoni-0.4.6/protoni/wsgi.py
--rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-05 11:16:28.000000 django_protoni-0.4.6/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2024-04-16 12:25:36.505520 django_protoni-0.4.6/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)     1026 2023-11-23 08:00:20.000000 django_protoni-0.4.6/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-14 09:54:51.594570 django_protoni-0.4.7/
+-rw-r--r--   0 aha        (501) staff       (20)      117 2024-05-14 09:54:51.594285 django_protoni-0.4.7/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-14 09:54:51.594067 django_protoni-0.4.7/django_protoni.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      117 2024-05-14 09:54:51.000000 django_protoni-0.4.7/django_protoni.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      816 2024-05-14 09:54:51.000000 django_protoni-0.4.7/django_protoni.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2024-05-14 09:54:51.000000 django_protoni-0.4.7/django_protoni.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      549 2024-05-14 09:54:51.000000 django_protoni-0.4.7/django_protoni.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     9402 2024-05-14 09:54:51.000000 django_protoni-0.4.7/django_protoni.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)       29 2024-05-14 09:54:51.000000 django_protoni-0.4.7/django_protoni.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)       15 2024-05-14 09:54:51.000000 django_protoni-0.4.7/django_protoni.egg-info/top_level.txt
+-rwxr-xr-x   0 aha        (501) staff       (20)     1005 2023-11-03 11:42:16.000000 django_protoni-0.4.7/manage.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-14 09:54:51.592151 django_protoni-0.4.7/protoni/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django_protoni-0.4.7/protoni/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)     8176 2024-01-26 14:34:24.000000 django_protoni-0.4.7/protoni/asetukset.py
+-rw-r--r--   0 aha        (501) staff       (20)      731 2023-11-03 11:42:40.000000 django_protoni-0.4.7/protoni/asgi.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2024-05-14 09:54:51.593764 django_protoni-0.4.7/protoni/laajennos/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-10-04 08:10:20.000000 django_protoni-0.4.7/protoni/laajennos/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      261 2021-10-04 08:10:20.000000 django_protoni-0.4.7/protoni/laajennos/celery.py
+-rw-r--r--   0 aha        (501) staff       (20)      441 2023-06-05 11:08:55.000000 django_protoni-0.4.7/protoni/laajennos/corsheaders.py
+-rw-r--r--   0 aha        (501) staff       (20)      425 2021-10-08 10:28:51.000000 django_protoni-0.4.7/protoni/laajennos/debug_toolbar.py
+-rw-r--r--   0 aha        (501) staff       (20)      161 2021-10-04 08:10:20.000000 django_protoni-0.4.7/protoni/laajennos/dj_database_url.py
+-rw-r--r--   0 aha        (501) staff       (20)      113 2021-10-14 08:09:21.000000 django_protoni-0.4.7/protoni/laajennos/extensions.py
+-rw-r--r--   0 aha        (501) staff       (20)      165 2021-10-04 08:10:20.000000 django_protoni-0.4.7/protoni/laajennos/heroku.py
+-rw-r--r--   0 aha        (501) staff       (20)      518 2021-10-04 08:45:41.000000 django_protoni-0.4.7/protoni/laajennos/hosts.py
+-rw-r--r--   0 aha        (501) staff       (20)     1110 2021-10-04 08:10:20.000000 django_protoni-0.4.7/protoni/laajennos/pipeline.py
+-rw-r--r--   0 aha        (501) staff       (20)     2001 2024-04-16 08:32:57.000000 django_protoni-0.4.7/protoni/laajennos/sentry.py
+-rw-r--r--   0 aha        (501) staff       (20)      356 2021-10-08 10:28:51.000000 django_protoni-0.4.7/protoni/laajennos/whitenoise.py
+-rw-r--r--   0 aha        (501) staff       (20)     1823 2023-11-23 08:00:27.000000 django_protoni-0.4.7/protoni/nakymat.py
+-rw-r--r--   0 aha        (501) staff       (20)     1397 2024-01-29 11:51:19.000000 django_protoni-0.4.7/protoni/osoitteet.py
+-rw-r--r--   0 aha        (501) staff       (20)     2240 2024-01-29 11:56:30.000000 django_protoni-0.4.7/protoni/palvelimet.py
+-rw-r--r--   0 aha        (501) staff       (20)     1656 2023-06-05 11:08:55.000000 django_protoni-0.4.7/protoni/palvelin.py
+-rw-r--r--   0 aha        (501) staff       (20)      289 2024-04-30 08:09:27.000000 django_protoni-0.4.7/protoni/tyoasema.py
+-rw-r--r--   0 aha        (501) staff       (20)      224 2021-10-04 08:10:20.000000 django_protoni-0.4.7/protoni/wsgi.py
+-rw-r--r--   0 aha        (501) staff       (20)       80 2023-06-05 11:16:28.000000 django_protoni-0.4.7/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2024-05-14 09:54:51.594621 django_protoni-0.4.7/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)     1026 2023-11-23 08:00:20.000000 django_protoni-0.4.7/setup.py
```

### Comparing `django_protoni-0.4.6/django_protoni.egg-info/SOURCES.txt` & `django_protoni-0.4.7/django_protoni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/django_protoni.egg-info/entry_points.txt` & `django_protoni-0.4.7/django_protoni.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/django_protoni.egg-info/historia.json` & `django_protoni-0.4.7/django_protoni.egg-info/historia.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428571%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '04aa3ba564bb4ed7446bdca9595a0fea15823b93'), ('versio', "*

 * *           "'0.4.7'), ('kuvaus', 'Parametrisoitu `DEBUG` myös työasematestauksessa')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "Parametrisoitu `DEBUG` my\u00f6s ty\u00f6asematestauksessa",
+        "revisio": "04aa3ba564bb4ed7446bdca9595a0fea15823b93",
+        "versio": "0.4.7"
+    },
+    {
         "kuvaus": "Parametrisoitu `SENTRY_DENYLIST`-luettelo",
         "revisio": "e81aaab0133a78a6484772f34750c4dce4056678",
         "versio": "0.4.6"
     },
     {
         "kuvaus": "Korjattu Python 3.9- -yhteensopivuus",
         "revisio": "e13fe4371d296fa3560bcc1aab3f427bd17de7fb",
```

### Comparing `django_protoni-0.4.6/manage.py` & `django_protoni-0.4.7/manage.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/asetukset.py` & `django_protoni-0.4.7/protoni/asetukset.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/asgi.py` & `django_protoni-0.4.7/protoni/asgi.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/laajennos/hosts.py` & `django_protoni-0.4.7/protoni/laajennos/hosts.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/laajennos/pipeline.py` & `django_protoni-0.4.7/protoni/laajennos/pipeline.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/laajennos/sentry.py` & `django_protoni-0.4.7/protoni/laajennos/sentry.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/nakymat.py` & `django_protoni-0.4.7/protoni/nakymat.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/osoitteet.py` & `django_protoni-0.4.7/protoni/osoitteet.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/palvelimet.py` & `django_protoni-0.4.7/protoni/palvelimet.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/protoni/palvelin.py` & `django_protoni-0.4.7/protoni/palvelin.py`

 * *Files identical despite different names*

### Comparing `django_protoni-0.4.6/setup.py` & `django_protoni-0.4.7/setup.py`

 * *Files identical despite different names*

