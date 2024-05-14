# Comparing `tmp/vuv-0.0.3.tar.gz` & `tmp/vuv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vuv-0.0.3.tar", last modified: Sun Feb 19 06:59:37 2023, max compression
+gzip compressed data, was "vuv-0.0.4.tar", last modified: Tue May 14 07:28:00 2024, max compression
```

## Comparing `vuv-0.0.3.tar` & `vuv-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-19 06:59:37.976845 vuv-0.0.3/
--rw-r--r--   0 yt        (1000) yt        (1000)     1140 2023-02-19 06:59:37.976845 vuv-0.0.3/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      603 2023-02-18 11:08:07.000000 vuv-0.0.3/README.md
--rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-02-19 06:59:37.976845 vuv-0.0.3/setup.cfg
--rw-r--r--   0 yt        (1000) yt        (1000)      942 2023-02-19 06:58:25.000000 vuv-0.0.3/setup.py
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-19 06:59:37.976845 vuv-0.0.3/src/
-drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-02-19 06:59:37.976845 vuv-0.0.3/src/vuv.egg-info/
--rw-r--r--   0 yt        (1000) yt        (1000)     1140 2023-02-19 06:59:37.000000 vuv-0.0.3/src/vuv.egg-info/PKG-INFO
--rw-r--r--   0 yt        (1000) yt        (1000)      187 2023-02-19 06:59:37.000000 vuv-0.0.3/src/vuv.egg-info/SOURCES.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-02-19 06:59:37.000000 vuv-0.0.3/src/vuv.egg-info/dependency_links.txt
--rw-r--r--   0 yt        (1000) yt        (1000)       34 2023-02-19 06:59:37.000000 vuv-0.0.3/src/vuv.egg-info/entry_points.txt
--rw-r--r--   0 yt        (1000) yt        (1000)        4 2023-02-19 06:59:37.000000 vuv-0.0.3/src/vuv.egg-info/top_level.txt
--rw-r--r--   0 yt        (1000) yt        (1000)     1284 2023-02-19 06:58:09.000000 vuv-0.0.3/src/vuv.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-14 07:28:00.417365 vuv-0.0.4/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1632 2024-05-14 07:28:00.417365 vuv-0.0.4/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1093 2024-05-14 06:38:50.000000 vuv-0.0.4/README.md
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2024-05-14 07:28:00.417365 vuv-0.0.4/setup.cfg
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      944 2024-05-14 06:39:39.000000 vuv-0.0.4/setup.py
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-14 07:28:00.417365 vuv-0.0.4/src/
+drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2024-05-14 07:28:00.417365 vuv-0.0.4/src/vuv.egg-info/
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1632 2024-05-14 07:28:00.000000 vuv-0.0.4/src/vuv.egg-info/PKG-INFO
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)      187 2024-05-14 07:28:00.000000 vuv-0.0.4/src/vuv.egg-info/SOURCES.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2024-05-14 07:28:00.000000 vuv-0.0.4/src/vuv.egg-info/dependency_links.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)       34 2024-05-14 07:28:00.000000 vuv-0.0.4/src/vuv.egg-info/entry_points.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)        4 2024-05-14 07:28:00.000000 vuv-0.0.4/src/vuv.egg-info/top_level.txt
+-rw-r--r--   0 takefuji  (1000) takefuji  (1000)     1284 2023-02-19 06:58:09.000000 vuv-0.0.4/src/vuv.py
```

### Comparing `vuv-0.0.3/setup.py` & `vuv-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="vuv",
-    version="0.0.3",
+    version="0.0.4",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="comparing effects on mortality between fully vaccinated and unvaccinated",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ytakefuji/vuv",
+    url="https://github.com/y-takefuji/vuv",
     project_urls={
-        "Bug Tracker": "https://github.com/ytakefuji/vuv",
+        "Bug Tracker": "https://github.com/y-takefuji/vuv",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     py_modules=['vuv'],
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     entry_points = {
         'console_scripts': [
             'vuv = vuv:main'
         ]
     },
 )
```

### Comparing `vuv-0.0.3/src/vuv.py` & `vuv-0.0.4/src/vuv.py`

 * *Files identical despite different names*

