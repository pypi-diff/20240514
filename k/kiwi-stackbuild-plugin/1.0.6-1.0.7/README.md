# Comparing `tmp/kiwi_stackbuild_plugin-1.0.6.tar.gz` & `tmp/kiwi_stackbuild_plugin-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kiwi_stackbuild_plugin-1.0.6.tar", last modified: Thu Mar 17 09:49:06 2022, max compression
+gzip compressed data, was "dist/kiwi_stackbuild_plugin-1.0.7.tar", last modified: Thu Mar 17 09:48:56 2022, max compression
```

## Comparing `kiwi_stackbuild_plugin-1.0.6.tar` & `kiwi_stackbuild_plugin-1.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/MANIFEST.in
--rwxr-xr-x   0 runner    (1001) docker     (121)     1729 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/.virtualenv.requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     9840 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/tasks/system_stackbuild.py
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/tasks/system_stash.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/package/
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/package/python-kiwi_stackbuild_plugin.changes
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/package/python-kiwi_stackbuild_plugin-spec-template
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/package/python-kiwi_stackbuild_plugin-rpmlintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/tox.ini
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 09:49:06.000000 kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-03-17 09:48:27.000000 kiwi_stackbuild_plugin-1.0.6/.virtualenv.dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/MANIFEST.in
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1729 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/.virtualenv.requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)     9840 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/tasks/system_stackbuild.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5706 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/tasks/system_stash.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/package/
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/package/python-kiwi_stackbuild_plugin.changes
+-rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/package/python-kiwi_stackbuild_plugin-spec-template
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/package/python-kiwi_stackbuild_plugin-rpmlintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-17 09:48:56.000000 kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      598 2022-03-17 09:48:24.000000 kiwi_stackbuild_plugin-1.0.7/.virtualenv.dev-requirements.txt
```

### Comparing `kiwi_stackbuild_plugin-1.0.6/LICENSE` & `kiwi_stackbuild_plugin-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/setup.py` & `kiwi_stackbuild_plugin-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/defaults.py` & `kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/defaults.py`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/exceptions.py` & `kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/tasks/system_stackbuild.py` & `kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/tasks/system_stackbuild.py`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/tasks/system_stash.py` & `kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/tasks/system_stash.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         )
         stash_container_tag = self.command_args['--tag'] or 'latest'
         container_config = StackBuildDefaults.get_container_config(
             image_name, stash_container_tag, contact_info.author
         )
         log.info('Initializing stash container')
         oci = OCI.new()
-        if os.path.exists(stash_container_file_name):
+        if os.path.isfile(stash_container_file_name):
             log.info('--> Adding new layer on existing stash')
             oci.import_container_image(
                 f'oci-archive:{stash_container_file_name}:'
                 f'{image_name}:{stash_container_tag}'
             )
         else:
             log.info('--> Creating initial layer')
```

### Comparing `kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin/version.py` & `kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with kiwi-stackbuild.  If not, see <http://www.gnu.org/licenses/>
 #
 """
 Global version information used in kiwi-rebuild-plugin and the package
 """
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 __githash__ = '$Format:%H$'
```

### Comparing `kiwi_stackbuild_plugin-1.0.6/package/python-kiwi_stackbuild_plugin-spec-template` & `kiwi_stackbuild_plugin-1.0.7/package/python-kiwi_stackbuild_plugin-spec-template`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/PKG-INFO` & `kiwi_stackbuild_plugin-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwi_stackbuild_plugin
-Version: 1.0.6
+Version: 1.0.7
 Summary: KIWI - Stack Build Plugin
 Home-page: https://github.com/OSInside/kiwi-stackbuild-plugin
 Author: Marcus Schaefer
 Author-email: ms@suse.com
 License: GPLv3+
 Download-URL: https://download.opensuse.org/repositories/Virtualization:/Appliances:/Builder
 Platform: UNKNOWN
```

### Comparing `kiwi_stackbuild_plugin-1.0.6/Makefile` & `kiwi_stackbuild_plugin-1.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/tox.ini` & `kiwi_stackbuild_plugin-1.0.7/tox.ini`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/README.rst` & `kiwi_stackbuild_plugin-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/PKG-INFO` & `kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwi-stackbuild-plugin
-Version: 1.0.6
+Version: 1.0.7
 Summary: KIWI - Stack Build Plugin
 Home-page: https://github.com/OSInside/kiwi-stackbuild-plugin
 Author: Marcus Schaefer
 Author-email: ms@suse.com
 License: GPLv3+
 Download-URL: https://download.opensuse.org/repositories/Virtualization:/Appliances:/Builder
 Platform: UNKNOWN
```

### Comparing `kiwi_stackbuild_plugin-1.0.6/kiwi_stackbuild_plugin.egg-info/SOURCES.txt` & `kiwi_stackbuild_plugin-1.0.7/kiwi_stackbuild_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwi_stackbuild_plugin-1.0.6/.virtualenv.dev-requirements.txt` & `kiwi_stackbuild_plugin-1.0.7/.virtualenv.dev-requirements.txt`

 * *Files identical despite different names*

