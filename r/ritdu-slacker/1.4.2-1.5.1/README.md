# Comparing `tmp/ritdu_slacker-1.4.2.tar.gz` & `tmp/ritdu_slacker-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritdu_slacker-1.4.2.tar", max compression
+gzip compressed data, was "ritdu_slacker-1.5.1.tar", max compression
```

## Comparing `ritdu_slacker-1.4.2.tar` & `ritdu_slacker-1.5.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-15 20:15:22.201449 ritdu_slacker-1.4.2/LICENSE
--rw-r--r--   0        0        0     4042 2024-03-15 20:15:22.201449 ritdu_slacker-1.4.2/README.md
--rw-r--r--   0        0        0     1164 2024-03-15 20:15:22.201449 ritdu_slacker-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      610 2024-03-15 20:15:22.201449 ritdu_slacker-1.4.2/ritdu_slacker/__init__.py
--rw-r--r--   0        0        0     2698 2024-03-15 20:15:22.201449 ritdu_slacker-1.4.2/ritdu_slacker/api.py
--rw-r--r--   0        0        0     4880 2024-03-15 20:15:22.201449 ritdu_slacker-1.4.2/ritdu_slacker/cli.py
--rw-r--r--   0        0        0      143 2024-03-15 20:15:22.201449 ritdu_slacker-1.4.2/ritdu_slacker/main.py
--rw-r--r--   0        0        0     5097 1970-01-01 00:00:00.000000 ritdu_slacker-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4220 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/README.md
+-rw-r--r--   0        0        0     1164 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/ritdu_slacker/__init__.py
+-rw-r--r--   0        0        0     2698 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/ritdu_slacker/api.py
+-rw-r--r--   0        0        0     4896 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/ritdu_slacker/cli.py
+-rw-r--r--   0        0        0     2769 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/ritdu_slacker/formatter.py
+-rw-r--r--   0        0        0      143 2024-05-14 08:02:11.278652 ritdu_slacker-1.5.1/ritdu_slacker/main.py
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 ritdu_slacker-1.5.1/PKG-INFO
```

### Comparing `ritdu_slacker-1.4.2/LICENSE` & `ritdu_slacker-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ritdu_slacker-1.4.2/README.md` & `ritdu_slacker-1.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,10 @@
 publish              Publish the package
 setup-binaries       Setup binaries for development. Poetry, Twine.
 test                 Test the package
 vscode               Update VSCode settings
 ```
 
 Please read the _Makefile_ to see what each task does.
+
+## Deployment
+To deploy a new version of the package to PyPI, you need to bump the version in the _pyproject.toml_ file and then push the tag (prefixed by v) to the repository.
```

### Comparing `ritdu_slacker-1.4.2/pyproject.toml` & `ritdu_slacker-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ritdu-slacker"
-version = "1.4.2"
+version = "1.5.1"
 description = "Simple internal Slack API wrapper"
 authors = [
     "Ringier Tech <tools@ringier.co.za>",
 ]
 homepage = "https://github.com/RingierIMU/ritdu-slacker/"
 repository = "https://github.com/RingierIMU/ritdu-slacker/"
 license = "MIT"
```

### Comparing `ritdu_slacker-1.4.2/ritdu_slacker/__init__.py` & `ritdu_slacker-1.5.1/ritdu_slacker/__init__.py`

 * *Files identical despite different names*

### Comparing `ritdu_slacker-1.4.2/ritdu_slacker/api.py` & `ritdu_slacker-1.5.1/ritdu_slacker/api.py`

 * *Files identical despite different names*

### Comparing `ritdu_slacker-1.4.2/ritdu_slacker/cli.py` & `ritdu_slacker-1.5.1/ritdu_slacker/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,17 +83,17 @@
             text = json.loads(text)
         else:
             text = f"{text}"
         result = sender.post_message(
             text=text,
             thread_uuid=thread_uuid if thread_uuid else "",
             message_uuid=message_uuid if message_uuid else "",
-            message_or_thread_uuid=message_or_thread_uuid
-            if message_or_thread_uuid
-            else "",
+            message_or_thread_uuid=(
+                message_or_thread_uuid if message_or_thread_uuid else ""
+            ),
             workspace=workspace,
             command=command,
             channel=channel,
             thread_broadcast=thread_broadcast,
         )
         print(json.dumps(result))
 
@@ -164,17 +164,17 @@
         file_basename = os.path.basename(file)
         sender = get_client()
         with open(file, "rb") as open_file:
             result = sender.post_file(
                 text=f"{text}" if text else f"File: {file_basename}",
                 thread_uuid=thread_uuid if thread_uuid else "",
                 message_uuid=message_uuid if message_uuid else "",
-                message_or_thread_uuid=message_or_thread_uuid
-                if message_or_thread_uuid
-                else "",
+                message_or_thread_uuid=(
+                    message_or_thread_uuid if message_or_thread_uuid else ""
+                ),
                 workspace=workspace,
                 channel=channel,
                 command=command,
                 file_bytes=open_file,
                 thread_broadcast=thread_broadcast,
             )
         print(json.dumps(result))
```

### Comparing `ritdu_slacker-1.4.2/PKG-INFO` & `ritdu_slacker-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ritdu-slacker
-Version: 1.4.2
+Version: 1.5.1
 Summary: Simple internal Slack API wrapper
 Home-page: https://github.com/RingierIMU/ritdu-slacker/
 License: MIT
 Author: Ringier Tech
 Author-email: tools@ringier.co.za
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -95,7 +95,10 @@
 setup-binaries       Setup binaries for development. Poetry, Twine.
 test                 Test the package
 vscode               Update VSCode settings
 ```
 
 Please read the _Makefile_ to see what each task does.
 
+## Deployment
+To deploy a new version of the package to PyPI, you need to bump the version in the _pyproject.toml_ file and then push the tag (prefixed by v) to the repository.
+
```

