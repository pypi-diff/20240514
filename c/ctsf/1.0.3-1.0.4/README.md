# Comparing `tmp/ctsf-1.0.3.tar.gz` & `tmp/ctsf-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctsf-1.0.3.tar", last modified: Sat May 11 12:02:27 2024, max compression
+gzip compressed data, was "ctsf-1.0.4.tar", last modified: Tue May 14 03:28:03 2024, max compression
```

## Comparing `ctsf-1.0.3.tar` & `ctsf-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:02:27.868236 ctsf-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 12:02:23.000000 ctsf-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-11 12:02:27.868236 ctsf-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-11 12:02:23.000000 ctsf-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:02:27.868236 ctsf-1.0.3/ctsf/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:02:27.868236 ctsf-1.0.3/ctsf/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/ctsf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:02:27.868236 ctsf-1.0.3/ctsf/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/modules/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-11 12:02:23.000000 ctsf-1.0.3/ctsf/modules/who.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:02:27.868236 ctsf-1.0.3/ctsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-11 12:02:27.000000 ctsf-1.0.3/ctsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-11 12:02:27.000000 ctsf-1.0.3/ctsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:02:27.000000 ctsf-1.0.3/ctsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 12:02:27.000000 ctsf-1.0.3/ctsf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 12:02:27.000000 ctsf-1.0.3/ctsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 12:02:27.000000 ctsf-1.0.3/ctsf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:02:27.868236 ctsf-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-11 12:02:23.000000 ctsf-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-14 03:27:59.000000 ctsf-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 03:28:03.844659 ctsf-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-14 03:27:59.000000 ctsf-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.840659 ctsf-1.0.4/ctsf/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/ctsf/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/ctsf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/ctsf/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/modules/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/modules/who.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/ctsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:28:03.844659 ctsf-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-14 03:27:59.000000 ctsf-1.0.4/setup.py
```

### Comparing `ctsf-1.0.3/LICENSE` & `ctsf-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctsf-1.0.3/PKG-INFO` & `ctsf-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctsf
-Version: 1.0.3
+Version: 1.0.4
 Summary: Certificate Transparency Subdomain Finder + WHOIS Data
 Home-page: https://erfansamandarian.com/ctsf
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ctsf-1.0.3/README.md` & `ctsf-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ctsf-1.0.3/ctsf/ctsf.py` & `ctsf-1.0.4/ctsf/ctsf.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 def arguments():
     parser = argparse.ArgumentParser(
         prog="ctsf", description="Certificate Transparency Subdomain Finder"
     )
     parser.add_argument(
         "--domain",
         help="Uniform Resource Locator",
+        required=True
     )
     parser.add_argument(
         "--who",
         help="WHOIS Data",
         default="false",
         action="store_true",
     )
```

### Comparing `ctsf-1.0.3/ctsf/modules/request.py` & `ctsf-1.0.4/ctsf/modules/request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import requests
 
-version = "1.0.3"  # can i change this in setup.py?
+version = "1.0.4"  # can i change this in setup.py?
 
 
 def banner():
     banner = """
 .------..------..------..------.
 |C.--. ||T.--. ||F.--. ||S.--. |
 | :/\: || :/\: || :(): || :/\: |
@@ -27,18 +27,17 @@
     banner()
     subdomains = []
     target = clear_url(domain)
 
     req = requests.get("https://crt.sh/?q=%.{d}&output=json".format(d=target))
 
     for index, value in enumerate(req.json()):
-        if value is not None:
-            subdomains.extend(value["name_value"].split("\n"))
-
-    print("=" * 32)
+        subdomains.extend(value["name_value"].split("\n"))
 
     subdomains = list(sorted(set(subdomains)))  # todo: remove duplicates
 
+    print("=" * 32)
+
     for subdomain in subdomains:
         print("[+] :: {s}".format(s=subdomain))
 
     print("=" * 32)
```

### Comparing `ctsf-1.0.3/ctsf/modules/who.py` & `ctsf-1.0.4/ctsf/modules/who.py`

 * *Files identical despite different names*

### Comparing `ctsf-1.0.3/ctsf.egg-info/PKG-INFO` & `ctsf-1.0.4/ctsf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctsf
-Version: 1.0.3
+Version: 1.0.4
 Summary: Certificate Transparency Subdomain Finder + WHOIS Data
 Home-page: https://erfansamandarian.com/ctsf
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ctsf-1.0.3/setup.py` & `ctsf-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     description="Certificate Transparency Subdomain Finder + WHOIS Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Erfan Samandarian",
     author_email="mail@erfansamandarian.com",
     url="https://erfansamandarian.com/ctsf",
     license="MIT",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     install_requires=["requests", "python-whois"],
     py_modules=["ctsf"],
     entry_points={"console_scripts": ["ctsf=ctsf:main"]},
 )
```

