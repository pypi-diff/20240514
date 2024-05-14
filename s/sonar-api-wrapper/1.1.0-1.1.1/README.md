# Comparing `tmp/sonar_api_wrapper-1.1.0-py3-none-any.whl.zip` & `tmp/sonar_api_wrapper-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6069 bytes, number of entries: 7
+Zip file size: 6093 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      168 b- defN 20-Feb-02 00:00 sonar_api_wrapper/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 sonar_api_wrapper/__version__.py
--rw-r--r--  2.0 unx     5274 b- defN 20-Feb-02 00:00 sonar_api_wrapper/client.py
-?rw-r--r--  2.0 unx     4720 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      599 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.0.dist-info/RECORD
-7 files, 11948 bytes uncompressed, 4997 bytes compressed:  58.2%
+-rw-r--r--  2.0 unx     5302 b- defN 20-Feb-02 00:00 sonar_api_wrapper/client.py
+?rw-r--r--  2.0 unx     4720 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      599 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.1.1.dist-info/RECORD
+7 files, 11976 bytes uncompressed, 5021 bytes compressed:  58.1%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: sonar_api_wrapper/__version__.py
 Comment: 
 
 Filename: sonar_api_wrapper/client.py
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.0.dist-info/METADATA
+Filename: sonar_api_wrapper-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.0.dist-info/WHEEL
+Filename: sonar_api_wrapper-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.0.dist-info/licenses/LICENSE
+Filename: sonar_api_wrapper-1.1.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: sonar_api_wrapper-1.1.0.dist-info/RECORD
+Filename: sonar_api_wrapper-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sonar_api_wrapper/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

## sonar_api_wrapper/client.py

```diff
@@ -18,14 +18,17 @@
     INFO = 'INFO'
     MINOR = 'MINOR'
     MAJOR = 'MAJOR'
     CRITICAL = 'CRITICAL'
     BLOCKER = 'BLOCKER'
 
 
+PAGINATION_MAX_SIZE = 500
+
+
 def set_from_env(env_name: str, default_value: str) -> str:
     if os.getenv(env_name) is not None:
         return os.getenv(env_name)
     else:
         return default_value
```

## Comparing `sonar_api_wrapper-1.1.0.dist-info/METADATA` & `sonar_api_wrapper-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sonar-api-wrapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: Sonar API Wrapper - a Sonarqube api wrapper
 Project-URL: Homepage, https://github.com/AlessandroStaffolani/sonar-api-wrapper
 Project-URL: Repository, https://github.com/AlessandroStaffolani/sonar-api-wrapper.git
 Author-email: Alessandro Staffolani <alestam93@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Alessandro Staffolani
```

## Comparing `sonar_api_wrapper-1.1.0.dist-info/licenses/LICENSE` & `sonar_api_wrapper-1.1.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

