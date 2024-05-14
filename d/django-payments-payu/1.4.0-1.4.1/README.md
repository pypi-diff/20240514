# Comparing `tmp/django-payments-payu-1.4.0.tar.gz` & `tmp/django-payments-payu-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-payments-payu-1.4.0.tar", last modified: Fri Apr 12 12:55:38 2024, max compression
+gzip compressed data, was "django-payments-payu-1.4.1.tar", last modified: Tue May 14 08:24:50 2024, max compression
```

## Comparing `django-payments-payu-1.4.0.tar` & `django-payments-payu-1.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.123158 django-payments-payu-1.4.0/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      349 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.123158 django-payments-payu-1.4.0/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4383 2024-03-19 14:15:03.000000 django-payments-payu-1.4.0/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      432 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      264 2021-10-28 14:11:55.000000 django-payments-payu-1.4.0/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-12 12:35:22.000000 django-payments-payu-1.4.0/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3318 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2432 2024-04-12 12:40:15.000000 django-payments-payu-1.4.0/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      181 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1553 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/Makefile
--rw-r--r--   0 petr      (1000) petr      (1000)     9421 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     6133 2024-04-12 12:35:22.000000 django-payments-payu-1.4.0/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/django_payments_payu.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     9421 2024-04-12 12:55:37.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      828 2024-04-12 12:55:38.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:55:37.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-03-19 14:34:07.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       14 2024-04-12 12:55:37.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8431 2022-03-17 16:38:53.000000 django-payments-payu-1.4.0/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      441 2024-04-12 12:52:42.000000 django-payments-payu-1.4.0/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      230 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2021-10-29 12:27:43.000000 django-payments-payu-1.4.0/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2022-03-17 16:38:53.000000 django-payments-payu-1.4.0/mypy.ini
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/payments_payu/
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-12 12:37:59.000000 django-payments-payu-1.4.0/payments_payu/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    29026 2024-04-12 12:36:09.000000 django-payments-payu-1.4.0/payments_payu/provider.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      155 2024-03-19 14:01:28.000000 django-payments-payu-1.4.0/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-03-19 13:42:55.000000 django-payments-payu-1.4.0/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      129 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2022-03-17 16:38:53.000000 django-payments-payu-1.4.0/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      319 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2255 2024-03-19 14:42:22.000000 django-payments-payu-1.4.0/setup.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      629 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3009 2024-03-19 14:15:03.000000 django-payments-payu-1.4.0/tests/settings.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    69794 2024-04-12 12:36:09.000000 django-payments-payu-1.4.0/tests/test_payu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      258 2022-03-17 16:39:01.000000 django-payments-payu-1.4.0/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      537 2021-10-28 14:11:55.000000 django-payments-payu-1.4.0/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.545273 django-payments-payu-1.4.1/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      349 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.545273 django-payments-payu-1.4.1/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4383 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      432 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      264 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3318 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2530 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      181 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1553 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/Makefile
+-rw-r--r--   0 petr      (1000) petr      (1000)     9519 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6133 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/django_payments_payu.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     9519 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      828 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       14 2024-05-14 08:24:50.000000 django-payments-payu-1.4.1/django_payments_payu.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8431 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      441 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      230 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/mypy.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/payments_payu/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/payments_payu/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    29190 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/payments_payu/provider.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      155 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      129 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      319 2024-05-14 08:24:50.553273 django-payments-payu-1.4.1/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2255 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:50.549273 django-payments-payu-1.4.1/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      629 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3009 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    78613 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/test_payu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      258 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      537 2024-05-14 08:24:49.000000 django-payments-payu-1.4.1/tox.ini
```

### Comparing `django-payments-payu-1.4.0/.github/workflows/main.yml` & `django-payments-payu-1.4.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/CONTRIBUTING.rst` & `django-payments-payu-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/HISTORY.rst` & `django-payments-payu-1.4.1/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 History
 -------
 
+1.4.1 (2024-05-14)
+******************
+* fix captured_amount not being saved when processing data
+
 1.4.0 (2024-04-12)
 ******************
 * fix backward compatibility by making PayuProvider's get_refund_description argument optional
 * add `renewal_triggered_by` parameter to `payment.set_renew_token`
 * make PayuProvider.refund fail if get_refund_description is not provided
 * make PayuProvider.refund raise PayuApiError if an unexpected response is received
 * deprecate the default value of get_refund_description; set it to a callable instead
```

### Comparing `django-payments-payu-1.4.0/LICENSE` & `django-payments-payu-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/Makefile` & `django-payments-payu-1.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/PKG-INFO` & `django-payments-payu-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-payments-payu
-Version: 1.4.0
+Version: 1.4.1
 Summary: PayU payments provider for django-payments
 Home-page: https://github.com/PetrDlouhy/django-payments-payu
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-payments-payu
 Classifier: Development Status :: 3 - Alpha
@@ -139,14 +139,18 @@
 
 
 
 
 History
 -------
 
+1.4.1 (2024-05-14)
+******************
+* fix captured_amount not being saved when processing data
+
 1.4.0 (2024-04-12)
 ******************
 * fix backward compatibility by making PayuProvider's get_refund_description argument optional
 * add `renewal_triggered_by` parameter to `payment.set_renew_token`
 * make PayuProvider.refund fail if get_refund_description is not provided
 * make PayuProvider.refund raise PayuApiError if an unexpected response is received
 * deprecate the default value of get_refund_description; set it to a callable instead
```

### Comparing `django-payments-payu-1.4.0/README.rst` & `django-payments-payu-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/django_payments_payu.egg-info/PKG-INFO` & `django-payments-payu-1.4.1/django_payments_payu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-payments-payu
-Version: 1.4.0
+Version: 1.4.1
 Summary: PayU payments provider for django-payments
 Home-page: https://github.com/PetrDlouhy/django-payments-payu
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-payments-payu
 Classifier: Development Status :: 3 - Alpha
@@ -139,14 +139,18 @@
 
 
 
 
 History
 -------
 
+1.4.1 (2024-05-14)
+******************
+* fix captured_amount not being saved when processing data
+
 1.4.0 (2024-04-12)
 ******************
 * fix backward compatibility by making PayuProvider's get_refund_description argument optional
 * add `renewal_triggered_by` parameter to `payment.set_renew_token`
 * make PayuProvider.refund fail if get_refund_description is not provided
 * make PayuProvider.refund raise PayuApiError if an unexpected response is received
 * deprecate the default value of get_refund_description; set it to a callable instead
```

### Comparing `django-payments-payu-1.4.0/django_payments_payu.egg-info/SOURCES.txt` & `django-payments-payu-1.4.1/django_payments_payu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/docs/Makefile` & `django-payments-payu-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/docs/conf.py` & `django-payments-payu-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/docs/make.bat` & `django-payments-payu-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/payments_payu/provider.py` & `django-payments-payu-1.4.1/payments_payu/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,14 +585,17 @@
                         status == PaymentStatus.CONFIRMED
                         and "totalAmount" in data["order"]
                     ):
                         payment.captured_amount = dequantize_price(
                             data["order"]["totalAmount"],
                             data["order"]["currencyCode"],
                         )
+                        payment.objects.filter(pk=payment.pk).update(
+                            captured_amount=payment.captured_amount
+                        )
                     payment.change_status(status)
                     return HttpResponse("ok", status=200)
         return HttpResponse("not ok", status=500)
 
     def process_data(self, payment, request, *args, **kwargs):
         self.request = request
```

### Comparing `django-payments-payu-1.4.0/runtests.py` & `django-payments-payu-1.4.1/runtests.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/setup.py` & `django-payments-payu-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/tests/README.md` & `django-payments-payu-1.4.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/tests/settings.py` & `django-payments-payu-1.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.4.0/tests/test_payu.py` & `django-payments-payu-1.4.1/tests/test_payu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import unicode_literals
 
 import contextlib
 import json
 import warnings
+from copy import deepcopy
 from decimal import Decimal
 from unittest import TestCase
 
 from mock import MagicMock, Mock, patch
 from payments import FraudStatus, PaymentStatus, PurchasedItem, RedirectNeeded
 
 from payments_payu.provider import PayuApiError, PayuProvider
@@ -29,17 +30,68 @@
     def __init__(self, json):
         self.json = json
 
     def __eq__(self, other):
         return self.json == json.loads(other)
 
 
+class PaymentQuerySet(Mock):
+    __payments = {}
+
+    def create(self, **kwargs):
+        if kwargs:
+            raise NotImplementedError(f"arguments not supported yet: {kwargs}")
+        id_ = max(self.__payments) + 1 if self.__payments else 1
+        self.__payments[id_] = {}
+        payment = Payment()
+        payment.id = id_
+        payment.save()
+        return payment
+
+    def get(self, *args, **kwargs):
+        if args or kwargs:
+            return self.filter(*args, **kwargs).get()
+        payment = Payment()
+        (payment_fields,) = self.__payments.values()
+        for payment_field_name, payment_field_value in payment_fields.items():
+            setattr(payment, payment_field_name, deepcopy(payment_field_value))
+        return payment
+
+    def filter(self, *args, pk=None, **kwargs):
+        if args or kwargs:
+            raise NotImplementedError(f"arguments not supported yet: {args}, {kwargs}")
+        if pk is not None:
+            return PaymentQuerySet(
+                {pk_: payment for pk_, payment in self.__payments.items() if pk_ == pk}
+            )
+        return self
+
+    def update(self, **kwargs):
+        for payment in self.__payments.values():
+            for field_name, field_value in kwargs.items():
+                if not any(
+                    field.name == field_name
+                    for field in Payment._meta.get_fields(
+                        include_parents=True, include_hidden=True
+                    )
+                ):
+                    raise NotImplementedError(
+                        f"updating unknown field not supported yet: {field_name}"
+                    )
+                payment[field_name] = deepcopy(field_value)
+
+    def delete(self):
+        self.__payments.clear()
+
+
 class Payment(Mock):
     UNSET = object()
 
+    objects = PaymentQuerySet()
+
     id = 1
     description = "payment"
     currency = "USD"
     delivery = Decimal(10)
     status = PaymentStatus.WAITING
     fraud_status = FraudStatus.UNKNOWN
     tax = Decimal(10)
@@ -60,21 +112,28 @@
                 "capture": {"href": "http://capture.com"},
                 "refund": {"href": "http://refund.com"},
                 "execute": {"href": "http://execute.com"},
             }
         }
     )
 
-    def change_fraud_status(self, status, message=""):
+    @property
+    def pk(self):
+        return self.id
+
+    def change_fraud_status(self, status, message="", commit=True):
         self.fraud_status = status
         self.message = message
+        if commit:
+            self.save()
 
     def change_status(self, status, message=""):
         self.status = status
         self.message = message
+        self.save(update_fields=["status", "message"])
 
     def get_failure_url(self):
         return "http://cancel.com"
 
     def get_process_url(self):
         return "/process_url/token"
 
@@ -106,20 +165,73 @@
         self.token = token
         self.card_expire_year = card_expire_year
         self.card_expire_month = card_expire_month
         self.card_masked_number = card_masked_number
         self.automatic_renewal = automatic_renewal
         self.renewal_triggered_by = renewal_triggered_by
 
+    def save(self, *args, update_fields=None, **kwargs):
+        if args or kwargs:
+            raise NotImplementedError(f"arguments not supported yet: {args}, {kwargs}")
+        if update_fields is None:
+            update_fields = {
+                field.name
+                for field in self._meta.get_fields(
+                    include_parents=True, include_hidden=True
+                )
+            }
+        Payment.objects.filter(pk=self.pk).update(
+            **{field: getattr(self, field) for field in update_fields}
+        )
+
+    def refresh_from_db(self, *args, **kwargs):
+        if args or kwargs:
+            raise NotImplementedError(f"arguments not supported yet: {args}, {kwargs}")
+        payment_from_db = Payment.objects.get(pk=self.pk)
+        for field in self._meta.get_fields(include_parents=True, include_hidden=True):
+            field_value_from_db = getattr(payment_from_db, field.name)
+            setattr(self, field.name, field_value_from_db)
+
+    class Meta(Mock):
+        def get_fields(self, include_parents=True, include_hidden=False):
+            fields = []
+            for field_name in {
+                "id",
+                "description",
+                "currency",
+                "delivery",
+                "status",
+                "fraud_status",
+                "tax",
+                "total",
+                "billing_first_name",
+                "billing_last_name",
+                "billing_email",
+                "captured_amount",
+                "variant",
+                "transaction_id",
+                "message",
+                "customer_ip_address",
+                "token",
+                "extra_data",
+            }:
+                field = Mock()
+                field.name = field_name
+                fields.append(field)
+            return tuple(fields)
+
+    _meta = Meta()
+
 
 class TestPayuProvider(TestCase):
     urls = "myapp.test_urls"
 
     def setUp(self):
-        self.payment = Payment()
+        Payment.objects.delete()
+        self.payment = Payment.objects.create()
 
     def set_up_provider(self, recurring, express, **kwargs):
         with patch("requests.post") as mocked_post:
             data = MagicMock()
             data = '{"access_token": "test_access_token"}'
             json.loads(data)
             post = MagicMock()
@@ -625,14 +737,17 @@
             payment=self.payment, request=mocked_request
         )
         self.assertEqual(ret_val.__class__.__name__, "HttpResponse")
         self.assertEqual(ret_val.status_code, 200)
         self.assertEqual(ret_val.content, b"ok")
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_notification_cancelled(self):
         """Test processing PayU cancelled notification"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         self.payment.transaction_id = "123"
@@ -659,14 +774,17 @@
         )
 
         self.assertEqual(ret_val.__class__.__name__, "HttpResponse")
         self.assertEqual(ret_val.status_code, 200)
         self.assertEqual(ret_val.content, b"ok")
         self.assertEqual(self.payment.status, PaymentStatus.REJECTED)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.REJECTED)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_notification_refund(self):
         """Test processing PayU refund notification"""
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
 
@@ -695,14 +813,18 @@
         )
         self.assertEqual(ret_val.__class__.__name__, "HttpResponse")
         self.assertEqual(ret_val.status_code, 200)
         self.assertEqual(ret_val.content, b"ok")
         self.assertEqual(self.payment.status, PaymentStatus.REFUNDED)
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.REFUNDED)
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
 
     def test_process_notification_partial_refund(self):
         """Test processing PayU partial refund notification"""
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.total = 220
         self.payment.captured_amount = self.payment.total
         self.payment.save()
@@ -730,14 +852,17 @@
         mocked_request.status_code = 200
         ret_val = self.provider.process_data(
             payment=self.payment, request=mocked_request
         )
         self.assertEqual(ret_val.__class__.__name__, "HttpResponse")
         self.assertEqual(ret_val.status_code, 200)
         self.assertEqual(ret_val.content, b"ok")
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal("110"))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.payment.refresh_from_db()
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal("110"))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
 
     def test_process_notification_refund_not_finalized(self):
         """Test processing PayU partial refund notification"""
@@ -788,14 +913,17 @@
             payment=self.payment, request=mocked_request
         )
         self.assertEqual(ret_val.__class__.__name__, "HttpResponse")
         self.assertEqual(ret_val.status_code, 200)
         self.assertEqual(ret_val.content, b"ok")
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(self.payment.captured_amount, Decimal("2"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(self.payment.captured_amount, Decimal("2"))
 
     def test_process_notification_error(self):
         """Test processing PayU notification with wrong signature"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         mocked_request = MagicMock()
@@ -808,14 +936,17 @@
             payment=self.payment, request=mocked_request
         )
         self.assertEqual(ret_val.__class__.__name__, "HttpResponse")
         self.assertEqual(ret_val.status_code, 500)
         self.assertEqual(ret_val.content, b"not ok")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.WAITING)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_notification_error_malformed_post(self):
         """Test processing PayU notification with malformed POST"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         mocked_request = MagicMock()
@@ -881,14 +1012,17 @@
                 headers={
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.WAITING)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_renew(self):
         """Test processing renew"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         with patch("requests.post") as mocked_post:
@@ -945,14 +1079,17 @@
                 headers={
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.WAITING)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_renew_card_on_file(self):
         """Test processing renew"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         self.provider.card_on_file = True
@@ -1010,14 +1147,17 @@
                 headers={
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.WAITING)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_auto_complete_recurring(self):
         """Test processing renew. The function should return 'success' string, if nothing is required from user."""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         with patch("requests.post") as mocked_post:
@@ -1025,14 +1165,17 @@
             post.text = '{"status": {"statusCode": "SUCCESS"}, "orderId": 123}'
             post.status_code = 200
             mocked_post.return_value = post
             redirect = self.provider.auto_complete_recurring(self.payment)
             self.assertEqual(redirect, "success")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.WAITING)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_auto_complete_recurring_cvv2(self):
         """Test processing renew when cvv2 form is required - it should return the payment processing URL"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         with patch("requests.post") as mocked_post:
@@ -1046,14 +1189,17 @@
             )
             post.status_code = 200
             mocked_post.return_value = post
             redirect = self.provider.auto_complete_recurring(self.payment)
             self.assertEqual(redirect, "https://example.com/payment/token")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.WAITING)
+        self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_delete_card_token(self):
         """Test delete_card_token()"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         self.payment.transaction_id = "1234"
@@ -1112,14 +1258,16 @@
                 "http://mock.url/api/v2_1/orders/1234",
                 headers={
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.REJECTED)
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.REJECTED)
 
     def test_reject_order_error(self):
         """Test processing renew"""
         self.set_up_provider(
             True, True, get_refund_description=lambda payment, amount: "test"
         )
         self.payment.transaction_id = "1234"
@@ -1134,14 +1282,16 @@
                 "http://mock.url/api/v2_1/orders/1234",
                 headers={
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.status, PaymentStatus.WAITING)
 
     def test_refund(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
                 True,
                 True,
@@ -1199,24 +1349,29 @@
             ext_refund_id="ext 1234 110",
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment, Decimal(110))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(amount, Decimal(110))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(210))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses,
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [payment_extra_data_refund_response_previous, refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(210))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
             [payment_extra_data_refund_response_previous, refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_no_amount(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
@@ -1257,24 +1412,30 @@
             ext_refund_id="ext 1234 None",
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment)
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(amount, Decimal(220))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses, [refund_request_response_body]
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_no_get_refund_ext_id(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
@@ -1316,24 +1477,30 @@
 
         with refund_request_patch as refund_request_mock:
             with patch(
                 "uuid.uuid4", return_value="caf231c5-cbc1-4af3-96b7-95798b1cb846"
             ):
                 amount = self.provider.refund(self.payment, Decimal(110))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(amount, Decimal(110))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses, [refund_request_response_body]
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_no_ext_id(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
@@ -1372,24 +1539,30 @@
             ext_refund_id=None,
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment, Decimal(110))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(amount, Decimal(110))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses, [refund_request_response_body]
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_no_ext_id_twice(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
@@ -1429,25 +1602,30 @@
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount1 = self.provider.refund(self.payment, Decimal(200))
             amount2 = self.provider.refund(self.payment, Decimal(200))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 2)
         self.assertEqual(amount2, amount1)
         self.assertEqual(amount2, Decimal(200))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses,
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body, refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
             [refund_request_response_body, refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_finalized(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
@@ -1488,24 +1666,30 @@
             ext_refund_id="ext 1234 110",
             response_body=refund_request_response_body,
         )
 
         with refund_request_patch as refund_request_mock:
             amount = self.provider.refund(self.payment, Decimal(110))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(amount, Decimal(110))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses, [refund_request_response_body]
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_canceled(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
@@ -1548,23 +1732,29 @@
 
         with self.assertRaisesRegex(
             ValueError, "refund 5000009987 of payment 1 canceled"
         ):
             with refund_request_patch as refund_request_mock:
                 self.provider.refund(self.payment, Decimal(110))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses, [refund_request_response_body]
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_error(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
@@ -1603,23 +1793,29 @@
             r"statusCode=OPENPAYU_BUSINESS_ERROR, "
             r"codeLiteral=NO_BALANCE, "
             r"statusDesc=Lack of funds in account",
         ):
             with refund_request_patch as refund_request_mock:
                 self.provider.refund(self.payment, Decimal(110))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data)[
-            "refund_responses"
-        ]
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
-            payment_extra_data_refund_responses, [refund_request_response_body]
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
+        )
+        self.payment.refresh_from_db()
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertEqual(
+            json.loads(self.payment.extra_data)["refund_responses"],
+            [refund_request_response_body],
         )
         self.assertFalse(caught_warnings)
 
     def test_refund_no_get_refund_description(self):
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             self.set_up_provider(
@@ -1631,21 +1827,27 @@
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
 
         with self.assertRaisesRegex(ValueError, r"^get_refund_description not set"):
             self.provider.refund(self.payment, Decimal(110))
 
-        payment_extra_data_refund_responses = json.loads(self.payment.extra_data).get(
-            "refund_responses", []
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertFalse(
+            json.loads(self.payment.extra_data).get("refund_responses", [])
         )
+        self.payment.refresh_from_db()
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
-        self.assertFalse(payment_extra_data_refund_responses)
+        self.assertFalse(
+            json.loads(self.payment.extra_data).get("refund_responses", [])
+        )
         self.assertEqual(len(caught_warnings), 1)
         self.assertTrue(issubclass(caught_warnings[0].category, DeprecationWarning))
         self.assertEqual(
             str(caught_warnings[0].message),
             "A default value of get_refund_description is deprecated. Set it to a callable instead.",
         )
```

### Comparing `django-payments-payu-1.4.0/tox.ini` & `django-payments-payu-1.4.1/tox.ini`

 * *Files identical despite different names*

