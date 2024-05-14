# Comparing `tmp/aipkgs_core-0.4.4.tar.gz` & `tmp/aipkgs_core-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_core-0.4.4.tar", max compression
+gzip compressed data, was "aipkgs_core-0.4.5.tar", max compression
```

## Comparing `aipkgs_core-0.4.4.tar` & `aipkgs_core-0.4.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-0.4.4/LICENSE.md
--rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-0.4.4/README.rst
--rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-0.4.4/aipkgs_core/__init__.py
--rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-0.4.4/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
--rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-0.4.4/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
--rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-0.4.4/aipkgs_core/encryption/encryption.py
--rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-0.4.4/aipkgs_core/logger/helpers.py
--rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
--rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
--rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
--rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
--rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
--rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
--rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-0.4.4/aipkgs_core/utils/date_helpers.py
--rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-0.4.4/aipkgs_core/utils/dir_helpers.py
--rw-r--r--   0        0        0      645 2024-05-12 23:55:44.559082 aipkgs_core-0.4.4/aipkgs_core/utils/email.py
--rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-0.4.4/aipkgs_core/utils/file_helpers.py
--rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-0.4.4/aipkgs_core/utils/json.py
--rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-0.4.4/aipkgs_core/utils/phone_number.py
--rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-0.4.4/aipkgs_core/utils/singleton.py
--rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-0.4.4/aipkgs_core/utils/string_helpers.py
--rw-r--r--   0        0        0      654 2024-05-09 14:48:47.729452 aipkgs_core-0.4.4/aipkgs_core/utils/utils.py
--rw-r--r--   0        0        0      983 2024-05-12 23:56:22.561756 aipkgs_core-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 aipkgs_core-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-0.4.5/LICENSE.md
+-rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-0.4.5/README.rst
+-rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-0.4.5/aipkgs_core/__init__.py
+-rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-0.4.5/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
+-rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-0.4.5/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
+-rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-0.4.5/aipkgs_core/encryption/encryption.py
+-rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-0.4.5/aipkgs_core/logger/helpers.py
+-rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
+-rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
+-rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
+-rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
+-rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
+-rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-0.4.5/aipkgs_core/utils/date_helpers.py
+-rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-0.4.5/aipkgs_core/utils/dir_helpers.py
+-rw-r--r--   0        0        0     1084 2024-05-14 10:16:31.693520 aipkgs_core-0.4.5/aipkgs_core/utils/email.py
+-rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-0.4.5/aipkgs_core/utils/file_helpers.py
+-rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-0.4.5/aipkgs_core/utils/json.py
+-rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-0.4.5/aipkgs_core/utils/phone_number.py
+-rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-0.4.5/aipkgs_core/utils/singleton.py
+-rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-0.4.5/aipkgs_core/utils/string_helpers.py
+-rw-r--r--   0        0        0      654 2024-05-09 14:48:47.729452 aipkgs_core-0.4.5/aipkgs_core/utils/utils.py
+-rw-r--r--   0        0        0      983 2024-05-14 10:16:35.204027 aipkgs_core-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 aipkgs_core-0.4.5/PKG-INFO
```

### Comparing `aipkgs_core-0.4.4/LICENSE.md` & `aipkgs_core-0.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/__init__.py` & `aipkgs_core-0.4.5/aipkgs_core/__init__.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc` & `aipkgs_core-0.4.5/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc` & `aipkgs_core-0.4.5/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/encryption/encryption.py` & `aipkgs_core-0.4.5/aipkgs_core/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/json.cpython-38.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/json.cpython-39.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc` & `aipkgs_core-0.4.5/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/date_helpers.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/dir_helpers.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/email.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/email.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,7 +12,18 @@
                                check_deliverability=check_deliverability,
                                allow_empty_local=allow_empty_local)
 
         email = valid.email
         return True
     except EmailNotValidError as e:
         return False
+
+
+def is_valid_email(email: str,
+                   allow_smtputf8: bool = False,
+                   check_deliverability: bool = False,
+                   allow_empty_local: bool = False
+                   ) -> bool:
+    return is_email_valid(email,
+                          allow_smtputf8=allow_smtputf8,
+                          check_deliverability=check_deliverability,
+                          allow_empty_local=allow_empty_local)
```

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/file_helpers.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/json.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/json.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/singleton.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/string_helpers.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/string_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/aipkgs_core/utils/utils.py` & `aipkgs_core-0.4.5/aipkgs_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.4/pyproject.toml` & `aipkgs_core-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-core"
-version = "0.4.4"
+version = "0.4.5"
 description = "Core package for aipy packages."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
 keywords = ["ai"]
```

### Comparing `aipkgs_core-0.4.4/PKG-INFO` & `aipkgs_core-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-core
-Version: 0.4.4
+Version: 0.4.5
 Summary: Core package for aipy packages.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
```
