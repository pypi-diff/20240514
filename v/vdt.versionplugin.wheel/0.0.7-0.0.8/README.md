# Comparing `tmp/vdt.versionplugin.wheel-0.0.7.tar.gz` & `tmp/vdt_versionplugin_wheel-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdt.versionplugin.wheel-0.0.7.tar", last modified: Wed Dec 30 10:26:27 2020, max compression
+gzip compressed data, was "vdt_versionplugin_wheel-0.0.8.tar", last modified: Tue May 14 07:41:23 2024, max compression
```

## Comparing `vdt.versionplugin.wheel-0.0.7.tar` & `vdt_versionplugin_wheel-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/
--rw-r--r--   0 ebone      (502) staff       (20)      340 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/PKG-INFO
--rw-r--r--   0 ebone      (502) staff       (20)     1925 2020-12-30 10:25:23.000000 vdt.versionplugin.wheel-0.0.7/README.md
--rw-r--r--   0 ebone      (502) staff       (20)       38 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/setup.cfg
--rw-r--r--   0 ebone      (502) staff       (20)      691 2020-12-30 10:25:23.000000 vdt.versionplugin.wheel-0.0.7/setup.py
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt/
--rw-r--r--   0 ebone      (502) staff       (20)       56 2015-06-15 11:51:14.000000 vdt.versionplugin.wheel-0.0.7/vdt/__init__.py
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/
--rw-r--r--   0 ebone      (502) staff       (20)       56 2015-06-15 11:51:14.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/__init__.py
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/
--rw-r--r--   0 ebone      (502) staff       (20)      114 2020-12-30 10:25:23.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/__init__.py
--rw-r--r--   0 ebone      (502) staff       (20)     1689 2020-12-30 10:25:23.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/package.py
--rw-r--r--   0 ebone      (502) staff       (20)      435 2016-04-20 07:36:14.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/shared.py
--rw-r--r--   0 ebone      (502) staff       (20)      180 2015-06-16 14:33:33.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/utils.py
--rw-r--r--   0 ebone      (502) staff       (20)      948 2020-12-30 10:25:23.000000 vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/version.py
-drwxr-xr-x   0 ebone      (502) staff       (20)        0 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/
--rw-r--r--   0 ebone      (502) staff       (20)        1 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/dependency_links.txt
--rw-r--r--   0 ebone      (502) staff       (20)       22 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/namespace_packages.txt
--rw-r--r--   0 ebone      (502) staff       (20)      340 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/PKG-INFO
--rw-r--r--   0 ebone      (502) staff       (20)       64 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/requires.txt
--rw-r--r--   0 ebone      (502) staff       (20)      569 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/SOURCES.txt
--rw-r--r--   0 ebone      (502) staff       (20)        4 2020-12-30 10:26:27.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/top_level.txt
--rw-r--r--   0 ebone      (502) staff       (20)        1 2015-06-15 13:24:04.000000 vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/zip-safe
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:41:23.592887 vdt_versionplugin_wheel-0.0.8/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     1491 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/LICENSE
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      441 2024-05-14 07:41:23.592684 vdt_versionplugin_wheel-0.0.8/PKG-INFO
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     1925 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/README.md
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       38 2024-05-14 07:41:23.592930 vdt_versionplugin_wheel-0.0.8/setup.cfg
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      691 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/setup.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:41:23.590575 vdt_versionplugin_wheel-0.0.8/vdt/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       56 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/vdt/__init__.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:41:23.591459 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       56 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/__init__.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:41:23.592227 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      114 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/__init__.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     1689 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/package.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      435 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/shared.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      180 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/utils.py
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)     1148 2024-05-14 07:17:52.000000 vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/version.py
+drwxr-xr-x   0 larsvandekerkhof   (501) staff       (20)        0 2024-05-14 07:41:23.592466 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      441 2024-05-14 07:41:23.000000 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/PKG-INFO
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)      577 2024-05-14 07:41:23.000000 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/SOURCES.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:41:23.000000 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/dependency_links.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       22 2024-05-14 07:41:23.000000 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/namespace_packages.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)       64 2024-05-14 07:41:23.000000 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/requires.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        4 2024-05-14 07:41:23.000000 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/top_level.txt
+-rw-r--r--   0 larsvandekerkhof   (501) staff       (20)        1 2024-05-14 07:41:23.000000 vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vdt.versionplugin.wheel-0.0.7/README.md` & `vdt_versionplugin_wheel-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vdt.versionplugin.wheel-0.0.7/setup.py` & `vdt_versionplugin_wheel-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 from setuptools import find_packages, setup
 
 pkgname = "vdt.versionplugin.wheel"
 
 setup(
     name=pkgname,
-    version="0.0.7",
+    version="0.0.8",
     description="vdt.version plugin for building python wheels.",
     author="Lars van de Kerkhof",
     author_email="lars@devopsconsulting.nl",
     maintainer="Lars van de Kerkhof",
     maintainer_email="lars@devopsconsulting.nl",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/package.py` & `vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/package.py`

 * *Files identical despite different names*

### Comparing `vdt.versionplugin.wheel-0.0.7/vdt/versionplugin/wheel/version.py` & `vdt_versionplugin_wheel-0.0.8/vdt/versionplugin/wheel/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,21 +11,27 @@
 
 log = logging.getLogger('vdt.versionplugin.wheel.version')
 
 
 __all__ = ('get_version')
 
 
+def get_python_version(version_args):
+    result = subprocess.check_output(['python', 'setup.py', '--version'])
+    return Version(result.decode("utf-8"), extra_args=version_args)
+
+
 def get_version(version_args):
     """
     Retrieve the version from the repo, if no version tag
     can be found, read it from the setup script
 
     It can be assumed that this script will be ran in the
     root of the repository.
     """
+    python_version = get_python_version(version_args)
     try:
-        return get_git_version(version_args)
+        gitversion = get_git_version(version_args)
+        return gitversion if gitversion >= python_version else python_version
     except VersionNotFound:
         log.debug('no version tag found, taking version from setup.py')
-        result = subprocess.check_output(['python', 'setup.py', '--version'])
-        return Version(result.decode("utf-8"), extra_args=version_args)
+        return python_version
```

### Comparing `vdt.versionplugin.wheel-0.0.7/vdt.versionplugin.wheel.egg-info/SOURCES.txt` & `vdt_versionplugin_wheel-0.0.8/vdt.versionplugin.wheel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 vdt/__init__.py
 vdt.versionplugin.wheel.egg-info/PKG-INFO
 vdt.versionplugin.wheel.egg-info/SOURCES.txt
 vdt.versionplugin.wheel.egg-info/dependency_links.txt
 vdt.versionplugin.wheel.egg-info/namespace_packages.txt
```

