# Comparing `tmp/PythonToSW-1.0.6.tar.gz` & `tmp/PythonToSW-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.0.6.tar", last modified: Tue May 14 18:03:02 2024, max compression
+gzip compressed data, was "PythonToSW-1.0.7.tar", last modified: Tue May 14 18:07:36 2024, max compression
```

## Comparing `PythonToSW-1.0.6.tar` & `PythonToSW-1.0.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:03:02.260313 PythonToSW-1.0.6/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      118 2024-05-14 18:02:11.000000 PythonToSW-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1731 2024-05-14 18:03:02.259565 PythonToSW-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.6/README.md
--rw-rw-rw-   0        0        0        5 2024-05-14 18:02:32.000000 PythonToSW-1.0.6/VERSION
--rw-rw-rw-   0        0        0       42 2024-05-14 18:03:02.260313 PythonToSW-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1967 2024-05-14 18:02:21.000000 PythonToSW-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:03:02.228066 PythonToSW-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:03:02.235060 PythonToSW-1.0.6/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:03:02.241061 PythonToSW-1.0.6/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.0.6/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.0.6/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    10523 2024-05-14 17:19:07.000000 PythonToSW-1.0.6/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:03:02.258818 PythonToSW-1.0.6/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.6/src/PythonToSW/executions/__toImport.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.6/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.6/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.6/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:03:02.258818 PythonToSW-1.0.6/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1731 2024-05-14 18:03:02.000000 PythonToSW-1.0.6/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1614 2024-05-14 18:03:02.000000 PythonToSW-1.0.6/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:03:02.000000 PythonToSW-1.0.6/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-14 18:03:02.000000 PythonToSW-1.0.6/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 18:03:02.000000 PythonToSW-1.0.6/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.443158 PythonToSW-1.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       66 2024-05-14 18:04:45.000000 PythonToSW-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1731 2024-05-14 18:07:36.442412 PythonToSW-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.7/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-14 18:07:03.000000 PythonToSW-1.0.7/VERSION
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:07:36.443158 PythonToSW-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1967 2024-05-14 18:02:21.000000 PythonToSW-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.406413 PythonToSW-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.413160 PythonToSW-1.0.7/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.424918 PythonToSW-1.0.7/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.0.7/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.0.7/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    10866 2024-05-14 18:06:38.000000 PythonToSW-1.0.7/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.440919 PythonToSW-1.0.7/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.7/src/PythonToSW/executions/__toImport.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.7/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.7/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.7/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:07:36.441665 PythonToSW-1.0.7/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1614 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 18:07:36.000000 PythonToSW-1.0.7/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.0.6/LICENSE` & `PythonToSW-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/PKG-INFO` & `PythonToSW-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.6/README.md` & `PythonToSW-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/setup.py` & `PythonToSW-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/__init__.py` & `PythonToSW-1.0.7/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/addon/script.lua` & `PythonToSW-1.0.7/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/addon.py` & `PythonToSW-1.0.7/src/PythonToSW/addon.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from . import helpers
 from . import exceptions
 from . import executions
 from . import Event
 
 # ---- // Main
 class Addon():
-    def __init__(self, addonName: str, port: int):
+    def __init__(self, addonName: str, port: int, *, showStartupMessage: bool = True):
         self.addonName = addonName
         self.port = port
         self.app = flask.Flask(__name__)
         self.running = False
         self.addonPath = os.path.join(os.path.dirname(__file__), "addon")
         self.destinationAddonPath = os.path.join(os.getenv("APPDATA"), "Stormworks", "data", "missions")
         
@@ -51,14 +51,16 @@
         
         if not os.path.exists(self.destinationAddonPath):
             raise exceptions.InternalError(f"Addon destination path does not exist: {os.path.abspath(self.destinationAddonPath)}. Please install and run Stormworks: Build and Rescue.")
         
         self.pendingExecutions: dict[str, executions.BaseExecution] = {}
         self.callbacks: dict[str, Event] = {}
         
+        self.showStartupMessage = showStartupMessage
+        
     # Start the addon
     def start(self, codeFunc: "function"):
         if self.running:
             raise exceptions.FailedStartAttempt("Addon is already running")
         
         # set running
         self.running = True
@@ -68,14 +70,18 @@
         
         # setup routes
         self.__setupRoutes()
         
         # hide flask output
         self.__hideFlaskOutput()
         
+        # show message
+        if self.showStartupMessage:
+            print(f"[PythonToSW] {self.addonName} has started, listening on port {self.port}. Create a save with your addon enabled in Stormworks and keep this running.")
+        
         # start server
         threading.Thread(target = codeFunc).start()
         self.app.run(host = "127.0.0.1", port = self.port, threaded = True)
         
     # Execute a server function in the addon
     def execute(self, execution: executions.BaseExecution):
         # check if addon is running
```

### Comparing `PythonToSW-1.0.6/src/PythonToSW/event.py` & `PythonToSW-1.0.7/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/exceptions.py` & `PythonToSW-1.0.7/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/__toImport.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/__toImport.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/announce.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.0.7/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/helpers.py` & `PythonToSW-1.0.7/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW/matrix.py` & `PythonToSW-1.0.7/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.6/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.0.7/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.6/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.0.7/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files identical despite different names*
