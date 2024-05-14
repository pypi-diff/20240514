# Comparing `tmp/resend-1.0.1.tar.gz` & `tmp/resend-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resend-1.0.1.tar", last modified: Thu May  9 02:27:02 2024, max compression
+gzip compressed data, was "resend-1.0.2.tar", last modified: Tue May 14 01:37:48 2024, max compression
```

## Comparing `resend-1.0.1.tar` & `resend-1.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.991140 resend-1.0.1/
--rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.0.1/LICENSE.md
--rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 02:27:02.991051 resend-1.0.1/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1605 2024-05-09 01:36:14.000000 resend-1.0.1/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.987158 resend-1.0.1/resend/
--rw-r--r--   0 derich     (501) staff       (20)      743 2024-05-09 01:36:14.000000 resend-1.0.1/resend/__init__.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.988472 resend-1.0.1/resend/api_keys/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/api_keys/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)      998 2024-05-09 01:36:14.000000 resend-1.0.1/resend/api_keys/_api_key.py
--rw-r--r--   0 derich     (501) staff       (20)     2310 2024-05-09 01:36:14.000000 resend-1.0.1/resend/api_keys/_api_keys.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.988907 resend-1.0.1/resend/audiences/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/audiences/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1192 2024-05-09 01:36:14.000000 resend-1.0.1/resend/audiences/_audience.py
--rw-r--r--   0 derich     (501) staff       (20)     2305 2024-05-09 01:36:14.000000 resend-1.0.1/resend/audiences/_audiences.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.989311 resend-1.0.1/resend/contacts/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/contacts/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1795 2024-05-09 01:36:14.000000 resend-1.0.1/resend/contacts/_contact.py
--rw-r--r--   0 derich     (501) staff       (20)     4400 2024-05-09 01:36:14.000000 resend-1.0.1/resend/contacts/_contacts.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.989829 resend-1.0.1/resend/domains/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1987 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/_domain.py
--rw-r--r--   0 derich     (501) staff       (20)     3887 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/_domains.py
--rw-r--r--   0 derich     (501) staff       (20)     1416 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/_record.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.990781 resend-1.0.1/resend/emails/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)      489 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_attachment.py
--rw-r--r--   0 derich     (501) staff       (20)      755 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_batch.py
--rw-r--r--   0 derich     (501) staff       (20)     2601 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_email.py
--rw-r--r--   0 derich     (501) staff       (20)     2717 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_emails.py
--rw-r--r--   0 derich     (501) staff       (20)      524 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_tag.py
--rw-r--r--   0 derich     (501) staff       (20)     5985 2024-05-09 01:36:14.000000 resend-1.0.1/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)        0 2023-08-19 17:45:00.000000 resend-1.0.1/resend/py.typed
--rw-r--r--   0 derich     (501) staff       (20)     2331 2024-05-09 01:36:14.000000 resend-1.0.1/resend/request.py
--rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-09 02:27:00.000000 resend-1.0.1/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.988020 resend-1.0.1/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      825 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 02:15:39.000000 resend-1.0.1/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-09 02:27:02.991731 resend-1.0.1/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1171 2024-05-09 02:27:00.000000 resend-1.0.1/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.903787 resend-1.0.2/
+-rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.0.2/LICENSE.md
+-rw-r--r--   0 derich     (501) staff       (20)     2430 2024-05-14 01:37:48.903715 resend-1.0.2/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1627 2024-05-14 01:16:37.000000 resend-1.0.2/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.899984 resend-1.0.2/resend/
+-rw-r--r--   0 derich     (501) staff       (20)     1003 2024-05-14 01:16:37.000000 resend-1.0.2/resend/__init__.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.901211 resend-1.0.2/resend/api_keys/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/api_keys/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)      998 2024-05-09 01:36:14.000000 resend-1.0.2/resend/api_keys/_api_key.py
+-rw-r--r--   0 derich     (501) staff       (20)     2310 2024-05-09 01:36:14.000000 resend-1.0.2/resend/api_keys/_api_keys.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.901668 resend-1.0.2/resend/audiences/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/audiences/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1192 2024-05-09 01:36:14.000000 resend-1.0.2/resend/audiences/_audience.py
+-rw-r--r--   0 derich     (501) staff       (20)     2305 2024-05-09 01:36:14.000000 resend-1.0.2/resend/audiences/_audiences.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.902043 resend-1.0.2/resend/contacts/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/contacts/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1795 2024-05-09 01:36:14.000000 resend-1.0.2/resend/contacts/_contact.py
+-rw-r--r--   0 derich     (501) staff       (20)     4400 2024-05-09 01:36:14.000000 resend-1.0.2/resend/contacts/_contacts.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.902667 resend-1.0.2/resend/domains/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1987 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/_domain.py
+-rw-r--r--   0 derich     (501) staff       (20)     3887 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/_domains.py
+-rw-r--r--   0 derich     (501) staff       (20)     1416 2024-05-09 01:36:14.000000 resend-1.0.2/resend/domains/_record.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.903440 resend-1.0.2/resend/emails/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)      489 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_attachment.py
+-rw-r--r--   0 derich     (501) staff       (20)      755 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_batch.py
+-rw-r--r--   0 derich     (501) staff       (20)     2601 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_email.py
+-rw-r--r--   0 derich     (501) staff       (20)     2717 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_emails.py
+-rw-r--r--   0 derich     (501) staff       (20)      524 2024-05-09 01:36:14.000000 resend-1.0.2/resend/emails/_tag.py
+-rw-r--r--   0 derich     (501) staff       (20)     6102 2024-05-14 01:16:37.000000 resend-1.0.2/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)        0 2023-08-19 17:45:00.000000 resend-1.0.2/resend/py.typed
+-rw-r--r--   0 derich     (501) staff       (20)     2363 2024-05-14 01:16:37.000000 resend-1.0.2/resend/request.py
+-rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-14 01:37:45.000000 resend-1.0.2/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-14 01:37:48.900732 resend-1.0.2/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2430 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      825 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-14 01:37:48.000000 resend-1.0.2/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-14 01:37:48.904498 resend-1.0.2/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1172 2024-05-14 01:16:37.000000 resend-1.0.2/setup.py
```

### Comparing `resend-1.0.1/LICENSE.md` & `resend-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/PKG-INFO` & `resend-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.0.1
+Version: 1.0.2
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -71,10 +71,10 @@
     "cc": ["cc@resend.dev"],
     "tags": [
         {"name": "tag1", "value": "tagvalue1"},
         {"name": "tag2", "value": "tagvalue2"},
     ],
 }
 
-r = resend.Emails.send(params)
-print(r)
+email: resend.Email = resend.Emails.send(params)
+print(email)
 ```
```

### Comparing `resend-1.0.1/README.md` & `resend-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     "cc": ["cc@resend.dev"],
     "tags": [
         {"name": "tag1", "value": "tagvalue1"},
         {"name": "tag2", "value": "tagvalue2"},
     ],
 }
 
-r = resend.Emails.send(params)
-print(r)
+email: resend.Email = resend.Emails.send(params)
+print(email)
 ```
```

### Comparing `resend-1.0.1/resend/__init__.py` & `resend-1.0.2/resend/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 
+from .api_keys._api_key import ApiKey
 from .api_keys._api_keys import ApiKeys
+from .audiences._audience import Audience
 from .audiences._audiences import Audiences
+from .contacts._contact import Contact
 from .contacts._contacts import Contacts
+from .domains._domain import Domain
 from .domains._domains import Domains
 from .emails._attachment import Attachment
 from .emails._batch import Batch
+from .emails._email import Email
 from .emails._emails import Emails
 from .emails._tag import Tag
 from .request import Request
 from .version import get_version
 
 # Config vars
 api_key = os.environ.get("RESEND_API_KEY")
@@ -24,10 +29,15 @@
     "Emails",
     "ApiKeys",
     "Domains",
     "Batch",
     "Audiences",
     "Contacts",
     # Types
+    "Audience",
+    "Contact",
+    "Domain",
+    "ApiKey",
+    "Email",
     "Attachment",
     "Tag",
 ]
```

### Comparing `resend-1.0.1/resend/api_keys/_api_key.py` & `resend-1.0.2/resend/api_keys/_api_key.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/api_keys/_api_keys.py` & `resend-1.0.2/resend/api_keys/_api_keys.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/audiences/_audience.py` & `resend-1.0.2/resend/audiences/_audience.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/audiences/_audiences.py` & `resend-1.0.2/resend/audiences/_audiences.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/contacts/_contact.py` & `resend-1.0.2/resend/contacts/_contact.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/contacts/_contacts.py` & `resend-1.0.2/resend/contacts/_contacts.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/domains/_domain.py` & `resend-1.0.2/resend/domains/_domain.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/domains/_domains.py` & `resend-1.0.2/resend/domains/_domains.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/domains/_record.py` & `resend-1.0.2/resend/domains/_record.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/emails/_batch.py` & `resend-1.0.2/resend/emails/_batch.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/emails/_email.py` & `resend-1.0.2/resend/emails/_email.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/emails/_emails.py` & `resend-1.0.2/resend/emails/_emails.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/emails/_tag.py` & `resend-1.0.2/resend/emails/_tag.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/resend/exceptions.py` & `resend-1.0.2/resend/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Resend Exceptions module.
 
 This module defines the base types for platform-wide error
 codes as outlined in https://resend.com/docs/errors.
 """
 
-from typing import Dict
+from typing import Any, Dict, Union
 
 
 class ResendError(Exception):
     """Base class for all errors raised by Resend SDK.
     This is the parent class of all exceptions (server side)
     raised by the Resend SDK. Developers can simply catch
     this class and inspect its `code` to implement more specific
@@ -21,15 +21,15 @@
         message: A human-readable error message string.
         suggested_action: A suggested action path to help the user.
         error_type: Maps to the `type` field from the Resend API
     """
 
     def __init__(
         self,
-        code: str,
+        code: Union[str, int],
         error_type: str,
         message: str,
         suggested_action: str,
     ):
         Exception.__init__(self, message)
         self.code = code
         self.message = message
@@ -40,15 +40,15 @@
 class MissingApiKeyError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
         message: str,
         error_type: str,
-        code: str,
+        code: Union[str, int],
     ):
         suggested_action = """Include the following header
         Authorization: Bearer YOUR_API_KEY in the request."""
 
         message = "Missing API key in the authorization header."
 
         ResendError.__init__(
@@ -63,15 +63,15 @@
 class InvalidApiKeyError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
         message: str,
         error_type: str,
-        code: str,
+        code: Union[str, int],
     ):
         suggested_action = """Generate a new API key in the dashboard."""
 
         ResendError.__init__(
             self,
             message=message,
             suggested_action=suggested_action,
@@ -83,15 +83,15 @@
 class ValidationError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
         message: str,
         error_type: str,
-        code: str,
+        code: Union[str, int],
     ):
         default_message = """
         The request body is missing one or more required fields."""
 
         suggested_action = """Check the error message
         to see the list of missing fields."""
 
@@ -110,15 +110,15 @@
 class MissingRequiredFieldsError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
         message: str,
         error_type: str,
-        code: str,
+        code: Union[str, int],
     ):
         default_message = """
         The request body is missing one or more required fields."""
 
         suggested_action = """Check the error message
         to see the list of missing fields."""
 
@@ -137,15 +137,15 @@
 class ApplicationError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
         message: str,
         error_type: str,
-        code: str,
+        code: Union[str, int],
     ):
         default_message = """
         Something went wrong."""
 
         suggested_action = """Contact Resend support."""
 
         if message == "":
@@ -157,27 +157,27 @@
             message=message,
             suggested_action=suggested_action,
             error_type=error_type,
         )
 
 
 # Dict with error code -> error type mapping
-ERRORS: Dict = {
+ERRORS: Dict[str, Dict[str, Any]] = {
     "400": {"validation_error": ValidationError},
     "422": {
         "missing_required_fields": MissingRequiredFieldsError,
         "validation_error": ValidationError,
     },
     "401": {"missing_api_key": MissingApiKeyError},
     "403": {"invalid_api_key": InvalidApiKeyError},
     "500": {"application_error": ApplicationError},
 }
 
 
-def raise_for_code_and_type(code: str, error_type: str, message: str) -> None:
+def raise_for_code_and_type(code: Union[str, int], error_type: str, message: str) -> None:
     """Raise the appropriate error based on the code and type.
 
     Args:
         code (str): The error code
         error_type (str): The error type
         message (str): The error message
```

### Comparing `resend-1.0.1/resend/request.py` & `resend-1.0.2/resend/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Dict
+from typing import Any, Dict
 
 import requests
 
 import resend
 from resend.exceptions import raise_for_code_and_type
 from resend.version import get_version
 
 
 # This class wraps the HTTP request creation logic
 class Request:
-    def __init__(self, path: str, params: Dict, verb: str):
+    def __init__(self, path: str, params: Dict[Any, Any], verb: str):
         self.path = path
         self.params = params
         self.verb = verb
 
-    def perform(self):
+    def perform(self) -> Any:
         """Is the main function that makes the HTTP request
         to the Resend API. It uses the path, params, and verb attributes
         to make the request.
 
         Returns:
             Dict: The JSON response from the API
 
@@ -38,15 +38,15 @@
             raise_for_code_and_type(
                 code=error.get("statusCode"),
                 message=error.get("message"),
                 error_type=error.get("name"),
             )
         return resp.json()
 
-    def __get_headers(self) -> Dict:
+    def __get_headers(self) -> Dict[Any, Any]:
         """get_headers returns the HTTP headers that will be
         used for every req.
 
         Returns:
             Dict: configured HTTP Headers
         """
         return {
```

### Comparing `resend-1.0.1/resend.egg-info/PKG-INFO` & `resend-1.0.2/resend.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.0.1
+Version: 1.0.2
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -71,10 +71,10 @@
     "cc": ["cc@resend.dev"],
     "tags": [
         {"name": "tag1", "value": "tagvalue1"},
         {"name": "tag2", "value": "tagvalue2"},
     ],
 }
 
-r = resend.Emails.send(params)
-print(r)
+email: resend.Email = resend.Emails.send(params)
+print(email)
 ```
```

### Comparing `resend-1.0.1/resend.egg-info/SOURCES.txt` & `resend-1.0.2/resend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resend-1.0.1/setup.py` & `resend-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
+
 from resend.version import get_version
 
 install_requires = open("requirements.txt").readlines()
 
 setup(
     name="resend",
     version=get_version(),
```

