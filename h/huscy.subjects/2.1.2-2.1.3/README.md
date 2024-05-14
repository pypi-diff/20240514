# Comparing `tmp/huscy.subjects-2.1.2.tar.gz` & `tmp/huscy.subjects-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.subjects-2.1.2.tar", last modified: Fri Sep 22 14:44:55 2023, max compression
+gzip compressed data, was "huscy.subjects-2.1.3.tar", last modified: Tue May 14 11:09:16 2024, max compression
```

## Comparing `huscy.subjects-2.1.2.tar` & `huscy.subjects-2.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-22 14:44:55.515959 huscy.subjects-2.1.2/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3980 2023-09-22 14:44:55.515959 huscy.subjects-2.1.2/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2095 2023-04-11 15:22:54.000000 huscy.subjects-2.1.2/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-22 14:44:55.499959 huscy.subjects-2.1.2/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-22 14:44:55.499959 huscy.subjects-2.1.2/huscy/subjects/
--rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2023-09-22 08:31:22.000000 huscy.subjects-2.1.2/huscy/subjects/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2496 2022-10-17 12:29:15.000000 huscy.subjects-2.1.2/huscy/subjects/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-21 19:01:54.000000 huscy.subjects-2.1.2/huscy/subjects/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-22 14:44:55.515959 huscy.subjects-2.1.2/huscy/subjects/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4491 2020-11-23 17:38:26.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5418 2022-11-10 10:58:50.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     7787 2021-10-28 16:39:39.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0002_auto_20210810_0124.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1498 2021-10-28 16:39:39.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0003_auto_20211028_1133.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      245 2022-10-11 07:31:35.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0004_delete_note.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1834 2022-10-11 14:39:42.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0005_auto_20221011_0432.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      287 2022-10-20 08:32:27.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0006_rename_contact_contactold.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3841 2022-10-20 08:32:27.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0007_contact.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      714 2022-10-20 08:32:27.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0008_auto_20221018_0935.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      251 2022-10-20 08:32:27.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/0009_delete_contactold.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-05-14 14:27:02.000000 huscy.subjects-2.1.2/huscy/subjects/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4388 2022-10-20 08:32:27.000000 huscy.subjects-2.1.2/huscy/subjects/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      187 2020-05-14 14:27:02.000000 huscy.subjects-2.1.2/huscy/subjects/pagination.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      494 2022-10-11 07:31:35.000000 huscy.subjects-2.1.2/huscy/subjects/permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3796 2022-10-17 12:29:15.000000 huscy.subjects-2.1.2/huscy/subjects/serializers.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4293 2022-11-10 10:58:50.000000 huscy.subjects-2.1.2/huscy/subjects/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      517 2023-09-22 08:31:22.000000 huscy.subjects-2.1.2/huscy/subjects/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4467 2022-11-10 10:58:50.000000 huscy.subjects-2.1.2/huscy/subjects/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-09-22 14:44:55.499959 huscy.subjects-2.1.2/huscy.subjects.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3980 2023-09-22 14:44:55.000000 huscy.subjects-2.1.2/huscy.subjects.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1027 2023-09-22 14:44:55.000000 huscy.subjects-2.1.2/huscy.subjects.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-09-22 14:44:55.000000 huscy.subjects-2.1.2/huscy.subjects.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      253 2023-09-22 14:44:55.000000 huscy.subjects-2.1.2/huscy.subjects.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-09-22 14:44:55.000000 huscy.subjects-2.1.2/huscy.subjects.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-09-22 14:44:55.515959 huscy.subjects-2.1.2/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1937 2023-04-17 15:12:04.000000 huscy.subjects-2.1.2/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-14 11:09:16.396063 huscy.subjects-2.1.3/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3930 2024-05-14 11:09:16.396063 huscy.subjects-2.1.3/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2090 2024-05-13 11:00:16.000000 huscy.subjects-2.1.3/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-14 11:09:16.388063 huscy.subjects-2.1.3/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-14 11:09:16.392063 huscy.subjects-2.1.3/huscy/subjects/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       89 2024-05-13 11:00:16.000000 huscy.subjects-2.1.3/huscy/subjects/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2496 2022-10-17 12:29:15.000000 huscy.subjects-2.1.3/huscy/subjects/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-21 19:01:54.000000 huscy.subjects-2.1.3/huscy/subjects/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-14 11:09:16.392063 huscy.subjects-2.1.3/huscy/subjects/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4491 2020-11-23 17:38:26.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5418 2022-11-10 10:58:50.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     7787 2021-10-28 16:39:39.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0002_auto_20210810_0124.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1498 2021-10-28 16:39:39.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0003_auto_20211028_1133.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      245 2022-10-11 07:31:35.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0004_delete_note.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1834 2022-10-11 14:39:42.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0005_auto_20221011_0432.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      287 2022-10-20 08:32:27.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0006_rename_contact_contactold.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3841 2022-10-20 08:32:27.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0007_contact.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      714 2022-10-20 08:32:27.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0008_auto_20221018_0935.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      251 2022-10-20 08:32:27.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/0009_delete_contactold.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-05-14 14:27:02.000000 huscy.subjects-2.1.3/huscy/subjects/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4388 2022-10-20 08:32:27.000000 huscy.subjects-2.1.3/huscy/subjects/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      187 2020-05-14 14:27:02.000000 huscy.subjects-2.1.3/huscy/subjects/pagination.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      494 2022-10-11 07:31:35.000000 huscy.subjects-2.1.3/huscy/subjects/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3796 2022-10-17 12:29:15.000000 huscy.subjects-2.1.3/huscy/subjects/serializers.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4293 2022-11-10 10:58:50.000000 huscy.subjects-2.1.3/huscy/subjects/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      517 2023-09-22 08:31:22.000000 huscy.subjects-2.1.3/huscy/subjects/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4467 2022-11-10 10:58:50.000000 huscy.subjects-2.1.3/huscy/subjects/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-14 11:09:16.388063 huscy.subjects-2.1.3/huscy.subjects.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3930 2024-05-14 11:09:16.000000 huscy.subjects-2.1.3/huscy.subjects.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1027 2024-05-14 11:09:16.000000 huscy.subjects-2.1.3/huscy.subjects.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2024-05-14 11:09:16.000000 huscy.subjects-2.1.3/huscy.subjects.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      250 2024-05-14 11:09:16.000000 huscy.subjects-2.1.3/huscy.subjects.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2024-05-14 11:09:16.000000 huscy.subjects-2.1.3/huscy.subjects.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2024-05-14 11:09:16.396063 huscy.subjects-2.1.3/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1831 2024-05-13 11:00:16.000000 huscy.subjects-2.1.3/setup.py
```

### Comparing `huscy.subjects-2.1.2/PKG-INFO` & `huscy.subjects-2.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: huscy.subjects
-Version: 2.1.2
+Version: 2.1.3
 Summary: Managing subjects in a human research context.
 Home-page: https://bitbucket.org/huscy/subjects
-Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
-Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
+Author: Mathias Goldau, Stefan Bunde
+Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: huscy.subjects
         ======
         
         ![PyPi Version](https://img.shields.io/pypi/v/huscy-subjects.svg)
         ![PyPi Status](https://img.shields.io/pypi/status/huscy-subjects)
         ![PyPI Downloads](https://img.shields.io/pypi/dm/huscy-subjects)
@@ -20,15 +20,15 @@
         
         Requirements
         ------
         
         - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.1 and 4.2.
+        Tox tests on Django versions 4.2 and 5.0.
         
         
         
         Installation
         ------
         
         To install `husy.subjects` simply run:
@@ -108,14 +108,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.subjects-2.1.2/README.md` & `huscy.subjects-2.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Requirements
 ------
 
 - Python 3.8+
 - A supported version of Django
 
-Tox tests on Django versions 3.2, 4.1 and 4.2.
+Tox tests on Django versions 4.2 and 5.0.
 
 
 
 Installation
 ------
 
 To install `husy.subjects` simply run:
```

### Comparing `huscy.subjects-2.1.2/huscy/subjects/admin.py` & `huscy.subjects-2.1.3/huscy/subjects/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/migrations/0001_initial.py` & `huscy.subjects-2.1.3/huscy/subjects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py` & `huscy.subjects-2.1.3/huscy/subjects/migrations/0001_squashed_0009_delete_contactold.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/migrations/0002_auto_20210810_0124.py` & `huscy.subjects-2.1.3/huscy/subjects/migrations/0002_auto_20210810_0124.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/migrations/0003_auto_20211028_1133.py` & `huscy.subjects-2.1.3/huscy/subjects/migrations/0003_auto_20211028_1133.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/migrations/0005_auto_20221011_0432.py` & `huscy.subjects-2.1.3/huscy/subjects/migrations/0005_auto_20221011_0432.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/migrations/0007_contact.py` & `huscy.subjects-2.1.3/huscy/subjects/migrations/0007_contact.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/migrations/0008_auto_20221018_0935.py` & `huscy.subjects-2.1.3/huscy/subjects/migrations/0008_auto_20221018_0935.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/models.py` & `huscy.subjects-2.1.3/huscy/subjects/models.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/serializers.py` & `huscy.subjects-2.1.3/huscy/subjects/serializers.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/services.py` & `huscy.subjects-2.1.3/huscy/subjects/services.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/urls.py` & `huscy.subjects-2.1.3/huscy/subjects/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy/subjects/views.py` & `huscy.subjects-2.1.3/huscy/subjects/views.py`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/huscy.subjects.egg-info/PKG-INFO` & `huscy.subjects-2.1.3/huscy.subjects.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: huscy.subjects
-Version: 2.1.2
+Version: 2.1.3
 Summary: Managing subjects in a human research context.
 Home-page: https://bitbucket.org/huscy/subjects
-Author: Alexander Tyapkov, Mathias Goldau, Stefan Bunde
-Author-email: tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de
+Author: Mathias Goldau, Stefan Bunde
+Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: huscy.subjects
         ======
         
         ![PyPi Version](https://img.shields.io/pypi/v/huscy-subjects.svg)
         ![PyPi Status](https://img.shields.io/pypi/status/huscy-subjects)
         ![PyPI Downloads](https://img.shields.io/pypi/dm/huscy-subjects)
@@ -20,15 +20,15 @@
         
         Requirements
         ------
         
         - Python 3.8+
         - A supported version of Django
         
-        Tox tests on Django versions 3.2, 4.1 and 4.2.
+        Tox tests on Django versions 4.2 and 5.0.
         
         
         
         Installation
         ------
         
         To install `husy.subjects` simply run:
@@ -108,14 +108,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: testing
```

### Comparing `huscy.subjects-2.1.2/huscy.subjects.egg-info/SOURCES.txt` & `huscy.subjects-2.1.3/huscy.subjects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.subjects-2.1.2/setup.py` & `huscy.subjects-2.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,51 +13,46 @@
     version=__version__,
     license='AGPLv3+',
 
     description='Managing subjects in a human research context.',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
-    author='Alexander Tyapkov, Mathias Goldau, Stefan Bunde',
-    author_email='tyapkov@gmail.com, goldau@cbs.mpg.de, stefanbunde+git@posteo.de',
+    author='Mathias Goldau, Stefan Bunde',
+    author_email='stefanbunde+git@posteo.de',
 
     url='https://bitbucket.org/huscy/subjects',
 
     packages=find_namespace_packages(include=['huscy.*']),
 
     install_requires=[
-        'Django>=3.2',
-        'djangorestframework>=3.11',
+        'Django>=4.2',
+        'djangorestframework>=3.14',
         'django-countries>=7.1',
         'django-guardian>=2.2',
-        'django-phonenumber-field[phonenumberslite]>=5',
-        'django-reversion>=3',
+        'django-phonenumber-field[phonenumberslite]>=5.1',
+        'django-reversion>=4',
         'drf-nested-routers>=0.90',
         'python-dateutil>=2.7',
     ],
     extras_require={
-        'development': [
-            'psycopg2-binary',
-        ],
-        'testing': [
-            'tox',
-            'watchdog==0.9',
-        ]
+        'development': ['psycopg2-binary'],
+        'testing': ['tox', 'watchdog']
     },
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.1',
         'Framework :: Django :: 4.2',
+        'Framework :: Django :: 5.0',
     ],
 )
```

