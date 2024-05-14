# Comparing `tmp/alfetcher-1.0.0a0.tar.gz` & `tmp/alfetcher-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfetcher-1.0.0a0.tar", last modified: Sat Apr 20 08:30:18 2024, max compression
+gzip compressed data, was "alfetcher-1.1.0.tar", last modified: Tue May 14 12:12:57 2024, max compression
```

## Comparing `alfetcher-1.0.0a0.tar` & `alfetcher-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/alfetcher/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/al_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23029 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/al_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/alfetcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/alfetcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 08:30:18.000000 alfetcher-1.0.0a0/alfetcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:30:18.458609 alfetcher-1.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 08:30:08.000000 alfetcher-1.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:12:57.164239 alfetcher-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-14 12:12:48.000000 alfetcher-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-14 12:12:57.164239 alfetcher-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-14 12:12:48.000000 alfetcher-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:12:57.164239 alfetcher-1.1.0/alfetcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-14 12:12:48.000000 alfetcher-1.1.0/alfetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-14 12:12:48.000000 alfetcher-1.1.0/alfetcher/al_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-14 12:12:48.000000 alfetcher-1.1.0/alfetcher/al_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-14 12:12:48.000000 alfetcher-1.1.0/alfetcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:12:57.164239 alfetcher-1.1.0/alfetcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-14 12:12:57.000000 alfetcher-1.1.0/alfetcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-14 12:12:57.000000 alfetcher-1.1.0/alfetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:12:57.000000 alfetcher-1.1.0/alfetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 12:12:57.000000 alfetcher-1.1.0/alfetcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 12:12:57.000000 alfetcher-1.1.0/alfetcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-14 12:12:48.000000 alfetcher-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:12:57.164239 alfetcher-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-14 12:12:48.000000 alfetcher-1.1.0/setup.py
```

### Comparing `alfetcher-1.0.0a0/LICENSE` & `alfetcher-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alfetcher-1.0.0a0/PKG-INFO` & `alfetcher-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: alfetcher
-Version: 1.0.0a0
-Summary: A simple library to help you fetch data from AniList.
-Author: Dominik Procházka
-Maintainer: Dominik Procházka
-Project-URL: Homepage, https://github.com/prochy-exe/alfetcher
-Project-URL: Documentation, https://github.com/prochy-exe/alfetcher/wiki
-Project-URL: Source, https://github.com/prochy-exe/alfetcher
-Keywords: python,anilist,al
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Flask
-Classifier: Topic :: Database
-Classifier: Topic :: Games/Entertainment
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: flask
-Requires-Dist: gevent
-
 # alfetcher
 
 A simple library to help you fetch data from AniList
 
 ## Description
 
 Welcome to my first python project!
@@ -85,14 +58,24 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
+* [1.1.0](https://github.com/prochy-exe/alfetcher/releases/tag/v1.1.0)
+    * [fix typo](https://github.com/prochy-exe/alfetcher/commit/dbf3d14e90c4cfeebcef51503a884efd1e1178b5)
+    * [allow some functions to not require user token](https://github.com/prochy-exe/alfetcher/commit/f3e58106709d5b1626b65384977fe22a05c7d647)
+    * [use local ip address instead of localhost](https://github.com/prochy-exe/alfetcher/commit/9d6500229980faf68b20fe4a559a8d2bc08fed1b)
+    * [print list name when no anime found](https://github.com/prochy-exe/alfetcher/commit/efca221b8f78ac0848aaa7d8813b6b5c36e89c28)
+    * [drop user list caching](https://github.com/prochy-exe/alfetcher/commit/954fe02ef643e228561a2c3e845e18b431947652)
+    * [add function to update progress in users list](https://github.com/prochy-exe/alfetcher/commit/c040d8836efb44352dd2f1339305cb9c5296f97d)
+    * [add function to convert from al to mal id](https://github.com/prochy-exe/alfetcher/commit/278805356c25dcabb4029b01e337c40f83b135ac)
+    * [dates: Make sure they are not None](https://github.com/prochy-exe/alfetcher/commit/92db92773cea64ec7e8c8f12bcf4bc624c2400b2)
+    * [Formatting changes](https://github.com/prochy-exe/alfetcher/commit/b4a96be729ab23cff87fe00c2e0deab7d6b742f7)
 * [1.0.0](https://github.com/prochy-exe/alfetcher/releases/tag/v1.0.0)
     * [Initial Release](https://github.com/prochy-exe/alfetcher/commit/4b67b1d8719d183012446a065c5b6c941ec6518e)
 
 ## Acknowledgments
 
 Huge thanks to AniList team for their great page and database:
 * [AniList](https://anilist.co/home)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `alfetcher-1.0.0a0/alfetcher/al_config_utils.py` & `alfetcher-1.1.0/alfetcher/al_config_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,26 @@
-import os, webbrowser, platform, requests, gevent, gc
+import os, webbrowser, platform, requests, gevent, gc, socket
 from flask import Flask, request, redirect
 from gevent.pywsgi import WSGIServer
 from urllib.parse import parse_qs
 from .utils import utils_save_json
 
+def get_ip_address():
+    try:
+        s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        s.connect(("8.8.8.8", 80))
+        ip_address = s.getsockname()[0]
+        s.close()
+        return ip_address
+    except Exception as e:
+        print("Error:", e)
+        return None
+
+host_ip = get_ip_address()
+
 # Paths
 script_path = os.path.dirname(os.path.abspath(__file__))
 config_path = os.path.join(script_path, 'config', 'config.json')
 
 is_ssh = 'SSH_CONNECTION' in os.environ
 is_displayless = 'DISPLAY' not in os.environ
 is_linux = platform.system() == 'Linux'
@@ -18,66 +31,66 @@
  
 def setup_webserver():
     app = Flask(__name__)
 
     # Enable CORS for all routes
     @app.after_request
     def add_cors_headers(response):
-        response.headers['Access-Control-Allow-Origin'] = '*'
-        response.headers['Access-Control-Allow-Headers'] = 'Content-Type'
-        response.headers['Access-Control-Allow-Methods'] = 'GET, POST, OPTIONS'
+        response.headers['Access-Control-Allow-Origin'] = "*"
+        response.headers['Access-Control-Allow-Headers'] = "Content-Type"
+        response.headers['Access-Control-Allow-Methods'] = "GET, POST, OPTIONS"
         return response
 
     @app.route('/access_token') #Listen for token webhook
     def receive_token():
         def make_request(code):
             headers = {
-                'Content-Type': 'application/json',
-                'Accept': 'application/json',
+                'Content-Type': "application/json",
+                'Accept': "application/json",
             }
             json = {
-                'grant_type': 'authorization_code',
+                'grant_type': "authorization_code",
                 'client_id': global_id,
                 'client_secret': global_secret,
-                'redirect_uri': 'http://localhost:8888/access_token',
+                'redirect_uri': f"http://{host_ip}:8888/access_token",
                 'code': f'{code}'
             }
-            response = requests.post('https://anilist.co/api/v2/oauth/token', json=json, headers=headers)
+            response = requests.post("https://anilist.co/api/v2/oauth/token", json=json, headers=headers)
             return response.json()
 
         # Extracting query parameters from the request URL
         query = request.query_string.decode()
         params = parse_qs(query)
 
         # Extracting the 'code' parameter from the query
         code = params.get('code', [''])[0]
 
         # Do something with the code
         global access_token
         access_token = make_request(code)['access_token']
         http_server.stop()
-        return redirect('https://anilist.co')
+        return redirect("https://anilist.co")
         
     def start_webserver():
         if headless_config:
-           print('Open this URL in your browser: ', global_tooltip)
+           print("Open this URL in your browser: ", global_tooltip)
         else:
-            print('Authentificate in the opened tab')
+            print("Authentificate in the opened tab")
             webbrowser.open(global_tooltip, 0)
         http_server.serve_forever()
 
-    http_server = WSGIServer(('127.0.0.1', 8888), app, log=None)
+    http_server = WSGIServer((host_ip, 8888), app, log=None)
 
     return start_webserver, http_server 
         
 def config_setup(print_only = False):
     setup_function, _ = setup_webserver()  # Setup the server function here
     
     def gen_please(name, help):
-        return f'Please input your {name} here ({help}):\n'
+        return f"Please input your {name} here ({help}):\n"
     
     def get_input(prompt, data_type = str):
         while True:
             user_input = input(prompt)
             try:
                 converted_input = data_type(user_input)
                 return converted_input
@@ -86,32 +99,32 @@
     
     def generate_api_key(client_id, client_secret):
         global global_id
         global global_secret
         global global_tooltip
         global_id = client_id
         global_secret = client_secret
-        global_tooltip = f"http://anilist.co/api/v2/oauth/authorize?client_id={client_id}&redirect_uri=http://localhost:8888/access_token&response_type=code" 
+        global_tooltip = f"http://anilist.co/api/v2/oauth/authorize?client_id={client_id}&redirect_uri=http://{host_ip}:8888/access_token&response_type=code" 
         setup_function()  # Start the server here
         user_token = access_token
         gevent.killall(
             [obj for obj in gc.get_objects() if isinstance(obj, gevent.Greenlet)]
         ) #kill all gevent greenlets to prevert interference
         return user_token    
     
     config_dict = {}
     print("ONLY THE USER TOKEN WILL BE SAVED!!!!")
     print("Please create a new API client")
     if headless_config:
         if is_displayless:
-            print('The setup process cannot be continued on this machine')
-            print('Please SSH into this machine, set the access key as an env variable or import the config directly')
-        client_id = get_input(gen_please('Anilist API Client ID',"https://anilist.co/settings/developer"))
-        client_secret = get_input(gen_please('Anilist API Client Secret',f"https://anilist.co/settings/client/{client_id}"))
+            print("The setup process cannot be continued on this machine")
+            print("Please SSH into this machine, set the access key as an env variable or import the config directly")
+        client_id = get_input(gen_please("Anilist API Client ID","https://anilist.co/settings/developer"))
+        client_secret = get_input(gen_please("Anilist API Client Secret",f"https://anilist.co/settings/client/{client_id}"))
     else:
-        webbrowser.open('https://anilist.co/settings/developer', 0)
-        client_id = get_input(gen_please('Anilist API Client ID',"Paste the Client ID"))    
-        client_secret = get_input(gen_please('Anilist API Client Secret',"Paste the Client Secret"))
+        webbrowser.open("https://anilist.co/settings/developer", 0)
+        client_id = get_input(gen_please("Anilist API Client ID","Paste the Client ID"))    
+        client_secret = get_input(gen_please("Anilist API Client Secret","Paste the Client Secret"))
     config_dict['anilist_user_token'] = generate_api_key(client_id, client_secret)
     if not print_only:    
         utils_save_json(config_path, config_dict)
     return config_dict
```

### Comparing `alfetcher-1.0.0a0/alfetcher/al_fetcher.py` & `alfetcher-1.1.0/alfetcher/al_fetcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import requests, time, os, copy, math
 from datetime import datetime, timedelta
 from .utils import utils_save_json, utils_read_json
 from .al_config_utils import config_setup
 
-total_user = {}
-user_entries = {}
 script_path = os.path.dirname(os.path.abspath(__file__))
 anilist_id_cache_path = os.path.join(script_path, 'cache', 'anilist_id_cache.json')
 anilist_search_cache_path = os.path.join(script_path, 'cache', 'anilist_search_cache.json')
 config_path = os.path.join(script_path, 'config', 'config.json')
 
 
 # Utils
@@ -43,27 +41,27 @@
             try:
                 end_date = datetime.strptime(cache[anime]['end_date'], '%Y-%m-%d').date()
             except:
                 end_date = None
             if not release_date:
                 continue
             status = cache[anime]['status']
-            if status == 'RELEASING':
+            if status == "RELEASING":
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
+            elif status == "NOT_YET_RELEASED":
                 if release_date:
                     if current_date > release_date:
                         cache.update(get_anime_info(anime, True))
         config_dict['checked_date'] = current_date.strftime('%Y-%m-%d')
         utils_save_json(config_path, config_dict)
         utils_save_json(anilist_id_cache_path, cache, True)
 
@@ -76,47 +74,50 @@
     try:
         return config['anilist_user_token']
     except:
         return config_setup()['anilist_user_token']
 
 # Functions
 
-def make_graphql_request(query, variables=None, anilist_token=None):
-    if anilist_token:
-        pass
-    elif 'anilist_key' in os.environ:
-        anilist_token = os.getenv('anilist_key')
-        if not os.path.exists(os.path.dirname(config_path)):
-            os.makedirs(os.path.dirname(config_path))
-    else:
-        anilist_token = load_config()
-
+def make_graphql_request(query, variables=None, anilist_token=None, user_request = False):
     # Constants for GraphQL endpoint and headers
-    ANILIST_API_URL = 'https://graphql.anilist.co'
-    HEADERS = {'Content-Type': 'application/json', 'Authorization': f'Bearer {anilist_token}'}
+    ANILIST_API_URL = "https://graphql.anilist.co"
+    HEADERS = {}
+    HEADERS['Content-Type'] = "application/json"
+    
+    if user_request:
+        if anilist_token:
+            pass
+        elif 'anilist_key' in os.environ:
+            anilist_token = os.getenv('anilist_key')
+            if not os.path.exists(os.path.dirname(config_path)):
+                os.makedirs(os.path.dirname(config_path))
+        else:
+            anilist_token = load_config()
+        HEADERS['Authorization'] = f"Bearer {anilist_token}"
 
     def make_request():
         response = requests.post(ANILIST_API_URL, json={'query': query, 'variables': variables}, headers=HEADERS)
         return response
 
     retries = 0
     while True:
         response = make_request()
         if response.status_code == 200:
             return response.json().get('data', {})
         elif response.status_code == 429:
             print(f"Rate limit exceeded. Waiting before retrying...")
-            print(query, variables, HEADERS, sep='\n')
+            print(query, variables, HEADERS, sep="\n")
             print(response.json())
             retry_after = int(response.headers.get('retry-after', 1))
             time.sleep(retry_after)
             retries += 1
         elif response.status_code == 500 or response.status_code == 400:
-            print(f"Unknown error occured, retrying...")
-            print(query, variables, HEADERS, sep='\n')
+            print(f"Unknown error occurred, retrying...")
+            print(query, variables, HEADERS, sep="\n")
             print(response.json())
             retries += 1
         elif response.status_code == 404:
             print(f"Anime not found")
             return None
         else:
             print(f"Error {response.status_code}: {variables}")
@@ -125,22 +126,26 @@
         # Exponential backoff with a maximum of 5 retries
         if retries >= 5:
             print("Maximum retries reached. Exiting.")
             return {}
                 
         print(f"Retrying... (Attempt {retries})")
 
-def get_latest_anime_entry_for_user(status = 'ALL', anilist_token=None,  username=None):
+def get_latest_anime_entry_for_user(status = "ALL", anilist_token=None,  username=None):
     if not username:
         username = get_userdata(anilist_token)[0]
+        user_request = True
+    else:
+        user_request = False
+        
     status = status.upper()
-    status_options = ['CURRENT', 'PLANNING', 'COMPLETED', 'DROPPED', 'PAUSED', 'REPEATING']
-    if status != 'ALL':
+    status_options = ["CURRENT", "PLANNING", "COMPLETED", "DROPPED", "PAUSED", "REPEATING"]
+    if status != "ALL":
         if not status in status_options:
-            print("Invalid status option. Allowed options are:", ', '.join(str(option) for option in status_options) )
+            print("Invalid status option. Allowed options are:", ", ".join(str(option) for option in status_options) )
             return
         query = '''
         query ($username: String) {
             MediaListCollection(userName: $username, type: ANIME, status: %s, sort: [UPDATED_TIME_DESC]) {
         ''' %status
     else:
         query = '''
@@ -199,45 +204,45 @@
                 }
             }
         }
     }
     '''
     variables = {'username': username}
 
-    data = make_graphql_request(query, variables, anilist_token)
+    data = make_graphql_request(query, variables, anilist_token, user_request=user_request)
 
-    if not username in user_entries:
-        user_entries[username] = {}
-        
     if data:
         entries = data.get('MediaListCollection', {}).get('lists', [])[0].get('entries', [])
         if entries:
             for anime in entries:
                 anime_id = str(anime['media']['id'])
                 anime_info = generate_anime_entry(anime['media'])
                 user_entry = {}    # Initialize as a dictionary if not already initialized
                 user_entry[anime_id] = {}    # Initialize as a dictionary if not already initialized
                 user_entry[anime_id].update(anime_info)
                 user_entry[anime_id]['watched_ep'] = anime['progress']
                 user_entry[anime_id]['watching_status'] = anime['status']
-                user_entries[username][anime_id] = user_entry
                 return user_entry
 
-    print(f"No entries found for {username}'s planned anime list.")
+    print(f"No entries found for {username}'s {status.lower()} anime list.")
     return None
 
-def get_all_anime_for_user(status_list='ALL', anilist_token=None, username=None):
+def get_all_anime_for_user(status_list="ALL", anilist_token=None, username=None):
     if not username:
         username = get_userdata(anilist_token)[0]
+        user_request = True
+    else:
+        user_request = False
+        
     def main_function(status):
         status = status.upper()
-        status_options = ['CURRENT', 'PLANNING', 'COMPLETED', 'DROPPED', 'PAUSED', 'REPEATING']
-        if status != 'ALL':
+        status_options = ["CURRENT", "PLANNING", "COMPLETED", "DROPPED", "PAUSED", "REPEATING"]
+        if status != "ALL":
             if not status in status_options:
-                print("Invalid status option. Allowed options are:", ', '.join(str(option) for option in status_options) )
+                print("Invalid status option. Allowed options are:", ", ".join(str(option) for option in status_options) )
                 return
             query = '''
             query ($username: String) {
                 MediaListCollection(userName: $username, type: ANIME, status: %s, sort: [UPDATED_TIME_DESC]) {
             ''' %status
         else:
             query = '''
@@ -296,24 +301,15 @@
                     }
                 }
             }
         }
         '''
         variables = {'username': username}
 
-        data = make_graphql_request(query, variables, anilist_token)
-
-        if not username in user_entries:
-            user_entries[username] = {}
-
-        if not username in total_user:
-            total_user[username] = {}
-
-        if not status in user_entries[username]:
-            user_entries[username][status] = {}
+        data = make_graphql_request(query, variables, anilist_token, user_request=user_request)
 
         user_ids = {}
             
         if data:
                 entries = data.get('MediaListCollection', {}).get('lists', [])
                 full_entries = {}
                 for entry in entries: 
@@ -328,72 +324,62 @@
                             anime_id = str(anime_id)
                             anime_info = generate_anime_entry(anime_entry_data)
                             if not anime_id in user_ids:
                                 user_ids[anime_id] = {}    # Initialize as a dictionary if not already initialized
                             user_ids[anime_id].update(anime_info)
                             user_ids[anime_id]['watched_ep'] = anime['progress']
                             user_ids[anime_id]['watching_status'] = anime['status']
-                        user_entries[username][status].update(user_ids)
-                        return
-        print(f"No entries found for {username}'s planned anime list.")
+                        return user_ids
+        print(f"No entries found for {username}'s {status.lower()} anime list.")
         return None    
 
     if isinstance(status_list, str):
         status_list = status_list.upper()
         main_function(status_list)
-        return user_entries[username][status_list]
+        return main_function(status_list)
     elif len(status_list) == 1:
         status_list = status_list[0].upper()
-        main_function(status_list)
-        return user_entries[username][status_list]
+        return main_function(status_list)
     elif isinstance(status_list, list):
+        ani_list = {}
         for status in status_list:
             status.upper()
-            main_function(status)
-            total_user[username].update(user_entries[username][status])
-        return total_user[username]
+            ani_list.update(main_function(status))
+        return ani_list
 
 def get_anime_entry_for_user(anilist_id, anilist_token=None, username=None):
     if not username:
         username = get_userdata(anilist_token)[0]
+        user_request = True
+    else:
+        user_request = False
+        
     anilist_id = str(anilist_id)
-    try:
-        if anilist_id in user_entries[username]['ALL']:
-                    return {anilist_id: user_entries[username]['ALL'][anilist_id]}
-    except KeyError:
-        query = '''
-        query ($mediaId: Int, $username: String) {
-            MediaList(mediaId: $mediaId, userName: $username, type: ANIME) {
-                mediaId
-                progress
-                status
-            }
-        }
-        '''
-        variables = {'mediaId': anilist_id, 'username': username}
-        data = make_graphql_request(query, variables, anilist_token)
-        if data:
-            anime = data.get('MediaList', {})
-            anime_id = str(anime['mediaId'])
-            anime_info = get_anime_info(anime_id, False, anilist_token)
-            user_entry = {}    # Initialize as a dictionary if not already initialized
-            user_entry[anime_id] = {}    # Initialize as a dictionary if not already initialized
-            user_entry[anime_id].update(anime_info)
-            user_entry[anime_id]['watched_ep'] = anime['progress']
-            user_entry[anime_id]['watching_status'] = anime['status']
-            if not username in user_entries:
-                user_entries[username] = {}
-            user_entries[username][anime_id] = user_entry
-            return user_entry
+    query = '''
+    query ($mediaId: Int, $username: String) {
+        MediaList(mediaId: $mediaId, userName: $username, type: ANIME) {
+            mediaId
+            progress
+            status
+        }   
+    }
+    '''
+    variables = {'mediaId': anilist_id, 'username': username}
+    data = make_graphql_request(query, variables, anilist_token, user_request=user_request)
+    if data:
+        anime = data.get('MediaList', {})
+        anime_id = str(anime['mediaId'])
+        anime_info = get_anime_info(anime_id, False, anilist_token)
+        user_entry = {}    # Initialize as a dictionary if not already initialized
+        user_entry.update(anime_info)
+        user_entry[anime_id]['watched_ep'] = anime['progress']
+        user_entry[anime_id]['watching_status'] = anime['status']
+        return user_entry
     return None
 
-def reset_user_cache(username):
-    user_entries[username] = {}
-    total_user[username] = {}
-
 def get_anime_info(anime_id, force_update = False, anilist_token=None):
     if force_update:
         anime_cache = {}
     else:
         anime_cache = load_cache()
     anime_id = str(anime_id)
     if not anime_id:
@@ -475,56 +461,56 @@
             anime_data[anime_id] = {}
             anime_data[anime_id].update(generate_anime_entry(anime_info))
         return anime_data
     return {}
 
 def generate_anime_entry(anime_info):
     def get_release_date(anime_data):
-            start_date = anime_data.get('startDate', {})
-            day = start_date.get('day', 28)
-            day = 28 if day is None else day
-            try:
-                release_date = datetime(start_date['year'], start_date.get('month', 1), day).strftime('%Y-%m-%d')
-            except TypeError:
-                release_date = None
-            return release_date
+        start_date = anime_data.get('startDate', {})
+        year = start_date.get('year')
+        month = start_date.get('month')
+        if not year or not month:
+            return None
+        day = start_date.get('day') if start_date['day'] else 1
+        release_date = datetime(year, month, day).strftime('%Y-%m-%d')
+        return release_date
         
     def get_end_date(anime_data):
-            end_date = anime_data.get('endDate', {})
-            day = end_date.get('day', 28)
-            day = 28 if day is None else day
-            try:
-                end_date = datetime(end_date['year'], end_date.get('month', 1), day).strftime('%Y-%m-%d')
-            except TypeError:
-                end_date = None
-            return end_date         
+        end_date = anime_data.get('endDate', {})
+        year = end_date.get('year')
+        month = end_date.get('month')
+        if not year or not month:
+            return None
+        day = end_date.get('day') if end_date['day'] else 1
+        end_date = datetime(year, month, day).strftime('%Y-%m-%d')
+        return end_date         
 
     def getRelated():
         relations = {}
         edges = anime_info['relations']['edges']
         for edge in edges:
-            if edge['relationType'] == 'PREQUEL' or edge['relationType'] == 'SEQUEL':
+            if edge['relationType'] == "PREQUEL" or edge['relationType'] == "SEQUEL":
                 relation_id = str(edge['node']['id'])
                 relations[relation_id] = {}
                 relations[relation_id]['main_title'] = edge['node']['title']['romaji']
                 relations[relation_id]['status'] = edge['node']['status']
                 relations[relation_id]['type'] = edge['relationType']
         if not relations:
             relations = None
         return relations
 
     def is_sus(anime_data):
         genres = anime_data['genres']
         tags = [item['name'] for item in anime_data['tags']]
         adult_status = anime_data['isAdult']
-        sus_tags = ['Nudity', 'Bondage', 'Masochism', 'Sadism', 'Exhibitionism']
+        sus_tags = ["Nudity", "Bondage", "Masochism", "Sadism", "Exhibitionism"]
         for sus_tag in sus_tags:
             if sus_tag in tags:
                 return True
-        if 'Ecchi' in genres or adult_status:
+        if "Ecchi" in genres or adult_status:
             return True
         else:
             return False
 
     def generate_upcoming_ep(release_date):
         current_date = datetime.now().date()
         release_date = datetime.strptime(release_date, '%Y-%m-%d').date()
@@ -542,15 +528,15 @@
         anime_info['title']['english'],
         anime_info['title']['native'],
     ] + anime_info['synonyms']
     anime_data['synonyms'] = [item for item in anime_data['synonyms'] if item is not None]    
     anime_data['status'] = anime_info['status']
     anime_data['release_date'] = get_release_date(anime_info)
     anime_data['end_date'] = get_end_date(anime_info)
-    anime_data['upcoming_ep'] = ((generate_upcoming_ep(anime_data['release_date']) if anime_data['status'] == 'RELEASING' else None) 
+    anime_data['upcoming_ep'] = ((generate_upcoming_ep(anime_data['release_date']) if anime_data['status'] == "RELEASING" else None) 
                                 if not anime_info['nextAiringEpisode'] else anime_info['nextAiringEpisode']['episode']) #who needs readability
     anime_data['format'] = anime_info['format']
     anime_data['related'] = getRelated()
     utils_save_json(anilist_id_cache_path, {anime_id: anime_data}, False)
     return anime_data
 
 def get_id(name, anilist_token=None):
@@ -559,15 +545,15 @@
     def fetch_from_anilist():
         # Fetch anime info from Anilist API or any other source
         anime_name = anilist_fetch_id(name)
         anime_info = str(anime_name) if anime_name else None
         if anime_info:
             ani_dict = get_anime_info(anime_info, False, anilist_token)
             status = ani_dict[anime_info]['status']
-            if status == 'NOT_YET_RELEASED':
+            if status == "NOT_YET_RELEASED":
                 anime_info = None
             json_out = {name: anime_info}
             utils_save_json(anilist_search_cache_path, json_out, False)
             return anime_info
         return None
     # Check if anime_id exists in cache
     try:
@@ -608,14 +594,59 @@
                 large
             }
         }
     }
     """
     
     variables = {}
-    data = make_graphql_request(query, variables, anilist_token)
+    data = make_graphql_request(query, variables, anilist_token, user_request = True)
 
     if data:
         # Extract the username from the response data
         username = data['Viewer']['name']
         profile_pic = data['Viewer']['avatar']['large']
-        return [username, profile_pic]
+        return [username, profile_pic]
+
+def al_to_mal_id(al_id):
+    query = """
+    query ($mediaId: Int) {
+        Media(id: $mediaId, type: ANIME) {
+            idMal
+        }
+    }
+    """
+    variables = {'mediaId': al_id}
+    data = make_graphql_request(query, variables)
+
+    if data:
+        return int(data['Media']['idMal'])
+    return None
+
+def update_entry(anime_id, progress, anilist_token=None):
+    progress = int(progress)
+    total_eps = get_anime_info(anime_id, anilist_token=anilist_token)[anime_id]['total_eps']
+    query = """
+        mutation ($mediaId: Int, $progress: Int, $status: MediaListStatus) {
+            SaveMediaListEntry(mediaId: $mediaId, progress: $progress, status: $status) {
+                id
+            }
+        }
+    """
+    variables = {}
+    variables['mediaId'] = anime_id
+    variables['progress'] = progress
+    if progress == total_eps:
+        variables['status'] = 'COMPLETED'
+    elif progress == 0:
+        variables['status'] = 'PLANNING'
+        query = """
+            mutation ($mediaId: Int, $status: MediaListStatus) {
+                SaveMediaListEntry(mediaId: $mediaId, status: $status) {
+                    id
+                }
+            }
+        """
+        del variables['progress']
+    else:
+        variables['status'] = 'CURRENT'
+    make_graphql_request(query, variables, anilist_token, user_request = True)
+    print('Updating progress successful')
```

### Comparing `alfetcher-1.0.0a0/alfetcher/utils.py` & `alfetcher-1.1.0/alfetcher/utils.py`

 * *Files identical despite different names*

### Comparing `alfetcher-1.0.0a0/pyproject.toml` & `alfetcher-1.1.0/pyproject.toml`

 * *Files identical despite different names*

