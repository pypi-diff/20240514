# Comparing `tmp/opgg_py-1.3.0.tar.gz` & `tmp/opgg_py-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opgg_py-1.3.0.tar", last modified: Mon Apr 29 06:36:35 2024, max compression
+gzip compressed data, was "opgg_py-1.3.1.tar", last modified: Tue May 14 15:26:00 2024, max compression
```

## Comparing `opgg_py-1.3.0.tar` & `opgg_py-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:36:35.434543 opgg_py-1.3.0/
--rw-rw-rw-   0        0        0     1524 2023-08-25 15:24:47.000000 opgg_py-1.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     6480 2024-04-29 06:36:35.434038 opgg_py-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5429 2023-09-26 00:09:10.000000 opgg_py-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 06:36:35.415382 opgg_py-1.3.0/opgg/
--rw-rw-rw-   0        0        0      314 2023-08-31 16:10:36.000000 opgg_py-1.3.0/opgg/__init__.py
--rw-rw-rw-   0        0        0    22867 2024-04-28 16:30:30.000000 opgg_py-1.3.0/opgg/cacher.py
--rw-rw-rw-   0        0        0    18303 2023-08-30 17:43:35.000000 opgg_py-1.3.0/opgg/champion.py
--rw-rw-rw-   0        0        0     5628 2024-04-29 06:02:42.000000 opgg_py-1.3.0/opgg/game.py
--rw-rw-rw-   0        0        0     8734 2024-04-29 05:56:35.000000 opgg_py-1.3.0/opgg/league_stats.py
--rw-rw-rw-   0        0        0    32932 2024-04-29 06:00:39.000000 opgg_py-1.3.0/opgg/opgg.py
--rw-rw-rw-   0        0        0     1464 2023-08-27 16:37:13.000000 opgg_py-1.3.0/opgg/params.py
--rw-rw-rw-   0        0        0     2978 2023-08-27 16:37:23.000000 opgg_py-1.3.0/opgg/season.py
--rw-rw-rw-   0        0        0    10351 2024-04-29 05:46:09.000000 opgg_py-1.3.0/opgg/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:36:35.433032 opgg_py-1.3.0/opgg.py.egg-info/
--rw-rw-rw-   0        0        0     6480 2024-04-29 06:36:35.000000 opgg_py-1.3.0/opgg.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-04-29 06:36:35.000000 opgg_py-1.3.0/opgg.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:36:35.000000 opgg_py-1.3.0/opgg.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-29 06:36:35.000000 opgg_py-1.3.0/opgg.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-29 06:36:35.000000 opgg_py-1.3.0/opgg.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-29 06:36:35.440661 opgg_py-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1649 2024-04-29 06:34:54.000000 opgg_py-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:26:00.162725 opgg_py-1.3.1/
+-rw-rw-rw-   0        0        0     1524 2023-08-25 15:24:47.000000 opgg_py-1.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     6480 2024-05-14 15:26:00.161718 opgg_py-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5429 2023-09-26 00:09:10.000000 opgg_py-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 15:26:00.142727 opgg_py-1.3.1/opgg/
+-rw-rw-rw-   0        0        0      314 2023-08-31 16:10:36.000000 opgg_py-1.3.1/opgg/__init__.py
+-rw-rw-rw-   0        0        0    22867 2024-04-28 16:30:30.000000 opgg_py-1.3.1/opgg/cacher.py
+-rw-rw-rw-   0        0        0    18303 2023-08-30 17:43:35.000000 opgg_py-1.3.1/opgg/champion.py
+-rw-rw-rw-   0        0        0     5628 2024-04-29 06:02:42.000000 opgg_py-1.3.1/opgg/game.py
+-rw-rw-rw-   0        0        0     8734 2024-04-29 05:56:35.000000 opgg_py-1.3.1/opgg/league_stats.py
+-rw-rw-rw-   0        0        0    33908 2024-05-14 15:18:15.000000 opgg_py-1.3.1/opgg/opgg.py
+-rw-rw-rw-   0        0        0     1464 2023-08-27 16:37:13.000000 opgg_py-1.3.1/opgg/params.py
+-rw-rw-rw-   0        0        0     2978 2023-08-27 16:37:23.000000 opgg_py-1.3.1/opgg/season.py
+-rw-rw-rw-   0        0        0    10351 2024-04-29 05:46:09.000000 opgg_py-1.3.1/opgg/summoner.py
+drwxrwxrwx   0        0        0        0 2024-05-14 15:26:00.160678 opgg_py-1.3.1/opgg.py.egg-info/
+-rw-rw-rw-   0        0        0     6480 2024-05-14 15:26:00.000000 opgg_py-1.3.1/opgg.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-14 15:26:00.000000 opgg_py-1.3.1/opgg.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 15:26:00.000000 opgg_py-1.3.1/opgg.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-14 15:26:00.000000 opgg_py-1.3.1/opgg.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-14 15:26:00.000000 opgg_py-1.3.1/opgg.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-14 15:26:00.163896 opgg_py-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2024-05-14 15:24:43.000000 opgg_py-1.3.1/setup.py
```

### Comparing `opgg_py-1.3.0/LICENSE.txt` & `opgg_py-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/PKG-INFO` & `opgg_py-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opgg.py
-Version: 1.3.0
+Version: 1.3.1
 Summary: An unofficial Python library for scraping/accessing data from OP.GG
 Home-page: https://github.com/ShoobyDoo/OPGG.py
 Author: ShoobyDoo
 Project-URL: Bug Reports, https://github.com/ShoobyDoo/OPGG.py/issues
 Project-URL: Source, https://github.com/ShoobyDoo/OPGG.py
 Keywords: opgg,league-of-legends,web-scraping,summoner,data,riot-api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `opgg_py-1.3.0/README.md` & `opgg_py-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg/cacher.py` & `opgg_py-1.3.1/opgg/cacher.py`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg/champion.py` & `opgg_py-1.3.1/opgg/champion.py`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg/game.py` & `opgg_py-1.3.1/opgg/game.py`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg/league_stats.py` & `opgg_py-1.3.1/opgg/league_stats.py`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg/opgg.py` & `opgg_py-1.3.1/opgg/opgg.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,31 +54,31 @@
         }
         self._all_champions = None
         self._all_seasons = None
 
         # ===== SETUP START =====
         logging.root.name = 'OPGG.py'
 
-        logging.basicConfig(
-            filename=f'./logs/opgg_{datetime.now().strftime("%Y-%m-%d")}.log',
-            filemode='a+', 
-            format='[%(asctime)s][%(name)-22s][%(levelname)-7s] : %(message)s', 
-            datefmt='%d-%b-%y %H:%M:%S',
-            level=logging.INFO
-        )
-
         if not os.path.exists('./logs'):
             logging.info("Creating logs directory...")
             os.mkdir('./logs')
         else:
             # remove empty log files
             for file in os.listdir('./logs'):
                 if os.stat(f"./logs/{file}").st_size == 0 and file != f'opgg_{datetime.now().strftime("%Y-%m-%d")}.log':
                     logging.info(f"Removing empty log file: {file}")
                     os.remove(f"./logs/{file}")
+                    
+        logging.basicConfig(
+            filename=f'./logs/opgg_{datetime.now().strftime("%Y-%m-%d")}.log',
+            filemode='a+', 
+            format='[%(asctime)s][%(name)-22s][%(levelname)-7s] : %(message)s', 
+            datefmt='%d-%b-%y %H:%M:%S',
+            level=logging.INFO
+        )
         # ===== SETUP END =====
         
         # allow the user to interact with the logger
         self._logger = logging.getLogger("OPGG.py")        
         
         # at object creation, setup and query the cache
         self._cacher = Cacher()
@@ -359,15 +359,15 @@
     
     def search(self, summoner_names: str | list[str], region = Region.NA) -> Summoner | list[Summoner] | str:
         """
         Search for a single or multiple summoner(s) on OPGG.
 
         ### Args:
             summoner_names : `str` | `list[str]`
-                Pass either a `str` (comma seperated) or `list[str]` of summoner names.
+                Pass either a `str` (comma seperated) or `list[str]` of summoner names + regional identifier (#NA1, #EUW, etc).
                 
             region : `Region, optional`
                 Pass the region you want to search in. Defaults to "NA".
 
         ### Returns:
             `list[Summoner]` | `str` : A single or list of Summoner objects, or a string if no summoner(s) were found.
         """
@@ -382,15 +382,18 @@
         #   -> If found, add to list of cached summoner ids, and below iterate over and set the summoner id property
         #   -> As an extension of the above, these requests would go directly to the api to pull summary/full data
         #   -> If not found, add to list of summoner names to query
         # 2. Build the summoner objects accordingly
         cached_summoner_ids = []
         uncached_summoners = []
         
+        # TODO: Cache get/set logic needs to be reworked to account for regional identifiers. Currently, you could have 2 of the same users on different regions and the cache will just return whatever the first entry that was cached would've been. This is not ideal, perhaps I should force people to append the regional identifiers? This would result in unique entries in the cache...
         for summoner_name in summoner_names:
+            if ('#' not in summoner_name):
+                raise Exception(f"No regional identifier was found for query: \"{summoner_name}\". Please include the identifier as well and try again. (#NA1, #EUW, etc.)")
             cached_id = self.cacher.get_summoner_id(summoner_name)
             if cached_id:
                 cached_summoner_ids.append(cached_id)
             else:
                 uncached_summoners.append(summoner_name)
         
         # pass only uncached summoners to get_page_props()
@@ -431,21 +434,26 @@
         
         # bit of weirdness around generic usernames. If you pass "abc" for example, it will return multiple summoners in the page props.
         # To help, we will check against opgg's "internal_name" property, which seems to be the username.lower() with spaces removed.        
         summoners = []
         for summoner_name in summoner_names:
             # if there are multiple search results for a SINGLE summoner_name, query MUST include the regional identifier
             if (len(page_props["summoners"]) > 1 and '#' in summoner_name):
+                logging.debug(f"MULTI-RESULT | page_props->summoners: {page_props['summoners']}")
                 only_summoner_name, only_region = summoner_name.split("#")
                 for summoner in page_props["summoners"]:
                     if (only_summoner_name.strip() == summoner["game_name"] and only_region.strip() == summoner["tagline"]):
                         self.summoner_id = summoner["summoner_id"]
                         break
-            else:
+            
+            elif (len(page_props["summoners"]) > 1 and '#' not in summoner_name):
                 raise Exception(f"Multiple search results were returned for \"{summoner_name}\". Please include the identifier as well and try again. (#NA1, #EUW, etc.)")
+
+            elif (len(page_props["summoners"]) == 1):
+                self.summoner_id = page_props["summoners"][0]["summoner_id"]
             
             summoner = self.get_summoner()
             summoners.append(summoner)
             self.logger.info(f"Summoner object built for: {summoner.name} ({summoner.summoner_id}), caching...")
             self.cacher.insert_summoner(summoner.name, summoner.summoner_id)
             
         # cached summoners go straight to api
```

### Comparing `opgg_py-1.3.0/opgg/params.py` & `opgg_py-1.3.1/opgg/params.py`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg/season.py` & `opgg_py-1.3.1/opgg/season.py`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg/summoner.py` & `opgg_py-1.3.1/opgg/summoner.py`

 * *Files identical despite different names*

### Comparing `opgg_py-1.3.0/opgg.py.egg-info/PKG-INFO` & `opgg_py-1.3.1/opgg.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opgg.py
-Version: 1.3.0
+Version: 1.3.1
 Summary: An unofficial Python library for scraping/accessing data from OP.GG
 Home-page: https://github.com/ShoobyDoo/OPGG.py
 Author: ShoobyDoo
 Project-URL: Bug Reports, https://github.com/ShoobyDoo/OPGG.py/issues
 Project-URL: Source, https://github.com/ShoobyDoo/OPGG.py
 Keywords: opgg,league-of-legends,web-scraping,summoner,data,riot-api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `opgg_py-1.3.0/setup.py` & `opgg_py-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name="opgg.py",
-    version="1.3.0",
+    version="1.3.1",
     description="An unofficial Python library for scraping/accessing data from OP.GG",  # Optional
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ShoobyDoo/OPGG.py",
     # This should be your name or the name of the organization which owns the
     # project.
     author="ShoobyDoo",
```

