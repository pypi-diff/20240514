# Comparing `tmp/netbox_contextmenus-1.4.0.tar.gz` & `tmp/netbox_contextmenus-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_contextmenus-1.4.0.tar", last modified: Fri May 10 13:28:15 2024, max compression
+gzip compressed data, was "netbox_contextmenus-1.4.1.tar", last modified: Tue May 14 11:01:11 2024, max compression
```

## Comparing `netbox_contextmenus-1.4.0.tar` & `netbox_contextmenus-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:28:15.157003 netbox_contextmenus-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 13:28:07.000000 netbox_contextmenus-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 13:28:15.157003 netbox_contextmenus-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-10 13:28:07.000000 netbox_contextmenus-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:28:15.153003 netbox_contextmenus-1.4.0/netbox_contextmenus/
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-10 13:28:07.000000 netbox_contextmenus-1.4.0/netbox_contextmenus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-10 13:28:07.000000 netbox_contextmenus-1.4.0/netbox_contextmenus/pluginvars.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-10 13:28:07.000000 netbox_contextmenus-1.4.0/netbox_contextmenus/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:28:15.153003 netbox_contextmenus-1.4.0/netbox_contextmenus/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:28:15.153003 netbox_contextmenus-1.4.0/netbox_contextmenus/static/netbox_contextmenus/
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-05-10 13:28:07.000000 netbox_contextmenus-1.4.0/netbox_contextmenus/static/netbox_contextmenus/nbcm.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:28:15.153003 netbox_contextmenus-1.4.0/netbox_contextmenus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 13:28:15.000000 netbox_contextmenus-1.4.0/netbox_contextmenus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-10 13:28:15.000000 netbox_contextmenus-1.4.0/netbox_contextmenus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:28:15.000000 netbox_contextmenus-1.4.0/netbox_contextmenus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 13:28:15.000000 netbox_contextmenus-1.4.0/netbox_contextmenus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:28:15.157003 netbox_contextmenus-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-10 13:28:07.000000 netbox_contextmenus-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:01:11.555594 netbox_contextmenus-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 11:01:07.000000 netbox_contextmenus-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-14 11:01:11.555594 netbox_contextmenus-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-14 11:01:07.000000 netbox_contextmenus-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:01:11.555594 netbox_contextmenus-1.4.1/netbox_contextmenus/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-14 11:01:07.000000 netbox_contextmenus-1.4.1/netbox_contextmenus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 11:01:07.000000 netbox_contextmenus-1.4.1/netbox_contextmenus/pluginvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-14 11:01:07.000000 netbox_contextmenus-1.4.1/netbox_contextmenus/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:01:11.551594 netbox_contextmenus-1.4.1/netbox_contextmenus/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:01:11.555594 netbox_contextmenus-1.4.1/netbox_contextmenus/static/netbox_contextmenus/
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-05-14 11:01:07.000000 netbox_contextmenus-1.4.1/netbox_contextmenus/static/netbox_contextmenus/nbcm.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:01:11.555594 netbox_contextmenus-1.4.1/netbox_contextmenus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-14 11:01:11.000000 netbox_contextmenus-1.4.1/netbox_contextmenus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-14 11:01:11.000000 netbox_contextmenus-1.4.1/netbox_contextmenus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:01:11.000000 netbox_contextmenus-1.4.1/netbox_contextmenus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 11:01:11.000000 netbox_contextmenus-1.4.1/netbox_contextmenus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:01:11.555594 netbox_contextmenus-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-14 11:01:07.000000 netbox_contextmenus-1.4.1/setup.py
```

### Comparing `netbox_contextmenus-1.4.0/PKG-INFO` & `netbox_contextmenus-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_contextmenus
-Version: 1.4.0
+Version: 1.4.1
 Summary: Add context menu to links in NetBox
 Home-page: https://github.com/PieterL75/netbox_contextmenus
 Author: Pieter Lambrecht
 Author-email: pieter.lambrecht@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +21,9 @@
 
 ## Installation:
 
 - install as a any regular plugin.  See  [https://docs.netbox.dev/en/stable/plugins/installation/](https://docs.netbox.dev/en/stable/plugins/installation/)
 - PyPi Packagename is 'netbox-contextmenus'.
 - NetBox packagenam is 'netbox_contextmenus'.
 - Remove (delete, remark) BANNER_BOTTOM from the configuration file. If you need to set a bottom banner, then use the ConfigurationRevisions of NetBox [https://docs.netbox.dev/en/stable/configuration/#dynamic-configuration-parameters](https://docs.netbox.dev/en/stable/configuration/#dynamic-configuration-parameters)
+- run a collect static `/opt/netbox/venv/bin/python3 manage.py collectstatic --no-input`
 - restart the netbox service
```

### Comparing `netbox_contextmenus-1.4.0/README.md` & `netbox_contextmenus-1.4.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 
 ## Installation:
 
 - install as a any regular plugin.  See  [https://docs.netbox.dev/en/stable/plugins/installation/](https://docs.netbox.dev/en/stable/plugins/installation/)
 - PyPi Packagename is 'netbox-contextmenus'.
 - NetBox packagenam is 'netbox_contextmenus'.
 - Remove (delete, remark) BANNER_BOTTOM from the configuration file. If you need to set a bottom banner, then use the ConfigurationRevisions of NetBox [https://docs.netbox.dev/en/stable/configuration/#dynamic-configuration-parameters](https://docs.netbox.dev/en/stable/configuration/#dynamic-configuration-parameters)
+- run a collect static `/opt/netbox/venv/bin/python3 manage.py collectstatic --no-input`
 - restart the netbox service
```

### Comparing `netbox_contextmenus-1.4.0/netbox_contextmenus/signals.py` & `netbox_contextmenus-1.4.1/netbox_contextmenus/signals.py`

 * *Files identical despite different names*

### Comparing `netbox_contextmenus-1.4.0/netbox_contextmenus/static/netbox_contextmenus/nbcm.js` & `netbox_contextmenus-1.4.1/netbox_contextmenus/static/netbox_contextmenus/nbcm.js`

 * *Files identical despite different names*

### Comparing `netbox_contextmenus-1.4.0/netbox_contextmenus.egg-info/PKG-INFO` & `netbox_contextmenus-1.4.1/netbox_contextmenus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_contextmenus
-Version: 1.4.0
+Version: 1.4.1
 Summary: Add context menu to links in NetBox
 Home-page: https://github.com/PieterL75/netbox_contextmenus
 Author: Pieter Lambrecht
 Author-email: pieter.lambrecht@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
@@ -21,8 +21,9 @@
 
 ## Installation:
 
 - install as a any regular plugin.  See  [https://docs.netbox.dev/en/stable/plugins/installation/](https://docs.netbox.dev/en/stable/plugins/installation/)
 - PyPi Packagename is 'netbox-contextmenus'.
 - NetBox packagenam is 'netbox_contextmenus'.
 - Remove (delete, remark) BANNER_BOTTOM from the configuration file. If you need to set a bottom banner, then use the ConfigurationRevisions of NetBox [https://docs.netbox.dev/en/stable/configuration/#dynamic-configuration-parameters](https://docs.netbox.dev/en/stable/configuration/#dynamic-configuration-parameters)
+- run a collect static `/opt/netbox/venv/bin/python3 manage.py collectstatic --no-input`
 - restart the netbox service
```

### Comparing `netbox_contextmenus-1.4.0/setup.py` & `netbox_contextmenus-1.4.1/setup.py`

 * *Files identical despite different names*

