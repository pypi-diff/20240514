# Comparing `tmp/indipyclient-0.1.2.tar.gz` & `tmp/indipyclient-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.1.2.tar` & `indipyclient-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.2/LICENSE
--rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.2/README.md
--rw-r--r--   0        0        0      416 2024-05-13 19:28:53.000000 indipyclient-0.1.2/indipyclient/__init__.py
--rw-r--r--   0        0        0     4030 2024-05-09 13:19:51.000000 indipyclient-0.1.2/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.2/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    22033 2024-05-13 16:45:57.000000 indipyclient-0.1.2/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.2/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.2/indipyclient/console/windows.py
--rw-r--r--   0        0        0    26738 2024-05-03 13:06:57.000000 indipyclient-0.1.2/indipyclient/events.py
--rw-r--r--   0        0        0    33660 2024-05-13 11:23:49.000000 indipyclient-0.1.2/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16279 2024-05-03 09:59:43.000000 indipyclient-0.1.2/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.2/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-05-13 19:28:14.000000 indipyclient-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.3/README.md
+-rw-r--r--   0        0        0      416 2024-05-14 10:23:25.000000 indipyclient-0.1.3/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3520 2024-05-14 07:13:24.000000 indipyclient-0.1.3/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.3/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    22122 2024-05-14 07:04:08.000000 indipyclient-0.1.3/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.3/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.3/indipyclient/console/windows.py
+-rw-r--r--   0        0        0    26738 2024-05-03 13:06:57.000000 indipyclient-0.1.3/indipyclient/events.py
+-rw-r--r--   0        0        0    33660 2024-05-13 11:23:49.000000 indipyclient-0.1.3/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16279 2024-05-03 09:59:43.000000 indipyclient-0.1.3/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.3/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-14 10:23:12.000000 indipyclient-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.3/PKG-INFO
```

### Comparing `indipyclient-0.1.2/LICENSE` & `indipyclient-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/README.md` & `indipyclient-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/indipyclient/__main__.py` & `indipyclient-0.1.3/indipyclient/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,31 +16,15 @@
 
 from . import version
 
 from .console.consoleclient import ConsoleClient, ConsoleControl
 
 
 async def runclient(client, control):
-    "Run the client.asyncrun() and control.asyncrun() coroutines"
-    t1 = asyncio.create_task(client.asyncrun())
-    t2 = asyncio.create_task(control.asyncrun())
-    try:
-        await asyncio.gather(t1, t2)
-    except Exception:
-        # one task has raised an exception, shutdown and wait for the
-        # remaining task to shutdown
-        logger.exception("Exception report from  __main__.runclient coroutine")
-        # set flags in these classes requesting them to stop
-        client.shutdown()
-        control.shutdown()
-        while not t1.done():
-            await asyncio.sleep(0)
-        while not t2.done():
-            await asyncio.sleep(0)
-
+    await asyncio.gather(client.asyncrun(), control.asyncrun())
 
 
 def main():
     """The commandline entry point to run the terminal client."""
 
     parser = argparse.ArgumentParser(usage="indipyclient [options]",
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
@@ -96,14 +80,18 @@
             if level != loglevel:
                 print("Error: Failed to set logging")
                 return 1
         except:
             print("Error: If given, the loglevel should be 1, 2, 3 or 4")
             return 1
 
-    asyncio.run(runclient(client, control))
+    try:
+        asyncio.run(runclient(client, control))
+    finally:
+        # clear curses setup
+        control.console_reset()
 
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `indipyclient-0.1.2/indipyclient/console/consoleclient.py` & `indipyclient-0.1.3/indipyclient/console/consoleclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,27 +150,30 @@
     def shutdown(self):
         "Sets self._shutdown to True which shuts down the client"
         self._shutdown = True
 
 
     async def _checkshutdown(self):
         "If self._shutdown becomes True, shutdown"
-        while (not self._shutdown) and (not self.client.stopped):
+        while (not self._shutdown) and (not self.client.stopped) and (not self.stop):
+            # no shutdown requested, just continue
             await asyncio.sleep(0)
         # so either shutdown has been requested or the ipyclient has stopped for some reason
-        self._shutdown = True
         if not self.client.stopped:
             # client is still running, shut it down
             self.client.report("Shutting down client - please wait")
             self.client.shutdown()
         # Now stop console co-routines
         self.stop = True
         while (not self.updatescreenstopped) and (not self.getinputstopped):
             await asyncio.sleep(0)
-        # async tasks finished, clear up the terminal
+
+
+    def console_reset(self):
+        "Resets console, called in finally clause at program shutdown"
         curses.nocbreak()
         self.stdscr.keypad(False)
         curses.curs_set(1)
         curses.echo()
         curses.endwin()
```

### Comparing `indipyclient-0.1.2/indipyclient/console/widgets.py` & `indipyclient-0.1.3/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/indipyclient/console/windows.py` & `indipyclient-0.1.3/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/indipyclient/events.py` & `indipyclient-0.1.3/indipyclient/events.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/indipyclient/ipyclient.py` & `indipyclient-0.1.3/indipyclient/ipyclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/indipyclient/propertymembers.py` & `indipyclient-0.1.3/indipyclient/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/indipyclient/propertyvectors.py` & `indipyclient-0.1.3/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.2/pyproject.toml` & `indipyclient-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.1.2"
+version = "0.1.3"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.1.2/PKG-INFO` & `indipyclient-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

