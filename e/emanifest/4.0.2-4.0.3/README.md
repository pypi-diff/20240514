# Comparing `tmp/emanifest-4.0.2.tar.gz` & `tmp/emanifest-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emanifest-4.0.2.tar", last modified: Tue Mar 26 18:06:27 2024, max compression
+gzip compressed data, was "emanifest-4.0.3.tar", last modified: Tue May 14 19:29:59 2024, max compression
```

## Comparing `emanifest-4.0.2.tar` & `emanifest-4.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:06:27.988602 emanifest-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-26 18:06:02.000000 emanifest-4.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-26 18:06:02.000000 emanifest-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-03-26 18:06:27.988602 emanifest-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-03-26 18:06:02.000000 emanifest-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-26 18:06:02.000000 emanifest-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 18:06:27.988602 emanifest-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:06:27.984602 emanifest-4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:06:27.984602 emanifest-4.0.2/src/emanifest/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-26 18:06:02.000000 emanifest-4.0.2/src/emanifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39713 2024-03-26 18:06:02.000000 emanifest-4.0.2/src/emanifest/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:06:27.988602 emanifest-4.0.2/src/emanifest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-03-26 18:06:27.000000 emanifest-4.0.2/src/emanifest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-26 18:06:27.000000 emanifest-4.0.2/src/emanifest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 18:06:27.000000 emanifest-4.0.2/src/emanifest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-26 18:06:27.000000 emanifest-4.0.2/src/emanifest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 18:06:27.000000 emanifest-4.0.2/src/emanifest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:29:59.325941 emanifest-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-14 19:29:45.000000 emanifest-4.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 19:29:45.000000 emanifest-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-14 19:29:59.325941 emanifest-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-05-14 19:29:45.000000 emanifest-4.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-14 19:29:45.000000 emanifest-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:29:59.325941 emanifest-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:29:59.321941 emanifest-4.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:29:59.321941 emanifest-4.0.3/src/emanifest/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 19:29:45.000000 emanifest-4.0.3/src/emanifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40204 2024-05-14 19:29:45.000000 emanifest-4.0.3/src/emanifest/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:29:59.325941 emanifest-4.0.3/src/emanifest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-14 19:29:59.000000 emanifest-4.0.3/src/emanifest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 19:29:59.000000 emanifest-4.0.3/src/emanifest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:29:59.000000 emanifest-4.0.3/src/emanifest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-14 19:29:59.000000 emanifest-4.0.3/src/emanifest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 19:29:59.000000 emanifest-4.0.3/src/emanifest.egg-info/top_level.txt
```

### Comparing `emanifest-4.0.2/LICENSE.txt` & `emanifest-4.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emanifest-4.0.2/PKG-INFO` & `emanifest-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emanifest
-Version: 4.0.2
+Version: 4.0.3
 Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency
 Author-email: William Nicholas  <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>
 Maintainer-email: William Nicholas <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>, Scott Christian <christian.scott@epa.gov>
 License: CCO 1.0
 Project-URL: issues, https://github.com/USEPA/e-Manifest/issues
 Project-URL: documentation, https://github.com/USEPA/e-Manifest/emanifest-py
 Project-URL: homepage, https://github.com/USEPA/e-Manifest
```

### Comparing `emanifest-4.0.2/README.md` & `emanifest-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `emanifest-4.0.2/pyproject.toml` & `emanifest-4.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "emanifest"
-version = "4.0.2"
+version = "4.0.3"
 description = "An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency"
 readme = "README.md"
 authors = [
     { name = "William Nicholas ", email = "nicholas.william@epa.gov" },
     { name = "David Graham", email = "graham.david@epa.gov" },
 ]
 maintainers = [
```

### Comparing `emanifest-4.0.2/src/emanifest/client.py` & `emanifest-4.0.3/src/emanifest/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -937,15 +937,28 @@
             transporterOrder (int) : If the site is a transporter, the order of that transporter on the manifest
 
         Returns:
             dict: message of success or failure
         """
         endpoint = f"{self.base_url}v1/emanifest/manifest/quicker-sign"
         return self.__rcra_request("POST", endpoint, **kwargs)
+        
+    def get_available_manifests(self, mtn: str) -> RcrainfoResponse:
+        """
+        Returns previous and future signature-related information about manifest and respective sites
+
+        Args:
+            mtn (str): Manifest tracking number
 
+        Returns:
+            dict: object containing manifest signature details
+        """
+        endpoint = f"{self.base_url}v1/emanifest/manifest/available-to-sign/{mtn}"
+        return self.__rcra_request("GET", endpoint)
+        
     def save_manifest(
         self, manifest_json: dict, zip_file: bytes = None
     ) -> RcrainfoResponse:
         """
         Save Manifest by providing e-Manifest JSON and optional Zip attachment
 
         Args:
```

### Comparing `emanifest-4.0.2/src/emanifest.egg-info/PKG-INFO` & `emanifest-4.0.3/src/emanifest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emanifest
-Version: 4.0.2
+Version: 4.0.3
 Summary: An API utility wrapper for accessing the e-Manifest hazardous waste tracking system maintained by the US Environmental Protection Agency
 Author-email: William Nicholas  <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>
 Maintainer-email: William Nicholas <nicholas.william@epa.gov>, David Graham <graham.david@epa.gov>, Scott Christian <christian.scott@epa.gov>
 License: CCO 1.0
 Project-URL: issues, https://github.com/USEPA/e-Manifest/issues
 Project-URL: documentation, https://github.com/USEPA/e-Manifest/emanifest-py
 Project-URL: homepage, https://github.com/USEPA/e-Manifest
```

