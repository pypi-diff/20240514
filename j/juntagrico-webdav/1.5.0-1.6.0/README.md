# Comparing `tmp/juntagrico-webdav-1.5.0.tar.gz` & `tmp/juntagrico_webdav-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\juntagrico-webdav-1.5.0.tar", last modified: Tue Feb  8 09:34:19 2022, max compression
+gzip compressed data, was "juntagrico_webdav-1.6.0.tar", last modified: Mon May 13 21:59:48 2024, max compression
```

## Comparing `juntagrico-webdav-1.5.0.tar` & `juntagrico_webdav-1.6.0.tar`

### file list

```diff
@@ -1,45 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.966400 juntagrico-webdav-1.5.0/
--rw-rw-rw-   0        0        0     7816 2019-01-28 20:05:30.000000 juntagrico-webdav-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      261 2021-05-02 19:18:49.000000 juntagrico-webdav-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3034 2022-02-08 09:34:19.967400 juntagrico-webdav-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1969 2021-05-02 19:18:49.000000 juntagrico-webdav-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.767405 juntagrico-webdav-1.5.0/juntagrico_webdav/
--rw-rw-rw-   0        0        0       47 2022-02-08 09:33:38.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/__init__.py
--rw-rw-rw-   0        0        0      328 2019-02-03 12:24:39.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/admin.py
--rw-rw-rw-   0        0        0      159 2021-05-02 19:32:07.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/apps.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.824403 juntagrico-webdav-1.5.0/juntagrico_webdav/dao/
--rw-rw-rw-   0        0        0        0 2019-01-28 20:05:30.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/dao/__init__.py
--rw-rw-rw-   0        0        0      324 2019-01-28 21:28:40.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/dao/webdavserverdao.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.839403 juntagrico-webdav-1.5.0/juntagrico_webdav/entity/
--rw-rw-rw-   0        0        0        0 2019-01-28 20:05:30.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/entity/__init__.py
--rw-rw-rw-   0        0        0     1115 2021-03-23 07:52:52.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/entity/servers.py
--rw-rw-rw-   0        0        0      249 2021-05-02 19:18:49.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/juntagricoapp.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.887399 juntagrico-webdav-1.5.0/juntagrico_webdav/migrations/
--rw-rw-rw-   0        0        0     1260 2019-01-28 22:00:43.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1020 2019-12-24 13:05:59.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/migrations/0002_auto_20191111_1501.py
--rw-rw-rw-   0        0        0        0 2019-01-28 20:05:30.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/migrations/__init__.py
--rw-rw-rw-   0        0        0        0 2021-03-23 07:51:30.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/models.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.650413 juntagrico-webdav-1.5.0/juntagrico_webdav/static/
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.906436 juntagrico-webdav-1.5.0/juntagrico_webdav/static/js/
--rw-rw-rw-   0        0        0     1830 2019-01-31 20:06:25.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/static/js/initWDList.js
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.652399 juntagrico-webdav-1.5.0/juntagrico_webdav/templates/
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.946411 juntagrico-webdav-1.5.0/juntagrico_webdav/templates/wd/
--rw-rw-rw-   0        0        0      521 2019-10-19 18:27:07.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/templates/wd/admin_menu.html
--rw-rw-rw-   0        0        0      954 2021-05-02 19:18:49.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/templates/wd/list.html
--rw-rw-rw-   0        0        0      293 2019-01-30 21:01:38.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/templates/wd/menu.html
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.958399 juntagrico-webdav-1.5.0/juntagrico_webdav/templatetags/
--rw-rw-rw-   0        0        0        0 2019-01-28 21:36:12.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/templatetags/__init__.py
--rw-rw-rw-   0        0        0      306 2021-03-23 07:53:11.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/templatetags/menus.py
--rw-rw-rw-   0        0        0      220 2021-05-02 19:18:49.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/urls.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.964442 juntagrico-webdav-1.5.0/juntagrico_webdav/util/
--rw-rw-rw-   0        0        0        0 2019-01-28 20:05:30.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/util/__init__.py
--rw-rw-rw-   0        0        0     2568 2021-05-02 19:32:07.000000 juntagrico-webdav-1.5.0/juntagrico_webdav/views.py
-drwxrwxrwx   0        0        0        0 2022-02-08 09:34:19.810399 juntagrico-webdav-1.5.0/juntagrico_webdav.egg-info/
--rw-rw-rw-   0        0        0     3034 2022-02-08 09:34:19.000000 juntagrico-webdav-1.5.0/juntagrico_webdav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2022-02-08 09:34:19.000000 juntagrico-webdav-1.5.0/juntagrico_webdav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-08 09:34:19.000000 juntagrico-webdav-1.5.0/juntagrico_webdav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-02-08 09:34:19.000000 juntagrico-webdav-1.5.0/juntagrico_webdav.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-02-08 09:34:19.000000 juntagrico-webdav-1.5.0/juntagrico_webdav.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2022-02-08 09:33:20.000000 juntagrico-webdav-1.5.0/requirements.txt
--rw-rw-rw-   0        0        0       75 2022-02-08 09:34:19.970405 juntagrico-webdav-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1645 2021-05-02 19:18:49.000000 juntagrico-webdav-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.304076 juntagrico_webdav-1.6.0/juntagrico_webdav/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.304076 juntagrico_webdav-1.6.0/juntagrico_webdav/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/migrations/0002_auto_20191111_1501.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.300076 juntagrico_webdav-1.6.0/juntagrico_webdav/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.304076 juntagrico_webdav-1.6.0/juntagrico_webdav/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/static/js/initWDList.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.300076 juntagrico_webdav-1.6.0/juntagrico_webdav/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.300076 juntagrico_webdav-1.6.0/juntagrico_webdav/templates/juntagrico/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/juntagrico_webdav/templates/juntagrico/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/templates/juntagrico/menu/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/templates/juntagrico/menu/user.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/juntagrico_webdav/templates/wd/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/templates/wd/list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/juntagrico_webdav/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/templatetags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/juntagrico_webdav/templatetags/juntagrico_webdav/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/templatetags/juntagrico_webdav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/templatetags/juntagrico_webdav/menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/juntagrico_webdav/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/juntagrico_webdav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-05-13 21:59:48.000000 juntagrico_webdav-1.6.0/juntagrico_webdav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-13 21:59:48.000000 juntagrico_webdav-1.6.0/juntagrico_webdav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:59:48.000000 juntagrico_webdav-1.6.0/juntagrico_webdav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 21:59:48.000000 juntagrico_webdav-1.6.0/juntagrico_webdav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 21:59:48.000000 juntagrico_webdav-1.6.0/juntagrico_webdav.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 21:59:38.000000 juntagrico_webdav-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:59:48.308076 juntagrico_webdav-1.6.0/setup.cfg
```

### Comparing `juntagrico-webdav-1.5.0/LICENSE` & `juntagrico_webdav-1.6.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
-
-  0. Additional Definitions.
-
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
-
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
-
-  An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-  The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-  The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-  1. Exception to Section 3 of the GNU GPL.
-
-  You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-  2. Conveying Modified Versions.
-
-  If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
-
-  3. Object Code Incorporating Material from Library Header Files.
-
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
-
-  5. Combined Libraries.
-
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
-
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
-
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
-
-  If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
+                   GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+
+  This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+  0. Additional Definitions.
+
+  As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+  "The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+  An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+  A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+  The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+  The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+  1. Exception to Section 3 of the GNU GPL.
+
+  You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+  2. Conveying Modified Versions.
+
+  If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+   a) under this License, provided that you make a good faith effort to
+   ensure that, in the event an Application does not supply the
+   function or data, the facility still operates, and performs
+   whatever part of its purpose remains meaningful, or
+
+   b) under the GNU GPL, with none of the additional permissions of
+   this License applicable to that copy.
+
+  3. Object Code Incorporating Material from Library Header Files.
+
+  The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+   a) Give prominent notice with each copy of the object code that the
+   Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the object code with a copy of the GNU GPL and this license
+   document.
+
+  4. Combined Works.
+
+  You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+   a) Give prominent notice with each copy of the Combined Work that
+   the Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the Combined Work with a copy of the GNU GPL and this license
+   document.
+
+   c) For a Combined Work that displays copyright notices during
+   execution, include the copyright notice for the Library among
+   these notices, as well as a reference directing the user to the
+   copies of the GNU GPL and this license document.
+
+   d) Do one of the following:
+
+       0) Convey the Minimal Corresponding Source under the terms of this
+       License, and the Corresponding Application Code in a form
+       suitable for, and under terms that permit, the user to
+       recombine or relink the Application with a modified version of
+       the Linked Version to produce a modified Combined Work, in the
+       manner specified by section 6 of the GNU GPL for conveying
+       Corresponding Source.
+
+       1) Use a suitable shared library mechanism for linking with the
+       Library.  A suitable mechanism is one that (a) uses at run time
+       a copy of the Library already present on the user's computer
+       system, and (b) will operate properly with a modified version
+       of the Library that is interface-compatible with the Linked
+       Version.
+
+   e) Provide Installation Information, but only if you would otherwise
+   be required to provide such information under section 6 of the
+   GNU GPL, and only to the extent that such information is
+   necessary to install and execute a modified version of the
+   Combined Work produced by recombining or relinking the
+   Application with a modified version of the Linked Version. (If
+   you use option 4d0, the Installation Information must accompany
+   the Minimal Corresponding Source and Corresponding Application
+   Code. If you use option 4d1, you must provide the Installation
+   Information in the manner specified by section 6 of the GNU GPL
+   for conveying Corresponding Source.)
+
+  5. Combined Libraries.
+
+  You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+   a) Accompany the combined library with a copy of the same work based
+   on the Library, uncombined with any other library facilities,
+   conveyed under the terms of this License.
+
+   b) Give prominent notice with the combined library that part of it
+   is a work based on the Library, and explaining where to find the
+   accompanying uncombined form of the same work.
+
+  6. Revised Versions of the GNU Lesser General Public License.
+
+  The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+  Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+  If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
+Library.
```

### Comparing `juntagrico-webdav-1.5.0/PKG-INFO` & `juntagrico_webdav-1.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,61 @@
-Metadata-Version: 1.1
-Name: juntagrico-webdav
-Version: 1.5.0
-Summary: juntagrico-webdav
-Home-page: http://juntagrico.org
-Author: juntagrico
-Author-email: info@juntagrico.org
-License: LPGLv3
-Description: # juntagrico-webdav
-        
-        [![juntagrico-ci](https://github.com/juntagrico/juntagrico-webdav/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-webdav/actions/workflows/juntagrico-ci.yml)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/a597b9f0d54b836f1b46/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-webdav/maintainability)
-        [![Test Coverage](https://api.codeclimate.com/v1/badges/a597b9f0d54b836f1b46/test_coverage)](https://codeclimate.com/github/juntagrico/juntagrico-webdav/test_coverage)
-        [![image](https://img.shields.io/pypi/v/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
-        [![image](https://img.shields.io/pypi/l/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
-        [![image](https://img.shields.io/pypi/pyversions/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
-        [![image](https://img.shields.io/pypi/status/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
-        [![image](https://img.shields.io/pypi/dm/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav/)
-        [![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-webdav.svg)](https://github.com/juntagrico/juntagrico-webdav)
-        [![image](https://img.shields.io/github/commit-activity/y/juntagrico/juntagrico-webdav)](https://github.com/juntagrico/juntagrico-webdav)
-        [![Requirements Status](https://requires.io/github/juntagrico/juntagrico-webdav/requirements.svg?branch=main)](https://requires.io/github/juntagrico/juntagrico-webdav/requirements/?branch=main)
-        
-        This app allows to include webdav folders into juntagrico in order to share files with your members.
-        
-        This is an extension for juntagrico. You can find more information about juntagrico here
-        (https://github.com/juntagrico/juntagrico).
-        
-        For more information information about how to install this app hop over to the doc section of the repo.
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Other Audience
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+# juntagrico-webdav
+
+[![juntagrico-ci](https://github.com/juntagrico/juntagrico-webdav/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-webdav/actions/workflows/juntagrico-ci.yml)
+[![Maintainability](https://api.codeclimate.com/v1/badges/a597b9f0d54b836f1b46/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-webdav/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/a597b9f0d54b836f1b46/test_coverage)](https://codeclimate.com/github/juntagrico/juntagrico-webdav/test_coverage)
+[![image](https://img.shields.io/pypi/v/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
+[![image](https://img.shields.io/pypi/l/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
+[![image](https://img.shields.io/pypi/pyversions/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
+[![image](https://img.shields.io/pypi/status/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav)
+[![image](https://img.shields.io/pypi/dm/juntagrico-webdav.svg)](https://pypi.python.org/pypi/juntagrico-webdav/)
+[![image](https://img.shields.io/github/last-commit/juntagrico/juntagrico-webdav.svg)](https://github.com/juntagrico/juntagrico-webdav)
+[![image](https://img.shields.io/github/commit-activity/y/juntagrico/juntagrico-webdav)](https://github.com/juntagrico/juntagrico-webdav)
+[![Requirements Status](https://requires.io/github/juntagrico/juntagrico-webdav/requirements.svg?branch=main)](https://requires.io/github/juntagrico/juntagrico-webdav/requirements/?branch=main)
+
+This app allows to include webdav folders into juntagrico in order to share files with your members.
+
+This is an extension for juntagrico. You can find more information about juntagrico here
+(https://github.com/juntagrico/juntagrico).
+
+# Installation
+
+Install juntagrico-webdav via `pip`
+
+    $ pip install juntagrico-webdav
+
+or add it in your projects `requirements.txt`
+
+In `settings.py` add `'juntagrico_webdav',` **before** juntagrico.
+
+```python
+INSTALLED_APPS = [
+    ...
+    'juntagrico_webdav',
+    'juntagrico',
+]
+```
+
+To avoid reloading the files list all the time, configure caching in `settings.py`
+
+```python
+CACHES = {
+    'default': {
+        'BACKEND': 'django.core.cache.backends.db.DatabaseCache',
+        'LOCATION': 'juntagrico_app_cache_table',
+        'TIMEOUT': None,
+    }
+}
+```
+
+then run
+
+    $ python -m manage createcachetable
+
+In your `urls.py` you also need to extend the pattern:
+
+```python
+urlpatterns = [
+    ...
+    path('', include('juntagrico_webdav.urls')),
+]
+```
```

### Comparing `juntagrico-webdav-1.5.0/juntagrico_webdav/migrations/0001_initial.py` & `juntagrico_webdav-1.6.0/juntagrico_webdav/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Generated by Django 2.1.3 on 2019-01-28 22:00
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='WebdavServer',
-            fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('name', models.CharField(default='', max_length=100, verbose_name='Name')),
-                ('url', models.CharField(default='', max_length=100, verbose_name='Server URL')),
-                ('path', models.CharField(default='', max_length=100, verbose_name='Ordner Pfad')),
-                ('username', models.CharField(default='', max_length=100, verbose_name='Benutzer Name')),
-                ('password', models.CharField(default='', max_length=100, verbose_name='Passwort')),
-                ('menu_title', models.CharField(default='', max_length=100, verbose_name='Menu Titel')),
-                ('active', models.BooleanField(default=True, verbose_name='aktiv')),
-                ('type', models.PositiveIntegerField(choices=[(1, 'User'), (2, 'Admin')], verbose_name='Typ')),
-            ],
-        ),
-    ]
+# Generated by Django 2.1.3 on 2019-01-28 22:00
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='WebdavServer',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(default='', max_length=100, verbose_name='Name')),
+                ('url', models.CharField(default='', max_length=100, verbose_name='Server URL')),
+                ('path', models.CharField(default='', max_length=100, verbose_name='Ordner Pfad')),
+                ('username', models.CharField(default='', max_length=100, verbose_name='Benutzer Name')),
+                ('password', models.CharField(default='', max_length=100, verbose_name='Passwort')),
+                ('menu_title', models.CharField(default='', max_length=100, verbose_name='Menu Titel')),
+                ('active', models.BooleanField(default=True, verbose_name='aktiv')),
+                ('type', models.PositiveIntegerField(choices=[(1, 'User'), (2, 'Admin')], verbose_name='Typ')),
+            ],
+        ),
+    ]
```

### Comparing `juntagrico-webdav-1.5.0/juntagrico_webdav/migrations/0002_auto_20191111_1501.py` & `juntagrico_webdav-1.6.0/juntagrico_webdav/migrations/0002_auto_20191111_1501.py`

 * *Files identical despite different names*

### Comparing `juntagrico-webdav-1.5.0/juntagrico_webdav/templates/wd/list.html` & `juntagrico_webdav-1.6.0/juntagrico_webdav/templates/wd/list.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 00000000: 7b25 2065 7874 656e 6473 2022 6261 7365  {% extends "base
 00000010: 2e68 746d 6c22 2025 7d0a 7b25 206c 6f61  .html" %}.{% loa
-00000020: 6420 6a75 6e74 6167 7269 636f 2e63 6f6e  d juntagrico.con
-00000030: 6669 6720 257d 0a7b 2520 626c 6f63 6b20  fig %}.{% block 
-00000040: 7061 6765 5f74 6974 6c65 2025 7d0a 2020  page_title %}.  
-00000050: 2020 3c68 333e 7b7b 7765 6264 6176 5f73    <h3>{{webdav_s
-00000060: 6572 7665 722e 6e61 6d65 7d7d 3c2f 6833  erver.name}}</h3
-00000070: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
-00000080: 0a0a 7b25 2062 6c6f 636b 2063 6f6e 7465  ..{% block conte
-00000090: 6e74 2025 7d0a 2020 2020 203c 7461 626c  nt %}.     <tabl
-000000a0: 6520 6964 3d22 6669 6c74 6572 2d74 6162  e id="filter-tab
-000000b0: 6c65 2220 636c 6173 733d 226c 6973 7420  le" class="list 
-000000c0: 7461 626c 6522 2073 7479 6c65 3d22 6469  table" style="di
-000000d0: 7370 6c61 793a 2074 6162 6c65 3b22 3e0a  splay: table;">.
-000000e0: 2020 2020 2020 2020 3c74 6865 6164 3e0a          <thead>.
-000000f0: 2020 2020 2020 2020 3c74 723e 0a20 2020          <tr>.   
-00000100: 2020 2020 2020 2020 203c 7468 3e4e 616d           <th>Nam
-00000110: 653c 2f74 683e 0a20 2020 2020 2020 2020  e</th>.         
-00000120: 2020 203c 7468 3e47 65c3 a46e 6465 7274     <th>Ge..ndert
-00000130: 3c2f 7468 3e0a 2020 2020 2020 2020 3c2f  </th>.        </
-00000140: 7472 3e0a 2020 2020 2020 2020 3c2f 7468  tr>.        </th
-00000150: 6561 643e 0a20 2020 2020 2020 203c 7462  ead>.        <tb
-00000160: 6f64 793e 0a20 2020 2020 2020 207b 2520  ody>.        {% 
-00000170: 666f 7220 6669 6c65 2069 6e20 6669 6c65  for file in file
-00000180: 7320 257d 0a20 2020 2020 2020 2020 2020  s %}.           
-00000190: 203c 7472 3e0a 2020 2020 2020 2020 2020   <tr>.          
-000001a0: 2020 2020 2020 3c74 643e 0a20 2020 2020        <td>.     
-000001b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000001c0: 6120 6872 6566 3d22 7b25 2075 726c 2027  a href="{% url '
-000001d0: 7765 6264 6176 3a67 6574 2d66 696c 6527  webdav:get-file'
-000001e0: 2069 643d 7765 6264 6176 5f73 6572 7665   id=webdav_serve
-000001f0: 722e 6964 2066 696c 653d 6669 6c65 2e75  r.id file=file.u
-00000200: 726c 2025 7d22 3e7b 7b20 6669 6c65 2e6e  rl %}">{{ file.n
-00000210: 616d 6520 7d7d 3c2f 613e 0a20 2020 2020  ame }}</a>.     
-00000220: 2020 2020 2020 2020 2020 203c 2f74 643e             </td>
-00000230: 3c74 643e 0a20 2020 2020 2020 2020 2020  <td>.           
-00000240: 2020 2020 2020 2020 207b 7b20 6669 6c65           {{ file
-00000250: 2e64 6174 6520 7d7d 0a20 2020 2020 2020  .date }}.       
-00000260: 2020 2020 2020 2020 203c 2f74 643e 0a20           </td>. 
-00000270: 2020 2020 2020 2020 2020 203c 2f74 723e             </tr>
-00000280: 0a20 2020 2020 2020 207b 2520 656e 6466  .        {% endf
-00000290: 6f72 2025 7d0a 2020 2020 2020 2020 3c2f  or %}.        </
-000002a0: 7462 6f64 793e 0a20 2020 203c 2f74 6162  tbody>.    </tab
-000002b0: 6c65 3e0a 2020 2020 0a7b 2520 656e 6462  le>.    .{% endb
-000002c0: 6c6f 636b 2025 7d0a 0a7b 2520 626c 6f63  lock %}..{% bloc
-000002d0: 6b20 7363 7269 7074 7320 257d 0a20 2020  k scripts %}.   
-000002e0: 203c 7363 7269 7074 2074 7970 653d 2274   <script type="t
-000002f0: 6578 742f 6a61 7661 7363 7269 7074 2220  ext/javascript" 
-00000300: 7372 633d 222f 7374 6174 6963 2f65 7874  src="/static/ext
-00000310: 6572 6e61 6c2f 6461 7461 7461 626c 6573  ernal/datatables
-00000320: 2e6d 696e 2e6a 7322 3e3c 2f73 6372 6970  .min.js"></scrip
-00000330: 743e 0a20 2020 203c 7363 7269 7074 2074  t>.    <script t
-00000340: 7970 653d 2274 6578 742f 6a61 7661 7363  ype="text/javasc
-00000350: 7269 7074 2220 7372 633d 222f 7374 6174  ript" src="/stat
-00000360: 6963 2f65 7874 6572 6e61 6c2f 7265 7175  ic/external/requ
-00000370: 6972 652e 6d69 6e2e 6a73 2220 6461 7461  ire.min.js" data
-00000380: 2d6d 6169 6e3d 222f 7374 6174 6963 2f6a  -main="/static/j
-00000390: 732f 696e 6974 5744 4c69 7374 2e6a 7322  s/initWDList.js"
-000003a0: 3e3c 2f73 6372 6970 743e 0a7b 2520 656e  ></script>.{% en
-000003b0: 6462 6c6f 636b 2025 7d0a                 dblock %}.
+00000020: 6420 7374 6174 6963 2025 7d0a 7b25 206c  d static %}.{% l
+00000030: 6f61 6420 6a75 6e74 6167 7269 636f 2e63  oad juntagrico.c
+00000040: 6f6e 6669 6720 257d 0a7b 2520 626c 6f63  onfig %}.{% bloc
+00000050: 6b20 7061 6765 5f74 6974 6c65 2025 7d0a  k page_title %}.
+00000060: 2020 2020 3c68 333e 7b7b 7765 6264 6176      <h3>{{webdav
+00000070: 5f73 6572 7665 722e 6e61 6d65 7d7d 3c2f  _server.name}}</
+00000080: 6833 3e0a 7b25 2065 6e64 626c 6f63 6b20  h3>.{% endblock 
+00000090: 257d 0a0a 7b25 2062 6c6f 636b 2063 6f6e  %}..{% block con
+000000a0: 7465 6e74 2025 7d0a 2020 2020 203c 7461  tent %}.     <ta
+000000b0: 626c 6520 6964 3d22 6669 6c74 6572 2d74  ble id="filter-t
+000000c0: 6162 6c65 2220 636c 6173 733d 226c 6973  able" class="lis
+000000d0: 7420 7461 626c 6522 3e0a 2020 2020 2020  t table">.      
+000000e0: 2020 3c74 6865 6164 3e0a 2020 2020 2020    <thead>.      
+000000f0: 2020 3c74 723e 0a20 2020 2020 2020 2020    <tr>.         
+00000100: 2020 203c 7468 3e4e 616d 653c 2f74 683e     <th>Name</th>
+00000110: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
+00000120: 3e47 65c3 a46e 6465 7274 3c2f 7468 3e0a  >Ge..ndert</th>.
+00000130: 2020 2020 2020 2020 3c2f 7472 3e0a 2020          </tr>.  
+00000140: 2020 2020 2020 3c2f 7468 6561 643e 0a20        </thead>. 
+00000150: 2020 2020 2020 203c 7462 6f64 793e 0a20         <tbody>. 
+00000160: 2020 2020 2020 207b 2520 666f 7220 6669         {% for fi
+00000170: 6c65 2069 6e20 6669 6c65 7320 257d 0a20  le in files %}. 
+00000180: 2020 2020 2020 2020 2020 203c 7472 3e0a             <tr>.
+00000190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000001a0: 3c74 643e 0a20 2020 2020 2020 2020 2020  <td>.           
+000001b0: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
+000001c0: 3d22 7b25 2075 726c 2027 7765 6264 6176  ="{% url 'webdav
+000001d0: 3a67 6574 2d66 696c 6527 2069 643d 7765  :get-file' id=we
+000001e0: 6264 6176 5f73 6572 7665 722e 6964 2066  bdav_server.id f
+000001f0: 696c 653d 6669 6c65 2e75 726c 2025 7d22  ile=file.url %}"
+00000200: 3e7b 7b20 6669 6c65 2e6e 616d 6520 7d7d  >{{ file.name }}
+00000210: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
+00000220: 2020 2020 203c 2f74 643e 3c74 643e 0a20       </td><td>. 
+00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000240: 2020 207b 7b20 6669 6c65 2e64 6174 6520     {{ file.date 
+00000250: 7d7d 0a20 2020 2020 2020 2020 2020 2020  }}.             
+00000260: 2020 203c 2f74 643e 0a20 2020 2020 2020     </td>.       
+00000270: 2020 2020 203c 2f74 723e 0a20 2020 2020       </tr>.     
+00000280: 2020 207b 2520 656e 6466 6f72 2025 7d0a     {% endfor %}.
+00000290: 2020 2020 2020 2020 3c2f 7462 6f64 793e          </tbody>
+000002a0: 0a20 2020 203c 2f74 6162 6c65 3e0a 7b25  .    </table>.{%
+000002b0: 2065 6e64 626c 6f63 6b20 257d 0a0a 7b25   endblock %}..{%
+000002c0: 2062 6c6f 636b 2073 6372 6970 7473 2025   block scripts %
+000002d0: 7d0a 2020 2020 3c73 6372 6970 7420 7479  }.    <script ty
+000002e0: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+000002f0: 6970 7422 2073 7263 3d22 7b25 2073 7461  ipt" src="{% sta
+00000300: 7469 6320 226a 756e 7461 6772 6963 6f2f  tic "juntagrico/
+00000310: 6578 7465 726e 616c 2f64 6174 6174 6162  external/datatab
+00000320: 6c65 732f 6461 7461 7461 626c 6573 2e6d  les/datatables.m
+00000330: 696e 2e6a 7322 2025 7d22 3e3c 2f73 6372  in.js" %}"></scr
+00000340: 6970 743e 0a20 2020 203c 7363 7269 7074  ipt>.    <script
+00000350: 2074 7970 653d 2274 6578 742f 6a61 7661   type="text/java
+00000360: 7363 7269 7074 223e 0a20 2020 2020 2020  script">.       
+00000370: 2024 2866 756e 6374 696f 6e28 297b 0a20   $(function(){. 
+00000380: 2020 2020 2020 2020 2020 2024 2822 2366             $("#f
+00000390: 696c 7465 722d 7461 626c 6522 292e 4461  ilter-table").Da
+000003a0: 7461 5461 626c 6528 7b22 6f72 6465 7269  taTable({"orderi
+000003b0: 6e67 223a 2074 7275 657d 293b 0a20 2020  ng": true});.   
+000003c0: 2020 2020 207d 290a 2020 2020 3c2f 7363       }).    </sc
+000003d0: 7269 7074 3e0a 7b25 2065 6e64 626c 6f63  ript>.{% endbloc
+000003e0: 6b20 257d 0a                             k %}.
```

### Comparing `juntagrico-webdav-1.5.0/juntagrico_webdav/views.py` & `juntagrico_webdav-1.6.0/juntagrico_webdav/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,73 @@
+import os
 import requests
 import dateparser
 from xml.etree import ElementTree as ET
-from re import sub
 from urllib.parse import unquote, urlsplit
 
-from django.shortcuts import render, get_object_or_404
+from django.shortcuts import render, get_object_or_404, redirect
 from django.http import HttpResponse, Http404
 from django.contrib.auth.decorators import login_required
-from juntagrico_webdav.entity.servers import WebdavServer
+from juntagrico_webdav.models import WebdavServer
 
 
 @login_required
 def list(request, id):
     server = get_object_or_404(WebdavServer, pk=id)
+    if server.type == WebdavServer.ADMIN_SERVER and not request.user.is_staff:
+        return redirect('home')
     url = server.url + '/' + server.path
     username = server.username
     password = server.password
     session = requests.Session()
     session.auth = (username, password)
     session.get(url)
     headers = {'Accept': '*/*', 'Depth': '1'}
     response = session.request('PROPFIND', url, headers=headers)
     files = []
+    last_mod_datetime = None
     tree = ET.fromstring(response.content)
     for prop in tree.findall('./{DAV:}response'):
-        href = prop.find('./{DAV:}href').text
-        href = sub("/.+/", '/', href)[1:]
-        name = unquote(urlsplit(href).path)
+        collection_element = prop.find(".//{DAV:}resourcetype/{DAV:}collection")
+        if collection_element is not None:
+            # skip folders
+            continue
+        href = prop.find("./{DAV:}href").text
+        href = urlsplit(href).path
+        href = os.path.basename(href)
+        name = unquote(href)
         last_mod_date = prop.find('.//{DAV:}getlastmodified').text
         last_mod_datetime = dateparser.parse(last_mod_date, languages=['en'])
         if last_mod_datetime is not None:
             last_mod_date = last_mod_datetime.strftime("%d.%m.%Y %H:%M:%S")
         if name != '':
             element = {'url': href,
                        'name': name,
                        'date': last_mod_date,
                        'datetime': last_mod_datetime}
             files.append(element)
-    if server.sortby < 3 or last_mod_datetime is None:
+    if server.sorted_by_name or last_mod_datetime is None:
         files.sort(key=lambda x: x['name'])
-        if server.sortby == 2:
-            files.reverse()
     else:
         files.sort(key=lambda x: x['datetime'])
-        if server.sortby == 4:
-            files.reverse()
+    if server.sorted_desc:
+        files.reverse()
     renderdict = {
         'webdav_server': server,
         'files': files,
         'menu': {'wd': 'active'},
     }
     return render(request, "wd/list.html", renderdict)
 
 
 @login_required
 def get_item(request, id, file):
     server = get_object_or_404(WebdavServer, pk=id)
+    if server.type == WebdavServer.ADMIN_SERVER and not request.user.is_staff:
+        return redirect('home')
     url = server.url + '/' + server.path + '/' + file
     username = server.username
     password = server.password
     session = requests.Session()
     session.auth = (username, password)
     session.get(url)
     file_response = session.request('GET', url)
```

### Comparing `juntagrico-webdav-1.5.0/juntagrico_webdav.egg-info/SOURCES.txt` & `juntagrico_webdav-1.6.0/juntagrico_webdav.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
 juntagrico_webdav/__init__.py
 juntagrico_webdav/admin.py
 juntagrico_webdav/apps.py
-juntagrico_webdav/juntagricoapp.py
 juntagrico_webdav/models.py
 juntagrico_webdav/urls.py
 juntagrico_webdav/views.py
 juntagrico_webdav.egg-info/PKG-INFO
 juntagrico_webdav.egg-info/SOURCES.txt
 juntagrico_webdav.egg-info/dependency_links.txt
 juntagrico_webdav.egg-info/requires.txt
 juntagrico_webdav.egg-info/top_level.txt
-juntagrico_webdav/dao/__init__.py
-juntagrico_webdav/dao/webdavserverdao.py
-juntagrico_webdav/entity/__init__.py
-juntagrico_webdav/entity/servers.py
 juntagrico_webdav/migrations/0001_initial.py
 juntagrico_webdav/migrations/0002_auto_20191111_1501.py
 juntagrico_webdav/migrations/__init__.py
 juntagrico_webdav/static/js/initWDList.js
-juntagrico_webdav/templates/wd/admin_menu.html
+juntagrico_webdav/templates/juntagrico/menu/admin.html
+juntagrico_webdav/templates/juntagrico/menu/user.html
 juntagrico_webdav/templates/wd/list.html
-juntagrico_webdav/templates/wd/menu.html
 juntagrico_webdav/templatetags/__init__.py
-juntagrico_webdav/templatetags/menus.py
-juntagrico_webdav/util/__init__.py
+juntagrico_webdav/templatetags/juntagrico_webdav/__init__.py
+juntagrico_webdav/templatetags/juntagrico_webdav/menus.py
```

