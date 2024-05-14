# Comparing `tmp/tom_iag-0.2.8.tar.gz` & `tmp/tom_iag-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_iag-0.2.8.tar", max compression
+gzip compressed data, was "tom_iag-0.2.9.tar", max compression
```

## Comparing `tom_iag-0.2.8.tar` & `tom_iag-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-09-07 09:54:19.301164 tom_iag-0.2.8/LICENSE
--rw-r--r--   0        0        0      169 2023-09-07 09:54:19.301164 tom_iag-0.2.8/README.md
--rw-r--r--   0        0        0      438 2023-09-07 09:54:19.301164 tom_iag-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-07 09:54:19.301164 tom_iag-0.2.8/tom_iag/__init__.py
--rw-r--r--   0        0        0    23504 2023-09-07 09:54:19.301164 tom_iag-0.2.8/tom_iag/iag.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 tom_iag-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-12-15 19:40:54.905983 tom_iag-0.2.9/LICENSE
+-rw-r--r--   0        0        0      169 2023-12-15 19:40:54.905983 tom_iag-0.2.9/README.md
+-rw-r--r--   0        0        0      438 2023-12-15 19:40:54.905983 tom_iag-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-15 19:40:54.905983 tom_iag-0.2.9/tom_iag/__init__.py
+-rw-r--r--   0        0        0    23511 2023-12-15 19:40:54.905983 tom_iag-0.2.9/tom_iag/iag.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 tom_iag-0.2.9/PKG-INFO
```

### Comparing `tom_iag-0.2.8/LICENSE` & `tom_iag-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_iag-0.2.8/tom_iag/iag.py` & `tom_iag-0.2.9/tom_iag/iag.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
         )
 
     def readout_choices(self):
         return sorted([(f["code"], f["name"]) for f in self._instrument["modes"]["readout"]["modes"]])
 
 
 class MonetSouthImagingObservationForm(IAGImagingObservationForm):
-    INSTRUMENT = "1M2 FLI230"
+    INSTRUMENT = "1M2 MONETS FLI230"
 
     @property
     def _instrument(self):
         return get_instruments()[MonetSouthImagingObservationForm.INSTRUMENT]
 
     def instrument_choices(self):
         return [(MonetSouthImagingObservationForm.INSTRUMENT, self._instrument["name"])]
```

### Comparing `tom_iag-0.2.8/PKG-INFO` & `tom_iag-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-iag
-Version: 0.2.8
+Version: 0.2.9
 Summary: IAG telescopes facility module for the TOM Toolkit
 Home-page: https://github.com/thusser/tom_iag
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

