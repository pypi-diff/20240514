# Comparing `tmp/django-drf-otp-0.0.8.tar.gz` & `tmp/django-drf-otp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-drf-otp-0.0.8.tar", last modified: Mon Jan 22 11:34:19 2024, max compression
+gzip compressed data, was "django-drf-otp-0.0.9.tar", last modified: Tue Mar 12 14:30:03 2024, max compression
```

## Comparing `django-drf-otp-0.0.8.tar` & `django-drf-otp-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.490783 django-drf-otp-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)    11538 2024-01-22 11:34:19.490783 django-drf-otp-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10682 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.482783 django-drf-otp-0.0.8/django_drf_otp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/enums.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.474783 django-drf-otp-0.0.8/django_drf_otp/locale/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.474783 django-drf-otp-0.0.8/django_drf_otp/locale/tr/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.482783 django-drf-otp-0.0.8/django_drf_otp/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     2090 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/locale/tr/LC_MESSAGES/django.po
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.486783 django-drf-otp-0.0.8/django_drf_otp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2904 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/0002_populate_notification_preference.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/0003_remove_verificationtoken_expire_date.py
--rw-rw-rw-   0 root         (0) root         (0)      707 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/0004_alter_usernotificationpreference_id_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/0005_verificationtoken_secret_chars_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/0006_verificationtoken_active_token_idx.py
--rw-rw-rw-   0 root         (0) root         (0)      476 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/0007_alter_verificationtoken_secret_chars.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/notifiers.py
--rw-rw-rw-   0 root         (0) root         (0)     3383 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     3861 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/services.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/strategies.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.474783 django-drf-otp-0.0.8/django_drf_otp/templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.486783 django-drf-otp-0.0.8/django_drf_otp/templates/django_drf_otp/
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/templates/django_drf_otp/email.html
--rw-rw-rw-   0 root         (0) root         (0)     2712 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4514 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/django_drf_otp/viewsets.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-22 11:34:19.482783 django-drf-otp-0.0.8/django_drf_otp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    11538 2024-01-22 11:34:19.000000 django-drf-otp-0.0.8/django_drf_otp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1223 2024-01-22 11:34:19.000000 django-drf-otp-0.0.8/django_drf_otp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-22 11:34:19.000000 django-drf-otp-0.0.8/django_drf_otp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-01-22 11:34:19.000000 django-drf-otp-0.0.8/django_drf_otp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-01-22 11:34:19.000000 django-drf-otp-0.0.8/django_drf_otp.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1032 2024-01-22 11:34:19.490783 django-drf-otp-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-22 11:34:08.000000 django-drf-otp-0.0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)    11538 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10682 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/django_drf_otp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.153271 django-drf-otp-0.0.9/django_drf_otp/locale/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.153271 django-drf-otp-0.0.9/django_drf_otp/locale/tr/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/django_drf_otp/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2090 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/locale/tr/LC_MESSAGES/django.po
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/django_drf_otp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/0002_populate_notification_preference.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/0003_remove_verificationtoken_expire_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/0004_alter_usernotificationpreference_id_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/0005_verificationtoken_secret_chars_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/0006_verificationtoken_active_token_idx.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/0007_alter_verificationtoken_secret_chars.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/notifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3383 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3861 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/strategies.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.153271 django-drf-otp-0.0.9/django_drf_otp/templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/django_drf_otp/templates/django_drf_otp/
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/templates/django_drf_otp/email.html
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     4514 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/django_drf_otp/viewsets.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/django_drf_otp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11538 2024-03-12 14:30:03.000000 django-drf-otp-0.0.9/django_drf_otp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2024-03-12 14:30:03.000000 django-drf-otp-0.0.9/django_drf_otp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-12 14:30:03.000000 django-drf-otp-0.0.9/django_drf_otp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-03-12 14:30:03.000000 django-drf-otp-0.0.9/django_drf_otp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-12 14:30:03.000000 django-drf-otp-0.0.9/django_drf_otp.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2024-03-12 14:30:03.157271 django-drf-otp-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-12 14:29:55.000000 django-drf-otp-0.0.9/setup.py
```

### Comparing `django-drf-otp-0.0.8/LICENSE` & `django-drf-otp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/PKG-INFO` & `django-drf-otp-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-otp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app to supports 2FA(Two Factor Authentication) on djangorestframework.
 Home-page: https://bitbucket.org/akinonteam/django_drf_otp/
 Author: Akinon
 Author-email: dev@akinon.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-otp-0.0.8/README.md` & `django-drf-otp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/exceptions.py` & `django-drf-otp-0.0.9/django_drf_otp/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/locale/tr/LC_MESSAGES/django.po` & `django-drf-otp-0.0.9/django_drf_otp/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/migrations/0001_initial.py` & `django-drf-otp-0.0.9/django_drf_otp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/migrations/0002_populate_notification_preference.py` & `django-drf-otp-0.0.9/django_drf_otp/migrations/0002_populate_notification_preference.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/migrations/0004_alter_usernotificationpreference_id_and_more.py` & `django-drf-otp-0.0.9/django_drf_otp/migrations/0004_alter_usernotificationpreference_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/migrations/0005_verificationtoken_secret_chars_and_more.py` & `django-drf-otp-0.0.9/django_drf_otp/migrations/0005_verificationtoken_secret_chars_and_more.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/models.py` & `django-drf-otp-0.0.9/django_drf_otp/models.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/notifiers.py` & `django-drf-otp-0.0.9/django_drf_otp/notifiers.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/serializers.py` & `django-drf-otp-0.0.9/django_drf_otp/serializers.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/services.py` & `django-drf-otp-0.0.9/django_drf_otp/services.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/settings.py` & `django-drf-otp-0.0.9/django_drf_otp/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "TOTP_TOKEN_TTL": 300,
     "DEFAULT_TOKEN_TYPE": TokenType.TOTP,
     "DEFAULT_NOTIFICATION_TYPE": NotificationType.EMAIL,
     "EMAIL_CONFIG": {
         "SUBJECT": _("Verification Token"),
         "TEMPLATE_PATH": "django_drf_otp/email.html",
     },
+    "OTP_DISABLED_USERS": [],
 }
 
 
 class Settings:
     def __init__(self, defaults: Dict, user_settings: Optional[Dict]) -> None:
         self._user_settings = user_settings
         self.defaults = defaults or DEFAULTS
```

### Comparing `django-drf-otp-0.0.8/django_drf_otp/strategies.py` & `django-drf-otp-0.0.9/django_drf_otp/strategies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+import re
 import typing
 from abc import ABC, abstractmethod
 from typing import Optional, Union
 
 from django.contrib.auth.models import AbstractUser
 from pyotp import TOTP
 
@@ -51,15 +52,25 @@
     def verify_token(self, token: str, extra_secret_chars: Optional[str] = None) -> bool:
         token_class = self._get_token_class(extra_secret_chars=extra_secret_chars)
         return token_class.verify(otp=token)
 
     def generate_token_for_user(self, user: AbstractUser) -> VerificationToken:
         secret_chars = VerificationToken.generate_secret_chars(user=user)
 
-        token = self.generate_token(extra_secret_chars=secret_chars)
+        email = user.email
+        match = re.search(r"\+(.*?)@", email)
+        if match:
+            email = email.replace(match.group(0), "@")
+
+        otp_token_data = next(
+            filter(lambda x: x.get("email") == email, otp_settings.OTP_DISABLED_USERS),
+            {"token": self.generate_token(extra_secret_chars=secret_chars)},
+        )
+        token = otp_token_data["token"]
+
         verification_token = self.create_verification_token(
             user=user,
             token=token,
             token_type=self.token_type,
             secret_chars=secret_chars,
         )
         self.deactivate_old_verification_tokens(verification_token=verification_token)
```

### Comparing `django-drf-otp-0.0.8/django_drf_otp/templates/django_drf_otp/email.html` & `django-drf-otp-0.0.9/django_drf_otp/templates/django_drf_otp/email.html`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/test_settings.py` & `django-drf-otp-0.0.9/django_drf_otp/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp/viewsets.py` & `django-drf-otp-0.0.9/django_drf_otp/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/django_drf_otp.egg-info/PKG-INFO` & `django-drf-otp-0.0.9/django_drf_otp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-drf-otp
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Django app to supports 2FA(Two Factor Authentication) on djangorestframework.
 Home-page: https://bitbucket.org/akinonteam/django_drf_otp/
 Author: Akinon
 Author-email: dev@akinon.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-drf-otp-0.0.8/django_drf_otp.egg-info/SOURCES.txt` & `django-drf-otp-0.0.9/django_drf_otp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-drf-otp-0.0.8/setup.cfg` & `django-drf-otp-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-drf-otp
-version = 0.0.8
+version = 0.0.9
 description = A Django app to supports 2FA(Two Factor Authentication) on djangorestframework.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/akinonteam/django_drf_otp/
 author = Akinon
 author_email = dev@akinon.com
 license = MIT
```

