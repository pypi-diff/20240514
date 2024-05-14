# Comparing `tmp/feems-0.10.6.tar.gz` & `tmp/feems-0.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feems-0.10.6.tar", max compression
+gzip compressed data, was "feems-0.10.7.tar", max compression
```

## Comparing `feems-0.10.6.tar` & `feems-0.10.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1063 2024-04-09 13:01:21.405516 feems-0.10.6/LICENSE
--rw-r--r--   0        0        0    10244 2024-04-09 13:01:21.405516 feems-0.10.6/feems/.DS_Store
--rw-r--r--   0        0        0      394 2024-04-09 13:01:21.405516 feems-0.10.6/feems/__init__.py
--rw-r--r--   0        0        0     6148 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/.DS_Store
--rw-r--r--   0        0        0      545 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/__init__.py
--rw-r--r--   0        0        0    17594 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/component_base.py
--rw-r--r--   0        0        0    37115 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/component_electric.py
--rw-r--r--   0        0        0    27269 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/component_mechanical.py
--rw-r--r--   0        0        0    56446 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/node.py
--rw-r--r--   0        0        0    10356 2024-04-09 13:01:21.405516 feems-0.10.6/feems/components_model/utility.py
--rw-r--r--   0        0        0      555 2024-04-09 13:01:21.405516 feems-0.10.6/feems/constant.py
--rw-r--r--   0        0        0        0 2024-04-09 13:01:21.405516 feems-0.10.6/feems/emission.py
--rw-r--r--   0        0        0      133 2024-04-09 13:01:21.405516 feems-0.10.6/feems/exceptions.py
--rw-r--r--   0        0        0    23941 2024-04-09 13:01:21.405516 feems-0.10.6/feems/fuel.py
--rw-r--r--   0        0        0     6148 2024-04-09 13:01:21.405516 feems-0.10.6/feems/package_data/.DS_Store
--rw-r--r--   0        0        0     2477 2024-04-09 13:01:21.405516 feems-0.10.6/feems/package_data/fuel_eu_fuel_table.csv
--rw-r--r--   0        0        0     1060 2024-04-09 13:01:21.405516 feems-0.10.6/feems/package_data/fuel_imo_table.csv
--rw-r--r--   0        0        0        0 2024-04-09 13:01:21.405516 feems-0.10.6/feems/py.typed
--rw-r--r--   0        0        0     7686 2024-04-09 13:01:21.405516 feems-0.10.6/feems/runsimulation.py
--rw-r--r--   0        0        0     6651 2024-04-09 13:01:21.405516 feems-0.10.6/feems/simulation_interface.py
--rw-r--r--   0        0        0    58164 2024-04-09 13:01:21.405516 feems-0.10.6/feems/system_model.py
--rw-r--r--   0        0        0     7656 2024-04-09 13:01:21.405516 feems-0.10.6/feems/types_for_feems.py
--rw-r--r--   0        0        0      700 2024-04-09 13:01:21.405516 feems-0.10.6/pyproject.toml
--rw-r--r--   0        0        0      944 2024-04-09 13:01:21.405516 feems-0.10.6/readme.md
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 feems-0.10.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-14 10:59:17.162897 feems-0.10.7/LICENSE
+-rw-r--r--   0        0        0    10244 2024-05-14 10:59:17.162897 feems-0.10.7/feems/.DS_Store
+-rw-r--r--   0        0        0      394 2024-05-14 10:59:17.162897 feems-0.10.7/feems/__init__.py
+-rw-r--r--   0        0        0     6148 2024-05-14 10:59:17.162897 feems-0.10.7/feems/components_model/.DS_Store
+-rw-r--r--   0        0        0      545 2024-05-14 10:59:17.162897 feems-0.10.7/feems/components_model/__init__.py
+-rw-r--r--   0        0        0    17970 2024-05-14 10:59:17.162897 feems-0.10.7/feems/components_model/component_base.py
+-rw-r--r--   0        0        0    38019 2024-05-14 10:59:17.162897 feems-0.10.7/feems/components_model/component_electric.py
+-rw-r--r--   0        0        0    27745 2024-05-14 10:59:17.162897 feems-0.10.7/feems/components_model/component_mechanical.py
+-rw-r--r--   0        0        0    56446 2024-05-14 10:59:17.162897 feems-0.10.7/feems/components_model/node.py
+-rw-r--r--   0        0        0    10356 2024-05-14 10:59:17.162897 feems-0.10.7/feems/components_model/utility.py
+-rw-r--r--   0        0        0      555 2024-05-14 10:59:17.162897 feems-0.10.7/feems/constant.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:59:17.162897 feems-0.10.7/feems/emission.py
+-rw-r--r--   0        0        0      133 2024-05-14 10:59:17.162897 feems-0.10.7/feems/exceptions.py
+-rw-r--r--   0        0        0    23941 2024-05-14 10:59:17.162897 feems-0.10.7/feems/fuel.py
+-rw-r--r--   0        0        0     6148 2024-05-14 10:59:17.162897 feems-0.10.7/feems/package_data/.DS_Store
+-rw-r--r--   0        0        0     2477 2024-05-14 10:59:17.162897 feems-0.10.7/feems/package_data/fuel_eu_fuel_table.csv
+-rw-r--r--   0        0        0     1060 2024-05-14 10:59:17.162897 feems-0.10.7/feems/package_data/fuel_imo_table.csv
+-rw-r--r--   0        0        0        0 2024-05-14 10:59:17.162897 feems-0.10.7/feems/py.typed
+-rw-r--r--   0        0        0     7686 2024-05-14 10:59:17.162897 feems-0.10.7/feems/runsimulation.py
+-rw-r--r--   0        0        0     6651 2024-05-14 10:59:17.162897 feems-0.10.7/feems/simulation_interface.py
+-rw-r--r--   0        0        0    58164 2024-05-14 10:59:17.162897 feems-0.10.7/feems/system_model.py
+-rw-r--r--   0        0        0     7656 2024-05-14 10:59:17.162897 feems-0.10.7/feems/types_for_feems.py
+-rw-r--r--   0        0        0      700 2024-05-14 10:59:17.162897 feems-0.10.7/pyproject.toml
+-rw-r--r--   0        0        0      944 2024-05-14 10:59:17.162897 feems-0.10.7/readme.md
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 feems-0.10.7/PKG-INFO
```

### Comparing `feems-0.10.6/LICENSE` & `feems-0.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/.DS_Store` & `feems-0.10.7/feems/.DS_Store`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/components_model/.DS_Store` & `feems-0.10.7/feems/components_model/.DS_Store`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/components_model/__init__.py` & `feems-0.10.7/feems/components_model/__init__.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/components_model/component_base.py` & `feems-0.10.7/feems/components_model/component_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Union, List, Tuple, Optional, TypeVar, Dict
 from dataclasses import dataclass, field
+from uuid import uuid4
 
 import numpy as np
 import pandas as pd
 from scipy.interpolate import PchipInterpolator
 from scipy.optimize import newton, root, least_squares
 
 from .utility import (
@@ -48,23 +49,26 @@
     def __init__(
         self,
         name: str,
         type_: TypeComponent,
         power_type: TypePower,
         rated_power: Power_kW = Power_kW(0.0),
         rated_speed: Speed_rpm = Speed_rpm(0.0),
+        uid: Optional[str] = None,
     ):
         self.type = type_
         self.power_type = power_type
         self.name = name
         self.rated_power = rated_power
         self.rated_speed = rated_speed
         self.status = np.ones(1).astype(bool)  # Status on/off
         self.power_input = np.array([0])  # power input
         self.power_output = np.array([0])  # power output
+        # if uid is not given, create a random uid
+        self.uid = str(uuid4()) if uid is None else uid
 
     def get_type_name(self) -> str:
         return self.type.name
 
     def get_load(self, power: Optional[T] = None) -> T:
         if power is None:
             return np.abs(self.power_input) / self.rated_power
@@ -90,17 +94,23 @@
         type_: TypeComponent,
         power_type: TypePower,
         name: str = "",
         rated_power: Power_kW = Power_kW(0.0),
         eff_curve: np.ndarray = np.array([1]),
         rated_speed: Speed_rpm = Speed_rpm(0.0),
         file_name: str = None,
+        uid: Optional[str] = None,
     ):
         super(BasicComponent, self).__init__(
-            name, type_, power_type, rated_power, rated_speed
+            name=name, 
+            type_=type_, 
+            power_type=power_type, 
+            rated_power=rated_power, 
+            rated_speed=rated_speed, 
+            uid=uid
         )
         if file_name is not None:
             df = pd.read_csv(file_name, index_col=0)
             self.rated_power = df["Rated Power"].values[0]
             self.rated_speed = df["Rated Speed"].values[0]
             (
                 self._efficiency_interp,
@@ -413,14 +423,15 @@
         self,
         type_: TypeComponent,
         power_type: TypePower,
         name: str,
         components: List[BasicComponent],
         rated_power: Power_kW = None,
         rated_speed: Speed_rpm = None,
+        uid: Optional[str] = None,
     ):
         self.component_names = []
         self.components = components
         #: Calculate the total efficiency
         load = np.arange(0, 1.01, 0.1)
         efficiency_total = np.ones(len(load))
         for i, component in enumerate(components):
@@ -441,8 +452,9 @@
         super(SerialSystem, self).__init__(
             name=name,
             type_=type_,
             power_type=power_type,
             rated_power=rated_power,
             rated_speed=rated_speed,
             eff_curve=efficiency_points,
+            uid=uid,
         )
```

### Comparing `feems-0.10.6/feems/components_model/component_electric.py` & `feems-0.10.7/feems/components_model/component_electric.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,23 +48,25 @@
         name: str = "",
         rated_power: Power_kW = Power_kW(1),
         eff_curve: np.ndarray = np.array([1]),
         power_type: TypePower = TypePower.NONE,
         rated_speed: Speed_rpm = Speed_rpm(0),
         switchboard_id: SwbId = SwbId(0),
         file_name: str = None,
+        uid: Optional[str] = None,
     ):
         super().__init__(
             type_=type_,
             power_type=power_type,
             name=name,
             rated_power=rated_power,
             rated_speed=rated_speed,
             eff_curve=eff_curve,
             file_name=file_name,
+            uid=uid,
         )
         self.power_type = power_type
         if power_type in [
             TypePower.POWER_SOURCE,
             TypePower.PTI_PTO,
             TypePower.ENERGY_STORAGE,
         ]:
@@ -87,23 +89,25 @@
         name: str,
         rated_power: Power_kW,
         rated_speed: Speed_rpm,
         power_type: TypePower = TypePower.NONE,
         switchboard_id: SwbId = SwbId(0),
         number_poles: int = 1,
         eff_curve: np.ndarray = np.ones(1),
+        uid: Optional[str] = None,
     ):
         super(ElectricMachine, self).__init__(
             type_=type_,
             name=name,
             power_type=power_type,
             rated_power=rated_power,
             rated_speed=rated_speed,
             eff_curve=eff_curve,
             switchboard_id=switchboard_id,
+            uid=uid,
         )
         self.number_of_poles = number_poles
 
     def get_shaft_power_load_from_electric_power(
         self,
         power_electric: Union[float, np.ndarray],
         strict_power_balance: bool = False,
@@ -199,22 +203,24 @@
         rated_capacity_kwh: float,
         charging_rate_c: float,
         discharge_rate_c: float,
         soc0: float = 0.80,
         eff_charging: float = 0.975,
         eff_discharging: float = 0.975,
         switchboard_id: SwbId = SwbId(0),
+        uid: Optional[str] = None,
     ):
         rated_power = Power_kW(rated_capacity_kwh * discharge_rate_c)
         super().__init__(
             TypeComponent.BATTERY,
             name,
             rated_power,
             power_type=TypePower.ENERGY_STORAGE,
             switchboard_id=switchboard_id,
+            uid=uid,
         )
         self.rated_capacity_kWh = rated_capacity_kwh
         self.charging_rate_C = charging_rate_c
         self.discharging_rate_C = discharge_rate_c
         self.soc0 = soc0
         self.eff_charging = eff_charging
         self.eff_discharging = eff_discharging
@@ -333,17 +339,24 @@
         type_: TypeComponent,
         name: str,
         power_type: TypePower,
         components: list,
         switchboard_id: SwbId,
         rated_power: Power_kW,
         rated_speed: Speed_rpm = Speed_rpm(0),
+        uid: Optional[str] = None,
     ):
         super(SerialSystemElectric, self).__init__(
-            type_, power_type, name, components, rated_power, rated_speed
+            type_=type_, 
+            power_type=power_type, 
+            name=name, 
+            components=components, 
+            rated_power=rated_power,
+            rated_speed=rated_speed,
+            uid=uid,
         )
 
         #: Set the load sharing mode 0 as default value if the component is either a power source,
         #: PTI/PTO or ESS
         if self.power_type in [
             TypePower.POWER_SOURCE,
             TypePower.PTI_PTO,
@@ -357,21 +370,23 @@
     def __init__(
         self,
         name: str,
         rated_power: Power_kW,
         eff_curve: np.ndarray,
         fuel_type: TypeFuel = TypeFuel.HYDROGEN,
         fuel_origin: FuelOrigin = FuelOrigin.RENEWABLE_NON_BIO,
+        uid: Optional[str] = None,
     ):
         super(FuelCell, self).__init__(
             type_=TypeComponent.FUEL_CELL,
             power_type=TypePower.POWER_SOURCE,
             name=name,
             rated_power=rated_power,
             eff_curve=eff_curve,
+            uid=uid,
         )
         self.fuel_type = fuel_type
         self.fuel_origin = fuel_origin
 
     def get_fuel_cell_run_point(
         self,
         power_out_kw: np.ndarray = None,
@@ -437,22 +452,24 @@
     def __init__(
         self,
         name: str,
         fuel_cell_module: FuelCell,
         converter: ElectricComponent,
         switchboard_id: SwbId,
         number_modules: int = 1,
+        uid: Optional[str] = None,
     ):
         super(FuelCellSystem, self).__init__(
             name=name,
             type_=TypeComponent.FUEL_CELL_SYSTEM,
             rated_power=converter.rated_power,
             eff_curve=converter._efficiency_points,
             power_type=TypePower.POWER_SOURCE,
             switchboard_id=switchboard_id,
+            uid=uid,
         )
         self.converter = converter
         self.fuel_cell = fuel_cell_module
         self.number_modules = number_modules
 
     def get_fuel_cell_run_point(
         self,
@@ -511,24 +528,26 @@
 
     def __init__(
         self,
         name: str,
         battery: Battery,
         converter: ElectricComponent,
         switchboard_id: SwbId,
+        uid: Optional[str] = None,
     ):
         super().__init__(
             name=name,
             rated_capacity_kwh=battery.rated_capacity_kWh,
             charging_rate_c=battery.charging_rate_C,
             discharge_rate_c=battery.discharging_rate_C,
             soc0=battery.soc0,
             eff_charging=battery.eff_charging,
             eff_discharging=battery.eff_discharging,
             switchboard_id=switchboard_id,
+            uid=uid,
         )
         self.type = TypeComponent.BATTERY_SYSTEM
         self.rated_power = converter.rated_power
         self.converter = converter
         self.battery = battery
 
     def get_power_input_from_bidirectional_output(
@@ -584,21 +603,23 @@
 
     def __init__(
         self,
         name: str,
         aux_engine: Engine,
         generator: ElectricMachine,
         rectifier: ElectricComponent = None,
+        uid: Optional[str] = None,
     ):
         super(Genset, self).__init__(
             name=name,
             type_=TypeComponent.GENSET,
             power_type=TypePower.POWER_SOURCE,
             rated_power=generator.rated_power,
             rated_speed=generator.rated_speed,
+            uid=uid,
         )
         self.fuel_type = aux_engine.fuel_type
         self.aux_engine = aux_engine
         #: For DC genset, rectifier is included
         if type(rectifier) is ElectricComponent:
             generator_rectifier = SerialSystemElectric(
                 name="{:s} with rectifier".format(generator.name),
@@ -662,23 +683,25 @@
         self,
         name: str,
         components: list,
         switchboard_id: SwbId,
         rated_power: Power_kW,
         rated_speed: Speed_rpm = Speed_rpm(0),
         shaft_line_id: int = 1,
+        uid: Optional[str] = None,
     ):
         super(PTIPTO, self).__init__(
             TypeComponent.PTI_PTO_SYSTEM,
             name,
             TypePower.PTI_PTO,
             components,
             switchboard_id,
             rated_power,
             rated_speed,
+            uid=uid,
         )
         self.shaft_line_id = shaft_line_id
         self.full_pti_mode = np.zeros(1).astype(bool)
 
 
 class SuperCapacitor(ElectricComponent):
     """
@@ -687,32 +710,35 @@
     :param name: Component name
     :param rated_capacity_wh: Rated capacity in Wh
     :param rated_power: Rated power in kW
     :param soc0: State of charge in percentage
     :param eff_charging: Efficiency for charging in percentage
     :param eff_discharging: Efficiency for discharging in percentage
     :param switchboard_id: Switchboard ID
+    :param uid: Unique ID
     """
 
     def __init__(
         self,
         name: str,
         rated_capacity_wh: float,
         rated_power: Power_kW,
         soc0: float = 0.8,
         eff_charging: float = 0.995,
         eff_discharging: float = 0.995,
         switchboard_id: SwbId = SwbId(0),
+        uid: Optional[str] = None,
     ):
         super().__init__(
             TypeComponent.SUPERCAPACITOR,
             name,
             rated_power,
             power_type=TypePower.ENERGY_STORAGE,
             switchboard_id=switchboard_id,
+            uid=uid,
         )
         self.rated_capacity_Wh = rated_capacity_wh
         self.soc0 = soc0
         self.eff_charging = eff_charging
         self.eff_discharging = eff_discharging
 
     def get_energy_stored_kj(
@@ -817,23 +843,25 @@
 
     def __init__(
         self,
         name: str,
         supercapacitor: SuperCapacitor,
         converter: ElectricComponent,
         switchboard_id: SwbId,
+        uid: Optional[str] = None,
     ):
         super().__init__(
             name=name,
             rated_capacity_wh=supercapacitor.rated_capacity_Wh,
             rated_power=supercapacitor.rated_power,
             soc0=supercapacitor.soc0,
             eff_charging=supercapacitor.eff_charging,
             eff_discharging=supercapacitor.eff_discharging,
             switchboard_id=switchboard_id,
+            uid=uid,
         )
         self.converter = converter
         self.supercapacitor = supercapacitor
 
     def get_power_input_from_bidirectional_output(
         self, power_output: Union[float, np.ndarray], strict_power_balance: bool = False
     ) -> Tuple[Union[float, np.ndarray], Union[float, np.ndarray]]:
@@ -878,22 +906,27 @@
 
     :param name: Component name
     :param rated_power: Rated power in kW
     :param switchboard_id: Switchboard ID
     """
 
     def __init__(
-        self, name: str, rated_power: Power_kW, switchboard_id: SwbId = SwbId(0)
+        self, 
+        name: str, 
+        rated_power: Power_kW, 
+        switchboard_id: SwbId = SwbId(0),
+        uid: Optional[str] = None,
     ):
         super().__init__(
             TypeComponent.SHORE_POWER,
             name,
             rated_power,
             power_type=TypePower.POWER_SOURCE,
             switchboard_id=switchboard_id,
+            uid=uid,
         )
 
 
 class ShorePowerConnectionSystem(ShorePowerConnection):
     """
     Shore power connection class
 
@@ -925,21 +958,23 @@
     """
 
     def __init__(
         self,
         name: str,
         cogas: COGAS,
         generator: ElectricMachine,
+        uid: Optional[str] = None,
     ):
         super().__init__(
             name=name,
             type_=TypeComponent.COGES,
             power_type=TypePower.POWER_SOURCE,
             rated_power=generator.rated_power,
             rated_speed=generator.rated_speed,
+            uid=uid,
         )
         self.fuel_type = cogas.fuel_type
         self.cogas = cogas
         self.generator = generator
         self.switchboard_id = generator.switchboard_id
         self.status = np.ones(0).astype(bool)
         self.load_sharing_mode = np.zeros(1)
```

### Comparing `feems-0.10.6/feems/components_model/component_mechanical.py` & `feems-0.10.7/feems/components_model/component_mechanical.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,21 +68,23 @@
         rated_speed: Speed_rpm = Speed_rpm(0.0),
         bsfc_curve: np.ndarray = None,
         fuel_type: TypeFuel = TypeFuel.DIESEL,
         fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
         file_name: str = None,
         emissions_curves: List[EmissionCurve] = None,
         engine_cycle_type: EngineCycleType = EngineCycleType.DIESEL,
+        uid: Optional[str] = None,
     ):
         super(Engine, self).__init__(
             name=name,
             type_=type_,
             power_type=TypePower.POWER_SOURCE,
             rated_power=rated_power,
             rated_speed=rated_speed,
+            uid=uid,
         )
         self.fuel_type = fuel_type
         self.fuel_origin = fuel_origin
         self.engine_cycle_type = engine_cycle_type
         self._setup_bsfc(bsfc_curve, file_name)
         self._setup_emissions(emissions_curves)
         self._setup_nox(nox_calculation_method, rated_speed)
@@ -234,25 +236,27 @@
         bsfc_curve: np.ndarray = None,
         fuel_type: TypeFuel = TypeFuel.NATURAL_GAS,
         fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
         bspfc_curve: np.ndarray = None,
         pilot_fuel_type: TypeFuel.DIESEL,
         pilot_fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
         emissions_curves: List[EmissionCurve] = None,
+        uid: Optional[str] = None,
     ):
         super().__init__(
             type_=type_,
             nox_calculation_method=nox_calculation_method,
             name=name,
             rated_power=rated_power,
             rated_speed=rated_speed,
             bsfc_curve=bsfc_curve,
             fuel_type=fuel_type,
             fuel_origin=fuel_origin,
             emissions_curves=emissions_curves,
+            uid=uid,
         )
         self.bspfc_curve = bspfc_curve
         self.pilot_fuel_type = pilot_fuel_type
         self.pilot_fuel_origin = pilot_fuel_origin
         (
             self.specific_pilot_fuel_consumption_interp,
             self.specific_pilot_fuel_consumption_points,
@@ -317,21 +321,23 @@
     """
 
     def __init__(
         self,
         name,
         engine: Union[Engine, EngineDualFuel],
         shaft_line_id: int = 1,
+        uid: Optional[str] = None,
     ):
         super().__init__(
             name=name,
             power_type=TypePower.POWER_SOURCE,
             type_=TypeComponent.MAIN_ENGINE,
             rated_power=engine.rated_power,
             rated_speed=engine.rated_speed,
+            uid=uid,
         )
         self.engine = engine
         self.shaft_line_id = shaft_line_id
 
     @property
     def fuel_consumer_type_fuel_eu_maritime(self) -> FuelConsumerClassFuelEUMaritime:
         return self.engine.fuel_consumer_type_fuel_eu_maritime
@@ -388,33 +394,43 @@
         power_type: TypePower,
         name: str = "",
         rated_power: Power_kW = Power_kW(0),
         eff_curve: np.ndarray = np.array([1]),
         rated_speed: Speed_rpm = Speed_rpm(0),
         shaft_line_id: int = 1,
         file_name: str = None,
+        uid: Optional[str] = None,
     ):
         super(MechanicalPropulsionComponent, self).__init__(
-            type_, power_type, name, rated_power, eff_curve, rated_speed, file_name
+            type_=type_, 
+            power_type=power_type,
+            name=name,
+            rated_power=rated_power,
+            eff_curve=eff_curve,
+            rated_speed=rated_speed,
+            file_name=file_name,
+            uid=uid,
         )
         self.shaft_line_id = shaft_line_id
 
 
 class MainEngineWithGearBoxForMechanicalPropulsion(MainEngineForMechanicalPropulsion):
     def __init__(
         self,
         name: str,
         engine: Union[Engine, EngineDualFuel],
         gearbox: BasicComponent,
         shaft_line_id: int = 1,
+        uid: Optional[str] = None,
     ):
         super(MainEngineWithGearBoxForMechanicalPropulsion, self).__init__(
             name=name,
             engine=engine,
             shaft_line_id=shaft_line_id,
+            uid=uid,
         )
         self.gearbox = gearbox
 
     def get_engine_run_point_from_power_out_kw(
         self,
         power: np.ndarray = None,
         fuel_specified_by: FuelSpecifiedBy = FuelSpecifiedBy.IMO,
@@ -474,14 +490,15 @@
         rated_speed: Speed_rpm = Speed_rpm(0),
         gas_turbine_power_curve: np.ndarray = None,
         steam_turbine_power_curve: np.ndarray = None,
         fuel_type: TypeFuel = TypeFuel.DIESEL,
         fuel_origin: FuelOrigin = FuelOrigin.FOSSIL,
         emissions_curves: List[EmissionCurve] = None,
         nox_calculation_method: NOxCalculationMethod = NOxCalculationMethod.TIER_3,
+        uid: Optional[str] = None,
     ):
         """Constructor for COGES component"""
         # Validate the inputs for curves. The length of the curves should be the same and the x values should be the same.
         if (
             gas_turbine_power_curve is not None
             and steam_turbine_power_curve is not None
         ):
@@ -501,14 +518,15 @@
         super().__init__(
             type_=TypeComponent.COGAS,
             power_type=TypePower.POWER_SOURCE,
             name=name,
             rated_power=rated_power,
             eff_curve=eff_curve,
             rated_speed=rated_speed,
+            uid=uid,
         )
         self.gas_turbine_power_curve = gas_turbine_power_curve
         self.steam_turbine_power_curve = steam_turbine_power_curve
         if (
             self.gas_turbine_power_curve is not None
             and self.steam_turbine_power_curve is not None
         ):
```

### Comparing `feems-0.10.6/feems/components_model/node.py` & `feems-0.10.7/feems/components_model/node.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/components_model/utility.py` & `feems-0.10.7/feems/components_model/utility.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/constant.py` & `feems-0.10.7/feems/constant.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/fuel.py` & `feems-0.10.7/feems/fuel.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/package_data/.DS_Store` & `feems-0.10.7/feems/package_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/package_data/fuel_eu_fuel_table.csv` & `feems-0.10.7/feems/package_data/fuel_eu_fuel_table.csv`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/package_data/fuel_imo_table.csv` & `feems-0.10.7/feems/package_data/fuel_imo_table.csv`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/runsimulation.py` & `feems-0.10.7/feems/runsimulation.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/simulation_interface.py` & `feems-0.10.7/feems/simulation_interface.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/system_model.py` & `feems-0.10.7/feems/system_model.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/feems/types_for_feems.py` & `feems-0.10.7/feems/types_for_feems.py`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/pyproject.toml` & `feems-0.10.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feems"
-version = "0.10.6"
+version = "0.10.7"
 description = ""
 authors = ["Kevin Koosup Yum <kevinkoosup.yum@sintef.no>"]
 readme = "readme.md"
 include = ["feems/py.typed"]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `feems-0.10.6/readme.md` & `feems-0.10.7/readme.md`

 * *Files identical despite different names*

### Comparing `feems-0.10.6/PKG-INFO` & `feems-0.10.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feems
-Version: 0.10.6
+Version: 0.10.7
 Summary: 
 License: MIT
 Author: Kevin Koosup Yum
 Author-email: kevinkoosup.yum@sintef.no
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

