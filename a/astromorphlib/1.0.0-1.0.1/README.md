# Comparing `tmp/astromorphlib-1.0.0.tar.gz` & `tmp/astromorphlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/joseaher/Dropbox/work/prog/packages_astromorphlib/dist/.tmp-4__lf6fw/astromorphlib-1.0.0.tar", last modified: Fri May 10 22:03:40 2024, max compression
+gzip compressed data, was "/home/joseaher/Dropbox/work/prog/packages_astromorphlib/dist/.tmp-dajen9jk/astromorphlib-1.0.1.tar", last modified: Mon May 13 23:55:24 2024, max compression
```

## Comparing `astromorphlib-1.0.0.tar` & `astromorphlib-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-10 22:03:40.417747 astromorphlib-1.0.0/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      399 2022-04-05 21:26:30.000000 astromorphlib-1.0.0/LICENSE.txt
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      236 2023-11-07 17:33:39.000000 astromorphlib-1.0.0/MANIFEST.in
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)     4355 2024-05-10 22:03:40.417747 astromorphlib-1.0.0/PKG-INFO
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)     4030 2024-05-10 21:55:52.000000 astromorphlib-1.0.0/README.md
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-10 22:03:40.417747 astromorphlib-1.0.0/astromorphlib.egg-info/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)     4355 2024-05-10 22:03:40.000000 astromorphlib-1.0.0/astromorphlib.egg-info/PKG-INFO
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      797 2024-05-10 22:03:40.000000 astromorphlib-1.0.0/astromorphlib.egg-info/SOURCES.txt
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)        1 2024-05-10 22:03:40.000000 astromorphlib-1.0.0/astromorphlib.egg-info/dependency_links.txt
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)        9 2024-05-10 22:03:40.000000 astromorphlib-1.0.0/astromorphlib.egg-info/top_level.txt
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-10 22:03:40.405747 astromorphlib-1.0.0/docs/
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)      634 2023-11-07 00:45:50.000000 astromorphlib-1.0.0/docs/Makefile
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-10 22:03:40.405747 astromorphlib-1.0.0/docs/_static/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)    17104 2023-11-01 11:16:11.000000 astromorphlib-1.0.0/docs/_static/logo.png
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     1248 2023-11-07 05:43:09.000000 astromorphlib-1.0.0/docs/conf.py
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      107 2023-11-07 03:20:16.000000 astromorphlib-1.0.0/docs/examples.rst
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     4866 2024-05-10 22:01:50.000000 astromorphlib-1.0.0/docs/index.rst
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      956 2024-03-11 20:27:29.000000 astromorphlib-1.0.0/docs/installation.rst
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)      800 2023-11-07 00:45:50.000000 astromorphlib-1.0.0/docs/make.bat
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-10 22:03:40.409747 astromorphlib-1.0.0/docs/notebooks/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)   951121 2024-01-10 21:52:53.000000 astromorphlib-1.0.0/docs/notebooks/Enviroment-search.ipynb
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)  3001950 2024-03-01 22:52:12.000000 astromorphlib-1.0.0/docs/notebooks/fitting.ipynb
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     1552 2024-03-01 22:50:48.000000 astromorphlib-1.0.0/docs/notebooks/properties.dat
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)       92 2024-03-01 22:29:13.000000 astromorphlib-1.0.0/docs/notebooks/simbad_table.tab
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)  5411368 2024-03-01 22:37:46.000000 astromorphlib-1.0.0/docs/notebooks/testing.ipynb
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      106 2024-01-10 15:35:03.000000 astromorphlib-1.0.0/docs/parameters.rst
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)       30 2023-11-07 02:56:02.000000 astromorphlib-1.0.0/docs/requirements.txt
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)       38 2024-05-10 22:03:40.417747 astromorphlib-1.0.0/setup.cfg
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      773 2024-05-10 21:43:37.000000 astromorphlib-1.0.0/setup.py
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-10 22:03:40.413747 astromorphlib-1.0.0/stat_lib/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)   294972 2022-05-01 21:05:42.000000 astromorphlib-1.0.0/stat_lib/Table_Arp_Madore_pairs_updated.txt
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)   158723 2024-05-10 19:06:06.000000 astromorphlib-1.0.0/stat_lib/__init__.py
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)    90209 2022-10-31 23:13:27.000000 astromorphlib-1.0.0/stat_lib/__init__old.py
-drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-10 22:03:40.417747 astromorphlib-1.0.0/stat_lib/__pycache__/
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)    86949 2024-02-28 16:45:37.000000 astromorphlib-1.0.0/stat_lib/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)    20743 2024-01-10 20:33:45.000000 astromorphlib-1.0.0/stat_lib/__pycache__/stat_lib.cpython-38.pyc
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)   156205 2023-07-11 18:48:15.000000 astromorphlib-1.0.0/stat_lib/iDR4_obs_seeing.csv
--rw-rw-r--   0 joseaher  (1000) joseaher  (1000)   175683 2023-07-11 18:47:07.000000 astromorphlib-1.0.0/stat_lib/iDR4_zero-points.csv
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)      682 2024-03-01 22:47:29.000000 astromorphlib-1.0.0/stat_lib/properties.dat
--rw-r--r--   0 joseaher  (1000) joseaher  (1000)   106560 2022-04-05 22:04:36.000000 astromorphlib-1.0.0/stat_lib/zero_points.fits
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-13 23:55:24.327331 astromorphlib-1.0.1/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      399 2022-04-05 21:26:30.000000 astromorphlib-1.0.1/LICENSE.txt
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      236 2023-11-07 17:33:39.000000 astromorphlib-1.0.1/MANIFEST.in
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)     4355 2024-05-13 23:55:24.327331 astromorphlib-1.0.1/PKG-INFO
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)     4030 2024-05-10 21:55:52.000000 astromorphlib-1.0.1/README.md
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-13 23:55:24.327331 astromorphlib-1.0.1/astromorphlib.egg-info/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)     4355 2024-05-13 23:55:24.000000 astromorphlib-1.0.1/astromorphlib.egg-info/PKG-INFO
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      797 2024-05-13 23:55:24.000000 astromorphlib-1.0.1/astromorphlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)        1 2024-05-13 23:55:24.000000 astromorphlib-1.0.1/astromorphlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)        9 2024-05-13 23:55:24.000000 astromorphlib-1.0.1/astromorphlib.egg-info/top_level.txt
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-13 23:55:24.307331 astromorphlib-1.0.1/docs/
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)      634 2023-11-07 00:45:50.000000 astromorphlib-1.0.1/docs/Makefile
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-13 23:55:24.307331 astromorphlib-1.0.1/docs/_static/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)    17104 2023-11-01 11:16:11.000000 astromorphlib-1.0.1/docs/_static/logo.png
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     1248 2023-11-07 05:43:09.000000 astromorphlib-1.0.1/docs/conf.py
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      107 2023-11-07 03:20:16.000000 astromorphlib-1.0.1/docs/examples.rst
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     4866 2024-05-10 22:01:50.000000 astromorphlib-1.0.1/docs/index.rst
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      956 2024-03-11 20:27:29.000000 astromorphlib-1.0.1/docs/installation.rst
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)      800 2023-11-07 00:45:50.000000 astromorphlib-1.0.1/docs/make.bat
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-13 23:55:24.311331 astromorphlib-1.0.1/docs/notebooks/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)   951121 2024-01-10 21:52:53.000000 astromorphlib-1.0.1/docs/notebooks/Enviroment-search.ipynb
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)  3001950 2024-03-01 22:52:12.000000 astromorphlib-1.0.1/docs/notebooks/fitting.ipynb
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)     1552 2024-03-01 22:50:48.000000 astromorphlib-1.0.1/docs/notebooks/properties.dat
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)       92 2024-03-01 22:29:13.000000 astromorphlib-1.0.1/docs/notebooks/simbad_table.tab
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)  5411368 2024-03-01 22:37:46.000000 astromorphlib-1.0.1/docs/notebooks/testing.ipynb
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      106 2024-01-10 15:35:03.000000 astromorphlib-1.0.1/docs/parameters.rst
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)       30 2023-11-07 02:56:02.000000 astromorphlib-1.0.1/docs/requirements.txt
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)       38 2024-05-13 23:55:24.327331 astromorphlib-1.0.1/setup.cfg
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      773 2024-05-13 23:51:11.000000 astromorphlib-1.0.1/setup.py
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-13 23:55:24.327331 astromorphlib-1.0.1/stat_lib/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)   294972 2022-05-01 21:05:42.000000 astromorphlib-1.0.1/stat_lib/Table_Arp_Madore_pairs_updated.txt
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)   155112 2024-05-13 23:42:23.000000 astromorphlib-1.0.1/stat_lib/__init__.py
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)    90209 2022-10-31 23:13:27.000000 astromorphlib-1.0.1/stat_lib/__init__old.py
+drwxrwxr-x   0 joseaher  (1000) joseaher  (1000)        0 2024-05-13 23:55:24.327331 astromorphlib-1.0.1/stat_lib/__pycache__/
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)    86949 2024-02-28 16:45:37.000000 astromorphlib-1.0.1/stat_lib/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)    20743 2024-01-10 20:33:45.000000 astromorphlib-1.0.1/stat_lib/__pycache__/stat_lib.cpython-38.pyc
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)   156205 2023-07-11 18:48:15.000000 astromorphlib-1.0.1/stat_lib/iDR4_obs_seeing.csv
+-rw-rw-r--   0 joseaher  (1000) joseaher  (1000)   175683 2023-07-11 18:47:07.000000 astromorphlib-1.0.1/stat_lib/iDR4_zero-points.csv
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)      682 2024-03-01 22:47:29.000000 astromorphlib-1.0.1/stat_lib/properties.dat
+-rw-r--r--   0 joseaher  (1000) joseaher  (1000)   106560 2022-04-05 22:04:36.000000 astromorphlib-1.0.1/stat_lib/zero_points.fits
```

### Comparing `astromorphlib-1.0.0/PKG-INFO` & `astromorphlib-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromorphlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python scripts to analyze the morphology of isolated/interacting galaxies
 Home-page: https://gitlab.com/joseaher/astromorphlib
 Author: J. A. Hernandez-Jimenez
 Author-email: joseaher@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `astromorphlib-1.0.0/README.md` & `astromorphlib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/astromorphlib.egg-info/PKG-INFO` & `astromorphlib-1.0.1/astromorphlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromorphlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python scripts to analyze the morphology of isolated/interacting galaxies
 Home-page: https://gitlab.com/joseaher/astromorphlib
 Author: J. A. Hernandez-Jimenez
 Author-email: joseaher@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `astromorphlib-1.0.0/astromorphlib.egg-info/SOURCES.txt` & `astromorphlib-1.0.1/astromorphlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/Makefile` & `astromorphlib-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/_static/logo.png` & `astromorphlib-1.0.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/conf.py` & `astromorphlib-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/index.rst` & `astromorphlib-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/installation.rst` & `astromorphlib-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/make.bat` & `astromorphlib-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/notebooks/Enviroment-search.ipynb` & `astromorphlib-1.0.1/docs/notebooks/Enviroment-search.ipynb`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/notebooks/fitting.ipynb` & `astromorphlib-1.0.1/docs/notebooks/fitting.ipynb`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/notebooks/properties.dat` & `astromorphlib-1.0.1/docs/notebooks/properties.dat`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/docs/notebooks/testing.ipynb` & `astromorphlib-1.0.1/docs/notebooks/testing.ipynb`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/setup.py` & `astromorphlib-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='astromorphlib',
-      version='1.0.0',
+      version='1.0.1',
       description='Python scripts to analyze the morphology of isolated/interacting galaxies',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='J. A. Hernandez-Jimenez',
       author_email='joseaher@gmail.com',
       url = "https://gitlab.com/joseaher/astromorphlib",
       packages=['stat_lib'],
```

### Comparing `astromorphlib-1.0.0/stat_lib/Table_Arp_Madore_pairs_updated.txt` & `astromorphlib-1.0.1/stat_lib/Table_Arp_Madore_pairs_updated.txt`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/stat_lib/__init__.py` & `astromorphlib-1.0.1/stat_lib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1293,19 +1293,19 @@
     simbad_table = simbad.Simbad.query_object(gal)
     if bool(simbad_table) is False:
         print ("\nthe target was not found, please double-checking" +
                  "the target name")
         return
 
     if not os.path.exists('simbad_table.tab'):
-        simbad_table['MAIN_ID'] = gal
-        tab_gal = Table((gal,
-                      simbad_table['RA_d'][0], simbad_table['DEC_d'][0],
-                      simbad_table['RV_VALUE'][0], simbad_table['Z_VALUE'][0],
-                      simbad_table['FLUX_B'][0]),
+        simbad_table['MAIN_ID'][0] = gal
+        tab_gal = Table((simbad_table['MAIN_ID'],
+                         simbad_table['RA_d'], simbad_table['DEC_d'],
+                         simbad_table['RV_VALUE'], simbad_table['Z_VALUE'],
+        simbad_table['FLUX_B']),
                       names=('gal','ra','dec','vel','z', 'mag'))
         tab_gal.write('simbad_table.tab', format='ascii')
         idg=0
     else:
         tab_gal = Table.read('simbad_table.tab', format='ascii')
         if any(tab_gal['gal'] == gal):
             idg=np.where(tab_gal['gal']==gal)[0][0]
@@ -1721,21 +1721,21 @@
         print ("sep_kpc = sep.arcsec*arc_kpc")
         print ("print ('Separation between a Secondary and Primary" +
                " $\\sim$ {:.1f}\\,kpc ({:.1f}$\\\\arcsec$)'.format(sep_kpc, sep.arcsec))")
 
 def simbad_thumbnail(GAL, tab_gal='simbad', size_image_phy=100,
                      limtvel=500,  ned_plot='no', width = 300, height = 300,
                      labeltxt = 'off', xtpos=10, ytpos=20, deltay=10, miny=20,
-                     minx=20):
+                     minx=20, search_cone=2/3600., show_plot='yes'):
     """
     Perform query in simbad database looking for neiborgh galaxies.
 
     Parameters:
     ------------
-    - gal: Galaxy name (str type).
+    - gal: Galaxy name (str type) or an array [ra, dec] deg.
     - tab_gal: Input table (pandas DataFrame or equivalent) or "simbad" to
                download the galaxy data from Simbad database.
     - size_image_phy: Physical size of the image in kpc unit (default: 50).
     - limtvel: Maximum delta velocity limit (km/s) of the radial velocity for
                the companion  galaxies (default: 500).
     - ned_plot: Perform the same query in NED database (default: 'no')
     - width: Image width in pix (default: 300).
@@ -1745,53 +1745,43 @@
     - ytpos: Y-coordinate position in pix for label object offset (default: 20).
     - deltay: Delta Y-position for labels of object with close X-coordinates
               (default: 10).
     - miny: Minimum separation in Y-coordinates for activate the deltay
             (default: 20).
     - minx: Minimum separation in X-coordinates for activate the deltay
             (default: 20).
+    - search_cone: region size of query region to get the object information
+                   in arcsec (default: 2/3600).
+    - show_plot: Display plots ('yes' or 'no', default: 'yes').
 
     Returns:
     --------
-    None
+    The Simbad table of the fetched objects
     """
 
     ######################
     # Loading the galaxy #
     ######################
 
-    print (Fore.BLUE +"\nBasic information:")
-    print (Fore.BLUE +"-------------------")
-    if isinstance(tab_gal, str):
-        simbad_table = simbad.Simbad.query_object(GAL)
-        if bool(simbad_table) is False:
-            print ("\nthe target was not found, please double-checking" +
-                    "the target name")
-            return
-
-        galvel = simbad_table['RV_VALUE'].value[0]
 
-        print(Fore.BLUE +'Galaxy Name: {} '.format(GAL))
-        print(Fore.BLUE +'MAIN_ID: {} '.format(simbad_table['MAIN_ID'].value[0]))
-
-        simbad_table['MAIN_ID'] = GAL
-        tab_gal = Table((simbad_table['MAIN_ID'],
-                         simbad_table['DEC_d'], simbad_table['RA_d'],
-                         simbad_table['RV_VALUE'], simbad_table['Z_VALUE']),
-                         names=('gal','dec','ra','vel','z'))
-        idg=0
+    if isinstance(tab_gal, str):
+        if tab_gal == 'simbad':
+            GAL, tab_gal, idg = simbad_gal (GAL, search_cone=search_cone)
+        else:
+            GAL, tab_gal, idg = ned_gal (GAL, search_cone=search_cone)
     else:
         idg =np.where(tab_gal['gal']==GAL)[0][0]
-        galvel = tab_gal['vel'][idg]
-
-        print(Fore.BLUE +'Galaxy Name: {} '.format(gal))
 
+    galvel = tab_gal['vel'][idg]
     D = galvel/H
     kpc_arc = np.tan(np.deg2rad(1./3600))*D*1e3
 
+
+    print (Fore.BLUE +"\nBasic information:")
+    print (Fore.BLUE +"-------------------")
     print(Fore.BLUE +'RA  = {} '.format(tab_gal['ra'][idg]))
     print(Fore.BLUE +'DEC = {} '.format(tab_gal['dec'][idg]))
     print(Fore.BLUE +'Rad Vel = {:.1f} km/s'.format(galvel))
     print(Fore.BLUE +'Distance = {:.1f} Mpc\n'.format(D))
 
     arcdist = (size_image_phy*2)/kpc_arc
     fov = arcdist/3600.
@@ -1810,15 +1800,15 @@
     hdu = fits.open('fits_images/{}_simbad_{}kpc.fits'.format(GAL,
                     size_image_phy))
     ima_simbad = plt.imread('images/{}_simbad_{}kpc.png'.format(GAL,
                             size_image_phy))
 
     # Downloading  Simbad Table
     print (Fore.BLACK + "\n------------------------\n")
-    table=simbad_cat(GAL, tab_gal, size_image_phy, region='circle',
+    table = simbad_cat(GAL, tab_gal, size_image_phy, region='circle',
                      limtvel=limtvel, server=None)
     table = table[table['RV_VALUE']>0]
 
     galcoord = SkyCoord(ra*u.deg, dec*u.deg)
     skyc=SkyCoord(table['RA_d'], table['DEC_d'])
     sep = galcoord.separation(skyc)
 
@@ -1830,16 +1820,14 @@
     for i in np.arange(len(skyc)):
 
         txt = "Proyected distance "
         print (txt+"{} and ({}) {} ({} km/s) is = {:.1f}\\,kpc ({:.1f}$\\arcsec$)".format(
         GAL, i, table['MAIN_ID'][i], table['RV_VALUE'][i], sep_kpc[i],
         sep.arcsec[i]))
 
-
-
     if ned_plot == 'yes':
         plt.figure(figsize=(20,10))
         plt.subplot(121)
     else:
         plt.figure(figsize=(10,10))
         plt.subplot(111)
     plt.imshow(ima_simbad, extent=np.array([-1,1,-1,1])*size_image_phy)
@@ -1962,14 +1950,21 @@
 
     plt.xlabel('x (kpc)')
     plt.ylabel('y (kpc)')
     plt.minorticks_on()
     plt.savefig('images/{}_simbad_{}kpc_markers.png'.format(GAL, size_image_phy),
                 bbox_inches='tight')
 
+    if show_plot=='yes':
+        plt.show()
+    else:
+        plt.close()
+
+    return table
+
 def decals_mass(gal, tab_gal, size_image_phy, outputfile='properties.dat',
                 suf_num=-1, show_plot='yes', dr=8, pathg = 'fits_images/'):
 
     import functions as func
     try:
         idg =np.where(tab_gal['gal']==gal)[0][0]
     except:
@@ -2464,25 +2459,27 @@
                  roundhi=0.2, sharplo=0.2, aper_stars=5, aper_center=10,
                  segmap=None, eta=0.2, petro_extent_cas=1.5,
                  flag_area_th=3, flag_SN_th=3, perc_SN_flag=50,
                  env_info='no', region='circle', server=None, limtvel=500,
                  xtpos=10, ytpos=20, deltay=10, miny = 20, simbadima='no',
                  field_size_phy=99,
                  sizet=20, run_auto='no', show_plot='yes',  plot_model='yes',
-                 outputfile='properties.dat'):
+                 outputfile='properties.dat', search_cone=2/3600.):
     """
     Perform photometric modeling on galaxy images by using SPLU-data
 
     Parameters:
     ------------
-    - gal: Galaxy name (str type).
+    - gal: Galaxy name (str type) or an array [ra, dec] deg.
     - tab_gal: Input table (pandas DataFrame or equivalent) or "simbad" to
                download the galaxy data from Simbad database.
     - size_image_phy: Physical size of the image in kpc unit (default: 50).
     - band: Band for photometry (default: 'R').
+    - search_cone: region size of query region to get the psf value
+                   in arcsec (default: 2/3600).
     - snr: Signal-to-noise ratio threshold to detect sources (default: 2.0).
     - area_min: Minimum area for object detection in kpc unit (default: 10).
     - deblend: Deblending option ('off' or 'on', default: 'off').
     - area_min_deblend: Minimum detection area for deblending in kpc unit
                        (default: 20).
     - sky_box: Sky box size for background estimation in pix unit
                (default: [100, 100]).
@@ -2554,96 +2551,52 @@
     ```
     """
 
     ######################
     # Loading the galaxy #
     ######################
 
-    print (Fore.BLUE +"\nBasic information:")
-    print (Fore.BLUE +"-------------------")
     if isinstance(tab_gal, str):
-        simbad_table = simbad.Simbad.query_object(gal)
-        if bool(simbad_table) is False:
-            print ("\nthe target was not found, please double-checking" +
-                    "the target name")
-            return
-
-        galvel = simbad_table['RV_VALUE'].value[0]
-
-        print(Fore.BLUE +'Galaxy Name: {} '.format(gal))
-        print(Fore.BLUE +'MAIN_ID: {} '.format(simbad_table['MAIN_ID'].value[0]))
-        print(Fore.BLUE +'mag_B: {:.2f} '.format(simbad_table['FLUX_B'].value[0]))
-
-        if not os.path.exists('simbad_table.tab'):
-            simbad_table['MAIN_ID'] = gal
-            tab_gal = Table((simbad_table['MAIN_ID'],
-                             simbad_table['RA_d'], simbad_table['DEC_d'],
-                             simbad_table['RV_VALUE'], simbad_table['Z_VALUE'],
-                             simbad_table['FLUX_B']),
-                             names=('gal','ra','dec','vel','z', 'mag'))
-            tab_gal.write('simbad_table.tab', format='ascii')
-            idg=0
+        if tab_gal == 'simbad':
+            gal, tab_gal, idg = simbad_gal (gal, search_cone=search_cone)
         else:
-            tab_gal = Table.read('simbad_table.tab', format='ascii')
-            if any(tab_gal['gal'] == gal):
-                idg=np.where(tab_gal['gal']==gal)[0][0]
-            else:
-                tab_gal.add_row()
-                idg = -1
-                tab_gal['gal'][idg] =  simbad_table['MAIN_ID']
-                tab_gal['ra'][idg] =  simbad_table['RA_d']
-                tab_gal['dec'][idg] =  simbad_table['DEC_d']
-                tab_gal['vel'][idg] =  simbad_table['RV_VALUE']
-                tab_gal['z'][idg] =  simbad_table['Z_VALUE']
-                tab_gal['mag'][idg] =  simbad_table['FLUX_B']
-                tab_gal.write('simbad_table.tab', format='ascii', overwrite=True)
-
+            gal, tab_gal, idg = ned_gal (gal, search_cone=search_cone)
     else:
-        print(Fore.BLUE +'Galaxy Name: {} '.format(gal))
         idg =np.where(tab_gal['gal']==gal)[0][0]
-        galvel = tab_gal['vel'][idg]
-
-        print(Fore.BLUE +'Galaxy Name: {} '.format(gal))
 
-        try:
-            print(Fore.BLUE +'Z: {} '.format(tab_gal['z'][idg]))
-        except:
-            galZ = galvel/3e5
-            tab_gal.add_column(np.zeros((len(tab_gal)))*np.nan,name='z')
-            tab_gal['z'][idg] = galZ
 
-    idg =np.where(tab_gal['gal']==gal)[0][0]
-    D = tab_gal['vel'][idg]/H
+    galvel = tab_gal['vel'][idg]
+    D = galvel/H
     arc_kpc = np.tan(np.deg2rad(1./3600.))*D*1e3
+    sc_imag = 0.55
 
+    size_image=((size_image_phy/arc_kpc)/sc_imag)*2
+    size_image_kpc = int(size_image)*0.5*sc_imag*arc_kpc
+    area_min_pix = area_min/arc_kpc**2/sc_imag**2
+    area_min_deblend_pix = area_min_deblend/arc_kpc**2/sc_imag**2
+
+    print (Fore.BLUE +"\nBasic information:")
+    print (Fore.BLUE +"-------------------")
     try:
         direcbase = os.path.dirname(os.path.realpath(__file__))
         AM = Table.read(direcbase + '/Table_Arp_Madore_pairs_updated.txt',
                         format='ascii')
         id_am + np.where(AM['gal']==gal)[0]
         print (Fore.RED +"\nThis is galaxy is in Arp & Maodore Catalog:")
         print ("------------------------")
         print(AM['cat','cross_ID'][id_am])
         print(AM['desc','codes'][id_am])
     except:
         pass
-
-    sc_imag = 0.55
-
     print(Fore.BLUE +'RA  = {} '.format(tab_gal['ra'][idg]))
     print(Fore.BLUE +'DEC = {} '.format(tab_gal['dec'][idg]))
     print(Fore.BLUE +'Rad Vel = {:.1f} km/s'.format(galvel))
     print(Fore.BLUE +'Distance = {:.1f}  Mpc'.format(D))
     print(Fore.BLUE +'arc_kpc = {:.4f}'.format(arc_kpc))
-    size_image=((size_image_phy/arc_kpc)/sc_imag)*2
-    size_image_kpc = int(size_image)*0.5*sc_imag*arc_kpc
     print (Fore.BLUE +'image size in pix = {:.1f}'.format(size_image))
-    #area_min=(((np.square(areagal)*np.pi)/arc_kpc**2)/sc_imag**2)
-    area_min_pix = area_min/arc_kpc**2/sc_imag**2
-    area_min_deblend_pix = area_min_deblend/arc_kpc**2/sc_imag**2
     print (Fore.BLUE +'Minimum detection area {:.1f} kcp^2 = {:.0f} pix'.format(area_min,
            area_min_pix))
     textp = 'Minimum deblending detection area '
     print (Fore.BLUE+textp+'{:.1f} kcp^2 = {:.0f} pix'.format(area_min_deblend,
                    int(area_min_deblend_pix)))
 
     ###############################
@@ -3050,15 +3003,15 @@
                         sizet=20,
                         outputfile='properties.dat', dr=10, search_cone=2/3600.):
     """
         Perform photometric modeling on galaxy images by using Legacy-data
 
         Parameters:
         ------------
-        - gal: Galaxy name (str type).
+        - gal: Galaxy name (str type) or an array [ra, dec] deg.
         - tab_gal: input table (pandas DataFrame or equivalent) or "simbad" to
                    download the galaxy data from Simbad database
                    (default: 'simbad').
         - size_image_phy: Physical size of the image in kpc unit (default: 50).
         - band: Band for photometry (default: 'r').
         - dr: Data release of legacy survey (default: 10).
         - search_cone: region size of query region to get the psf value
@@ -3129,100 +3082,66 @@
         ```
     """
 
     ######################
     # Loading the galaxy #
     ######################
 
-    print (Fore.BLUE +"\nBasic information:")
-    print (Fore.BLUE +"-------------------")
     if isinstance(tab_gal, str):
-        simbad_table = simbad.Simbad.query_object(gal)
-        if bool(simbad_table) is False:
-            print ("\nthe target was not found, please double-checking" +
-                    "the target name")
-            return
-
-        galvel = simbad_table['RV_VALUE'].value[0]
-
-        print(Fore.BLUE +'Galaxy Name: {} '.format(gal))
-        print(Fore.BLUE +'MAIN_ID: {} '.format(simbad_table['MAIN_ID'].value[0]))
-        print(Fore.BLUE +'mag_B: {:.2f} '.format(simbad_table['FLUX_B'].value[0]))
-
-        if not os.path.exists('simbad_table.tab'):
-            simbad_table['MAIN_ID'] = gal
-            tab_gal = Table((simbad_table['MAIN_ID'],
-                             simbad_table['RA_d'], simbad_table['DEC_d'],
-                             simbad_table['RV_VALUE'], simbad_table['Z_VALUE'],
-                             simbad_table['FLUX_B']),
-                             names=('gal','ra','dec','vel','z', 'mag'))
-            tab_gal.write('simbad_table.tab', format='ascii')
-            idg=0
+        if tab_gal == 'simbad':
+            gal, tab_gal, idg = simbad_gal (gal, search_cone=search_cone)
         else:
-            tab_gal = Table.read('simbad_table.tab', format='ascii')
-            if any(tab_gal['gal'] == gal):
-                idg=np.where(tab_gal['gal']==gal)[0][0]
-            else:
-                tab_gal.add_row()
-                idg = -1
-                tab_gal['gal'][idg] =  simbad_table['MAIN_ID']
-                tab_gal['ra'][idg] =  simbad_table['RA_d']
-                tab_gal['dec'][idg] =  simbad_table['DEC_d']
-                tab_gal['vel'][idg] =  simbad_table['RV_VALUE']
-                tab_gal['z'][idg] =  simbad_table['Z_VALUE']
-                tab_gal['mag'][idg] =  simbad_table['FLUX_B']
-                tab_gal.write('simbad_table.tab', format='ascii', overwrite=True)
-
+            gal, tab_gal, idg = ned_gal (gal, search_cone=search_cone)
     else:
         idg =np.where(tab_gal['gal']==gal)[0][0]
-        galvel = tab_gal['vel'][idg]
-
-        print(Fore.BLUE +'Galaxy Name: {} '.format(gal))
-
-        try:
-            print(Fore.BLUE +'Z: {} '.format(tab_gal['z'][idg]))
-        except:
-            galZ = galvel/3e5
-            tab_gal.add_column(np.zeros((len(tab_gal)))*np.nan,name='z')
-            tab_gal['z'][idg] = galZ
 
+    galvel = tab_gal['vel'][idg]
     D = galvel/H
     arc_kpc = np.tan(np.deg2rad(1./3600.))*D*1e3
     sc_ima = 0.27
 
+    size_image=((size_image_phy/arc_kpc)/sc_ima)*2
+    size_image_kpc = int(size_image)*sc_ima*arc_kpc
+    area_min_pix = area_min/arc_kpc**2/sc_ima**2
+    area_min_deblend_pix=area_min_deblend/arc_kpc**2/sc_ima**2
+
+    print (Fore.BLUE +"\nBasic information:")
+    print (Fore.BLUE +"-------------------")
+    print(Fore.BLUE +'Galaxy Name: {} '.format(gal))
+    try:
+        print(Fore.BLUE +'Z: {} '.format(tab_gal['z'][idg]))
+    except:
+        galZ = galvel/3e5
+        tab_gal.add_column(np.zeros((len(tab_gal)))*np.nan,name='z')
+        tab_gal['z'][idg] = galZ
     try:
         print(Fore.RED +'Jclass {} '.format(tab_gal['Jclass'][idg]))
     except:
         pass
     print(Fore.BLUE +'RA  = {} '.format(tab_gal['ra'][idg]))
     print(Fore.BLUE +'DEC = {} '.format(tab_gal['dec'][idg]))
     print(Fore.BLUE +'Rad Vel = {:.1f} km/s'.format(galvel))
     print(Fore.BLUE +'Distance = {:.1f} Mpc'.format(D))
     print(Fore.BLUE +'arc_kpc = {:.4f}'.format(arc_kpc))
-    size_image=((size_image_phy/arc_kpc)/sc_ima)*2
-    size_image_kpc = int(size_image)*sc_ima*arc_kpc
     print (Fore.BLUE +'image size in pix: {:.1f}'.format(size_image))
-    area_min_pix = area_min/arc_kpc**2/sc_ima**2
-    area_min_deblend_pix=area_min_deblend/arc_kpc**2/sc_ima**2
     print (Fore.BLUE +'Minimum detection area in the Field' +
            '{:.1f} kcp^2 = {:.0f} pix'.format(area_min, int(area_min_pix)))
     textp = 'Minimum deblending detection area '
     print (Fore.BLUE+textp+'{:.1f} kcp^2 = {:.0f} pix'.format(area_min_deblend,
                int(area_min_deblend_pix)))
 
-
     if not os.path.exists('fits_images'):
         os.system('mkdir fits_images')
         print (Fore.RED+ '\nThe folder fits_images was created')
 
     if not os.path.exists('images'):
         os.system('mkdir images')
         print (Fore.RED+ '\nThe folder images was created')
 
-    print(Fore.BLACK +'\n\nLoading/Downloading the images and tables')
+    print(Fore.BLACK +'\n\nLoading/Downloading the images')
     print('---------------------------------------------')
 
     home = 'https://www.legacysurvey.org/viewer/fits-cutout?'
     path = 'fits_images/{}_{}_{}kpc.fits'.format(gal, band, size_image_phy)
     if not os.path.exists(path):
         print (f"\nDowloading {path} ...")
         part0 = 'ra={}&dec={}&layer={}&pixscale=0.27&bands={}&size={}'.format(
@@ -3484,15 +3403,15 @@
                         sizet=20, width = 300, height = 300,
                         outputfile='properties.dat', search_cone=2/3600.):
     """
         Perform photometric modeling on galaxy images by using Legacy-data
 
         Parameters:
         ------------
-        - gal: Galaxy name (str type)  or array [ra, dec] deg.
+        - gal: Galaxy name (str type)  or  an array [ra, dec] deg.
         - tab_gal: input table (pandas DataFrame or equivalent) or "simbad/ned" to
                    download the galaxy data from Simbad/Ned database
                    (default: 'simbad').
         - size_image_phy: Physical size of the image in kpc unit (default: 50).
         - band: Band for photometry (default: 'r').
         - search_cone: region size of query region to get the psf value
                        in arcsec (default: 2/3600).
```

### Comparing `astromorphlib-1.0.0/stat_lib/__init__old.py` & `astromorphlib-1.0.1/stat_lib/__init__old.py`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/stat_lib/__pycache__/__init__.cpython-38.pyc` & `astromorphlib-1.0.1/stat_lib/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/stat_lib/__pycache__/stat_lib.cpython-38.pyc` & `astromorphlib-1.0.1/stat_lib/__pycache__/stat_lib.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/stat_lib/iDR4_obs_seeing.csv` & `astromorphlib-1.0.1/stat_lib/iDR4_obs_seeing.csv`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/stat_lib/iDR4_zero-points.csv` & `astromorphlib-1.0.1/stat_lib/iDR4_zero-points.csv`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/stat_lib/properties.dat` & `astromorphlib-1.0.1/stat_lib/properties.dat`

 * *Files identical despite different names*

### Comparing `astromorphlib-1.0.0/stat_lib/zero_points.fits` & `astromorphlib-1.0.1/stat_lib/zero_points.fits`

 * *Files identical despite different names*

