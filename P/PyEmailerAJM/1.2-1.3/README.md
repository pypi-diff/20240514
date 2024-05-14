# Comparing `tmp/PyEmailerAJM-1.2.tar.gz` & `tmp/PyEmailerAJM-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailerAJM-1.2.tar", last modified: Fri Nov 17 12:30:01 2023, max compression
+gzip compressed data, was "PyEmailerAJM-1.3.tar", last modified: Tue May 14 11:59:58 2024, max compression
```

## Comparing `PyEmailerAJM-1.2.tar` & `PyEmailerAJM-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-17 12:30:01.677498 PyEmailerAJM-1.2/
--rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      513 2023-11-17 12:30:01.677704 PyEmailerAJM-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-17 12:30:01.655353 PyEmailerAJM-1.2/PyEmailerAJM/
--rw-rw-rw-   0        0        0    10037 2023-11-17 12:24:50.000000 PyEmailerAJM-1.2/PyEmailerAJM/PyEmailerAJM.py
--rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.2/PyEmailerAJM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-17 12:30:01.673943 PyEmailerAJM-1.2/PyEmailerAJM.egg-info/
--rw-rw-rw-   0        0        0      513 2023-11-17 12:30:01.000000 PyEmailerAJM-1.2/PyEmailerAJM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-11-17 12:30:01.000000 PyEmailerAJM-1.2/PyEmailerAJM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-17 12:30:01.000000 PyEmailerAJM-1.2/PyEmailerAJM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-11-17 12:30:01.000000 PyEmailerAJM-1.2/PyEmailerAJM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-17 12:30:01.000000 PyEmailerAJM-1.2/PyEmailerAJM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      253 2023-09-12 19:19:18.000000 PyEmailerAJM-1.2/README.md
--rw-rw-rw-   0        0        0       86 2023-11-17 12:30:01.681693 PyEmailerAJM-1.2/setup.cfg
--rw-rw-rw-   0        0        0      600 2023-11-17 12:21:58.000000 PyEmailerAJM-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:59:58.435606 PyEmailerAJM-1.3/
+-rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      513 2024-05-14 11:59:58.436600 PyEmailerAJM-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 11:59:58.408640 PyEmailerAJM-1.3/PyEmailerAJM/
+-rw-rw-rw-   0        0        0    10428 2024-05-14 11:50:42.000000 PyEmailerAJM-1.3/PyEmailerAJM/PyEmailerAJM.py
+-rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.3/PyEmailerAJM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 11:59:58.432576 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/
+-rw-rw-rw-   0        0        0      513 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 11:59:58.000000 PyEmailerAJM-1.3/PyEmailerAJM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      388 2024-05-14 11:38:54.000000 PyEmailerAJM-1.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-14 11:59:58.440594 PyEmailerAJM-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-14 11:51:15.000000 PyEmailerAJM-1.3/setup.py
```

### Comparing `PyEmailerAJM-1.2/LICENSE.txt` & `PyEmailerAJM-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyEmailerAJM-1.2/PKG-INFO` & `PyEmailerAJM-1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.2
+Version: 1.3
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.2.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.3.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.2/PyEmailerAJM/PyEmailerAJM.py` & `PyEmailerAJM-1.3/PyEmailerAJM/PyEmailerAJM.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 
 class EmailerNotSetupError(Exception):
     ...
 
 
 class PyEmailer:
+    # the email tab_char
+    tab_char = '&emsp;'
+
     def __init__(self, display_window: bool,
                  send_emails: bool, logger: Logger = None,
                  auto_send: bool = False,
                  email_app_name: str = 'outlook.application'):
 
         if logger:
             self._logger = logger
@@ -79,27 +82,33 @@
         else:
             try:
                 raise ValueError("This message has no body.")
             except ValueError as e:
                 self._logger.error(e, exc_info=True)
                 raise e
 
-    def FindMsgBySubject(self, subject: str, forwarded_message_match: bool = True) -> list:
+    def FindMsgBySubject(self, subject: str, forwarded_message_match: bool = True,
+                         reply_msg_match: bool = True) -> list:
         """Matches the message.Subject string to the subject attr string and returns a list of messages.
         If forward_message_match is True than messages are matched without
         regard to if they start with 'FW:' or 'FWD:'"""
         matched_messages = []
         for message in self.GetMessages():
             if forwarded_message_match:
                 if (message.Subject == subject or
                         (message.Subject.startswith('FW:')
                          and message.Subject.split('FW:')[1].strip() == subject) or
                         (message.Subject.startswith('FWD:')
                          and message.Subject.split('FWD:')[1].strip() == subject)):
                     matched_messages.append(message)
+            if reply_msg_match:
+                if (message.Subject == subject or
+                        (message.Subject.startswith('RE:')
+                         and message.Subject.split('RE:')[1].strip() == subject)):
+                    matched_messages.append(message)
             else:
                 if message.Subject == subject:
                     matched_messages.append(message)
 
         return matched_messages
 
     def SaveAllEmailAttachments(self, msg, save_dir_path):
```

### Comparing `PyEmailerAJM-1.2/PyEmailerAJM.egg-info/PKG-INFO` & `PyEmailerAJM-1.3/PyEmailerAJM.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.2
+Version: 1.3
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.2.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.3.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.2/setup.py` & `PyEmailerAJM-1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(
     name='PyEmailerAJM',
-    version='1.2',
+    version='1.3',
     packages=['PyEmailerAJM'],
     url='https://github.com/amcsparron2793-Water/PyEmailer',
-    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.2.tar.gz',
+    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.3.tar.gz',
     keywords=["Outlook", "Email", "Automation"],
     install_requires=['pywin32'],
     license='MIT License',
     author='Amcsparron',
     author_email='amcsparron@albanyny.gov',
     description='Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support'
 )
```

