# Comparing `tmp/firmitas-0.1.2.tar.gz` & `tmp/firmitas-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firmitas-0.1.2.tar", max compression
+gzip compressed data, was "firmitas-0.1.3a0.tar", max compression
```

## Comparing `firmitas-0.1.2.tar` & `firmitas-0.1.3a0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    35148 2023-06-06 13:46:04.925465 firmitas-0.1.2/LICENSE
--rw-r--r--   0        0        0     9560 2023-06-06 13:46:04.925465 firmitas-0.1.2/README.md
--rw-r--r--   0        0        0     2037 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/base/__init__.py
--rw-r--r--   0        0        0     7304 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/base/maintool.py
--rw-r--r--   0        0        0        0 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/__init__.py
--rw-r--r--   0        0        0    19059 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/certlist.yml
--rw-r--r--   0        0        0      203 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/logrdata.py
--rw-r--r--   0        0        0     1611 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/conf/standard.py
--rw-r--r--   0        0        0      617 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/main.py
--rw-r--r--   0        0        0     1147 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/unit/gogithub.py
--rw-r--r--   0        0        0     2096 2023-06-06 13:46:04.925465 firmitas-0.1.2/firmitas/unit/gopagure.py
--rw-r--r--   0        0        0     1780 2023-06-08 05:48:14.087401 firmitas-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    11103 1970-01-01 00:00:00.000000 firmitas-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-22 04:48:14.266789 firmitas-0.1.3a0/LICENSE
+-rw-r--r--   0        0        0     9560 2024-04-22 04:48:14.266789 firmitas-0.1.3a0/README.md
+-rw-r--r--   0        0        0     2921 2024-05-14 09:20:43.700142 firmitas-0.1.3a0/firmitas/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-14 09:20:43.701141 firmitas-0.1.3a0/firmitas/base/__init__.py
+-rw-r--r--   0        0        0     8020 2024-05-14 09:20:43.702142 firmitas-0.1.3a0/firmitas/base/maintool.py
+-rw-r--r--   0        0        0      882 2024-05-14 09:20:43.702142 firmitas-0.1.3a0/firmitas/conf/__init__.py
+-rw-r--r--   0        0        0    19059 2024-04-22 04:48:14.266789 firmitas-0.1.3a0/firmitas/conf/certlist.yml
+-rw-r--r--   0        0        0    19059 2024-04-24 02:42:43.492215 firmitas-0.1.3a0/firmitas/conf/certlist.yml.save
+-rw-r--r--   0        0        0     1087 2024-05-14 09:20:43.702142 firmitas-0.1.3a0/firmitas/conf/logrdata.py
+-rw-r--r--   0        0        0     2602 2024-05-14 09:20:43.702142 firmitas-0.1.3a0/firmitas/conf/standard.py
+-rw-r--r--   0        0        0     1511 2024-05-14 09:20:43.702142 firmitas-0.1.3a0/firmitas/main.py
+-rw-r--r--   0        0        0     2031 2024-05-14 09:20:43.702142 firmitas-0.1.3a0/firmitas/unit/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-14 09:20:43.703142 firmitas-0.1.3a0/firmitas/unit/gogithub.py
+-rw-r--r--   0        0        0      882 2024-05-14 09:20:43.703142 firmitas-0.1.3a0/firmitas/unit/gogitlab.py
+-rw-r--r--   0        0        0     3019 2024-05-14 09:20:43.703142 firmitas-0.1.3a0/firmitas/unit/gopagure.py
+-rw-r--r--   0        0        0     1674 2024-05-14 09:30:00.182020 firmitas-0.1.3a0/pyproject.toml
+-rw-r--r--   0        0        0    11156 1970-01-01 00:00:00.000000 firmitas-0.1.3a0/PKG-INFO
```

### Comparing `firmitas-0.1.2/LICENSE` & `firmitas-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.2/README.md` & `firmitas-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.2/firmitas/base/maintool.py` & `firmitas-0.1.3a0/firmitas/base/maintool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+"""
+Firmitas
+Copyright (C) 2023-2024 Akashdeep Dhar
+
+This program is free software: you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation, either version 3 of the License, or (at your option) any later
+version.
+
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
+details.
+
+You should have received a copy of the GNU General Public License along with
+this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Any Red Hat trademarks that are incorporated in the source code or
+documentation are not subject to the GNU General Public License and may only
+be used or replicated with the express permission of Red Hat, Inc.
+"""
+
+
 import os
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import yaml
 from cryptography import x509
@@ -18,35 +41,35 @@
     strtdate, stopdate = certobjc.not_valid_before, certobjc.not_valid_after
     daystobt, daystodd = (strtdate - datetime.now()).days, (stopdate - datetime.now()).days
     cstarted, cstopped = False if daystobt >= 0 else True, False if daystodd >= 0 else True
     logrdata.logrobjc.debug(f"[{commname}] Issued by {issuauth}")
     logrdata.logrobjc.debug(f"[{commname}] Serial number {serialno}")
     logrdata.logrobjc.debug(
         f"[{commname}] Valid from {strtdate} ({abs(daystobt)} days "
-        + "{'passed since beginning' if cstarted else 'left before beginning'})"
+        + f"{'passed since beginning' if cstarted else 'left before beginning'})"
     )
     logrdata.logrobjc.debug(
         f"[{commname}] Valid until {stopdate} ({abs(daystodd)} days "
-        + "{'passed since expiring' if cstopped else 'left before expiring'})"
+        + f"{'passed since expiring' if cstopped else 'left before expiring'})"
     )
     return strtdate, stopdate, cstarted, cstopped, daystobt, daystodd, issuauth, serialno
 
 
 def probedir():
     logrdata.logrobjc.info("Probing into the configured directory")
     doneqant, failqant, totlqant = 0, 0, 0
-    if os.path.exists(standard.hostloca):
-        standard.certdict = yaml.safe_load(Path(standard.hostloca).read_text())
-        logrdata.logrobjc.info(
-            f"Validating {len(standard.certdict)} X.509-standard TLS certificates"
-        )
-        for nameindx in standard.certdict:
-            totlqant += 1
-            certpath = Path(standard.certloca, standard.certdict[nameindx]["path"])
-            if os.path.exists(certpath):
+    standard.certdict = yaml.safe_load(Path(standard.hostloca).read_text())
+    logrdata.logrobjc.info(
+        f"Validating {len(standard.certdict)} X.509-standard TLS certificates"
+    )
+    for nameindx in standard.certdict:
+        totlqant += 1
+        certpath = Path(standard.certloca, standard.certdict[nameindx]["path"])
+        if os.path.exists(certpath):
+            try:
                 certobjc = x509.load_pem_x509_certificate(certpath.read_bytes(), default_backend())
                 (
                     standard.certdict[nameindx]["certstat"]["strtdate"],
                     standard.certdict[nameindx]["certstat"]["stopdate"],
                     standard.certdict[nameindx]["certstat"]["cstarted"],
                     standard.certdict[nameindx]["certstat"]["cstopped"],
                     standard.certdict[nameindx]["certstat"]["daystobt"],
@@ -55,31 +78,31 @@
                     standard.certdict[nameindx]["certstat"]["serialno"],
                 ) = readcert(certobjc)
                 doneqant += 1
                 logrdata.logrobjc.info(
                     f"[{nameindx}] The specified X.509-standard TLS certificate was read "
                     + "successfully"
                 )
-            else:
+            except ValueError:
                 failqant += 1
-                logrdata.logrobjc.warning(
-                    f"[{nameindx}] The specified X.509-standard TLS certificate could not "
-                    + "be located"
+                logrdata.logrobjc.error(
+                    f"[{nameindx}] The specified X.509-standard TLS certificate could not be read"
                 )
-        logrdata.logrobjc.info(
-            f"Of {totlqant} TLS certificates, {doneqant} TLS certificate(s) were read successfully "
-            + f"while {failqant} TLS certificate(s) could not be read"
-        )
-        with open(standard.hostloca, "w") as yamlfile:
-            yaml.safe_dump(standard.certdict, yamlfile)
-    else:
-        logrdata.logrobjc.error(
-            "Please set the directory containing the service hostname map properly"
-        )
-        sys.exit(1)
+        else:
+            failqant += 1
+            logrdata.logrobjc.warning(
+                f"[{nameindx}] The specified X.509-standard TLS certificate could not "
+                + "be located"
+            )
+    logrdata.logrobjc.info(
+        f"Of {totlqant} TLS certificates, {doneqant} TLS certificate(s) were read successfully "
+        + f"while {failqant} TLS certificate(s) could not be read"
+    )
+    with open(standard.hostloca, "w") as yamlfile:
+        yaml.safe_dump(standard.certdict, yamlfile)
 
 
 def gonotify():
     bfstrtcn, afstopcn, totlqant, succqant = 0, 0, 0, 0
     if standard.gitforge == "pagure":
         for certindx in standard.certdict:
             totlqant += 1
@@ -133,10 +156,7 @@
             yaml.safe_dump(standard.certdict, yamlfile)
     elif standard.gitforge == "gitlab":
         logrdata.logrobjc.error("The notification has not yet been implemented on GitLab")
         sys.exit(1)
     elif standard.gitforge == "github":
         logrdata.logrobjc.error("The notification has not yet been implemented on GitHub")
         sys.exit(1)
-    else:
-        logrdata.logrobjc.error("The specified ticketing repository forge is not yet supported")
-        sys.exit(1)
```

### Comparing `firmitas-0.1.2/firmitas/conf/certlist.yml` & `firmitas-0.1.3a0/firmitas/conf/certlist.yml`

 * *Files identical despite different names*

### Comparing `firmitas-0.1.2/pyproject.toml` & `firmitas-0.1.3a0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firmitas"
-version = "0.1.2"
+version = "0.1.3a"
 description = "Simple notification service for X.509-standard TLS certificate statuses"
 authors = ["Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/t0xic0der/firmitas/"
 repository = "https://gitlab.com/t0xic0der/firmitas/"
@@ -28,36 +28,28 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 click = ">=8.0.0,<9"
 cryptography = ">=36.0.0,<42"
 pyyaml = ">=5.0.0,<7"
 requests = ">=2.20.0,<3"
 
-[tool.poetry.dev-dependencies]
-black = "^23.0.0"
-isort = "^5.10.1"
-pytest = "^7.1.3"
-flake8 = "<6.0.1"
-pytest-black = "^0.3.12"
-pytest-flake8 = "^1.0.7"
-pytest-isort = "^3.0.0"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.1.3 || ^8.0.0"
+pytest-cov = "^4.1.0 || ^5.0.0"
+ruff = "^0.2.0 || ^0.3.0"
 tox = "^4.0.0"
-bandit = "^1.7.4"
+vcrpy = "^5.1.0 || ^6.0.0"
+pytest-recording = "^0.13.0"
 
-[tool.pytest.ini_options]
-addopts = "--black --isort --flake8"
-flake8-max-line-length = 100
-asyncio_mode = "auto"
-
-[tool.isort]
-line_length = 100
-profile = "black"
-
-[tool.black]
+[tool.ruff]
 line-length = 100
+fix = true
+
+[tool.ruff.lint]
+select = ["E", "F", "W", "I", "S", "B", "UP"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 firmitas = "firmitas.main:main"
```

### Comparing `firmitas-0.1.2/PKG-INFO` & `firmitas-0.1.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firmitas
-Version: 0.1.2
+Version: 0.1.3a0
 Summary: Simple notification service for X.509-standard TLS certificate statuses
 Home-page: https://gitlab.com/t0xic0der/firmitas/
 License: GPL-3.0-or-later
 Keywords: notification,security,certificate
 Author: Akashdeep Dhar
 Author-email: akashdeep.dhar@gmail.com
 Maintainer: Akashdeep Dhar
@@ -17,14 +17,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Operating System
 Requires-Dist: click (>=8.0.0,<9)
 Requires-Dist: cryptography (>=36.0.0,<42)
```

