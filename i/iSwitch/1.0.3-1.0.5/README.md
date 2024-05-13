# Comparing `tmp/iSwitch-1.0.3.tar.gz` & `tmp/iSwitch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iSwitch-1.0.3.tar", last modified: Mon May 13 21:41:06 2024, max compression
+gzip compressed data, was "iSwitch-1.0.5.tar", last modified: Mon May 13 22:02:11 2024, max compression
```

## Comparing `iSwitch-1.0.3.tar` & `iSwitch-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 21:41:06.002993 iSwitch-1.0.3/
--rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.3/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     5119 2024-05-13 21:41:06.002098 iSwitch-1.0.3/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     4768 2024-05-13 19:12:41.000000 iSwitch-1.0.3/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 21:41:06.001156 iSwitch-1.0.3/iSwitch.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     5119 2024-05-13 21:41:05.000000 iSwitch-1.0.3/iSwitch.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-13 21:41:05.000000 iSwitch-1.0.3/iSwitch.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-13 21:41:05.000000 iSwitch-1.0.3/iSwitch.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-13 21:41:05.000000 iSwitch-1.0.3/iSwitch.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-13 21:41:05.000000 iSwitch-1.0.3/iSwitch.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 21:41:05.999981 iSwitch-1.0.3/iswitch/
--rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.3/iswitch/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6560 2024-05-13 16:12:36.000000 iSwitch-1.0.3/iswitch/_client.py
--rw-r--r--   0 mac        (501) staff       (20)     7677 2024-05-12 22:15:34.000000 iSwitch-1.0.3/iswitch/_services.py
--rw-r--r--   0 mac        (501) staff       (20)     7350 2024-05-13 21:39:26.000000 iSwitch-1.0.3/iswitch/_types.py
--rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.3/iswitch/_utils.py
--rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-13 21:41:06.003194 iSwitch-1.0.3/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      617 2024-05-13 21:40:21.000000 iSwitch-1.0.3/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 22:02:11.845070 iSwitch-1.0.5/
+-rw-r--r--   0 mac        (501) staff       (20)     1057 2024-05-11 18:46:44.000000 iSwitch-1.0.5/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     5119 2024-05-13 22:02:11.844569 iSwitch-1.0.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     4768 2024-05-13 19:12:41.000000 iSwitch-1.0.5/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 22:02:11.843951 iSwitch-1.0.5/iSwitch.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     5119 2024-05-13 22:02:11.000000 iSwitch-1.0.5/iSwitch.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      276 2024-05-13 22:02:11.000000 iSwitch-1.0.5/iSwitch.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2024-05-13 22:02:11.000000 iSwitch-1.0.5/iSwitch.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       26 2024-05-13 22:02:11.000000 iSwitch-1.0.5/iSwitch.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        8 2024-05-13 22:02:11.000000 iSwitch-1.0.5/iSwitch.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2024-05-13 22:02:11.843128 iSwitch-1.0.5/iswitch/
+-rw-r--r--   0 mac        (501) staff       (20)      328 2024-05-12 10:01:33.000000 iSwitch-1.0.5/iswitch/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6560 2024-05-13 16:12:36.000000 iSwitch-1.0.5/iswitch/_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     7672 2024-05-13 21:46:29.000000 iSwitch-1.0.5/iswitch/_services.py
+-rw-r--r--   0 mac        (501) staff       (20)     7350 2024-05-13 21:39:26.000000 iSwitch-1.0.5/iswitch/_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     3247 2024-05-12 10:42:22.000000 iSwitch-1.0.5/iswitch/_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)       38 2024-05-13 22:02:11.845414 iSwitch-1.0.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      617 2024-05-13 22:02:04.000000 iSwitch-1.0.5/setup.py
```

### Comparing `iSwitch-1.0.3/LICENSE` & `iSwitch-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.3/PKG-INFO` & `iSwitch-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSwitch
-Version: 1.0.3
+Version: 1.0.5
 Summary: SwitchPay Python SDK for AllDotPy internal use. 
 Home-page: https://github.com/AllDotPy/iSwitch.git
 Author: #Einswilli
 Author-email: einswilligoeh@email.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
```

### Comparing `iSwitch-1.0.3/README.md` & `iSwitch-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.3/iSwitch.egg-info/PKG-INFO` & `iSwitch-1.0.5/iSwitch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iSwitch
-Version: 1.0.3
+Version: 1.0.5
 Summary: SwitchPay Python SDK for AllDotPy internal use. 
 Home-page: https://github.com/AllDotPy/iSwitch.git
 Author: #Einswilli
 Author-email: einswilligoeh@email.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
```

### Comparing `iSwitch-1.0.3/iswitch/_client.py` & `iSwitch-1.0.5/iswitch/_client.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.3/iswitch/_services.py` & `iSwitch-1.0.5/iswitch/_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,11 +231,11 @@
                 ]
             }
         }
     }
     
 
 ##      GET SERVICE FUNCTION
-def get_service(service:str) -> BaseService|None:
+def get_service(service:str) -> BaseService:
     ''' Return service from a given name. '''
     
     return Factory.get(service)
```

### Comparing `iSwitch-1.0.3/iswitch/_types.py` & `iSwitch-1.0.5/iswitch/_types.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.3/iswitch/_utils.py` & `iSwitch-1.0.5/iswitch/_utils.py`

 * *Files identical despite different names*

### Comparing `iSwitch-1.0.3/setup.py` & `iSwitch-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # LOADING DOCUMENTATION
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = 'iSwitch',
-    version = '1.0.3',
+    version = '1.0.5',
     packages = find_packages(),
     install_requires = [
         'httpx',
         'simplejson',
         'colorlog'
     ],
     long_description=long_description,
```

