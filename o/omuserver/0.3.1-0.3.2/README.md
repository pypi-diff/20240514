# Comparing `tmp/omuserver-0.3.1.tar.gz` & `tmp/omuserver-0.3.2.tar.gz`

## Comparing `omuserver-0.3.1.tar` & `omuserver-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/__init__.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/__main__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/config.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/directories.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/helper.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/version.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/extension.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/asset/__init__.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/asset/asset_extension.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/asset/permissions.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/dashboard/permission.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/i18n/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/i18n/i18n_extension.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/i18n/permissions.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/permission/__init__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/permission/permission_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/plugin/plugin_connection.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/plugin/plugin_loader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/plugin/plugin_session_connection.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/registry/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/registry/registry.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/registry/registry_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/server/__init__.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/server/server_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/signal/__init__.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/signal/signal_extension.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/__init__.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/cached_table.py
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/serialized_table.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/server_table.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/session_table_handler.py
--rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/table_extension.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/adapters/__init__.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/adapters/sqlitetable.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/extension/table/adapters/tableadapter.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/network/__init__.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/network/network.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/network/packet_dispatcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/security/__init__.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/security/security.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/server/__init__.py
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/server/omuserver.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/server/server.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/session/__init__.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/session/aiohttp_connection.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 omuserver-0.3.1/src/omuserver/session/session.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.3.1/test/helper_test.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuserver-0.3.1/.gitignore
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.3.1/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 omuserver-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuserver-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/__init__.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/__main__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/config.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/directories.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/helper.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/version.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/extension.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/asset/__init__.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/asset/permissions.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/dashboard/permission.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/i18n/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/i18n/i18n_extension.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/i18n/permissions.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/permission/__init__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_connection.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_loader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/plugin/plugin_session_connection.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/registry/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/registry/registry.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/server/__init__.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/server/permissions.py
+-rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/server/server_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/signal/__init__.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/signal/signal_extension.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/__init__.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/cached_table.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/serialized_table.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/server_table.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/session_table_handler.py
+-rw-r--r--   0        0        0    10604 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/table_extension.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/adapters/__init__.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/adapters/sqlitetable.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/extension/table/adapters/tableadapter.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/network/__init__.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/network/network.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/network/packet_dispatcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/security/__init__.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/security/security.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/server/__init__.py
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/server/omuserver.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/server/server.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/session/__init__.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/session/aiohttp_connection.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 omuserver-0.3.2/src/omuserver/session/session.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.3.2/test/helper_test.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuserver-0.3.2/.gitignore
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.3.2/README.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 omuserver-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 omuserver-0.3.2/PKG-INFO
```

### Comparing `omuserver-0.3.1/src/omuserver/__main__.py` & `omuserver-0.3.2/src/omuserver/__main__.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/directories.py` & `omuserver-0.3.2/src/omuserver/directories.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/helper.py` & `omuserver-0.3.2/src/omuserver/helper.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/asset/asset_extension.py` & `omuserver-0.3.2/src/omuserver/extension/asset/asset_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/asset/permissions.py` & `omuserver-0.3.2/src/omuserver/extension/asset/permissions.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/dashboard/dashboard_extension.py` & `omuserver-0.3.2/src/omuserver/extension/dashboard/dashboard_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/dashboard/permission.py` & `omuserver-0.3.2/src/omuserver/extension/dashboard/permission.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/endpoint/endpoint_extension.py` & `omuserver-0.3.2/src/omuserver/extension/endpoint/endpoint_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/i18n/permissions.py` & `omuserver-0.3.2/src/omuserver/extension/i18n/permissions.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/permission/permission_extension.py` & `omuserver-0.3.2/src/omuserver/extension/permission/permission_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/plugin/plugin_connection.py` & `omuserver-0.3.2/src/omuserver/extension/plugin/plugin_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/plugin/plugin_extension.py` & `omuserver-0.3.2/src/omuserver/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/plugin/plugin_loader.py` & `omuserver-0.3.2/src/omuserver/extension/plugin/plugin_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,22 +134,16 @@
         )
 
 
 class PluginLoader:
     def __init__(self, server: Server) -> None:
         self._server = server
         self.plugins: dict[str, Plugin] = {}
-        server.event.start += self.handle_server_start
         server.event.stop += self.handle_server_stop
 
-    async def handle_server_start(self) -> None:
-        for plugin in self.plugins.values():
-            if plugin.on_start_server is not None:
-                await plugin.on_start_server(self._server)
-
     async def handle_server_stop(self) -> None:
         for plugin in self.plugins.values():
             if plugin.on_stop_server is not None:
                 await plugin.on_stop_server(self._server)
 
     async def run_plugins(self):
         entry_points = importlib.metadata.entry_points(group=PLUGIN_GROUP)
@@ -157,14 +151,20 @@
             if entry_point.dist is None:
                 raise ValueError(f"Invalid plugin: {entry_point} has no distribution")
             plugin_key = entry_point.dist.name
             if plugin_key in self.plugins:
                 raise ValueError(f"Duplicate plugin: {entry_point}")
             plugin = self.load_plugin_from_entry_point(entry_point)
             self.plugins[plugin_key] = plugin
+
+        for plugin in self.plugins.values():
+            if plugin.on_start_server is not None:
+                await plugin.on_start_server(self._server)
+
+        for plugin in self.plugins.values():
             await self.run_plugin(plugin)
 
     async def load_updated_plugins(self):
         entry_points = importlib.metadata.entry_points(group=PLUGIN_GROUP)
         for entry_point in entry_points:
             if entry_point.dist is None:
                 raise ValueError(f"Invalid plugin: {entry_point} has no distribution")
```

### Comparing `omuserver-0.3.1/src/omuserver/extension/plugin/plugin_session_connection.py` & `omuserver-0.3.2/src/omuserver/extension/plugin/plugin_session_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/registry/registry.py` & `omuserver-0.3.2/src/omuserver/extension/registry/registry.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/registry/registry_extension.py` & `omuserver-0.3.2/src/omuserver/extension/registry/registry_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/signal/signal_extension.py` & `omuserver-0.3.2/src/omuserver/extension/signal/signal_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/table/cached_table.py` & `omuserver-0.3.2/src/omuserver/extension/table/cached_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/table/serialized_table.py` & `omuserver-0.3.2/src/omuserver/extension/table/serialized_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/table/server_table.py` & `omuserver-0.3.2/src/omuserver/extension/table/server_table.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/table/session_table_handler.py` & `omuserver-0.3.2/src/omuserver/extension/table/session_table_handler.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/table/table_extension.py` & `omuserver-0.3.2/src/omuserver/extension/table/table_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/table/adapters/sqlitetable.py` & `omuserver-0.3.2/src/omuserver/extension/table/adapters/sqlitetable.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/extension/table/adapters/tableadapter.py` & `omuserver-0.3.2/src/omuserver/extension/table/adapters/tableadapter.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/network/network.py` & `omuserver-0.3.2/src/omuserver/network/network.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/network/packet_dispatcher.py` & `omuserver-0.3.2/src/omuserver/network/packet_dispatcher.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/security/security.py` & `omuserver-0.3.2/src/omuserver/security/security.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/server/omuserver.py` & `omuserver-0.3.2/src/omuserver/server/omuserver.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/server/server.py` & `omuserver-0.3.2/src/omuserver/server/server.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/session/aiohttp_connection.py` & `omuserver-0.3.2/src/omuserver/session/aiohttp_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/src/omuserver/session/session.py` & `omuserver-0.3.2/src/omuserver/session/session.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.3.1/pyproject.toml` & `omuserver-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuserver"
-version = "0.3.1"
+version = "0.3.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "loguru>=0.7.2",
     "aiohttp>=3.9.3",
```

### Comparing `omuserver-0.3.1/PKG-INFO` & `omuserver-0.3.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omuserver
-Version: 0.3.1
+Version: 0.3.2
 Summary: Add your description here
 Author-email: am230 <111672334+am230@users.noreply.github.com>
 Requires-Python: >=3.12
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: click>=8.1.7
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: omu>=0.1.4
```

