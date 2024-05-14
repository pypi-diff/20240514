# Comparing `tmp/interpolator_for_wrfchem-1.1.0.tar.gz` & `tmp/interpolator_for_wrfchem-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpolator_for_wrfchem-1.1.0.tar", max compression
+gzip compressed data, was "interpolator_for_wrfchem-1.2.0.tar", max compression
```

## Comparing `interpolator_for_wrfchem-1.1.0.tar` & `interpolator_for_wrfchem-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     1074 2024-02-06 14:04:33.000000 interpolator_for_wrfchem-1.1.0/LICENSE
--rw-r--r--   0        0        0     2724 2024-02-06 14:05:02.000000 interpolator_for_wrfchem-1.1.0/README.md
--rw-r--r--   0        0        0     7571 2024-03-20 11:07:06.010810 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/__init__.py
--rw-r--r--   0        0        0       50 2023-12-13 14:36:46.000000 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/__main__.py
--rw-r--r--   0        0        0     5120 2024-03-20 11:07:10.670811 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/global_model.py
--rw-r--r--   0        0        0     2888 2024-01-29 14:22:43.000000 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/interpolation.py
--rw-r--r--   0        0        0     2628 2024-03-20 11:07:17.890811 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/met_em.py
--rw-r--r--   0        0        0        0 2023-12-19 09:13:27.000000 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/res/__init__.py
--rw-r--r--   0        0        0     4603 2023-12-19 09:06:49.000000 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/res/cams_eac4_model_levels.csv
--rw-r--r--   0        0        0     4175 2024-03-20 11:03:24.580797 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/species_map.py
--rw-r--r--   0        0        0     1212 2024-01-09 08:25:51.000000 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/utils.py
--rw-r--r--   0        0        0     2857 2023-12-22 14:29:50.000000 interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/wrf.py
--rw-r--r--   0        0        0      658 2024-03-20 11:07:38.340810 interpolator_for_wrfchem-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3367 1970-01-01 00:00:00.000000 interpolator_for_wrfchem-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-02-06 14:04:33.000000 interpolator_for_wrfchem-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3497 2024-05-14 14:44:48.563466 interpolator_for_wrfchem-1.2.0/README.md
+-rw-r--r--   0        0        0     7801 2024-05-14 14:02:26.283465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/__init__.py
+-rw-r--r--   0        0        0       50 2023-12-13 14:36:46.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/__main__.py
+-rw-r--r--   0        0        0      130 2024-05-14 13:59:05.663473 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__init__.py
+-rw-r--r--   0        0        0      386 2024-05-14 14:02:29.673465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     9806 2024-05-14 14:08:58.743470 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__pycache__/cams.cpython-312.pyc
+-rw-r--r--   0        0        0     1214 2024-05-14 14:02:29.693465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/__pycache__/prototype.cpython-312.pyc
+-rw-r--r--   0        0        0     7073 2024-05-14 14:08:55.993470 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/cams.py
+-rw-r--r--   0        0        0      546 2024-05-14 13:35:26.773462 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/prototype.py
+-rw-r--r--   0        0        0     2888 2024-05-14 14:45:10.223466 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/interpolation.py
+-rw-r--r--   0        0        0     2628 2024-03-20 11:07:17.890811 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/met_em.py
+-rw-r--r--   0        0        0        0 2023-12-19 09:13:27.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/__init__.py
+-rw-r--r--   0        0        0      184 2023-12-19 10:58:50.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    10577 2024-05-14 13:43:25.533463 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/cams_l137.csv
+-rw-r--r--   0        0        0     4603 2023-12-19 09:06:49.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/cams_l60.csv
+-rw-r--r--   0        0        0     4124 2024-05-14 13:19:32.453465 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/species_map.py
+-rw-r--r--   0        0        0     1212 2024-01-09 08:25:51.000000 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/utils.py
+-rw-r--r--   0        0        0     2806 2024-05-14 12:56:08.583462 interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/wrf.py
+-rw-r--r--   0        0        0      658 2024-05-14 14:45:19.553467 interpolator_for_wrfchem-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 interpolator_for_wrfchem-1.2.0/PKG-INFO
```

### Comparing `interpolator_for_wrfchem-1.1.0/LICENSE` & `interpolator_for_wrfchem-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.1.0/README.md` & `interpolator_for_wrfchem-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 - Potentially support many global models (currently supports CAMS EAC4)
 
 The application is written in Python and is meant to be used a command-line tool. Some potential limitations:
 
 - The application currently assumes that fields are mixing ratios.
 - The global model fields should be on a regular lat-lon grid.
 - No nesting support
--
 
 ## Installation
 
 The application is available on PyPI and can be installed using pip:
 
 ```bash
 pip install interpolator-for-wrfchem
@@ -35,24 +34,31 @@
 The interpolator will update `wrfinput` and `wrfbdy` files to include the chemistry information.
 
 ![Workflow](./workflow.drawio.png)
 
 The interpolator is a command-line tool and can be run as follows:
 
 ```bash
-interpolator-for-wrfchem <global model data path> <met_em path> <wrfinput_d01 path> <wrfbdy_d01 path> <species map path> <output path>
+interpolator-for-wrfchem <global model name> <global model data path> <met_em path> <wrfinput path> <species map path>
 ```
 
-The `wrfinput_d01` and `wrfbdy_d01` files **WILL BE MODIFIED**!
+The `wrfinput` and `wrfbdy` files **WILL BE MODIFIED**! The `global model name` can be one of the following:
+
+- `cams_eac4`: CAMS EAC4 data (w/ 60 vertical levels)
+- `cams_global_forecasts`: CAMS global forecasts (w/ 137 vertical levels)
 
 There are some optional flags:
 
+- `--wrfbdy=`: Path to the `wrfbdy_d01` file, if not provided, the boundary is not updated.
 - `--copy-icbc`: Make a backup of the `wrfinput` and `wrfbdy` files before updating them.
-- `--no-ic` and `--no-bc`: Do not update the `wrfinput` and `wrfbdy` files, respectively.
-- `--diagnostics`: Store some diagnostic information in the `diag.nc` file.
+- `--no-ic`: Do not update the `wrfinput`. You must nonetheless provide the path to the `wrfinput` file as it is required to read some information.
+- `--diagnostics`: Store some diagnostic information in the `diag_cams_interp.nc` file.
+
+When you use nested domains, you can run the application multiple times, each time pointing to a different `wrfinput` file. You can omit the `wrfbdy` file when running the application for the nested domains' `wrfinput` files.
+If you need to update `wrfbdy` files for the future without touching `wrfinput` (e.g. for a cycling run), point to a correct `wrfinput` file (correct means it's the same model grid and configuration) and use the `--no-ic` flag.
 
 ## Species mapping
 
 In many cases, the available fields of the global model do not directly correspond to the ones used by the chemistry/dust scheme you want to use in WRF-CHEM. For example, you might have dust concentrations available in different size bins. The application supports "species mapping", through which the WRF-CHEM fields are created through a linear combination of global model fields, after interpolation.
 
 Detailed description of the species file format is available in [species_maps.md](./species_maps/species_maps.md).
```

### Comparing `interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/__init__.py` & `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,61 +2,62 @@
 import shutil
 from collections import namedtuple
 from pathlib import Path
 
 import numpy as np
 
 from interpolator_for_wrfchem import utils
-from interpolator_for_wrfchem.global_model import CAMS_EAC4_ML
+from interpolator_for_wrfchem.global_models import GLOBAL_MODELS
 from interpolator_for_wrfchem.interpolation import interpolate_to_wrf
 from interpolator_for_wrfchem.met_em import MetEm
 from interpolator_for_wrfchem.species_map import SpeciesMap, convert_si
-from interpolator_for_wrfchem.wrf import WRF
+from interpolator_for_wrfchem.wrf import WRFBoundary, WRFInput
 
 
 def main():
     """Entrypoint, parse arguments and run script"""
     args = cmd_args()
 
     # Backup wrfinput/wrfbdy if requested
     if args.copy_icbc:
         print("Backing up wrfinput/wrfbdy to wrfinput.orig/wrfbdy.orig")
         if args.wrfinput.with_suffix(".orig").exists():
             print("Backup file already exists, will not overwrite")
         else:
             shutil.copy(args.wrfinput, args.wrfinput.with_suffix(".orig"))
 
-        if args.wrfbdy.with_suffix(".orig").exists():
-            print("Backup file already exists, will not overwrite")
-        else:
-            shutil.copy(args.wrfbdy, args.wrfbdy.with_suffix(".orig"))
+        if "wrfbdy" in args and args.wrfbdy is not None:
+            if args.wrfbdy.with_suffix(".orig").exists():
+                print("Backup file already exists, will not overwrite")
+            else:
+                shutil.copy(args.wrfbdy, args.wrfbdy.with_suffix(".orig"))
 
     # Read input files: mapping def., global model, WRF
     mapping = SpeciesMap(Path(args.mapping))
     print(mapping)
 
-    wrf = WRF(Path(args.wrfinput), Path(args.wrfbdy))
+    wrf = WRFInput(args.wrfinput)
     wrf_ds = wrf.get_dataset()
     print(wrf)
 
     met_em = MetEm(Path(args.met_em), wrf_ds)
     print(met_em)
 
-    cams = CAMS_EAC4_ML(Path(args.input_files), mapping.required_source_species)
-    print(cams)
+    global_model = GLOBAL_MODELS[args.global_model](
+        Path(args.input_files), mapping.required_source_species
+    )
+    print(global_model)
 
     # Interpolate initial conditions
-    if wrf.wrfinput_time not in cams.times:
+    if wrf.time not in global_model.times:
         raise RuntimeError(
-            f"Could not find global model file for wrfinput time {wrf.wrfinput_time}"
+            f"Could not find global model file for wrfinput time {wrf.nc_file_time}"
         )
 
-    cams_ds = cams.get_dataset(
-        wrf.wrfinput_time,
-    )
+    cams_ds = global_model.get_dataset(wrf.time)
 
     # Initial conditions
     if not args.no_ic:
         cams_interp_ds = interpolate_to_wrf(wrf_ds, cams_ds)
 
         if args.diagnostics:
             cams_diag_ds = cams_interp_ds.copy()
@@ -80,23 +81,24 @@
                 )
             wrf_vars[name] = (wrf_vars[name] * spec.weight) + spec.offset
 
         # Write to WRF
         for name, arr in wrf_vars.items():
             alias = mapping.aliases_target.get(name, name)
 
-            if alias not in wrf.wrfinput.variables:
-                wrf.wrfinput.createVariable(
+            if alias not in wrf.nc_file.variables:
+                wrf.nc_file.createVariable(
                     alias, "f4", ("Time", "bottom_top", "south_north", "west_east")
                 )
-            wrf.wrfinput.variables[alias][0, :, :, :] = arr
+            wrf.nc_file.variables[alias][0, :, :, :] = arr
 
     # Compute boundary
-    if not args.no_bc:
-        for t_idx, t in enumerate(wrf.wrfbdy_time):
+    if "wrfbdy" in args:
+        wrfbdy = WRFBoundary(args.wrfbdy)
+        for t_idx, t in enumerate(wrfbdy.times):
             wrf_pres = met_em.get_pres(t)
 
             for bdy in ["BXS", "BXE", "BYS", "BYE"]:
                 # Get WRF profile and replace pressure from met_em
                 wrf_bdy = utils.get_boundary_profile(wrf_ds, bdy)
                 wrf_bdy["pres"] = utils.get_boundary_profile(wrf_pres, bdy)
 
@@ -124,76 +126,77 @@
                         )
                     wrf_vars[name] = (wrf_vars[name] * spec.weight) + spec.offset
 
                 # Write to wrfbdy
                 for name, arr in wrf_vars.items():
                     alias = mapping.aliases_target.get(name, name) + f"_{bdy}"
 
-                    if alias not in wrf.wrfbdy.variables:
-                        wrf.wrfbdy.createVariable(alias, "f4", ("Time", *arr.dims))
-                    wrf.wrfbdy.variables[alias][t_idx, ...] = arr
+                    if alias not in wrfbdy.nc_file.variables:
+                        wrfbdy.nc_file.createVariable(alias, "f4", ("Time", *arr.dims))
+                    wrfbdy.nc_file.variables[alias][t_idx, ...] = arr
 
         # Compute tendencies
         # For each boundary, store the difference between the current and previous value
         # inside the {var}_BT{bdy} variable, where {bdy} is one of XS, XE, YS, YE.
-        for t_idx, t in enumerate(wrf.wrfbdy_time):
+        for t_idx, t in enumerate(wrfbdy.times):
             if t_idx == 0:
                 continue
-            dt = (t - wrf.wrfbdy_time[t_idx - 1]).total_seconds()
+            dt = (t - wrfbdy.times[t_idx - 1]).total_seconds()
 
             for name in wrf_vars.keys():
                 for bdy in ["XS", "XE", "YS", "YE"]:
                     bdy_var = f"{name}_B{bdy}"
                     bdy_t_var = f"{name}_BT{bdy}"
 
-                    if bdy_t_var not in wrf.wrfbdy.variables:
-                        wrf.wrfbdy.createVariable(
-                            bdy_t_var, "f4", wrf.wrfbdy[bdy_var].dimensions
+                    if bdy_t_var not in wrfbdy.nc_file.variables:
+                        wrfbdy.nc_file.createVariable(
+                            bdy_t_var, "f4", wrfbdy.nc_file[bdy_var].dimensions
                         )
 
-                    wrf.wrfbdy.variables[bdy_t_var][t_idx, ...] = (
-                        wrf.wrfbdy.variables[bdy_var][t_idx, ...]
-                        - wrf.wrfbdy.variables[bdy_var][t_idx - 1, ...]
+                    wrfbdy.nc_file.variables[bdy_t_var][t_idx, ...] = (
+                        wrfbdy.nc_file.variables[bdy_var][t_idx, ...]
+                        - wrfbdy.nc_file.variables[bdy_var][t_idx - 1, ...]
                     ) / dt
 
     wrf.close()
 
 
 def cmd_args():
     argparser = argparse.ArgumentParser(
         description="Interpolate WRF-Chem output to a regular grid"
     )
     argparser.add_argument(
+        "global_model",
+        type=str,
+        help="Global model to use",
+        choices=list(GLOBAL_MODELS.keys()),
+    )
+    argparser.add_argument(
         "input_files", type=Path, help="Global model fields to interpolate"
     )
     argparser.add_argument("met_em", type=Path, help="Directory of met_em files")
-    argparser.add_argument("wrfinput", type=Path, help="WRF input file to update")
-    argparser.add_argument("wrfbdy", type=Path, help="WRF boundary file to update")
     argparser.add_argument("mapping", type=Path, help="Mapping file to use")
+
+    argparser.add_argument("wrfinput", type=Path, help="WRF input file")
+    argparser.add_argument("--wrfbdy", type=Path, help="WRF boundary file to update")
+
     argparser.add_argument(
-        "--copy-icbc",
-        "-c",
-        action="store_true",
-        help="Do not modify wrfinput/wrfbdy, instead copy them to wrfinput.orig/wrfbdy.orig",
-    )
-    argparser.add_argument(
-        "--diagnostics",
-        "-d",
+        "--no-ic",
         action="store_true",
-        help="Write out diagnostic file for debugging. It will be written to the current directory with the name `diag.nc`.",
+        help="Do not update initial conditions, wrfinput file still required.",
     )
     argparser.add_argument(
-        "--no-ic",
+        "--copy-icbc",
         action="store_true",
-        help="Do not interpolate initial conditions",
+        help="Copy wrfinput/wrfbdy to wrfinput.orig/wrfbdy.orig before modifying, will not overwrite any existing .orig files",
     )
     argparser.add_argument(
-        "--no-bc",
+        "--diagnostics",
         action="store_true",
-        help="Do not interpolate boundary conditions",
+        help="Write out diagnostic file for debugging. It will be written to the current directory with the name `diag_cams_interp.nc`.",
     )
     args = vars(argparser.parse_args())
 
     args_type = namedtuple(
         "Args",
         args.keys(),
     )
```

### Comparing `interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/global_model.py` & `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/global_models/cams.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,40 +4,43 @@
 
 import cftime
 import netCDF4 as nc
 import pandas as pd
 import xarray as xr
 
 import interpolator_for_wrfchem.res as res
+from interpolator_for_wrfchem.global_models.prototype import GlobalModel
 
 
-class CAMS_EAC4_ML:
+class CAMS_Base(GlobalModel):
     """
-    Handles interactions with a directory of EAC4-model level files. The given directory
-    should contains a set of directories named `YYYY-MM-DD`, each containing a pair of
-    `levtype_ml.nc` and `levtype_sfc.nc` files. This class handles model level data.
+    Handles interactions w/ a directory of CAMS Global Atmospheric Composition forecasts.
+    The given directory should contain a set of directories named `YYYY-MM-DD`, each
+    containing a pair of `levtype_ml.nc` and `levtype_sfc.nc` files. This class handles
+    model level data.
+
+    The 3D pressure field is created using the surface pressure and the model definition [1],
+    which is different between the re-analysis (e.g., EAC4) and the operational forecasts.
+    Thus, we have two subclasses of this that are almost the same, but use different model
+    level definitions.
 
-    The 3D pressure field is created using the surface pressure and the model definitions
-    from [1], while the methodology is described in [2].
-
-    [1] https://confluence.ecmwf.int/display/UDOC/L60+model+level+definitions
-    [2] https://confluence.ecmwf.int/display/CKB/ERA5%3A+compute+pressure+and+geopotential+on+model+levels%2C+geopotential+height+and+geometric+height
+    [1] https://confluence.ecmwf.int/display/CKB/ERA5%3A+compute+pressure+and+geopotential+on+model+levels%2C+geopotential+height+and+geometric+height
     """
 
     dir: Path
     """Where the files are located"""
 
     times: dict[dt.datetime, dict[str, Path]]
     """Dictionary of times and file paths"""
 
     required_vars: list[str]
     """The list of variables to be read from the files"""
 
     level_def: pd.DataFrame
-    """L60 model level definitions"""
+    """Model level definitions (L60 or L137)"""
 
     def __init__(self, dir: Path | str, required_vars: list[str] = []):
         """
         Prepare a CAMS EAC4 reanalysis product, in model levels
 
         Args:
             dir: The directory containing the files
@@ -48,15 +51,16 @@
             dir = Path(dir)
         self.dir = dir
         self.required_vars = required_vars
 
         # Read information about the vertical levels, required for creating the
         # 3D pressure field
         self.level_def = pd.read_csv(
-            importlib.resources.files(res) / "cams_eac4_model_levels.csv"
+            importlib.resources.files(res)
+            / "cams_l60.csv"  # Change filename in subclass!
         )
 
         self._explore_directory()
 
     def _explore_directory(self):
         """Traverses the directory to find CAMS files, reads time and variable info"""
 
@@ -119,16 +123,17 @@
             # Read coordinates
             data["longitude"] = ((ds["longitude"][:] - 180) % 360) - 180
             data["latitude"] = ds["latitude"][:]
             data["level"] = ds["level"][:]
 
         # Create the 3D pressure field
         psfc = sp.reshape(1, *sp.shape)
-        a = self.level_def["a [Pa]"].values.reshape(61, 1, 1)
-        b = self.level_def["b"].values.reshape(61, 1, 1)
+        n_levels = len(self.level_def.index)
+        a = self.level_def["a [Pa]"].values.reshape(n_levels, 1, 1)
+        b = self.level_def["b"].values.reshape(n_levels, 1, 1)
 
         pres_hf = a + b * psfc  # Half-level pressure
         pres = (pres_hf[1:, :, :] + pres_hf[:-1, :, :]) / 2  # Full-level pressure
         pres = pres / 100  # Convert to hPa
         data["pres"] = (("level", "latitude", "longitude"), pres)
 
         # Create dataset
@@ -143,7 +148,57 @@
         return ds
 
     @property
     def available_times(self) -> list[dt.datetime]:
         """Returns the list of available times"""
 
         return list(self.times.keys())
+
+
+class CAMS_EAC4(CAMS_Base):
+    def __init__(self, dir: Path | str, required_vars: list[str] = []):
+        """
+        Prepare a CAMS EAC4 reanalysis product, in model levels
+
+        Args:
+            dir: The directory containing the files
+            required_vars: A list of variables that are used and will be present in the
+                            returned datasets
+        """
+        if isinstance(dir, str):
+            dir = Path(dir)
+        self.dir = dir
+        self.required_vars = required_vars
+
+        # Read information about the vertical levels, required for creating the
+        # 3D pressure field
+        self.level_def = pd.read_csv(importlib.resources.files(res) / "cams_l60.csv")
+
+        self._explore_directory()
+
+    def __str__(self) -> str:
+        return f"CAMS EAC4({self.dir})"
+
+
+class CAMS_Global_Forecasts(CAMS_Base):
+    def __init__(self, dir: Path | str, required_vars: list[str] = []):
+        """
+        Prepare a CAMS Global Atmospheric Forecast product, in model levels
+
+        Args:
+            dir: The directory containing the files
+            required_vars: A list of variables that are used and will be present in the
+                            returned datasets
+        """
+        if isinstance(dir, str):
+            dir = Path(dir)
+        self.dir = dir
+        self.required_vars = required_vars
+
+        # Read information about the vertical levels, required for creating the
+        # 3D pressure field
+        self.level_def = pd.read_csv(importlib.resources.files(res) / "cams_l137.csv")
+
+        self._explore_directory()
+
+    def __str__(self) -> str:
+        return f"CAMS Global Forecasts({self.dir})"
```

### Comparing `interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/interpolation.py` & `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/interpolation.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/met_em.py` & `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/met_em.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/res/cams_eac4_model_levels.csv` & `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/res/cams_l60.csv`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/species_map.py` & `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/species_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 def convert_si(value: Any, from_prefix: str, to_prefix: str):
     if from_prefix == to_prefix:
         return value
     if from_prefix not in SI_PREFIX:
         raise ValueError(f"Unknown SI prefix {from_prefix}")
     if to_prefix not in SI_PREFIX:
         raise ValueError(f"Unknown SI prefix {to_prefix}")
-    print(f"From: {from_prefix}, To: {to_prefix}")
     return value * 10 ** (SI_PREFIX[from_prefix] - SI_PREFIX[to_prefix])
 
 
 @dataclass
 class Units:
     global_model: str = field(default="")
     regional_model: str = field(default="")
```

### Comparing `interpolator_for_wrfchem-1.1.0/interpolator_for_wrfchem/utils.py` & `interpolator_for_wrfchem-1.2.0/interpolator_for_wrfchem/utils.py`

 * *Files identical despite different names*

### Comparing `interpolator_for_wrfchem-1.1.0/pyproject.toml` & `interpolator_for_wrfchem-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interpolator-for-wrfchem"
-version = "1.1.0"
+version = "1.2.0"
 description = "Interpolates global chemistry fields for use with WRF-CHEM"
 authors = ["Thanasis Georgiou <ageorgiou@noa.gr>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 interpolator-for-wrfchem = "interpolator_for_wrfchem:main"
```

### Comparing `interpolator_for_wrfchem-1.1.0/PKG-INFO` & `interpolator_for_wrfchem-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpolator-for-wrfchem
-Version: 1.1.0
+Version: 1.2.0
 Summary: Interpolates global chemistry fields for use with WRF-CHEM
 Author: Thanasis Georgiou
 Author-email: ageorgiou@noa.gr
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cftime (>=1.6.3,<2.0.0)
@@ -27,15 +27,14 @@
 - Potentially support many global models (currently supports CAMS EAC4)
 
 The application is written in Python and is meant to be used a command-line tool. Some potential limitations:
 
 - The application currently assumes that fields are mixing ratios.
 - The global model fields should be on a regular lat-lon grid.
 - No nesting support
--
 
 ## Installation
 
 The application is available on PyPI and can be installed using pip:
 
 ```bash
 pip install interpolator-for-wrfchem
@@ -53,24 +52,31 @@
 The interpolator will update `wrfinput` and `wrfbdy` files to include the chemistry information.
 
 ![Workflow](./workflow.drawio.png)
 
 The interpolator is a command-line tool and can be run as follows:
 
 ```bash
-interpolator-for-wrfchem <global model data path> <met_em path> <wrfinput_d01 path> <wrfbdy_d01 path> <species map path> <output path>
+interpolator-for-wrfchem <global model name> <global model data path> <met_em path> <wrfinput path> <species map path>
 ```
 
-The `wrfinput_d01` and `wrfbdy_d01` files **WILL BE MODIFIED**!
+The `wrfinput` and `wrfbdy` files **WILL BE MODIFIED**! The `global model name` can be one of the following:
+
+- `cams_eac4`: CAMS EAC4 data (w/ 60 vertical levels)
+- `cams_global_forecasts`: CAMS global forecasts (w/ 137 vertical levels)
 
 There are some optional flags:
 
+- `--wrfbdy=`: Path to the `wrfbdy_d01` file, if not provided, the boundary is not updated.
 - `--copy-icbc`: Make a backup of the `wrfinput` and `wrfbdy` files before updating them.
-- `--no-ic` and `--no-bc`: Do not update the `wrfinput` and `wrfbdy` files, respectively.
-- `--diagnostics`: Store some diagnostic information in the `diag.nc` file.
+- `--no-ic`: Do not update the `wrfinput`. You must nonetheless provide the path to the `wrfinput` file as it is required to read some information.
+- `--diagnostics`: Store some diagnostic information in the `diag_cams_interp.nc` file.
+
+When you use nested domains, you can run the application multiple times, each time pointing to a different `wrfinput` file. You can omit the `wrfbdy` file when running the application for the nested domains' `wrfinput` files.
+If you need to update `wrfbdy` files for the future without touching `wrfinput` (e.g. for a cycling run), point to a correct `wrfinput` file (correct means it's the same model grid and configuration) and use the `--no-ic` flag.
 
 ## Species mapping
 
 In many cases, the available fields of the global model do not directly correspond to the ones used by the chemistry/dust scheme you want to use in WRF-CHEM. For example, you might have dust concentrations available in different size bins. The application supports "species mapping", through which the WRF-CHEM fields are created through a linear combination of global model fields, after interpolation.
 
 Detailed description of the species file format is available in [species_maps.md](./species_maps/species_maps.md).
```

