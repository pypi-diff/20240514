# Comparing `tmp/sshanalysis-0.0.1.tar.gz` & `tmp/sshanalysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sshanalysis-0.0.1.tar", last modified: Mon Oct 18 08:28:49 2021, max compression
+gzip compressed data, was "sshanalysis-0.0.2.tar", last modified: Tue May 14 07:35:06 2024, max compression
```

## Comparing `sshanalysis-0.0.1.tar` & `sshanalysis-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-10-18 08:28:49.358342 sshanalysis-0.0.1/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4740 2021-10-18 08:28:49.358342 sshanalysis-0.0.1/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4195 2021-10-18 08:28:01.000000 sshanalysis-0.0.1/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2021-10-18 08:28:49.358342 sshanalysis-0.0.1/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      974 2021-10-18 08:04:16.000000 sshanalysis-0.0.1/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-10-18 08:28:49.342746 sshanalysis-0.0.1/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-10-18 08:28:49.358342 sshanalysis-0.0.1/src/sshanalysis.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4740 2021-10-18 08:28:48.000000 sshanalysis-0.0.1/src/sshanalysis.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      235 2021-10-18 08:28:48.000000 sshanalysis-0.0.1/src/sshanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2021-10-18 08:28:48.000000 sshanalysis-0.0.1/src/sshanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       50 2021-10-18 08:28:48.000000 sshanalysis-0.0.1/src/sshanalysis.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       12 2021-10-18 08:28:48.000000 sshanalysis-0.0.1/src/sshanalysis.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5391 2021-10-18 08:11:11.000000 sshanalysis-0.0.1/src/sshanalysis.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-14 07:35:06.687361 sshanalysis-0.0.2/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5007 2024-05-14 07:35:06.687361 sshanalysis-0.0.2/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4460 2024-05-14 07:32:51.000000 sshanalysis-0.0.2/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-05-14 07:35:06.687361 sshanalysis-0.0.2/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      976 2024-05-14 07:33:48.000000 sshanalysis-0.0.2/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-14 07:35:06.687361 sshanalysis-0.0.2/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-14 07:35:06.687361 sshanalysis-0.0.2/src/sshanalysis.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5007 2024-05-14 07:35:06.000000 sshanalysis-0.0.2/src/sshanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      235 2024-05-14 07:35:06.000000 sshanalysis-0.0.2/src/sshanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-05-14 07:35:06.000000 sshanalysis-0.0.2/src/sshanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       50 2024-05-14 07:35:06.000000 sshanalysis-0.0.2/src/sshanalysis.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       12 2024-05-14 07:35:06.000000 sshanalysis-0.0.2/src/sshanalysis.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     5391 2021-10-18 08:11:11.000000 sshanalysis-0.0.2/src/sshanalysis.py
```

### Comparing `sshanalysis-0.0.1/PKG-INFO` & `sshanalysis-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: sshanalysis
-Version: 0.0.1
+Version: 0.0.2
 Summary: A visualization analysis tool against ssh-server attacks
-Home-page: https://github.com/ytakefuji/sshanalysis
+Home-page: https://github.com/y-takefuji/sshanalysis
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/sshanalysis
+Project-URL: Bug Tracker, https://github.com/y-takefuji/sshanalysis
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # How to install sshanalysis on Linux
+This research is under review.
+
+sshanalysis has been downloaded by 484 users worldwide.
+
 <pre>
-sshanalysis is available in public and can be installed by pip command:
+sshanalysis is available in public and can be installed 
+by pip command:
 $pip install -U sshanalysis
 </pre>
 
 # How to run sshanalysis on Linux
 <pre>
-$ sshanalysis ssh_log_file
+$ sshanalysis your_ssh_log_file
 or
 $ sshanalysis /var/log/auth.log
 or
 When you run the following command, the file /var/log/auth.log will be used automatically.
 $ sshanalysis
 </pre>
 
@@ -85,19 +90,19 @@
 The larger circle, the more number of attacks against a ssh server.
 Although, country names were embedded on each graph,
 no one knows whether captured IPs are true, spoofed, or springboarded.
 
 sshanalysis can generate all IPs with the number of recorded attacks.
 sshanalysis can generate top 10 IPs information associated with locations (country names).
 
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/neuro.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu1.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu2.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu3.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu4.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/neuro.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu1.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu2.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu3.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu4.png' width=640 height=480>
 
 # sshanalysis.py
 sshanalysis.py consists of three modules. 
 The first module generates a csv file containing the number of recorded attacks 
 against the sorted IP addresses by using a /var/log/auth.log file or the specified log_file. 
 The second module is for generating the country names associated with the captured IP addresses in the specified log_file. 
 And the last module is for drawing a circle-graph.
@@ -109,14 +114,20 @@
 sshanalysis.py can generate an IPs file (all attacking IPs with the number of attacks), 
 top 10 r.csv file (the number of attacks, IP address, country name), 
 and r.png (circle graph).
 
 We don't know whether captured IPs are true, spoofed, or springboarded.
 
 # auth.log
+The maximum size of github file is 25M.
+
+The split command is used to split the auth.log file into multiple files of 20M in size.
+
+$ split -b 20M auth.log auth_log
+
 My auth.log was split into two files: auth_logaa and auth_logab.
 
 To create auth.log, cat auth_log* >auth.log
```

### Comparing `sshanalysis-0.0.1/README.md` & `sshanalysis-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # How to install sshanalysis on Linux
+This research is under review.
+
+sshanalysis has been downloaded by 484 users worldwide.
+
 <pre>
-sshanalysis is available in public and can be installed by pip command:
+sshanalysis is available in public and can be installed 
+by pip command:
 $pip install -U sshanalysis
 </pre>
 
 # How to run sshanalysis on Linux
 <pre>
-$ sshanalysis ssh_log_file
+$ sshanalysis your_ssh_log_file
 or
 $ sshanalysis /var/log/auth.log
 or
 When you run the following command, the file /var/log/auth.log will be used automatically.
 $ sshanalysis
 </pre>
 
@@ -69,19 +74,19 @@
 The larger circle, the more number of attacks against a ssh server.
 Although, country names were embedded on each graph,
 no one knows whether captured IPs are true, spoofed, or springboarded.
 
 sshanalysis can generate all IPs with the number of recorded attacks.
 sshanalysis can generate top 10 IPs information associated with locations (country names).
 
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/neuro.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu1.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu2.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu3.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu4.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/neuro.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu1.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu2.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu3.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu4.png' width=640 height=480>
 
 # sshanalysis.py
 sshanalysis.py consists of three modules. 
 The first module generates a csv file containing the number of recorded attacks 
 against the sorted IP addresses by using a /var/log/auth.log file or the specified log_file. 
 The second module is for generating the country names associated with the captured IP addresses in the specified log_file. 
 And the last module is for drawing a circle-graph.
@@ -93,13 +98,19 @@
 sshanalysis.py can generate an IPs file (all attacking IPs with the number of attacks), 
 top 10 r.csv file (the number of attacks, IP address, country name), 
 and r.png (circle graph).
 
 We don't know whether captured IPs are true, spoofed, or springboarded.
 
 # auth.log
+The maximum size of github file is 25M.
+
+The split command is used to split the auth.log file into multiple files of 20M in size.
+
+$ split -b 20M auth.log auth_log
+
 My auth.log was split into two files: auth_logaa and auth_logab.
 
 To create auth.log, cat auth_log* >auth.log
```

### Comparing `sshanalysis-0.0.1/setup.py` & `sshanalysis-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sshanalysis",
-    version="0.0.1",
+    version="0.0.2",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A visualization analysis tool against ssh-server attacks",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/sshanalysis",
+    url="https://github.com/y-takefuji/sshanalysis",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/sshanalysis",
+        "Bug Tracker": "https://github.com/y-takefuji/sshanalysis",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['sshanalysis'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'sshanalysis = sshanalysis:main'
         ]
     },
 )
```

### Comparing `sshanalysis-0.0.1/src/sshanalysis.egg-info/PKG-INFO` & `sshanalysis-0.0.2/src/sshanalysis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: sshanalysis
-Version: 0.0.1
+Version: 0.0.2
 Summary: A visualization analysis tool against ssh-server attacks
-Home-page: https://github.com/ytakefuji/sshanalysis
+Home-page: https://github.com/y-takefuji/sshanalysis
 Author: yoshiyasu takefuji
 Author-email: takefuji@keio.jp
 License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/ytakefuji/sshanalysis
+Project-URL: Bug Tracker, https://github.com/y-takefuji/sshanalysis
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # How to install sshanalysis on Linux
+This research is under review.
+
+sshanalysis has been downloaded by 484 users worldwide.
+
 <pre>
-sshanalysis is available in public and can be installed by pip command:
+sshanalysis is available in public and can be installed 
+by pip command:
 $pip install -U sshanalysis
 </pre>
 
 # How to run sshanalysis on Linux
 <pre>
-$ sshanalysis ssh_log_file
+$ sshanalysis your_ssh_log_file
 or
 $ sshanalysis /var/log/auth.log
 or
 When you run the following command, the file /var/log/auth.log will be used automatically.
 $ sshanalysis
 </pre>
 
@@ -85,19 +90,19 @@
 The larger circle, the more number of attacks against a ssh server.
 Although, country names were embedded on each graph,
 no one knows whether captured IPs are true, spoofed, or springboarded.
 
 sshanalysis can generate all IPs with the number of recorded attacks.
 sshanalysis can generate top 10 IPs information associated with locations (country names).
 
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/neuro.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu1.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu2.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu3.png' width=640 height=480>
-<img src='https://github.com/ytakefuji/sshanalysis/raw/main/gpu4.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/neuro.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu1.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu2.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu3.png' width=640 height=480>
+<img src='https://github.com/y-takefuji/sshanalysis/raw/main/gpu4.png' width=640 height=480>
 
 # sshanalysis.py
 sshanalysis.py consists of three modules. 
 The first module generates a csv file containing the number of recorded attacks 
 against the sorted IP addresses by using a /var/log/auth.log file or the specified log_file. 
 The second module is for generating the country names associated with the captured IP addresses in the specified log_file. 
 And the last module is for drawing a circle-graph.
@@ -109,14 +114,20 @@
 sshanalysis.py can generate an IPs file (all attacking IPs with the number of attacks), 
 top 10 r.csv file (the number of attacks, IP address, country name), 
 and r.png (circle graph).
 
 We don't know whether captured IPs are true, spoofed, or springboarded.
 
 # auth.log
+The maximum size of github file is 25M.
+
+The split command is used to split the auth.log file into multiple files of 20M in size.
+
+$ split -b 20M auth.log auth_log
+
 My auth.log was split into two files: auth_logaa and auth_logab.
 
 To create auth.log, cat auth_log* >auth.log
```

### Comparing `sshanalysis-0.0.1/src/sshanalysis.py` & `sshanalysis-0.0.2/src/sshanalysis.py`

 * *Files identical despite different names*

