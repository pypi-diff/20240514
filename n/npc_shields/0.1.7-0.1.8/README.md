# Comparing `tmp/npc_shields-0.1.7.tar.gz` & `tmp/npc_shields-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npc_shields-0.1.7.tar", last modified: Fri May 10 02:02:51 2024, max compression
+gzip compressed data, was "npc_shields-0.1.8.tar", last modified: Tue May 14 17:33:31 2024, max compression
```

## Comparing `npc_shields-0.1.7.tar` & `npc_shields-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:02:51.763826 npc_shields-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-10 02:02:51.763826 npc_shields-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-10 02:02:23.000000 npc_shields-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-10 02:02:49.000000 npc_shields-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:02:51.763826 npc_shields-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:02:51.759826 npc_shields-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:02:51.759826 npc_shields-0.1.7/src/npc_shields/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:02:51.759826 npc_shields-0.1.7/src/npc_shields/drawings/
--rw-r--r--   0 runner    (1001) docker     (127)    85004 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/drawings/2001.svg
--rw-r--r--   0 runner    (1001) docker     (127)   150594 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/drawings/2002.svg
--rw-r--r--   0 runner    (1001) docker     (127)   108511 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/drawings/2005.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99489 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/drawings/2006.svg
--rw-r--r--   0 runner    (1001) docker     (127)    84797 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/drawings/Templeton_combos.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-10 02:02:46.000000 npc_shields-0.1.7/src/npc_shields/injections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/insertions.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/shields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-10 02:02:23.000000 npc_shields-0.1.7/src/npc_shields/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:02:51.763826 npc_shields-0.1.7/src/npc_shields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-10 02:02:51.000000 npc_shields-0.1.7/src/npc_shields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 02:02:51.000000 npc_shields-0.1.7/src/npc_shields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:02:51.000000 npc_shields-0.1.7/src/npc_shields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 02:02:51.000000 npc_shields-0.1.7/src/npc_shields.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 02:02:51.000000 npc_shields-0.1.7/src/npc_shields.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:31.140971 npc_shields-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-14 17:33:31.140971 npc_shields-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-14 17:32:59.000000 npc_shields-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-14 17:33:28.000000 npc_shields-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 17:33:31.140971 npc_shields-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:31.132971 npc_shields-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:31.136971 npc_shields-0.1.8/src/npc_shields/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:31.140971 npc_shields-0.1.8/src/npc_shields/drawings/
+-rw-r--r--   0 runner    (1001) docker     (127)    85004 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/drawings/2001.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   150594 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/drawings/2002.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   108511 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/drawings/2005.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99489 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/drawings/2006.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    84797 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/drawings/Templeton_combos.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-14 17:33:25.000000 npc_shields-0.1.8/src/npc_shields/injections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/insertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/shields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-14 17:32:59.000000 npc_shields-0.1.8/src/npc_shields/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-14 17:33:26.000000 npc_shields-0.1.8/src/npc_shields/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:33:31.140971 npc_shields-0.1.8/src/npc_shields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-14 17:33:31.000000 npc_shields-0.1.8/src/npc_shields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 17:33:31.000000 npc_shields-0.1.8/src/npc_shields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:33:31.000000 npc_shields-0.1.8/src/npc_shields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 17:33:31.000000 npc_shields-0.1.8/src/npc_shields.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 17:33:31.000000 npc_shields-0.1.8/src/npc_shields.egg-info/top_level.txt
```

### Comparing `npc_shields-0.1.7/PKG-INFO` & `npc_shields-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc_shields
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tools for Neuropixels probe insertion: providing suggested targets, recording actual insertions, storing notes.
 Author-email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_shields
 Project-URL: Issues, https://github.com/AllenInstitute/npc_shields/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ipywidgets>=7
 Requires-Dist: npc-session>=0.1.30
+Requires-Dist: pydantic>=2.7.1
+Requires-Dist: eval-type-backport>=0.2.0
 
 # npc_shields
 
 [![PyPI](https://img.shields.io/pypi/v/npc-shields.svg?label=PyPI&color=blue)](https://pypi.org/project/npc-shields/)
 [![Python version](https://img.shields.io/pypi/pyversions/npc-shields)](https://pypi.org/project/npc-shields/)
 
 [![Coverage](https://img.shields.io/codecov/c/github/alleninstitute/npc_shields?logo=codecov)](https://app.codecov.io/github/AllenInstitute/npc_shields)
```

### Comparing `npc_shields-0.1.7/README.md` & `npc_shields-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.7/pyproject.toml` & `npc_shields-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [project]
 name = "npc_shields"
-version = "0.1.7"
+version = "0.1.8"
 description = "Tools for Neuropixels probe insertion: providing suggested targets, recording actual insertions, storing notes."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "ipywidgets>=7",
     "npc-session>=0.1.30",
+    "pydantic>=2.7.1",
+    "eval-type-backport>=0.2.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `npc_shields-0.1.7/src/npc_shields/drawings/2001.svg` & `npc_shields-0.1.8/src/npc_shields/drawings/2001.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.7/src/npc_shields/drawings/2002.svg` & `npc_shields-0.1.8/src/npc_shields/drawings/2002.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.7/src/npc_shields/drawings/2005.svg` & `npc_shields-0.1.8/src/npc_shields/drawings/2005.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.7/src/npc_shields/drawings/2006.svg` & `npc_shields-0.1.8/src/npc_shields/drawings/2006.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.7/src/npc_shields/drawings/Templeton_combos.svg` & `npc_shields-0.1.8/src/npc_shields/drawings/Templeton_combos.svg`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.7/src/npc_shields/injections.py` & `npc_shields-0.1.8/src/npc_shields/injections.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import dataclasses
 import datetime
 from collections.abc import Sequence
 from typing import Any, Literal
 
 import npc_session
+import pydantic
 
 import npc_shields.shields
 import npc_shields.types
 
 
-@dataclasses.dataclass(frozen=True, unsafe_hash=True)
-class Injection:
+class Injection(pydantic.BaseModel):
     """An injection through a hole in a shield at a particular brain location (site + depth).
 
     - should allow for no shield (e.g. burr hole)
     - should record hemisphere
     - may consist of multiple individual injections
 
     >>> i = Injection(
@@ -36,84 +36,94 @@
     ...     number_of_injections=3,
     ...     notes="This was a test injection",
     ...     is_control=False,
     ...     is_anaesthetized=True,
     ... )
     """
 
-    shield: npc_shields.types.Shield | None
-    """The shield through which the injection was made."""
+    model_config = pydantic.ConfigDict(
+        arbitrary_types_allowed=True,
+    )
+
+    @pydantic.field_serializer("shield", when_used="always")
+    def serialize_shield_field(
+        self, shield: npc_shields.types.Shield
+    ) -> dict[str, Any]:
+        return shield.to_json() if shield is not None else None
 
     target_structure: str
     """The intended brain structure for the injection ('VISp' etc.)."""
 
-    hemisphere: Literal["left", "right"]
+    hemisphere: Literal["left", "right"] = "left"
     """The hemisphere of the brain where the injection was made ('left' or 'right')."""
 
     depth_um: float
     """Depth of the injection, in microns from brain surface."""
 
-    substance: str
+    substance: str = "muscimol"
     """Name of the injected substance."""
 
-    manufacturer: str | None
+    manufacturer: str | None = "Sigma-Aldrich"
     """Manufacturer of the injected substance."""
 
-    identifier: str | None
+    identifier: str | None = "M1523"
     """Identifier of the injected substance (e.g. manufacture serial number)."""
 
     total_volume_nl: float
     """Total volume injected, in nanoliters."""
 
     concentration_mg_ml: float | None
     """Concentration of the injected substance in milligrams per milliliter."""
 
     flow_rate_nl_s: float
     """Flow rate of the injection in nanoliters per second."""
 
-    start_time: datetime.datetime
+    start_time: datetime.datetime = datetime.datetime.now()
     """Time of the first injection, as a datetime object."""
 
+    @pydantic.field_serializer("start_time", when_used="always")
+    def serialize_start_time_field(self, start_time: datetime.datetime) -> str:
+        return start_time.isoformat(sep=" ", timespec="seconds")
+
     is_anaesthetized: bool
     """Whether the subject was anaesthetized during the injection."""
 
+    number_of_injections: int
+    """Number of individual injections made at this site + depth."""
+
     # args with defaults ----------------------------------------------- #
 
+    shield: npc_shields.types.Shield | None = None
+    """The shield through which the injection was made."""
+
     location: str | None = None
     """The hole in the shield through which the injection was made (e.g. 'C3').
 
     - alternatively, a string indicating location of a burr hole or other non-shield location.
     """
 
     location_ap: float | None = None
     """Distance in millimeters from bregma to injection site along
     anterior-posterior axis (+ve is anterior)."""
 
     location_ml: float | None = None
     """Distance in millimeters from brain midline to injection site along
     medial-lateral axis."""
 
-    fluorescence_nm: float | None = None
+    fluorescence_nm: int | None = None
     """Emission wavelength of the substance injected, if it fluoresces."""
 
-    number_of_injections: int = 1
-    """Number of individual injections made at this site + depth."""
-
     is_control: bool = False
     """Whether the purpose of the injection was a control."""
 
     notes: str | None = None
     """Text notes for the injection."""
 
     def to_json(self) -> dict[str, Any]:
-        data = dataclasses.asdict(self)
-        data["start_time"] = self.start_time.isoformat()
-        if self.shield is not None:
-            data["shield"] = self.shield.to_json()
-        return data
+        return self.model_dump()
 
 
 @dataclasses.dataclass
 class InjectionRecord:
     """A record of a set of injections.
 
     >>> i = Injection(
@@ -136,18 +146,18 @@
     ... )
     >>> r = InjectionRecord(
     ...     injections=[i],
     ...     session="366122_20240101",
     ...     experiment_day=1,
     ... )
     >>> r.to_json()
-    {'injections': [{'shield': {'name': '2002', 'drawing_id': '0283-200-002'}, 'target_structure': 'VISp', 'hemisphere': 'left', 'depth_um': 3000, 'substance': 'Fluorogold', 'manufacturer': 'Sigma', 'identifier': '12345', 'total_volume_nl': 1.0, 'concentration_mg_ml': 10.0, 'flow_rate_nl_s': 0.1, 'start_time': '2023-01-01T12:00:00', 'is_anaesthetized': False, 'location': None, 'location_ap': None, 'location_ml': None, 'fluorescence_nm': 500, 'number_of_injections': 3, 'is_control': False, 'notes': 'This was a test injection'}], 'session': '366122_20240101', 'experiment_day': 1}
+    {'injections': [{'target_structure': 'VISp', 'hemisphere': 'left', 'depth_um': 3000.0, 'substance': 'Fluorogold', 'manufacturer': 'Sigma', 'identifier': '12345', 'total_volume_nl': 1.0, 'concentration_mg_ml': 10.0, 'flow_rate_nl_s': 0.1, 'start_time': '2023-01-01 12:00:00', 'is_anaesthetized': False, 'number_of_injections': 3, 'shield': {'name': '2002', 'drawing_id': '0283-200-002'}, 'location': None, 'location_ap': None, 'location_ml': None, 'fluorescence_nm': 500, 'is_control': False, 'notes': 'This was a test injection'}], 'session': '366122_20240101', 'experiment_day': 1}
     """
 
-    injections: Sequence[Injection]
+    injections: Sequence[npc_shields.types.Injection]
     """A record of each injection made."""
 
     session: str | npc_session.SessionRecord
     """Record of the session, including subject, date, session index."""
 
     experiment_day: int
     """1-indexed day of experiment for the subject specified in `session`."""
```

### Comparing `npc_shields-0.1.7/src/npc_shields/insertions.py` & `npc_shields-0.1.8/src/npc_shields/insertions.py`

 * *Files identical despite different names*

### Comparing `npc_shields-0.1.7/src/npc_shields/shields.py` & `npc_shields-0.1.8/src/npc_shields/shields.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 f">{label}</tspan>", f"> {''.join(probe_letters)}</tspan>"
             )
     return data
 
 
 def get_shield(
     name_or_id: str | int,
-) -> npc_shields.types.Shield:
+) -> npc_shields.shields.Shield:
     """
     Get an existing shield instance by name or drawing ID.
 
     >>> x = get_shield("2002")
     >>> y = get_shield("0283-200-002")
     >>> assert x is y
     """
@@ -144,23 +144,23 @@
             if str(name_or_id).lower() == str(getattr(shield, attr)).lower():
                 return shield
     raise ValueError(
         f"Shield {name_or_id!r} not found: should be one of {[s.name for s in shields]}"
     )
 
 
-def get_shields() -> tuple[npc_shields.types.Shield, ...]:
+def get_shields() -> tuple[Shield, ...]:
     """
     All known shields, sorted by drawing ID.
 
     >>> x = get_shields()
     """
     return tuple(
         sorted(
-            (v for v in globals().values() if isinstance(v, npc_shields.types.Shield)),
+            (v for v in globals().values() if isinstance(v, Shield)),
             key=lambda x: x.drawing_id,
         )
     )
 
 
 if __name__ == "__main__":
     import doctest
```

### Comparing `npc_shields-0.1.7/src/npc_shields/types.py` & `npc_shields-0.1.8/src/npc_shields/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     @property
     def shield(self) -> Shield | None:
         """The shield through which the injection was made."""
         ...
 
     @property
-    def location(self) -> str:
+    def location(self) -> str | None:
         """The hole in the shield through which the injection was made (e.g. 'C3').
 
         - alternatively, a string indicating location of a burr hole or other non-shield location.
         """
         ...
 
     @property
@@ -138,15 +138,15 @@
 
     @property
     def depth_um(self) -> float:
         """Depth of the injection, in microns from brain surface."""
         ...
 
     @property
-    def fluorescence_nm(self) -> float | None:
+    def fluorescence_nm(self) -> int | None:
         """Wavelength of fluorescence for the injection."""
         ...
 
     @property
     def manufacturer(self) -> str | None:
         """Manufacturer of the injected substance."""
         ...
```

### Comparing `npc_shields-0.1.7/src/npc_shields.egg-info/PKG-INFO` & `npc_shields-0.1.8/src/npc_shields.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npc_shields
-Version: 0.1.7
+Version: 0.1.8
 Summary: Tools for Neuropixels probe insertion: providing suggested targets, recording actual insertions, storing notes.
 Author-email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/npc_shields
 Project-URL: Issues, https://github.com/AllenInstitute/npc_shields/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ipywidgets>=7
 Requires-Dist: npc-session>=0.1.30
+Requires-Dist: pydantic>=2.7.1
+Requires-Dist: eval-type-backport>=0.2.0
 
 # npc_shields
 
 [![PyPI](https://img.shields.io/pypi/v/npc-shields.svg?label=PyPI&color=blue)](https://pypi.org/project/npc-shields/)
 [![Python version](https://img.shields.io/pypi/pyversions/npc-shields)](https://pypi.org/project/npc-shields/)
 
 [![Coverage](https://img.shields.io/codecov/c/github/alleninstitute/npc_shields?logo=codecov)](https://app.codecov.io/github/AllenInstitute/npc_shields)
```

### Comparing `npc_shields-0.1.7/src/npc_shields.egg-info/SOURCES.txt` & `npc_shields-0.1.8/src/npc_shields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

