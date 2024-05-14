# Comparing `tmp/PythonToSW-1.0.2.tar.gz` & `tmp/PythonToSW-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.0.2.tar", last modified: Tue May 14 17:38:27 2024, max compression
+gzip compressed data, was "PythonToSW-1.0.3.tar", last modified: Tue May 14 17:39:37 2024, max compression
```

## Comparing `PythonToSW-1.0.2.tar` & `PythonToSW-1.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:38:27.455996 PythonToSW-1.0.2/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       88 2024-05-14 17:36:24.000000 PythonToSW-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1754 2024-05-14 17:38:27.455237 PythonToSW-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.2/README.md
--rw-rw-rw-   0        0        0        5 2024-05-14 17:38:26.000000 PythonToSW-1.0.2/VERSION
--rw-rw-rw-   0        0        0       42 2024-05-14 17:38:27.456743 PythonToSW-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1887 2024-05-14 17:37:27.000000 PythonToSW-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:38:27.419829 PythonToSW-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 17:38:27.426818 PythonToSW-1.0.2/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/__init__.py
--rw-rw-rw-   0        0        0    10523 2024-05-14 17:19:07.000000 PythonToSW-1.0.2/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:38:27.454235 PythonToSW-1.0.2/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.2/src/PythonToSW/executions/__toImport.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.2/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.2/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.2/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:38:27.454235 PythonToSW-1.0.2/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1754 2024-05-14 17:38:27.000000 PythonToSW-1.0.2/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2024-05-14 17:38:27.000000 PythonToSW-1.0.2/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:38:27.000000 PythonToSW-1.0.2/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-14 17:38:27.000000 PythonToSW-1.0.2/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 17:38:27.000000 PythonToSW-1.0.2/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 17:39:37.404347 PythonToSW-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       88 2024-05-14 17:36:24.000000 PythonToSW-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1754 2024-05-14 17:39:37.403600 PythonToSW-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.0.3/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-14 17:39:34.000000 PythonToSW-1.0.3/VERSION
+-rw-rw-rw-   0        0        0       42 2024-05-14 17:39:37.404347 PythonToSW-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1980 2024-05-14 17:39:26.000000 PythonToSW-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:39:37.358005 PythonToSW-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 17:39:37.364992 PythonToSW-1.0.3/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/__init__.py
+-rw-rw-rw-   0        0        0    10523 2024-05-14 17:19:07.000000 PythonToSW-1.0.3/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:39:37.402107 PythonToSW-1.0.3/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     3265 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0      936 2024-05-14 16:48:31.000000 PythonToSW-1.0.3/src/PythonToSW/executions/__toImport.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1309 2024-05-14 16:56:13.000000 PythonToSW-1.0.3/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.0.3/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.0.3/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:39:37.402855 PythonToSW-1.0.3/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1754 2024-05-14 17:39:37.000000 PythonToSW-1.0.3/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2024-05-14 17:39:37.000000 PythonToSW-1.0.3/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:39:37.000000 PythonToSW-1.0.3/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-14 17:39:37.000000 PythonToSW-1.0.3/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 17:39:37.000000 PythonToSW-1.0.3/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.0.2/LICENSE` & `PythonToSW-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/PKG-INFO` & `PythonToSW-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.2/README.md` & `PythonToSW-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/setup.py` & `PythonToSW-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
+import os
 from setuptools import setup, find_packages
 
 # ---- // Variables
-with open("VERSION", encoding = "utf-8") as file:
+with open(os.path.join(os.path.dirname(__file__), "VERSION"), encoding = "utf-8") as file:
     version = file.read()
     print(version)
     
-with open("README.md", encoding = "utf-8") as file:
+with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding = "utf-8") as file:
     long_description = file.read()
 
 # ---- // Main
 setup(
     name= "PythonToSW",
     version = version,
     author = "Cuh4",
```

### Comparing `PythonToSW-1.0.2/src/PythonToSW/__init__.py` & `PythonToSW-1.0.3/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/addon.py` & `PythonToSW-1.0.3/src/PythonToSW/addon.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/event.py` & `PythonToSW-1.0.3/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/exceptions.py` & `PythonToSW-1.0.3/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/__toImport.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/__toImport.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/announce.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.0.3/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/helpers.py` & `PythonToSW-1.0.3/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW/matrix.py` & `PythonToSW-1.0.3/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.0.2/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.0.3/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.0.2/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.0.3/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

