# Comparing `tmp/itrm-0.2.0.tar.gz` & `tmp/itrm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itrm-0.2.0.tar", last modified: Mon May 13 17:04:42 2024, max compression
+gzip compressed data, was "itrm-0.2.1.tar", last modified: Mon May 13 18:59:54 2024, max compression
```

## Comparing `itrm-0.2.0.tar` & `itrm-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.397034 itrm-0.2.0/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.2.0/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15006 2024-05-13 17:04:42.396902 itrm-0.2.0/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    14549 2024-05-13 17:03:52.000000 itrm-0.2.0/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.2.0/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-13 17:04:42.397272 itrm-0.2.0/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.395173 itrm-0.2.0/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.395916 itrm-0.2.0/src/itrm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.2.0/src/itrm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    64134 2024-05-13 17:00:18.000000 itrm-0.2.0/src/itrm/itrm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 17:04:42.396686 itrm-0.2.0/src/itrm.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    15006 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-13 17:04:42.000000 itrm-0.2.0/src/itrm.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 18:59:54.335517 itrm-0.2.1/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 itrm-0.2.1/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15019 2024-05-13 18:59:54.335203 itrm-0.2.1/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    14562 2024-05-13 18:59:25.000000 itrm-0.2.1/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 itrm-0.2.1/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      579 2024-05-13 18:59:54.335784 itrm-0.2.1/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 18:59:54.333413 itrm-0.2.1/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 18:59:54.334122 itrm-0.2.1/src/itrm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-05-06 19:09:39.000000 itrm-0.2.1/src/itrm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    65264 2024-05-13 18:57:36.000000 itrm-0.2.1/src/itrm/itrm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 18:59:54.334968 itrm-0.2.1/src/itrm.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    15019 2024-05-13 18:59:54.000000 itrm-0.2.1/src/itrm.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-13 18:59:54.000000 itrm-0.2.1/src/itrm.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-13 18:59:54.000000 itrm-0.2.1/src/itrm.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-13 18:59:54.000000 itrm-0.2.1/src/itrm.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-13 18:59:54.000000 itrm-0.2.1/src/itrm.egg-info/top_level.txt
```

### Comparing `itrm-0.2.0/LICENSE.txt` & `itrm-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `itrm-0.2.0/PKG-INFO` & `itrm-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,15 +55,16 @@
 | ---------     | :-----------: | --------------------------------- |
 | `uni`         | `True`        | flag to use Unicode characters    |
 | `cols`        | `60`          | default column width              |
 | `rows`        | `20`          | default row height                |
 | `ar`          | `0.48`        | aspect ratio of characters        |
 
 There is also a method for changing the color map: `itrm.config.cmap()`. It
-takes a string: `"colors"`, `"grays"`, `"reds"`, `"greens"`, or `"blues"`.
+takes a string: `"colors"`, `"viridis"`, `"grays"`, `"reds"`, `"greens"`, or
+`"blues"`.
 
 ## Interactive Plots
 
 ```python
 itrm.iplot(x, y=None, label=None, rows=1, cols=1,
         lg=None, overlay=False):
 ```
```

### Comparing `itrm-0.2.0/README.md` & `itrm-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 | ---------     | :-----------: | --------------------------------- |
 | `uni`         | `True`        | flag to use Unicode characters    |
 | `cols`        | `60`          | default column width              |
 | `rows`        | `20`          | default row height                |
 | `ar`          | `0.48`        | aspect ratio of characters        |
 
 There is also a method for changing the color map: `itrm.config.cmap()`. It
-takes a string: `"colors"`, `"grays"`, `"reds"`, `"greens"`, or `"blues"`.
+takes a string: `"colors"`, `"viridis"`, `"grays"`, `"reds"`, `"greens"`, or
+`"blues"`.
 
 ## Interactive Plots
 
 ```python
 itrm.iplot(x, y=None, label=None, rows=1, cols=1,
         lg=None, overlay=False):
 ```
```

### Comparing `itrm-0.2.0/setup.cfg` & `itrm-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = itrm
-version = 0.2.0
+version = 0.2.1
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Interactive Terminal Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/itrm
 classifiers =
```

### Comparing `itrm-0.2.0/src/itrm/itrm.py` & `itrm-0.2.1/src/itrm/itrm.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,42 +33,47 @@
 import time
 import math
 import numpy as np
 
 
 # Constants
 # (blue, green, yellow, orange, magenta, purple)
-DARK_COLORS = [33, 40, 220, 202, 201,  93]
-LITE_COLORS = [75, 82, 228, 214, 213, 135]
-DARK_GRAYS = [253, 250, 247, 244, 241, 238]
-LITE_GRAYS = [255, 252, 249, 246, 243, 240]
-DARK_REDS = [197, 196, 160, 124,  88, 52]
-LITE_REDS = [198, 197, 196, 160, 124, 88]
-DARK_GREENS = [47, 46, 40, 34, 28, 22]
-LITE_GREENS = [48, 47, 46, 40, 34, 28]
-DARK_BLUES = [27, 21, 20, 19, 18, 17]
-LITE_BLUES = [33, 27, 21, 20, 19, 18]
+DARK_COLORS  = [ 33,  40, 220, 202, 201,  93]
+LITE_COLORS  = [ 75,  82, 228, 214, 213, 135]
+DARK_VIRIDIS = [184, 113,  36,  30,  60,  53]
+LITE_VIRIDIS = [227, 156,  79,  73, 103,  96]
+DARK_GRAYS   = [253, 250, 247, 244, 241, 238]
+LITE_GRAYS   = [255, 252, 249, 246, 243, 240]
+DARK_REDS    = [197, 196, 160, 124,  88,  52]
+LITE_REDS    = [198, 197, 196, 160, 124,  88]
+DARK_GREENS  = [ 47,  46,  40,  34,  28,  22]
+LITE_GREENS  = [ 48,  47,  46,  40,  34,  28]
+DARK_BLUES   = [ 27,  21,  20,  19,  18,  17]
+LITE_BLUES   = [ 33,  27,  21,  20,  19,  18]
 COLOR_CNT = 6 # number of colors in the color map
 eps = 1e-32 # minimum magnitude
 
 
 class config: # configuration settings
     uni = True # flag to use Unicode characters
     cols = 60 # default column width
     rows = 20 # default row height
     ar = 0.48 # aspect ratio of characters
     darks = DARK_COLORS # dark color map
     lites = LITE_COLORS # light color map
-    
+
     def cmap(cmap="colors"):
         if not isinstance(cmap, str):
             raise ValueError(f"cmap must be a string: {cmap}")
         if cmap == "colors":
             config.darks = DARK_COLORS
             config.lites = LITE_COLORS
+        elif cmap == "viridis":
+            config.darks = DARK_VIRIDIS
+            config.lites = LITE_VIRIDIS
         elif cmap == "grays":
             config.darks = DARK_GRAYS
             config.lites = LITE_GRAYS
         elif cmap == "reds":
             config.darks = DARK_REDS
             config.lites = LITE_REDS
         elif cmap == "greens":
@@ -1876,7 +1881,41 @@
         for j in range(spc_len):
             print(r, end="", flush=True)
         if colorize:
             print("\x1b[0m", end="", flush=True)
 
     # Show the cursor.
     print("\x1b[?25h", end="", flush=True)
+
+
+def viridis_map():
+    """
+    Display the viridis color palette. The original RGB values came from
+    https://waldyrious.net/viridis-palette-generator/.
+    """
+
+    # Input colors.
+    vir = np.array([
+            [253, 231, 37],
+            [122, 209, 81],
+            [34, 168, 132],
+            [42, 120, 142],
+            [65, 68, 135],
+            [68, 1, 84]])
+
+    # Show dark colors.
+    for n in range(6):
+        r = int(5*vir[n, 0]/255)
+        g = int(5*vir[n, 1]/255)
+        b = int(5*vir[n, 2]/255)
+        c = 16 + 36*r + 6*g + b
+        print(f"\x1b[48;5;{c}m {c:03d} \x1b[0m ", end="")
+    print()
+
+    # Show dark colors.
+    for n in range(6):
+        r = int(5*vir[n, 0]/255 + 1)
+        g = int(5*vir[n, 1]/255 + 1)
+        b = int(5*vir[n, 2]/255 + 1)
+        c = 16 + 36*r + 6*g + b
+        print(f"\x1b[48;5;{c}m {c:03d} \x1b[0m ", end="")
+    print()
```

### Comparing `itrm-0.2.0/src/itrm.egg-info/PKG-INFO` & `itrm-0.2.1/src/itrm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itrm
-Version: 0.2.0
+Version: 0.2.1
 Summary: Interactive Terminal Utilities
 Home-page: https://gitlab.com/davidwoodburn/itrm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -55,15 +55,16 @@
 | ---------     | :-----------: | --------------------------------- |
 | `uni`         | `True`        | flag to use Unicode characters    |
 | `cols`        | `60`          | default column width              |
 | `rows`        | `20`          | default row height                |
 | `ar`          | `0.48`        | aspect ratio of characters        |
 
 There is also a method for changing the color map: `itrm.config.cmap()`. It
-takes a string: `"colors"`, `"grays"`, `"reds"`, `"greens"`, or `"blues"`.
+takes a string: `"colors"`, `"viridis"`, `"grays"`, `"reds"`, `"greens"`, or
+`"blues"`.
 
 ## Interactive Plots
 
 ```python
 itrm.iplot(x, y=None, label=None, rows=1, cols=1,
         lg=None, overlay=False):
 ```
```

