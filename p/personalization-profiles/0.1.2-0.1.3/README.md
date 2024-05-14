# Comparing `tmp/personalization_profiles-0.1.2.tar.gz` & `tmp/personalization_profiles-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personalization_profiles-0.1.2.tar", last modified: Tue May 14 20:45:28 2024, max compression
+gzip compressed data, was "personalization_profiles-0.1.3.tar", last modified: Tue May 14 20:47:02 2024, max compression
```

## Comparing `personalization_profiles-0.1.2.tar` & `personalization_profiles-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:45:28.796766 personalization_profiles-0.1.2/
--rw-r--r--   0 borakaragul   (501) staff       (20)      131 2024-05-14 20:45:28.796566 personalization_profiles-0.1.2/PKG-INFO
-drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:45:28.795521 personalization_profiles-0.1.2/personalization_profiles/
--rw-r--r--   0 borakaragul   (501) staff       (20)      912 2024-05-13 17:31:09.000000 personalization_profiles-0.1.2/personalization_profiles/AdventurousTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      804 2024-05-13 17:31:09.000000 personalization_profiles-0.1.2/personalization_profiles/BudgetTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      830 2024-05-13 17:31:09.000000 personalization_profiles-0.1.2/personalization_profiles/BusinessTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      918 2024-05-13 17:31:09.000000 personalization_profiles-0.1.2/personalization_profiles/EcoTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      773 2024-05-14 19:13:29.000000 personalization_profiles-0.1.2/personalization_profiles/FamilyTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)     2528 2024-05-14 19:30:38.000000 personalization_profiles-0.1.2/personalization_profiles/PersonaManager.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      167 2024-05-13 17:31:09.000000 personalization_profiles-0.1.2/personalization_profiles/PersonaType.py
--rw-r--r--   0 borakaragul   (501) staff       (20)     3055 2024-05-14 19:13:21.000000 personalization_profiles-0.1.2/personalization_profiles/PersonalizationProfile.py
--rw-r--r--   0 borakaragul   (501) staff       (20)     1041 2024-05-14 19:23:23.000000 personalization_profiles-0.1.2/personalization_profiles/User.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      268 2024-05-14 18:54:26.000000 personalization_profiles-0.1.2/personalization_profiles/__init__.py
-drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:45:28.796355 personalization_profiles-0.1.2/personalization_profiles.egg-info/
--rw-r--r--   0 borakaragul   (501) staff       (20)      131 2024-05-14 20:45:28.000000 personalization_profiles-0.1.2/personalization_profiles.egg-info/PKG-INFO
--rw-r--r--   0 borakaragul   (501) staff       (20)      670 2024-05-14 20:45:28.000000 personalization_profiles-0.1.2/personalization_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 borakaragul   (501) staff       (20)        1 2024-05-14 20:45:28.000000 personalization_profiles-0.1.2/personalization_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 borakaragul   (501) staff       (20)       12 2024-05-14 20:45:28.000000 personalization_profiles-0.1.2/personalization_profiles.egg-info/requires.txt
--rw-r--r--   0 borakaragul   (501) staff       (20)       25 2024-05-14 20:45:28.000000 personalization_profiles-0.1.2/personalization_profiles.egg-info/top_level.txt
--rw-r--r--   0 borakaragul   (501) staff       (20)       38 2024-05-14 20:45:28.796800 personalization_profiles-0.1.2/setup.cfg
--rw-r--r--   0 borakaragul   (501) staff       (20)      272 2024-05-14 20:43:15.000000 personalization_profiles-0.1.2/setup.py
+drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:47:02.853700 personalization_profiles-0.1.3/
+-rw-r--r--   0 borakaragul   (501) staff       (20)      176 2024-05-14 20:47:02.853491 personalization_profiles-0.1.3/PKG-INFO
+drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:47:02.852466 personalization_profiles-0.1.3/personalization_profiles/
+-rw-r--r--   0 borakaragul   (501) staff       (20)      912 2024-05-13 17:31:09.000000 personalization_profiles-0.1.3/personalization_profiles/AdventurousTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      804 2024-05-13 17:31:09.000000 personalization_profiles-0.1.3/personalization_profiles/BudgetTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      830 2024-05-13 17:31:09.000000 personalization_profiles-0.1.3/personalization_profiles/BusinessTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      918 2024-05-13 17:31:09.000000 personalization_profiles-0.1.3/personalization_profiles/EcoTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      773 2024-05-14 19:13:29.000000 personalization_profiles-0.1.3/personalization_profiles/FamilyTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)     2528 2024-05-14 19:30:38.000000 personalization_profiles-0.1.3/personalization_profiles/PersonaManager.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      167 2024-05-13 17:31:09.000000 personalization_profiles-0.1.3/personalization_profiles/PersonaType.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)     3055 2024-05-14 19:13:21.000000 personalization_profiles-0.1.3/personalization_profiles/PersonalizationProfile.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)     1041 2024-05-14 19:23:23.000000 personalization_profiles-0.1.3/personalization_profiles/User.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      268 2024-05-14 18:54:26.000000 personalization_profiles-0.1.3/personalization_profiles/__init__.py
+drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:47:02.853305 personalization_profiles-0.1.3/personalization_profiles.egg-info/
+-rw-r--r--   0 borakaragul   (501) staff       (20)      176 2024-05-14 20:47:02.000000 personalization_profiles-0.1.3/personalization_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 borakaragul   (501) staff       (20)      670 2024-05-14 20:47:02.000000 personalization_profiles-0.1.3/personalization_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 borakaragul   (501) staff       (20)        1 2024-05-14 20:47:02.000000 personalization_profiles-0.1.3/personalization_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 borakaragul   (501) staff       (20)       27 2024-05-14 20:47:02.000000 personalization_profiles-0.1.3/personalization_profiles.egg-info/requires.txt
+-rw-r--r--   0 borakaragul   (501) staff       (20)       25 2024-05-14 20:47:02.000000 personalization_profiles-0.1.3/personalization_profiles.egg-info/top_level.txt
+-rw-r--r--   0 borakaragul   (501) staff       (20)       38 2024-05-14 20:47:02.853736 personalization_profiles-0.1.3/setup.cfg
+-rw-r--r--   0 borakaragul   (501) staff       (20)      309 2024-05-14 20:47:00.000000 personalization_profiles-0.1.3/setup.py
```

### Comparing `personalization_profiles-0.1.2/personalization_profiles/AdventurousTraveler.py` & `personalization_profiles-0.1.3/personalization_profiles/AdventurousTraveler.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles/BudgetTraveler.py` & `personalization_profiles-0.1.3/personalization_profiles/BudgetTraveler.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles/BusinessTraveler.py` & `personalization_profiles-0.1.3/personalization_profiles/BusinessTraveler.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles/EcoTraveler.py` & `personalization_profiles-0.1.3/personalization_profiles/EcoTraveler.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles/FamilyTraveler.py` & `personalization_profiles-0.1.3/personalization_profiles/FamilyTraveler.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles/PersonaManager.py` & `personalization_profiles-0.1.3/personalization_profiles/PersonaManager.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles/PersonalizationProfile.py` & `personalization_profiles-0.1.3/personalization_profiles/PersonalizationProfile.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles/User.py` & `personalization_profiles-0.1.3/personalization_profiles/User.py`

 * *Files identical despite different names*

### Comparing `personalization_profiles-0.1.2/personalization_profiles.egg-info/SOURCES.txt` & `personalization_profiles-0.1.3/personalization_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

