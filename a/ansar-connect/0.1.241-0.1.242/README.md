# Comparing `tmp/ansar_connect-0.1.241.tar.gz` & `tmp/ansar_connect-0.1.242.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.241.tar", last modified: Fri May 10 15:15:42 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.242.tar", last modified: Tue May 14 09:46:59 2024, max compression
```

## Comparing `ansar_connect-0.1.241.tar` & `ansar_connect-0.1.242.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.241/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.241/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 12:39:56.000000 ansar_connect-0.1.241/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 12:39:45.000000 ansar_connect-0.1.241/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.241/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.241/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.241/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.241/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-10 15:15:38.000000 ansar_connect-0.1.241/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.241/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.241/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.241/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.241/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.241/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.241/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.241/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.241/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.241/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.241/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.241/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33939 2024-05-10 00:17:44.000000 ansar_connect-0.1.241/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.241/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.241/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.241/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.241/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.241/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.241/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-10 15:15:42.048604 ansar_connect-0.1.241/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-10 15:15:42.000000 ansar_connect-0.1.241/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-10 15:15:42.000000 ansar_connect-0.1.241/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-10 15:15:42.000000 ansar_connect-0.1.241/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-10 15:15:42.000000 ansar_connect-0.1.241/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-10 15:15:42.000000 ansar_connect-0.1.241/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-10 15:15:42.000000 ansar_connect-0.1.241/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:46:59.772635 ansar_connect-0.1.242/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.242/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-14 09:46:59.772635 ansar_connect-0.1.242/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.242/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-14 09:46:50.000000 ansar_connect-0.1.242/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-14 09:46:59.772635 ansar_connect-0.1.242/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-14 09:46:43.000000 ansar_connect-0.1.242/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:46:59.768635 ansar_connect-0.1.242/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:46:59.768635 ansar_connect-0.1.242/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:46:59.768635 ansar_connect-0.1.242/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.242/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.242/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.242/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.242/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:46:59.768635 ansar_connect-0.1.242/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-14 09:46:56.000000 ansar_connect-0.1.242/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.242/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.242/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.242/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10461 2024-05-10 15:14:29.000000 ansar_connect-0.1.242/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.242/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14241 2024-05-09 13:41:02.000000 ansar_connect-0.1.242/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.242/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.242/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.242/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.242/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.242/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33894 2024-05-13 17:10:04.000000 ansar_connect-0.1.242/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.242/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.242/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.242/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.242/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.242/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.242/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:46:59.772635 ansar_connect-0.1.242/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-14 09:46:59.000000 ansar_connect-0.1.242/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-14 09:46:59.000000 ansar_connect-0.1.242/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-14 09:46:59.000000 ansar_connect-0.1.242/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-14 09:46:59.000000 ansar_connect-0.1.242/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-14 09:46:59.000000 ansar_connect-0.1.242/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-14 09:46:59.000000 ansar_connect-0.1.242/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.241/LICENSE` & `ansar_connect-0.1.242/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/PKG-INFO` & `ansar_connect-0.1.242/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.241
+Version: 0.1.242
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.83
+Requires-Dist: ansar-create>=0.1.84
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.241/README.md` & `ansar_connect-0.1.242/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/pyproject.toml` & `ansar_connect-0.1.242/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries"
 ]
 dynamic = ["description", "version", "scripts"]
 dependencies = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.83"
+    "ansar-create>=0.1.84"
 ]
 
 [project.urls]
 Documentation = "https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html"
```

### Comparing `ansar_connect-0.1.241/setup.py` & `ansar_connect-0.1.242/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.83",
+    "ansar-create>=0.1.84",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
     author_email="scott.18.ansar@gmail.com.com",
```

### Comparing `ansar_connect-0.1.241/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.242/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.242/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.242/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.242/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/__init__.py` & `ansar_connect-0.1.242/src/ansar/connect/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 1e31c7f836460e7835addd3f00b2eb537f9f3ff8
-Version: 0.1.240 (2024-05-11@03:15:38+NZST)
+Commit: 12d113b4216c3f3a08ce0be636283ab288b26e6a
+Version: 0.1.241 (2024-05-14@21:46:56+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.241/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.242/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/directory.py` & `ansar_connect-0.1.242/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.242/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.242/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/group_if.py` & `ansar_connect-0.1.242/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/grouping.py` & `ansar_connect-0.1.242/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/moving.py` & `ansar_connect-0.1.242/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/networking.py` & `ansar_connect-0.1.242/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.242/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/node.py` & `ansar_connect-0.1.242/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.242/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/procedure.py` & `ansar_connect-0.1.242/src/ansar/connect/procedure.py`

 * *Files 1% similar despite different names*

```diff
@@ -502,15 +502,15 @@
 # Standardize checking and diagnostics for all the
 # cloud interactions.
 def crud_address_and_token(crud, ipp, token):
 	if crud > 1:
 		f = ar.Faulted('multiple operations specified', 'not supported')
 		return f
 	if not ipp:
-		f = ar.Faulted('no address defined for the ansar cloud', 'use --cloud-ip=<address> --store-settings')
+		f = ar.Faulted('no address defined for the ansar cloud')
 		return f
 	if not token:
 		f = ar.Faulted('not logged in', 'need to signup or login')
 		return f
 	return None
 
 # Create a new account.
```

### Comparing `ansar_connect-0.1.241/src/ansar/connect/product.py` & `ansar_connect-0.1.242/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/socketry.py` & `ansar_connect-0.1.242/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/standard.py` & `ansar_connect-0.1.242/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/transporting.py` & `ansar_connect-0.1.242/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.242/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar/connect/wan.py` & `ansar_connect-0.1.242/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.241/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.242/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.241
+Version: 0.1.242
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.83
+Requires-Dist: ansar-create>=0.1.84
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.241/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.242/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

