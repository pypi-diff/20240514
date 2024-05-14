# Comparing `tmp/beets_webrouter-0.3.0-py3-none-any.whl.zip` & `tmp/beets_webrouter-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 41005 bytes, number of entries: 10
--rw-r--r--  2.0 unx       75 b- defN 24-Feb-25 22:40 beetsplug/__init__.py
--rw-r--r--  2.0 unx     3813 b- defN 24-Feb-25 22:40 beetsplug/webrouter/__init__.py
--rw-r--r--  2.0 unx      155 b- defN 24-Feb-25 22:40 beetsplug/webrouter/config_default.yaml
--rw-r--r--  2.0 unx      212 b- defN 24-Feb-25 22:40 beetsplug/webrouter/favicon.py
--rw-r--r--  2.0 unx   112309 b- defN 24-Feb-25 22:40 beetsplug/webrouter/static/favicon.ico
--rw-r--r--  2.0 unx     1070 b- defN 24-Feb-25 22:41 beets_webrouter-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2220 b- defN 24-Feb-25 22:41 beets_webrouter-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-25 22:41 beets_webrouter-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Feb-25 22:41 beets_webrouter-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 24-Feb-25 22:41 beets_webrouter-0.3.0.dist-info/RECORD
-10 files, 120824 bytes uncompressed, 39507 bytes compressed:  67.3%
+Zip file size: 41044 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       75 b- defN 24-May-14 01:43 beetsplug/__init__.py
+-rw-r--r--  2.0 unx     3869 b- defN 24-May-14 01:43 beetsplug/webrouter/__init__.py
+-rw-r--r--  2.0 unx      155 b- defN 24-May-14 01:43 beetsplug/webrouter/config_default.yaml
+-rw-r--r--  2.0 unx      212 b- defN 24-May-14 01:43 beetsplug/webrouter/favicon.py
+-rw-r--r--  2.0 unx   112309 b- defN 24-May-14 01:43 beetsplug/webrouter/static/favicon.ico
+-rw-r--r--  2.0 unx     1070 b- defN 24-May-14 01:43 beets_webrouter-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2220 b- defN 24-May-14 01:43 beets_webrouter-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 01:43 beets_webrouter-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-14 01:43 beets_webrouter-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 24-May-14 01:43 beets_webrouter-0.4.0.dist-info/RECORD
+10 files, 120880 bytes uncompressed, 39546 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: beetsplug/webrouter/favicon.py
 Comment: 
 
 Filename: beetsplug/webrouter/static/favicon.ico
 Comment: 
 
-Filename: beets_webrouter-0.3.0.dist-info/LICENSE
+Filename: beets_webrouter-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: beets_webrouter-0.3.0.dist-info/METADATA
+Filename: beets_webrouter-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: beets_webrouter-0.3.0.dist-info/WHEEL
+Filename: beets_webrouter-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: beets_webrouter-0.3.0.dist-info/top_level.txt
+Filename: beets_webrouter-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: beets_webrouter-0.3.0.dist-info/RECORD
+Filename: beets_webrouter-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beetsplug/webrouter/__init__.py

```diff
@@ -88,14 +88,14 @@
                 app,
                 supports_credentials=self.config['cors_supports_credentials'].get(bool),
             )
 
         for k,v in cfg:
             app.config[k] = v.get()
 
-        if self.config['reverse_proxy']:
+        if self.config['reverse_proxy'] or os.getenv('BEETS_WEBROUTER_REVERSE_PROXY') == 'true':
             app.wsgi_app = ReverseProxied(app.wsgi_app)
 
 class BlueprintRoute:
     def __init__(self, url_prefix, blueprint):
         self.url_prefix = url_prefix
         self.blueprint = blueprint
```

## Comparing `beets_webrouter-0.3.0.dist-info/LICENSE` & `beets_webrouter-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beets_webrouter-0.3.0.dist-info/METADATA` & `beets_webrouter-0.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beets-webrouter
-Version: 0.3.0
+Version: 0.4.0
 Summary: Serve multiple beets APIs on the same host/port
 Home-page: https://github.com/mgoltzsche/beets-webrouter
 Author: Max Goltzsche
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
```

