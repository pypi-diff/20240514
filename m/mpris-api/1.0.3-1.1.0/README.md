# Comparing `tmp/mpris-api-1.0.3.tar.gz` & `tmp/mpris-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-28wwoi7m/mpris-api-1.0.3.tar", last modified: Sun May 12 15:48:24 2024, max compression
+gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-49rz3x46/mpris-api-1.1.0.tar", last modified: Tue May 14 14:15:40 2024, max compression
```

## Comparing `mpris-api-1.0.3.tar` & `mpris-api-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.0.3/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      102 2024-05-12 15:19:56.000000 mpris-api-1.0.3/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-12 15:48:24.000000 mpris-api-1.0.3/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.0.3/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5218 2024-05-12 11:28:20.000000 mpris-api-1.0.3/pkg/mpris_api/MprisService.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1836 2024-05-12 09:34:58.000000 mpris-api-1.0.3/pkg/mpris_api/MprisUpdateNotifier.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-12 15:44:42.000000 mpris-api-1.0.3/pkg/mpris_api/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api/adapter/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2151 2024-05-12 08:39:29.000000 mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.0.3/pkg/mpris_api/adapter/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api/common/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1485 2024-05-12 11:19:02.000000 mpris-api-1.0.3/pkg/mpris_api/common/DbusObject.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.0.3/pkg/mpris_api/common/DbusObjectSpec.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      483 2024-05-12 09:42:57.000000 mpris-api-1.0.3/pkg/mpris_api/common/DbusType.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.0.3/pkg/mpris_api/common/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      209 2024-05-12 09:55:02.000000 mpris-api-1.0.3/pkg/mpris_api/common/dbusDecorators.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api/interface/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1429 2024-05-12 09:12:24.000000 mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfaceBase.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2759 2024-05-12 10:04:49.000000 mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfacePlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7286 2024-05-12 11:21:27.000000 mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfacePlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3437 2024-05-12 09:58:10.000000 mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfaceRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3439 2024-05-12 11:21:27.000000 mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfaceTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.0.3/pkg/mpris_api/interface/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api/model/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.0.3/pkg/mpris_api/model/MprisConstant.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      201 2024-05-11 07:59:37.000000 mpris-api-1.0.3/pkg/mpris_api/model/MprisLoopStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2576 2024-05-12 11:11:07.000000 mpris-api-1.0.3/pkg/mpris_api/model/MprisMetaData.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      211 2024-05-11 07:59:57.000000 mpris-api-1.0.3/pkg/mpris_api/model/MprisPlaybackStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      656 2024-05-12 10:00:54.000000 mpris-api-1.0.3/pkg/mpris_api/model/MprisPlaylist.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      316 2024-05-11 12:27:27.000000 mpris-api-1.0.3/pkg/mpris_api/model/MprisPlaylistOrdering.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.0.3/pkg/mpris_api/model/MprisTrack.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.0.3/pkg/mpris_api/model/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.0.3/pkg/mpris_api/py.typed
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1352 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       41 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-12 15:48:24.000000 mpris-api-1.0.3/pkg/mpris_api.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      903 2024-05-12 15:43:25.000000 mpris-api-1.0.3/pyproject.toml
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:48:24.000000 mpris-api-1.0.3/requirements/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       51 2024-05-12 15:43:43.000000 mpris-api-1.0.3/requirements/release.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-12 15:48:24.000000 mpris-api-1.0.3/setup.cfg
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.1.0/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      102 2024-05-12 15:19:56.000000 mpris-api-1.1.0/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-14 14:15:40.000000 mpris-api-1.1.0/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.1.0/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5218 2024-05-12 11:28:20.000000 mpris-api-1.1.0/pkg/mpris_api/MprisService.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2040 2024-05-14 14:07:54.000000 mpris-api-1.1.0/pkg/mpris_api/MprisUpdateNotifier.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-14 14:09:56.000000 mpris-api-1.1.0/pkg/mpris_api/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api/adapter/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2151 2024-05-12 08:39:29.000000 mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.1.0/pkg/mpris_api/adapter/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api/common/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1485 2024-05-12 11:19:02.000000 mpris-api-1.1.0/pkg/mpris_api/common/DbusObject.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.1.0/pkg/mpris_api/common/DbusObjectSpec.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      483 2024-05-12 09:42:57.000000 mpris-api-1.1.0/pkg/mpris_api/common/DbusType.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.1.0/pkg/mpris_api/common/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      209 2024-05-12 09:55:02.000000 mpris-api-1.1.0/pkg/mpris_api/common/dbusDecorators.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      462 2024-05-14 14:05:19.000000 mpris-api-1.1.0/pkg/mpris_api/common/dbusEnums.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api/interface/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1686 2024-05-14 14:11:03.000000 mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfaceBase.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2909 2024-05-14 14:01:30.000000 mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfacePlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7493 2024-05-14 14:01:30.000000 mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfacePlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3572 2024-05-14 14:01:30.000000 mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfaceRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3601 2024-05-14 14:01:30.000000 mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfaceTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.1.0/pkg/mpris_api/interface/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api/model/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.1.0/pkg/mpris_api/model/MprisConstant.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      201 2024-05-11 07:59:37.000000 mpris-api-1.1.0/pkg/mpris_api/model/MprisLoopStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2632 2024-05-14 13:51:57.000000 mpris-api-1.1.0/pkg/mpris_api/model/MprisMetaData.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      211 2024-05-11 07:59:57.000000 mpris-api-1.1.0/pkg/mpris_api/model/MprisPlaybackStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      713 2024-05-14 13:51:36.000000 mpris-api-1.1.0/pkg/mpris_api/model/MprisPlaylist.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      316 2024-05-11 12:27:27.000000 mpris-api-1.1.0/pkg/mpris_api/model/MprisPlaylistOrdering.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.1.0/pkg/mpris_api/model/MprisTrack.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.1.0/pkg/mpris_api/model/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.1.0/pkg/mpris_api/py.typed
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1386 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       41 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-14 14:15:40.000000 mpris-api-1.1.0/pkg/mpris_api.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      903 2024-05-12 15:43:25.000000 mpris-api-1.1.0/pyproject.toml
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-14 14:15:40.000000 mpris-api-1.1.0/requirements/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       51 2024-05-12 15:43:43.000000 mpris-api-1.1.0/requirements/release.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-14 14:15:40.000000 mpris-api-1.1.0/setup.cfg
```

### Comparing `mpris-api-1.0.3/LICENSE.txt` & `mpris-api-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/PKG-INFO` & `mpris-api-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.0.3
+Version: 1.1.0
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.0.3/README.md` & `mpris-api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/MprisService.py` & `mpris-api-1.1.0/pkg/mpris_api/MprisService.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/MprisUpdateNotifier.py` & `mpris-api-1.1.0/pkg/mpris_api/MprisUpdateNotifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 from typing import Dict, List, Optional, Type
 
-from mpris_api.interface.MprisInterfaceBase import MprisInterfaceBase
-from mpris_api.interface.MprisInterfacePlayer import MprisInterfacePlayer
-from mpris_api.interface.MprisInterfacePlayLists import MprisInterfacePlayLists
-from mpris_api.interface.MprisInterfaceRoot import MprisInterfaceRoot
-from mpris_api.interface.MprisInterfaceTrackList import MprisInterfaceTrackList
+from mpris_api.interface.MprisInterfaceBase import MprisInterfaceBase, TDbusPropertyId
+from mpris_api.interface.MprisInterfacePlayLists import MprisInterfacePlayLists, MprisPlayListsPropertyId
+from mpris_api.interface.MprisInterfacePlayer import MprisInterfacePlayer, MprisPlayerPropertyId
+from mpris_api.interface.MprisInterfaceRoot import MprisInterfaceRoot, MprisRootPropertyId
+from mpris_api.interface.MprisInterfaceTrackList import MprisInterfaceTrackList, MprisTrackListPropertyId
 
 
 class _NullInterface(MprisInterfaceBase):
     pass
 
 
 _NULL_INTERFACE = _NullInterface(name='')
@@ -26,25 +26,25 @@
             for interface in interfaces
         }
 
     def notifyAll(self) -> None:
         for interface in self._interfaces.values():
             interface.emitAll()
 
-    def notifyRoot(self, fields: Optional[List[str]] = None) -> None:
+    def notifyRoot(self, fields: Optional[List[MprisRootPropertyId]] = None) -> None:
         self._notifyInterface(interfaceType=MprisInterfaceRoot, fields=fields)
 
-    def notifyPlayer(self, fields: Optional[List[str]] = None) -> None:
+    def notifyPlayer(self, fields: Optional[List[MprisPlayerPropertyId]] = None) -> None:
         self._notifyInterface(interfaceType=MprisInterfacePlayer, fields=fields)
 
-    def notifyTracklist(self, fields: Optional[List[str]] = None) -> None:
+    def notifyTracklist(self, fields: Optional[List[MprisTrackListPropertyId]] = None) -> None:
         self._notifyInterface(interfaceType=MprisInterfaceTrackList, fields=fields)
 
-    def notifyPlaylists(self, fields: Optional[List[str]] = None) -> None:
+    def notifyPlaylists(self, fields: Optional[List[MprisPlayListsPropertyId]] = None) -> None:
         self._notifyInterface(interfaceType=MprisInterfacePlayLists, fields=fields)
 
     def _notifyInterface(
         self,
         interfaceType: Type[MprisInterfaceBase],
-        fields: Optional[List[str]]
+        fields: Optional[List[TDbusPropertyId]]
     ) -> None:
-        self._interfaces.get(interfaceType, _NULL_INTERFACE).emitFields(names=fields)
+        self._interfaces.get(interfaceType, _NULL_INTERFACE).emitFields(fieldIds=fields)
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py` & `mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterPlayer.py` & `mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterPlayer.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterRoot.py` & `mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterRoot.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/adapter/IMprisAdapterTrackList.py` & `mpris-api-1.1.0/pkg/mpris_api/adapter/IMprisAdapterTrackList.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/common/DbusObject.py` & `mpris-api-1.1.0/pkg/mpris_api/common/DbusObject.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/common/DbusObjectSpec.py` & `mpris-api-1.1.0/pkg/mpris_api/common/DbusObjectSpec.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfaceBase.py` & `mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfaceBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 # Copyright by: P.J. Grochowski
 
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Type, TypeVar, cast
 
 from dbus_next.service import (ServiceInterface as DbusServiceInterface)
 
+from mpris_api.common.dbusEnums import DbusPropertyId
+
 T = TypeVar('T')
+TDbusPropertyId = TypeVar('TDbusPropertyId', bound=DbusPropertyId)
 
 
 class IDbusProperty(ABC):
     @property
     @abstractmethod
     def name(self) -> str: ...
     @abstractmethod
@@ -19,29 +22,30 @@
 
 
 class MprisInterfaceBase(DbusServiceInterface):
 
     def emitAll(self) -> None:
         self.emitFields()
 
-    def emitFields(self, names: Optional[List[str]] = None) -> None:
-        self._emitFields(fieldDict=self._getProperties(names=names))
+    def emitFields(self, fieldIds: Optional[List[TDbusPropertyId]] = None) -> None:
+        self._emitFields(fieldDict=self._getProperties(fieldIds=fieldIds))
 
     def _emitFields(self, fieldDict: Dict[str, Any]) -> None:
         self.emit_properties_changed(
             changed_properties=fieldDict,
             invalidated_properties=[]
         )
 
-    def _getProperties(self, names: Optional[List[str]]) -> Dict[str, Any]:
+    def _getProperties(self, fieldIds: Optional[List[TDbusPropertyId]]) -> Dict[str, Any]:
+        fieldNames = [str(fieldId) for fieldId in fieldIds] if fieldIds is not None else None
         properties = cast(List[IDbusProperty], DbusServiceInterface._get_properties(self))
         return {
             prop.name: prop.__get__(self, self.__class__)
             for prop in properties
-            if self._shouldGetProperty(prop=prop, names=names)
+            if self._shouldGetProperty(prop=prop, names=fieldNames)
         }
 
     @staticmethod
     def _shouldGetProperty(prop: IDbusProperty, names: Optional[List[str]]) -> bool:
         return (
             names is None
             or prop.name in names
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfacePlayLists.py` & `mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfacePlayLists.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,68 +5,69 @@
 from typing import no_type_check
 
 from dbus_next import PropertyAccess
 
 from mpris_api.adapter.IMprisAdapterPlayLists import IMprisAdapterPlayLists
 from mpris_api.common.DbusType import DbusType
 from mpris_api.common.dbusDecorators import dbusMethod, dbusProperty, dbusSignal
+from mpris_api.common.dbusEnums import DbusMethodId, DbusPropertyId, DbusSignalId
 from mpris_api.interface.MprisInterfaceBase import MprisInterfaceBase
 from mpris_api.model.MprisConstant import MprisConstant
 from mpris_api.model.MprisPlaylistOrdering import MprisPlaylistOrdering
 
 
-class MprisPlayListsSignal:
-    PLAYLIST_CHANGED: str = 'PlaylistChanged'
+class MprisPlayListsSignalId(DbusSignalId):
+    PLAYLIST_CHANGED = 'PlaylistChanged'
 
 
-class MprisPlayListsProperty:
-    PLAYLIST_COUNT: str = 'PlaylistCount'
-    ORDERINGS: str = 'Orderings'
-    ACTIVE_PLAYLIST: str = 'ActivePlaylist'
+class MprisPlayListsPropertyId(DbusPropertyId):
+    PLAYLIST_COUNT = 'PlaylistCount'
+    ORDERINGS = 'Orderings'
+    ACTIVE_PLAYLIST = 'ActivePlaylist'
 
 
-class MprisPlayListsMethod:
-    ACTIVATE_PLAYLIST: str = 'ActivatePlaylist'
-    GET_PLAYLISTS: str = 'GetPlaylists'
+class MprisPlayListsMethodId(DbusMethodId):
+    ACTIVATE_PLAYLIST = 'ActivatePlaylist'
+    GET_PLAYLISTS = 'GetPlaylists'
 
 
 class MprisInterfacePlayLists(MprisInterfaceBase):
 
     def __init__(self, adapter: IMprisAdapterPlayLists) -> None:
         super().__init__(f'{MprisConstant.NAME}.Playlists')
         self._adapter: IMprisAdapterPlayLists = adapter
 
-    @dbusSignal(name=MprisPlayListsSignal.PLAYLIST_CHANGED)
+    @dbusSignal(name=MprisPlayListsSignalId.PLAYLIST_CHANGED.value)
     @no_type_check
     def playlistChanged(self, playlist: DbusType.TUPLE_OSS) -> None:
         pass
 
-    @dbusProperty(name=MprisPlayListsProperty.PLAYLIST_COUNT, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayListsPropertyId.PLAYLIST_COUNT.value, access=PropertyAccess.READ)
     @no_type_check
     def playlistCount(self) -> DbusType.UINT32:
         return self._adapter.getPlaylistCount()
 
-    @dbusProperty(name=MprisPlayListsProperty.ORDERINGS, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayListsPropertyId.ORDERINGS.value, access=PropertyAccess.READ)
     @no_type_check
     def orderings(self) -> DbusType.STRING_ARRAY:
         return [ordering.value for ordering in self._adapter.getAvailableOrderings()]
 
-    @dbusProperty(name=MprisPlayListsProperty.ACTIVE_PLAYLIST, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayListsPropertyId.ACTIVE_PLAYLIST.value, access=PropertyAccess.READ)
     @no_type_check
     def activePlaylist(self) -> DbusType.MAYBE_TUPLE_OSS:
         activePlaylist = self._adapter.getActivePlaylist()
         return (False, None) if activePlaylist is None\
             else (True, activePlaylist.toTuple())
 
-    @dbusMethod(name=MprisPlayListsMethod.ACTIVATE_PLAYLIST)
+    @dbusMethod(name=MprisPlayListsMethodId.ACTIVATE_PLAYLIST.value)
     @no_type_check
     def activatePlaylist(self, playlistId: DbusType.OBJECT) -> None:
         self._adapter.activatePlaylist(playlistId=playlistId)
 
-    @dbusMethod(name=MprisPlayListsMethod.GET_PLAYLISTS)
+    @dbusMethod(name=MprisPlayListsMethodId.GET_PLAYLISTS.value)
     @no_type_check
     def getPlaylists(
         self,
         index: DbusType.UINT32,
         maxCount: DbusType.UINT32,
         order: DbusType.STRING,
         reverseOrder: DbusType.BOOL
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfacePlayer.py` & `mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfacePlayer.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,212 +7,213 @@
 from dbus_next import PropertyAccess
 from tunit.unit import Microseconds
 
 from mpris_api.adapter.IMprisAdapterPlayer import IMprisAdapterPlayer
 from mpris_api.common.DbusObjectSpec import DbusObjectSpec
 from mpris_api.common.DbusType import DbusType
 from mpris_api.common.dbusDecorators import dbusMethod, dbusProperty, dbusSignal
+from mpris_api.common.dbusEnums import DbusMethodId, DbusPropertyId, DbusSignalId
 from mpris_api.interface.MprisInterfaceBase import MprisInterfaceBase
 from mpris_api.model.MprisConstant import MprisConstant
 from mpris_api.model.MprisLoopStatus import MprisLoopStatus
 from mpris_api.model.MprisMetaData import MprisMetaDataField
 from mpris_api.model.MprisPlaybackStatus import MprisPlaybackStatus
 
 
 class MprisInvalidTrackException(Exception):
     pass
 
 
-class MprisPlayerSignal:
-    SEEKED: str = 'Seeked'
+class MprisPlayerSignalId(DbusSignalId):
+    SEEKED = 'Seeked'
 
 
-class MprisPlayerProperty:
-    CAN_CONTROL: str = 'CanControl'
-    CAN_PLAY: str = 'CanPlay'
-    CAN_PAUSE: str = 'CanPause'
-    CAN_GO_NEXT: str = 'CanGoNext'
-    CAN_GO_PREVIOUS: str = 'CanGoPrevious'
-    CAN_SEEK: str = 'CanSeek'
-    MINIMUM_RATE: str = 'MinimumRate'
-    MAXIMUM_RATE: str = 'MaximumRate'
-    RATE: str = 'Rate'
-    VOLUME: str = 'Volume'
-    METADATA: str = 'Metadata'
-    PLAYBACK_STATUS: str = 'PlaybackStatus'
-    POSITION: str = 'Position'
-    LOOP_STATUS: str = 'LoopStatus'
-    SHUFFLE: str = 'Shuffle'
-
-
-class MprisPlayerMethod:
-    STOP: str = 'Stop'
-    PLAY: str = 'Play'
-    PAUSE: str = 'Pause'
-    PLAY_PAUSE: str = 'PlayPause'
-    NEXT: str = 'Next'
-    PREVIOUS: str = 'Previous'
-    SEEK: str = 'Seek'
-    SET_POSITION: str = 'SetPosition'
-    OPEN_URI: str = 'OpenUri'
+class MprisPlayerPropertyId(DbusPropertyId):
+    CAN_CONTROL = 'CanControl'
+    CAN_PLAY = 'CanPlay'
+    CAN_PAUSE = 'CanPause'
+    CAN_GO_NEXT = 'CanGoNext'
+    CAN_GO_PREVIOUS = 'CanGoPrevious'
+    CAN_SEEK = 'CanSeek'
+    MINIMUM_RATE = 'MinimumRate'
+    MAXIMUM_RATE = 'MaximumRate'
+    RATE = 'Rate'
+    VOLUME = 'Volume'
+    METADATA = 'Metadata'
+    PLAYBACK_STATUS = 'PlaybackStatus'
+    POSITION = 'Position'
+    LOOP_STATUS = 'LoopStatus'
+    SHUFFLE = 'Shuffle'
+
+
+class MprisPlayerMethodId(DbusMethodId):
+    STOP = 'Stop'
+    PLAY = 'Play'
+    PAUSE = 'Pause'
+    PLAY_PAUSE = 'PlayPause'
+    NEXT = 'Next'
+    PREVIOUS = 'Previous'
+    SEEK = 'Seek'
+    SET_POSITION = 'SetPosition'
+    OPEN_URI = 'OpenUri'
 
 
 class MprisInterfacePlayer(MprisInterfaceBase):
 
     def __init__(self, adapter: IMprisAdapterPlayer) -> None:
         super().__init__(f'{MprisConstant.NAME}.Player')
         self._adapter: IMprisAdapterPlayer = adapter
 
-    @dbusSignal(name=MprisPlayerSignal.SEEKED)
+    @dbusSignal(name=MprisPlayerSignalId.SEEKED.value)
     @no_type_check
     def seeked(self, position: DbusType.INT64) -> None:
         return
 
-    @dbusProperty(name=MprisPlayerProperty.CAN_CONTROL, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.CAN_CONTROL.value, access=PropertyAccess.READ)
     @no_type_check
     def canControl(self) -> DbusType.BOOL:
         return self._adapter.canControl()
 
-    @dbusProperty(name=MprisPlayerProperty.CAN_PLAY, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.CAN_PLAY.value, access=PropertyAccess.READ)
     @no_type_check
     def canPlay(self) -> DbusType.BOOL:
         return self._adapter.canPlay()
 
-    @dbusProperty(name=MprisPlayerProperty.CAN_PAUSE, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.CAN_PAUSE.value, access=PropertyAccess.READ)
     @no_type_check
     def canPause(self) -> DbusType.BOOL:
         return self._adapter.canPause()
 
-    @dbusProperty(name=MprisPlayerProperty.CAN_GO_NEXT, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.CAN_GO_NEXT.value, access=PropertyAccess.READ)
     @no_type_check
     def canGoNext(self) -> DbusType.BOOL:
         return self._adapter.canGoNext()
 
-    @dbusProperty(name=MprisPlayerProperty.CAN_GO_PREVIOUS, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.CAN_GO_PREVIOUS.value, access=PropertyAccess.READ)
     @no_type_check
     def canGoPrevious(self) -> DbusType.BOOL:
         return self._adapter.canGoPrevious()
 
-    @dbusProperty(name=MprisPlayerProperty.CAN_SEEK, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.CAN_SEEK.value, access=PropertyAccess.READ)
     @no_type_check
     def canSeek(self) -> DbusType.BOOL:
         return self._adapter.canSeek()
 
-    @dbusProperty(name=MprisPlayerProperty.MINIMUM_RATE, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.MINIMUM_RATE.value, access=PropertyAccess.READ)
     @no_type_check
     def minimumRate(self) -> DbusType.DOUBLE:
         return self._adapter.getMinimumRate()
 
-    @dbusProperty(name=MprisPlayerProperty.MAXIMUM_RATE, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.MAXIMUM_RATE.value, access=PropertyAccess.READ)
     @no_type_check
     def maximumRate(self) -> DbusType.DOUBLE:
         return self._adapter.getMaximumRate()
 
-    @dbusProperty(name=MprisPlayerProperty.RATE)
+    @dbusProperty(name=MprisPlayerPropertyId.RATE.value)
     @no_type_check
     def rate(self) -> DbusType.DOUBLE:
         return self._adapter.getRate()
 
     @rate.setter  # type: ignore
     @no_type_check
     def rate(self, value: DbusType.DOUBLE) -> None:
         self._adapter.setRate(value=value)
 
-    @dbusProperty(name=MprisPlayerProperty.VOLUME)
+    @dbusProperty(name=MprisPlayerPropertyId.VOLUME.value)
     @no_type_check
     def volume(self) -> DbusType.DOUBLE:
         return self._adapter.getVolume()
 
     @volume.setter  # type: ignore
     @no_type_check
     def volume(self, value: DbusType.DOUBLE) -> None:
         self._adapter.setVolume(value=value)
 
-    @dbusProperty(name=MprisPlayerProperty.METADATA, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.METADATA.value, access=PropertyAccess.READ)
     @no_type_check
     def metadata(self) -> DbusType.VARIANT_DICT:
         metaData = self._adapter.getMetadata().toVariantDict()
         if metaData[MprisMetaDataField.TRACK_ID] == MprisConstant.NO_TRACK_PATH:
             raise MprisInvalidTrackException(f'Interface cannot return metadata with reserved track ID! trackId="{MprisConstant.NO_TRACK_PATH}"')
 
         return metaData
 
-    @dbusProperty(name=MprisPlayerProperty.PLAYBACK_STATUS, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.PLAYBACK_STATUS.value, access=PropertyAccess.READ)
     @no_type_check
     def playbackStatus(self) -> DbusType.STRING:
         return self._adapter.getPlaybackStatus().value
 
-    @dbusProperty(name=MprisPlayerProperty.POSITION, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisPlayerPropertyId.POSITION.value, access=PropertyAccess.READ)
     @no_type_check
     def position(self) -> DbusType.INT64:
         return int(self._adapter.getPosition())
 
-    @dbusProperty(name=MprisPlayerProperty.LOOP_STATUS)
+    @dbusProperty(name=MprisPlayerPropertyId.LOOP_STATUS.value)
     @no_type_check
     def loopStatus(self) -> DbusType.STRING:
         return self._adapter.getLoopStatus().value
 
     @loopStatus.setter  # type: ignore
     @no_type_check
     def loopStatus(self, value: DbusType.STRING) -> None:
         self._adapter.setLoopStatus(value=MprisLoopStatus(value=value))
 
-    @dbusProperty(name=MprisPlayerProperty.SHUFFLE)
+    @dbusProperty(name=MprisPlayerPropertyId.SHUFFLE.value)
     @no_type_check
     def shuffle(self) -> DbusType.BOOL:
         return self._adapter.isShuffle()
 
     @shuffle.setter  # type: ignore
     @no_type_check
     def shuffle(self, value: DbusType.BOOL) -> None:
         self._adapter.setShuffle(value=value)
 
-    @dbusMethod(name=MprisPlayerMethod.STOP)
+    @dbusMethod(name=MprisPlayerMethodId.STOP.value)
     @no_type_check
     def stop(self) -> None:
         self._adapter.stop()
 
-    @dbusMethod(name=MprisPlayerMethod.PLAY)
+    @dbusMethod(name=MprisPlayerMethodId.PLAY.value)
     @no_type_check
     def play(self) -> None:
         self._adapter.play()
 
-    @dbusMethod(name=MprisPlayerMethod.PAUSE)
+    @dbusMethod(name=MprisPlayerMethodId.PAUSE.value)
     @no_type_check
     def pause(self) -> None:
         self._adapter.pause()
 
-    @dbusMethod(name=MprisPlayerMethod.PLAY_PAUSE)
+    @dbusMethod(name=MprisPlayerMethodId.PLAY_PAUSE.value)
     @no_type_check
     def playPause(self) -> None:
         playbackStatus = self._adapter.getPlaybackStatus()
         if playbackStatus == MprisPlaybackStatus.PLAYING:
             self._adapter.pause()
         else:
             self._adapter.play()
 
-    @dbusMethod(name=MprisPlayerMethod.NEXT)
+    @dbusMethod(name=MprisPlayerMethodId.NEXT.value)
     @no_type_check
     def next(self) -> None:
         self._adapter.next()
 
-    @dbusMethod(name=MprisPlayerMethod.PREVIOUS)
+    @dbusMethod(name=MprisPlayerMethodId.PREVIOUS.value)
     @no_type_check
     def previous(self) -> None:
         self._adapter.previous()
 
-    @dbusMethod(name=MprisPlayerMethod.SEEK)
+    @dbusMethod(name=MprisPlayerMethodId.SEEK.value)
     @no_type_check
     def seek(self, offset: DbusType.INT64) -> None:
         position = self._adapter.getPosition() + offset
         self._adapter.seek(position=position)
 
-    @dbusMethod(name=MprisPlayerMethod.SET_POSITION)
+    @dbusMethod(name=MprisPlayerMethodId.SET_POSITION.value)
     @no_type_check
     def setPosition(self, trackId: DbusType.OBJECT, position: DbusType.INT64) -> None:
         DbusObjectSpec.assertValid(dbusObj=trackId)
         self._adapter.seek(position=Microseconds(position), trackId=trackId)
 
-    @dbusMethod(name=MprisPlayerMethod.OPEN_URI)
+    @dbusMethod(name=MprisPlayerMethodId.OPEN_URI.value)
     @no_type_check
     def openUri(self, uri: DbusType.STRING) -> None:
         self._adapter.openUri(uri=uri)
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfaceRoot.py` & `mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfaceRoot.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,95 +6,96 @@
 from typing import no_type_check
 
 from dbus_next import PropertyAccess
 
 from mpris_api.adapter.IMprisAdapterRoot import IMprisAdapterRoot
 from mpris_api.common.DbusType import DbusType
 from mpris_api.common.dbusDecorators import dbusMethod, dbusProperty
+from mpris_api.common.dbusEnums import DbusMethodId, DbusPropertyId
 from mpris_api.interface.MprisInterfaceBase import MprisInterfaceBase
 from mpris_api.model.MprisConstant import MprisConstant
 
 
-class MprisRootProperty:
-    CAN_QUIT: str = 'CanQuit'
-    CAN_RAISE: str = 'CanRaise'
-    CAN_SET_FULL_SCREEN: str = 'CanSetFullscreen'
-    HAS_TRACK_LIST: str = 'HasTrackList'
-    FULL_SCREEN: str = 'Fullscreen'
-    IDENTITY: str = 'Identity'
-    DESKTOP_ENTRY: str = 'DesktopEntry'
-    SUPPORTED_URI_SCHEMES: str = 'SupportedUriSchemes'
-    SUPPORTED_MIME_TYPES: str = 'SupportedMimeTypes'
+class MprisRootPropertyId(DbusPropertyId):
+    CAN_QUIT = 'CanQuit'
+    CAN_RAISE = 'CanRaise'
+    CAN_SET_FULL_SCREEN = 'CanSetFullscreen'
+    HAS_TRACK_LIST = 'HasTrackList'
+    FULL_SCREEN = 'Fullscreen'
+    IDENTITY = 'Identity'
+    DESKTOP_ENTRY = 'DesktopEntry'
+    SUPPORTED_URI_SCHEMES = 'SupportedUriSchemes'
+    SUPPORTED_MIME_TYPES = 'SupportedMimeTypes'
 
 
-class MprisRootMethod:
-    QUIT: str = 'Quit'
-    RAISE: str = 'Raise'
+class MprisRootMethodId(DbusMethodId):
+    QUIT = 'Quit'
+    RAISE = 'Raise'
 
 
 class MprisInterfaceRoot(MprisInterfaceBase):
 
     def __init__(self, adapter: IMprisAdapterRoot) -> None:
         super().__init__(MprisConstant.NAME)
         self._adapter: IMprisAdapterRoot = adapter
 
-    @dbusProperty(name=MprisRootProperty.CAN_QUIT, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.CAN_QUIT.value, access=PropertyAccess.READ)
     @no_type_check
     def canQuit(self) -> DbusType.BOOL:
         return self._adapter.canQuit()
 
-    @dbusProperty(name=MprisRootProperty.CAN_RAISE, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.CAN_RAISE.value, access=PropertyAccess.READ)
     @no_type_check
     def canRaise(self) -> DbusType.BOOL:
         return self._adapter.canRaise()
 
-    @dbusProperty(name=MprisRootProperty.CAN_SET_FULL_SCREEN, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.CAN_SET_FULL_SCREEN.value, access=PropertyAccess.READ)
     @no_type_check
     def canSetFullscreen(self) -> DbusType.BOOL:
         return self._adapter.canSetFullscreen()
 
-    @dbusProperty(name=MprisRootProperty.IDENTITY, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.IDENTITY.value, access=PropertyAccess.READ)
     @no_type_check
     def identity(self) -> DbusType.STRING:
         return self._adapter.getIdentity()
 
-    @dbusProperty(name=MprisRootProperty.DESKTOP_ENTRY, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.DESKTOP_ENTRY.value, access=PropertyAccess.READ)
     @no_type_check
     def desktopEntry(self) -> DbusType.STRING:
         desktopEntry = self._adapter.getDesktopEntry()
         return '' if desktopEntry is None\
             else str(Path(desktopEntry).with_suffix(''))
 
-    @dbusProperty(name=MprisRootProperty.SUPPORTED_URI_SCHEMES, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.SUPPORTED_URI_SCHEMES.value, access=PropertyAccess.READ)
     @no_type_check
     def supportedUriSchemes(self) -> DbusType.STRING_ARRAY:
         return self._adapter.getSupportedUriSchemes()
 
-    @dbusProperty(name=MprisRootProperty.SUPPORTED_MIME_TYPES, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.SUPPORTED_MIME_TYPES.value, access=PropertyAccess.READ)
     @no_type_check
     def supportedMimeTypes(self) -> DbusType.STRING_ARRAY:
         return self._adapter.getSupportedMimeTypes()
 
-    @dbusProperty(name=MprisRootProperty.HAS_TRACK_LIST, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisRootPropertyId.HAS_TRACK_LIST.value, access=PropertyAccess.READ)
     @no_type_check
     def hasTracklist(self) -> DbusType.BOOL:
         return self._adapter.hasTracklist()
 
-    @dbusProperty(name=MprisRootProperty.FULL_SCREEN)
+    @dbusProperty(name=MprisRootPropertyId.FULL_SCREEN.value)
     @no_type_check
     def fullScreen(self) -> DbusType.BOOL:
         return self._adapter.isFullScreen()
 
     @fullScreen.setter  # type: ignore
     @no_type_check
     def fullScreen(self, value: DbusType.BOOL) -> None:
         self._adapter.setFullScreen(value=value)
 
-    @dbusMethod(name=MprisRootMethod.QUIT)
+    @dbusMethod(name=MprisRootMethodId.QUIT.value)
     @no_type_check
     def quitApp(self) -> None:
         self._adapter.quitApp()
 
-    @dbusMethod(name=MprisRootMethod.RAISE)
+    @dbusMethod(name=MprisRootMethodId.RAISE.value)
     @no_type_check
     def raiseApp(self) -> None:
         self._adapter.raiseApp()
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api/interface/MprisInterfaceTrackList.py` & `mpris-api-1.1.0/pkg/mpris_api/interface/MprisInterfaceTrackList.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,91 +5,92 @@
 from typing import no_type_check
 
 from dbus_next import PropertyAccess
 
 from mpris_api.adapter.IMprisAdapterTrackList import IMprisAdapterTrackList
 from mpris_api.common.DbusType import DbusType
 from mpris_api.common.dbusDecorators import dbusMethod, dbusProperty, dbusSignal
+from mpris_api.common.dbusEnums import DbusMethodId, DbusPropertyId, DbusSignalId
 from mpris_api.interface.MprisInterfaceBase import MprisInterfaceBase
 from mpris_api.model.MprisConstant import MprisConstant
 
 
-class MprisTrackListSignal:
-    TRACK_LIST_REPLACED: str = 'TrackListReplaced'
-    TRACK_ADDED: str = 'TrackAdded'
-    TRACK_REMOVED: str = 'TrackRemoved'
-    TRACK_METADATA_CHANGED: str = 'TrackMetadataChanged'
-
-
-class MprisTrackListProperty:
-    TRACKS: str = 'Tracks'
-    CAN_EDIT_TRACKS: str = 'CanEditTracks'
-
-
-class MprisTrackListMethod:
-    GET_TRACKS_METADATA: str = 'GetTracksMetadata'
-    ADD_TRACK: str = 'AddTrack'
-    REMOVE_TRACK: str = 'RemoveTrack'
-    GO_TO: str = 'GoTo'
+class MprisTrackListSignalId(DbusSignalId):
+    TRACK_LIST_REPLACED = 'TrackListReplaced'
+    TRACK_ADDED = 'TrackAdded'
+    TRACK_REMOVED = 'TrackRemoved'
+    TRACK_METADATA_CHANGED = 'TrackMetadataChanged'
+
+
+class MprisTrackListPropertyId(DbusPropertyId):
+    TRACKS = 'Tracks'
+    CAN_EDIT_TRACKS = 'CanEditTracks'
+
+
+class MprisTrackListMethodId(DbusMethodId):
+    GET_TRACKS_METADATA = 'GetTracksMetadata'
+    ADD_TRACK = 'AddTrack'
+    REMOVE_TRACK = 'RemoveTrack'
+    GO_TO = 'GoTo'
 
 
 class MprisInterfaceTrackList(MprisInterfaceBase):
 
     def __init__(self, adapter: IMprisAdapterTrackList) -> None:
         super().__init__(f'{MprisConstant.NAME}.TrackList')
         self._adapter: IMprisAdapterTrackList = adapter
 
-    @dbusSignal(name=MprisTrackListSignal.TRACK_LIST_REPLACED)
+    @dbusSignal(name=MprisTrackListSignalId.TRACK_LIST_REPLACED.value)
     @no_type_check
     def trackListReplaced(self, tracks: DbusType.OBJECT_ARRAY, currentTrack: DbusType.OBJECT) -> None:
         pass
 
-    @dbusSignal(name=MprisTrackListSignal.TRACK_ADDED)
+    @dbusSignal(name=MprisTrackListSignalId.TRACK_ADDED.value)
     @no_type_check
     def trackAdded(self, metaData: DbusType.VARIANT_DICT, afterTrack: DbusType.OBJECT) -> None:
         pass
 
-    @dbusSignal(name=MprisTrackListSignal.TRACK_REMOVED)
+    @dbusSignal(name=MprisTrackListSignalId.TRACK_REMOVED.value)
     @no_type_check
     def trackRemoved(self, trackId: DbusType.OBJECT) -> None:
         pass
 
-    @dbusSignal(name=MprisTrackListSignal.TRACK_METADATA_CHANGED)
+    @dbusSignal(name=MprisTrackListSignalId.TRACK_METADATA_CHANGED.value)
     @no_type_check
     def trackMetadataChanged(self, trackId: DbusType.OBJECT, metaData: DbusType.VARIANT_DICT) -> None:
         pass
 
-    @dbusProperty(name=MprisTrackListProperty.CAN_EDIT_TRACKS, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisTrackListPropertyId.CAN_EDIT_TRACKS.value, access=PropertyAccess.READ)
     @no_type_check
     def canEditTracks(self) -> DbusType.BOOL:
         return self._adapter.canEditTracks()
 
-    @dbusProperty(name=MprisTrackListProperty.TRACKS, access=PropertyAccess.READ)
+    @dbusProperty(name=MprisTrackListPropertyId.TRACKS.value, access=PropertyAccess.READ)
     @no_type_check
     def tracks(self) -> DbusType.OBJECT_ARRAY:
         return [str(track) for track in self._adapter.getTracks()]
 
-    @dbusMethod(name=MprisTrackListMethod.GET_TRACKS_METADATA)
+    @dbusMethod(name=MprisTrackListMethodId.GET_TRACKS_METADATA.value)
     @no_type_check
     def getTracksMetadata(self, trackIds: DbusType.OBJECT_ARRAY) -> DbusType.VARIANT_DICT_ARRAY:
         metaDataList = self._adapter.getTracksMetadata(trackIds=trackIds)
         return [metaData.toVariantDict() for metaData in metaDataList]
 
-    @dbusMethod(name=MprisTrackListMethod.ADD_TRACK)
+    @dbusMethod(name=MprisTrackListMethodId.ADD_TRACK.value)
     @no_type_check
     def addTrack(self, uri: DbusType.STRING, afterTrack: DbusType.OBJECT, goTo: DbusType.BOOL) -> None:
         afterTrackIdOpt = afterTrack if afterTrack != MprisConstant.NO_TRACK_PATH else None
         self._adapter.addTrack(
             uri=uri,
             afterTrackId=afterTrackIdOpt,
             goTo=goTo
         )
 
-    @dbusMethod(name=MprisTrackListMethod.REMOVE_TRACK)
+    @dbusMethod(name=MprisTrackListMethodId.REMOVE_TRACK.value)
     @no_type_check
     def removeTrack(self, trackId: DbusType.OBJECT) -> None:
         self._adapter.removeTrack(trackId=trackId)
 
-    @dbusMethod(name=MprisTrackListMethod.GO_TO)
+    @dbusMethod(name=MprisTrackListMethodId.GO_TO.value)
     @no_type_check
     def goTo(self, trackId: DbusType.OBJECT) -> None:
         self._adapter.gotTo(trackId=trackId)
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api/model/MprisMetaData.py` & `mpris-api-1.1.0/pkg/mpris_api/model/MprisMetaData.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     MprisMetaDataField.ALBUM_ARTIST: 'as',
     MprisMetaDataField.DISC_NUMBER: 'i',
     MprisMetaDataField.TRACK_NUMBER: 'i',
     MprisMetaDataField.COMMENT: 'as',
 }
 
 
-@dataclass(frozen=True, **({'kw_only': True} if sys.version_info >= (3, 10) else {}))
+@dataclass(frozen=True, **({'kw_only': True} if sys.version_info >= (3, 10) else {}))  # TODO: Adjust when support dropped for: Python < 3.10
 class MprisMetaData:
     trackId: DbusObject
     length: Optional[Microseconds] = None
     artUrl: Optional[str] = None
     url: Optional[str] = None
     title: Optional[str] = None
     artists: Optional[List[str]] = None
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api/model/MprisPlaylist.py` & `mpris-api-1.1.0/pkg/mpris_api/model/MprisPlaylist.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 from mpris_api.common.DbusObjectSpec import DbusObjectSpec
 
 
-@dataclass(frozen=True, **({'kw_only': True} if sys.version_info >= (3, 10) else {}))
+@dataclass(frozen=True, **({'kw_only': True} if sys.version_info >= (3, 10) else {}))   # TODO: Adjust when support dropped for: Python < 3.10
 class MprisPlaylist:
     playlistId: str
     name: str
     iconUri: Optional[str] = None
 
     def __post_init__(self) -> None:
         DbusObjectSpec.assertValid(dbusObj=self.playlistId)
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api.egg-info/PKG-INFO` & `mpris-api-1.1.0/pkg/mpris_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.0.3
+Version: 1.1.0
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.0.3/pkg/mpris_api.egg-info/SOURCES.txt` & `mpris-api-1.1.0/pkg/mpris_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pkg/mpris_api/adapter/IMprisAdapterTrackList.py
 pkg/mpris_api/adapter/__init__.py
 pkg/mpris_api/common/DbusObject.py
 pkg/mpris_api/common/DbusObjectSpec.py
 pkg/mpris_api/common/DbusType.py
 pkg/mpris_api/common/__init__.py
 pkg/mpris_api/common/dbusDecorators.py
+pkg/mpris_api/common/dbusEnums.py
 pkg/mpris_api/interface/MprisInterfaceBase.py
 pkg/mpris_api/interface/MprisInterfacePlayLists.py
 pkg/mpris_api/interface/MprisInterfacePlayer.py
 pkg/mpris_api/interface/MprisInterfaceRoot.py
 pkg/mpris_api/interface/MprisInterfaceTrackList.py
 pkg/mpris_api/interface/__init__.py
 pkg/mpris_api/model/MprisConstant.py
```

### Comparing `mpris-api-1.0.3/pyproject.toml` & `mpris-api-1.1.0/pyproject.toml`

 * *Files identical despite different names*

