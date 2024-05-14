# Comparing `tmp/MachSysS-0.6.5.tar.gz` & `tmp/machsyss-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MachSysS-0.6.5.tar", last modified: Tue Apr  9 12:53:48 2024, max compression
+gzip compressed data, was "machsyss-0.6.6.tar", last modified: Tue May 14 10:59:21 2024, max compression
```

## Comparing `MachSysS-0.6.5.tar` & `machsyss-0.6.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 12:53:42.000000 MachSysS-0.6.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 12:53:42.000000 MachSysS-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.959060 MachSysS-0.6.5/MachSysS/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_feems_result_to_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_gymir_result_to_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_proto_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    29834 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_to_feems.py
--rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/convert_to_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/feems_result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/feems_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/gymir_result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/gymir_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/system_structure_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    34703 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/system_structure_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 12:53:42.000000 MachSysS-0.6.5/MachSysS/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/MachSysS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 12:53:48.000000 MachSysS-0.6.5/MachSysS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 12:53:48.963060 MachSysS-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 12:53:42.000000 MachSysS-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:42.000000 MachSysS-0.6.5/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-09 12:53:42.000000 MachSysS-0.6.5/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:53:48.963060 MachSysS-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-09 12:53:42.000000 MachSysS-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:48.963060 MachSysS-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    35477 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-09 12:53:42.000000 MachSysS-0.6.5/tests/utility_compare_proto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.326342 machsyss-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-14 10:59:17.000000 machsyss-0.6.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-14 10:59:17.000000 machsyss-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 10:59:17.000000 machsyss-0.6.6/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.322342 machsyss-0.6.6/MachSysS/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16973 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17658 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/convert_feems_result_to_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/convert_gymir_result_to_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/convert_proto_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31977 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/convert_to_feems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23935 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/convert_to_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/feems_result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/feems_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/gymir_result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/gymir_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/system_structure_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35803 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/system_structure_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-14 10:59:17.000000 machsyss-0.6.6/MachSysS/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.326342 machsyss-0.6.6/MachSysS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-14 10:59:21.000000 machsyss-0.6.6/MachSysS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-14 10:59:21.000000 machsyss-0.6.6/MachSysS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:59:21.000000 machsyss-0.6.6/MachSysS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:59:21.000000 machsyss-0.6.6/MachSysS.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 10:59:21.000000 machsyss-0.6.6/MachSysS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 10:59:21.000000 machsyss-0.6.6/MachSysS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-14 10:59:21.326342 machsyss-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-14 10:59:17.000000 machsyss-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.326342 machsyss-0.6.6/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:17.000000 machsyss-0.6.6/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-14 10:59:17.000000 machsyss-0.6.6/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:59:21.326342 machsyss-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-14 10:59:17.000000 machsyss-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:21.326342 machsyss-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:59:17.000000 machsyss-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 10:59:17.000000 machsyss-0.6.6/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35477 2024-05-14 10:59:17.000000 machsyss-0.6.6/tests/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-14 10:59:17.000000 machsyss-0.6.6/tests/utility_compare_proto.py
```

### Comparing `MachSysS-0.6.5/CONTRIBUTING.md` & `machsyss-0.6.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/LICENSE` & `machsyss-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS/_modidx.py` & `machsyss-0.6.6/MachSysS/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Autogenerated by nbdev
 
 d = {
     "settings": {
         "branch": "master",
         "doc_baseurl": "/MachSysS/",
         "doc_host": "https://keviny.github.io",
-        "git_url": "https://SintefOceanEnergySystem@dev.azure.com/SintefOceanEnergySystem/MachinerySystemStucture/_git/MachinerySystemStucture",
+        "git_url": "https://github.com/SINTEF/FEEMS",
         "lib_path": "MachSysS",
     },
     "syms": {
         "MachSysS.convert_feems_result_to_proto": {
             "MachSysS.convert_feems_result_to_proto.FEEMSResultConverter": (
                 "convertfeemsresulttoproto.html#feemsresultconverter",
                 "MachSysS/convert_feems_result_to_proto.py",
```

### Comparing `MachSysS-0.6.5/MachSysS/convert_feems_result_to_proto.py` & `machsyss-0.6.6/MachSysS/convert_feems_result_to_proto.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS/convert_gymir_result_to_proto.py` & `machsyss-0.6.6/MachSysS/convert_gymir_result_to_proto.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS/convert_proto_timeseries.py` & `machsyss-0.6.6/MachSysS/convert_proto_timeseries.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS/convert_to_feems.py` & `machsyss-0.6.6/MachSysS/convert_to_feems.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,14 +75,16 @@
     EmissionCurvePoint,
     EmissionType,
     NOxCalculationMethod,
 )
 
 import MachSysS.system_structure_pb2 as proto
 
+_MIN_LENGTH_UID = 5
+
 
 def convert_proto_point_to_list(point: proto.Point) -> List[float]:
     """Converts protobuf point to a list"""
     return [point.x, point.y]
 
 
 def convert_proto_curve1d_to_np_array(curve: proto.Curve1D) -> np.ndarray:
@@ -116,14 +118,15 @@
         name=proto_component.name,
         rated_power=proto_component.rated_power_kw,
         eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
             proto_component.efficiency
         ),
         power_type=power_type,
         switchboard_id=switchboard_id,
+        uid=proto_component.uid if len(proto_component.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_electric_machine_to_feems(
     proto_component: proto.ElectricMachine,
     component_type: TypeComponent,
     power_type: TypePower,
@@ -135,14 +138,15 @@
         rated_power=proto_component.rated_power_kw,
         rated_speed=proto_component.rated_speed_rpm,
         power_type=power_type,
         eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
             proto_component.efficiency
         ),
         switchboard_id=switchboard_id,
+        uid=proto_component.uid if len(proto_component.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_fuel_cell_system_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> FuelCellSystem:
     """Converts protobuf subsystem message to feems component"""
@@ -153,27 +157,33 @@
         name=subsystem.fuel_cell.name,
         rated_power=subsystem.fuel_cell.rated_power_kw,
         eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
             subsystem.fuel_cell.efficiency
         ),
         fuel_type=TypeFuel(subsystem.fuel_cell.fuel.fuel_type),
         fuel_origin=FuelOrigin(subsystem.fuel_cell.fuel.fuel_origin),
+        uid=(
+            subsystem.fuel_cell.uid
+            if len(subsystem.fuel_cell.uid) > _MIN_LENGTH_UID
+            else None
+        ),
     )
     converter = convert_proto_electric_component_to_feems(
         subsystem.converter1,
         component_type=TypeComponent.POWER_CONVERTER,
         power_type=TypePower.POWER_TRANSMISSION,
         switchboard_id=switchboard_id,
     )
     return FuelCellSystem(
         name=subsystem.name,
         fuel_cell_module=fuel_cell,
         converter=converter,
         switchboard_id=switchboard_id,
         number_modules=number_modules,
+        uid=subsystem.uid if len(subsystem.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_emission_curve_to_feems(
     emission_curve: proto.EmissionCurve,
 ) -> EmissionCurve:
     """Converts protobuf emission curve to numpy array"""
@@ -231,25 +241,27 @@
             ),
             fuel_type=TypeFuel(proto_engine.main_fuel.fuel_type),
             fuel_origin=FuelOrigin(proto_engine.main_fuel.fuel_origin),
             pilot_fuel_type=TypeFuel(proto_engine.pilot_fuel.fuel_type),
             pilot_fuel_origin=FuelOrigin(proto_engine.pilot_fuel.fuel_origin),
             nox_calculation_method=nox_calculation_method,
             emissions_curves=emission_curves,
+            uid=proto_engine.uid if len(proto_engine.uid) > _MIN_LENGTH_UID else None,
         )
     return Engine(
         type_=type_engine,
         name=proto_engine.name,
         rated_power=proto_engine.rated_power_kw,
         rated_speed=proto_engine.rated_speed_rpm,
         bsfc_curve=convert_proto_efficiency_bsfc_power_to_np_array(proto_engine.bsfc),
         fuel_type=TypeFuel(proto_engine.main_fuel.fuel_type),
         fuel_origin=FuelOrigin(proto_engine.main_fuel.fuel_origin),
         nox_calculation_method=nox_calculation_method,
         emissions_curves=emission_curves,
+        uid=proto_engine.uid if len(proto_engine.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_cogas_to_feems(
     proto_cogas: proto.COGAS,
 ) -> Engine:
     """Converts protobuf COGAS message to feems COGAS component"""
@@ -275,14 +287,15 @@
         steam_turbine_power_curve=convert_proto_efficiency_bsfc_power_to_np_array(
             proto_cogas.steam_turbine_power_curve
         ),
         fuel_type=TypeFuel(proto_cogas.fuel.fuel_type),
         fuel_origin=FuelOrigin(proto_cogas.fuel.fuel_origin),
         nox_calculation_method=nox_calculation_method,
         emissions_curves=emission_curves,
+        uid=proto_cogas.uid if len(proto_cogas.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_genset_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> Genset:
     """Converts protobuf subsystem message to feems component"""
@@ -298,44 +311,54 @@
         rectifier = convert_proto_electric_component_to_feems(
             proto_component=subsystem.converter1,
             component_type=TypeComponent.RECTIFIER,
             power_type=TypePower.POWER_TRANSMISSION,
             switchboard_id=switchboard_id,
         )
     return Genset(
-        name=subsystem.name, aux_engine=engine, generator=generator, rectifier=rectifier
+        name=subsystem.name,
+        aux_engine=engine,
+        generator=generator,
+        rectifier=rectifier,
+        uid=subsystem.uid if len(subsystem.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_coges_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> COGES:
     """Converts protobuf subsystem message to feems component"""
     cogas = convert_proto_cogas_to_feems(proto_cogas=subsystem.cogas)
     generator = convert_proto_electric_machine_to_feems(
         proto_component=subsystem.electric_machine,
         component_type=TypeComponent.SYNCHRONOUS_MACHINE,
         power_type=TypePower.POWER_SOURCE,
         switchboard_id=switchboard_id,
     )
-    return COGES(name=subsystem.name, cogas=cogas, generator=generator)
+    return COGES(
+        name=subsystem.name,
+        cogas=cogas,
+        generator=generator,
+        uid=subsystem.uid if len(subsystem.uid) > _MIN_LENGTH_UID else None,
+    )
 
 
 def convert_proto_battery_to_feems(
     proto_component: proto.Battery, switchboard_id: int = 0
 ) -> Battery:
     return Battery(
         name=proto_component.name,
         rated_capacity_kwh=proto_component.energy_capacity_kwh,
         charging_rate_c=proto_component.rated_charging_rate_c,
         discharge_rate_c=proto_component.rated_discharging_rate_c,
         eff_charging=proto_component.efficiency_charging,
         eff_discharging=proto_component.efficiency_discharging,
         soc0=proto_component.initial_state_of_charge,
         switchboard_id=switchboard_id,
+        uid=proto_component.uid if len(proto_component.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_battery_system_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> BatterySystem:
     """Converts protobuf subsystem message to feems component"""
@@ -348,28 +371,30 @@
         power_type=TypePower.POWER_TRANSMISSION,
     )
     return BatterySystem(
         name=subsystem.name,
         battery=battery,
         converter=converter,
         switchboard_id=switchboard_id,
+        uid=subsystem.uid if len(subsystem.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_supercapacitor_to_feems(
     proto_component: proto.SuperCapacitor, switchboard_id: int = 0
 ) -> SuperCapacitor:
     return SuperCapacitor(
         name=proto_component.name,
         rated_capacity_wh=proto_component.energy_capacity_wh,
         rated_power=proto_component.rated_power_kw,
         eff_charging=proto_component.efficiency_charging,
         eff_discharging=proto_component.efficiency_discharging,
         soc0=proto_component.initial_state_of_charge,
         switchboard_id=switchboard_id,
+        uid=proto_component.uid if len(proto_component.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_supercapacitor_system_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> SuperCapacitorSystem:
     """Converts protobuf subsystem message to feems component"""
@@ -382,14 +407,15 @@
         power_type=TypePower.POWER_TRANSMISSION,
     )
     return SuperCapacitorSystem(
         name=subsystem.name,
         supercapacitor=supercapacitor,
         converter=converter,
         switchboard_id=switchboard_id,
+        uid=subsystem.uid if len(subsystem.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def collect_electric_components_from_sub_system(
     subsystem: proto.Subsystem,
 ) -> List[Dict[str, Union[str, Union[proto.ElectricMachine, proto.ElectricComponent]]]]:
     field_names = [
@@ -465,14 +491,15 @@
     return PTIPTO(
         name=subsystem.name,
         components=components_feems,
         rated_power=None if subsystem.rated_power_kw == 0 else subsystem.rated_power_kw,
         rated_speed=subsystem.rated_speed_rpm,
         switchboard_id=switchboard_id,
         shaft_line_id=shaft_line_id,
+        uid=subsystem.uid if len(subsystem.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_proto_serial_subsystem_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> SerialSystemElectric:
     proto_components = collect_electric_components_from_sub_system(subsystem)
@@ -490,14 +517,15 @@
         power_type=TypePower(subsystem.power_type),
         components=components_feems,
         switchboard_id=switchboard_id,
         rated_power=None if subsystem.rated_power_kw == 0 else subsystem.rated_power_kw,
         rated_speed=(
             None if subsystem.rated_speed_rpm == 0 else subsystem.rated_speed_rpm
         ),
+        uid=subsystem.uid if len(subsystem.uid) > _MIN_LENGTH_UID else None,
     )
 
 
 def convert_generic_electric_subsystem_to_feems(
     subsystem: proto.Subsystem, switchboard_id: int
 ) -> Union[ElectricComponent, SerialSystemElectric, PTIPTO]:
     proto_components = collect_electric_components_from_sub_system(subsystem)
@@ -601,14 +629,19 @@
                 MainEngineForMechanicalPropulsion(
                     name=sub_system.name,
                     engine=convert_proto_engine_to_feems(
                         proto_engine=sub_system.engine,
                         type_engine=TypeComponent.MAIN_ENGINE,
                     ),
                     shaft_line_id=shaft_line_id,
+                    uid=(
+                        sub_system.uid
+                        if len(sub_system.uid) > _MIN_LENGTH_UID
+                        else None
+                    ),
                 )
             )
         elif (
             sub_system.component_type
             == proto.Subsystem.ComponentType.MAIN_ENGINE_WITH_GEARBOX
         ):
             components.append(
@@ -616,23 +649,33 @@
                     name=sub_system.name,
                     main_engine=convert_proto_engine_to_feems(
                         proto_engine=sub_system.engine,
                         type_engine=TypeComponent.MAIN_ENGINE_WITH_GEARBOX,
                     ),
                     gearbox=BasicComponent(
                         type_=TypeComponent.GEARBOX,
-                        name=sub_system.gearbox.name,
+                        name=sub_system.gear.name,
                         power_type=TypePower.POWER_TRANSMISSION,
                         rated_power=sub_system.gear.rated_power_kw,
                         rated_speed=sub_system.gear.rated_speed_rpm,
                         eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
                             efficiency_bsfc_power=sub_system.gear.efficiency
                         ),
+                        uid=(
+                            sub_system.gear.uid
+                            if len(sub_system.gear.uid) > _MIN_LENGTH_UID
+                            else None
+                        ),
                     ),
                     shaft_line_id=shaft_line_id,
+                    uid=(
+                        sub_system.uid
+                        if len(sub_system.uid) > _MIN_LENGTH_UID
+                        else None
+                    ),
                 )
             )
         elif sub_system.component_type == proto.Subsystem.ComponentType.PTI_PTO_SYSTEM:
             if pti_ptos is None:
                 components.append(
                     convert_proto_pti_pto_subsystem_to_feems(
                         subsystem=sub_system,
@@ -669,14 +712,19 @@
                     name=sub_system.name,
                     shaft_line_id=shaft_line_id,
                     rated_power=sub_system.rated_power_kw,
                     rated_speed=sub_system.rated_speed_rpm,
                     eff_curve=convert_proto_efficiency_bsfc_power_to_np_array(
                         efficiency_bsfc_power=sub_system.propeller.efficiency
                     ),
+                    uid=(
+                        sub_system.uid
+                        if len(sub_system.uid) > _MIN_LENGTH_UID
+                        else None
+                    ),
                 )
             )
         else:
             raise ValueError(
                 f"The component type {TypeComponent(sub_system.component_type)} "
                 f"is not supported."
             )
```

### Comparing `MachSysS-0.6.5/MachSysS/convert_to_protobuf.py` & `machsyss-0.6.6/MachSysS/convert_to_protobuf.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,26 +131,28 @@
     """Convert elecrtic machine component of FEEMS to protobuf message"""
     return proto.ElectricMachine(
         name=component.name,
         rated_power_kw=component.rated_power,
         rated_speed_rpm=component.rated_speed,
         efficiency=convert_efficiency_curve_to_protobuf(component),
         order_from_switchboard_or_shaftline=order_from_switchboard,
+        uid=component.uid,
     )
 
 
 def convert_electric_component_to_protobuf(
     component: ElectricComponent, order_from_switchboard: int = 1
 ) -> proto.ElectricMachine:
     """Convert converter component of FEEMS to protobuf message"""
     return proto.ElectricComponent(
         name=component.name,
         rated_power_kw=component.rated_power,
         efficiency=convert_efficiency_curve_to_protobuf(component),
         order_from_switchboard_or_shaftline=order_from_switchboard,
+        uid=component.uid,
     )
 
 
 def convert_battery_component_to_protobuf(
     component: Battery, order_from_switchboard: int = 1
 ) -> proto.ElectricMachine:
     """Convert battery component of FEEMS to protobuf message"""
@@ -159,14 +161,15 @@
         energy_capacity_kwh=component.rated_capacity_kWh,
         rated_charging_rate_c=component.charging_rate_C,
         rated_discharging_rate_c=component.discharging_rate_C,
         efficiency_charging=component.eff_charging,
         efficiency_discharging=component.eff_discharging,
         initial_state_of_charge=component.soc0,
         order_from_switchboard_or_shaftline=order_from_switchboard,
+        uid=component.uid,
     )
 
 
 def convert_supercapacitor_component_to_protobuf(
     component: SuperCapacitor, order_from_switchboard: int = 1
 ) -> proto.ElectricMachine:
     """Convert converter component of FEEMS to protobuf message"""
@@ -174,24 +177,32 @@
         name=component.name,
         energy_capacity_wh=component.rated_capacity_Wh,
         rated_power_kw=component.rated_power,
         efficiency_charging=component.eff_charging,
         efficiency_discharging=component.eff_discharging,
         initial_state_of_charge=component.soc0,
         order_from_switchboard_or_shaftline=order_from_switchboard,
+        uid=component.uid,
     )
 
 
 def convert_serial_electric_system_to_protobuf(
     component: Union[SerialSystemElectric, PTIPTO],
     initial_order_from_switchboard: int = 1,
 ) -> proto.Subsystem:
     """Convert serial electric system or PTI/PTO component to protobuf message"""
     order = initial_order_from_switchboard
-    subsystem = proto.Subsystem()
+    subsystem = proto.Subsystem(
+        name=component.name,
+        rated_power_kw=component.rated_power,
+        rated_speed_rpm=component.rated_speed,
+        component_type=component.type.value,
+        power_type=component.power_type.value,
+        uid=component.uid,
+    )
     for subcomponent in component.components:
         if subcomponent.type == TypeComponent.TRANSFORMER:
             subsystem.transformer.CopyFrom(
                 convert_electric_component_to_protobuf(
                     component=subcomponent, order_from_switchboard=order
                 )
             )
@@ -276,14 +287,15 @@
         nox_calculation_method=convert_nox_calculation_method_to_protobuf(
             engine_feems.nox_calculation_method
         ),
         emission_curves=convert_emission_curves_to_protobuf(
             engine_feems.emission_curves
         ),
         order_from_switchboard_or_shaftline=order_from_shaftline_or_switchboard,
+        uid=engine_feems.uid,
     )
     if isinstance(engine_feems, EngineDualFuel):
         engine.pilot_bsfc.CopyFrom(
             convert_bsfc_curve_to_protobuf(engine_feems, for_pilot_fuel=True)
         )
         engine.pilot_fuel.CopyFrom(
             proto.Fuel(
@@ -309,14 +321,15 @@
             fuel_origin=component.fuel_origin.value,
         ),
         nox_calculation_method=convert_nox_calculation_method_to_protobuf(
             component.nox_calculation_method
         ),
         emission_curves=convert_emission_curves_to_protobuf(component.emission_curves),
         order_from_switchboard_or_shaftline=order_from_shaftline_or_switchboard,
+        uid=component.uid,
     )
     if component.gas_turbine_power_curve is not None:
         cogas.gas_turbine_power_curve.CopyFrom(
             convert_np_array_to_protobuf_power_curve(component.gas_turbine_power_curve)
         )
         cogas.steam_turbine_power_curve.CopyFrom(
             convert_np_array_to_protobuf_power_curve(
@@ -335,14 +348,15 @@
     for component in switchboard_feems.components:
         subsystem = proto.Subsystem(
             power_type=component.power_type.value,
             component_type=component.type.value,
             name=component.name,
             rated_power_kw=component.rated_power,
             rated_speed_rpm=component.rated_speed,
+            uid=component.uid,
         )
         if component.type == TypeComponent.GENERATOR:
             subsystem.electric_machine.CopyFrom(
                 convert_electric_machine_to_protobuf(
                     component=component,
                 )
             )
@@ -360,14 +374,15 @@
                     ),
                     fuel=proto.Fuel(
                         fuel_type=component.fuel_cell.fuel_type.value,
                         fuel_origin=component.fuel_cell.fuel_origin.value,
                     ),
                     number_modules=component.number_modules,
                     order_from_switchboard_or_shaftline=2,
+                    uid=component.fuel_cell.uid,
                 )
             )
         elif component.type == TypeComponent.COGES:
             component = cast(COGES, component)
             subsystem.cogas.CopyFrom(
                 convert_cogas_component_to_protobuf(
                     component=component.cogas, order_from_shaftline_or_switchboard=2
@@ -455,23 +470,25 @@
         gear = cast(MechanicalPropulsionComponent, gear)
         gear_proto = proto.Gear(
             name=gear.name,
             rated_power_kw=gear.rated_power,
             rated_speed_rpm=gear.rated_speed,
             efficiency=convert_efficiency_curve_to_protobuf(gear),
             order_from_switchboard_or_shaftline=1,
+            uid=gear.uid,
         )
 
     for component in shaftline_feems.components:
         subsystem = proto.Subsystem(
             power_type=component.power_type.value,
             component_type=component.type.value,
             name=component.name,
             rated_power_kw=component.rated_power,
             rated_speed_rpm=component.rated_speed,
+            uid=component.uid,
         )
         if component.type == TypeComponent.MAIN_ENGINE:
             component = cast(MainEngineForMechanicalPropulsion, component)
             subsystem.engine.CopyFrom(
                 convert_engine_component_to_protobuf(
                     engine_feems=component.engine, order_from_shaftline_or_switchboard=1
                 )
@@ -493,24 +510,26 @@
             subsystem.gear.CopyFrom(
                 proto.Gear(
                     name=component.gearbox.name,
                     rated_power_kw=component.gearbox.rated_power,
                     rated_speed_rpm=component.gearbox.rated_speed,
                     efficiency=convert_efficiency_curve_to_protobuf(component.gearbox),
                     order_from_switchboard_or_shaftline=1,
+                    uid=component.gearbox.uid,
                 )
             )
         elif component.type == TypeComponent.PROPELLER_LOAD:
             if gear_proto is not None:
                 subsystem.gear.CopyFrom(gear_proto)
             subsystem.propeller.CopyFrom(
                 proto.Propeller(
                     efficiency=convert_efficiency_curve_to_protobuf(component),
                     propulsor_id=propeller_id,
                     order_from_switchboard_or_shaftline=2,
+                    uid=component.uid,
                 )
             )
             propeller_id += 1
         elif component.type == TypeComponent.PTI_PTO_SYSTEM:
             subsystem.MergeFrom(
                 convert_serial_electric_system_to_protobuf(component=component)
             )
```

### Comparing `MachSysS-0.6.5/MachSysS/feems_result_pb2.py` & `machsyss-0.6.6/MachSysS/feems_result_pb2.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS/feems_result_pb2.pyi` & `machsyss-0.6.6/MachSysS/feems_result_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import system_structure_pb2 as _system_structure_pb2
+from . import system_structure_pb2 as _system_structure_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import (
     ClassVar as _ClassVar,
     Iterable as _Iterable,
     Mapping as _Mapping,
```

### Comparing `MachSysS-0.6.5/MachSysS/gymir_result_pb2.py` & `machsyss-0.6.6/MachSysS/gymir_result_pb2.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS/gymir_result_pb2.pyi` & `machsyss-0.6.6/MachSysS/gymir_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS/system_structure_pb2.py` & `machsyss-0.6.6/MachSysS/system_structure_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16system_structure.proto\x12\x18machinerySystemStructure"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01":\n\x07\x43urve1D\x12/\n\x06points\x18\x01 \x03(\x0b\x32\x1f.machinerySystemStructure.Point"_\n\tBSFCCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"e\n\x0f\x45\x66\x66iciencyCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"X\n\x04\x42SFC\x12\x32\n\x05\x63urve\x18\x01 \x01(\x0b\x32#.machinerySystemStructure.BSFCCurve\x12\x12\n\x05value\x18\x02 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value"s\n\nEfficiency\x12=\n\x05\x63urve\x18\x01 \x01(\x0b\x32).machinerySystemStructure.EfficiencyCurveH\x00\x88\x01\x01\x12\x12\n\x05value\x18\x02 \x01(\x01H\x01\x88\x01\x01\x42\x08\n\x06_curveB\x08\n\x06_value"`\n\nPowerCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"\x85\x01\n\x19PropulsionPowerTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"\x85\x01\n\x17\x41uxiliaryLoadTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x16\n\x0eswitchboard_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"8\n\rAuxiliaryLoad\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x0f\n\x07load_kw\x18\x02 \x01(\x01"\xa2\x01\n\rEmissionCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D\x12=\n\remission_type\x18\x04 \x01(\x0e\x32&.machinerySystemStructure.EmissionType"\xd8\x01\n\x04Gear\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ngear_ratio\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x04 \x01(\x01\x12\x38\n\nefficiency\x18\x05 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01"x\n\x04\x46uel\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x39\n\x0b\x66uel_origin\x18\x02 \x01(\x0e\x32$.machinerySystemStructure.FuelOrigin"\x85\x06\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12,\n\x04\x62sfc\x18\x04 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x31\n\tmain_fuel\x18\x05 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x32\n\npilot_bsfc\x18\x07 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x32\n\npilot_fuel\x18\x08 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12U\n\x16nox_calculation_method\x18\t \x01(\x0e\x32\x35.machinerySystemStructure.Engine.NOxCalculationMethod\x12@\n\x0f\x65mission_curves\x18\n \x03(\x0b\x32\'.machinerySystemStructure.EmissionCurve\x12K\n\x11\x65ngine_cycle_type\x18\x0b \x01(\x0e\x32\x30.machinerySystemStructure.Engine.EngineCycleType\x12\x16\n\x0eunit_price_usd\x18\x0c \x01(\x01\x12\x15\n\rstart_delay_s\x18\r \x01(\x01\x12\x19\n\x11turn_off_power_kw\x18\x0e \x01(\x01"E\n\x14NOxCalculationMethod\x12\n\n\x06TIER_2\x10\x00\x12\n\n\x06TIER_1\x10\x01\x12\n\n\x06TIER_3\x10\x02\x12\t\n\x05\x43URVE\x10\x03"O\n\x0f\x45ngineCycleType\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x44IESEL\x10\x01\x12\x08\n\x04OTTO\x10\x02\x12\x1c\n\x18LEAN_BURN_SPARK_IGNITION\x10\x03"\xce\x04\n\x05\x43OGAS\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12\x38\n\nefficiency\x18\x04 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12\x45\n\x17gas_turbine_power_curve\x18\x05 \x01(\x0b\x32$.machinerySystemStructure.PowerCurve\x12G\n\x19steam_turbine_power_curve\x18\x06 \x01(\x0b\x32$.machinerySystemStructure.PowerCurve\x12,\n\x04\x66uel\x18\x07 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12+\n#order_from_switchboard_or_shaftline\x18\x08 \x01(\r\x12U\n\x16nox_calculation_method\x18\t \x01(\x0e\x32\x35.machinerySystemStructure.Engine.NOxCalculationMethod\x12@\n\x0f\x65mission_curves\x18\n \x03(\x0b\x32\'.machinerySystemStructure.EmissionCurve\x12\x16\n\x0eunit_price_usd\x18\x0b \x01(\x01\x12\x15\n\rstart_delay_s\x18\x0c \x01(\x01\x12\x19\n\x11turn_off_power_kw\x18\r \x01(\x01"\xcf\x01\n\x0f\x45lectricMachine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12\x38\n\nefficiency\x18\x04 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x06 \x01(\x01"\x82\x03\n\x07\x42\x61ttery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x13\x65nergy_capacity_kwh\x18\x02 \x01(\x01\x12\x1d\n\x15rated_charging_rate_c\x18\x03 \x01(\x01\x12 \n\x18rated_discharging_rate_c\x18\x04 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x05 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x06 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x07 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x08 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\t \x01(\x01\x12&\n\x1eself_discharge_percent_per_day\x18\n \x01(\x01\x12\x1f\n\x17state_of_energy_minimum\x18\x0b \x01(\x01\x12\x1f\n\x17state_of_energy_maximum\x18\x0c \x01(\x01"\xb8\x01\n\x11\x45lectricComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01"\xac\x02\n\x08\x46uelCell\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12,\n\x04\x66uel\x18\x06 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01\x12\x16\n\x0enumber_modules\x18\x08 \x01(\r\x12\x1e\n\x16power_minimum_specific\x18\t \x01(\x01\x12\x15\n\rstart_delay_s\x18\n \x01(\x01"\x96\x01\n\tPropeller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x38\n\nefficiency\x18\x02 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r"$\n\nBusBreaker\x12\x16\n\x0eswitchboard_to\x18\x01 \x01(\x05"\xf5\x01\n\x0eSuperCapacitor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12\x65nergy_capacity_wh\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x04 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x05 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x06 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x07 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x08 \x01(\x01"\xba\x01\n\x13MechanicalComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01"\x80\x0e\n\tSubsystem\x12,\n\x04gear\x18\x01 \x01(\x0b\x32\x1e.machinerySystemStructure.Gear\x12\x30\n\x06\x65ngine\x18\x02 \x01(\x0b\x32 .machinerySystemStructure.Engine\x12\x43\n\x10\x65lectric_machine\x18\x03 \x01(\x0b\x32).machinerySystemStructure.ElectricMachine\x12@\n\x0btransformer\x18\x04 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter1\x18\x05 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter2\x18\x06 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12\x32\n\x07\x62\x61ttery\x18\x07 \x01(\x0b\x32!.machinerySystemStructure.Battery\x12\x35\n\tfuel_cell\x18\x08 \x01(\x0b\x32".machinerySystemStructure.FuelCell\x12\x36\n\tpropeller\x18\t \x01(\x0b\x32#.machinerySystemStructure.Propeller\x12\x39\n\x0b\x62us_breaker\x18\n \x01(\x0b\x32$.machinerySystemStructure.BusBreaker\x12@\n\x0esupercapacitor\x18\x0b \x01(\x0b\x32(.machinerySystemStructure.SuperCapacitor\x12?\n\nother_load\x18\x0c \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12.\n\x05\x63ogas\x18\r \x01(\x0b\x32\x1f.machinerySystemStructure.COGAS\x12\x41\n\npower_type\x18\x0e \x01(\x0e\x32-.machinerySystemStructure.Subsystem.PowerType\x12I\n\x0e\x63omponent_type\x18\x0f \x01(\x0e\x32\x31.machinerySystemStructure.Subsystem.ComponentType\x12\x0c\n\x04name\x18\x10 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x11 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x12 \x01(\x01\x12-\n%ramp_up_rate_limit_percent_per_second\x18\x13 \x01(\x01\x12/\n\'ramp_down_rate_limit_percent_per_second\x18\x14 \x01(\x01\x12\x17\n\x0f\x62\x61se_load_order\x18\x15 \x01(\r"s\n\tPowerType\x12\t\n\x05NONE1\x10\x00\x12\x10\n\x0cPOWER_SOURCE\x10\x01\x12\x12\n\x0ePOWER_CONSUMER\x10\x02\x12\x0b\n\x07PTI_PTO\x10\x03\x12\x12\n\x0e\x45NERGY_STORAGE\x10\x04\x12\x14\n\x10SHORE_CONNECTION\x10\x05"\xbd\x04\n\rComponentType\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMAIN_ENGINE\x10\x01\x12\x14\n\x10\x41UXILIARY_ENGINE\x10\x02\x12\r\n\tGENERATOR\x10\x03\x12\x14\n\x10PROPULSION_DRIVE\x10\x04\x12\x0e\n\nOTHER_LOAD\x10\x05\x12\x12\n\x0ePTI_PTO_SYSTEM\x10\x06\x12\x12\n\x0e\x42\x41TTERY_SYSTEM\x10\x07\x12\x14\n\x10\x46UEL_CELL_SYSTEM\x10\x08\x12\r\n\tRECTIFIER\x10\t\x12\x1c\n\x18MAIN_ENGINE_WITH_GEARBOX\x10\n\x12\x12\n\x0e\x45LECTRIC_MOTOR\x10\x0b\x12\n\n\x06GENSET\x10\x0c\x12\x0f\n\x0bTRANSFORMER\x10\r\x12\x0c\n\x08INVERTER\x10\x0e\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x0f\x12\x14\n\x10\x41\x43TIVE_FRONT_END\x10\x10\x12\x13\n\x0fPOWER_CONVERTER\x10\x11\x12\x17\n\x13SYNCHRONOUS_MACHINE\x10\x12\x12\x15\n\x11INDUCTION_MACHINE\x10\x13\x12\x0b\n\x07GEARBOX\x10\x14\x12\r\n\tFUEL_CELL\x10\x15\x12\x12\n\x0ePROPELLER_LOAD\x10\x16\x12\x19\n\x15OTHER_MECHANICAL_LOAD\x10\x17\x12\x0b\n\x07\x42\x41TTERY\x10\x18\x12\x12\n\x0eSUPERCAPACITOR\x10\x19\x12\x19\n\x15SUPERCAPACITOR_SYSTEM\x10\x1a\x12\x0f\n\x0bSHORE_POWER\x10\x1b\x12\t\n\x05\x43OGAS\x10\x1c\x12\t\n\x05\x43OGES\x10\x1d"^\n\x0bSwitchboard\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"[\n\tShaftLine\x12\x15\n\rshaft_line_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"L\n\x10MechanicalSystem\x12\x38\n\x0bshaft_lines\x18\x01 \x03(\x0b\x32#.machinerySystemStructure.ShaftLine"M\n\x0e\x45lectricSystem\x12;\n\x0cswitchboards\x18\x01 \x03(\x0b\x32%.machinerySystemStructure.Switchboard"Y\n\x0b\x46uelStorage\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x13\n\x0b\x63\x61pacity_kg\x18\x02 \x01(\x01"\xfe\x03\n\x0fMachinerySystem\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x0fpropulsion_type\x18\x02 \x01(\x0e\x32\x38.machinerySystemStructure.MachinerySystem.PropulsionType\x12;\n\x0c\x66uel_storage\x18\x03 \x03(\x0b\x32%.machinerySystemStructure.FuelStorage\x12.\n&maximum_allowed_genset_load_percentage\x18\x04 \x01(\x01\x12\x45\n\x11mechanical_system\x18\x05 \x01(\x0b\x32*.machinerySystemStructure.MechanicalSystem\x12\x41\n\x0f\x65lectric_system\x18\x06 \x01(\x0b\x32(.machinerySystemStructure.ElectricSystem\x12\x31\n)maximum_allowed_fuel_cell_load_percentage\x18\x07 \x01(\x01\x12$\n\x1c\x61verage_base_load_percentage\x18\x08 \x01(\x01":\n\x0ePropulsionType\x12\x0e\n\nMECHANICAL\x10\x00\x12\x0c\n\x08\x45LECTRIC\x10\x01\x12\n\n\x06HYBRID\x10\x02*T\n\x0c\x45missionType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SOX\x10\x01\x12\x07\n\x03NOX\x10\x02\x12\x06\n\x02\x43O\x10\x03\x12\x06\n\x02PM\x10\x04\x12\x06\n\x02HC\x10\x05\x12\x07\n\x03\x43H4\x10\x06\x12\x07\n\x03N2O\x10\x07*\x90\x01\n\x08\x46uelType\x12\n\n\x06\x44IESEL\x10\x00\x12\x07\n\x03HFO\x10\x01\x12\x0f\n\x0bNATURAL_GAS\x10\x02\x12\x0c\n\x08HYDROGEN\x10\x03\x12\x0b\n\x07\x41MMONIA\x10\x04\x12\x0f\n\x0bLPG_PROPANE\x10\x05\x12\x0e\n\nLPG_BUTANE\x10\x06\x12\x0b\n\x07\x45THANOL\x10\x07\x12\x0c\n\x08METHANOL\x10\x08\x12\x07\n\x03LFO\x10\t*C\n\nFuelOrigin\x12\t\n\x05NONE1\x10\x00\x12\n\n\x06\x46OSSIL\x10\x01\x12\x07\n\x03\x42IO\x10\x02\x12\x15\n\x11RENEWABLE_NON_BIO\x10\x03*E\n\x0f\x46uelSpecifiedBy\x12\t\n\x05NONE2\x10\x00\x12\x14\n\x10\x46UEL_EU_MARITIME\x10\x01\x12\x07\n\x03IMO\x10\x02\x12\x08\n\x04USER\x10\x03\x62\x06proto3'
+    b'\n\x16system_structure.proto\x12\x18machinerySystemStructure"\x1d\n\x05Point\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01":\n\x07\x43urve1D\x12/\n\x06points\x18\x01 \x03(\x0b\x32\x1f.machinerySystemStructure.Point"_\n\tBSFCCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"e\n\x0f\x45\x66\x66iciencyCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"X\n\x04\x42SFC\x12\x32\n\x05\x63urve\x18\x01 \x01(\x0b\x32#.machinerySystemStructure.BSFCCurve\x12\x12\n\x05value\x18\x02 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value"s\n\nEfficiency\x12=\n\x05\x63urve\x18\x01 \x01(\x0b\x32).machinerySystemStructure.EfficiencyCurveH\x00\x88\x01\x01\x12\x12\n\x05value\x18\x02 \x01(\x01H\x01\x88\x01\x01\x42\x08\n\x06_curveB\x08\n\x06_value"`\n\nPowerCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"\x85\x01\n\x19PropulsionPowerTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"\x85\x01\n\x17\x41uxiliaryLoadTimeSeries\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x16\n\x0eswitchboard_id\x18\x03 \x01(\r\x12\x30\n\x05\x63urve\x18\x04 \x01(\x0b\x32!.machinerySystemStructure.Curve1D"8\n\rAuxiliaryLoad\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x0f\n\x07load_kw\x18\x02 \x01(\x01"\xa2\x01\n\rEmissionCurve\x12\x0f\n\x07x_label\x18\x01 \x01(\t\x12\x0f\n\x07y_label\x18\x02 \x01(\t\x12\x30\n\x05\x63urve\x18\x03 \x01(\x0b\x32!.machinerySystemStructure.Curve1D\x12=\n\remission_type\x18\x04 \x01(\x0e\x32&.machinerySystemStructure.EmissionType"\xe5\x01\n\x04Gear\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ngear_ratio\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x04 \x01(\x01\x12\x38\n\nefficiency\x18\x05 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01\x12\x0b\n\x03uid\x18\x08 \x01(\t"x\n\x04\x46uel\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x39\n\x0b\x66uel_origin\x18\x02 \x01(\x0e\x32$.machinerySystemStructure.FuelOrigin"\x92\x06\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12,\n\x04\x62sfc\x18\x04 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x31\n\tmain_fuel\x18\x05 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12+\n#order_from_switchboard_or_shaftline\x18\x06 \x01(\r\x12\x32\n\npilot_bsfc\x18\x07 \x01(\x0b\x32\x1e.machinerySystemStructure.BSFC\x12\x32\n\npilot_fuel\x18\x08 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12U\n\x16nox_calculation_method\x18\t \x01(\x0e\x32\x35.machinerySystemStructure.Engine.NOxCalculationMethod\x12@\n\x0f\x65mission_curves\x18\n \x03(\x0b\x32\'.machinerySystemStructure.EmissionCurve\x12K\n\x11\x65ngine_cycle_type\x18\x0b \x01(\x0e\x32\x30.machinerySystemStructure.Engine.EngineCycleType\x12\x16\n\x0eunit_price_usd\x18\x0c \x01(\x01\x12\x15\n\rstart_delay_s\x18\r \x01(\x01\x12\x19\n\x11turn_off_power_kw\x18\x0e \x01(\x01\x12\x0b\n\x03uid\x18\x0f \x01(\t"E\n\x14NOxCalculationMethod\x12\n\n\x06TIER_2\x10\x00\x12\n\n\x06TIER_1\x10\x01\x12\n\n\x06TIER_3\x10\x02\x12\t\n\x05\x43URVE\x10\x03"O\n\x0f\x45ngineCycleType\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x44IESEL\x10\x01\x12\x08\n\x04OTTO\x10\x02\x12\x1c\n\x18LEAN_BURN_SPARK_IGNITION\x10\x03"\xdb\x04\n\x05\x43OGAS\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12\x38\n\nefficiency\x18\x04 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12\x45\n\x17gas_turbine_power_curve\x18\x05 \x01(\x0b\x32$.machinerySystemStructure.PowerCurve\x12G\n\x19steam_turbine_power_curve\x18\x06 \x01(\x0b\x32$.machinerySystemStructure.PowerCurve\x12,\n\x04\x66uel\x18\x07 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12+\n#order_from_switchboard_or_shaftline\x18\x08 \x01(\r\x12U\n\x16nox_calculation_method\x18\t \x01(\x0e\x32\x35.machinerySystemStructure.Engine.NOxCalculationMethod\x12@\n\x0f\x65mission_curves\x18\n \x03(\x0b\x32\'.machinerySystemStructure.EmissionCurve\x12\x16\n\x0eunit_price_usd\x18\x0b \x01(\x01\x12\x15\n\rstart_delay_s\x18\x0c \x01(\x01\x12\x19\n\x11turn_off_power_kw\x18\r \x01(\x01\x12\x0b\n\x03uid\x18\x0e \x01(\t"\xdc\x01\n\x0f\x45lectricMachine\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x03 \x01(\x01\x12\x38\n\nefficiency\x18\x04 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x06 \x01(\x01\x12\x0b\n\x03uid\x18\x07 \x01(\t"\x8f\x03\n\x07\x42\x61ttery\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x13\x65nergy_capacity_kwh\x18\x02 \x01(\x01\x12\x1d\n\x15rated_charging_rate_c\x18\x03 \x01(\x01\x12 \n\x18rated_discharging_rate_c\x18\x04 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x05 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x06 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x07 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x08 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\t \x01(\x01\x12&\n\x1eself_discharge_percent_per_day\x18\n \x01(\x01\x12\x1f\n\x17state_of_energy_minimum\x18\x0b \x01(\x01\x12\x1f\n\x17state_of_energy_maximum\x18\x0c \x01(\x01\x12\x0b\n\x03uid\x18\r \x01(\t"\xc5\x01\n\x11\x45lectricComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01\x12\x0b\n\x03uid\x18\x06 \x01(\t"\xb9\x02\n\x08\x46uelCell\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12,\n\x04\x66uel\x18\x06 \x01(\x0b\x32\x1e.machinerySystemStructure.Fuel\x12\x16\n\x0eunit_price_usd\x18\x07 \x01(\x01\x12\x16\n\x0enumber_modules\x18\x08 \x01(\r\x12\x1e\n\x16power_minimum_specific\x18\t \x01(\x01\x12\x15\n\rstart_delay_s\x18\n \x01(\x01\x12\x0b\n\x03uid\x18\x0b \x01(\t"\xa3\x01\n\tPropeller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x38\n\nefficiency\x18\x02 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12\x14\n\x0cpropulsor_id\x18\x03 \x01(\r\x12+\n#order_from_switchboard_or_shaftline\x18\x05 \x01(\r\x12\x0b\n\x03uid\x18\x06 \x01(\t"$\n\nBusBreaker\x12\x16\n\x0eswitchboard_to\x18\x01 \x01(\x05"\x82\x02\n\x0eSuperCapacitor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12\x65nergy_capacity_wh\x18\x02 \x01(\x01\x12\x16\n\x0erated_power_kw\x18\x03 \x01(\x01\x12\x1b\n\x13\x65\x66\x66iciency_charging\x18\x04 \x01(\x01\x12\x1e\n\x16\x65\x66\x66iciency_discharging\x18\x05 \x01(\x01\x12\x1f\n\x17initial_state_of_charge\x18\x06 \x01(\x01\x12+\n#order_from_switchboard_or_shaftline\x18\x07 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x08 \x01(\x01\x12\x0b\n\x03uid\x18\t \x01(\t"\xc7\x01\n\x13MechanicalComponent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x02 \x01(\x01\x12\x38\n\nefficiency\x18\x03 \x01(\x0b\x32$.machinerySystemStructure.Efficiency\x12+\n#order_from_switchboard_or_shaftline\x18\x04 \x01(\r\x12\x16\n\x0eunit_price_usd\x18\x05 \x01(\x01\x12\x0b\n\x03uid\x18\x06 \x01(\t"\x8d\x0e\n\tSubsystem\x12,\n\x04gear\x18\x01 \x01(\x0b\x32\x1e.machinerySystemStructure.Gear\x12\x30\n\x06\x65ngine\x18\x02 \x01(\x0b\x32 .machinerySystemStructure.Engine\x12\x43\n\x10\x65lectric_machine\x18\x03 \x01(\x0b\x32).machinerySystemStructure.ElectricMachine\x12@\n\x0btransformer\x18\x04 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter1\x18\x05 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12?\n\nconverter2\x18\x06 \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12\x32\n\x07\x62\x61ttery\x18\x07 \x01(\x0b\x32!.machinerySystemStructure.Battery\x12\x35\n\tfuel_cell\x18\x08 \x01(\x0b\x32".machinerySystemStructure.FuelCell\x12\x36\n\tpropeller\x18\t \x01(\x0b\x32#.machinerySystemStructure.Propeller\x12\x39\n\x0b\x62us_breaker\x18\n \x01(\x0b\x32$.machinerySystemStructure.BusBreaker\x12@\n\x0esupercapacitor\x18\x0b \x01(\x0b\x32(.machinerySystemStructure.SuperCapacitor\x12?\n\nother_load\x18\x0c \x01(\x0b\x32+.machinerySystemStructure.ElectricComponent\x12.\n\x05\x63ogas\x18\r \x01(\x0b\x32\x1f.machinerySystemStructure.COGAS\x12\x41\n\npower_type\x18\x0e \x01(\x0e\x32-.machinerySystemStructure.Subsystem.PowerType\x12I\n\x0e\x63omponent_type\x18\x0f \x01(\x0e\x32\x31.machinerySystemStructure.Subsystem.ComponentType\x12\x0c\n\x04name\x18\x10 \x01(\t\x12\x16\n\x0erated_power_kw\x18\x11 \x01(\x01\x12\x17\n\x0frated_speed_rpm\x18\x12 \x01(\x01\x12-\n%ramp_up_rate_limit_percent_per_second\x18\x13 \x01(\x01\x12/\n\'ramp_down_rate_limit_percent_per_second\x18\x14 \x01(\x01\x12\x17\n\x0f\x62\x61se_load_order\x18\x15 \x01(\r\x12\x0b\n\x03uid\x18\x16 \x01(\t"s\n\tPowerType\x12\t\n\x05NONE1\x10\x00\x12\x10\n\x0cPOWER_SOURCE\x10\x01\x12\x12\n\x0ePOWER_CONSUMER\x10\x02\x12\x0b\n\x07PTI_PTO\x10\x03\x12\x12\n\x0e\x45NERGY_STORAGE\x10\x04\x12\x14\n\x10SHORE_CONNECTION\x10\x05"\xbd\x04\n\rComponentType\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMAIN_ENGINE\x10\x01\x12\x14\n\x10\x41UXILIARY_ENGINE\x10\x02\x12\r\n\tGENERATOR\x10\x03\x12\x14\n\x10PROPULSION_DRIVE\x10\x04\x12\x0e\n\nOTHER_LOAD\x10\x05\x12\x12\n\x0ePTI_PTO_SYSTEM\x10\x06\x12\x12\n\x0e\x42\x41TTERY_SYSTEM\x10\x07\x12\x14\n\x10\x46UEL_CELL_SYSTEM\x10\x08\x12\r\n\tRECTIFIER\x10\t\x12\x1c\n\x18MAIN_ENGINE_WITH_GEARBOX\x10\n\x12\x12\n\x0e\x45LECTRIC_MOTOR\x10\x0b\x12\n\n\x06GENSET\x10\x0c\x12\x0f\n\x0bTRANSFORMER\x10\r\x12\x0c\n\x08INVERTER\x10\x0e\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x0f\x12\x14\n\x10\x41\x43TIVE_FRONT_END\x10\x10\x12\x13\n\x0fPOWER_CONVERTER\x10\x11\x12\x17\n\x13SYNCHRONOUS_MACHINE\x10\x12\x12\x15\n\x11INDUCTION_MACHINE\x10\x13\x12\x0b\n\x07GEARBOX\x10\x14\x12\r\n\tFUEL_CELL\x10\x15\x12\x12\n\x0ePROPELLER_LOAD\x10\x16\x12\x19\n\x15OTHER_MECHANICAL_LOAD\x10\x17\x12\x0b\n\x07\x42\x41TTERY\x10\x18\x12\x12\n\x0eSUPERCAPACITOR\x10\x19\x12\x19\n\x15SUPERCAPACITOR_SYSTEM\x10\x1a\x12\x0f\n\x0bSHORE_POWER\x10\x1b\x12\t\n\x05\x43OGAS\x10\x1c\x12\t\n\x05\x43OGES\x10\x1d"^\n\x0bSwitchboard\x12\x16\n\x0eswitchboard_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"[\n\tShaftLine\x12\x15\n\rshaft_line_id\x18\x01 \x01(\r\x12\x37\n\nsubsystems\x18\x02 \x03(\x0b\x32#.machinerySystemStructure.Subsystem"L\n\x10MechanicalSystem\x12\x38\n\x0bshaft_lines\x18\x01 \x03(\x0b\x32#.machinerySystemStructure.ShaftLine"M\n\x0e\x45lectricSystem\x12;\n\x0cswitchboards\x18\x01 \x03(\x0b\x32%.machinerySystemStructure.Switchboard"Y\n\x0b\x46uelStorage\x12\x35\n\tfuel_type\x18\x01 \x01(\x0e\x32".machinerySystemStructure.FuelType\x12\x13\n\x0b\x63\x61pacity_kg\x18\x02 \x01(\x01"\xfe\x03\n\x0fMachinerySystem\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x0fpropulsion_type\x18\x02 \x01(\x0e\x32\x38.machinerySystemStructure.MachinerySystem.PropulsionType\x12;\n\x0c\x66uel_storage\x18\x03 \x03(\x0b\x32%.machinerySystemStructure.FuelStorage\x12.\n&maximum_allowed_genset_load_percentage\x18\x04 \x01(\x01\x12\x45\n\x11mechanical_system\x18\x05 \x01(\x0b\x32*.machinerySystemStructure.MechanicalSystem\x12\x41\n\x0f\x65lectric_system\x18\x06 \x01(\x0b\x32(.machinerySystemStructure.ElectricSystem\x12\x31\n)maximum_allowed_fuel_cell_load_percentage\x18\x07 \x01(\x01\x12$\n\x1c\x61verage_base_load_percentage\x18\x08 \x01(\x01":\n\x0ePropulsionType\x12\x0e\n\nMECHANICAL\x10\x00\x12\x0c\n\x08\x45LECTRIC\x10\x01\x12\n\n\x06HYBRID\x10\x02*T\n\x0c\x45missionType\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03SOX\x10\x01\x12\x07\n\x03NOX\x10\x02\x12\x06\n\x02\x43O\x10\x03\x12\x06\n\x02PM\x10\x04\x12\x06\n\x02HC\x10\x05\x12\x07\n\x03\x43H4\x10\x06\x12\x07\n\x03N2O\x10\x07*\x90\x01\n\x08\x46uelType\x12\n\n\x06\x44IESEL\x10\x00\x12\x07\n\x03HFO\x10\x01\x12\x0f\n\x0bNATURAL_GAS\x10\x02\x12\x0c\n\x08HYDROGEN\x10\x03\x12\x0b\n\x07\x41MMONIA\x10\x04\x12\x0f\n\x0bLPG_PROPANE\x10\x05\x12\x0e\n\nLPG_BUTANE\x10\x06\x12\x0b\n\x07\x45THANOL\x10\x07\x12\x0c\n\x08METHANOL\x10\x08\x12\x07\n\x03LFO\x10\t*C\n\nFuelOrigin\x12\t\n\x05NONE1\x10\x00\x12\n\n\x06\x46OSSIL\x10\x01\x12\x07\n\x03\x42IO\x10\x02\x12\x15\n\x11RENEWABLE_NON_BIO\x10\x03*E\n\x0f\x46uelSpecifiedBy\x12\t\n\x05NONE2\x10\x00\x12\x14\n\x10\x46UEL_EU_MARITIME\x10\x01\x12\x07\n\x03IMO\x10\x02\x12\x08\n\x04USER\x10\x03\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "system_structure_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
-    _globals["_EMISSIONTYPE"]._serialized_start = 7315
-    _globals["_EMISSIONTYPE"]._serialized_end = 7399
-    _globals["_FUELTYPE"]._serialized_start = 7402
-    _globals["_FUELTYPE"]._serialized_end = 7546
-    _globals["_FUELORIGIN"]._serialized_start = 7548
-    _globals["_FUELORIGIN"]._serialized_end = 7615
-    _globals["_FUELSPECIFIEDBY"]._serialized_start = 7617
-    _globals["_FUELSPECIFIEDBY"]._serialized_end = 7686
+    _globals["_EMISSIONTYPE"]._serialized_start = 7458
+    _globals["_EMISSIONTYPE"]._serialized_end = 7542
+    _globals["_FUELTYPE"]._serialized_start = 7545
+    _globals["_FUELTYPE"]._serialized_end = 7689
+    _globals["_FUELORIGIN"]._serialized_start = 7691
+    _globals["_FUELORIGIN"]._serialized_end = 7758
+    _globals["_FUELSPECIFIEDBY"]._serialized_start = 7760
+    _globals["_FUELSPECIFIEDBY"]._serialized_end = 7829
     _globals["_POINT"]._serialized_start = 52
     _globals["_POINT"]._serialized_end = 81
     _globals["_CURVE1D"]._serialized_start = 83
     _globals["_CURVE1D"]._serialized_end = 141
     _globals["_BSFCCURVE"]._serialized_start = 143
     _globals["_BSFCCURVE"]._serialized_end = 238
     _globals["_EFFICIENCYCURVE"]._serialized_start = 240
@@ -49,55 +49,55 @@
     _globals["_AUXILIARYLOADTIMESERIES"]._serialized_start = 785
     _globals["_AUXILIARYLOADTIMESERIES"]._serialized_end = 918
     _globals["_AUXILIARYLOAD"]._serialized_start = 920
     _globals["_AUXILIARYLOAD"]._serialized_end = 976
     _globals["_EMISSIONCURVE"]._serialized_start = 979
     _globals["_EMISSIONCURVE"]._serialized_end = 1141
     _globals["_GEAR"]._serialized_start = 1144
-    _globals["_GEAR"]._serialized_end = 1360
-    _globals["_FUEL"]._serialized_start = 1362
-    _globals["_FUEL"]._serialized_end = 1482
-    _globals["_ENGINE"]._serialized_start = 1485
-    _globals["_ENGINE"]._serialized_end = 2258
-    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_start = 2108
-    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_end = 2177
-    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_start = 2179
-    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_end = 2258
-    _globals["_COGAS"]._serialized_start = 2261
-    _globals["_COGAS"]._serialized_end = 2851
-    _globals["_ELECTRICMACHINE"]._serialized_start = 2854
-    _globals["_ELECTRICMACHINE"]._serialized_end = 3061
-    _globals["_BATTERY"]._serialized_start = 3064
-    _globals["_BATTERY"]._serialized_end = 3450
-    _globals["_ELECTRICCOMPONENT"]._serialized_start = 3453
-    _globals["_ELECTRICCOMPONENT"]._serialized_end = 3637
-    _globals["_FUELCELL"]._serialized_start = 3640
-    _globals["_FUELCELL"]._serialized_end = 3940
-    _globals["_PROPELLER"]._serialized_start = 3943
-    _globals["_PROPELLER"]._serialized_end = 4093
-    _globals["_BUSBREAKER"]._serialized_start = 4095
-    _globals["_BUSBREAKER"]._serialized_end = 4131
-    _globals["_SUPERCAPACITOR"]._serialized_start = 4134
-    _globals["_SUPERCAPACITOR"]._serialized_end = 4379
-    _globals["_MECHANICALCOMPONENT"]._serialized_start = 4382
-    _globals["_MECHANICALCOMPONENT"]._serialized_end = 4568
-    _globals["_SUBSYSTEM"]._serialized_start = 4571
-    _globals["_SUBSYSTEM"]._serialized_end = 6363
-    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_start = 5672
-    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_end = 5787
-    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_start = 5790
-    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_end = 6363
-    _globals["_SWITCHBOARD"]._serialized_start = 6365
-    _globals["_SWITCHBOARD"]._serialized_end = 6459
-    _globals["_SHAFTLINE"]._serialized_start = 6461
-    _globals["_SHAFTLINE"]._serialized_end = 6552
-    _globals["_MECHANICALSYSTEM"]._serialized_start = 6554
-    _globals["_MECHANICALSYSTEM"]._serialized_end = 6630
-    _globals["_ELECTRICSYSTEM"]._serialized_start = 6632
-    _globals["_ELECTRICSYSTEM"]._serialized_end = 6709
-    _globals["_FUELSTORAGE"]._serialized_start = 6711
-    _globals["_FUELSTORAGE"]._serialized_end = 6800
-    _globals["_MACHINERYSYSTEM"]._serialized_start = 6803
-    _globals["_MACHINERYSYSTEM"]._serialized_end = 7313
-    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_start = 7255
-    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_end = 7313
+    _globals["_GEAR"]._serialized_end = 1373
+    _globals["_FUEL"]._serialized_start = 1375
+    _globals["_FUEL"]._serialized_end = 1495
+    _globals["_ENGINE"]._serialized_start = 1498
+    _globals["_ENGINE"]._serialized_end = 2284
+    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_start = 2134
+    _globals["_ENGINE_NOXCALCULATIONMETHOD"]._serialized_end = 2203
+    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_start = 2205
+    _globals["_ENGINE_ENGINECYCLETYPE"]._serialized_end = 2284
+    _globals["_COGAS"]._serialized_start = 2287
+    _globals["_COGAS"]._serialized_end = 2890
+    _globals["_ELECTRICMACHINE"]._serialized_start = 2893
+    _globals["_ELECTRICMACHINE"]._serialized_end = 3113
+    _globals["_BATTERY"]._serialized_start = 3116
+    _globals["_BATTERY"]._serialized_end = 3515
+    _globals["_ELECTRICCOMPONENT"]._serialized_start = 3518
+    _globals["_ELECTRICCOMPONENT"]._serialized_end = 3715
+    _globals["_FUELCELL"]._serialized_start = 3718
+    _globals["_FUELCELL"]._serialized_end = 4031
+    _globals["_PROPELLER"]._serialized_start = 4034
+    _globals["_PROPELLER"]._serialized_end = 4197
+    _globals["_BUSBREAKER"]._serialized_start = 4199
+    _globals["_BUSBREAKER"]._serialized_end = 4235
+    _globals["_SUPERCAPACITOR"]._serialized_start = 4238
+    _globals["_SUPERCAPACITOR"]._serialized_end = 4496
+    _globals["_MECHANICALCOMPONENT"]._serialized_start = 4499
+    _globals["_MECHANICALCOMPONENT"]._serialized_end = 4698
+    _globals["_SUBSYSTEM"]._serialized_start = 4701
+    _globals["_SUBSYSTEM"]._serialized_end = 6506
+    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_start = 5815
+    _globals["_SUBSYSTEM_POWERTYPE"]._serialized_end = 5930
+    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_start = 5933
+    _globals["_SUBSYSTEM_COMPONENTTYPE"]._serialized_end = 6506
+    _globals["_SWITCHBOARD"]._serialized_start = 6508
+    _globals["_SWITCHBOARD"]._serialized_end = 6602
+    _globals["_SHAFTLINE"]._serialized_start = 6604
+    _globals["_SHAFTLINE"]._serialized_end = 6695
+    _globals["_MECHANICALSYSTEM"]._serialized_start = 6697
+    _globals["_MECHANICALSYSTEM"]._serialized_end = 6773
+    _globals["_ELECTRICSYSTEM"]._serialized_start = 6775
+    _globals["_ELECTRICSYSTEM"]._serialized_end = 6852
+    _globals["_FUELSTORAGE"]._serialized_start = 6854
+    _globals["_FUELSTORAGE"]._serialized_end = 6943
+    _globals["_MACHINERYSYSTEM"]._serialized_start = 6946
+    _globals["_MACHINERYSYSTEM"]._serialized_end = 7456
+    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_start = 7398
+    _globals["_MACHINERYSYSTEM_PROPULSIONTYPE"]._serialized_end = 7456
 # @@protoc_insertion_point(module_scope)
```

### Comparing `MachSysS-0.6.5/MachSysS/system_structure_pb2.pyi` & `machsyss-0.6.6/MachSysS/system_structure_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -233,38 +233,42 @@
         "name",
         "gear_ratio",
         "rated_power_kw",
         "rated_speed_rpm",
         "efficiency",
         "order_from_switchboard_or_shaftline",
         "unit_price_usd",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     GEAR_RATIO_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     RATED_SPEED_RPM_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     gear_ratio: float
     rated_power_kw: float
     rated_speed_rpm: float
     efficiency: Efficiency
     order_from_switchboard_or_shaftline: int
     unit_price_usd: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         gear_ratio: _Optional[float] = ...,
         rated_power_kw: _Optional[float] = ...,
         rated_speed_rpm: _Optional[float] = ...,
         efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
         unit_price_usd: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class Fuel(_message.Message):
     __slots__ = ("fuel_type", "fuel_origin")
     FUEL_TYPE_FIELD_NUMBER: _ClassVar[int]
     FUEL_ORIGIN_FIELD_NUMBER: _ClassVar[int]
     fuel_type: FuelType
@@ -287,14 +291,15 @@
         "pilot_fuel",
         "nox_calculation_method",
         "emission_curves",
         "engine_cycle_type",
         "unit_price_usd",
         "start_delay_s",
         "turn_off_power_kw",
+        "uid",
     )
 
     class NOxCalculationMethod(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         TIER_2: _ClassVar[Engine.NOxCalculationMethod]
         TIER_1: _ClassVar[Engine.NOxCalculationMethod]
         TIER_3: _ClassVar[Engine.NOxCalculationMethod]
@@ -326,28 +331,30 @@
     PILOT_FUEL_FIELD_NUMBER: _ClassVar[int]
     NOX_CALCULATION_METHOD_FIELD_NUMBER: _ClassVar[int]
     EMISSION_CURVES_FIELD_NUMBER: _ClassVar[int]
     ENGINE_CYCLE_TYPE_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
     START_DELAY_S_FIELD_NUMBER: _ClassVar[int]
     TURN_OFF_POWER_KW_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     rated_power_kw: float
     rated_speed_rpm: float
     bsfc: BSFC
     main_fuel: Fuel
     order_from_switchboard_or_shaftline: int
     pilot_bsfc: BSFC
     pilot_fuel: Fuel
     nox_calculation_method: Engine.NOxCalculationMethod
     emission_curves: _containers.RepeatedCompositeFieldContainer[EmissionCurve]
     engine_cycle_type: Engine.EngineCycleType
     unit_price_usd: float
     start_delay_s: float
     turn_off_power_kw: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         rated_speed_rpm: _Optional[float] = ...,
         bsfc: _Optional[_Union[BSFC, _Mapping]] = ...,
         main_fuel: _Optional[_Union[Fuel, _Mapping]] = ...,
@@ -358,14 +365,15 @@
             _Union[Engine.NOxCalculationMethod, str]
         ] = ...,
         emission_curves: _Optional[_Iterable[_Union[EmissionCurve, _Mapping]]] = ...,
         engine_cycle_type: _Optional[_Union[Engine.EngineCycleType, str]] = ...,
         unit_price_usd: _Optional[float] = ...,
         start_delay_s: _Optional[float] = ...,
         turn_off_power_kw: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class COGAS(_message.Message):
     __slots__ = (
         "name",
         "rated_power_kw",
         "rated_speed_rpm",
@@ -375,41 +383,44 @@
         "fuel",
         "order_from_switchboard_or_shaftline",
         "nox_calculation_method",
         "emission_curves",
         "unit_price_usd",
         "start_delay_s",
         "turn_off_power_kw",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     RATED_SPEED_RPM_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
     GAS_TURBINE_POWER_CURVE_FIELD_NUMBER: _ClassVar[int]
     STEAM_TURBINE_POWER_CURVE_FIELD_NUMBER: _ClassVar[int]
     FUEL_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     NOX_CALCULATION_METHOD_FIELD_NUMBER: _ClassVar[int]
     EMISSION_CURVES_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
     START_DELAY_S_FIELD_NUMBER: _ClassVar[int]
     TURN_OFF_POWER_KW_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     rated_power_kw: float
     rated_speed_rpm: float
     efficiency: Efficiency
     gas_turbine_power_curve: PowerCurve
     steam_turbine_power_curve: PowerCurve
     fuel: Fuel
     order_from_switchboard_or_shaftline: int
     nox_calculation_method: Engine.NOxCalculationMethod
     emission_curves: _containers.RepeatedCompositeFieldContainer[EmissionCurve]
     unit_price_usd: float
     start_delay_s: float
     turn_off_power_kw: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         rated_speed_rpm: _Optional[float] = ...,
         efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
         gas_turbine_power_curve: _Optional[_Union[PowerCurve, _Mapping]] = ...,
@@ -419,45 +430,50 @@
         nox_calculation_method: _Optional[
             _Union[Engine.NOxCalculationMethod, str]
         ] = ...,
         emission_curves: _Optional[_Iterable[_Union[EmissionCurve, _Mapping]]] = ...,
         unit_price_usd: _Optional[float] = ...,
         start_delay_s: _Optional[float] = ...,
         turn_off_power_kw: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class ElectricMachine(_message.Message):
     __slots__ = (
         "name",
         "rated_power_kw",
         "rated_speed_rpm",
         "efficiency",
         "order_from_switchboard_or_shaftline",
         "unit_price_usd",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     RATED_SPEED_RPM_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     rated_power_kw: float
     rated_speed_rpm: float
     efficiency: Efficiency
     order_from_switchboard_or_shaftline: int
     unit_price_usd: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         rated_speed_rpm: _Optional[float] = ...,
         efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
         unit_price_usd: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class Battery(_message.Message):
     __slots__ = (
         "name",
         "energy_capacity_kwh",
         "rated_charging_rate_c",
@@ -466,146 +482,162 @@
         "efficiency_discharging",
         "initial_state_of_charge",
         "order_from_switchboard_or_shaftline",
         "unit_price_usd",
         "self_discharge_percent_per_day",
         "state_of_energy_minimum",
         "state_of_energy_maximum",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     ENERGY_CAPACITY_KWH_FIELD_NUMBER: _ClassVar[int]
     RATED_CHARGING_RATE_C_FIELD_NUMBER: _ClassVar[int]
     RATED_DISCHARGING_RATE_C_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_CHARGING_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_DISCHARGING_FIELD_NUMBER: _ClassVar[int]
     INITIAL_STATE_OF_CHARGE_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
     SELF_DISCHARGE_PERCENT_PER_DAY_FIELD_NUMBER: _ClassVar[int]
     STATE_OF_ENERGY_MINIMUM_FIELD_NUMBER: _ClassVar[int]
     STATE_OF_ENERGY_MAXIMUM_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     energy_capacity_kwh: float
     rated_charging_rate_c: float
     rated_discharging_rate_c: float
     efficiency_charging: float
     efficiency_discharging: float
     initial_state_of_charge: float
     order_from_switchboard_or_shaftline: int
     unit_price_usd: float
     self_discharge_percent_per_day: float
     state_of_energy_minimum: float
     state_of_energy_maximum: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         energy_capacity_kwh: _Optional[float] = ...,
         rated_charging_rate_c: _Optional[float] = ...,
         rated_discharging_rate_c: _Optional[float] = ...,
         efficiency_charging: _Optional[float] = ...,
         efficiency_discharging: _Optional[float] = ...,
         initial_state_of_charge: _Optional[float] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
         unit_price_usd: _Optional[float] = ...,
         self_discharge_percent_per_day: _Optional[float] = ...,
         state_of_energy_minimum: _Optional[float] = ...,
         state_of_energy_maximum: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class ElectricComponent(_message.Message):
     __slots__ = (
         "name",
         "rated_power_kw",
         "efficiency",
         "order_from_switchboard_or_shaftline",
         "unit_price_usd",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     rated_power_kw: float
     efficiency: Efficiency
     order_from_switchboard_or_shaftline: int
     unit_price_usd: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
         unit_price_usd: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class FuelCell(_message.Message):
     __slots__ = (
         "name",
         "rated_power_kw",
         "efficiency",
         "order_from_switchboard_or_shaftline",
         "fuel",
         "unit_price_usd",
         "number_modules",
         "power_minimum_specific",
         "start_delay_s",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     FUEL_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
     NUMBER_MODULES_FIELD_NUMBER: _ClassVar[int]
     POWER_MINIMUM_SPECIFIC_FIELD_NUMBER: _ClassVar[int]
     START_DELAY_S_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     rated_power_kw: float
     efficiency: Efficiency
     order_from_switchboard_or_shaftline: int
     fuel: Fuel
     unit_price_usd: float
     number_modules: int
     power_minimum_specific: float
     start_delay_s: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
         fuel: _Optional[_Union[Fuel, _Mapping]] = ...,
         unit_price_usd: _Optional[float] = ...,
         number_modules: _Optional[int] = ...,
         power_minimum_specific: _Optional[float] = ...,
         start_delay_s: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class Propeller(_message.Message):
     __slots__ = (
         "name",
         "efficiency",
         "propulsor_id",
         "order_from_switchboard_or_shaftline",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
     PROPULSOR_ID_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     efficiency: Efficiency
     propulsor_id: int
     order_from_switchboard_or_shaftline: int
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
         propulsor_id: _Optional[int] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class BusBreaker(_message.Message):
     __slots__ = ("switchboard_to",)
     SWITCHBOARD_TO_FIELD_NUMBER: _ClassVar[int]
     switchboard_to: int
     def __init__(self, switchboard_to: _Optional[int] = ...) -> None: ...
@@ -616,68 +648,76 @@
         "energy_capacity_wh",
         "rated_power_kw",
         "efficiency_charging",
         "efficiency_discharging",
         "initial_state_of_charge",
         "order_from_switchboard_or_shaftline",
         "unit_price_usd",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     ENERGY_CAPACITY_WH_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_CHARGING_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_DISCHARGING_FIELD_NUMBER: _ClassVar[int]
     INITIAL_STATE_OF_CHARGE_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     energy_capacity_wh: float
     rated_power_kw: float
     efficiency_charging: float
     efficiency_discharging: float
     initial_state_of_charge: float
     order_from_switchboard_or_shaftline: int
     unit_price_usd: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         energy_capacity_wh: _Optional[float] = ...,
         rated_power_kw: _Optional[float] = ...,
         efficiency_charging: _Optional[float] = ...,
         efficiency_discharging: _Optional[float] = ...,
         initial_state_of_charge: _Optional[float] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
         unit_price_usd: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class MechanicalComponent(_message.Message):
     __slots__ = (
         "name",
         "rated_power_kw",
         "efficiency",
         "order_from_switchboard_or_shaftline",
         "unit_price_usd",
+        "uid",
     )
     NAME_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     EFFICIENCY_FIELD_NUMBER: _ClassVar[int]
     ORDER_FROM_SWITCHBOARD_OR_SHAFTLINE_FIELD_NUMBER: _ClassVar[int]
     UNIT_PRICE_USD_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     name: str
     rated_power_kw: float
     efficiency: Efficiency
     order_from_switchboard_or_shaftline: int
     unit_price_usd: float
+    uid: str
     def __init__(
         self,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         efficiency: _Optional[_Union[Efficiency, _Mapping]] = ...,
         order_from_switchboard_or_shaftline: _Optional[int] = ...,
         unit_price_usd: _Optional[float] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class Subsystem(_message.Message):
     __slots__ = (
         "gear",
         "engine",
         "electric_machine",
@@ -695,14 +735,15 @@
         "component_type",
         "name",
         "rated_power_kw",
         "rated_speed_rpm",
         "ramp_up_rate_limit_percent_per_second",
         "ramp_down_rate_limit_percent_per_second",
         "base_load_order",
+        "uid",
     )
 
     class PowerType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         NONE1: _ClassVar[Subsystem.PowerType]
         POWER_SOURCE: _ClassVar[Subsystem.PowerType]
         POWER_CONSUMER: _ClassVar[Subsystem.PowerType]
@@ -797,14 +838,15 @@
     COMPONENT_TYPE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     RATED_POWER_KW_FIELD_NUMBER: _ClassVar[int]
     RATED_SPEED_RPM_FIELD_NUMBER: _ClassVar[int]
     RAMP_UP_RATE_LIMIT_PERCENT_PER_SECOND_FIELD_NUMBER: _ClassVar[int]
     RAMP_DOWN_RATE_LIMIT_PERCENT_PER_SECOND_FIELD_NUMBER: _ClassVar[int]
     BASE_LOAD_ORDER_FIELD_NUMBER: _ClassVar[int]
+    UID_FIELD_NUMBER: _ClassVar[int]
     gear: Gear
     engine: Engine
     electric_machine: ElectricMachine
     transformer: ElectricComponent
     converter1: ElectricComponent
     converter2: ElectricComponent
     battery: Battery
@@ -818,14 +860,15 @@
     component_type: Subsystem.ComponentType
     name: str
     rated_power_kw: float
     rated_speed_rpm: float
     ramp_up_rate_limit_percent_per_second: float
     ramp_down_rate_limit_percent_per_second: float
     base_load_order: int
+    uid: str
     def __init__(
         self,
         gear: _Optional[_Union[Gear, _Mapping]] = ...,
         engine: _Optional[_Union[Engine, _Mapping]] = ...,
         electric_machine: _Optional[_Union[ElectricMachine, _Mapping]] = ...,
         transformer: _Optional[_Union[ElectricComponent, _Mapping]] = ...,
         converter1: _Optional[_Union[ElectricComponent, _Mapping]] = ...,
@@ -841,14 +884,15 @@
         component_type: _Optional[_Union[Subsystem.ComponentType, str]] = ...,
         name: _Optional[str] = ...,
         rated_power_kw: _Optional[float] = ...,
         rated_speed_rpm: _Optional[float] = ...,
         ramp_up_rate_limit_percent_per_second: _Optional[float] = ...,
         ramp_down_rate_limit_percent_per_second: _Optional[float] = ...,
         base_load_order: _Optional[int] = ...,
+        uid: _Optional[str] = ...,
     ) -> None: ...
 
 class Switchboard(_message.Message):
     __slots__ = ("switchboard_id", "subsystems")
     SWITCHBOARD_ID_FIELD_NUMBER: _ClassVar[int]
     SUBSYSTEMS_FIELD_NUMBER: _ClassVar[int]
     switchboard_id: int
```

### Comparing `MachSysS-0.6.5/MachSysS/utility.py` & `machsyss-0.6.6/MachSysS/utility.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/MachSysS.egg-info/PKG-INFO` & `machsyss-0.6.6/MachSysS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MachSysS
-Version: 0.6.5
+Version: 0.6.6
 Summary: Machinery System Structure for interface
 Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS protobuf system structure
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `MachSysS-0.6.5/MachSysS.egg-info/SOURCES.txt` & `machsyss-0.6.6/MachSysS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/PKG-INFO` & `machsyss-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MachSysS
-Version: 0.6.5
+Version: 0.6.6
 Summary: Machinery System Structure for interface
 Home-page: https://github.com/SINTEF/FEEMS
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: FEEMS protobuf system structure
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `MachSysS-0.6.5/settings.ini` & `machsyss-0.6.6/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 description = Machinery System Structure for interface
 keywords = FEEMS protobuf system structure
 user = keviny
 author = Kevin Koosup Yum
 author_email = kevinkoosup.yum@sintef.no
 copyright = SINTEF Ocean
-version = 0.6.5
+version = 0.6.6
 min_python = 3.10
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
```

### Comparing `MachSysS-0.6.5/setup.py` & `machsyss-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/tests/utility.py` & `machsyss-0.6.6/tests/utility.py`

 * *Files identical despite different names*

### Comparing `MachSysS-0.6.5/tests/utility_compare_proto.py` & `machsyss-0.6.6/tests/utility_compare_proto.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,14 +153,15 @@
     """
     non_component_attribute_keys = [
         "powerType",
         "componentType",
         "name",
         "ratedPowerKw",
         "ratedSpeedRpm",
+        "uid",
     ]
     subsystem1_dict = MessageToDict(subsystem1)
     subsystem2_dict = MessageToDict(subsystem2)
     subsystem1_dict_non_components = reduce(
         lambda acc, key: (
             {**acc, **{key: subsystem1_dict.pop(key)}}
             if key in subsystem1_dict
```

