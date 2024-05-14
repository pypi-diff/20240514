# Comparing `tmp/fast_gmail-1.0.9.tar.gz` & `tmp/fast_gmail-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.0.9.tar", last modified: Wed May  8 13:01:40 2024, max compression
+gzip compressed data, was "fast_gmail-1.1.0.tar", last modified: Tue May 14 12:40:14 2024, max compression
```

## Comparing `fast_gmail-1.0.9.tar` & `fast_gmail-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.9/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14864 2024-04-20 07:12:16.000000 fast_gmail-1.0.9/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/fast_gmail/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.9/fast_gmail/__init__.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.9/fast_gmail/draft.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    22026 2024-05-08 12:44:06.000000 fast_gmail-1.0.9/fast_gmail/gmail.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.0.9/fast_gmail/helpers.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    25256 2024-04-20 07:20:24.000000 fast_gmail-1.0.9/fast_gmail/message.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.9/fast_gmail/search.py
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-05-08 13:01:40.000000 fast_gmail-1.0.9/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-05-08 13:01:40.682925 fast_gmail-1.0.9/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-05-08 12:44:38.000000 fast_gmail-1.0.9/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.1.0/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14864 2024-04-20 07:12:16.000000 fast_gmail-1.1.0/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-14 12:40:14.795512 fast_gmail-1.1.0/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.1.0/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.1.0/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    22531 2024-05-14 12:36:50.000000 fast_gmail-1.1.0/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.1.0/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25256 2024-04-20 07:20:24.000000 fast_gmail-1.1.0/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.1.0/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-05-14 12:40:06.000000 fast_gmail-1.1.0/setup.py
```

### Comparing `fast_gmail-1.0.9/LICENSE` & `fast_gmail-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.9/PKG-INFO` & `fast_gmail-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.9
+Version: 1.1.0
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.0.9/README.md` & `fast_gmail-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.9/fast_gmail/gmail.py` & `fast_gmail-1.1.0/fast_gmail/gmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 from typing import Union
 from typing import List
+from typing import Any
 import mimetypes
 import base64
 import os
 import json
 
 from email.message import EmailMessage
 from email.header import Header
@@ -45,24 +46,29 @@
 		self,
 		token_file_path: str = "token.json",
 		credentials_file_path: str = "credentials.json",
 		port: int = 3000, # set the local server port for Authorized redirect URI
 		separator_symbol: str = ", ",
 		user_id: str = "me",
 		application_type: ApplicationType = ApplicationType.WEB,
+		auth_token: Optional[dict] = None,
 		code: Optional[str] = None
 	)-> None:
 		"""https://github.com/googleapis/google-api-python-client/blob/main/docs/oauth-installed.md"""
 
 		# set separator for spliting/joining the array of existing previous_page_tokens for pagination
 		self.SEPARATOR_SYMBOL = separator_symbol
+
 		# The file token.json stores the user's access and refresh tokens, and is
 		# created automatically when the authorization flow completes for the first time.
-		if os.path.exists(token_file_path):
-			self.credentials = Credentials.from_authorized_user_file(token_file_path, SCOPES)
+		if not auth_token:
+			if os.path.exists(token_file_path):
+				self.credentials = Credentials.from_authorized_user_file(token_file_path, SCOPES)
+		else:
+			self.credentials = Credentials.from_authorized_user_info(auth_token, SCOPES)
 		self.auth_url: str = ""
 		# If there are no (valid) credentials available, let the user log in.
 		if not self.credentials or not self.credentials.valid:
 			if self.credentials and self.credentials.expired and self.credentials.refresh_token:
 				# refresh access token
 				self.credentials = Credentials(
 					token=None,  # No initial token provided, refresh token will be used
@@ -110,26 +116,34 @@
                         )
 						if code:
 							self.flow.fetch_token(code=code)
 							self.credentials = self.flow.credentials
 						else:
 							self.auth_url = f"{self.flow.authorization_url()[0]}&prompt=consent"
 							return
-			# Save the credentials for the next run
-			with open(token_file_path, "w") as token:
-				token.write(self.credentials.to_json())
+			if not auth_token:
+				# Save the credentials for the next run
+				with open(token_file_path, "w") as token:
+					token.write(self.credentials.to_json())
+			else:
+				# save the credentials as a dict
+				self.auth_token = json.loads(self.credentials.to_json())
 		try:
 			# Call the Gmail API and set the instance 
 			self.google_service = GoogleService(
 				service = build("gmail", "v1", credentials = self.credentials),
 				user_id = user_id
 			)
 		except HttpError as e:
 			raise e
 
+	def get_auth_token(self)-> dict:
+		"""Returns a JSON representation of this instance. It can be passed to from_authorized_user_info() to create a new credential instance."""
+		return self.auth_token
+
 	def get_message(self, id: str)-> Optional[Message]:
 		if not self.google_service:
 			return None
 		return Message(
 			google_service=GoogleService(
 				service=self.google_service.service,
 				user_id=self.google_service.user_id,
```

### Comparing `fast_gmail-1.0.9/fast_gmail/helpers.py` & `fast_gmail-1.1.0/fast_gmail/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.9/fast_gmail/message.py` & `fast_gmail-1.1.0/fast_gmail/message.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.9/fast_gmail/search.py` & `fast_gmail-1.1.0/fast_gmail/search.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.9/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.1.0/fast_gmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.9
+Version: 1.1.0
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.0.9/setup.py` & `fast_gmail-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_descrition=f.read()
 
 setup(
     name="fast_gmail",
-    version="1.0.9",
+    version="1.1.0",
     description="GmailApi wrapper",
     long_description=long_descrition,
     long_description_content_type='text/markdown',
     author="Aleti",
     author_email="aleti.open.source@gmail.com",
     url="https://github.com/aleti1/fast_gmail",
     license="MIT",
```

