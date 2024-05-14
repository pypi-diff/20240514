# Comparing `tmp/riversand-1.2.5.tar.gz` & `tmp/riversand-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riversand-1.2.5.tar", last modified: Tue May 14 11:27:20 2024, max compression
+gzip compressed data, was "riversand-1.2.6.tar", last modified: Tue May 14 12:50:36 2024, max compression
```

## Comparing `riversand-1.2.5.tar` & `riversand-1.2.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-14 11:27:20.985306 riversand-1.2.5/
--rw-rw-r--   0 user      (1001) user      (1001)    35150 2023-02-25 18:17:07.000000 riversand-1.2.5/LICENSE
--rw-r--r--   0 user      (1001) user      (1001)     3897 2024-05-14 11:27:20.985306 riversand-1.2.5/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)     2973 2024-05-14 11:24:56.000000 riversand-1.2.5/README.md
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-14 11:27:20.985306 riversand-1.2.5/riversand/
--rw-rw-r--   0 user      (1001) user      (1001)      739 2024-05-10 17:59:33.000000 riversand-1.2.5/riversand/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)      220 2024-05-14 11:25:25.000000 riversand-1.2.5/riversand/_version.py
--rw-rw-r--   0 user      (1001) user      (1001)    35160 2024-05-12 15:25:43.000000 riversand-1.2.5/riversand/calc.py
--rw-rw-r--   0 user      (1001) user      (1001)    69209 2024-05-12 15:20:42.000000 riversand-1.2.5/riversand/geospatial.py
--rw-rw-r--   0 user      (1001) user      (1001)     4150 2024-05-10 16:12:46.000000 riversand-1.2.5/riversand/params.py
--rw-rw-r--   0 user      (1001) user      (1001)    11378 2024-02-28 08:29:04.000000 riversand-1.2.5/riversand/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)    51865 2024-05-14 11:25:52.000000 riversand-1.2.5/riversand/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)    16086 2024-05-10 20:13:34.000000 riversand-1.2.5/riversand/xml.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-14 11:27:20.985306 riversand-1.2.5/riversand.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     3897 2024-05-14 11:27:20.000000 riversand-1.2.5/riversand.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      360 2024-05-14 11:27:20.000000 riversand-1.2.5/riversand.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-05-14 11:27:20.000000 riversand-1.2.5/riversand.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       59 2024-05-14 11:27:20.000000 riversand-1.2.5/riversand.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       10 2024-05-14 11:27:20.000000 riversand-1.2.5/riversand.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2024-05-14 11:27:20.985306 riversand-1.2.5/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     1269 2024-05-14 11:25:16.000000 riversand-1.2.5/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-14 12:50:36.015655 riversand-1.2.6/
+-rw-rw-r--   0 user      (1001) user      (1001)    35150 2023-02-25 18:17:07.000000 riversand-1.2.6/LICENSE
+-rw-r--r--   0 user      (1001) user      (1001)     3897 2024-05-14 12:50:36.015655 riversand-1.2.6/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)     2973 2024-05-14 12:49:55.000000 riversand-1.2.6/README.md
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-14 12:50:36.015655 riversand-1.2.6/riversand/
+-rw-rw-r--   0 user      (1001) user      (1001)      739 2024-05-10 17:59:33.000000 riversand-1.2.6/riversand/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)      220 2024-05-14 12:49:37.000000 riversand-1.2.6/riversand/_version.py
+-rw-rw-r--   0 user      (1001) user      (1001)    35160 2024-05-12 15:25:43.000000 riversand-1.2.6/riversand/calc.py
+-rw-rw-r--   0 user      (1001) user      (1001)    68709 2024-05-14 12:47:18.000000 riversand-1.2.6/riversand/geospatial.py
+-rw-rw-r--   0 user      (1001) user      (1001)     4150 2024-05-10 16:12:46.000000 riversand-1.2.6/riversand/params.py
+-rw-rw-r--   0 user      (1001) user      (1001)    11378 2024-02-28 08:29:04.000000 riversand-1.2.6/riversand/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    51865 2024-05-14 11:25:52.000000 riversand-1.2.6/riversand/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)    16086 2024-05-10 20:13:34.000000 riversand-1.2.6/riversand/xml.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-05-14 12:50:36.015655 riversand-1.2.6/riversand.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3897 2024-05-14 12:50:36.000000 riversand-1.2.6/riversand.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      350 2024-05-14 12:50:36.000000 riversand-1.2.6/riversand.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2024-05-14 12:50:36.000000 riversand-1.2.6/riversand.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       59 2024-05-14 12:50:36.000000 riversand-1.2.6/riversand.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       10 2024-05-14 12:50:36.000000 riversand-1.2.6/riversand.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2024-05-14 12:50:36.015655 riversand-1.2.6/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     1269 2024-05-14 12:49:25.000000 riversand-1.2.6/setup.py
```

### Comparing `riversand-1.2.5/LICENSE` & `riversand-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `riversand-1.2.5/PKG-INFO` & `riversand-1.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riversand
-Version: 1.2.5
+Version: 1.2.6
 Summary: Catchmentwide erosion rate calculator
 Home-page: https://github.com/kstueb/riversand
 Author: Konstanze Stuebner
 Author-email: kstueb@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -56,16 +56,16 @@
 Definitely check out the documentation of the online calculator (e.g. [here](http://stoneage.ice-d.org/math/docs/v3/v3_input_explained.html)
 or [here](https://sites.google.com/a/bgc.org/v3docs/)) and the publication
 [Balco et al. (2008)](http://hess.ess.washington.edu/math/docs/al_be_v2/al_be_calc_2007.pdf)
 before using this calculator.
 
 Documentation
 -------------
-- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/quickstart_v1.2.5.ipynb)
-- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/step_by_step_v1.2.5.ipynb)
+- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/quickstart_v1.2.6.ipynb)
+- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/step_by_step_v1.2.6.ipynb)
 - [`test_data/`](https://github.com/kstueb/riversand/blob/main/example_scripts/test_data) : geotiffs of a 35m-resolution digital elevation model, a topographic shielding raster generated with [TopoToolbox](https://topotoolbox.wordpress.com/) and a binary raster indicating quartz-bearing and quartz-free lithologies; shapefiles with catchment outlines; a spreadsheet with sample data. 
 
 Installation
 ------------
 Install riversand by running:
 ```
 $ pip install riversand
```

### Comparing `riversand-1.2.5/README.md` & `riversand-1.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 Definitely check out the documentation of the online calculator (e.g. [here](http://stoneage.ice-d.org/math/docs/v3/v3_input_explained.html)
 or [here](https://sites.google.com/a/bgc.org/v3docs/)) and the publication
 [Balco et al. (2008)](http://hess.ess.washington.edu/math/docs/al_be_v2/al_be_calc_2007.pdf)
 before using this calculator.
 
 Documentation
 -------------
-- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/quickstart_v1.2.5.ipynb)
-- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/step_by_step_v1.2.5.ipynb)
+- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/quickstart_v1.2.6.ipynb)
+- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/step_by_step_v1.2.6.ipynb)
 - [`test_data/`](https://github.com/kstueb/riversand/blob/main/example_scripts/test_data) : geotiffs of a 35m-resolution digital elevation model, a topographic shielding raster generated with [TopoToolbox](https://topotoolbox.wordpress.com/) and a binary raster indicating quartz-bearing and quartz-free lithologies; shapefiles with catchment outlines; a spreadsheet with sample data. 
 
 Installation
 ------------
 Install riversand by running:
 ```
 $ pip install riversand
```

### Comparing `riversand-1.2.5/riversand/__init__.py` & `riversand-1.2.6/riversand/__init__.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.5/riversand/calc.py` & `riversand-1.2.6/riversand/calc.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.5/riversand/geospatial.py` & `riversand-1.2.6/riversand/geospatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -549,42 +549,25 @@
                             
         if self.path_to_data is not None:
             fname = os.path.join(self.path_to_data, fname)
             
         df = pd.DataFrame()
         
         try:
-            df = pd.read_csv(fname)
+            df = pd.read_csv(fname, sep=None, engine='python') # python engine automatically detects separator
             
-            # I believe this is only needed for csv files
-            for c in df.columns:
-                try:
-                    df[c] = df[c].str.strip(' \n\t')
-                except:
-                    pass
         except:
             try:
-                xls = pd.ExcelFile(fname)
-            except ImportError as e:
-                raise e
-            except IOError as e:
-                if e.errno==2:
-                    raise FileNotFoundError("{}: No such file or directory"
-                                            .format(e.filename))
-                else:
-                    raise e
-            else:
-                df = xls.parse(0) # imports the first sheet no matter the name
-    
-        for c in df.columns:
-            c_new = c.strip(' \n\t')
-            df.rename(columns={c: c_new}, inplace=True)
+                df = pd.read_excel(fname) # imports the first sheet no matter the name
+            except:
+                #print("Failing to read input as csv or excel file.")
+                pass
         
         if df.empty:
-            raise ValueError("No sample data in file")
+            raise ValueError("Failing to read file / no sample data in file")
         
         # sorting as in Params.all_keys w/o topographic and other info at end 
         topo_keys = ['lat', 'latitude', 'lon', 'long', 'longitude', 'elev', 'elevation']
         mandatory_keys = [k for k in Params.all_keys if k not in topo_keys]
         other_keys = [k for k in topo_keys if k in df.keys()] # additional topographic info
         other_keys += [k for k in df.keys() if k not in Params.all_keys] # additional other
```

### Comparing `riversand-1.2.5/riversand/params.py` & `riversand-1.2.6/riversand/params.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.5/riversand/plot.py` & `riversand-1.2.6/riversand/plot.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.5/riversand/utils.py` & `riversand-1.2.6/riversand/utils.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.5/riversand/xml.py` & `riversand-1.2.6/riversand/xml.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.5/riversand.egg-info/PKG-INFO` & `riversand-1.2.6/riversand.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riversand
-Version: 1.2.5
+Version: 1.2.6
 Summary: Catchmentwide erosion rate calculator
 Home-page: https://github.com/kstueb/riversand
 Author: Konstanze Stuebner
 Author-email: kstueb@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -56,16 +56,16 @@
 Definitely check out the documentation of the online calculator (e.g. [here](http://stoneage.ice-d.org/math/docs/v3/v3_input_explained.html)
 or [here](https://sites.google.com/a/bgc.org/v3docs/)) and the publication
 [Balco et al. (2008)](http://hess.ess.washington.edu/math/docs/al_be_v2/al_be_calc_2007.pdf)
 before using this calculator.
 
 Documentation
 -------------
-- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/quickstart_v1.2.5.ipynb)
-- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/step_by_step_v1.2.5.ipynb)
+- [`quickstart.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/quickstart_v1.2.6.ipynb)
+- [`step_by_step.ipynb`](https://github.com/kstueb/riversand/blob/main/example_scripts/step_by_step_v1.2.6.ipynb)
 - [`test_data/`](https://github.com/kstueb/riversand/blob/main/example_scripts/test_data) : geotiffs of a 35m-resolution digital elevation model, a topographic shielding raster generated with [TopoToolbox](https://topotoolbox.wordpress.com/) and a binary raster indicating quartz-bearing and quartz-free lithologies; shapefiles with catchment outlines; a spreadsheet with sample data. 
 
 Installation
 ------------
 Install riversand by running:
 ```
 $ pip install riversand
```

### Comparing `riversand-1.2.5/setup.py` & `riversand-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup   
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()   
 setup(                                
    name = 'riversand',
-   version = '1.2.5',
+   version = '1.2.6',
    packages = ['riversand'],
    author = 'Konstanze Stuebner',
    author_email = 'kstueb@gmail.com',
    url = 'https://github.com/kstueb/riversand',
    description = 'Catchmentwide erosion rate calculator',
    classifiers = ["Programming Language :: Python",
                   "Programming Language :: Python :: 3",
```

