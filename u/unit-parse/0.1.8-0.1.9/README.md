# Comparing `tmp/unit_parse-0.1.8.tar.gz` & `tmp/unit_parse-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_parse-0.1.8.tar", last modified: Wed Jun 28 12:38:32 2023, max compression
+gzip compressed data, was "unit_parse-0.1.9.tar", last modified: Tue May 14 17:49:56 2024, max compression
```

## Comparing `unit_parse-0.1.8.tar` & `unit_parse-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 12:38:32.317249 unit_parse-0.1.8/
--rw-rw-rw-   0        0        0     1564 2022-01-21 14:16:08.000000 unit_parse-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      163 2022-01-24 16:14:12.000000 unit_parse-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    15781 2023-06-28 12:38:32.318247 unit_parse-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    15239 2023-06-28 12:37:07.000000 unit_parse-0.1.8/README.md
--rw-rw-rw-   0        0        0      909 2022-01-28 18:08:18.000000 unit_parse-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      882 2023-06-28 12:38:32.330249 unit_parse-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0       75 2022-01-21 14:08:54.000000 unit_parse-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:38:32.148247 unit_parse-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 12:38:32.206256 unit_parse-0.1.8/src/unit_parse/
--rw-rw-rw-   0        0        0      298 2022-01-28 02:11:29.000000 unit_parse-0.1.8/src/unit_parse/__init__.py
--rw-rw-rw-   0        0        0     6061 2022-01-30 20:54:17.000000 unit_parse-0.1.8/src/unit_parse/classification.py
--rw-rw-rw-   0        0        0     4615 2023-06-28 12:37:07.000000 unit_parse-0.1.8/src/unit_parse/config.py
--rw-rw-rw-   0        0        0    13298 2022-01-29 16:47:51.000000 unit_parse-0.1.8/src/unit_parse/core.py
--rw-rw-rw-   0        0        0     2849 2022-01-23 00:40:48.000000 unit_parse-0.1.8/src/unit_parse/logger.py
--rw-rw-rw-   0        0        0     1604 2022-01-30 18:31:33.000000 unit_parse-0.1.8/src/unit_parse/main.py
--rw-rw-rw-   0        0        0     4295 2022-01-28 16:58:31.000000 unit_parse-0.1.8/src/unit_parse/pre_processing_multiple.py
--rw-rw-rw-   0        0        0     6943 2023-06-28 12:37:07.000000 unit_parse-0.1.8/src/unit_parse/pre_processing_substitution.py
--rw-rw-rw-   0        0        0     7314 2022-01-30 20:05:18.000000 unit_parse-0.1.8/src/unit_parse/reduce_quantities.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:38:32.270248 unit_parse-0.1.8/src/unit_parse/support_files/
--rw-rw-rw-   0        0        0     4423 2021-08-21 14:49:38.000000 unit_parse-0.1.8/src/unit_parse/support_files/constants_en.txt
--rw-rw-rw-   0        0        0    23746 2022-01-27 22:54:21.000000 unit_parse-0.1.8/src/unit_parse/support_files/default_en.txt
--rw-rw-rw-   0        0        0  4226694 2022-01-24 15:40:56.000000 unit_parse-0.1.8/src/unit_parse/support_files/dictionary.txt
--rw-rw-rw-   0        0        0     5227 2022-01-30 22:09:28.000000 unit_parse-0.1.8/src/unit_parse/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 12:38:32.245249 unit_parse-0.1.8/src/unit_parse.egg-info/
--rw-rw-rw-   0        0        0    15781 2023-06-28 12:38:32.000000 unit_parse-0.1.8/src/unit_parse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      993 2023-06-28 12:38:32.000000 unit_parse-0.1.8/src/unit_parse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 12:38:32.000000 unit_parse-0.1.8/src/unit_parse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-01-21 14:17:37.000000 unit_parse-0.1.8/src/unit_parse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       74 2023-06-28 12:38:32.000000 unit_parse-0.1.8/src/unit_parse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-28 12:38:32.000000 unit_parse-0.1.8/src/unit_parse.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-28 12:38:32.315251 unit_parse-0.1.8/tests/
--rw-rw-rw-   0        0        0     3398 2022-01-30 21:20:07.000000 unit_parse-0.1.8/tests/test_classification.py
--rw-rw-rw-   0        0        0      621 2022-01-28 14:41:32.000000 unit_parse-0.1.8/tests/test_config.py
--rw-rw-rw-   0        0        0     5886 2022-01-28 17:19:43.000000 unit_parse-0.1.8/tests/test_core.py
--rw-rw-rw-   0        0        0     5875 2022-01-30 20:17:29.000000 unit_parse-0.1.8/tests/test_main.py
--rw-rw-rw-   0        0        0      200 2022-01-28 17:37:44.000000 unit_parse-0.1.8/tests/test_pint.py
--rw-rw-rw-   0        0        0      202 2022-01-28 02:06:45.000000 unit_parse-0.1.8/tests/test_pint_error.py
--rw-rw-rw-   0        0        0     2957 2022-01-28 14:55:51.000000 unit_parse-0.1.8/tests/test_pre_processing_multiple.py
--rw-rw-rw-   0        0        0     7083 2023-06-28 12:37:07.000000 unit_parse-0.1.8/tests/test_pre_processing_substitution.py
--rw-rw-rw-   0        0        0     4699 2022-01-30 20:08:52.000000 unit_parse-0.1.8/tests/test_reduce_quantity.py
--rw-rw-rw-   0        0        0     3815 2022-01-30 20:32:56.000000 unit_parse-0.1.8/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:49:56.927268 unit_parse-0.1.9/
+-rw-rw-rw-   0        0        0     1564 2022-03-26 22:11:05.000000 unit_parse-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      163 2022-03-26 22:11:05.000000 unit_parse-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    16004 2024-05-14 17:49:56.927268 unit_parse-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15239 2022-08-25 22:04:02.000000 unit_parse-0.1.9/README.md
+-rw-rw-rw-   0        0        0      909 2024-05-14 17:20:37.000000 unit_parse-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      882 2024-05-14 17:49:56.932276 unit_parse-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0       75 2022-03-26 22:11:05.000000 unit_parse-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:49:56.850396 unit_parse-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-14 17:49:56.878292 unit_parse-0.1.9/src/unit_parse/
+-rw-rw-rw-   0        0        0      298 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/__init__.py
+-rw-rw-rw-   0        0        0     6061 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/classification.py
+-rw-rw-rw-   0        0        0     4615 2022-08-25 23:02:31.000000 unit_parse-0.1.9/src/unit_parse/config.py
+-rw-rw-rw-   0        0        0    13349 2024-05-14 17:44:30.000000 unit_parse-0.1.9/src/unit_parse/core.py
+-rw-rw-rw-   0        0        0     2849 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/logger.py
+-rw-rw-rw-   0        0        0     1604 2022-08-25 23:02:31.000000 unit_parse-0.1.9/src/unit_parse/main.py
+-rw-rw-rw-   0        0        0     4295 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/pre_processing_multiple.py
+-rw-rw-rw-   0        0        0     6995 2024-05-14 17:44:30.000000 unit_parse-0.1.9/src/unit_parse/pre_processing_substitution.py
+-rw-rw-rw-   0        0        0        0 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/py.typed
+-rw-rw-rw-   0        0        0     7314 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/reduce_quantities.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:49:56.909061 unit_parse-0.1.9/src/unit_parse/support_files/
+-rw-rw-rw-   0        0        0     4497 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/support_files/constants_en.txt
+-rw-rw-rw-   0        0        0    24486 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/support_files/default_en.txt
+-rw-rw-rw-   0        0        0  4226694 2022-03-26 22:11:05.000000 unit_parse-0.1.9/src/unit_parse/support_files/dictionary.txt
+-rw-rw-rw-   0        0        0     5227 2022-08-25 23:02:31.000000 unit_parse-0.1.9/src/unit_parse/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 17:49:56.925262 unit_parse-0.1.9/src/unit_parse.egg-info/
+-rw-rw-rw-   0        0        0    16004 2024-05-14 17:49:56.000000 unit_parse-0.1.9/src/unit_parse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-05-14 17:49:56.000000 unit_parse-0.1.9/src/unit_parse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 17:49:56.000000 unit_parse-0.1.9/src/unit_parse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-03-27 17:19:56.000000 unit_parse-0.1.9/src/unit_parse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       74 2024-05-14 17:49:56.000000 unit_parse-0.1.9/src/unit_parse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-14 17:49:56.000000 unit_parse-0.1.9/src/unit_parse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 17:49:56.924255 unit_parse-0.1.9/tests/
+-rw-rw-rw-   0        0        0     3398 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_classification.py
+-rw-rw-rw-   0        0        0      621 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_config.py
+-rw-rw-rw-   0        0        0     5886 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_core.py
+-rw-rw-rw-   0        0        0     6013 2024-05-14 17:44:30.000000 unit_parse-0.1.9/tests/test_main.py
+-rw-rw-rw-   0        0        0      200 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_pint.py
+-rw-rw-rw-   0        0        0      202 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_pint_error.py
+-rw-rw-rw-   0        0        0     2957 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_pre_processing_multiple.py
+-rw-rw-rw-   0        0        0     7126 2024-05-14 17:44:30.000000 unit_parse-0.1.9/tests/test_pre_processing_substitution.py
+-rw-rw-rw-   0        0        0     4699 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_reduce_quantity.py
+-rw-rw-rw-   0        0        0     3815 2022-03-26 22:11:05.000000 unit_parse-0.1.9/tests/test_utils.py
```

### Comparing `unit_parse-0.1.8/LICENSE.txt` & `unit_parse-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/PKG-INFO` & `unit_parse-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: unit_parse
-Version: 0.1.8
-Summary: Parse units from strings. From mess to order!
-Home-page: https://github.com/dylanwal/unit_parse
-Author: Dylan Walsh
-License: BSD
-Platform: any
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 # Unit Parse (unit_parse)
 
 ---
 ---
 ![PyPI](https://img.shields.io/pypi/v/unit_parse)
 ![tests](https://raw.githubusercontent.com/dylanwal/unit_parse/master/tests/badges/tests-badge.svg)
 ![coverage](https://raw.githubusercontent.com/dylanwal/unit_parse/master/tests/badges/coverage-badge.svg)
```

### Comparing `unit_parse-0.1.8/README.md` & `unit_parse-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: unit_parse
+Version: 0.1.9
+Summary: Parse units from strings. From mess to order!
+Home-page: https://github.com/dylanwal/unit_parse
+Author: Dylan Walsh
+License: BSD
+Platform: any
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: pint==0.19
+Provides-Extra: testing
+Requires-Dist: pytest>=6.0; extra == "testing"
+Requires-Dist: pytest-cov>=2.0; extra == "testing"
+Requires-Dist: mypy>=0.910; extra == "testing"
+Requires-Dist: flake8>=3.9; extra == "testing"
+
 # Unit Parse (unit_parse)
 
 ---
 ---
 ![PyPI](https://img.shields.io/pypi/v/unit_parse)
 ![tests](https://raw.githubusercontent.com/dylanwal/unit_parse/master/tests/badges/tests-badge.svg)
 ![coverage](https://raw.githubusercontent.com/dylanwal/unit_parse/master/tests/badges/coverage-badge.svg)
```

### Comparing `unit_parse-0.1.8/pyproject.toml` & `unit_parse-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/setup.cfg` & `unit_parse-0.1.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 745f 7061 7273 650d 0a76   = unit_parse..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e38 0d0a  ersion = 0.1.8..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e39 0d0a  ersion = 0.1.9..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 5061  description = Pa
 00000040: 7273 6520 756e 6974 7320 6672 6f6d 2073  rse units from s
 00000050: 7472 696e 6773 2e20 4672 6f6d 206d 6573  trings. From mes
 00000060: 7320 746f 206f 7264 6572 210d 0a6c 6f6e  s to order!..lon
 00000070: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
 00000080: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
 00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
```

### Comparing `unit_parse-0.1.8/src/unit_parse/classification.py` & `unit_parse-0.1.9/src/unit_parse/classification.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse/config.py` & `unit_parse-0.1.9/src/unit_parse/config.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse/core.py` & `unit_parse-0.1.9/src/unit_parse/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,18 +98,19 @@
     out: float, Unit, Quantity, None
 
     """
     try:
         return float(text)
     except Exception:
         pass
-    try:
-        return Unit(text)
-    except Exception:
-        pass
+    if not contains_number(text):
+        try:
+            return Unit(text)
+        except Exception:
+            pass
     try:
         return Quantity(text)
     except Exception:
         pass
 
     return get_quantity(text)
```

### Comparing `unit_parse-0.1.8/src/unit_parse/logger.py` & `unit_parse-0.1.9/src/unit_parse/logger.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse/main.py` & `unit_parse-0.1.9/src/unit_parse/main.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse/pre_processing_multiple.py` & `unit_parse-0.1.9/src/unit_parse/pre_processing_multiple.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse/pre_processing_substitution.py` & `unit_parse-0.1.9/src/unit_parse/pre_processing_substitution.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,20 @@
             exp_new = exp.replace("-", "**-", 1)
         else:
             exp_new = exp.replace("+", "**", 1)
         text_in = text_in.replace(exp, exp_new)
 
     found_sci_notation = re.findall("[0-9]e[-+]?[0-9]{1,5}", text_in)
     for exp in found_sci_notation:
-        exp_new = exp.replace("e", "*10**", 1)
+        exp_new = exp.replace("e+", "*10**", 1).replace("e", "*10**", 1)
         text_in = text_in.replace(exp, exp_new)
 
     found_sci_notation = re.findall("[0-9]E[-+]?[0-9]{1,5}", text_in)
     for exp in found_sci_notation:
-        exp_new = exp.replace("E", "*10**", 1)
+        exp_new = exp.replace("E+", "*10**", 1).replace("E", "*10**", 1)
         text_in = text_in.replace(exp, exp_new)
 
     found_sci_notation = re.findall("[0-9][*]10[0-9]{1,5}", text_in)
     for exp in found_sci_notation:
         exp_new = exp.replace("10", "10**", 1)
         text_in = text_in.replace(exp, exp_new)
```

### Comparing `unit_parse-0.1.8/src/unit_parse/reduce_quantities.py` & `unit_parse-0.1.9/src/unit_parse/reduce_quantities.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse/support_files/constants_en.txt` & `unit_parse-0.1.9/src/unit_parse/support_files/constants_en.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# Default Pint constants definition file
-# Based on the International System of Units
-# Language: english
-# Source: https://physics.nist.gov/cuu/Constants/
-#         https://physics.nist.gov/PhysRefData/XrayTrans/Html/search.html
-# :copyright: 2013,2019 by Pint Authors, see AUTHORS for more details.
-
-#### MATHEMATICAL CONSTANTS ####
-# As computed by Maxima with fpprec:50
-
-pi     = 3.1415926535897932384626433832795028841971693993751 = π  # pi
-tansec = 4.8481368111333441675396429478852851658848753880815e-6   # tangent of 1 arc-second ~ arc_second/radian
-ln10   = 2.3025850929940456840179914546843642076011014886288      # natural logarithm of 10
-wien_x = 4.9651142317442763036987591313228939440555849867973      # solution to (x-5)*exp(x)+5 = 0 => x = W(5/exp(5))+5
-wien_u = 2.8214393721220788934031913302944851953458817440731      # solution to (u-3)*exp(u)+3 = 0 => u = W(3/exp(3))+3
-eulers_number = 2.71828182845904523536028747135266249775724709369995
-
-#### DEFINED EXACT CONSTANTS ####
-
-speed_of_light = 299792458 m/s = c = c_0                      # since 1983
-planck_constant = 6.62607015e-34 J s = h                      # since May 2019
-elementary_charge = 1.602176634e-19 C = e                     # since May 2019
-avogadro_number = 6.02214076e23                               # since May 2019
-boltzmann_constant = 1.380649e-23 J K^-1 = k = k_B            # since May 2019
-standard_gravity = 9.80665 m/s^2 = g_0 = g0 = g_n = gravity   # since 1901
-standard_atmosphere = 1.01325e5 Pa = atm = atmosphere         # since 1954
-conventional_josephson_constant = 4.835979e14 Hz / V = K_J90  # since Jan 1990
-conventional_von_klitzing_constant = 2.5812807e4 ohm = R_K90  # since Jan 1990
-
-#### DERIVED EXACT CONSTANTS ####
-# Floating-point conversion may introduce inaccuracies
-
-zeta = c / (cm/s) = ζ
-dirac_constant = h / (2 * π) = ħ = hbar = atomic_unit_of_action = a_u_action
-avogadro_constant = avogadro_number * mol^-1 = N_A
-molar_gas_constant = k * N_A = R
-faraday_constant = e * N_A
-conductance_quantum = 2 * e ** 2 / h = G_0
-magnetic_flux_quantum = h / (2 * e) = Φ_0 = Phi_0
-josephson_constant = 2 * e / h = K_J
-von_klitzing_constant = h / e ** 2 = R_K
-stefan_boltzmann_constant = 2 / 15 * π ** 5 * k ** 4 / (h ** 3 * c ** 2) = σ = sigma
-first_radiation_constant = 2 * π * h * c ** 2 = c_1
-second_radiation_constant = h * c / k = c_2
-wien_wavelength_displacement_law_constant = h * c / (k * wien_x)
-wien_frequency_displacement_law_constant = wien_u * k / h
-
-#### MEASURED CONSTANTS ####
-# Recommended CODATA-2018 values
-# To some extent, what is measured and what is derived is a bit arbitrary.
-# The choice of measured constants is based on convenience and on available uncertainty.
-# The uncertainty in the last significant digits is given in parentheses as a comment.
-
-newtonian_constant_of_gravitation = 6.67430e-11 m^3/(kg s^2) = _ = gravitational_constant  # (15)
-rydberg_constant = 1.0973731568160e7 * m^-1 = R_∞ = R_inf                                  # (21)
-electron_g_factor = -2.00231930436256 = g_e                                                # (35)
-atomic_mass_constant = 1.66053906660e-27 kg = m_u                                          # (50)
-electron_mass = 9.1093837015e-31 kg = m_e = atomic_unit_of_mass = a_u_mass                 # (28)
-proton_mass = 1.67262192369e-27 kg = m_p                                                   # (51)
-neutron_mass = 1.67492749804e-27 kg = m_n                                                  # (95)
-lattice_spacing_of_Si = 1.920155716e-10 m = d_220                                          # (32)
-K_alpha_Cu_d_220 = 0.80232719                                                              # (22)
-K_alpha_Mo_d_220 = 0.36940604                                                              # (19)
-K_alpha_W_d_220 = 0.108852175                                                              # (98)
-
-#### DERIVED CONSTANTS ####
-
-fine_structure_constant = (2 * h * R_inf / (m_e * c)) ** 0.5 = α = alpha
-vacuum_permeability = 2 * α * h / (e ** 2 * c) = µ_0 = mu_0 = mu0 = magnetic_constant
-vacuum_permittivity = e ** 2 / (2 * α * h * c) = ε_0 = epsilon_0 = eps_0 = eps0 = electric_constant
-impedance_of_free_space = 2 * α * h / e ** 2 = Z_0 = characteristic_impedance_of_vacuum
-coulomb_constant = α * hbar * c / e ** 2 = k_C
-classical_electron_radius = α * hbar / (m_e * c) = r_e
-thomson_cross_section = 8 / 3 * π * r_e ** 2 = σ_e = sigma_e
+# Default Pint constants definition file
+# Based on the International System of Units
+# Language: english
+# Source: https://physics.nist.gov/cuu/Constants/
+#         https://physics.nist.gov/PhysRefData/XrayTrans/Html/search.html
+# :copyright: 2013,2019 by Pint Authors, see AUTHORS for more details.
+
+#### MATHEMATICAL CONSTANTS ####
+# As computed by Maxima with fpprec:50
+
+pi     = 3.1415926535897932384626433832795028841971693993751 = π  # pi
+tansec = 4.8481368111333441675396429478852851658848753880815e-6   # tangent of 1 arc-second ~ arc_second/radian
+ln10   = 2.3025850929940456840179914546843642076011014886288      # natural logarithm of 10
+wien_x = 4.9651142317442763036987591313228939440555849867973      # solution to (x-5)*exp(x)+5 = 0 => x = W(5/exp(5))+5
+wien_u = 2.8214393721220788934031913302944851953458817440731      # solution to (u-3)*exp(u)+3 = 0 => u = W(3/exp(3))+3
+eulers_number = 2.71828182845904523536028747135266249775724709369995
+
+#### DEFINED EXACT CONSTANTS ####
+
+speed_of_light = 299792458 m/s = c = c_0                      # since 1983
+planck_constant = 6.62607015e-34 J s = h                      # since May 2019
+elementary_charge = 1.602176634e-19 C = e                     # since May 2019
+avogadro_number = 6.02214076e23                               # since May 2019
+boltzmann_constant = 1.380649e-23 J K^-1 = k = k_B            # since May 2019
+standard_gravity = 9.80665 m/s^2 = g_0 = g0 = g_n = gravity   # since 1901
+standard_atmosphere = 1.01325e5 Pa = atm = atmosphere         # since 1954
+conventional_josephson_constant = 4.835979e14 Hz / V = K_J90  # since Jan 1990
+conventional_von_klitzing_constant = 2.5812807e4 ohm = R_K90  # since Jan 1990
+
+#### DERIVED EXACT CONSTANTS ####
+# Floating-point conversion may introduce inaccuracies
+
+zeta = c / (cm/s) = ζ
+dirac_constant = h / (2 * π) = ħ = hbar = atomic_unit_of_action = a_u_action
+avogadro_constant = avogadro_number * mol^-1 = N_A
+molar_gas_constant = k * N_A = R
+faraday_constant = e * N_A
+conductance_quantum = 2 * e ** 2 / h = G_0
+magnetic_flux_quantum = h / (2 * e) = Φ_0 = Phi_0
+josephson_constant = 2 * e / h = K_J
+von_klitzing_constant = h / e ** 2 = R_K
+stefan_boltzmann_constant = 2 / 15 * π ** 5 * k ** 4 / (h ** 3 * c ** 2) = σ = sigma
+first_radiation_constant = 2 * π * h * c ** 2 = c_1
+second_radiation_constant = h * c / k = c_2
+wien_wavelength_displacement_law_constant = h * c / (k * wien_x)
+wien_frequency_displacement_law_constant = wien_u * k / h
+
+#### MEASURED CONSTANTS ####
+# Recommended CODATA-2018 values
+# To some extent, what is measured and what is derived is a bit arbitrary.
+# The choice of measured constants is based on convenience and on available uncertainty.
+# The uncertainty in the last significant digits is given in parentheses as a comment.
+
+newtonian_constant_of_gravitation = 6.67430e-11 m^3/(kg s^2) = _ = gravitational_constant  # (15)
+rydberg_constant = 1.0973731568160e7 * m^-1 = R_∞ = R_inf                                  # (21)
+electron_g_factor = -2.00231930436256 = g_e                                                # (35)
+atomic_mass_constant = 1.66053906660e-27 kg = m_u                                          # (50)
+electron_mass = 9.1093837015e-31 kg = m_e = atomic_unit_of_mass = a_u_mass                 # (28)
+proton_mass = 1.67262192369e-27 kg = m_p                                                   # (51)
+neutron_mass = 1.67492749804e-27 kg = m_n                                                  # (95)
+lattice_spacing_of_Si = 1.920155716e-10 m = d_220                                          # (32)
+K_alpha_Cu_d_220 = 0.80232719                                                              # (22)
+K_alpha_Mo_d_220 = 0.36940604                                                              # (19)
+K_alpha_W_d_220 = 0.108852175                                                              # (98)
+
+#### DERIVED CONSTANTS ####
+
+fine_structure_constant = (2 * h * R_inf / (m_e * c)) ** 0.5 = α = alpha
+vacuum_permeability = 2 * α * h / (e ** 2 * c) = µ_0 = mu_0 = mu0 = magnetic_constant
+vacuum_permittivity = e ** 2 / (2 * α * h * c) = ε_0 = epsilon_0 = eps_0 = eps0 = electric_constant
+impedance_of_free_space = 2 * α * h / e ** 2 = Z_0 = characteristic_impedance_of_vacuum
+coulomb_constant = α * hbar * c / e ** 2 = k_C
+classical_electron_radius = α * hbar / (m_e * c) = r_e
+thomson_cross_section = 8 / 3 * π * r_e ** 2 = σ_e = sigma_e
```

### Comparing `unit_parse-0.1.8/src/unit_parse/support_files/default_en.txt` & `unit_parse-0.1.9/src/unit_parse/support_files/default_en.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,740 +1,740 @@
-# Default Pint units definition file
-# Based on the International System of Units
-# Language: english
-# :copyright: 2013,2019 by Pint Authors, see AUTHORS for more details.
-
-# Syntax
-# ======
-# Units
-# -----
-# <canonical name> = <relation to another unit or dimension> [= <symbol>] [= <alias>] [ = <alias> ] [...]
-#
-# The canonical name and aliases should be expressed in singular form.
-# Pint automatically deals with plurals built by adding 's' to the singular form; plural
-# forms that don't follow this rule should be instead explicitly listed as aliases.
-#
-# If a unit has no symbol and one wants to define aliases, then the symbol should be
-# conventionally set to _.
-#
-# Example:
-#     millennium = 1e3 * year = _ = millennia
-#
-#
-# Prefixes
-# --------
-# <prefix>- = <amount> [= <symbol>] [= <alias>] [ = <alias> ] [...]
-#
-# Example:
-#     deca- =  1e+1  = da- = deka-
-#
-#
-# Derived dimensions
-# ------------------
-# [dimension name] = <relation to other dimensions>
-#
-# Example:
-#     [density] = [mass] / [volume]
-#
-# Note that primary dimensions don't need to be declared; they can be
-# defined for the first time in a unit definition.
-# E.g. see below `meter = [length]`
-#
-#
-# Additional aliases
-# ------------------
-# @alias <canonical name or previous alias> = <alias> [ = <alias> ] [...]
-#
-# Used to add aliases to already existing unit definitions.
-# Particularly useful when one wants to enrich definitions
-# from defaults_en.txt with custom aliases.
-#
-# Example:
-#     @alias meter = my_meter
-
-# See also: https://pint.readthedocs.io/en/latest/defining.html
-
-@defaults
-    group = international
-    system = mks
-@end
-
-
-#### PREFIXES ####
-
-# decimal prefixes
-yocto- = 1e-24 = y-
-zepto- = 1e-21 = z-
-atto- =  1e-18 = a-
-femto- = 1e-15 = f-
-pico- =  1e-12 = p-
-nano- =  1e-9  = n-
-micro- = 1e-6  = µ- = u-
-milli- = 1e-3  = m-
-centi- = 1e-2  = c-
-deci- =  1e-1  = d-
-deca- =  1e+1  = da- = deka-
-hecto- = 1e2   = h-
-kilo- =  1e3   = k-
-mega- =  1e6   = M-
-giga- =  1e9   = G-
-tera- =  1e12  = T-
-peta- =  1e15  = P-
-exa- =   1e18  = E-
-zetta- = 1e21  = Z-
-yotta- = 1e24  = Y-
-
-# binary_prefixes
-kibi- = 2**10 = Ki-
-mebi- = 2**20 = Mi-
-gibi- = 2**30 = Gi-
-tebi- = 2**40 = Ti-
-pebi- = 2**50 = Pi-
-exbi- = 2**60 = Ei-
-zebi- = 2**70 = Zi-
-yobi- = 2**80 = Yi-
-
-# extra_prefixes
-semi- = 0.5 = _ = demi-
-sesqui- = 1.5
-
-
-#### BASE UNITS ####
-
-meter = [length] = m = metre
-second = [time] = s = sec
-ampere = [current] = A = amp
-candela = [luminosity] = cd = candle
-gram = [mass] = g
-mole = [substance] = mol
-kelvin = [temperature]; offset: 0 = K = degK = °K = degree_Kelvin = degreeK  # older names supported for compatibility
-radian = [] = rad
-bit = []
-count = []
-
-
-#### CONSTANTS ####
-
-@import constants_en.txt
-
-
-#### UNITS ####
-# Common and less common, grouped by quantity.
-# Conversion factors are exact (except when noted),
-# although floating-point conversion may introduce inaccuracies
-
-# Angle
-turn = 2 * π * radian = _ = revolution = cycle = circle
-degree = π / 180 * radian = deg = arcdeg = arcdegree = angular_degree
-arcminute = degree / 60 = arcmin = arc_minute = angular_minute
-arcsecond = arcminute / 60 = arcsec = arc_second = angular_second
-milliarcsecond = 1e-3 * arcsecond = mas
-grade = π / 200 * radian = grad = gon
-mil = π / 32000 * radian
-
-# Solid angle
-steradian = radian ** 2 = sr
-square_degree = (π / 180) ** 2 * sr = sq_deg = sqdeg
-
-# Information
-baud = bit / second = Bd = bps
-
-byte = 8 * bit = B = octet
-# byte = 8 * bit = _ = octet
-## NOTE: B (byte) symbol can conflict with Bell
-
-# Length
-angstrom = 1e-10 * meter = Å = ångström = Å
-micron = micrometer = µ
-fermi = femtometer = fm
-light_year = speed_of_light * julian_year = ly = lightyear
-astronomical_unit = 149597870700 * meter = au  # since Aug 2012
-parsec = 1 / tansec * astronomical_unit = pc
-nautical_mile = 1852 * meter = nmi
-bohr = hbar / (alpha * m_e * c) = a_0 = a0 = bohr_radius = atomic_unit_of_length = a_u_length
-x_unit_Cu = K_alpha_Cu_d_220 * d_220 / 1537.4 = Xu_Cu
-x_unit_Mo = K_alpha_Mo_d_220 * d_220 / 707.831 = Xu_Mo
-angstrom_star = K_alpha_W_d_220 * d_220 / 0.2090100 = Å_star
-planck_length = (hbar * gravitational_constant / c ** 3) ** 0.5
-
-# Mass
-metric_ton = 1e3 * kilogram = t = tonne
-unified_atomic_mass_unit = atomic_mass_constant = u = amu
-dalton = atomic_mass_constant = Da
-grain = 64.79891 * milligram = gr
-gamma_mass = microgram
-carat = 200 * milligram = ct = karat
-planck_mass = (hbar * c / gravitational_constant) ** 0.5
-
-# Time
-minute = 60 * second = min
-hour = 60 * minute = hr
-day = 24 * hour = d
-week = 7 * day
-fortnight = 2 * week
-year = 365.25 * day = yr = julian_year
-month = year / 12
-
-# decade = 10 * year
-## NOTE: decade [time] can conflict with decade [dimensionless]
-
-century = 100 * year = _ = centuries
-millennium = 1e3 * year = _ = millennia
-eon = 1e9 * year
-shake = 1e-8 * second
-svedberg = 1e-13 * second
-atomic_unit_of_time = hbar / E_h = a_u_time
-gregorian_year = 365.2425 * day
-sidereal_year = 365.256363004 * day                # approximate, as of J2000 epoch
-tropical_year = 365.242190402 * day                # approximate, as of J2000 epoch
-common_year = 365 * day
-leap_year = 366 * day
-sidereal_day = day / 1.00273790935079524           # approximate
-sidereal_month = 27.32166155 * day                 # approximate
-tropical_month = 27.321582 * day                   # approximate
-synodic_month = 29.530589 * day = _ = lunar_month  # approximate
-planck_time = (hbar * gravitational_constant / c ** 5) ** 0.5
-
-# Temperature
-degree_Celsius = kelvin; offset: 273.15 = °C = celsius = degC = degreeC
-degree_Rankine = 5 / 9 * kelvin; offset: 0 = °R = rankine = degR = degreeR
-degree_Fahrenheit = 5 / 9 * kelvin; offset: 233.15 + 200 / 9 = °F = fahrenheit = degF = degreeF
-degree_Reaumur = 4 / 5 * kelvin; offset: 273.15 = °Re = reaumur = degRe = degreeRe = degree_Réaumur = réaumur
-atomic_unit_of_temperature = E_h / k = a_u_temp
-planck_temperature = (hbar * c ** 5 / gravitational_constant / k ** 2) ** 0.5
-
-# Area
-[area] = [length] ** 2
-are = 100 * meter ** 2
-barn = 1e-28 * meter ** 2 = b
-darcy = centipoise * centimeter ** 2 / (second * atmosphere)
-hectare = 100 * are = ha
-
-# Volume
-[volume] = [length] ** 3
-liter = decimeter ** 3 = l = L = litre
-cubic_centimeter = centimeter ** 3 = cc
-lambda = microliter = λ
-stere = meter ** 3
-
-# Frequency
-[frequency] = 1 / [time]
-hertz = 1 / second = Hz
-revolutions_per_minute = revolution / minute = rpm
-revolutions_per_second = revolution / second = rps
-counts_per_second = count / second = cps
-
-# Wavenumber
-[wavenumber] = 1 / [length]
-reciprocal_centimeter = 1 / cm = cm_1 = kayser
-
-# Velocity
-[velocity] = [length] / [time] = [speed]
-knot = nautical_mile / hour = kt = knot_international = international_knot
-mile_per_hour = mile / hour = mph = MPH
-kilometer_per_hour = kilometer / hour = kph = KPH
-kilometer_per_second = kilometer / second = kps
-meter_per_second = meter / second = mps
-foot_per_second = foot / second = fps
-
-# Acceleration
-[acceleration] = [velocity] / [time]
-galileo = centimeter / second ** 2 = Gal
-
-# Force
-[force] = [mass] * [acceleration]
-newton = kilogram * meter / second ** 2 = N
-dyne = gram * centimeter / second ** 2 = dyn
-force_kilogram = g_0 * kilogram = kgf = kilogram_force = pond
-force_gram = g_0 * gram = gf = gram_force
-force_metric_ton = g_0 * metric_ton = tf = metric_ton_force = force_t = t_force
-atomic_unit_of_force = E_h / a_0 = a_u_force
-
-# Energy
-[energy] = [force] * [length]
-joule = newton * meter = J
-erg = dyne * centimeter
-watt_hour = watt * hour = Wh = watthour
-electron_volt = e * volt = eV
-rydberg = h * c * R_inf = Ry
-hartree = 2 * rydberg = E_h = Eh = hartree_energy = atomic_unit_of_energy = a_u_energy
-calorie = 4.184 * joule = cal = thermochemical_calorie = cal_th
-international_calorie = 4.1868 * joule = cal_it = international_steam_table_calorie
-fifteen_degree_calorie = 4.1855 * joule = cal_15
-british_thermal_unit = 1055.056 * joule = Btu = BTU = Btu_iso
-international_british_thermal_unit = 1e3 * pound / kilogram * degR / kelvin * international_calorie = Btu_it
-thermochemical_british_thermal_unit = 1e3 * pound / kilogram * degR / kelvin * calorie = Btu_th
-quadrillion_Btu = 1e15 * Btu = quad
-therm = 1e5 * Btu = thm = EC_therm
-US_therm = 1.054804e8 * joule  # approximate, no exact definition
-ton_TNT = 1e9 * calorie = tTNT
-tonne_of_oil_equivalent = 1e10 * international_calorie = toe
-atmosphere_liter = atmosphere * liter = atm_l
-
-# Power
-[power] = [energy] / [time]
-watt = joule / second = W
-volt_ampere = volt * ampere = VA
-horsepower = 550 * foot * force_pound / second = hp = UK_horsepower = hydraulic_horsepower
-boiler_horsepower = 33475 * Btu / hour                            # unclear which Btu
-metric_horsepower = 75 * force_kilogram * meter / second
-electrical_horsepower = 746 * watt
-refrigeration_ton = 12e3 * Btu / hour = _ = ton_of_refrigeration  # approximate, no exact definition
-standard_liter_per_minute = atmosphere * liter / minute = slpm = slm
-conventional_watt_90 = K_J90 ** 2 * R_K90 / (K_J ** 2 * R_K) * watt = W_90
-
-# Momentum
-[momentum] = [length] * [mass] / [time]
-
-# Density (as auxiliary for pressure)
-[density] = [mass] / [volume]
-mercury = 13.5951 * kilogram / liter = Hg = Hg_0C = Hg_32F = conventional_mercury
-water = 1.0 * kilogram / liter = H2O = conventional_water
-mercury_60F = 13.5568 * kilogram / liter = Hg_60F   # approximate
-water_39F = 0.999972 * kilogram / liter = water_4C  # approximate
-water_60F = 0.999001 * kilogram / liter             # approximate
-
-# Pressure
-[pressure] = [force] / [area]
-pascal = newton / meter ** 2 = Pa
-barye = dyne / centimeter ** 2 = Ba = barie = barad = barrie = baryd
-bar = 1e5 * pascal
-technical_atmosphere = kilogram * g_0 / centimeter ** 2 = at
-torr = atm / 760
-pound_force_per_square_inch = force_pound / inch ** 2 = psi
-kip_per_square_inch = kip / inch ** 2 = ksi
-millimeter_Hg = millimeter * Hg * g_0 = mmHg = mm_Hg = millimeter_Hg_0C
-centimeter_Hg = centimeter * Hg * g_0 = cmHg = cm_Hg = centimeter_Hg_0C
-inch_Hg = inch * Hg * g_0 = inHg = in_Hg = inch_Hg_32F
-inch_Hg_60F = inch * Hg_60F * g_0
-inch_H2O_39F = inch * water_39F * g_0
-inch_H2O_60F = inch * water_60F * g_0
-foot_H2O = foot * water * g_0 = ftH2O = feet_H2O
-centimeter_H2O = centimeter * water * g_0 = cmH2O = cm_H2O
-sound_pressure_level = 20e-6 * pascal = SPL
-
-# Torque
-[torque] = [force] * [length]
-foot_pound = foot * force_pound = ft_lb = footpound
-
-# Viscosity
-[viscosity] = [pressure] * [time]
-poise = 0.1 * Pa * second = P
-reyn = psi * second
-
-# Kinematic viscosity
-[kinematic_viscosity] = [area] / [time]
-stokes = centimeter ** 2 / second = St
-
-# Fluidity
-[fluidity] = 1 / [viscosity]
-rhe = 1 / poise
-
-# Amount of substance
-particle = 1 / N_A = _ = molecule
-part_per_million = 1 * particle / (1000000 * particle) = ppm
-part_per_billion = 1 * particle / (1000000000 * particle) = ppb
-
-# Concentration
-[concentration] = [substance] / [volume]
-molar = mole / liter = M
-
-# Catalytic activity
-[activity] = [substance] / [time]
-katal = mole / second = kat
-enzyme_unit = micromole / minute = U = enzymeunit
-
-# Entropy
-[entropy] = [energy] / [temperature]
-clausius = calorie / kelvin = Cl
-
-# Molar entropy
-[molar_entropy] = [entropy] / [substance]
-entropy_unit = calorie / kelvin / mole = eu
-
-# Radiation
-becquerel = counts_per_second = Bq
-curie = 3.7e10 * becquerel = Ci
-rutherford = 1e6 * becquerel = Rd
-gray = joule / kilogram = Gy
-sievert = joule / kilogram = Sv
-rads = 0.01 * gray
-rem = 0.01 * sievert
-roentgen = 2.58e-4 * coulomb / kilogram = _ = röntgen  # approximate, depends on medium
-
-# Heat transimission
-[heat_transmission] = [energy] / [area]
-peak_sun_hour = 1e3 * watt_hour / meter ** 2 = PSH
-langley = thermochemical_calorie / centimeter ** 2 = Ly
-
-# Luminance
-[luminance] = [luminosity] / [area]
-nit = candela / meter ** 2
-stilb = candela / centimeter ** 2
-lambert = 1 / π * candela / centimeter ** 2
-
-# Luminous flux
-[luminous_flux] = [luminosity]
-lumen = candela * steradian = lm
-
-# Illuminance
-[illuminance] = [luminous_flux] / [area]
-lux = lumen / meter ** 2 = lx
-
-# Intensity
-[intensity] = [power] / [area]
-atomic_unit_of_intensity = 0.5 * ε_0 * c * atomic_unit_of_electric_field ** 2 = a_u_intensity
-
-# Current
-biot = 10 * ampere = Bi
-abampere = biot = abA
-atomic_unit_of_current = e / atomic_unit_of_time = a_u_current
-mean_international_ampere = mean_international_volt / mean_international_ohm = A_it
-US_international_ampere = US_international_volt / US_international_ohm = A_US
-conventional_ampere_90 = K_J90 * R_K90 / (K_J * R_K) * ampere = A_90
-planck_current = (c ** 6 / gravitational_constant / k_C) ** 0.5
-
-# Charge
-[charge] = [current] * [time]
-coulomb = ampere * second = C
-abcoulomb = 10 * C = abC
-faraday = e * N_A * mole
-conventional_coulomb_90 = K_J90 * R_K90 / (K_J * R_K) * coulomb = C_90
-ampere_hour = ampere * hour = Ah
-
-# Electric potential
-[electric_potential] = [energy] / [charge]
-volt = joule / coulomb = V
-abvolt = 1e-8 * volt = abV
-mean_international_volt = 1.00034 * volt = V_it  # approximate
-US_international_volt = 1.00033 * volt = V_US    # approximate
-conventional_volt_90 = K_J90 / K_J * volt = V_90
-
-# Electric field
-[electric_field] = [electric_potential] / [length]
-atomic_unit_of_electric_field = e * k_C / a_0 ** 2 = a_u_electric_field
-
-# Electric displacement field
-[electric_displacement_field] = [charge] / [area]
-
-# Resistance
-[resistance] = [electric_potential] / [current]
-ohm = volt / ampere = Ω
-abohm = 1e-9 * ohm = abΩ
-mean_international_ohm = 1.00049 * ohm = Ω_it = ohm_it  # approximate
-US_international_ohm = 1.000495 * ohm = Ω_US = ohm_US   # approximate
-conventional_ohm_90 = R_K / R_K90 * ohm = Ω_90 = ohm_90
-
-# Resistivity
-[resistivity] = [resistance] * [length]
-
-# Conductance
-[conductance] = [current] / [electric_potential]
-siemens = ampere / volt = S = mho
-absiemens = 1e9 * siemens = abS = abmho
-
-# Capacitance
-[capacitance] = [charge] / [electric_potential]
-farad = coulomb / volt = F
-abfarad = 1e9 * farad = abF
-conventional_farad_90 = R_K90 / R_K * farad = F_90
-
-# Inductance
-[inductance] = [magnetic_flux] / [current]
-henry = weber / ampere = H
-abhenry = 1e-9 * henry = abH
-conventional_henry_90 = R_K / R_K90 * henry = H_90
-
-# Magnetic flux
-[magnetic_flux] = [electric_potential] * [time]
-weber = volt * second = Wb
-unit_pole = µ_0 * biot * centimeter
-
-# Magnetic field
-[magnetic_field] = [magnetic_flux] / [area]
-tesla = weber / meter ** 2 = T
-gamma = 1e-9 * tesla = γ
-
-# Magnetomotive force
-[magnetomotive_force] = [current]
-ampere_turn = ampere = At
-biot_turn = biot
-gilbert = 1 / (4 * π) * biot_turn = Gb
-
-# Magnetic field strength
-[magnetic_field_strength] = [current] / [length]
-
-# Electric dipole moment
-[electric_dipole] = [charge] * [length]
-debye = 1e-9 / ζ * coulomb * angstrom = D  # formally 1 D = 1e-10 Fr*Å, but we generally want to use it outside the Gaussian context
-
-# Electric quadrupole moment
-[electric_quadrupole] = [charge] * [area]
-buckingham = debye * angstrom
-
-# Magnetic dipole moment
-[magnetic_dipole] = [current] * [area]
-bohr_magneton = e * hbar / (2 * m_e) = µ_B = mu_B
-nuclear_magneton = e * hbar / (2 * m_p) = µ_N = mu_N
-
-# Logaritmic Unit Definition
-#  Unit = scale; logbase; logfactor 
-#  x_dB = [logfactor] * log( x_lin / [scale] ) / log( [logbase] )
- 
-# Logaritmic Units of dimensionless quantity: [ https://en.wikipedia.org/wiki/Level_(logarithmic_quantity) ]
-
-decibelmilliwatt = 1e-3 watt; logbase: 10; logfactor: 10 = dBm
-decibelmicrowatt = 1e-6 watt; logbase: 10; logfactor: 10 = dBu
-
-decibel = 1 ; logbase: 10; logfactor: 10 = dB
-# bell = 1 ; logbase: 10; logfactor: = B
-## NOTE: B (Bell) symbol conflicts with byte
-
-decade = 1 ; logbase: 10; logfactor: 1
-## NOTE: decade [time] can conflict with decade [dimensionless]
-
-octave = 1 ; logbase: 2; logfactor: 1 = oct
-
-neper = 1 ; logbase: 2.71828182845904523536028747135266249775724709369995; logfactor: 0.5 = Np
-# neper = 1 ; logbase: eulers_number; logfactor: 0.5 = Np
-
-#### UNIT GROUPS ####
-# Mostly for length, area, volume, mass, force
-# (customary or specialized units)
-
-@group USCSLengthInternational
-    thou = 1e-3 * inch = th = mil_length
-    inch = yard / 36 = in = international_inch = inches = international_inches
-    hand = 4 * inch
-    foot = yard / 3 = ft = international_foot = feet = international_feet
-    yard = 0.9144 * meter = yd = international_yard  # since Jul 1959
-    mile = 1760 * yard = mi = international_mile
-
-    circular_mil = π / 4 * mil_length ** 2 = cmil
-    square_inch = inch ** 2 = sq_in = square_inches
-    square_foot = foot ** 2 = sq_ft = square_feet
-    square_yard = yard ** 2 = sq_yd
-    square_mile = mile ** 2 = sq_mi
-
-    cubic_inch = in ** 3 = cu_in
-    cubic_foot = ft ** 3 = cu_ft = cubic_feet
-    cubic_yard = yd ** 3 = cu_yd
-@end
-
-@group USCSLengthSurvey
-    link = 1e-2 * chain = li = survey_link
-    survey_foot = 1200 / 3937 * meter = sft
-    fathom = 6 * survey_foot
-    rod = 16.5 * survey_foot = rd = pole = perch
-    chain = 4 * rod
-    furlong = 40 * rod = fur
-    cables_length = 120 * fathom
-    survey_mile = 5280 * survey_foot = smi = us_statute_mile
-    league = 3 * survey_mile
-
-    square_rod = rod ** 2 = sq_rod = sq_pole = sq_perch
-    acre = 10 * chain ** 2
-    square_survey_mile = survey_mile ** 2 = _ = section
-    square_league = league ** 2
-
-    acre_foot = acre * survey_foot = _ = acre_feet
-@end
-
-@group USCSDryVolume
-    dry_pint = bushel / 64 = dpi = US_dry_pint
-    dry_quart = bushel / 32 = dqt = US_dry_quart
-    dry_gallon = bushel / 8 = dgal = US_dry_gallon
-    peck = bushel / 4 = pk
-    bushel = 2150.42 cubic_inch = bu
-    dry_barrel = 7056 cubic_inch = _ = US_dry_barrel
-    board_foot = ft * ft * in = FBM = board_feet = BF = BDFT = super_foot = superficial_foot = super_feet = superficial_feet
-@end
-
-@group USCSLiquidVolume
-    minim = pint / 7680
-    fluid_dram = pint / 128 = fldr = fluidram = US_fluid_dram = US_liquid_dram
-    fluid_ounce = pint / 16 = floz = US_fluid_ounce = US_liquid_ounce
-    gill = pint / 4 = gi = liquid_gill = US_liquid_gill
-    pint = quart / 2 = pt = liquid_pint = US_pint
-    fifth = gallon / 5 = _ = US_liquid_fifth
-    quart = gallon / 4 = qt = liquid_quart = US_liquid_quart
-    gallon = 231 * cubic_inch = gal = liquid_gallon = US_liquid_gallon
-@end
-
-@group USCSVolumeOther
-    teaspoon = fluid_ounce / 6 = tsp
-    tablespoon = fluid_ounce / 2 = tbsp
-    shot = 3 * tablespoon = jig = US_shot
-    cup = pint / 2 = cp = liquid_cup = US_liquid_cup
-    barrel = 31.5 * gallon = bbl
-    oil_barrel = 42 * gallon = oil_bbl
-    beer_barrel = 31 * gallon = beer_bbl
-    hogshead = 63 * gallon
-@end
-
-@group Avoirdupois
-    dram = pound / 256 = dr = avoirdupois_dram = avdp_dram = drachm
-    ounce = pound / 16 = oz = avoirdupois_ounce = avdp_ounce
-    pound = 7e3 * grain = lb = avoirdupois_pound = avdp_pound
-    stone = 14 * pound
-    quarter = 28 * stone
-    bag = 94 * pound
-    hundredweight = 100 * pound = cwt = short_hundredweight
-    long_hundredweight = 112 * pound
-    ton = 2e3 * pound = _ = short_ton
-    long_ton = 2240 * pound
-    slug = g_0 * pound * second ** 2 / foot
-    slinch = g_0 * pound * second ** 2 / inch = blob = slugette
-
-    force_ounce = g_0 * ounce = ozf = ounce_force
-    force_pound = g_0 * pound = lbf = pound_force
-    force_ton = g_0 * ton = _ = ton_force = force_short_ton = short_ton_force
-    force_long_ton = g_0 * long_ton = _ = long_ton_force
-    kip = 1e3 * force_pound
-    poundal = pound * foot / second ** 2 = pdl
-@end
-
-@group AvoirdupoisUK using Avoirdupois
-    UK_hundredweight = long_hundredweight = UK_cwt
-    UK_ton = long_ton
-    UK_force_ton = force_long_ton = _ = UK_ton_force
-@end
-
-@group AvoirdupoisUS using Avoirdupois
-    US_hundredweight = hundredweight = US_cwt
-    US_ton = ton
-    US_force_ton = force_ton = _ = US_ton_force
-@end
-
-@group Troy
-    pennyweight = 24 * grain = dwt
-    troy_ounce = 480 * grain = toz = ozt
-    troy_pound = 12 * troy_ounce = tlb = lbt
-@end
-
-@group Apothecary
-    scruple = 20 * grain
-    apothecary_dram = 3 * scruple = ap_dr
-    apothecary_ounce = 8 * apothecary_dram = ap_oz
-    apothecary_pound = 12 * apothecary_ounce = ap_lb
-@end
-
-@group ImperialVolume
-    imperial_minim = imperial_fluid_ounce / 480
-    imperial_fluid_scruple = imperial_fluid_ounce / 24
-    imperial_fluid_drachm = imperial_fluid_ounce / 8 = imperial_fldr = imperial_fluid_dram
-    imperial_fluid_ounce = imperial_pint / 20 = imperial_floz = UK_fluid_ounce
-    imperial_gill = imperial_pint / 4 = imperial_gi = UK_gill
-    imperial_cup = imperial_pint / 2 = imperial_cp = UK_cup
-    imperial_pint = imperial_gallon / 8 = imperial_pt = UK_pint
-    imperial_quart = imperial_gallon / 4 = imperial_qt = UK_quart
-    imperial_gallon = 4.54609 * liter = imperial_gal = UK_gallon
-    imperial_peck = 2 * imperial_gallon = imperial_pk = UK_pk
-    imperial_bushel = 8 * imperial_gallon = imperial_bu = UK_bushel
-    imperial_barrel = 36 * imperial_gallon = imperial_bbl = UK_bbl
-@end
-
-
-
-
-#### CONVERSION CONTEXTS ####
-
-@context(n=1) spectroscopy = sp
-    # n index of refraction of the medium.
-    [length] <-> [frequency]: speed_of_light / n / value
-    [frequency] -> [energy]: planck_constant * value
-    [energy] -> [frequency]: value / planck_constant
-    # allow wavenumber / kayser
-    [wavenumber] <-> [length]: 1 / value
-@end
-
-@context boltzmann
-    [temperature] -> [energy]: boltzmann_constant * value
-    [energy] -> [temperature]: value / boltzmann_constant
-@end
-
-@context energy
-    [energy] -> [energy] / [substance]: value * N_A
-    [energy] / [substance] -> [energy]: value / N_A
-    [energy] -> [mass]: value / c ** 2
-    [mass] -> [energy]: value * c ** 2
-@end
-
-@context(mw=0,volume=0,solvent_mass=0) chemistry = chem
-    # mw is the molecular weight of the species
-    # volume is the volume of the solution
-    # solvent_mass is the mass of solvent in the solution
-
-    # moles -> mass require the molecular weight
-    [substance] -> [mass]: value * mw
-    [mass] -> [substance]: value / mw
-
-    # moles/volume -> mass/volume and moles/mass -> mass/mass
-    # require the  molecular weight
-    [substance] / [volume] -> [mass] / [volume]: value * mw
-    [mass] / [volume] -> [substance] / [volume]: value / mw
-    [substance] / [mass] -> [mass] / [mass]: value * mw
-    [mass] / [mass] -> [substance] / [mass]: value / mw
-
-    # moles/volume -> moles requires the solution volume
-    [substance] / [volume] -> [substance]: value * volume
-    [substance] -> [substance] / [volume]: value / volume
-
-    # moles/mass -> moles requires the solvent (usually water) mass
-    [substance] / [mass] -> [substance]: value * solvent_mass
-    [substance] -> [substance] / [mass]: value / solvent_mass
-
-    # moles/mass -> moles/volume require the solvent mass and the volume
-    [substance] / [mass] -> [substance]/[volume]: value * solvent_mass / volume
-    [substance] / [volume] -> [substance] / [mass]: value / solvent_mass * volume
-
-@end
-
-
-
-#### SYSTEMS OF UNITS ####
-
-@system SI
-    second
-    meter
-    kilogram
-    ampere
-    kelvin
-    mole
-    candela
-@end
-
-@system mks using international
-    meter
-    kilogram
-    second
-@end
-
-
-
-@system atomic using international
-    # based on unit m_e, e, hbar, k_C, k
-    bohr: meter
-    electron_mass: gram
-    atomic_unit_of_time: second
-    atomic_unit_of_current: ampere
-    atomic_unit_of_temperature: kelvin
-@end
-
-@system Planck using international
-    # based on unit c, gravitational_constant, hbar, k_C, k
-    planck_length: meter
-    planck_mass: gram
-    planck_time: second
-    planck_current: ampere
-    planck_temperature: kelvin
-@end
-
-@system imperial using ImperialVolume, USCSLengthInternational, AvoirdupoisUK
-    yard
-    pound
-@end
-
-@system US using USCSLiquidVolume, USCSDryVolume, USCSVolumeOther, USCSLengthInternational, USCSLengthSurvey, AvoirdupoisUS
-    yard
-    pound
-@end
+# Default Pint units definition file
+# Based on the International System of Units
+# Language: english
+# :copyright: 2013,2019 by Pint Authors, see AUTHORS for more details.
+
+# Syntax
+# ======
+# Units
+# -----
+# <canonical name> = <relation to another unit or dimension> [= <symbol>] [= <alias>] [ = <alias> ] [...]
+#
+# The canonical name and aliases should be expressed in singular form.
+# Pint automatically deals with plurals built by adding 's' to the singular form; plural
+# forms that don't follow this rule should be instead explicitly listed as aliases.
+#
+# If a unit has no symbol and one wants to define aliases, then the symbol should be
+# conventionally set to _.
+#
+# Example:
+#     millennium = 1e3 * year = _ = millennia
+#
+#
+# Prefixes
+# --------
+# <prefix>- = <amount> [= <symbol>] [= <alias>] [ = <alias> ] [...]
+#
+# Example:
+#     deca- =  1e+1  = da- = deka-
+#
+#
+# Derived dimensions
+# ------------------
+# [dimension name] = <relation to other dimensions>
+#
+# Example:
+#     [density] = [mass] / [volume]
+#
+# Note that primary dimensions don't need to be declared; they can be
+# defined for the first time in a unit definition.
+# E.g. see below `meter = [length]`
+#
+#
+# Additional aliases
+# ------------------
+# @alias <canonical name or previous alias> = <alias> [ = <alias> ] [...]
+#
+# Used to add aliases to already existing unit definitions.
+# Particularly useful when one wants to enrich definitions
+# from defaults_en.txt with custom aliases.
+#
+# Example:
+#     @alias meter = my_meter
+
+# See also: https://pint.readthedocs.io/en/latest/defining.html
+
+@defaults
+    group = international
+    system = mks
+@end
+
+
+#### PREFIXES ####
+
+# decimal prefixes
+yocto- = 1e-24 = y-
+zepto- = 1e-21 = z-
+atto- =  1e-18 = a-
+femto- = 1e-15 = f-
+pico- =  1e-12 = p-
+nano- =  1e-9  = n-
+micro- = 1e-6  = µ- = u-
+milli- = 1e-3  = m-
+centi- = 1e-2  = c-
+deci- =  1e-1  = d-
+deca- =  1e+1  = da- = deka-
+hecto- = 1e2   = h-
+kilo- =  1e3   = k-
+mega- =  1e6   = M-
+giga- =  1e9   = G-
+tera- =  1e12  = T-
+peta- =  1e15  = P-
+exa- =   1e18  = E-
+zetta- = 1e21  = Z-
+yotta- = 1e24  = Y-
+
+# binary_prefixes
+kibi- = 2**10 = Ki-
+mebi- = 2**20 = Mi-
+gibi- = 2**30 = Gi-
+tebi- = 2**40 = Ti-
+pebi- = 2**50 = Pi-
+exbi- = 2**60 = Ei-
+zebi- = 2**70 = Zi-
+yobi- = 2**80 = Yi-
+
+# extra_prefixes
+semi- = 0.5 = _ = demi-
+sesqui- = 1.5
+
+
+#### BASE UNITS ####
+
+meter = [length] = m = metre
+second = [time] = s = sec
+ampere = [current] = A = amp
+candela = [luminosity] = cd = candle
+gram = [mass] = g
+mole = [substance] = mol
+kelvin = [temperature]; offset: 0 = K = degK = °K = degree_Kelvin = degreeK  # older names supported for compatibility
+radian = [] = rad
+bit = []
+count = []
+
+
+#### CONSTANTS ####
+
+@import constants_en.txt
+
+
+#### UNITS ####
+# Common and less common, grouped by quantity.
+# Conversion factors are exact (except when noted),
+# although floating-point conversion may introduce inaccuracies
+
+# Angle
+turn = 2 * π * radian = _ = revolution = cycle = circle
+degree = π / 180 * radian = deg = arcdeg = arcdegree = angular_degree
+arcminute = degree / 60 = arcmin = arc_minute = angular_minute
+arcsecond = arcminute / 60 = arcsec = arc_second = angular_second
+milliarcsecond = 1e-3 * arcsecond = mas
+grade = π / 200 * radian = grad = gon
+mil = π / 32000 * radian
+
+# Solid angle
+steradian = radian ** 2 = sr
+square_degree = (π / 180) ** 2 * sr = sq_deg = sqdeg
+
+# Information
+baud = bit / second = Bd = bps
+
+byte = 8 * bit = B = octet
+# byte = 8 * bit = _ = octet
+## NOTE: B (byte) symbol can conflict with Bell
+
+# Length
+angstrom = 1e-10 * meter = Å = ångström = Å
+micron = micrometer = µ
+fermi = femtometer = fm
+light_year = speed_of_light * julian_year = ly = lightyear
+astronomical_unit = 149597870700 * meter = au  # since Aug 2012
+parsec = 1 / tansec * astronomical_unit = pc
+nautical_mile = 1852 * meter = nmi
+bohr = hbar / (alpha * m_e * c) = a_0 = a0 = bohr_radius = atomic_unit_of_length = a_u_length
+x_unit_Cu = K_alpha_Cu_d_220 * d_220 / 1537.4 = Xu_Cu
+x_unit_Mo = K_alpha_Mo_d_220 * d_220 / 707.831 = Xu_Mo
+angstrom_star = K_alpha_W_d_220 * d_220 / 0.2090100 = Å_star
+planck_length = (hbar * gravitational_constant / c ** 3) ** 0.5
+
+# Mass
+metric_ton = 1e3 * kilogram = t = tonne
+unified_atomic_mass_unit = atomic_mass_constant = u = amu
+dalton = atomic_mass_constant = Da
+grain = 64.79891 * milligram = gr
+gamma_mass = microgram
+carat = 200 * milligram = ct = karat
+planck_mass = (hbar * c / gravitational_constant) ** 0.5
+
+# Time
+minute = 60 * second = min
+hour = 60 * minute = hr
+day = 24 * hour = d
+week = 7 * day
+fortnight = 2 * week
+year = 365.25 * day = yr = julian_year
+month = year / 12
+
+# decade = 10 * year
+## NOTE: decade [time] can conflict with decade [dimensionless]
+
+century = 100 * year = _ = centuries
+millennium = 1e3 * year = _ = millennia
+eon = 1e9 * year
+shake = 1e-8 * second
+svedberg = 1e-13 * second
+atomic_unit_of_time = hbar / E_h = a_u_time
+gregorian_year = 365.2425 * day
+sidereal_year = 365.256363004 * day                # approximate, as of J2000 epoch
+tropical_year = 365.242190402 * day                # approximate, as of J2000 epoch
+common_year = 365 * day
+leap_year = 366 * day
+sidereal_day = day / 1.00273790935079524           # approximate
+sidereal_month = 27.32166155 * day                 # approximate
+tropical_month = 27.321582 * day                   # approximate
+synodic_month = 29.530589 * day = _ = lunar_month  # approximate
+planck_time = (hbar * gravitational_constant / c ** 5) ** 0.5
+
+# Temperature
+degree_Celsius = kelvin; offset: 273.15 = °C = celsius = degC = degreeC
+degree_Rankine = 5 / 9 * kelvin; offset: 0 = °R = rankine = degR = degreeR
+degree_Fahrenheit = 5 / 9 * kelvin; offset: 233.15 + 200 / 9 = °F = fahrenheit = degF = degreeF
+degree_Reaumur = 4 / 5 * kelvin; offset: 273.15 = °Re = reaumur = degRe = degreeRe = degree_Réaumur = réaumur
+atomic_unit_of_temperature = E_h / k = a_u_temp
+planck_temperature = (hbar * c ** 5 / gravitational_constant / k ** 2) ** 0.5
+
+# Area
+[area] = [length] ** 2
+are = 100 * meter ** 2
+barn = 1e-28 * meter ** 2 = b
+darcy = centipoise * centimeter ** 2 / (second * atmosphere)
+hectare = 100 * are = ha
+
+# Volume
+[volume] = [length] ** 3
+liter = decimeter ** 3 = l = L = litre
+cubic_centimeter = centimeter ** 3 = cc
+lambda = microliter = λ
+stere = meter ** 3
+
+# Frequency
+[frequency] = 1 / [time]
+hertz = 1 / second = Hz
+revolutions_per_minute = revolution / minute = rpm
+revolutions_per_second = revolution / second = rps
+counts_per_second = count / second = cps
+
+# Wavenumber
+[wavenumber] = 1 / [length]
+reciprocal_centimeter = 1 / cm = cm_1 = kayser
+
+# Velocity
+[velocity] = [length] / [time] = [speed]
+knot = nautical_mile / hour = kt = knot_international = international_knot
+mile_per_hour = mile / hour = mph = MPH
+kilometer_per_hour = kilometer / hour = kph = KPH
+kilometer_per_second = kilometer / second = kps
+meter_per_second = meter / second = mps
+foot_per_second = foot / second = fps
+
+# Acceleration
+[acceleration] = [velocity] / [time]
+galileo = centimeter / second ** 2 = Gal
+
+# Force
+[force] = [mass] * [acceleration]
+newton = kilogram * meter / second ** 2 = N
+dyne = gram * centimeter / second ** 2 = dyn
+force_kilogram = g_0 * kilogram = kgf = kilogram_force = pond
+force_gram = g_0 * gram = gf = gram_force
+force_metric_ton = g_0 * metric_ton = tf = metric_ton_force = force_t = t_force
+atomic_unit_of_force = E_h / a_0 = a_u_force
+
+# Energy
+[energy] = [force] * [length]
+joule = newton * meter = J
+erg = dyne * centimeter
+watt_hour = watt * hour = Wh = watthour
+electron_volt = e * volt = eV
+rydberg = h * c * R_inf = Ry
+hartree = 2 * rydberg = E_h = Eh = hartree_energy = atomic_unit_of_energy = a_u_energy
+calorie = 4.184 * joule = cal = thermochemical_calorie = cal_th
+international_calorie = 4.1868 * joule = cal_it = international_steam_table_calorie
+fifteen_degree_calorie = 4.1855 * joule = cal_15
+british_thermal_unit = 1055.056 * joule = Btu = BTU = Btu_iso
+international_british_thermal_unit = 1e3 * pound / kilogram * degR / kelvin * international_calorie = Btu_it
+thermochemical_british_thermal_unit = 1e3 * pound / kilogram * degR / kelvin * calorie = Btu_th
+quadrillion_Btu = 1e15 * Btu = quad
+therm = 1e5 * Btu = thm = EC_therm
+US_therm = 1.054804e8 * joule  # approximate, no exact definition
+ton_TNT = 1e9 * calorie = tTNT
+tonne_of_oil_equivalent = 1e10 * international_calorie = toe
+atmosphere_liter = atmosphere * liter = atm_l
+
+# Power
+[power] = [energy] / [time]
+watt = joule / second = W
+volt_ampere = volt * ampere = VA
+horsepower = 550 * foot * force_pound / second = hp = UK_horsepower = hydraulic_horsepower
+boiler_horsepower = 33475 * Btu / hour                            # unclear which Btu
+metric_horsepower = 75 * force_kilogram * meter / second
+electrical_horsepower = 746 * watt
+refrigeration_ton = 12e3 * Btu / hour = _ = ton_of_refrigeration  # approximate, no exact definition
+standard_liter_per_minute = atmosphere * liter / minute = slpm = slm
+conventional_watt_90 = K_J90 ** 2 * R_K90 / (K_J ** 2 * R_K) * watt = W_90
+
+# Momentum
+[momentum] = [length] * [mass] / [time]
+
+# Density (as auxiliary for pressure)
+[density] = [mass] / [volume]
+mercury = 13.5951 * kilogram / liter = Hg = Hg_0C = Hg_32F = conventional_mercury
+water = 1.0 * kilogram / liter = H2O = conventional_water
+mercury_60F = 13.5568 * kilogram / liter = Hg_60F   # approximate
+water_39F = 0.999972 * kilogram / liter = water_4C  # approximate
+water_60F = 0.999001 * kilogram / liter             # approximate
+
+# Pressure
+[pressure] = [force] / [area]
+pascal = newton / meter ** 2 = Pa
+barye = dyne / centimeter ** 2 = Ba = barie = barad = barrie = baryd
+bar = 1e5 * pascal
+technical_atmosphere = kilogram * g_0 / centimeter ** 2 = at
+torr = atm / 760
+pound_force_per_square_inch = force_pound / inch ** 2 = psi
+kip_per_square_inch = kip / inch ** 2 = ksi
+millimeter_Hg = millimeter * Hg * g_0 = mmHg = mm_Hg = millimeter_Hg_0C
+centimeter_Hg = centimeter * Hg * g_0 = cmHg = cm_Hg = centimeter_Hg_0C
+inch_Hg = inch * Hg * g_0 = inHg = in_Hg = inch_Hg_32F
+inch_Hg_60F = inch * Hg_60F * g_0
+inch_H2O_39F = inch * water_39F * g_0
+inch_H2O_60F = inch * water_60F * g_0
+foot_H2O = foot * water * g_0 = ftH2O = feet_H2O
+centimeter_H2O = centimeter * water * g_0 = cmH2O = cm_H2O
+sound_pressure_level = 20e-6 * pascal = SPL
+
+# Torque
+[torque] = [force] * [length]
+foot_pound = foot * force_pound = ft_lb = footpound
+
+# Viscosity
+[viscosity] = [pressure] * [time]
+poise = 0.1 * Pa * second = P
+reyn = psi * second
+
+# Kinematic viscosity
+[kinematic_viscosity] = [area] / [time]
+stokes = centimeter ** 2 / second = St
+
+# Fluidity
+[fluidity] = 1 / [viscosity]
+rhe = 1 / poise
+
+# Amount of substance
+particle = 1 / N_A = _ = molecule
+part_per_million = 1 * particle / (1000000 * particle) = ppm
+part_per_billion = 1 * particle / (1000000000 * particle) = ppb
+
+# Concentration
+[concentration] = [substance] / [volume]
+molar = mole / liter = M
+
+# Catalytic activity
+[activity] = [substance] / [time]
+katal = mole / second = kat
+enzyme_unit = micromole / minute = U = enzymeunit
+
+# Entropy
+[entropy] = [energy] / [temperature]
+clausius = calorie / kelvin = Cl
+
+# Molar entropy
+[molar_entropy] = [entropy] / [substance]
+entropy_unit = calorie / kelvin / mole = eu
+
+# Radiation
+becquerel = counts_per_second = Bq
+curie = 3.7e10 * becquerel = Ci
+rutherford = 1e6 * becquerel = Rd
+gray = joule / kilogram = Gy
+sievert = joule / kilogram = Sv
+rads = 0.01 * gray
+rem = 0.01 * sievert
+roentgen = 2.58e-4 * coulomb / kilogram = _ = röntgen  # approximate, depends on medium
+
+# Heat transimission
+[heat_transmission] = [energy] / [area]
+peak_sun_hour = 1e3 * watt_hour / meter ** 2 = PSH
+langley = thermochemical_calorie / centimeter ** 2 = Ly
+
+# Luminance
+[luminance] = [luminosity] / [area]
+nit = candela / meter ** 2
+stilb = candela / centimeter ** 2
+lambert = 1 / π * candela / centimeter ** 2
+
+# Luminous flux
+[luminous_flux] = [luminosity]
+lumen = candela * steradian = lm
+
+# Illuminance
+[illuminance] = [luminous_flux] / [area]
+lux = lumen / meter ** 2 = lx
+
+# Intensity
+[intensity] = [power] / [area]
+atomic_unit_of_intensity = 0.5 * ε_0 * c * atomic_unit_of_electric_field ** 2 = a_u_intensity
+
+# Current
+biot = 10 * ampere = Bi
+abampere = biot = abA
+atomic_unit_of_current = e / atomic_unit_of_time = a_u_current
+mean_international_ampere = mean_international_volt / mean_international_ohm = A_it
+US_international_ampere = US_international_volt / US_international_ohm = A_US
+conventional_ampere_90 = K_J90 * R_K90 / (K_J * R_K) * ampere = A_90
+planck_current = (c ** 6 / gravitational_constant / k_C) ** 0.5
+
+# Charge
+[charge] = [current] * [time]
+coulomb = ampere * second = C
+abcoulomb = 10 * C = abC
+faraday = e * N_A * mole
+conventional_coulomb_90 = K_J90 * R_K90 / (K_J * R_K) * coulomb = C_90
+ampere_hour = ampere * hour = Ah
+
+# Electric potential
+[electric_potential] = [energy] / [charge]
+volt = joule / coulomb = V
+abvolt = 1e-8 * volt = abV
+mean_international_volt = 1.00034 * volt = V_it  # approximate
+US_international_volt = 1.00033 * volt = V_US    # approximate
+conventional_volt_90 = K_J90 / K_J * volt = V_90
+
+# Electric field
+[electric_field] = [electric_potential] / [length]
+atomic_unit_of_electric_field = e * k_C / a_0 ** 2 = a_u_electric_field
+
+# Electric displacement field
+[electric_displacement_field] = [charge] / [area]
+
+# Resistance
+[resistance] = [electric_potential] / [current]
+ohm = volt / ampere = Ω
+abohm = 1e-9 * ohm = abΩ
+mean_international_ohm = 1.00049 * ohm = Ω_it = ohm_it  # approximate
+US_international_ohm = 1.000495 * ohm = Ω_US = ohm_US   # approximate
+conventional_ohm_90 = R_K / R_K90 * ohm = Ω_90 = ohm_90
+
+# Resistivity
+[resistivity] = [resistance] * [length]
+
+# Conductance
+[conductance] = [current] / [electric_potential]
+siemens = ampere / volt = S = mho
+absiemens = 1e9 * siemens = abS = abmho
+
+# Capacitance
+[capacitance] = [charge] / [electric_potential]
+farad = coulomb / volt = F
+abfarad = 1e9 * farad = abF
+conventional_farad_90 = R_K90 / R_K * farad = F_90
+
+# Inductance
+[inductance] = [magnetic_flux] / [current]
+henry = weber / ampere = H
+abhenry = 1e-9 * henry = abH
+conventional_henry_90 = R_K / R_K90 * henry = H_90
+
+# Magnetic flux
+[magnetic_flux] = [electric_potential] * [time]
+weber = volt * second = Wb
+unit_pole = µ_0 * biot * centimeter
+
+# Magnetic field
+[magnetic_field] = [magnetic_flux] / [area]
+tesla = weber / meter ** 2 = T
+gamma = 1e-9 * tesla = γ
+
+# Magnetomotive force
+[magnetomotive_force] = [current]
+ampere_turn = ampere = At
+biot_turn = biot
+gilbert = 1 / (4 * π) * biot_turn = Gb
+
+# Magnetic field strength
+[magnetic_field_strength] = [current] / [length]
+
+# Electric dipole moment
+[electric_dipole] = [charge] * [length]
+debye = 1e-9 / ζ * coulomb * angstrom = D  # formally 1 D = 1e-10 Fr*Å, but we generally want to use it outside the Gaussian context
+
+# Electric quadrupole moment
+[electric_quadrupole] = [charge] * [area]
+buckingham = debye * angstrom
+
+# Magnetic dipole moment
+[magnetic_dipole] = [current] * [area]
+bohr_magneton = e * hbar / (2 * m_e) = µ_B = mu_B
+nuclear_magneton = e * hbar / (2 * m_p) = µ_N = mu_N
+
+# Logaritmic Unit Definition
+#  Unit = scale; logbase; logfactor 
+#  x_dB = [logfactor] * log( x_lin / [scale] ) / log( [logbase] )
+ 
+# Logaritmic Units of dimensionless quantity: [ https://en.wikipedia.org/wiki/Level_(logarithmic_quantity) ]
+
+decibelmilliwatt = 1e-3 watt; logbase: 10; logfactor: 10 = dBm
+decibelmicrowatt = 1e-6 watt; logbase: 10; logfactor: 10 = dBu
+
+decibel = 1 ; logbase: 10; logfactor: 10 = dB
+# bell = 1 ; logbase: 10; logfactor: = B
+## NOTE: B (Bell) symbol conflicts with byte
+
+decade = 1 ; logbase: 10; logfactor: 1
+## NOTE: decade [time] can conflict with decade [dimensionless]
+
+octave = 1 ; logbase: 2; logfactor: 1 = oct
+
+neper = 1 ; logbase: 2.71828182845904523536028747135266249775724709369995; logfactor: 0.5 = Np
+# neper = 1 ; logbase: eulers_number; logfactor: 0.5 = Np
+
+#### UNIT GROUPS ####
+# Mostly for length, area, volume, mass, force
+# (customary or specialized units)
+
+@group USCSLengthInternational
+    thou = 1e-3 * inch = th = mil_length
+    inch = yard / 36 = in = international_inch = inches = international_inches
+    hand = 4 * inch
+    foot = yard / 3 = ft = international_foot = feet = international_feet
+    yard = 0.9144 * meter = yd = international_yard  # since Jul 1959
+    mile = 1760 * yard = mi = international_mile
+
+    circular_mil = π / 4 * mil_length ** 2 = cmil
+    square_inch = inch ** 2 = sq_in = square_inches
+    square_foot = foot ** 2 = sq_ft = square_feet
+    square_yard = yard ** 2 = sq_yd
+    square_mile = mile ** 2 = sq_mi
+
+    cubic_inch = in ** 3 = cu_in
+    cubic_foot = ft ** 3 = cu_ft = cubic_feet
+    cubic_yard = yd ** 3 = cu_yd
+@end
+
+@group USCSLengthSurvey
+    link = 1e-2 * chain = li = survey_link
+    survey_foot = 1200 / 3937 * meter = sft
+    fathom = 6 * survey_foot
+    rod = 16.5 * survey_foot = rd = pole = perch
+    chain = 4 * rod
+    furlong = 40 * rod = fur
+    cables_length = 120 * fathom
+    survey_mile = 5280 * survey_foot = smi = us_statute_mile
+    league = 3 * survey_mile
+
+    square_rod = rod ** 2 = sq_rod = sq_pole = sq_perch
+    acre = 10 * chain ** 2
+    square_survey_mile = survey_mile ** 2 = _ = section
+    square_league = league ** 2
+
+    acre_foot = acre * survey_foot = _ = acre_feet
+@end
+
+@group USCSDryVolume
+    dry_pint = bushel / 64 = dpi = US_dry_pint
+    dry_quart = bushel / 32 = dqt = US_dry_quart
+    dry_gallon = bushel / 8 = dgal = US_dry_gallon
+    peck = bushel / 4 = pk
+    bushel = 2150.42 cubic_inch = bu
+    dry_barrel = 7056 cubic_inch = _ = US_dry_barrel
+    board_foot = ft * ft * in = FBM = board_feet = BF = BDFT = super_foot = superficial_foot = super_feet = superficial_feet
+@end
+
+@group USCSLiquidVolume
+    minim = pint / 7680
+    fluid_dram = pint / 128 = fldr = fluidram = US_fluid_dram = US_liquid_dram
+    fluid_ounce = pint / 16 = floz = US_fluid_ounce = US_liquid_ounce
+    gill = pint / 4 = gi = liquid_gill = US_liquid_gill
+    pint = quart / 2 = pt = liquid_pint = US_pint
+    fifth = gallon / 5 = _ = US_liquid_fifth
+    quart = gallon / 4 = qt = liquid_quart = US_liquid_quart
+    gallon = 231 * cubic_inch = gal = liquid_gallon = US_liquid_gallon
+@end
+
+@group USCSVolumeOther
+    teaspoon = fluid_ounce / 6 = tsp
+    tablespoon = fluid_ounce / 2 = tbsp
+    shot = 3 * tablespoon = jig = US_shot
+    cup = pint / 2 = cp = liquid_cup = US_liquid_cup
+    barrel = 31.5 * gallon = bbl
+    oil_barrel = 42 * gallon = oil_bbl
+    beer_barrel = 31 * gallon = beer_bbl
+    hogshead = 63 * gallon
+@end
+
+@group Avoirdupois
+    dram = pound / 256 = dr = avoirdupois_dram = avdp_dram = drachm
+    ounce = pound / 16 = oz = avoirdupois_ounce = avdp_ounce
+    pound = 7e3 * grain = lb = avoirdupois_pound = avdp_pound
+    stone = 14 * pound
+    quarter = 28 * stone
+    bag = 94 * pound
+    hundredweight = 100 * pound = cwt = short_hundredweight
+    long_hundredweight = 112 * pound
+    ton = 2e3 * pound = _ = short_ton
+    long_ton = 2240 * pound
+    slug = g_0 * pound * second ** 2 / foot
+    slinch = g_0 * pound * second ** 2 / inch = blob = slugette
+
+    force_ounce = g_0 * ounce = ozf = ounce_force
+    force_pound = g_0 * pound = lbf = pound_force
+    force_ton = g_0 * ton = _ = ton_force = force_short_ton = short_ton_force
+    force_long_ton = g_0 * long_ton = _ = long_ton_force
+    kip = 1e3 * force_pound
+    poundal = pound * foot / second ** 2 = pdl
+@end
+
+@group AvoirdupoisUK using Avoirdupois
+    UK_hundredweight = long_hundredweight = UK_cwt
+    UK_ton = long_ton
+    UK_force_ton = force_long_ton = _ = UK_ton_force
+@end
+
+@group AvoirdupoisUS using Avoirdupois
+    US_hundredweight = hundredweight = US_cwt
+    US_ton = ton
+    US_force_ton = force_ton = _ = US_ton_force
+@end
+
+@group Troy
+    pennyweight = 24 * grain = dwt
+    troy_ounce = 480 * grain = toz = ozt
+    troy_pound = 12 * troy_ounce = tlb = lbt
+@end
+
+@group Apothecary
+    scruple = 20 * grain
+    apothecary_dram = 3 * scruple = ap_dr
+    apothecary_ounce = 8 * apothecary_dram = ap_oz
+    apothecary_pound = 12 * apothecary_ounce = ap_lb
+@end
+
+@group ImperialVolume
+    imperial_minim = imperial_fluid_ounce / 480
+    imperial_fluid_scruple = imperial_fluid_ounce / 24
+    imperial_fluid_drachm = imperial_fluid_ounce / 8 = imperial_fldr = imperial_fluid_dram
+    imperial_fluid_ounce = imperial_pint / 20 = imperial_floz = UK_fluid_ounce
+    imperial_gill = imperial_pint / 4 = imperial_gi = UK_gill
+    imperial_cup = imperial_pint / 2 = imperial_cp = UK_cup
+    imperial_pint = imperial_gallon / 8 = imperial_pt = UK_pint
+    imperial_quart = imperial_gallon / 4 = imperial_qt = UK_quart
+    imperial_gallon = 4.54609 * liter = imperial_gal = UK_gallon
+    imperial_peck = 2 * imperial_gallon = imperial_pk = UK_pk
+    imperial_bushel = 8 * imperial_gallon = imperial_bu = UK_bushel
+    imperial_barrel = 36 * imperial_gallon = imperial_bbl = UK_bbl
+@end
+
+
+
+
+#### CONVERSION CONTEXTS ####
+
+@context(n=1) spectroscopy = sp
+    # n index of refraction of the medium.
+    [length] <-> [frequency]: speed_of_light / n / value
+    [frequency] -> [energy]: planck_constant * value
+    [energy] -> [frequency]: value / planck_constant
+    # allow wavenumber / kayser
+    [wavenumber] <-> [length]: 1 / value
+@end
+
+@context boltzmann
+    [temperature] -> [energy]: boltzmann_constant * value
+    [energy] -> [temperature]: value / boltzmann_constant
+@end
+
+@context energy
+    [energy] -> [energy] / [substance]: value * N_A
+    [energy] / [substance] -> [energy]: value / N_A
+    [energy] -> [mass]: value / c ** 2
+    [mass] -> [energy]: value * c ** 2
+@end
+
+@context(mw=0,volume=0,solvent_mass=0) chemistry = chem
+    # mw is the molecular weight of the species
+    # volume is the volume of the solution
+    # solvent_mass is the mass of solvent in the solution
+
+    # moles -> mass require the molecular weight
+    [substance] -> [mass]: value * mw
+    [mass] -> [substance]: value / mw
+
+    # moles/volume -> mass/volume and moles/mass -> mass/mass
+    # require the  molecular weight
+    [substance] / [volume] -> [mass] / [volume]: value * mw
+    [mass] / [volume] -> [substance] / [volume]: value / mw
+    [substance] / [mass] -> [mass] / [mass]: value * mw
+    [mass] / [mass] -> [substance] / [mass]: value / mw
+
+    # moles/volume -> moles requires the solution volume
+    [substance] / [volume] -> [substance]: value * volume
+    [substance] -> [substance] / [volume]: value / volume
+
+    # moles/mass -> moles requires the solvent (usually water) mass
+    [substance] / [mass] -> [substance]: value * solvent_mass
+    [substance] -> [substance] / [mass]: value / solvent_mass
+
+    # moles/mass -> moles/volume require the solvent mass and the volume
+    [substance] / [mass] -> [substance]/[volume]: value * solvent_mass / volume
+    [substance] / [volume] -> [substance] / [mass]: value / solvent_mass * volume
+
+@end
+
+
+
+#### SYSTEMS OF UNITS ####
+
+@system SI
+    second
+    meter
+    kilogram
+    ampere
+    kelvin
+    mole
+    candela
+@end
+
+@system mks using international
+    meter
+    kilogram
+    second
+@end
+
+
+
+@system atomic using international
+    # based on unit m_e, e, hbar, k_C, k
+    bohr: meter
+    electron_mass: gram
+    atomic_unit_of_time: second
+    atomic_unit_of_current: ampere
+    atomic_unit_of_temperature: kelvin
+@end
+
+@system Planck using international
+    # based on unit c, gravitational_constant, hbar, k_C, k
+    planck_length: meter
+    planck_mass: gram
+    planck_time: second
+    planck_current: ampere
+    planck_temperature: kelvin
+@end
+
+@system imperial using ImperialVolume, USCSLengthInternational, AvoirdupoisUK
+    yard
+    pound
+@end
+
+@system US using USCSLiquidVolume, USCSDryVolume, USCSVolumeOther, USCSLengthInternational, USCSLengthSurvey, AvoirdupoisUS
+    yard
+    pound
+@end
```

### Comparing `unit_parse-0.1.8/src/unit_parse/support_files/dictionary.txt` & `unit_parse-0.1.9/src/unit_parse/support_files/dictionary.txt`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse/utils.py` & `unit_parse-0.1.9/src/unit_parse/utils.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/src/unit_parse.egg-info/PKG-INFO` & `unit_parse-0.1.9/src/unit_parse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
-Name: unit-parse
-Version: 0.1.8
+Name: unit_parse
+Version: 0.1.9
 Summary: Parse units from strings. From mess to order!
 Home-page: https://github.com/dylanwal/unit_parse
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE.txt
+Requires-Dist: pint==0.19
+Provides-Extra: testing
+Requires-Dist: pytest>=6.0; extra == "testing"
+Requires-Dist: pytest-cov>=2.0; extra == "testing"
+Requires-Dist: mypy>=0.910; extra == "testing"
+Requires-Dist: flake8>=3.9; extra == "testing"
 
 # Unit Parse (unit_parse)
 
 ---
 ---
 ![PyPI](https://img.shields.io/pypi/v/unit_parse)
 ![tests](https://raw.githubusercontent.com/dylanwal/unit_parse/master/tests/badges/tests-badge.svg)
```

### Comparing `unit_parse-0.1.8/src/unit_parse.egg-info/SOURCES.txt` & `unit_parse-0.1.9/src/unit_parse.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/unit_parse/classification.py
 src/unit_parse/config.py
 src/unit_parse/core.py
 src/unit_parse/logger.py
 src/unit_parse/main.py
 src/unit_parse/pre_processing_multiple.py
 src/unit_parse/pre_processing_substitution.py
+src/unit_parse/py.typed
 src/unit_parse/reduce_quantities.py
 src/unit_parse/utils.py
 src/unit_parse.egg-info/PKG-INFO
 src/unit_parse.egg-info/SOURCES.txt
 src/unit_parse.egg-info/dependency_links.txt
 src/unit_parse.egg-info/not-zip-safe
 src/unit_parse.egg-info/requires.txt
```

### Comparing `unit_parse-0.1.8/tests/test_classification.py` & `unit_parse-0.1.9/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/tests/test_config.py` & `unit_parse-0.1.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/tests/test_core.py` & `unit_parse-0.1.9/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/tests/test_main.py` & `unit_parse-0.1.9/tests/test_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
-from unit_parse import parser, Quantity
-
+from unit_parse import Quantity, parser
 
 examples = [
     # standard examples
     ["5", Quantity("5")],
     ["5 g", Quantity("5 g")],
     ["5 g/ml", Quantity("5 g/ml")],
     ["1 K", Quantity("1 kelvin")],
@@ -61,14 +60,15 @@
 
     # conditions
     ["37.34 kJ/mole (at 25 °C)", [[Quantity("37.34 kJ/mole"), Quantity("25 degC")]]],
     ['20.8 mm Hg @ 25 °C', [[Quantity('20.8 mmHg'), Quantity('25 degC')]]],
     ['20.8 mm Hg (25 °C)', [[Quantity('20.8 mmHg'), Quantity('25 degC')]]],
     ['20.8 mm Hg at 25 °C', [[Quantity('20.8 mmHg'), Quantity('25 degC')]]],
     ["-4,395.63 kJ/mol at 25 °C", [[Quantity('-4395.63 kJ/mol'), Quantity('25 degC')]]],
+    ["1.0A @ 25kW", [[Quantity('1.0A'), Quantity('25kW')]]],
 
     # list of quantities
     ['18 mm Hg; 20 mm Hg', Quantity('20 mmHg')],
     ['18 mm Hg @ 68 °F; 20 mm Hg @ 77° F',
      [[Quantity('18 mmHg'), Quantity('68 degF')], [Quantity('20 mmHg'), Quantity('77 degF')]]],
     ['18 mm Hg @ 68 °F ; 20 mm Hg @ 77° F (NTP, 1992)',
      [[Quantity('18 mmHg'), Quantity('68 degF')], [Quantity('20 mmHg'), Quantity('77 degF')]]],
@@ -77,14 +77,16 @@
     ["Low threshold= 13.1150 mg/cu m; High threshold= 26840 mg/cu m; Irritating concn= 22875 mg/cu m.",
      Quantity('22875 mg/m**3')],
     ['Melting point: 75% -17.5 °C; 80% 4.6 °C; 85% 21 °C.', Quantity("4.6 degC")],
 
     # ranges
     ['115.2-115.3 °C', Quantity('115.2 degC')],
     ['115.2 - 115.3 °C', Quantity('115.2 degC')],
+    ["1-2 °C",  Quantity('1 degC')],
+    ["0-1 °C",  Quantity('0 degC')],
 
     # words
     ["8.20x10+1 ppm; pure", Quantity("8.20*10**1 ppm")],
     ['40 °F (NTP, 1992)', Quantity("40 degF")],
     ['4.0 °C (39.2 °F) - closed cup', Quantity("4 degC")],
     ['4.0 °C [39.2 g/[mol * s]] - closed cup', [[Quantity("4 degC"), Quantity("39.2 g/(mol * s)")]]],
     ['4.0 °C [39.2 g/[mol * s] approx.] - closed cup', [[Quantity("4 degC"), Quantity("39.2 g/(mol * s)")]]],
```

### Comparing `unit_parse-0.1.8/tests/test_pre_processing_multiple.py` & `unit_parse-0.1.9/tests/test_pre_processing_multiple.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/tests/test_pre_processing_substitution.py` & `unit_parse-0.1.9/tests/test_pre_processing_substitution.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     ["15 10**2 s", "15*10**2 s"],
     ['-14.390 BTU/LB= -7992 CAL/G= -334.6*10**5 J/KG', '-14.390 BTU/LB= -7992 CAL/G= -334.6*10**5 J/KG'],
     ["	0.909 g/cm3", "0.909 g/cm3"],
     ['5.3e1 g/mol', '5.3*10**1 g/mol'],
     ['5.3E1 g/mol', '5.3*10**1 g/mol'],
     ['5.3 109 g/mol', '5.3*10**9 g/mol'],
     ["3.6E+00004 mg/L", "3.6*10**4 mg/L"],
+    ["3.6E00004 mg/L", "3.6*10**4 mg/L"],
 
     # negative control (no changes made)
     ['5.3*10**1 g/mol', '5.3*10**1 g/mol'],
     ["42.3 gcm-3", "42.3 gcm-3"],
     ["0.909 g/cm3", "0.909 g/cm3"],
     ["40 °F", "40 °F"],
     ["39.2 g/[mol * s]]", "39.2 g/[mol * s]]"],
```

### Comparing `unit_parse-0.1.8/tests/test_reduce_quantity.py` & `unit_parse-0.1.9/tests/test_reduce_quantity.py`

 * *Files identical despite different names*

### Comparing `unit_parse-0.1.8/tests/test_utils.py` & `unit_parse-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

