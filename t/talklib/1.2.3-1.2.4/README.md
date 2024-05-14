# Comparing `tmp/talklib-1.2.3.tar.gz` & `tmp/talklib-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talklib-1.2.3.tar", last modified: Fri May 10 16:33:09 2024, max compression
+gzip compressed data, was "talklib-1.2.4.tar", last modified: Tue May 14 14:54:01 2024, max compression
```

## Comparing `talklib-1.2.3.tar` & `talklib-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:33:09.886851 talklib-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-10 16:33:04.000000 talklib-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-10 16:33:09.886851 talklib-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-05-10 16:33:04.000000 talklib-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-10 16:33:04.000000 talklib-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 16:33:04.000000 talklib-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:33:09.886851 talklib-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:33:09.882851 talklib-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:33:09.886851 talklib-1.2.3/src/talklib/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 16:33:04.000000 talklib-1.2.3/src/talklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-10 16:33:04.000000 talklib-1.2.3/src/talklib/ev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-10 16:33:04.000000 talklib-1.2.3/src/talklib/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-10 16:33:04.000000 talklib-1.2.3/src/talklib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)    22305 2024-05-10 16:33:04.000000 talklib-1.2.3/src/talklib/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-10 16:33:04.000000 talklib-1.2.3/src/talklib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:33:09.886851 talklib-1.2.3/src/talklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-10 16:33:09.000000 talklib-1.2.3/src/talklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-10 16:33:09.000000 talklib-1.2.3/src/talklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:33:09.000000 talklib-1.2.3/src/talklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 16:33:09.000000 talklib-1.2.3/src/talklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 16:33:09.000000 talklib-1.2.3/src/talklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:54:01.230472 talklib-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-14 14:53:55.000000 talklib-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-14 14:54:01.230472 talklib-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-05-14 14:53:55.000000 talklib-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 14:53:55.000000 talklib-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 14:53:55.000000 talklib-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:54:01.230472 talklib-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:54:01.226472 talklib-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:54:01.226472 talklib-1.2.4/src/talklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-14 14:53:55.000000 talklib-1.2.4/src/talklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-14 14:53:55.000000 talklib-1.2.4/src/talklib/ev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-14 14:53:55.000000 talklib-1.2.4/src/talklib/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-14 14:53:55.000000 talklib-1.2.4/src/talklib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22305 2024-05-14 14:53:55.000000 talklib-1.2.4/src/talklib/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-14 14:53:55.000000 talklib-1.2.4/src/talklib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:54:01.230472 talklib-1.2.4/src/talklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-14 14:54:01.000000 talklib-1.2.4/src/talklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 14:54:01.000000 talklib-1.2.4/src/talklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:54:01.000000 talklib-1.2.4/src/talklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 14:54:01.000000 talklib-1.2.4/src/talklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 14:54:01.000000 talklib-1.2.4/src/talklib.egg-info/top_level.txt
```

### Comparing `talklib-1.2.3/LICENSE.txt` & `talklib-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.2.3/PKG-INFO` & `talklib-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.2.3/README.md` & `talklib-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `talklib-1.2.3/pyproject.toml` & `talklib-1.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "talklib"
-version = "1.2.3"
+version = "1.2.4"
 description = "A package to automate processing of shows/segments airing on the TL"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 maintainers = [{name = "Ben Weddle", email = "ben.weddle@gmail.com"}]
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
```

### Comparing `talklib-1.2.3/requirements.txt` & `talklib-1.2.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `talklib-1.2.3/src/talklib/ev.py` & `talklib-1.2.4/src/talklib/ev.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.3/src/talklib/ffmpeg.py` & `talklib-1.2.4/src/talklib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.3/src/talklib/notify.py` & `talklib-1.2.4/src/talklib/notify.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,12 +86,12 @@
         '''send email to TL gmail account via relay address'''
         if not (self.email_enable and self.enable_all):
             return
         format = EmailMessage()
         format.set_content(message)
         format['Subject'] = subject
         format['From'] = self.EV.fromEmail
-        format['To'] = "ben.weddle@nashville.gov" # PLEASE FIX ME!!
+        format['To'] = self.EV.toEmail
 
         mail = smtplib.SMTP(host=self.EV.mail_server)
         mail.send_message(format)
         mail.quit()
```

### Comparing `talklib-1.2.3/src/talklib/show.py` & `talklib-1.2.4/src/talklib/show.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.3/src/talklib/utils.py` & `talklib-1.2.4/src/talklib/utils.py`

 * *Files identical despite different names*

### Comparing `talklib-1.2.3/src/talklib.egg-info/PKG-INFO` & `talklib-1.2.4/src/talklib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talklib
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package to automate processing of shows/segments airing on the TL
 Author-email: Ben Weddle <ben.weddle@gmail.com>
 Maintainer-email: Ben Weddle <ben.weddle@gmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `talklib-1.2.3/src/talklib.egg-info/requires.txt` & `talklib-1.2.4/src/talklib.egg-info/requires.txt`

 * *Files identical despite different names*

