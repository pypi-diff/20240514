# Comparing `tmp/linkedin_user_scrape-1.0.2.tar.gz` & `tmp/linkedin_user_scrape-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin_user_scrape-1.0.2.tar", last modified: Tue May 14 13:06:13 2024, max compression
+gzip compressed data, was "linkedin_user_scrape-1.0.3.tar", last modified: Tue May 14 13:14:23 2024, max compression
```

## Comparing `linkedin_user_scrape-1.0.2.tar` & `linkedin_user_scrape-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:06:13.576876 linkedin_user_scrape-1.0.2/
--rw-r--r--   0 harikabv   (501) staff       (20)      392 2024-05-14 13:06:13.576665 linkedin_user_scrape-1.0.2/PKG-INFO
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:06:13.575670 linkedin_user_scrape-1.0.2/linkedin_user_scrape/
--rw-r--r--   0 harikabv   (501) staff       (20)       43 2024-05-14 11:28:41.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape/__init__.py
--rw-r--r--   0 harikabv   (501) staff       (20)     7464 2024-05-14 11:30:25.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape/scraper.py
--rw-r--r--   0 harikabv   (501) staff       (20)     1601 2024-05-14 11:28:22.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape/utils.py
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:06:13.576460 linkedin_user_scrape-1.0.2/linkedin_user_scrape.egg-info/
--rw-r--r--   0 harikabv   (501) staff       (20)      392 2024-05-14 13:06:13.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape.egg-info/PKG-INFO
--rw-r--r--   0 harikabv   (501) staff       (20)      322 2024-05-14 13:06:13.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 13:06:13.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       24 2024-05-14 13:06:13.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape.egg-info/requires.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       21 2024-05-14 13:06:13.000000 linkedin_user_scrape-1.0.2/linkedin_user_scrape.egg-info/top_level.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-14 13:06:13.576932 linkedin_user_scrape-1.0.2/setup.cfg
--rw-r--r--   0 harikabv   (501) staff       (20)      557 2024-05-14 13:06:03.000000 linkedin_user_scrape-1.0.2/setup.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:14:23.646489 linkedin_user_scrape-1.0.3/
+-rw-r--r--   0 harikabv   (501) staff       (20)      376 2024-05-14 13:14:23.646279 linkedin_user_scrape-1.0.3/PKG-INFO
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:14:23.645156 linkedin_user_scrape-1.0.3/linkedin_user_scrape/
+-rw-r--r--   0 harikabv   (501) staff       (20)       43 2024-05-14 11:28:41.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape/__init__.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     7464 2024-05-14 11:30:25.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape/scraper.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     1601 2024-05-14 11:28:22.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape/utils.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 13:14:23.646070 linkedin_user_scrape-1.0.3/linkedin_user_scrape.egg-info/
+-rw-r--r--   0 harikabv   (501) staff       (20)      376 2024-05-14 13:14:23.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 harikabv   (501) staff       (20)      322 2024-05-14 13:14:23.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 13:14:23.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       23 2024-05-14 13:14:23.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape.egg-info/requires.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       21 2024-05-14 13:14:23.000000 linkedin_user_scrape-1.0.3/linkedin_user_scrape.egg-info/top_level.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-14 13:14:23.646544 linkedin_user_scrape-1.0.3/setup.cfg
+-rw-r--r--   0 harikabv   (501) staff       (20)      523 2024-05-14 13:14:10.000000 linkedin_user_scrape-1.0.3/setup.py
```

### Comparing `linkedin_user_scrape-1.0.2/linkedin_user_scrape/scraper.py` & `linkedin_user_scrape-1.0.3/linkedin_user_scrape/scraper.py`

 * *Files identical despite different names*

### Comparing `linkedin_user_scrape-1.0.2/linkedin_user_scrape/utils.py` & `linkedin_user_scrape-1.0.3/linkedin_user_scrape/utils.py`

 * *Files identical despite different names*

### Comparing `linkedin_user_scrape-1.0.2/setup.py` & `linkedin_user_scrape-1.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
-REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 setup(
     name='linkedin_user_scrape',
-    version='1.0.2',
+    version='1.0.3',
     author='Harika B V',
     author_email='harikabv.dev@gmail.com',
     description='LinkedIn scraper to parse user profiles',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
-    install_requires=REQUIREMENTS,
+    install_requires=[
+        'selenium'
+        'beautifulsoup4'
+    ],
     python_requires='>=3.6',
 )
```

