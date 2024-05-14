# Comparing `tmp/omu-0.3.1.tar.gz` & `tmp/omu-0.3.2.tar.gz`

## Comparing `omu-0.3.1.tar` & `omu-0.3.2.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/address.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/app.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/bytebuffer.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/errors.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/event_emitter.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/helper.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/identifier.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/model.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/plugin.py
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/serializer.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/version.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/client/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/client/client.py
--rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/client/omuclient.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/client/token.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/extension.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/extension_registry.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/asset/__init__.py
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/asset/asset_extension.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/dashboard/packets.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/endpoint/endpoint.py
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/endpoint/packets.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/i18n/__init__.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/i18n/i18n_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/permission/__init__.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/permission/permission.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/permission/permission_extension.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/plugin/package_info.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/plugin/plugin.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/registry/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/registry/packets.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/registry/registry.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/registry/registry_extension.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/server/__init__.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/server/server_extension.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/signal/__init__.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/signal/packets.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/signal/signal.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/signal/signal_extension.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/table/__init__.py
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/table/packets.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/table/table.py
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/extension/table/table_extension.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/interface/__init__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/interface/keyable.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/interface/named.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/localization/__init__.py
--rw-r--r--   0        0        0    33932 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/localization/locale.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/localization/localization.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/connection.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/network.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/packet_mapper.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/websocket_connection.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/packet/__init__.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/packet/packet.py
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 omu-0.3.1/src/omu/network/packet/packet_types.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omu-0.3.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.3.1/README.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 omu-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omu-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/address.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/app.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/bytebuffer.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/errors.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/event_emitter.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/helper.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/identifier.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/model.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/plugin.py
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/serializer.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/version.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/client/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/client/client.py
+-rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/client/omuclient.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/client/token.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/extension.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/extension_registry.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/asset/__init__.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/dashboard/packets.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/endpoint/endpoint.py
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/endpoint/packets.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/i18n/__init__.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/i18n/i18n_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/permission/__init__.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/permission/permission.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/plugin/package_info.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/plugin/plugin.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/registry/__init__.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/registry/packets.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/registry/registry.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/server/__init__.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/server/packets.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/server/server_extension.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/signal/__init__.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/signal/packets.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/signal/signal.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/signal/signal_extension.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/table/__init__.py
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/table/packets.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/table/table.py
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/extension/table/table_extension.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/interface/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/interface/keyable.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/interface/named.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/localization/__init__.py
+-rw-r--r--   0        0        0    33932 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/localization/locale.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/localization/localization.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/connection.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/network.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/packet_mapper.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/websocket_connection.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/packet/__init__.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/packet/packet.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 omu-0.3.2/src/omu/network/packet/packet_types.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omu-0.3.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.3.2/README.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 omu-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omu-0.3.2/PKG-INFO
```

### Comparing `omu-0.3.1/src/omu/app.py` & `omu-0.3.2/src/omu/app.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/bytebuffer.py` & `omu-0.3.2/src/omu/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/errors.py` & `omu-0.3.2/src/omu/errors.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/event_emitter.py` & `omu-0.3.2/src/omu/event_emitter.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/helper.py` & `omu-0.3.2/src/omu/helper.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/identifier.py` & `omu-0.3.2/src/omu/identifier.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/plugin.py` & `omu-0.3.2/src/omu/plugin.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/serializer.py` & `omu-0.3.2/src/omu/serializer.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/client/client.py` & `omu-0.3.2/src/omu/client/client.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/client/omuclient.py` & `omu-0.3.2/src/omu/client/omuclient.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/client/token.py` & `omu-0.3.2/src/omu/client/token.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/extension.py` & `omu-0.3.2/src/omu/extension/extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/extension_registry.py` & `omu-0.3.2/src/omu/extension/extension_registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/asset/asset_extension.py` & `omu-0.3.2/src/omu/extension/asset/asset_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/dashboard/__init__.py` & `omu-0.3.2/src/omu/extension/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/dashboard/dashboard_extension.py` & `omu-0.3.2/src/omu/extension/dashboard/dashboard_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/dashboard/packets.py` & `omu-0.3.2/src/omu/extension/dashboard/packets.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/endpoint/endpoint.py` & `omu-0.3.2/src/omu/extension/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/endpoint/endpoint_extension.py` & `omu-0.3.2/src/omu/extension/endpoint/endpoint_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/endpoint/packets.py` & `omu-0.3.2/src/omu/extension/endpoint/packets.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/i18n/i18n_extension.py` & `omu-0.3.2/src/omu/extension/i18n/i18n_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/permission/permission.py` & `omu-0.3.2/src/omu/extension/permission/permission.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/permission/permission_extension.py` & `omu-0.3.2/src/omu/extension/permission/permission_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/plugin/package_info.py` & `omu-0.3.2/src/omu/extension/plugin/package_info.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/plugin/plugin.py` & `omu-0.3.2/src/omu/extension/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/plugin/plugin_extension.py` & `omu-0.3.2/src/omu/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/registry/packets.py` & `omu-0.3.2/src/omu/extension/registry/packets.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/registry/registry.py` & `omu-0.3.2/src/omu/extension/registry/registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/registry/registry_extension.py` & `omu-0.3.2/src/omu/extension/registry/registry_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/server/server_extension.py` & `omu-0.3.2/src/omu/extension/server/server_extension.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-
 from omu.app import App
 from omu.client import Client
+from omu.event_emitter import Unlisten
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
 from omu.extension.registry import RegistryType
+from omu.extension.server.packets import ConsolePacket
 from omu.extension.table import TablePermissions, TableType
+from omu.helper import Coro
 from omu.identifier import Identifier
 from omu.network.packet import PacketType
 from omu.serializer import Serializer
 
 SERVER_EXTENSION_TYPE = ExtensionType(
     "server", lambda client: ServerExtension(client), lambda: []
 )
@@ -34,29 +36,66 @@
     serializer=Serializer.model(Identifier).to_array(),
 )
 VERSION_REGISTRY_TYPE = RegistryType[str | None].create_json(
     SERVER_EXTENSION_TYPE,
     "version",
     default_value=None,
 )
+SERVER_CONSOLE_PERMISSION_ID = SERVER_EXTENSION_TYPE / "console"
+CONSOLE_GET_ENDPOINT_TYPE = EndpointType[int | None, list[str]].create_json(
+    SERVER_EXTENSION_TYPE,
+    "console",
+    permission_id=SERVER_CONSOLE_PERMISSION_ID,
+)
+CONSOLE_LISTEN_PACKET_TYPE = PacketType[None].create_json(
+    SERVER_EXTENSION_TYPE,
+    "console_listen",
+)
+CONSOLE_PACKET_TYPE = PacketType[ConsolePacket].create_serialized(
+    SERVER_EXTENSION_TYPE,
+    "console",
+    serializer=ConsolePacket,
+)
 
 
 class ServerExtension(Extension):
     def __init__(self, client: Client) -> None:
         client.network.register_packet(
             REQUIRE_APPS_PACKET_TYPE,
+            CONSOLE_LISTEN_PACKET_TYPE,
+            CONSOLE_PACKET_TYPE,
         )
+        client.network.add_packet_handler(CONSOLE_PACKET_TYPE, self._on_console)
         self.client = client
         self.apps = client.tables.get(APP_TABLE_TYPE)
         self.required_apps: set[Identifier] = set()
+        self.console_listeners: list[Coro[[list[str]], None]] = []
         client.network.add_task(self.on_task)
 
     async def on_task(self) -> None:
-        await self.client.send(REQUIRE_APPS_PACKET_TYPE, [*self.required_apps])
+        if self.required_apps:
+            await self.client.send(REQUIRE_APPS_PACKET_TYPE, [*self.required_apps])
 
     async def shutdown(self, restart: bool = False) -> bool:
         return await self.client.endpoints.call(SHUTDOWN_ENDPOINT_TYPE, restart)
 
     def require(self, *app_ids: Identifier) -> None:
         if self.client.running:
             raise RuntimeError("Cannot require apps after the client has started")
         self.required_apps.update(app_ids)
+
+    async def console_get(self, line_count: int | None = None) -> list[str]:
+        return await self.client.endpoints.call(CONSOLE_GET_ENDPOINT_TYPE, line_count)
+
+    async def console_listen(self, listener: Coro[[list[str]], None]) -> Unlisten:
+        if len(self.console_listeners) == 0:
+
+            async def listen():
+                await self.client.send(CONSOLE_LISTEN_PACKET_TYPE, None)
+
+            self.client.when_ready(listen)
+        self.console_listeners.append(listener)
+        return lambda: self.console_listeners.remove(listener)
+
+    async def _on_console(self, packet: ConsolePacket) -> None:
+        for listener in self.console_listeners:
+            await listener(packet.lines)
```

### Comparing `omu-0.3.1/src/omu/extension/signal/packets.py` & `omu-0.3.2/src/omu/extension/signal/packets.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/signal/signal.py` & `omu-0.3.2/src/omu/extension/signal/signal.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/signal/signal_extension.py` & `omu-0.3.2/src/omu/extension/signal/signal_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/table/packets.py` & `omu-0.3.2/src/omu/extension/table/packets.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/table/table.py` & `omu-0.3.2/src/omu/extension/table/table.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/extension/table/table_extension.py` & `omu-0.3.2/src/omu/extension/table/table_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/localization/locale.py` & `omu-0.3.2/src/omu/localization/locale.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/network/connection.py` & `omu-0.3.2/src/omu/network/connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/network/network.py` & `omu-0.3.2/src/omu/network/network.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/network/packet_mapper.py` & `omu-0.3.2/src/omu/network/packet_mapper.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/network/websocket_connection.py` & `omu-0.3.2/src/omu/network/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/network/packet/packet.py` & `omu-0.3.2/src/omu/network/packet/packet.py`

 * *Files identical despite different names*

### Comparing `omu-0.3.1/src/omu/network/packet/packet_types.py` & `omu-0.3.2/src/omu/network/packet/packet_types.py`

 * *Files identical despite different names*

