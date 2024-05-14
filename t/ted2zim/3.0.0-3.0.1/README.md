# Comparing `tmp/ted2zim-3.0.0.tar.gz` & `tmp/ted2zim-3.0.1.tar.gz`

## Comparing `ted2zim-3.0.0.tar` & `ted2zim-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 ted2zim-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 ted2zim-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 ted2zim-3.0.0/Dockerfile
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 ted2zim-3.0.0/entrypoint.sh
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 ted2zim-3.0.0/openzim.toml
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ted2zim-3.0.0/tasks.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/constants.py
--rwxr-xr-x   0        0        0     6019 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/entrypoint.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/languages.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/processing.py
--rw-r--r--   0        0        0    54583 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/scraper.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/utils.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/locale/hi/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/multi/__init__.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/multi/entrypoint.py
--rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/multi/scraper.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/article.html
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/favicon.png
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/home.html
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/app.js
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/article.css
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/article.js
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/db.js
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/home.css
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/webp-trigger.js
--rwxr-xr-x   0        0        0   142472 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Black.ttf
--rwxr-xr-x   0        0        0   135820 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Bold.ttf
--rwxr-xr-x   0        0        0   140276 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Light.ttf
--rwxr-xr-x   0        0        0   145932 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf
--rwxr-xr-x   0        0        0   145348 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Regular.ttf
--rw-r--r--   0        0        0    16277 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED.png
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED_small.png
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ted2zim-3.0.0/tests/test_dummy.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 ted2zim-3.0.0/tests/test_languages.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 ted2zim-3.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ted2zim-3.0.0/LICENSE
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 ted2zim-3.0.0/README.md
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 ted2zim-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 ted2zim-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 ted2zim-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 ted2zim-3.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 ted2zim-3.0.1/Dockerfile
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 ted2zim-3.0.1/entrypoint.sh
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 ted2zim-3.0.1/openzim.toml
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 ted2zim-3.0.1/tasks.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/constants.py
+-rwxr-xr-x   0        0        0     6019 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/entrypoint.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/languages.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/processing.py
+-rw-r--r--   0        0        0    54618 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/scraper.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/utils.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/locale/hi/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/multi/__init__.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/multi/entrypoint.py
+-rw-r--r--   0        0        0    12893 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/multi/scraper.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/article.html
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/favicon.png
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/home.html
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/app.js
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/article.css
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/article.js
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/db.js
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/home.css
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/webp-trigger.js
+-rwxr-xr-x   0        0        0   142472 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Black.ttf
+-rwxr-xr-x   0        0        0   135820 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Bold.ttf
+-rwxr-xr-x   0        0        0   140276 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Light.ttf
+-rwxr-xr-x   0        0        0   145932 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf
+-rwxr-xr-x   0        0        0   145348 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Regular.ttf
+-rw-r--r--   0        0        0    16277 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/img/TED.png
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 ted2zim-3.0.1/src/ted2zim/templates/assets/img/TED_small.png
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 ted2zim-3.0.1/tests/test_dummy.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 ted2zim-3.0.1/tests/test_languages.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 ted2zim-3.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ted2zim-3.0.1/LICENSE
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 ted2zim-3.0.1/README.md
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 ted2zim-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 ted2zim-3.0.1/PKG-INFO
```

### Comparing `ted2zim-3.0.0/.pre-commit-config.yaml` & `ted2zim-3.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/CHANGELOG.md` & `ted2zim-3.0.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 ## Changelog
 
 All notable changes to this project are documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (as of version 2.0.11).
 
+## [3.0.1] - 2024-05-14
+
+### Fixed
+
+- Change log level from ERROR to WARNING for missing translations (#197)
+- Fix HTTP retries to consider any HTTP failure, not only bad HTTP status code (#162)
+
 ## [3.0.0] - 2024-04-19
 
 ### Added
 
-- New `long_description` CLI argument to set the ZIM long description
-- New `disable_metadata_check` CLI argument to disable the metadata checks which are automated since zimscraperlib 3.x
+- New `--long-description` CLI argument to set the ZIM long description
+- New `--disable-metadata-check` CLI argument to disable the metadata checks which are automated since zimscraperlib 3.x
 - When `--languages` CLI arugment is not passed, no filtering by language is done (#171)
 
 ### Changed
 
 - Changed default publisher metadata from 'Kiwix' to 'openZIM'
 - Validate ZIM metadata as early as possible
 - Migrate to zimscraperlib 3.3.2 (including **new VideoLowWebm encoder preset version 2**)
```

### Comparing `ted2zim-3.0.0/Dockerfile` & `ted2zim-3.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/openzim.toml` & `ted2zim-3.0.1/openzim.toml`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/tasks.py` & `ted2zim-3.0.1/tasks.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/constants.py` & `ted2zim-3.0.1/src/ted2zim/constants.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/entrypoint.py` & `ted2zim-3.0.1/src/ted2zim/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/languages.py` & `ted2zim-3.0.1/src/ted2zim/languages.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/processing.py` & `ted2zim-3.0.1/src/ted2zim/processing.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/scraper.py` & `ted2zim-3.0.1/src/ted2zim/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -825,16 +825,17 @@
                 soup.find(
                     "script", attrs={"id": "__NEXT_DATA__"}
                 ).string  # pyright: ignore
             )["props"]["pageProps"]["videoData"]
 
             requested_lang_code = self.get_lang_code_from_url(url)
             if requested_lang_code and json_data["language"] != requested_lang_code:
-                logger.error(
-                    f"Video has not yet been translated into {requested_lang_code}"
+                logger.warning(
+                    f"Video at {url} has not yet been translated into "
+                    f"{requested_lang_code}"
                 )
                 return None
             # Desrialize the data at json_data["playerData"] into a dict
             # and overwrite it accordingly
             json_data["playerData"] = json.loads(json_data["playerData"])
             return json_data
         except Exception:
```

### Comparing `ted2zim-3.0.0/src/ted2zim/utils.py` & `ted2zim-3.0.1/src/ted2zim/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,27 +34,27 @@
     - a pause of 1 sec is done before every request (including first one)
     """
 
     if url == f"{BASE_URL}playlists/57":
         url = f"{BASE_URL}playlists/57/björk_6_talks_that_are_music"
     max_attempts, attempt = 5, 1
     while True:
-        time.sleep(1)  # delay requests
-        if json_data:
-            req = requests.post(
-                url,
-                headers={"User-Agent": "Mozilla/5.0"},
-                json=json_data,
-                timeout=REQUESTS_TIMEOUT,
-            )
-        else:
-            req = requests.get(
-                url, headers={"User-Agent": "Mozilla/5.0"}, timeout=REQUESTS_TIMEOUT
-            )
         try:
+            time.sleep(1)  # delay requests
+            if json_data:
+                req = requests.post(
+                    url,
+                    headers={"User-Agent": "Mozilla/5.0"},
+                    json=json_data,
+                    timeout=REQUESTS_TIMEOUT,
+                )
+            else:
+                req = requests.get(
+                    url, headers={"User-Agent": "Mozilla/5.0"}, timeout=REQUESTS_TIMEOUT
+                )
             req.raise_for_status()
             return req
         except Exception as exc:
             if req.status_code == HTTPStatus.NOT_FOUND:
                 raise exc
             time.sleep(30 * attempt)  # wait upon failure
```

### Comparing `ted2zim-3.0.0/src/ted2zim/locale/hi/LC_MESSAGES/messages.po` & `ted2zim-3.0.1/src/ted2zim/locale/hi/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/multi/entrypoint.py` & `ted2zim-3.0.1/src/ted2zim/multi/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/multi/scraper.py` & `ted2zim-3.0.1/src/ted2zim/multi/scraper.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/article.html` & `ted2zim-3.0.1/src/ted2zim/templates/article.html`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/favicon.png` & `ted2zim-3.0.1/src/ted2zim/templates/favicon.png`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/home.html` & `ted2zim-3.0.1/src/ted2zim/templates/home.html`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/app.js` & `ted2zim-3.0.1/src/ted2zim/templates/assets/app.js`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/article.css` & `ted2zim-3.0.1/src/ted2zim/templates/assets/article.css`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/article.js` & `ted2zim-3.0.1/src/ted2zim/templates/assets/article.js`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/db.js` & `ted2zim-3.0.1/src/ted2zim/templates/assets/db.js`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/home.css` & `ted2zim-3.0.1/src/ted2zim/templates/assets/home.css`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/webp-trigger.js` & `ted2zim-3.0.1/src/ted2zim/templates/assets/webp-trigger.js`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Black.ttf` & `ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Bold.ttf` & `ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Light.ttf` & `ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf` & `ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/font/Roboto-Regular.ttf` & `ted2zim-3.0.1/src/ted2zim/templates/assets/font/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED.png` & `ted2zim-3.0.1/src/ted2zim/templates/assets/img/TED.png`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/src/ted2zim/templates/assets/img/TED_small.png` & `ted2zim-3.0.1/src/ted2zim/templates/assets/img/TED_small.png`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/tests/test_languages.py` & `ted2zim-3.0.1/tests/test_languages.py`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/.gitignore` & `ted2zim-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/LICENSE` & `ted2zim-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/README.md` & `ted2zim-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ted2zim-3.0.0/pyproject.toml` & `ted2zim-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Make ZIM file from TED Talks"
 readme = "README.md"
 dependencies = [
   "python-dateutil==2.9.0.post0",
   "zimscraperlib==3.3.2",
   "requests==2.31.0",
   "beautifulsoup4==4.12.3",
-  "Jinja2==3.1.3",
+  "Jinja2==3.1.4",
   "kiwixstorage==0.8.3",
   "pif==0.8.2",
   "python-slugify==8.0.4",
   "yt-dlp", # yt-dlp should be updated as frequently as possible
 ]
 dynamic = ["authors", "classifiers", "keywords", "license", "version", "urls"]
```

### Comparing `ted2zim-3.0.0/PKG-INFO` & `ted2zim-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ted2zim
-Version: 3.0.0
+Version: 3.0.1
 Summary: Make ZIM file from TED Talks
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Project-URL: Homepage, https://github.com/openzim/ted
 Author-email: openZIM <dev@openzim.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offline,openzim,ted,zim
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.12
 Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: jinja2==3.1.3
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: kiwixstorage==0.8.3
 Requires-Dist: pif==0.8.2
 Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: python-slugify==8.0.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: yt-dlp
 Requires-Dist: zimscraperlib==3.3.2
```

