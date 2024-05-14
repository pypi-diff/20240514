# Comparing `tmp/fotoobo-2.1.0.tar.gz` & `tmp/fotoobo-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fotoobo-2.1.0.tar", max compression
+gzip compressed data, was "fotoobo-2.1.1.tar", max compression
```

## Comparing `fotoobo-2.1.0.tar` & `fotoobo-2.1.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     7633 2024-03-05 10:07:56.226528 fotoobo-2.1.0/LICENSE
--rw-r--r--   0        0        0     2574 2024-03-05 10:07:56.226528 fotoobo-2.1.0/README.md
--rw-r--r--   0        0        0      409 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/__init__.py
--rw-r--r--   0        0        0      195 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/__init__.py
--rw-r--r--   0        0        0     1805 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/convert.py
--rw-r--r--   0        0        0       20 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/ems/__init__.py
--rw-r--r--   0        0        0     1478 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/ems/get_commands.py
--rw-r--r--   0        0        0      774 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/ems/main.py
--rw-r--r--   0        0        0    11043 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/ems/monitor_commands.py
--rw-r--r--   0        0        0       20 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/faz/__init__.py
--rw-r--r--   0        0        0      966 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/faz/get_commands.py
--rw-r--r--   0        0        0      629 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/faz/main.py
--rw-r--r--   0        0        0       20 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/fgt/__init__.py
--rw-r--r--   0        0        0     2829 2024-03-05 10:07:56.230528 fotoobo-2.1.0/fotoobo/cli/fgt/config_commands.py
--rw-r--r--   0        0        0     1230 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/fgt/get_commands.py
--rw-r--r--   0        0        0     3535 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/fgt/main.py
--rw-r--r--   0        0        0     3893 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/fgt/monitor_commands.py
--rw-r--r--   0        0        0       20 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/fmg/__init__.py
--rw-r--r--   0        0        0     3161 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/fmg/get_commands.py
--rw-r--r--   0        0        0     3519 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/fmg/main.py
--rw-r--r--   0        0        0     1789 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/get.py
--rw-r--r--   0        0        0     5301 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/cli/main.py
--rw-r--r--   0        0        0      196 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/exceptions/__init__.py
--rw-r--r--   0        0        0     1963 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/exceptions/exceptions.py
--rw-r--r--   0        0        0      423 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/__init__.py
--rw-r--r--   0        0        0    13882 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/convert.py
--rw-r--r--   0        0        0     1007 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/fortianalyzer.py
--rw-r--r--   0        0        0     6756 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/forticlientems.py
--rw-r--r--   0        0        0     3010 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/fortigate.py
--rw-r--r--   0        0        0    11340 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/fortigate_config.py
--rw-r--r--   0        0        0     8666 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/fortigate_config_check.py
--rw-r--r--   0        0        0      584 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/fortigate_info.py
--rw-r--r--   0        0        0    12633 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/fortimanager.py
--rw-r--r--   0        0        0     6726 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/fortinet/fortinet.py
--rw-r--r--   0        0        0      310 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/__init__.py
--rw-r--r--   0        0        0     1218 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/cli.py
--rw-r--r--   0        0        0     4680 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/config.py
--rw-r--r--   0        0        0     5339 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/files.py
--rw-r--r--   0        0        0    10815 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/log.py
--rw-r--r--   0        0        0     4977 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/output.py
--rw-r--r--   0        0        0    10251 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/result.py
--rw-r--r--   0        0        0     8459 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/helpers/vault.py
--rw-r--r--   0        0        0      126 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/inventory/__init__.py
--rw-r--r--   0        0        0      586 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/inventory/generic.py
--rw-r--r--   0        0        0     8309 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/inventory/inventory.py
--rwxr-xr-x   0        0        0     1361 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/main.py
--rw-r--r--   0        0        0      427 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/__init__.py
--rw-r--r--   0        0        0     1274 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/convert.py
--rw-r--r--   0        0        0       91 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/ems/__init__.py
--rw-r--r--   0        0        0     1556 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/ems/get.py
--rw-r--r--   0        0        0     8376 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/ems/monitor.py
--rw-r--r--   0        0        0       55 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/faz/__init__.py
--rw-r--r--   0        0        0      786 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/faz/get.py
--rw-r--r--   0        0        0      128 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fgt/__init__.py
--rw-r--r--   0        0        0     4573 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fgt/config.py
--rw-r--r--   0        0        0     2370 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fgt/get.py
--rw-r--r--   0        0        0     2967 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fgt/main.py
--rw-r--r--   0        0        0     4266 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fgt/monitor.py
--rw-r--r--   0        0        0      105 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fmg/__init__.py
--rw-r--r--   0        0        0     4626 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fmg/get.py
--rw-r--r--   0        0        0     3094 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/fmg/main.py
--rw-r--r--   0        0        0     1900 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/get.py
--rw-r--r--   0        0        0     1368 2024-03-05 10:07:56.234528 fotoobo-2.1.0/fotoobo/tools/greet.py
--rw-r--r--   0        0        0     4592 2024-03-05 10:07:56.234528 fotoobo-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 fotoobo-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2024-05-14 11:39:59.727291 fotoobo-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2574 2024-05-14 11:39:59.727291 fotoobo-2.1.1/README.md
+-rw-r--r--   0        0        0      409 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/__init__.py
+-rw-r--r--   0        0        0     1806 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/convert.py
+-rw-r--r--   0        0        0       20 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/ems/__init__.py
+-rw-r--r--   0        0        0     1479 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/ems/get_commands.py
+-rw-r--r--   0        0        0      775 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/ems/main.py
+-rw-r--r--   0        0        0    11044 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/ems/monitor_commands.py
+-rw-r--r--   0        0        0       20 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/faz/__init__.py
+-rw-r--r--   0        0        0      967 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/faz/get_commands.py
+-rw-r--r--   0        0        0      630 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/faz/main.py
+-rw-r--r--   0        0        0       20 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fgt/__init__.py
+-rw-r--r--   0        0        0     2829 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fgt/config_commands.py
+-rw-r--r--   0        0        0     1231 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fgt/get_commands.py
+-rw-r--r--   0        0        0     3536 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fgt/main.py
+-rw-r--r--   0        0        0     3894 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fgt/monitor_commands.py
+-rw-r--r--   0        0        0       20 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fmg/__init__.py
+-rw-r--r--   0        0        0     3162 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fmg/get_commands.py
+-rw-r--r--   0        0        0     3520 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/fmg/main.py
+-rw-r--r--   0        0        0     1790 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/get.py
+-rw-r--r--   0        0        0     5301 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/cli/main.py
+-rw-r--r--   0        0        0      196 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/exceptions/__init__.py
+-rw-r--r--   0        0        0     1964 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/exceptions/exceptions.py
+-rw-r--r--   0        0        0      423 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/__init__.py
+-rw-r--r--   0        0        0    13883 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/convert.py
+-rw-r--r--   0        0        0     1008 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/fortianalyzer.py
+-rw-r--r--   0        0        0     6756 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/forticlientems.py
+-rw-r--r--   0        0        0     3011 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/fortigate.py
+-rw-r--r--   0        0        0    11341 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/fortigate_config.py
+-rw-r--r--   0        0        0     8667 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/fortigate_config_check.py
+-rw-r--r--   0        0        0      585 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/fortigate_info.py
+-rw-r--r--   0        0        0    12634 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/fortimanager.py
+-rw-r--r--   0        0        0     6726 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/fortinet/fortinet.py
+-rw-r--r--   0        0        0      310 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/helpers/__init__.py
+-rw-r--r--   0        0        0     1218 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/helpers/cli.py
+-rw-r--r--   0        0        0     4681 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/helpers/config.py
+-rw-r--r--   0        0        0     5340 2024-05-14 11:39:59.731291 fotoobo-2.1.1/fotoobo/helpers/files.py
+-rw-r--r--   0        0        0    10976 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/helpers/log.py
+-rw-r--r--   0        0        0     4978 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/helpers/output.py
+-rw-r--r--   0        0        0    10251 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/helpers/result.py
+-rw-r--r--   0        0        0     8459 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/helpers/vault.py
+-rw-r--r--   0        0        0      127 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/inventory/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/inventory/generic.py
+-rw-r--r--   0        0        0     8310 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/inventory/inventory.py
+-rwxr-xr-x   0        0        0     1362 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/main.py
+-rw-r--r--   0        0        0      428 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/__init__.py
+-rw-r--r--   0        0        0     1275 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/convert.py
+-rw-r--r--   0        0        0       92 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/ems/__init__.py
+-rw-r--r--   0        0        0     1557 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/ems/get.py
+-rw-r--r--   0        0        0     8377 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/ems/monitor.py
+-rw-r--r--   0        0        0       56 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/faz/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/faz/get.py
+-rw-r--r--   0        0        0      129 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fgt/__init__.py
+-rw-r--r--   0        0        0     4574 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fgt/config.py
+-rw-r--r--   0        0        0     2371 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fgt/get.py
+-rw-r--r--   0        0        0     2968 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fgt/main.py
+-rw-r--r--   0        0        0     4267 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fgt/monitor.py
+-rw-r--r--   0        0        0      105 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fmg/__init__.py
+-rw-r--r--   0        0        0     4627 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fmg/get.py
+-rw-r--r--   0        0        0     3095 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/fmg/main.py
+-rw-r--r--   0        0        0     1901 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/get.py
+-rw-r--r--   0        0        0     1369 2024-05-14 11:39:59.735291 fotoobo-2.1.1/fotoobo/tools/greet.py
+-rw-r--r--   0        0        0     4591 2024-05-14 11:39:59.735291 fotoobo-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4260 1970-01-01 00:00:00.000000 fotoobo-2.1.1/PKG-INFO
```

### Comparing `fotoobo-2.1.0/LICENSE` & `fotoobo-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/README.md` & `fotoobo-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/cli/convert.py` & `fotoobo-2.1.1/fotoobo/cli/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The fotoobo convert commands
 """
+
 import logging
 from pathlib import Path
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.helpers.files import load_json_file, save_json_file
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/ems/get_commands.py` & `fotoobo-2.1.1/fotoobo/cli/ems/get_commands.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiClient EMS get commands
 """
+
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.tools import ems
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/ems/main.py` & `fotoobo-2.1.1/fotoobo/cli/ems/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiClient EMS commands
 """
+
 import logging
 
 import typer
 
 from fotoobo.cli.ems import get_commands as get
 from fotoobo.cli.ems import monitor_commands as monitor
 from fotoobo.helpers import cli_path
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/ems/monitor_commands.py` & `fotoobo-2.1.1/fotoobo/cli/ems/monitor_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiClient EMS monitor commands
 """
+
 import logging
 from pathlib import Path
 from typing import Optional, Union
 
 import typer
 
 from fotoobo.helpers import cli_path
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/faz/get_commands.py` & `fotoobo-2.1.1/fotoobo/cli/faz/get_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiAnalyzer get commands
 """
+
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.tools import faz
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/faz/main.py` & `fotoobo-2.1.1/fotoobo/cli/faz/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiAnalyzer commands
 """
+
 import logging
 
 import typer
 
 from fotoobo.cli.faz import get_commands as get
 from fotoobo.helpers import cli_path
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/fgt/config_commands.py` & `fotoobo-2.1.1/fotoobo/cli/fgt/config_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/cli/fgt/get_commands.py` & `fotoobo-2.1.1/fotoobo/cli/fgt/get_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiGate get commands
 """
+
 # pylint: disable=anomalous-backslash-in-string
 import logging
 
 import typer
 
 from fotoobo.helpers import cli_path
 from fotoobo.tools import fgt
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/fgt/main.py` & `fotoobo-2.1.1/fotoobo/cli/fgt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiGate commands
 """
+
 import logging
 import os
 from datetime import datetime
 from pathlib import Path
 
 import typer
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/fgt/monitor_commands.py` & `fotoobo-2.1.1/fotoobo/cli/fgt/monitor_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiGate check commands
 """
+
 import logging
 from pathlib import Path
 from typing import Dict, Optional
 
 import typer
 from rich.pretty import pprint
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/fmg/get_commands.py` & `fotoobo-2.1.1/fotoobo/cli/fmg/get_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiManager get commands
 """
+
 import logging
 from pathlib import Path
 from typing import Dict, List, Union
 
 import typer
 
 from fotoobo.helpers import cli_path
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/fmg/main.py` & `fotoobo-2.1.1/fotoobo/cli/fmg/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiManager commands
 """
+
 import logging
 from pathlib import Path
 
 import typer
 
 from fotoobo.cli.fmg import get_commands as get
 from fotoobo.helpers import cli_path
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/get.py` & `fotoobo-2.1.1/fotoobo/cli/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The fotoobo get commands
 """
+
 import logging
 
 import typer
 from rich import print as rich_print
 from rich.panel import Panel
 
 from fotoobo.helpers import cli_path
```

### Comparing `fotoobo-2.1.0/fotoobo/cli/main.py` & `fotoobo-2.1.1/fotoobo/cli/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/exceptions/exceptions.py` & `fotoobo-2.1.1/fotoobo/exceptions/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This is the fotoobo exception module.
 """
+
 from typing import Any
 
 from requests.exceptions import HTTPError
 
 
 class GeneralException(Exception):
     """
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/convert.py` & `fotoobo-2.1.1/fotoobo/fortinet/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Please refer to docs_legacy/convert_checkpoint_mappings.drawio.svg to see how a Checkpoint asset is
 going to be converted into a Fortinet asset.
 
 The Fortinet assets are referenced by their names. Even if we set an uuid we cannot use the uuid to
 access the asset. The uuid is only supported for network assets and not for service assets.
 """
+
 import copy
 import logging
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from fotoobo.exceptions import GeneralError
 from fotoobo.helpers.files import load_json_file, save_json_file
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/fortianalyzer.py` & `fotoobo-2.1.1/fotoobo/fortinet/fortianalyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiAnalyzer Class
 """
+
 import logging
 from typing import Any
 
 from .fortimanager import FortiManager
 
 log = logging.getLogger("fotoobo")
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/forticlientems.py` & `fotoobo-2.1.1/fotoobo/fortinet/forticlientems.py`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/fortigate.py` & `fotoobo-2.1.1/fotoobo/fortinet/fortigate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiGate Class
 """
+
 import logging
 from typing import Any, Dict, Optional
 
 import requests
 
 from fotoobo.exceptions import APIError, GeneralWarning
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/fortigate_config.py` & `fotoobo-2.1.1/fotoobo/fortinet/fortigate_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiGate configuration class represents the whole or parts of a FortiGate configuration
 """
+
 import logging
 from pathlib import Path
 from typing import IO, Any, Dict, List, Optional
 
 from fotoobo.exceptions import GeneralWarning
 from fotoobo.helpers.files import load_json_file, save_json_file
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/fortigate_config_check.py` & `fotoobo-2.1.1/fotoobo/fortinet/fortigate_config_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiGate configuration checker
 """
+
 import logging
 from typing import Any, Dict, List
 
 from fotoobo.exceptions import GeneralError
 from fotoobo.fortinet.fortigate_config import FortiGateConfig
 from fotoobo.helpers.result import Result
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/fortigate_info.py` & `fotoobo-2.1.1/fotoobo/fortinet/fortigate_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The FortiGateInfo class
 """
+
 from dataclasses import dataclass
 
 
 @dataclass(eq=False, order=False)
 class FortiGateInfo:
     """
     This dataclass holds FortiGate meta information from the configuration file.
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/fortimanager.py` & `fotoobo-2.1.1/fotoobo/fortinet/fortimanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiManager Class
 """
+
 import logging
 import re
 from pathlib import Path
 from time import sleep
 from typing import Any, Dict, List, Optional
 
 import requests
```

### Comparing `fotoobo-2.1.0/fotoobo/fortinet/fortinet.py` & `fotoobo-2.1.1/fotoobo/fortinet/fortinet.py`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/helpers/cli.py` & `fotoobo-2.1.1/fotoobo/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/helpers/config.py` & `fotoobo-2.1.1/fotoobo/helpers/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The config helper is used to load and set basic configuration for fotoobo. Some configuration
 options may be set by the global configuration file which by default points to fotoobo.yaml in the
 local directory. Some configuration options may be set by command line parameters as described in
 the cli help system.
 If there are configuration options available in the global configuration file and also as a command
 line option, the command line option takes precedence over the global configuration file option.
 """
+
 import os
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 from fotoobo.exceptions import GeneralError
 from fotoobo.helpers.files import load_yaml_file
```

### Comparing `fotoobo-2.1.0/fotoobo/helpers/files.py` & `fotoobo-2.1.1/fotoobo/helpers/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Some helper functions for file manipulation.
 """
+
 import json
 import logging
 import re
 from ftplib import FTP, FTP_TLS
 from pathlib import Path
 from typing import Any, Dict, List, Union
 from zipfile import ZIP_DEFLATED, ZipFile
```

### Comparing `fotoobo-2.1.0/fotoobo/helpers/log.py` & `fotoobo-2.1.1/fotoobo/helpers/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 The logging helper class is used if you want to write logs to the screen or a file. It is set up
 to do pretty printing screen output with rich and writing "normal" text to a logfile.
 Basic logging options can be configured in the main configuration file. See config_helper.py
 """
+
 import logging
 import logging.config
 import os
 import pwd
 import socket
 from datetime import datetime
 from logging.handlers import RotatingFileHandler, SysLogHandler
@@ -215,17 +216,19 @@
                     if "log_syslog" in config.logging:
                         try:
                             syslog_handler = SysLogHandler(
                                 address=(
                                     config.logging["log_syslog"]["host"],
                                     int(config.logging["log_syslog"]["port"]),
                                 ),
-                                socktype=socket.SOCK_STREAM
-                                if config.logging["log_syslog"]["protocol"] == "TCP"
-                                else socket.SOCK_DGRAM,
+                                socktype=(
+                                    socket.SOCK_STREAM
+                                    if config.logging["log_syslog"]["protocol"] == "TCP"
+                                    else socket.SOCK_DGRAM
+                                ),
                             )
 
                         except (OSError, socket.gaierror) as error:
                             raise GeneralError(
                                 f"Cannot configure SysLog logging: {str(error)}"
                             ) from error
 
@@ -252,17 +255,19 @@
                         try:
                             audit_syslog_handler = SysLogHandler(
                                 address=(
                                     config.audit_logging["log_syslog"]["host"],
                                     int(config.audit_logging["log_syslog"]["port"]),
                                 ),
                                 facility=LOG_AUTH,
-                                socktype=socket.SOCK_STREAM
-                                if config.audit_logging["log_syslog"]["protocol"] == "TCP"
-                                else socket.SOCK_DGRAM,
+                                socktype=(
+                                    socket.SOCK_STREAM
+                                    if config.audit_logging["log_syslog"]["protocol"] == "TCP"
+                                    else socket.SOCK_DGRAM
+                                ),
                             )
 
                         except (OSError, socket.gaierror) as error:
                             raise GeneralError(
                                 f"Cannot configure SysLog logging: {str(error)}"
                             ) from error
```

### Comparing `fotoobo-2.1.0/fotoobo/helpers/output.py` & `fotoobo-2.1.1/fotoobo/helpers/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The beautiful output helper
 """
+
 import os
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, List
 
 from rich.console import Console
```

### Comparing `fotoobo-2.1.0/fotoobo/helpers/result.py` & `fotoobo-2.1.1/fotoobo/helpers/result.py`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/helpers/vault.py` & `fotoobo-2.1.1/fotoobo/helpers/vault.py`

 * *Files identical despite different names*

### Comparing `fotoobo-2.1.0/fotoobo/inventory/generic.py` & `fotoobo-2.1.1/fotoobo/inventory/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A module for defining a generic device
 """
+
 from typing import Union
 
 
 class GenericDevice:
     """
     This is the class for a generic device.
```

### Comparing `fotoobo-2.1.0/fotoobo/inventory/inventory.py` & `fotoobo-2.1.1/fotoobo/inventory/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Devices class for storing device information
 """
+
 import logging
 import re
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 from fotoobo.exceptions import GeneralWarning
 from fotoobo.fortinet.fortianalyzer import FortiAnalyzer
```

### Comparing `fotoobo-2.1.0/fotoobo/main.py` & `fotoobo-2.1.1/fotoobo/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 The second task is to catch all exceptions and print a friendly message on the screen instead of
 a traceback. The traceback is written to a traceback.log file in the local directory for debug
 purposes.
 
 The exceptions in the main functions cannot be tested because the test-method for typer always
 exits with its own exit codes (1 or 2) when an exception rises.
 """
+
 import sys
 import traceback
 
 from fotoobo.cli.main import app
 from fotoobo.exceptions import APIError, GeneralError, GeneralWarning
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/convert.py` & `fotoobo-2.1.1/fotoobo/tools/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The fotoobo converter utility
 """
+
 import logging
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from fotoobo.fortinet.convert import CheckpointConverter
 from fotoobo.helpers.files import create_dir
 from fotoobo.helpers.result import Result
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/ems/get.py` & `fotoobo-2.1.1/fotoobo/tools/ems/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiClient EMS get module
 """
+
 import logging
 from typing import Dict, List
 
 from fotoobo.fortinet.forticlientems import FortiClientEMS
 from fotoobo.helpers.config import config
 from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/ems/monitor.py` & `fotoobo-2.1.1/fotoobo/tools/ems/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiClient EMS monitor module
 """
+
 import logging
 from datetime import datetime
 from typing import Any, Dict
 
 from fotoobo.fortinet.forticlientems import FortiClientEMS
 from fotoobo.helpers.config import config
 from fotoobo.helpers.result import Result
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/faz/get.py` & `fotoobo-2.1.1/fotoobo/tools/faz/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiAnalyzer get version utility
 """
+
 import logging
 
 from fotoobo.helpers.config import config
 from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/fgt/config.py` & `fotoobo-2.1.1/fotoobo/tools/fgt/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiGate configuration check utility
 """
+
 import logging
 from pathlib import Path
 from typing import Any, List
 
 import typer
 
 from fotoobo.exceptions import GeneralError, GeneralWarning
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/fgt/get.py` & `fotoobo-2.1.1/fotoobo/tools/fgt/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiGate get version utility
 """
+
 import concurrent.futures
 import logging
 from typing import Optional, Tuple
 
 from rich.progress import Progress
 
 from fotoobo.exceptions import GeneralError, GeneralWarning
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/fgt/main.py` & `fotoobo-2.1.1/fotoobo/tools/fgt/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiGate backup utility
 """
+
 import concurrent.futures
 import json
 import logging
 from typing import Optional, Tuple
 
 from rich.progress import Progress
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/fgt/monitor.py` & `fotoobo-2.1.1/fotoobo/tools/fgt/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiGate check hamaster utility
 """
+
 import concurrent.futures
 import logging
 from typing import Dict, Tuple
 
 from rich.progress import Progress
 
 from fotoobo.fortinet.fortigate import FortiGate
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/fmg/get.py` & `fotoobo-2.1.1/fotoobo/tools/fmg/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiManager get ADOMs utility
 """
+
 import logging
 from typing import Any, Dict, List, Optional, Union
 
 from fotoobo.exceptions.exceptions import GeneralError
 from fotoobo.helpers.config import config
 from fotoobo.helpers.result import Result
 from fotoobo.inventory import Inventory
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/fmg/main.py` & `fotoobo-2.1.1/fotoobo/tools/fmg/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 FortiManager assign utility
 """
+
 import logging
 from pathlib import Path
 
 from fotoobo.exceptions.exceptions import GeneralWarning
 from fotoobo.helpers.config import config
 from fotoobo.helpers.files import load_json_file
 from fotoobo.helpers.result import Result
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/get.py` & `fotoobo-2.1.1/fotoobo/tools/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The fotoobo get utility
 """
+
 import importlib.metadata
 import logging
 from typing import Dict, List
 
 from rich.text import Text
 from rich.tree import Tree
```

### Comparing `fotoobo-2.1.0/fotoobo/tools/greet.py` & `fotoobo-2.1.1/fotoobo/tools/greet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The fotoobo greeting utility
 
 This function is a hidden fotoobo command which is meant for testing purposes. It has no functional
 effect. Use and modify it whenever you want. But be sure to also write the tests for it.
 """
+
 import logging
 
 import typer
 
 log = logging.getLogger("fotoobo")
```

### Comparing `fotoobo-2.1.0/pyproject.toml` & `fotoobo-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fotoobo"
-version = "2.1.0"
+version = "2.1.1"
 description = "The awesome Fortinet Toolbox"
 authors = ["Patrik Spiess <patrik.spiess@mgb.ch>", "Lukas Murer-Jäckle <lukas.murer@mgb.ch>"]
 readme = "README.md"
 license = "LGPL-3.0-only"
 repository = "https://github.com/migros/fotoobo"
 classifiers = [
     "Framework :: Pytest",
@@ -39,22 +39,22 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.13"
 typer = "~0.6.0"
 rich = "~12.5.1"
 PyYAML = "~6.0.0"
 requests = "~2.31.0"
-Jinja2 = "~3.1.2"
+Jinja2 = "~3.1.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "~7.2.0"
-black = "~22.10.0"
+black = "~24.03.0"
 mypy = ">0.9, <1.0"
 tox = "~4.4.0"
-pylint = "~2.15.0"
+pylint = "~3.1.0"
 pytest-cov = "~4.0.0"
 types-requests = "~2.27.11"
 isort = "~5.10.1"
 types-PyYAML = "~6.0.5"
 pygount = "~1.5.0"
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `fotoobo-2.1.0/PKG-INFO` & `fotoobo-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fotoobo
-Version: 2.1.0
+Version: 2.1.1
 Summary: The awesome Fortinet Toolbox
 Home-page: https://github.com/migros/fotoobo
 License: LGPL-3.0-only
 Author: Patrik Spiess
 Author-email: patrik.spiess@mgb.ch
 Requires-Python: >=3.8.0,<3.13
 Classifier: Framework :: Pytest
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: Jinja2 (>=3.1.2,<3.2.0)
+Requires-Dist: Jinja2 (>=3.1.4,<3.2.0)
 Requires-Dist: PyYAML (>=6.0.0,<6.1.0)
 Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: rich (>=12.5.1,<12.6.0)
 Requires-Dist: typer (>=0.6.0,<0.7.0)
 Project-URL: Repository, https://github.com/migros/fotoobo
 Description-Content-Type: text/markdown
```

