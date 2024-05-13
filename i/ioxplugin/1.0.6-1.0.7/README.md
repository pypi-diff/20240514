# Comparing `tmp/ioxplugin-1.0.6.tar.gz` & `tmp/ioxplugin-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioxplugin-1.0.6.tar", last modified: Mon May 13 08:17:21 2024, max compression
+gzip compressed data, was "ioxplugin-1.0.7.tar", last modified: Mon May 13 09:07:25 2024, max compression
```

## Comparing `ioxplugin-1.0.6.tar` & `ioxplugin-1.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/ioxplugin/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/ast_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_controller_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_main_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_node_impl_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_to_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/iox_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/main_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/new_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/node_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/nodedef.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/oauth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/plugin_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/uom.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/ioxplugin/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/ioxplugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 08:17:21.000000 ioxplugin-1.0.6/ioxplugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:17:21.195151 ioxplugin-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 08:17:11.000000 ioxplugin-1.0.6/tests/test_ioxplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/ioxplugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56393 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/ast_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_controller_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_main_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_node_impl_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_to_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/iox_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/main_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/new_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/node_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/nodedef.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3014 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/oauth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/plugin_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/uom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/ioxplugin/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/ioxplugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 09:07:25.000000 ioxplugin-1.0.7/ioxplugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:07:25.038709 ioxplugin-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 09:07:14.000000 ioxplugin-1.0.7/tests/test_ioxplugin.py
```

### Comparing `ioxplugin-1.0.6/PKG-INFO` & `ioxplugin-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.6
+Version: 1.0.7
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.6/ioxplugin/__init__.py` & `ioxplugin-1.0.7/ioxplugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/ast_util.py` & `ioxplugin-1.0.7/ioxplugin/ast_util.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/commands.py` & `ioxplugin-1.0.7/ioxplugin/commands.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/editor.py` & `ioxplugin-1.0.7/ioxplugin/editor.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/iox_controller_template.py` & `ioxplugin-1.0.7/ioxplugin/iox_controller_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CONTROLLER_TEMPLATE_HEADER='''
 import udi_interface, os, sys, json, time
 from udi_interface import OAuth
 LOGGER = udi_interface.LOGGER
 Custom = udi_interface.Custom
 from ioxplugin import Plugin, OAuthService
 
+DATA_PATH='./data'
 '''
 
 #
 #from ModbusDeviceNode import ModbusDeviceNode
 #class ModbusControllerNode(udi_interface.Node):
 #   id = 'modbuscontroll'
 #    """This is a list of properties that were defined in the nodedef"""
@@ -31,15 +32,15 @@
 
 CONTROLLER_TEMPLATE_BODY='''
 
     def setProtocolHandler(self, protocolHandler):
         self.protocolHandler = protocolHandler
 
     def initOAuth(self):
-        if protocolHandler and protocolHandler.plugin and protocolHandler.plugin.meta and protocolHandler.plugin.meta.getEnableOAUTH2():
+        if self.protocolHandler and self.protocolHandler.plugin and self.protocolHandler.plugin.meta and self.protocolHandler.plugin.meta.getEnableOAUTH2():
             self.oauthService = OAuthService(self.polyglot)
 
     def parameter_handler(self, params):
         self.Parameters.load(params)
         return self.protocolHandler.processParams(self.Parameters)
 
     def configHandler(self, param):
@@ -56,15 +57,15 @@
 
     def start(self):
         LOGGER.info(f'Starting... ')
         self.poly.addNode(self)
         self.addAllNodes()
         self.poly.updateProfile()
         self.poly.setCustomParamsDoc()
-        self.updateStatus(1 if self.protocolHandler.start() else 0)
+        self.updateStatus(1 if self.protocolHandler.start() else 0, True)
         self.poly.ready()
         return True
 
     def stop(self):
         LOGGER.info(f'Stopping ... ')
         self.protocolHandler.stop()
         self.updateStatus(0)
```

### Comparing `ioxplugin-1.0.6/ioxplugin/iox_main_template.py` & `ioxplugin-1.0.7/ioxplugin/iox_main_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 LOGGER = udi_interface.LOGGER
 if __name__ == '__main__':
     try:
         polyglot = udi_interface.Interface([])
         polyglot.start(version.ud_plugin_version)
         plugin = None
         if not os.path.exists(PLUGIN_FILE_NAME):
-            polyglot.Notices[config]=f"{PLUGIN_FILE_NAME} does not exist. Uplaod it using file upload ..."
+            polyglot.Notices['config']=f"{PLUGIN_FILE_NAME} does not exist. Uplaod it using file upload ..."
         else:
             plugin = Plugin(PLUGIN_FILE_NAME)
             plugin.toIoX()
             plugin.generateCode(path='./')
         
         protocolHandler = __PROTOCOL_HANDLER_CLASS__(plugin)
         controller = __CONTROLLER_NODE_CLASS__(polyglot, protocolHandler)
+        protocolHandler.setController(controller)
         controller.start()
         polyglot.runForever()
     except (KeyboardInterrupt, SystemExit):
         LOGGER.info('exiting ...')
         sys(0)
 '''
```

### Comparing `ioxplugin-1.0.6/ioxplugin/iox_node_gen.py` & `ioxplugin-1.0.7/ioxplugin/iox_node_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/iox_profile.py` & `ioxplugin-1.0.7/ioxplugin/iox_profile.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/iox_to_modbus.py` & `ioxplugin-1.0.7/ioxplugin/iox_to_modbus.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/iox_transport.py` & `ioxplugin-1.0.7/ioxplugin/iox_transport.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/log.py` & `ioxplugin-1.0.7/ioxplugin/log.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/main_gen.py` & `ioxplugin-1.0.7/ioxplugin/main_gen.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/new_project.py` & `ioxplugin-1.0.7/ioxplugin/new_project.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/node_properties.py` & `ioxplugin-1.0.7/ioxplugin/node_properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/nodedef.py` & `ioxplugin-1.0.7/ioxplugin/nodedef.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/oauth_service.py` & `ioxplugin-1.0.7/ioxplugin/oauth_service.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/plugin.py` & `ioxplugin-1.0.7/ioxplugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/plugin_meta.py` & `ioxplugin-1.0.7/ioxplugin/plugin_meta.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/properties.py` & `ioxplugin-1.0.7/ioxplugin/properties.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/protocol.py` & `ioxplugin-1.0.7/ioxplugin/protocol.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/uom.py` & `ioxplugin-1.0.7/ioxplugin/uom.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin/validator.py` & `ioxplugin-1.0.7/ioxplugin/validator.py`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/ioxplugin.egg-info/PKG-INFO` & `ioxplugin-1.0.7/ioxplugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioxplugin
-Version: 1.0.6
+Version: 1.0.7
 Summary: IoX Plugin Helper Package
 Home-page: https://github.com/universaldevices/ioxplugin.git
 Author: Michel Kohanim
 Author-email: support@universal-devices.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ioxplugin-1.0.6/ioxplugin.egg-info/SOURCES.txt` & `ioxplugin-1.0.7/ioxplugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ioxplugin-1.0.6/setup.py` & `ioxplugin-1.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ioxplugin',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     description='IoX Plugin Helper Package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Michel Kohanim',
     author_email='support@universal-devices.com',
     url='https://github.com/universaldevices/ioxplugin.git',
```

