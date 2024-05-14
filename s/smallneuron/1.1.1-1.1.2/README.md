# Comparing `tmp/smallneuron-1.1.1.tar.gz` & `tmp/smallneuron-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallneuron-1.1.1.tar", last modified: Fri Apr 26 20:44:57 2024, max compression
+gzip compressed data, was "smallneuron-1.1.2.tar", last modified: Tue May 14 20:54:50 2024, max compression
```

## Comparing `smallneuron-1.1.1.tar` & `smallneuron-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.989407 smallneuron-1.1.1/
--rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.1/.gitignore
--rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.1/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-26 20:44:57.989407 smallneuron-1.1.1/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-14 21:53:34.000000 smallneuron-1.1.1/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.1/example.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-04-26 20:35:05.000000 smallneuron-1.1.1/pyproject.toml
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-04-26 20:44:57.989407 smallneuron-1.1.1/setup.cfg
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.985407 smallneuron-1.1.1/src/
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.985407 smallneuron-1.1.1/src/smallneuron/
--rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/__init__.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/build
--rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/gpio_h3.c
--rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/gpio_h3.h
--rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron/gpio_h3.so
--rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.1/src/smallneuron/logger.py
--rw-rw-r--   0 andres    (1000) andres    (1000)    13916 2024-04-19 22:22:47.000000 smallneuron-1.1.1/src/smallneuron/smallneuron.py
--rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.1/src/smallneuron/snapi.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/sndummy.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.1/src/smallneuron/sngpio.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/sninput.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/snmqtt.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     3048 2024-04-26 20:35:05.000000 smallneuron-1.1.1/src/smallneuron/snserial.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.1/src/smallneuron/sntimer.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.989407 smallneuron-1.1.1/src/smallneuron.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-04-26 20:44:57.000000 smallneuron-1.1.1/src/smallneuron.egg-info/top_level.txt
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-04-26 20:44:57.985407 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.790821 smallneuron-1.1.2/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      441 2024-02-20 00:54:30.000000 smallneuron-1.1.2/.gitignore
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1074 2024-02-18 18:56:34.000000 smallneuron-1.1.2/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 20:54:50.790821 smallneuron-1.1.2/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      753 2024-04-26 21:59:55.000000 smallneuron-1.1.2/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3645 2024-04-14 20:50:42.000000 smallneuron-1.1.2/example.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      655 2024-05-14 20:53:12.000000 smallneuron-1.1.2/pyproject.toml
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2024-05-14 20:54:50.790821 smallneuron-1.1.2/setup.cfg
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.782821 smallneuron-1.1.2/src/
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.786821 smallneuron-1.1.2/src/smallneuron/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      242 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/__init__.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)      231 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/build
+-rw-rw-r--   0 andres    (1000) andres    (1000)    21308 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/gpio_h3.c
+-rw-rw-r--   0 andres    (1000) andres    (1000)     7411 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/gpio_h3.h
+-rwxrwxr-x   0 andres    (1000) andres    (1000)    26760 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron/gpio_h3.so
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1388 2024-04-17 20:53:40.000000 smallneuron-1.1.2/src/smallneuron/logger.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)    13970 2024-05-13 15:29:30.000000 smallneuron-1.1.2/src/smallneuron/smallneuron.py
+-rwxrwxr-x   0 andres    (1000) andres    (1000)     4503 2024-04-23 16:54:05.000000 smallneuron-1.1.2/src/smallneuron/snapi.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1066 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/sndummy.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1472 2024-04-14 22:44:26.000000 smallneuron-1.1.2/src/smallneuron/sngpio.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3011 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/sninput.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     2350 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/snmqtt.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     3094 2024-05-14 20:50:23.000000 smallneuron-1.1.2/src/smallneuron/snserial.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      985 2024-04-14 22:54:22.000000 smallneuron-1.1.2/src/smallneuron/sntimer.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.786821 smallneuron-1.1.2/src/smallneuron.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1247 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      774 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-05-14 20:54:50.000000 smallneuron-1.1.2/src/smallneuron.egg-info/top_level.txt
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2024-05-14 20:54:50.786821 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1062 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      496 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       12 2024-02-18 18:56:34.000000 smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/top_level.txt
```

### Comparing `smallneuron-1.1.1/LICENSE` & `smallneuron-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/PKG-INFO` & `smallneuron-1.1.2/src/smallneuron_pelainux.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smallneuron
-Version: 1.1.1
+Name: smallneuron_pelainux
+Version: 0.1.4
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,16 +31,12 @@
 # Install tools
 sudo apt install python3-pip python3-venv
 python3 -m pip install build # pip3 install build
 
 
 # Build
 python3 -m build
-python3 -m twine upload --repository testpypi dist/* # test
-python3 -m twine upload  dist/*                      # prod
-
+python3 -m twine upload --repository testpypi dist/*
 
 # Install
 Installing module
-	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux    # test
-  
-  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.0.0 # prod
+	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux
```

### Comparing `smallneuron-1.1.1/README.md` & `smallneuron-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 python3 -m twine upload  dist/*                      # prod
 
 
 # Install
 Installing module
 	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux    # test
   
-  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.0.0 # prod
+  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.1.1 # prod
```

### Comparing `smallneuron-1.1.1/example.py` & `smallneuron-1.1.2/example.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/pyproject.toml` & `smallneuron-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 
 [project]
 name = "smallneuron"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Andres Artigas", email="andres@artigas.cl" },
 ]
 description = "Small Neuron Workflow"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smallneuron-1.1.1/src/smallneuron/gpio_h3.c` & `smallneuron-1.1.2/src/smallneuron/gpio_h3.c`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/gpio_h3.h` & `smallneuron-1.1.2/src/smallneuron/gpio_h3.h`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/gpio_h3.so` & `smallneuron-1.1.2/src/smallneuron/gpio_h3.so`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/logger.py` & `smallneuron-1.1.2/src/smallneuron/logger.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/smallneuron.py` & `smallneuron-1.1.2/src/smallneuron/smallneuron.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         log.notice("*** STARTED ***")
 
     def putEvent(self, event, params=None):  # lanzamos un evento ahora
         #print("pushEvent:", event, "params:", params) 
         if params == None:
             params = {}
 
-        self.events.put((event, params, {}))
+        self.events.put((event, params, {})) # TODO: parece el el tercer argumento no se usa nunca
 
     def watchEvent(self,event, event_args={}, event_pattern=None, 
                 bridge=None, bridge_args={}, mode="loop",period=1):
                 watcher=SnWatcher(self,event,event_args, event_pattern)
                 watcher.run(bridge,bridge_args,mode,period)
                 return watcher
```

### Comparing `smallneuron-1.1.1/src/smallneuron/snapi.py` & `smallneuron-1.1.2/src/smallneuron/snapi.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/sndummy.py` & `smallneuron-1.1.2/src/smallneuron/sndummy.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/sngpio.py` & `smallneuron-1.1.2/src/smallneuron/sngpio.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/sninput.py` & `smallneuron-1.1.2/src/smallneuron/sninput.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/snmqtt.py` & `smallneuron-1.1.2/src/smallneuron/snmqtt.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron/snserial.py` & `smallneuron-1.1.2/src/smallneuron/snserial.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 def eventWait(snserial):
     try:
         log.info("reader started")
         fails=0
         while True:
             try:
+                if not snserial.isOpen():
+                    snserial.rotateOpen()
                 line = snserial.read_until(snserial.eol)
                 fails=0
                 for e in snserial.events:
                     if re.search(e[1], line) != None:
                         if snserial.eventManager == None:
                             log.error("Warning eventManager not defined")
                         else:
@@ -34,15 +36,14 @@
             except Exception as e:
                 fails=fails+1
                 if fails > 10:
                     raise("Falla multiples veces lectura serial "+str(fails))
                 log.error("Reintentamos lectura "+str(e) )
                 time.sleep(1)
                 snserial.close()
-                snserial.rotateOpen()
                 
     except Exception as e:
         log.error(e)
         log.error(traceback.format_exc())
         snserial.eventManager.putEvent("panic", str(e))
```

### Comparing `smallneuron-1.1.1/src/smallneuron/sntimer.py` & `smallneuron-1.1.2/src/smallneuron/sntimer.py`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron.egg-info/PKG-INFO` & `smallneuron-1.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallneuron
-Version: 1.1.1
+Version: 1.1.2
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,8 +39,8 @@
 python3 -m twine upload  dist/*                      # prod
 
 
 # Install
 Installing module
 	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux    # test
   
-  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.0.0 # prod
+  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.1.1 # prod
```

### Comparing `smallneuron-1.1.1/src/smallneuron.egg-info/SOURCES.txt` & `smallneuron-1.1.2/src/smallneuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smallneuron-1.1.1/src/smallneuron_pelainux.egg-info/PKG-INFO` & `smallneuron-1.1.2/src/smallneuron.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: smallneuron_pelainux
-Version: 0.1.4
+Name: smallneuron
+Version: 1.1.2
 Summary: Small Neuron Workflow
 Author-email: Andres Artigas <andres@artigas.cl>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,12 +31,16 @@
 # Install tools
 sudo apt install python3-pip python3-venv
 python3 -m pip install build # pip3 install build
 
 
 # Build
 python3 -m build
-python3 -m twine upload --repository testpypi dist/*
+python3 -m twine upload --repository testpypi dist/* # test
+python3 -m twine upload  dist/*                      # prod
+
 
 # Install
 Installing module
-	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux
+	sudo python3 -m pip install --upgrade --index-url https://test.pypi.org/simple/ --no-deps smallneuron-pelainux    # test
+  
+  sudo python3 -m pip install --upgrade --index-url https://pypi.org/simple/ --no-deps smallneuron==1.1.1 # prod
```

