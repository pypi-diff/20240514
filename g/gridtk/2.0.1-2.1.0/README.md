# Comparing `tmp/gridtk-2.0.1.tar.gz` & `tmp/gridtk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridtk-2.0.1.tar", last modified: Fri Mar  3 14:51:29 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `gridtk-2.0.1.tar` & `gridtk-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.259638 gridtk-2.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.255638 gridtk-2.0.1/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    34670 2023-02-10 23:04:22.000000 gridtk-2.0.1/LICENSES/GPL-3.0-or-later.txt
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-03-03 14:37:18.000000 gridtk-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2049 2023-03-03 14:51:29.259638 gridtk-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-03-03 14:48:17.000000 gridtk-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.255638 gridtk-2.0.1/doc/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-02-10 23:04:22.000000 gridtk-2.0.1/doc/api.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-03-02 21:16:18.000000 gridtk-2.0.1/doc/catalog.json
--rw-rw-rw-   0 root         (0) root         (0)     3353 2023-03-02 21:16:18.000000 gridtk-2.0.1/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-02-10 23:04:22.000000 gridtk-2.0.1/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-03-02 21:41:44.000000 gridtk-2.0.1/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-02-10 23:04:22.000000 gridtk-2.0.1/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-02-10 23:04:22.000000 gridtk-2.0.1/doc/nitpick-exceptions.txt
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-02-10 23:04:22.000000 gridtk-2.0.1/doc/usage-api.rst
--rw-rw-rw-   0 root         (0) root         (0)    13076 2023-02-10 23:04:22.000000 gridtk-2.0.1/doc/usage-cli.rst
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-03-03 14:48:17.000000 gridtk-2.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-03 14:51:29.259638 gridtk-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-02-10 23:04:22.000000 gridtk-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.251639 gridtk-2.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.255638 gridtk-2.0.1/src/gridtk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 23:04:22.000000 gridtk-2.0.1/src/gridtk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5981 2023-02-13 17:13:35.000000 gridtk-2.0.1/src/gridtk/easy.py
--rw-rw-rw-   0 root         (0) root         (0)    17416 2023-02-13 17:13:35.000000 gridtk-2.0.1/src/gridtk/local.py
--rw-rw-rw-   0 root         (0) root         (0)    16933 2023-02-13 17:13:35.000000 gridtk-2.0.1/src/gridtk/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    19115 2023-02-13 17:13:35.000000 gridtk-2.0.1/src/gridtk/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.259638 gridtk-2.0.1/src/gridtk/script/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 23:04:22.000000 gridtk-2.0.1/src/gridtk/script/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-02-13 17:13:35.000000 gridtk-2.0.1/src/gridtk/script/grid.py
--rw-rw-rw-   0 root         (0) root         (0)    26092 2023-03-02 21:16:18.000000 gridtk-2.0.1/src/gridtk/script/jman.py
--rw-rw-rw-   0 root         (0) root         (0)     4617 2023-02-13 17:13:35.000000 gridtk-2.0.1/src/gridtk/setshell.py
--rw-rw-rw-   0 root         (0) root         (0)    11248 2023-02-13 17:13:35.000000 gridtk-2.0.1/src/gridtk/sge.py
--rw-rw-rw-   0 root         (0) root         (0)    10623 2023-03-02 21:16:18.000000 gridtk-2.0.1/src/gridtk/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.259638 gridtk-2.0.1/src/gridtk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2049 2023-03-03 14:51:29.000000 gridtk-2.0.1/src/gridtk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2023-03-03 14:51:29.000000 gridtk-2.0.1/src/gridtk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 14:51:29.000000 gridtk-2.0.1/src/gridtk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      238 2023-03-03 14:51:29.000000 gridtk-2.0.1/src/gridtk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-03-03 14:51:29.000000 gridtk-2.0.1/src/gridtk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-03 14:51:29.000000 gridtk-2.0.1/src/gridtk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 14:51:28.000000 gridtk-2.0.1/src/gridtk.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.259638 gridtk-2.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-10 23:04:22.000000 gridtk-2.0.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-02-13 17:13:35.000000 gridtk-2.0.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 14:51:29.259638 gridtk-2.0.1/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-10 23:04:22.000000 gridtk-2.0.1/tests/data/test_array.sh
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-02-10 23:04:22.000000 gridtk-2.0.1/tests/data/test_script.sh
--rw-rw-rw-   0 root         (0) root         (0)    17424 2023-02-13 17:13:35.000000 gridtk-2.0.1/tests/test_local.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2023-02-13 17:13:35.000000 gridtk-2.0.1/tests/test_tools.py
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 gridtk-2.1.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/api.rst
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/catalog.json
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/conf.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/index.rst
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/install.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/links.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/nitpick-exceptions.txt
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/usage-api.rst
+-rw-r--r--   0        0        0    13076 2020-02-02 00:00:00.000000 gridtk-2.1.0/doc/usage-cli.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/__init__.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/easy.py
+-rw-r--r--   0        0        0    17414 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/local.py
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/manager.py
+-rw-r--r--   0        0        0    19115 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/models.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/setshell.py
+-rw-r--r--   0        0        0    11247 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/sge.py
+-rw-r--r--   0        0        0    10613 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/script/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/script/grid.py
+-rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 gridtk-2.1.0/src/gridtk/script/jman.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gridtk-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 gridtk-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 gridtk-2.1.0/tests/test_local.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 gridtk-2.1.0/tests/test_tools.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 gridtk-2.1.0/tests/data/test_array.sh
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 gridtk-2.1.0/tests/data/test_script.sh
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 gridtk-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 gridtk-2.1.0/README.md
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 gridtk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 gridtk-2.1.0/PKG-INFO
```

### Comparing `gridtk-2.0.1/LICENSES/GPL-3.0-or-later.txt` & `gridtk-2.1.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/PKG-INFO` & `gridtk-2.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,16 @@
-Metadata-Version: 2.1
-Name: gridtk
-Version: 2.0.1
-Summary: Grid-enabled job submitter and execution monitor for Idiap
-Author-email: Andre Anjos <andre.anjos@idiap.ch>, Manuel Guenther <manuel.guenther@idiap.ch>
-License: GNU General Public License v3 (GPLv3)
-Project-URL: documentation, https://gridtk.readthedocs.io/en/v2.0.1/
-Project-URL: homepage, https://pypi.org/project/gridtk
-Project-URL: repository, https://gitlab.idiap.ch/software/gridtk
-Project-URL: changelog, https://gitlab.idiap.ch/software/gridtk/-/releases
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: qa
-Provides-Extra: doc
-Provides-Extra: test
-
 <!--
 SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v2.0.1-orange.svg)](https://gridtk.readthedocs.io/en/v2.0.1/)
-[![build](https://gitlab.idiap.ch/software/gridtk/badges/v2.0.1/pipeline.svg)](https://gitlab.idiap.ch/software/gridtk/commits/v2.0.1)
-[![coverage](https://gitlab.idiap.ch/software/gridtk/badges/v2.0.1/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/gridtk/v2.0.1/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v2.1.0-orange.svg)](https://gridtk.readthedocs.io/en/v2.1.0/)
+[![build](https://gitlab.idiap.ch/software/gridtk/badges/v2.1.0/pipeline.svg)](https://gitlab.idiap.ch/software/gridtk/commits/v2.1.0)
+[![coverage](https://gitlab.idiap.ch/software/gridtk/badges/v2.1.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/gridtk/v2.1.0/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/gridtk)
 
 
 # Grid-enabled job submitter and execution monitor for Idiap
 
 This package provides a set of python wrappers around SGE utilities like
 `qsub`, `qstat` and `qdel`, and simplify job submission and management. It
```

### Comparing `gridtk-2.0.1/doc/conf.py` & `gridtk-2.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/doc/index.rst` & `gridtk-2.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/doc/install.rst` & `gridtk-2.1.0/doc/install.rst`

 * *Files 23% similar despite different names*

```diff
@@ -4,43 +4,71 @@
 
 .. _gridtk.install:
 
 ==============
  Installation
 ==============
 
-We support two installation modes, through pip_, or mamba_ (conda).
+Installation may follow one of two paths: deployment or development. Choose the
+relevant tab for details on each of those installation paths.
 
 
-.. tab:: pip/stable
+.. tab:: Deployment (pip/uv)
+
+   Install using pip_, or your preferred Python project management solution (e.g.
+   uv_, rye_ or poetry_).
+
+   **Stable** release, from PyPI:
 
    .. code:: sh
 
       pip install gridtk
 
-
-.. tab:: pip/beta
+   **Latest** development branch, from its git repository:
 
    .. code:: sh
 
-      pip install git+https://gitlab.idiap.ch/software/gridtk
+      pip install git+https://gitlab.idiap.ch/software/gridtk@main
 
 
-.. tab:: conda/stable
+.. tab:: Deployment (pixi)
+
+   Use pixi_ to add this package as a dependence:
 
    .. code:: sh
 
-      mamba install -c conda-forge gridtk
+      pixi add gridtk
+
 
+.. tab:: Development
 
-.. tab:: conda/beta
+   Checkout the repository, and then use pixi_ to setup a full development
+   environment:
 
    .. code:: sh
 
-      mamba install -c https://www.idiap.ch/software/biosignal/conda/label/beta -c conda-forge gridtk
+      git clone git@gitlab.idiap.ch:software/gridtk
+      pixi install --frozen
+
+   .. tip::
+
+      The ``--frozen`` flag will ensure that the latest lock-file available
+      with sources is used.  If you'd like to update the lock-file to the
+      latest set of compatible dependencies, remove that option.
+
+      If you use `direnv to setup your pixi environment
+      <https://pixi.sh/latest/features/environment/#using-pixi-with-direnv>`_
+      when you enter the directory containing this package, you can use a
+      ``.envrc`` file similar to this:
+
+      .. code:: sh
+
+         watch_file pixi.lock
+         export PIXI_FROZEN="true"
+         eval "$(pixi shell-hook)"
 
 
 .. _gridtk.config:
 
 Setup
 -----
```

### Comparing `gridtk-2.0.1/doc/usage-api.rst` & `gridtk-2.1.0/doc/usage-api.rst`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/doc/usage-cli.rst` & `gridtk-2.1.0/doc/usage-cli.rst`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/src/gridtk/easy.py` & `gridtk-2.1.0/src/gridtk/easy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
 """Common arguments to grid jobs."""
 
 import os
 import sys
 
 from . import manager, tools
```

### Comparing `gridtk-2.0.1/src/gridtk/local.py` & `gridtk-2.1.0/src/gridtk/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
-
 """Defines the job manager which can help you managing submitted grid jobs."""
 
 import copy
 import logging
 import os
 import subprocess
 import sys
```

### Comparing `gridtk-2.0.1/src/gridtk/manager.py` & `gridtk-2.1.0/src/gridtk/manager.py`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/src/gridtk/models.py` & `gridtk-2.1.0/src/gridtk/models.py`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/src/gridtk/script/grid.py` & `gridtk-2.1.0/src/gridtk/script/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
 """Executes a given command within the context of a shell script that has its
 enviroment set like Idiap's 'SETSHELL grid' does."""
 
 from __future__ import annotations
 
 import os
 import shutil
```

### Comparing `gridtk-2.0.1/src/gridtk/script/jman.py` & `gridtk-2.1.0/src/gridtk/script/jman.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
-
 """A logging Idiap/SGE job manager."""
 
 from __future__ import annotations
 
 __epilog__ = """ For a list of available commands:
   >>> %(prog)s --help
```

### Comparing `gridtk-2.0.1/src/gridtk/setshell.py` & `gridtk-2.1.0/src/gridtk/setshell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
 """Wrappers for Idiap's SETSHELL functionality."""
 
 from __future__ import annotations
 
 import logging
 import os
 import signal
```

### Comparing `gridtk-2.0.1/src/gridtk/sge.py` & `gridtk-2.1.0/src/gridtk/sge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
 """Defines the job manager which can help you managing submitted grid jobs."""
 
 from __future__ import annotations
 
 import logging
 import os
 import re
```

### Comparing `gridtk-2.0.1/src/gridtk/tools.py` & `gridtk-2.1.0/src/gridtk/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
-
 """Functions that replace shell-based utilities for grid submission and
 probing."""
 
 from __future__ import annotations
 
 import logging
 import math
@@ -228,15 +227,15 @@
         if isinstance(array, (str, bytes)):
             try:
                 i = int(array)
                 scmd.append("1-%d:1" % i)
             except ValueError:
                 # must be complete...
                 scmd.append("%s" % array)
-        if isinstance(array, (str, bytes)):
+        if isinstance(array, int):
             scmd.append("1-%d:1" % array)
         if isinstance(array, (tuple, list)):
             if len(array) < 1 or len(array) > 3:
                 raise RuntimeError(
                     "Array tuple should have length between 1 and 3"
                 )
             elif len(array) == 1:
```

### Comparing `gridtk-2.0.1/tests/test_local.py` & `gridtk-2.1.0/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `gridtk-2.0.1/tests/test_tools.py` & `gridtk-2.1.0/tests/test_tools.py`

 * *Files identical despite different names*

