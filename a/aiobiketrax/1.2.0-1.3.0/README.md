# Comparing `tmp/aiobiketrax-1.2.0.tar.gz` & `tmp/aiobiketrax-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiobiketrax-1.2.0.tar", max compression
+gzip compressed data, was "aiobiketrax-1.3.0.tar", max compression
```

## Comparing `aiobiketrax-1.2.0.tar` & `aiobiketrax-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1057 2022-07-07 22:22:53.680609 aiobiketrax-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     2888 2022-11-16 07:27:12.410369 aiobiketrax-1.2.0/README.md
--rw-r--r--   0        0        0       53 2024-05-13 19:54:50.153267 aiobiketrax-1.2.0/aiobiketrax/__init__.py
--rw-r--r--   0        0        0    19826 2024-01-24 21:38:06.690061 aiobiketrax-1.2.0/aiobiketrax/api.py
--rw-r--r--   0        0        0     4774 2024-05-10 12:40:51.265662 aiobiketrax-1.2.0/aiobiketrax/cli.py
--rw-r--r--   0        0        0    16875 2024-05-10 12:08:40.740386 aiobiketrax-1.2.0/aiobiketrax/client.py
--rw-r--r--   0        0        0      163 2024-01-24 21:38:06.692494 aiobiketrax-1.2.0/aiobiketrax/consts.py
--rw-r--r--   0        0        0      412 2024-01-24 21:38:06.693226 aiobiketrax-1.2.0/aiobiketrax/exceptions.py
--rw-r--r--   0        0        0    33955 2024-05-10 12:17:11.768767 aiobiketrax-1.2.0/aiobiketrax/models.py
--rw-r--r--   0        0        0      982 2024-05-13 19:54:33.294821 aiobiketrax-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 aiobiketrax-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-07-07 22:22:53.680609 aiobiketrax-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2888 2022-11-16 07:27:12.410369 aiobiketrax-1.3.0/README.md
+-rw-r--r--   0        0        0       53 2024-05-14 05:56:00.175944 aiobiketrax-1.3.0/aiobiketrax/__init__.py
+-rw-r--r--   0        0        0    19826 2024-01-24 21:38:06.690061 aiobiketrax-1.3.0/aiobiketrax/api.py
+-rw-r--r--   0        0        0     4774 2024-05-10 12:40:51.265662 aiobiketrax-1.3.0/aiobiketrax/cli.py
+-rw-r--r--   0        0        0    18122 2024-05-13 22:59:04.070703 aiobiketrax-1.3.0/aiobiketrax/client.py
+-rw-r--r--   0        0        0      163 2024-01-24 21:38:06.692494 aiobiketrax-1.3.0/aiobiketrax/consts.py
+-rw-r--r--   0        0        0      412 2024-01-24 21:38:06.693226 aiobiketrax-1.3.0/aiobiketrax/exceptions.py
+-rw-r--r--   0        0        0    34279 2024-05-14 05:50:52.781470 aiobiketrax-1.3.0/aiobiketrax/models.py
+-rw-r--r--   0        0        0      982 2024-05-14 05:55:52.998918 aiobiketrax-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3641 1970-01-01 00:00:00.000000 aiobiketrax-1.3.0/PKG-INFO
```

### Comparing `aiobiketrax-1.2.0/LICENSE.md` & `aiobiketrax-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiobiketrax-1.2.0/README.md` & `aiobiketrax-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiobiketrax-1.2.0/aiobiketrax/api.py` & `aiobiketrax-1.3.0/aiobiketrax/api.py`

 * *Files identical despite different names*

### Comparing `aiobiketrax-1.2.0/aiobiketrax/cli.py` & `aiobiketrax-1.3.0/aiobiketrax/cli.py`

 * *Files identical despite different names*

### Comparing `aiobiketrax-1.2.0/aiobiketrax/client.py` & `aiobiketrax-1.3.0/aiobiketrax/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,17 +270,32 @@
     async def set_tracking_enabled(self, tracking_enabled: bool) -> None:
         _LOGGER.debug(
             "Setting tracking enabled state of device %s to %s.",
             self._id,
             tracking_enabled,
         )
 
+        # The app makes a distinction between older and newer tracker devices,
+        # depending on the unique identifier. It is not clear how to handle
+        # this correctly, so a warning is issued for now.
+        if self._device.unique_id.startswith(
+            "4710264"
+        ) or self._device.unique_id.startswith("8710"):
+            _LOGGER.warn(
+                "Setting tracking enabled state might not work for device %s, "
+                + "because it is considered a newer type of device.",
+                self._id,
+            )
+
         device = models.Device.from_dict(self._device.to_dict())
 
+        # The app seems to do this in two separate call, but combining them
+        # seems to work as well.
         device.disabled = not tracking_enabled
+        device.attributes.gps_disabled = not tracking_enabled
 
         self._account._devices[self._id] = await self._account.traccar_api.put_device(
             self._id, device
         )
 
     @property
     def _device(self) -> models.Device:
@@ -316,17 +331,31 @@
         """
         Get the trips sorted by start time.
         """
         return self._account._sorted_trips.get(self._id, [])
 
     @property
     def id(self) -> int:
+        """
+        Get the identifier of the device.
+        """
         return self._id
 
     @property
+    def unique_id(self) -> str:
+        """
+        Get the unique identifier of the device.
+
+        This is the identifier on the device settings page in the app. However,
+        it is not the same identifier as the `id` property on the device
+        response object.
+        """
+        return self._device.unique_id
+
+    @property
     def name(self) -> str:
         return self._device.name
 
     @property
     def is_deleted(self) -> bool:
         return self._device is None
 
@@ -354,14 +383,18 @@
     def is_charging(self) -> Optional[bool]:
         if not self._position:
             return None
 
         return self._position.attributes.charge
 
     @property
+    def is_double_battery(self) -> bool:
+        return self._device.attributes.double_battery or False
+
+    @property
     def geofence_radius(self) -> Optional[int]:
         return self._device.attributes.geofence_radius
 
     @property
     def guard_type(self) -> Optional[str]:
         return self._device.attributes.guard_type
```

### Comparing `aiobiketrax-1.2.0/aiobiketrax/models.py` & `aiobiketrax-1.3.0/aiobiketrax/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -525,14 +525,15 @@
         return result
 
 
 @dataclass
 class DeviceAttributes:
     alarm: Optional[bool] = None
     auto_guard: Optional[bool] = None
+    double_battery: Optional[bool] = None
     fw_version: Optional[str] = None
     geofence_radius: Optional[int] = None
     gps_disabled: Optional[bool] = None
     guarded: Optional[bool] = None
     guard_type: Optional[str] = None
     last_alarm: Optional[int] = None
     passport: Optional[Passport] = None
@@ -540,26 +541,28 @@
     trial_end: Optional[datetime] = None
 
     @staticmethod
     def from_dict(obj: Any) -> "DeviceAttributes":
         assert isinstance(obj, dict)
         alarm = from_union([from_bool, from_none], obj.get("alarm"))
         auto_guard = from_union([from_bool, from_none], obj.get("autoGuard"))
+        double_battery = from_union([from_bool, from_none], obj.get("doubleBattery"))
         fw_version = from_union([from_str, from_none], obj.get("fwVersion"))
         geofence_radius = from_union([from_int, from_none], obj.get("geofenceRadius"))
         gps_disabled = from_union([from_bool, from_none], obj.get("gpsDisabled"))
         guarded = from_union([from_bool, from_none], obj.get("guarded"))
         guard_type = from_union([from_str, from_none], obj.get("guardType"))
         last_alarm = from_union([from_int, from_none], obj.get("lastAlarm"))
         passport = from_union([Passport.from_dict, from_none], obj.get("passport"))
         stolen = from_union([from_bool, from_none], obj.get("stolen"))
         trial_end = from_union([from_datetime, from_none], obj.get("trialEnd"))
         return DeviceAttributes(
             alarm,
             auto_guard,
+            double_battery,
             fw_version,
             geofence_radius,
             gps_disabled,
             guarded,
             guard_type,
             last_alarm,
             passport,
@@ -569,14 +572,18 @@
 
     def to_dict(self) -> dict:
         result: dict = {}
         if self.alarm is not None:
             result["alarm"] = from_union([from_bool, from_none], self.alarm)
         if self.auto_guard is not None:
             result["autoGuard"] = from_union([from_bool, from_none], self.auto_guard)
+        if self.double_battery is not None:
+            result["doubleBattery"] = from_union(
+                [from_bool, from_none], self.double_battery
+            )
         if self.fw_version is not None:
             result["fwVersion"] = from_union([from_str, from_none], self.fw_version)
         if self.geofence_radius is not None:
             result["geofenceRadius"] = from_union(
                 [from_int, from_none], self.geofence_radius
             )
         if self.gps_disabled is not None:
```

### Comparing `aiobiketrax-1.2.0/pyproject.toml` & `aiobiketrax-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 '''
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "aiobiketrax"
-version = "1.2.0"
+version = "1.3.0"
 description = "Python library for interacting with the PowUnity BikeTrax GPS tracker."
 authors = ["Bas Stottelaar <basstottelaar@gmail.com>"]
 keywords = ["biketrax", "powunity", "asyncio", "iot", "gps"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/basilfx/aiobiketrax"
 repository = "https://github.com/basilfx/aiobiketrax"
```

### Comparing `aiobiketrax-1.2.0/PKG-INFO` & `aiobiketrax-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiobiketrax
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python library for interacting with the PowUnity BikeTrax GPS tracker.
 Home-page: https://github.com/basilfx/aiobiketrax
 License: MIT
 Keywords: biketrax,powunity,asyncio,iot,gps
 Author: Bas Stottelaar
 Author-email: basstottelaar@gmail.com
 Requires-Python: >=3.12,<4.0
```

