# Comparing `tmp/django-payments-payu-1.3.1.tar.gz` & `tmp/django-payments-payu-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-payments-payu-1.3.1.tar", last modified: Tue Mar 19 14:45:41 2024, max compression
+gzip compressed data, was "django-payments-payu-1.4.0.tar", last modified: Fri Apr 12 12:55:38 2024, max compression
```

## Comparing `django-payments-payu-1.3.1.tar` & `django-payments-payu-1.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.848207 django-payments-payu-1.3.1/
--rw-rw-r--   0 petr      (1000) petr      (1000)      146 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.844207 django-payments-payu-1.3.1/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      349 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.844207 django-payments-payu-1.3.1/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4383 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      432 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      264 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      140 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3318 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1532 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      181 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1553 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/Makefile
--rw-r--r--   0 petr      (1000) petr      (1000)     8332 2024-03-19 14:45:41.848207 django-payments-payu-1.3.1/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     5944 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.848207 django-payments-payu-1.3.1/django_payments_payu.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     8332 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/django_payments_payu.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      828 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/django_payments_payu.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/django_payments_payu.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/django_payments_payu.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       14 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/django_payments_payu.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.844207 django-payments-payu-1.3.1/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8431 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      441 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      230 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/mypy.ini
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.848207 django-payments-payu-1.3.1/payments_payu/
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/payments_payu/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    28512 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/payments_payu/provider.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      155 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      129 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      319 2024-03-19 14:45:41.848207 django-payments-payu-1.3.1/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2255 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/setup.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.848207 django-payments-payu-1.3.1/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)      629 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/tests/README.md
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/tests/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     3009 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/tests/settings.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    64513 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/tests/test_payu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      258 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      537 2024-03-19 14:45:41.000000 django-payments-payu-1.3.1/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      146 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.123158 django-payments-payu-1.4.0/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      349 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.123158 django-payments-payu-1.4.0/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4383 2024-03-19 14:15:03.000000 django-payments-payu-1.4.0/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      432 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      264 2021-10-28 14:11:55.000000 django-payments-payu-1.4.0/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-12 12:35:22.000000 django-payments-payu-1.4.0/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3318 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2432 2024-04-12 12:40:15.000000 django-payments-payu-1.4.0/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      181 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1553 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/Makefile
+-rw-r--r--   0 petr      (1000) petr      (1000)     9421 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6133 2024-04-12 12:35:22.000000 django-payments-payu-1.4.0/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/django_payments_payu.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     9421 2024-04-12 12:55:37.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)      828 2024-04-12 12:55:38.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:55:37.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-03-19 14:34:07.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       14 2024-04-12 12:55:37.000000 django-payments-payu-1.4.0/django_payments_payu.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8431 2022-03-17 16:38:53.000000 django-payments-payu-1.4.0/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      441 2024-04-12 12:52:42.000000 django-payments-payu-1.4.0/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      230 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2021-10-29 12:27:43.000000 django-payments-payu-1.4.0/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2022-03-17 16:38:53.000000 django-payments-payu-1.4.0/mypy.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/payments_payu/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-12 12:37:59.000000 django-payments-payu-1.4.0/payments_payu/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    29026 2024-04-12 12:36:09.000000 django-payments-payu-1.4.0/payments_payu/provider.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      155 2024-03-19 14:01:28.000000 django-payments-payu-1.4.0/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-03-19 13:42:55.000000 django-payments-payu-1.4.0/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      129 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2022-03-17 16:38:53.000000 django-payments-payu-1.4.0/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      319 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2255 2024-03-19 14:42:22.000000 django-payments-payu-1.4.0/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:55:38.127158 django-payments-payu-1.4.0/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      629 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/tests/README.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2020-05-30 10:03:47.000000 django-payments-payu-1.4.0/tests/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3009 2024-03-19 14:15:03.000000 django-payments-payu-1.4.0/tests/settings.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    69794 2024-04-12 12:36:09.000000 django-payments-payu-1.4.0/tests/test_payu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      258 2022-03-17 16:39:01.000000 django-payments-payu-1.4.0/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      537 2021-10-28 14:11:55.000000 django-payments-payu-1.4.0/tox.ini
```

### Comparing `django-payments-payu-1.3.1/.github/workflows/main.yml` & `django-payments-payu-1.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/CONTRIBUTING.rst` & `django-payments-payu-1.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/LICENSE` & `django-payments-payu-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/Makefile` & `django-payments-payu-1.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/PKG-INFO` & `django-payments-payu-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-payments-payu
-Version: 1.3.1
+Version: 1.4.0
 Summary: PayU payments provider for django-payments
 Home-page: https://github.com/PetrDlouhy/django-payments-payu
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-payments-payu
 Classifier: Development Status :: 3 - Alpha
@@ -78,15 +78,15 @@
    :shop_name:              Name of the shop send to the API
    :sandbox:                if ``True``, set the endpoint to sandbox
    :endpoint:               endpoint URL, if not set, the will be automatically set based on `sandbox` settings
    :recurring_payments:     enable recurring payments, only valid with ``express_payments=True``, see bellow for additional setup, that is needed
    :express_payments:       use PayU express form
    :widget_branding:        tell express form to show PayU branding
    :store_card:             (default: False) whether PayU should store the card
-   :get_refund_description: A mandatory callable that is called with two keyword arguments `payment` and `amount` in order to get the string description of the particular refund whenever ``provider.refund(payment, amount)`` is called.
+   :get_refund_description: An optional callable that is called with two keyword arguments `payment` and `amount` in order to get the string description of the particular refund whenever ``provider.refund(payment, amount)`` is called. The callable is optional because of backwards compatibility. However, if it is not set, an attempt to refund raises an exception. A default value of `get_refund_description` is deprecated.
    :get_refund_ext_id:      An optional callable that is called with two keyword arguments `payment` and `amount` in order to get the External string refund ID of the particular refund whenever ``provider.refund(payment, amount)`` is called. If ``None`` is returned, no External refund ID is set. An External refund ID is not necessary if partial refunds won't be performed more than once per second. Otherwise, a unique ID is recommended since `PayuProvider.refund` is idempotent and if exactly same data will be provided, it will return the result of the already previously performed refund instead of performing a new refund. Defaults to a random UUID version 4 in the standard form.
 
 
    NOTE: notifications about the payment status from PayU are requested to be sent to `django-payments` `process_payment` url. The request from PayU can fail for several reasons (i.e. it can be blocked by proxy). Use "Show reports" page in PayU administration to get more information about the requests.
 
 
 **Recurring payments**:
@@ -139,19 +139,35 @@
 
 
 
 
 History
 -------
 
+1.4.0 (2024-04-12)
+******************
+* fix backward compatibility by making PayuProvider's get_refund_description argument optional
+* add `renewal_triggered_by` parameter to `payment.set_renew_token`
+* make PayuProvider.refund fail if get_refund_description is not provided
+* make PayuProvider.refund raise PayuApiError if an unexpected response is received
+* deprecate the default value of get_refund_description; set it to a callable instead
+* deprecate `automatic_renewal` parameter of `payment.set_renew_token`; use `renewal_triggered_by` parameter instead
+* deprecate `None` value of `renewal_triggered_by` parameter of `payment.set_renew_token`; set `"user"`/`"task"`/`"other"` instead
+
+1.3.1 (2024-03-19)
+******************
+* Fix description on PyPI
+
 1.3.0 (2024-03-19)
 ******************
+* add get_refund_description and get_refund_ext_id arguments to PayuProvider
 * add PayuProvider.refund
 * update payment.captured_amount only when order is completed
 * subtract refunds from payment.captured_amount rather than from payment.total
+* rename PayuProvider.payu_api_order_url to payu_api_orders_url
 * tests for Django 2.2-5.0 Python 3.7-3.12
 
 1.2.4 (2022-03-17)
 ******************
 * treat partial refunds
 * tests for Django 2.2-4.0 Python 3.7-3.10
```

### Comparing `django-payments-payu-1.3.1/README.rst` & `django-payments-payu-1.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
    :shop_name:              Name of the shop send to the API
    :sandbox:                if ``True``, set the endpoint to sandbox
    :endpoint:               endpoint URL, if not set, the will be automatically set based on `sandbox` settings
    :recurring_payments:     enable recurring payments, only valid with ``express_payments=True``, see bellow for additional setup, that is needed
    :express_payments:       use PayU express form
    :widget_branding:        tell express form to show PayU branding
    :store_card:             (default: False) whether PayU should store the card
-   :get_refund_description: A mandatory callable that is called with two keyword arguments `payment` and `amount` in order to get the string description of the particular refund whenever ``provider.refund(payment, amount)`` is called.
+   :get_refund_description: An optional callable that is called with two keyword arguments `payment` and `amount` in order to get the string description of the particular refund whenever ``provider.refund(payment, amount)`` is called. The callable is optional because of backwards compatibility. However, if it is not set, an attempt to refund raises an exception. A default value of `get_refund_description` is deprecated.
    :get_refund_ext_id:      An optional callable that is called with two keyword arguments `payment` and `amount` in order to get the External string refund ID of the particular refund whenever ``provider.refund(payment, amount)`` is called. If ``None`` is returned, no External refund ID is set. An External refund ID is not necessary if partial refunds won't be performed more than once per second. Otherwise, a unique ID is recommended since `PayuProvider.refund` is idempotent and if exactly same data will be provided, it will return the result of the already previously performed refund instead of performing a new refund. Defaults to a random UUID version 4 in the standard form.
 
 
    NOTE: notifications about the payment status from PayU are requested to be sent to `django-payments` `process_payment` url. The request from PayU can fail for several reasons (i.e. it can be blocked by proxy). Use "Show reports" page in PayU administration to get more information about the requests.
 
 
 **Recurring payments**:
```

### Comparing `django-payments-payu-1.3.1/django_payments_payu.egg-info/PKG-INFO` & `django-payments-payu-1.4.0/django_payments_payu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-payments-payu
-Version: 1.3.1
+Version: 1.4.0
 Summary: PayU payments provider for django-payments
 Home-page: https://github.com/PetrDlouhy/django-payments-payu
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-payments-payu
 Classifier: Development Status :: 3 - Alpha
@@ -78,15 +78,15 @@
    :shop_name:              Name of the shop send to the API
    :sandbox:                if ``True``, set the endpoint to sandbox
    :endpoint:               endpoint URL, if not set, the will be automatically set based on `sandbox` settings
    :recurring_payments:     enable recurring payments, only valid with ``express_payments=True``, see bellow for additional setup, that is needed
    :express_payments:       use PayU express form
    :widget_branding:        tell express form to show PayU branding
    :store_card:             (default: False) whether PayU should store the card
-   :get_refund_description: A mandatory callable that is called with two keyword arguments `payment` and `amount` in order to get the string description of the particular refund whenever ``provider.refund(payment, amount)`` is called.
+   :get_refund_description: An optional callable that is called with two keyword arguments `payment` and `amount` in order to get the string description of the particular refund whenever ``provider.refund(payment, amount)`` is called. The callable is optional because of backwards compatibility. However, if it is not set, an attempt to refund raises an exception. A default value of `get_refund_description` is deprecated.
    :get_refund_ext_id:      An optional callable that is called with two keyword arguments `payment` and `amount` in order to get the External string refund ID of the particular refund whenever ``provider.refund(payment, amount)`` is called. If ``None`` is returned, no External refund ID is set. An External refund ID is not necessary if partial refunds won't be performed more than once per second. Otherwise, a unique ID is recommended since `PayuProvider.refund` is idempotent and if exactly same data will be provided, it will return the result of the already previously performed refund instead of performing a new refund. Defaults to a random UUID version 4 in the standard form.
 
 
    NOTE: notifications about the payment status from PayU are requested to be sent to `django-payments` `process_payment` url. The request from PayU can fail for several reasons (i.e. it can be blocked by proxy). Use "Show reports" page in PayU administration to get more information about the requests.
 
 
 **Recurring payments**:
@@ -139,19 +139,35 @@
 
 
 
 
 History
 -------
 
+1.4.0 (2024-04-12)
+******************
+* fix backward compatibility by making PayuProvider's get_refund_description argument optional
+* add `renewal_triggered_by` parameter to `payment.set_renew_token`
+* make PayuProvider.refund fail if get_refund_description is not provided
+* make PayuProvider.refund raise PayuApiError if an unexpected response is received
+* deprecate the default value of get_refund_description; set it to a callable instead
+* deprecate `automatic_renewal` parameter of `payment.set_renew_token`; use `renewal_triggered_by` parameter instead
+* deprecate `None` value of `renewal_triggered_by` parameter of `payment.set_renew_token`; set `"user"`/`"task"`/`"other"` instead
+
+1.3.1 (2024-03-19)
+******************
+* Fix description on PyPI
+
 1.3.0 (2024-03-19)
 ******************
+* add get_refund_description and get_refund_ext_id arguments to PayuProvider
 * add PayuProvider.refund
 * update payment.captured_amount only when order is completed
 * subtract refunds from payment.captured_amount rather than from payment.total
+* rename PayuProvider.payu_api_order_url to payu_api_orders_url
 * tests for Django 2.2-5.0 Python 3.7-3.12
 
 1.2.4 (2022-03-17)
 ******************
 * treat partial refunds
 * tests for Django 2.2-4.0 Python 3.7-3.10
```

### Comparing `django-payments-payu-1.3.1/django_payments_payu.egg-info/SOURCES.txt` & `django-payments-payu-1.4.0/django_payments_payu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/docs/Makefile` & `django-payments-payu-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/docs/conf.py` & `django-payments-payu-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/docs/make.bat` & `django-payments-payu-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/payments_payu/provider.py` & `django-payments-payu-1.4.0/payments_payu/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hashlib
 import json
 import logging
 import uuid
+import warnings
 from decimal import ROUND_HALF_UP, Decimal
 from urllib.parse import urljoin
 
 import requests
 from django import forms
 from django.http.response import HttpResponse, HttpResponseRedirect
 from django.utils.html import format_html
@@ -181,15 +182,24 @@
         self.payu_api_orders_url = urljoin(self.payu_api_url, "orders/")
         self.payu_api_paymethods_url = urljoin(self.payu_api_url, "paymethods/")
         self.payu_widget_branding = kwargs.pop("widget_branding", False)
         self.payu_store_card = kwargs.pop("store_card", False)
         self.payu_shop_name = kwargs.pop("shop_name", "")
         self.grant_type = kwargs.pop("grant_type", "client_credentials")
         self.recurring_payments = kwargs.pop("recurring_payments", False)
-        self.get_refund_description = kwargs.pop("get_refund_description")
+        self.get_refund_description = kwargs.pop(
+            "get_refund_description",
+            # TODO: The default is deprecated. Remove in the next major release.
+            None,
+        )
+        if self.get_refund_description is None:
+            warnings.warn(
+                "A default value of get_refund_description is deprecated. Set it to a callable instead.",
+                DeprecationWarning,
+            )
         self.get_refund_ext_id = kwargs.pop(
             "get_refund_ext_id", lambda payment, amount: str(uuid.uuid4())
         )
 
         # Use card on file paremeter instead of recurring.
         # PayU asks CVV2 every time with this setting which can be used for testing purposes.
         self.card_on_file = kwargs.pop("card_on_file", False)
@@ -427,15 +437,15 @@
                     ],
                     card_expire_month=response_dict["payMethods"]["payMethod"]["card"][
                         "expirationMonth"
                     ],
                     card_masked_number=response_dict["payMethods"]["payMethod"]["card"][
                         "number"
                     ],
-                    automatic_renewal=self.recurring_payments,
+                    renewal_triggered_by="task" if self.recurring_payments else "user",
                 )
             add_extra_data(payment, {"card_response": response_dict})
 
             if response_dict["status"]["statusCode"] == "SUCCESS":
                 if "redirectUri" in response_dict:
                     payment.pay_link = response_dict["redirectUri"]
                     payment.save()
@@ -600,14 +610,17 @@
             )
         else:
             return HttpResponse(
                 "request not recognized by django-payments-payu provider", status=500
             )
 
     def refund(self, payment, amount=None):
+        if self.get_refund_description is None:
+            raise ValueError("get_refund_description not set")
+
         request_url = self._get_payu_api_order_url(payment.transaction_id) + "/refunds"
 
         request_data = {
             "refund": {
                 "currencyCode": payment.currency,
                 "description": self.get_refund_description(
                     payment=payment, amount=amount
@@ -640,48 +653,48 @@
         except Exception:
             refund_id = None
 
         try:
             response_status = dict(response["status"])
             response_status_code = response_status["statusCode"]
         except Exception:
-            raise ValueError(
+            raise PayuApiError(
                 f"invalid response to refund {refund_id or '???'} of payment {payment.id}: {response}"
             )
         if response_status_code != "SUCCESS":
             raise ValueError(
                 f"refund {refund_id or '???'} of payment {payment.id} failed: "
                 f"code={response_status.get('code', '???')}, "
                 f"statusCode={response_status_code}, "
                 f"codeLiteral={response_status.get('codeLiteral', '???')}, "
                 f"statusDesc={response_status.get('statusDesc', '???')}"
             )
         if refund_id is None:
-            raise ValueError(
+            raise PayuApiError(
                 f"invalid response to refund of payment {payment.id}: {response}"
             )
 
         try:
             refund_order_id = response["orderId"]
             refund_status = refund["status"]
             refund_currency = refund["currencyCode"]
             refund_amount = dequantize_price(refund["amount"], refund_currency)
         except Exception:
-            raise ValueError(
+            raise PayuApiError(
                 f"invalid response to refund {refund_id} of payment {payment.id}: {response}"
             )
         if refund_order_id != payment.transaction_id:
             raise NotImplementedError(
                 f"response of refund {refund_id} of payment {payment.id} containing a different order_id "
                 f"not supported yet: {refund_order_id}"
             )
         if refund_status == "CANCELED":
             raise ValueError(f"refund {refund_id} of payment {payment.id} canceled")
         elif refund_status not in {"PENDING", "FINALIZED"}:
-            raise ValueError(
+            raise PayuApiError(
                 f"invalid status of refund {refund_id} of payment {payment.id}"
             )
         if refund_currency != payment.currency:
             raise NotImplementedError(
                 f"refund {refund_id} of payment {payment.id} in different currency not supported yet: "
                 f"{refund_currency}"
             )
```

### Comparing `django-payments-payu-1.3.1/runtests.py` & `django-payments-payu-1.4.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/setup.py` & `django-payments-payu-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/tests/README.md` & `django-payments-payu-1.4.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/tests/settings.py` & `django-payments-payu-1.4.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-payments-payu-1.3.1/tests/test_payu.py` & `django-payments-payu-1.4.0/tests/test_payu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import unicode_literals
 
 import contextlib
 import json
+import warnings
 from decimal import Decimal
 from unittest import TestCase
 
 from mock import MagicMock, Mock, patch
 from payments import FraudStatus, PaymentStatus, PurchasedItem, RedirectNeeded
 
 from payments_payu.provider import PayuApiError, PayuProvider
@@ -29,14 +30,16 @@
         self.json = json
 
     def __eq__(self, other):
         return self.json == json.loads(other)
 
 
 class Payment(Mock):
+    UNSET = object()
+
     id = 1
     description = "payment"
     currency = "USD"
     delivery = Decimal(10)
     status = PaymentStatus.WAITING
     fraud_status = FraudStatus.UNKNOWN
     tax = Decimal(10)
@@ -93,36 +96,32 @@
 
     def set_renew_token(
         self,
         token,
         card_expire_year=None,
         card_expire_month=None,
         card_masked_number=None,
-        automatic_renewal=None,
+        automatic_renewal=UNSET,
+        renewal_triggered_by=UNSET,
     ):
         self.token = token
         self.card_expire_year = card_expire_year
         self.card_expire_month = card_expire_month
         self.card_masked_number = card_masked_number
         self.automatic_renewal = automatic_renewal
+        self.renewal_triggered_by = renewal_triggered_by
 
 
 class TestPayuProvider(TestCase):
     urls = "myapp.test_urls"
 
     def setUp(self):
         self.payment = Payment()
 
-    def set_up_provider(
-        self,
-        recurring,
-        express,
-        get_refund_description=lambda payment, amount: "test",
-        **kwargs,
-    ):
+    def set_up_provider(self, recurring, express, **kwargs):
         with patch("requests.post") as mocked_post:
             data = MagicMock()
             data = '{"access_token": "test_access_token"}'
             json.loads(data)
             post = MagicMock()
             post.text = data
             post.status_code = 200
@@ -130,40 +129,45 @@
             self.provider = PayuProvider(
                 client_secret=SECRET,
                 second_key=SECOND_KEY,
                 pos_id=POS_ID,
                 base_payu_url="http://mock.url/",
                 recurring_payments=recurring,
                 express_payments=express,
-                get_refund_description=get_refund_description,
                 **kwargs,
             )
 
     def test_redirect_to_recurring_payment(self):
         """Test that if the payment recurrence is set, the user is redirected to renew payment form"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         form = self.provider.get_form(payment=self.payment)
         self.assertEqual(form.__class__.__name__, "RenewPaymentForm")
         self.assertEqual(form.action, "https://example.com/process_url/token")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_redirect_payu(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = '{"redirectUri": "test_redirect_uri", "status": {"statusCode": "SUCCESS"}, "orderId": 123}'
             post.status_code = 200
             mocked_post.return_value = post
             with self.assertRaises(RedirectNeeded) as context:
                 self.provider.get_form(payment=self.payment)
             self.assertEqual(context.exception.args[0], "test_redirect_uri")
 
     def test_redirect_payu_store_token(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "test_redirect_uri",
                     "status": {"statusCode": "SUCCESS"},
                     "orderId": 123,
@@ -184,18 +188,21 @@
             with self.assertRaises(RedirectNeeded) as context:
                 self.provider.get_form(payment=self.payment)
             self.assertEqual(context.exception.args[0], "test_redirect_uri")
             self.assertEqual(self.payment.token, 1211)
             self.assertEqual(self.payment.card_expire_year, 2021)
             self.assertEqual(self.payment.card_expire_month, 1)
             self.assertEqual(self.payment.card_masked_number, "1234xxx")
-            self.assertEqual(self.payment.automatic_renewal, True)
+            self.assertEqual(self.payment.automatic_renewal, Payment.UNSET)
+            self.assertEqual(self.payment.renewal_triggered_by, "task")
 
     def test_redirect_payu_unknown_status(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post_text = {
                 "redirectUri": "test_redirect_uri",
                 "status": {"statusCode": "FOO", "codeLiteral": "Foo code"},
                 "orderId": 123,
             }
@@ -240,15 +247,17 @@
                 headers={
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
 
     def test_redirect_payu_bussiness_error(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post_text = {
                 "redirectUri": "test_redirect_uri",
                 "status": {"statusCode": "BUSINESS_ERROR", "codeLiteral": "Foo code"},
                 "orderId": 123,
             }
@@ -257,15 +266,17 @@
             mocked_post.return_value = post
             with self.assertRaises(RedirectNeeded) as context:
                 self.provider.get_form(payment=self.payment)
             self.assertEqual(context.exception.args[0], "http://cancel.com")
             self.assertEqual(self.payment.fraud_status, FraudStatus.REJECT)
 
     def test_redirect_payu_duplicate_order(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.status = PaymentStatus.CONFIRMED
         self.payment.save()
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post_text = {
                 "redirectUri": "test_redirect_uri",
                 "status": {
@@ -278,15 +289,17 @@
             post.status_code = 200
             mocked_post.return_value = post
             with self.assertRaises(RedirectNeeded) as context:
                 self.provider.get_form(payment=self.payment)
             self.assertEqual(context.exception.args[0], "")
 
     def test_redirect_payu_no_status_code(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post_text = {
                 "redirectUri": "test_redirect_uri",
                 "orderId": 123,
             }
             post.text = json.dumps(post_text)
@@ -330,15 +343,17 @@
                 headers={
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
 
     def test_redirect_payu_unauthorized_status(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "test_redirect_uri",
                     "status": {"statusCode": "UNAUTHORIZED"},
                     "orderId": 123,
@@ -361,15 +376,17 @@
                     "client_id": "123abc",
                     "client_secret": "123abc",
                 },
                 headers={"Content-Type": "application/x-www-form-urlencoded"},
             )
 
     def test_get_access_token_trusted_merchant(self):
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "test_redirect_uri",
                     "token_type": "test_token_type",
                     "access_token": "test_access_token",
@@ -392,15 +409,17 @@
                     "ext_customer_id": 123,
                 },
                 headers={"Content-Type": "application/x-www-form-urlencoded"},
             )
 
     def test_redirect_cvv_form(self):
         """Test redirection to CVV form if requested by PayU"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "test_redirect_uri",
                     "status": {"statusCode": "WARNING_CONTINUE_CVV"},
                     "orderId": 123,
@@ -451,15 +470,17 @@
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
 
     def test_showing_cvv_form(self):
         """Test redirection to CVV form if requested by PayU"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.extra_data = json.dumps({"cvv_url": "foo_url"})
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "http://test_redirect_uri.com/",
                     "status": {"statusCode": "SUCCESS"},
@@ -479,15 +500,17 @@
             )
             self.assertTrue(
                 "cvv-url=foo_url" in form.fields["script"].widget.render("a", "b")
             )
 
     def test_redirect_3ds_form(self):
         """Test redirection to 3DS page if requested by PayU"""
-        self.set_up_provider(True, False)
+        self.set_up_provider(
+            True, False, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "test_redirect_uri",
                     "status": {"statusCode": "WARNING_CONTINUE_3DS"},
                     "orderId": 123,
@@ -533,15 +556,17 @@
                     "Content-Type": "application/json",
                 },
             )
             self.assertEqual(context.exception.args[0], "test_redirect_uri")
 
     def test_payu_renew_form(self):
         """Test showing PayU card form"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         transaction_id = "1234"
         data = MagicMock()
         data.return_value = {
             "id": transaction_id,
             "token_type": "test_token_type",
             "access_token": "test_access_token",
             "links": [{"rel": "approval_url", "href": "http://approval_url.com"}],
@@ -553,15 +578,17 @@
         self.assertEqual(form.__class__.__name__, "RenewPaymentForm")
         self.assertEqual(form.action, "https://example.com/process_url/token")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_payu_widget_form(self):
         """Test showing PayU card widget"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.token = None
         transaction_id = "1234"
         data = MagicMock()
         data.return_value = {
             "id": transaction_id,
             "token_type": "test_token_type",
             "access_token": "test_access_token",
@@ -578,15 +605,17 @@
             in form.fields["script"].widget.render("a", "b")
         )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_notification(self):
         """Test processing PayU notification"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         mocked_request = MagicMock()
         mocked_request.body = json.dumps({"order": {"status": "COMPLETED"}}).encode(
             "utf8"
         )
         mocked_request.META = {
             "CONTENT_TYPE": "application/json",
             "HTTP_OPENPAYU_SIGNATURE": "signature=a12fbd21c48e69bedee18edf042b816c;algorithm=MD5",
@@ -599,15 +628,17 @@
         self.assertEqual(ret_val.status_code, 200)
         self.assertEqual(ret_val.content, b"ok")
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_notification_cancelled(self):
         """Test processing PayU cancelled notification"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.transaction_id = "123"
         self.payment.save()
         mocked_request = MagicMock()
         mocked_request.body = json.dumps(
             {
                 "order": dict(
                     self.provider.get_processor(self.payment).as_json(),
@@ -635,15 +666,17 @@
 
     def test_process_notification_refund(self):
         """Test processing PayU refund notification"""
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
 
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         mocked_request = MagicMock()
         mocked_request.body = json.dumps(
             {
                 "order": {"status": "COMPLETED"},
                 "refund": {
                     "amount": "22000",
                     "currencyCode": "USD",
@@ -671,15 +704,17 @@
         """Test processing PayU partial refund notification"""
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.total = 220
         self.payment.captured_amount = self.payment.total
         self.payment.save()
         self.payment.refresh_from_db()
 
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         mocked_request = MagicMock()
         mocked_request.body = json.dumps(
             {
                 "order": {"status": "COMPLETED"},
                 "refund": {
                     "amount": "11000",
                     "currencyCode": "USD",
@@ -702,15 +737,17 @@
         self.payment.refresh_from_db()
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal("110"))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
 
     def test_process_notification_refund_not_finalized(self):
         """Test processing PayU partial refund notification"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         mocked_request = MagicMock()
         mocked_request.body = json.dumps(
             {
                 "order": {"status": "COMPLETED"},
                 "refund": {
                     "amount": "11000",
                     "currencyCode": "USD",
@@ -725,15 +762,17 @@
         }
         mocked_request.status_code = 200
         with self.assertRaisesRegex(Exception, "Refund was not finelized"):
             self.provider.process_data(payment=self.payment, request=mocked_request)
 
     def test_process_notification_total_amount(self):
         """Test processing PayU notification if it captures correct amount"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         mocked_request = MagicMock()
         mocked_request.body = json.dumps(
             {
                 "order": {
                     "status": "COMPLETED",
                     "totalAmount": 200,
                     "currencyCode": "USD",
@@ -752,15 +791,17 @@
         self.assertEqual(ret_val.status_code, 200)
         self.assertEqual(ret_val.content, b"ok")
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(self.payment.captured_amount, Decimal("2"))
 
     def test_process_notification_error(self):
         """Test processing PayU notification with wrong signature"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         mocked_request = MagicMock()
         mocked_request.body = b"{}"
         mocked_request.META = {
             "CONTENT_TYPE": "application/json",
             "HTTP_OPENPAYU_SIGNATURE": "signature=foo;algorithm=MD5",
         }
         ret_val = self.provider.process_data(
@@ -770,25 +811,29 @@
         self.assertEqual(ret_val.status_code, 500)
         self.assertEqual(ret_val.content, b"not ok")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_notification_error_malformed_post(self):
         """Test processing PayU notification with malformed POST"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         mocked_request = MagicMock()
         mocked_request.body = b"{}"
         mocked_request.META = {"CONTENT_TYPE": "application/json"}
         with self.assertRaises(PayuApiError) as context:
             self.provider.process_data(payment=self.payment, request=mocked_request)
         self.assertEqual(context.exception.args[0], "Malformed POST")
 
     def test_process_first_renew(self):
         """Test processing first renew"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.token = None
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = '{"status": {"statusCode": "SUCCESS"}, "orderId": 123}'
             post.status_code = 200
             mocked_post.POST = {"value": "renew_token"}
             mocked_post.return_value = post
@@ -839,15 +884,17 @@
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_renew(self):
         """Test processing renew"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "http://test_redirect_uri.com/",
                     "status": {"statusCode": "SUCCESS"},
                     "orderId": 123,
@@ -901,15 +948,17 @@
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_process_renew_card_on_file(self):
         """Test processing renew"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.provider.card_on_file = True
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "http://test_redirect_uri.com/",
                     "status": {"statusCode": "SUCCESS"},
@@ -964,28 +1013,32 @@
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_auto_complete_recurring(self):
         """Test processing renew. The function should return 'success' string, if nothing is required from user."""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = '{"status": {"statusCode": "SUCCESS"}, "orderId": 123}'
             post.status_code = 200
             mocked_post.return_value = post
             redirect = self.provider.auto_complete_recurring(self.payment)
             self.assertEqual(redirect, "success")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_auto_complete_recurring_cvv2(self):
         """Test processing renew when cvv2 form is required - it should return the payment processing URL"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         with patch("requests.post") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {
                     "redirectUri": "test_redirect_uri",
                     "status": {"statusCode": "WARNING_CONTINUE_CVV"},
                     "orderId": 123,
@@ -996,15 +1049,17 @@
             redirect = self.provider.auto_complete_recurring(self.payment)
             self.assertEqual(redirect, "https://example.com/payment/token")
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
         self.assertEqual(self.payment.captured_amount, Decimal("0"))
 
     def test_delete_card_token(self):
         """Test delete_card_token()"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.transaction_id = "1234"
         with patch("requests.delete") as mocked_post:
             post = MagicMock()
             post.text = '{"status": {"statusCode": "SUCCESS"}}'
             post.status_code = 204
             mocked_post.return_value = post
             rejected = self.provider.delete_card_token("FOO_TOKEN")
@@ -1015,15 +1070,17 @@
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
 
     def test_get_paymethod_tokens(self):
         """Test delete_card_token()"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.transaction_id = "1234"
         with patch("requests.get") as mocked_post:
             post = MagicMock()
             post.text = json.dumps(
                 {"cardTokens": [{"name": "Google Pay", "status": "ENABLED"}]}
             )
             post.status_code = 200
@@ -1036,15 +1093,17 @@
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
 
     def test_reject_order(self):
         """Test processing renew"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.transaction_id = "1234"
         with patch("requests.delete") as mocked_post:
             post = MagicMock()
             post.text = '{"status": {"statusCode": "SUCCESS"}}'
             post.status_code = 200
             mocked_post.return_value = post
             rejected = self.provider.reject_order(self.payment)
@@ -1056,15 +1115,17 @@
                     "Content-Type": "application/json",
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.REJECTED)
 
     def test_reject_order_error(self):
         """Test processing renew"""
-        self.set_up_provider(True, True)
+        self.set_up_provider(
+            True, True, get_refund_description=lambda payment, amount: "test"
+        )
         self.payment.transaction_id = "1234"
         with patch("requests.delete") as mocked_post:
             post = MagicMock()
             post.text = '{"status": {"statusCode": "FAIL"}}'
             post.status_code = 200
             mocked_post.return_value = post
             rejected = self.provider.reject_order(self.payment)
@@ -1075,20 +1136,22 @@
                     "Authorization": "Bearer test_access_token",
                     "Content-Type": "application/json",
                 },
             )
         self.assertEqual(self.payment.status, PaymentStatus.WAITING)
 
     def test_refund(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-            get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+                get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
+            )
         payment_extra_data_refund_response_previous = {
             "orderId": "1234",
             "refund": {
                 "refundId": "5000009986",
                 "extRefundId": "ext 1234 10",
                 "amount": "1000",
                 "currencyCode": "USD",
@@ -1148,22 +1211,25 @@
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(210))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses,
             [payment_extra_data_refund_response_previous, refund_request_response_body],
         )
+        self.assertFalse(caught_warnings)
 
     def test_refund_no_amount(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-            get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+                get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
+            )
         self.payment.transaction_id = "1234"
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
         refund_request_response_body = {
             "orderId": "1234",
             "refund": {
@@ -1202,21 +1268,24 @@
         self.assertEqual(amount, Decimal(220))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses, [refund_request_response_body]
         )
+        self.assertFalse(caught_warnings)
 
     def test_refund_no_get_refund_ext_id(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+            )
         self.payment.transaction_id = "1234"
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
         refund_request_response_body = {
             "orderId": "1234",
             "refund": {
@@ -1258,22 +1327,25 @@
         self.assertEqual(amount, Decimal(110))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses, [refund_request_response_body]
         )
+        self.assertFalse(caught_warnings)
 
     def test_refund_no_ext_id(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-            get_refund_ext_id=lambda payment, amount: None,
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+                get_refund_ext_id=lambda payment, amount: None,
+            )
         self.payment.transaction_id = "1234"
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
         refund_request_response_body = {
             "orderId": "1234",
             "refund": {
@@ -1311,22 +1383,25 @@
         self.assertEqual(amount, Decimal(110))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses, [refund_request_response_body]
         )
+        self.assertFalse(caught_warnings)
 
     def test_refund_no_ext_id_twice(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-            get_refund_ext_id=lambda payment, amount: None,
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+                get_refund_ext_id=lambda payment, amount: None,
+            )
         self.payment.transaction_id = "1234"
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
         refund_request_response_body = {
             "orderId": "1234",
             "refund": {
@@ -1367,22 +1442,25 @@
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses,
             [refund_request_response_body, refund_request_response_body],
         )
+        self.assertFalse(caught_warnings)
 
     def test_refund_finalized(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-            get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+                get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
+            )
         self.payment.transaction_id = "1234"
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
         refund_request_response_body = {
             "orderId": "1234",
             "refund": {
@@ -1421,22 +1499,25 @@
         self.assertEqual(amount, Decimal(110))
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses, [refund_request_response_body]
         )
+        self.assertFalse(caught_warnings)
 
     def test_refund_canceled(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-            get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+                get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
+            )
         self.payment.transaction_id = "1234"
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
         refund_request_response_body = {
             "orderId": "1234",
             "refund": {
@@ -1477,22 +1558,25 @@
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses, [refund_request_response_body]
         )
+        self.assertFalse(caught_warnings)
 
     def test_refund_error(self):
-        self.set_up_provider(
-            True,
-            True,
-            get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
-            get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
-        )
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_description=lambda payment, amount: f"desc {payment.transaction_id} {amount}",
+                get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
+            )
         self.payment.transaction_id = "1234"
         self.payment.captured_amount = self.payment.total
         self.payment.change_status(PaymentStatus.CONFIRMED)
         self.payment.save()
         refund_request_response_body = {
             "status": {
                 "statusCode": "OPENPAYU_BUSINESS_ERROR",
@@ -1529,14 +1613,45 @@
         self.assertEqual(refund_request_mock.call_count, 1)
         self.assertEqual(self.payment.total, Decimal(220))
         self.assertEqual(self.payment.captured_amount, Decimal(220))
         self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
         self.assertEqual(
             payment_extra_data_refund_responses, [refund_request_response_body]
         )
+        self.assertFalse(caught_warnings)
+
+    def test_refund_no_get_refund_description(self):
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+            self.set_up_provider(
+                True,
+                True,
+                get_refund_ext_id=lambda payment, amount: f"ext {payment.transaction_id} {amount}",
+            )
+        self.payment.transaction_id = "1234"
+        self.payment.captured_amount = self.payment.total
+        self.payment.change_status(PaymentStatus.CONFIRMED)
+        self.payment.save()
+
+        with self.assertRaisesRegex(ValueError, r"^get_refund_description not set"):
+            self.provider.refund(self.payment, Decimal(110))
+
+        payment_extra_data_refund_responses = json.loads(self.payment.extra_data).get(
+            "refund_responses", []
+        )
+        self.assertEqual(self.payment.total, Decimal(220))
+        self.assertEqual(self.payment.captured_amount, Decimal(220))
+        self.assertEqual(self.payment.status, PaymentStatus.CONFIRMED)
+        self.assertFalse(payment_extra_data_refund_responses)
+        self.assertEqual(len(caught_warnings), 1)
+        self.assertTrue(issubclass(caught_warnings[0].category, DeprecationWarning))
+        self.assertEqual(
+            str(caught_warnings[0].message),
+            "A default value of get_refund_description is deprecated. Set it to a callable instead.",
+        )
 
     @contextlib.contextmanager
     def _patch_refund(
         self,
         base_payu_url,
         order_id,
         access_token,
```

### Comparing `django-payments-payu-1.3.1/tox.ini` & `django-payments-payu-1.4.0/tox.ini`

 * *Files identical despite different names*

