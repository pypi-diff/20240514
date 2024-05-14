# Comparing `tmp/pdrive-0.6.1.tar.gz` & `tmp/pdrive-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdrive-0.6.1.tar", last modified: Sat Jul 18 05:06:52 2020, max compression
+gzip compressed data, was "pdrive-0.7.0.tar", last modified: Tue May 14 14:07:40 2024, max compression
```

## Comparing `pdrive-0.6.1.tar` & `pdrive-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2020-07-18 05:06:52.000000 pdrive-0.6.1/
--rw-r--r--   0 huy        (501) staff       (20)      242 2020-07-18 05:06:52.000000 pdrive-0.6.1/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)     1275 2020-07-09 21:03:22.000000 pdrive-0.6.1/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive/backend/
--rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.6.1/pdrive/backend/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)     4778 2020-07-18 00:57:06.000000 pdrive-0.6.1/pdrive/backend/web.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive/frontend/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive/frontend/dist/
--rw-r--r--   0 huy        (501) staff       (20)    28200 2020-07-18 04:41:27.000000 pdrive-0.6.1/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff
--rw-r--r--   0 huy        (501) staff       (20)    55956 2020-07-18 04:41:27.000000 pdrive-0.6.1/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf
--rw-r--r--   0 huy        (501) staff       (20)  6999766 2020-07-18 04:41:27.000000 pdrive-0.6.1/pdrive/frontend/dist/build.js
--rw-r--r--   0 huy        (501) staff       (20)     1145 2020-07-09 21:03:22.000000 pdrive-0.6.1/pdrive/frontend/index.html
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)      242 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      452 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)       52 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive.egg-info/entry_points.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 01:29:51.000000 pdrive-0.6.1/pdrive.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)        6 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        7 2020-07-18 05:06:52.000000 pdrive-0.6.1/pdrive.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2020-07-18 05:06:52.000000 pdrive-0.6.1/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)     1360 2020-07-18 05:05:35.000000 pdrive-0.6.1/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.973730 pdrive-0.7.0/
+-rw-r--r--   0 huy        (501) staff       (20)    35147 2020-07-09 21:03:22.000000 pdrive-0.7.0/LICENSE
+-rw-r--r--   0 huy        (501) staff       (20)      242 2024-05-14 14:07:40.972809 pdrive-0.7.0/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)     1274 2020-07-20 21:16:34.000000 pdrive-0.7.0/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.890133 pdrive-0.7.0/pdrive/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.901505 pdrive-0.7.0/pdrive/backend/
+-rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.7.0/pdrive/backend/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     5792 2024-05-14 14:01:30.000000 pdrive-0.7.0/pdrive/backend/web.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.902989 pdrive-0.7.0/pdrive/frontend/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.906736 pdrive-0.7.0/pdrive/frontend/dist/
+-rw-r--r--   0 huy        (501) staff       (20)    28200 2020-07-18 04:41:27.000000 pdrive-0.7.0/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff
+-rw-r--r--   0 huy        (501) staff       (20)    55956 2020-07-18 04:41:27.000000 pdrive-0.7.0/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf
+-rw-r--r--   0 huy        (501) staff       (20)  6999766 2020-07-18 04:41:27.000000 pdrive-0.7.0/pdrive/frontend/dist/build.js
+-rw-r--r--   0 huy        (501) staff       (20)     1145 2020-07-09 21:03:22.000000 pdrive-0.7.0/pdrive/frontend/index.html
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.897797 pdrive-0.7.0/pdrive.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)      242 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      460 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       52 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 01:29:51.000000 pdrive-0.7.0/pdrive.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        7 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-14 14:07:40.973899 pdrive-0.7.0/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)     1390 2024-05-14 14:06:52.000000 pdrive-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pdrive-0.6.1/README.md` & `pdrive-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 pdrive is a browser-based document and file manager based on Python 3 and vue.js. If you need a quick way of browsing files on a remote server, this is the tool for you.
 
 You can use it as a pretty alternative to `python -m http.server` or as a simple interface into a remote network-attached-storage drive.
 
 It's designed to combine the excellent usability of Google Drive with the benefits of having control over your own data.
 
-![in mov](https://cloud.githubusercontent.com/assets/121183/21594148/018e5c90-d0d4-11e6-9464-74737d860b0b.gif)
+![pdrive](https://user-images.githubusercontent.com/121183/87987433-7e86fb00-ca93-11ea-9236-14823d0650c2.gif)
 
 
 ### installation
 
 ```
 pip install pdrive
 ```
```

### Comparing `pdrive-0.6.1/pdrive/backend/__init__.py` & `pdrive-0.7.0/pdrive/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdrive-0.6.1/pdrive/backend/web.py` & `pdrive-0.7.0/pdrive/backend/web.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,29 +11,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import gunicorn.app.base
 import sys
 import os.path as pth
 import os
 import json
 import shutil
 
 from argparse import ArgumentParser
 from flask import Flask
 from flask import make_response
 from flask import request
 from flask import render_template
 from flask import send_file
 from flask import send_from_directory
 
-frontend_path = pth.join(pth.split(pth.split(pth.abspath(__file__))[0])[0], "frontend")
+frontend_path = pth.join(
+    pth.split(pth.split(pth.abspath(__file__))[0])[0], "frontend")
 
 app = Flask(__name__,
             static_folder=pth.join(frontend_path, "dist"),
             static_url_path="/dist")
 
 
 basedir = os.path.abspath(os.curdir)
@@ -77,15 +79,16 @@
             return json.dumps(payload)
         elif payload["command"] == "cp":
             paths = payload["paths"]
             destination = payload["destination"]
             for p in paths:
                 name = os.path.split(p)[1]
                 copy = shutil.copytree if os.path.isdir(p) else shutil.copy
-                dest = pth.join(destination, name) if os.path.isdir(destination) and os.path.isdir(p) else destination
+                dest = pth.join(destination, name) if os.path.isdir(
+                    destination) and os.path.isdir(p) else destination
                 copy(p, dest)
             return json.dumps(payload)
 
         elif payload["command"] == "mkdir":
             path = payload["path"]
             if not os.path.exists(path):
                 os.makedirs(path)
@@ -154,12 +157,44 @@
 
 
 def main():
     p = ArgumentParser()
     p.add_argument("-H", "--host", default="127.0.0.1")
     p.add_argument("-p", "--port", default=9999)
     a = p.parse_args()
-    app.run(host=a.host, port=a.port)
+
+    # If gunicorn is available use it rather than the
+    # default dev server
+    try:
+        import gunicorn
+        import gunicorn.app.base
+
+        class Application(gunicorn.app.base.BaseApplication):
+
+            def __init__(self, app, options=None):
+                self.options = options or {}
+                self.application = app
+                super().__init__()
+
+            def load_config(self):
+                config = {key: value for key, value in self.options.items()
+                          if key in self.cfg.settings and value is not None}
+                for key, value in config.items():
+                    self.cfg.set(key.lower(), value)
+
+            def load(self):
+                return self.application
+
+        # start app
+        options = {
+            'bind': '%s:%s' % (a.host, a.port),
+            'workers': 3,
+            'timeout': 120,
+        }
+        Application(app, options).run()
+
+    except ImportError:
+        app.run(host=a.host, port=a.port)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pdrive-0.6.1/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff` & `pdrive-0.7.0/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff`

 * *Files identical despite different names*

### Comparing `pdrive-0.6.1/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf` & `pdrive-0.7.0/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf`

 * *Files identical despite different names*

### Comparing `pdrive-0.6.1/pdrive/frontend/dist/build.js` & `pdrive-0.7.0/pdrive/frontend/dist/build.js`

 * *Files identical despite different names*

### Comparing `pdrive-0.6.1/pdrive/frontend/index.html` & `pdrive-0.7.0/pdrive/frontend/index.html`

 * *Files identical despite different names*

### Comparing `pdrive-0.6.1/setup.py` & `pdrive-0.7.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup
 
 setup(name='pdrive',
-      version='0.6.1',
+      version='0.7.0',
       description='File manager',
       author='Huy Nguyen',
       author_email='121183+huyng@users.noreply.github.com',
       packages=['pdrive', "pdrive.frontend", "pdrive.backend"],
       package_data={
           'pdrive.frontend': ['index.html', 'dist/*']
       },
@@ -32,8 +32,9 @@
           ]
       },
       install_requires=["Flask"],
       zip_safe=False,
       url="https://github.com/huyng/pdrive")
 
 # to distribute run:
-# python setup.py register sdist  upload
+# python setup.py register sdist upload
+# python -m twine  upload dist
```

