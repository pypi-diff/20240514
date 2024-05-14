# Comparing `tmp/PythonToSW-1.0.4.tar.gz` & `tmp/PythonToSW-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.0.4.tar", last modified: Tue May 14 17:56:46 2024, max compression
+gzip compressed data, was "PythonToSW-1.0.5.tar", last modified: Tue May 14 18:00:31 2024, max compression
```

## Comparing `PythonToSW-1.0.4.tar` & `PythonToSW-1.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:56:46.397674 PythonToSW-1.0.4/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       88 2024-05-14 17:36:24.000000 PythonToSW-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1754 2024-05-14 17:56:46.396673 PythonToSW-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.4/README.md
--rw-rw-rw-   0        0        0        5 2024-05-14 17:56:44.000000 PythonToSW-1.0.4/VERSION
--rw-rw-rw-   0        0        0       42 2024-05-14 17:56:46.398183 PythonToSW-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2091 2024-05-14 17:56:41.000000 PythonToSW-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:56:46.360317 PythonToSW-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 17:56:46.367057 PythonToSW-1.0.4/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/__init__.py
--rw-rw-rw-   0        0        0    10523 2024-05-14 17:19:07.000000 PythonToSW-1.0.4/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:56:46.395926 PythonToSW-1.0.4/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.4/src/PythonToSW/executions/__toImport.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.4/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.4/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.4/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:56:46.396673 PythonToSW-1.0.4/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1754 2024-05-14 17:56:46.000000 PythonToSW-1.0.4/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2024-05-14 17:56:46.000000 PythonToSW-1.0.4/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:56:46.000000 PythonToSW-1.0.4/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-14 17:56:46.000000 PythonToSW-1.0.4/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 17:56:46.000000 PythonToSW-1.0.4/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 18:00:31.260275 PythonToSW-1.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       88 2024-05-14 17:36:24.000000 PythonToSW-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1731 2024-05-14 18:00:31.259447 PythonToSW-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.5/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-14 18:00:28.000000 PythonToSW-1.0.5/VERSION
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:00:31.260275 PythonToSW-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2072 2024-05-14 18:00:18.000000 PythonToSW-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:00:31.223458 PythonToSW-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:00:31.230404 PythonToSW-1.0.5/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/__init__.py
+-rw-rw-rw-   0        0        0    10523 2024-05-14 17:19:07.000000 PythonToSW-1.0.5/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:00:31.257870 PythonToSW-1.0.5/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.5/src/PythonToSW/executions/__toImport.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.5/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.5/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.5/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:00:31.258626 PythonToSW-1.0.5/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-05-14 18:00:31.000000 PythonToSW-1.0.5/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2024-05-14 18:00:31.000000 PythonToSW-1.0.5/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:00:31.000000 PythonToSW-1.0.5/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-14 18:00:31.000000 PythonToSW-1.0.5/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 18:00:31.000000 PythonToSW-1.0.5/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.0.4/LICENSE` & `PythonToSW-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/PKG-INFO` & `PythonToSW-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: uuid
-Requires-Dist: urllib
 Requires-Dist: xmltodict
 Requires-Dist: flask
 
 # ⚙️ | PythonToSW
 
 ## 📚 | Overview
 A Python package that allows you to create basic addons in Stormworks: Build and Rescue with Python.
```

### Comparing `PythonToSW-1.0.4/README.md` & `PythonToSW-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/setup.py` & `PythonToSW-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     ],
     
     install_requires = [
         "pyperclip",
         "requests",
         "urllib3",
         "uuid",
-        "urllib",
         "xmltodict",
         "flask"
     ],
 
     python_requires = ">=3.12",
     include_package_data = True,
     package_dir = {"": "src"}
```

### Comparing `PythonToSW-1.0.4/src/PythonToSW/__init__.py` & `PythonToSW-1.0.5/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/addon.py` & `PythonToSW-1.0.5/src/PythonToSW/addon.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/event.py` & `PythonToSW-1.0.5/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/exceptions.py` & `PythonToSW-1.0.5/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/__toImport.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/__toImport.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/announce.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.0.5/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/helpers.py` & `PythonToSW-1.0.5/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW/matrix.py` & `PythonToSW-1.0.5/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.4/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.0.5/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: uuid
-Requires-Dist: urllib
 Requires-Dist: xmltodict
 Requires-Dist: flask
 
 # ⚙️ | PythonToSW
 
 ## 📚 | Overview
 A Python package that allows you to create basic addons in Stormworks: Build and Rescue with Python.
```

### Comparing `PythonToSW-1.0.4/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.0.5/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

