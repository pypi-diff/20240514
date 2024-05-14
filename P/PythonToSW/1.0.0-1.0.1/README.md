# Comparing `tmp/PythonToSW-1.0.0.tar.gz` & `tmp/PythonToSW-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.0.0.tar", last modified: Tue May 14 16:57:55 2024, max compression
+gzip compressed data, was "PythonToSW-1.0.1.tar", last modified: Tue May 14 17:15:24 2024, max compression
```

## Comparing `PythonToSW-1.0.0.tar` & `PythonToSW-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 16:57:55.323897 PythonToSW-1.0.0/
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:57:55.323150 PythonToSW-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 16:57:55.294715 PythonToSW-1.0.0/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/__init__.py
--rw-rw-rw-   0        0        0    10523 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:57:55.321657 PythonToSW-1.0.0/PythonToSW/executions/
--rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.0/PythonToSW/executions/__toImport.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 16:56:13.000000 PythonToSW-1.0.0/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.0/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:57:55.322403 PythonToSW-1.0.0/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:57:55.000000 PythonToSW-1.0.0/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1321 2024-05-14 16:57:55.000000 PythonToSW-1.0.0/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 16:57:55.000000 PythonToSW-1.0.0/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 16:57:55.000000 PythonToSW-1.0.0/PythonToSW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 16:57:55.323897 PythonToSW-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1446 2024-05-14 16:57:52.000000 PythonToSW-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:15:24.190394 PythonToSW-1.0.1/
+-rw-rw-rw-   0        0        0     1564 2024-05-14 17:15:24.189648 PythonToSW-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 17:15:24.158193 PythonToSW-1.0.1/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/__init__.py
+-rw-rw-rw-   0        0        0    10523 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:15:24.188135 PythonToSW-1.0.1/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.1/PythonToSW/executions/__toImport.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1618 2024-05-14 16:56:13.000000 PythonToSW-1.0.1/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.1/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:15:24.188902 PythonToSW-1.0.1/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1564 2024-05-14 17:15:24.000000 PythonToSW-1.0.1/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1321 2024-05-14 17:15:24.000000 PythonToSW-1.0.1/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:15:24.000000 PythonToSW-1.0.1/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 17:15:24.000000 PythonToSW-1.0.1/PythonToSW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:15:24.190394 PythonToSW-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1637 2024-05-14 17:14:48.000000 PythonToSW-1.0.1/setup.py
```

### Comparing `PythonToSW-1.0.0/PKG-INFO` & `PythonToSW-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.0/PythonToSW/__init__.py` & `PythonToSW-1.0.1/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/addon.py` & `PythonToSW-1.0.1/PythonToSW/addon.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/event.py` & `PythonToSW-1.0.1/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/exceptions.py` & `PythonToSW-1.0.1/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/__init__.py` & `PythonToSW-1.0.1/PythonToSW/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/__toImport.py` & `PythonToSW-1.0.1/PythonToSW/executions/__toImport.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.0.1/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/addAuth.py` & `PythonToSW-1.0.1/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.0.1/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.0.1/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.0.1/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/announce.py` & `PythonToSW-1.0.1/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.0.1/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.0.1/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.0.1/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.0.1/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.0.1/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.0.1/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.0.1/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.0.1/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.0.1/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.0.1/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.0.1/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.0.1/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.0.1/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.0.1/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.0.1/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.0.1/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/removePopup.py` & `PythonToSW-1.0.1/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.0.1/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.0.1/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/executions/setPopup.py` & `PythonToSW-1.0.1/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/helpers.py` & `PythonToSW-1.0.1/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW/matrix.py` & `PythonToSW-1.0.1/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.0.1/PythonToSW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.0/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.0.1/PythonToSW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.0/setup.py` & `PythonToSW-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,21 +20,29 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
 from setuptools import setup, find_packages
 
+# ---- // Variables
+with open("../VERSION", encoding = "utf-8") as file:
+    version = file.read()
+    print(version)
+    
+with open("../README.md", encoding = "utf-8") as file:
+    long_description = file.read()
+
 # ---- // Main
 setup(
     name= "PythonToSW",
-    version = "1.0.0",
+    version = version,
     author = "Cuh4",
     description = "A package that allows you to create addons in Stormworks with Python, handled through HTTP.",
-    long_description = open("../README.md", encoding = "utf-8").read(),
+    long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = find_packages(),
     license = "Apache License 2.0",
     
     classifiers = [
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

