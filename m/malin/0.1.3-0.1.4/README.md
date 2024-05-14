# Comparing `tmp/malin-0.1.3.tar.gz` & `tmp/malin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malin-0.1.3.tar", max compression
+gzip compressed data, was "malin-0.1.4.tar", max compression
```

## Comparing `malin-0.1.3.tar` & `malin-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       67 2024-05-14 13:27:31.227071 malin-0.1.3/malin/__init__.py
--rw-r--r--   0        0        0       32 2024-05-14 13:35:40.951891 malin-0.1.3/malin/actions/__init__.py
--rw-r--r--   0        0        0     1229 2024-05-13 14:34:57.085992 malin-0.1.3/malin/actions/scan.py
--rw-r--r--   0        0        0       80 2024-05-14 13:35:54.355565 malin-0.1.3/malin/errors/__init__.py
--rw-r--r--   0        0        0       29 2024-05-13 14:35:22.657421 malin-0.1.3/malin/errors/engine_error.py
--rw-r--r--   0        0        0      298 2024-05-14 11:46:30.922977 malin-0.1.3/malin/errors/parser_error.py
--rw-r--r--   0        0        0      574 2024-05-13 14:27:42.080696 malin-0.1.3/malin/malin.py
--rw-r--r--   0        0        0       88 2024-05-14 13:34:26.915707 malin-0.1.3/malin/models/__init__.py
--rw-r--r--   0        0        0       83 2024-05-13 14:32:45.847772 malin-0.1.3/malin/models/scan_error.py
--rw-r--r--   0        0        0      141 2024-05-13 14:24:13.581645 malin-0.1.3/malin/models/scan_summary.py
--rw-r--r--   0        0        0      290 2024-05-14 13:36:13.153348 malin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 07:54:08.000000 malin-0.1.3/README.md
--rw-r--r--   0        0        0      315 1970-01-01 00:00:00.000000 malin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       67 2024-05-14 13:27:31.227071 malin-0.1.4/malin/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-14 13:35:40.951891 malin-0.1.4/malin/actions/__init__.py
+-rw-r--r--   0        0        0     1229 2024-05-14 15:26:00.528701 malin-0.1.4/malin/actions/scan.py
+-rw-r--r--   0        0        0       80 2024-05-14 13:35:54.355565 malin-0.1.4/malin/errors/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-13 14:35:22.657421 malin-0.1.4/malin/errors/engine_error.py
+-rw-r--r--   0        0        0      298 2024-05-14 11:46:30.922977 malin-0.1.4/malin/errors/parser_error.py
+-rw-r--r--   0        0        0      572 2024-05-14 14:50:54.388957 malin-0.1.4/malin/malin.py
+-rw-r--r--   0        0        0       88 2024-05-14 13:34:26.915707 malin-0.1.4/malin/models/__init__.py
+-rw-r--r--   0        0        0       83 2024-05-13 14:32:45.847772 malin-0.1.4/malin/models/scan_error.py
+-rw-r--r--   0        0        0      141 2024-05-13 14:24:13.581645 malin-0.1.4/malin/models/scan_summary.py
+-rw-r--r--   0        0        0      303 2024-05-14 15:26:16.154799 malin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 07:54:08.000000 malin-0.1.4/README.md
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 malin-0.1.4/PKG-INFO
```

### Comparing `malin-0.1.3/malin/actions/scan.py` & `malin-0.1.4/malin/actions/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         file = request.files['file']
 
         if file.filename == '':
             return jsonify(ScanError(error='No selected file')), 400
 
 
-        filepath: str = f'{tempfile.gettempdir()}/{file.filename}'
+        filepath: str = f'{tempfile.gettempdir()}\{file.filename}'
 
         if not file:
             return jsonify(ScanError(error='Something went wrong')), 500
 
         # Saving the file
         file.save(filepath)
```

### Comparing `malin-0.1.3/malin/malin.py` & `malin-0.1.4/malin/malin.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     parser: Callable[[str], ScanSummary]
  
     def __post_init__(self):
         self.app = Flask("malin")
          
         self.app.add_url_rule('/', 'UploadFile', ScanAction(self.engine, self.parser), methods=['POST'])   
         
-    def run(self, host='127.0.0.1', port=5000):
+    def run(self, host='0.0.0.0', port=5000):
         self.app.run(host=host, port=port)
```

