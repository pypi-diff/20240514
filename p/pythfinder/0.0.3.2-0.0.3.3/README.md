# Comparing `tmp/pythfinder-0.0.3.2.tar.gz` & `tmp/pythfinder-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythfinder-0.0.3.2.tar", last modified: Tue May 14 18:00:42 2024, max compression
+gzip compressed data, was "pythfinder-0.0.3.3.tar", last modified: Tue May 14 18:09:43 2024, max compression
```

## Comparing `pythfinder-0.0.3.2.tar` & `pythfinder-0.0.3.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.552543 pythfinder-0.0.3.2/
--rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0      310 2024-05-14 18:00:42.552543 pythfinder-0.0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-05-14 17:14:21.000000 pythfinder-0.0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.452268 pythfinder-0.0.3.2/pythfinder/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.467899 pythfinder-0.0.3.2/pythfinder/Components/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.483524 pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/
--rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/__init__.py
--rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/booleanEx.py
--rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/edgeDetectorEx.py
--rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/errorEx.py
--rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/mathEx.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.499151 pythfinder-0.0.3.2/pythfinder/Components/Constants/
--rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.2/pythfinder/Components/Constants/__init__.py
--rw-rw-rw-   0        0        0    20781 2024-05-14 16:07:20.000000 pythfinder-0.0.3.2/pythfinder/Components/Constants/constants.py
--rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.2/pythfinder/Components/Constants/constrains.py
--rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.2/pythfinder/Components/Constants/screenSize.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.514777 pythfinder-0.0.3.2/pythfinder/Components/Controllers/
--rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.2/pythfinder/Components/Controllers/PIDCoefficients.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.2/pythfinder/Components/Controllers/PIDController.py
--rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.2/pythfinder/Components/Controllers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.530403 pythfinder-0.0.3.2/pythfinder/Components/Menu/
--rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.2/pythfinder/Components/Menu/__init__.py
--rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.2/pythfinder/Components/Menu/buttons.py
--rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.2/pythfinder/Components/Menu/enums.py
--rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.2/pythfinder/Components/Menu/main.py
--rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.2/pythfinder/Components/Menu/menus.py
--rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.2/pythfinder/Components/__init__.py
--rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.2/pythfinder/Components/background.py
--rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.2/pythfinder/Components/controls.py
--rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.2/pythfinder/Components/fade.py
--rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.2/pythfinder/Components/robot.py
--rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.2/pythfinder/Components/table.py
--rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.2/pythfinder/Components/trail.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.552543 pythfinder-0.0.3.2/pythfinder/Trajectory/
--rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.2/pythfinder/Trajectory/__init__.py
--rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.2/pythfinder/Trajectory/builder.py
--rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.2/pythfinder/Trajectory/feedback.py
--rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.2/pythfinder/Trajectory/feedforward.py
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.2/pythfinder/Trajectory/kinematics.py
--rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.2/pythfinder/Trajectory/splines.py
--rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.2/pythfinder/__init__.py
--rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.2/pythfinder/core.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:00:42.452268 pythfinder-0.0.3.2/pythfinder.egg-info/
--rw-rw-rw-   0        0        0      310 2024-05-14 18:00:42.000000 pythfinder-0.0.3.2/pythfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2024-05-14 18:00:42.000000 pythfinder-0.0.3.2/pythfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:00:42.000000 pythfinder-0.0.3.2/pythfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 18:00:42.000000 pythfinder-0.0.3.2/pythfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 18:00:42.552543 pythfinder-0.0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      506 2024-05-14 17:59:58.000000 pythfinder-0.0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.921224 pythfinder-0.0.3.3/
+-rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      310 2024-05-14 18:09:43.921224 pythfinder-0.0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-05-14 17:14:21.000000 pythfinder-0.0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.808488 pythfinder-0.0.3.3/pythfinder/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.840666 pythfinder-0.0.3.3/pythfinder/Components/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.860787 pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/
+-rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/__init__.py
+-rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/booleanEx.py
+-rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/edgeDetectorEx.py
+-rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/errorEx.py
+-rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/mathEx.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.870847 pythfinder-0.0.3.3/pythfinder/Components/Constants/
+-rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.3/pythfinder/Components/Constants/__init__.py
+-rw-rw-rw-   0        0        0    20781 2024-05-14 18:06:58.000000 pythfinder-0.0.3.3/pythfinder/Components/Constants/constants.py
+-rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.3/pythfinder/Components/Constants/constrains.py
+-rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.3/pythfinder/Components/Constants/screenSize.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.880891 pythfinder-0.0.3.3/pythfinder/Components/Controllers/
+-rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.3/pythfinder/Components/Controllers/PIDCoefficients.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.3/pythfinder/Components/Controllers/PIDController.py
+-rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.3/pythfinder/Components/Controllers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.900995 pythfinder-0.0.3.3/pythfinder/Components/Menu/
+-rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.3/pythfinder/Components/Menu/__init__.py
+-rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.3/pythfinder/Components/Menu/buttons.py
+-rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.3/pythfinder/Components/Menu/enums.py
+-rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.3/pythfinder/Components/Menu/main.py
+-rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.3/pythfinder/Components/Menu/menus.py
+-rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.3/pythfinder/Components/__init__.py
+-rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.3/pythfinder/Components/background.py
+-rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.3/pythfinder/Components/controls.py
+-rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.3/pythfinder/Components/fade.py
+-rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.3/pythfinder/Components/robot.py
+-rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.3/pythfinder/Components/table.py
+-rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.3/pythfinder/Components/trail.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.921224 pythfinder-0.0.3.3/pythfinder/Trajectory/
+-rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.3/pythfinder/Trajectory/__init__.py
+-rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.3/pythfinder/Trajectory/builder.py
+-rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.3/pythfinder/Trajectory/feedback.py
+-rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.3/pythfinder/Trajectory/feedforward.py
+-rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.3/pythfinder/Trajectory/kinematics.py
+-rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.3/pythfinder/Trajectory/splines.py
+-rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.3/pythfinder/__init__.py
+-rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.3/pythfinder/core.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:09:43.820554 pythfinder-0.0.3.3/pythfinder.egg-info/
+-rw-rw-rw-   0        0        0      310 2024-05-14 18:09:43.000000 pythfinder-0.0.3.3/pythfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1401 2024-05-14 18:09:43.000000 pythfinder-0.0.3.3/pythfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:09:43.000000 pythfinder-0.0.3.3/pythfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 18:09:43.000000 pythfinder-0.0.3.3/pythfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:09:43.921224 pythfinder-0.0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      506 2024-05-14 18:09:23.000000 pythfinder-0.0.3.3/setup.py
```

### Comparing `pythfinder-0.0.3.2/LICENSE.txt` & `pythfinder-0.0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/booleanEx.py` & `pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/booleanEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/edgeDetectorEx.py` & `pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/edgeDetectorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/errorEx.py` & `pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/errorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/BetterClasses/mathEx.py` & `pythfinder-0.0.3.3/pythfinder/Components/BetterClasses/mathEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Constants/constants.py` & `pythfinder-0.0.3.3/pythfinder/Components/Constants/constants.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Constants/constrains.py` & `pythfinder-0.0.3.3/pythfinder/Components/Constants/constrains.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Constants/screenSize.py` & `pythfinder-0.0.3.3/pythfinder/Components/Constants/screenSize.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Controllers/PIDCoefficients.py` & `pythfinder-0.0.3.3/pythfinder/Components/Controllers/PIDCoefficients.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Controllers/PIDController.py` & `pythfinder-0.0.3.3/pythfinder/Components/Controllers/PIDController.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Menu/buttons.py` & `pythfinder-0.0.3.3/pythfinder/Components/Menu/buttons.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Menu/enums.py` & `pythfinder-0.0.3.3/pythfinder/Components/Menu/enums.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Menu/main.py` & `pythfinder-0.0.3.3/pythfinder/Components/Menu/main.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/Menu/menus.py` & `pythfinder-0.0.3.3/pythfinder/Components/Menu/menus.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/background.py` & `pythfinder-0.0.3.3/pythfinder/Components/background.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/controls.py` & `pythfinder-0.0.3.3/pythfinder/Components/controls.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/fade.py` & `pythfinder-0.0.3.3/pythfinder/Components/fade.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/robot.py` & `pythfinder-0.0.3.3/pythfinder/Components/robot.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/table.py` & `pythfinder-0.0.3.3/pythfinder/Components/table.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Components/trail.py` & `pythfinder-0.0.3.3/pythfinder/Components/trail.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Trajectory/builder.py` & `pythfinder-0.0.3.3/pythfinder/Trajectory/builder.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Trajectory/feedback.py` & `pythfinder-0.0.3.3/pythfinder/Trajectory/feedback.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Trajectory/feedforward.py` & `pythfinder-0.0.3.3/pythfinder/Trajectory/feedforward.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Trajectory/kinematics.py` & `pythfinder-0.0.3.3/pythfinder/Trajectory/kinematics.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/Trajectory/splines.py` & `pythfinder-0.0.3.3/pythfinder/Trajectory/splines.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder/core.py` & `pythfinder-0.0.3.3/pythfinder/core.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.2/pythfinder.egg-info/SOURCES.txt` & `pythfinder-0.0.3.3/pythfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

