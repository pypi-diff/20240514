# Comparing `tmp/sqs_client-0.1.5.tar.gz` & `tmp/sqs_client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqs_client-0.1.5.tar", last modified: Mon May  6 08:50:22 2024, max compression
+gzip compressed data, was "sqs_client-0.1.6.tar", last modified: Tue May 14 04:13:32 2024, max compression
```

## Comparing `sqs_client-0.1.5.tar` & `sqs_client-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:22.767235 sqs_client-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 08:50:08.000000 sqs_client-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-06 08:50:22.767235 sqs_client-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-06 08:50:08.000000 sqs_client-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-06 08:50:08.000000 sqs_client-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 08:50:22.767235 sqs_client-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:22.763235 sqs_client-0.1.5/sqs_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-06 08:50:08.000000 sqs_client-0.1.5/sqs_client/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:50:22.767235 sqs_client-0.1.5/sqs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 08:50:22.000000 sqs_client-0.1.5/sqs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:32.464771 sqs_client-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 04:13:13.000000 sqs_client-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-14 04:13:32.464771 sqs_client-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-14 04:13:13.000000 sqs_client-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-14 04:13:13.000000 sqs_client-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-14 04:13:32.464771 sqs_client-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:32.464771 sqs_client-0.1.6/sqs_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-14 04:13:13.000000 sqs_client-0.1.6/sqs_client/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:13:32.464771 sqs_client-0.1.6/sqs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 04:13:32.000000 sqs_client-0.1.6/sqs_client.egg-info/top_level.txt
```

### Comparing `sqs_client-0.1.5/LICENSE` & `sqs_client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.5/PKG-INFO` & `sqs_client-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqs-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: SQS client
 Author-email: Digital Fortress <hai.huynh@digitalfortress.dev>
 Project-URL: Homepage, https://github.com/digitalfortress-dev/python-sqs-client
 Project-URL: Issues, https://github.com/digitalfortress-dev/python-sqs-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sqs_client-0.1.5/README.md` & `sqs_client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.5/pyproject.toml` & `sqs_client-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqs-client"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Digital Fortress", email="hai.huynh@digitalfortress.dev" },
 ]
 description = "SQS client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sqs_client-0.1.5/sqs_client/client.py` & `sqs_client-0.1.6/sqs_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,19 +173,18 @@
                 WaitTimeSeconds=wait_time_seconds,
             )
 
             if "Messages" in messages and messages["Messages"]:
                 for message in messages["Messages"]:
                     try:
                         callback(message)
+                        self.delete_message(queue_name, message)
                     except Exception as e:
                         exception(e)
 
-                    self.delete_message(queue_name, message)
-
     def publish(
         self,
         queue_name,
         message,
         delay_seconds=0,
     ):
         """
```

### Comparing `sqs_client-0.1.5/sqs_client/publisher.py` & `sqs_client-0.1.6/sqs_client/publisher.py`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.5/sqs_client/task.py` & `sqs_client-0.1.6/sqs_client/task.py`

 * *Files identical despite different names*

### Comparing `sqs_client-0.1.5/sqs_client.egg-info/PKG-INFO` & `sqs_client-0.1.6/sqs_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqs-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: SQS client
 Author-email: Digital Fortress <hai.huynh@digitalfortress.dev>
 Project-URL: Homepage, https://github.com/digitalfortress-dev/python-sqs-client
 Project-URL: Issues, https://github.com/digitalfortress-dev/python-sqs-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

