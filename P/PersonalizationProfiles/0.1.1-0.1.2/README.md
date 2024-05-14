# Comparing `tmp/PersonalizationProfiles-0.1.1.tar.gz` & `tmp/PersonalizationProfiles-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PersonalizationProfiles-0.1.1.tar", last modified: Tue May 14 19:14:14 2024, max compression
+gzip compressed data, was "PersonalizationProfiles-0.1.2.tar", last modified: Tue May 14 20:06:23 2024, max compression
```

## Comparing `PersonalizationProfiles-0.1.1.tar` & `PersonalizationProfiles-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 19:14:14.766347 PersonalizationProfiles-0.1.1/
--rw-r--r--   0 borakaragul   (501) staff       (20)       94 2024-05-14 19:14:14.766156 PersonalizationProfiles-0.1.1/PKG-INFO
-drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 19:14:14.765960 PersonalizationProfiles-0.1.1/PersonalizationProfiles.egg-info/
--rw-r--r--   0 borakaragul   (501) staff       (20)       94 2024-05-14 19:14:14.000000 PersonalizationProfiles-0.1.1/PersonalizationProfiles.egg-info/PKG-INFO
--rw-r--r--   0 borakaragul   (501) staff       (20)      665 2024-05-14 19:14:14.000000 PersonalizationProfiles-0.1.1/PersonalizationProfiles.egg-info/SOURCES.txt
--rw-r--r--   0 borakaragul   (501) staff       (20)        1 2024-05-14 19:14:14.000000 PersonalizationProfiles-0.1.1/PersonalizationProfiles.egg-info/dependency_links.txt
--rw-r--r--   0 borakaragul   (501) staff       (20)       12 2024-05-14 19:14:14.000000 PersonalizationProfiles-0.1.1/PersonalizationProfiles.egg-info/requires.txt
--rw-r--r--   0 borakaragul   (501) staff       (20)       25 2024-05-14 19:14:14.000000 PersonalizationProfiles-0.1.1/PersonalizationProfiles.egg-info/top_level.txt
-drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 19:14:14.765805 PersonalizationProfiles-0.1.1/personalization_profiles/
--rw-r--r--   0 borakaragul   (501) staff       (20)      912 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.1/personalization_profiles/AdventurousTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      804 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.1/personalization_profiles/BudgetTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      830 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.1/personalization_profiles/BusinessTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      918 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.1/personalization_profiles/EcoTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      773 2024-05-14 19:13:29.000000 PersonalizationProfiles-0.1.1/personalization_profiles/FamilyTraveler.py
--rw-r--r--   0 borakaragul   (501) staff       (20)     2489 2024-05-14 19:13:32.000000 PersonalizationProfiles-0.1.1/personalization_profiles/PersonaManager.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      167 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.1/personalization_profiles/PersonaType.py
--rw-r--r--   0 borakaragul   (501) staff       (20)     3055 2024-05-14 19:13:21.000000 PersonalizationProfiles-0.1.1/personalization_profiles/PersonalizationProfile.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      832 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.1/personalization_profiles/User.py
--rw-r--r--   0 borakaragul   (501) staff       (20)      268 2024-05-14 18:54:26.000000 PersonalizationProfiles-0.1.1/personalization_profiles/__init__.py
--rw-r--r--   0 borakaragul   (501) staff       (20)       38 2024-05-14 19:14:14.766385 PersonalizationProfiles-0.1.1/setup.cfg
--rw-r--r--   0 borakaragul   (501) staff       (20)      224 2024-05-14 19:13:50.000000 PersonalizationProfiles-0.1.1/setup.py
+drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:06:23.396512 PersonalizationProfiles-0.1.2/
+-rw-r--r--   0 borakaragul   (501) staff       (20)      130 2024-05-14 20:06:23.396315 PersonalizationProfiles-0.1.2/PKG-INFO
+drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:06:23.396122 PersonalizationProfiles-0.1.2/PersonalizationProfiles.egg-info/
+-rw-r--r--   0 borakaragul   (501) staff       (20)      130 2024-05-14 20:06:23.000000 PersonalizationProfiles-0.1.2/PersonalizationProfiles.egg-info/PKG-INFO
+-rw-r--r--   0 borakaragul   (501) staff       (20)      665 2024-05-14 20:06:23.000000 PersonalizationProfiles-0.1.2/PersonalizationProfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 borakaragul   (501) staff       (20)        1 2024-05-14 20:06:23.000000 PersonalizationProfiles-0.1.2/PersonalizationProfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 borakaragul   (501) staff       (20)       12 2024-05-14 20:06:23.000000 PersonalizationProfiles-0.1.2/PersonalizationProfiles.egg-info/requires.txt
+-rw-r--r--   0 borakaragul   (501) staff       (20)       25 2024-05-14 20:06:23.000000 PersonalizationProfiles-0.1.2/PersonalizationProfiles.egg-info/top_level.txt
+drwxr-xr-x   0 borakaragul   (501) staff       (20)        0 2024-05-14 20:06:23.395977 PersonalizationProfiles-0.1.2/personalization_profiles/
+-rw-r--r--   0 borakaragul   (501) staff       (20)      912 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.2/personalization_profiles/AdventurousTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      804 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.2/personalization_profiles/BudgetTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      830 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.2/personalization_profiles/BusinessTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      918 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.2/personalization_profiles/EcoTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      773 2024-05-14 19:13:29.000000 PersonalizationProfiles-0.1.2/personalization_profiles/FamilyTraveler.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)     2528 2024-05-14 19:30:38.000000 PersonalizationProfiles-0.1.2/personalization_profiles/PersonaManager.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      167 2024-05-13 17:31:09.000000 PersonalizationProfiles-0.1.2/personalization_profiles/PersonaType.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)     3055 2024-05-14 19:13:21.000000 PersonalizationProfiles-0.1.2/personalization_profiles/PersonalizationProfile.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)     1041 2024-05-14 19:23:23.000000 PersonalizationProfiles-0.1.2/personalization_profiles/User.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)      268 2024-05-14 18:54:26.000000 PersonalizationProfiles-0.1.2/personalization_profiles/__init__.py
+-rw-r--r--   0 borakaragul   (501) staff       (20)       38 2024-05-14 20:06:23.396551 PersonalizationProfiles-0.1.2/setup.cfg
+-rw-r--r--   0 borakaragul   (501) staff       (20)      271 2024-05-14 20:06:06.000000 PersonalizationProfiles-0.1.2/setup.py
```

### Comparing `PersonalizationProfiles-0.1.1/PersonalizationProfiles.egg-info/SOURCES.txt` & `PersonalizationProfiles-0.1.2/PersonalizationProfiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/AdventurousTraveler.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/AdventurousTraveler.py`

 * *Files identical despite different names*

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/BudgetTraveler.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/BudgetTraveler.py`

 * *Files identical despite different names*

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/BusinessTraveler.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/BusinessTraveler.py`

 * *Files identical despite different names*

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/EcoTraveler.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/EcoTraveler.py`

 * *Files identical despite different names*

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/FamilyTraveler.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/FamilyTraveler.py`

 * *Files identical despite different names*

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/PersonaManager.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/PersonaManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # number of questions used in personalization survey to determine persona
 PERSONA_SURVEY_LIMIT = 6
 
 class PersonaManager():
     def __init__(self,user_data:dict, preferences:str) -> None:
         self.user_data = user_data
         self.Persona = None
-        self.preferences = list(preferences)
+        self.preferences = list(map(lambda x:int(x),list(preferences)))
         self.get_personalization_profile()
 
     def set_persona(self) -> str:
         """
         Maps the user's travel preferences to a predefined persona.
         Possible return values are 
         "BusinessTraveler", "BudgetTraveler", "FamilyTraveler", "AdventurousTraveler", "EcoTraveler"
@@ -31,37 +31,36 @@
             [0.086, 0.25, 0.057, 0.245, 0.176],
             [0.257, 0.175, 0.287, 0.094, 0.176],
             [0.105, 0.088, 0.149, 0.094, 0.265],
             [0.257, 0.075, 0.276, 0.075, 0.118],
             [0.086, 0.225, 0.195, 0.255, 0.137]
         ])
 
-        preferences_array = np.array(self.preferences)[:PERSONA_SURVEY_LIMIT]).reshape(1, -1)
+        preferences_array = np.array(self.preferences)[:PERSONA_SURVEY_LIMIT].reshape(1, -1)
 
         # Multiply the matrices
         result = np.dot(weights.T, preferences_array.T)
         # Get the index of the maximum value
         max_index = np.argmax(result)
 
         personas = list(PersonaType)
         selected_persona = personas[max_index]
         self.persona_type = selected_persona
 
     def get_personalization_profile(self) -> None:
+        #set persona type
         self.set_persona()
-
         if self.persona_type == PersonaType.BusinessTraveler:
             self.Persona = BusinessTraveler()  
         elif self.persona_type == PersonaType.BudgetTraveler:
             self.Persona = BudgetTraveler()
         elif self.persona_type == PersonaType.FamilyTraveler:
             self.Persona = FamilyTraveler()
         elif self.persona_type == PersonaType.AdventurousTraveler:
             self.Persona = AdventurousTraveler()
         elif self.persona_type == PersonaType.EcoTraveler:
             self.Persona = EcoTraveler()
-        # record the time preferences
-        #set persona type
+        # record the time preferences and user data
         self.Persona.set_profile(self.user_data)
         self.Persona.persona_type = self.persona_type
         self.Persona.set_preferences(self.preferences)
```

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/PersonalizationProfile.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/PersonalizationProfile.py`

 * *Files identical despite different names*

### Comparing `PersonalizationProfiles-0.1.1/personalization_profiles/User.py` & `PersonalizationProfiles-0.1.2/personalization_profiles/User.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 
 class User():
-    def __init__(self, name=None) -> None:
+    def __init__(self, name=None, email=None) -> None:
         """
         Initialize a Person object.
 
         Args:
             name (str): The person's name.
             preferences (dict): The person's preferences for personalization.
             is_introduced (bool): Indicates whether the person has been introduced.
 
         Returns:
             None
         """
         self.name = name
+        self.email = email
+
 
     def set_profile(self,user_profile:dict) -> None:
         """
         Sets the user's profile information.
 
         Args:
             user_profile (dict): A dictionary containing the user's profile information.
 
         Returns:
             None
         """
         self.name = user_profile["name"]
+        self.email = user_profile["email"]
         
     def get_name(self) -> str:
         """
         Returns the name of the user.
         """
         return self.name
+    
+    def get_email(self) -> str:
+        """
+        Returns the email of the user.
+        """
+        return self.email
```

