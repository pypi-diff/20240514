# Comparing `tmp/pythfinder-0.0.3.4.tar.gz` & `tmp/pythfinder-0.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythfinder-0.0.3.4.tar", last modified: Tue May 14 18:19:24 2024, max compression
+gzip compressed data, was "pythfinder-0.0.3.5.tar", last modified: Tue May 14 18:26:59 2024, max compression
```

## Comparing `pythfinder-0.0.3.4.tar` & `pythfinder-0.0.3.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.402591 pythfinder-0.0.3.4/
--rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0      310 2024-05-14 18:19:24.402591 pythfinder-0.0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-05-14 17:14:21.000000 pythfinder-0.0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.274675 pythfinder-0.0.3.4/pythfinder/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.317950 pythfinder-0.0.3.4/pythfinder/Components/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.333574 pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/
--rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/__init__.py
--rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/booleanEx.py
--rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/edgeDetectorEx.py
--rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/errorEx.py
--rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/mathEx.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.349202 pythfinder-0.0.3.4/pythfinder/Components/Constants/
--rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.4/pythfinder/Components/Constants/__init__.py
--rw-rw-rw-   0        0        0    20781 2024-05-14 18:06:58.000000 pythfinder-0.0.3.4/pythfinder/Components/Constants/constants.py
--rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.4/pythfinder/Components/Constants/constrains.py
--rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.4/pythfinder/Components/Constants/screenSize.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.349202 pythfinder-0.0.3.4/pythfinder/Components/Controllers/
--rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.4/pythfinder/Components/Controllers/PIDCoefficients.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.4/pythfinder/Components/Controllers/PIDController.py
--rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.4/pythfinder/Components/Controllers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.380453 pythfinder-0.0.3.4/pythfinder/Components/Menu/
--rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.4/pythfinder/Components/Menu/__init__.py
--rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.4/pythfinder/Components/Menu/buttons.py
--rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.4/pythfinder/Components/Menu/enums.py
--rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.4/pythfinder/Components/Menu/main.py
--rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.4/pythfinder/Components/Menu/menus.py
--rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.4/pythfinder/Components/__init__.py
--rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.4/pythfinder/Components/background.py
--rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.4/pythfinder/Components/controls.py
--rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.4/pythfinder/Components/fade.py
--rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.4/pythfinder/Components/robot.py
--rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.4/pythfinder/Components/table.py
--rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.4/pythfinder/Components/trail.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.380453 pythfinder-0.0.3.4/pythfinder/Images/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.380453 pythfinder-0.0.3.4/pythfinder/Images/Controls/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.4/pythfinder/Images/Controls/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.380453 pythfinder-0.0.3.4/pythfinder/Images/Menu/
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.380453 pythfinder-0.0.3.4/pythfinder/Images/Menu/General/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.4/pythfinder/Images/Menu/General/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.4/pythfinder/Images/Menu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.386961 pythfinder-0.0.3.4/pythfinder/Images/Robot/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.4/pythfinder/Images/Robot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.386961 pythfinder-0.0.3.4/pythfinder/Images/Table/
--rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.4/pythfinder/Images/Table/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.4/pythfinder/Images/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.386961 pythfinder-0.0.3.4/pythfinder/Trajectory/
--rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.4/pythfinder/Trajectory/__init__.py
--rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.4/pythfinder/Trajectory/builder.py
--rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.4/pythfinder/Trajectory/feedback.py
--rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.4/pythfinder/Trajectory/feedforward.py
--rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.4/pythfinder/Trajectory/kinematics.py
--rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.4/pythfinder/Trajectory/splines.py
--rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.4/pythfinder/__init__.py
--rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.4/pythfinder/core.py
-drwxrwxrwx   0        0        0        0 2024-05-14 18:19:24.302331 pythfinder-0.0.3.4/pythfinder.egg-info/
--rw-rw-rw-   0        0        0      310 2024-05-14 18:19:24.000000 pythfinder-0.0.3.4/pythfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1620 2024-05-14 18:19:24.000000 pythfinder-0.0.3.4/pythfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 18:19:24.000000 pythfinder-0.0.3.4/pythfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 18:19:24.000000 pythfinder-0.0.3.4/pythfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 18:19:24.402591 pythfinder-0.0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      506 2024-05-14 18:19:17.000000 pythfinder-0.0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.294147 pythfinder-0.0.3.5/
+-rw-rw-rw-   0        0        0     1295 2024-05-14 05:43:57.000000 pythfinder-0.0.3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      310 2024-05-14 18:26:59.294147 pythfinder-0.0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-05-14 18:26:37.000000 pythfinder-0.0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.175159 pythfinder-0.0.3.5/pythfinder/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.216013 pythfinder-0.0.3.5/pythfinder/Components/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.216013 pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/
+-rw-rw-rw-   0        0        0      102 2024-05-14 05:32:56.000000 pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/__init__.py
+-rw-rw-rw-   0        0        0     1168 2024-05-13 14:52:24.000000 pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/booleanEx.py
+-rw-rw-rw-   0        0        0      627 2024-05-13 14:52:55.000000 pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/edgeDetectorEx.py
+-rw-rw-rw-   0        0        0     1140 2024-05-13 15:07:55.000000 pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/errorEx.py
+-rw-rw-rw-   0        0        0     4862 2024-05-13 14:45:33.000000 pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/mathEx.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.231644 pythfinder-0.0.3.5/pythfinder/Components/Constants/
+-rw-rw-rw-   0        0        0       78 2024-05-14 05:33:11.000000 pythfinder-0.0.3.5/pythfinder/Components/Constants/__init__.py
+-rw-rw-rw-   0        0        0    20781 2024-05-14 18:06:58.000000 pythfinder-0.0.3.5/pythfinder/Components/Constants/constants.py
+-rw-rw-rw-   0        0        0     2905 2024-05-13 15:08:14.000000 pythfinder-0.0.3.5/pythfinder/Components/Constants/constrains.py
+-rw-rw-rw-   0        0        0     2705 2024-05-13 15:11:03.000000 pythfinder-0.0.3.5/pythfinder/Components/Constants/screenSize.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.247272 pythfinder-0.0.3.5/pythfinder/Components/Controllers/
+-rw-rw-rw-   0        0        0      642 2024-05-13 15:12:44.000000 pythfinder-0.0.3.5/pythfinder/Components/Controllers/PIDCoefficients.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 16:07:14.000000 pythfinder-0.0.3.5/pythfinder/Components/Controllers/PIDController.py
+-rw-rw-rw-   0        0        0       60 2024-05-14 05:33:22.000000 pythfinder-0.0.3.5/pythfinder/Components/Controllers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.262896 pythfinder-0.0.3.5/pythfinder/Components/Menu/
+-rw-rw-rw-   0        0        0       87 2024-05-14 05:33:37.000000 pythfinder-0.0.3.5/pythfinder/Components/Menu/__init__.py
+-rw-rw-rw-   0        0        0    22248 2024-05-14 16:06:43.000000 pythfinder-0.0.3.5/pythfinder/Components/Menu/buttons.py
+-rw-rw-rw-   0        0        0     1583 2024-05-13 16:09:13.000000 pythfinder-0.0.3.5/pythfinder/Components/Menu/enums.py
+-rw-rw-rw-   0        0        0    22448 2024-05-14 16:06:48.000000 pythfinder-0.0.3.5/pythfinder/Components/Menu/main.py
+-rw-rw-rw-   0        0        0     4103 2024-05-14 16:07:01.000000 pythfinder-0.0.3.5/pythfinder/Components/Menu/menus.py
+-rw-rw-rw-   0        0        0      244 2024-05-14 05:35:39.000000 pythfinder-0.0.3.5/pythfinder/Components/__init__.py
+-rw-rw-rw-   0        0        0     5720 2024-05-14 16:04:43.000000 pythfinder-0.0.3.5/pythfinder/Components/background.py
+-rw-rw-rw-   0        0        0     9569 2024-05-14 16:05:08.000000 pythfinder-0.0.3.5/pythfinder/Components/controls.py
+-rw-rw-rw-   0        0        0     1853 2024-05-14 16:05:12.000000 pythfinder-0.0.3.5/pythfinder/Components/fade.py
+-rw-rw-rw-   0        0        0     9861 2024-05-14 15:58:30.000000 pythfinder-0.0.3.5/pythfinder/Components/robot.py
+-rw-rw-rw-   0        0        0     1975 2024-05-14 16:05:20.000000 pythfinder-0.0.3.5/pythfinder/Components/table.py
+-rw-rw-rw-   0        0        0     4633 2024-05-14 16:05:37.000000 pythfinder-0.0.3.5/pythfinder/Components/trail.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.262896 pythfinder-0.0.3.5/pythfinder/Images/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.262896 pythfinder-0.0.3.5/pythfinder/Images/Controls/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:56.000000 pythfinder-0.0.3.5/pythfinder/Images/Controls/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.262896 pythfinder-0.0.3.5/pythfinder/Images/Menu/
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.262896 pythfinder-0.0.3.5/pythfinder/Images/Menu/General/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:26.000000 pythfinder-0.0.3.5/pythfinder/Images/Menu/General/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:10.000000 pythfinder-0.0.3.5/pythfinder/Images/Menu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.262896 pythfinder-0.0.3.5/pythfinder/Images/Robot/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:18:58.000000 pythfinder-0.0.3.5/pythfinder/Images/Robot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.262896 pythfinder-0.0.3.5/pythfinder/Images/Table/
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:19:06.000000 pythfinder-0.0.3.5/pythfinder/Images/Table/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 18:17:47.000000 pythfinder-0.0.3.5/pythfinder/Images/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.278522 pythfinder-0.0.3.5/pythfinder/Trajectory/
+-rw-rw-rw-   0        0        0      126 2024-05-14 05:34:50.000000 pythfinder-0.0.3.5/pythfinder/Trajectory/__init__.py
+-rw-rw-rw-   0        0        0    52721 2024-05-14 16:09:04.000000 pythfinder-0.0.3.5/pythfinder/Trajectory/builder.py
+-rw-rw-rw-   0        0        0     1709 2024-05-14 16:06:07.000000 pythfinder-0.0.3.5/pythfinder/Trajectory/feedback.py
+-rw-rw-rw-   0        0        0     4366 2024-05-14 16:06:12.000000 pythfinder-0.0.3.5/pythfinder/Trajectory/feedforward.py
+-rw-rw-rw-   0        0        0     1564 2024-05-14 16:06:17.000000 pythfinder-0.0.3.5/pythfinder/Trajectory/kinematics.py
+-rw-rw-rw-   0        0        0     5914 2024-05-14 16:06:21.000000 pythfinder-0.0.3.5/pythfinder/Trajectory/splines.py
+-rw-rw-rw-   0        0        0       98 2024-05-14 05:35:53.000000 pythfinder-0.0.3.5/pythfinder/__init__.py
+-rw-rw-rw-   0        0        0    11119 2024-05-14 16:29:39.000000 pythfinder-0.0.3.5/pythfinder/core.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:26:59.181258 pythfinder-0.0.3.5/pythfinder.egg-info/
+-rw-rw-rw-   0        0        0      310 2024-05-14 18:26:59.000000 pythfinder-0.0.3.5/pythfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1620 2024-05-14 18:26:59.000000 pythfinder-0.0.3.5/pythfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:26:59.000000 pythfinder-0.0.3.5/pythfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 18:26:59.000000 pythfinder-0.0.3.5/pythfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:26:59.294147 pythfinder-0.0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-05-14 18:26:54.000000 pythfinder-0.0.3.5/setup.py
```

### Comparing `pythfinder-0.0.3.4/LICENSE.txt` & `pythfinder-0.0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/booleanEx.py` & `pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/booleanEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/edgeDetectorEx.py` & `pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/edgeDetectorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/errorEx.py` & `pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/errorEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/BetterClasses/mathEx.py` & `pythfinder-0.0.3.5/pythfinder/Components/BetterClasses/mathEx.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Constants/constants.py` & `pythfinder-0.0.3.5/pythfinder/Components/Constants/constants.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Constants/constrains.py` & `pythfinder-0.0.3.5/pythfinder/Components/Constants/constrains.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Constants/screenSize.py` & `pythfinder-0.0.3.5/pythfinder/Components/Constants/screenSize.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Controllers/PIDCoefficients.py` & `pythfinder-0.0.3.5/pythfinder/Components/Controllers/PIDCoefficients.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Controllers/PIDController.py` & `pythfinder-0.0.3.5/pythfinder/Components/Controllers/PIDController.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Menu/buttons.py` & `pythfinder-0.0.3.5/pythfinder/Components/Menu/buttons.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Menu/enums.py` & `pythfinder-0.0.3.5/pythfinder/Components/Menu/enums.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Menu/main.py` & `pythfinder-0.0.3.5/pythfinder/Components/Menu/main.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/Menu/menus.py` & `pythfinder-0.0.3.5/pythfinder/Components/Menu/menus.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/background.py` & `pythfinder-0.0.3.5/pythfinder/Components/background.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/controls.py` & `pythfinder-0.0.3.5/pythfinder/Components/controls.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/fade.py` & `pythfinder-0.0.3.5/pythfinder/Components/fade.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/robot.py` & `pythfinder-0.0.3.5/pythfinder/Components/robot.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/table.py` & `pythfinder-0.0.3.5/pythfinder/Components/table.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Components/trail.py` & `pythfinder-0.0.3.5/pythfinder/Components/trail.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Trajectory/builder.py` & `pythfinder-0.0.3.5/pythfinder/Trajectory/builder.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Trajectory/feedback.py` & `pythfinder-0.0.3.5/pythfinder/Trajectory/feedback.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Trajectory/feedforward.py` & `pythfinder-0.0.3.5/pythfinder/Trajectory/feedforward.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Trajectory/kinematics.py` & `pythfinder-0.0.3.5/pythfinder/Trajectory/kinematics.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/Trajectory/splines.py` & `pythfinder-0.0.3.5/pythfinder/Trajectory/splines.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder/core.py` & `pythfinder-0.0.3.5/pythfinder/core.py`

 * *Files identical despite different names*

### Comparing `pythfinder-0.0.3.4/pythfinder.egg-info/SOURCES.txt` & `pythfinder-0.0.3.5/pythfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

