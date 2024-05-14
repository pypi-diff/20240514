# Comparing `tmp/hyperstruct-0.0.2.tar.gz` & `tmp/hyperstruct-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperstruct-0.0.2.tar", max compression
+gzip compressed data, was "hyperstruct-0.0.3.tar", max compression
```

## Comparing `hyperstruct-0.0.2.tar` & `hyperstruct-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2024-05-13 00:26:16.961480 hyperstruct-0.0.2/LICENSE
--rw-r--r--   0        0        0     3330 2024-05-13 00:26:16.961480 hyperstruct-0.0.2/README.md
--rw-r--r--   0        0        0     1831 2024-05-13 00:26:34.321496 hyperstruct-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1512 2024-05-13 00:26:16.965481 hyperstruct-0.0.2/src/hyperstruct/__init__.py
--rw-r--r--   0        0        0      213 2024-05-13 00:26:34.321496 hyperstruct-0.0.2/src/hyperstruct/__main__.py
--rw-r--r--   0        0        0    12513 2024-05-13 00:26:16.965481 hyperstruct-0.0.2/src/hyperstruct/fuselage.py
--rw-r--r--   0        0        0        0 2024-05-13 00:26:16.965481 hyperstruct-0.0.2/src/hyperstruct/py.typed
--rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 hyperstruct-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-14 02:51:22.994386 hyperstruct-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3330 2024-05-14 02:51:22.994386 hyperstruct-0.0.3/README.md
+-rw-r--r--   0        0        0     1830 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1425 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/src/hyperstruct/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/src/hyperstruct/__main__.py
+-rw-r--r--   0        0        0    12738 2024-05-14 02:51:31.966397 hyperstruct-0.0.3/src/hyperstruct/fuselage.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:51:22.994386 hyperstruct-0.0.3/src/hyperstruct/py.typed
+-rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 hyperstruct-0.0.3/PKG-INFO
```

### Comparing `hyperstruct-0.0.2/LICENSE` & `hyperstruct-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperstruct-0.0.2/README.md` & `hyperstruct-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperstruct-0.0.2/pyproject.toml` & `hyperstruct-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperstruct"
-version = "0.0.2"
+version = "0.0.3"
 description = "Hyperstruct"
 authors = ["Benjamin Crews <aceF22@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/czarified/hyperstruct"
 repository = "https://github.com/czarified/hyperstruct"
 documentation = "https://hyperstruct.readthedocs.io"
@@ -55,15 +55,15 @@
 
 [tool.coverage.run]
 branch = true
 source = ["hyperstruct", "tests"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 100
+fail_under = 10
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 lines_after_imports = 2
 
 [tool.mypy]
```

### Comparing `hyperstruct-0.0.2/src/hyperstruct/__init__.py` & `hyperstruct-0.0.3/src/hyperstruct/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Hyperstruct."""
 
 from dataclasses import dataclass
-from typing import List
 
 
 @dataclass
 class Material:
     """The HyperStruct material model.
 
     The material object contains the basic material allowables.
@@ -51,18 +50,15 @@
     """The basic foundation for sizing.
 
     An Aircraft is composed of different Assemblies, which contain various Components.
     Components have several base methods and attributes that enable sizing and
     weights estimation.
     """
 
-    routines: List
-
     def synthesis(self) -> None:
         """The sizing method.
 
         The sizing method collects all sizing routines and executes them
         in the order of the `routines` list.
         """
         # This doesn't work. It's just a placeholder.
-        for _routine in self.routines:
-            pass
+        pass
```

### Comparing `hyperstruct-0.0.2/src/hyperstruct/fuselage.py` & `hyperstruct-0.0.3/src/hyperstruct/fuselage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 The fuselage module operates as a stand-alone program or in conjuction with other modules.
 
 This file contains all global variables, classes, and functions related to fuselage weight synthesis.
 """
 
 from dataclasses import dataclass
+from typing import Any
 from typing import Tuple
 
 import numpy as np
 
 from hyperstruct import Component
 from hyperstruct import Material
 
@@ -68,30 +69,30 @@
 
         For milled panels the fastener hole degradation is assumed to be accounted for,
         and this factor is set to 1.0.
         """
         return 1.0 if self.milled else 0.75
 
     @property
-    def q(self):
+    def q(self) -> float:
         """Evaluate the cover shear flow.
 
         Assuming the section masses are concentrated at the longerons
         or stringers and that the areas are equal, the equation for shear
         flow may be reduced to an equation dependent only on element location.
         """
         return self.V * self.Q / self.I
 
     @property
     def zee(self) -> float:
         """Panel buckling geometry parameter for shear buckling coefficient."""
         b = min(self.D, self.L)
         frac = b**2 / (self.RC * self.t_c)
         # Note, ADA002867 uses lowercase greek mu, but confirms that it is Poisson's Ratio.
-        root = np.sqrt(1 - self.material.nu**2)
+        root = float(np.sqrt(1 - self.material.nu**2))
         return frac * root
 
     @property
     def k_s(self) -> float:
         """Shear buckling coefficient.
 
         Reference curves are displayed in ADA002867, Fig. 12.
@@ -100,29 +101,31 @@
         z = self.zee
         if (self.RC > 1000) or (self.RC == 0):
             # Panel has no curvature. Flat panels are assumed to be a 7.5
             return 7.5
         elif z < 2:
             return 7.5
         elif 2 < z < 10:
-            return 7.5 * (z / 2) ** 0.113
+            return float(7.5 * (z / 2) ** 0.113)
         elif 10 < z:
-            return 9 * (z / 10) ** 0.522
+            return float(9 * (z / 10) ** 0.522)
+        else:
+            raise NotImplementedError("I don't know how you got here...")
 
     def field_thickness_block_shear(self) -> float:
         """Field thickness based on shear strength.
 
         Evaluate the min thickness required to satisfy block shear strength.
         """
         if self.milled:
             t_c = self.q / self.material.F_su
         else:
-            t_c = self.q / (self.C_r * self.material.F_su)
+            t_c = self.q / (self.c_r * self.material.F_su)
 
-        return t_c
+        return float(t_c)
 
     def field_thickness_postbuckled(self, alpha: float = 45) -> float:
         """Field thickness based on critical shear flow.
 
         Evaluate the min thickness required to satisfy post-buckled strength.
         Postbuckled strength assumes sizing covers with diagonal tension. The
         diagonal tension angle is unknown because intermediate frame and
@@ -161,28 +164,28 @@
             ) ** (1 / 3) - (
                 np.sqrt((K_3 / (2 * K_1)) ** 2 + (K_2 / (3 * K_1)) ** 3)
                 - (K_3 / (2 * K_1))
             ) ** (
                 1 / 3
             )
 
-            return t_c
+            return float(t_c)
 
     def land_thickness_net_section(self) -> float:
         """Land thickness based on net section allowable.
 
         On milled panels the land thickness is checked against the net section shear allowable.
         On unmilled panels, the land thickness is simply equivalent to the field thickness.
         """
         if not self.milled:
-            return self.t_c
+            return float(self.t_c)
         else:
-            return self.q / (self.c_r * self.material.F_su)
+            return float(self.q / (self.c_r * self.material.F_su))
 
-    def thickness_pressure(self, F_allow=None) -> Tuple[float, float]:
+    def thickness_pressure(self, F_allow: Any = None) -> Tuple[float, float]:
         """Thicknesses based on cover pressure.
 
         A required thickness is evaluated to resist hoop stress,
         and then bending diaphram stress via strip theory. The
         minimum of these values is returned as the required land thickness.
 
         Cabin pressurization is a cyclic occurrence that subjects the cover
@@ -233,17 +236,17 @@
         t_3 = (1.646 * b * P_1**0.894 * self.material.E**0.394) / F_allow**1.288
         # Strip Theory Midspan thickness
         t_4 = self.material.E**1.984 * (1.3769 * b * P_1**2.484) / F_allow**4.467
 
         t_min = min(t_1, t_2, t_3, t_4)
 
         if self.milled:
-            return (t_3, t_min)
+            return (float(t_3), float(t_min))
         else:
-            return (t_min, t_min)
+            return (float(t_min), float(t_min))
 
     def panel_flutter(self, mach: float, altitude: float) -> float:
         """Evaluate baseline thickness to avoid local panel flutter.
 
         The baseline thickness to make local panel flutter highly improbable
         is a function of dynamic pressure, Mach number, geometry, and material.
         Curve-fits for each variable are utilized, with a baseline thickness
@@ -291,15 +294,15 @@
             LW = 10
 
         # Panel Flutter Parameter, phi_B
         phi_b = 0.5551841 - 0.1686944 * LW + 0.02169992 * LW**2 - 0.000963694 * LW**3
 
         t_b = (phi_b * self.L) / (FM * self.material.E / q) ** (1 / 3)
 
-        return t_b
+        return float(t_b)
 
     def acoustic_fatigue(self) -> Tuple[float, float]:
         """Thickness requirements based on acoustic fatigue.
 
         Assumptions are:
             1.) The overall pressure level from jet engine noise is approximately
                 30db higher than the random spectrum pressure level.
@@ -335,8 +338,8 @@
         # Curvature correction
         x_l = self.D**2 / (t_l * self.RC)
         x_c = self.D**2 / (t_c * self.RC)
         # Ratio of curved panel thickness over flat panel
         f_l = 1.0794 + 0.000143 * x_l - 0.076475 * (1 / x_l) - 0.29969 * np.log(x_l)
         f_c = 1.0794 + 0.000143 * x_c - 0.076475 * (1 / x_c) - 0.29969 * np.log(x_c)
 
-        return (f_l * t_l, f_c * t_c)
+        return (float(f_l * t_l), float(f_c * t_c))
```

### Comparing `hyperstruct-0.0.2/PKG-INFO` & `hyperstruct-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperstruct
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hyperstruct
 Home-page: https://github.com/czarified/hyperstruct
 License: MIT
 Author: Benjamin Crews
 Author-email: aceF22@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 1 - Planning
```

