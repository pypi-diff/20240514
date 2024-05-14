# Comparing `tmp/trame-quasar-0.2.0.tar.gz` & `tmp/trame-quasar-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-quasar-0.2.0.tar", last modified: Fri Aug 25 17:49:22 2023, max compression
+gzip compressed data, was "trame-quasar-0.2.1.tar", last modified: Tue May 14 00:28:27 2024, max compression
```

## Comparing `trame-quasar-0.2.0.tar` & `trame-quasar-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.175957 trame-quasar-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1960 2023-08-25 17:49:22.175957 trame-quasar-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1220 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      883 2023-08-25 17:49:22.175957 trame-quasar-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.167957 trame-quasar-0.2.0/trame/
--rw-r--r--   0 root         (0) root         (0)       64 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.167957 trame-quasar-0.2.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       64 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame/modules/quasar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.167957 trame-quasar-0.2.0/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       65 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       37 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/trame/ui/quasar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.171957 trame-quasar-0.2.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       64 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame/widgets/quasar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.171957 trame-quasar-0.2.0/trame_quasar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.171957 trame-quasar-0.2.0/trame_quasar/module/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.171957 trame-quasar-0.2.0/trame_quasar/module/quasar/
--rw-r--r--   0 root         (0) root         (0)      359 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/module/quasar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.175957 trame-quasar-0.2.0/trame_quasar/module/quasar/vue3/
--rw-r--r--   0 root         (0) root         (0)   510477 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/module/quasar/vue3/1.js
--rw-r--r--   0 root         (0) root         (0)     1549 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/module/quasar/vue3/2.css
--rw-r--r--   0 root         (0) root         (0)   204012 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/module/quasar/vue3/3.css
--rw-r--r--   0 root         (0) root         (0)      398 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/module/quasar/vue3/trame_utils.js
--rw-r--r--   0 root         (0) root         (0)      302 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/module/quasar/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.175957 trame-quasar-0.2.0/trame_quasar/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/trame_quasar/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)      672 2023-08-25 17:48:42.000000 trame-quasar-0.2.0/trame_quasar/ui/quasar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.175957 trame-quasar-0.2.0/trame_quasar/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)   380824 2023-08-25 17:48:55.000000 trame-quasar-0.2.0/trame_quasar/widgets/quasar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 17:49:22.171957 trame-quasar-0.2.0/trame_quasar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1960 2023-08-25 17:49:22.000000 trame-quasar-0.2.0/trame_quasar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      795 2023-08-25 17:49:22.000000 trame-quasar-0.2.0/trame_quasar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-25 17:49:22.000000 trame-quasar-0.2.0/trame_quasar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-25 17:49:22.000000 trame-quasar-0.2.0/trame_quasar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-08-25 17:49:22.000000 trame-quasar-0.2.0/trame_quasar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.460245 trame-quasar-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1960 2024-05-14 00:28:27.460245 trame-quasar-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      883 2024-05-14 00:28:27.460245 trame-quasar-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.452245 trame-quasar-0.2.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.452245 trame-quasar-0.2.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame/modules/quasar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.452245 trame-quasar-0.2.1/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/trame/ui/quasar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.452245 trame-quasar-0.2.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame/widgets/quasar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.452245 trame-quasar-0.2.1/trame_quasar/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame_quasar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.456245 trame-quasar-0.2.1/trame_quasar/module/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame_quasar/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.456245 trame-quasar-0.2.1/trame_quasar/module/quasar/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.460245 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/
+-rw-r--r--   0 root         (0) root         (0)   510477 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/1.js
+-rw-r--r--   0 root         (0) root         (0)   204012 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/2.css
+-rw-r--r--   0 root         (0) root         (0)   129724 2024-05-14 00:28:09.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/KFOkCnqEu92Fr1MmgWxP.ttf
+-rw-r--r--   0 root         (0) root         (0)   129768 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/KFOlCnqEu92Fr1MmEU9vAw.ttf
+-rw-r--r--   0 root         (0) root         (0)   128256 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/KFOlCnqEu92Fr1MmSU5vAw.ttf
+-rw-r--r--   0 root         (0) root         (0)   128676 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/KFOlCnqEu92Fr1MmWUlvAw.ttf
+-rw-r--r--   0 root         (0) root         (0)   129228 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/KFOlCnqEu92Fr1MmYUtvAw.ttf
+-rw-r--r--   0 root         (0) root         (0)   129584 2024-05-14 00:28:10.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/KFOmCnqEu92Fr1Me5Q.ttf
+-rw-r--r--   0 root         (0) root         (0)   356840 2024-05-14 00:28:09.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/flUhRq6tzZclQEJ-Vdg-IuiaDsNZ.ttf
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/fonts.css
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/trame_utils.js
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/module/quasar/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.460245 trame-quasar-0.2.1/trame_quasar/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/trame_quasar/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-14 00:27:59.000000 trame-quasar-0.2.1/trame_quasar/ui/quasar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.460245 trame-quasar-0.2.1/trame_quasar/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   380824 2024-05-14 00:28:11.000000 trame-quasar-0.2.1/trame_quasar/widgets/quasar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 00:28:27.456245 trame-quasar-0.2.1/trame_quasar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1960 2024-05-14 00:28:27.000000 trame-quasar-0.2.1/trame_quasar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-05-14 00:28:27.000000 trame-quasar-0.2.1/trame_quasar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 00:28:27.000000 trame-quasar-0.2.1/trame_quasar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-14 00:28:27.000000 trame-quasar-0.2.1/trame_quasar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-14 00:28:27.000000 trame-quasar-0.2.1/trame_quasar.egg-info/top_level.txt
```

### Comparing `trame-quasar-0.2.0/LICENSE` & `trame-quasar-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-quasar-0.2.0/PKG-INFO` & `trame-quasar-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-quasar
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quasar widget library for trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-quasar-0.2.0/README.rst` & `trame-quasar-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-quasar-0.2.0/setup.cfg` & `trame-quasar-0.2.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-quasar
-version = 0.2.0
+version = 0.2.1
 description = Quasar widget library for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-quasar-0.2.0/trame_quasar/module/quasar/vue3/1.js` & `trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/1.js`

 * *Files identical despite different names*

### Comparing `trame-quasar-0.2.0/trame_quasar/module/quasar/vue3/3.css` & `trame-quasar-0.2.1/trame_quasar/module/quasar/vue3/2.css`

 * *Files identical despite different names*

### Comparing `trame-quasar-0.2.0/trame_quasar/ui/quasar.py` & `trame-quasar-0.2.1/trame_quasar/ui/quasar.py`

 * *Files identical despite different names*

### Comparing `trame-quasar-0.2.0/trame_quasar/widgets/quasar.py` & `trame-quasar-0.2.1/trame_quasar/widgets/quasar.py`

 * *Files 0% similar despite different names*

```diff
@@ -23626,44 +23626,44 @@
 0005c490: 2020 5d0a 2020 2020 2020 2020 7365 6c66    ].        self
 0005c4a0: 2e5f 6576 656e 745f 6e61 6d65 7320 2b3d  ._event_names +=
 0005c4b0: 205b 0a20 2020 2020 2020 2020 2020 2022   [.            "
 0005c4c0: 7669 7274 7561 6c5f 7363 726f 6c6c 222c  virtual_scroll",
 0005c4d0: 0a20 2020 2020 2020 205d 0a0a 0a41 6273  .        ]...Abs
 0005c4e0: 7472 6163 7445 6c65 6d65 6e74 2e72 6567  tractElement.reg
 0005c4f0: 6973 7465 725f 6469 7265 6374 6976 6528  ister_directive(
-0005c500: 2276 2d69 6e74 6572 7365 6374 696f 6e22  "v-intersection"
-0005c510: 290a 4162 7374 7261 6374 456c 656d 656e  ).AbstractElemen
-0005c520: 742e 7265 6769 7374 6572 5f64 6972 6563  t.register_direc
-0005c530: 7469 7665 2822 762d 7363 726f 6c6c 2d66  tive("v-scroll-f
-0005c540: 6972 6522 290a 4162 7374 7261 6374 456c  ire").AbstractEl
-0005c550: 656d 656e 742e 7265 6769 7374 6572 5f64  ement.register_d
-0005c560: 6972 6563 7469 7665 2822 762d 636c 6f73  irective("v-clos
-0005c570: 652d 706f 7075 7022 290a 4162 7374 7261  e-popup").Abstra
-0005c580: 6374 456c 656d 656e 742e 7265 6769 7374  ctElement.regist
-0005c590: 6572 5f64 6972 6563 7469 7665 2822 762d  er_directive("v-
-0005c5a0: 7363 726f 6c6c 2229 0a41 6273 7472 6163  scroll").Abstrac
-0005c5b0: 7445 6c65 6d65 6e74 2e72 6567 6973 7465  tElement.registe
-0005c5c0: 725f 6469 7265 6374 6976 6528 2276 2d6d  r_directive("v-m
-0005c5d0: 7574 6174 696f 6e22 290a 4162 7374 7261  utation").Abstra
-0005c5e0: 6374 456c 656d 656e 742e 7265 6769 7374  ctElement.regist
-0005c5f0: 6572 5f64 6972 6563 7469 7665 2822 762d  er_directive("v-
-0005c600: 746f 7563 682d 7061 6e22 290a 4162 7374  touch-pan").Abst
-0005c610: 7261 6374 456c 656d 656e 742e 7265 6769  ractElement.regi
-0005c620: 7374 6572 5f64 6972 6563 7469 7665 2822  ster_directive("
-0005c630: 762d 746f 7563 682d 7377 6970 6522 290a  v-touch-swipe").
-0005c640: 4162 7374 7261 6374 456c 656d 656e 742e  AbstractElement.
-0005c650: 7265 6769 7374 6572 5f64 6972 6563 7469  register_directi
-0005c660: 7665 2822 762d 746f 7563 682d 7265 7065  ve("v-touch-repe
-0005c670: 6174 2229 0a41 6273 7472 6163 7445 6c65  at").AbstractEle
-0005c680: 6d65 6e74 2e72 6567 6973 7465 725f 6469  ment.register_di
-0005c690: 7265 6374 6976 6528 2276 2d6d 6f72 7068  rective("v-morph
-0005c6a0: 2229 0a41 6273 7472 6163 7445 6c65 6d65  ").AbstractEleme
-0005c6b0: 6e74 2e72 6567 6973 7465 725f 6469 7265  nt.register_dire
-0005c6c0: 6374 6976 6528 2276 2d74 6f75 6368 2d68  ctive("v-touch-h
-0005c6d0: 6f6c 6422 290a 4162 7374 7261 6374 456c  old").AbstractEl
+0005c500: 2276 2d74 6f75 6368 2d68 6f6c 6422 290a  "v-touch-hold").
+0005c510: 4162 7374 7261 6374 456c 656d 656e 742e  AbstractElement.
+0005c520: 7265 6769 7374 6572 5f64 6972 6563 7469  register_directi
+0005c530: 7665 2822 762d 696e 7465 7273 6563 7469  ve("v-intersecti
+0005c540: 6f6e 2229 0a41 6273 7472 6163 7445 6c65  on").AbstractEle
+0005c550: 6d65 6e74 2e72 6567 6973 7465 725f 6469  ment.register_di
+0005c560: 7265 6374 6976 6528 2276 2d74 6f75 6368  rective("v-touch
+0005c570: 2d73 7769 7065 2229 0a41 6273 7472 6163  -swipe").Abstrac
+0005c580: 7445 6c65 6d65 6e74 2e72 6567 6973 7465  tElement.registe
+0005c590: 725f 6469 7265 6374 6976 6528 2276 2d73  r_directive("v-s
+0005c5a0: 6372 6f6c 6c2d 6669 7265 2229 0a41 6273  croll-fire").Abs
+0005c5b0: 7472 6163 7445 6c65 6d65 6e74 2e72 6567  tractElement.reg
+0005c5c0: 6973 7465 725f 6469 7265 6374 6976 6528  ister_directive(
+0005c5d0: 2276 2d74 6f75 6368 2d72 6570 6561 7422  "v-touch-repeat"
+0005c5e0: 290a 4162 7374 7261 6374 456c 656d 656e  ).AbstractElemen
+0005c5f0: 742e 7265 6769 7374 6572 5f64 6972 6563  t.register_direc
+0005c600: 7469 7665 2822 762d 636c 6f73 652d 706f  tive("v-close-po
+0005c610: 7075 7022 290a 4162 7374 7261 6374 456c  pup").AbstractEl
+0005c620: 656d 656e 742e 7265 6769 7374 6572 5f64  ement.register_d
+0005c630: 6972 6563 7469 7665 2822 762d 746f 7563  irective("v-touc
+0005c640: 682d 7061 6e22 290a 4162 7374 7261 6374  h-pan").Abstract
+0005c650: 456c 656d 656e 742e 7265 6769 7374 6572  Element.register
+0005c660: 5f64 6972 6563 7469 7665 2822 762d 7363  _directive("v-sc
+0005c670: 726f 6c6c 2229 0a41 6273 7472 6163 7445  roll").AbstractE
+0005c680: 6c65 6d65 6e74 2e72 6567 6973 7465 725f  lement.register_
+0005c690: 6469 7265 6374 6976 6528 2276 2d6d 7574  directive("v-mut
+0005c6a0: 6174 696f 6e22 290a 4162 7374 7261 6374  ation").Abstract
+0005c6b0: 456c 656d 656e 742e 7265 6769 7374 6572  Element.register
+0005c6c0: 5f64 6972 6563 7469 7665 2822 762d 6d6f  _directive("v-mo
+0005c6d0: 7270 6822 290a 4162 7374 7261 6374 456c  rph").AbstractEl
 0005c6e0: 656d 656e 742e 7265 6769 7374 6572 5f64  ement.register_d
 0005c6f0: 6972 6563 7469 7665 2822 762d 7269 7070  irective("v-ripp
 0005c700: 6c65 2229 0a0a 0a5f 5f61 6c6c 5f5f 203d  le")...__all__ =
 0005c710: 205b 0a20 2020 2022 5141 6a61 7842 6172   [.    "QAjaxBar
 0005c720: 222c 0a20 2020 2022 5141 7661 7461 7222  ",.    "QAvatar"
 0005c730: 2c0a 2020 2020 2251 4261 6467 6522 2c0a  ,.    "QBadge",.
 0005c740: 2020 2020 2251 4261 6e6e 6572 222c 0a20      "QBanner",.
```

### Comparing `trame-quasar-0.2.0/trame_quasar.egg-info/PKG-INFO` & `trame-quasar-0.2.1/trame_quasar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-quasar
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quasar widget library for trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

