# Comparing `tmp/linkedin_user_scrape-1.0.0.tar.gz` & `tmp/linkedin_user_scrape-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin_user_scrape-1.0.0.tar", last modified: Tue May 14 11:09:12 2024, max compression
+gzip compressed data, was "linkedin_user_scrape-1.0.1.tar", last modified: Tue May 14 11:39:38 2024, max compression
```

## Comparing `linkedin_user_scrape-1.0.0.tar` & `linkedin_user_scrape-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 11:09:12.588575 linkedin_user_scrape-1.0.0/
--rw-r--r--   0 harikabv   (501) staff       (20)      338 2024-05-14 11:09:12.588366 linkedin_user_scrape-1.0.0/PKG-INFO
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 11:09:12.588156 linkedin_user_scrape-1.0.0/linkedin_user_scrape.egg-info/
--rw-r--r--   0 harikabv   (501) staff       (20)      338 2024-05-14 11:09:12.000000 linkedin_user_scrape-1.0.0/linkedin_user_scrape.egg-info/PKG-INFO
--rw-r--r--   0 harikabv   (501) staff       (20)      184 2024-05-14 11:09:12.000000 linkedin_user_scrape-1.0.0/linkedin_user_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 11:09:12.000000 linkedin_user_scrape-1.0.0/linkedin_user_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 11:09:12.000000 linkedin_user_scrape-1.0.0/linkedin_user_scrape.egg-info/top_level.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-14 11:09:12.588623 linkedin_user_scrape-1.0.0/setup.cfg
--rw-r--r--   0 harikabv   (501) staff       (20)      448 2024-05-14 11:08:37.000000 linkedin_user_scrape-1.0.0/setup.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 11:39:38.838101 linkedin_user_scrape-1.0.1/
+-rw-r--r--   0 harikabv   (501) staff       (20)      338 2024-05-14 11:39:38.837900 linkedin_user_scrape-1.0.1/PKG-INFO
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 11:39:38.836910 linkedin_user_scrape-1.0.1/linkedin_user_scrape/
+-rw-r--r--   0 harikabv   (501) staff       (20)       43 2024-05-14 11:28:41.000000 linkedin_user_scrape-1.0.1/linkedin_user_scrape/__init__.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     7464 2024-05-14 11:30:25.000000 linkedin_user_scrape-1.0.1/linkedin_user_scrape/scraper.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     1601 2024-05-14 11:28:22.000000 linkedin_user_scrape-1.0.1/linkedin_user_scrape/utils.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 11:39:38.837702 linkedin_user_scrape-1.0.1/linkedin_user_scrape.egg-info/
+-rw-r--r--   0 harikabv   (501) staff       (20)      338 2024-05-14 11:39:38.000000 linkedin_user_scrape-1.0.1/linkedin_user_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 harikabv   (501) staff       (20)      279 2024-05-14 11:39:38.000000 linkedin_user_scrape-1.0.1/linkedin_user_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 11:39:38.000000 linkedin_user_scrape-1.0.1/linkedin_user_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       21 2024-05-14 11:39:38.000000 linkedin_user_scrape-1.0.1/linkedin_user_scrape.egg-info/top_level.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-14 11:39:38.838154 linkedin_user_scrape-1.0.1/setup.cfg
+-rw-r--r--   0 harikabv   (501) staff       (20)      448 2024-05-14 11:39:35.000000 linkedin_user_scrape-1.0.1/setup.py
```

