# Comparing `tmp/youtube_up-0.4.0.tar.gz` & `tmp/youtube_up-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_up-0.4.0.tar", max compression
+gzip compressed data, was "youtube_up-0.4.1.tar", max compression
```

## Comparing `youtube_up-0.4.0.tar` & `youtube_up-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4156 2024-03-23 23:34:41.080073 youtube_up-0.4.0/README.md
--rw-r--r--   0        0        0      767 2024-03-23 23:34:41.084073 youtube_up-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3651 2024-03-23 23:34:41.084073 youtube_up-0.4.0/youtube_up/__init__.py
--rw-r--r--   0        0        0     6543 2024-03-23 23:34:41.084073 youtube_up-0.4.0/youtube_up/__main__.py
--rw-r--r--   0        0        0    14842 2024-03-23 23:34:41.084073 youtube_up-0.4.0/youtube_up/metadata.py
--rw-r--r--   0        0        0     5805 2024-03-23 23:34:41.084073 youtube_up-0.4.0/youtube_up/polyfills.py
--rw-r--r--   0        0        0    18683 2024-03-23 23:34:41.084073 youtube_up-0.4.0/youtube_up/schema.py
--rw-r--r--   0        0        0    18461 2024-03-23 23:34:41.084073 youtube_up-0.4.0/youtube_up/uploader.py
--rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 youtube_up-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4156 2024-05-14 18:05:03.922781 youtube_up-0.4.1/README.md
+-rw-r--r--   0        0        0      767 2024-05-14 18:05:03.922781 youtube_up-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3651 2024-05-14 18:05:03.922781 youtube_up-0.4.1/youtube_up/__init__.py
+-rw-r--r--   0        0        0     6543 2024-05-14 18:05:03.922781 youtube_up-0.4.1/youtube_up/__main__.py
+-rw-r--r--   0        0        0    14842 2024-05-14 18:05:03.922781 youtube_up-0.4.1/youtube_up/metadata.py
+-rw-r--r--   0        0        0     5805 2024-05-14 18:05:03.922781 youtube_up-0.4.1/youtube_up/polyfills.py
+-rw-r--r--   0        0        0    18683 2024-05-14 18:05:03.922781 youtube_up-0.4.1/youtube_up/schema.py
+-rw-r--r--   0        0        0    18531 2024-05-14 18:05:03.922781 youtube_up-0.4.1/youtube_up/uploader.py
+-rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 youtube_up-0.4.1/PKG-INFO
```

### Comparing `youtube_up-0.4.0/README.md` & `youtube_up-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `youtube_up-0.4.0/pyproject.toml` & `youtube_up-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "youtube-up"
-version = "0.4.0"
+version = "0.4.1"
 description = "Upload videos to YouTube using the internal YouTube API"
 authors = ["7x11x13 <x7x11x13@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/7x11x13/youtube-up"
 documentation = "https://7x11x13.xyz/youtube-up/youtube_up"
 keywords = ["YouTube", "upload"]
```

### Comparing `youtube_up-0.4.0/youtube_up/__init__.py` & `youtube_up-0.4.1/youtube_up/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube_up-0.4.0/youtube_up/__main__.py` & `youtube_up-0.4.1/youtube_up/__main__.py`

 * *Files identical despite different names*

### Comparing `youtube_up-0.4.0/youtube_up/metadata.py` & `youtube_up-0.4.1/youtube_up/metadata.py`

 * *Files identical despite different names*

### Comparing `youtube_up-0.4.0/youtube_up/polyfills.py` & `youtube_up-0.4.1/youtube_up/polyfills.py`

 * *Files identical despite different names*

### Comparing `youtube_up-0.4.0/youtube_up/schema.py` & `youtube_up-0.4.1/youtube_up/schema.py`

 * *Files identical despite different names*

### Comparing `youtube_up-0.4.0/youtube_up/uploader.py` & `youtube_up-0.4.1/youtube_up/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,14 +242,16 @@
                     driver = webdriver.Chrome(options=options, service=service)
                 else:
                     driver = webdriver.Chrome(options=options)
             except Exception:
                 raise YTUploaderException(
                     "Could not launch Firefox or Chrome. Make sure geckodriver or chromedriver is installed"
                 )
+        
+        driver.set_page_load_timeout(self._selenium_timeout)
 
         driver.get("https://youtube.com")
 
         for cookie in self._cookies:
             if cookie.name != "SESSION_TOKEN":
                 driver.add_cookie(cookie.__dict__)
```

### Comparing `youtube_up-0.4.0/PKG-INFO` & `youtube_up-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-up
-Version: 0.4.0
+Version: 0.4.1
 Summary: Upload videos to YouTube using the internal YouTube API
 Home-page: https://github.com/7x11x13/youtube-up
 Keywords: YouTube,upload
 Author: 7x11x13
 Author-email: x7x11x13@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

