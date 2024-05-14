# Comparing `tmp/shox-0.1.1.tar.gz` & `tmp/shox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shox-0.1.1.tar", last modified: Tue May 14 21:21:59 2024, max compression
+gzip compressed data, was "shox-0.1.3.tar", last modified: Tue May 14 21:40:41 2024, max compression
```

## Comparing `shox-0.1.1.tar` & `shox-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:21:59.237070 shox-0.1.1/
--rw-r--r--   0 eric      (1000) eric      (1000)       54 2024-05-14 20:53:51.000000 shox-0.1.1/MANIFEST.in
--rw-r--r--   0 eric      (1000) eric      (1000)      792 2024-05-14 21:21:59.236070 shox-0.1.1/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)      280 2024-05-14 20:43:41.000000 shox-0.1.1/README.md
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:21:59.234070 shox-0.1.1/Shodan/
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:21:59.235070 shox-0.1.1/Shodan/IPResult/
--rw-r--r--   0 eric      (1000) eric      (1000)        0 2024-05-11 07:39:44.000000 shox-0.1.1/Shodan/IPResult/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)      813 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/IPResult/general_information.py
--rw-r--r--   0 eric      (1000) eric      (1000)      485 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/IPResult/ip_result.py
--rw-r--r--   0 eric      (1000) eric      (1000)      184 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/IPResult/open_ports.py
--rw-r--r--   0 eric      (1000) eric      (1000)     2573 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/IPResult/vulnerabilities.py
--rw-r--r--   0 eric      (1000) eric      (1000)      233 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/IPResult/web_technologies.py
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:21:59.235070 shox-0.1.1/Shodan/URLResult/
--rw-r--r--   0 eric      (1000) eric      (1000)        0 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/URLResult/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)        0 2024-05-11 07:39:44.000000 shox-0.1.1/Shodan/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     3531 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/cli_jib.py
--rw-r--r--   0 eric      (1000) eric      (1000)     2177 2024-05-14 20:43:41.000000 shox-0.1.1/Shodan/shodan_temp.py
--rw-r--r--   0 eric      (1000) eric      (1000)       53 2024-05-14 21:07:25.000000 shox-0.1.1/requirements.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       38 2024-05-14 21:21:59.237070 shox-0.1.1/setup.cfg
--rw-r--r--   0 eric      (1000) eric      (1000)     1026 2024-05-14 21:21:55.000000 shox-0.1.1/setup.py
-drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:21:59.236070 shox-0.1.1/shox.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)      792 2024-05-14 21:21:59.000000 shox-0.1.1/shox.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)      502 2024-05-14 21:21:59.000000 shox-0.1.1/shox.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        1 2024-05-14 21:21:59.000000 shox-0.1.1/shox.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       48 2024-05-14 21:21:59.000000 shox-0.1.1/shox.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       54 2024-05-14 21:21:59.000000 shox-0.1.1/shox.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        7 2024-05-14 21:21:59.000000 shox-0.1.1/shox.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:40:41.023144 shox-0.1.3/
+-rw-r--r--   0 eric      (1000) eric      (1000)       54 2024-05-14 20:53:51.000000 shox-0.1.3/MANIFEST.in
+-rw-r--r--   0 eric      (1000) eric      (1000)      792 2024-05-14 21:40:41.022144 shox-0.1.3/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)      280 2024-05-14 20:43:41.000000 shox-0.1.3/README.md
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:40:41.017144 shox-0.1.3/Shodan/
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:40:41.019144 shox-0.1.3/Shodan/IPResult/
+-rw-r--r--   0 eric      (1000) eric      (1000)        0 2024-05-11 07:39:44.000000 shox-0.1.3/Shodan/IPResult/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)      813 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/IPResult/general_information.py
+-rw-r--r--   0 eric      (1000) eric      (1000)      485 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/IPResult/ip_result.py
+-rw-r--r--   0 eric      (1000) eric      (1000)      184 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/IPResult/open_ports.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     2573 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/IPResult/vulnerabilities.py
+-rw-r--r--   0 eric      (1000) eric      (1000)      233 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/IPResult/web_technologies.py
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:40:41.021144 shox-0.1.3/Shodan/URLResult/
+-rw-r--r--   0 eric      (1000) eric      (1000)        0 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/URLResult/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)        0 2024-05-11 07:39:44.000000 shox-0.1.3/Shodan/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     3531 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/cli_jib.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     2177 2024-05-14 20:43:41.000000 shox-0.1.3/Shodan/shodan_temp.py
+-rw-r--r--   0 eric      (1000) eric      (1000)       53 2024-05-14 21:07:25.000000 shox-0.1.3/requirements.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       38 2024-05-14 21:40:41.023144 shox-0.1.3/setup.cfg
+-rw-r--r--   0 eric      (1000) eric      (1000)     1041 2024-05-14 21:35:42.000000 shox-0.1.3/setup.py
+drwxr-xr-x   0 eric      (1000) eric      (1000)        0 2024-05-14 21:40:41.022144 shox-0.1.3/shox.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)      792 2024-05-14 21:40:40.000000 shox-0.1.3/shox.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)      502 2024-05-14 21:40:40.000000 shox-0.1.3/shox.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2024-05-14 21:40:40.000000 shox-0.1.3/shox.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       63 2024-05-14 21:40:40.000000 shox-0.1.3/shox.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       54 2024-05-14 21:40:40.000000 shox-0.1.3/shox.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        7 2024-05-14 21:40:40.000000 shox-0.1.3/shox.egg-info/top_level.txt
```

### Comparing `shox-0.1.1/PKG-INFO` & `shox-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shox
-Version: 0.1.1
+Version: 0.1.3
 Summary: A powerful tool that combines the port-scanning and OSINT-gathering capabilities of shodan.io with the onhand downloadable exploits of ExploitDB.
 Home-page: https://gitlab.com/JIbald/shox
 Author: Vadin02
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shox-0.1.1/Shodan/IPResult/general_information.py` & `shox-0.1.3/Shodan/IPResult/general_information.py`

 * *Files identical despite different names*

### Comparing `shox-0.1.1/Shodan/IPResult/vulnerabilities.py` & `shox-0.1.3/Shodan/IPResult/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `shox-0.1.1/Shodan/cli_jib.py` & `shox-0.1.3/Shodan/cli_jib.py`

 * *Files identical despite different names*

### Comparing `shox-0.1.1/Shodan/shodan_temp.py` & `shox-0.1.3/Shodan/shodan_temp.py`

 * *Files identical despite different names*

### Comparing `shox-0.1.1/setup.py` & `shox-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='shox',
-    version='0.1.1',
+    version='0.1.3',
     description='A powerful tool that combines the port-scanning and OSINT-gathering capabilities of shodan.io with the onhand downloadable exploits of ExploitDB.',
     author='Vadin02',
     url='https://gitlab.com/JIbald/shox',
     packages=find_packages(),
     install_requires=[
         'flask',
         'flasgger',
         'click',
         'requests',
         'beautifulsoup4',
         'selenium',
     ],
     entry_points={
         'console_scripts': [
-            'shox-api=api',
-            'shox-cli=cli',
+            'shox-api=api:start',
+            'shox-cli=cli:call_api',
         ],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `shox-0.1.1/shox.egg-info/PKG-INFO` & `shox-0.1.3/shox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shox
-Version: 0.1.1
+Version: 0.1.3
 Summary: A powerful tool that combines the port-scanning and OSINT-gathering capabilities of shodan.io with the onhand downloadable exploits of ExploitDB.
 Home-page: https://gitlab.com/JIbald/shox
 Author: Vadin02
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

