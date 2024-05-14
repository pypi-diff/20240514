# Comparing `tmp/biobb_common-4.1.0.tar.gz` & `tmp/biobb_common-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_common-4.1.0.tar", last modified: Sat Sep  2 13:09:49 2023, max compression
+gzip compressed data, was "biobb_common-4.2.0.tar", last modified: Tue May 14 16:56:11 2024, max compression
```

## Comparing `biobb_common-4.1.0.tar` & `biobb_common-4.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-02 13:09:49.810221 biobb_common-4.1.0/
--rw-r--r--   0 pau        (501) staff       (20)    11358 2021-06-09 08:40:38.000000 biobb_common-4.1.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     4319 2023-09-02 13:09:49.809818 biobb_common-4.1.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     3420 2023-09-02 13:08:11.000000 biobb_common-4.1.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-02 13:09:49.801603 biobb_common-4.1.0/biobb_common/
--rw-r--r--   0 pau        (501) staff       (20)       44 2023-09-02 13:07:37.000000 biobb_common-4.1.0/biobb_common/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-02 13:09:49.803907 biobb_common-4.1.0/biobb_common/command_wrapper/
--rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-09 08:40:38.000000 biobb_common-4.1.0/biobb_common/command_wrapper/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     2184 2023-08-30 11:18:26.000000 biobb_common-4.1.0/biobb_common/command_wrapper/cmd_wrapper.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-02 13:09:49.804857 biobb_common-4.1.0/biobb_common/configuration/
--rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-09 08:40:38.000000 biobb_common-4.1.0/biobb_common/configuration/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)    15890 2023-08-30 10:01:24.000000 biobb_common-4.1.0/biobb_common/configuration/settings.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-02 13:09:49.806088 biobb_common-4.1.0/biobb_common/generic/
--rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-22 07:52:51.000000 biobb_common-4.1.0/biobb_common/generic/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)    18564 2023-09-01 15:52:55.000000 biobb_common-4.1.0/biobb_common/generic/biobb_object.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-02 13:09:49.809102 biobb_common-4.1.0/biobb_common/tools/
--rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-09 08:40:38.000000 biobb_common-4.1.0/biobb_common/tools/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)    27141 2023-08-30 10:37:47.000000 biobb_common-4.1.0/biobb_common/tools/file_utils.py
--rw-r--r--   0 pau        (501) staff       (20)    11607 2023-08-30 14:20:18.000000 biobb_common-4.1.0/biobb_common/tools/test_fixtures.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-02 13:09:49.803243 biobb_common-4.1.0/biobb_common.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     4319 2023-09-02 13:09:49.000000 biobb_common-4.1.0/biobb_common.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      563 2023-09-02 13:09:49.000000 biobb_common-4.1.0/biobb_common.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-09-02 13:09:49.000000 biobb_common-4.1.0/biobb_common.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       26 2023-09-02 13:09:49.000000 biobb_common-4.1.0/biobb_common.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       13 2023-09-02 13:09:49.000000 biobb_common-4.1.0/biobb_common.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-09-02 13:09:49.810376 biobb_common-4.1.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1216 2023-09-02 13:07:09.000000 biobb_common-4.1.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-14 16:56:11.735624 biobb_common-4.2.0/
+-rw-r--r--   0 pau        (501) staff       (20)    11358 2021-06-09 08:40:38.000000 biobb_common-4.2.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     4319 2024-05-14 16:56:11.735057 biobb_common-4.2.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     3420 2024-05-14 16:41:32.000000 biobb_common-4.2.0/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-14 16:56:11.726877 biobb_common-4.2.0/biobb_common/
+-rw-r--r--   0 pau        (501) staff       (20)       44 2024-05-14 16:40:14.000000 biobb_common-4.2.0/biobb_common/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-14 16:56:11.729520 biobb_common-4.2.0/biobb_common/command_wrapper/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-09 08:40:38.000000 biobb_common-4.2.0/biobb_common/command_wrapper/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     2184 2023-08-30 11:18:26.000000 biobb_common-4.2.0/biobb_common/command_wrapper/cmd_wrapper.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-14 16:56:11.730699 biobb_common-4.2.0/biobb_common/configuration/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-09 08:40:38.000000 biobb_common-4.2.0/biobb_common/configuration/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)    15977 2024-03-20 13:57:13.000000 biobb_common-4.2.0/biobb_common/configuration/settings.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-14 16:56:11.731639 biobb_common-4.2.0/biobb_common/generic/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-22 07:52:51.000000 biobb_common-4.2.0/biobb_common/generic/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)    18901 2024-05-13 20:48:21.000000 biobb_common-4.2.0/biobb_common/generic/biobb_object.py
+-rw-r--r--   0 pau        (501) staff       (20)        0 2024-02-12 15:51:14.000000 biobb_common-4.2.0/biobb_common/py.typed
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-14 16:56:11.734147 biobb_common-4.2.0/biobb_common/tools/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2021-06-09 08:40:38.000000 biobb_common-4.2.0/biobb_common/tools/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)    28096 2024-05-13 22:20:18.000000 biobb_common-4.2.0/biobb_common/tools/file_utils.py
+-rw-r--r--   0 pau        (501) staff       (20)    11881 2024-05-13 22:13:40.000000 biobb_common-4.2.0/biobb_common/tools/test_fixtures.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-14 16:56:11.728826 biobb_common-4.2.0/biobb_common.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     4319 2024-05-14 16:56:11.000000 biobb_common-4.2.0/biobb_common.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      585 2024-05-14 16:56:11.000000 biobb_common-4.2.0/biobb_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-14 16:56:11.000000 biobb_common-4.2.0/biobb_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-14 16:56:11.000000 biobb_common-4.2.0/biobb_common.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       13 2024-05-14 16:56:11.000000 biobb_common-4.2.0/biobb_common.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-14 16:56:11.735785 biobb_common-4.2.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1264 2024-05-14 16:39:14.000000 biobb_common-4.2.0/setup.py
```

### Comparing `biobb_common-4.1.0/LICENSE` & `biobb_common-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_common-4.1.0/PKG-INFO` & `biobb_common-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: biobb_common
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_common is the base package required to use the biobb packages.
 Home-page: https://github.com/bioexcel/biobb_common
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_common.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-common.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_common?label=Version)](https://GitHub.com/bioexcel/biobb_common/tags/)
 [![](https://img.shields.io/pypi/v/biobb-common.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-common/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_common?label=Conda)](https://anaconda.org/bioconda/biobb_common)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_common?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_common)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_common?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_common:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_common:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)]()
 [![](https://img.shields.io/pypi/pyversions/biobb-common.svg?label=Python%20Versions)]()
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)]()
 
 [![](https://readthedocs.org/projects/biobb-common/badge/?version=latest&label=Docs)](https://biobb-common.readthedocs.io/en/latest/?badge=latest)
@@ -50,22 +50,22 @@
 ### Introduction
 Biobb_common is the base package required to use the biobb
 packages.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_common.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-common.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.1
+v4.2.0 2024.1
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_common-4.1.0/README.md` & `biobb_common-4.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_common?label=Version)](https://GitHub.com/bioexcel/biobb_common/tags/)
 [![](https://img.shields.io/pypi/v/biobb-common.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-common/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_common?label=Conda)](https://anaconda.org/bioconda/biobb_common)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_common?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_common)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_common?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_common:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_common:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)]()
 [![](https://img.shields.io/pypi/pyversions/biobb-common.svg?label=Python%20Versions)]()
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)]()
 
 [![](https://readthedocs.org/projects/biobb-common/badge/?version=latest&label=Docs)](https://biobb-common.readthedocs.io/en/latest/?badge=latest)
@@ -28,22 +28,22 @@
 ### Introduction
 Biobb_common is the base package required to use the biobb
 packages.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_common.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-common.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.1
+v4.2.0 2024.1
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_common-4.1.0/biobb_common/command_wrapper/cmd_wrapper.py` & `biobb_common-4.2.0/biobb_common/command_wrapper/cmd_wrapper.py`

 * *Files identical despite different names*

### Comparing `biobb_common-4.1.0/biobb_common/configuration/settings.py` & `biobb_common-4.2.0/biobb_common/configuration/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,29 +32,29 @@
 """
 
 import yaml
 import json
 import logging
 from pathlib import Path
 from biobb_common.tools import file_utils as fu
-from typing import Optional
+from typing import Dict, Any, Optional
 
 GALAXY_CHARACTER_MAP = {
     "__gt__": ">",
     "__lt__": "<",
     "__sq__": "'",
     "__dq__": '"',
     "__ob__": "[",
     "__cb__": "]",
     "__oc__": "{",
     "__cc__": "}",
     "__cn__": "\n",
     "__cr__": "\r",
     "__tc__": "\t",
-    "__pd__": "#",
+    "__pd__": "#"
 }
 
 
 def trans_galaxy_charmap(input_str):
     """Fixes escape characters introduced by Galaxy on Json inputs"""
     for ch in GALAXY_CHARACTER_MAP:
         input_str = input_str.replace(ch, GALAXY_CHARACTER_MAP[ch])
@@ -110,17 +110,15 @@
 
     def get_working_dir_path(self) -> str:
         if self.system:
             return self.properties[self.system].get("working_dir_path")
 
         return self.properties.get("working_dir_path")
 
-    def get_prop_dic(
-        self, prefix: Optional[str] = None, global_log: Optional[logging.Logger] = None
-    ) -> dict:
+    def get_prop_dic(self, prefix: Optional[str] = None, global_log: Optional[logging.Logger] = None) -> Dict[str, Any]:
         """get_prop_dic() returns the properties dictionary where keys are the
         step names in the configuration YAML file and every value contains another
         nested dictionary containing the keys and values of each step properties section.
         All the paths in the system section are copied in each nested dictionary.
         For each nested dictionary the following keys are added:
             | **path** (*str*): Absolute path to the step working dir.
             | **step** (*str*): Name of the step.
@@ -132,15 +130,16 @@
         Args:
             prefix (str): Prefix if provided.
             global_log (:obj:Logger): Log from the main workflow.
 
         Returns:
             dict: Dictionary of properties.
         """
-        prop_dic = dict()
+
+        prop_dic: Dict[str, Any] = dict()
         prefix = "" if prefix is None else prefix.strip()
 
         # There is no step
         if "paths" in self.properties or "properties" in self.properties:
             prop_dic = dict()
             if self.system:
                 prop_dic["path"] = str(
@@ -307,28 +306,30 @@
                 if isinstance(value, str) and value.startswith("file:"):
                     prop_dic[key2] = value.split(":")[1]
                 else:
                     if self.system:
                         prop_dic[key2] = str(
                             Path(
                                 self.properties[self.system]["working_dir_path"]
-                            ).joinpath(prefix, key, value)
+                            ).joinpath(prefix, key2, value)
                         )
                     else:
                         prop_dic[key2] = str(
                             Path(self.properties["working_dir_path"]).joinpath(
                                 prefix, value
                             )
                         )
 
         # Properties with step name
         else:
+
             for key in prop_dic:
                 for key2, value in prop_dic[key].items():
                     if isinstance(value, str) and value.startswith("dependency"):
+                        dependency_step = value.split("/")[1]
                         while isinstance(value, str) and value.startswith("dependency"):
                             dependency_step = value.split("/")[1]
                             value = prop_dic[value.split("/")[1]][value.split("/")[2]]
                         if self.properties.get(self.system):
                             prop_dic[key][key2] = str(
                                 Path(
                                     self.properties[self.system]["working_dir_path"]
```

### Comparing `biobb_common-4.1.0/biobb_common/generic/biobb_object.py` & `biobb_common-4.2.0/biobb_common/generic/biobb_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Module containing the BiobbObject generic parent class."""
 import os
 import importlib
 import difflib
 import typing
-from typing import Optional, Mapping, Set, Union, Dict, List
+from typing import Optional, Mapping, Set, Union, Dict, List, Any
 import warnings
 from pathlib import Path
 from sys import platform
 import shutil
 from pydoc import locate
 from biobb_common.tools import file_utils as fu
 from biobb_common.command_wrapper import cmd_wrapper
+from logging import Logger
 
 
 class BiobbObject:
     """
     | biobb_common BiobbObject
     | Generic parent class for the rest of the Biobb clases.
     | The BiobbOject class contains all the properties and methods that are common to all the biobb blocks.
@@ -32,67 +33,65 @@
             * **container_volume_path** (*str*) - ("/data") Path to an internal directory in the container.
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash -c") Path to the binary executable of the container shell.
             * **container_generic_command** (*str*) - ("run") Which command typically run or exec will be used to execute your image.
     """
 
-    def __init__(self, properties: Optional[dict] = None, **kwargs) -> None:
+    def __init__(self, properties=None, **kwargs) -> None:  # type: ignore
         properties = properties or {}
 
         # Input/Output files
-        self.io_dict: Dict[str, Union[str, Dict[str, Union[str, Path]]]] = {"in": {}, "out": {}}
+        self.io_dict: Dict[str, Dict] = {"in": {}, "out": {}}
 
         # container Specific
-        self.container_path = properties.get("container_path")
+        self.container_path: Optional[str] = properties.get("container_path")
         self.container_image: str = properties.get("container_image", '')
-        self.container_volume_path = properties.get(
+        self.container_volume_path: str = properties.get(
             "container_volume_path", "/data")
-        self.container_working_dir = properties.get("container_working_dir")
-        self.container_user_id = properties.get("container_user_id")
-        self.container_shell_path = properties.get(
+        self.container_working_dir: Optional[str] = properties.get("container_working_dir")
+        self.container_user_id: Optional[str] = properties.get("container_user_id")
+        self.container_shell_path: str = properties.get(
             "container_shell_path", "/bin/bash -c"
         )
-        self.container_generic_command = properties.get(
+        self.container_generic_command: str = properties.get(
             "container_generic_command", "run"
         )
 
         # stage
-        self.stage_io_dict: Dict[str, Union[str, Dict[str, Union[str, Path]]]] = {"in": {}, "out": {}}
+        self.stage_io_dict: Dict[str, Any] = {"in": {}, "out": {}}
 
         # Properties common in all BB
         self.disable_sandbox: bool = properties.get("disable_sandbox", False)
         self.chdir_sandbox: bool = properties.get("chdir_sandbox", False)
-        self.binary_path = properties.get("binary_path")
-        self.can_write_console_log = properties.get(
+        self.binary_path: Optional[str] = properties.get("binary_path")
+        self.can_write_console_log: bool = properties.get(
             "can_write_console_log", True)
-        self.global_log = properties.get("global_log", None)
-        self.out_log = None
-        self.err_log = None
-        self.prefix = properties.get("prefix", None)
-        self.step = properties.get("step", None)
-        self.path = properties.get("path", "")
-        self.remove_tmp = properties.get("remove_tmp", True)
-        self.restart = properties.get("restart", False)
+        self.global_log: Optional[Logger] = properties.get("global_log", None)
+        self.out_log: Optional[Logger] = None
+        self.err_log: Optional[Logger] = None
+        self.prefix: Optional[str] = properties.get("prefix", None)
+        self.step: Optional[str] = properties.get("step", None)
+        self.path: str = properties.get("path", "")
+        self.remove_tmp: bool = properties.get("remove_tmp", True)
+        self.restart: bool = properties.get("restart", False)
         self.cmd: List[str] = []
-        self.return_code = None
+        self.return_code: int = 0
         self.tmp_files: List[Union[str, Path]] = []
-        self.env_vars_dict: typing.Mapping = properties.get(
+        self.env_vars_dict: typing.Dict = properties.get(
             "env_vars_dict", {})
         self.shell_path: typing.Union[str, Path] = properties.get(
             "shell_path", os.getenv("SHELL", "/bin/bash")
         )
 
-        self.dev = properties.get("dev", None)
-        self.check_extensions = properties.get("check_extensions", True)
-        self.check_var_typing = properties.get("check_var_typing", True)
+        self.dev: Optional[str] = properties.get("dev", None)
+        self.check_extensions: bool = properties.get("check_extensions", True)
+        self.check_var_typing: bool = properties.get("check_var_typing", True)
         self.locals_var_dict: Mapping[str, str] = dict()
-        self.doc_arguments_dict, self.doc_properties_dict = fu.get_doc_dicts(
-            self.__doc__
-        )
+        self.doc_arguments_dict, self.doc_properties_dict = fu.get_doc_dicts(self.__doc__)
 
         try:
             self.version = importlib.import_module(
                 self.__module__.split(".")[0]
             ).__version__
         except Exception:
             self.version = None
@@ -131,15 +130,18 @@
         )
 
         # Check types
         if check_var_typing and self.doc_properties_dict:
             for prop, value in properties.items():
                 if self.doc_properties_dict.get(prop):
                     property_type = self.doc_properties_dict[prop].get("type")
-                    if not isinstance(value, locate(property_type)):
+                    classinfo: object = locate(property_type).__class__
+                    if classinfo == type:
+                        classinfo = locate(property_type)
+                    if not isinstance(value, classinfo):  # type: ignore
                         warnings.warn(
                             f"Warning: {prop} property type not recognized. Got {type(value)} Expected {locate(property_type)}"
                         )
 
         error_properties = set(
             [prop for prop in properties.keys() if prop not in self.__dict__.keys()]
         )
@@ -159,15 +161,15 @@
             fu.log(
                 f"Executing {self.__module__} Version: {self.version}",
                 self.out_log,
                 self.global_log,
             )
 
         if self.restart:
-            if fu.check_complete_files(self.io_dict["out"].values()):
+            if fu.check_complete_files(self.io_dict["out"].values()):  # type: ignore
                 fu.log(
                     "Restart is enabled, this step: %s will the skipped" % self.step,
                     self.out_log,
                     self.global_log,
                 )
                 return True
         return False
```

### Comparing `biobb_common-4.1.0/biobb_common/tools/file_utils.py` & `biobb_common-4.2.0/biobb_common/tools/file_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 import shutil
 import uuid
 import warnings
 import zipfile
 from sys import platform
 from pathlib import Path
 import typing
-from typing import Optional
+from typing import Optional, Union, List, Sequence, Dict
 import sys
 
 
-def create_unique_file_path(parent_dir: str = None, extension: str = None) -> str:
+def create_unique_file_path(parent_dir: Optional[Union[str, Path]] = None, extension: Optional[Union[str, Path]] = None) -> str:
     if not parent_dir:
         parent_dir = Path.cwd()
     if not extension:
         extension = ""
     while True:
-        name = str(uuid.uuid4()) + extension
+        name = f"{uuid.uuid4()}{extension}"
         file_path = Path.joinpath(Path(parent_dir).resolve(), name)
         if not file_path.exists():
             return str(file_path)
 
 
 def create_dir(dir_path: str) -> str:
     """Returns the directory **dir_path** and create it if path does not exist.
@@ -90,15 +90,15 @@
             if path:
                 new_dir = str(Path(path).joinpath(new_dir))
             if out_log:
                 out_log.info("Trying with: " + new_dir)
     raise FileExistsError
 
 
-def get_working_dir_path(working_dir_path: str = None, restart: bool = False) -> str:
+def get_working_dir_path(working_dir_path: Optional[Union[str, Path]] = None, restart: bool = False) -> str:
     """Return the directory **working_dir_path** and create it if working_dir_path
     does not exist. If **working_dir_path** exists a consecutive numerical suffix
     is added to the end of the **working_dir_path** and is returned.
 
     Args:
         working_dir_path (str): Path to the workflow results.
         restart (bool): If step result exists do not execute the step again.
@@ -111,32 +111,33 @@
 
     working_dir_path = str(Path(working_dir_path).resolve())
 
     if (not Path(working_dir_path).exists()) or restart:
         return str(Path(working_dir_path))
 
     cont = 1
-    while Path(working_dir_path).exists():
+    while Path(str(working_dir_path)).exists():
         working_dir_path = (
             re.split(r"_[0-9]+$", str(working_dir_path))[0] + "_" + str(cont)
         )
         cont += 1
     return str(working_dir_path)
 
 
 def zip_list(
-    zip_file: str, file_list: typing.Iterable[str], out_log: logging.Logger = None
+    zip_file: Union[str, Path], file_list: Sequence[Union[str, Path]], out_log: Optional[logging.Logger] = None
 ):
     """Compress all files listed in **file_list** into **zip_file** zip file.
 
     Args:
         zip_file (str): Output compressed zip file.
         file_list (:obj:`list` of :obj:`str`): Input list of files to be compressed.
         out_log (:obj:`logging.Logger`): Input log object.
     """
+    file_list = list(file_list)
     file_list.sort()
     Path(zip_file).parent.mkdir(parents=True, exist_ok=True)
     with zipfile.ZipFile(zip_file, "w") as zip_f:
         inserted = []
         for index, f in enumerate(file_list):
             base_name = Path(f).name
             if base_name in inserted:
@@ -146,42 +147,42 @@
     if out_log:
         out_log.info("Adding:")
         out_log.info(str(file_list))
         out_log.info("to: " + str(Path(zip_file).resolve()))
 
 
 def unzip_list(
-    zip_file: str, dest_dir: str = None, out_log: logging.Logger = None
-) -> typing.List[str]:
+    zip_file: Union[str, Path], dest_dir: Optional[Union[str, Path]] = None, out_log: Optional[logging.Logger] = None
+) -> List[str]:
     """Extract all files in the zipball file and return a list containing the
         absolute path of the extracted files.
 
     Args:
         zip_file (str): Input compressed zip file.
         dest_dir (str): Path to directory where the files will be extracted.
         out_log (:obj:`logging.Logger`): Input log object.
 
     Returns:
         :obj:`list` of :obj:`str`: List of paths of the extracted files.
     """
     with zipfile.ZipFile(zip_file, "r") as zip_f:
         zip_f.extractall(path=dest_dir)
-        file_list = [str(Path(dest_dir).joinpath(f)) for f in zip_f.namelist()]
+        file_list = [str(Path(str(dest_dir)).joinpath(f)) for f in zip_f.namelist()]
 
     if out_log:
         out_log.info("Extracting: " + str(Path(zip_file).resolve()))
         out_log.info("to:")
         out_log.info(str(file_list))
 
     return file_list
 
 
 def search_topology_files(
-    top_file: str, out_log: logging.Logger = None
-) -> typing.List[str]:
+    top_file: Union[str, Path], out_log: Optional[logging.Logger] = None
+) -> List[str]:
     """Search the top and itp files to create a list of the topology files
 
     Args:
         top_file (str): Topology GROMACS top file.
         out_log (:obj:`logging.Logger`): Input log object.
 
     Returns:
@@ -197,23 +198,23 @@
                 if include_file:
                     found_file = str(Path(top_dir_name).joinpath(include_file.group(1)))
                     file_list += search_topology_files(found_file, out_log)
     else:
         if out_log:
             out_log.info("Ignored file %s" % top_file)
         return file_list
-    return file_list + [top_file]
+    return file_list + [str(top_file)]
 
 
 def zip_top(
-    zip_file: str,
-    top_file: str,
-    out_log: logging.Logger = None,
+    zip_file: Union[str, Path],
+    top_file: Union[str, Path],
+    out_log: Optional[logging.Logger] = None,
     remove_original_files: bool = True,
-) -> typing.List[str]:
+) -> List[str]:
     """Compress all *.itp and *.top files in the cwd into **zip_file** zip file.
 
     Args:
         zip_file (str): Output compressed zip file.
         top_file (str): Topology TOP GROMACS file.
         out_log (:obj:`logging.Logger`): Input log object.
 
@@ -225,17 +226,17 @@
     zip_list(zip_file, file_list, out_log)
     if remove_original_files:
         rm_file_list(file_list, out_log)
     return file_list
 
 
 def unzip_top(
-    zip_file: str,
-    out_log: logging.Logger = None,
-    unique_dir: typing.Union[pathlib.Path, str] = None,
+    zip_file: Union[str, Path],
+    out_log: Optional[logging.Logger] = None,
+    unique_dir: Optional[typing.Union[pathlib.Path, str]] = None,
 ) -> str:
     """Extract all files in the zip_file and copy the file extracted ".top" file to top_file.
 
     Args:
         zip_file (str): Input topology zipball file path.
         out_log (:obj:`logging.Logger`): Input log object.
         unique_dir (str): Directory where the topology will be extracted.
@@ -257,17 +258,17 @@
 
 
 def get_logs_prefix():
     return 4 * " "
 
 
 def get_logs(
-    path: str = None,
-    prefix: str = None,
-    step: str = None,
+    path: Optional[Union[str, Path]] = None,
+    prefix: Optional[str] = None,
+    step: Optional[str] = None,
     can_write_console: bool = True,
     level: str = "INFO",
     light_format: bool = False,
 ) -> typing.Tuple[logging.Logger, logging.Logger]:
     """Get the error and and out Python Logger objects.
 
     Args:
@@ -409,39 +410,39 @@
         "mili seconds",
     ]
     t = time_ps * 1000
     for tu in time_units:
         if t < 1000:
             return str(t) + " " + tu
 
-        t /= 1000
+        t = int(t/1000)
     return str(time_ps)
 
 
-def check_properties(obj: object, properties: dict, reserved_properties: dict = None):
+def check_properties(obj: object, properties: dict, reserved_properties: Optional[Sequence[str]] = None):
     if not reserved_properties:
         reserved_properties = []
-    reserved_properties = set(["system", "working_dir_path"] + reserved_properties)
     error_properties = set(
         [prop for prop in properties.keys() if prop not in obj.__dict__.keys()]
     )
-    error_properties -= reserved_properties
+    error_properties -= set(["system", "working_dir_path"] + list(reserved_properties))
     for error_property in error_properties:
         close_property = difflib.get_close_matches(
             error_property, obj.__dict__.keys(), n=1, cutoff=0.01
         )
         close_property = close_property[0] if close_property else ""
         warnings.warn(
             "Warning: %s is not a recognized property. The most similar property is: %s"
             % (error_property, close_property)
         )
 
 
 def create_name(
-    path: str = None, prefix: str = None, step: str = None, name: str = None
+    path: Optional[Union[str, Path]] = None, prefix: Optional[str] = None,
+    step: Optional[str] = None, name: Optional[str] = None
 ) -> str:
     """Return file name.
 
     Args:
         path (str): Path to the file directory.
         prefix (str): Prefix added to the name of the file.
         step (str):  String added between the **prefix** arg and the **name** arg of the file.
@@ -462,24 +463,24 @@
             name = prefix + "_" + name
         else:
             name = prefix
     if path:
         if name:
             name = str(Path(path).joinpath(name))
         else:
-            name = path
+            name = str(path)
     return name
 
 
 def write_failed_output(file_name: str):
     with open(file_name, "w") as f:
         f.write("Error\n")
 
 
-def rm(file_name: str) -> str:
+def rm(file_name: Union[str, Path]) -> Optional[Union[str, Path]]:
     try:
         file_path = pathlib.Path(file_name)
         if file_path.exists():
             if file_path.is_dir():
                 shutil.rmtree(file_name)
                 return file_name
             if file_path.is_file():
@@ -487,40 +488,36 @@
                 return file_name
     except Exception:
         pass
     return None
 
 
 def rm_file_list(
-    file_list: typing.Iterable[str], out_log: logging.Logger = None
-) -> typing.List[str]:
-    removed_files = [f for f in file_list if rm(f)]
+    file_list: typing.Iterable[Union[str, Path]], out_log: Optional[logging.Logger] = None
+) -> List[str]:
+    removed_files = [str(f) for f in file_list if rm(f)]
     if out_log:
         log("Removed: %s" % str(removed_files), out_log)
     return removed_files
 
 
 def check_complete_files(output_file_list: typing.Iterable[str]) -> bool:
     for output_file in filter(None, output_file_list):
         if not (Path(output_file).is_file() and Path(output_file).stat().st_size > 0):
             return False
     return True
 
 
-def copy_to_container(
-    container_path: str,
-    container_volume_path: str,
-    io_dict: typing.Mapping,
-    out_log: logging.Logger = None,
-) -> dict:
+def copy_to_container(container_path: Optional[Union[str, Path]], container_volume_path: str,
+                      io_dict: Dict, out_log: Optional[logging.Logger] = None) -> Dict:
     if not container_path:
         return io_dict
 
     unique_dir = str(Path(create_unique_dir()).resolve())
-    container_io_dict = {"in": {}, "out": {}, "unique_dir": unique_dir}
+    container_io_dict: Dict = {"in": {}, "out": {}, "unique_dir": unique_dir}
 
     # IN files COPY and assign INTERNAL PATH
     for file_ref, file_path in io_dict["in"].items():
         if file_path:
             if Path(file_path).exists():
                 shutil.copy2(file_path, unique_dir)
                 log(f"Copy: {file_path} to {unique_dir}")
@@ -552,105 +549,105 @@
                 Path(container_io_dict["unique_dir"]).joinpath(Path(file_path).name)
             )
             if Path(container_file_path).exists():
                 shutil.copy2(container_file_path, io_dict["out"][file_ref])
 
 
 def create_cmd_line(
-    cmd: typing.Iterable[str],
-    container_path: str = "",
-    host_volume: str = None,
-    container_volume: str = None,
-    container_working_dir: str = None,
-    container_user_uid: str = None,
-    container_shell_path: str = None,
-    container_image: str = None,
-    out_log: logging.Logger = None,
-    global_log: logging.Logger = None,
-) -> typing.List[str]:
+    cmd: List[str],
+    container_path: Optional[Union[str, Path]] = "",
+    host_volume: Optional[Union[str, Path]] = None,
+    container_volume: Optional[Union[str, Path]] = None,
+    container_working_dir: Optional[Union[str, Path]] = None,
+    container_user_uid: Optional[str] = None,
+    container_shell_path: Optional[Union[str, Path]] = None,
+    container_image: Optional[Union[str, Path]] = None,
+    out_log: Optional[logging.Logger] = None,
+    global_log: Optional[logging.Logger] = None
+) -> List[str]:
     container_path = container_path or ""
-    if container_path.endswith("singularity"):
+    if str(container_path).endswith("singularity"):
         log("Using Singularity image %s" % container_image, out_log, global_log)
-        if not Path(container_image).exists():
+        if not Path(str(container_image)).exists():
             log(
                 f"{container_image} does not exist trying to pull it",
                 out_log,
                 global_log,
             )
-            container_image_name = str(Path(container_image).with_suffix(".sif").name)
+            container_image_name = str(Path(str(container_image)).with_suffix(".sif").name)
             singularity_pull_cmd = [
-                container_path,
+                str(container_path),
                 "pull",
                 "--name",
-                container_image_name,
-                container_image,
+                str(container_image_name),
+                str(container_image),
             ]
             try:
                 from biobb_common.command_wrapper import cmd_wrapper
 
-                cmd_wrapper.CmdWrapper(singularity_pull_cmd, out_log).launch()
+                cmd_wrapper.CmdWrapper(cmd=singularity_pull_cmd, out_log=out_log).launch()
                 if Path(container_image_name).exists():
                     container_image = container_image_name
                 else:
                     raise FileNotFoundError
             except FileNotFoundError:
                 log(f"{' '.join(singularity_pull_cmd)} not found", out_log, global_log)
                 raise FileNotFoundError
-        singularity_cmd = [
-            container_path,
+        singularity_cmd: List[str] = [
+            str(container_path),
             "exec",
             "-e",
             "--bind",
-            host_volume + ":" + container_volume,
-            container_image,
+            str(host_volume) + ":" + str(container_volume),
+            str(container_image),
         ]
         # If we are working on a mac remove -e option because is still no available
         if platform == "darwin":
             if "-e" in singularity_cmd:
                 singularity_cmd.remove("-e")
 
         cmd = ['"' + " ".join(cmd) + '"']
-        singularity_cmd.extend([container_shell_path, "-c"])
+        singularity_cmd.extend([str(container_shell_path), "-c"])
         return singularity_cmd + cmd
 
-    elif container_path.endswith("docker"):
+    elif str(container_path).endswith("docker"):
         log("Using Docker image %s" % container_image, out_log, global_log)
-        docker_cmd = [container_path, "run"]
+        docker_cmd = [str(container_path), "run"]
         if container_working_dir:
             docker_cmd.append("-w")
-            docker_cmd.append(container_working_dir)
+            docker_cmd.append(str(container_working_dir))
         if container_volume:
             docker_cmd.append("-v")
-            docker_cmd.append(host_volume + ":" + container_volume)
+            docker_cmd.append(str(host_volume) + ":" + str(container_volume))
         if container_user_uid:
             docker_cmd.append("--user")
             docker_cmd.append(container_user_uid)
 
-        docker_cmd.append(container_image)
+        docker_cmd.append(str(container_image))
 
         cmd = ['"' + " ".join(cmd) + '"']
-        docker_cmd.extend([container_shell_path, "-c"])
+        docker_cmd.extend([str(container_shell_path), "-c"])
         return docker_cmd + cmd
 
-    elif container_path.endswith("pcocc"):
+    elif str(container_path).endswith("pcocc"):
         # pcocc run -I racov56:pmx cli.py mutate -h
         log("Using pcocc image %s" % container_image, out_log, global_log)
-        pcocc_cmd = [container_path, "run", "-I", container_image]
+        pcocc_cmd = [str(container_path), "run", "-I", str(container_image)]
         if container_working_dir:
             pcocc_cmd.append("--cwd")
-            pcocc_cmd.append(container_working_dir)
+            pcocc_cmd.append(str(container_working_dir))
         if container_volume:
             pcocc_cmd.append("--mount")
-            pcocc_cmd.append(host_volume + ":" + container_volume)
+            pcocc_cmd.append(str(host_volume) + ":" + str(container_volume))
         if container_user_uid:
             pcocc_cmd.append("--user")
             pcocc_cmd.append(container_user_uid)
 
         cmd = ['\\"' + " ".join(cmd) + '\\"']
-        pcocc_cmd.extend([container_shell_path, "-c"])
+        pcocc_cmd.extend([str(container_shell_path), "-c"])
         return pcocc_cmd + cmd
 
     else:
         # log('Not using any container', out_log, global_log)
         return cmd
 
 
@@ -665,40 +662,42 @@
         r"(?:\*\ *\*\*)(?P<property>.*?)(?:\*\*)\ *(?:\(\*)(?P<type>\w*)(?:\*\))\ *\-\ ?(?:\()(?P<default_value>.*?)(?:\))\ *(?:(?:\[)(?P<wf_property>WF property)(?:\]))?\ *(?:(?:\[)(?P<range_start>[\-]?\d+(?:\.\d+)?)\~(?P<range_stop>[\-]?\d+(?:\.\d+)?)(?:\|)?(?P<range_step>\d+(?:\.\d+)?)?(?:\]))?\ *(?:(?:\[)(.*?)(?:\]))?\ *(?P<description>.*)"
     )
     regex_property_value = re.compile(
         r"(?P<value>\w*)\ *(?:(?:\()(?P<description>.*?)?(?:\)))?"
     )
 
     doc_lines = list(
-        map(str.strip, filter(lambda line: line.strip(), doc.splitlines()))
+        map(str.strip, filter(lambda line: line.strip(), str(doc).splitlines()))
     )
     args_index = doc_lines.index(
         next(filter(lambda line: line.lower().startswith("args"), doc_lines))
     )
     properties_index = doc_lines.index(
         next(filter(lambda line: line.lower().startswith("properties"), doc_lines))
     )
     examples_index = doc_lines.index(
         next(filter(lambda line: line.lower().startswith("examples"), doc_lines))
     )
-    arguments_lines_list = doc_lines[args_index + 1 : properties_index]
-    properties_lines_list = doc_lines[properties_index + 1 : examples_index]
+    arguments_lines_list = doc_lines[args_index + 1: properties_index]
+    properties_lines_list = doc_lines[properties_index + 1: examples_index]
 
     doc_arguments_dict = {}
     for argument_line in arguments_lines_list:
-        argument_dict = regex_argument.match(argument_line).groupdict()
+        match_argument = regex_argument.match(argument_line)
+        argument_dict = match_argument.groupdict() if match_argument is not None else {}
         argument_dict["formats"] = {
             match.group("extension"): match.group("edam")
             for match in regex_argument_formats.finditer(argument_dict["formats"])
         }
         doc_arguments_dict[argument_dict.pop("argument")] = argument_dict
 
     doc_properties_dict = {}
     for property_line in properties_lines_list:
-        property_dict = regex_property.match(property_line).groupdict()
+        match_property = regex_property.match(property_line)
+        property_dict = match_property.groupdict() if match_property is not None else {}
         property_dict["values"] = None
         if "Values:" in property_dict["description"]:
             property_dict["description"], property_dict["values"] = property_dict[
                 "description"
             ].split("Values:")
             property_dict["values"] = {
                 match.group("value"): match.group("description")
@@ -713,15 +712,15 @@
 def check_argument(
     path: Optional[pathlib.Path],
     argument: str,
     optional: bool,
     module_name: str,
     input_output: Optional[str] = None,
     output_files_created: bool = False,
-    extension_list: Optional[typing.List[str]] = None,
+    extension_list: Optional[Sequence[str]] = None,
     raise_exception: bool = True,
     check_extensions: bool = True,
     out_log: Optional[logging.Logger] = None,
 ) -> None:
     if optional and not path:
         return None
 
@@ -740,15 +739,15 @@
             )
         warnings.warn(unable_to_determine_string)
 
     if input_file or output_files_created:
         not_found_error_string = (
             f"Path {path} --- {module_name}: Unexisting {argument} file."
         )
-        if not path.exists():
+        if not Path(str(path)).exists():
             log(not_found_error_string, out_log)
             if raise_exception:
                 raise FileNotFoundError(
                     errno.ENOENT, os.strerror(errno.ENOENT), not_found_error_string
                 )
             warnings.warn(not_found_error_string)
     # else:
@@ -757,15 +756,15 @@
     #         log(not_found_dir_error_string, out_log)
     #         if raise_exception:
     #             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), not_found_dir_error_string)
     #         warnings.warn(not_found_dir_error_string)
 
     if check_extensions and extension_list:
         no_extension_error_string = f"{module_name} {argument}: {path} has no extension. If you want to suppress this message, please set the check_extensions property to False"
-        if not path.suffix:
+        if not Path(str(path)).suffix:
             log(no_extension_error_string)
             warnings.warn(no_extension_error_string)
         else:
             not_valid_extension_error_string = f"{module_name} {argument}: {path} extension is not in the valid extensions list: {extension_list}. If you want to suppress this message, please set the check_extensions property to False"
-            if not path.suffix[1:].lower() in extension_list:
+            if not Path(str(path)).suffix[1:].lower() in extension_list:
                 log(not_valid_extension_error_string)
                 warnings.warn(not_valid_extension_error_string)
```

### Comparing `biobb_common-4.1.0/biobb_common/tools/test_fixtures.py` & `biobb_common-4.2.0/biobb_common/tools/test_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import typing
 from typing import Optional
 from pathlib import Path
 import sys
 import shutil
 import hashlib
-import Bio.PDB
+import Bio.PDB  # type: ignore
 import codecs
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 import numpy as np
 
 
 def test_setup(test_object, dict_key: Optional[str] = None, config: Optional[str] = None):
@@ -19,15 +19,15 @@
     attributes to the **test_object** and create a directory to launch the unitest.
 
     Args:
         test_object (:obj:`test`): The test object.
         dict_key (str): Key of the test parameters in the yaml config file.
         config (str): Path to the configuration file.
     """
-    test_object.testfile_dir = str(Path(Path(sys.modules[test_object.__module__].__file__).resolve()).parent)
+    test_object.testfile_dir = str(Path(Path(str(sys.modules[test_object.__module__].__file__)).resolve()).parent)
     test_object.unitest_dir = str(Path(test_object.testfile_dir).parent)
     test_object.test_dir = str(Path(test_object.unitest_dir).parent)
     test_object.data_dir = str(Path(test_object.test_dir).joinpath('data'))
     test_object.reference_dir = str(Path(test_object.test_dir).joinpath('reference'))
     if config:
         test_object.conf_file_path = config
     else:
@@ -135,14 +135,17 @@
     if file_a.endswith(image_extensions) and file_b.endswith(image_extensions):
         return compare_images(file_a, file_b, kwargs.get('percent_tolerance', 1.0))
 
     return compare_hash(file_a, file_b)
 
 
 def compare_line_by_line(file_a: str, file_b: str, ignore_list: typing.List[typing.Union[str, int]]) -> bool:
+    print(f"Comparing ignoring lines containing this words: {ignore_list}")
+    print("     FILE_A: "+file_a)
+    print("     FILE_B: "+file_b)
     with open(file_a) as fa, open(file_b) as fb:
         for index, (line_a, line_b) in enumerate(zip(fa, fb)):
             if index in ignore_list or any(word in line_a for word in ignore_list if isinstance(word, str)):
                 continue
             elif line_a != line_b:
                 return False
         return True
@@ -200,17 +203,18 @@
         atoms_b = [atom for atom in atoms_b if not atom.get_name().startswith('H')]
 
     print("     Atoms ALIGNED in PDB_A: "+str(len(atoms_a)))
     print("     Atoms ALIGNED in PDB_B: "+str(len(atoms_b)))
     super_imposer = Bio.PDB.Superimposer()
     super_imposer.set_atoms(atoms_a, atoms_b)
     super_imposer.apply(atoms_b)
-    print('     RMS: '+str(super_imposer.rms))
+    super_imposer_rms = super_imposer.rms if super_imposer.rms is not None else float('inf')
+    print('     RMS: '+str(super_imposer_rms))
     print('     RMS_CUTOFF: '+str(rmsd_cutoff))
-    return super_imposer.rms < rmsd_cutoff
+    return super_imposer_rms < rmsd_cutoff
 
 
 def compare_top_itp(file_a: str, file_b: str) -> bool:
     """ Compare top/itp files """
     print("Comparing TOP/ITP:")
     print("     FILE_A: "+file_a)
     print("     FILE_B: "+file_b)
@@ -261,15 +265,15 @@
         if not np.allclose(array_a, array_b, rtol=percent_tolerance / 100):
             return False
     return True
 
 
 def compare_images(file_a: str, file_b: str, percent_tolerance: float = 1.0) -> bool:
     try:
-        from PIL import Image
+        from PIL import Image  # type: ignore
         import imagehash
     except ImportError:
         print("To compare images, please install the following packages: Pillow, imagehash")
         return False
 
     """ Compare two files using size """
     print("Comparing images of both files:")
```

### Comparing `biobb_common-4.1.0/biobb_common.egg-info/PKG-INFO` & `biobb_common-4.2.0/biobb_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: biobb-common
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_common is the base package required to use the biobb packages.
 Home-page: https://github.com/bioexcel/biobb_common
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_common.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-common.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_common?label=Version)](https://GitHub.com/bioexcel/biobb_common/tags/)
 [![](https://img.shields.io/pypi/v/biobb-common.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-common/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_common?label=Conda)](https://anaconda.org/bioconda/biobb_common)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_common?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_common)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_common?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_common:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_common:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)]()
 [![](https://img.shields.io/pypi/pyversions/biobb-common.svg?label=Python%20Versions)]()
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)]()
 
 [![](https://readthedocs.org/projects/biobb-common/badge/?version=latest&label=Docs)](https://biobb-common.readthedocs.io/en/latest/?badge=latest)
@@ -50,22 +50,22 @@
 ### Introduction
 Biobb_common is the base package required to use the biobb
 packages.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_common.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-common.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.1
+v4.2.0 2024.1
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_common-4.1.0/biobb_common.egg-info/SOURCES.txt` & `biobb_common-4.2.0/biobb_common.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 biobb_common/__init__.py
+biobb_common/py.typed
 biobb_common.egg-info/PKG-INFO
 biobb_common.egg-info/SOURCES.txt
 biobb_common.egg-info/dependency_links.txt
 biobb_common.egg-info/requires.txt
 biobb_common.egg-info/top_level.txt
 biobb_common/command_wrapper/__init__.py
 biobb_common/command_wrapper/cmd_wrapper.py
```

### Comparing `biobb_common-4.1.0/setup.py` & `biobb_common-4.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_common",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_common is the base package required to use the biobb packages.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_common",
     project_urls={
-        "Documentation": "http://biobb_common.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-common.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/",
     },
     packages=setuptools.find_packages(exclude=["docs"]),
+    package_data={'biobb_common': ['py.typed']},
     install_requires=["pyyaml", "requests", "biopython"],
-    python_requires=">=3.8",
+    python_requires='>=3.8',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
-        "Operating System :: Unix",
+        "Operating System :: Unix"
     ],
 )
```

