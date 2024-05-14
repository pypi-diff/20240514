# Comparing `tmp/neon-iris-0.1.1a5.tar.gz` & `tmp/neon-iris-0.1.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-iris-0.1.1a5.tar", last modified: Wed Apr 10 22:23:25 2024, max compression
+gzip compressed data, was "neon-iris-0.1.1a6.tar", last modified: Tue May 14 16:12:37 2024, max compression
```

## Comparing `neon-iris-0.1.1a5.tar` & `neon-iris-0.1.1a6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/models/web_sat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/res/
--rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/res/start_listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/static/sprite.css
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/static/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/voice_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/web_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/neon_iris/web_sat_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/neon_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 22:23:25.000000 neon-iris-0.1.1a5/neon_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:23:25.041458 neon-iris-0.1.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-10 22:23:21.000000 neon-iris-0.1.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:12:37.381595 neon-iris-0.1.1a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-14 16:12:37.381595 neon-iris-0.1.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:12:37.377595 neon-iris-0.1.1a6/neon_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:12:37.381595 neon-iris-0.1.1a6/neon_iris/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/models/web_sat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:12:37.381595 neon-iris-0.1.1a6/neon_iris/res/
+-rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/res/start_listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:12:37.381595 neon-iris-0.1.1a6/neon_iris/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/static/sprite.css
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/static/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:12:37.381595 neon-iris-0.1.1a6/neon_iris/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/voice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18144 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/web_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/neon_iris/web_sat_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:12:37.377595 neon-iris-0.1.1a6/neon_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-14 16:12:37.000000 neon-iris-0.1.1a6/neon_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-14 16:12:37.000000 neon-iris-0.1.1a6/neon_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:12:37.000000 neon-iris-0.1.1a6/neon_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 16:12:37.000000 neon-iris-0.1.1a6/neon_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 16:12:37.000000 neon-iris-0.1.1a6/neon_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 16:12:37.000000 neon-iris-0.1.1a6/neon_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:12:37.381595 neon-iris-0.1.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-14 16:12:33.000000 neon-iris-0.1.1a6/setup.py
```

### Comparing `neon-iris-0.1.1a5/LICENSE.md` & `neon-iris-0.1.1a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/PKG-INFO` & `neon-iris-0.1.1a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-iris
-Version: 0.1.1a5
+Version: 0.1.1a6
 Summary: Interactive Relay for Intelligence Systems
 Home-page: https://github.com/neongeckocom/neon-iris
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-iris-0.1.1a5/README.md` & `neon-iris-0.1.1a6/README.md`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/__init__.py` & `neon-iris-0.1.1a6/neon_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/cli.py` & `neon-iris-0.1.1a6/neon_iris/cli.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/client.py` & `neon-iris-0.1.1a6/neon_iris/client.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/llm.py` & `neon-iris-0.1.1a6/neon_iris/llm.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/models/__init__.py` & `neon-iris-0.1.1a6/neon_iris/models/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/models/web_sat.py` & `neon-iris-0.1.1a6/neon_iris/models/web_sat.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/res/start_listening.wav` & `neon-iris-0.1.1a6/neon_iris/res/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/static/sprite.css` & `neon-iris-0.1.1a6/neon_iris/static/sprite.css`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/static/styles.css` & `neon-iris-0.1.1a6/neon_iris/static/styles.css`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/templates/index.html` & `neon-iris-0.1.1a6/neon_iris/templates/index.html`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/util.py` & `neon-iris-0.1.1a6/neon_iris/util.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/version.py` & `neon-iris-0.1.1a6/neon_iris/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a5"
+__version__ = "0.1.1a6"
```

### Comparing `neon-iris-0.1.1a5/neon_iris/voice_client.py` & `neon-iris-0.1.1a6/neon_iris/voice_client.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/web_client.py` & `neon-iris-0.1.1a6/neon_iris/web_client.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris/web_sat_client.py` & `neon-iris-0.1.1a6/neon_iris/web_sat_client.py`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/neon_iris.egg-info/PKG-INFO` & `neon-iris-0.1.1a6/neon_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-iris
-Version: 0.1.1a5
+Version: 0.1.1a6
 Summary: Interactive Relay for Intelligence Systems
 Home-page: https://github.com/neongeckocom/neon-iris
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-iris-0.1.1a5/neon_iris.egg-info/SOURCES.txt` & `neon-iris-0.1.1a6/neon_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-iris-0.1.1a5/setup.py` & `neon-iris-0.1.1a6/setup.py`

 * *Files identical despite different names*

