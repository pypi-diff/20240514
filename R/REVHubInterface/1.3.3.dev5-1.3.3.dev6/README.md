# Comparing `tmp/revhubinterface-1.3.3.dev5.tar.gz` & `tmp/revhubinterface-1.3.3.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.3.dev5.tar", last modified: Tue May 14 06:51:06 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.3.dev6.tar", last modified: Tue May 14 06:58:36 2024, max compression
```

## Comparing `revhubinterface-1.3.3.dev5.tar` & `revhubinterface-1.3.3.dev6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:06.344449 revhubinterface-1.3.3.dev5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:06.336449 revhubinterface-1.3.3.dev5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:06.340449 revhubinterface-1.3.3.dev5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 06:51:06.344449 revhubinterface-1.3.3.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:06.340449 revhubinterface-1.3.3.dev5/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:06.344449 revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 06:51:06.000000 revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-14 06:51:06.000000 revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:51:06.000000 revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 06:51:06.000000 revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 06:51:06.000000 revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 06:51:06.000000 revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:51:06.340449 revhubinterface-1.3.3.dev5/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 06:51:01.000000 revhubinterface-1.3.3.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:51:06.344449 revhubinterface-1.3.3.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:58:36.714625 revhubinterface-1.3.3.dev6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:58:36.706625 revhubinterface-1.3.3.dev6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:58:36.706625 revhubinterface-1.3.3.dev6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 06:58:36.714625 revhubinterface-1.3.3.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:58:36.710625 revhubinterface-1.3.3.dev6/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61200 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:58:36.714625 revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-14 06:58:36.000000 revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-14 06:58:36.000000 revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 06:58:36.000000 revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-14 06:58:36.000000 revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 06:58:36.000000 revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 06:58:36.000000 revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 06:58:36.710625 revhubinterface-1.3.3.dev6/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-14 06:58:27.000000 revhubinterface-1.3.3.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 06:58:36.714625 revhubinterface-1.3.3.dev6/setup.cfg
```

### Comparing `revhubinterface-1.3.3.dev5/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.3.dev6/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/.github/workflows/python-publish.yml` & `revhubinterface-1.3.3.dev6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/LICENSE.txt` & `revhubinterface-1.3.3.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/PKG-INFO` & `revhubinterface-1.3.3.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev5
+Version: 1.3.3.dev6
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev5/README.md` & `revhubinterface-1.3.3.dev6/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVADC.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVModule.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVServo.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface/__main__.py` & `revhubinterface-1.3.3.dev6/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.3.dev5
+Version: 1.3.3.dev6
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.3.dev6/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/REVHubInterface.spec` & `revhubinterface-1.3.3.dev6/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.3.dev6/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.3.dev6/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/flatpak/python3-requirements.json` & `revhubinterface-1.3.3.dev6/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files 3% similar despite different names*

#### Comparing `revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.metainfo.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component type="desktop-application">
   <id>org.unofficialrevport.REVHubInterface</id>
   <launchable type="desktop-id">org.unofficialrevport.REVHubInterface.desktop</launchable>
-  <name>REV Hub Interface</name>
+  <name>REV Hub Interface - Community Edition</name>
   <metadata_license>FSFAP</metadata_license>
   <project_license>BSD-3-Clause</project_license>
   <summary>Directly control a REV Robotics Expansion Hub</summary>
   <description>
     <p>The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC.</p>
     <p>This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.</p>
     <p>This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows). Though initially created by REV, this version of the software is not maintained by or affiliated with REV. Do not contact REV support about any issues you experience with this software.</p>
```

### Comparing `revhubinterface-1.3.3.dev5/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.3.dev6/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.3.dev5/pyproject.toml` & `revhubinterface-1.3.3.dev6/pyproject.toml`

 * *Files identical despite different names*

