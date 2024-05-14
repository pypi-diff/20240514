# Comparing `tmp/pymatgen_io_validation-0.0.3.tar.gz` & `tmp/pymatgen_io_validation-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen_io_validation-0.0.3.tar", last modified: Wed May  8 23:24:14 2024, max compression
+gzip compressed data, was "pymatgen_io_validation-0.0.4.tar", last modified: Tue May 14 19:00:40 2024, max compression
```

## Comparing `pymatgen_io_validation-0.0.3.tar` & `pymatgen_io_validation-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.046465 pymatgen_io_validation-0.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/examples/MP_compliant_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.046465 pymatgen_io_validation-0.0.3/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.046465 pymatgen_io_validation-0.0.3/pymatgen/io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/pymatgen/io/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_common_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_for_excess_empty_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    42260 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_incar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_kpoints_kspacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_potcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/compare_to_MP_ehull.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15892 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pymatgen/io/validation/vasp_defaults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15266 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 23:24:14.000000 pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 23:24:14.054465 pymatgen_io_validation-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:24:14.050465 pymatgen_io_validation-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-05-08 23:24:09.000000 pymatgen_io_validation-0.0.3/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:40.362910 pymatgen_io_validation-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-14 19:00:40.362910 pymatgen_io_validation-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13771 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:40.358910 pymatgen_io_validation-0.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/examples/MP_compliant_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:40.354910 pymatgen_io_validation-0.0.4/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:40.358910 pymatgen_io_validation-0.0.4/pymatgen/io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:40.358910 pymatgen_io_validation-0.0.4/pymatgen/io/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_common_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_for_excess_empty_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42743 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_incar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_kpoints_kspacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_potcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/compare_to_MP_ehull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pymatgen/io/validation/vasp_defaults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:40.362910 pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-14 19:00:40.000000 pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-14 19:00:40.000000 pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:00:40.000000 pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 19:00:40.000000 pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 19:00:40.000000 pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-14 19:00:40.362910 pymatgen_io_validation-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:00:40.362910 pymatgen_io_validation-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    27307 2024-05-14 19:00:31.000000 pymatgen_io_validation-0.0.4/tests/test_validation.py
```

### Comparing `pymatgen_io_validation-0.0.3/LICENSE` & `pymatgen_io_validation-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.3/PKG-INFO` & `pymatgen_io_validation-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-io-validation
-Version: 0.0.3
+Version: 0.0.4
 Summary: A comprehensive I/O validator for electronic structure calculations
 Home-page: https://github.com/materialsproject/pymatgen-io-validation
 Author: Janosh Riebesell, Jason Munro, Aaron Kaplan
 Author-email: Matthew Kuner <matthewkuner@gmail.com>
 Maintainer: Matthew Kuner
 License: modified BSD
 Keywords: io,validation,dft,vasp
@@ -76,15 +76,15 @@
 
 
 Rationale
 ====
 
 | **Parameter** | **Reason** |
 | ---- | ---- |
-| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states “please do not use this tag [ADDGRID] as default in all your calculations!”. ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
+| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states "please do not use this tag [ADDGRID] as default in all your calculations!". ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
 | AEXX / AMGGAX / AMGGAC / AGGAX / ALDAC / ALDAX | These parameters should be the VASP defaults unless otherwise specified in a given MP input set, as changing them is effectively a change to the level of theory. |
 | ALGO / IALGO | ALGO must be one of: "Normal", "Conjugate", "All", "Fast", "Exact". (This corresponds to an IALGO of 38, 58, 58, 68, 90, respectively). |
 | DEPER / EBREAK / WEIMIN | DEPER, EBREAK, and WEIMIN should not be changed according to the VASP wiki, hence MP requires them to remain as their default values. |
 | EDIFF | EDIFF must be equal to or greater than the value in the relevant MP input set. This will ensure compatibility between results with those in the MP Database. |
 | EDIFFG | Should be the same or better than in the relevant MP input set. For MP input sets with an energy-based cutoff, the calculation must have an energy change between the last two steps be less in magnitude than the specified EDIFFG (so even if your calculation uses force-based convergence, the energy must converge within the MP input set’s specification). The same logic applies to MP input sets with force-based EDIFFG settings. |
 | EFERMI | EFERMI must be one of: "LEGACY", "MIDGAP" |
 | EFIELD | Current MP input sets used to construct the main MP database do not set EFIELD, and hence we require this to be unset or set to 0. |
@@ -121,23 +121,23 @@
 | LMONO | LMONO must be set to False (the VASP default). |
 | LEFG | LEFG must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
 | LEPSILON | LEPSILON must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
 | LHFCALC | The value of LHFCALC should match that of the relevant MP input set, as it will otherwise result in a change in the level of theory applied in the calculation. |
 | LHYPERFINE | LHYPERFINE must be set to False (the VASP default). |
 | LKPROJ | LKPROJ must be set to False (the VASP default). |
 | LKPOINTS_OPT | LKPOINTS_OPT must be set to False. |
-| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that “Energies should be evaluated with the default setting for LMAXPAW”. |
-| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the “bench_vasp_pars.docx” document in https://github.com/materialsproject/pymatgen/issues/3322. |
+| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that "Energies should be evaluated with the default setting for LMAXPAW". |
+| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the "bench_vasp_pars.docx" document in https://github.com/materialsproject/pymatgen/issues/3322. |
 | LMAXTAU | LMAXTAU must be set to 6 (the VASP default when using LASPH = True). |
 | LMP2LT / LSMP2LT | Both must be set to False (VASP defaults) |
 | LNONCOLLINEAR / LSORBIT | Both must be set to False (VASP defaults) |
 | LOCPROJ | LOCPROJ must be set to None (the VASP default). |
 | LOPTICS | LOPTICS must be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
 | LORBIT | LORBIT must **<u>*not*</u>** be None if the user also sets ISPIN=2, otherwise all values of LORBIT are acceptable. This is due to magnetization values not being output when ISPIN=2 and LORBIT = None are set together. |
-| LREAL | If the LREAL in the relevant MP input set is “Auto”, then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
+| LREAL | If the LREAL in the relevant MP input set is "Auto", then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
 | LRPA | LRPA must be set to False (the VASP default). MP does not currently support random phase approximation (RPA) calculations. |
 | LSPECTRAL | LSPECTRAL must be set to False (the VASP default for most calculations). |
 | LSUBROT | LSUBROT must be set to False (the VASP default). |
 | MAGMOM | While any initial magnetic moments are allowed, the final total magnetic moment for any given atom must be less than 5 $\mu_B$ (Bohr magnetons) (except for elements Gd and Eu, which must be less than 10 $\mu_B$). This simply serves as a filter for erroneous data. |
 | ML_LMFF | ML_LMFF must be set to False (the VASP default). |
 | NGX / NGY / NGZ | The values for NGX/NGY/NGZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
 | NGFX / NGFY / NGFZ | The values for NGFX/NGFY/NGFZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
```

### Comparing `pymatgen_io_validation-0.0.3/README.md` & `pymatgen_io_validation-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 Rationale
 ====
 
 | **Parameter** | **Reason** |
 | ---- | ---- |
-| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states “please do not use this tag [ADDGRID] as default in all your calculations!”. ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
+| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states "please do not use this tag [ADDGRID] as default in all your calculations!". ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
 | AEXX / AMGGAX / AMGGAC / AGGAX / ALDAC / ALDAX | These parameters should be the VASP defaults unless otherwise specified in a given MP input set, as changing them is effectively a change to the level of theory. |
 | ALGO / IALGO | ALGO must be one of: "Normal", "Conjugate", "All", "Fast", "Exact". (This corresponds to an IALGO of 38, 58, 58, 68, 90, respectively). |
 | DEPER / EBREAK / WEIMIN | DEPER, EBREAK, and WEIMIN should not be changed according to the VASP wiki, hence MP requires them to remain as their default values. |
 | EDIFF | EDIFF must be equal to or greater than the value in the relevant MP input set. This will ensure compatibility between results with those in the MP Database. |
 | EDIFFG | Should be the same or better than in the relevant MP input set. For MP input sets with an energy-based cutoff, the calculation must have an energy change between the last two steps be less in magnitude than the specified EDIFFG (so even if your calculation uses force-based convergence, the energy must converge within the MP input set’s specification). The same logic applies to MP input sets with force-based EDIFFG settings. |
 | EFERMI | EFERMI must be one of: "LEGACY", "MIDGAP" |
 | EFIELD | Current MP input sets used to construct the main MP database do not set EFIELD, and hence we require this to be unset or set to 0. |
@@ -85,23 +85,23 @@
 | LMONO | LMONO must be set to False (the VASP default). |
 | LEFG | LEFG must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
 | LEPSILON | LEPSILON must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
 | LHFCALC | The value of LHFCALC should match that of the relevant MP input set, as it will otherwise result in a change in the level of theory applied in the calculation. |
 | LHYPERFINE | LHYPERFINE must be set to False (the VASP default). |
 | LKPROJ | LKPROJ must be set to False (the VASP default). |
 | LKPOINTS_OPT | LKPOINTS_OPT must be set to False. |
-| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that “Energies should be evaluated with the default setting for LMAXPAW”. |
-| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the “bench_vasp_pars.docx” document in https://github.com/materialsproject/pymatgen/issues/3322. |
+| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that "Energies should be evaluated with the default setting for LMAXPAW". |
+| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the "bench_vasp_pars.docx" document in https://github.com/materialsproject/pymatgen/issues/3322. |
 | LMAXTAU | LMAXTAU must be set to 6 (the VASP default when using LASPH = True). |
 | LMP2LT / LSMP2LT | Both must be set to False (VASP defaults) |
 | LNONCOLLINEAR / LSORBIT | Both must be set to False (VASP defaults) |
 | LOCPROJ | LOCPROJ must be set to None (the VASP default). |
 | LOPTICS | LOPTICS must be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
 | LORBIT | LORBIT must **<u>*not*</u>** be None if the user also sets ISPIN=2, otherwise all values of LORBIT are acceptable. This is due to magnetization values not being output when ISPIN=2 and LORBIT = None are set together. |
-| LREAL | If the LREAL in the relevant MP input set is “Auto”, then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
+| LREAL | If the LREAL in the relevant MP input set is "Auto", then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
 | LRPA | LRPA must be set to False (the VASP default). MP does not currently support random phase approximation (RPA) calculations. |
 | LSPECTRAL | LSPECTRAL must be set to False (the VASP default for most calculations). |
 | LSUBROT | LSUBROT must be set to False (the VASP default). |
 | MAGMOM | While any initial magnetic moments are allowed, the final total magnetic moment for any given atom must be less than 5 $\mu_B$ (Bohr magnetons) (except for elements Gd and Eu, which must be less than 10 $\mu_B$). This simply serves as a filter for erroneous data. |
 | ML_LMFF | ML_LMFF must be set to False (the VASP default). |
 | NGX / NGY / NGZ | The values for NGX/NGY/NGZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
 | NGFX / NGFY / NGFZ | The values for NGFX/NGFY/NGFZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
```

### Comparing `pymatgen_io_validation-0.0.3/examples/MP_compliant_job.py` & `pymatgen_io_validation-0.0.4/examples/MP_compliant_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from jobflow import Flow
 from monty.serialization import dumpfn
 import numpy as np
 from pymatgen.core import Structure, Lattice
 
 
 def get_GaAs_structure(a0: float = 5.6) -> Structure:
-
     lattice_vectors = a0 * np.array([[0.0 if i == j else 0.5 for j in range(3)] for i in range(3)])
     return Structure(
         lattice=Lattice(lattice_vectors),
         species=["Ga", "As"],
         coords=[[0.125, 0.125, 0.125], [0.875, 0.875, 0.875]],
         coords_are_cartesian=False,
     )
@@ -28,17 +27,19 @@
     else:
         flow.metadata = metadata.copy()
         if name:
             flow.name = name
 
 
 def get_MP_compliant_r2SCAN_flow(
-    structure: Structure, user_incar_settings: dict | None = None, metadata: dict | None = None, name: str | None = None
+    structure: Structure,
+    user_incar_settings: dict | None = None,
+    metadata: dict | None = None,
+    name: str | None = None,
 ) -> Flow:
-
     from atomate2.vasp.jobs.mp import MPMetaGGAStaticMaker
     from atomate2.vasp.powerups import update_user_incar_settings
 
     maker = MPMetaGGAStaticMaker()
 
     user_incar_settings = user_incar_settings or {}
     if len(user_incar_settings) > 0:
@@ -49,28 +50,26 @@
     metadata = metadata or {}
     assign_meta(flow, metadata, name=name)
 
     return flow
 
 
 def run_job_fully_locally(flow, job_store=None):
-
     from jobflow import run_locally, JobStore
     from maggma.stores import MemoryStore
 
     if job_store is None:
         job_store = JobStore(MemoryStore(), additional_stores={"data": MemoryStore()})
 
     response = run_locally(flow, store=job_store, create_folders=True)
     uuid = list(response)[0]
     return response[uuid][1].output
 
 
 def MP_compliant_calc():
-
     structure = get_GaAs_structure()
     flow = get_MP_compliant_r2SCAN_flow(
         structure=structure,
         user_incar_settings={  # some forward-looking settings
             "LREAL": False,
             "LMAXMIX": 6,
             "LCHARG": False,  # following tags just set for convenience
@@ -80,15 +79,14 @@
             "KPAR": 2,
         },
     )
     return run_job_fully_locally(flow)
 
 
 def MP_non_compliant_calc():
-
     structure = get_GaAs_structure()
     flow = get_MP_compliant_r2SCAN_flow(
         structure=structure,
         user_incar_settings={  # some backward-looking settings
             "ENCUT": 450.0,
             "ENAUG": 900.0,
             "KSPACING": 0.5,
@@ -99,24 +97,25 @@
             "KPAR": 2,
         },
     )
     return run_job_fully_locally(flow)
 
 
 def MP_flows() -> None:
-
     compliant_task_doc = MP_compliant_calc()
     dumpfn(jsanitize(compliant_task_doc), "./MP_compatible_GaAs_r2SCAN_static.json.gz")
 
     non_compliant_task_doc = MP_non_compliant_calc()
-    dumpfn(jsanitize(non_compliant_task_doc), "./MP_incompatible_GaAs_r2SCAN_static.json.gz")
+    dumpfn(
+        jsanitize(non_compliant_task_doc),
+        "./MP_incompatible_GaAs_r2SCAN_static.json.gz",
+    )
 
 
 def generate_task_documents(cdir, task_id: str | None = None, filename: str | None = None) -> TaskDocument:
-
     from atomate.vasp.drones import VaspDrone
     from emmet.core.mpid import MPID
 
     drone = VaspDrone(store_volumetric_data=[])
     task_doc_dict = drone.assimilate(cdir)
 
     task_id = task_id or "mp-100000000"
@@ -126,9 +125,8 @@
     if filename:
         dumpfn(jsanitize(task_doc), filename)
 
     return task_doc
 
 
 if __name__ == "__main__":
-
     MP_flows()
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/__init__.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_common_errors.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_common_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     def _check_parse(self) -> None:
         if self.parameters == {} or self.parameters is None:
             self.reasons.append(
                 "CAN NOT PROPERLY PARSE CALCULATION --> Issue parsing input parameters from the vasprun.xml file."
             )
 
     def _check_gga_and_metagga(self) -> None:
-
         # Check for cases where both GGA and METAGGA are set. This should *not* be allowed, as it can erroneously change
         # the outputted energy significantly. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867
         # for more details.
         if self.incar.get("GGA", "--") != "--" and str(self.incar.get("METAGGA", None)).lower() not in {"--", "none"}:
             self.reasons.append(
                 "KNOWN BUG --> GGA and METAGGA should never be specified together, as this can cause major errors in the "
                 "outputted energy. See https://github.com/materialsproject/atomate2/issues/453#issuecomment-1699605867 "
@@ -97,15 +96,14 @@
 
     def _check_electronic_convergence(self) -> None:
         # check if structure electronically converged
 
         if self.incar.get("ALGO", self.defaults["ALGO"]["value"]).lower() != "chi":
             # Response function calculations are non-self-consistent: only one ionic step, no electronic SCF
             if self.parameters.get("LEPSILON", self.defaults["LEPSILON"]["value"]):
-
                 final_esteps = self.ionic_steps[-1]["electronic_steps"]
                 to_check = {"e_wo_entrp", "e_fr_energy", "e_0_energy"}
 
                 for i in range(len(final_esteps)):
                     if set(final_esteps[i]) != to_check:
                         break
                     i += 1
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_for_excess_empty_space.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_for_excess_empty_space.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,19 @@
     max_lattice_vec_2_empty_dist = max(lattice_vec_2_diffs) * lattice_vec_lengths[1]
 
     lattice_vec_3_frac_coords = list(np.sort(fcoords[:, 2]))
     lattice_vec_3_frac_coords.append(lattice_vec_3_frac_coords[0] + 1)
     lattice_vec_3_diffs = np.diff(lattice_vec_3_frac_coords)
     max_lattice_vec_3_empty_dist = max(lattice_vec_3_diffs) * lattice_vec_lengths[2]
 
-    max_empty_distance = max(max_lattice_vec_1_empty_dist, max_lattice_vec_2_empty_dist, max_lattice_vec_3_empty_dist)
+    max_empty_distance = max(
+        max_lattice_vec_1_empty_dist,
+        max_lattice_vec_2_empty_dist,
+        max_lattice_vec_3_empty_dist,
+    )
 
     # Check 2: get max voronoi polyhedra volume in structure
     def get_max_voronoi_polyhedra_volume(structure):
         max_voronoi_polyhedra_vol = 0
         vnn = VoronoiNN().get_all_voronoi_polyhedra(structure)
         for polyhedra in vnn:
             for key in polyhedra.keys():
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_incar.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_incar.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         # defaults to unspecified INCAR tags, and by updating
         # any INCAR tag that has a specified update method
         working_params.update_parameters_and_defaults()
 
         # Validate each parameter in the set of working parameters
         simple_validator = BasicValidator()
         for key in working_params.defaults:
-
             if self.fast and len(self.reasons) > 0:
                 # fast check: stop checking whenever a single check fails
                 break
 
             simple_validator.check_parameter(
                 reasons=self.reasons,
                 warnings=self.warnings,
@@ -322,15 +321,18 @@
             self.valid_values["LREAL"] = ["FALSE", "AUTO", "A"]
         elif str(self.input_set.incar.get("LREAL")).upper() in ["FALSE"]:
             self.valid_values["LREAL"] = ["FALSE"]
 
         self.parameters["LREAL"] = str(self._incar.get("LREAL", self.defaults["LREAL"]["value"])).upper()
         # PREC.
         self.parameters["PREC"] = self.parameters["PREC"].upper()
-        if self.input_set.incar.get("PREC", self.defaults["PREC"]["value"]).upper() in ["ACCURATE", "HIGH"]:
+        if self.input_set.incar.get("PREC", self.defaults["PREC"]["value"]).upper() in [
+            "ACCURATE",
+            "HIGH",
+        ]:
             self.valid_values["PREC"] = ["ACCURATE", "ACCURA", "HIGH"]
         else:
             raise ValueError("Validation code check for PREC tag needs to be updated to account for a new input set!")
         self.defaults["PREC"]["operation"] = "in"
 
         # ROPT. Should be better than or equal to default for the PREC level.
         # This only matters if projectors are done in real-space.
@@ -370,15 +372,18 @@
             self.valid_values["EFERMI"] = ["LEGACY", "MIDGAP"]
             self.defaults["EFERMI"]["operation"] = "in"
 
         # IWAVPR.
         if self._incar.get("IWAVPR"):
             self.parameters["IWAVPR"] = self._incar["IWAVPR"] if self._incar["IWAVPR"] is not None else 0
             self.defaults["IWAVPR"].update(
-                {"operation": "==", "comment": "VASP discourages users from setting the IWAVPR tag (as of July 2023)."}
+                {
+                    "operation": "==",
+                    "comment": "VASP discourages users from setting the IWAVPR tag (as of July 2023).",
+                }
             )
 
         # LCORR.
         if self.parameters["IALGO"] != 58:
             self.defaults["LCORR"].update(
                 {
                     "operation": "==",
@@ -447,16 +452,24 @@
 
         grid_keys = {"NGX", "NGXF", "NGY", "NGYF", "NGZ", "NGZF"}
         # NGX/Y/Z and NGXF/YF/ZF. Not checked if not in INCAR file (as this means the VASP default was used).
         if any(i for i in grid_keys if i in self._incar.keys()):
             self.valid_values["ENMAX"] = max(self.parameters["ENMAX"], self.valid_values["ENMAX"])
 
             (
-                [self.valid_values["NGX"], self.valid_values["NGY"], self.valid_values["NGZ"]],
-                [self.valid_values["NGXF"], self.valid_values["NGYF"], self.valid_values["NGZF"]],
+                [
+                    self.valid_values["NGX"],
+                    self.valid_values["NGY"],
+                    self.valid_values["NGZ"],
+                ],
+                [
+                    self.valid_values["NGXF"],
+                    self.valid_values["NGYF"],
+                    self.valid_values["NGZF"],
+                ],
             ) = self.input_set.calculate_ng(custom_encut=self.valid_values["ENMAX"])
 
             for key in grid_keys:
                 self.valid_values[key] = int(self.valid_values[key] * self._fft_grid_tolerance)
 
                 self.defaults[key] = {
                     "value": self.valid_values[key],
@@ -562,15 +575,16 @@
 
         # Also check if SIGMA is too large according to the VASP wiki,
         # which occurs when the entropy term in the energy is greater than 1 meV/atom.
         self.parameters["ELECTRONIC ENTROPY"] = -1e20
         for ionic_step in self._ionic_steps:
             if eentropy := ionic_step["electronic_steps"][-1].get("eentropy"):
                 self.parameters["ELECTRONIC ENTROPY"] = max(
-                    self.parameters["ELECTRONIC ENTROPY"], abs(eentropy / self.structure.num_sites)
+                    self.parameters["ELECTRONIC ENTROPY"],
+                    abs(eentropy / self.structure.num_sites),
                 )
 
         convert_eV_to_meV = 1000
         self.parameters["ELECTRONIC ENTROPY"] = round(self.parameters["ELECTRONIC ENTROPY"] * convert_eV_to_meV, 3)
         self.valid_values["ELECTRONIC ENTROPY"] = 0.001 * convert_eV_to_meV
 
         self.defaults["ELECTRONIC ENTROPY"] = {
@@ -698,15 +712,16 @@
             # Check for large changes in energy between ionic steps (usually indicates too high POTIM)
             if self._nionic_steps > 1:
                 # Do not use `e_0_energy`, as there is a bug in the vasprun.xml when printing that variable
                 # (see https://www.vasp.at/forum/viewtopic.php?t=16942 for more details).
                 cur_ionic_step_energies = [ionic_step["e_fr_energy"] for ionic_step in self._ionic_steps]
                 cur_ionic_step_energy_gradient = np.diff(cur_ionic_step_energies)
                 self.parameters["MAX ENERGY GRADIENT"] = round(
-                    max(np.abs(cur_ionic_step_energy_gradient)) / self.structure.num_sites, 3
+                    max(np.abs(cur_ionic_step_energy_gradient)) / self.structure.num_sites,
+                    3,
                 )
                 self.valid_values["MAX ENERGY GRADIENT"] = 1
                 self.defaults["MAX ENERGY GRADIENT"] = {
                     "value": None,
                     "tag": "ionic",
                     "operation": "<=",
                     "comment": (
@@ -732,15 +747,16 @@
 
         if self.task_doc["output"]["forces"] is None:
             self.defaults["EDIFFG"]["warning"] = "TaskDoc does not contain output forces!"
             self.defaults["EDIFFG"]["operation"] = "auto fail"
 
         elif self.valid_values["EDIFFG"] < 0.0:
             self.parameters["EDIFFG"] = round(
-                max([np.linalg.norm(force_on_atom) for force_on_atom in self.task_doc["output"]["forces"]]), 3
+                max([np.linalg.norm(force_on_atom) for force_on_atom in self.task_doc["output"]["forces"]]),
+                3,
             )
 
             self.valid_values["EDIFFG"] = abs(self.valid_values["EDIFFG"])
             self.defaults["EDIFFG"].update(
                 {
                     "value": self.defaults["EDIFFG"]["value"],
                     "operation": "<=",
@@ -784,15 +800,25 @@
     -----------
     operations : set[str]
         List of acceptable operations, such as "==" for strict equality, or "in" to
         check if a Sequence contains an element
     """
 
     # avoiding dunder methods because these raise too many NotImplemented's
-    operations: set[str | None] = {"==", ">", ">=", "<", "<=", "in", "approx", "auto fail", None}
+    operations: set[str | None] = {
+        "==",
+        ">",
+        ">=",
+        "<",
+        "<=",
+        "in",
+        "approx",
+        "auto fail",
+        None,
+    }
 
     def __init__(self, global_tolerance=1.0e-4) -> None:
         """Set math.isclose tolerance"""
         self.tolerance = global_tolerance
 
     def _comparator(self, lhs: Any, operation: str, rhs: Any, **kwargs) -> bool:
         """
@@ -862,14 +888,17 @@
         append_comments : str or None (default)
             Additional comments that may be helpful for the user to understand why
             a check failed.
         """
 
         append_comments = append_comments or ""
 
+        if isinstance(current_value, str):
+            current_value = current_value.upper()
+
         kwargs: dict[str, Any] = {}
         if operation == "approx" and isinstance(current_value, float):
             kwargs.update({"rel_tol": tolerance or self.tolerance, "abs_tol": 0.0})
         valid_value = self._comparator(current_value, operation, reference_value, **kwargs)
 
         if not valid_value:
             error_list.append(
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_kpoints_kspacing.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_kpoints_kspacing.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,17 @@
         # Check number of kpoints used
         valid_num_kpts = self._get_valid_num_kpts()
 
         if isinstance(self.kpoints, Kpoints):
             self.kpoints = self.kpoints.as_dict()
 
         cur_num_kpts = max(
-            self.kpoints.get("nkpoints", 0), np.prod(self.kpoints.get("kpoints")), len(self.kpoints.get("kpoints"))
+            self.kpoints.get("nkpoints", 0),
+            np.prod(self.kpoints.get("kpoints")),
+            len(self.kpoints.get("kpoints")),
         )
         if cur_num_kpts < valid_num_kpts:
             self.reasons.append(
                 f"INPUT SETTINGS --> KPOINTS or KSPACING: {cur_num_kpts} kpoints were "
                 f"used, but it should have been at least {valid_num_kpts}."
             )
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_package_versions.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_package_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Optionally check whether package versions are up to date. """
+"""Optionally check whether package versions are up to date."""
 
 from __future__ import annotations
 from importlib.metadata import version
 import requests
 import warnings
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/check_potcar.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/check_potcar.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,21 @@
                         # quick return, only matters that one POTCAR didn't match
                         break
 
             if len(incorrect_potcars) > 0:
                 # format error string
                 incorrect_potcars = [potcar.split("_")[0] for potcar in incorrect_potcars]
                 if len(incorrect_potcars) == 2:
-                    incorrect_potcars = ", ".join(incorrect_potcars[:-1]) + f" and {incorrect_potcars[-1]}"  # type: ignore
+                    incorrect_potcars = (
+                        ", ".join(incorrect_potcars[:-1]) + f" and {incorrect_potcars[-1]}"
+                    )  # type: ignore
                 elif len(incorrect_potcars) >= 3:
-                    incorrect_potcars = ", ".join(incorrect_potcars[:-1]) + "," + f" and {incorrect_potcars[-1]}"  # type: ignore
+                    incorrect_potcars = (
+                        ", ".join(incorrect_potcars[:-1]) + "," + f" and {incorrect_potcars[-1]}"
+                    )  # type: ignore
 
                 self.reasons.append(
                     f"PSEUDOPOTENTIALS --> Incorrect POTCAR files were used for {incorrect_potcars}. "
                     "Alternatively, our potcar checker may have an issue--please create a GitHub issue if you "
                     "believe the POTCARs used are correct."
                 )
 
@@ -153,14 +157,16 @@
             set(potcar_stats_1["keywords"].get(key)) == set(potcar_stats_2["keywords"].get(key))  # type: ignore
             for key in ["header", "data"]
         )
 
         data_match = False
         if key_match:
             data_diff = [
-                abs(potcar_stats_1["stats"].get(key, {}).get(stat) - potcar_stats_2["stats"].get(key, {}).get(stat))  # type: ignore
+                abs(
+                    potcar_stats_1["stats"].get(key, {}).get(stat) - potcar_stats_2["stats"].get(key, {}).get(stat)
+                )  # type: ignore
                 for stat in ["MEAN", "ABSMEAN", "VAR", "MIN", "MAX"]
                 for key in ["header", "data"]
             ]
             data_match = all(np.array(data_diff) < self.data_match_tol)
 
         return key_match and data_match
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/common.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Common class constructor for validation checks. """
+"""Common class constructor for validation checks."""
 
 from dataclasses import dataclass
 
 
 @dataclass
 class BaseValidator:
     """
@@ -43,13 +43,12 @@
         Execute any checks on the class with a name prefix `_check_`.
 
         See class docstr for an example.
         """
 
         checklist = {attr for attr in dir(self) if attr.startswith("_check_")}
         for attr in checklist:
-
             if self.fast and len(self.reasons) > 0:
                 # fast check: stop checking whenever a single check fails
                 break
 
             getattr(self, attr)()
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/compare_to_MP_ehull.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/compare_to_MP_ehull.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,18 @@
     elements = task_doc.output.structure.composition.to_reduced_dict.keys()
 
     with MPRester(mp_api_key) as mpr:
         # Obtain GGA, GGA+U, and r2SCAN ComputedStructureEntry objects
         entries = mpr.get_entries_in_chemsys(
             elements=elements,
             compatible_only=True,
-            additional_criteria={"thermo_types": ["GGA_GGA+U", "R2SCAN"], "is_stable": True},
+            additional_criteria={
+                "thermo_types": ["GGA_GGA+U", "R2SCAN"],
+                "is_stable": True,
+            },
         )
 
         entries.append(cur_structure_entry)
 
         # Apply corrections locally with the mixing scheme
         scheme = MaterialsProjectDFTMixingScheme()
         corrected_entries = scheme.process_entries(entries)
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/settings.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # mypy: ignore-errors
 
 """
 Settings for pymatgen-io-validation. Used to be part of EmmetSettings.
 """
+
 from importlib.resources import files as import_resource_files
 import json
 from pathlib import Path
 from typing import Dict, Type, TypeVar, Union
 
 import requests
 from monty.json import MontyDecoder
@@ -59,14 +60,16 @@
             "GGA Structure Optimization": "pymatgen.io.vasp.sets.MPRelaxSet",
             "GGA+U Structure Optimization": "pymatgen.io.vasp.sets.MPRelaxSet",
             "R2SCAN Structure Optimization": "pymatgen.io.vasp.sets.MPScanRelaxSet",
             "SCAN Structure Optimization": "pymatgen.io.vasp.sets.MPScanRelaxSet",
             "PBESol Structure Optimization": "pymatgen.io.vasp.sets.MPScanRelaxSet",
             "GGA Static": "pymatgen.io.vasp.sets.MPStaticSet",
             "GGA+U Static": "pymatgen.io.vasp.sets.MPStaticSet",
+            "PBE Static": "pymatgen.io.vasp.sets.MPStaticSet",
+            "PBE+U Static": "pymatgen.io.vasp.sets.MPStaticSet",
             "R2SCAN Static": "pymatgen.io.vasp.sets.MPScanStaticSet",
             "SCAN Static": "pymatgen.io.vasp.sets.MPScanStaticSet",
             "PBESol Static": "pymatgen.io.vasp.sets.MPScanStaticSet",
             "HSE06 Static": "pymatgen.io.vasp.sets.MPScanStaticSet",
             "GGA NSCF Uniform": "pymatgen.io.vasp.sets.MPNonSCFSet",
             "GGA+U NSCF Uniform": "pymatgen.io.vasp.sets.MPNonSCFSet",
             "GGA NSCF Line": "pymatgen.io.vasp.sets.MPNonSCFSet",
@@ -118,15 +121,15 @@
         config_file_path: str = values.get("config_file", DEFAULT_CONFIG_FILE_PATH)
 
         new_values = {}
 
         if config_file_path.startswith("http"):
             new_values = requests.get(config_file_path).json()
         elif Path(config_file_path).exists():
-            with open(config_file_path) as f:
+            with open(config_file_path, encoding="utf8") as f:
                 new_values = json.load(f)
 
         new_values.update(values)
 
         return new_values
 
     @classmethod
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/validation.py` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     CheckCommonErrors,
     CheckVaspVersion,
 )
 from pymatgen.io.validation.check_kpoints_kspacing import CheckKpointsKspacing
 from pymatgen.io.validation.check_potcar import CheckPotcar
 from pymatgen.io.validation.settings import IOValidationSettings
 
-from typing import TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
 
 SETTINGS = IOValidationSettings()
 _vasp_defaults = loadfn(SETTINGS.VASP_DEFAULTS_FILENAME)
 
@@ -49,15 +49,15 @@
 
 
 class ValidationDoc(EmmetBaseModel):
     """
     Validation document for a VASP calculation
     """
 
-    task_id: MPID = Field(..., description="The task_id for this validation document")
+    task_id: Optional[MPID] = Field(None, description="The task_id for this validation document")
 
     valid: bool = Field(False, description="Whether this task is valid or not")
 
     last_updated: datetime = Field(
         description="Last updated date for this document",
         default_factory=datetime.utcnow,
     )
@@ -151,17 +151,15 @@
 
         # used for INCAR tag checks where you need to look at the actual INCAR (semi-rare)
         incar = calcs_reversed[0]["input"]["incar"]
 
         orig_inputs = {} if (task_doc["orig_inputs"] is None) else task_doc["orig_inputs"]
 
         cls_kwargs: dict[str, Any] = {
-            "task_id": (
-                task_doc["task_id"] if task_doc["task_id"] else -1
-            ),  # Unsure about what might be a better way to do this...
+            "task_id": task_doc["task_id"] if task_doc["task_id"] else None,
             "calc_type": _get_calc_type(calcs_reversed, orig_inputs),
             "task_type": _get_task_type(calcs_reversed, orig_inputs),
             "run_type": _get_run_type(calcs_reversed),
             "reasons": [],
             "warnings": [],
         }
 
@@ -186,25 +184,29 @@
             structure = calcs_reversed[0]["input"]["structure"]
         else:
             structure = task_doc["input"]["structure"] or task_doc["output"]["structure"]
         structure = Structure.from_dict(structure)
 
         try:
             valid_input_set = _get_input_set(
-                cls_kwargs["run_type"], cls_kwargs["task_type"], cls_kwargs["calc_type"], structure, input_sets, bandgap
+                cls_kwargs["run_type"],
+                cls_kwargs["task_type"],
+                cls_kwargs["calc_type"],
+                structure,
+                input_sets,
+                bandgap,
             )
         except Exception as e:
             cls_kwargs["reasons"].append(
                 "NO MATCHING MP INPUT SET --> no matching MP input set was found. If you believe this to be a mistake, please create a GitHub issue."
             )
             valid_input_set = None
             print(f"Error while finding MP input set: {e}.")
 
         if valid_input_set:
-
             # Tests ordered by expected computational burden - help optimize `fast` check
             # Intuitively, more important checks (INCAR, KPOINTS, and POTCAR settings) would come first
             # But to optimize speed in fast mode (relevant for validating a large batch of calculations)
             # the faster checks have to come first:
             #   1. VASP version
             #   2. Common errors (known bugs in VASP, erratic SCF convergence, etc.)
             #   3. KPOINTS or KSPACING (from INCAR)
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen/io/validation/vasp_defaults.yaml` & `pymatgen_io_validation-0.0.4/pymatgen/io/validation/vasp_defaults.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
   tag: chemical shift
   operation: ==
 LNONCOLLINEAR:
   value: false
   tag: ncl
   operation: ==
 LOCPROJ:
-  value: None
+  value: NONE
   tag: misc
   operation: ==
 LOPTICS:
   value: false
   tag: tddft
   operation: ==
 LORBIT:
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/PKG-INFO` & `pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-io-validation
-Version: 0.0.3
+Version: 0.0.4
 Summary: A comprehensive I/O validator for electronic structure calculations
 Home-page: https://github.com/materialsproject/pymatgen-io-validation
 Author: Janosh Riebesell, Jason Munro, Aaron Kaplan
 Author-email: Matthew Kuner <matthewkuner@gmail.com>
 Maintainer: Matthew Kuner
 License: modified BSD
 Keywords: io,validation,dft,vasp
@@ -76,15 +76,15 @@
 
 
 Rationale
 ====
 
 | **Parameter** | **Reason** |
 | ---- | ---- |
-| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states “please do not use this tag [ADDGRID] as default in all your calculations!”. ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
+| ADDGRID | ADDGRID must be set to False. MP uses ADDGRID = False, as the VASP manual states "please do not use this tag [ADDGRID] as default in all your calculations!". ADDGRID can affect the outputted forces, hence all calculations are thus required to have ADDGRID = False for compatibility. |
 | AEXX / AMGGAX / AMGGAC / AGGAX / ALDAC / ALDAX | These parameters should be the VASP defaults unless otherwise specified in a given MP input set, as changing them is effectively a change to the level of theory. |
 | ALGO / IALGO | ALGO must be one of: "Normal", "Conjugate", "All", "Fast", "Exact". (This corresponds to an IALGO of 38, 58, 58, 68, 90, respectively). |
 | DEPER / EBREAK / WEIMIN | DEPER, EBREAK, and WEIMIN should not be changed according to the VASP wiki, hence MP requires them to remain as their default values. |
 | EDIFF | EDIFF must be equal to or greater than the value in the relevant MP input set. This will ensure compatibility between results with those in the MP Database. |
 | EDIFFG | Should be the same or better than in the relevant MP input set. For MP input sets with an energy-based cutoff, the calculation must have an energy change between the last two steps be less in magnitude than the specified EDIFFG (so even if your calculation uses force-based convergence, the energy must converge within the MP input set’s specification). The same logic applies to MP input sets with force-based EDIFFG settings. |
 | EFERMI | EFERMI must be one of: "LEGACY", "MIDGAP" |
 | EFIELD | Current MP input sets used to construct the main MP database do not set EFIELD, and hence we require this to be unset or set to 0. |
@@ -121,23 +121,23 @@
 | LMONO | LMONO must be set to False (the VASP default). |
 | LEFG | LEFG must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
 | LEPSILON | LEPSILON must be set to False (the VASP default), unless explicitly specified to be True by the relevant MP input set. |
 | LHFCALC | The value of LHFCALC should match that of the relevant MP input set, as it will otherwise result in a change in the level of theory applied in the calculation. |
 | LHYPERFINE | LHYPERFINE must be set to False (the VASP default). |
 | LKPROJ | LKPROJ must be set to False (the VASP default). |
 | LKPOINTS_OPT | LKPOINTS_OPT must be set to False. |
-| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that “Energies should be evaluated with the default setting for LMAXPAW”. |
-| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the “bench_vasp_pars.docx” document in https://github.com/materialsproject/pymatgen/issues/3322. |
+| LMAXPAW | LMAXPAW must remain unspecified, as the VASP wiki states that "Energies should be evaluated with the default setting for LMAXPAW". |
+| LMAXMIX | LMAXMIX must be set to 6. This is based on tests from Aaron Kaplan (@esoteric-ephemera) — see the "bench_vasp_pars.docx" document in https://github.com/materialsproject/pymatgen/issues/3322. |
 | LMAXTAU | LMAXTAU must be set to 6 (the VASP default when using LASPH = True). |
 | LMP2LT / LSMP2LT | Both must be set to False (VASP defaults) |
 | LNONCOLLINEAR / LSORBIT | Both must be set to False (VASP defaults) |
 | LOCPROJ | LOCPROJ must be set to None (the VASP default). |
 | LOPTICS | LOPTICS must be set to False (the VASP default), unless explicitly specified by the relevant MP input set. |
 | LORBIT | LORBIT must **<u>*not*</u>** be None if the user also sets ISPIN=2, otherwise all values of LORBIT are acceptable. This is due to magnetization values not being output when ISPIN=2 and LORBIT = None are set together. |
-| LREAL | If the LREAL in the relevant MP input set is “Auto”, then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
+| LREAL | If the LREAL in the relevant MP input set is "Auto", then the user must be one of: "Auto", False. Otherwise, if the LREAL in the relevant MP input set is False, then the user must use False. |
 | LRPA | LRPA must be set to False (the VASP default). MP does not currently support random phase approximation (RPA) calculations. |
 | LSPECTRAL | LSPECTRAL must be set to False (the VASP default for most calculations). |
 | LSUBROT | LSUBROT must be set to False (the VASP default). |
 | MAGMOM | While any initial magnetic moments are allowed, the final total magnetic moment for any given atom must be less than 5 $\mu_B$ (Bohr magnetons) (except for elements Gd and Eu, which must be less than 10 $\mu_B$). This simply serves as a filter for erroneous data. |
 | ML_LMFF | ML_LMFF must be set to False (the VASP default). |
 | NGX / NGY / NGZ | The values for NGX/NGY/NGZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
 | NGFX / NGFY / NGFZ | The values for NGFX/NGFY/NGFZ must be at least 0.9 times the default value for the respective parameter generated by VASP. If the user simply does not specify these parameters, the calculation should be compatible with MP data. |
```

### Comparing `pymatgen_io_validation-0.0.3/pymatgen_io_validation.egg-info/SOURCES.txt` & `pymatgen_io_validation-0.0.4/pymatgen_io_validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.3/pyproject.toml` & `pymatgen_io_validation-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.3/setup.cfg` & `pymatgen_io_validation-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pymatgen_io_validation-0.0.3/setup.py` & `pymatgen_io_validation-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,37 @@
 
 from setuptools import setup, find_namespace_packages
 
 import os
 
 SETUP_PTH = os.path.dirname(os.path.abspath(__file__))
 
-with open(os.path.join(SETUP_PTH, "README.md")) as f:
+with open(os.path.join(SETUP_PTH, "README.md"), encoding="utf8") as f:
     desc = f.read()
 
 
 setup(
     name="pymatgen-io-validation",
     packages=find_namespace_packages(include=["pymatgen.io.*"]),
     version="0.0.3",
-    install_requires=["pymatgen>=2022.0.3", "emmet-core>=0.77.1", "pydantic>=2.4.2", "requests>=2.28.1"],
+    install_requires=[
+        "pymatgen>=2024.5.1",
+        "emmet-core>=0.83.6",
+        "pydantic>=2.4.2",
+        "requests>=2.28.1",
+    ],
     extras_require={},
     package_data={"pymatgen.io.validation": ["*.yaml"]},
     author="Matthew Kuner, Janosh Riebesell, Jason Munro, Aaron Kaplan",
     author_email="matthewkuner@berkeley.edu",
     maintainer="Matthew Kuner",
     url="https://github.com/materialsproject/pymatgen-io-validation",
     license="BSD",
     description="A comprehensive I/O validator for electronic structure calculations",
-    long_description=open("README.md").read(),
+    long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     keywords=["pymatgen"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Development Status :: 4 - Beta",
```

### Comparing `pymatgen_io_validation-0.0.3/tests/test_validation.py` & `pymatgen_io_validation-0.0.4/tests/test_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 @pytest.mark.parametrize(
     "object_name",
     [
         pytest.param("SiOptimizeDouble", id="SiOptimizeDouble"),
     ],
 )
 def test_potcar_validation(test_dir, object_name):
-
     task_doc = test_data_task_docs[object_name]
 
     correct_potcar_summary_stats = loadfn(test_dir / "vasp" / "Si_potcar_spec.json.gz")
 
     # Check POTCAR (this test should PASS, as we ARE using a MP-compatible pseudopotential)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.potcar_spec = correct_potcar_summary_stats
@@ -151,28 +150,34 @@
     # POTIM check #2 (checks energy change between steps)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.input.parameters["IBRION"] = 2
     temp_ionic_step_1 = copy.deepcopy(temp_task_doc.calcs_reversed[0].output.ionic_steps[0])
     temp_ionic_step_2 = copy.deepcopy(temp_ionic_step_1)
     temp_ionic_step_1.e_fr_energy = 0
     temp_ionic_step_2.e_fr_energy = 10000
-    temp_task_doc.calcs_reversed[0].output.ionic_steps = [temp_ionic_step_1, temp_ionic_step_2]
+    temp_task_doc.calcs_reversed[0].output.ionic_steps = [
+        temp_ionic_step_1,
+        temp_ionic_step_2,
+    ]
     run_check(temp_task_doc, "POTIM", False)
 
     # EDIFFG energy convergence check (this check should not raise any invalid reasons)
     temp_task_doc = copy.deepcopy(task_doc)
     run_check(temp_task_doc, "ENERGY CHANGE BETWEEN LAST TWO IONIC STEPS", True)
 
     # EDIFFG energy convergence check (this check SHOULD fail)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_ionic_step_1 = copy.deepcopy(temp_task_doc.calcs_reversed[0].output.ionic_steps[0])
     temp_ionic_step_2 = copy.deepcopy(temp_ionic_step_1)
     temp_ionic_step_1.e_0_energy = -1
     temp_ionic_step_2.e_0_energy = -2
-    temp_task_doc.calcs_reversed[0].output.ionic_steps = [temp_ionic_step_1, temp_ionic_step_2]
+    temp_task_doc.calcs_reversed[0].output.ionic_steps = [
+        temp_ionic_step_1,
+        temp_ionic_step_2,
+    ]
     run_check(temp_task_doc, "ENERGY CHANGE BETWEEN LAST TWO IONIC STEPS", False)
 
     # EDIFFG / force convergence check (the MP input set for R2SCAN has force convergence criteria)
     # (the below test should NOT fail, because final forces are 0)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.incar["METAGGA"] = "R2SCAN"
     temp_task_doc.output.forces = [[0, 0, 0], [0, 0, 0]]
@@ -274,15 +279,17 @@
     temp_task_doc.calcs_reversed[0].output.outcar["magnetization"] = []
     run_check(temp_task_doc, "LORBIT", False)
 
     # LMAXTAU check for METAGGA calcs (A value of 4 should fail for the `La` chemsys (has f electrons))
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.chemsys = "La"
     temp_task_doc.calcs_reversed[0].input.structure = Structure(
-        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]], species=["La", "La"], coords=[[0, 0, 0], [0.5, 0.5, 0.5]]
+        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]],
+        species=["La", "La"],
+        coords=[[0, 0, 0], [0.5, 0.5, 0.5]],
     )
     temp_task_doc.calcs_reversed[0].input.incar["LMAXTAU"] = 4
     temp_task_doc.calcs_reversed[0].input.incar["METAGGA"] = "R2SCAN"
     run_check(temp_task_doc, "LMAXTAU", False)
 
     # LMAXTAU check for METAGGA calcs (A value of 2 should fail for the `Si` chemsys)
     temp_task_doc = copy.deepcopy(task_doc)
@@ -402,28 +409,32 @@
     run_check(temp_task_doc, "MAGNETISM", False)
 
     # Excessive final magmom check (elements Gd or Eu present)
     # Should pass here, as it has a final magmom < 10
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.input.parameters["ISPIN"] = 2
     temp_task_doc.calcs_reversed[0].input.structure = Structure(
-        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]], species=["Gd", "Eu"], coords=[[0, 0, 0], [0.5, 0.5, 0.5]]
+        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]],
+        species=["Gd", "Eu"],
+        coords=[[0, 0, 0], [0.5, 0.5, 0.5]],
     )
     temp_task_doc.calcs_reversed[0].output.outcar["magnetization"] = (
         {"s": 9.0, "p": 0.0, "d": 0.0, "tot": 9.0},
         {"s": 9.0, "p": 0.0, "d": 0.0, "tot": 9.0},
     )
     run_check(temp_task_doc, "MAGNETISM", True)
 
     # Excessive final magmom check (elements Gd or Eu present)
     # Should not pass here, as it has a final magmom > 10
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.input.parameters["ISPIN"] = 2
     temp_task_doc.calcs_reversed[0].input.structure = Structure(
-        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]], species=["Gd", "Eu"], coords=[[0, 0, 0], [0.5, 0.5, 0.5]]
+        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]],
+        species=["Gd", "Eu"],
+        coords=[[0, 0, 0], [0.5, 0.5, 0.5]],
     )
     temp_task_doc.calcs_reversed[0].output.outcar["magnetization"] = (
         {"s": 11.0, "p": 0.0, "d": 0.0, "tot": 11.0},
         {"s": 11.0, "p": 0.0, "d": 0.0, "tot": 11.0},
     )
     run_check(temp_task_doc, "MAGNETISM", False)
 
@@ -458,33 +469,41 @@
 def test_kpoints_checks(object_name):
     task_doc = test_data_task_docs[object_name]
     task_doc.calcs_reversed[0].output.structure._charge = 0.0  # patch for old test files
 
     # Valid mesh type check (should flag HCP structures)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.structure = Structure(
-        lattice=[[0.5, -0.866025403784439, 0], [0.5, 0.866025403784439, 0], [0, 0, 1.6329931618554521]],
+        lattice=[
+            [0.5, -0.866025403784439, 0],
+            [0.5, 0.866025403784439, 0],
+            [0, 0, 1.6329931618554521],
+        ],
         coords=[[0, 0, 0], [0.333333333333333, -0.333333333333333, 0.5]],
         species=["H", "H"],
     )  # HCP structure
     _update_kpoints_for_test(temp_task_doc, {"generation_style": "monkhorst"})
     run_check(temp_task_doc, "INPUT SETTINGS --> KPOINTS or KGAMMA:", False)
 
     # Valid mesh type check (should flag FCC structures)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.structure = Structure(
-        lattice=[[0.0, 0.5, 0.5], [0.5, 0.0, 0.5], [0.5, 0.5, 0.0]], coords=[[0, 0, 0]], species=["H"]
+        lattice=[[0.0, 0.5, 0.5], [0.5, 0.0, 0.5], [0.5, 0.5, 0.0]],
+        coords=[[0, 0, 0]],
+        species=["H"],
     )  # FCC structure
     _update_kpoints_for_test(temp_task_doc, {"generation_style": "monkhorst"})
     run_check(temp_task_doc, "INPUT SETTINGS --> KPOINTS or KGAMMA:", False)
 
     # Valid mesh type check (should *not* flag BCC structures)
     temp_task_doc = copy.deepcopy(task_doc)
     temp_task_doc.calcs_reversed[0].input.structure = Structure(
-        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]], species=["H", "H"], coords=[[0, 0, 0], [0.5, 0.5, 0.5]]
+        lattice=[[2.9, 0, 0], [0, 2.9, 0], [0, 0, 2.9]],
+        species=["H", "H"],
+        coords=[[0, 0, 0], [0.5, 0.5, 0.5]],
     )  # BCC structure
     _update_kpoints_for_test(temp_task_doc, {"generation_style": "monkhorst"})
     run_check(temp_task_doc, "INPUT SETTINGS --> KPOINTS or KGAMMA:", True)
 
     # Too few kpoints check
     temp_task_doc = copy.deepcopy(task_doc)
     _update_kpoints_for_test(temp_task_doc, {"kpoints": [[3, 3, 3]]})
@@ -540,23 +559,24 @@
     temp_task_doc.calcs_reversed[0].vasp_version = "5.0.0"
     temp_task_doc.calcs_reversed[0].input.incar["METAGGA"] = "R2SCAN"
     temp_task_doc.input.parameters["ISPIN"] = 2
     run_check(temp_task_doc, "POTENTIAL BUG --> We believe", False)
 
 
 def test_task_document(test_dir):
-
     from emmet.core.vasp.task_valid import TaskDocument
 
     calcs = {}
     calcs["compliant"] = loadfn(
-        str(test_dir / "vasp" / "TaskDocuments" / "MP_compatible_GaAs_r2SCAN_static_TaskDocument.json.gz"), cls=None
+        str(test_dir / "vasp" / "TaskDocuments" / "MP_compatible_GaAs_r2SCAN_static_TaskDocument.json.gz"),
+        cls=None,
     )
     calcs["non-compliant"] = loadfn(
-        str(test_dir / "vasp" / "TaskDocuments" / "MP_incompatible_GaAs_r2SCAN_static_TaskDocument.json.gz"), cls=None
+        str(test_dir / "vasp" / "TaskDocuments" / "MP_incompatible_GaAs_r2SCAN_static_TaskDocument.json.gz"),
+        cls=None,
     )
 
     valid_docs = {}
     for calc in calcs:
         valid_docs[calc] = ValidationDoc.from_task_doc(TaskDocument(**calcs[calc]))
         # quickly check that `from_dict` and `from_task_doc` give same document
         assert set(ValidationDoc.from_dict(calcs[calc]).reasons) == set(valid_docs[calc].reasons)
```

