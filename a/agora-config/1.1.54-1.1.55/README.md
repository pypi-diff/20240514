# Comparing `tmp/agora_config-1.1.54-py2.py3-none-any.whl.zip` & `tmp/agora_config-1.1.55-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9227 bytes, number of entries: 13
+Zip file size: 9225 bytes, number of entries: 13
 -rw-r--r--  2.0 fat       70 b- defN 23-Sep-06 12:54 agora_config/__init__.py
 -rw-r--r--  2.0 fat     7203 b- defN 24-Apr-23 15:18 agora_config/agora_config.py
 -rw-r--r--  2.0 fat      745 b- defN 23-Sep-06 12:54 agora_config/command_line_provider.py
 -rw-r--r--  2.0 fat     2600 b- defN 23-Sep-06 12:54 agora_config/dict_of_dict.py
 -rw-r--r--  2.0 fat      646 b- defN 23-Sep-06 12:54 agora_config/environment_variable_provider.py
 -rw-r--r--  2.0 fat     3644 b- defN 23-Sep-06 12:54 agora_config/file_key_provider.py
 -rw-r--r--  2.0 fat     2418 b- defN 23-Sep-06 12:54 agora_config/file_provider.py
 -rw-r--r--  2.0 fat     1099 b- defN 23-Sep-06 12:54 agora_config/last_value_callbacks.py
--rw-r--r--  2.0 fat       25 b- defN 24-May-13 17:00 agora_config/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.54.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.54.dist-info/WHEEL
--rw-r--r--  2.0 fat     1900 b- defN 16-Jan-01 00:00 agora_config-1.1.54.dist-info/METADATA
--rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.54.dist-info/RECORD
-13 files, 21690 bytes uncompressed, 7359 bytes compressed:  66.1%
+-rw-r--r--  2.0 fat       25 b- defN 24-May-14 10:55 agora_config/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.55.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.55.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1900 b- defN 16-Jan-01 00:00 agora_config-1.1.55.dist-info/METADATA
+-rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.55.dist-info/RECORD
+13 files, 21690 bytes uncompressed, 7357 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: agora_config/last_value_callbacks.py
 Comment: 
 
 Filename: agora_config/version.py
 Comment: 
 
-Filename: agora_config-1.1.54.dist-info/LICENSE
+Filename: agora_config-1.1.55.dist-info/LICENSE
 Comment: 
 
-Filename: agora_config-1.1.54.dist-info/WHEEL
+Filename: agora_config-1.1.55.dist-info/WHEEL
 Comment: 
 
-Filename: agora_config-1.1.54.dist-info/METADATA
+Filename: agora_config-1.1.55.dist-info/METADATA
 Comment: 
 
-Filename: agora_config-1.1.54.dist-info/RECORD
+Filename: agora_config-1.1.55.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_config/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.54'
+__version__ = '1.1.55'
```

## Comparing `agora_config-1.1.54.dist-info/METADATA` & `agora_config-1.1.55.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: agora_config
-Version: 1.1.54
+Version: 1.1.55
 Summary: Configuration libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.54
+Requires-Dist: agora_logging == 1.1.55
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_config
 
 This package is the Configuration library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
```

## Comparing `agora_config-1.1.54.dist-info/RECORD` & `agora_config-1.1.55.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 agora_config/agora_config.py,sha256=RoVr0AlxIGOCpwD7HAPB_d2SRLakeSFjZVyU7dg5kpU,7203
 agora_config/command_line_provider.py,sha256=ufrsQ-227QaO4oyjnxOR1HZWbYc9J78iu_OClhPBQ0A,745
 agora_config/dict_of_dict.py,sha256=2TDOYcb6bYn2wGkeRDENwNf8ylEJPbltQNuQCPg7m_o,2600
 agora_config/environment_variable_provider.py,sha256=V86CVODvwLKqetl6V7qwSLrnAGtYe7H__6v59lU3Lfk,646
 agora_config/file_key_provider.py,sha256=_FcCcc_nVnQlpHeORofOYVidPWHvkL_j_O6eyiv5d2Q,3644
 agora_config/file_provider.py,sha256=C859Nok0wLO3lH33xADH-1n7XYAu0VTcp1dEt3TZufs,2418
 agora_config/last_value_callbacks.py,sha256=IvCr6BVNMu8q9rqfmfeOy4I4hiZ73LC4epORXYzS3R0,1099
-agora_config/version.py,sha256=4WdBeM0yBfBzaTQBed8t9GEwEa64wGAS3T9tdCg7Q-g,25
-agora_config-1.1.54.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_config-1.1.54.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_config-1.1.54.dist-info/METADATA,sha256=DDRwhevXCdoLuSLprCrhjDhGGG5VOS74UYLh_O6TwHU,1900
-agora_config-1.1.54.dist-info/RECORD,,
+agora_config/version.py,sha256=UIT0aCiTGWEy2qWr4VqukZwUGe31Qh5aJKvW2JtVB1w,25
+agora_config-1.1.55.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_config-1.1.55.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_config-1.1.55.dist-info/METADATA,sha256=wEtLw4u39j26OkISv2gaD_QRx_tN7W9cCi8BB7WxhBg,1900
+agora_config-1.1.55.dist-info/RECORD,,
```

