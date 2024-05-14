# Comparing `tmp/elm_messenger-0.3.0.tar.gz` & `tmp/elm_messenger-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm_messenger-0.3.0.tar", last modified: Mon May 13 00:13:27 2024, max compression
+gzip compressed data, was "elm_messenger-0.3.1.tar", last modified: Tue May 14 03:11:52 2024, max compression
```

## Comparing `elm_messenger-0.3.0.tar` & `elm_messenger-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7181 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-13 00:13:27.000000 elm_messenger-0.3.0/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     8444 2024-05-12 23:36:00.000000 elm_messenger-0.3.0/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2024-05-13 00:13:27.873296 elm_messenger-0.3.0/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.0/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7181 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     7467 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-14 03:11:52.000000 elm_messenger-0.3.1/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     8028 2024-05-13 18:59:35.000000 elm_messenger-0.3.1/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2024-05-14 03:11:52.007553 elm_messenger-0.3.1/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.1/setup.py
```

### Comparing `elm_messenger-0.3.0/PKG-INFO` & `elm_messenger-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Messenger game framework toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `elm_messenger-0.3.0/Readme.md` & `elm_messenger-0.3.1/Readme.md`

 * *Files identical despite different names*

### Comparing `elm_messenger-0.3.0/elm_messenger.egg-info/PKG-INFO` & `elm_messenger-0.3.1/elm_messenger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Messenger game framework toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `elm_messenger-0.3.0/messengercli/messenger.py` & `elm_messenger-0.3.1/messengercli/messenger.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,19 +92,17 @@
                 [f"src/Scenes/{scene}/Components/ComponentBase.elm"],
             ).rep(scene)
 
         os.makedirs(f"src/Scenes/{scene}/Components/{name}", exist_ok=True)
         Updater(
             [
                 ".messenger/component/UserComponent/Model.elm",
-                ".messenger/component/UserComponent/Msg.elm",
             ],
             [
                 f"src/Scenes/{scene}/Components/{name}/Model.elm",
-                f"src/Scenes/{scene}/Components/{name}/Msg.elm",
             ],
         ).rep(scene).rep(name)
 
     def format(self):
         os.system("elm-format src/ --yes")
 
     def add_layer(self, scene: str, layer: str, has_component: bool):
@@ -118,22 +116,14 @@
         if has_component and not os.path.exists(
             f"src/Scenes/{scene}/Components/ComponentBase.elm"
         ):
             raise Exception("Please first create a component.")
         self.config["scenes"][scene].append(layer)
         self.dump_config()
         os.mkdir(f"src/Scenes/{scene}/{layer}")
-        Updater(
-            [
-                ".messenger/layer/Msg.elm",
-            ],
-            [
-                f"src/Scenes/{scene}/{layer}/Msg.elm",
-            ],
-        ).rep(scene).rep(layer)
         if has_component:
             Updater(
                 [
                     ".messenger/layer/ModelC.elm",
                 ],
                 [
                     f"src/Scenes/{scene}/{layer}/Model.elm",
@@ -221,19 +211,18 @@
     input(f"You are going to create a component named {name} in {scene}, continue?")
     msg.add_component(name, scene)
     msg.format()
     print("Done!")
 
 
 @app.command()
-def update(scene=typer.Option(False, "--scene", "-s", help="Update scenes.")):
+def update():
     msg = Messenger()
     input(f"You are going to regenerate elm files based on settings, continue?")
-    if scene:
-        msg.update_scenes()
+    msg.update_scenes()
     msg.format()
     print("Done!")
 
 
 @app.command()
 def scene(
     name: str,
```

### Comparing `elm_messenger-0.3.0/messengercli/updater.py` & `elm_messenger-0.3.1/messengercli/updater.py`

 * *Files identical despite different names*

