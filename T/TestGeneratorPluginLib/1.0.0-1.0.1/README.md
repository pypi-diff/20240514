# Comparing `tmp/TestGeneratorPluginLib-1.0.0.tar.gz` & `tmp/TestGeneratorPluginLib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.0.0.tar", last modified: Tue May 14 16:00:37 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.0.1.tar", last modified: Tue May 14 16:12:12 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.0.0.tar` & `TestGeneratorPluginLib-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 16:00:37.989641 TestGeneratorPluginLib-1.0.0/
--rw-rw-rw-   0        0        0     1090 2024-03-07 10:01:21.000000 TestGeneratorPluginLib-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1697 2024-05-14 16:00:37.989641 TestGeneratorPluginLib-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-14 16:00:37.979642 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      191 2024-05-14 15:38:16.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0      830 2024-05-14 13:55:45.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-14 15:58:58.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0      965 2024-05-14 13:49:41.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0     2728 2024-05-14 15:39:52.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     3248 2024-05-14 13:55:45.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-14 16:00:37.989641 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1697 2024-05-14 16:00:37.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2024-05-14 16:00:37.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 16:00:37.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-14 16:00:37.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-14 16:00:37.000000 TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 16:00:37.989641 TestGeneratorPluginLib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-14 15:58:58.000000 TestGeneratorPluginLib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-14 16:12:12.648520 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      191 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0      830 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0      965 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0     2728 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     3248 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-14 16:12:12.000000 TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 16:12:12.664090 TestGeneratorPluginLib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-14 16:11:30.000000 TestGeneratorPluginLib-1.0.1/setup.py
```

### Comparing `TestGeneratorPluginLib-1.0.0/LICENSE` & `TestGeneratorPluginLib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.0/PKG-INFO` & `TestGeneratorPluginLib-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
@@ -25,13 +25,9 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyQt6~=6.6.1
-Requires-Dist: qasync~=0.27.1
-Requires-Dist: PyQtUIkit~=2.8.5
-Requires-Dist: setuptools~=68.2.0
 
 TestGenerator Plugin Library
```

### Comparing `TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.0.0/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.0.1/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
@@ -25,13 +25,9 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PyQt6~=6.6.1
-Requires-Dist: qasync~=0.27.1
-Requires-Dist: PyQtUIkit~=2.8.5
-Requires-Dist: setuptools~=68.2.0
 
 TestGenerator Plugin Library
```

### Comparing `TestGeneratorPluginLib-1.0.0/setup.py` & `TestGeneratorPluginLib-1.0.1/setup.py`

 * *Files identical despite different names*

