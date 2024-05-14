# Comparing `tmp/dem_roughness_calculator-1.2.2.tar.gz` & `tmp/dem_roughness_calculator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dem_roughness_calculator-1.2.2.tar", last modified: Sat May 11 00:04:11 2024, max compression
+gzip compressed data, was "dem_roughness_calculator-1.3.0.tar", last modified: Tue May 14 08:48:26 2024, max compression
```

## Comparing `dem_roughness_calculator-1.2.2.tar` & `dem_roughness_calculator-1.3.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:11.063836 dem_roughness_calculator-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-11 00:04:11.063836 dem_roughness_calculator-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:11.063836 dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-11 00:04:11.000000 dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-11 00:04:11.000000 dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 00:04:11.000000 dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-11 00:04:11.000000 dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 00:04:11.000000 dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 00:04:11.000000 dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:11.059836 dem_roughness_calculator-1.2.2/roughness_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:11.059836 dem_roughness_calculator-1.2.2/roughness_calculator/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:11.063836 dem_roughness_calculator-1.2.2/roughness_calculator/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/encapsulating_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui/preview_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:11.063836 dem_roughness_calculator-1.2.2/roughness_calculator/old_entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/old_entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/old_entry_points/demcli.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/roughness_calculator/old_entry_points/demgui.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 00:04:11.063836 dem_roughness_calculator-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:11.063836 dem_roughness_calculator-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-11 00:04:02.000000 dem_roughness_calculator-1.2.2/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:26.193303 dem_roughness_calculator-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-14 08:48:26.193303 dem_roughness_calculator-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:26.189303 dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-14 08:48:26.000000 dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-14 08:48:26.000000 dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:48:26.000000 dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 08:48:26.000000 dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 08:48:26.000000 dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 08:48:26.000000 dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:26.185303 dem_roughness_calculator-1.3.0/roughness_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:26.189303 dem_roughness_calculator-1.3.0/roughness_calculator/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:26.189303 dem_roughness_calculator-1.3.0/roughness_calculator/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/encapsulating_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:26.189303 dem_roughness_calculator-1.3.0/roughness_calculator/old_entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/old_entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/old_entry_points/demcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/roughness_calculator/old_entry_points/demgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:48:26.193303 dem_roughness_calculator-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:26.189303 dem_roughness_calculator-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-14 08:48:17.000000 dem_roughness_calculator-1.3.0/tests/test_application_driver.py
```

### Comparing `dem_roughness_calculator-1.2.2/LICENSE` & `dem_roughness_calculator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.2/PKG-INFO` & `dem_roughness_calculator-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.2.2
+Version: 1.3.0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,7 +16,8 @@
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pillow>=10.3.0
 Requires-Dist: rasterio>=1.3.10
 Requires-Dist: setuptools>=69.5.1
 Requires-Dist: customtkinter~=5.2.2
+Requires-Dist: scipy~=1.13.0
```

### Comparing `dem_roughness_calculator-1.2.2/README.md` & `dem_roughness_calculator-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/PKG-INFO` & `dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.2.2
+Version: 1.3.0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,7 +16,8 @@
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pillow>=10.3.0
 Requires-Dist: rasterio>=1.3.10
 Requires-Dist: setuptools>=69.5.1
 Requires-Dist: customtkinter~=5.2.2
+Requires-Dist: scipy~=1.13.0
```

### Comparing `dem_roughness_calculator-1.2.2/dem_roughness_calculator.egg-info/SOURCES.txt` & `dem_roughness_calculator-1.3.0/dem_roughness_calculator.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 roughness_calculator/log_config.py
 roughness_calculator/main.py
 roughness_calculator/classes/__init__.py
 roughness_calculator/classes/application_driver.py
 roughness_calculator/classes/defaults.py
 roughness_calculator/classes/geo_tiff_processor.py
 roughness_calculator/classes/processing_parameters.py
+roughness_calculator/classes/threshold_optimizer.py
 roughness_calculator/gui/__init__.py
+roughness_calculator/gui/analyze_and_optimize.py
 roughness_calculator/gui/defaults.py
 roughness_calculator/gui/encapsulating_frame.py
 roughness_calculator/gui/footer_frame.py
 roughness_calculator/gui/header_frame.py
 roughness_calculator/gui/parameter_input.py
 roughness_calculator/gui/path_frame.py
 roughness_calculator/gui/preview_image.py
```

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/classes/application_driver.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/classes/application_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 application_driver.py
 ---------------------
-Version: 1.2.2
+Version: 1.3.0
 Author: Lukas Batschelet
-Date: 11.05.2024
+Date: 14.05.2024
 ---------------------
 This module contains the ApplicationDriver class which is responsible for running the application.
 It acts as a sort of interface between the calling User Interface (UI) and the GeoTIFFProcessor class.
 This enables the separation of concerns and allows for easier testing and maintenance of the code.
 (i.e. the UI does not need to know how the processing is done, it just needs to know how to call the processing.)
 """
 import datetime
@@ -40,25 +40,29 @@
 
         self.params = params
 
         self.input_path = params.input_path  # Store the path to the input GeoTIFF file
         self.output_dir = params.output_dir  # Store the path to the output directory if provided
 
         # Attempt to create an output filename if an output directory is provided
-        self.output_path = ApplicationDriver.create_output_filename(params, include_path=True) if params.output_dir else None
+        self.output_path = ApplicationDriver.create_output_filename(params,
+                                                                    include_path=True) if params.output_dir else None
 
         # Store additional processing parameters
         self.window_size = params.window_size
         self.band_number = params.band_number
         self.high_value_threshold = params.high_value_threshold
         self.category_thresholds = params.category_thresholds
 
         self.processed_data = None  # This will hold the processed data after running the processor
         self.preview = None  # This will hold the image preview of the processed data
 
+        self.processed_uncategorized_data = None
+        self.processed_profile = None
+
         # Initialize the GeoTIFFProcessor with the parameters
         self.processor = GeoTIFFProcessor(params)
 
     def run(self) -> None:
         """
         Initiates the processing of the GeoTIFF file.
 
@@ -73,26 +77,28 @@
         # Log the start of the processing
         logging.info("Starting processing...")
         logging.info(f"Input path: {self.input_path}")
         logging.info(f"Output dir: {self.output_dir}")
 
         # Process the GeoTIFF file and store the result in self.processed_data
         self.processed_data = self.processor.process_tiff()
+        self.processed_uncategorized_data = self.processor.processed_uncategorized_data
+        self.processed_profile = self.processor.processed_profile
 
         # If an output directory is provided or running in CLI mode, save the processed data immediately
         if self.output_dir:
             self.save_processed_data(self.output_dir)
 
         # Otherwise, generate a preview of the processed data
         else:
             self.produce_preview()
 
         logging.info("Processing completed.")
 
-    def produce_preview(self, nodata_value: int = Defaults.NODATA_VALUE) -> None:
+    def produce_preview(self, nodata_value: int = Defaults.NO_DATA_VALUE) -> None:
         """
         Generates a preview image from the processed data stored in self.processed_data.
         This method avoids re-reading the data from file, making it more efficient.
         Uses pseudo-color to represent the data visually, ensuring nodata values are transparent.
 
         Args:
             nodata_value (int, optional): The value representing 'no data' in the dataset. Defaults to -9999.
@@ -136,60 +142,43 @@
             logging.info("Preview generated successfully.")
         except Exception as e:
             logging.error(f"Failed to produce preview: {str(e)}")
             self.preview = None
             # Raise a new error, preserving the original traceback
             raise RuntimeError("Failed to produce preview due to an error.") from e
 
-    def save_processed_data(self,
-                            output_path: str,
-                            nodata: int = Defaults.NODATA_VALUE,
-                            dtype: str = Defaults.DTYPE) -> None:
+    def save_processed_data(self, output_path: str) -> None:
         """
-        Saves the processed data to a GeoTIFF file using the stored profile.
+        Saves the processed data to a GeoTIFF file using the stored processed_profile.
 
         Args:
             output_path (str): The path where the processed data will be saved.
-            nodata (int, optional): The value representing 'no data' in the dataset. Defaults to -9999.
-            dtype (str, optional): The data type of the output GeoTIFF file. Defaults to 'float32'.
 
         Raises:
-            ValueError: If the processed data or the profile is not available for saving.
+            ValueError: If the processed data or the processed_profile is not available for saving.
         """
-        # Check if processed data and profile are available
-        if self.processed_data is None or self.processor.profile is None:
-            logging.error("Processed data or profile is not available for saving.")
-            raise ValueError("Processed data or profile is missing.")
-
-        # Update the profile with the provided data type and nodata value
-        self.processor.profile.update(dtype=dtype, nodata=nodata)
-
-        # Calculate the new pixel size, width, and height based on the window size
-        pixel_size = self.window_size
-        width = int((self.processor.profile['width'] * self.processor.profile['transform'][0]) / pixel_size)
-        height = int((self.processor.profile['height'] * abs(self.processor.profile['transform'][4])) / pixel_size)
-
-        # Update the transform, width, and height in the profile
-        self.processor.profile['transform'] = rasterio.Affine(pixel_size, 0, self.processor.profile['transform'][2], 0, -pixel_size, self.processor.profile['transform'][5])
-        self.processor.profile['width'] = width
-        self.processor.profile['height'] = height
+        # Check if processed data and processed_profile are available
+        if self.processed_data is None or self.processor.processed_profile is None:
+            logging.error("Processed data or processed_profile is not available for saving.")
+            raise ValueError("Processed data or processed_profile is missing.")
 
         # Open the output path as a new GeoTIFF file in write mode
-        with rasterio.open(output_path, 'w', **self.processor.profile) as dst:
+        with rasterio.open(output_path, 'w', **self.processor.processed_profile) as dst:
             # Write the processed data to the first band of the GeoTIFF file
             dst.write(self.processed_data, 1)
 
         logging.info(f"Processed data saved to {output_path}")
 
     @staticmethod
     def create_output_filename(params: ProcessingParameters, include_path: bool = True) -> str:
         """
         Generates a filename based on the input file, current date, and processing parameters.
 
-        The filename is generated in the following format: YYYYMMDD_basename_Surface-Roughness_windowSize-meter_threshold1_threshold2_...
+        The filename is generated in the following format:
+        YYYYMMDD_basename_Surface-Roughness_windowSize-meter_threshold1_threshold2_...
 
         Args:
             params (ProcessingParameters): The processing parameters.
             include_path (bool): Whether to include the path in the filename.
 
         Returns:
             str: The generated filename with the full path if include_path is True, otherwise just the filename.
```

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/classes/defaults.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/classes/defaults.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+"""
+defaults.py
+-----------
+Version: 1.3.0
+Author: Lukas Batschelet
+Date: 14.05.2024
+-----------
+This module defines default values for the whole package.
+"""
 from typing import Final, Optional, List
 
-
 class Defaults:
     """
     A class used to define default values for the whole package.
 
     Attributes
     ----------
     OUTPUT_DIR : Optional[str]
@@ -13,19 +21,25 @@
         The default window size for processing.
     BAND_NUMBER : int
         The default band number to process in the GeoTIFF file.
     HIGH_VALUE_THRESHOLD : float
         The default high value threshold for categorizing data.
     CATEGORY_THRESHOLDS : Optional[List[float]]
         The default category thresholds for categorizing data. None means no categorization will be applied.
-    NODATA_VALUE : int
+    NO_DATA_VALUE : int
         The default value to use for nodata pixels.
     DTYPE : str
         The default data type for the output data.
+    DEFAULT_CATEGORY_INCREMENT : float
+        The default increment to use when interpolating missing category thresholds.
+    LOG_UPDATE_INTERVAL : int
+        The default interval for updating the log window.
     """
     OUTPUT_DIR: Final[Optional[str]] = None
     WINDOW_SIZE: Final[float] = 1.0
     BAND_NUMBER: Final[int] = 1
     HIGH_VALUE_THRESHOLD: Final[float] = 10.0
     CATEGORY_THRESHOLDS: Final[Optional[List[float]]] = None
-    NODATA_VALUE: Final[int] = -9999
+    NO_DATA_VALUE: Final[int] = -9999
     DTYPE: Final[str] = 'float32'
+    DEFAULT_CATEGORY_INCREMENT: Final[float] = 0.1
+    LOG_UPDATE_INTERVAL: Final[int] = 1000
```

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/classes/geo_tiff_processor.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/classes/geo_tiff_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 geo_tiff_processor.py
 ---------------------
-Version: 1.2.2
+Version: 1.3.0
 Author: Lukas Batschelet
-Date: 11.05.2024
+Date: 14.05.2024
 ---------------------
 This module contains the GeoTIFFProcessor class which is responsible for processing GeoTIFF files.
 It provides methods for loading, processing, and saving GeoTIFF files.
 Until now, only a method to calculate the roughness of a GeoTIFF file has been implemented.
 """
 import logging
 from typing import Optional, List, Tuple
@@ -49,17 +49,20 @@
         self.window_size = params.window_size
         self.band_number = params.band_number
         self.high_value_threshold = params.high_value_threshold
         self.category_thresholds = params.category_thresholds
 
         # Initialize the dataset, processed_data, and profile attributes to None
         self.dataset = None
-        self.processed_data = None
         self.profile = None
 
+        self.processed_data = None
+        self.processed_uncategorized_data = None
+        self.processed_profile = None
+
         logger.info(f"GeoTIFFProcessor initialized with parameters: {params}")
 
     def process_tiff(self) -> np.ndarray:
         """
         Main method for processing the GeoTIFF file.
         Returns the processed data instead of saving it directly.
 
@@ -88,21 +91,30 @@
             # Calculate the roughness of the GeoTIFF file
             processed_data = self.calculate_roughness(data)
             # Apply nodata values to the roughness data
             processed_data = self.apply_nodata(processed_data)
             # Filter out high values from the roughness data
             processed_data = self.apply_filter(processed_data)
 
+            # Store the uncategorized data
+            self.processed_uncategorized_data = processed_data
+
             # If thresholds are defined, apply them to the roughness data
             if self.category_thresholds:
                 processed_data = self.apply_thresholds(processed_data)
             # Store the processed data and the profile of the GeoTIFF file
             self.processed_data = processed_data
             self.profile = self.dataset.profile  # Store profile before closing
 
+            # Create a new profile for the processed data based on the original profile
+            self.processed_profile = self.profile.copy()
+
+            # Update the transform, width, and height in the processed_profile
+            self.update_transform(Defaults.NO_DATA_VALUE, Defaults.DTYPE, self.window_size)
+
             # Return the processed data
             return processed_data
         except Exception as e:
             # Log the error and raise a new error
             logging.error(f"An error occurred during processing: {e}")
             raise RuntimeError(f"An error occurred during processing: {e}")
         finally:
@@ -243,15 +255,15 @@
         try:
             with rasterio.open(self.input_path) as src:
                 logger.info(f"GeoTIFF metadata: {src.meta}")
         except rasterio.errors.RasterioIOError as e:
             logger.error(f"Failed to open GeoTIFF: {e}")
             raise ValueError(f"Invalid GeoTIFF file: {self.input_path}")
 
-    def apply_filter(self, roughness: np.ndarray, nodata_value: int = Defaults.NODATA_VALUE) -> np.ndarray:
+    def apply_filter(self, roughness: np.ndarray, nodata_value: int = Defaults.NO_DATA_VALUE) -> np.ndarray:
         """
         Filters out high values from the roughness array.
 
         This method replaces values in the roughness array that are greater than the high value
         threshold with a nodata value.
 
         Args:
@@ -269,15 +281,15 @@
             raise ValueError("Roughness data is required for filtering.")
 
         roughness[roughness > self.high_value_threshold] = nodata_value
         logging.info("High values filtered from the roughness data.")
 
         return roughness
 
-    def apply_nodata(self, roughness: np.ndarray, nodata_value: int = Defaults.NODATA_VALUE) -> np.ndarray:
+    def apply_nodata(self, roughness: np.ndarray, nodata_value: int = Defaults.NO_DATA_VALUE) -> np.ndarray:
         """
         Applies nodata value and filters out zero values from the roughness array.
 
         This method replaces zero values in the roughness array with a nodata value.
 
         Args:
             roughness (np.ndarray): The roughness array.
@@ -328,15 +340,15 @@
             # Return the pixel size
             return pixel_size
         except AttributeError as e:
             # Log the error and raise the original exception
             logging.error("Error accessing transform of the dataset: " + str(e))
             raise
 
-    def apply_thresholds(self, data: np.ndarray, nodata_value: int = Defaults.NODATA_VALUE) -> np.ndarray:
+    def apply_thresholds(self, data: np.ndarray, nodata_value: int = Defaults.NO_DATA_VALUE) -> np.ndarray:
         """
         Applies thresholds to the data array.
 
         This method replaces values in the data array that are within certain ranges defined by the category thresholds
         with the corresponding category number. Values greater than or equal to the highest threshold and less than or
         equal to the high value threshold are replaced with the highest category number.
 
@@ -378,7 +390,20 @@
         # Create a mask for values within the high value range
         high_value_mask = (data >= self.category_thresholds[-1]) & (data <= self.high_value_threshold) & valid_mask
         # Replace values within the high value range with the highest category number
         categorized_data[high_value_mask] = len(self.category_thresholds)
 
         logging.info("Data categorized based on thresholds.")
         return categorized_data
+
+    def update_transform(self, nodata: int, dtype: str, pixel_size: float):
+        # Update the profile with the provided data type and nodata value
+        self.processed_profile.update(dtype=dtype, nodata=nodata)
+
+        # Calculate the new width and height based on the window size
+        width = int((self.processed_profile['width'] * self.processed_profile['transform'][0]) / pixel_size)
+        height = int((self.processed_profile['height'] * abs(self.processed_profile['transform'][4])) / pixel_size)
+
+        # Update the transform, width, and height in the processed_profile
+        self.processed_profile['transform'] = rasterio.Affine(pixel_size, 0, self.processed_profile['transform'][2], 0, -pixel_size, self.processed_profile['transform'][5])
+        self.processed_profile['width'] = width
+        self.processed_profile['height'] = height
```

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/classes/processing_parameters.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/classes/processing_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 processing_parameters.py
 ---
-Version: 1.2.2
+Version: 1.3.0
 Author: Lukas Batschelet
-Date: 11.05.2024
+Date: 14.05.2024
 ---
 Class to encapsulate the processing parameters for the surface roughness calculator application.
 The used dataclass decorator is a Python 3.7 feature that allows for the creation of classes with
 attributes and methods without the need for boilerplate code. The dataclass decorator automatically
 generates special methods like __init__(), __repr__(), and __eq__() based on the attributes defined
 in the class.
 """
```

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/cli_main.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/cli_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 cli_main.py
 -----------
-Version: 1.2.2
+Version: 1.3.0
 Author: Lukas Batschelet
-Date: 11.05.2024
+Date: 14.05.2024
 -----------
 """
 import argparse
 import logging
 import sys
 
 from roughness_calculator.classes.application_driver import ApplicationDriver
```

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/gui/encapsulating_frame.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/gui/encapsulating_frame.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/gui/header_frame.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/gui/header_frame.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/gui/parameter_input.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/gui/parameter_input.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tkinter as tk
 
 import customtkinter as ctk
 
+from roughness_calculator.gui.analyze_and_optimize import AnalyzeAndOptimizeFrame
 from roughness_calculator.gui.defaults import DEFAULTS
 
 
 class ParameterFrame(ctk.CTkFrame):
     def __init__(self, parent, main_gui, **kwargs):
         super().__init__(parent, **kwargs)
 
@@ -56,36 +57,74 @@
                            self.main_gui))
         self.high_value_threshold_field.grid(row=1,
                                              column=1,
                                              padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX),
                                              pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
                                              sticky="nsew")
 
+        # Create a new frame for the buttons
+        self.button_frame = ctk.CTkFrame(self)
+        self.button_frame.grid(row=2,
+                               column=0,
+                               columnspan=2,
+                               padx=DEFAULTS.PADX,
+                               pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY),
+                               sticky="ew")
+        # Set equal weights for each column in the button frame
+        self.button_frame.grid_columnconfigure([0, 1, 2], weight=1)
+
         self.start_processing_button = (
-            ctk.CTkButton(self, text="Start Processing", command=self.main_gui.start_processing))
-        self.start_processing_button.grid(row=2,
+            ctk.CTkButton(self.button_frame, text="Start Processing", command=self.main_gui.start_processing))
+        self.start_processing_button.grid(row=0,
                                           column=0,
                                           padx=(DEFAULTS.PADX, DEFAULTS.PADX * 0.5),
-                                          pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY),
-                                          sticky="ew")  # Place the button in the new row
+                                          pady=DEFAULTS.PADY,
+                                          sticky="ew")
+
+        # Create a new button
+        self.analyze_and_optimize_button = ctk.CTkButton(self.button_frame,
+                                                         text="Analyze and optimize...",
+                                                         command=self.toggle_frame, state=tk.DISABLED)
+        self.analyze_and_optimize_button.grid(row=0,
+                                              column=1,
+                                              padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
+                                              pady=DEFAULTS.PADY,
+                                              sticky="ew")
 
         self.save_file_button = (
-            ctk.CTkButton(self, text="Save File", command=self.main_gui.save_image, state=tk.DISABLED))
-        self.save_file_button.grid(row=2,
-                                   column=1,
-                                   padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX),
-                                   pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY),
-                                   sticky="ew")  # Place the button in the new row
+            ctk.CTkButton(self.button_frame, text="Save File", command=self.main_gui.save_image, state=tk.DISABLED))
+        self.save_file_button.grid(row=0,
+                                   column=2,
+                                   padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
+                                   pady=DEFAULTS.PADY,
+                                   sticky="ew")
+
+        # Create a new frame and initially hide it
+        self.analyze_and_optimize_frame = AnalyzeAndOptimizeFrame(self, main_gui)
+        self.analyze_and_optimize_frame.grid(row=3,
+                                             column=0,
+                                             columnspan=3,
+                                             padx=DEFAULTS.PADX,
+                                             pady=(0, DEFAULTS.PADY),
+                                             sticky="ew")
+        self.analyze_and_optimize_frame.grid_remove()
+
+    def toggle_frame(self):
+        if self.analyze_and_optimize_frame.winfo_viewable():
+            self.analyze_and_optimize_frame.grid_remove()
+        else:
+            self.analyze_and_optimize_frame.grid()
 
     def get_parameters(self):
         return {
             "window_size": self.window_size_field.get() or None,
             "category_thresholds": self.category_thresholds_field.get() or None,
             "band_number": self.band_number_field.get() or None,
-            "high_value_threshold": self.high_value_threshold_field.get() or None
+            "high_value_threshold": self.high_value_threshold_field.get() or None,
+            "control_input_path": self.analyze_and_optimize_frame.control_input_path_field.get() or None
         }
 
 
 class DescriptionField(ctk.CTkLabel):
     def __init__(self, parent, text, **kwargs):
         super().__init__(parent, text=text, **kwargs)
```

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/gui/path_frame.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/gui/preview_image.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.2/roughness_calculator/log_config.py` & `dem_roughness_calculator-1.3.0/roughness_calculator/log_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 log_config.py
 -----------
-Version: 1.2.2
+Version: 1.3.0
 Author: Lukas Batschelet
-Date: 11.05.2024
+Date: 14.05.2024
 -----------
 This module sets up the logging for the application.
 """
 
 import logging
 import os
```

### Comparing `dem_roughness_calculator-1.2.2/setup.py` & `dem_roughness_calculator-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='dem-roughness-calculator',
-    version='1.2.2',
+    version='1.3.0',
     packages=find_packages(),  # Automatically find all packages in the directory
     url='https://github.com/lbatschelet/dem-roughness-calculator',
     license='GPL-3.0',
     author='lbatschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     install_requires=requirements,  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
```

