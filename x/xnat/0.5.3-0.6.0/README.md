# Comparing `tmp/xnat-0.5.3.tar.gz` & `tmp/xnat-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xnat-0.5.3.tar", last modified: Mon Dec  4 14:35:43 2023, max compression
+gzip compressed data, was "dist/xnat-0.6.0.tar", last modified: Tue May 14 16:26:10 2024, max compression
```

## Comparing `xnat-0.5.3.tar` & `xnat-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 14:35:43.000000 xnat-0.5.3/
--rw-rw-rw-   0 root         (0) root         (0)    10349 2023-12-04 14:35:34.000000 xnat-0.5.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-12-04 14:35:34.000000 xnat-0.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3302 2023-12-04 14:35:43.000000 xnat-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2215 2023-12-04 14:35:34.000000 xnat-0.5.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-12-04 14:35:34.000000 xnat-0.5.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-04 14:35:43.000000 xnat-0.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3095 2023-12-04 14:35:34.000000 xnat-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat/
--rw-rw-rw-   0 root         (0) root         (0)    28720 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat/client/
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/download.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/importing.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/listings.py
--rw-rw-rw-   0 root         (0) root         (0)     5978 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/prearchive.py
--rw-rw-rw-   0 root         (0) root         (0)     6014 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/scripts.py
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/search.py
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/client/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4517 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    52636 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/convert_xsd.py
--rw-rw-rw-   0 root         (0) root         (0)    47674 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/core.py
--rw-rw-rw-   0 root         (0) root         (0)     5295 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6076 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/header.py
--rw-rw-rw-   0 root         (0) root         (0)     2567 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/inspect.py
--rw-rw-rw-   0 root         (0) root         (0)    36421 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3377 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)    18805 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/prearchive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8778 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/scripts/copy_project.py
--rw-rw-rw-   0 root         (0) root         (0)    11540 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/scripts/data_integrity_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/scripts/import_experiment_dir.py
--rw-rw-rw-   0 root         (0) root         (0)    11788 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/search.py
--rw-rw-rw-   0 root         (0) root         (0)    18520 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/services.py
--rw-rw-rw-   0 root         (0) root         (0)    51269 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/session.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/type_hints.py
--rw-rw-rw-   0 root         (0) root         (0)     2980 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/users.py
--rw-rw-rw-   0 root         (0) root         (0)     6553 2023-12-04 14:35:34.000000 xnat-0.5.3/xnat/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3302 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      860 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-12-04 14:35:43.000000 xnat-0.5.3/xnat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10349 2024-05-14 16:26:01.000000 xnat-0.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-14 16:26:01.000000 xnat-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-05-14 16:26:10.000000 xnat-0.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2024-05-14 16:26:01.000000 xnat-0.6.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-14 16:26:01.000000 xnat-0.6.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 16:26:10.000000 xnat-0.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3074 2024-05-14 16:26:01.000000 xnat-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/
+-rw-rw-rw-   0 root         (0) root         (0)    29831 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/importing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/listings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5253 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/prearchive.py
+-rw-rw-rw-   0 root         (0) root         (0)     5282 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5312 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/scripts.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/cli/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     4517 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    52743 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/convert_xsd.py
+-rw-rw-rw-   0 root         (0) root         (0)    47814 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     5295 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6066 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2567 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/map.py
+-rw-rw-rw-   0 root         (0) root         (0)    42165 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3365 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)    18865 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/prearchive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9501 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/copy_project.py
+-rw-rw-rw-   0 root         (0) root         (0)    11540 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/data_integrity_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/delete_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/scripts/import_experiment_dir.py
+-rw-rw-rw-   0 root         (0) root         (0)    11788 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/search.py
+-rw-rw-rw-   0 root         (0) root         (0)    18611 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/services.py
+-rw-rw-rw-   0 root         (0) root         (0)    51455 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/type_hints.py
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     6559 2024-05-14 16:26:01.000000 xnat-0.6.0/xnat/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3302 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      155 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-14 16:26:10.000000 xnat-0.6.0/xnat.egg-info/top_level.txt
```

### Comparing `xnat-0.5.3/LICENSE` & `xnat-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/PKG-INFO` & `xnat-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnat
-Version: 0.5.3
+Version: 0.6.0
 Summary: An XNAT client that exposes the XNAT REST interface as python objects. Part of the interface is automatically generated based on the servers data model as defined by the xnat schema.
 Home-page: https://gitlab.com/radiology/infrastructure/xnatpy
 Author: H.C. Achterberg
 Author-email: hakim.achterberg@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `xnat-0.5.3/README.rst` & `xnat-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/setup.py` & `xnat-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 import os
 from setuptools import setup
 
 # Get information about the version (polling mercurial if possible)
-version = '0.5.3'
+version = '0.6.0'
 
 # When building something else than a release (tag) append the job id to the version.
 if os.environ.get('CI_COMMIT_TAG'):
     pass
 elif os.environ.get('CI_JOB_ID'):
     version += ".{}".format(os.environ['CI_JOB_ID'])
 
@@ -37,24 +37,24 @@
         f_version.write('version = "{}"\n'.format(version))
 
     # Set the entry point
     entry_points = {
         "console_scripts": [
             "xnat_cp_project = xnat.scripts.copy_project:main",
             "xnat_data_integrity-check = xnat.scripts.data_integrity_check:main" ,
-            "xnat = xnat.client:cli",
+            "xnat = xnat.cli:cli",
         ]
     }
 
     setup(
         name='xnat',
         version=version,
         author='H.C. Achterberg',
         author_email='hakim.achterberg@gmail.com',
-        packages=[str('xnat'), str('xnat.scripts'), str('xnat.client')],
+        packages=['xnat', 'xnat.scripts', 'xnat.cli'],
         url='https://gitlab.com/radiology/infrastructure/xnatpy',
         license='Apache 2.0',
         description='An XNAT client that exposes the XNAT REST interface as python objects. Part of the interface is automatically generated based on the servers data model as defined by the xnat schema.',
         long_description=open('README.rst').read(),
         install_requires=_requires,
         entry_points=entry_points,
         classifiers=[
```

### Comparing `xnat-0.5.3/xnat/__init__.py` & `xnat-0.6.0/xnat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,40 +18,53 @@
 function actually in the package. All following classes are created based on
 the https://central.xnat.org/schema/xnat/xnat.xsd schema and the xnatcore and
 xnatbase modules, using the convert_xsd.
 """
 
 import getpass
 import hashlib
+import importlib.abc
 import importlib.machinery
 import importlib.util
 import logging
 import os
 from pathlib import Path
 import platform
 import netrc
 import re
-import tempfile
+from io import StringIO
 import time
 
 import requests
 import requests.cookies
 import urllib3
 from urllib import parse
 
 from . import exceptions, search
 from .session import XNATSession, BaseXNATSession
 from .constants import DEFAULT_SCHEMAS
 from .convert_xsd import SchemaParser
+from .map import MappingLevel
 from .utils import JSessionAuth
+from .mixin import FilterFunctions
 
 GEN_MODULES = {}
 
-__version__ = '0.5.3'
-__all__ = ['connect', 'exceptions']
+__version__ = '0.6.0'
+__all__ = ['connect', 'exceptions', 'MappingLevel', 'FilterFunctions']
+
+class StringLoader(importlib.abc.SourceLoader):
+    def __init__(self, data):
+        self.data = data
+
+    def get_data(self, pathname):
+        return self.data.encode('utf-8')
+    
+    def get_filename(self, fullname: str) -> str:
+        return f"<in_memory:{fullname}>"
 
 
 def check_auth_guest(requests_session, server, logger):
     """
     Try to figure out of the requests session is properly logged in as the desired user
 
     :param requests.Session requests_session: requests session
@@ -347,18 +360,19 @@
 
 
 def _wipe_jsession(requests_session, server):
     requests_session.delete(server.rstrip('/') + '/data/JSESSION', timeout=10)
     requests_session.close()
 
 
-def build_model(xnat_session, extension_types, connection_id):
+def build_parser(xnat_session, extension_types):
     """
-    Build the XNAT data model for a given connection
+    Build the XNAT parser
     """
+
     logger = xnat_session.logger
     debug = xnat_session.debug
 
     # Check XNAT version
     logger.info('Determining XNAT version')
     version = xnat_session.xnat_version
 
@@ -382,27 +396,37 @@
     else:
         logger.warning('Found an unsupported version ({}), trying 1.7 compatible model builder'.format(version))
         build_function = parse_schemas_17
 
     logger.info('Start parsing schemas and building object model')
     build_function(parser, xnat_session, extension_types=extension_types)
 
-    # Write code to temp file
-    with tempfile.NamedTemporaryFile(mode='w', suffix='_generated_xnat.py', delete=False) as code_file:
-        parser.write(code_file=code_file)
+    return parser, xnat_session
+
 
-    logger.debug('Code file written to: {}'.format(code_file.name))
+def build_model(xnat_session, extension_types, connection_id):
+    """
+    Build the XNAT data model for a given connection
+    """
+
+    logger = xnat_session.logger
+
+    parser, xnat_session = build_parser(xnat_session, extension_types=extension_types)
+
+    # Write code to temp file
+    code_stringio = StringIO()
+    parser.write(code_file=code_stringio)
 
-    # The module is loaded in its private namespace based on the code_file name
+    # The module is loaded in its private namespace based on the connection_id
+    source_code = code_stringio.getvalue()
     module_name = 'xnat.generated.model_{}'.format(connection_id)
-    loader = importlib.machinery.SourceFileLoader(module_name, code_file.name)
+    loader = StringLoader(source_code)
     spec = importlib.util.spec_from_loader(module_name, loader)
     xnat_module = importlib.util.module_from_spec(spec)
     loader.exec_module(xnat_module)
-    xnat_module._SOURCE_CODE_FILE = code_file.name
 
     logger.debug('Loaded generated module')
 
     # Register all types parsed
     for key, cls in parser.class_list.items():
         if not (cls.name is None or (cls.base_class is not None and cls.base_class.startswith('xs:'))):
             cls_obj = getattr(xnat_module, cls.writer.python_name, None)
@@ -412,32 +436,35 @@
                 logger.warning("Cannot find class to register for {}".format(cls.name))
 
     xnat_module.SESSION = xnat_session
 
     # Add the required information from the module into the xnat_session object
     xnat_session.XNAT_CLASS_LOOKUP.update(xnat_module.XNAT_CLASS_LOOKUP)
     xnat_session.classes = xnat_module
-    xnat_session._source_code_file = code_file.name
+    xnat_session.source_code = source_code
     search.inject_search_fields(xnat_session)
     logger.info('Object model created successfully')
 
 
 def connect(server=None, user=None, password=None, verify=True, netrc_file=None, debug=False,
             extension_types=True, loglevel=None, logger=None, detect_redirect=True,
             no_parse_model=False, default_timeout=300, auth_provider=None, jsession=None,
             cli=False):
     """
     Connect to a server and generate the correct classed based on the servers xnat.xsd
     This function returns an object that can be used as a context operator. It will call
     disconnect automatically when the context is left. If it is used as a function, then
     the user should call ``.disconnect()`` to destroy the session and temporary code file.
 
-    :param str server: uri of the server to connect to (including http:// or https://)
-    :param str user: username to use, leave empty to use netrc entry or anonymous login.
-    :param str password: password to use with the username, leave empty when using netrc.
+    :param str server: uri of the server to connect to (including http:// or https://),
+                       leave empty to use the `XNATPY_HOST` or `XNAT_HOST` environment variables
+    :param str user: username to use, leave empty to use the `XNATPY_USER` or `XNAT_USER`
+                     environment variables, netrc entry or anonymous login (in that order).
+    :param str password: password to use with the username, leave empty when using netrc or the
+                         `XNATPY_PASS` or `XNAT_PASS` environment variables.
                          If a username is given and no password, there will be a prompt
                          on the console requesting the password.
     :param bool verify: verify the https certificates, if this is false the connection will
                         be encrypted with ssl, but the certificates are not checked. This is
                         potentially dangerous, but required for self-signed certificates.
     :param str netrc_file: alternative location to use for the netrc file (path pointing to
                            a file following the netrc syntax)
@@ -476,29 +503,14 @@
         >>> connection = xnat.connect('https://central.xnat.org')
         >>> subjects = connection.projects['Sample_DICOM'].subjects
         >>> print('Subjects in the SampleDICOM project: {}'.format(subjects))
         Subjects in the SampleDICOM project: <XNATListing (CENTRAL_S01894, dcmtest1): <SubjectData CENTRAL_S01894>, (CENTRAL_S00461, PACE_HF_SUPINE): <SubjectData CENTRAL_S00461>>
         >>> connection.disconnect()
     """
 
-    # Auto-detect server based on environment variables
-    if server is None:
-        # Try and detect if we are on a jupyter hub instance
-        server = os.environ.get('XNAT_HOST')
-        if server:
-            user = os.environ.get('XNAT_USER')
-            password = os.environ.get('XNAT_PASS')
-
-    if server is None:
-        server = os.environ.get('XNATPY_HOST')
-
-    if server is None:
-        raise exceptions.XNATValueError('Cannot auto-detect which server to use, make sure either the XNAT_HOST'
-                                        ' or XNATPY_HOST environment variable is set!')
-
     # Generate a hash for the connection
     hasher = hashlib.md5()
     hasher.update(server.encode('utf-8'))
     hasher.update(str(time.time()).encode('utf-8'))
     connection_id = hasher.hexdigest()
 
     # Setup the logger for this connection
@@ -550,14 +562,31 @@
 
     if not verify:
         requests_session.verify = False
 
     # Start out with any accidental auth, fill token once retrieved
     requests_session.auth = JSessionAuth()
 
+    # Auto-detect server based on environment variables
+    if not server:
+        if not (server := os.environ.get("XNATPY_HOST")):
+            if not (server := os.environ.get("XNAT_HOST")):
+                raise RuntimeError("No server specified: no argument nor environment variable found")
+    if not user:
+        if not (user := os.environ.get("XNATPY_USER")):
+            if not (user := os.environ.get("XNAT_USER")):
+                logger.info("No username set, using anonymous/netrc login")
+    if not password:
+        if not (password := os.environ.get("XNATPY_PASS")):
+            if not (password := os.environ.get("XNAT_PASS")):
+                logger.info("No password set, using anonymous/netrc login")
+    if server is None:
+        raise exceptions.XNATValueError('Cannot auto-detect which server to use, make sure either the XNAT_HOST'
+                                        ' or XNATPY_HOST environment variable is set!')
+
     # Remove port and add .local to the domain in case there is no . in host
     # See issue #5388 in psf/requests for more info 
     domain = parse.urlparse(server).netloc
     if ":" in domain:
         domain = domain.split(":")[0]
     if "." not in domain:
         domain = "{domain}.local".format(domain=domain)
@@ -569,14 +598,15 @@
             value=jsession,
         )
         requests_session.cookies.set_cookie(cookie)
     else:
         if password is None:
             queried_user, queried_password = query_netrc(server, netrc_file, logger)
             if user is None or queried_user == user:
+                user = queried_user
                 password = queried_password
             elif queried_user is not None:
                 logger.warning(f'Query result from .netrc is user {queried_user} but specified user was {user}')
 
         if user is not None and password is None:
             password = getpass.getpass(prompt=str("Please enter the password for user '{}':".format(user)))
```

### Comparing `xnat-0.5.3/xnat/client/importing.py` & `xnat-0.6.0/xnat/cli/importing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 import click
-import xnat
 
 from xnat import exceptions
-from .utils import unpack_context
+from .helpers import xnatpy_all_options, connect_cli
+
 
 @click.group(name="import")
-@click.pass_context
-def importing(ctx):
+def importing():
     """
     Commands to import data from your machine into XNAT
     """
 
 
-
 @importing.command()
 @click.argument('folder')
 @click.option('--destination', help="The destination to upload the scan to.")
 @click.option('--project', help="The project in the archive to assign the session to (only accepts project ID, not a label).")
 @click.option('--subject', help="The subject in the archive to assign the session to.")
 @click.option('--experiment', help="The experiment in the archive to assign the session content to.")
 @click.option('--import_handler')
 @click.option('--quarantine', is_flag=True, help="Flag to indicate session should be quarantined.")
 @click.option('--trigger_pipelines', is_flag=True, help="Indicate that importing should trigger pipelines.")
-@click.pass_context
-def experiment(ctx,
-               folder,
+@xnatpy_all_options
+def experiment(folder,
                destination,
                project,
                subject,
                experiment,
                import_handler,
                quarantine,
-               trigger_pipelines):
+               trigger_pipelines,
+               **kwargs):
     """Import experiment from the target folder to XNAT"""
     try:
-        ctx = unpack_context(ctx)
-        with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, no_parse_model=True, loglevel=ctx.loglevel) as session:
+        with connect_cli(no_parse_model=True, **kwargs) as session:
             session.services.import_dir(folder, quarantine=quarantine, destination=destination,
                                           trigger_pipelines=trigger_pipelines, project=project, subject=subject,
                                           experiment=experiment, import_handler=import_handler)
             session.logger.info("Import complete!")
     except exceptions.XNATLoginFailedError:
         print(f"ERROR Failed to login")
```

### Comparing `xnat-0.5.3/xnat/client/listings.py` & `xnat-0.6.0/xnat/cli/listings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,65 @@
 import click
-import xnat
 
-from .utils import unpack_context
+from .helpers import connect_cli, xnatpy_all_options
 
 
 @click.group(name="list")
-@click.pass_context
-def listings(ctx):
+def listings():
     """
     Commands to list different XNAT objects either in machine- or human-readable formats.
     """
     pass
 
 
 @listings.command()
 @click.option('--filter', help="Filter criteria to select projects.")
 @click.option('--header/--no-header', default=True, help="Include header in the listing or not.")
 @click.option('--column', multiple=True, help="Columns to include in the listing.")
-@click.pass_context
-def projects(ctx, column, filter, header):
+@xnatpy_all_options
+def projects(column, filter, header, output_format, **kwargs):
     """List projects in the target XNAT."""
-    ctx = unpack_context(ctx)
-
     if not column:
         column = None
 
     if filter:
         filter = filter.split('=')
         filter = {filter[0]: filter[1]}
 
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, loglevel=ctx.loglevel) as session:
-        if ctx.output_format == 'csv':
+    with connect_cli(**kwargs) as session:
+        if output_format == 'csv':
             result = session.projects.tabulate_csv(columns=column, filter=filter, header=header)
             click.echo(result.strip())
         else:
             click.echo("List of accessible projects")
             click.echo("====================================================")
             for proj in session.projects.filter(filters=filter).values():
                 click.echo(proj.cli_str())
 
 
 @listings.command()
 @click.option('--project', help="Project id to list subjects from.")
 @click.option('--filter', help="Filter criteria to select subjects.")
 @click.option('--header/--no-header', default=True, help="Include header in the listing or not.")
 @click.option('--column', multiple=True, help="Columns to include in the listing.")
-@click.pass_context
-def subjects(ctx, project, column, filter, header):
+@xnatpy_all_options
+def subjects(project, column, filter, header, output_format, **kwargs):
     """List subjects in the target XNAT."""
-    ctx = unpack_context(ctx)
-    
     if not column:
         column = None
 
     if filter:
         filter = filter.split('=')
         filter = {filter[0]: filter[1]}
 
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, loglevel=ctx.loglevel) as session:
-        
+    with connect_cli(**kwargs) as session:
         if project is not None:
             subjects = session.subjects.filter(project=projects)
         else:
             subjects = session.subjects
 
-        if ctx.output_format == 'csv':
+        if output_format == 'csv':
             result = subjects.tabulate_csv(columns=column, filter=filter, header=header)
             click.echo(result.strip())
         else:
             for subj in subjects.filter(filters=filter).values():
                 click.echo(subj.cli_str())
```

### Comparing `xnat-0.5.3/xnat/client/prearchive.py` & `xnat-0.6.0/xnat/cli/prearchive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 import click
-import xnat
 
-from .utils import unpack_context
+from .helpers import xnatpy_all_options, connect_cli
+
 
 @click.group(name="prearchive")
-@click.pass_context
-def prearchive(ctx):
+def prearchive():
     """
     Commands for prearchive management.
     """
 
 
 @prearchive.command()
-@click.pass_context
-def list(ctx):
+@xnatpy_all_options
+def list(**kwargs):
     """
     List all sessions currently in prearchive.
     """
-    ctx = unpack_context(ctx)
-
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, no_parse_model=True, loglevel=ctx.loglevel) as session:
+    with connect_cli(no_parse_model=True, **kwargs) as session:
         for sess in session.prearchive.sessions():
             click.echo(sess.cli_str())
 
 
 @prearchive.command()
 @click.option('--project', '-p', help="Project the session belongs to.")
 @click.option('--label', '-l', help="Session label.")
 @click.option('--subject', '-s', help="Session subject.")
 @click.option('--status', help="Session status.")
-@click.pass_context
-def delete(ctx, project, label, subject, status):
+@xnatpy_all_options
+def delete(project, label, subject, status, **kwargs):
     """Delete selected prearchive sessions."""
-    ctx = unpack_context(ctx)
-
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, loglevel=ctx.loglevel) as session:
+    with connect_cli(**kwargs) as session:
         selected_sessions = session.prearchive.find(project=project, subject=subject, label=label, status=status)
         if not selected_sessions:
             session.logger.warning("No prearchive sessions have been selected based on your criteria!")
         else:
             for sess in selected_sessions:
                 session.logger.debug("Deleting session {}".format(session.label))
                 sess.delete()
@@ -48,21 +41,18 @@
 
 @prearchive.command()
 @click.option('--project', '-p', help="Project the sessions currently belong to.")
 @click.option('--dest-project', help="Destination project.")
 @click.option('--label', '-l', "Session label.")
 @click.option('--subject', '-s', "Session subject.")
 @click.option('--status', "Session status.")
-@click.pass_context
-def move(ctx, project, dest_project, label, subject, status):
+@xnatpy_all_options
+def move(project, dest_project, label, subject, status, **kwargs):
     """Move selected prearchive sessions."""
-    ctx = unpack_context(ctx)
-
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, loglevel=ctx.loglevel) as session:
+    with connect_cli(**kwargs) as session:
         selected_sessions = session.prearchive.find(project=project, subject=subject, label=label, status=status)
         if not selected_sessions:
             session.logger.warning("No prearchive sessions have been selected based on your criteria!")
         else:
             for sess in selected_sessions:
                 session.logger.debug("Moving session {}".format(session.label))
                 sess.move(dest_project)
@@ -72,21 +62,18 @@
 @click.argument('--sessionid')
 @click.argument('--project')
 @click.option('--subject', help="The subject in the archive to assign the content to.")
 @click.option('--experiment', help="The experiment in the archive to assign the session content to.")
 @click.option('--overwrite', help="Action to take in case data already exists. Possible values: none, append, delete.")
 @click.option('--quarantine', is_flag=True, help="Indicate whether the session should be quarantined.")
 @click.option('--trigger-pipelines', is_flag=True, help="Indicate whether archiving should trigger pipelines.")
-@click.pass_context
-def archive(ctx, sessionid, project, subject, experiment, overwrite, quarantine, trigger_pipelines):
+@xnatpy_all_options
+def archive(sessionid, project, subject, experiment, overwrite, quarantine, trigger_pipelines, **kwargs):
     """Archive selected prearchive session."""
-    ctx = unpack_context(ctx)
-
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, loglevel=ctx.loglevel) as session:
+    with connect_cli(**kwargs) as session:
         selected_session = None
         for sess in session.prearchive.sessions:
             if sess.id == sessionid:
                 selected_session = sess
                 break
         
         if not selected_session:
@@ -101,21 +88,18 @@
 @click.option('--project', '-p', help="Project the session belongs to.")
 @click.option('--label', '-l', help="Session label.")
 @click.option('--subject', '-s', help="Session subject.")
 @click.option('--status', help="Session status.")
 @click.option('--overwrite', help="Action to take in case data already exists. Possible values: none, append, delete.")
 @click.option('--quarantine', is_flag=True, help="Indicate whether the session should be quarantined.")
 @click.option('--trigger-pipelines', is_flag=True, help="Indicate whether archiving should trigger pipelines.")
-@click.pass_context
-def bulk_archive(ctx, project, label, subject, status, overwrite, quarantine, trigger_pipelines):
+@xnatpy_all_options
+def bulk_archive(project, label, subject, status, overwrite, quarantine, trigger_pipelines, **kwargs):
     """Archive multiple selected prearchive sessions."""
-    ctx = unpack_context(ctx)
-
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, loglevel=ctx.loglevel) as session:
+    with connect_cli(**kwargs) as session:
         selected_sessions = session.prearchive.find(project=project, subject=subject, label=label, status=status)
         if not selected_sessions:
             session.logger.warning("No prearchive sessions have been selected based on your criteria!")
         else:
             for sess in selected_sessions:
                 session.logger.debug("Archiving session {}".format(session.label))
                 sess.archive(overwrite=overwrite, quarantine=quarantine, trigger_pipelines = trigger_pipelines)
```

### Comparing `xnat-0.5.3/xnat/client/rest.py` & `xnat-0.6.0/xnat/cli/rest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,132 @@
 import click
-import xnat
 
-from .utils import unpack_context
+from .helpers import connect_cli, xnatpy_login_options
+
 
 @click.group(name="rest")
-@click.pass_context
-def rest(ctx):
+def rest():
     """
     Perform various REST requests to the target XNAT.
     """
 
 @rest.command()
 @click.argument('path')
 @click.option('--query', multiple=True, help="The values to be added to the query string in the URI.")
 @click.option('--headers', multiple=True, help="HTTP headers to include.")
-@click.pass_context
-def get(ctx, path, query, headers):
+@xnatpy_login_options
+def get(path, query, headers, **kwargs):
     """Perform GET request to the target XNAT."""
-    ctx = unpack_context(ctx)
-    
     if query:
-        query = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), query)}
+        query = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), query)}
 
     if headers:
-        headers = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), headers)}
-    
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, no_parse_model=True, loglevel=ctx.loglevel) as session:
-        result = session.get(path, query=query, timeout=ctx.timeout)
+        headers = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), headers)}
+
+    with connect_cli(no_parse_model=True, **kwargs) as session:
+        result = session.get(path, query=query, headers=headers, timeout=kwargs.get("timeout"))
         click.echo('Result: {text}'.format(text=result.text))
-        click.echo('Path {path} {user}'.format(path=path, user=ctx.user))
+        click.echo('Path {path} {user}'.format(path=path, user=kwargs.get("user")))
 
 
 @rest.command()
 @click.argument('path')
 @click.option('--query', multiple=True, help="The values to be added to the query string in the URI.")
 @click.option('--headers', multiple=True, help="HTTP headers to include.")
-@click.pass_context
-def head(ctx, path, query, headers):
+@xnatpy_login_options
+def head(path, query, headers, **kwargs):
     """Perform HEAD request to the target XNAT."""
-    ctx = unpack_context(ctx)
-
     if query:
-        query = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), query)}
+        query = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), query)}
 
     if headers:
-        headers = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), headers)}
-    
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, no_parse_model=True, loglevel=ctx.loglevel) as session:
-        result = session.head(path, timeout=ctx.timeout, query=query, headers=headers)
+        headers = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), headers)}
+
+    with connect_cli(no_parse_model=True, **kwargs) as session:
+        result = session.head(path, query=query, headers=headers)
         click.echo('Result: {text}'.format(text=result.text))
-        click.echo('Path {path} {user}'.format(path=path, user=ctx.user))
+        click.echo('Path {path} {user}'.format(path=path, user=kwargs.get('user')))
 
 
 @rest.command()
 @click.argument('path')
 @click.option('--jsonpath', '-j', help="JSON payload file location.")
 @click.option('--datapath', '-d', help="Data payload file location.")
 @click.option('--query', multiple=True, help="The values to be added to the query string in the URI.")
 @click.option('--headers', multiple=True, help="HTTP headers to include.")
-@click.pass_context
-def post(ctx, path, jsonpath, datapath, query, headers):
+@xnatpy_login_options
+def post(path, jsonpath, datapath, query, headers, **kwargs):
     """Perform POST request to the target XNAT."""
-    ctx = unpack_context(ctx)
-    
     if jsonpath is not None:
         with open(jsonpath, 'r') as json_file:
             json_payload = json_file.read()
     else:
         json_payload = None
     
     if datapath is not None:
         with open(datapath, 'r') as data_file:
             data_payload = data_file.read()
     else:
         data_payload = None
 
     if query:
-        query = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), query)}
+        query = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), query)}
     
     if headers:
-        headers = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), headers)}
+        headers = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), headers)}
 
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, no_parse_model=True, loglevel=ctx.loglevel) as session:
-        result = session.post(path, json=json_payload, data=data_payload, query=query, timeout=ctx.timeout, headers=headers)
+    with connect_cli(no_parse_model=True, **kwargs) as session:
+        result = session.post(path, json=json_payload, data=data_payload, query=query, headers=headers)
         click.echo('Result: {text}'.format(text=result.text))
-        click.echo('Path {path} {user}'.format(path=path, user=ctx.user))
+        click.echo('Path {path} {user}'.format(path=path, user=kwargs.get('user')))
 
 
 @rest.command()
 @click.argument('path')
 @click.option('--jsonpath', '-j', help="JSON payload file location.")
 @click.option('--datapath', '-d', help="Data payload file location.")
 @click.option('--query', multiple=True, help="The values to be added to the query string in the URI.")
 @click.option('--headers', multiple=True, help="HTTP headers to include.")
-@click.pass_context
-def put(ctx, path, jsonpath, datapath, query, headers):
+@xnatpy_login_options
+def put(path, jsonpath, datapath, query, headers, **kwargs):
     """Perform PUT request to the target XNAT."""
-    ctx = unpack_context(ctx)
-    
     if jsonpath is not None:
         with open(jsonpath, 'r') as json_file:
             json_payload = json_file.read()
     else:
         json_payload = None
     
     if datapath is not None:
         with open(datapath, 'r') as data_file:
             data_payload = data_file.read()
     else:
         data_payload = None
     
     if query:
-        query = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), query)}
+        query = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), query)}
 
     if headers:
-        headers = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), headers)} 
+        headers = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), headers)}
 
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, no_parse_model=True, loglevel=ctx.loglevel) as session:
-        result = session.put(path, json=json_payload, data=data_payload, query=query, timeout=ctx.timeout, headers=headers)
+    with connect_cli(no_parse_model=True, **kwargs) as session:
+        result = session.put(path, json=json_payload, data=data_payload, query=query, headers=headers)
         click.echo('Result: {text}'.format(text=result.text))
-        click.echo('Path {path} {user}'.format(path=path, user=ctx.user))
+        click.echo('Path {path} {user}'.format(path=path, user=kwargs.get('user')))
 
 
 @rest.command()
 @click.argument('path')
 @click.option('--query', multiple=True, help="The values to be added to the query string in the URI.")
 @click.option('--headers', multiple=True, help="HTTP headers to include.")
-@click.pass_context
-def delete(ctx, path, query, headers):
+@xnatpy_login_options
+def delete(path, query, headers, **kwargs):
     """Perform DELETE request to the target XNAT."""
-    ctx = unpack_context(ctx)
-
     if query:
-        query = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), query)}
+        query = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), query)}
 
     if headers:
-        headers = {arg[0]:arg[1] for arg in map(lambda x: x.split("="), headers)} 
+        headers = {arg[0]: arg[1] for arg in map(lambda x: x.split("="), headers)}
 
-    with xnat.connect(ctx.host, user=ctx.user, netrc_file=ctx.netrc, jsession=ctx.jsession,
-                      cli=True, no_parse_model=True, loglevel=ctx.loglevel) as session:
-        result = session.delete(path, timeout=ctx.timeout, query=query, headers=headers)
+    with connect_cli(no_parse_model=True, **kwargs) as session:
+        result = session.delete(path, query=query, headers=headers)
         click.echo('Result: {text}'.format(text=result.text))
-        click.echo('Path {path} {user}'.format(path=path, user=ctx.user))
+        click.echo('Path {path} {user}'.format(path=path, user=kwargs.get('user')))
```

### Comparing `xnat-0.5.3/xnat/constants.py` & `xnat-0.6.0/xnat/constants.py`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/xnat/convert_xsd.py` & `xnat-0.6.0/xnat/convert_xsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 
 from __future__ import absolute_import
 from __future__ import print_function
 from __future__ import unicode_literals
 from abc import ABCMeta, abstractmethod, abstractproperty
 import collections
 import contextlib
-import inspect
-import keyword
 import os
 import re
+from string import Template
 from xml.etree import ElementTree
 
 from . import core
 from . import mixin
 from .datatypes import TYPE_TO_PYTHON
 from .constants import SECONDARY_LOOKUP_FIELDS, FIELD_HINTS, CORE_REST_OBJECTS
 from .utils import pythonize_class_name, pythonize_attribute_name, full_class_name
@@ -348,15 +347,15 @@
         data = prop.tostring()
         return data
 
     def header(self):
         base_mixin = self.get_base_template()
         if base_mixin is not None:
             header = '# Base mixin for {}: {}\n'.format(self.python_name, base_mixin)
-            header += "class {name}({base}, mixin.{mixin}):\n".format(name=self.python_name,
+            header += "class {name}(mixin.{mixin}, {base}):\n".format(name=self.python_name,
                                                                 base=self.python_base_class,
                                                                 mixin=base_mixin.__name__)
             header += '\n\n    # END HEADER\n'
         else:
             header = '# No base template found for {}\n'.format(self.python_name)
             header += "class {name}({base}):\n".format(name=self.python_name, base=self.python_base_class)
             header += '\n\n    # END HEADER\n'
@@ -396,15 +395,16 @@
             header += ("    @property\n"
                        "    def __display_identifier(self):\n"
                        "        return self.{}\n\n".format(self.display_identifier))
 
         return header
 
     # Abstract stuff that needs to be reimplemented by subclasses
-    @abstractproperty
+    @property
+    @abstractmethod
     def default_base_class(self):
         """
         The default base class if none is supplied
         """
 
 
 class SimpleClassWriter(BaseClassWriter):
@@ -1336,11 +1336,13 @@
         after = set(self.class_list.keys())
         if self.debug:
             self.logger.debug('Classes after prune: {}'.format(after))
             self.logger.info('Classes removed by pruning: {}'.format(sorted(before - after)))
 
         self.logger.info('Writing result')
         schemas = '\n'.join('# - {}'.format(s) for s in self.schemas)
-        code_file.write(FILE_HEADER.format(schemas=schemas,
-                                           file_secondary_lookup=SECONDARY_LOOKUP_FIELDS['xnat:fileData']))
+        string_template = Template(FILE_HEADER)
+        code_str = string_template.safe_substitute(SCHEMAS=schemas,
+                                                   FILE_SECONDARY_LOOKUP=SECONDARY_LOOKUP_FIELDS['xnat:fileData'])
+        code_file.write(code_str)
 
         code_file.write('\n\n\n'.join(c.tostring().strip() for c in self if c.name is not None))
```

### Comparing `xnat-0.5.3/xnat/core.py` & `xnat-0.6.0/xnat/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,19 @@
 class XNATObject(XNATBaseObject):
     @property
     @caching
     def fulldata(self) -> JSONType:
         data = self.xnat_session.get_json(self.uri)['items']
 
         # Determine original insert data (oldest entry)
-        insert_date = min(parse_datetime(x['meta']['start_date']) for x in data)
+        insert_date = [parse_datetime(x['meta']['start_date']) for x in data if x['meta'].get('start_date')]
+        if insert_date:
+            insert_date = min(insert_date)
+        else:
+            insert_date = None
 
         # Collect data and insert extra field
         data = next(x for x in data if not x['meta']['isHistory'])
         data['xnatpy'] = {
             'insert_date': insert_date
         }
         return data
```

### Comparing `xnat-0.5.3/xnat/datatypes.py` & `xnat-0.6.0/xnat/datatypes.py`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/xnat/exceptions.py` & `xnat-0.6.0/xnat/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -92,8 +92,13 @@
     The object manipulated is deleted and therefore destroyed. It should not be used anymore!
     """
 
 
 class XNATObjectAlreadyExistsError(XNATError):
     """
     The object being created already exists.
+    """
+
+class XNATMappingException(BaseException):
+    """
+    Exception occured while mapping a sub-object
     """
```

### Comparing `xnat-0.5.3/xnat/header.py` & `xnat-0.6.0/xnat/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 class XNATSubObjectMixin(XNATSubObject):
     @mixedproperty
     def xnat_session(self):
         return current_session()
 
 
 class FileData(XNATObjectMixin):
-    SECONDARY_LOOKUP_FIELD = "{file_secondary_lookup}"
+    SECONDARY_LOOKUP_FIELD = "$FILE_SECONDARY_LOOKUP"
     _XSI_TYPE = 'xnat:fileData'
 
     def __init__(self, uri=None, xnat_session=None, id_=None, datafields=None, parent=None, fieldname=None, overwrites=None, name=None):
         super(FileData, self).__init__(uri=uri,
                                        xnat_session=xnat_session,
                                        id_=id_,
                                        datafields=datafields,
@@ -184,27 +184,27 @@
     @property
     def data_path(self):
         parent = self.xnat_session.create_object(self.uri.split('/files/')[0])
 
         if parent.data_dir is None:
             return None
 
-        data_path = f"{{parent.data_dir}}/{{self.path}}"
+        data_path = f"{parent.data_dir}/{self.path}"
 
         if not os.path.exists(data_path):
-            self.logger.info(f'Determined data_path to be {{data_path}}, but it does not exist!')
+            self.logger.info(f'Determined data_path to be {data_path}, but it does not exist!')
             return None
 
         return data_path
 
 
 # Empty class lookup to place all new lookup values
-XNAT_CLASS_LOOKUP = {{
+XNAT_CLASS_LOOKUP = {
     "xnat:fileData": FileData,
-}}
+}
 
 
 # The following code represents the data structure of the XNAT server
 # It is automatically generated using
-# {schemas}
+# $SCHEMAS
```

### Comparing `xnat-0.5.3/xnat/inspect.py` & `xnat-0.6.0/xnat/inspect.py`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/xnat/mixin.py` & `xnat-0.6.0/xnat/mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from __future__ import annotations
+
 import os
+import sys
 from pathlib import Path
 import tempfile
 from zipfile import ZipFile
 import tarfile
 import shutil
-from typing import Optional, Union, IO
+from typing import Optional, Union, IO, Callable
+from .type_hints import JSONType
+from dataclasses import dataclass
 
 from io import BytesIO
 
 from .core import caching, XNATBaseObject, XNATListing
+from .map import MappingObjectStates, MappingLevel, check_result_type
 from .search import SearchField
 from .users import Users
 from .utils import mixedproperty, pythonize_attribute_name
 from . import exceptions
 
 try:
     PYDICOM_LOADED = True
@@ -111,15 +117,15 @@
                            secondary_lookup_field='label',
                            xsi_type='xnat:resourceCatalog')
 
     def create_resource(self, label, format=None, data_dir=None, method=None) -> 'AbstractResource':
         uri = f'{self.fulluri}/resources/{label}'
         self.xnat_session.put(uri, format=format)
         self.clearcache()  # The resources changed, so we have to clear the cache
-        resource = self.xnat_session.create_object(uri, type_='xnat:resourceCatalog')
+        resource = self.xnat_session.create_object(uri)
 
         if data_dir is not None:
             resource.upload_dir(data_dir, method=method)
 
         return resource
 
     def download_dir(self, target_dir, verbose=True, progress_callback=None):
@@ -163,14 +169,89 @@
 
         if not os.path.isdir(data_dir):
             self.logger.info(f'Determined data_dir to be {data_dir}, but it does not exist!')
             return None
 
         return data_dir
 
+    def mapping_iter(self, states: MappingObjectStates, level: MappingLevel, filter_function):
+        self.logger.debug(f'Start Iterating for project {self.name}')
+        with states.descend(self, MappingLevel.PROJECT):
+            for xnat_subject in self.subjects.values():
+                if states.succeeded(xnat_subject):
+                    continue
+                if filter_function and not filter_function.subject(xnat_subject):
+                    continue
+                if level == MappingLevel.SUBJECT:
+                    yield xnat_subject
+                else:
+                    yield from xnat_subject.mapping_iter(states, level, filter_function)
+        self.logger.debug(f'Finished Iterating for project {self.name}')
+
+    def map(self,
+            function: Callable[[XNATBaseObject, ...], JSONType],
+            level: Union[MappingLevel, str],
+            args: Optional[list] = None,
+            kwargs: Optional[dict] = None,
+            filter_function: "FilterFunctions" = None,
+            logfile: Union[str, Path, None] = None) -> dict[str, JSONType]:
+        """
+        Map a given function over all items of a certain level in a project. Function should take the XNAT object of the
+        level specified as the first argument and can take additional args and kwargs.
+
+        :param function: Function to apply to all items, this should return json serializable data.
+        :param level: The level off items which to apply the function to.
+        :param args: Extra position arguments to pass the function.
+        :param kwargs: Extra keyword arguments to pass to the function.
+        :param filter_function: Filter functions object that allows you to add filters for subject, experiments, and
+                                scans.
+        :param logfile: path to a logfile for recording the results of the map operation, this allows the resume the
+                        map in case of errors/crashes.
+        :return: A dictionary with the fulluri of each object found at the specified level as the ky and the result of
+                 the function as the value.
+        """
+        self.logger.info(f'Mapping {self.id} at level: {level}')
+        states = MappingObjectStates(logger=self.logger, filename=logfile)
+
+        if states.succeeded(self):
+            return {x.uri: x.result for x in states.values() if x.requested}
+
+        if args is None:
+            args = []
+
+        if kwargs is None:
+            kwargs = {}
+
+        if not isinstance(level, MappingLevel):
+            try:
+                level = MappingLevel(level)
+            except (ValueError, KeyError):
+                msg = f'Level "{level}" is not a valid MappingLevel, available: {[x.value for x in MappingLevel]}'
+                self.logger.error(msg)
+                raise ValueError(msg)
+
+        for uri, values in states.items():
+            self.logger.info(f'{uri}-{values.success}')
+
+        # Basically a for loop but with the option to send to the generator
+        for xnat_object in self.mapping_iter(states, level, filter_function):
+            try:
+                result = function(xnat_object, *args, **kwargs)
+            except BaseException as e:
+                states.failed(xnat_object, str(e), requested=True)
+            else:
+                # Make sure that if a logfile is used the result is compatible
+                if logfile and not check_result_type(result):
+                    raise TypeError(f'The result of the function is of incompatible'
+                                    f' with the map function type: [{type(result).__name__}] {result}')
+
+                states.success(xnat_object, result, requested=True)
+
+        return {x.uri: x.result for x in states.values() if x.requested}
+
 
 class InvestigatorData(XNATBaseObject):
     def __str__(self):
         title = self.title or ''
         first = self.firstname or ''
         last = self.lastname or ''
         fullname = '{title} {first} {last}'.format(title=title, first=first, last=last).strip()
@@ -274,50 +355,71 @@
         self.xnat_session.put(share_uri, query=query)
         self.clearcache()
 
     def create_resource(self, label, format=None, data_dir=None, method=None):
         uri = '{}/resources/{}'.format(self.fulluri, label)
         self.xnat_session.put(uri, format=format)
         self.clearcache()  # The resources changed, so we have to clear the cache
-        resource = self.xnat_session.create_object(uri, type_='xnat:resourceCatalog')
+        resource = self.xnat_session.create_object(uri)
 
         if data_dir is not None:
             resource.upload_dir(data_dir, method=method)
 
         return resource
     
     def cli_str(self):
         return "Subject {name}: id={id}, project:{proj}, full URI:{uri}".format(name=self.label, id=self.id, proj=self.project, uri=self.fulluri)
 
+    def mapping_iter(self,
+                     states: MappingObjectStates,
+                     level: MappingLevel,
+                     filter_function: 'FilterFunctions'):
+        self.logger.info(f'Start Iterating for subject {self.label}')
+        with states.descend(self, MappingLevel.SUBJECT):
+            for xnat_experiment in self.experiments.values():
+                if states.succeeded(xnat_experiment):
+                    continue
+                if filter_function and not filter_function.experiment(xnat_experiment):
+                    continue
+                if level == MappingLevel.EXPERIMENT:
+                    yield xnat_experiment
+                else:
+                    yield from xnat_experiment.mapping_iter(states, level, filter_function)
+        self.logger.info(f'Finished Iterating for subject {self.label}')
+
 
 class ExperimentData(XNATBaseObject):
     SECONDARY_LOOKUP_FIELD = 'label'
     FROM_SEARCH_URI = '{session_uri}/projects/{project}/subjects/{subject_id}/experiments/{session_id}'
     DEFAULT_SEARCH_FIELDS = ['id', 'project', 'subject_id']
 
     def __init__(self, uri=None, xnat_session=None, id_=None, datafields=None, parent=None, fieldname=None, overwrites=None, **kwargs):
 
         # If experiment is being created, check if experiment already exists
         if uri is None and parent is not None:
             if isinstance(parent, XNATListing):
                 check_parent = parent.parent
             else:
                 check_parent = parent
-            
+
+            if isinstance(check_parent, SubjectAssessorData):
+                check_parent = check_parent.subject
+
             if not isinstance(check_parent, SubjectData):
-                raise exceptions.XNATValueError(f'Cannot determine parent for experiment, should be a SubjectData, found {type(parent)}!')
+                raise exceptions.XNATValueError(f'Cannot determine parent for experiment, should be a'
+                                                f' SubjectData or SubjectAssessorData, found {type(parent)}!')
 
             project = check_parent.xnat_session.projects[check_parent.project]
 
             # Check what argument to use to build the URL
             if self._DISPLAY_IDENTIFIER is not None:
                 url_part_argument = pythonize_attribute_name(self._DISPLAY_IDENTIFIER)
             elif self.SECONDARY_LOOKUP_FIELD is not None:
                 url_part_argument = self.SECONDARY_LOOKUP_FIELD
-            
+
             # Get extra required url part
             url_part = str(kwargs.get(url_part_argument))
             if project.experiments.get(url_part) and not overwrites:
                 self.logger.error(f"Experiment with label {url_part} already exists in project {project.id}.")
                 raise exceptions.XNATObjectAlreadyExistsError(f'Experiment with label {url_part} already exists in project {project.id}.')
 
         super().__init__(uri, xnat_session, id_, datafields, parent, fieldname, overwrites, **kwargs)
@@ -398,14 +500,30 @@
 
         if not os.path.isdir(data_dir):
             self.logger.info(f'Determined data_dir to be {data_dir}, but it does not exist!')
             return None
 
         return data_dir
 
+    def mapping_iter(self,
+                     states: MappingObjectStates,
+                     level: MappingLevel,
+                     filter_function: 'FilterFunctions'):
+        self.logger.info(f'Start Iterating for experiment {self.label}')
+        with states.descend(self, MappingLevel.EXPERIMENT):
+            for xnat_scan in self.scans.values():
+                if states.succeeded(xnat_scan):
+                    continue
+                if filter_function and not filter_function.scan(xnat_scan):
+                    continue
+                if level == MappingLevel.SCAN:
+                    self.logger.info(f'Starting {xnat_scan}')
+                    yield xnat_scan
+        self.logger.info(f'Finished Iterating for experiment {self.label}')
+
 
 class SubjectAssessorData(XNATBaseObject):
     @property
     def fulluri(self):
         return '/data/archive/projects/{}/subjects/{}/experiments/{}'.format(self.project, self.subject_id, self.id)
 
     @property
@@ -428,30 +546,30 @@
         uri = '{}/assessors/{label}?xsiType={type}&label={label}&req_format=qs'.format(self.fulluri,
                                                                                        type=type_,
                                                                                        label=label)
         self.xnat_session.put(uri, accepted_status=(200, 201))
         self.clearcache()  # The resources changed, so we have to clear the cache
         return self.xnat_session.create_object('{}/assessors/{}'.format(self.fulluri, label), type_=type_)
 
-    def download(self, path, verbose=True):
-        self.xnat_session.download_zip(self.fulluri + '/scans/ALL/files', path, verbose=verbose)
+    def download(self, path, scan_filter='ALL', verbose=True):
+        self.xnat_session.download_zip(self.fulluri + '/scans/{}/files'.format(scan_filter), path, verbose=verbose)
 
-    def download_dir(self, target_dir, verbose=True):
+    def download_dir(self, target_dir, scan_filter='ALL', verbose=True):
         """
         Download the entire experiment and unpack it in a given directory. Note
         that this method will create a directory structure following
         $target_dir/{experiment.label} and unzip the experiment zips
         as given by XNAT into that. If the $target_dir/{experiment.label} does
         not exist, it will be created.
 
         :param str target_dir: directory to create experiment directory in
         :param bool verbose: show progress
         """
         # Check if there are actually file to be found
-        file_list = self.xnat_session.get_json(self.fulluri + '/scans/ALL/files')
+        file_list = self.xnat_session.get_json(self.fulluri + '/scans/{}/files'.format(scan_filter))
         if len(file_list['ResultSet']['Result']) == 0:
             # Just make sure the target directory exists and stop
             if not os.path.exists(target_dir):
                 os.mkdir(target_dir)
             return
 
         with tempfile.TemporaryFile() as temp_path:
@@ -501,15 +619,15 @@
                            secondary_lookup_field='label',
                            xsi_type='xnat:resourceCatalog')
 
     def create_resource(self, label, format=None, data_dir=None, method=None):
         uri = '{}/resources/{}'.format(self.fulluri, label)
         self.xnat_session.put(uri, format=format)
         self.clearcache()  # The resources changed, so we have to clear the cache
-        resource = self.xnat_session.create_object(uri, type_='xnat:resourceCatalog')
+        resource = self.xnat_session.create_object(uri)
 
         if data_dir is not None:
             resource.upload_dir(data_dir, method=method)
 
         return resource
 
     def download(self, path, verbose=True):
@@ -543,15 +661,15 @@
                            secondary_lookup_field='label',
                            xsi_type='xnat:resourceCatalog')
 
     def create_resource(self, label, format=None, data_dir=None, method='tgz_file'):
         uri = '{}/resources/{}'.format(self.uri, label)
         self.xnat_session.put(uri, format=format)
         self.clearcache()  # The resources changed, so we have to clear the cache
-        resource = self.xnat_session.create_object(uri, type_='xnat:resourceCatalog')
+        resource = self.xnat_session.create_object(uri)
 
         if data_dir is not None:
             resource.upload_dir(data_dir, method=method)
 
         return resource
 
     def download(self, path, verbose=True):
@@ -582,15 +700,14 @@
             experiment.project,
             self.image_session_id,
             self.id,
         )
         return self.xnat_session.services.dicom_dump(src=uri, fields=fields)
 
     def read_dicom(self, file=None, read_pixel_data=False, force=False):
-        # Check https://gist.github.com/obskyr/b9d4b4223e7eaf4eedcd9defabb34f13 for partial loading?
         if not PYDICOM_LOADED:
             raise RuntimeError('Cannot read DICOM, missing required dependency: pydicom')
 
         dicom_resource = self.resources.get('DICOM',
                                             self.resources.get('secondary'))
 
         if dicom_resource is None:
@@ -662,29 +779,27 @@
     @property
     def cache_id(self):
         return type(self).__name__, self.id
 
     @property
     @caching
     def fulldata(self):
-        # FIXME: ugly hack because direct query fails
+        # Ugly hack because direct query fails, we retrieve the parent listing data instead and filter from there
         uri, label = self.uri.rsplit('/', 1)
         data = self.xnat_session.get_json(uri)['ResultSet']['Result']
 
-        def _guess_key( d ):
-            if 'URI' not in d and 'ID' not in d and 'xnat_abstractresource_id' in d:
-                # HACK: This is a Resource where the label is not part of the uri, it uses this xnat_abstractresource_id instead.
-                return d['xnat_abstractresource_id']
-            else:
-                return d['label']
-
+        # First try to retrieve by id
         try:
-            data = next(x for x in data if _guess_key(x) == label)
+            data = next(x for x in data if x.get('xnat_abstractresource_id') == label)
         except StopIteration:
-            raise ValueError('Cannot find full data!')
+            # Then try to retrieve by label
+            try:
+                data = next(x for x in data if x.get('label') == label)
+            except StopIteration:
+                raise ValueError('Cannot find full data!')
 
         data['ID'] = data['xnat_abstractresource_id']  # Make sure the ID is present
         return data
 
     @property
     def data(self):
         return self.fulldata
@@ -941,7 +1056,14 @@
             data_dir = f"{parent.data_dir}/{self.format}"
 
         if not os.path.isdir(data_dir):
             self.logger.info(f'Determined data_dir to be {data_dir}, but it does not exist!')
             return None
 
         return data_dir
+
+
+@dataclass
+class FilterFunctions:
+    subject: Callable[[SubjectData], bool] = lambda x: True
+    experiment: Callable[[ExperimentData], bool] = lambda x: True
+    scan: Callable[[ImageScanData], bool] = lambda x: True
```

### Comparing `xnat-0.5.3/xnat/plugins.py` & `xnat-0.6.0/xnat/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
-import json
 from collections.abc import Mapping
 from .core import XNATBaseObject, caching
 
 try:
     PYDICOM_LOADED = True
     import pydicom
 except ImportError:
```

### Comparing `xnat-0.5.3/xnat/prearchive.py` & `xnat-0.6.0/xnat/prearchive.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,20 +180,20 @@
         :return: path of the downloaded zip file
         :rtype: str
         """
         self.xnat_session.download_zip(self.uri, path)
         return path
 
     def archive(self,
-                overwrite: str = None,
-                quarantine: bool = None,
-                trigger_pipelines: bool = None,
-                project: str = None,
-                subject: str = None,
-                experiment: str = None):
+                overwrite: Optional[str] = None,
+                quarantine: Optional[bool] = None,
+                trigger_pipelines: Optional[bool] = None,
+                project: Optional[str] = None,
+                subject: Optional[str] = None,
+                experiment: Optional[str] = None):
         """
         Method to archive this prearchive session to the main archive
 
         :param overwrite: how the handle existing data (none, append, delete)
         :param quarantine: flag to indicate session should be quarantined
         :param trigger_pipelines: indicate that archiving should trigger pipelines
         :param project: the project in the archive to assign the session to
```

### Comparing `xnat-0.5.3/xnat/scripts/copy_project.py` & `xnat-0.6.0/xnat/scripts/copy_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import tempfile
 import shutil
 
 from html.parser import HTMLParser
 
 import xnat
+from xnat.exceptions import XNATResponseError
 
 
 class XNATProjectCopier:
     def __init__(self, source_xnat, source_project, dest_xnat, dest_project):
         self.source_xnat = source_xnat
         self.source_project = source_project
         self.dest_xnat = dest_xnat
@@ -71,19 +72,24 @@
                 print('{}Skipping resource {}'.format(prefix, resource_id))
                 # Already there, do not copy
                 continue
 
             # Create a resources of the same xsitype
             print('{}Copying resource {}'.format(prefix, resource_id))
             dest_class = self.dest_xnat.XNAT_CLASS_LOOKUP[source_resource.__xsi_type__]
-            dest_resource = dest_class(
-                parent=dest_object,
-                label=source_resource.label,
-                content=source_resource.content
-            )
+            try:
+                dest_resource = dest_class(
+                    parent=dest_object,
+                    label=source_resource.label,
+                    content=source_resource.content
+                )
+            except XNATResponseError as e:
+                print('{} ERROR Copying resource {}'.format(prefix, resource_id))
+                print('Reason: {}'.format(e))
+                continue
 
             # Copy resource file contents
             if len(source_resource.files) > 0:
                 self.copy_resource(source_resource, dest_resource, prefix=prefix)
 
     def copy_experiment(self, source_experiment, dest_experiment):
         self.copy_fields(source_experiment, dest_experiment, prefix='    ')
@@ -121,37 +127,42 @@
         self.copy_fields(source_subject, dest_subject, prefix='  ')
         self.copy_resources(source_subject, dest_subject, prefix='  ')
 
         for source_experiment in source_subject.experiments.values():
             print('  copying experiment  {}'.format(source_experiment.label))
             if source_experiment.label in dest_subject.experiments:
                 print('    experiment already there.')
+                dest_experiment = dest_subject.experiments[source_experiment.label]
             elif hasattr(source_experiment, 'scans') and len(source_experiment.scans) > 0:
                 print('    copying data')
                 temp_file = os.path.join(self.temp_dir, source_experiment.label + '.zip')
                 try:
                     source_experiment.download(temp_file, verbose=False)
                     try:
                         dest_experiment = self.dest_xnat.services.import_(
                             temp_file,
+                            destination='archive',
                             project=self.dest_project.id,
                             subject=source_experiment.subject.label,
                             experiment=source_experiment.label
                         )
                     except xnat.exceptions.XNATUploadError as exception:
-                        print('    [ WARNING] Experiment did not include parsable dicom files, creating empty experiment')
+                        dest_class = self.dest_xnat.XNAT_CLASS_LOOKUP.get(source_experiment.__xsi_type__)
                         if 'not include parseable files' in exception.args[0]:
-                            dest_class = self.dest_xnat.XNAT_CLASS_LOOKUP.get(source_experiment.__xsi_type__)
-                            if dest_class is None:
-                                print('    [WARNING] {} class not found on destination server, skipping'.format(source_experiment.__xsi_type__))
-                                continue
-
+                            print('    [ WARNING] Experiment did not include parsable dicom files, creating empty experiment')
                             dest_experiment = dest_class(parent=dest_subject, label=source_experiment.label)
+                        elif dest_class is None:
+                            print('    [WARNING] {} class not found on destination server, skipping'.format(source_experiment.__xsi_type__))
+                            continue
                         else:
-                            raise
+                            print('    [WARNING] Issue copying experiment, creating manually...')
+                            dest_experiment = dest_class(parent=dest_subject, label=source_experiment.label)
+                except ConnectionError:
+                    print('    [ERROR] Failed to copy experiment')
+                    continue
                 finally:
                     try:
                         os.remove(temp_file)
                     except:
                         pass  # Allowed
 
             else:
```

### Comparing `xnat-0.5.3/xnat/scripts/data_integrity_check.py` & `xnat-0.6.0/xnat/scripts/data_integrity_check.py`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/xnat/scripts/import_experiment_dir.py` & `xnat-0.6.0/xnat/scripts/import_experiment_dir.py`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/xnat/search.py` & `xnat-0.6.0/xnat/search.py`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/xnat/services.py` & `xnat-0.6.0/xnat/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,18 @@
     def __init__(self, xnat_session):
         self._xnat_session = xnat_session
 
     @property
     def xnat_session(self):
         return self._xnat_session
 
-    def guess_content_type(self, path):
+    def guess_content_type(self, path: Union[str, Path]):
+        if isinstance(path, Path):
+            path = str(path)
+
         content_type, _ = mimetypes.guess_type(path)
 
         if content_type not in ['application/x-tar', 'application/zip']:
             if path.endswith('.zip'):
                 self.xnat_session.logger.warning(
                     'Found unexpect content type, but assuming zip based on the extension'
                 )
@@ -229,15 +232,15 @@
         if path is not None and data is not None:
             raise XNATValueError('Only accepts either data or path, but not both!')
         elif path is not None:
             if not os.path.exists(path):
                 raise FileNotFoundError("The file you are trying to import does not exist.")
 
             # Get mimetype of file
-            if content_type is None and isinstance(path, str):
+            if content_type is None and isinstance(path, (str, Path)):
                 content_type = self.guess_content_type(path)
 
             response = self.xnat_session.upload_file(uri=uri, path=path, query=query, content_type=content_type, method='post')
         elif data is not None and isinstance(data, str):
             response = self.xnat_session.upload_string(uri=uri, data=data, query=query, content_type=content_type, method='post')
         elif data is not None:
             response = self.xnat_session.upload_stream(uri=uri, stream=data, query=query, content_type=content_type, method='post')
```

### Comparing `xnat-0.5.3/xnat/session.py` & `xnat-0.6.0/xnat/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import io
 import netrc
 from pathlib import Path
 import os
 import re
 import threading
 from typing import Any, BinaryIO, Callable, Container, Dict, List, Optional, Tuple, Union, IO
+import zlib
 
 from progressbar import AdaptiveETA, AdaptiveTransferSpeed, Bar, BouncingBar, \
     DataSize, Percentage, ProgressBar, Timer, UnknownLength
 import requests
 from urllib import parse
 
 from . import exceptions
@@ -96,20 +97,20 @@
         else:
             self._original_uri = server.rstrip('/')
         self._logged_in_user = logged_in_user
         self._jsession = jsession
 
         self._cache = {'__objects__': {}}
         self.caching = True
-        self._source_code_file = None
         self._services = Services(xnat_session=self)
         self._plugins = Plugins(xnat_session=self)
         self._prearchive = Prearchive(xnat_session=self)
         self._users = Users(xnat_session=self)
         self._debug = debug
+        self._source_code = None
         self.logger = logger
         self.inspect = Inspect(self)
         self.request_timeout = default_timeout
 
         # Detect mouting for container service/jupyter hub
         self.mount_data_dir = os.environ.get('XNAT_DATA', None)
         self.mount_xsi_type = os.environ.get('XNAT_XSI_TYPE', None)
@@ -202,24 +203,14 @@
 
         # Set the server and interface to None
         if self._interface is not None:
             self._interface.close()
             self._interface = None
         self._server = None
 
-        # If this object is created using an automatically generated file
-        # we have to remove it.
-        if self._source_code_file is not None:
-            source_pyc = self._source_code_file + 'c'
-            if os.path.isfile(self._source_code_file):
-                os.remove(self._source_code_file)
-                self._source_code_file = None
-            if os.path.isfile(source_pyc):
-                os.remove(source_pyc)
-
         self.classes = None
 
         # Invalidate cache
         self._cache = {'__objects__': {}}
         self.caching = False
 
     @property
@@ -925,14 +916,33 @@
     def scan_types(self):
         """
          A list of scan types associated with this XNATSession instance
         """
         return self.xnat_session.get_json('/data/archive/scan_types')['ResultSet']['Result']
 
     @property
+    def source_code(self):
+        if self._source_code is not None:
+            return zlib.decompress(self._source_code).decode('utf-8')
+
+        return None
+
+    @source_code.setter
+    def source_code(self, value: str):
+        self._source_code = zlib.compress(value.encode('utf-8'))
+
+    def write_source_code(self, path: Union[str, Path]):
+        if self._source_code is None:
+            self.logger.warning('There is not source code created for this connection (model has not been built).')
+            return
+
+        with open(path, 'w') as fh_out:
+            fh_out.write(self.source_code)
+
+    @property
     @caching
     def xnat_version(self) -> str:
         """
         The version of the XNAT server
         """
         try:
             # XNAT SERVER 1.6.x
```

### Comparing `xnat-0.5.3/xnat/users.py` & `xnat-0.6.0/xnat/users.py`

 * *Files identical despite different names*

### Comparing `xnat-0.5.3/xnat/utils.py` & `xnat-0.6.0/xnat/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import datetime
+
+from datetime import datetime
 import re
 import keyword
 from functools import update_wrapper
 from io import BytesIO, BufferedIOBase, SEEK_SET, SEEK_END
 
 from dateutil import parser, tz
 import requests
 from requests.auth import AuthBase
 
 from .constants import TIMEZONES_DICT
 
 
-def parse_datetime(value: str, utc: bool = True) -> datetime.datetime:
+def parse_datetime(value: str, utc: bool = True) -> datetime:
     dt = parser.parse(value, tzinfos=TIMEZONES_DICT)
 
     if utc:
         utc_tz = tz.gettz('UTC')
         dt = dt.astimezone(utc_tz)
 
     return dt
```

### Comparing `xnat-0.5.3/xnat.egg-info/PKG-INFO` & `xnat-0.6.0/xnat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnat
-Version: 0.5.3
+Version: 0.6.0
 Summary: An XNAT client that exposes the XNAT REST interface as python objects. Part of the interface is automatically generated based on the servers data model as defined by the xnat schema.
 Home-page: https://gitlab.com/radiology/infrastructure/xnatpy
 Author: H.C. Achterberg
 Author-email: hakim.achterberg@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `xnat-0.5.3/xnat.egg-info/SOURCES.txt` & `xnat-0.6.0/xnat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 xnat/constants.py
 xnat/convert_xsd.py
 xnat/core.py
 xnat/datatypes.py
 xnat/exceptions.py
 xnat/header.py
 xnat/inspect.py
+xnat/map.py
 xnat/mixin.py
 xnat/plugins.py
 xnat/prearchive.py
 xnat/search.py
 xnat/services.py
 xnat/session.py
 xnat/type_hints.py
@@ -23,20 +24,21 @@
 xnat/version.py
 xnat.egg-info/PKG-INFO
 xnat.egg-info/SOURCES.txt
 xnat.egg-info/dependency_links.txt
 xnat.egg-info/entry_points.txt
 xnat.egg-info/requires.txt
 xnat.egg-info/top_level.txt
-xnat/client/__init__.py
-xnat/client/download.py
-xnat/client/importing.py
-xnat/client/listings.py
-xnat/client/prearchive.py
-xnat/client/rest.py
-xnat/client/scripts.py
-xnat/client/search.py
-xnat/client/utils.py
+xnat/cli/__init__.py
+xnat/cli/download.py
+xnat/cli/helpers.py
+xnat/cli/importing.py
+xnat/cli/listings.py
+xnat/cli/prearchive.py
+xnat/cli/rest.py
+xnat/cli/scripts.py
+xnat/cli/search.py
 xnat/scripts/__init__.py
 xnat/scripts/copy_project.py
 xnat/scripts/data_integrity_check.py
+xnat/scripts/delete_project.py
 xnat/scripts/import_experiment_dir.py
```

