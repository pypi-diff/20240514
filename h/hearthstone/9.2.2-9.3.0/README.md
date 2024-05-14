# Comparing `tmp/hearthstone-9.2.2.tar.gz` & `tmp/hearthstone-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-9.2.2.tar", last modified: Wed Apr 17 12:29:11 2024, max compression
+gzip compressed data, was "hearthstone-9.3.0.tar", last modified: Tue May 14 17:25:18 2024, max compression
```

## Comparing `hearthstone-9.2.2.tar` & `hearthstone-9.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:29:11.680287 hearthstone-9.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 12:28:49.000000 hearthstone-9.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-17 12:29:11.680287 hearthstone-9.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-17 12:28:49.000000 hearthstone-9.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:29:11.680287 hearthstone-9.2.2/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    61702 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:29:11.680287 hearthstone-9.2.2/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-17 12:28:49.000000 hearthstone-9.2.2/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:29:11.680287 hearthstone-9.2.2/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-17 12:29:11.000000 hearthstone-9.2.2/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-17 12:29:11.000000 hearthstone-9.2.2/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:29:11.000000 hearthstone-9.2.2/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 12:29:11.000000 hearthstone-9.2.2/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 12:29:11.000000 hearthstone-9.2.2/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:29:11.000000 hearthstone-9.2.2/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-17 12:29:11.680287 hearthstone-9.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-04-17 12:28:49.000000 hearthstone-9.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:25:18.606054 hearthstone-9.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-14 17:25:14.000000 hearthstone-9.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-14 17:25:18.606054 hearthstone-9.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-14 17:25:14.000000 hearthstone-9.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:25:18.606054 hearthstone-9.3.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61836 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:25:18.606054 hearthstone-9.3.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16605 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-14 17:25:14.000000 hearthstone-9.3.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:25:18.606054 hearthstone-9.3.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-14 17:25:18.000000 hearthstone-9.3.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-14 17:25:18.000000 hearthstone-9.3.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:25:18.000000 hearthstone-9.3.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 17:25:18.000000 hearthstone-9.3.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 17:25:18.000000 hearthstone-9.3.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:25:18.000000 hearthstone-9.3.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-14 17:25:18.606054 hearthstone-9.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       62 2024-05-14 17:25:14.000000 hearthstone-9.3.0/setup.py
```

### Comparing `hearthstone-9.2.2/LICENSE` & `hearthstone-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/PKG-INFO` & `hearthstone-9.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.2.2
+Version: 9.3.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-9.2.2/README.md` & `hearthstone-9.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/bountyxml.py` & `hearthstone-9.3.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/cardxml.py` & `hearthstone-9.3.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/dbf.py` & `hearthstone-9.3.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/deckstrings.py` & `hearthstone-9.3.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/entities.py` & `hearthstone-9.3.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/enums.py` & `hearthstone-9.3.0/hearthstone/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -852,18 +852,21 @@
 	MINIATURIZE = 3318
 	MINI = 3319
 	BACON_PASS_TOOLTIP = 3321
 	MAX_EXCAVATE_TIER = 3326
 	PALADIN_AURA = 3374
 	ZILLIAX_CUSTOMIZABLE_COSMETICMODULE = 3376
 	ZILLIAX_CUSTOMIZABLE_FUNCTIONALMODULE = 3377
+	GIGANTIFY = 3399
+	GIGANTIC = 3400
 	BACON_COMBAT_DAMAGE_CAP_ENABLED = 3403
 	SIDEBOARD_TYPE = 3427
 	CREATED_BY_TWINSPELL = 3432
 	CREATED_BY_MINIATURIZE = 3433
+	CREATED_BY_GIGANTIFY = 3434
 	SUPPRESS_HERO_STANDARD_SUMMON_FX = 3438
 	ZILLIAX_CUSTOMIZABLE_LINKED_COSMETICMOUDLE = 3450
 	MIN_SIDEBOARD_CARDS = 3459
 	FORGETFUL_ATTACK_VISUAL = 3460
 	SHUDDERWOCKHIGHLIGHTHINT = 3463
 	HERO_FRAME_TYPE = 3495
 	NUM_TURNS_LAST_AFFECTED_BY = 3464
@@ -872,18 +875,21 @@
 	HIDE_HEALTH_NUMBER = 3471
 	HIDE_ATTACK_NUMBER = 3472
 	ZILLIAX_CUSTOMIZABLE_SAVED_VERSION = 3477
 	DUOS_QUEUED_NOT_ON_TEAM = 3478
 	PLAYER_ABANDONED_BY_TEAMMATE = 3480
 	SUPPRESS_MILL_ANIMATION = 3481
 	IGNORE_SUPPRESS_MILL_ANIMATION = 3482
+	HERO_PASSIVE_ID = 3487
 	BACON_TEAMMATE_BONUS_MINION_DAMAGE_LAST_COMBAT = 3492
 	BACON_DUOS_PUNISH_LEAVERS = 3494
 	BACON_TRIPLED_BASE_MINION_ID2 = 3499
 	BACON_TRIPLED_BASE_MINION_ID3 = 3500
+	QUEST_HIDE_PROGRESS = 3523
+	TRANSFORM = 3562
 
 	InvisibleDeathrattle = 335
 	ImmuneToSpellpower = 349
 	AttackVisualType = 251
 	DevState = 268
 	GrantCharge = 355
 	HealTarget = 361
```

### Comparing `hearthstone-9.2.2/hearthstone/mercenaryxml.py` & `hearthstone-9.3.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/stringsfile.py` & `hearthstone-9.3.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/utils/__init__.py` & `hearthstone-9.3.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone/xmlutils.py` & `hearthstone-9.3.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/hearthstone.egg-info/PKG-INFO` & `hearthstone-9.3.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 9.2.2
+Version: 9.3.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-9.2.2/hearthstone.egg-info/SOURCES.txt` & `hearthstone-9.3.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-9.2.2/setup.cfg` & `hearthstone-9.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 9.2.2
+version = 9.3.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

