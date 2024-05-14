# Comparing `tmp/pdrive-0.7.0.tar.gz` & `tmp/pdrive-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdrive-0.7.0.tar", last modified: Tue May 14 14:07:40 2024, max compression
+gzip compressed data, was "pdrive-0.7.1.tar", last modified: Tue May 14 14:26:27 2024, max compression
```

## Comparing `pdrive-0.7.0.tar` & `pdrive-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.973730 pdrive-0.7.0/
--rw-r--r--   0 huy        (501) staff       (20)    35147 2020-07-09 21:03:22.000000 pdrive-0.7.0/LICENSE
--rw-r--r--   0 huy        (501) staff       (20)      242 2024-05-14 14:07:40.972809 pdrive-0.7.0/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)     1274 2020-07-20 21:16:34.000000 pdrive-0.7.0/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.890133 pdrive-0.7.0/pdrive/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.901505 pdrive-0.7.0/pdrive/backend/
--rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.7.0/pdrive/backend/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)     5792 2024-05-14 14:01:30.000000 pdrive-0.7.0/pdrive/backend/web.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.902989 pdrive-0.7.0/pdrive/frontend/
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.906736 pdrive-0.7.0/pdrive/frontend/dist/
--rw-r--r--   0 huy        (501) staff       (20)    28200 2020-07-18 04:41:27.000000 pdrive-0.7.0/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff
--rw-r--r--   0 huy        (501) staff       (20)    55956 2020-07-18 04:41:27.000000 pdrive-0.7.0/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf
--rw-r--r--   0 huy        (501) staff       (20)  6999766 2020-07-18 04:41:27.000000 pdrive-0.7.0/pdrive/frontend/dist/build.js
--rw-r--r--   0 huy        (501) staff       (20)     1145 2020-07-09 21:03:22.000000 pdrive-0.7.0/pdrive/frontend/index.html
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:07:40.897797 pdrive-0.7.0/pdrive.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)      242 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      460 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)       52 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/entry_points.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 01:29:51.000000 pdrive-0.7.0/pdrive.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        7 2024-05-14 14:07:40.000000 pdrive-0.7.0/pdrive.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-14 14:07:40.973899 pdrive-0.7.0/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)     1390 2024-05-14 14:06:52.000000 pdrive-0.7.0/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.138133 pdrive-0.7.1/
+-rw-r--r--   0 huy        (501) staff       (20)    35147 2020-07-09 21:03:22.000000 pdrive-0.7.1/LICENSE
+-rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 14:26:27.137688 pdrive-0.7.1/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)     1274 2020-07-20 21:16:34.000000 pdrive-0.7.1/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.109977 pdrive-0.7.1/pdrive/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.115310 pdrive-0.7.1/pdrive/backend/
+-rw-r--r--   0 huy        (501) staff       (20)      730 2020-07-09 21:03:22.000000 pdrive-0.7.1/pdrive/backend/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     5792 2024-05-14 14:01:30.000000 pdrive-0.7.1/pdrive/backend/web.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.116295 pdrive-0.7.1/pdrive/frontend/
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.119381 pdrive-0.7.1/pdrive/frontend/dist/
+-rw-r--r--   0 huy        (501) staff       (20)    28200 2020-07-18 04:41:27.000000 pdrive-0.7.1/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff
+-rw-r--r--   0 huy        (501) staff       (20)    55956 2020-07-18 04:41:27.000000 pdrive-0.7.1/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf
+-rw-r--r--   0 huy        (501) staff       (20)  6999766 2020-07-18 04:41:27.000000 pdrive-0.7.1/pdrive/frontend/dist/build.js
+-rw-r--r--   0 huy        (501) staff       (20)     1145 2020-07-09 21:03:22.000000 pdrive-0.7.1/pdrive/frontend/index.html
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-14 14:26:27.114266 pdrive-0.7.1/pdrive.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)     1870 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      460 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       52 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2020-07-18 01:29:51.000000 pdrive-0.7.1/pdrive.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)        6 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        7 2024-05-14 14:26:27.000000 pdrive-0.7.1/pdrive.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-14 14:26:27.138328 pdrive-0.7.1/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)     1621 2024-05-14 14:25:49.000000 pdrive-0.7.1/setup.py
```

### Comparing `pdrive-0.7.0/LICENSE` & `pdrive-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/README.md` & `pdrive-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/pdrive/backend/__init__.py` & `pdrive-0.7.1/pdrive/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/pdrive/backend/web.py` & `pdrive-0.7.1/pdrive/backend/web.py`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff` & `pdrive-0.7.1/pdrive/frontend/dist/313f7dacf2076822059d2dca26dedfc6.woff`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf` & `pdrive-0.7.1/pdrive/frontend/dist/4520188144a17fb24a6af28a70dae0ce.ttf`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/pdrive/frontend/dist/build.js` & `pdrive-0.7.1/pdrive/frontend/dist/build.js`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/pdrive/frontend/index.html` & `pdrive-0.7.1/pdrive/frontend/index.html`

 * *Files identical despite different names*

### Comparing `pdrive-0.7.0/setup.py` & `pdrive-0.7.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,24 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup
 
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+
 setup(name='pdrive',
-      version='0.7.0',
-      description='File manager',
+      version='0.7.1',
+      description='A simple file manager',
+      long_description=long_description,
+      long_description_content_type='text/markdown',
       author='Huy Nguyen',
       author_email='121183+huyng@users.noreply.github.com',
       packages=['pdrive', "pdrive.frontend", "pdrive.backend"],
       package_data={
           'pdrive.frontend': ['index.html', 'dist/*']
       },
       entry_points={
```

