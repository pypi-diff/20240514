# Comparing `tmp/ansar_create-0.1.84.tar.gz` & `tmp/ansar_create-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_create-0.1.84.tar", last modified: Tue May 14 09:45:21 2024, max compression
+gzip compressed data, was "ansar_create-0.1.85.tar", last modified: Tue May 14 16:39:58 2024, max compression
```

## Comparing `ansar_create-0.1.84.tar` & `ansar_create-0.1.85.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:45:21.873580 ansar_create-0.1.84/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.84/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-14 09:45:21.873580 ansar_create-0.1.84/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.84/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-05-09 12:38:05.000000 ansar_create-0.1.84/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-14 09:45:21.873580 ansar_create-0.1.84/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-05-09 12:37:55.000000 ansar_create-0.1.84/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:45:21.873580 ansar_create-0.1.84/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:45:21.873580 ansar_create-0.1.84/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:45:21.873580 ansar_create-0.1.84/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.84/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.84/src/ansar/command/ansar_group.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:45:21.873580 ansar_create-0.1.84/src/ansar/create/
--rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-14 09:45:18.000000 ansar_create-0.1.84/src/ansar/create/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.84/src/ansar/create/binding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.84/src/ansar/create/coding.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.84/src/ansar/create/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.84/src/ansar/create/home.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3607 2024-02-14 21:31:28.000000 ansar_create-0.1.84/src/ansar/create/latching.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.84/src/ansar/create/lifecycle.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.84/src/ansar/create/locking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.84/src/ansar/create/log.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.84/src/ansar/create/machine.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29779 2024-05-08 19:37:29.000000 ansar_create-0.1.84/src/ansar/create/object.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.84/src/ansar/create/pending.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    29471 2024-05-14 09:44:20.000000 ansar_create-0.1.84/src/ansar/create/point.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    79049 2024-04-14 03:56:16.000000 ansar_create-0.1.84/src/ansar/create/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.84/src/ansar/create/processing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.84/src/ansar/create/properties.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.84/src/ansar/create/retry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.84/src/ansar/create/rolling.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.84/src/ansar/create/root.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14196 2024-03-22 18:43:05.000000 ansar_create-0.1.84/src/ansar/create/space.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19735 2024-03-22 18:43:09.000000 ansar_create-0.1.84/src/ansar/create/storage.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.84/src/ansar/create/test.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.84/src/ansar/create/timing.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 09:45:21.873580 ansar_create-0.1.84/src/ansar_create.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-14 09:45:21.000000 ansar_create-0.1.84/src/ansar_create.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-14 09:45:21.000000 ansar_create-0.1.84/src/ansar_create.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-14 09:45:21.000000 ansar_create-0.1.84/src/ansar_create.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-14 09:45:21.000000 ansar_create-0.1.84/src/ansar_create.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-14 09:45:21.000000 ansar_create-0.1.84/src/ansar_create.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-14 09:45:21.000000 ansar_create-0.1.84/src/ansar_create.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:39:58.447603 ansar_create-0.1.85/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:18.000000 ansar_create-0.1.85/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-14 16:39:58.447603 ansar_create-0.1.85/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      901 2023-06-17 21:18:11.000000 ansar_create-0.1.85/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      718 2024-05-09 12:38:05.000000 ansar_create-0.1.85/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-14 16:39:58.447603 ansar_create-0.1.85/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2139 2024-05-09 12:37:55.000000 ansar_create-0.1.85/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:39:58.443603 ansar_create-0.1.85/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:39:58.443603 ansar_create-0.1.85/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:39:58.447603 ansar_create-0.1.85/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13081 2024-01-02 02:57:04.000000 ansar_create-0.1.85/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8950 2024-02-25 02:39:34.000000 ansar_create-0.1.85/src/ansar/command/ansar_group.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:39:58.447603 ansar_create-0.1.85/src/ansar/create/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5706 2024-05-14 16:39:55.000000 ansar_create-0.1.85/src/ansar/create/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2654 2023-07-13 04:39:47.000000 ansar_create-0.1.85/src/ansar/create/binding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1989 2023-12-23 01:56:16.000000 ansar_create-0.1.85/src/ansar/create/coding.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1857 2024-01-19 15:16:48.000000 ansar_create-0.1.85/src/ansar/create/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    13837 2024-02-24 20:57:36.000000 ansar_create-0.1.85/src/ansar/create/home.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3607 2024-02-14 21:31:28.000000 ansar_create-0.1.85/src/ansar/create/latching.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7383 2024-03-24 15:57:41.000000 ansar_create-0.1.85/src/ansar/create/lifecycle.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4061 2024-01-25 13:13:42.000000 ansar_create-0.1.85/src/ansar/create/locking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6164 2023-07-13 04:40:10.000000 ansar_create-0.1.85/src/ansar/create/log.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8495 2023-07-13 04:40:11.000000 ansar_create-0.1.85/src/ansar/create/machine.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29779 2024-05-08 19:37:29.000000 ansar_create-0.1.85/src/ansar/create/object.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9071 2024-01-18 15:23:10.000000 ansar_create-0.1.85/src/ansar/create/pending.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    29471 2024-05-14 09:44:20.000000 ansar_create-0.1.85/src/ansar/create/point.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    80287 2024-05-14 16:39:09.000000 ansar_create-0.1.85/src/ansar/create/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    31841 2024-01-22 04:26:11.000000 ansar_create-0.1.85/src/ansar/create/processing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3099 2024-03-26 19:19:48.000000 ansar_create-0.1.85/src/ansar/create/properties.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3741 2024-03-07 07:59:16.000000 ansar_create-0.1.85/src/ansar/create/retry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5938 2024-02-27 14:04:16.000000 ansar_create-0.1.85/src/ansar/create/rolling.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7477 2023-12-23 15:53:02.000000 ansar_create-0.1.85/src/ansar/create/root.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14196 2024-03-22 18:43:05.000000 ansar_create-0.1.85/src/ansar/create/space.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    19735 2024-03-22 18:43:09.000000 ansar_create-0.1.85/src/ansar/create/storage.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3959 2024-01-15 15:55:19.000000 ansar_create-0.1.85/src/ansar/create/test.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     5100 2024-01-26 08:38:29.000000 ansar_create-0.1.85/src/ansar/create/timing.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-14 16:39:58.447603 ansar_create-0.1.85/src/ansar_create.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1603 2024-05-14 16:39:58.000000 ansar_create-0.1.85/src/ansar_create.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      986 2024-05-14 16:39:58.000000 ansar_create-0.1.85/src/ansar_create.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-14 16:39:58.000000 ansar_create-0.1.85/src/ansar_create.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      104 2024-05-14 16:39:58.000000 ansar_create-0.1.85/src/ansar_create.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       22 2024-05-14 16:39:58.000000 ansar_create-0.1.85/src/ansar_create.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-14 16:39:58.000000 ansar_create-0.1.85/src/ansar_create.egg-info/top_level.txt
```

### Comparing `ansar_create-0.1.84/LICENSE` & `ansar_create-0.1.85/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/PKG-INFO` & `ansar_create-0.1.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.84
+Version: 0.1.85
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.84/README.md` & `ansar_create-0.1.85/README.md`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/pyproject.toml` & `ansar_create-0.1.85/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/setup.py` & `ansar_create-0.1.85/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/command/ansar_command.py` & `ansar_create-0.1.85/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/command/ansar_group.py` & `ansar_create-0.1.85/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/__init__.py` & `ansar_create-0.1.85/src/ansar/create/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-create.git
 Branch: main
-Commit: 37f396a1b75bb5b92de1b2b6e100dfd353b49e46
-Version: 0.1.83 (2024-05-14@21:45:18+NZST)
+Commit: fdb30048c2bf9501a663de355d9aa5ec61e74f47
+Version: 0.1.84 (2024-05-15@04:39:55+NZST)
 """
 
 from ansar.encode import *
 
 from .coding import cannot, lor
 from .space import NO_SUCH_ADDRESS
 from .space import create_an_object, find_object, destroy_an_object
```

### Comparing `ansar_create-0.1.84/src/ansar/create/binding.py` & `ansar_create-0.1.85/src/ansar/create/binding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/coding.py` & `ansar_create-0.1.85/src/ansar/create/coding.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/grouping.py` & `ansar_create-0.1.85/src/ansar/create/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/home.py` & `ansar_create-0.1.85/src/ansar/create/home.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/latching.py` & `ansar_create-0.1.85/src/ansar/create/latching.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/lifecycle.py` & `ansar_create-0.1.85/src/ansar/create/lifecycle.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/locking.py` & `ansar_create-0.1.85/src/ansar/create/locking.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/log.py` & `ansar_create-0.1.85/src/ansar/create/log.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/machine.py` & `ansar_create-0.1.85/src/ansar/create/machine.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/object.py` & `ansar_create-0.1.85/src/ansar/create/object.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/pending.py` & `ansar_create-0.1.85/src/ansar/create/pending.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/point.py` & `ansar_create-0.1.85/src/ansar/create/point.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/procedure.py` & `ansar_create-0.1.85/src/ansar/create/procedure.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,41 +371,46 @@
 # Extraction of logs for a role.
 #
 START_OF = ar.Enumeration(MONTH=0, WEEK=1, DAY=2, HOUR=3, MINUTE=4, HALF=5, QUARTER=6, TEN=7, FIVE=8)
 
 class LogSettings(object):
 	def __init__(self, role_name=None, home_path=None,
 			clock=False, from_=None, last=None, start=None, back=None,
-			to=None, span=None, count=None):
+			to=None, span=None, count=None,
+			sample=None):
 		# One of these for a <begin>
 		self.role_name = role_name
 		self.home_path = home_path
 		self.clock = clock
 		self.from_ = from_
 		self.last = last
 		self.start = start
 		self.back = back
 
 		# One of these (optional), for an <end>
 		self.to = to
 		self.span = span
 		self.count = count
 
+		self.sample = sample
+
 LOG_SETTINGS_SCHEMA = {
 	'role_name': ar.Unicode(),
 	'home_path': ar.Unicode(),
 	"clock": ar.Boolean,
 	"from_": ar.Unicode,
 	"last": START_OF,
 	"start": int,
 	"back": ar.TimeSpan,
 
 	"to": ar.Unicode,
 	"span": ar.TimeSpan,
 	"count": int,
+
+	"sample": ar.Unicode,
 }
 
 ar.bind(LogSettings, object_schema=LOG_SETTINGS_SCHEMA)
 
 #
 #
 class InputSettings(object):
@@ -1663,14 +1668,58 @@
 		return fault
 	return None
 
 bind_any(printer)
 
 #
 #
+def tabulate(header, kv):
+	t = []
+	for h in header:
+		v = kv.get(h, None)
+		if v is None:
+			return None
+		t.append(v)
+	t = '\t'.join(t)
+	return t
+
+def sampler(self, hr, begin, end, count, header):
+	try:
+		#t = '\t'.join(header)
+		#ar.output_line(t, newline=True)
+
+		for _, t in read_log(hr.role_logs, begin, end, count):
+			if self.halted:
+				return Aborted()
+			if t[24] != '&':
+				continue
+			dash = t.find(' - ', 36)
+			if dash == -1:
+				continue
+			text = t[dash + 3:-1]
+			colon = text.split(':')
+			equals = [c.split('=') for c in colon]
+			kv = {lr[0]: lr[1] for lr in equals}
+			kv['time'] = t[0:23]
+			t = tabulate(header, kv)
+			if t is None:
+				continue
+			ar.output_line(t, newline=True)
+	except (KeyboardInterrupt, SystemExit) as e:
+		raise e
+	except Exception as e:
+		condition = str(e)
+		fault = ar.Faulted(condition)
+		return fault
+	return None
+
+bind_any(printer)
+
+#
+#
 def world_or_clock(s, clock):
 	if clock:
 		t = ar.text_to_clock(s)
 		d = datetime.datetime.fromtimestamp(t, tz=ar.UTC)
 		return d
 	return ar.text_to_world(s)
 
@@ -1744,17 +1793,26 @@
 		e = ar.Failed(start_mark=(None, f'<begin> not defined and not inferred'))
 		raise ar.Incomplete(e)
 
 	if end is not None and end < begin:
 		e = ar.Failed(mark_order=(None, f'<end> comes before <begin>'))
 		raise ar.Incomplete(e)
 
+	header = None
+	if log.sample:
+		header = log.sample.split(',')
+		if len(header) < 1 or '' in header:
+			e = ar.Failed(sample_header=(None, f'<sample> empty or contains empty column'))
+			raise ar.Incomplete(e)
+
 	self.console(f'Extracting logs "{hr.role_name}" ({hr.home.home_path})')
 
-	if log.clock:
+	if header:
+		a = self.create(sampler, hr, begin, end, count, header)
+	elif log.clock:
 		a = self.create(clocker, hr, begin, end, count)
 	else:
 		a = self.create(printer, hr, begin, end, count)
 	m = self.select(Stop, Completed)
 	if isinstance(m, Stop):
 		halt(a)
 		m = self.select(Completed)
```

### Comparing `ansar_create-0.1.84/src/ansar/create/processing.py` & `ansar_create-0.1.85/src/ansar/create/processing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/properties.py` & `ansar_create-0.1.85/src/ansar/create/properties.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/retry.py` & `ansar_create-0.1.85/src/ansar/create/retry.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/rolling.py` & `ansar_create-0.1.85/src/ansar/create/rolling.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/root.py` & `ansar_create-0.1.85/src/ansar/create/root.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/space.py` & `ansar_create-0.1.85/src/ansar/create/space.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/storage.py` & `ansar_create-0.1.85/src/ansar/create/storage.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/test.py` & `ansar_create-0.1.85/src/ansar/create/test.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar/create/timing.py` & `ansar_create-0.1.85/src/ansar/create/timing.py`

 * *Files identical despite different names*

### Comparing `ansar_create-0.1.84/src/ansar_create.egg-info/PKG-INFO` & `ansar_create-0.1.85/src/ansar_create.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-create
-Version: 0.1.84
+Version: 0.1.85
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com>
 Project-URL: Documentation, https://ansar-create-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_create-0.1.84/src/ansar_create.egg-info/SOURCES.txt` & `ansar_create-0.1.85/src/ansar_create.egg-info/SOURCES.txt`

 * *Files identical despite different names*

