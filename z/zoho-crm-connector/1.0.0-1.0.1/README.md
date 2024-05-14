# Comparing `tmp/zoho_crm_connector-1.0.0.tar.gz` & `tmp/zoho_crm_connector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho_crm_connector-1.0.0.tar", last modified: Fri Aug 12 08:25:46 2022, max compression
+gzip compressed data, was "zoho_crm_connector-1.0.1.tar", last modified: Tue May 14 05:02:19 2024, max compression
```

## Comparing `zoho_crm_connector-1.0.0.tar` & `zoho_crm_connector-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-08-12 08:25:46.686246 zoho_crm_connector-1.0.0/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1064 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.0/LICENCE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       19 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.0/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     7647 2022-08-12 08:25:46.686246 zoho_crm_connector-1.0.0/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     7100 2022-08-12 08:25:13.000000 zoho_crm_connector-1.0.0/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)       63 2022-08-12 08:25:46.686246 zoho_crm_connector-1.0.0/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     1467 2022-08-12 08:25:45.000000 zoho_crm_connector-1.0.0/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-08-12 08:25:46.686246 zoho_crm_connector-1.0.0/zoho_crm_connector/
--rw-rw-r--   0 tim       (1000) tim       (1000)       35 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.0/zoho_crm_connector/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    20772 2022-08-12 04:59:28.000000 zoho_crm_connector-1.0.0/zoho_crm_connector/zoho_crm_api.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-08-12 08:25:46.686246 zoho_crm_connector-1.0.0/zoho_crm_connector.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     7647 2022-08-12 08:25:46.000000 zoho_crm_connector-1.0.0/zoho_crm_connector.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      327 2022-08-12 08:25:46.000000 zoho_crm_connector-1.0.0/zoho_crm_connector.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-08-12 08:25:46.000000 zoho_crm_connector-1.0.0/zoho_crm_connector.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        9 2022-08-12 08:25:46.000000 zoho_crm_connector-1.0.0/zoho_crm_connector.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       19 2022-08-12 08:25:46.000000 zoho_crm_connector-1.0.0/zoho_crm_connector.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1064 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.1/LICENCE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       19 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.1/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)     7744 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7193 2024-05-14 03:29:42.000000 zoho_crm_connector-1.0.1/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)       63 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1467 2024-05-14 03:28:56.000000 zoho_crm_connector-1.0.1/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/zoho_crm_connector/
+-rw-rw-r--   0 tim       (1000) tim       (1000)       35 2022-08-12 04:11:33.000000 zoho_crm_connector-1.0.1/zoho_crm_connector/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21233 2024-05-13 13:11:27.000000 zoho_crm_connector-1.0.1/zoho_crm_connector/zoho_crm_api.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-05-14 05:02:19.319558 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)     7744 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      327 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        9 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       19 2024-05-14 05:02:19.000000 zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/top_level.txt
```

### Comparing `zoho_crm_connector-1.0.0/LICENCE.txt` & `zoho_crm_connector-1.0.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `zoho_crm_connector-1.0.0/PKG-INFO` & `zoho_crm_connector-1.0.1/zoho_crm_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: zoho_crm_connector
-Version: 1.0.0
+Name: zoho-crm-connector
+Version: 1.0.1
 Summary: Zoho CRM connector
 Home-page: https://github.com/timrichardson/zoho_crm_package
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MIT
 Keywords: zoho crm
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: requests
 
 Zoho CRM Connector for Python
 ==================
 
 Zoho provides a Python SDK, but I found it a bit hard to use and it seems a bit complicated.
 For instance, there is a dependency on mysql.
 This module is a little more pragmatic and it returns pages of results with yield.
@@ -173,16 +173,17 @@
 ```
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload --skip-existing dist/*
 ```
 
 Changes
 ========
+v1.0.1 Fixed bug with get_users(): now all pages are returned, and the usertype filter works.
 
-v 1.0.0 It works well enough to be v1
+v1.0.0 It works well enough to be v1
 
 v0.4.6. Add a message to Quota Exceeded exception
 
 v0.4.5. Raise Runtime exception if token refresh fails to return a valid token
 
 v0.4.4 Merge new feature for kdodia (Karan Dodia): yield_deleted_records_from_module, update_zoho_module, and fixes for 204 response get_related_records
 
@@ -191,9 +192,7 @@
 v0.4.2 Fix a potential date bug with modified-since header
 
 v0.4.1: small changes to readme. Also, v.0.4.0 has a test case using the IN criteria which may be interesting.
 
 v 0.4.0: No longer retry when API limit is reached, raise an exception instead. 
 Reason: the Zoho CRM API rate limit is 24 hour rolling, and it can take minutes to get credits back. Too long to wait.
 
-
-
```

### Comparing `zoho_crm_connector-1.0.0/README.md` & `zoho_crm_connector-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -155,16 +155,17 @@
 ```
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload --skip-existing dist/*
 ```
 
 Changes
 ========
+v1.0.1 Fixed bug with get_users(): now all pages are returned, and the usertype filter works.
 
-v 1.0.0 It works well enough to be v1
+v1.0.0 It works well enough to be v1
 
 v0.4.6. Add a message to Quota Exceeded exception
 
 v0.4.5. Raise Runtime exception if token refresh fails to return a valid token
 
 v0.4.4 Merge new feature for kdodia (Karan Dodia): yield_deleted_records_from_module, update_zoho_module, and fixes for 204 response get_related_records
```

### Comparing `zoho_crm_connector-1.0.0/setup.py` & `zoho_crm_connector-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 cmdclass = {'build_sphinx': BuildDoc}
 
 # https://pypi.org/classifiers/
 
 name = 'zoho_crm_connector'
 keywords = 'zoho crm'
-version = '1.0.0'
+version = '1.0.1'
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=name,
```

### Comparing `zoho_crm_connector-1.0.0/zoho_crm_connector/zoho_crm_api.py` & `zoho_crm_connector-1.0.1/zoho_crm_connector/zoho_crm_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,24 +225,35 @@
             if 'info' in r_json:
                 if not r_json['info']['more_records']:
                     break
             else:
                 break
             page += 1
 
-    def get_users(self, user_type: str = None) -> dict:
+    def get_users(self, user_type: str = None, per_page:int=200) -> dict:
         """
         Get zoho users, filtering by a Zoho CRM user type. The default value of None is mapped to 'AllUsers'
+        user_type is documented: https://www.zoho.com/crm/developer/docs/api/v6/get-users.html
+
         """
         if self.zoho_user_cache is None:
-            user_type = 'AllUsers' or user_type
-            url = self.base_url + f"users?type={user_type}"
-            headers = {'Authorization': 'Zoho-oauthtoken ' + self.current_token['access_token']}
-            r = self.requests_session.get(url=url, headers=headers)
-            self.zoho_user_cache = self._validate_response(r)
+            user_type = user_type or 'AllUsers'
+            data = []
+            page = 0
+            while page < 999:
+                page += 1
+                url = self.base_url + f"users?type={user_type}&page={page}&per_page={per_page}"
+                headers = {'Authorization': 'Zoho-oauthtoken ' + self.current_token['access_token']}
+
+                r = self.requests_session.get(url=url, headers=headers)
+                validated_response = self._validate_response(r)
+                data.extend(validated_response['users'])
+                if not validated_response['info']['more_records']:
+                    break
+            self.zoho_user_cache = {"users": data}
         return self.zoho_user_cache
 
     def finduser_by_name(self, full_name: str) -> Tuple[str, str]:
         """ Tries to reutn the user as a tuple(full_name,Zoho user id), using the full full_name provided.
             The user must be active. If no such user is found, return the default user provided
             at initialisation of the Zoho_crm object."""
         users = self.get_users()
```

### Comparing `zoho_crm_connector-1.0.0/zoho_crm_connector.egg-info/PKG-INFO` & `zoho_crm_connector-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: zoho-crm-connector
-Version: 1.0.0
+Name: zoho_crm_connector
+Version: 1.0.1
 Summary: Zoho CRM connector
 Home-page: https://github.com/timrichardson/zoho_crm_package
 Author: Tim Richardson
 Author-email: tim@growthpath.com.au
 License: MIT
 Keywords: zoho crm
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
+Requires-Dist: requests
 
 Zoho CRM Connector for Python
 ==================
 
 Zoho provides a Python SDK, but I found it a bit hard to use and it seems a bit complicated.
 For instance, there is a dependency on mysql.
 This module is a little more pragmatic and it returns pages of results with yield.
@@ -173,16 +173,17 @@
 ```
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload --skip-existing dist/*
 ```
 
 Changes
 ========
+v1.0.1 Fixed bug with get_users(): now all pages are returned, and the usertype filter works.
 
-v 1.0.0 It works well enough to be v1
+v1.0.0 It works well enough to be v1
 
 v0.4.6. Add a message to Quota Exceeded exception
 
 v0.4.5. Raise Runtime exception if token refresh fails to return a valid token
 
 v0.4.4 Merge new feature for kdodia (Karan Dodia): yield_deleted_records_from_module, update_zoho_module, and fixes for 204 response get_related_records
 
@@ -191,9 +192,7 @@
 v0.4.2 Fix a potential date bug with modified-since header
 
 v0.4.1: small changes to readme. Also, v.0.4.0 has a test case using the IN criteria which may be interesting.
 
 v 0.4.0: No longer retry when API limit is reached, raise an exception instead. 
 Reason: the Zoho CRM API rate limit is 24 hour rolling, and it can take minutes to get credits back. Too long to wait.
 
-
-
```

