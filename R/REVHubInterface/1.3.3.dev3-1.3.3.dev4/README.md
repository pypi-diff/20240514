# Comparing `tmp/revhubinterface-1.3.3.dev3.tar.gz` & `tmp/revhubinterface-1.3.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.3.dev3.tar", last modified: Mon May 13 18:17:50 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.3.dev4.tar", last modified: Tue May 14 04:09:44 2024, max compression
```

## Comparing `revhubinterface-1.3.3.dev3.tar` & `revhubinterface-1.3.3.dev4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.438745 revhubinterface-1.3.3.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.438745 revhubinterface-1.3.3.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 18:17:50.000000 revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:17:50.442745 revhubinterface-1.3.3.dev3/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 18:17:45.000000 revhubinterface-1.3.3.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:17:50.446745 revhubinterface-1.3.3.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:09:44.551263 revhubinterface-1.3.3.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:09:44.543263 revhubinterface-1.3.3.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:09:44.547263 revhubinterface-1.3.3.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 04:09:44.551263 revhubinterface-1.3.3.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:09:44.547263 revhubinterface-1.3.3.dev4/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:09:44.551263 revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 04:09:44.000000 revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-14 04:09:44.000000 revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 04:09:44.000000 revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 04:09:44.000000 revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 04:09:44.000000 revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 04:09:44.000000 revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 04:09:44.551263 revhubinterface-1.3.3.dev4/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 04:09:39.000000 revhubinterface-1.3.3.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 04:09:44.551263 revhubinterface-1.3.3.dev4/setup.cfg
```

### Comparing `revhubinterface-1.3.3.dev3/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.3.dev4/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/.github/workflows/python-publish.yml` & `revhubinterface-1.3.3.dev4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/LICENSE.txt` & `revhubinterface-1.3.3.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/PKG-INFO` & `revhubinterface-1.3.3.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev3
+Version: 1.3.3.dev4
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev3/README.md` & `revhubinterface-1.3.3.dev4/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVADC.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVModule.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVServo.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface/__main__.py` & `revhubinterface-1.3.3.dev4/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev3
+Version: 1.3.3.dev4
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.3.dev4/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/REVHubInterface.spec` & `revhubinterface-1.3.3.dev4/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.3.dev4/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.3.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/flatpak/python3-requirements.json` & `revhubinterface-1.3.3.dev4/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files 26% similar despite different names*

#### Comparing `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml`

```diff
@@ -1,17 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component type="desktop-application">
   <id>org.unofficialrevport.REVHubInterface</id>
   <launchable type="desktop-id">org.unofficialrevport.REVHubInterface.desktop</launchable>
   <name>REV Hub Interface - Community Edition</name>
-  <metadata_license/>
-  <project_license/>
-  <summary>GUI program for manual control of a REV Robotics Expansion Hub from a PC. Unofficial &quot;Community Edition&quot;.</summary>
+  <metadata_license>FSFAP</metadata_license>
+  <project_license>BSD-3-Clause</project_license>
+  <summary>Directly control a REV Robotics Expansion Hub</summary>
   <description>The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC.
 
 This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.
 
-This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows). Though initially created by REV, this version of the software is **not maintained by or affiliated with REV.**  Do **not** contact REV support about any issues you experience with this software, instead you may create a GitHub Issue or ask in https://discord.gg/pU2fesSTqF.
-
-This software is licensed under the BSD-3-Clause license. The full text is availiable in the LICENSE.txt file.</description>
-  <developer_name>Unofficial REV Port Team</developer_name>
+This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows). Though initially created by REV, this version of the software is not maintained by or affiliated with REV. Do not contact REV support about any issues you experience with this software, instead you may create a GitHub Issue at https://github.com/unofficial-rev-port/REVHubInterface/ or ask in https://discord.gg/pU2fesSTqF.</description>
+  <url type="vcs-browser">https://github.com/unofficial-rev-port/REVHubInterface/</url>
+  <url type="contact">https://discord.gg/pU2fesSTqF</url>
+  <url type="homepage">https://github.com/unofficial-rev-port/REVHubInterface/</url>
+  <developer id="org.unofficialrevport">
+    <name>The Unofficial REV Port Team</name>
+    <url>https://unofficialrevport.org</url>
+  </developer>
+  <content_rating type="oars-1.0"/>
 </component>
```

### Comparing `revhubinterface-1.3.3.dev3/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.3.dev4/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev3/pyproject.toml` & `revhubinterface-1.3.3.dev4/pyproject.toml`

 * *Files identical despite different names*

