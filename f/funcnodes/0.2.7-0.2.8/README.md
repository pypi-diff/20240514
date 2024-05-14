# Comparing `tmp/funcnodes-0.2.7.tar.gz` & `tmp/funcnodes-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes-0.2.7.tar", max compression
+gzip compressed data, was "funcnodes-0.2.8.tar", max compression
```

## Comparing `funcnodes-0.2.7.tar` & `funcnodes-0.2.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1787 2024-05-14 09:23:48.926561 funcnodes-0.2.7/funcnodes/__init__.py
--rw-r--r--   0        0        0     6499 2024-05-07 08:28:48.305494 funcnodes-0.2.7/funcnodes/__main__.py
--rw-r--r--   0        0        0     2032 2024-05-06 20:07:59.075924 funcnodes-0.2.7/funcnodes/_logging.py
--rw-r--r--   0        0        0      278 2024-05-14 07:14:15.014932 funcnodes-0.2.7/funcnodes/basic_nodes/__init__.py
--rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.7/funcnodes/basic_nodes/logic.py
--rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.7/funcnodes/basic_nodes/math.py
--rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.7/funcnodes/config.py
--rw-r--r--   0        0        0     1911 2024-05-08 18:44:35.771663 funcnodes-0.2.7/funcnodes/data.py
--rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.7/funcnodes/eventmanager.py
--rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.7/funcnodes/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.7/funcnodes/frontends/__init__.py
--rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/asset-manifest.json
--rw-r--r--   0        0        0    29231 2024-05-14 07:55:51.314737 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/css/style.css
--rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/favicon.ico
--rw-r--r--   0        0        0      763 2024-05-14 08:01:24.659745 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/index.html
--rw-r--r--   0        0        0  4149018 2024-05-14 07:55:51.316736 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/743.js
--rw-r--r--   0        0        0     3258 2024-05-14 07:55:51.313726 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt
--rw-r--r--   0        0        0   256239 2024-05-14 07:55:51.314737 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/main.js
--rw-r--r--   0        0        0    11501 2024-05-14 07:55:51.314737 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
--rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/logo192.png
--rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/logo512.png
--rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/manifest.json
--rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/robots.txt
--rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/run.py
--rw-r--r--   0        0        0      323 2024-05-10 14:51:11.297311 funcnodes-0.2.7/funcnodes/graph.py
--rw-r--r--   0        0        0    28831 2024-05-14 09:16:23.727798 funcnodes-0.2.7/funcnodes/io.py
--rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.7/funcnodes/lib/__init__.py
--rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.7/funcnodes/lib/lib.py
--rw-r--r--   0        0        0     7259 2024-05-11 04:44:57.813753 funcnodes-0.2.7/funcnodes/lib/libfinder.py
--rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.7/funcnodes/lib/libparser.py
--rw-r--r--   0        0        0    33041 2024-05-14 09:16:20.326639 funcnodes-0.2.7/funcnodes/node.py
--rw-r--r--   0        0        0    20423 2024-05-14 07:16:32.158888 funcnodes-0.2.7/funcnodes/nodemaker.py
--rw-r--r--   0        0        0    11850 2024-05-11 05:25:23.856740 funcnodes-0.2.7/funcnodes/nodespace.py
--rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.7/funcnodes/triggerstack.py
--rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.7/funcnodes/utils/__init__.py
--rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.7/funcnodes/utils/data.py
--rw-r--r--   0        0        0     2744 2024-05-14 07:12:12.066097 funcnodes-0.2.7/funcnodes/utils/nodeutils.py
--rw-r--r--   0        0        0     5994 2024-05-14 09:16:47.009589 funcnodes-0.2.7/funcnodes/utils/serialization.py
--rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.7/funcnodes/worker/__init__.py
--rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.7/funcnodes/worker/external_worker.py
--rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.7/funcnodes/worker/loop.py
--rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.7/funcnodes/worker/remote_worker.py
--rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.7/funcnodes/worker/websocket.py
--rw-r--r--   0        0        0    38084 2024-05-14 08:52:44.600896 funcnodes-0.2.7/funcnodes/worker/worker.py
--rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.7/funcnodes/worker/worker_manager.py
--rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.7/LICENSE
--rw-r--r--   0        0        0      669 2024-05-14 09:23:33.563681 funcnodes-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.7/README.md
--rw-r--r--   0        0        0    13490 1970-01-01 00:00:00.000000 funcnodes-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1787 2024-05-14 12:52:21.747900 funcnodes-0.2.8/funcnodes/__init__.py
+-rw-r--r--   0        0        0     6736 2024-05-14 12:22:29.469309 funcnodes-0.2.8/funcnodes/__main__.py
+-rw-r--r--   0        0        0     2476 2024-05-14 12:14:27.351209 funcnodes-0.2.8/funcnodes/_logging.py
+-rw-r--r--   0        0        0      278 2024-05-14 07:14:15.014932 funcnodes-0.2.8/funcnodes/basic_nodes/__init__.py
+-rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.8/funcnodes/basic_nodes/logic.py
+-rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.8/funcnodes/basic_nodes/math.py
+-rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.8/funcnodes/config.py
+-rw-r--r--   0        0        0     1911 2024-05-08 18:44:35.771663 funcnodes-0.2.8/funcnodes/data.py
+-rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.8/funcnodes/eventmanager.py
+-rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.8/funcnodes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.8/funcnodes/frontends/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/asset-manifest.json
+-rw-r--r--   0        0        0    29231 2024-05-14 07:55:51.314737 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/css/style.css
+-rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/favicon.ico
+-rw-r--r--   0        0        0      763 2024-05-14 08:01:24.659745 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/index.html
+-rw-r--r--   0        0        0  4149018 2024-05-14 07:55:51.316736 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js
+-rw-r--r--   0        0        0     3258 2024-05-14 07:55:51.313726 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt
+-rw-r--r--   0        0        0   256239 2024-05-14 07:55:51.314737 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js
+-rw-r--r--   0        0        0    11501 2024-05-14 07:55:51.314737 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
+-rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo192.png
+-rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo512.png
+-rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/manifest.json
+-rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/robots.txt
+-rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/run.py
+-rw-r--r--   0        0        0      323 2024-05-10 14:51:11.297311 funcnodes-0.2.8/funcnodes/graph.py
+-rw-r--r--   0        0        0    29347 2024-05-14 10:50:19.461839 funcnodes-0.2.8/funcnodes/io.py
+-rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.8/funcnodes/lib/__init__.py
+-rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.8/funcnodes/lib/lib.py
+-rw-r--r--   0        0        0     7259 2024-05-11 04:44:57.813753 funcnodes-0.2.8/funcnodes/lib/libfinder.py
+-rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.8/funcnodes/lib/libparser.py
+-rw-r--r--   0        0        0    35376 2024-05-14 12:54:42.228979 funcnodes-0.2.8/funcnodes/node.py
+-rw-r--r--   0        0        0    20423 2024-05-14 07:16:32.158888 funcnodes-0.2.8/funcnodes/nodemaker.py
+-rw-r--r--   0        0        0    11850 2024-05-11 05:25:23.856740 funcnodes-0.2.8/funcnodes/nodespace.py
+-rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.8/funcnodes/triggerstack.py
+-rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.8/funcnodes/utils/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.8/funcnodes/utils/data.py
+-rw-r--r--   0        0        0     2744 2024-05-14 07:12:12.066097 funcnodes-0.2.8/funcnodes/utils/nodeutils.py
+-rw-r--r--   0        0        0     5994 2024-05-14 09:16:47.009589 funcnodes-0.2.8/funcnodes/utils/serialization.py
+-rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.8/funcnodes/worker/__init__.py
+-rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.8/funcnodes/worker/external_worker.py
+-rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.8/funcnodes/worker/loop.py
+-rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.8/funcnodes/worker/remote_worker.py
+-rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.8/funcnodes/worker/websocket.py
+-rw-r--r--   0        0        0    38268 2024-05-14 12:15:05.691889 funcnodes-0.2.8/funcnodes/worker/worker.py
+-rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.8/funcnodes/worker/worker_manager.py
+-rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.8/LICENSE
+-rw-r--r--   0        0        0      694 2024-05-14 12:52:09.360725 funcnodes-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.8/README.md
+-rw-r--r--   0        0        0    13535 1970-01-01 00:00:00.000000 funcnodes-0.2.8/PKG-INFO
```

### Comparing `funcnodes-0.2.7/funcnodes/__init__.py` & `funcnodes-0.2.8/funcnodes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,10 +65,10 @@
     "config",
     "RenderOptions",
     "NoValue",
     "DataEnum",
     "add_type",
 ]
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 DEBUG = True
```

### Comparing `funcnodes-0.2.7/funcnodes/__main__.py` & `funcnodes-0.2.8/funcnodes/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Type
 from funcnodes.frontends.funcnodes_react import run_server
 import funcnodes as fn
 import argparse
 from pprint import pprint
 import sys
 import os
+import setproctitle
 
 
 def task_run_server(args: argparse.Namespace):
     """
     Runs the server.
 
     Args:
@@ -17,14 +18,15 @@
     Returns:
       None
 
     Examples:
       >>> task_run_server(args)
       None
     """
+    setproctitle.setproctitle("funcnodes_server")
     run_server(port=args.port, open_browser=args.no_browser)
 
 
 def list_workers(args: argparse.Namespace):
     """
     Lists all workers.
 
@@ -60,14 +62,15 @@
       >>> start_new_worker(args)
       None
     """
     worker_class: Type[fn.worker.Worker] = getattr(fn.worker, args.workertype)
     fn.FUNCNODES_LOGGER.info(f"Starting new worker of type {args.workertype}")
 
     worker = worker_class(uuid=args.uuid, name=args.name)
+    setproctitle.setproctitle("worker " + worker.uuid())
     worker.run_forever()
 
 
 def start_existing_worker(args: argparse.Namespace):
     """
     Starts an existing worker.
 
@@ -116,14 +119,15 @@
         if not os.path.exists(cfg["python_path"]):
             raise Exception(f"Python executable not found: {cfg['python_path']}")
         os.execv(cfg["python_path"], ["-m", "funcnodes"] + sys.argv[1:])
 
     fn.FUNCNODES_LOGGER.info(f"Starting existing worker of type {args.workertype}")
     worker = worker_class(uuid=cfg["uuid"])
 
+    setproctitle.setproctitle("worker " + worker.uuid())
     worker.run_forever()
 
 
 def task_worker(args: argparse.Namespace):
     """
     Performs a task on worker(s).
 
@@ -162,14 +166,15 @@
     Returns:
       None
 
     Examples:
       >>> start_worker_manager(args)
       None
     """
+    setproctitle.setproctitle("worker_manager")
     fn.worker.worker_manager.start_worker_manager()
 
 
 def main():
     """
     The main function.
```

### Comparing `funcnodes-0.2.7/funcnodes/_logging.py` & `funcnodes-0.2.8/funcnodes/_logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 FUNCNODES_LOGGER = logging.getLogger("funcnodes")
 
 FUNCNODES_LOGGER.setLevel(logging.DEBUG)
 
 
 ch = logging.StreamHandler()
-fh = RotatingFileHandler(
-    os.path.join(LOGGINGDIR, "funcnodes.log"), maxBytes=1024 * 1024 * 5, backupCount=5
-)
+
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
 # Add the handler to the logger
 
 
 def _overwrite_add_handler(logger):
     """
@@ -34,36 +32,54 @@
     Examples:
       >>> _overwrite_add_handler(FUNCNODES_LOGGER)
     """
     _old_add_handler = logger.addHandler
 
     def _new_add_handler(hdlr):
         """
-    Adds a handler to the given logger.
+        Adds a handler to the given logger.
 
-    Args:
-      hdlr (Handler): The handler to add to the logger.
+        Args:
+          hdlr (Handler): The handler to add to the logger.
 
-    Returns:
-      None.
+        Returns:
+          None.
 
-    Examples:
-      >>> _new_add_handler(ch)
-    """
+        Examples:
+          >>> _new_add_handler(ch)
+        """
         hdlr.setFormatter(formatter)
         if hdlr not in logger.handlers:
             _old_add_handler(hdlr)
 
     logger.addHandler = _new_add_handler
 
 
 _overwrite_add_handler(FUNCNODES_LOGGER)
 
 FUNCNODES_LOGGER.addHandler(ch)
-FUNCNODES_LOGGER.addHandler(fh)
+
+
+def set_logging_dir(path):
+    if not os.path.exists(path):
+        os.makedirs(path)
+    for hdlr in FUNCNODES_LOGGER.handlers:
+        if isinstance(hdlr, RotatingFileHandler):
+            if hdlr.baseFilename.endswith("funcnodes.log"):
+                hdlr.close()
+                FUNCNODES_LOGGER.removeHandler(hdlr)
+
+    fh = RotatingFileHandler(
+        os.path.join(path, "funcnodes.log"), maxBytes=1024 * 1024 * 5, backupCount=5
+    )
+    fh.setFormatter(formatter)
+    FUNCNODES_LOGGER.addHandler(fh)
+
+
+set_logging_dir(LOGGINGDIR)
 
 
 def get_logger(name, propagate=True):
     """
     Returns a logger with the given name.
 
     Args:
```

### Comparing `funcnodes-0.2.7/funcnodes/basic_nodes/logic.py` & `funcnodes-0.2.8/funcnodes/basic_nodes/logic.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/basic_nodes/math.py` & `funcnodes-0.2.8/funcnodes/basic_nodes/math.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/config.py` & `funcnodes-0.2.8/funcnodes/config.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/data.py` & `funcnodes-0.2.8/funcnodes/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/eventmanager.py` & `funcnodes-0.2.8/funcnodes/eventmanager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/asset-manifest.json` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/css/style.css` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/css/style.css`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/favicon.ico` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/favicon.ico`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/index.html` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/index.html`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/743.js` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/743.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/main.js` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/logo192.png` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo192.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/logo512.png` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/logo512.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/frontends/funcnodes_react/run.py` & `funcnodes-0.2.8/funcnodes/frontends/funcnodes_react/run.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/io.py` & `funcnodes-0.2.8/funcnodes/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,14 +371,23 @@
             ser["description"] = self._description
         if (
             self.allow_multiple is not None
             and self.allow_multiple is not self.default_allow_multiple
         ):
             ser["allow_multiple"] = self.allow_multiple
 
+        if ser["name"] == ser["id"]:
+            del ser["name"]
+
+        if len(ser["render_options"]) == 0:
+            del ser["render_options"]
+
+        if len(ser["value_options"]) == 0:
+            del ser["value_options"]
+
         return ser
 
     @property
     def name(self) -> str:
         """Gets the name of the NodeIO."""
         return self._name
 
@@ -556,38 +565,42 @@
             type=self._typestr,
             description=self._description,
             uuid=self.uuid,
         )
         if self._allow_multiple is not None:
             ser["allow_multiple"] = self._allow_multiple
 
+        if ser["name"] == ser["uuid"]:
+            del ser["name"]
         return ser
 
     def full_serialize(self) -> FullNodeIOJSON:
         """Generates a JSON serializable dictionary of the NodeIO.
 
         Returns
         -------
         FullNodeIOJSON:
             JSON serializable dictionary of the NodeIO
         """
-        return FullNodeIOJSON(
+        ser = FullNodeIOJSON(
             id=self.uuid,
             full_id=self.full_id,
             name=self.name,
             type=self._typestr,
             is_input=self.is_input(),
             connected=self.is_connected(),
             node=self.node.uuid if self.node else None,
             value=self.value,
             does_trigger=self.does_trigger,
             render_options=self.render_options,
             value_options=self.value_options,
         )
 
+        return ser
+
     def _repr_json_(self) -> FullNodeIOJSON:
         return JSONEncoder.apply_custom_encoding(self.full_serialize(), preview=False)  # type: ignore
 
     @property
     def allow_multiple(self) -> bool:
         """
         Indicates whether this NodeInput allows multiple connections.
@@ -731,14 +744,19 @@
         )
         if self.required is not NodeInput.default_required:
             ser["required"] = self.required
         if self.does_trigger is not NodeInput.default_does_trigger:
             ser["does_trigger"] = self.does_trigger
         if self._default is not NoValue:
             ser["default"] = self._default
+        if (
+            self.value != self.default
+            and not self.is_connected()  # value is stored only if not connected
+        ):
+            ser["value"] = self.value
         return ser
 
     def to_dict(self) -> NodeInputOptions:
         ser: IOOptions = NodeInputOptions(
             **self.serialize(),
         )
         return ser
```

### Comparing `funcnodes-0.2.7/funcnodes/lib/lib.py` & `funcnodes-0.2.8/funcnodes/lib/lib.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/lib/libfinder.py` & `funcnodes-0.2.8/funcnodes/lib/libfinder.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/lib/libparser.py` & `funcnodes-0.2.8/funcnodes/lib/libparser.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/node.py` & `funcnodes-0.2.8/funcnodes/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 from .utils import (
     run_until_complete,
     deep_fill_dict,
     deep_remove_dict_on_equal,
 )
 from logging import getLogger
-from funcnodes._logging import get_logger
+from funcnodes._logging import get_logger, FUNCNODES_LOGGER
 
 triggerlogger = get_logger("trigger")
 
 
 class NodeTriggerError(Exception):
     @classmethod
     def from_error(cls, error: Exception):
@@ -71,17 +71,20 @@
     nodeclass = node if isinstance(node, type) else node.__class__
     classattr = list(nodeclass.__dict__.keys())
     for attr_name in dir(node):
         if attr_name not in classattr:
             classattr.append(attr_name)
 
     for attr_name in classattr:
-        attr = getattr(node, attr_name)
-        if isinstance(attr, NodeInput):
-            inputs.append(attr)
+        try:
+            attr = getattr(node, attr_name)
+            if isinstance(attr, NodeInput):
+                inputs.append(attr)
+        except AttributeError:
+            pass
     return inputs
 
 
 def _get_nodeclass_outputs(node: Type[Node] | Node) -> List[NodeOutput]:
     """
     Iterates over the attributes of a Node instance and returns the ones that are instances of NodeOutput.
 
@@ -95,17 +98,20 @@
     nodeclass = node if isinstance(node, type) else node.__class__
     classattr = list(nodeclass.__dict__.keys())
     for attr_name in dir(node):
         if attr_name not in classattr:
             classattr.append(attr_name)
 
     for attr_name in classattr:
-        attr = getattr(node, attr_name)
-        if isinstance(attr, NodeOutput):
-            outputs.append(attr)
+        try:
+            attr = getattr(node, attr_name)
+            if isinstance(attr, NodeOutput):
+                outputs.append(attr)
+        except AttributeError:
+            pass
     return outputs
 
 
 def _parse_nodeclass_io(node: Node):
     """
     Iterates over the attributes of a Node instance and parses the ones that are instances of NodeInput or NodeOutput.
     It then adds these as inputs or outputs to the class instance.
@@ -130,14 +136,15 @@
         if node_io_render:
             deep_fill_dict(
                 ser["render_options"], node_io_render, overwrite_existing=True
             )
 
         if node_io_options:
             deep_fill_dict(ser, node_io_options, overwrite_existing=True)
+
         node.add_input(
             NodeInput(
                 **ser,
             )
         )
 
     for op in outputs:
@@ -285,18 +292,43 @@
         id="_triggerinput",
         name="( )",
         description="Trigger the node",
         default=None,
         required=False,
     )
 
+    _class_io_serialized: Dict[str, NodeIOSerialization]
+
     @abstractmethod
     async def func(self, *args, **kwargs):
         """The function to be executed when the node is triggered."""
 
+    def __init_subclass__(cls, **kwargs):
+        ips = _get_nodeclass_inputs(cls)
+        ops = _get_nodeclass_outputs(cls)
+
+        cls._class_io_serialized: Dict[str, NodeIOSerialization] = {}
+
+        for io in ips + ops:
+            ipser = io.serialize()
+
+            # check if it is present in the previous
+            while ipser["id"] in cls._class_io_serialized:
+                io._uuid = io.uuid + "_"
+
+                FUNCNODES_LOGGER.warning(
+                    "IO with id %s already exists in %s. Changing id to %s",
+                    ipser["id"],
+                    cls,
+                    io.uuid,
+                )
+                ipser = io.serialize()
+
+            cls._class_io_serialized[ipser["id"]] = ipser
+
     def __init__(
         self,
         uuid: Optional[str] = None,
         reset_inputs_on_trigger: Optional[bool] = None,
         name: Optional[str] = None,
         id: Optional[str] = None,  # fallback for uuid
         render_options: Optional[RenderOptions] = None,
@@ -345,15 +377,15 @@
             inputs=[
                 ip.serialize_class()
                 for ip in _get_nodeclass_inputs(cls)
                 if ip.uuid != "_triggerinput"
             ],
             outputs=[op.serialize_class() for op in _get_nodeclass_outputs(cls)],
             description=cls.description,
-            node_name=cls.node_name,
+            node_name=getattr(cls, "node_name", cls.__name__),
         )
         if cls.default_reset_inputs_on_trigger != Node.default_reset_inputs_on_trigger:
             ser["reset_inputs_on_trigger"] = cls.default_reset_inputs_on_trigger
 
         return ser
 
     def full_serialize(self) -> FullNodeJSON:
@@ -407,22 +439,55 @@
         returns a json serializable dict of the node
         """
 
         ser = NodeJSON(
             name=self.name,
             id=self.uuid,
             node_id=self.node_id,
-            node_name=self.node_name,
-            io={
-                iod.uuid: iod.serialize()
-                for iod in self._inputs + self._outputs
-                if iod.uuid != "_triggerinput"
-            },
+            node_name=getattr(self, "node_name", self.__class__.__name__),
+            io={},
         )
 
+        for iod in self._inputs + self._outputs:
+            if iod.uuid == "_triggerinput":
+                continue
+            ioser = dict(iod.serialize())
+            del ioser["id"]
+
+            cls_ser = None
+            if iod.uuid in self._class_io_serialized:
+                cls_ser = self._class_io_serialized[iod.uuid]
+
+            if cls_ser:
+                if "description" in ioser:
+                    if ioser["description"] == cls_ser.get("description", ""):
+                        del ioser["description"]
+
+                if "default" in ioser:
+                    if ioser["default"] == cls_ser.get("default", NoValue):
+                        del ioser["default"]
+
+                if "type" in ioser:
+                    if ioser["type"] == cls_ser.get("type", "Any"):
+                        del ioser["type"]
+
+                if "value_options" in ioser:
+                    if ioser["value_options"] == cls_ser.get("value_options", {}):
+                        del ioser["value_options"]
+
+                if "render_options" in ioser:
+                    if ioser["render_options"] == cls_ser.get("render_options", {}):
+                        del ioser["render_options"]
+
+                if "default" in ioser:
+                    if ioser["default"] == cls_ser.get("default", NoValue):
+                        del ioser["default"]
+
+            ser["io"][iod.uuid] = ioser
+
         if self.reset_inputs_on_trigger != self.default_reset_inputs_on_trigger:
             ser["reset_inputs_on_trigger"] = self.reset_inputs_on_trigger
 
         if self.description != self.__class__.description:
             ser["description"] = self.description
 
         renderopt = self.render_options
```

### Comparing `funcnodes-0.2.7/funcnodes/nodemaker.py` & `funcnodes-0.2.8/funcnodes/nodemaker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/nodespace.py` & `funcnodes-0.2.8/funcnodes/nodespace.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/triggerstack.py` & `funcnodes-0.2.8/funcnodes/triggerstack.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/utils/data.py` & `funcnodes-0.2.8/funcnodes/utils/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/utils/nodeutils.py` & `funcnodes-0.2.8/funcnodes/utils/nodeutils.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/utils/serialization.py` & `funcnodes-0.2.8/funcnodes/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/worker/external_worker.py` & `funcnodes-0.2.8/funcnodes/worker/external_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/worker/loop.py` & `funcnodes-0.2.8/funcnodes/worker/loop.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/worker/remote_worker.py` & `funcnodes-0.2.8/funcnodes/worker/remote_worker.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/worker/websocket.py` & `funcnodes-0.2.8/funcnodes/worker/websocket.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/funcnodes/worker/worker.py` & `funcnodes-0.2.8/funcnodes/worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Node,
     NodeJSON,
     JSONEncoder,
     JSONDecoder,
     NodeClassNotFoundError,
     NodeOutput,
     NodeInput,
+    NoValue,
 )
 from funcnodes.utils import deep_fill_dict
 from funcnodes.lib import find_shelf, ShelfDict
 import traceback
 from exposedfunctionality import exposed_method, get_exposed_methods
 from typing_extensions import deprecated
 
@@ -568,14 +569,15 @@
             os.path.abspath(data_path)
             if data_path
             else os.path.join(
                 funcnodes.config.CONFIG_DIR, "workers", "worker_" + self._uuid
             )
         )
         self.data_path = self._data_path
+        funcnodes._logging.set_logging_dir(self.data_path)
         self.logger = funcnodes.get_logger(self._uuid, propagate=False)
         self.logger.addHandler(
             RotatingFileHandler(
                 os.path.join(self.data_path, "worker.log"),
                 maxBytes=100000,
                 backupCount=5,
             )
@@ -1018,15 +1020,17 @@
     def remove_node(self, id: str) -> str:
         return self.nodespace.remove_node_by_id(id)
 
     @exposed_method()
     def set_io_value(self, nid: str, ioid: str, value: Any, set_default: bool = False):
         node = self.get_node(nid)
         io = node.get_input(ioid)
-        if set_default:
+        if (
+            set_default and value != NoValue
+        ):  # novalue should not be set automatically as default via io set
             io.set_default(value)
         io.set_value(value)
 
         return io.value
 
     @exposed_method()
     def get_io_value(self, nid: str, ioid: str):
@@ -1035,17 +1039,17 @@
         return io.value
 
     @exposed_method()
     def trigger_node(self, nid: str):
         node = self.get_node(nid)
         node.request_trigger()
         return True
-    
+
     @exposed_method()
-    def get_node_status(self,nid:str):
+    def get_node_status(self, nid: str):
         node = self.get_node(nid)
         return node.status()
 
     @requests_save
     @exposed_method()
     def set_default_value(self, nid: str, ioid: str, value: Any):
         node = self.get_node(nid)
```

### Comparing `funcnodes-0.2.7/funcnodes/worker/worker_manager.py` & `funcnodes-0.2.8/funcnodes/worker/worker_manager.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/LICENSE` & `funcnodes-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/pyproject.toml` & `funcnodes-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "funcnodes"
-version = "0.2.7"
+version = "0.2.8"
 description = "funcnodes"
 authors = ["Julian Kimmig <julian.kimmig@linkdlab.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 exposedfunctionality = ">=0.3.7"
 websockets = "^12.0"
 virtualenv = "*"
 poetry-plugin-export = "^1.7"
 python-dotenv = "*"
 poetry = "*" 
 
 networkx = "^3.3"
+setproctitle = "^1.3.3"
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 coverage = "*"
 pandas = "^2.2"
 pillow = "^10.2"
 opencv-python = "^4.9"
 vulture = "^2.11"
```

### Comparing `funcnodes-0.2.7/README.md` & `funcnodes-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2.7/PKG-INFO` & `funcnodes-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: funcnodes
-Version: 0.2.7
+Version: 0.2.8
 Summary: funcnodes
 Author: Julian Kimmig
 Author-email: julian.kimmig@linkdlab.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: exposedfunctionality (>=0.3.7)
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: poetry
 Requires-Dist: poetry-plugin-export (>=1.7,<2.0)
 Requires-Dist: python-dotenv
+Requires-Dist: setproctitle (>=1.3.3,<2.0.0)
 Requires-Dist: virtualenv
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 # Funcnodes Project README
 
 ## Project Overview
```

