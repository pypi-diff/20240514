# Comparing `tmp/malfetcher-1.0.0a0.tar.gz` & `tmp/malfetcher-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malfetcher-1.0.0a0.tar", last modified: Sat Apr 20 08:29:17 2024, max compression
+gzip compressed data, was "malfetcher-1.1.0.tar", last modified: Tue May 14 12:09:59 2024, max compression
```

## Comparing `malfetcher-1.0.0a0.tar` & `malfetcher-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/malfetcher/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/mal_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/mal_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/malfetcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/malfetcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 08:29:17.000000 malfetcher-1.0.0a0/malfetcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:29:17.409688 malfetcher-1.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 08:29:08.000000 malfetcher-1.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:59.953037 malfetcher-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-14 12:09:51.000000 malfetcher-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-14 12:09:59.953037 malfetcher-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-14 12:09:51.000000 malfetcher-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:59.953037 malfetcher-1.1.0/malfetcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/mal_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/mal_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 12:09:51.000000 malfetcher-1.1.0/malfetcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:09:59.953037 malfetcher-1.1.0/malfetcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 12:09:59.000000 malfetcher-1.1.0/malfetcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 12:09:51.000000 malfetcher-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:09:59.953037 malfetcher-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-14 12:09:51.000000 malfetcher-1.1.0/setup.py
```

### Comparing `malfetcher-1.0.0a0/LICENSE` & `malfetcher-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malfetcher-1.0.0a0/malfetcher/mal_fetcher.py` & `malfetcher-1.1.0/malfetcher/mal_fetcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 import requests, time, os, copy, math
 from datetime import datetime, timedelta
 from .utils import utils_save_json, utils_read_json
-from .mal_config_utils import config_setup
+from .mal_config_utils import config_setup, regenerate_token
 
-total_user = {}
-user_entries = {}
 script_path = os.path.dirname(os.path.abspath(__file__))
 myanimelist_id_cache_path = os.path.join(script_path, 'cache', 'myanimelist_id_cache.json')
 myanimelist_search_cache_path = os.path.join(script_path, 'cache', 'myanimelist_search_cache.json')
 config_path = os.path.join(script_path, 'config', 'config.json')
-anime_request_url = 'https://api.myanimelist.net/v2/anime'
+anime_request_url = "https://api.myanimelist.net/v2/anime"
 
 al_to_mal_user_status = {
-    'CURRENT': 'watching',
-    'COMPLETED': 'completed',
-    'PAUSED': 'on_hold',
-    'DROPPED': 'dropped',
-    'PLANNING': 'plan_to_watch'
+    'CURRENT': "watching",
+    'COMPLETED': "completed",
+    'PAUSED': "on_hold",
+    'DROPPED': "dropped",
+    'PLANNING': "plan_to_watch"
 }
 
 mal_to_al_user_status = {v:k for k, v in al_to_mal_user_status.items()}
 
 al_to_mal_status = {
-    'FINISHED': 'finished_airing',
-    'RELEASING': 'currently_airing',
-    'NOT_YET_RELEASED': 'not_yet_aired'
+    'FINISHED': "finished_airing",
+    'RELEASING': "currently_airing",
+    'NOT_YET_RELEASED': "not_yet_aired"
 }
 
 mal_to_al_status = {v:k for k, v in al_to_mal_status.items()}
-skip_user_statuses = ['REPEATING']
+skip_user_statuses = ["REPEATING"]
+
+# Minimal user setup to interact with MyAnimeList API
+config = utils_read_json(config_path)
+if not config or 'myanimelist_client_id' not in config:
+    client_id = input("Please input your MyAnimeList API Client ID.\nhttps://myanimelist.net/apiconfig\n")
+    config['myanimelist_client_id'] = client_id
+    utils_save_json(config_path, config)
+else:
+    client_id = config['myanimelist_client_id']
 
 # Utils
 
 def clear_cache():
     config = utils_read_json(config_path)
     try:
-        del config['checked_date']
+        del config["checked_date"]
     except:
         pass
     os.remove(myanimelist_id_cache_path)
     os.remove(myanimelist_search_cache_path)
 
 def check_status_in_cache():
     og_cache = utils_read_json(myanimelist_id_cache_path)
@@ -59,33 +66,29 @@
                 release_date = datetime.strptime(cache[anime]['release_date'], '%Y-%m-%d').date()
             except:
                 release_date = None
             try:
                 end_date = datetime.strptime(cache[anime]['end_date'], '%Y-%m-%d').date()
             except:
                 end_date = None
-            if not release_date:
-                continue
             status = cache[anime]['status']
-            if status == 'RELEASING':
+            if status == "NOT_YET_RELEASED":
+                cache.update(get_anime_info(anime, True)) #force update everytime
+            elif status == "RELEASING" and release_date:
                     try:
                         next_ep_date = release_date + timedelta(cache[anime]['upcoming_ep'] * 7)
                         if end_date and current_date > end_date:
                             updated_info = get_anime_info(anime, True)
                             cache.update(updated_info)
                         if current_date > next_ep_date:
                             updated_info = get_anime_info(anime, True)
                             cache.update(updated_info)
                     except: #force update if we don't have the next episode
                         updated_info = get_anime_info(anime, True)
                         cache.update(updated_info)
-            elif status == 'NOT_YET_RELEASED':
-                if release_date:
-                    if current_date > release_date:
-                        cache.update(get_anime_info(anime, True))
         config_dict['checked_date'] = current_date.strftime('%Y-%m-%d')
         utils_save_json(config_path, config_dict)
         utils_save_json(myanimelist_id_cache_path, cache, True)
 
 def load_cache():
     check_status_in_cache()
     return utils_read_json(myanimelist_id_cache_path)
@@ -95,160 +98,164 @@
     try:
         return config['myanimelist_user_token']
     except:
         return config_setup()['myanimelist_user_token']
 
 # Functions
 
-def make_graphql_request(myanimelist_api_url, params, myanimelist_token=None):
-    if myanimelist_token:
-        pass
-    elif 'myanimelist_key' in os.environ:
-        myanimelist_token = os.getenv('myanimelist_key')
-        if not os.path.exists(config_path):
-            os.makedirs(os.path.dirname(config_path))
+def make_graphql_request(myanimelist_api_url, params, method='get', myanimelist_token=None, user_request = False):
+    local_token = False
+    if user_request:
+        if myanimelist_token:
+            pass
+        elif 'myanimelist_key' in os.environ:
+            myanimelist_token = os.getenv('myanimelist_key')
+            if not os.path.exists(config_path):
+                os.makedirs(os.path.dirname(config_path))
+        else:
+            myanimelist_token = load_config()
+            local_token = True
+        HEADERS = {'Authorization': f"Bearer {myanimelist_token}"}
     else:
-        myanimelist_token = load_config()
-
-    # Constants for GraphQL endpoint and headers
-    HEADERS = {'Authorization': f'Bearer {myanimelist_token}'}
+        HEADERS = {'X-MAL-CLIENT-ID': f"{client_id}"}
 
     def make_request():
-        response = requests.get(myanimelist_api_url, params=params, headers=HEADERS)
+        request_func = getattr(requests, method.lower(), None)
+        if method.lower() == 'put':
+           response = request_func(myanimelist_api_url, data=params, headers=HEADERS)
+        else: 
+            response = request_func(myanimelist_api_url, params=params, headers=HEADERS)    
         return response
 
     retries = 0
     while True:
         response = make_request()
         if response.status_code == 200:
             json_response = response.json()
             if 'data' in json_response:
                 return json_response['data']
             return json_response
         elif response.status_code == 429:
             print(f"Rate limit exceeded. Waiting before retrying...")
-            print(params, HEADERS, sep='\n')
+            print(params, HEADERS, sep="\n")
             print(response.json())
             retry_after = int(response.headers.get('retry-after', 1))
             time.sleep(retry_after)
             retries += 1
         elif response.status_code == 500 or response.status_code == 400:
-            print(f"Unknown error occured, retrying...")
-            print(params, HEADERS, sep='\n')
+            print(f"Unknown error occurred, retrying...")
+            print(params, HEADERS, sep="\n")
             print(response.json())
             retries += 1
         elif response.status_code == 404:
             print(f"Anime not found")
             return None
+        elif response.status_code == 401 and local_token:
+            print(f"Access token expired, refreshing")
+            regenerate_token()
+            retries += 1
         else:
             print(f"Error {response.status_code}: {params}")
             return {}
 
         # Exponential backoff with a maximum of 5 retries
         if retries >= 5:
             print("Maximum retries reached. Exiting.")
             return {}
                 
         print(f"Retrying... (Attempt {retries})")
 
-def get_latest_anime_entry_for_user(status = 'ALL', myanimelist_token=None,  username = None):
+def get_latest_anime_entry_for_user(status = "ALL", myanimelist_token=None,  username = None):
     if not username:
         username = get_userdata(myanimelist_token)[0]
+        user_request = True
+    else:
+        user_request = False
+
     status = status.upper()
-    status_options = ['CURRENT', 'PLANNING', 'COMPLETED', 'DROPPED', 'PAUSED', 'REPEATING']
+    status_options = ["CURRENT", "PLANNING", "COMPLETED", "DROPPED", "PAUSED", "REPEATING"]
     params = {}
     params['sort'] = 'anime_start_date'
     params['fields'] = (
-        'id,'
-        'title,'
-        'alternative_titles,'
-        'start_date,'
-        'end_date,'
-        'nsfw,'
-        'media_type,'
-        'status,'
-        'genres,'
-        'my_list_status,'
-        'num_episodes,'
-        'related_anime'
+        "id,"
+        "title,"
+        "alternative_titles,"
+        "start_date,"
+        "end_date,"
+        "nsfw,"
+        "media_type,"
+        "status,"
+        "genres,"
+        "my_list_status,"
+        "num_episodes,"
+        "related_anime"
     )
     params['limit'] = 1
-    if status != 'ALL':
+    if status != "ALL":
         if not status in status_options:
-            print("Invalid status option. Allowed options are:", ', '.join(str(option) for option in status_options) )
+            print("Invalid status option. Allowed options are:", ", ".join(str(option) for option in status_options) )
             return
         if status in skip_user_statuses:
             return
         params['status'] = al_to_mal_user_status[status]
 
-    request_url = f'https://api.myanimelist.net/v2/users/{username}/animelist'
-    data = make_graphql_request(request_url, params, myanimelist_token)
+    request_url = f"https://api.myanimelist.net/v2/users/{username}/animelist"
+    data = make_graphql_request(request_url, params, myanimelist_token = myanimelist_token, user_request = user_request)
 
-    if not username in user_entries:
-        user_entries[username] = {}
-        
     if data:
         anime = data[0]['node']
         anime_id = str(anime['id'])
         anime_info = generate_anime_entry(anime, myanimelist_token)
         user_entry = {}    # Initialize as a dictionary if not already initialized
         user_entry[anime_id] = {}    # Initialize as a dictionary if not already initialized
         user_entry[anime_id].update(anime_info)
         try:
             user_entry[anime_id]['watched_ep'] = anime['my_list_status']['num_episodes_watched']
             user_entry[anime_id]['watching_status'] = mal_to_al_user_status[anime['my_list_status']['status']]
         except:
             pass
-        user_entries[username][anime_id] = user_entry
         return user_entry
 
-    print(f"No entries found for {username}'s planned anime list.")
+    print(f"No entries found for {username}'s {status.lower()} anime list.")
     return None
 
-def get_all_anime_for_user(status_list='ALL', myanimelist_token=None, username = None):
+def get_all_anime_for_user(status_list="ALL", myanimelist_token=None, username = None):
     if not username:
         username = get_userdata(myanimelist_token)[0]
+        user_request = True
+    else:
+        user_request = False
+        
     def main_function(status):
         status = status.upper()
-        status_options = ['CURRENT', 'PLANNING', 'COMPLETED', 'DROPPED', 'PAUSED', 'REPEATING']
+        status_options = ["CURRENT", "PLANNING", "COMPLETED", "DROPPED", "PAUSED", "REPEATING"]
         params = {}
-        params['sort'] = 'anime_start_date'
+        params['sort'] = "anime_start_date"
         params['fields'] = (
-            'id,'
-            'title,'
-            'alternative_titles,'
-            'start_date,'
-            'end_date,'
-            'nsfw,'
-            'media_type,'
-            'status,'
-            'genres,'
-            'my_list_status,'
-            'num_episodes,'
-            'related_anime'
+            "id,"
+            "title,"
+            "alternative_titles,"
+            "start_date,"
+            "end_date,"
+            "nsfw,"
+            "media_type,"
+            "status,"
+            "genres,"
+            "my_list_status,"
+            "num_episodes,"
+            "related_anime"
         )
-        if status != 'ALL':
+        if status != "ALL":
             if not status in status_options:
-                print("Invalid status option. Allowed options are:", ', '.join(str(option) for option in status_options) )
-                return
-            if status in skip_user_statuses:
+                print("Invalid status option. Allowed options are:", ", ".join(str(option) for option in status_options) )
                 return
             params['status'] = al_to_mal_user_status[status]
 
-        request_url = f'https://api.myanimelist.net/v2/users/{username}/animelist'
-        data = make_graphql_request(request_url, params, myanimelist_token)
-
-        if not username in user_entries:
-            user_entries[username] = {}
-
-        if not username in total_user:
-            total_user[username] = {}
-
-        if not status in user_entries[username]:
-            user_entries[username][status] = {}
+        request_url = f"https://api.myanimelist.net/v2/users/{username}/animelist"
+        data = make_graphql_request(request_url, params, myanimelist_token = myanimelist_token, user_request = user_request)
 
         user_ids = {}
             
         if data:
             for anime_entry in data:
                 anime_entry_data = anime_entry['node']
                 anime_id = anime_entry_data['id']
@@ -258,71 +265,67 @@
                     user_ids[anime_id] = {}    # Initialize as a dictionary if not already initialized
                 user_ids[anime_id].update(anime_info)
                 try:
                     user_ids[anime_id]['watched_ep'] = anime_entry_data['my_list_status']['num_episodes_watched']
                     user_ids[anime_id]['watching_status'] = mal_to_al_user_status[anime_entry_data['my_list_status']['status']]
                 except:
                     pass
-            user_entries[username][status].update(user_ids)
-            return
-        print(f"No entries found for {username}'s planned anime list.")
+            return user_ids
+        print(f"No entries found for {username}'s {status.lower()} anime list.")
         return None    
 
     if isinstance(status_list, str):
         status_list = status_list.upper()
         main_function(status_list)
-        return user_entries[username][status_list]
+        return main_function(status_list)
     elif len(status_list) == 1:
-        status_list = status_list[0].upper()
-        main_function(status_list)
-        return user_entries[username][status_list]
+        status = status_list[0].upper()
+        if status in skip_user_statuses:
+            return
+        main_function(status)
+        return main_function(status_list)
     elif isinstance(status_list, list):
+        ani_list = {}
         for status in status_list:
+            if status in skip_user_statuses:
+                continue
             status.upper()
-            main_function(status)
-            total_user[username].update(user_entries[username][status])
-        return total_user[username]
+            ani_list.update(main_function(status))
+        return ani_list
 
 def get_anime_entry_for_user(myanimelist_id, myanimelist_token=None):
     myanimelist_id = str(myanimelist_id)
-    username = get_userdata(myanimelist_token)[0]
-    try:
-        if myanimelist_id in user_entries[username]['ALL']:
-                    return {myanimelist_id: user_entries[username]['ALL'][myanimelist_id]}
-    except KeyError:
-        params = {}
-        params['fields'] = (
-        'id,'
-        'title,'
-        'alternative_titles,'
-        'start_date,'
-        'end_date,'
-        'nsfw,'
-        'media_type,'
-        'status,'
-        'genres,'
-        'my_list_status,'
-        'num_episodes,'
-        'related_anime'
-        )
-        request_url = f'{anime_request_url}/{myanimelist_id}'
-        data = make_graphql_request(request_url, params, myanimelist_token)
-        anime_data = {}
-        if data:
-            anime_id = str(data['id'])
-            anime_data[anime_id] = {}
-            anime_data[anime_id].update(generate_anime_entry(data, myanimelist_token))
-            anime_data[anime_id]['watched_ep'] = data['my_list_status']['num_episodes_watched']
-            anime_data[anime_id]['watching_status'] = mal_to_al_user_status[data['my_list_status']['status']]
-            return anime_data
-    return None
 
-def reset_user_cache(username):
-    user_entries[username] = {}
-    total_user[username] = {}
+    params = {}
+    params['fields'] = (
+        "id,"
+        "title,"
+        "alternative_titles,"
+        "start_date,"
+        "end_date,"
+        "nsfw,"
+        "media_type,"
+        "status,"
+        "genres,"
+        "my_list_status,"
+        "num_episodes,"
+        "related_anime"
+    )
+    request_url = f"{anime_request_url}/{myanimelist_id}"
+    data = make_graphql_request(request_url, params, myanimelist_token = myanimelist_token, user_request=True)
+    anime_data = {}
+    if data:
+        anime_id = str(data['id'])
+        if 'my_list_status' not in data:
+            return None
+        anime_data[anime_id] = generate_anime_entry(data, myanimelist_token)
+        anime_data[anime_id]['watched_ep'] = data['my_list_status']['num_episodes_watched']
+        anime_data[anime_id]['watching_status'] = mal_to_al_user_status[data['my_list_status']['status']]
+        return anime_data
+    return None
 
 def get_anime_info(anime_id, force_update = False, myanimelist_token=None):
     if force_update:
         anime_cache = {}
     else:
         anime_cache = load_cache()
     anime_id = str(anime_id)
@@ -343,55 +346,55 @@
             return fetch_from_myanimelist()
     except TypeError:
         return fetch_from_myanimelist()
 
 def myanimelist_fetch_anime_info(myanimelist_id, myanimelist_token=None):
     params = {
         'fields': (
-            'id,'
-            'title,'
-            'alternative_titles,'
-            'start_date,'
-            'end_date,'
-            'nsfw,'
-            'media_type,'
-            'status,'
-            'genres,'
-            'my_list_status,'
-            'num_episodes,'
-            'related_anime'
+            "id,"
+            "title,"
+            "alternative_titles,"
+            "start_date,"
+            "end_date,"
+            "nsfw,"
+            "media_type,"
+            "status,"
+            "genres,"
+            "my_list_status,"
+            "num_episodes,"
+            "related_anime"
         )
     }
     
     request_url = f'{anime_request_url}/{myanimelist_id}'
-    data = make_graphql_request(request_url, params, myanimelist_token)
+    data = make_graphql_request(request_url, params, myanimelist_token = myanimelist_token)
     anime_data = {}
     if data:
         anime_id = str(data['id'])
         anime_data[anime_id] = {}
         anime_data[anime_id].update(generate_anime_entry(data, myanimelist_token))
     return anime_data
 
 def generate_anime_entry(anime_info, myanimelist_token):
     def getRelated():
         def get_additional_info(relation_id):
             params = {
-                'fields': 'status, related_anime'
+                'fields': "status, related_anime"
             }
-            data = make_graphql_request(anime_request_url + f'/{relation_id}', params, myanimelist_token)
+            data = make_graphql_request(anime_request_url + f"/{relation_id}", params, myanimelist_token = myanimelist_token)
             return data            
         
         relations = {}
         try:
             edges = anime_info['related_anime']
         except:
             edges = get_additional_info(anime_info['id'])['related_anime']
         for edge in edges:
             relation_type = edge['relation_type'].upper()
-            if relation_type == 'PREQUEL' or relation_type == 'SEQUEL':
+            if relation_type == "PREQUEL" or relation_type == "SEQUEL":
                 relation_id = str(edge['node']['id'])
                 relations[relation_id] = {}
                 relations[relation_id]['main_title'] = edge['node']['title']
                 relations[relation_id]['status'] = mal_to_al_status[get_additional_info(relation_id)['status']]
                 relations[relation_id]['type'] = relation_type
         if not relations:
             relations = None
@@ -408,29 +411,41 @@
 
     def generate_upcoming_ep(release_date):
             current_date = datetime.now().date()
             release_date = datetime.strptime(release_date, '%Y-%m-%d').date()
             upcoming_ep = math.ceil(int((current_date - release_date).days)/7) + 1
             return upcoming_ep
 
+    def ensure_day_in_date(date_str):
+        try:
+            datetime.strptime(date_str, '%Y-%m-%d')
+            return date_str
+        except ValueError:
+            try:
+                year_month = datetime.strptime(date_str, '%Y-%m')
+                full_date = year_month.replace(day=1)
+                return full_date.strftime('%Y-%m-%d')
+            except ValueError:
+                return None
+
     anime_id = str(anime_info['id'])
     anime_data = {}
     anime_data['al_id'] = mal_to_al_id(anime_id)
     anime_data['total_eps'] = anime_info['num_episodes']
     anime_data['is_sus'] = is_sus(anime_info)
     anime_data['main_title'] = anime_info['title']
     anime_data['synonyms'] = [
             anime_info['alternative_titles']['ja'],
             anime_info['alternative_titles']['en'],
     ] + anime_info['alternative_titles']['synonyms']
     anime_data['synonyms'] = [item for item in anime_data['synonyms'] if item is not None]    
     anime_data['status'] = mal_to_al_status[anime_info['status']]
-    anime_data['release_date'] = anime_info['start_date'] if 'start_date' in anime_info else None
-    anime_data['end_date'] = anime_info['end_date'] if 'end_date' in anime_info else None
-    anime_data['upcoming_ep'] = generate_upcoming_ep(anime_data['release_date']) if anime_data['status'] == 'RELEASING' else None
+    anime_data['release_date'] = ensure_day_in_date(anime_info['start_date']) if 'start_date' in anime_info else None
+    anime_data['end_date'] = ensure_day_in_date(anime_info['end_date']) if 'end_date' in anime_info else None
+    anime_data['upcoming_ep'] = generate_upcoming_ep(anime_data['release_date']) if anime_data['status'] == "RELEASING" else None
     anime_data['format'] = anime_info['media_type'].upper()
     anime_data['related'] = getRelated()
     utils_save_json(myanimelist_id_cache_path, {anime_id: anime_data}, False)
     return anime_data
 
 def get_id(name, myanimelist_token=None):
     search_cache = utils_read_json(myanimelist_search_cache_path)
@@ -438,15 +453,15 @@
     def fetch_from_myanimelist():
         # Fetch anime info from myanimelist API or any other source
         anime_name = myanimelist_fetch_id(name)
         anime_info = str(anime_name) if anime_name else None
         if anime_info:
             ani_dict = get_anime_info(anime_info, False, myanimelist_token)
             status = ani_dict[anime_info]['status']
-            if status == 'NOT_YET_RELEASED':
+            if status == "NOT_YET_RELEASED":
                 anime_info = None
             json_out = {name: anime_info}
             utils_save_json(myanimelist_search_cache_path, json_out, False)
             return anime_info
         return None
     # Check if anime_id exists in cache
     try:
@@ -459,25 +474,25 @@
         return fetch_from_myanimelist()
             
 def myanimelist_fetch_id(name, myanimelist_token=None):
     params = {
         'q': name,
         'limit': 1
     }
-    data = make_graphql_request(anime_request_url, params, myanimelist_token)
+    data = make_graphql_request(anime_request_url, params, myanimelist_token = myanimelist_token)
 
     if data:
         return str(data[0]['node']['id'])
 
     return None
 
 def get_userdata(myanimelist_token):
     params = {}
-    request_url = 'https://api.myanimelist.net/v2/users/@me'
-    data = make_graphql_request(request_url, params, myanimelist_token)
+    request_url = "https://api.myanimelist.net/v2/users/@me"
+    data = make_graphql_request(request_url, params, myanimelist_token = myanimelist_token, user_request = True)
 
     if data:
         # Extract the username from the response data
         username = data['name']
         profile_pic = data['picture']
         return [username, profile_pic]
 
@@ -487,15 +502,31 @@
     query ($malId: Int) {
         Media(idMal: $malId type: ANIME) {
             id
         }
     }
     """
     # Constants for GraphQL endpoint and headers
-    ANILIST_API_URL = 'https://graphql.anilist.co'
-    HEADERS = {'Content-Type': 'application/json'}
+    ANILIST_API_URL = "https://graphql.anilist.co"
+    HEADERS = {'Content-Type': "application/json"}
     variables = {'malId': mal_id}
     response = requests.post(ANILIST_API_URL, json={'query': query, 'variables': variables}, headers=HEADERS).json()
 
     if response:
         return int(response['data']['Media']['id'])
-    return None
+    return None
+
+def update_entry(anime_id, progress, myanimelist_token=None):
+    progress = int(progress)
+    total_eps = get_anime_info(anime_id, myanimelist_token=myanimelist_token)[anime_id]['total_eps']
+    params = {}
+    params['num_watched_episodes'] = progress
+    if progress == total_eps:
+        params['status'] = 'COMPLETED'
+    elif progress == 0:
+        params['status'] = 'PLANNING'
+        del params['num_watched_episodes']
+    else:
+        params['status'] = 'CURRENT'
+    request_url = f"https://api.myanimelist.net/v2/anime/{anime_id}/my_list_status"
+    make_graphql_request(request_url, params, 'put', myanimelist_token, True)
+    print('Updating progress successful')
```

### Comparing `malfetcher-1.0.0a0/malfetcher/utils.py` & `malfetcher-1.1.0/malfetcher/utils.py`

 * *Files identical despite different names*

### Comparing `malfetcher-1.0.0a0/pyproject.toml` & `malfetcher-1.1.0/pyproject.toml`

 * *Files identical despite different names*

